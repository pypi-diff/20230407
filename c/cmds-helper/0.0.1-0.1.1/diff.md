# Comparing `tmp/cmds_helper-0.0.1.tar.gz` & `tmp/cmds_helper-0.1.1.tar.gz`

## Comparing `cmds_helper-0.0.1.tar` & `cmds_helper-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 cmds_helper-0.0.1/example_cmd.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmds_helper-0.0.1/cmdshelper/__init__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 cmds_helper-0.0.1/cmdshelper/helper.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 cmds_helper-0.0.1/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cmds_helper-0.0.1/LICENSE
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 cmds_helper-0.0.1/README.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cmds_helper-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 cmds_helper-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/example_cmd.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/cmdshelper/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/cmdshelper/__main__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/cmdshelper/helper.py
+-rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/scripts/cdmshelper.bat
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/tests/run.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 cmds_helper-0.1.1/PKG-INFO
```

### Comparing `cmds_helper-0.0.1/.gitignore` & `cmds_helper-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cmds_helper-0.0.1/LICENSE` & `cmds_helper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmds_helper-0.0.1/README.md` & `cmds_helper-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # CMDS Helper
 
 This modul will help us to automate CLI Command we usually use in projects.
 
+### Installation
+
+Using pip :
+
+```pip
+pip install cmds-helper
+```
+
 ### How To Use
 
 - Install cmds-helper module using `pip`
 - Make runner file in root of your project files directory (i.e `run.py`)
   ```
   --ProjectDir
       --{{Your project files/folder}}
@@ -36,39 +44,39 @@
       ],
       ...
   }
   ```
 
   - `{your_cmd_identifier}` is identifier for calling all cmd command under that identifier. every identifier must be unique
 
-  - `cmd_command_to_run` is the cmd command you want to run. The command is string you usually type in CLI, but in the json file, you separate every command/optional/arguments using comma / ','.
+  - `cmd_command_to_run` is the cmd command you want to run. The command is string you usually type in CLI, but in the json file, you separate every command/optional/arguments using space / ' ' like usual.
 
   - In `cmd_command_to_run`, you can add argument to pass, with type `%{i}` (`i` is index arguments passes)
 
 - Example :
 
   ```json
   "gitACP" : [
-          "git,add,.",
-          "git,commit,-m,%1",
-          "git,push"
+          "git add .",
+          "git commit -m %1",
+          "git push"
       ]
   ```
 
   the identifier to call that command is `gitACP` (command to call git common command `[add, commit, and push]`). under that identifier, we specify all command we want to call
 
-  - `"git add ."` is typed `"git,add,."`
-  - `"git commit -m "{message}" "` is typed `"git,commit,-m,%1"`
+  - `"git add ."`
+  - `"git commit -m "{message}" "` is typed `"git commit -m %1"`
     - `%1` means that the first argument passed when calling that command identifier, will replacing `%1` into the passed string
     - If you just want add same commit message for each commit, you can just change `%1` into your message like `feat: add something`
-  - `"git push"` is typed `"git,push"`
+  - `"git push"`
 
   You can see another command examples in `example_cmd.json`
 
-- There are 2 ways to run this `file`, by CLI with passing `arg` or by hardcode the command in `script`
+- There are 4 ways to run this `file`, by CLI with passing `arg`, by hardcode the command in `script`, or by using `python -m`
 
   - CLI Passing argument :
 
     - After instantiate the class, you can type this code :
 
       ```py
       import sys
@@ -97,14 +105,42 @@
       ```py
 
       cmd.run(["gitACP","feat: add something"])
       ```
 
       to run it, you just need to run `run.py` file
 
+  - Straight from Python module
+
+    It is just as simple as you open the folder that you want to run the command
+
+    ```
+    python -m cmdshelper [command] [args_1] [args_2] ... [args_3]
+    ```
+
+    for example:
+
+    ```
+    python -m cmdshelper gitACP "feat: add something"
+    ```
+
+  - Simply just cdmshelper
+
+    It is just as simple as you open the folder that you want to run the command
+
+    ```
+    cmdshelper [command] [args_1] [args_2] ... [args_3]
+    ```
+
+    for example:
+
+    ```
+    cmdshelper gitACP "feat: add something"
+    ```
+
 - Full code in `run.py ` will be :
 
   ```py
   from cmdshelper.helper import Helper
   import sys
 
   cmd = Helper()
```

### Comparing `cmds_helper-0.0.1/pyproject.toml` & `cmds_helper-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cmds-helper"
-version = "0.0.1"
+version = "0.1.1"
 authors = [
-  { name="Keyisa Raihan", email="keyisakris@gmail.com" },
+  { name = "Keyisa Raihan", email = "keyisakris@gmail.com" },
+  { name = "Yoel Mountanus Sitorus", email = "sclous2012@gmail.com" },
 ]
 description = "CLI CMD Command helper"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/yotakeys/cmds-helper"
-"Bug Tracker" = "https://github.com/yotakeys/cmds-helper/issues"
+"Bug Tracker" = "https://github.com/yotakeys/cmds-helper/issues"
+
+[project.scripts]
+cmdshelper = "cmdshelper:main"
```

### Comparing `cmds_helper-0.0.1/PKG-INFO` & `cmds_helper-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: cmds-helper
-Version: 0.0.1
+Version: 0.1.1
 Summary: CLI CMD Command helper
 Project-URL: Homepage, https://github.com/yotakeys/cmds-helper
 Project-URL: Bug Tracker, https://github.com/yotakeys/cmds-helper/issues
-Author-email: Keyisa Raihan <keyisakris@gmail.com>
+Author-email: Keyisa Raihan <keyisakris@gmail.com>, Yoel Mountanus Sitorus <sclous2012@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # CMDS Helper
 
 This modul will help us to automate CLI Command we usually use in projects.
 
+### Installation
+
+Using pip :
+
+```pip
+pip install cmds-helper
+```
+
 ### How To Use
 
 - Install cmds-helper module using `pip`
 - Make runner file in root of your project files directory (i.e `run.py`)
   ```
   --ProjectDir
       --{{Your project files/folder}}
@@ -50,39 +58,39 @@
       ],
       ...
   }
   ```
 
   - `{your_cmd_identifier}` is identifier for calling all cmd command under that identifier. every identifier must be unique
 
-  - `cmd_command_to_run` is the cmd command you want to run. The command is string you usually type in CLI, but in the json file, you separate every command/optional/arguments using comma / ','.
+  - `cmd_command_to_run` is the cmd command you want to run. The command is string you usually type in CLI, but in the json file, you separate every command/optional/arguments using space / ' ' like usual.
 
   - In `cmd_command_to_run`, you can add argument to pass, with type `%{i}` (`i` is index arguments passes)
 
 - Example :
 
   ```json
   "gitACP" : [
-          "git,add,.",
-          "git,commit,-m,%1",
-          "git,push"
+          "git add .",
+          "git commit -m %1",
+          "git push"
       ]
   ```
 
   the identifier to call that command is `gitACP` (command to call git common command `[add, commit, and push]`). under that identifier, we specify all command we want to call
 
-  - `"git add ."` is typed `"git,add,."`
-  - `"git commit -m "{message}" "` is typed `"git,commit,-m,%1"`
+  - `"git add ."`
+  - `"git commit -m "{message}" "` is typed `"git commit -m %1"`
     - `%1` means that the first argument passed when calling that command identifier, will replacing `%1` into the passed string
     - If you just want add same commit message for each commit, you can just change `%1` into your message like `feat: add something`
-  - `"git push"` is typed `"git,push"`
+  - `"git push"`
 
   You can see another command examples in `example_cmd.json`
 
-- There are 2 ways to run this `file`, by CLI with passing `arg` or by hardcode the command in `script`
+- There are 4 ways to run this `file`, by CLI with passing `arg`, by hardcode the command in `script`, or by using `python -m`
 
   - CLI Passing argument :
 
     - After instantiate the class, you can type this code :
 
       ```py
       import sys
@@ -111,14 +119,42 @@
       ```py
 
       cmd.run(["gitACP","feat: add something"])
       ```
 
       to run it, you just need to run `run.py` file
 
+  - Straight from Python module
+
+    It is just as simple as you open the folder that you want to run the command
+
+    ```
+    python -m cmdshelper [command] [args_1] [args_2] ... [args_3]
+    ```
+
+    for example:
+
+    ```
+    python -m cmdshelper gitACP "feat: add something"
+    ```
+
+  - Simply just cdmshelper
+
+    It is just as simple as you open the folder that you want to run the command
+
+    ```
+    cmdshelper [command] [args_1] [args_2] ... [args_3]
+    ```
+
+    for example:
+
+    ```
+    cmdshelper gitACP "feat: add something"
+    ```
+
 - Full code in `run.py ` will be :
 
   ```py
   from cmdshelper.helper import Helper
   import sys
 
   cmd = Helper()
```

