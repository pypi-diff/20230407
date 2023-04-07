# Comparing `tmp/aligned_textgrid-0.2.1.tar.gz` & `tmp/aligned_textgrid-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligned_textgrid-0.2.1.tar", max compression
+gzip compressed data, was "aligned_textgrid-0.3.0.tar", max compression
```

## Comparing `aligned_textgrid-0.2.1.tar` & `aligned_textgrid-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-02-14 13:52:58.923117 aligned_textgrid-0.2.1/LICENSE
--rw-r--r--   0        0        0     6487 2023-03-16 20:38:52.636165 aligned_textgrid-0.2.1/README.md
--rw-r--r--   0        0        0     1202 2023-03-16 20:39:11.040183 aligned_textgrid-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-16 20:38:52.650751 aligned_textgrid-0.2.1/src/aligned_textgrid/__init__.py
--rw-r--r--   0        0        0     7514 2023-03-16 20:38:52.651068 aligned_textgrid-0.2.1/src/aligned_textgrid/aligned_textgrid.py
--rw-r--r--   0        0        0     3421 2023-03-16 20:38:52.651165 aligned_textgrid-0.2.1/src/aligned_textgrid/custom_classes.py
--rw-r--r--   0        0        0        0 2023-03-16 20:38:52.651210 aligned_textgrid-0.2.1/src/aligned_textgrid/sequences/__init__.py
--rw-r--r--   0        0        0    21266 2023-03-16 20:38:52.651548 aligned_textgrid-0.2.1/src/aligned_textgrid/sequences/sequences.py
--rw-r--r--   0        0        0    11247 2023-03-16 20:38:52.651962 aligned_textgrid-0.2.1/src/aligned_textgrid/sequences/tiers.py
--rw-r--r--   0        0        0     2191 2023-03-16 20:38:52.652306 aligned_textgrid-0.2.1/src/aligned_textgrid/sequences/word_and_phone.py
--rw-r--r--   0        0        0     7380 1970-01-01 00:00:00.000000 aligned_textgrid-0.2.1/setup.py
--rw-r--r--   0        0        0     7237 1970-01-01 00:00:00.000000 aligned_textgrid-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-14 13:52:58.923117 aligned_textgrid-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6584 2023-04-07 21:27:15.257112 aligned_textgrid-0.3.0/README.md
+-rw-r--r--   0        0        0     1202 2023-04-07 21:41:29.839214 aligned_textgrid-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      476 2023-04-07 21:27:15.258965 aligned_textgrid-0.3.0/src/aligned_textgrid/__init__.py
+-rw-r--r--   0        0        0     9712 2023-04-07 21:27:15.259154 aligned_textgrid-0.3.0/src/aligned_textgrid/aligned_textgrid.py
+-rw-r--r--   0        0        0     4178 2023-04-07 21:27:15.259321 aligned_textgrid-0.3.0/src/aligned_textgrid/custom_classes.py
+-rw-r--r--   0        0        0        0 2023-04-07 19:43:50.937280 aligned_textgrid-0.3.0/src/aligned_textgrid/sequences/__init__.py
+-rw-r--r--   0        0        0    21404 2023-04-07 21:27:15.259562 aligned_textgrid-0.3.0/src/aligned_textgrid/sequences/sequences.py
+-rw-r--r--   0        0        0    11896 2023-04-07 21:27:15.259791 aligned_textgrid-0.3.0/src/aligned_textgrid/sequences/tiers.py
+-rw-r--r--   0        0        0     2342 2023-04-07 21:27:15.259958 aligned_textgrid-0.3.0/src/aligned_textgrid/sequences/word_and_phone.py
+-rw-r--r--   0        0        0     7480 1970-01-01 00:00:00.000000 aligned_textgrid-0.3.0/setup.py
+-rw-r--r--   0        0        0     7334 1970-01-01 00:00:00.000000 aligned_textgrid-0.3.0/PKG-INFO
```

### Comparing `aligned_textgrid-0.2.1/LICENSE` & `aligned_textgrid-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.2.1/README.md` & `aligned_textgrid-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 ![PyPI](https://img.shields.io/pypi/v/aligned-textgrid)
 ![lint_and_test](https://github.com/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/actions/workflows/test_and_run.yml/badge.svg?event=pull_request&branch=main)
 [![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/branch/dev/graph/badge.svg?token=27YSOQ5ZEL)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid)
 [![Maintainability](https://api.codeclimate.com/v1/badges/2387cd247bd8f1211323/maintainability)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/maintainability)
 [![Documentation Status](https://readthedocs.org/projects/alignedtextgrid/badge/?version=latest)](https://alignedtextgrid.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/552633207.svg)](https://zenodo.org/badge/latestdoi/552633207)
+
 
 # aligned_textgrid
 
 The aligned-textgrid package provides a python interface for representing and operating on TextGrids produced by forced aligners like [FAVE](https://github.com/JoFrhwld/FAVE) or the [Montreal Forced Aligner](https://montreal-forced-aligner.readthedocs.io/en/latest/). Classes provided by aligned-textgrid represent hierarchical and precedence relationships among data stored in TextGrid formats allowing for simplified and more accessible analysis of aligned speech data.
 
 ## Installation
 To install aligned-textgrid using pip, run the following command in your terminal:
@@ -59,8 +61,8 @@
 ```{python}
 from random import randint
 num_words = len(tg[wordTier])
 
 word = tg[wordTier][randint(0,num_words)]
 ```
 
-The aligned-textgrid package aims to resolve these issues by incorporating these relationships into the representations from the start. The attribute `.fol` of `aligned_textgrid.sequences.sequences.SequenceInterval` provides access to the next interval in the sequence even if you don't know precisely where in the sequence you are. You can also use the `.intier` and `.subset_list` attributes to navigate up and down the tier hierarchy.
+The aligned-textgrid package aims to resolve these issues by incorporating these relationships into the representations from the start. The attribute `.fol` of `aligned_textgrid.sequences.sequences.SequenceInterval` provides access to the next interval in the sequence even if you don't know precisely where in the sequence you are. You can also use the `.intier` and `.subset_list` attributes to navigate up and down the tier hierarchy.
```

### Comparing `aligned_textgrid-0.2.1/pyproject.toml` & `aligned_textgrid-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aligned_textgrid"
-version = "0.2.1"
+version = "0.3.0"
 description = "Classes for defining sequential information from TextGrids"
 authors = ["JoFrhwld <JoFrhwld@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "aligned_textgrid", from="src"}]
 exclude = [
     "notebooks/",
```

### Comparing `aligned_textgrid-0.2.1/src/aligned_textgrid/aligned_textgrid.py` & `aligned_textgrid-0.3.0/src/aligned_textgrid/aligned_textgrid.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,21 +51,21 @@
         entry_classes: 
             Sequence[Sequence[Type[SequenceInterval]]] |
             Sequence[Type[SequenceInterval]]
               = [SequenceInterval]
     ):
         self.entry_classes = entry_classes
         if textgrid:
-            self.tg_tiers = self._nestify_tiers(textgrid)
+            self.tg_tiers, self.entry_classes = self._nestify_tiers(textgrid, entry_classes)
         elif textgrid_path:
             tg = openTextgrid(
                 fnFullPath=textgrid_path, 
                 includeEmptyIntervals=True
             )
-            self.tg_tiers = self._nestify_tiers(tg)
+            self.tg_tiers, self.entry_classes = self._nestify_tiers(tg, entry_classes)
 
         self.tier_groups = self._relate_tiers()
         self.entry_classes = [[tier.entry_class for tier in tg] for tg in self.tier_groups]
 
     
     def __contains__(self, item):
         return item in self.tier_groups
@@ -99,57 +99,125 @@
         raise StopIteration
     
     def __repr__(self):
         n_groups = len(self.tier_groups)
         n_tiers = [len(x) for x in self.tier_groups]
         entry_classes = [[x.__name__ for x in y] for y in self.entry_classes]
         return f"AlignedTextGrid with {n_groups} groups, each with {repr(n_tiers)} tiers. {repr(entry_classes)}"
+    
+    def _extend_classes(
+            self, 
+            tg: Textgrid, 
+            entry_classes
+        ):
+        """_summary_
+
+        Args:
+            tg (_type_): _description_
+            entry_classes (_type_): _description_
+        """
+
+        ntiers = len(tg.tiers)
+        if not type(entry_classes[0]) in [list, tuple]:
+            class_supers = [c.superset_class for c in entry_classes]
+            try:
+                top_idxes = [i for i,c in enumerate(class_supers) if issubclass(c, Top)]
+            except ValueError:
+                top_idxes = []
+
+        if type(entry_classes[0]) in [list, tuple]:
+            return entry_classes
+        if len(entry_classes) == 1:
+            extension = len(tg.tiers) // len(entry_classes)
+            entry_classes = [entry_classes] * extension
+            return entry_classes
+        if len(top_idxes) <= 1:
+            extension = len(tg.tiers) // len(entry_classes)
+            entry_classes = [entry_classes] * extension
+            return entry_classes
+        return entry_classes
 
     def _nestify_tiers(
         self,
-        textgrid: Textgrid
+        textgrid: Textgrid,
+        entry_classes: list[SequenceInterval]
     ):
         """_private method to nestify tiers_
 
         Takes a flat list of tiers and nests them according to 
         the nesting, or implied nesting, of `self.entry_classes`
 
         Args:
             textgrid (Textgrid): _description_
+            entry_classes (list[SequenceInterval]): _description_
 
         Returns:
             (list[IntervalTier]): _description_
-        """
-        tier_idx = 0
+        """ 
+
         tier_list = []
-       
-        if not type(self.entry_classes[0]) in [tuple, list]:
-            extension = len(textgrid.tiers) // len(self.entry_classes)
-            self.entry_classes = [self.entry_classes] * extension
-        elif len(self.entry_classes) == 1:
-            extension = len(textgrid.tiers) // len(self.entry_classes[0])
-            self.entry_classes = [self.entry_classes[0]] * extension
-
-        for idx, class_tup in enumerate(self.entry_classes):
-            tier_list.append([])
-            for jdx, classes in enumerate(class_tup):
-                tier_list[idx].append(textgrid.tiers[tier_idx])
-                tier_idx += 1
-        return tier_list
+
+        entry_classes = self._extend_classes(textgrid, entry_classes)
+        if type(entry_classes[0]) in [list, tuple]:
+            tier_idx = 0
+            for idx, class_tup in enumerate(entry_classes):
+                tier_list.append([])
+                for jdx, classes in enumerate(class_tup):
+                    tier_list[idx].append(textgrid.tiers[tier_idx])
+                    tier_idx += 1
+            return tier_list, entry_classes
+        
+        super_classes = [c.superset_class for c in entry_classes]
+        top_idxes = [i for i,c in enumerate(super_classes) if issubclass(c, Top)]
+
+        if len(top_idxes) <= 1:
+            return [textgrid.tiers], [entry_classes]
+        
+        ## Nestifying hierarchywise
+        entry_list = []
+        for top_idx in top_idxes:
+            this_tierlist = []
+            this_entrylist = []
+
+            this_tierlist.append(textgrid.tiers[top_idx])
+            this_entrylist.append(entry_classes[top_idx])
+
+            done = False
+            while not done:
+                curr = this_entrylist[-1]
+                if issubclass(curr.subset_class, Bottom):
+                    done = True
+                    break
+
+                try:
+                    next_idx = entry_classes.index(curr.subset_class)
+                except ValueError:
+                    done = True
+                    break
+
+                this_tierlist.append(textgrid.tiers[next_idx])
+                this_entrylist.append(entry_classes[next_idx])
+
+            tier_list.append(this_tierlist)
+            entry_list.append(this_entrylist)
+        
+        return tier_list, entry_list
 
     def _relate_tiers(self):
         """_Private method_
 
         creates RelatedTier objects for each set of
         nested IntervalTier and entry class
 
         Returns:
             (list[TierGroup]): _description_
         """
+
         tier_groups = []
+
         for tier_group, classes in zip(self.tg_tiers, self.entry_classes):
             tier_list = []
             for tier, entry_class in zip(tier_group, classes):
                 tier_list.append(SequenceTier(tier, entry_class))
             tier_groups.append(TierGroup(tier_list))
         return tier_groups
```

### Comparing `aligned_textgrid-0.2.1/src/aligned_textgrid/custom_classes.py` & `aligned_textgrid-0.3.0/src/aligned_textgrid/custom_classes.py`

 * *Files 17% similar despite different names*

```diff
@@ -62,30 +62,63 @@
     """
     def _constructor(
             self, 
             Interval = Interval(None, None, None)
         ):
         SequenceInterval.__init__(self, Interval=Interval)
 
+    def _top_constructor(self):
+        Top.__init__(self)
+
+    def _bottom_constructor(self):
+        Bottom.__init__(self)
+
+
+    n_top = len(Top.__subclasses__())
+    n_bottom = len(Bottom.__subclasses__())
+
+    this_top_name = f"Top_{n_top}"
+    this_bottom_name = f"Bottom_{n_bottom}"
+
+    this_top = type(
+        this_top_name,
+        (Top, ), 
+        {"__init__": _top_constructor}
+    )
+    
+    this_bottom = type(
+        this_bottom_name, 
+        (Bottom, ), 
+        {"__init__": _bottom_constructor}
+    )
+
     if return_order is None:
         return_order = class_list
 
     class_out_list = []
     if type(class_list) is str:
-        newclass = type(class_list, (SequenceInterval, ), {"__init__": _constructor})
+        newclass = type(
+            class_list, 
+            (SequenceInterval, ), 
+            {"__init__": _constructor}
+        )
+        newclass.set_superset_class(this_top)
+        newclass.set_subset_class(this_bottom)
         return newclass
     elif type(class_list) is list:
         for name in class_list:
             class_out_list.append(
                 type(name, (SequenceInterval,), {"__init__": _constructor})
             )
         for idx, entry in enumerate(class_out_list):
+            if idx == 0:
+                entry.set_superset_class(this_top)
             if idx == len(class_out_list)-1:
-                pass
+                entry.set_subset_class(this_bottom)
             else:
-                class_out_list[idx].set_subset_class(class_out_list[idx+1])
+                entry.set_subset_class(class_out_list[idx+1])
         if type(return_order[0]) is int:
             return_list = [class_out_list[idx] for idx in return_order]
         elif type(return_order[0]) is str:
             return_idx = [return_order.index(x) for x in class_list]
             return_list = [class_out_list[idx] for idx in return_idx] 
         return return_list
```

### Comparing `aligned_textgrid-0.2.1/src/aligned_textgrid/sequences/sequences.py` & `aligned_textgrid-0.3.0/src/aligned_textgrid/sequences/sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,156 +4,25 @@
 """
 
 from praatio.utilities.constants import Interval
 from praatio.data_classes.interval_tier import IntervalTier
 from typing import Type, Any
 import numpy as np
 import warnings
-class SequenceInterval:
-    """
-    A class to describe an interval with precedence relationships and hierarchical relationships
 
-    Parameters:
-        Interval: A Praat textgrid Interval
-
-    Attributes:
-        start (float):
-            Start time of the interval
-        end (float):
-            End time of the interval
-        label (Any):
-            Label of the interval
-        intier (SequenceTier):
-            The sequence tier the current interval is within.
-        tier_index (int):
-            The index of sequence within its tier.
-        fol (SequenceInterval):
-            Instance of the following interval. Is the same subclass as the current instance.
-        prev (SequenceInterval): 
-            Instance of the previous interval. Is the same subclass as current instance.
-        super_instance (SequenceInterval): 
-            The instance of the superset. Cannot be the same subclass as the current instance.
-        subset_list (List[SequenceInterval]): 
-            A list of subset instances. Cannot be the same subclass of the current instance.
-        sub_starts (numpy.ndarray):
-            A numpy array of start times for the subset list
-        sub_ends (numpy.ndarray):
-            A numpy array of end times for the subset list
-        sub_labels (List[Any]):
-            A list of labels from the subset list
-        [] :
-            Indexes into the `subset_list`
-    """    
+class HierarchyMixins:
 
     # Ultimately, both of these class variables should be be
     # set to subclasses of SequenceInterval, but that can't be
     # done in the class definition since those subclasses
     # can't exist until after both SequenceVariable
     # and those subclasses have been created.
     superset_class = None
     subset_class = None
-
-    # utilities
-    def __init__(
-        self, 
-        Interval: Interval = Interval(None, None, None)
-    ):
-        if not Interval:
-            Interval = Interval(None, None, None)
-        self.start = Interval.start
-        self.end = Interval.end
-        self.label = Interval.label
         
-        self.fol = None
-        self.prev = None
-
-        ## prevent infinite recursion
-        if self.label != "#":
-            self.set_final()
-        if self.label != "#":
-            self.set_initial()
-
-        self.subset_list = []
-        self.super_instance= None
-
-        self.intier = None
-
-    def __contains__(self, item):
-        return item in self.subset_list
-
-    def __getitem__(self, idx):
-        return self.subset_list[idx]
-
-    def __iter__(self):
-        self.current = 0
-        return self
-    
-    def __len__(self):
-        return len(self.subset_list)
-    
-    def __next__(self):
-        if self.current < len(self.subset_list):
-            this_seg = self.subset_list[self.current]
-            self.current+=1
-            return this_seg
-        else:
-            raise StopIteration
-        
-    def index(
-            self,
-            subset_instance
-    ) -> int:
-        """_Returns subset instance index_
-
-        Args:
-            subset_instance (SequenceInterval): 
-                A subset instance to get the index of.
-
-        Returns:
-            int: The index of `subset_instance`
-        """
-        return self.subset_list.index(subset_instance)
-
-    def pop(
-            self,
-            subset_instance
-    ):
-        """_Pop a sequence interval from the subset list_
-
-        Args:
-            subset_instance (SequenceInterval): A sequence interval to pop
-        """
-        if subset_instance in self.subset_list:
-            pop_idx = self.index(subset_instance)
-            self.subset_list.pop(pop_idx)
-            self._set_subset_precedence()
-        else:
-            raise Exception("Subset instance not in subset list")
-    
-    def __repr__(self) -> str:
-        out_string = f"Class {type(self).__name__}, label: {self.label}"
-        if self.superset_class:
-            out_string += f", .superset_class: {self.superset_class.__name__}"
-            if self.super_instance:
-                out_string += f", .super_instance: {self.super_instance.label}"
-            else:
-                out_string += f", .super_instance, None"            
-        else:
-            out_string += ", .superset_class: None"     
-        if self.subset_class:
-            out_string += f", .subset_class: {self.subset_class.__name__}"
-            if self.subset_list:
-                out_string += f", .subset_list: {repr(self.sub_labels)}"
-        else:
-            out_string += ", .subset_class: None"
-        return out_string
-    
-    # Hierarchy methods
-    ## Superset Methods
-
     @classmethod
     def set_superset_class(
             cls, 
             superset_class: type = None
         ):
         """_Set the superset class_
 
@@ -161,72 +30,75 @@
             superset_class (Type[SequenceInterval], optional): 
                 Must be a subclass of Sequence Interval, but not the *same* class as the
                 current instance. Defaults to None.
 
         """
         if superset_class is None:
             cls.superset_class = None
-        elif cls is Top:
+        elif "Top" in cls.__name__ :
             cls.superset_class = None
-        elif issubclass(superset_class, SequenceInterval) and not superset_class is cls:
+        elif issubclass(superset_class, HierarchyPart) and not superset_class is cls:
             cls.superset_class = superset_class
             # avoid recursion here!
             if not cls.superset_class.subset_class is cls:
                 cls.superset_class.set_subset_class(cls)
         elif superset_class is cls:
             raise Exception(f"Sequence {cls.__name__} can't have {superset_class.__name__} as its superset class.")
-        elif not issubclass(superset_class, SequenceInterval):
+        elif not issubclass(superset_class, HierarchyPart):
             raise Exception(f"Sequence {cls.__name__} superset_class must be subclass of SequenceInterval. {superset_class.__name__} was given.")
         else:
             raise Exception(f"Unknown error setting {superset_class.__name__} as superset class of {cls.__name__}")
-
-    def set_super_instance(self, super_instance = None):
-        """_Sets the specific superset relationship_
-
-        Args:
-            super_instance (SegmentInterval, optional): 
-                Sets the superset relationship between this object and `super_instance` object.
-                Current object is appended to `super_instance`'s subset list.
-        """
-
-        if super_instance is None:
-            warnings.warn("No superset instance provided")   
-        elif isinstance(super_instance, self.superset_class) and not super_instance is self.super_instance:
-            self.super_instance = super_instance
-            self.super_instance.append_subset_list(self)
-        else:
-            raise Exception(f"The superset_class was defined as {self.superset_class.__name__}, but provided super_instance was {type(super_instance).__name__}")
-                        
-
-    ## Subset Methods
+        
     @classmethod
     def set_subset_class(cls, subset_class = None):
         """_summary_
 
         Args:
             subset_class (Type[SequenceInterval], optional): 
                 Must be a subclass of SequenceInterval, but not the *same* as the current instance.
                 Defaults to None.
         """
 
         if subset_class is None:
             cls.subset_class = None
-        elif cls is Bottom:
+        elif "Bottom" in cls.__name__:
             cls.subset_class = None
-        elif issubclass(subset_class, SequenceInterval) and not subset_class is cls:
+        elif issubclass(subset_class, HierarchyPart) and not subset_class is cls:
             cls.subset_class = subset_class
             # avoid recursion here!
             if not cls.subset_class.superset_class is cls:
                 cls.subset_class.set_superset_class(cls)
-        elif not issubclass(subset_class, SequenceInterval):
+        elif not issubclass(subset_class, HierarchyPart):
             raise Exception(f"Sequence {cls.__name__} subset_class must be subclass of SequenceInterval. {subset_class.__name__} was given.")
         elif subset_class is cls:
             raise Exception(f"Sequence {cls.__name__} can't have {subset_class.__name__} as its subset class.")
         else:
-            raise Exception(f"Unknown error setting {subset_class.__name__} as subset class of {cls.__name__}")    
+            raise Exception(f"Unknown error setting {subset_class.__name__} as subset class of {cls.__name__}")            
+
+class InstanceMixins(HierarchyMixins):
+
+    def set_super_instance(self, super_instance = None):
+        """_Sets the specific superset relationship_
+
+        Args:
+            super_instance (SegmentInterval, optional): 
+                Sets the superset relationship between this object and `super_instance` object.
+                Current object is appended to `super_instance`'s subset list.
+        """
+
+        if super_instance is None:
+            warnings.warn("No superset instance provided")   
+        elif isinstance(super_instance, self.superset_class) and not super_instance is self.super_instance:
+            self.super_instance = super_instance
+            self.super_instance.append_subset_list(self)
+        else:
+            raise Exception(f"The superset_class was defined as {self.superset_class.__name__}, but provided super_instance was {type(super_instance).__name__}")
+                        
+
+    ## Subset Methods
         
     def set_subset_list(self, subset_list = None):
         """_Appends all objects to the `subset_list`_
 
         Args:
             subset_list (List[SequenceInterval], optional): 
                 A list of SequenceInterval subclass objects. Cannot be the
@@ -287,97 +159,14 @@
             Private method. Sorts the subset_list
         """
         if len(self.subset_list) > 0:
             item_starts = self.sub_starts
             item_order = np.argsort(item_starts)
             self.subset_list = [self.subset_list[idx] for idx in item_order]
 
-    ### Subset Properties
-    @property
-    def sub_starts(self):
-        if len(self.subset_list) > 0:
-            start_arr = np.array([
-                seg.start for seg in self.subset_list
-            ])
-            return start_arr
-        else:
-            return np.array([])
-        
-    @property
-    def sub_ends(self):
-        if len(self.subset_list) > 0:
-            end_arr = np.array([
-                seg.end for seg in self.subset_list
-            ])
-            return end_arr
-        else:
-            return np.array([])
-    
-    @property
-    def sub_labels(self):
-        if len(self.subset_list) > 0:
-            lab_list = [seg.label for seg in self.subset_list]
-            return lab_list
-        else:
-            return []
-
-    ## Subset Validation
-    def validate(self) -> bool:
-        """_Validate the subset list_
-        Validation checks to see if
-
-        1. The first item in `subset_list` starts at the same time as `self`.
-        If not, does it start before or after `self.start`
-        2. The last item in `subset_list` ends at the same time as `self`.
-        If not, does it end before or after `self.end`.
-        3. Do all of the subset intervals fit "snugly" inside of the superset,
-        that is, with no gaps or overlaps.
-
-        This doesn't raise any exceptions, but does issue a warning for any
-        checks that don't pass.
-
-        Returns:
-            (bool):
-                - `True` if all checks pass, or if the `subset_list` is empty.
-                - `False` if any checks fail.
-        """
-        validation_concerns = []
-        if len(self.subset_list) == 0:
-            return True
-        else:
-            if not np.allclose(self.start, self.sub_starts[0]):
-                if self.start < self.sub_starts:
-                    validation_concerns.append(
-                        "First subset interval starts after current interval"
-                    )
-                else:
-                    validation_concerns.append(
-                        "First subset interval starts before current interval"
-                    )
-            if not np.allclose(self.end, self.sub_ends[-1]):
-                if self.end > self.sub_ends[-1]:
-                    validation_concerns.append(
-                        "Last subset interval ends before current interval"
-                    )
-                else:
-                    validation_concerns.append(
-                        "Last subset interval ends after current interval"
-                    )
-            if not np.allclose(self.sub_starts[1:], self.sub_ends[:-1]):
-                validation_concerns.append(
-                    "Not all subintervals fit snugly"
-                )
-            ## prepping messages
-            if len(validation_concerns) == 0:
-                return True
-            else:
-                validation_warn = "\n".join(validation_concerns)
-                warnings.warn(validation_warn)
-                return False
-
     # Precedence Methods
     def set_fol(
             self, next_int):
         """_Sets the following instance_
 
         Args:
             next_int (SequenceInterval): 
@@ -429,15 +218,71 @@
     def set_initial(self):
         """_Sets the current object as having no `prev` interval_
 
         While `self.prev` is defined for these intervals, the actual 
         instance does not appear in `self.super_instance.subset_list`
         """
         self.set_prev(type(self)(Interval(None, None, "#")))
-    
+
+    ## Subset Validation
+    def validate(self) -> bool:
+        """_Validate the subset list_
+        Validation checks to see if
+
+        1. The first item in `subset_list` starts at the same time as `self`.
+        If not, does it start before or after `self.start`
+        2. The last item in `subset_list` ends at the same time as `self`.
+        If not, does it end before or after `self.end`.
+        3. Do all of the subset intervals fit "snugly" inside of the superset,
+        that is, with no gaps or overlaps.
+
+        This doesn't raise any exceptions, but does issue a warning for any
+        checks that don't pass.
+
+        Returns:
+            (bool):
+                - `True` if all checks pass, or if the `subset_list` is empty.
+                - `False` if any checks fail.
+        """
+        validation_concerns = []
+        if len(self.subset_list) == 0:
+            return True
+        else:
+            if not np.allclose(self.start, self.sub_starts[0]):
+                if self.start < self.sub_starts:
+                    validation_concerns.append(
+                        "First subset interval starts after current interval"
+                    )
+                else:
+                    validation_concerns.append(
+                        "First subset interval starts before current interval"
+                    )
+            if not np.allclose(self.end, self.sub_ends[-1]):
+                if self.end > self.sub_ends[-1]:
+                    validation_concerns.append(
+                        "Last subset interval ends before current interval"
+                    )
+                else:
+                    validation_concerns.append(
+                        "Last subset interval ends after current interval"
+                    )
+            if not np.allclose(self.sub_starts[1:], self.sub_ends[:-1]):
+                validation_concerns.append(
+                    "Not all subintervals fit snugly"
+                )
+            ## prepping messages
+            if len(validation_concerns) == 0:
+                return True
+            else:
+                validation_warn = "\n".join(validation_concerns)
+                warnings.warn(validation_warn)
+                return False        
+
+class TierMixins:
+
     ## Tier operations
     @property
     def tier_index(self):
         if not self.intier is None:
             return self.intier.index(self)
         else:
             return None
@@ -470,15 +315,190 @@
         Returns:
             (SequenceInterval): The SequenceInterval at the relative index
         """
         if not self.intier is None:
             return self.intier[self.tier_index + idx]
         else:
             return None
+
+    def return_interval(self) -> Interval:
+        """_Return current object as `Interval`_
+        
+        Will be useful for saving back to textgrid
+
+        Returns:
+            (praatio.utilities.constants.Interval): A `praatio` `Interval` object
+        """
+        return Interval(self.start, self.end, self.label)        
+                
+class HierarchyPart(HierarchyMixins):
+    def __init__(self):
+        pass
+
+class SequenceInterval(InstanceMixins, TierMixins, HierarchyPart):
+    """
+    A class to describe an interval with precedence relationships and hierarchical relationships
+
+    Parameters:
+        Interval: A Praat textgrid Interval
+
+    Attributes:
+        start (float):
+            Start time of the interval
+        end (float):
+            End time of the interval
+        label (Any):
+            Label of the interval
+        intier (SequenceTier):
+            The sequence tier the current interval is within.
+        tier_index (int):
+            The index of sequence within its tier.
+        fol (SequenceInterval):
+            Instance of the following interval. Is the same subclass as the current instance.
+        prev (SequenceInterval): 
+            Instance of the previous interval. Is the same subclass as current instance.
+        super_instance (SequenceInterval): 
+            The instance of the superset. Cannot be the same subclass as the current instance.
+        subset_list (List[SequenceInterval]): 
+            A list of subset instances. Cannot be the same subclass of the current instance.
+        sub_starts (numpy.ndarray):
+            A numpy array of start times for the subset list
+        sub_ends (numpy.ndarray):
+            A numpy array of end times for the subset list
+        sub_labels (List[Any]):
+            A list of labels from the subset list
+        [] :
+            Indexes into the `subset_list`
+    """    
+
+    # utilities
+    def __init__(
+        self, 
+        Interval: Interval = Interval(None, None, None)
+    ):
+        super().__init__()
+        if not Interval:
+            Interval = Interval(None, None, None)
+        self.start = Interval.start
+        self.end = Interval.end
+        self.label = Interval.label
         
+        self.fol = None
+        self.prev = None
+
+        ## prevent infinite recursion
+        if self.label != "#":
+            self.set_final()
+        if self.label != "#":
+            self.set_initial()
+
+        self.subset_list = []
+        self.super_instance= None
+
+        self.intier = None
+
+    def __contains__(self, item):
+        return item in self.subset_list
+
+    def __getitem__(self, idx):
+        return self.subset_list[idx]
+
+    def __iter__(self):
+        self.current = 0
+        return self
+    
+    def __len__(self):
+        return len(self.subset_list)
+    
+    def __next__(self):
+        if self.current < len(self.subset_list):
+            this_seg = self.subset_list[self.current]
+            self.current+=1
+            return this_seg
+        else:
+            raise StopIteration
+        
+    def index(
+            self,
+            subset_instance
+    ) -> int:
+        """_Returns subset instance index_
+
+        Args:
+            subset_instance (SequenceInterval): 
+                A subset instance to get the index of.
+
+        Returns:
+            int: The index of `subset_instance`
+        """
+        return self.subset_list.index(subset_instance)
+
+    def pop(
+            self,
+            subset_instance
+    ):
+        """_Pop a sequence interval from the subset list_
+
+        Args:
+            subset_instance (SequenceInterval): A sequence interval to pop
+        """
+        if subset_instance in self.subset_list:
+            pop_idx = self.index(subset_instance)
+            self.subset_list.pop(pop_idx)
+            self._set_subset_precedence()
+        else:
+            raise Exception("Subset instance not in subset list")
+    
+    def __repr__(self) -> str:
+        out_string = f"Class {type(self).__name__}, label: {self.label}"
+        if self.superset_class:
+            out_string += f", .superset_class: {self.superset_class.__name__}"
+            if self.super_instance:
+                out_string += f", .super_instance: {self.super_instance.label}"
+            else:
+                out_string += f", .super_instance, None"            
+        else:
+            out_string += ", .superset_class: None"     
+        if self.subset_class:
+            out_string += f", .subset_class: {self.subset_class.__name__}"
+            if self.subset_list:
+                out_string += f", .subset_list: {repr(self.sub_labels)}"
+        else:
+            out_string += ", .subset_class: None"
+        return out_string
+    
+    # properties
+    @property
+    def sub_starts(self):
+        if len(self.subset_list) > 0:
+            start_arr = np.array([
+                seg.start for seg in self.subset_list
+            ])
+            return start_arr
+        else:
+            return np.array([])
+        
+    @property
+    def sub_ends(self):
+        if len(self.subset_list) > 0:
+            end_arr = np.array([
+                seg.end for seg in self.subset_list
+            ])
+            return end_arr
+        else:
+            return np.array([])
+    
+    @property
+    def sub_labels(self):
+        if len(self.subset_list) > 0:
+            lab_list = [seg.label for seg in self.subset_list]
+            return lab_list
+        else:
+            return []
+      
     ## Fusion
     def fuse_rightwards(
             self, 
             label_fun = lambda x, y: " ".join([x, y])
         ):
         """_Fuse the current segment with the following segment_
 
@@ -556,43 +576,33 @@
 
         Args:
             feature (str): New attribute name
             value (Any): New attribute value
         """
         setattr(self, feature, value)
 
-    def return_interval(self) -> Interval:
-        """_Return current object as `Interval`_
-        
-        Will be useful for saving back to textgrid
-
-        Returns:
-            (praatio.utilities.constants.Interval): A `praatio` `Interval` object
-        """
-        return Interval(self.start, self.end, self.label)
-
-class Top(SequenceInterval):
+class Top(HierarchyPart):
     """_A top level interval class_
     
     This is a special subclass intended to be the `superset_class` 
     for classes at the top of the hierarchy.
 
     """
-    def __init__(self, Interval=Interval(None, None, None)):
-        super().__init__(Interval)
+    def __init__(self):
+        super().__init__()
 
-class Bottom(SequenceInterval):
+class Bottom(HierarchyPart):
     """_A bottom level interval class_
 
     This is a special subclass intended to be the `subset_class` 
     for classes at the bottom of the hierarchy.
 
     """
-    def __init__(self, Interval=Interval(None, None, None)):
-        super().__init__(Interval)
+    def __init__(self):
+        super().__init__()
 
 # This is how the default behavior of `SequenceInterval` 
 # with respect to subset and superset classes is controlled
 Top.set_superset_class()
 Bottom.set_subset_class()
 SequenceInterval.set_superset_class(Top)
 SequenceInterval.set_subset_class(Bottom)
```

### Comparing `aligned_textgrid-0.2.1/src/aligned_textgrid/sequences/tiers.py` & `aligned_textgrid-0.3.0/src/aligned_textgrid/sequences/tiers.py`

 * *Files 17% similar despite different names*

```diff
@@ -301,27 +301,47 @@
         ) -> list[SequenceTier]:
         """_Arranges tiers by hierarchy_
 
         Args:
             tiers (list[SequenceTier]): _description_
         """
         top_to_bottom = []
-        to_arrange = len(tiers)
-        top_idx = [x.superset_class for x in tiers].index(Top)
+        tier_classes = [x.entry_class for x in tiers]
+        seed_tier = tiers[0]
+        done = False
+        while not done:
+            if issubclass(seed_tier.superset_class, Top):
+                top_idx = tiers.index(seed_tier)
+                done = True
+                break
+            elif seed_tier.superset_class not in tier_classes:
+                top_idx = tiers.index(seed_tier)
+                done = True
+                break
+            else:
+                next_tier_idx = tier_classes.index(seed_tier.superset_class)
+                seed_tier = tiers[next_tier_idx]
+
+
         top_to_bottom.append(tiers[top_idx])
-        to_arrange += -1
-        while to_arrange > 0:
+        done = False
+        while not done:
             curr = top_to_bottom[-1]
-            if curr.subset_class is Bottom:
+            if issubclass(curr.subset_class, Bottom):
+                done = True
                 break
-            next_idx = [x.entry_class for x in tiers].index(curr.subset_class)
-            top_to_bottom.append(tiers[next_idx])
-            to_arrange += -1
+            else:
+                try:
+                    next_idx = [x.entry_class for x in tiers].index(curr.subset_class)
+                except ValueError:
+                    return top_to_bottom
+                
+                top_to_bottom.append(tiers[next_idx])
         return(top_to_bottom)
-    
+            
     @property
     def entry_classes(self):
         return [x.entry_class for x in self.tier_list]
     
     @property
     def tier_names(self):
         return [x.name for x in self.tier_list]
```

### Comparing `aligned_textgrid-0.2.1/src/aligned_textgrid/sequences/word_and_phone.py` & `aligned_textgrid-0.3.0/src/aligned_textgrid/sequences/word_and_phone.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,12 +72,21 @@
     def phone_list(self):
         return self.subset_list
 
     @property
     def phones(self):
         return self.sub_labels
 
-Word.set_superset_class(Top)
+class Top_wp(Top):
+    def __init__(self):
+        super.__init__()
+
+class Bottom_wp(Bottom):
+    def __init__(self):
+        super.__init__()
+
+
+Word.set_superset_class(Top_wp)
 Word.set_subset_class(Phone)
-Phone.set_subset_class(Bottom)
+Phone.set_subset_class(Bottom_wp)
 # not necessary
 # Phone.set_superset_class(Word)
```

### Comparing `aligned_textgrid-0.2.1/setup.py` & `aligned_textgrid-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24.2,<2.0.0', 'praatio>=6.0.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'aligned-textgrid',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'Classes for defining sequential information from TextGrids',
-    'long_description': '![PyPI](https://img.shields.io/pypi/v/aligned-textgrid)\n![lint_and_test](https://github.com/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/actions/workflows/test_and_run.yml/badge.svg?event=pull_request&branch=main)\n[![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/branch/dev/graph/badge.svg?token=27YSOQ5ZEL)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid)\n[![Maintainability](https://api.codeclimate.com/v1/badges/2387cd247bd8f1211323/maintainability)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/maintainability)\n[![Documentation Status](https://readthedocs.org/projects/alignedtextgrid/badge/?version=latest)](https://alignedtextgrid.readthedocs.io/en/latest/?badge=latest)\n\n# aligned_textgrid\n\nThe aligned-textgrid package provides a python interface for representing and operating on TextGrids produced by forced aligners like [FAVE](https://github.com/JoFrhwld/FAVE) or the [Montreal Forced Aligner](https://montreal-forced-aligner.readthedocs.io/en/latest/). Classes provided by aligned-textgrid represent hierarchical and precedence relationships among data stored in TextGrid formats allowing for simplified and more accessible analysis of aligned speech data.\n\n## Installation\nTo install aligned-textgrid using pip, run the following command in your terminal:\n\n```bash\npip install aligned-textgrid\n```\n\n## Example Use Cases\n\n- You want to quickly loop through the Phone tier of a Textgrid, and *also* access information about the word it is a part of.\n- You want to quickly loop over the Word tier of a Textgrid and quickly count how many phones it has.\n- You want to programmatically merge together adjacent Textgrid intervals.\n\nFor examples on how to use the pacakge, see the [Documentation Usage ppages](https://alignedtextgrid.readthedocs.io/en/latest/usage/)\n\n## Not another TextGrid implementation\nThe aligned-textgrid package is not another TextGrid implementation. TextGrids are a plain text data format used chiefly by the Praat software suite. Programmers have implemented interfaces for this data format so that scripting and data wrangling can be done in a user\'s programming language of choice. These intefaces include [praatio](http://timmahrt.github.io/praatIO/praatio.html) and Kyle Gorman\'s [textgrid.py](https://github.com/kylebgorman/textgrid). \n\nWhat sets aligned-textgrid apart from other implementations of the TextGrid format is an emphasis on the *relationships* among different items represented in the data. Let\'s explore this using Gorman\'s `textgrid.py`:\n\n```{python}\nfrom textgrid import TextGrid\n\ntg = TextGrid.fromFile(\'usage/resources/josef-fruehwald_speaker.TextGrid\')\n```\n\nIn `tg` we now have a representation of our TextGrid. TextGrids are primarily organized into tiers which can store data as either points or intervals. In `textgrid.py` these tiers are accessed by their index, so `tg[0]` is the highest tier, `tg[1]` is the next highest, and so on (our data only has two tiers). These tiers can also have names like in our data:\n\n```{python}\nprint(f"First tier is named {tg[0].name}")\nprint(f"Second tier is named {tg[1].name}")\n```\n\nIn the case of *aligned* TextGrid data like ours, these names are more than a convenience. Tiers on aligned data are *hierarchical*. Both of our tiers represent the same information but at different levels of granularity: the `words` tier represents the data as a series of words and the `phones` tier represents the data as a series of phones. Put another way, the `phones` tier and the `words` tier are codependent. Praat TextGrids, and by extension its Python implementations, are largely agnostic when it comes to the relationship between tiers. This allows them to handle a wide range of use cases, but for *aligned* data, the dependency relationships between tiers are metadata which should be incorporated into the data representations. Through classes like `TierGroup`, aligned-textgrid extends these general TextGrid data structures for use with force-aligned data.\n\n### Relating data within and across tiers\nPraat TextGrids store time-dependent data, and within a tier each data entry has an ordered relationship to others within its tier. While having the specific time-domain data is useful, often what we are interested in is the abstracted relationship between points like which came first or whether two annotations overlap in time. Python implementations of TextGrids store the time-domain data as part of the representation, but these ordered relationships are represented more abstractly.\n\n```{python}\nwordTier = 0\n\ntg[wordTier][0] > tg[wordTier][1]\n```\n\nIn `textgrid.py`, we can compare two words and get a true or false value. In the example above, the comparison is false: word zero does not occur after word 1. <!-- On an abstract level this ordering as actually kinda confusing. A > B => false which makes sense if you consider time stamps, but if we want to treat > and < as *precedence* operators rather than comparitors, the truth table needs flipped. (1) we might want to do that (2) we might want to document that behavior. -CB 13 March 2023 -->\n\nA major issue when working with these precedence orderings is knowing and remembering where in the data you are. In the following example, we use the `random` library to choose an arbitrary entry in the word tier. We do not store the index of this piece of data, so how do we know its relationship to other pieces of data? What word comes after it or before it? How would we get to them? In this case, we could use the `.index()` method to search the original list for the item we have. This works well, but it is costly because the whole data set needs to be searched. For a short passage like we\'re using, that is not a major problem, but when working with hours-long audio recordings, searches like that can slow down an analysis or data coding script.\n\n```{python}\nfrom random import randint\nnum_words = len(tg[wordTier])\n\nword = tg[wordTier][randint(0,num_words)]\n```\n\nThe aligned-textgrid package aims to resolve these issues by incorporating these relationships into the representations from the start. The attribute `.fol` of `aligned_textgrid.sequences.sequences.SequenceInterval` provides access to the next interval in the sequence even if you don\'t know precisely where in the sequence you are. You can also use the `.intier` and `.subset_list` attributes to navigate up and down the tier hierarchy.',
+    'long_description': '![PyPI](https://img.shields.io/pypi/v/aligned-textgrid)\n![lint_and_test](https://github.com/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/actions/workflows/test_and_run.yml/badge.svg?event=pull_request&branch=main)\n[![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/branch/dev/graph/badge.svg?token=27YSOQ5ZEL)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid)\n[![Maintainability](https://api.codeclimate.com/v1/badges/2387cd247bd8f1211323/maintainability)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/maintainability)\n[![Documentation Status](https://readthedocs.org/projects/alignedtextgrid/badge/?version=latest)](https://alignedtextgrid.readthedocs.io/en/latest/?badge=latest)\n[![DOI](https://zenodo.org/badge/552633207.svg)](https://zenodo.org/badge/latestdoi/552633207)\n\n\n# aligned_textgrid\n\nThe aligned-textgrid package provides a python interface for representing and operating on TextGrids produced by forced aligners like [FAVE](https://github.com/JoFrhwld/FAVE) or the [Montreal Forced Aligner](https://montreal-forced-aligner.readthedocs.io/en/latest/). Classes provided by aligned-textgrid represent hierarchical and precedence relationships among data stored in TextGrid formats allowing for simplified and more accessible analysis of aligned speech data.\n\n## Installation\nTo install aligned-textgrid using pip, run the following command in your terminal:\n\n```bash\npip install aligned-textgrid\n```\n\n## Example Use Cases\n\n- You want to quickly loop through the Phone tier of a Textgrid, and *also* access information about the word it is a part of.\n- You want to quickly loop over the Word tier of a Textgrid and quickly count how many phones it has.\n- You want to programmatically merge together adjacent Textgrid intervals.\n\nFor examples on how to use the pacakge, see the [Documentation Usage ppages](https://alignedtextgrid.readthedocs.io/en/latest/usage/)\n\n## Not another TextGrid implementation\nThe aligned-textgrid package is not another TextGrid implementation. TextGrids are a plain text data format used chiefly by the Praat software suite. Programmers have implemented interfaces for this data format so that scripting and data wrangling can be done in a user\'s programming language of choice. These intefaces include [praatio](http://timmahrt.github.io/praatIO/praatio.html) and Kyle Gorman\'s [textgrid.py](https://github.com/kylebgorman/textgrid). \n\nWhat sets aligned-textgrid apart from other implementations of the TextGrid format is an emphasis on the *relationships* among different items represented in the data. Let\'s explore this using Gorman\'s `textgrid.py`:\n\n```{python}\nfrom textgrid import TextGrid\n\ntg = TextGrid.fromFile(\'usage/resources/josef-fruehwald_speaker.TextGrid\')\n```\n\nIn `tg` we now have a representation of our TextGrid. TextGrids are primarily organized into tiers which can store data as either points or intervals. In `textgrid.py` these tiers are accessed by their index, so `tg[0]` is the highest tier, `tg[1]` is the next highest, and so on (our data only has two tiers). These tiers can also have names like in our data:\n\n```{python}\nprint(f"First tier is named {tg[0].name}")\nprint(f"Second tier is named {tg[1].name}")\n```\n\nIn the case of *aligned* TextGrid data like ours, these names are more than a convenience. Tiers on aligned data are *hierarchical*. Both of our tiers represent the same information but at different levels of granularity: the `words` tier represents the data as a series of words and the `phones` tier represents the data as a series of phones. Put another way, the `phones` tier and the `words` tier are codependent. Praat TextGrids, and by extension its Python implementations, are largely agnostic when it comes to the relationship between tiers. This allows them to handle a wide range of use cases, but for *aligned* data, the dependency relationships between tiers are metadata which should be incorporated into the data representations. Through classes like `TierGroup`, aligned-textgrid extends these general TextGrid data structures for use with force-aligned data.\n\n### Relating data within and across tiers\nPraat TextGrids store time-dependent data, and within a tier each data entry has an ordered relationship to others within its tier. While having the specific time-domain data is useful, often what we are interested in is the abstracted relationship between points like which came first or whether two annotations overlap in time. Python implementations of TextGrids store the time-domain data as part of the representation, but these ordered relationships are represented more abstractly.\n\n```{python}\nwordTier = 0\n\ntg[wordTier][0] > tg[wordTier][1]\n```\n\nIn `textgrid.py`, we can compare two words and get a true or false value. In the example above, the comparison is false: word zero does not occur after word 1. <!-- On an abstract level this ordering as actually kinda confusing. A > B => false which makes sense if you consider time stamps, but if we want to treat > and < as *precedence* operators rather than comparitors, the truth table needs flipped. (1) we might want to do that (2) we might want to document that behavior. -CB 13 March 2023 -->\n\nA major issue when working with these precedence orderings is knowing and remembering where in the data you are. In the following example, we use the `random` library to choose an arbitrary entry in the word tier. We do not store the index of this piece of data, so how do we know its relationship to other pieces of data? What word comes after it or before it? How would we get to them? In this case, we could use the `.index()` method to search the original list for the item we have. This works well, but it is costly because the whole data set needs to be searched. For a short passage like we\'re using, that is not a major problem, but when working with hours-long audio recordings, searches like that can slow down an analysis or data coding script.\n\n```{python}\nfrom random import randint\nnum_words = len(tg[wordTier])\n\nword = tg[wordTier][randint(0,num_words)]\n```\n\nThe aligned-textgrid package aims to resolve these issues by incorporating these relationships into the representations from the start. The attribute `.fol` of `aligned_textgrid.sequences.sequences.SequenceInterval` provides access to the next interval in the sequence even if you don\'t know precisely where in the sequence you are. You can also use the `.intier` and `.subset_list` attributes to navigate up and down the tier hierarchy.\n',
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://alignedtextgrid.readthedocs.io/en/latest/',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `aligned_textgrid-0.2.1/PKG-INFO` & `aligned_textgrid-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligned-textgrid
-Version: 0.2.1
+Version: 0.3.0
 Summary: Classes for defining sequential information from TextGrids
 Home-page: https://alignedtextgrid.readthedocs.io/en/latest/
 License: GPL-3.0-or-later
 Author: JoFrhwld
 Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -17,14 +17,16 @@
 Description-Content-Type: text/markdown
 
 ![PyPI](https://img.shields.io/pypi/v/aligned-textgrid)
 ![lint_and_test](https://github.com/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/actions/workflows/test_and_run.yml/badge.svg?event=pull_request&branch=main)
 [![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/branch/dev/graph/badge.svg?token=27YSOQ5ZEL)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid)
 [![Maintainability](https://api.codeclimate.com/v1/badges/2387cd247bd8f1211323/maintainability)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/maintainability)
 [![Documentation Status](https://readthedocs.org/projects/alignedtextgrid/badge/?version=latest)](https://alignedtextgrid.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/552633207.svg)](https://zenodo.org/badge/latestdoi/552633207)
+
 
 # aligned_textgrid
 
 The aligned-textgrid package provides a python interface for representing and operating on TextGrids produced by forced aligners like [FAVE](https://github.com/JoFrhwld/FAVE) or the [Montreal Forced Aligner](https://montreal-forced-aligner.readthedocs.io/en/latest/). Classes provided by aligned-textgrid represent hierarchical and precedence relationships among data stored in TextGrid formats allowing for simplified and more accessible analysis of aligned speech data.
 
 ## Installation
 To install aligned-textgrid using pip, run the following command in your terminal:
@@ -78,7 +80,8 @@
 from random import randint
 num_words = len(tg[wordTier])
 
 word = tg[wordTier][randint(0,num_words)]
 ```
 
 The aligned-textgrid package aims to resolve these issues by incorporating these relationships into the representations from the start. The attribute `.fol` of `aligned_textgrid.sequences.sequences.SequenceInterval` provides access to the next interval in the sequence even if you don't know precisely where in the sequence you are. You can also use the `.intier` and `.subset_list` attributes to navigate up and down the tier hierarchy.
+
```

