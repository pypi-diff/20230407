# Comparing `tmp/msgspec-0.9.0.tar.gz` & `tmp/msgspec-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgspec-0.9.0.tar", last modified: Wed Sep 14 01:57:43 2022, max compression
+gzip compressed data, was "msgspec-0.9.1.tar", last modified: Fri Oct 28 01:50:07 2022, max compression
```

## Comparing `msgspec-0.9.0.tar` & `msgspec-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 01:57:43.347200 msgspec-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-09-14 01:57:42.000000 msgspec-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-09-14 01:57:42.000000 msgspec-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4151 2022-09-14 01:57:43.347200 msgspec-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-09-14 01:57:42.000000 msgspec-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 01:57:43.347200 msgspec-0.9.0/msgspec/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)   446150 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/_core.c
--rw-r--r--   0 runner    (1001) docker     (121)    17792 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-09-14 01:57:43.347200 msgspec-0.9.0/msgspec/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    12509 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/atof.h
--rw-r--r--   0 runner    (1001) docker     (121)    36515 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/atof_consts.h
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/common.h
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/msgpack.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    60010 2022-09-14 01:57:42.000000 msgspec-0.9.0/msgspec/ryu.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 01:57:43.347200 msgspec-0.9.0/msgspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4151 2022-09-14 01:57:43.000000 msgspec-0.9.0/msgspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-14 01:57:43.000000 msgspec-0.9.0/msgspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 01:57:43.000000 msgspec-0.9.0/msgspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 01:57:43.000000 msgspec-0.9.0/msgspec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-14 01:57:43.000000 msgspec-0.9.0/msgspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-09-14 01:57:43.347200 msgspec-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-09-14 01:57:42.000000 msgspec-0.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    70238 2022-09-14 01:57:42.000000 msgspec-0.9.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 01:50:07.074549 msgspec-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-10-28 01:50:06.000000 msgspec-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-28 01:50:06.000000 msgspec-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4202 2022-10-28 01:50:07.074549 msgspec-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-10-28 01:50:06.000000 msgspec-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 01:50:07.074549 msgspec-0.9.1/msgspec/
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4151 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)   447024 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/_core.c
+-rw-r--r--   0 runner    (1001) docker     (121)    17792 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-28 01:50:07.074549 msgspec-0.9.1/msgspec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12509 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/atof.h
+-rw-r--r--   0 runner    (1001) docker     (121)    36515 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/atof_consts.h
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/msgpack.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    60010 2022-10-28 01:50:06.000000 msgspec-0.9.1/msgspec/ryu.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 01:50:07.074549 msgspec-0.9.1/msgspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4202 2022-10-28 01:50:07.000000 msgspec-0.9.1/msgspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-28 01:50:07.000000 msgspec-0.9.1/msgspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 01:50:07.000000 msgspec-0.9.1/msgspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 01:50:07.000000 msgspec-0.9.1/msgspec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-28 01:50:07.000000 msgspec-0.9.1/msgspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-10-28 01:50:07.074549 msgspec-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-10-28 01:50:06.000000 msgspec-0.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    70238 2022-10-28 01:50:06.000000 msgspec-0.9.1/versioneer.py
```

### Comparing `msgspec-0.9.0/LICENSE` & `msgspec-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `msgspec-0.9.0/PKG-INFO` & `msgspec-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: msgspec
-Version: 0.9.0
+Version: 0.9.1
 Summary: A fast and friendly JSON/MessagePack library, with optional schema validation
 Home-page: https://jcristharif.com/msgspec/
 Maintainer: Jim Crist-Harif
 Maintainer-email: jcristharif@gmail.com
 License: BSD
 Project-URL: Documentation, https://jcristharif.com/msgspec/
 Project-URL: Source, https://github.com/jcrist/msgspec/
@@ -92,8 +92,9 @@
 Keywords: JSON msgpack Messagepack serialization schema
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `msgspec-0.9.0/README.rst` & `msgspec-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `msgspec-0.9.0/msgspec/__init__.pyi` & `msgspec-0.9.1/msgspec/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 class __StructMeta(type):
     def __new__(
         cls: Type[type], name: str, bases: tuple, classdict: dict
     ) -> "__StructMeta": ...
 
 class Struct(metaclass=__StructMeta):
     __struct_fields__: ClassVar[Tuple[str, ...]]
+    __match_args__: ClassVar[Tuple[str, ...]]
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def __init_subclass__(
         cls,
         tag: Union[None, bool, str, int, Callable[[str], Union[str, int]]] = None,
         tag_field: Union[None, str] = None,
         rename: Union[
             None,
```

### Comparing `msgspec-0.9.0/msgspec/_core.c` & `msgspec-0.9.1/msgspec/_core.c`

 * *Files 0% similar despite different names*

```diff
@@ -11586,14 +11586,15 @@
 
 static PyObject *
 json_decode_datetime(
     JSONDecoderState *self, const char *buf, Py_ssize_t size, PathNode *path
 ) {
     int year, month, day, hour, minute, second, microsecond = 0, offset = 0;
     const char *buf_end = buf + size;
+    bool round_up_micros = false;
     char c;
 
     /* A valid datetime is at least 20 characters in length */
     if (size < 20) goto invalid;
 
     /* Parse date */
     if ((buf = json_read_fixint(buf, 4, &year)) == NULL) goto invalid;
@@ -11614,28 +11615,43 @@
     if ((buf = json_read_fixint(buf, 2, &second)) == NULL) goto invalid;
 
     /* This is the last read that doesn't need a bounds check */
     c = *buf++;
 
     /* Parse decimal if present.
      *
-     * We accept up to 6 decimal digits and error if more are present. We
-     * *could* instead drop the excessive digits and round, but that's more
-     * complicated. Other systems commonly accept 3 or 6 digits, but RFC3339
-     * doesn't specify a decimal precision.  */
+     * Python datetime's only supports microsecond precision, but RFC3339
+     * doesn't specify a decimal precision limit. To work around this we
+     * support infinite decimal digits, but round to the closest microsecond.
+     * This means that nanosecond timestamps won't properly roundtrip through
+     * datetime objects, but there's not much we can do about that. Other
+     * systems commonly accept 3 or 6 digits, support for/usage of nanosecond
+     * precision is rare. */
     if (c == '.') {
         int ndigits = 0;
-        while (buf < buf_end) {
+        while (buf < buf_end && ndigits < 6) {
             c = *buf++;
-            if (!is_digit(c)) break;
+            if (!is_digit(c)) goto end_decimal;
             ndigits++;
-            /* if decimal precision is higher than we support, error */
-            if (ndigits > 6) goto invalid;
             microsecond = microsecond * 10 + (c - '0');
         }
+        c = *buf++;
+        if (is_digit(c)) {
+            /* This timestamp has higher precision than microseconds; parse
+            * the next digit to support rounding, then skip all remaining
+            * digits */
+            if ((c - '0') >= 5) {
+                round_up_micros = true;
+            }
+            while (buf < buf_end) {
+                c = *buf++;
+                if (!is_digit(c)) break;
+            }
+        }
+end_decimal:
         /* Error if no digits after decimal */
         if (ndigits == 0) goto invalid;
         int pow10[6] = {100000, 10000, 1000, 100, 10, 1};
         /* Scale microseconds appropriately */
         microsecond *= pow10[ndigits - 1];
     }
 
@@ -11668,14 +11684,26 @@
     if (year == 0) goto invalid;
     if (month == 0 || month > 12) goto invalid;
     if (day == 0 || day > days_in_month(year, month)) goto invalid;
     if (hour > 23) goto invalid;
     if (minute > 59) goto invalid;
     if (second > 59) goto invalid;
 
+    if (MS_UNLIKELY(round_up_micros)) {
+        microsecond++;
+        if (microsecond == 1000000) {
+            microsecond = 0;
+            second++;
+            if (second == 60) {
+                second = 0;
+                offset--;
+            }
+        }
+    }
+
     if (offset) {
         if (datetime_apply_tz_offset(&year, &month, &day, &hour, &minute, offset) < 0) {
             goto invalid;
         }
     }
     return PyDateTimeAPI->DateTime_FromDateAndTime(
         year, month, day, hour, minute, second, microsecond,
```

### Comparing `msgspec-0.9.0/msgspec/_utils.py` & `msgspec-0.9.1/msgspec/_utils.py`

 * *Files identical despite different names*

### Comparing `msgspec-0.9.0/msgspec/atof.h` & `msgspec-0.9.1/msgspec/atof.h`

 * *Files identical despite different names*

### Comparing `msgspec-0.9.0/msgspec/atof_consts.h` & `msgspec-0.9.1/msgspec/atof_consts.h`

 * *Files identical despite different names*

### Comparing `msgspec-0.9.0/msgspec/common.h` & `msgspec-0.9.1/msgspec/common.h`

 * *Files identical despite different names*

### Comparing `msgspec-0.9.0/msgspec/json.pyi` & `msgspec-0.9.1/msgspec/json.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -29,27 +29,35 @@
     def encode_into(
         self, obj: Any, buffer: bytearray, offset: Optional[int] = 0
     ) -> None: ...
 
 class Decoder(Generic[T]):
     type: Type[T]
     dec_hook: dec_hook_sig
+
     @overload
     def __init__(
         self: Decoder[Any],
         *,
         dec_hook: dec_hook_sig = None,
     ) -> None: ...
     @overload
     def __init__(
         self: Decoder[T],
         type: Type[T] = ...,
         *,
         dec_hook: dec_hook_sig = None,
     ) -> None: ...
+    @overload
+    def __init__(
+        self: Decoder[Any],
+        type: Any = ...,
+        *,
+        dec_hook: dec_hook_sig = None,
+    ) -> None: ...
     def decode(self, data: bytes) -> T: ...
 
 @overload
 def decode(
     buf: bytes,
     *,
     dec_hook: dec_hook_sig = None,
@@ -57,12 +65,19 @@
 @overload
 def decode(
     buf: bytes,
     *,
     type: Type[T] = ...,
     dec_hook: dec_hook_sig = None,
 ) -> T: ...
+@overload
+def decode(
+    buf: bytes,
+    *,
+    type: Any = ...,
+    dec_hook: dec_hook_sig = None,
+) -> Any: ...
 def encode(obj: Any, *, enc_hook: enc_hook_sig = None) -> bytes: ...
 def schema(type: Any) -> Dict[str, Any]: ...
 def schema_components(
     types: Iterable[Any], ref_template: str = "#/$defs/{name}"
 ) -> Tuple[Tuple[Dict[str, Any], ...], Dict[str, Any]]: ...
```

### Comparing `msgspec-0.9.0/msgspec/msgpack.pyi` & `msgspec-0.9.1/msgspec/msgpack.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,22 @@
     def __init__(
         self: Decoder[T],
         type: Type[T] = ...,
         *,
         dec_hook: dec_hook_sig = None,
         ext_hook: ext_hook_sig = None,
     ) -> None: ...
+    @overload
+    def __init__(
+        self: Decoder[Any],
+        type: Any = ...,
+        *,
+        dec_hook: dec_hook_sig = None,
+        ext_hook: ext_hook_sig = None,
+    ) -> None: ...
     def decode(self, data: bytes) -> T: ...
 
 class Encoder:
     enc_hook: enc_hook_sig
     write_buffer_size: int
     def __init__(
         self,
@@ -59,8 +67,16 @@
 def decode(
     buf: bytes,
     *,
     type: Type[T] = ...,
     dec_hook: dec_hook_sig = None,
     ext_hook: ext_hook_sig = None,
 ) -> T: ...
+@overload
+def decode(
+    buf: bytes,
+    *,
+    type: Any = ...,
+    dec_hook: dec_hook_sig = None,
+    ext_hook: ext_hook_sig = None,
+) -> Any: ...
 def encode(obj: Any, *, enc_hook: enc_hook_sig = None) -> bytes: ...
```

### Comparing `msgspec-0.9.0/msgspec/ryu.h` & `msgspec-0.9.1/msgspec/ryu.h`

 * *Files identical despite different names*

### Comparing `msgspec-0.9.0/msgspec.egg-info/PKG-INFO` & `msgspec-0.9.1/msgspec.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: msgspec
-Version: 0.9.0
+Version: 0.9.1
 Summary: A fast and friendly JSON/MessagePack library, with optional schema validation
 Home-page: https://jcristharif.com/msgspec/
 Maintainer: Jim Crist-Harif
 Maintainer-email: jcristharif@gmail.com
 License: BSD
 Project-URL: Documentation, https://jcristharif.com/msgspec/
 Project-URL: Source, https://github.com/jcrist/msgspec/
@@ -92,8 +92,9 @@
 Keywords: JSON msgpack Messagepack serialization schema
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `msgspec-0.9.0/setup.cfg` & `msgspec-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `msgspec-0.9.0/setup.py` & `msgspec-0.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     keywords="JSON msgpack Messagepack serialization schema",
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     license="BSD",
     packages=["msgspec"],
     package_data={"msgspec": ["py.typed", "*.pyi"]},
     ext_modules=ext_modules,
     long_description=(
         open("README.rst", encoding="utf-8").read()
```

### Comparing `msgspec-0.9.0/versioneer.py` & `msgspec-0.9.1/versioneer.py`

 * *Files identical despite different names*

