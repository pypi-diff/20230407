# Comparing `tmp/PySink-0.0.8.tar.gz` & `tmp/PySink-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySink-0.0.8.tar", last modified: Mon Feb 27 18:35:17 2023, max compression
+gzip compressed data, was "PySink-0.0.9.tar", last modified: Thu Mar 30 18:09:10 2023, max compression
```

## Comparing `PySink-0.0.8.tar` & `PySink-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:35:17.378709 PySink-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-27 18:35:08.000000 PySink-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17486 2023-02-27 18:35:17.378709 PySink-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:35:17.378709 PySink-0.0.8/PySink/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-27 18:35:08.000000 PySink-0.0.8/PySink/AsyncManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-27 18:35:08.000000 PySink-0.0.8/PySink/AsyncWorker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:35:17.378709 PySink-0.0.8/PySink/Widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-02-27 18:35:08.000000 PySink-0.0.8/PySink/Widgets/ProgressBarWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-27 18:35:08.000000 PySink-0.0.8/PySink/Widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-27 18:35:08.000000 PySink-0.0.8/PySink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:35:17.378709 PySink-0.0.8/PySink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17486 2023-02-27 18:35:17.000000 PySink-0.0.8/PySink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-27 18:35:17.000000 PySink-0.0.8/PySink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 18:35:17.000000 PySink-0.0.8/PySink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-27 18:35:17.000000 PySink-0.0.8/PySink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-27 18:35:17.000000 PySink-0.0.8/PySink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-02-27 18:35:08.000000 PySink-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 18:35:17.378709 PySink-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-27 18:35:08.000000 PySink-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:09:10.647069 PySink-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-30 18:08:49.000000 PySink-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-03-30 18:09:10.647069 PySink-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:09:10.643069 PySink-0.0.9/PySink/
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-03-30 18:08:49.000000 PySink-0.0.9/PySink/AsyncManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-03-30 18:08:49.000000 PySink-0.0.9/PySink/AsyncWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-30 18:08:49.000000 PySink-0.0.9/PySink/CancellableAsyncWorker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:09:10.647069 PySink-0.0.9/PySink/Objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-30 18:08:49.000000 PySink-0.0.9/PySink/Objects/AsyncWorkerProgress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-30 18:08:49.000000 PySink-0.0.9/PySink/Objects/AsyncWorkerResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-30 18:08:49.000000 PySink-0.0.9/PySink/Objects/AsyncWorkerSignals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-30 18:08:49.000000 PySink-0.0.9/PySink/Objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:09:10.647069 PySink-0.0.9/PySink/Widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-03-30 18:08:49.000000 PySink-0.0.9/PySink/Widgets/ProgressBarWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-30 18:08:49.000000 PySink-0.0.9/PySink/Widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-30 18:08:49.000000 PySink-0.0.9/PySink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:09:10.647069 PySink-0.0.9/PySink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-03-30 18:09:10.000000 PySink-0.0.9/PySink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-30 18:09:10.000000 PySink-0.0.9/PySink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 18:09:10.000000 PySink-0.0.9/PySink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-30 18:09:10.000000 PySink-0.0.9/PySink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 18:09:10.000000 PySink-0.0.9/PySink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-03-30 18:08:49.000000 PySink-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-30 18:08:49.000000 PySink-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 18:09:10.647069 PySink-0.0.9/setup.cfg
```

### Comparing `PySink-0.0.8/LICENSE` & `PySink-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PySink-0.0.8/PKG-INFO` & `PySink-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,101 +1,85 @@
-Metadata-Version: 2.1
-Name: PySink
-Version: 0.0.8
-Summary: PySide6 Helpers for Powerful Async Desktop Apps
-Home-page: UNKNOWN
-Author: Zack Johnson
-Author-email: <zackjohnson298@gmail.com>
-License: UNKNOWN
-Keywords: python,app,gui,async,application,desktop,ui
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # PySink
 
 Created by Zack Johnson
 
-<span style="color:red">
-Under construction, not ready for use!
-</span>
+## Under construction, not yet ready for use!!
+
+Full documentation can be found on ReadTheDocs
 
 PySink is an extension of the PySide6 Qt Framework that simplifies the implementation
-of Asynchronous tasks in your Desktop Applications. It contains several
+of Asynchronous tasks in Desktop Applications. It contains several
 helper Widgets and Classes that enable you to build powerful and professional
 desktop applications without worrying about managing threads or freezing 
 UI with long-running tasks. PySink's implementation suggests an MVC 
 architecture for your application, but should perform well in other architectures
 such as MVVM.
 
-## Getting Started
+## Basic Overview
 PySink is based on the concept of Workers and Managers. Workers are custom objects that 
-perform your long-running tasks. They inherit from the provided *AsyncWorker* class and 
+perform long-running tasks. They inherit from the provided *AsyncWorker* class and 
 override the *AsyncWorker.run()* method to perform the tasks, emitting progress values and 
-optional status messages along the way. These workers are managed by a generalized object called the *AsyncManager*. 
+optional status messages along the way. These workers are managed by a generalized object called the
+*AsyncManager*. 
+
+The Manager is an object that manages all the workers/threading and handles the termination/cancellation 
+of said threads and workers when necessary. The Manager can also pass along the signals emitted by 
+the worker (you can also connect to the worker's signals directly, see example 5 below).
+
+The two signals that
+
+## Getting Started
 
-The Manager is an object that manages all the threading, passes along the signals and values 
-emitted by the Worker, and handles the cancellation of said threads and workers when necessary.
 
 Let's look at a couple examples to help you get started. Full examples and all source code can 
 be found at https://github.com/zackjohnson298/PySink
 
 ### Example 1: Defining and Using a Custom Async Worker
 In this first example, we will create a custom AsyncWorker that performs *time.sleep()* 
 for a specified duration and number of cycles. To create a new worker, define a class
 that inherits from *PySink.AsyncWorker*. Any values needed by the worker should be passed
 in via it's *\_\_init\_\_* method: 
 
 ```python
 from PySink import AsyncWorker
 
 
-class DemoAsyncWorker(AsyncWorker):
+class DemoAsyncWorker1(AsyncWorker):
     def __init__(self, delay_seconds: int, cycles=4):
-        super(DemoAsyncWorker, self).__init__()
+        super(DemoAsyncWorker1, self).__init__()
         # Store the values passed in during initialization
         self.delay_seconds = delay_seconds
         self.cycles = cycles
 ```
-To implement your long-running task, simply override AsyncWorker's *run* method.
-This method takes no parameters and returns nothing, it just performs your task. 
-Progress/status is emitted by calling the *self.update_progress(progress, message)*
-method, and when your task is done you can emit any results via the 
-*self.complete(\*\*kwargs)* method:
+To implement the long-running task, simply override AsyncWorker's *run* method.
+This method takes no parameters and returns nothing, it' only job is to perform the long-running task. 
+Progress is emitted by calling the *self.update_progress(progress, message)*method, and when the task is
+done you can emit any results via the *self.complete(\*\*kwargs)* method:
 
 ```python
 from PySink import AsyncWorker
 import time
 
 
-class DemoAsyncWorker(AsyncWorker):
+class DemoAsyncWorker1(AsyncWorker):
     def __init__(self, delay_seconds: int, cycles=4):
-        super(DemoAsyncWorker, self).__init__()
+        super(DemoAsyncWorker1, self).__init__()
+        # Store the values passed in during initialization
         self.delay_seconds = delay_seconds
         self.cycles = cycles
 
     def run(self):
-        progress = 0
-        progress_increment = 100 / self.cycles
-        # Update progress by providing a progress value from 0-100 with an 
-        #   optional message
-        self.update_progress(0, 'Starting Task')
+        # Update discrete progress by providing a progress value from 0-100 with an optional message
+        progress = 5
+        self.update_progress(progress, 'Starting Task')
         for ii in range(self.cycles):
             time.sleep(self.delay_seconds)
-            progress += progress_increment
+            progress += 90 / self.cycles
             self.update_progress(progress, f'Progress message #{ii + 1}')
-        # Call the self.complete method to end your task, passing any 
-        #   results as keyword arguments
+        # Call the self.complete method to end your task, passing any results as keyword arguments
         demo_result = 12
         self.complete(demo_result=demo_result)
 ```
 Starting your custom worker is as simple as creating an AsyncManager, tying 
 its signals to your callback methods, and passing your custom Worker to its *start_worker(worker)* method. 
 *(We also need a QApplication running for the event loop 
 to start, which you will already have in your PySide6 Application).* Let's see 
@@ -261,15 +245,15 @@
 ```
 
 Including the snippet within the *\_\_name__ == \_\_main__* block allows you to run this
 as a script on its own and see the window you've just created. Doing this allows you to make 
 sure the UI looks correct before you connect any actions to the View. 
 Run the script to see the app window:
 
-![alt text](img/example2_main_view.png "Title")
+![alt text](docs/img/example2_main_view.png "Title")
 
 This very simple app has a start button, progress bar, and some labels to display the data.
 The View also has a signal that gets emitted on the button press, as well as a 
 few helper methods to reset the UI and set the progress and output values. Exposing the 
 signals and providing methods like this are not required to make an app work. However, 
 doing so decouples the UI from the application logic allowing for much more flexibility in
 the future.
@@ -287,59 +271,60 @@
 
 class MainController:
     def __init__(self, view: MainView):
         # Initialize/Store Attributes
         self.view = view
         self.async_manager = AsyncManager()
         # Connect UI Signals
-        self.view.button_pushed_signal.connect(self.start_task)
+        self.view.start_signal.connect(self.start_task)
         # Connect Async Signals
         self.async_manager.worker_progress_signal.connect(self.view.set_progress)
         self.async_manager.worker_finished_signal.connect(self.task_complete_callback)
         # Initialize UI State
-        self.view.show_button()
+        self.view.hide_progress()
 
     def start_task(self):
         # Update UI
         self.view.clear()
         self.view.show_progress()
         # Initialize/Start Worker
         worker = DemoAsyncWorker(2, cycles=5)
         self.async_manager.start_worker(worker)
 
     def task_complete_callback(self, results):
         # Update UI
         self.view.clear()
-        self.view.show_button()
+        self.view.hide_progress()
         # Handle results
         self.view.set_result(results.get('demo_result'))
         self.view.set_warnings(results.get('warnings'))
         self.view.set_errors(results.get('errors'))
 ```
 In this example, the Controller gets initialized with the view it is controlling. Injecting 
 the dependency like this allows you to create layers in your App Architecture, and moves the 
 responsibility of 'showing' the window up a level. It also makes the Controller testable. 
 By mocking the attributes and methods of our view in a different class (that
 doesn't need UI at all) tests can be automated much faster. Again, this is not required to 
 get a PySink app to work, but this practice will be beneficial in the long run.
 
 Let's take a closer look at the Controller's *\_\_init\_\_()* method:
+
 ```python
 class MainController:
     def __init__(self, view: MainView):
         # Initialize/Store Attributes
         self.view = view
         self.async_manager = AsyncManager()
         # Connect UI Signals
-        self.view.button_pushed_signal.connect(self.start_task)
+        self.view.start_signal.connect(self.start_task)
         # Connect Async Signals
         self.async_manager.worker_progress_signal.connect(self.view.set_progress)
         self.async_manager.worker_finished_signal.connect(self.task_complete_callback)
         # Initialize UI State
-        self.view.show_button()
+        self.view.hide_progress()
 ```
 
 Within the *\_\_init__()* method, any attributes needed by the controller are initialized and
 stored. In this case, those are the View and an AsyncManager (storing the manager as an 
 attribute ensures that the worker and thread stay alive after calling the Manager's 
 *start_worker* method).
 
@@ -376,21 +361,21 @@
 Now let's look at what happens when the worker is done running its task. Since the 
 AsyncManager's *worker_finished_signal* was connected to the Controller's 
 *task_complete_callback*, that callback will be executed upon the worker's completion. 
 Here's what the callback looks like:
 
 ```python
     def task_complete_callback(self, results):
-        # Update UI
-        self.view.clear()
-        self.view.show_button()
-        # Handle results
-        self.view.set_result(results.get('demo_result'))
-        self.view.set_warnings(results.get('warnings'))
-        self.view.set_errors(results.get('errors'))
+    # Update UI
+    self.view.clear()
+    self.view.hide_progress()
+    # Handle results
+    self.view.set_result(results.get('demo_result'))
+    self.view.set_warnings(results.get('warnings'))
+    self.view.set_errors(results.get('errors'))
 ```
 
 As stated in the previous example, the results of the worker's task are provided as a 
 dictionary that gets passed in to the completion callback. This dictionary contains the 
 values defined as keyword arguments within the worker's *run* method, as well as any 
 warnings/errors encountered during the task. In this callback, the UI is again updated to 
 reflect the task's completion and the results are displayed to the user by passing them into
@@ -413,17 +398,15 @@
 view.show()
 app.exec()
 ```
 
 Run the script and the application will start. Pushing the start button within the app will 
 trigger the long-running task, and at its completion data from the worker will be displayed:
 
-![alt text](img/example2_while_running.png "Title")
+![alt text](docs/img/example2_while_running.png "Title")
 
-![alt text](img/example2_complete.png "Title")
+![alt text](docs/img/example2_complete.png "Title")
 
 
 Congratulations! You've just created an asynchronous app with PySink!
 Full example code can be found at https://github.com/zackjohnson298/PySink 
 in the examples/example2 folder.
-
-
```

### Comparing `PySink-0.0.8/PySink.egg-info/PKG-INFO` & `PySink-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,101 +1,122 @@
 Metadata-Version: 2.1
 Name: PySink
-Version: 0.0.8
+Version: 0.0.9
 Summary: PySide6 Helpers for Powerful Async Desktop Apps
-Home-page: UNKNOWN
-Author: Zack Johnson
-Author-email: <zackjohnson298@gmail.com>
-License: UNKNOWN
+Author-email: Zack Johnson <zackjohnson298@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Zack Johnson
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 Keywords: python,app,gui,async,application,desktop,ui
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 # PySink
 
 Created by Zack Johnson
 
-<span style="color:red">
-Under construction, not ready for use!
-</span>
+## Under construction, not yet ready for use!!
+
+Full documentation can be found on ReadTheDocs
 
 PySink is an extension of the PySide6 Qt Framework that simplifies the implementation
-of Asynchronous tasks in your Desktop Applications. It contains several
+of Asynchronous tasks in Desktop Applications. It contains several
 helper Widgets and Classes that enable you to build powerful and professional
 desktop applications without worrying about managing threads or freezing 
 UI with long-running tasks. PySink's implementation suggests an MVC 
 architecture for your application, but should perform well in other architectures
 such as MVVM.
 
-## Getting Started
+## Basic Overview
 PySink is based on the concept of Workers and Managers. Workers are custom objects that 
-perform your long-running tasks. They inherit from the provided *AsyncWorker* class and 
+perform long-running tasks. They inherit from the provided *AsyncWorker* class and 
 override the *AsyncWorker.run()* method to perform the tasks, emitting progress values and 
-optional status messages along the way. These workers are managed by a generalized object called the *AsyncManager*. 
+optional status messages along the way. These workers are managed by a generalized object called the
+*AsyncManager*. 
+
+The Manager is an object that manages all the workers/threading and handles the termination/cancellation 
+of said threads and workers when necessary. The Manager can also pass along the signals emitted by 
+the worker (you can also connect to the worker's signals directly, see example 5 below).
+
+The two signals that
+
+## Getting Started
 
-The Manager is an object that manages all the threading, passes along the signals and values 
-emitted by the Worker, and handles the cancellation of said threads and workers when necessary.
 
 Let's look at a couple examples to help you get started. Full examples and all source code can 
 be found at https://github.com/zackjohnson298/PySink
 
 ### Example 1: Defining and Using a Custom Async Worker
 In this first example, we will create a custom AsyncWorker that performs *time.sleep()* 
 for a specified duration and number of cycles. To create a new worker, define a class
 that inherits from *PySink.AsyncWorker*. Any values needed by the worker should be passed
 in via it's *\_\_init\_\_* method: 
 
 ```python
 from PySink import AsyncWorker
 
 
-class DemoAsyncWorker(AsyncWorker):
+class DemoAsyncWorker1(AsyncWorker):
     def __init__(self, delay_seconds: int, cycles=4):
-        super(DemoAsyncWorker, self).__init__()
+        super(DemoAsyncWorker1, self).__init__()
         # Store the values passed in during initialization
         self.delay_seconds = delay_seconds
         self.cycles = cycles
 ```
-To implement your long-running task, simply override AsyncWorker's *run* method.
-This method takes no parameters and returns nothing, it just performs your task. 
-Progress/status is emitted by calling the *self.update_progress(progress, message)*
-method, and when your task is done you can emit any results via the 
-*self.complete(\*\*kwargs)* method:
+To implement the long-running task, simply override AsyncWorker's *run* method.
+This method takes no parameters and returns nothing, it' only job is to perform the long-running task. 
+Progress is emitted by calling the *self.update_progress(progress, message)*method, and when the task is
+done you can emit any results via the *self.complete(\*\*kwargs)* method:
 
 ```python
 from PySink import AsyncWorker
 import time
 
 
-class DemoAsyncWorker(AsyncWorker):
+class DemoAsyncWorker1(AsyncWorker):
     def __init__(self, delay_seconds: int, cycles=4):
-        super(DemoAsyncWorker, self).__init__()
+        super(DemoAsyncWorker1, self).__init__()
+        # Store the values passed in during initialization
         self.delay_seconds = delay_seconds
         self.cycles = cycles
 
     def run(self):
-        progress = 0
-        progress_increment = 100 / self.cycles
-        # Update progress by providing a progress value from 0-100 with an 
-        #   optional message
-        self.update_progress(0, 'Starting Task')
+        # Update discrete progress by providing a progress value from 0-100 with an optional message
+        progress = 5
+        self.update_progress(progress, 'Starting Task')
         for ii in range(self.cycles):
             time.sleep(self.delay_seconds)
-            progress += progress_increment
+            progress += 90 / self.cycles
             self.update_progress(progress, f'Progress message #{ii + 1}')
-        # Call the self.complete method to end your task, passing any 
-        #   results as keyword arguments
+        # Call the self.complete method to end your task, passing any results as keyword arguments
         demo_result = 12
         self.complete(demo_result=demo_result)
 ```
 Starting your custom worker is as simple as creating an AsyncManager, tying 
 its signals to your callback methods, and passing your custom Worker to its *start_worker(worker)* method. 
 *(We also need a QApplication running for the event loop 
 to start, which you will already have in your PySide6 Application).* Let's see 
@@ -261,15 +282,15 @@
 ```
 
 Including the snippet within the *\_\_name__ == \_\_main__* block allows you to run this
 as a script on its own and see the window you've just created. Doing this allows you to make 
 sure the UI looks correct before you connect any actions to the View. 
 Run the script to see the app window:
 
-![alt text](img/example2_main_view.png "Title")
+![alt text](docs/img/example2_main_view.png "Title")
 
 This very simple app has a start button, progress bar, and some labels to display the data.
 The View also has a signal that gets emitted on the button press, as well as a 
 few helper methods to reset the UI and set the progress and output values. Exposing the 
 signals and providing methods like this are not required to make an app work. However, 
 doing so decouples the UI from the application logic allowing for much more flexibility in
 the future.
@@ -287,59 +308,60 @@
 
 class MainController:
     def __init__(self, view: MainView):
         # Initialize/Store Attributes
         self.view = view
         self.async_manager = AsyncManager()
         # Connect UI Signals
-        self.view.button_pushed_signal.connect(self.start_task)
+        self.view.start_signal.connect(self.start_task)
         # Connect Async Signals
         self.async_manager.worker_progress_signal.connect(self.view.set_progress)
         self.async_manager.worker_finished_signal.connect(self.task_complete_callback)
         # Initialize UI State
-        self.view.show_button()
+        self.view.hide_progress()
 
     def start_task(self):
         # Update UI
         self.view.clear()
         self.view.show_progress()
         # Initialize/Start Worker
         worker = DemoAsyncWorker(2, cycles=5)
         self.async_manager.start_worker(worker)
 
     def task_complete_callback(self, results):
         # Update UI
         self.view.clear()
-        self.view.show_button()
+        self.view.hide_progress()
         # Handle results
         self.view.set_result(results.get('demo_result'))
         self.view.set_warnings(results.get('warnings'))
         self.view.set_errors(results.get('errors'))
 ```
 In this example, the Controller gets initialized with the view it is controlling. Injecting 
 the dependency like this allows you to create layers in your App Architecture, and moves the 
 responsibility of 'showing' the window up a level. It also makes the Controller testable. 
 By mocking the attributes and methods of our view in a different class (that
 doesn't need UI at all) tests can be automated much faster. Again, this is not required to 
 get a PySink app to work, but this practice will be beneficial in the long run.
 
 Let's take a closer look at the Controller's *\_\_init\_\_()* method:
+
 ```python
 class MainController:
     def __init__(self, view: MainView):
         # Initialize/Store Attributes
         self.view = view
         self.async_manager = AsyncManager()
         # Connect UI Signals
-        self.view.button_pushed_signal.connect(self.start_task)
+        self.view.start_signal.connect(self.start_task)
         # Connect Async Signals
         self.async_manager.worker_progress_signal.connect(self.view.set_progress)
         self.async_manager.worker_finished_signal.connect(self.task_complete_callback)
         # Initialize UI State
-        self.view.show_button()
+        self.view.hide_progress()
 ```
 
 Within the *\_\_init__()* method, any attributes needed by the controller are initialized and
 stored. In this case, those are the View and an AsyncManager (storing the manager as an 
 attribute ensures that the worker and thread stay alive after calling the Manager's 
 *start_worker* method).
 
@@ -376,21 +398,21 @@
 Now let's look at what happens when the worker is done running its task. Since the 
 AsyncManager's *worker_finished_signal* was connected to the Controller's 
 *task_complete_callback*, that callback will be executed upon the worker's completion. 
 Here's what the callback looks like:
 
 ```python
     def task_complete_callback(self, results):
-        # Update UI
-        self.view.clear()
-        self.view.show_button()
-        # Handle results
-        self.view.set_result(results.get('demo_result'))
-        self.view.set_warnings(results.get('warnings'))
-        self.view.set_errors(results.get('errors'))
+    # Update UI
+    self.view.clear()
+    self.view.hide_progress()
+    # Handle results
+    self.view.set_result(results.get('demo_result'))
+    self.view.set_warnings(results.get('warnings'))
+    self.view.set_errors(results.get('errors'))
 ```
 
 As stated in the previous example, the results of the worker's task are provided as a 
 dictionary that gets passed in to the completion callback. This dictionary contains the 
 values defined as keyword arguments within the worker's *run* method, as well as any 
 warnings/errors encountered during the task. In this callback, the UI is again updated to 
 reflect the task's completion and the results are displayed to the user by passing them into
@@ -413,17 +435,15 @@
 view.show()
 app.exec()
 ```
 
 Run the script and the application will start. Pushing the start button within the app will 
 trigger the long-running task, and at its completion data from the worker will be displayed:
 
-![alt text](img/example2_while_running.png "Title")
+![alt text](docs/img/example2_while_running.png "Title")
 
-![alt text](img/example2_complete.png "Title")
+![alt text](docs/img/example2_complete.png "Title")
 
 
 Congratulations! You've just created an asynchronous app with PySink!
 Full example code can be found at https://github.com/zackjohnson298/PySink 
 in the examples/example2 folder.
-
-
```

### Comparing `PySink-0.0.8/README.md` & `PySink-0.0.9/PySink.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,122 @@
+Metadata-Version: 2.1
+Name: PySink
+Version: 0.0.9
+Summary: PySide6 Helpers for Powerful Async Desktop Apps
+Author-email: Zack Johnson <zackjohnson298@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Zack Johnson
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Keywords: python,app,gui,async,application,desktop,ui
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PySink
 
 Created by Zack Johnson
 
-<span style="color:red">
-Under construction, not ready for use!
-</span>
+## Under construction, not yet ready for use!!
+
+Full documentation can be found on ReadTheDocs
 
 PySink is an extension of the PySide6 Qt Framework that simplifies the implementation
-of Asynchronous tasks in your Desktop Applications. It contains several
+of Asynchronous tasks in Desktop Applications. It contains several
 helper Widgets and Classes that enable you to build powerful and professional
 desktop applications without worrying about managing threads or freezing 
 UI with long-running tasks. PySink's implementation suggests an MVC 
 architecture for your application, but should perform well in other architectures
 such as MVVM.
 
-## Getting Started
+## Basic Overview
 PySink is based on the concept of Workers and Managers. Workers are custom objects that 
-perform your long-running tasks. They inherit from the provided *AsyncWorker* class and 
+perform long-running tasks. They inherit from the provided *AsyncWorker* class and 
 override the *AsyncWorker.run()* method to perform the tasks, emitting progress values and 
-optional status messages along the way. These workers are managed by a generalized object called the *AsyncManager*. 
+optional status messages along the way. These workers are managed by a generalized object called the
+*AsyncManager*. 
+
+The Manager is an object that manages all the workers/threading and handles the termination/cancellation 
+of said threads and workers when necessary. The Manager can also pass along the signals emitted by 
+the worker (you can also connect to the worker's signals directly, see example 5 below).
+
+The two signals that
+
+## Getting Started
 
-The Manager is an object that manages all the threading, passes along the signals and values 
-emitted by the Worker, and handles the cancellation of said threads and workers when necessary.
 
 Let's look at a couple examples to help you get started. Full examples and all source code can 
 be found at https://github.com/zackjohnson298/PySink
 
 ### Example 1: Defining and Using a Custom Async Worker
 In this first example, we will create a custom AsyncWorker that performs *time.sleep()* 
 for a specified duration and number of cycles. To create a new worker, define a class
 that inherits from *PySink.AsyncWorker*. Any values needed by the worker should be passed
 in via it's *\_\_init\_\_* method: 
 
 ```python
 from PySink import AsyncWorker
 
 
-class DemoAsyncWorker(AsyncWorker):
+class DemoAsyncWorker1(AsyncWorker):
     def __init__(self, delay_seconds: int, cycles=4):
-        super(DemoAsyncWorker, self).__init__()
+        super(DemoAsyncWorker1, self).__init__()
         # Store the values passed in during initialization
         self.delay_seconds = delay_seconds
         self.cycles = cycles
 ```
-To implement your long-running task, simply override AsyncWorker's *run* method.
-This method takes no parameters and returns nothing, it just performs your task. 
-Progress/status is emitted by calling the *self.update_progress(progress, message)*
-method, and when your task is done you can emit any results via the 
-*self.complete(\*\*kwargs)* method:
+To implement the long-running task, simply override AsyncWorker's *run* method.
+This method takes no parameters and returns nothing, it' only job is to perform the long-running task. 
+Progress is emitted by calling the *self.update_progress(progress, message)*method, and when the task is
+done you can emit any results via the *self.complete(\*\*kwargs)* method:
 
 ```python
 from PySink import AsyncWorker
 import time
 
 
-class DemoAsyncWorker(AsyncWorker):
+class DemoAsyncWorker1(AsyncWorker):
     def __init__(self, delay_seconds: int, cycles=4):
-        super(DemoAsyncWorker, self).__init__()
+        super(DemoAsyncWorker1, self).__init__()
+        # Store the values passed in during initialization
         self.delay_seconds = delay_seconds
         self.cycles = cycles
 
     def run(self):
-        progress = 0
-        progress_increment = 100 / self.cycles
-        # Update progress by providing a progress value from 0-100 with an 
-        #   optional message
-        self.update_progress(0, 'Starting Task')
+        # Update discrete progress by providing a progress value from 0-100 with an optional message
+        progress = 5
+        self.update_progress(progress, 'Starting Task')
         for ii in range(self.cycles):
             time.sleep(self.delay_seconds)
-            progress += progress_increment
+            progress += 90 / self.cycles
             self.update_progress(progress, f'Progress message #{ii + 1}')
-        # Call the self.complete method to end your task, passing any 
-        #   results as keyword arguments
+        # Call the self.complete method to end your task, passing any results as keyword arguments
         demo_result = 12
         self.complete(demo_result=demo_result)
 ```
 Starting your custom worker is as simple as creating an AsyncManager, tying 
 its signals to your callback methods, and passing your custom Worker to its *start_worker(worker)* method. 
 *(We also need a QApplication running for the event loop 
 to start, which you will already have in your PySide6 Application).* Let's see 
@@ -241,15 +282,15 @@
 ```
 
 Including the snippet within the *\_\_name__ == \_\_main__* block allows you to run this
 as a script on its own and see the window you've just created. Doing this allows you to make 
 sure the UI looks correct before you connect any actions to the View. 
 Run the script to see the app window:
 
-![alt text](img/example2_main_view.png "Title")
+![alt text](docs/img/example2_main_view.png "Title")
 
 This very simple app has a start button, progress bar, and some labels to display the data.
 The View also has a signal that gets emitted on the button press, as well as a 
 few helper methods to reset the UI and set the progress and output values. Exposing the 
 signals and providing methods like this are not required to make an app work. However, 
 doing so decouples the UI from the application logic allowing for much more flexibility in
 the future.
@@ -267,59 +308,60 @@
 
 class MainController:
     def __init__(self, view: MainView):
         # Initialize/Store Attributes
         self.view = view
         self.async_manager = AsyncManager()
         # Connect UI Signals
-        self.view.button_pushed_signal.connect(self.start_task)
+        self.view.start_signal.connect(self.start_task)
         # Connect Async Signals
         self.async_manager.worker_progress_signal.connect(self.view.set_progress)
         self.async_manager.worker_finished_signal.connect(self.task_complete_callback)
         # Initialize UI State
-        self.view.show_button()
+        self.view.hide_progress()
 
     def start_task(self):
         # Update UI
         self.view.clear()
         self.view.show_progress()
         # Initialize/Start Worker
         worker = DemoAsyncWorker(2, cycles=5)
         self.async_manager.start_worker(worker)
 
     def task_complete_callback(self, results):
         # Update UI
         self.view.clear()
-        self.view.show_button()
+        self.view.hide_progress()
         # Handle results
         self.view.set_result(results.get('demo_result'))
         self.view.set_warnings(results.get('warnings'))
         self.view.set_errors(results.get('errors'))
 ```
 In this example, the Controller gets initialized with the view it is controlling. Injecting 
 the dependency like this allows you to create layers in your App Architecture, and moves the 
 responsibility of 'showing' the window up a level. It also makes the Controller testable. 
 By mocking the attributes and methods of our view in a different class (that
 doesn't need UI at all) tests can be automated much faster. Again, this is not required to 
 get a PySink app to work, but this practice will be beneficial in the long run.
 
 Let's take a closer look at the Controller's *\_\_init\_\_()* method:
+
 ```python
 class MainController:
     def __init__(self, view: MainView):
         # Initialize/Store Attributes
         self.view = view
         self.async_manager = AsyncManager()
         # Connect UI Signals
-        self.view.button_pushed_signal.connect(self.start_task)
+        self.view.start_signal.connect(self.start_task)
         # Connect Async Signals
         self.async_manager.worker_progress_signal.connect(self.view.set_progress)
         self.async_manager.worker_finished_signal.connect(self.task_complete_callback)
         # Initialize UI State
-        self.view.show_button()
+        self.view.hide_progress()
 ```
 
 Within the *\_\_init__()* method, any attributes needed by the controller are initialized and
 stored. In this case, those are the View and an AsyncManager (storing the manager as an 
 attribute ensures that the worker and thread stay alive after calling the Manager's 
 *start_worker* method).
 
@@ -356,21 +398,21 @@
 Now let's look at what happens when the worker is done running its task. Since the 
 AsyncManager's *worker_finished_signal* was connected to the Controller's 
 *task_complete_callback*, that callback will be executed upon the worker's completion. 
 Here's what the callback looks like:
 
 ```python
     def task_complete_callback(self, results):
-        # Update UI
-        self.view.clear()
-        self.view.show_button()
-        # Handle results
-        self.view.set_result(results.get('demo_result'))
-        self.view.set_warnings(results.get('warnings'))
-        self.view.set_errors(results.get('errors'))
+    # Update UI
+    self.view.clear()
+    self.view.hide_progress()
+    # Handle results
+    self.view.set_result(results.get('demo_result'))
+    self.view.set_warnings(results.get('warnings'))
+    self.view.set_errors(results.get('errors'))
 ```
 
 As stated in the previous example, the results of the worker's task are provided as a 
 dictionary that gets passed in to the completion callback. This dictionary contains the 
 values defined as keyword arguments within the worker's *run* method, as well as any 
 warnings/errors encountered during the task. In this callback, the UI is again updated to 
 reflect the task's completion and the results are displayed to the user by passing them into
@@ -393,15 +435,15 @@
 view.show()
 app.exec()
 ```
 
 Run the script and the application will start. Pushing the start button within the app will 
 trigger the long-running task, and at its completion data from the worker will be displayed:
 
-![alt text](img/example2_while_running.png "Title")
+![alt text](docs/img/example2_while_running.png "Title")
 
-![alt text](img/example2_complete.png "Title")
+![alt text](docs/img/example2_complete.png "Title")
 
 
 Congratulations! You've just created an asynchronous app with PySink!
 Full example code can be found at https://github.com/zackjohnson298/PySink 
 in the examples/example2 folder.
```

