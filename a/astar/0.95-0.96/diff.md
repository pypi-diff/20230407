# Comparing `tmp/astar-0.95-py3-none-any.whl.zip` & `tmp/astar-0.96-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 6094 bytes, number of entries: 5
--rw-r--r--  2.0 unx     5212 b- defN 80-Jan-01 00:00 astar/__init__.py
--rw-r--r--  2.0 unx     1496 b- defN 80-Jan-01 00:00 astar-0.95.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 astar-0.95.dist-info/WHEEL
-?rw-r--r--  2.0 unx     8526 b- defN 16-Jan-01 00:00 astar-0.95.dist-info/METADATA
-?rw-r--r--  2.0 unx      356 b- defN 16-Jan-01 00:00 astar-0.95.dist-info/RECORD
-5 files, 15678 bytes uncompressed, 5438 bytes compressed:  65.3%
+Zip file size: 7022 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     8784 b- defN 80-Jan-01 00:00 astar/__init__.py
+-rw-r--r--  2.0 unx     1496 b- defN 80-Jan-01 00:00 astar-0.96.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8619 b- defN 80-Jan-01 00:00 astar-0.96.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 astar-0.96.dist-info/WHEEL
+?rw-r--r--  2.0 unx      356 b- defN 16-Jan-01 00:00 astar-0.96.dist-info/RECORD
+5 files, 19343 bytes uncompressed, 6366 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: astar/__init__.py
 Comment: 
 
-Filename: astar-0.95.dist-info/LICENSE
+Filename: astar-0.96.dist-info/LICENSE
 Comment: 
 
-Filename: astar-0.95.dist-info/WHEEL
+Filename: astar-0.96.dist-info/METADATA
 Comment: 
 
-Filename: astar-0.95.dist-info/METADATA
+Filename: astar-0.96.dist-info/WHEEL
 Comment: 
 
-Filename: astar-0.95.dist-info/RECORD
+Filename: astar-0.96.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## astar/__init__.py

```diff
@@ -1,47 +1,145 @@
 # -*- coding: utf-8 -*-
 """ generic A-Star path searching algorithm """
 
+import logging
 from abc import ABC, abstractmethod
-from heapq import heappush, heappop
-from typing import Iterable, Union, TypeVar, Generic
-
-# infinity as a constant
-Infinite = float("inf")
+from heapq import heapify, heappush, heappop
+from typing import Type, Callable, Dict, Iterable, Union, TypeVar, Generic
+from math import inf as infinity
 
 # introduce generic type
 T = TypeVar("T")
 
-class AStar(ABC, Generic[T]):
 
-    __slots__ = ()
+################################################################################
+class SearchNode(Generic[T]):
+    """Representation of a search node"""
+
+    __slots__ = ("data", "gscore", "fscore", "closed", "came_from", "in_openset")
+
+    def __init__(
+        self, data: T, gscore: float = infinity, fscore: float = infinity
+    ) -> None:
+        self.data = data
+        self.gscore = gscore
+        self.fscore = fscore
+        self.closed = False
+        self.in_openset = False
+        self.came_from: Union[None, SearchNode[T]] = None
+
+    def __lt__(self, b: "SearchNode[T]") -> bool:
+        """Natural order is based on the fscore value & is used by heapq operations"""
+        return self.fscore < b.fscore
+
+
+################################################################################
+class SearchNodeDict(Dict[T, SearchNode[T]]):
+    """A dict that returns a new SearchNode when a key is missing"""
+
+    def __missing__(self, k) -> SearchNode[T]:
+        v = SearchNode(k)
+        self.__setitem__(k, v)
+        return v
+
+
+################################################################################
+SNType = TypeVar("SNType", bound=SearchNode)
+
+
+class OpenSet(ABC, Generic[SNType]):
+    """As we may have performance issues with the heapq module when an item is
+    re-inserted, we may use other implementations for this feature.
+
+     - By default the HeapQOpenSet class just relies on the heapq module, it does not need any external dependency.
+
+     - The SortedContainersOpenSet class uses the sortedcointainers module. As
+       this module is optional, it will be used only if your own project
+       depends on it.
 
-    class SearchNode:
-        """Representation of a search node"""
+    """
 
-        __slots__ = ("data", "gscore", "fscore", "closed", "came_from", "out_openset")
+    @abstractmethod
+    def push(self, item: SNType) -> None:
+        """Add an item to the queue"""
+        raise NotImplementedError
 
-        def __init__(
-            self, data: T, gscore: float = Infinite, fscore: float = Infinite
-        ) -> None:
-            self.data = data
-            self.gscore = gscore
-            self.fscore = fscore
-            self.closed = False
-            self.out_openset = True
-            self.came_from = None
-
-        def __lt__(self, b: "AStar.SearchNode") -> bool:
-            return self.fscore < b.fscore
-
-    class SearchNodeDict(dict):
-        def __missing__(self, k):
-            v = AStar.SearchNode(k)
-            self.__setitem__(k, v)
-            return v
+    @abstractmethod
+    def pop(self) -> SNType:
+        """Remove and return the smallest item from the queue"""
+        raise NotImplementedError
+
+    @abstractmethod
+    def remove(self, item: SNType) -> None:
+        """remove an item from the queue, ensuring that the queue is still valid afterwards"""
+        raise NotImplementedError
+
+
+################################################################################
+class HeapQOpenSet(OpenSet[SNType], Generic[SNType]):
+    """just a wrapper around heapq operations"""
+
+    def __init__(self):
+        self.heap = []
+        heapify(self.heap)
+
+    def push(self, item: SNType) -> None:
+        """Add an item to the queue"""
+        item.in_openset = True
+        heappush(self.heap, item)
+
+    def pop(self) -> SNType:
+        """Remove and return the smallest item from the queue"""
+        item = heappop(self.heap)
+        item.in_openset = False
+        return item
+
+    def remove(self, item: SNType):
+        self.heap.remove(item)
+        heapify(
+            self.heap
+        )  # costly operation but necessary as remove operation destroy the structure of the heap
+        item.in_openset = False
+
+
+################################################################################
+OpenSetImpl: Type[OpenSet] = HeapQOpenSet
+
+try:
+    import sortedcontainers
+
+    class SortedContainersOpenSet(OpenSet[SNType], Generic[SNType]):
+        def __init__(self):
+            self.sortedlist = sortedcontainers.SortedList(key=lambda x: x.fscore)
+
+        def push(self, item: SNType) -> None:
+            item.in_openset = True
+            self.sortedlist.add(item)
+
+        def pop(self) -> SNType:
+            item = self.sortedlist.pop(0)
+            item.in_openset = False
+            return item
+
+        def remove(self, item: SNType):
+            self.sortedlist.remove(item)
+            item.in_openset = False
+
+    OpenSetImpl = SortedContainersOpenSet
+    logging.info("using sortedcontainers for heap operations")
+
+except Exception as e:
+    logging.info("sortedcontainers module not loaded, using the default heapq module")
+
+
+################################################################################*
+
+
+class AStar(ABC, Generic[T]):
+    __slots__ = ()
 
     @abstractmethod
     def heuristic_cost_estimate(self, current: T, goal: T) -> float:
         """
         Computes the estimated (rough) distance between a node and the goal.
         The second parameter is always the goal.
         This method must be implemented in a subclass.
@@ -86,70 +184,84 @@
             return reversed(list(_gen()))
 
     def astar(
         self, start: T, goal: T, reversePath: bool = False
     ) -> Union[Iterable[T], None]:
         if self.is_goal_reached(start, goal):
             return [start]
-        searchNodes = AStar.SearchNodeDict()
-        startNode = searchNodes[start] = AStar.SearchNode(
+
+        openSet: OpenSet[SearchNode[T]] = OpenSetImpl()
+        searchNodes: SearchNodeDict[T] = SearchNodeDict()
+        startNode = searchNodes[start] = SearchNode(
             start, gscore=0.0, fscore=self.heuristic_cost_estimate(start, goal)
         )
-        openSet: list = []
-        heappush(openSet, startNode)
+        openSet.push(startNode)
+
         while openSet:
-            current = heappop(openSet)
+            current = openSet.pop()
+
             if self.is_goal_reached(current.data, goal):
                 return self.reconstruct_path(current, reversePath)
-            current.out_openset = True
+
             current.closed = True
+
             for neighbor in map(lambda n: searchNodes[n], self.neighbors(current.data)):
                 if neighbor.closed:
                     continue
+
                 tentative_gscore = current.gscore + self.distance_between(
                     current.data, neighbor.data
                 )
+
                 if tentative_gscore >= neighbor.gscore:
                     continue
+
+                neighbor_from_openset = neighbor.in_openset
+
+                if neighbor_from_openset:
+                    # we have to remove the item from the heap, as its score has changed
+                    openSet.remove(neighbor)
+
+                # update the node
                 neighbor.came_from = current
                 neighbor.gscore = tentative_gscore
                 neighbor.fscore = tentative_gscore + self.heuristic_cost_estimate(
                     neighbor.data, goal
                 )
-                if neighbor.out_openset:
-                    neighbor.out_openset = False
-                    heappush(openSet, neighbor)
-                else:
-                    # re-add the node in order to re-sort the heap
-                    openSet.remove(neighbor)
-                    heappush(openSet, neighbor)
+
+                openSet.push(neighbor)
+
         return None
 
 
+################################################################################
+U = TypeVar("U")
+
+
 def find_path(
-    start: T,
-    goal: T,
-    neighbors_fnct,
+    start: U,
+    goal: U,
+    neighbors_fnct: Callable[[U], Iterable[U]],
     reversePath=False,
-    heuristic_cost_estimate_fnct=lambda a, b: Infinite,
-    distance_between_fnct=lambda a, b: 1.0,
-    is_goal_reached_fnct=lambda a, b: a == b,
-) -> Union[Iterable[T], None]:
+    heuristic_cost_estimate_fnct: Callable[[U, U], float] = lambda a, b: infinity,
+    distance_between_fnct: Callable[[U, U], float] = lambda a, b: 1.0,
+    is_goal_reached_fnct: Callable[[U, U], bool] = lambda a, b: a == b,
+) -> Union[Iterable[U], None]:
     """A non-class version of the path finding algorithm"""
 
     class FindPath(AStar):
-        def heuristic_cost_estimate(self, current, goal):
-            return heuristic_cost_estimate_fnct(current, goal)
+        def heuristic_cost_estimate(self, current: U, goal: U) -> float:
+            return heuristic_cost_estimate_fnct(current, goal)  # type: ignore
 
-        def distance_between(self, n1, n2):
+        def distance_between(self, n1: U, n2: U) -> float:
             return distance_between_fnct(n1, n2)
 
-        def neighbors(self, node):
-            return neighbors_fnct(node)
+        def neighbors(self, node) -> Iterable[U]:
+            return neighbors_fnct(node)  # type: ignore
 
-        def is_goal_reached(self, current, goal):
-            return is_goal_reached_fnct(current, goal)
+        def is_goal_reached(self, current, goal) -> bool:
+            return is_goal_reached_fnct(current, goal)  # type: ignore
 
     return FindPath().astar(start, goal, reversePath)
 
 
 __all__ = ["AStar", "find_path"]
```

## Comparing `astar-0.95.dist-info/LICENSE` & `astar-0.96.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `astar-0.95.dist-info/METADATA` & `astar-0.96.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: astar
-Version: 0.95
+Version: 0.96
 Summary: generic A-Star path searching algorithm
 Home-page: https://github.com/jrialland/python-astar
 License: BSD
 Author: J Rialland
 Author-email: julien.rialland@gmail.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: sortedcontainers (>=2.4.0)
 Project-URL: Repository, https://github.com/jrialland/python-astar
 Description-Content-Type: text/x-rst
 
 .. image:: https://badge.fury.io/py/astar.svg
     :target: https://badge.fury.io/py/astar
 
 .. image:: https://app.travis-ci.com/jrialland/python-astar.svg?branch=master
```

