# Comparing `tmp/donatellopyzza-1.5.0.tar.gz` & `tmp/donatellopyzza-1.5.1.tar.gz`

## Comparing `donatellopyzza-1.5.0.tar` & `donatellopyzza-1.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/__init__.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/envBuilder.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/game.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/main.py
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/mazeGenerator.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/turtleAgent.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/environments/hard_maze.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/environments/maze.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/environments/test.txt
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/images/pizza.png
--rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/images/turtle.png
--rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/images/turtle_small.png
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/agent.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/careTaker.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/constants.py
--rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/grid.py
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/gui.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/map.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/memento.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/orientation.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/originator.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/parser.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/square.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/turn.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/LICENSE
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/__init__.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/envBuilder.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/game.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/main.py
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/mazeGenerator.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/turtleAgent.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/data/environments/hard_maze.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/data/environments/maze.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/data/environments/test.txt
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/data/images/pizza.png
+-rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/data/images/turtle.png
+-rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/data/images/turtle_small.png
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/agent.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/careTaker.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/constants.py
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/grid.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/gui.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/map.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/memento.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/orientation.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/originator.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/parser.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/square.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/donatellopyzza/grid/turn.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/LICENSE
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 donatellopyzza-1.5.1/PKG-INFO
```

### Comparing `donatellopyzza-1.5.0/donatellopyzza/envBuilder.py` & `donatellopyzza-1.5.1/donatellopyzza/envBuilder.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/game.py` & `donatellopyzza-1.5.1/donatellopyzza/game.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/main.py` & `donatellopyzza-1.5.1/donatellopyzza/main.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/mazeGenerator.py` & `donatellopyzza-1.5.1/donatellopyzza/mazeGenerator.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/data/images/pizza.png` & `donatellopyzza-1.5.1/donatellopyzza/data/images/pizza.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/data/images/turtle.png` & `donatellopyzza-1.5.1/donatellopyzza/data/images/turtle.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/data/images/turtle_small.png` & `donatellopyzza-1.5.1/donatellopyzza/data/images/turtle_small.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/grid/agent.py` & `donatellopyzza-1.5.1/donatellopyzza/grid/agent.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/grid/grid.py` & `donatellopyzza-1.5.1/donatellopyzza/grid/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             return Feedback.MOVED
         if not square is None:
             #Si l'agent n'a pas bougé alors il a rencontré un mur
             if square.equal(old_square):
                 return Feedback.COLLISION
             elif square.isPizza():
                 self.foundPizza = True
-                return Feedback.IS_ON_PIZZA
+                return Feedback.MOVED_ON_PIZZA
             return Feedback.MOVED
         elif not square_touched is None:
             if square_touched.isWall():
                 return Feedback.TOUCHED_WALL
             elif square_touched.isPizza():
                 return Feedback.TOUCHED_PIZZA
             return Feedback.TOUCHED_NOTHING
```

### Comparing `donatellopyzza-1.5.0/donatellopyzza/grid/gui.py` & `donatellopyzza-1.5.1/donatellopyzza/grid/gui.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/grid/map.py` & `donatellopyzza-1.5.1/donatellopyzza/grid/map.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/grid/parser.py` & `donatellopyzza-1.5.1/donatellopyzza/grid/parser.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/donatellopyzza/grid/square.py` & `donatellopyzza-1.5.1/donatellopyzza/grid/square.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/LICENSE` & `donatellopyzza-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.0/README.md` & `donatellopyzza-1.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,43 +17,25 @@
 `pip install -r requirements.txt`
 
 `pip install donatellopyzza`
 
 
 ## Getting started
 
-`Action` and `Feedback` define the different actions and feedbacks types. You can use the following actions in your code:
-
-    Action.MOVE_FORWARD -> make your turtle go one step forward
-    Action.TURN_RIGHT -> your turtle will turn on its right
-    Action.TURN_LEFT -> on its left
-    Action.TOUCH -> the turtle will touch the cell in front of it to know its type
-
-
-Depending on your action, the game can provide you one of the following feedback:
-
-    Feedback.COLLISION -> you just tried to walk in a wall !
-    Feedback.MOVED -> you successfully moved
-    Feedback.MOVED_ON_PIZZA -> your turtle is on the pizza (congratulation!)
-    Feedback.TOUCHED_WALL -> you just touched a wall
-    Feedback.TOUCHED_NOTHING -> the touched cell is empty (no wall, no pizza, you can walk on it)
-    Feedback.TOUCHED_PIZZA -> the turtle touched the pizza
-
-
-Now you know how to play, let's create the game and its environment:
-
 First, import the right modules to run the game:
 
 ```python
 from donatellopyzza import Game
 from donatellopyzza import Action
 from donatellopyzza import Feedback
+from donatellopyzza import Maze
 ```
 
 `Game` is a class that you will use to create a game instance
+Let's create the game and its environment:
 
 ```python
 # specify the name of the environment
 __ENVIRONMENT__ = "maze"
 # display the interface (or not)
 __GUI__ = True
 
@@ -68,14 +50,45 @@
 ```python
 feedback = turtle.execute(Action.FORWARD)
 print(feedback)
 ```
 
 You can use the feedback from the `execute()` method to see what happened after your action.
 
+## Knowing actions and feedbacks
+
+`Action` and `Feedback` define the different actions and feedbacks types. You can use the following actions in your code:
+
+    Action.MOVE_FORWARD -> make your turtle go one step forward
+    Action.TURN_RIGHT -> your turtle will turn on its right
+    Action.TURN_LEFT -> on its left
+    Action.TOUCH -> the turtle will touch the cell in front of it to know its type
+
+
+Depending on your action, the game can provide you one of the following feedback:
+
+    Feedback.COLLISION -> you just tried to walk in a wall !
+    Feedback.MOVED -> you successfully moved
+    Feedback.MOVED_ON_PIZZA -> your turtle is on the pizza (congratulation!)
+    Feedback.TOUCHED_WALL -> you just touched a wall
+    Feedback.TOUCHED_NOTHING -> the touched cell is empty (no wall, no pizza, you can walk on it)
+    Feedback.TOUCHED_PIZZA -> the turtle touched the pizza
+
+
+## Generating and save you own mazes
+
+`Maze` is a class used to generate and save new mazes. You can save retrieve saved maze by their names as indicated in example files. A new maze is generated (and save) as follow:
+
+```python
+maze = Maze.create_maze(10, 10)
+fn = "test"
+maze.save(maze, filename=fn)
+```
+
+
 For more details, you can find several complete examples of the game loop in the `examples` folder on the github repository of this project.
 
 Have fun!
 
 
 ## What's new
 
@@ -83,8 +96,10 @@
     Integration of a maze generator from Alexandru Văleanu (https://github.com/AlexandruValeanu/Mazify)
 - 2023-01-17 (v1.2)
     Initial release
 
 
 ## Roadmap
 
+- remove the green band on the right of the screen when using the GUI
+- make some easy tutorials to help beginners use this package 
 - ~~add a gridworld generator~~
```

### Comparing `donatellopyzza-1.5.0/pyproject.toml` & `donatellopyzza-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DonatelloPyzza"
-version = "1.5.0"
+version = "1.5.1"
 authors = [
   { name="Mickaël Bettinelli", email="mickael.bettinelli@univ-smb.fr" },
 ]
 description = "A simple grid environment to learn Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `donatellopyzza-1.5.0/PKG-INFO` & `donatellopyzza-1.5.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DonatelloPyzza
-Version: 1.5.0
+Version: 1.5.1
 Summary: A simple grid environment to learn Python
 Project-URL: Homepage, https://github.com/MilowB/Donatello
 Project-URL: Bug Tracker, https://github.com/MilowB/Donatello/pulls
 Author-email: Mickaël Bettinelli <mickael.bettinelli@univ-smb.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,43 +31,25 @@
 `pip install -r requirements.txt`
 
 `pip install donatellopyzza`
 
 
 ## Getting started
 
-`Action` and `Feedback` define the different actions and feedbacks types. You can use the following actions in your code:
-
-    Action.MOVE_FORWARD -> make your turtle go one step forward
-    Action.TURN_RIGHT -> your turtle will turn on its right
-    Action.TURN_LEFT -> on its left
-    Action.TOUCH -> the turtle will touch the cell in front of it to know its type
-
-
-Depending on your action, the game can provide you one of the following feedback:
-
-    Feedback.COLLISION -> you just tried to walk in a wall !
-    Feedback.MOVED -> you successfully moved
-    Feedback.MOVED_ON_PIZZA -> your turtle is on the pizza (congratulation!)
-    Feedback.TOUCHED_WALL -> you just touched a wall
-    Feedback.TOUCHED_NOTHING -> the touched cell is empty (no wall, no pizza, you can walk on it)
-    Feedback.TOUCHED_PIZZA -> the turtle touched the pizza
-
-
-Now you know how to play, let's create the game and its environment:
-
 First, import the right modules to run the game:
 
 ```python
 from donatellopyzza import Game
 from donatellopyzza import Action
 from donatellopyzza import Feedback
+from donatellopyzza import Maze
 ```
 
 `Game` is a class that you will use to create a game instance
+Let's create the game and its environment:
 
 ```python
 # specify the name of the environment
 __ENVIRONMENT__ = "maze"
 # display the interface (or not)
 __GUI__ = True
 
@@ -82,14 +64,45 @@
 ```python
 feedback = turtle.execute(Action.FORWARD)
 print(feedback)
 ```
 
 You can use the feedback from the `execute()` method to see what happened after your action.
 
+## Knowing actions and feedbacks
+
+`Action` and `Feedback` define the different actions and feedbacks types. You can use the following actions in your code:
+
+    Action.MOVE_FORWARD -> make your turtle go one step forward
+    Action.TURN_RIGHT -> your turtle will turn on its right
+    Action.TURN_LEFT -> on its left
+    Action.TOUCH -> the turtle will touch the cell in front of it to know its type
+
+
+Depending on your action, the game can provide you one of the following feedback:
+
+    Feedback.COLLISION -> you just tried to walk in a wall !
+    Feedback.MOVED -> you successfully moved
+    Feedback.MOVED_ON_PIZZA -> your turtle is on the pizza (congratulation!)
+    Feedback.TOUCHED_WALL -> you just touched a wall
+    Feedback.TOUCHED_NOTHING -> the touched cell is empty (no wall, no pizza, you can walk on it)
+    Feedback.TOUCHED_PIZZA -> the turtle touched the pizza
+
+
+## Generating and save you own mazes
+
+`Maze` is a class used to generate and save new mazes. You can save retrieve saved maze by their names as indicated in example files. A new maze is generated (and save) as follow:
+
+```python
+maze = Maze.create_maze(10, 10)
+fn = "test"
+maze.save(maze, filename=fn)
+```
+
+
 For more details, you can find several complete examples of the game loop in the `examples` folder on the github repository of this project.
 
 Have fun!
 
 
 ## What's new
 
@@ -97,8 +110,10 @@
     Integration of a maze generator from Alexandru Văleanu (https://github.com/AlexandruValeanu/Mazify)
 - 2023-01-17 (v1.2)
     Initial release
 
 
 ## Roadmap
 
+- remove the green band on the right of the screen when using the GUI
+- make some easy tutorials to help beginners use this package 
 - ~~add a gridworld generator~~
```

