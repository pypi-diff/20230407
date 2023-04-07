# Comparing `tmp/murkrow-0.2.0.tar.gz` & `tmp/murkrow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murkrow-0.2.0.tar", max compression
+gzip compressed data, was "murkrow-0.3.0.tar", max compression
```

## Comparing `murkrow-0.2.0.tar` & `murkrow-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1504 2023-04-06 23:40:21.685931 murkrow-0.2.0/LICENSE
--rw-r--r--   0        0        0     1536 2023-04-06 23:55:12.092008 murkrow-0.2.0/README.md
--rw-r--r--   0        0        0      374 2023-04-07 00:30:55.625174 murkrow-0.2.0/murkrow/__init__.py
--rw-r--r--   0        0        0     2783 2023-04-06 23:40:21.688098 murkrow-0.2.0/murkrow/display.py
--rw-r--r--   0        0        0     1587 2023-04-07 00:18:50.562830 murkrow-0.2.0/murkrow/messaging.py
--rw-r--r--   0        0        0      981 2023-04-07 00:29:36.934709 murkrow-0.2.0/murkrow/murkrow.py
--rw-r--r--   0        0        0     2818 2023-04-07 00:30:55.624980 murkrow-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-04-06 23:40:21.688686 murkrow-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      624 2023-04-07 00:08:40.215618 murkrow-0.2.0/tests/test_murkrow.py
--rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 murkrow-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-06 23:40:21.685931 murkrow-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1536 2023-04-06 23:55:12.092008 murkrow-0.3.0/README.md
+-rw-r--r--   0        0        0      374 2023-04-07 19:34:52.211320 murkrow-0.3.0/murkrow/__init__.py
+-rw-r--r--   0        0        0     3419 2023-04-07 18:17:08.297847 murkrow-0.3.0/murkrow/display.py
+-rw-r--r--   0        0        0     1657 2023-04-07 18:40:38.406623 murkrow-0.3.0/murkrow/messaging.py
+-rw-r--r--   0        0        0     2390 2023-04-07 18:58:56.825050 murkrow-0.3.0/murkrow/murkrow.py
+-rw-r--r--   0        0        0     2849 2023-04-07 19:34:52.211116 murkrow-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-04-06 23:40:21.688686 murkrow-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      624 2023-04-07 00:08:40.215618 murkrow-0.3.0/tests/test_murkrow.py
+-rw-r--r--   0        0        0     2518 1970-01-01 00:00:00.000000 murkrow-0.3.0/PKG-INFO
```

### Comparing `murkrow-0.2.0/LICENSE` & `murkrow-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `murkrow-0.2.0/README.md` & `murkrow-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `murkrow-0.2.0/murkrow/display.py` & `murkrow-0.3.0/murkrow/display.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+"""display.py!
+
+This module provides a `Markdown` class that works similarly to `IPython.display.Markdown` with
+a few extra features.
+
+* The `Markdown`'s display updates in place while messages are appended to it
+* The `Markdown`'s display can be updated from an iterator
+
+"""
+
 import os
 from binascii import hexlify
 from typing import Any, Dict, Iterator, Tuple, Union
 
 from IPython.core import display_functions
 
 
 class Markdown:
-    """
-    A class for displaying a markdown string that can be updated in place.
+    """A class for displaying a markdown string that can be updated in place.
 
     This class provides an easy way to create and update a Markdown string in Jupyter Notebooks. It
     supports real-time updates of Markdown content which is useful for emitting ChatGPT suggestions
     as they are generated.
 
     Attributes:
         message (str): The Markdown string to display
@@ -38,58 +47,65 @@
         >>> markdown.extend(text_generator())
         ```markdown
         Hello world! This is an update! 1 2 3
         ```
     """
 
     def __init__(self, message: str = "") -> None:
+        """Initialize a `Markdown` object with an optional message."""
         self._message: str = message
         self._display_id: str = hexlify(os.urandom(8)).decode('ascii')
 
     def append(self, delta: str) -> None:
+        """Append a string to the `Markdown`."""
         self.message += delta
 
     def extend(self, delta_generator: Iterator[str]) -> None:
+        """Extend the `Markdown` with a generator/iterator of strings."""
         for delta in delta_generator:
             self.append(delta)
 
-    def consume(self, delta_generator: Iterator[str]) -> None:
-        self.extend(delta_generator)
+    # Alias consume
+    consume = extend
 
     def display(self) -> None:
-        '''Display the `Markdown` with a display ID for receiving updates'''
+        """Display the `Markdown` with a display ID for receiving updates."""
         display_functions.display(self, display_id=self._display_id)
 
     def update_displays(self) -> None:
-        '''Force an update to all displays'''
+        """Force an update to all displays of this `Markdown`."""
         display_functions.display(self, display_id=self._display_id, update=True)
 
     @property
     def metadata(self) -> Dict[str, Any]:
+        """Return the metadata for the `Markdown`."""
         return {
             "murkrow": {
                 "default": True,
             }
         }
 
     def __repr__(self) -> str:
+        """Provide a plaintext version of the `Markdown`."""
         message = self._message
         if message is None or message == "":
             message = " "
         return message
 
     def _repr_markdown_(self) -> Union[str, Tuple[str, Dict[str, Any]]]:
+        """Emit our markdown with metadata."""
         message = self._message
         # Handle some platforms that don't support empty Markdown
         if message is None or message == "":
             message = " "
 
         return message, self.metadata
 
     @property
     def message(self) -> str:
+        """Return the `Markdown` message."""
         return self._message
 
     @message.setter
     def message(self, value: str) -> None:
         self._message = value
         self.update_displays()
```

### Comparing `murkrow-0.2.0/pyproject.toml` & `murkrow-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "murkrow"
-version = "0.2.0"
+version = "0.3.0"
 homepage = "https://github.com/rgbkrk/murkrow"
 description = "Markdown for LLMs."
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -19,15 +19,18 @@
 packages = [
     { include = "murkrow" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
+ipython = ">=7, <9"
+openai = "^0.27.4"
 
+[tool.poetry.dev-dependencies]
 black  = { version = "^23.3.0", optional = true}
 isort  = { version = "^5.12.0", optional = true}
 flake8  = { version = "^3.9.2", optional = true}
 flake8-docstrings = { version = "^1.6.0", optional = true }
 mypy = {version = "^0.900", optional = true}
 pytest  = { version = "^6.2.4", optional = true}
 pytest-cov  = { version = "^2.12.0", optional = true}
@@ -40,16 +43,14 @@
 mkdocstrings  = { version = "^0.15.2", optional = true}
 mkdocs-material-extensions  = { version = "^1.0.1", optional = true}
 twine  = { version = "^3.3.0", optional = true}
 mkdocs-autorefs = {version = "^0.2.1", optional = true}
 pre-commit = {version = "^2.12.0", optional = true}
 toml = {version = "^0.10.2", optional = true}
 bump2version = {version = "^1.0.1", optional = true}
-ipython = ">=7, <9"
-openai = "^0.27.4"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "mypy",
```

### Comparing `murkrow-0.2.0/tests/test_murkrow.py` & `murkrow-0.3.0/tests/test_murkrow.py`

 * *Files identical despite different names*

