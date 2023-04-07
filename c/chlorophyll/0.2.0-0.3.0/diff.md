# Comparing `tmp/chlorophyll-0.2.0.tar.gz` & `tmp/chlorophyll-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chlorophyll-0.2.0.tar", last modified: Tue Aug 30 18:10:33 2022, max compression
+gzip compressed data, was "chlorophyll-0.3.0.tar", last modified: Fri Apr  7 16:04:39 2023, max compression
```

## Comparing `chlorophyll-0.2.0.tar` & `chlorophyll-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 bende     (1000) bende     (1000)        0 2022-08-30 18:10:33.463325 chlorophyll-0.2.0/
--rw-r--r--   0 bende     (1000) bende     (1000)     1648 2022-08-30 18:10:33.463325 chlorophyll-0.2.0/PKG-INFO
--rw-r--r--   0 bende     (1000) bende     (1000)      600 2022-07-26 12:39:10.000000 chlorophyll-0.2.0/README.md
-drwxr-xr-x   0 bende     (1000) bende     (1000)        0 2022-08-30 18:10:33.411325 chlorophyll-0.2.0/chlorophyll/
--rw-r--r--   0 bende     (1000) bende     (1000)       31 2022-07-26 12:39:10.000000 chlorophyll-0.2.0/chlorophyll/__init__.py
--rw-r--r--   0 bende     (1000) bende     (1000)     7610 2022-08-30 18:09:50.000000 chlorophyll-0.2.0/chlorophyll/codeview.py
-drwxr-xr-x   0 bende     (1000) bende     (1000)        0 2022-08-30 18:10:33.463325 chlorophyll-0.2.0/chlorophyll/colorschemes/
--rw-r--r--   0 bende     (1000) bende     (1000)     1380 2022-07-26 12:39:10.000000 chlorophyll-0.2.0/chlorophyll/colorschemes/ayu-dark.toml
--rw-r--r--   0 bende     (1000) bende     (1000)     1380 2022-07-26 12:39:10.000000 chlorophyll-0.2.0/chlorophyll/colorschemes/ayu-light.toml
--rw-r--r--   0 bende     (1000) bende     (1000)     1402 2022-07-26 12:39:10.000000 chlorophyll-0.2.0/chlorophyll/colorschemes/dracula.toml
--rw-r--r--   0 bende     (1000) bende     (1000)     1402 2022-08-13 19:44:23.000000 chlorophyll-0.2.0/chlorophyll/colorschemes/mariana.toml
--rw-r--r--   0 bende     (1000) bende     (1000)     1402 2022-07-26 12:39:10.000000 chlorophyll-0.2.0/chlorophyll/colorschemes/monokai.toml
--rw-r--r--   0 bende     (1000) bende     (1000)     4364 2022-07-26 13:18:26.000000 chlorophyll-0.2.0/chlorophyll/schemeparser.py
-drwxr-xr-x   0 bende     (1000) bende     (1000)        0 2022-08-30 18:10:33.431325 chlorophyll-0.2.0/chlorophyll.egg-info/
--rw-r--r--   0 bende     (1000) bende     (1000)     1648 2022-08-30 18:10:33.000000 chlorophyll-0.2.0/chlorophyll.egg-info/PKG-INFO
--rw-r--r--   0 bende     (1000) bende     (1000)      461 2022-08-30 18:10:33.000000 chlorophyll-0.2.0/chlorophyll.egg-info/SOURCES.txt
--rw-r--r--   0 bende     (1000) bende     (1000)        1 2022-08-30 18:10:33.000000 chlorophyll-0.2.0/chlorophyll.egg-info/dependency_links.txt
--rw-r--r--   0 bende     (1000) bende     (1000)       14 2022-08-30 18:10:33.000000 chlorophyll-0.2.0/chlorophyll.egg-info/requires.txt
--rw-r--r--   0 bende     (1000) bende     (1000)       12 2022-08-30 18:10:33.000000 chlorophyll-0.2.0/chlorophyll.egg-info/top_level.txt
--rw-r--r--   0 bende     (1000) bende     (1000)       38 2022-08-30 18:10:33.463325 chlorophyll-0.2.0/setup.cfg
--rw-r--r--   0 bende     (1000) bende     (1000)     1137 2022-08-30 18:10:21.000000 chlorophyll-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:04:39.527256 chlorophyll-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-07 16:04:39.527256 chlorophyll-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:04:39.523256 chlorophyll-0.3.0/chlorophyll/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/codeview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:04:39.527256 chlorophyll-0.3.0/chlorophyll/colorschemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/colorschemes/ayu-dark.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/colorschemes/ayu-light.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/colorschemes/dracula.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/colorschemes/mariana.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/colorschemes/monokai.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/schemeparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:04:39.527256 chlorophyll-0.3.0/chlorophyll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-07 16:04:39.000000 chlorophyll-0.3.0/chlorophyll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-07 16:04:39.000000 chlorophyll-0.3.0/chlorophyll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:04:39.000000 chlorophyll-0.3.0/chlorophyll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 16:04:39.000000 chlorophyll-0.3.0/chlorophyll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 16:04:39.000000 chlorophyll-0.3.0/chlorophyll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:04:39.527256 chlorophyll-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/setup.py
```

### Comparing `chlorophyll-0.2.0/PKG-INFO` & `chlorophyll-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: chlorophyll
-Version: 0.2.0
+Version: 0.3.0
 Summary: A module that fills your code with color - syntax highlighted text box widget for Tkinter.
 Home-page: https://gitlab.com/rdbende/chlorophyll
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
-Description: <h1 align="center">Chlorophyll</h1>
-        
-        A module that fills your code with color - syntax highlighted text box widget for Tkinter.
-        
-        This module is the successor to [`tkcode`](https://github.com/rdbende/tkcode), as it is deprecated - please do not use it anymore.
-        
-        ## Installation
-        
-        `pip install chlorophyll`
-        
-        ## Basic usage
-        Until there's no documentation
-        
-        ```python
-        import tkinter
-        
-        import pygments.lexers
-        from chlorophyll import CodeView
-        
-        root = tkinter.Tk()
-        
-        codeview = CodeView(root, lexer=pygments.lexers.RustLexer, color_scheme="monokai")
-        codeview.pack(fill="both", expand=True)
-        
-        root.mainloop()
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">Chlorophyll</h1>
+
+A module that fills your code with color - syntax highlighted text box widget for Tkinter.
+
+This module is the successor to [`tkcode`](https://github.com/rdbende/tkcode), as it is deprecated - please do not use it anymore.
+
+## Installation
+
+`pip install chlorophyll`
+
+## Basic usage
+Until there's no documentation
+
+```python
+import tkinter
+
+import pygments.lexers
+from chlorophyll import CodeView
+
+root = tkinter.Tk()
+
+codeview = CodeView(root, lexer=pygments.lexers.RustLexer, color_scheme="monokai")
+codeview.pack(fill="both", expand=True)
+
+root.mainloop()
+```
+
+
```

### Comparing `chlorophyll-0.2.0/README.md` & `chlorophyll-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.2.0/chlorophyll/codeview.py` & `chlorophyll-0.3.0/chlorophyll/codeview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import contextlib
 import tkinter
 from pathlib import Path
-from tkinter import ttk
+from tkinter import Event, TclError, ttk
 from tkinter.font import Font
 from typing import Any
 
 import pygments
 import pygments.lexers
 import toml
 
@@ -51,27 +51,34 @@
         )
 
         contmand = "Command" if self._windowingsystem == "aqua" else "Control"
 
         super().bind(f"<{contmand}-c>", self._copy)
         super().bind(f"<{contmand}-v>", self._paste)
         super().bind(f"<{contmand}-a>", self._select_all)
+        super().bind(f"<{contmand}-Shift-Z>", self.redo)
 
         self._orig = f"{self._w}_widget"
         self.tk.call("rename", self._w, self._orig)
         self.tk.createcommand(self._w, self._cmd_proxy)
 
         self._set_lexer(lexer)
         self._set_color_scheme(color_scheme)
 
     def _select_all(self, *_) -> str:
         self.tag_add("sel", "1.0", "end")
         self.mark_set("insert", "end")
         return "break"
 
+    def redo(self, event: Event | None = None) -> None:
+        try:
+            self.edit_redo()
+        except TclError:
+            pass
+
     def _paste(self, *_):
         insert = self.index(f"@0,0 + {self.cget('height') // 2} lines")
 
         with contextlib.suppress(tkinter.TclError):
             self.delete("sel.first", "sel.last")
             self.tag_remove("sel", "1.0", "end")
             self.insert("insert", self.clipboard_get())
```

### Comparing `chlorophyll-0.2.0/chlorophyll/colorschemes/ayu-dark.toml` & `chlorophyll-0.3.0/chlorophyll/colorschemes/ayu-dark.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.2.0/chlorophyll/colorschemes/ayu-light.toml` & `chlorophyll-0.3.0/chlorophyll/colorschemes/ayu-light.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.2.0/chlorophyll/colorschemes/dracula.toml` & `chlorophyll-0.3.0/chlorophyll/colorschemes/dracula.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.2.0/chlorophyll/colorschemes/mariana.toml` & `chlorophyll-0.3.0/chlorophyll/colorschemes/mariana.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.2.0/chlorophyll/colorschemes/monokai.toml` & `chlorophyll-0.3.0/chlorophyll/colorschemes/monokai.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.2.0/chlorophyll/schemeparser.py` & `chlorophyll-0.3.0/chlorophyll/schemeparser.py`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.2.0/chlorophyll.egg-info/PKG-INFO` & `chlorophyll-0.3.0/chlorophyll.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: chlorophyll
-Version: 0.2.0
+Version: 0.3.0
 Summary: A module that fills your code with color - syntax highlighted text box widget for Tkinter.
 Home-page: https://gitlab.com/rdbende/chlorophyll
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
-Description: <h1 align="center">Chlorophyll</h1>
-        
-        A module that fills your code with color - syntax highlighted text box widget for Tkinter.
-        
-        This module is the successor to [`tkcode`](https://github.com/rdbende/tkcode), as it is deprecated - please do not use it anymore.
-        
-        ## Installation
-        
-        `pip install chlorophyll`
-        
-        ## Basic usage
-        Until there's no documentation
-        
-        ```python
-        import tkinter
-        
-        import pygments.lexers
-        from chlorophyll import CodeView
-        
-        root = tkinter.Tk()
-        
-        codeview = CodeView(root, lexer=pygments.lexers.RustLexer, color_scheme="monokai")
-        codeview.pack(fill="both", expand=True)
-        
-        root.mainloop()
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">Chlorophyll</h1>
+
+A module that fills your code with color - syntax highlighted text box widget for Tkinter.
+
+This module is the successor to [`tkcode`](https://github.com/rdbende/tkcode), as it is deprecated - please do not use it anymore.
+
+## Installation
+
+`pip install chlorophyll`
+
+## Basic usage
+Until there's no documentation
+
+```python
+import tkinter
+
+import pygments.lexers
+from chlorophyll import CodeView
+
+root = tkinter.Tk()
+
+codeview = CodeView(root, lexer=pygments.lexers.RustLexer, color_scheme="monokai")
+codeview.pack(fill="both", expand=True)
+
+root.mainloop()
+```
+
+
```

### Comparing `chlorophyll-0.2.0/setup.py` & `chlorophyll-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 
 setup(
     name="chlorophyll",
-    version="0.2.0",
+    version="0.3.0",
     description="A module that fills your code with color - syntax highlighted text box widget for Tkinter.",
     author="rdbende",
     author_email="rdbende@gmail.com",
     url="https://gitlab.com/rdbende/chlorophyll",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["pygments", "toml"],
```

