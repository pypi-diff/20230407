# Comparing `tmp/mcon-0.0.6.tar.gz` & `tmp/mcon-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcon-0.0.6.tar", last modified: Sat Mar 18 22:43:55 2023, max compression
+gzip compressed data, was "mcon-0.0.7.tar", last modified: Fri Apr  7 20:50:28 2023, max compression
```

## Comparing `mcon-0.0.6.tar` & `mcon-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     6416 2023-03-18 22:43:55.347033 mcon-0.0.6/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5731 2023-03-05 14:26:30.700861 mcon-0.0.6/README.md
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1831 2023-03-04 20:32:05.372811 mcon-0.0.6/.gitignore
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      659 2023-03-05 18:20:28.304444 mcon-0.0.6/.pre-commit-config.yaml
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        0 2023-02-17 17:19:34.408808 mcon-0.0.6/mcon/py.typed
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5430 2023-03-04 20:18:49.403493 mcon-0.0.6/tests/run_tests.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5570 2023-03-18 22:19:25.724362 mcon-0.0.6/mcon/builders/pyextension.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    21466 2023-03-18 21:42:30.240372 mcon-0.0.6/mcon/builders/python.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      983 2023-03-06 04:40:04.067826 mcon-0.0.6/mcon/builders/django.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      543 2023-03-05 15:15:43.879300 mcon-0.0.6/mcon/builders/sphinx.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2937 2023-03-04 22:14:13.449507 mcon-0.0.6/mcon/builders/c.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2500 2023-03-18 22:14:34.941204 mcon-0.0.6/mcon/builders/install.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2083 2023-03-04 20:20:46.580783 mcon-0.0.6/mcon/builders/archive.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      302 2023-03-18 22:43:10.574112 mcon-0.0.6/mcon/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     7380 2023-03-18 21:59:25.715336 mcon-0.0.6/mcon/environment.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    11258 2023-03-17 00:12:31.944867 mcon-0.0.6/mcon/entry.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5661 2023-03-18 22:08:14.349072 mcon-0.0.6/mcon/builder.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1595 2023-03-05 22:16:57.253404 mcon-0.0.6/mcon/pybuild.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     6940 2023-03-05 22:38:06.020040 mcon-0.0.6/mcon/main.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    25355 2023-03-18 22:33:05.673268 mcon-0.0.6/mcon/execution.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2066 2023-03-18 22:14:34.933204 mcon-0.0.6/mcon/types.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1290 2023-03-18 22:43:40.890739 mcon-0.0.6/pyproject.toml
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      685 2023-03-05 22:18:11.810166 mcon-0.0.6/construct.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     6416 2023-04-07 20:50:28.941931 mcon-0.0.7/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5731 2023-03-05 14:26:30.700861 mcon-0.0.7/README.md
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1831 2023-03-04 20:32:05.372811 mcon-0.0.7/.gitignore
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      659 2023-03-05 18:20:28.304444 mcon-0.0.7/.pre-commit-config.yaml
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        0 2023-02-17 17:19:34.408808 mcon-0.0.7/mcon/py.typed
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5430 2023-03-04 20:18:49.403493 mcon-0.0.7/tests/run_tests.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5570 2023-03-18 22:19:25.724362 mcon-0.0.7/mcon/builders/pyextension.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    21466 2023-03-18 21:42:30.240372 mcon-0.0.7/mcon/builders/python.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      983 2023-03-06 04:40:04.067826 mcon-0.0.7/mcon/builders/django.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      543 2023-03-05 15:15:43.879300 mcon-0.0.7/mcon/builders/sphinx.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2937 2023-03-04 22:14:13.449507 mcon-0.0.7/mcon/builders/c.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2500 2023-03-18 22:14:34.941204 mcon-0.0.7/mcon/builders/install.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2083 2023-03-04 20:20:46.580783 mcon-0.0.7/mcon/builders/archive.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      302 2023-03-18 22:43:10.574112 mcon-0.0.7/mcon/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7380 2023-03-18 21:59:25.715336 mcon-0.0.7/mcon/environment.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    11543 2023-03-20 13:42:38.457896 mcon-0.0.7/mcon/entry.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5661 2023-03-18 22:08:14.349072 mcon-0.0.7/mcon/builder.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1595 2023-03-05 22:16:57.253404 mcon-0.0.7/mcon/pybuild.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7102 2023-04-07 20:47:34.092627 mcon-0.0.7/mcon/main.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    25355 2023-03-18 22:33:05.673268 mcon-0.0.7/mcon/execution.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2066 2023-03-18 22:14:34.933204 mcon-0.0.7/mcon/types.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1290 2023-04-07 20:49:36.145973 mcon-0.0.7/pyproject.toml
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      685 2023-03-05 22:18:11.810166 mcon-0.0.7/construct.py
```

### Comparing `mcon-0.0.6/PKG-INFO` & `mcon-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcon
-Version: 0.0.6
+Version: 0.0.7
 Summary: Mini software construction and build framework
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Author-Email: Andrew Brown <andrew@brownan.org>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `mcon-0.0.6/README.md` & `mcon-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/.gitignore` & `mcon-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/.pre-commit-config.yaml` & `mcon-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/tests/run_tests.py` & `mcon-0.0.7/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/builders/pyextension.py` & `mcon-0.0.7/mcon/builders/pyextension.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/builders/python.py` & `mcon-0.0.7/mcon/builders/python.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/builders/django.py` & `mcon-0.0.7/mcon/builders/django.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/builders/sphinx.py` & `mcon-0.0.7/mcon/builders/sphinx.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/builders/c.py` & `mcon-0.0.7/mcon/builders/c.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/builders/install.py` & `mcon-0.0.7/mcon/builders/install.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/builders/archive.py` & `mcon-0.0.7/mcon/builders/archive.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/environment.py` & `mcon-0.0.7/mcon/environment.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/entry.py` & `mcon-0.0.7/mcon/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,18 @@
         try:
             entry = env.execution.entries[path]
             if not isinstance(entry, cls):
                 raise TypeError(
                     f"Path {path} already exists but is the wrong type. Expected "
                     f"{cls} got {type(entry)}"
                 )
+            for key, value in kwargs.items():
+                if key not in entry.settable_attributes:
+                    raise ValueError(f"Cannot set property {key} on {cls}")
+                setattr(entry, key, value)
             return entry
         except KeyError:
             pass
 
         entry = super().__call__(env, path, *args, **kwargs)
         env.execution.entries[path] = entry
         return entry
@@ -70,14 +74,18 @@
 class Entry(Node, metaclass=EntryMeta):
     """Represents a file or a directory on the filesystem with a path
 
     The path may or may not exist until it is built. After its builder builds it,
     the path is expected to exist.
     """
 
+    settable_attributes: List[str] = [
+        "leave",
+    ]
+
     def __init__(self, env: "Environment", path: StrPath, *, leave: bool = False):
         super().__init__(env)
         self.path: Path = env.root.joinpath(path)
         self.leave = leave
         self.out_of_date: bool = False
 
     def __hash__(self) -> int:
```

### Comparing `mcon-0.0.6/mcon/builder.py` & `mcon-0.0.7/mcon/builder.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/pybuild.py` & `mcon-0.0.7/mcon/pybuild.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/main.py` & `mcon-0.0.7/mcon/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     root.setLevel(level)
     handler = logging.StreamHandler()
     handler.setFormatter(ColorFormatter(log_format))
     root.addHandler(handler)
 
     construct_path = Path(args["construct"]).resolve()
     execution = Execution(construct_path.parent)
+    execution.update(os.environ)
     execute_construct(
         construct_path,
         execution,
     )
 
     prepared = execution.prepare_build(args["target"])
 
@@ -218,19 +219,23 @@
         else:
             parts.append("├─")
 
     parts.append(name)
 
     print("".join(parts))
     if omit_children:
+        if last_child:
+            new_depth_seq = depth_seq[:-1] + [False, True]
+        else:
+            new_depth_seq = depth_seq + [True]
         _print_line(
             False,
             False,
             False,
-            depth_seq + [depth_seq[-1]],
+            new_depth_seq,
             True,
             "(child nodes shown above)",
             False,
         )
 
 
 if __name__ == "__main__":
```

### Comparing `mcon-0.0.6/mcon/execution.py` & `mcon-0.0.7/mcon/execution.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/mcon/types.py` & `mcon-0.0.7/mcon/types.py`

 * *Files identical despite different names*

### Comparing `mcon-0.0.6/pyproject.toml` & `mcon-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "toml",
     "packaging",
 ]
 backend-path = ["."]
 
 [project]
 name = "mcon"
-version = "0.0.6"
+version = "0.0.7"
 description = "Mini software construction and build framework"
 readme = "README.md"
 authors = [
     {name = "Andrew Brown", email = "andrew@brownan.org"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `mcon-0.0.6/construct.py` & `mcon-0.0.7/construct.py`

 * *Files identical despite different names*

