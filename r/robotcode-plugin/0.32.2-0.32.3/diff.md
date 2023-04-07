# Comparing `tmp/robotcode_plugin-0.32.2.tar.gz` & `tmp/robotcode_plugin-0.32.3.tar.gz`

## Comparing `robotcode_plugin-0.32.2.tar` & `robotcode_plugin-0.32.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/src/robotcode/plugin/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/src/robotcode/plugin/__version__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/src/robotcode/plugin/click_helper.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/src/robotcode/plugin/manager.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/src/robotcode/plugin/py.typed
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/src/robotcode/plugin/specs.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/README.md
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/pyproject.toml
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.2/PKG-INFO
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/src/robotcode/plugin/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/src/robotcode/plugin/__version__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/src/robotcode/plugin/click_helper.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/src/robotcode/plugin/manager.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/src/robotcode/plugin/py.typed
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/src/robotcode/plugin/specs.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/README.md
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/pyproject.toml
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_plugin-0.32.3/PKG-INFO
```

### Comparing `robotcode_plugin-0.32.2/src/robotcode/plugin/__init__.py` & `robotcode_plugin-0.32.3/src/robotcode/plugin/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -109,9 +109,34 @@
                 if self.config.colored_output == ColoredOutput.YES:
                     self.warning('Package "rich" is required to use colored output.')
 
         click.echo(text)
 
         return
 
+    def echo(
+        self, message: Union[str, Callable[[], Any], None], file: Optional[IO[AnyStr]] = None, nl: bool = True
+    ) -> None:
+        click.secho(
+            message() if callable(message) else message,
+            file=file,
+            nl=nl,
+            color=self.colored,
+        )
+
+    def echo_as_markdown(self, text: str) -> None:
+        if self.colored:
+            try:
+                from rich.console import Console
+                from rich.markdown import Markdown
+
+                Console().print(Markdown(text, justify="left"))
+
+                return
+            except ImportError:
+                if self.config.colored_output == ColoredOutput.YES:
+                    self.warning('Package "rich" is required to use colored output.')
+
+        click.echo(text)
+
 
 pass_application = click.make_pass_decorator(Application, ensure=True)
```

### Comparing `robotcode_plugin-0.32.2/src/robotcode/plugin/click_helper.py` & `robotcode_plugin-0.32.3/src/robotcode/plugin/click_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.32.2/src/robotcode/plugin/manager.py` & `robotcode_plugin-0.32.3/src/robotcode/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.32.2/.gitignore` & `robotcode_plugin-0.32.3/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.32.2/LICENSE.txt` & `robotcode_plugin-0.32.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.32.2/README.md` & `robotcode_plugin-0.32.3/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.32.2/pyproject.toml` & `robotcode_plugin-0.32.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.32.2/PKG-INFO` & `robotcode_plugin-0.32.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-plugin
-Version: 0.32.2
+Version: 0.32.3
 Summary: Some classes for RobotCode plugin management
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
 Author-email: Daniel Biehl <dbiehl@live.de>
```

