# Comparing `tmp/iot-device-0.5.8.tar.gz` & `tmp/iot-device-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iot-device-0.5.8.tar", last modified: Sat Jul 10 03:49:48 2021, max compression
+gzip compressed data, was "iot-device-0.5.9.tar", last modified: Mon Jul 12 23:12:41 2021, max compression
```

## Comparing `iot-device-0.5.8.tar` & `iot-device-0.5.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 iot       (1000) iot       (1001)        0 2021-07-10 03:49:48.406017 iot-device-0.5.8/
--rw-r--r--   0 iot       (1000) iot       (1001)     1063 2021-05-20 01:26:44.000000 iot-device-0.5.8/LICENSE.txt
--rw-r--r--   0 iot       (1000) iot       (1001)       77 2021-05-20 01:26:44.000000 iot-device-0.5.8/MANIFEST.in
--rw-r--r--   0 iot       (1000) iot       (1001)      497 2021-07-10 03:49:48.406017 iot-device-0.5.8/PKG-INFO
--rw-r--r--   0 iot       (1000) iot       (1001)      902 2021-05-20 01:26:44.000000 iot-device-0.5.8/README.md
-drwxr-xr-x   0 iot       (1000) iot       (1001)        0 2021-07-10 03:49:48.402017 iot-device-0.5.8/iot_device/
--rw-r--r--   0 iot       (1000) iot       (1001)      247 2021-06-01 23:37:25.000000 iot-device-0.5.8/iot_device/__init__.py
--rw-r--r--   0 iot       (1000) iot       (1001)     1036 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/certificate.py
--rw-r--r--   0 iot       (1000) iot       (1001)     2362 2021-06-01 23:06:14.000000 iot-device-0.5.8/iot_device/device.py
--rw-r--r--   0 iot       (1000) iot       (1001)     8134 2021-07-10 03:46:47.000000 iot-device-0.5.8/iot_device/device_config.py
--rw-r--r--   0 iot       (1000) iot       (1001)     4938 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/device_registry.py
--rw-r--r--   0 iot       (1000) iot       (1001)     7614 2021-06-01 23:25:29.000000 iot-device-0.5.8/iot_device/device_server.py
--rw-r--r--   0 iot       (1000) iot       (1001)      235 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/discover.py
--rw-r--r--   0 iot       (1000) iot       (1001)     1666 2021-07-01 23:50:34.000000 iot-device-0.5.8/iot_device/discover_mdns.py
--rw-r--r--   0 iot       (1000) iot       (1001)     1041 2021-06-02 00:04:08.000000 iot-device-0.5.8/iot_device/discover_serial.py
--rw-r--r--   0 iot       (1000) iot       (1001)     1964 2021-07-09 22:12:15.000000 iot-device-0.5.8/iot_device/env.py
--rw-r--r--   0 iot       (1000) iot       (1001)     1771 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/eval.py
--rw-r--r--   0 iot       (1000) iot       (1001)      479 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/eval_defaults.py
--rw-r--r--   0 iot       (1000) iot       (1001)     4772 2021-06-30 01:36:55.000000 iot-device-0.5.8/iot_device/eval_file_ops.py
--rw-r--r--   0 iot       (1000) iot       (1001)     4018 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/eval_rlist.py
--rw-r--r--   0 iot       (1000) iot       (1001)     3234 2021-07-09 22:17:02.000000 iot-device-0.5.8/iot_device/eval_rsync.py
--rw-r--r--   0 iot       (1000) iot       (1001)     2131 2021-06-01 23:19:09.000000 iot-device-0.5.8/iot_device/mp_device.py
--rw-r--r--   0 iot       (1000) iot       (1001)     2858 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/mp_protocol.py
--rwxr-xr-x   0 iot       (1000) iot       (1001)    24873 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/pyboard.py
--rw-r--r--   0 iot       (1000) iot       (1001)     3098 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/pydevice.py
--rw-r--r--   0 iot       (1000) iot       (1001)     1647 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/repl_protocol.py
--rw-r--r--   0 iot       (1000) iot       (1001)      229 2021-06-01 23:23:15.000000 iot-device-0.5.8/iot_device/secrets.py
--rw-r--r--   0 iot       (1000) iot       (1001)     1222 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/serial_device.py
--rw-r--r--   0 iot       (1000) iot       (1001)     2257 2021-05-20 01:26:44.000000 iot-device-0.5.8/iot_device/telnet_device.py
--rw-r--r--   0 iot       (1000) iot       (1001)      585 2021-07-09 22:19:33.000000 iot-device-0.5.8/iot_device/utilities.py
--rw-r--r--   0 iot       (1000) iot       (1001)       73 2021-07-10 03:48:08.000000 iot-device-0.5.8/iot_device/version.py
--rw-r--r--   0 iot       (1000) iot       (1001)     1959 2021-06-01 23:20:52.000000 iot-device-0.5.8/iot_device/webrepl_device.py
-drwxr-xr-x   0 iot       (1000) iot       (1001)        0 2021-07-10 03:49:48.406017 iot-device-0.5.8/iot_device.egg-info/
--rw-r--r--   0 iot       (1000) iot       (1001)      497 2021-07-10 03:49:47.000000 iot-device-0.5.8/iot_device.egg-info/PKG-INFO
--rw-r--r--   0 iot       (1000) iot       (1001)      896 2021-07-10 03:49:47.000000 iot-device-0.5.8/iot_device.egg-info/SOURCES.txt
--rw-r--r--   0 iot       (1000) iot       (1001)        1 2021-07-10 03:49:47.000000 iot-device-0.5.8/iot_device.egg-info/dependency_links.txt
--rw-r--r--   0 iot       (1000) iot       (1001)       62 2021-07-10 03:49:47.000000 iot-device-0.5.8/iot_device.egg-info/requires.txt
--rw-r--r--   0 iot       (1000) iot       (1001)       11 2021-07-10 03:49:47.000000 iot-device-0.5.8/iot_device.egg-info/top_level.txt
--rw-r--r--   0 iot       (1000) iot       (1001)        1 2021-07-10 03:49:47.000000 iot-device-0.5.8/iot_device.egg-info/zip-safe
--rw-r--r--   0 iot       (1000) iot       (1001)       38 2021-07-10 03:49:48.406017 iot-device-0.5.8/setup.cfg
--rw-r--r--   0 iot       (1000) iot       (1001)      901 2021-06-02 01:02:01.000000 iot-device-0.5.8/setup.py
+drwxr-xr-x   0 iot       (1000) iot       (1000)        0 2021-07-12 23:12:41.624189 iot-device-0.5.9/
+-rw-r--r--   0 iot       (1000) iot       (1000)     1063 2021-05-20 01:26:44.000000 iot-device-0.5.9/LICENSE.txt
+-rw-r--r--   0 iot       (1000) iot       (1000)       77 2021-05-20 01:26:44.000000 iot-device-0.5.9/MANIFEST.in
+-rw-r--r--   0 iot       (1000) iot       (1000)      497 2021-07-12 23:12:41.624189 iot-device-0.5.9/PKG-INFO
+-rw-r--r--   0 iot       (1000) iot       (1000)      902 2021-05-20 01:26:44.000000 iot-device-0.5.9/README.md
+drwxr-xr-x   0 iot       (1000) iot       (1000)        0 2021-07-12 23:12:41.620190 iot-device-0.5.9/iot_device/
+-rw-r--r--   0 iot       (1000) iot       (1000)      247 2021-06-01 23:37:25.000000 iot-device-0.5.9/iot_device/__init__.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     1036 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/certificate.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     2362 2021-06-01 23:06:14.000000 iot-device-0.5.9/iot_device/device.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     7127 2021-07-10 22:50:48.000000 iot-device-0.5.9/iot_device/device_config.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     4938 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/device_registry.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     7614 2021-06-01 23:25:29.000000 iot-device-0.5.9/iot_device/device_server.py
+-rw-r--r--   0 iot       (1000) iot       (1000)      235 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/discover.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     1666 2021-07-01 23:50:34.000000 iot-device-0.5.9/iot_device/discover_mdns.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     1041 2021-06-02 00:04:08.000000 iot-device-0.5.9/iot_device/discover_serial.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     1190 2021-07-10 18:15:38.000000 iot-device-0.5.9/iot_device/env.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     1771 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/eval.py
+-rw-r--r--   0 iot       (1000) iot       (1000)      479 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/eval_defaults.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     4772 2021-06-30 01:36:55.000000 iot-device-0.5.9/iot_device/eval_file_ops.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     4018 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/eval_rlist.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     3234 2021-07-09 22:17:02.000000 iot-device-0.5.9/iot_device/eval_rsync.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     2131 2021-06-01 23:19:09.000000 iot-device-0.5.9/iot_device/mp_device.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     2858 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/mp_protocol.py
+-rwxr-xr-x   0 iot       (1000) iot       (1000)    24873 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/pyboard.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     3098 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/pydevice.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     1647 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/repl_protocol.py
+-rw-r--r--   0 iot       (1000) iot       (1000)      229 2021-06-01 23:23:15.000000 iot-device-0.5.9/iot_device/secrets.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     1222 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/serial_device.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     2257 2021-05-20 01:26:44.000000 iot-device-0.5.9/iot_device/telnet_device.py
+-rw-r--r--   0 iot       (1000) iot       (1000)      588 2021-07-10 17:47:34.000000 iot-device-0.5.9/iot_device/utilities.py
+-rw-r--r--   0 iot       (1000) iot       (1000)       73 2021-07-10 18:16:06.000000 iot-device-0.5.9/iot_device/version.py
+-rw-r--r--   0 iot       (1000) iot       (1000)     1959 2021-06-01 23:20:52.000000 iot-device-0.5.9/iot_device/webrepl_device.py
+drwxr-xr-x   0 iot       (1000) iot       (1000)        0 2021-07-12 23:12:41.624189 iot-device-0.5.9/iot_device.egg-info/
+-rw-r--r--   0 iot       (1000) iot       (1000)      497 2021-07-12 23:12:41.000000 iot-device-0.5.9/iot_device.egg-info/PKG-INFO
+-rw-r--r--   0 iot       (1000) iot       (1000)      896 2021-07-12 23:12:41.000000 iot-device-0.5.9/iot_device.egg-info/SOURCES.txt
+-rw-r--r--   0 iot       (1000) iot       (1000)        1 2021-07-12 23:12:41.000000 iot-device-0.5.9/iot_device.egg-info/dependency_links.txt
+-rw-r--r--   0 iot       (1000) iot       (1000)       62 2021-07-12 23:12:41.000000 iot-device-0.5.9/iot_device.egg-info/requires.txt
+-rw-r--r--   0 iot       (1000) iot       (1000)       11 2021-07-12 23:12:41.000000 iot-device-0.5.9/iot_device.egg-info/top_level.txt
+-rw-r--r--   0 iot       (1000) iot       (1000)        1 2021-07-12 23:12:41.000000 iot-device-0.5.9/iot_device.egg-info/zip-safe
+-rw-r--r--   0 iot       (1000) iot       (1000)       38 2021-07-12 23:12:41.624189 iot-device-0.5.9/setup.cfg
+-rw-r--r--   0 iot       (1000) iot       (1000)      901 2021-06-02 01:02:01.000000 iot-device-0.5.9/setup.py
```

### Comparing `iot-device-0.5.8/LICENSE.txt` & `iot-device-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/README.md` & `iot-device-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/certificate.py` & `iot-device-0.5.9/iot_device/certificate.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/device.py` & `iot-device-0.5.9/iot_device/device.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/device_config.py` & `iot-device-0.5.9/iot_device/device_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,38 +17,36 @@
     include-patterns: 
         - "./**/*.py"
         - "./**/*.mpy"
         - "./**/"
     exclude-patterns:
         - "boot_out.txt"
         - "/data"
-    libs:    # override IOT_LIBS
-        - $IOT49/libs
-        - iot49/libs
-        - "~"
+    path: $IOT_PROJECTS
     resources:
         - pystone.py: /flash
         - copy.py
         - abc.py:
         - boot: 
-            lib: $IOT49/boards/stm32/code
+            path: my_project/code
             unpack: true
             install-dir: /flash
             include-patterns:
                 - "./**/*.py"
         - boot: 
-            lib: $IOT49/boards/stm32/code
+            lib: ~/my_own_library
             unpack: false
             install-dir: /flash
 
 """
 
 class DeviceConfig:
     
     def __init__(self, name, uid, spec, file):
+        """Not usually called directly. Use get_device_config(s)"""
         self._name = name
         self._uid = uid
         self._spec = spec
         self._file = file
     
     @property
     def name(self):
@@ -58,43 +56,14 @@
     def uid(self):
         return self._uid
 
     @property
     def file(self):
         return self._file
 
-    @property
-    def resource_files(self):
-        """Returns a dict
-           path_on_mcu -> (mtime, size, path_on_host)
-        """
-        result = {}
-        sep = os.path.sep
-        for r in self.resources:
-            for f in r.files:
-                mcu_file = sep.join(f.strip(sep).split(sep)[1:]) if r.unpack else f
-                mcu_path = os.path.join(r.install_dir, mcu_file)
-                host_path = Env.expand_path(os.path.join(r.lib, f))
-                # add folders so rsync won't delete them
-                p = mcu_path
-                while p != '/':
-                    p = os.path.dirname(p)
-                    result[os.path.normpath(p)] = (0, -1, '')
-                # add the file
-                result[mcu_path] = (
-                    os.path.getmtime(host_path), 
-                    os.path.getsize(host_path), 
-                    host_path
-                )            
-        return result
-
-    @property
-    def resources(self):
-        return [ _Resource(self, r) for r in self._spec.get('resources', []) ]
-    
     def __str__(self):
         from io import StringIO
         s = StringIO()
         s.write(f"Configuration (in {self.file}):\n")
         for r in self.resources:
             s.write(f"  {r}\n")
         # s.write(f"    spec:                 {self._spec}\n")
@@ -115,59 +84,66 @@
 
     @staticmethod
     def get_device_configs():
         """Return dict name --> DeviceConfig"""
         result = {}
         names = set()
         uids  = set()
-        for dir in Env.iot_device_dirs():
-            try:
-                with cd(dir):
-                    for file in glob("*.yaml") + glob("*.yml"):
-                        with open(file) as f:
-                            for name, spec in yaml.safe_load(f.read()).items():
-                                if name in names:
-                                    raise ValueError(f"File {file}: device '{name}' redefined")
-                                names.add(name)
-                                uid = spec.get('uid')
-                                if not uid:
-                                    raise ValueError(f"File {file} device '{name}': field 'uid' is mandatory")
-                                uids.add(uid)
-                                result[name] = DeviceConfig(name, uid, spec, file)
-            except FileNotFoundError as e:
-                pass
+        try:
+            with cd(Env.iot_devices()):
+                for file in glob("*.yaml") + glob("*.yml"):
+                    with open(file) as f:
+                        for name, spec in yaml.safe_load(f.read()).items():
+                            if name in names:
+                                raise ValueError(f"File {file}: device '{name}' redefined")
+                            names.add(name)
+                            uid = spec.get('uid')
+                            if not uid:
+                                raise ValueError(f"File {file} device '{name}': field 'uid' is mandatory")
+                            uids.add(uid)
+                            result[name] = DeviceConfig(name, uid, spec, file)
+        except FileNotFoundError as e:
+            # folder Env.iot_devices() does not exist
+            pass
         return result
 
-
-"""Helpers"""
-
-class _Library:
-    """Folder with resources (e.g. Python files or packages, images, etc)"""
-    
-    def __init__(self, path):
-        self._path = path
-        p = Env.expand_path(path)
-        if not os.path.isdir(p):
-            raise ValueError(f"Library: '{path}' @ '{p}' is not a directory")
-        self._resources = os.listdir(p)
-        
-    def has_resource(self, name):
-        return name in self._resources
+    @property
+    def resources(self):
+        return [ _Resource(self, r) for r in self._spec.get('resources', []) ]
     
     @property
-    def path(self):
-        return self._path
-
+    def resource_files(self):
+        """Returns a dict
+           path_on_mcu -> (mtime, size, path_on_host)
+        """
+        result = {}
+        sep = os.path.sep
+        for r in self.resources:
+            for f in r.files:
+                mcu_file = sep.join(f.strip(sep).split(sep)[1:]) if r.unpack else f
+                mcu_path = os.path.join(r.install_dir, mcu_file)
+                host_path = Env.expand_path(os.path.join(r.path, f))
+                # add folders so rsync won't delete them
+                p = mcu_path
+                while p != '/':
+                    p = os.path.dirname(p)
+                    result[os.path.normpath(p)] = (0, -1, '')
+                # add the file
+                result[mcu_path] = (
+                    os.path.getmtime(host_path), 
+                    os.path.getsize(host_path), 
+                    host_path
+                )            
+        return result
 
 class _Resource:
     """Single Resource specified in yaml file"""
 
     def __init__(self, dev, spec):
         self._dev = dev
-        self._libs_cache = {}
         if isinstance(spec, str):
             self._resource = spec
             self._param = {}
         elif isinstance(spec, dict):
             self._resource = next(iter(spec.keys()))
             self._param = spec[self._resource]
             if not self._param:
@@ -187,15 +163,15 @@
     def files(self):
         """List of files in this resource, path relative lib"""
         result = []
         includes = self._param.get('include-patterns', self._dev._spec.get('include-patterns', [ './**/*.py', './**/*.mpy', './**/' ]))
         excludes = self._param.get('exclude-patterns', self._dev._spec.get('exclude-patterns', [ 'boot_out.txt' ]))
         if isinstance(includes, str): includes = [ includes ]
         if isinstance(excludes, str): excludes = [ excludes ]
-        path = os.path.join(self.lib, self.name)
+        path = os.path.join(self.path, self.name)
         if os.path.isfile(Env.expand_path(path)): return [ self.name ]
         try:
             with cd(path):
                 for inc in includes:
                     for file in glob(inc, recursive=True):
                         if not os.path.isfile(file): continue
                         for ex in excludes:
@@ -204,40 +180,32 @@
         except OSError:
             pass
         return result
 
     @property
     def unpack(self):
         """Upload directory (unpack False) or contents (unpack True)"""
-        if hasattr(self._param, 'unpack'):
+        if 'unpack' in self._param:
             return self._param['unpack'] 
-        path = os.path.join(self.lib, self.name)
-        return os.path.isdir(path) and not os.path.isfile(os.path.join(path, '__init__.py'))
+        full_path = os.path.join(self.path, self.name)
+        return os.path.isdir(full_path) and not os.path.isfile(os.path.join(full_path, '__init__.py'))
 
     @property
     def install_dir(self):
         """Directory on mcu in which this resource is located"""
-        d = self._param.get('install-dir', self._dev._spec.get('install-dir', '/lib'))
+        d = self._param.get('install-dir', self._dev._spec.get('install-dir', '/'))
         return d if d.startswith('/') else '/' + d
 
     @property
-    def lib(self):
-        """Library (folder) where this resource is located on the host.
-        Checks libs in order & returns first match."""       
-        for lib_name in self._libs:
-            if not lib_name: continue
-            if not lib_name in self._libs_cache:
-                self._libs_cache[lib_name] = _Library(lib_name)
-            l = self._libs_cache.get(lib_name)
-            if l.has_resource(self.name):
-                return l.path
-        raise ValueError(f"Resource {self.name} not found in libraries {self._libs}")
-
-    @property
-    def _libs(self):
-        """Path of libraries to search for this resource"""
-        libs = self._param.get('lib', self._dev._spec.get('libs', Env.iot_lib_dirs()))
-        return libs if isinstance(libs, list) else [ libs ]
+    def path(self):
+        """Library (folder) where this resource is located on the host."""
+        p = self._param.get('path', self._dev._spec.get('path', Env.iot_projects()))
+        p = Env.expand_path(p)
+        if not os.path.isabs(p):
+            p = os.path.join(Env.iot_projects(), p)
+            p = Env.expand_path(p)
+        return p
 
     def __str__(self):
         # return f"{self.lib}/{self.name} -> {self.install_dir}"
-        return f"Res {self.name:22} install-dir={self.install_dir:22} lib={self.lib}"
+        return f"Res {self.name:22} install-dir={self.install_dir:22} path={self.path}"
+
```

### Comparing `iot-device-0.5.8/iot_device/device_registry.py` & `iot-device-0.5.9/iot_device/device_registry.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/device_server.py` & `iot-device-0.5.9/iot_device/device_server.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/discover_mdns.py` & `iot-device-0.5.9/iot_device/discover_mdns.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/discover_serial.py` & `iot-device-0.5.9/iot_device/discover_serial.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/eval.py` & `iot-device-0.5.9/iot_device/eval.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/eval_file_ops.py` & `iot-device-0.5.9/iot_device/eval_file_ops.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/eval_rlist.py` & `iot-device-0.5.9/iot_device/eval_rlist.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/eval_rsync.py` & `iot-device-0.5.9/iot_device/eval_rsync.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/mp_device.py` & `iot-device-0.5.9/iot_device/mp_device.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/mp_protocol.py` & `iot-device-0.5.9/iot_device/mp_protocol.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/pyboard.py` & `iot-device-0.5.9/iot_device/pyboard.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/pydevice.py` & `iot-device-0.5.9/iot_device/pydevice.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/repl_protocol.py` & `iot-device-0.5.9/iot_device/repl_protocol.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/serial_device.py` & `iot-device-0.5.9/iot_device/serial_device.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/telnet_device.py` & `iot-device-0.5.9/iot_device/telnet_device.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device/utilities.py` & `iot-device-0.5.9/iot_device/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from contextlib import contextmanager
 import sys, os
 
 
 @contextmanager
 def cd(path=None):
     from .env import Env
-    path = path or Env.iot49_dir()
+    path = path or Env.iot_projects()
     cwd = os.getcwd()
     os.chdir(os.path.expandvars(os.path.expanduser(path)))
     try:
         yield
     finally:
         os.chdir(cwd)
```

### Comparing `iot-device-0.5.8/iot_device/webrepl_device.py` & `iot-device-0.5.9/iot_device/webrepl_device.py`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/iot_device.egg-info/SOURCES.txt` & `iot-device-0.5.9/iot_device.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iot-device-0.5.8/setup.py` & `iot-device-0.5.9/setup.py`

 * *Files identical despite different names*

