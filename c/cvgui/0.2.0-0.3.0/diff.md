# Comparing `tmp/cvgui-0.2.0.tar.gz` & `tmp/cvgui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvgui-0.2.0.tar", last modified: Fri Mar 31 20:35:57 2023, max compression
+gzip compressed data, was "cvgui-0.3.0.tar", last modified: Fri Apr  7 16:51:00 2023, max compression
```

## Comparing `cvgui-0.2.0.tar` & `cvgui-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,51 @@
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.843110 cvgui-0.2.0/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1073 2022-10-14 02:32:32.000000 cvgui-0.2.0/LICENSE.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      393 2023-03-31 20:35:57.843110 cvgui-0.2.0/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3550 2023-03-30 18:20:51.000000 cvgui-0.2.0/README.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.831110 cvgui-0.2.0/cvgui/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3754 2023-03-30 18:20:51.000000 cvgui-0.2.0/cvgui/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.839110 cvgui-0.2.0/cvgui/activity/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      481 2022-10-18 03:28:55.000000 cvgui-0.2.0/cvgui/activity/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5460 2023-03-31 20:35:52.000000 cvgui-0.2.0/cvgui/activity/activity.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      738 2023-03-31 20:35:52.000000 cvgui-0.2.0/cvgui/activity/scene.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.839110 cvgui-0.2.0/cvgui/core/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      825 2023-03-31 20:35:52.000000 cvgui-0.2.0/cvgui/core/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.839110 cvgui-0.2.0/cvgui/core/displaying/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      391 2023-03-31 20:35:52.000000 cvgui-0.2.0/cvgui/core/displaying/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6925 2023-03-31 20:35:52.000000 cvgui-0.2.0/cvgui/core/displaying/components.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1456 2023-03-31 20:35:52.000000 cvgui-0.2.0/cvgui/core/displaying/service.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.839110 cvgui-0.2.0/cvgui/core/recieving/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      370 2022-10-18 03:28:55.000000 cvgui-0.2.0/cvgui/core/recieving/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3127 2023-03-30 18:00:12.000000 cvgui-0.2.0/cvgui/core/recieving/service.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.839110 cvgui-0.2.0/cvgui/inputs/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      142 2022-10-14 21:28:10.000000 cvgui-0.2.0/cvgui/inputs/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.843110 cvgui-0.2.0/cvgui/inputs/computer_vision/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      218 2022-10-18 03:28:55.000000 cvgui-0.2.0/cvgui/inputs/computer_vision/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3195 2023-03-30 18:00:12.000000 cvgui-0.2.0/cvgui/inputs/computer_vision/computer_vision.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.843110 cvgui-0.2.0/cvgui/inputs/computer_vision/cv_model/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      105 2022-10-15 15:36:20.000000 cvgui-0.2.0/cvgui/inputs/computer_vision/cv_model/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2826 2023-03-30 18:00:12.000000 cvgui-0.2.0/cvgui/inputs/computer_vision/cv_model/blazepose.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.843110 cvgui-0.2.0/cvgui/inputs/computer_vision/frame_input/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       80 2022-10-15 15:36:20.000000 cvgui-0.2.0/cvgui/inputs/computer_vision/frame_input/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1367 2023-03-30 18:00:12.000000 cvgui-0.2.0/cvgui/inputs/computer_vision/frame_input/webcam.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.843110 cvgui-0.2.0/cvgui/inputs/mocap/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       65 2022-10-15 15:36:20.000000 cvgui-0.2.0/cvgui/inputs/mocap/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2022-10-14 02:32:32.000000 cvgui-0.2.0/cvgui/inputs/mocap/mocap_input.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.843110 cvgui-0.2.0/cvgui/user_interface/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      182 2023-03-31 20:35:52.000000 cvgui-0.2.0/cvgui/user_interface/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.843110 cvgui-0.2.0/cvgui/user_interface/pygame_ui/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2022-10-14 02:32:32.000000 cvgui-0.2.0/cvgui/user_interface/pygame_ui/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6775 2023-03-31 20:35:52.000000 cvgui-0.2.0/cvgui/user_interface/pygame_ui/pygame.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-03-31 20:35:57.835110 cvgui-0.2.0/cvgui.egg-info/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      393 2023-03-31 20:35:57.000000 cvgui-0.2.0/cvgui.egg-info/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      972 2023-03-31 20:35:57.000000 cvgui-0.2.0/cvgui.egg-info/SOURCES.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-03-31 20:35:57.000000 cvgui-0.2.0/cvgui.egg-info/dependency_links.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       96 2023-03-31 20:35:57.000000 cvgui-0.2.0/cvgui.egg-info/requires.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-03-31 20:35:57.000000 cvgui-0.2.0/cvgui.egg-info/top_level.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      107 2023-03-31 20:35:57.843110 cvgui-0.2.0/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1022 2023-03-31 20:35:52.000000 cvgui-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.734373 cvgui-0.3.0/
+-rw-rw-rw-   0        0        0     1094 2023-03-28 14:37:35.000000 cvgui-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      386 2023-04-07 16:51:00.734373 cvgui-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2897 2023-04-07 16:50:32.000000 cvgui-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.678373 cvgui-0.3.0/cvgui/
+-rw-rw-rw-   0        0        0      376 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.705374 cvgui-0.3.0/cvgui/activity/
+-rw-rw-rw-   0        0        0      494 2023-03-28 14:37:35.000000 cvgui-0.3.0/cvgui/activity/__init__.py
+-rw-rw-rw-   0        0        0     6826 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/activity/activity.py
+-rw-rw-rw-   0        0        0      831 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/activity/scene.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.706376 cvgui-0.3.0/cvgui/core/
+-rw-rw-rw-   0        0        0      889 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.710372 cvgui-0.3.0/cvgui/core/displaying/
+-rw-rw-rw-   0        0        0      356 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/displaying/__init__.py
+-rw-rw-rw-   0        0        0     7695 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/displaying/components.py
+-rw-rw-rw-   0        0        0     2857 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/displaying/service.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.713372 cvgui-0.3.0/cvgui/core/logging/
+-rw-rw-rw-   0        0        0      252 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/logging/__init__.py
+-rw-rw-rw-   0        0        0      831 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/logging/service.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.715372 cvgui-0.3.0/cvgui/core/receiving/
+-rw-rw-rw-   0        0        0      370 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/receiving/__init__.py
+-rw-rw-rw-   0        0        0     3508 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/receiving/service.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.716376 cvgui-0.3.0/cvgui/inputs/
+-rw-rw-rw-   0        0        0      148 2023-03-28 14:37:35.000000 cvgui-0.3.0/cvgui/inputs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.719375 cvgui-0.3.0/cvgui/inputs/computer_vision/
+-rw-rw-rw-   0        0        0      400 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/__init__.py
+-rw-rw-rw-   0        0        0     3557 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/computer_vision.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.721373 cvgui-0.3.0/cvgui/inputs/computer_vision/cv_model/
+-rw-rw-rw-   0        0        0      103 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/cv_model/__init__.py
+-rw-rw-rw-   0        0        0     3422 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/cv_model/blazepose.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.724373 cvgui-0.3.0/cvgui/inputs/computer_vision/frame_input/
+-rw-rw-rw-   0        0        0       78 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/frame_input/__init__.py
+-rw-rw-rw-   0        0        0     1495 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/frame_input/webcam.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.725374 cvgui-0.3.0/cvgui/outputs/
+-rw-rw-rw-   0        0        0      133 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/outputs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.728374 cvgui-0.3.0/cvgui/outputs/loggers/
+-rw-rw-rw-   0        0        0      178 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/outputs/loggers/__init__.py
+-rw-rw-rw-   0        0        0     3809 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/outputs/loggers/csv_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.729373 cvgui-0.3.0/cvgui/user_interface/
+-rw-rw-rw-   0        0        0      190 2023-04-07 15:07:31.000000 cvgui-0.3.0/cvgui/user_interface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.732373 cvgui-0.3.0/cvgui/user_interface/pygame_ui/
+-rw-rw-rw-   0        0        0      150 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/user_interface/pygame_ui/__init__.py
+-rw-rw-rw-   0        0        0     8951 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/user_interface/pygame_ui/pygame.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.701375 cvgui-0.3.0/cvgui.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-04-07 16:51:00.000000 cvgui-0.3.0/cvgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1064 2023-04-07 16:51:00.000000 cvgui-0.3.0/cvgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 16:51:00.000000 cvgui-0.3.0/cvgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-04-07 16:51:00.000000 cvgui-0.3.0/cvgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-07 16:51:00.000000 cvgui-0.3.0/cvgui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-04-07 16:51:00.735375 cvgui-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-04-07 16:50:32.000000 cvgui-0.3.0/setup.py
```

### Comparing `cvgui-0.2.0/README.md` & `cvgui-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,108 @@
-# cvgui
-
-`cvgui` is a library for creating body-interactive GUIs using computer
-vison.
-
-Documentation can be [found here](https://mitchellss.github.io/cvgui).
-
-
-**cvgui is a prototype. No guarantees can
-be made about the stability of the API or the library itself.**
-
-
-## Installation
-
-> pip install cvgui
-
-Requires Python 3.9 or later
-
-## Contributing
-
-Pull requests are welcome. Please see the [contributing guide](CONTRIBUTING.md) for more information.
-
-To begin development, first ensure that your python version is 3.9 or greater by running:
-> python --version
-
-Then, create a virtual environment...
-
-Windows:
-
-> python -m venv env
->
-> ./env/Scripts/activate
-
-Linux:
-
-> python -m venv env
->
-> source ./env/bin/activate
-
-And install the package in editable mode by running:
-
-> pip install -e .
-
-(The -e option makes it so any changes you make to the package are reflected
-at runtime and you don't have to re-install the package every time)
-
-To test and see if everything worked correctly, make sure you have a webcam plugged in and run:
-
-> python ./bin/examples/working_example.py
-
-To run the test program.
-
-## Example Program
-
-This example creates a simple activity with a skeleton and a button.
-When clicked, the button moves. Example programs can be found in the
-`bin/examples` directory.
-
-```python
-from random import randrange
-import cvgui
-
-WINDOW_WIDTH = 1280
-WINDOW_HEIGHT = 720
-WINDOW_FPS = 60
-
-# This name == main line is required for windows multiprocessing
-if __name__ == "__main__":
-
-    # Specify input as a webcam and computer vision model as blazepose
-    frame_input: cvgui.FrameInput = cvgui.Webcam(device_num=0, fps=30)
-    cv_model: cvgui.CVModel = cvgui.BlazePose()
-
-    # Create a pose generator based on a webcam + blazepose
-    pose_input: cvgui.PoseGenerator = cvgui.ComputerVisionPose(
-        frame_input=frame_input, model=cv_model)
-
-    # Specify GUI to be pygame
-    ui: cvgui.UserInterface = cvgui.PyGameUI(
-        width=WINDOW_WIDTH, height=WINDOW_HEIGHT, fps=WINDOW_FPS)
-
-    # Create activity
-    activity = cvgui.Activity(pose_input=pose_input, frontend=ui)
-
-    # Create a new scene
-    scene_1 = cvgui.Scene()
-    activity.add_scene(scene_1)
-
-    # Create a new button
-    button_1: cvgui.Button = cvgui.button(gui=ui,
-                                          pos=(WINDOW_WIDTH//2,
-                                               WINDOW_HEIGHT//2),
-                                          activation_distance=50,
-                                          color=(255, 0, 0, 255),
-                                          radius=50)
-
-    def callback(button: cvgui.Button) -> None:
-        '''
-        Define what the button should do when clicked.
-        In this case, randomly set a new button position
-        and randomly select a new color.
-        '''
-        button.pos = (randrange(600, 1000, 20), randrange(200, 600, 20))
-        button.color = (randrange(0, 255, 1), randrange(0, 255, 1),
-                        randrange(0, 255, 1), 255)
-
-    # Set the button to be clicked using the user's left or right hand
-    button_1.targets = [cv_model.LEFT_HAND, cv_model.RIGHT_HAND]
-
-    # Link the callback function to the button
-    button_1.callback = lambda: callback(button_1)
-
-    # Create a skeleton to map pose points to
-    skeleton: cvgui.Skeleton = cvgui.skeleton(
-        gui=ui, pos=(800, 600), scale=cv_model.DEFAULT_SCALE)
-
-    # Add the skeleton and button to the scene
-    scene_1.add_component(button_1)
-    scene_1.add_component(skeleton)
-
-    # Start activity
-    activity.run()
-```
+# cvgui
+
+`cvgui` is a library for creating body-interactive GUIs using computer
+vison.
+
+**cvgui is a prototype. No guarantees can
+be made about the stability of the API or the library itself.**
+
+
+## Installation
+
+```shell
+pip install cvgui
+```
+
+Requires Python 3.10
+
+## Usage
+
+```shell
+python ./my_activity.py
+```
+See the documentation [here](https://mitchellss.github.io/cvgui) for more information
+on how to create your own activities.
+
+## Contributing
+
+Pull requests are welcome. Please see the [contributing guide](CONTRIBUTING.md) for more information.
+
+
+## Example Program
+
+This example creates a simple activity with a skeleton and a button.
+When clicked, the button moves and changes color. Other example programs 
+can be found in the `bin/examples` directory.
+
+```python
+from random import randrange
+import cvgui
+
+WINDOW_WIDTH = 1280
+WINDOW_HEIGHT = 720
+WINDOW_FPS = 60
+
+
+def main():
+    # Specify input as a webcam and computer vision model as blazepose
+    frame_input = cvgui.Webcam(device_num=0, fps=30)
+    cv_model = cvgui.BlazePose()
+
+    # Create a pose generator based on a webcam + blazepose
+    pose_input = cvgui.ComputerVisionPose(
+        frame_input=frame_input, model=cv_model)
+
+    # Specify GUI to be pygame
+    ui = cvgui.PyGameUI(width=WINDOW_WIDTH,
+                        height=WINDOW_HEIGHT, fps=WINDOW_FPS)
+
+    # Create activity
+    activity = cvgui.Activity(pose_input=pose_input, frontend=ui)
+
+    # Create a new scene
+    scene_1 = cvgui.Scene()
+    activity.add_scene(scene_1)
+
+    # Create a new button
+    button_1 = cvgui.button(
+        gui=ui,
+        pos=(WINDOW_WIDTH//2,
+             WINDOW_HEIGHT//2),
+        activation_distance=50,
+        color=(255, 0, 0, 255),
+        radius=50
+    )
+
+    def callback() -> None:
+        '''
+        Define what the button should do when clicked.
+        In this case, randomly set a new button position
+        and randomly select a new color.
+        '''
+        button_1.pos = (randrange(600, 1000, 20), randrange(200, 600, 20))
+        button_1.color = (randrange(0, 255, 1), randrange(0, 255, 1),
+                          randrange(0, 255, 1), 255)
+
+    # Set the button to be clicked using the user's left or right hand
+    button_1.targets = [cv_model.LEFT_HAND, cv_model.RIGHT_HAND]
+
+    # Link the callback function to the button
+    button_1.callback = callback
+
+    # Create a skeleton to map pose points to
+    skeleton = cvgui.skeleton(gui=ui, pos=(
+        800, 600), scale=cv_model.DEFAULT_SCALE)
+
+    # Add the skeleton and button to the scene
+    scene_1.add_component(button_1)
+    scene_1.add_component(skeleton)
+
+    # Start activity
+    activity.run()
+
+
+# Everything must be run under "__name__ == __main__"
+# for windows multiprocessing
+if __name__ == "__main__":
+    main()
+```
```

### Comparing `cvgui-0.2.0/cvgui/core/__init__.py` & `cvgui-0.3.0/cvgui/core/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-"""
-Interfaces that describe abstract component functionality.
-
-The `core` package breaks down the program into its fundamental
-functionality and defines an interface for each function. If
-a concrete class is able to fulfill said interface, it can
-therefore be considered fit to fulfill the requirements of
-that function. For instance, both a MOCAP system and a
-computer vision + camera combo can provide a set of points
-when called upon that represent a human figure. These systems
-therefore fulfill the requirements of the `recieving` core
-package and could theoretically be implemented as core classes.
-"""
-from .displaying import (  # noqa
-    UserInterface,
-    skeleton,
-    button,
-    tracking_bubble,
-    Skeleton,
-    Button,
-    TrackingBubble
-  )
-from .recieving import CVModel, FrameInput, PoseGenerator  # noqa
+"""
+Interfaces that describe abstract component functionality.
+
+The `core` package breaks down the program into its fundamental
+functionality and defines an interface for each function. If
+a concrete class is able to fulfill said interface, it can
+therefore be considered fit to fulfill the requirements of
+that function. For instance, both a MOCAP system and a
+computer vision + camera combo can provide a set of points
+when called upon that represent a human figure. These systems
+therefore fulfill the requirements of the `receiving` core
+package and could theoretically be implemented as core classes.
+"""
+from .displaying import (  # noqa
+    UserInterface,
+    skeleton,
+    button,
+    tracking_bubble,
+    Skeleton,
+    Button,
+    TrackingBubble
+  )
+from .receiving import CVModel, FrameInput, PoseGenerator  # noqa
+from .logging import PoseLogger  # noqa
```

### Comparing `cvgui-0.2.0/cvgui/core/displaying/service.py` & `cvgui-0.3.0/cvgui/core/displaying/service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,83 @@
-"""The interface to implement to be considered a user interface."""
-from typing import Any, Tuple
-from typing_extensions import Protocol
-
-from cvgui.core.displaying.components import Button, Skeleton, TrackingBubble
-
-
-class UserInterface(Protocol):
-    """An abstract user interface capable of rendering components."""
-    window: Any
-    running: bool
-
-    def clear(self) -> None:
-        """Resets the user interface display."""
-
-    def new_gui(self) -> None:
-        """Sets up the user interface."""
-
-    def button(self, pos: Tuple[float, float],
-               activation_distance: float,
-               color: Tuple[int, int, int, int],
-               radius: int) -> Button:  # type: ignore
-        """
-        Creates a new button on the user
-        interface at the location specfied.
-        """
-
-    def skeleton(self, pos: Tuple[float, float],
-                 scale: int) -> Skeleton:  # type: ignore
-        """
-        Creates a new skeleton on the user
-        interface at the location specfied.
-        """
-
-    def tracking_bubble(self,
-                        target: int,
-                        color: Tuple[int, int, int, int],
-                        radius: int
-                        ) -> TrackingBubble:  # type: ignore
-        """
-        Creates a new tracking bubble on the user
-        interface that tracks the given point.
-        """
-
-    def update(self) -> None:
-        """Refreshes the user interface display."""
+"""This module defines the interface for a class to be considered \
+a user interface by `cvgui`. This ensures that all user-created \
+activities work reguardless of what user interface is used."""
+from typing import Any, Tuple
+from typing_extensions import Protocol
+
+from cvgui.core.displaying.components import Button, Skeleton, TrackingBubble
+
+
+class UserInterface(Protocol):
+    """An abstract user interface capable of rendering components."""
+
+    window: Any
+    """The window to render componets onto."""
+
+    running: bool
+    """Whether the user interface should continue rendering."""
+
+    def clear(self) -> None:
+        """Reset the user interface display."""
+
+    def new_gui(self) -> None:
+        """Set up the user interface."""
+
+    def button(self, pos: Tuple[float, float],
+               activation_distance: float,
+               color: Tuple[int, int, int, int],
+               radius: int) -> Button:  # type: ignore
+        """Create a circular button on the user \
+        interface.
+
+        Args:
+            pos (Tuple[float, float]): The coordinates \
+                to render the button at.
+            activation_distance (float): The distance \
+                from the target to the button to be \
+                    considered a click.
+            color (Tuple[int, int, int, int]): The color \
+                of the button.
+            radius (int): The radius of the button \
+
+        Returns:
+            Button: Button component with the specified settings.
+        """
+
+    def skeleton(self, pos: Tuple[float, float],
+                 scale: int) -> Skeleton:  # type: ignore
+        """Create a new skeleton on the user \
+        interface at the location specfied.
+
+        Args:
+            pos (Tuple[float, float]): The coordinates \
+                to center the skeleton at.
+            scale (int): How much to scale the skeleton \
+                points by.
+
+        Returns:
+            Skeleton: Skeleton component with the specified settings.
+        """
+
+    def tracking_bubble(
+        self,
+        target: int,
+        color: Tuple[int, int, int, int],
+        radius: int
+    ) -> TrackingBubble:  # type: ignore
+        """Create a new tracking bubble on the user \
+        interface that tracks the given point.
+
+        Args:
+            target (int): Index of the skeleton point that the \
+                tracking bubble should follow.
+            color (Tuple[int, int, int, int]): The color of the \
+                tracking bubble.
+            radius (int): The radius of the tracking bubble.
+
+        Returns:
+            TrackingBubble: TrackingBubble component with the \
+                specified settings.
+        """
+
+    def update(self) -> None:
+        """Refresh the user interface display."""
```

### Comparing `cvgui-0.2.0/cvgui/inputs/computer_vision/computer_vision.py` & `cvgui-0.3.0/cvgui/inputs/computer_vision/computer_vision.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,87 @@
-"""Generates poses based on a computer vision model and a frame input."""
-import cv2
-import numpy as np
-import multiprocessing as mp
-from cvgui.core.recieving.service import CVModel, FrameInput
-
-
-class ComputerVisionPose:
-    """Generates poses based on a computer vision model and a frame input."""
-
-    def __init__(self, frame_input: FrameInput, model: CVModel):
-        """Creates a new pose generator based on a computer vision
-        model.
-
-        Args:
-            frame_input (FrameInput): The input of images to the computer
-            vision model.
-            model (CVModel): The model use to interpret the images from
-            the frame input.
-        """
-        self.frame_input: FrameInput = frame_input
-        self.model: CVModel = model
-
-    def start(self, skeleton_queue: mp.Queue):
-        """
-        Starts two processes, one for capturing/displaying frame input data and
-        one for processing that frame input data to get skeletons out of them.
-        These are done as separate processes because otherwise the skeleton
-        processing greatly slows down the speed at which frames are collected,
-        resulting in video feedback that is "laggy".
-
-        Args:
-            skeleton_queue (multiprocessing.Queue): The queue to put skeleton
-                data into once it has been processed from frames.
-
-        Returns:
-            list[multiprocessing.Process]: All the processes started by this 
-                method so they can be closed correctly later down the line.
-        """
-        image_queue: mp.Queue = mp.Queue()
-        print("Starting image processing pipeline "
-              "(This might take a while on Windows)...")
-        cap = mp.Process(target=self.capture_and_show, args=(image_queue,))
-        proc = mp.Process(target=self.process_image,
-                          args=(image_queue, skeleton_queue))
-        cap.start()
-        proc.start()
-        return [cap, proc]
-
-    def capture_and_show(self, image_queue):
-        """
-        Infinitely retrieves new frames and places them in the image
-        queue. Additionally, displays incoming frames to the user in
-        real-time.
-        """
-        while True:
-            frame = self.frame_input.get_frame()
-            image_queue.put(frame)
-            cv2.imshow("Video Input", frame)
-            wait_key = cv2.waitKey(1)
-            if wait_key == 27:
-                pass
-
-    def process_image(self, image_queue, skeleton_queue):
-        """
-        Infinitely takes images from the given queue and turns them into 
-        skeleton data using a computer vision model.
-        """
-        while True:
-            if image_queue.empty():
-                continue
-            skeleton = self.model.get_pose(image_queue.get())
-            skeleton_queue.put(skeleton)
-
-    def get_pose(self) -> np.ndarray:
-        """Uses the frame input and computer vision model in tandem
-        to generate a single pose."""
-        frame: np.ndarray = self.frame_input.get_frame()
-        # Shaves about 5ms off each frame by passing by reference, not value
-        frame.flags.writeable = False
-        pose: np.ndarray = self.model.get_pose(frame)
-        return pose
+"""The computer_vision module contains the main ComputerVisionPose class \
+    that dictates the interactions between frame inputs and computer \
+        vision models."""
+from typing import Any, Iterable
+import multiprocessing as mp
+import multiprocessing.queues as mpq
+import cv2
+import numpy as np
+from cvgui.core.receiving.service import CVModel, FrameInput
+
+
+class ComputerVisionPose:
+    """Generates poses based on a computer vision model and a frame input."""
+
+    def __init__(self, frame_input: FrameInput, model: CVModel) -> None:
+        """Create a new pose generator based on a computer vision \
+        model.
+
+        Args:
+            frame_input (FrameInput): The input of images \
+            to the computer vision model.
+            model (CVModel): The model use to interpret the images \
+            from the frame input.
+        """
+        self.frame_input: FrameInput = frame_input
+        self.model: CVModel = model
+
+    def start(self, pose_queues: Iterable[mpq.Queue]) -> Iterable[mp.Process]:
+        """Start two processes, one for \
+        capturing/displaying frame input data and \
+        one for processing that frame input \
+        data to get poses out of them.
+
+        These are done as separate processes \
+        because otherwise the pose \
+        processing greatly slows down the \
+        speed at which frames are collected, \
+        resulting in video feedback that is "laggy".
+
+        Args:
+            pose_queue (multiprocessing.Queue): The queue to put pose \
+                data into once it has been processed from frames.
+
+        Returns:
+            list[multiprocessing.Process]: All the processes started by this \
+                method so they can be closed correctly later down the line.
+        """
+        image_queue: mpq.Queue = mp.Queue()
+        print("Starting image processing pipeline "
+              "(This might take a while on Windows)...")
+        cap = mp.Process(target=self._capture_and_show, args=(image_queue,))
+        proc = mp.Process(target=self._process_image,
+                          args=(image_queue, pose_queues))
+        cap.start()
+        proc.start()
+        return [cap, proc]
+
+    def _capture_and_show(self, image_queue) -> None:
+        """Infinitely retrieve new frames and place them in the image \
+        queue. Additionally, display incoming frames to the user in \
+        real-time."""
+        while True:
+            frame: np.ndarray = self.frame_input.get_frame()
+            image_queue.put(frame)
+            cv2.imshow("Video Input", frame)
+            wait_key: Any = cv2.waitKey(1)
+            if wait_key == 27:
+                pass
+
+    def _process_image(self, image_queue, pose_queues) -> None:
+        """Infinitely take images from the given queue and turn them into \
+        pose data using a computer vision model."""
+        while True:
+            if image_queue.empty():
+                continue
+            skeleton: np.ndarray = self.model.get_pose(image_queue.get())
+            for queue in pose_queues:
+                queue.put(skeleton)
+
+    def get_pose(self) -> np.ndarray:
+        """Use the frame input and computer vision model in tandem \
+        to generate a single pose."""
+        frame: np.ndarray = self.frame_input.get_frame()
+        # Shaves about 5ms off each frame by passing by reference, not value
+        frame.flags.writeable = False
+        pose: np.ndarray = self.model.get_pose(frame)
+        return pose
```

### Comparing `cvgui-0.2.0/cvgui/inputs/computer_vision/frame_input/webcam.py` & `cvgui-0.3.0/cvgui/inputs/computer_vision/frame_input/webcam.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-"""FrameInput implementation for a computer webcam."""
-from typing import Any
-import numpy as np
-import cv2
-
-
-class Webcam:
-    """FrameInput implementation for a computer webcam."""
-
-    def __init__(self, device_num: int, fps: int) -> None:
-        """Creates a new webcam frame input.
-
-        Args:
-            device_num (int): The device number of the webcam. Try 0 if unsure.
-            fps (int): The frames per second the webcam can provide.
-        """
-        self.device_num = device_num
-        self.fps = fps
-        self.cap: cv2.VideoCapture = None
-
-    def _configure(self) -> None:
-        """
-        Creates and configures the capture object. 
-
-        This cannot be done in the init function because of how 
-        Windows handles multiprocessing.
-        """
-        self.cap = cv2.VideoCapture(self.device_num)
-        self.cap.set(cv2.CAP_PROP_FPS, self.fps)
-        self.cap.set(cv2.CAP_PROP_FOURCC,
-                     cv2.VideoWriter_fourcc("M", "J", "P", "G"))
-
-    def get_frame(self) -> np.ndarray:
-        """Gets a frame from the webcam."""
-        if self.cap is None:
-            self._configure()
-
-        success: bool
-        color_image: np.ndarray
-        success, color_image = self.cap.read()
-        if not success:
-            return np.zeros(0)
-        color_image = cv2.flip(color_image, 1)
-        return color_image
+"""FrameInput implementation for a computer webcam."""
+import numpy as np
+import cv2
+
+
+class Webcam:
+    """Captures data from a camera connected to the computer."""
+
+    def __init__(self, device_num: int, fps: int) -> None:
+        """Object for capturing data from a camera connected to the computer.
+
+        Args:
+            device_num (int): The device number of the webcam. Generally this \
+                will be zero if there are no other webcams connected.
+            fps (int): The frames per second the webcam can provide.
+        """
+        self.device_num = device_num
+        self.fps = fps
+        self.cap: cv2.VideoCapture = None
+
+    def _configure(self) -> None:
+        """
+        Create and configures the capture object.
+
+        This cannot be done in the init function because of how \
+        Windows handles multiprocessing.
+        """
+        self.cap = cv2.VideoCapture(self.device_num)
+        self.cap.set(cv2.CAP_PROP_FPS, self.fps)
+        self.cap.set(cv2.CAP_PROP_FOURCC,
+                     cv2.VideoWriter_fourcc("M", "J", "P", "G"))
+
+    def get_frame(self) -> np.ndarray:
+        """Get a frame from the webcam."""
+        if self.cap is None:
+            self._configure()
+
+        success: bool
+        color_image: np.ndarray
+        success, color_image = self.cap.read()
+        if not success:
+            return np.zeros(0)
+        color_image = cv2.flip(color_image, 1)
+        return color_image
```

### Comparing `cvgui-0.2.0/cvgui/user_interface/pygame_ui/pygame.py` & `cvgui-0.3.0/cvgui/user_interface/pygame_ui/pygame.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,189 +1,245 @@
-"""User interface implementation of PyGame."""
-from cvgui.core.displaying.components import Button, Skeleton, TrackingBubble
-import numpy as np
-from pygame.constants import QUIT
-import pygame
-import math
-from typing import Any, Callable, List, Literal, Tuple
-
-X = 0
-Y = 1
-
-
-class PyGameUI:
-    """User interface implementation of PyGame."""
-    BACKGROUND: tuple[Literal[0], Literal[0], Literal[0]] = (0, 0, 0)
-
-    window: pygame.surface.Surface
-    fps_clock: pygame.time.Clock
-    running: bool
-
-    def __init__(self, height: int, width: int, fps: int) -> None:
-        self.width: int = width
-        self.height: int = height
-        self.fps: int = fps
-
-    def clear(self) -> None:
-        """Clears the pygame window by filling it with
-        a single color."""
-        self.window.fill(self.BACKGROUND)
-
-    def update(self) -> None:
-        """Updates the PyGame window."""
-        pygame.display.update()
-        self.fps_clock.tick(self.fps)
-
-        for event in pygame.event.get():
-            if event.type == QUIT:
-                pygame.quit()
-                self.running = False
-
-    def button(self, pos: Tuple[float, float],
-               activation_distance: float,
-               color: Tuple[int, int, int, int],
-               radius: int = 100) -> Button:
-        """Creates a PyGame button at the specified location."""
-        return PyGameButton(pos=pos, activation_distance=activation_distance,
-                            color=color, radius=radius)
-
-    def skeleton(self, pos: Tuple[float, float], scale: int) -> Skeleton:
-        """Creates a PyGame skeleton at the specified location."""
-        return PyGameSkeleton(pos=pos, scale=scale)
-
-    def tracking_bubble(self,
-                        target: int,
-                        color: Tuple[int, int, int, int],
-                        radius: int = 100
-                        ) -> TrackingBubble:
-        return PyGameTrackingBubble(color=color, target=target, radius=radius)
-
-    def new_gui(self) -> None:
-        """Initializes the PyGame user interface."""
-        pygame.init()
-        pygame.font.init()
-
-        # Game Setup
-        self.fps_clock = pygame.time.Clock()
-
-        self.window: pygame.surface.Surface = pygame.display.set_mode(
-            (self.width, self.height))
-        pygame.display.set_caption("cvgui")
-        self.window.fill(self.BACKGROUND)
-        self.running = True
-
-
-class PyGameTrackingBubble:
-
-    def __init__(self,
-                 color: Tuple[int, int, int, int],
-                 radius: int,
-                 target: int) -> None:
-        self.color = color
-        self.radius = radius
-        self.target = target
-        self.pos: Tuple[float, float] = (0, 0)
-
-    def render(self, window: Any) -> None:
-        color = pygame.color.Color(
-            self.color[0], self.color[1],
-            self.color[2], self.color[3])
-        pygame.draw.circle(
-            window, color,
-            (self.pos[X], self.pos[Y]),
-            self.radius
-        )
-
-
-class PyGameButton:
-    """Button implementation for PyGame."""
-
-    def __init__(self, pos: Tuple[float, float],
-                 activation_distance: float,
-                 color: Tuple[int, int, int, int],
-                 radius: int) -> None:
-        """Creates a new PyGameButton at the location specified."""
-        self.pos = pos
-        self.activation_distance: float = activation_distance
-        self.targets: List[int]
-        self.callback: Callable
-        self.color: Tuple[int, int, int, int] = color
-        self.radius: int = radius
-
-    def is_clicked(self, pos: Tuple[float, float]) -> bool:
-        """Checks if the button has been clicked."""
-        if abs(self.pos[X] - pos[X]) > self.activation_distance \
-                or abs(self.pos[Y] - pos[Y]) > self.activation_distance:
-            return False
-        if math.sqrt((self.pos[X] - pos[X])**2 + (self.pos[Y] - pos[Y])**2) \
-                > self.activation_distance:
-            return False
-        return True
-
-    def render(self, window) -> None:
-        """Draws the button on the pygame window."""
-        color = pygame.color.Color(
-            self.color[0], self.color[1],
-            self.color[2], self.color[3])
-        pygame.draw.circle(
-            window, color,
-            (self.pos[X], self.pos[Y]),
-            self.radius
-        )
-
-
-class PyGameSkeleton:
-    """Skeleton implementation in PyGame."""
-
-    # Where to connect limbs. Refer to here
-    # https://mediapipe.dev/images/mobile/pose_tracking_full_body_landmarks.png
-    # TODO: Move this somewhere else
-    CONNECTIONS: np.ndarray = np.array([
-        [16, 14], [16, 18], [16, 20], [16, 22],
-        [18, 20], [14, 12], [12, 11], [12, 24],
-        [11, 23], [11, 13], [15, 13], [15, 17],
-        [15, 19], [15, 21], [17, 19], [24, 23],
-        [26, 24], [26, 28], [25, 23], [25, 27],
-        [10, 9], [8, 6], [5, 6], [5, 4], [0, 4],
-        [0, 1], [2, 1], [2, 3], [3, 7], [28, 32],
-        [28, 30], [27, 29], [27, 31], [32, 30],
-        [29, 31]
-    ])
-
-    LIMB_COLOR: tuple[Literal[255], Literal[255],
-                      Literal[255]] = (255, 255, 255)
-    LIMB_WIDTH: Literal[2] = 2
-
-    LANDMARK_COLOR: tuple[Literal[0], Literal[255], Literal[0]] = (0, 255, 0)
-    LANDMARK_RADIUS: Literal[5] = 5
-    LANDMARK_OUTLINE_WIDTH: Literal[0] = 0
-
-    NUM_LANDMARKS: Literal[33] = 33
-    POINTS_PER_LANDMARK: Literal[4] = 4  # x, y, z, depth?
-
-    def __init__(self, pos: Tuple[float, float], scale: int) -> None:
-        """Creates a new PyGame skeleton."""
-        self.pos = pos
-        self.skeleton_points: np.ndarray = np.zeros((33, 4))
-        self.scale = scale
-
-    def render(self, window) -> None:
-        """Draws the skeleton on the pygame window."""
-        for landmark_pair in self.CONNECTIONS:
-            start_landmark: int = landmark_pair[X]
-            end_landmark: int = landmark_pair[Y]
-            line_start_x: float = self.skeleton_points[start_landmark][X]
-            line_start_y: float = self.skeleton_points[start_landmark][Y]
-            line_end_x: float = self.skeleton_points[end_landmark][X]
-            line_end_y: float = self.skeleton_points[end_landmark][Y]
-            pygame.draw.line(window, self.LIMB_COLOR,
-                             [float(line_start_x), float(line_start_y)],
-                             [float(line_end_x), float(line_end_y)],
-                             self.LIMB_WIDTH)
-
-        for _, landmark in enumerate(self.skeleton_points):
-            point_x: float = landmark[X]
-            point_y: float = landmark[Y]
-            pygame.draw.circle(window, self.LANDMARK_COLOR,
-                               [point_x, point_y],
-                               self.LANDMARK_RADIUS,
-                               self.LANDMARK_OUTLINE_WIDTH)
+"""User interface implementation of PyGame."""
+from typing import Any, Callable, List, Literal, Tuple
+import math
+import pygame
+from pygame.constants import QUIT
+import numpy as np
+from cvgui.core.displaying.components import Button, Skeleton, TrackingBubble
+
+X = 0
+Y = 1
+
+
+class PyGameUI:
+    """User interface implementation of PyGame."""
+
+    BACKGROUND: tuple[Literal[0], Literal[0], Literal[0]] = (0, 0, 0)
+
+    window: pygame.surface.Surface
+    fps_clock: pygame.time.Clock
+    running: bool
+
+    def __init__(self, height: int, width: int, fps: int) -> None:
+        """Create a new pygame user interface.
+
+        Args:
+            height (int): The height of the UI window.
+            width (int): The width of the UI window.
+            fps (int): How many frames per second to \
+                render in the UI window.
+        """
+        self.width: int = width
+        self.height: int = height
+        self.fps: int = fps
+
+    def clear(self) -> None:
+        """Clear the pygame window by filling it with \
+        a single color."""
+        self.window.fill(self.BACKGROUND)
+
+    def update(self) -> None:
+        """Update the PyGame window."""
+        pygame.display.update()
+        self.fps_clock.tick(self.fps)
+
+        for event in pygame.event.get():
+            if event.type == QUIT:
+                pygame.quit()
+                self.running = False
+
+    def button(self, pos: Tuple[float, float],
+               activation_distance: float,
+               color: Tuple[int, int, int, int],
+               radius: int = 100) -> Button:
+        """Create a PyGame button at the specified location."""
+        return PyGameButton(pos=pos, activation_distance=activation_distance,
+                            color=color, radius=radius)
+
+    def skeleton(self, pos: Tuple[float, float], scale: int) -> Skeleton:
+        """Create a PyGame skeleton at the specified location."""
+        return PyGameSkeleton(pos=pos, scale=scale)
+
+    def tracking_bubble(self,
+                        target: int,
+                        color: Tuple[int, int, int, int],
+                        radius: int = 100
+                        ) -> TrackingBubble:
+        """Create a pygame tracking bubble with the given settings.
+
+        Args:
+            target (int): The pose index the tracking bubble \
+                should follow
+            color (Tuple[int, int, int, int]): The color to make \
+                the tracking bubble.
+            radius (int, optional): The radius of the tracking bubble cirlce. \
+                Defaults to 100.
+
+        Returns:
+            TrackingBubble: _description_
+        """
+        return PyGameTrackingBubble(color=color, target=target, radius=radius)
+
+    def new_gui(self) -> None:
+        """Initialize the PyGame user interface."""
+        pygame.init()
+        pygame.font.init()
+
+        # Game Setup
+        self.fps_clock = pygame.time.Clock()
+
+        self.window: pygame.surface.Surface = pygame.display.set_mode(
+            (self.width, self.height))
+        pygame.display.set_caption("cvgui")
+        self.window.fill(self.BACKGROUND)
+        self.running = True
+
+
+class PyGameTrackingBubble:
+    """An implementation of the \
+        `cvgui.core.displaying.components.TrackingBubble` \
+            component in pygame."""
+
+    def __init__(self,
+                 color: Tuple[int, int, int, int],
+                 radius: int,
+                 target: int) -> None:
+        """Create a new pygame tracking bubble.
+
+        Args:
+            color (Tuple[int, int, int, int]): The color \
+                to make the tracking bubble.
+            radius (int): The radius to make the \
+                tracking bubble.
+            target (int): The index of the pose point that \
+                the pygame tracking bubble should follow.
+        """
+        self.color: Tuple[int, int, int, int] = color
+        self.radius: int = radius
+        self.target: int = target
+        self.pos: Tuple[float, float] = (0, 0)
+
+    def render(self, window: Any) -> None:
+        """Draw the tracking bubble on the \
+            pygame window.
+
+        Args:
+            window (Any): The pygame window
+            to draw the tracking bubble on.
+        """
+        color = pygame.color.Color(
+            self.color[0], self.color[1],
+            self.color[2], self.color[3])
+        pygame.draw.circle(
+            window, color,
+            (self.pos[X], self.pos[Y]),
+            self.radius
+        )
+
+
+class PyGameButton:
+    """An implementation of the \
+        `cvgui.core.displaying.components.Button` \
+            component in pygame."""
+
+    def __init__(self, pos: Tuple[float, float],
+                 activation_distance: float,
+                 color: Tuple[int, int, int, int],
+                 radius: int) -> None:
+        """Create a new PyGameButton at the location specified."""
+        self.pos = pos
+        """The position to render the button at."""
+
+        self.activation_distance: float = activation_distance
+        """The distance between and action and the button for \
+            it to be considered clicked."""
+
+        self.targets: List[int]
+        """Indicies of pose points that can click the button."""
+
+        self.callback: Callable
+        """The function to run when the button is clicked."""
+
+        self.color: Tuple[int, int, int, int] = color
+        """The color to make the button."""
+
+        self.radius: int = radius
+        """The radius to make the button."""
+
+    def is_clicked(self, pos: Tuple[float, float]) -> bool:
+        """Check if the button has been clicked."""
+        if abs(self.pos[X] - pos[X]) > self.activation_distance \
+                or abs(self.pos[Y] - pos[Y]) > self.activation_distance:
+            return False
+        if math.sqrt((self.pos[X] - pos[X])**2 + (self.pos[Y] - pos[Y])**2) \
+                > self.activation_distance:
+            return False
+        return True
+
+    def render(self, window) -> None:
+        """Draw the button on the pygame window."""
+        color = pygame.color.Color(
+            self.color[0], self.color[1],
+            self.color[2], self.color[3])
+        pygame.draw.circle(
+            window, color,
+            (self.pos[X], self.pos[Y]),
+            self.radius
+        )
+
+
+class PyGameSkeleton:
+    """Skeleton implementation in PyGame."""
+
+    # Where to connect limbs. Refer to here
+    # https://mediapipe.dev/images/mobile/pose_tracking_full_body_landmarks.png
+    # TODO: Move this somewhere else
+    CONNECTIONS: np.ndarray = np.array([
+        [16, 14], [16, 18], [16, 20], [16, 22],
+        [18, 20], [14, 12], [12, 11], [12, 24],
+        [11, 23], [11, 13], [15, 13], [15, 17],
+        [15, 19], [15, 21], [17, 19], [24, 23],
+        [26, 24], [26, 28], [25, 23], [25, 27],
+        [10, 9], [8, 6], [5, 6], [5, 4], [0, 4],
+        [0, 1], [2, 1], [2, 3], [3, 7], [28, 32],
+        [28, 30], [27, 29], [27, 31], [32, 30],
+        [29, 31]
+    ])
+
+    LIMB_COLOR: tuple[Literal[255], Literal[255],
+                      Literal[255]] = (255, 255, 255)
+    LIMB_WIDTH: Literal[2] = 2
+
+    LANDMARK_COLOR: tuple[Literal[0], Literal[255], Literal[0]] = (0, 255, 0)
+    LANDMARK_RADIUS: Literal[5] = 5
+    LANDMARK_OUTLINE_WIDTH: Literal[0] = 0
+
+    NUM_LANDMARKS: Literal[33] = 33
+    POINTS_PER_LANDMARK: Literal[4] = 4  # x, y, z, depth?
+
+    def __init__(self, pos: Tuple[float, float], scale: int) -> None:
+        """Create a new PyGame skeleton."""
+        self.pos = pos
+        self.skeleton_points: np.ndarray = np.zeros((33, 4))
+        self.scale = scale
+
+    def render(self, window) -> None:
+        """Draw the skeleton on the pygame window."""
+        for landmark_pair in self.CONNECTIONS:
+            start_landmark: int = landmark_pair[X]
+            end_landmark: int = landmark_pair[Y]
+            line_start_x: float = self.skeleton_points[start_landmark][X]
+            line_start_y: float = self.skeleton_points[start_landmark][Y]
+            line_end_x: float = self.skeleton_points[end_landmark][X]
+            line_end_y: float = self.skeleton_points[end_landmark][Y]
+            pygame.draw.line(window, self.LIMB_COLOR,
+                             [float(line_start_x), float(line_start_y)],
+                             [float(line_end_x), float(line_end_y)],
+                             self.LIMB_WIDTH)
+
+        for _, landmark in enumerate(self.skeleton_points):
+            point_x: float = landmark[X]
+            point_y: float = landmark[Y]
+            pygame.draw.circle(window, self.LANDMARK_COLOR,
+                               [point_x, point_y],
+                               self.LANDMARK_RADIUS,
+                               self.LANDMARK_OUTLINE_WIDTH)
```

### Comparing `cvgui-0.2.0/cvgui.egg-info/SOURCES.txt` & `cvgui-0.3.0/cvgui.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 cvgui/activity/__init__.py
 cvgui/activity/activity.py
 cvgui/activity/scene.py
 cvgui/core/__init__.py
 cvgui/core/displaying/__init__.py
 cvgui/core/displaying/components.py
 cvgui/core/displaying/service.py
-cvgui/core/recieving/__init__.py
-cvgui/core/recieving/service.py
+cvgui/core/logging/__init__.py
+cvgui/core/logging/service.py
+cvgui/core/receiving/__init__.py
+cvgui/core/receiving/service.py
 cvgui/inputs/__init__.py
 cvgui/inputs/computer_vision/__init__.py
 cvgui/inputs/computer_vision/computer_vision.py
 cvgui/inputs/computer_vision/cv_model/__init__.py
 cvgui/inputs/computer_vision/cv_model/blazepose.py
 cvgui/inputs/computer_vision/frame_input/__init__.py
 cvgui/inputs/computer_vision/frame_input/webcam.py
-cvgui/inputs/mocap/__init__.py
-cvgui/inputs/mocap/mocap_input.py
+cvgui/outputs/__init__.py
+cvgui/outputs/loggers/__init__.py
+cvgui/outputs/loggers/csv_logger.py
 cvgui/user_interface/__init__.py
 cvgui/user_interface/pygame_ui/__init__.py
 cvgui/user_interface/pygame_ui/pygame.py
```

### Comparing `cvgui-0.2.0/setup.py` & `cvgui-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 NAME = "cvgui"
 DESCRIPTION = "A library for creating body-interactive guis using computer vision."
 URL = "https://github.com/mitchellss/cvgui"
 EMAIL = "stephen.mitchell2299@gmail.com"
 AUTHOR = "Stephen Mitchell"
 REQUIRES_PYTHON = ">=3.9"
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 
 REQUIRED = [
     "mediapipe>=0.8.7.2",
     "numpy>=1.21.2",
     "opencv_python>=4.3.0.38",
     "typing_extensions>=4.3.0",
     "pygame>=2.0.0"
```

