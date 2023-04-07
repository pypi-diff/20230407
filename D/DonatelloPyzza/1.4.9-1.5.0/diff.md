# Comparing `tmp/donatellopyzza-1.4.9.tar.gz` & `tmp/donatellopyzza-1.5.0.tar.gz`

## Comparing `donatellopyzza-1.4.9.tar` & `donatellopyzza-1.5.0.tar`

### file list

```diff
@@ -1,32 +1,29 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/__init__.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/agent.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/careTaker.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/envBuilder.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/game.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/generator.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/grid.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/gui.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/main.py
--rw-r--r--   0        0        0    10706 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/map.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/memento.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/orientation.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/originator.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/parser.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/square.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/turn.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/turtleAgent.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/data/environments/hard_maze
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/data/environments/large_maze
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/data/environments/long_maze
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/data/environments/maze
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/data/environments/small_maze
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/data/environments/very_large_maze
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/data/images/pizza.png
--rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/data/images/turtle.png
--rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/data/images/turtle_small.png
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/donatellopyzza/grid/test.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/LICENSE
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/pyproject.toml
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 donatellopyzza-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/__init__.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/envBuilder.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/game.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/main.py
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/mazeGenerator.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/turtleAgent.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/environments/hard_maze.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/environments/maze.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/environments/test.txt
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/images/pizza.png
+-rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/images/turtle.png
+-rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/data/images/turtle_small.png
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/agent.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/careTaker.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/constants.py
+-rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/grid.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/gui.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/map.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/memento.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/orientation.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/originator.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/parser.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/square.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/donatellopyzza/grid/turn.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 donatellopyzza-1.5.0/PKG-INFO
```

### Comparing `donatellopyzza-1.4.9/donatellopyzza/agent.py` & `donatellopyzza-1.5.0/donatellopyzza/grid/agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import os, sys, pygame
-from .originator import *
-from .careTaker import *
-from .orientation import *
-from donatellopyzza.grid.test import *
+import os, sys
+import pygame
+from originator import *
+from careTaker import *
+from orientation import *
+
 from random import randint
 import pkg_resources
 
 class Agent:
     def __init__(self, name, begin, end, color):
-        self.test = Test()
         self._name = name
         self.orientation = Orientation.NORTH
         self.num = id(self)
         self.begin = begin
         self.end = end
         self.color = color
         self.originator = Originator()
         self.caretaker = CareTaker()
         self.position = None
-        path = pkg_resources.resource_filename(__name__, "data/images/turtle_small.png")
+        path = pkg_resources.resource_filename(__name__, "../data/images/turtle_small.png")
         self.turtle = pygame.image.load(path)
         self.angle = 0
 
     def setCurrentPosition(self, position):
         self.position = position
 
     def savePosition(self, square):
```

### Comparing `donatellopyzza-1.4.9/donatellopyzza/envBuilder.py` & `donatellopyzza-1.5.0/donatellopyzza/envBuilder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import os, sys, inspect
 import pkg_resources
 from pathlib import Path
 from pkg_resources import resource_string
 
 #Pour inclure les fichiers de l'environnement
-'''
 cmd_subfolder_grid = os.path.realpath(os.path.abspath(os.path.join(os.path.split(inspect.getfile( inspect.currentframe() ))[0],"grid")))
 if cmd_subfolder_grid not in sys.path:
     sys.path.insert(0, cmd_subfolder_grid)
-'''
 
-from .parser import Parser
-from .grid import Grid
+from parser import Parser
+from grid import Grid
 
 
 class EnvBuilder:
     def __init__(self, name: str, gui: bool):
         self.name = name
         self.gui = gui
 
     def get_data_path(self, path):
-        
         return pkg_resources.resource_filename(__name__, path + self.name)
 
     def build_grid(self):
         data_path = self.get_data_path("data/environments/")
         parser = Parser(data_path)
         gui, map, agents = parser.parse()
         # for simplicity matters, we only use one agent in this package
```

### Comparing `donatellopyzza-1.4.9/donatellopyzza/game.py` & `donatellopyzza-1.5.0/donatellopyzza/game.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from .turtleAgent import Turtle
 from .envBuilder import *
-from .generator import *
 # @DEBUG from .turtleAgent import Turtle
 # @DEBUG from .envBuilder import *
 # @DEBUG from .generator import *
 import time
 import random
 from enum import Enum
 
@@ -19,14 +18,15 @@
         member._value_ = value
         member.fullname = name
         return member
 
     def __int__(self):
         return self.value
 
+# TODO: remove duplicate in grid.py
 class Feedback(Enum):
     COLLISION = 0, "Collision"
     MOVED = 1, "Moved"
     MOVED_ON_PIZZA = 2, "Moved_on_pizza"
     TOUCHED_WALL = 3, "Touched_wall"
     TOUCHED_NOTHING = 4, "Touched_nothing"
     TOUCHED_PIZZA = 5, "Touched_pizza"
@@ -36,14 +36,17 @@
         member._value_ = value
         member.fullname = name
         return member
 
     def __int__(self):
         return self.value
 
+    def __eq__(self, fb):
+        return self.value == fb.value
+
 class Game:
     def __init__(self, envName, gui):
         self.envName = envName
         self.gui = gui
         self.env = None
         pass
 
@@ -65,13 +68,13 @@
     '''
     def isWon(self):
         res = self.env.pizzaIsFound()
         if res:
             print("-----------------------------------------------------")
             print("###                  YOU WIN                      ###")
             print("-----------------------------------------------------")
-            print("Pizza has been found with", self.nbActions, "actions !")
+            print("Pizza has been found with", self.env.nbActions, "actions !")
         return res
```

### Comparing `donatellopyzza-1.4.9/donatellopyzza/grid.py` & `donatellopyzza-1.5.0/donatellopyzza/grid/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from .map import *
-from .gui import *
-from .turn import *
+from map import *
+from gui import *
+from turn import *
 import pygame
 
 class Feedback(Enum):
     COLLISION = 0, "Collision"
     MOVED = 1, "Moved"
-    IS_ON_PIZZA = 2, "Is_on_pizza"
+    MOVED_ON_PIZZA = 2, "Moved_on_pizza"
     TOUCHED_WALL = 3, "Touched_wall"
     TOUCHED_NOTHING = 4, "Touched_nothing"
     TOUCHED_PIZZA = 5, "Touched_pizza"
 
     def __new__(cls, value, name):
         member = object.__new__(cls)
         member._value_ = value
```

### Comparing `donatellopyzza-1.4.9/donatellopyzza/gui.py` & `donatellopyzza-1.5.0/donatellopyzza/grid/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self.agentToDisplay = []
         self.height = height
         self.width = width
         self.squareWidth = 75
         self.disp = False
         self.colors = []
         self.shadeColors = []
-        path = pkg_resources.resource_filename(__name__, "data/images/pizza.png")
+        path = pkg_resources.resource_filename(__name__, "../data/images/pizza.png")
         self.pizza = pygame.image.load(path)
         for i in range(height * width):
             r = randint(15, 255)
             g = randint(0, 160)
             b = randint(0, 255)
             sr = r - 15
             self.colors.append(pygame.Color(r, g, b, 255))
```

### Comparing `donatellopyzza-1.4.9/donatellopyzza/map.py` & `donatellopyzza-1.5.0/donatellopyzza/grid/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .turn import *
-from .orientation import *
+from turn import *
+from orientation import *
 
 class Map:
     def __init__(self):
         self.num = id(self)
         self.squares = []
         self.numbAgents = 0
         self.askForReset = []
```

### Comparing `donatellopyzza-1.4.9/donatellopyzza/parser.py` & `donatellopyzza-1.5.0/donatellopyzza/grid/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from .gui import *
-from .square import *
-from .agent import *
-from .map import *
+from gui import *
+from square import *
+from agent import *
+from map import *
 import sys
 
 class Parser:
     def __init__(self, name):
-        self._name = name
+        self._name = name + ".txt"
 
     def parse(self):
         m = Map()
         
         file = open(self._name, "r") 
         lines = file.readlines()
         #Terrain
```

### Comparing `donatellopyzza-1.4.9/donatellopyzza/square.py` & `donatellopyzza-1.5.0/donatellopyzza/grid/square.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.4.9/donatellopyzza/data/images/pizza.png` & `donatellopyzza-1.5.0/donatellopyzza/data/images/pizza.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.4.9/donatellopyzza/data/images/turtle.png` & `donatellopyzza-1.5.0/donatellopyzza/data/images/turtle.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.4.9/donatellopyzza/data/images/turtle_small.png` & `donatellopyzza-1.5.0/donatellopyzza/data/images/turtle_small.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.4.9/LICENSE` & `donatellopyzza-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.4.9/README.md` & `donatellopyzza-1.5.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,29 @@
-# DonatelloPyzza
+## DonatelloPyzza
 
 A simple environment to help beginners learn Python in high school and at the university.
 A turtle can move through a grid and touch each cell until it finds the pizza.
 This game can be used at several levels:
 - for young beginners: they can hard-code a path to help the turtle find its pizza
 - for beginners: they can develop intuitive heuristics to find the pizza
 - for intermediate or advanced developers: they can develop a complex path finding method or AI-based solutions.
 
 You can manually create the grid world in which the turtle moves. Soon you will be able to generate new environements automatically through the game API.
 
-# Documentation
+![View of the game (please go to the homepage of the project to watch this gif)](https://github.com/MilowB/DonatelloPyzza/blob/master/views/example.gif)
+
+
+## Installation
+
+`pip install -r requirements.txt`
+
+`pip install donatellopyzza`
+
+
+## Getting started
 
 `Action` and `Feedback` define the different actions and feedbacks types. You can use the following actions in your code:
 
     Action.MOVE_FORWARD -> make your turtle go one step forward
     Action.TURN_RIGHT -> your turtle will turn on its right
     Action.TURN_LEFT -> on its left
     Action.TOUCH -> the turtle will touch the cell in front of it to know its type
@@ -26,14 +36,15 @@
     Feedback.MOVED_ON_PIZZA -> your turtle is on the pizza (congratulation!)
     Feedback.TOUCHED_WALL -> you just touched a wall
     Feedback.TOUCHED_NOTHING -> the touched cell is empty (no wall, no pizza, you can walk on it)
     Feedback.TOUCHED_PIZZA -> the turtle touched the pizza
 
 
 Now you know how to play, let's create the game and its environment:
+
 First, import the right modules to run the game:
 
 ```python
 from donatellopyzza import Game
 from donatellopyzza import Action
 from donatellopyzza import Feedback
 ```
@@ -57,11 +68,23 @@
 ```python
 feedback = turtle.execute(Action.FORWARD)
 print(feedback)
 ```
 
 You can use the feedback from the `execute()` method to see what happened after your action.
 
-For more details, you can find several complete examples of the game loop in the `examples` folder on the github repository for this project.
-
+For more details, you can find several complete examples of the game loop in the `examples` folder on the github repository of this project.
 
 Have fun!
+
+
+## What's new
+
+- 2023-04-07 (v1.5)
+    Integration of a maze generator from Alexandru Văleanu (https://github.com/AlexandruValeanu/Mazify)
+- 2023-01-17 (v1.2)
+    Initial release
+
+
+## Roadmap
+
+- ~~add a gridworld generator~~
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `donatellopyzza-1.4.9/pyproject.toml` & `donatellopyzza-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DonatelloPyzza"
-version = "1.4.9"
+version = "1.5.0"
 authors = [
   { name="Mickaël Bettinelli", email="mickael.bettinelli@univ-smb.fr" },
 ]
 description = "A simple grid environment to learn Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `donatellopyzza-1.4.9/PKG-INFO` & `donatellopyzza-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 Metadata-Version: 2.1
 Name: DonatelloPyzza
-Version: 1.4.9
+Version: 1.5.0
 Summary: A simple grid environment to learn Python
 Project-URL: Homepage, https://github.com/MilowB/Donatello
 Project-URL: Bug Tracker, https://github.com/MilowB/Donatello/pulls
 Author-email: Mickaël Bettinelli <mickael.bettinelli@univ-smb.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# DonatelloPyzza
+## DonatelloPyzza
 
 A simple environment to help beginners learn Python in high school and at the university.
 A turtle can move through a grid and touch each cell until it finds the pizza.
 This game can be used at several levels:
 - for young beginners: they can hard-code a path to help the turtle find its pizza
 - for beginners: they can develop intuitive heuristics to find the pizza
 - for intermediate or advanced developers: they can develop a complex path finding method or AI-based solutions.
 
 You can manually create the grid world in which the turtle moves. Soon you will be able to generate new environements automatically through the game API.
 
-# Documentation
+![View of the game (please go to the homepage of the project to watch this gif)](https://github.com/MilowB/DonatelloPyzza/blob/master/views/example.gif)
+
+
+## Installation
+
+`pip install -r requirements.txt`
+
+`pip install donatellopyzza`
+
+
+## Getting started
 
 `Action` and `Feedback` define the different actions and feedbacks types. You can use the following actions in your code:
 
     Action.MOVE_FORWARD -> make your turtle go one step forward
     Action.TURN_RIGHT -> your turtle will turn on its right
     Action.TURN_LEFT -> on its left
     Action.TOUCH -> the turtle will touch the cell in front of it to know its type
@@ -40,14 +50,15 @@
     Feedback.MOVED_ON_PIZZA -> your turtle is on the pizza (congratulation!)
     Feedback.TOUCHED_WALL -> you just touched a wall
     Feedback.TOUCHED_NOTHING -> the touched cell is empty (no wall, no pizza, you can walk on it)
     Feedback.TOUCHED_PIZZA -> the turtle touched the pizza
 
 
 Now you know how to play, let's create the game and its environment:
+
 First, import the right modules to run the game:
 
 ```python
 from donatellopyzza import Game
 from donatellopyzza import Action
 from donatellopyzza import Feedback
 ```
@@ -71,11 +82,23 @@
 ```python
 feedback = turtle.execute(Action.FORWARD)
 print(feedback)
 ```
 
 You can use the feedback from the `execute()` method to see what happened after your action.
 
-For more details, you can find several complete examples of the game loop in the `examples` folder on the github repository for this project.
-
+For more details, you can find several complete examples of the game loop in the `examples` folder on the github repository of this project.
 
 Have fun!
+
+
+## What's new
+
+- 2023-04-07 (v1.5)
+    Integration of a maze generator from Alexandru Văleanu (https://github.com/AlexandruValeanu/Mazify)
+- 2023-01-17 (v1.2)
+    Initial release
+
+
+## Roadmap
+
+- ~~add a gridworld generator~~
```

