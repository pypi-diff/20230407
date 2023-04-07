# Comparing `tmp/avasar-0.6.0.tar.gz` & `tmp/avasar-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avasar-0.6.0.tar", max compression
+gzip compressed data, was "avasar-0.7.0.tar", max compression
```

## Comparing `avasar-0.6.0.tar` & `avasar-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0        0 2023-03-05 22:20:25.812195 avasar-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-03-06 12:07:52.085967 avasar-0.6.0/avasar/__init__.py
--rw-r--r--   0        0        0       28 2023-03-06 16:54:29.691949 avasar-0.6.0/avasar/__main__.py
--rw-r--r--   0        0        0     2075 2023-03-07 14:21:39.208663 avasar-0.6.0/avasar/data/blades.toml
--rw-r--r--   0        0        0    35236 2023-03-06 15:42:15.961145 avasar-0.6.0/avasar/data/firstname-english-female.toml
--rw-r--r--   0        0        0    26690 2023-03-06 15:41:34.137528 avasar-0.6.0/avasar/data/firstname-english-male.toml
--rw-r--r--   0        0        0     7542 2023-03-06 15:41:44.906625 avasar-0.6.0/avasar/data/firstname-german-female.toml
--rw-r--r--   0        0        0     7884 2023-03-06 15:41:14.424307 avasar-0.6.0/avasar/data/firstname-german-male.toml
--rw-r--r--   0        0        0    14297 2023-03-06 17:26:54.618482 avasar-0.6.0/avasar/data/lastname-english.toml
--rw-r--r--   0        0        0    25462 2023-03-06 17:26:07.218468 avasar-0.6.0/avasar/data/lastname-german.toml
--rw-r--r--   0        0        0      851 2023-03-06 21:05:01.348209 avasar-0.6.0/avasar/data/person.py
--rw-r--r--   0        0        0     9818 2023-03-07 19:07:57.233638 avasar-0.6.0/avasar/data/person.toml
--rw-r--r--   0        0        0     9279 2023-03-07 18:35:49.554679 avasar-0.6.0/avasar/dsl.py
--rw-r--r--   0        0        0      922 2023-03-07 14:08:48.651738 avasar-0.6.0/avasar/main.py
--rw-r--r--   0        0        0      761 2023-03-07 19:08:25.929028 avasar-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 avasar-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-05 22:20:25.812195 avasar-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-06 12:07:52.085967 avasar-0.7.0/avasar/__init__.py
+-rw-r--r--   0        0        0       28 2023-03-06 16:54:29.691949 avasar-0.7.0/avasar/__main__.py
+-rw-r--r--   0        0        0     2056 2023-03-10 15:32:27.684561 avasar-0.7.0/avasar/data/blades.toml
+-rw-r--r--   0        0        0    35236 2023-03-06 15:42:15.961145 avasar-0.7.0/avasar/data/firstname-english-female.toml
+-rw-r--r--   0        0        0    26690 2023-03-06 15:41:34.137528 avasar-0.7.0/avasar/data/firstname-english-male.toml
+-rw-r--r--   0        0        0     7542 2023-03-06 15:41:44.906625 avasar-0.7.0/avasar/data/firstname-german-female.toml
+-rw-r--r--   0        0        0     7884 2023-03-06 15:41:14.424307 avasar-0.7.0/avasar/data/firstname-german-male.toml
+-rw-r--r--   0        0        0    14297 2023-03-06 17:26:54.618482 avasar-0.7.0/avasar/data/lastname-english.toml
+-rw-r--r--   0        0        0    25462 2023-03-06 17:26:07.218468 avasar-0.7.0/avasar/data/lastname-german.toml
+-rw-r--r--   0        0        0      851 2023-03-06 21:05:01.348209 avasar-0.7.0/avasar/data/person.py
+-rw-r--r--   0        0        0     9824 2023-03-10 15:29:59.807367 avasar-0.7.0/avasar/data/person.toml
+-rw-r--r--   0        0        0     3079 2023-04-07 19:28:33.599285 avasar-0.7.0/avasar/data/places.toml
+-rw-r--r--   0        0        0    10442 2023-04-07 19:58:18.751725 avasar-0.7.0/avasar/dsl.py
+-rw-r--r--   0        0        0      922 2023-04-07 16:00:11.905943 avasar-0.7.0/avasar/main.py
+-rw-r--r--   0        0        0      761 2023-04-07 20:02:49.401173 avasar-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 avasar-0.7.0/PKG-INFO
```

### Comparing `avasar-0.6.0/avasar/data/blades.toml` & `avasar-0.7.0/avasar/data/blades.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [[avasar]]
 name = "gen.character.blades"
 items = ["""
-\\s         Playbook | {words.blades.playbook.choice.capitalize}
-        Background | {words.blades.background.choice.capitalize}
-          Heritage | {words.blades.heritage.choice.capitalize}
-              Vice | {words.blades.vice.choice.capitalize}
+\\s         Playbook | {words.blades.playbook.choice}
+        Background | {words.blades.background.choice}
+          Heritage | {words.blades.heritage.choice}
+              Vice | {words.blades.vice.choice}
 """]
 
 [[avasar]]
 name = "gen.character.blades.kitsch"
-items = ["""
-{gen.character.blades}
+items = ["""\\s
  
+Name | Value
+-|-
+{gen.character.blades}
+ |  
 {gen.character.kitsch}
 """]
 
 [[avasar]]
 name = "words.blades.background"
 items = """
 academic
```

### Comparing `avasar-0.6.0/avasar/data/firstname-english-female.toml` & `avasar-0.7.0/avasar/data/firstname-english-female.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.6.0/avasar/data/firstname-english-male.toml` & `avasar-0.7.0/avasar/data/firstname-english-male.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.6.0/avasar/data/firstname-german-female.toml` & `avasar-0.7.0/avasar/data/firstname-german-female.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.6.0/avasar/data/firstname-german-male.toml` & `avasar-0.7.0/avasar/data/firstname-german-male.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.6.0/avasar/data/lastname-english.toml` & `avasar-0.7.0/avasar/data/lastname-english.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.6.0/avasar/data/lastname-german.toml` & `avasar-0.7.0/avasar/data/lastname-german.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.6.0/avasar/data/person.py` & `avasar-0.7.0/avasar/data/person.py`

 * *Files identical despite different names*

### Comparing `avasar-0.6.0/avasar/data/person.toml` & `avasar-0.7.0/avasar/data/person.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [[avasar]]
 name = "gen.character.kitsch"
 items = ["""
 \\s        Firstname | {words.firstname}
           Lastname | {words.lastname}
- 
+ | 
               Body | {words.person.body}
             Weight | {words.person.weight}
        Eye - Color | {words.person.eye.color}
       Hair - Color | {words.person.hair.color}
               Nose | {words.person.nose}
- 
+ | 
                Eye | {words.person.eye}
           Eyebrows | {words.person.eye.brows}
               Face | {words.person.face}
       Face - Cheek | {words.person.face.cheek}
        Face - Chin | {words.person.face.chin}
        Facial hair | {words.person.face.facial_hair}
       Hair - Style | {words.person.hair.style}
         Hair - Ext | {words.person.hair.style.ext}
         Skin Color | {words.person.skin.color}
- 
+ | 
              Cloth | {words.person.cloth.style}
     Cloth - Bottom | {words.person.cloth.bottom}
        Cloth - Top | {words.person.cloth.top}
      Cloth - Shoes | {words.person.cloth.shoes}
 Cloth - Accesories | {words.person.cloth.accesories}
        Cloth - Hat | {words.person.cloth.hat}
 """]
```

### Comparing `avasar-0.6.0/avasar/dsl.py` & `avasar-0.7.0/avasar/dsl.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,48 +10,69 @@
 _base = Path(__file__).parent
 _data = Path(_base, "data")
 
 # TODO: introduce conditionals
 # TODO: system for probability (using indexes and normal-distribution random value
 
 
+def cleanup(text):
+    return text.replace("]", "").replace("[", "")
+
+
 @dataclass
 class TransparentString:
     value: str
 
     def __repr__(self):
-        return self.value
+        return self.__str__()
 
     def __str__(self):
-        return self.value
+        return cleanup(self.value)
 
 
 class All:
     @property
-    def all(self):
+    def all_items(self):
         result = []
         size = 0
         for name in self._all.keys():
             size = max(size, len(name))
         for name, value in self._all.items():
             name = name.rjust(size)
-            result.append(f"{name} | {value.count.capitalize}")
-        return TransparentString("\n".join(result))
+            output = ",".join(value.count.capitalize._strings)
+            result.append(f"{name} | {output}")
+        c = self._get_context()
+        return Items(c, Config(), result)
+
+    @property
+    def all_short(self):
+        return self.all_items.short.column
+
+    @property
+    def all(self):
+        return self.all_items.column
 
 
 @dataclass
 class Namespace(All):
+    _context: "Context"
     _all: dict[str, "Text"] = field(default_factory=dict)
 
+    def _get_context(self):
+        return self._context
+
 
 @dataclass
 class Context(All):
     _groups: Optional[list[frozenset[str]]] = None
     _all: dict[str, "Text"] = field(default_factory=dict)
 
+    def _get_context(self):
+        return self
+
     def _set_groups(self, *args):
         groups = set()
         for group in args:
             if isinstance(group, str):
                 group = frozenset([group])
             elif isinstance(group, set):
                 group = frozenset(group)
@@ -113,15 +134,23 @@
         )
 
     @property
     def capitalize(self):
         return Items(
             _context=self._context,
             _config=self._config,
-            _items=[capitalize(x) for x in self._strings],
+            _items=[capitalize(self._context.fstr(x)) for x in self._strings],
+        )
+
+    @property
+    def short(self):
+        return Items(
+            _context=self._context,
+            _config=self._config,
+            _items=[short(x) for x in self._strings],
         )
 
     def __repr__(self):
         return self.__str__()
 
 
 @dataclass
@@ -134,20 +163,25 @@
     def _strings(self):
         return self._items
 
     @property
     def strings(self):
         return list(self._items)
 
+    @property
+    def column(self):
+        return TransparentString(self._context.fstr("\n".join(self._strings)))
+
     def __str__(self):
         items = self._strings
         if any([("\n" in x) for x in items]):
-            return self._context.fstr("\n-\n".join(self._strings))
+            result = "\n-\n".join(self._strings)
         else:
-            return self._context.fstr(", ".join(self._strings))
+            result = ", ".join(self._strings)
+        return cleanup(self._context.fstr(result))
 
     def __repr__(self):
         return self.__str__()
 
 
 class Distribution:
     STANDARD = 0
@@ -164,14 +198,17 @@
 class Text(Transform, All):
     name: str
     _context: Context
     _config: Config
     _items: dict[frozenset, list[str]]
     _all: dict[str, "Text"] = field(default_factory=dict)
 
+    def _get_context(self):
+        return self._context
+
     def _groups(self, *args):
         groups = set()
         for group in args:
             if isinstance(group, str):
                 group = frozenset([group])
             elif isinstance(group, set):
                 group = frozenset(group)
@@ -181,15 +218,15 @@
             result.extend(self._items[group])
         result = list(sorted(set(result)))
         return result
 
     def groups(self, *args):
         return Items(
             _context=self._context,
-            _config=self.config,
+            _config=self._config,
             _items=self._groups(*args),
         )
 
     def _groups_from_items(self):
         return frozenset(self._items.keys())
 
     @property
@@ -229,14 +266,27 @@
     def __str__(self):
         return str(self.count)
 
     def __repr__(self):
         return self.__str__()
 
 
+def short(string):
+    parts = string.split("[")
+    new = []
+    for part in parts:
+        a, ok, b = part.partition("]")
+        if ok:
+            new.append(b)
+        else:
+            new.append(f"{a}{b}")
+
+    return "".join(new)
+
+
 def capitalize(string):
     if len(string) > 0:
         return f"{string[0].upper()}{string[1:]}"
     else:
         return string
 
 
@@ -257,15 +307,15 @@
     for x in parts[:-1]:
         if all and isinstance(value, Text):
             cur._all[niceup_name(value.name[prefix:])] = value
             prefix += len(x) + 1
         if hasattr(cur, x):
             cur = getattr(cur, x)
         else:
-            new = Namespace()
+            new = Namespace(context)
             setattr(cur, x, new)
             cur = new
     try:
         if all and isinstance(value, Text):
             cur._all[niceup_name(value.name[prefix:])] = value
         if all:
             value._all[niceup_name(value.name[prefix:])] = value
@@ -322,26 +372,27 @@
                 else:
                     for comb in combs:
                         map[name][comb].extend(avasar["items"])
                     map[name][_default].extend(avasar["items"])
     for name in sorted(map.keys()):
         groups = map[name]
         group = defaultdict(list)
+        all_ = group["_all"] = {}
         for key, item in groups.items():
             item = list(sorted(set(item)))
             groups[key] = item
             if isinstance(key, frozenset) and len(key) == 1:
                 gr_name = list(key)[0]
-                group[gr_name] = Text(
+                all_[niceup_name(gr_name)] = group[gr_name] = Text(
                     name=name,
                     _context=context,
                     _config=configs[name],
                     _items={_default: item},
                 )
-        ns = Namespace()
+        ns = Namespace(context)
         ns.__dict__ = group
         obj = Text(
             name=name,
             _context=context,
             _config=configs[name],
             _items=groups,
         )
```

### Comparing `avasar-0.6.0/avasar/main.py` & `avasar-0.7.0/avasar/main.py`

 * *Files identical despite different names*

### Comparing `avasar-0.6.0/pyproject.toml` & `avasar-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avasar"
-version = "0.6.0"
+version = "0.7.0"
 description = "Text generation DSL in python"
 authors = ["Streampunk <glad.car1474@fastmail.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `avasar-0.6.0/PKG-INFO` & `avasar-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avasar
-Version: 0.6.0
+Version: 0.7.0
 Summary: Text generation DSL in python
 License: AGPL-3.0-or-later
 Author: Streampunk
 Author-email: glad.car1474@fastmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

