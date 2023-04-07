# Comparing `tmp/codenames-1.2.3.tar.gz` & `tmp/codenames-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codenames-1.2.3.tar", last modified: Fri Apr  7 15:36:48 2023, max compression
+gzip compressed data, was "codenames-1.2.4.tar", last modified: Fri Apr  7 19:28:54 2023, max compression
```

## Comparing `codenames-1.2.3.tar` & `codenames-1.2.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 15:36:48.926743 codenames-1.2.3/
--rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-07 15:36:48.926743 codenames-1.2.3/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      469 2022-05-18 20:32:47.000000 codenames-1.2.3/README.md
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 15:36:48.918743 codenames-1.2.3/codenames/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-13 11:39:47.000000 codenames-1.2.3/codenames/__init__.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 15:36:48.922743 codenames-1.2.3/codenames/boards/
--rw-rw-r--   0 akali     (1000) akali     (1000)       31 2022-05-13 11:39:47.000000 codenames-1.2.3/codenames/boards/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1941 2023-04-07 13:09:58.000000 codenames-1.2.3/codenames/boards/builder.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6098 2022-05-13 11:39:47.000000 codenames-1.2.3/codenames/boards/english.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6979 2022-05-13 11:39:47.000000 codenames-1.2.3/codenames/boards/hebrew.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 15:36:48.922743 codenames-1.2.3/codenames/game/
--rw-rw-r--   0 akali     (1000) akali     (1000)      160 2022-05-18 21:36:58.000000 codenames-1.2.3/codenames/game/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     8034 2023-04-07 15:36:10.000000 codenames-1.2.3/codenames/game/base.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      470 2022-05-13 11:39:47.000000 codenames-1.2.3/codenames/game/exceptions.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2149 2023-04-07 15:22:55.000000 codenames-1.2.3/codenames/game/player.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     4575 2022-05-13 11:39:47.000000 codenames-1.2.3/codenames/game/runner.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     8881 2023-04-07 15:28:27.000000 codenames-1.2.3/codenames/game/state.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 15:36:48.922743 codenames-1.2.3/codenames/online/
--rw-rw-r--   0 akali     (1000) akali     (1000)       80 2022-05-13 11:39:47.000000 codenames-1.2.3/codenames/online/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)    12980 2023-04-07 13:09:56.000000 codenames-1.2.3/codenames/online/online_adapter.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7634 2023-04-07 13:09:28.000000 codenames-1.2.3/codenames/online/online_game_runner.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1038 2022-05-13 11:39:47.000000 codenames-1.2.3/codenames/online/online_players.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2105 2022-05-13 11:39:47.000000 codenames-1.2.3/codenames/online/utils.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 15:36:48.922743 codenames-1.2.3/codenames/utils/
--rw-rw-r--   0 akali     (1000) akali     (1000)       31 2022-05-18 19:59:48.000000 codenames-1.2.3/codenames/utils/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)       48 2022-05-18 19:59:50.000000 codenames-1.2.3/codenames/utils/logging.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 15:36:48.922743 codenames-1.2.3/codenames.egg-info/
--rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-07 15:36:48.000000 codenames-1.2.3/codenames.egg-info/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      991 2023-04-07 15:36:48.000000 codenames-1.2.3/codenames.egg-info/SOURCES.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-07 15:36:48.000000 codenames-1.2.3/codenames.egg-info/dependency_links.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      114 2023-04-07 15:36:48.000000 codenames-1.2.3/codenames.egg-info/requires.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       16 2023-04-07 15:36:48.000000 codenames-1.2.3/codenames.egg-info/top_level.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      538 2023-04-07 13:12:43.000000 codenames-1.2.3/pyproject.toml
--rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-07 15:36:48.926743 codenames-1.2.3/setup.cfg
--rw-rw-r--   0 akali     (1000) akali     (1000)      556 2023-04-07 15:36:43.000000 codenames-1.2.3/setup.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 15:36:48.922743 codenames-1.2.3/tests/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-18 20:04:04.000000 codenames-1.2.3/tests/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1631 2022-05-18 21:34:44.000000 codenames-1.2.3/tests/board_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      713 2022-05-18 21:34:41.000000 codenames-1.2.3/tests/card_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7925 2022-06-10 19:44:20.000000 codenames-1.2.3/tests/flows_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7931 2023-04-07 13:03:22.000000 codenames-1.2.3/tests/game_runner_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     4701 2023-04-07 12:57:13.000000 codenames-1.2.3/tests/game_state_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      450 2022-05-18 21:34:44.000000 codenames-1.2.3/tests/player_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      645 2022-04-23 20:19:49.000000 codenames-1.2.3/tests/serialization_test.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 15:36:48.926743 codenames-1.2.3/tests/utils/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-02-23 19:10:50.000000 codenames-1.2.3/tests/utils/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     3697 2022-05-18 21:34:41.000000 codenames-1.2.3/tests/utils/constants.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1124 2022-02-23 19:10:50.000000 codenames-1.2.3/tests/utils/hooks.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2577 2022-05-18 21:34:44.000000 codenames-1.2.3/tests/utils/testing_players.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.194429 codenames-1.2.4/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-07 19:28:54.194429 codenames-1.2.4/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      469 2022-05-18 20:32:47.000000 codenames-1.2.4/README.md
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/__init__.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames/boards/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       31 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/boards/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1941 2023-04-07 13:09:58.000000 codenames-1.2.4/codenames/boards/builder.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     6098 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/boards/english.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     6979 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/boards/hebrew.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames/game/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      160 2022-05-18 21:36:58.000000 codenames-1.2.4/codenames/game/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     8034 2023-04-07 15:36:10.000000 codenames-1.2.4/codenames/game/base.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      470 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/game/exceptions.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2228 2023-04-07 19:26:56.000000 codenames-1.2.4/codenames/game/player.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     4575 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/game/runner.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     8881 2023-04-07 15:28:27.000000 codenames-1.2.4/codenames/game/state.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames/online/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       80 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/online/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)    12980 2023-04-07 13:09:56.000000 codenames-1.2.4/codenames/online/online_adapter.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     7634 2023-04-07 13:09:28.000000 codenames-1.2.4/codenames/online/online_game_runner.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1038 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/online/online_players.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2105 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/online/utils.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames/utils/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       31 2022-05-18 19:59:48.000000 codenames-1.2.4/codenames/utils/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)       48 2022-05-18 19:59:50.000000 codenames-1.2.4/codenames/utils/logging.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames.egg-info/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-07 19:28:54.000000 codenames-1.2.4/codenames.egg-info/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      991 2023-04-07 19:28:54.000000 codenames-1.2.4/codenames.egg-info/SOURCES.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-07 19:28:54.000000 codenames-1.2.4/codenames.egg-info/dependency_links.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)      114 2023-04-07 19:28:54.000000 codenames-1.2.4/codenames.egg-info/requires.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)       16 2023-04-07 19:28:54.000000 codenames-1.2.4/codenames.egg-info/top_level.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)      538 2023-04-07 13:12:43.000000 codenames-1.2.4/pyproject.toml
+-rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-07 19:28:54.194429 codenames-1.2.4/setup.cfg
+-rw-rw-r--   0 akali     (1000) akali     (1000)      556 2023-04-07 19:28:26.000000 codenames-1.2.4/setup.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.194429 codenames-1.2.4/tests/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-18 20:04:04.000000 codenames-1.2.4/tests/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1631 2022-05-18 21:34:44.000000 codenames-1.2.4/tests/board_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      713 2022-05-18 21:34:41.000000 codenames-1.2.4/tests/card_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     7925 2022-06-10 19:44:20.000000 codenames-1.2.4/tests/flows_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     7931 2023-04-07 13:03:22.000000 codenames-1.2.4/tests/game_runner_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     4701 2023-04-07 12:57:13.000000 codenames-1.2.4/tests/game_state_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      783 2023-04-07 19:28:08.000000 codenames-1.2.4/tests/player_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      645 2022-04-23 20:19:49.000000 codenames-1.2.4/tests/serialization_test.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.194429 codenames-1.2.4/tests/utils/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-02-23 19:10:50.000000 codenames-1.2.4/tests/utils/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     3697 2022-05-18 21:34:41.000000 codenames-1.2.4/tests/utils/constants.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1124 2022-02-23 19:10:50.000000 codenames-1.2.4/tests/utils/hooks.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2729 2023-04-07 19:28:19.000000 codenames-1.2.4/tests/utils/testing_players.py
```

### Comparing `codenames-1.2.3/PKG-INFO` & `codenames-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codenames
-Version: 1.2.3
+Version: 1.2.4
 Summary: Codenames board game logic implementation in python.
 Home-page: https://github.com/asaf-kali/codenames
 Author: Asaf Kali
 Author-email: akali93@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `codenames-1.2.3/codenames/boards/builder.py` & `codenames-1.2.4/codenames/boards/builder.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/codenames/boards/english.py` & `codenames-1.2.4/codenames/boards/english.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/codenames/boards/hebrew.py` & `codenames-1.2.4/codenames/boards/hebrew.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/codenames/game/base.py` & `codenames-1.2.4/codenames/game/base.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/codenames/game/player.py` & `codenames-1.2.4/codenames/game/player.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,23 +27,24 @@
     def other(self) -> "PlayerRole":
         if self == PlayerRole.HINTER:
             return PlayerRole.GUESSER
         return PlayerRole.HINTER
 
 
 class Player:
-    def __init__(self, name: str):
+    def __init__(self, name: str, team_color: Optional[TeamColor] = None):
         self.name: str = name
-        self.team_color: Optional[TeamColor] = None
+        self.team_color = team_color
 
     def __str__(self):
         team = ""
         if self.team_color:
             team = f" {self.team_color}"
-        return f"{self.name} -{team} {self.role.value}"
+        class_name = self.__class__.__name__
+        return f"{self.name} -{team} {self.role} ({class_name})"
 
     @property
     def role(self) -> PlayerRole:
         raise NotImplementedError()
 
     @property
     def is_human(self) -> bool:
```

### Comparing `codenames-1.2.3/codenames/game/runner.py` & `codenames-1.2.4/codenames/game/runner.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/codenames/game/state.py` & `codenames-1.2.4/codenames/game/state.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/codenames/online/online_adapter.py` & `codenames-1.2.4/codenames/online/online_adapter.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/codenames/online/online_game_runner.py` & `codenames-1.2.4/codenames/online/online_game_runner.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/codenames/online/online_players.py` & `codenames-1.2.4/codenames/online/online_players.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/codenames/online/utils.py` & `codenames-1.2.4/codenames/online/utils.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/codenames.egg-info/PKG-INFO` & `codenames-1.2.4/codenames.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codenames
-Version: 1.2.3
+Version: 1.2.4
 Summary: Codenames board game logic implementation in python.
 Home-page: https://github.com/asaf-kali/codenames
 Author: Asaf Kali
 Author-email: akali93@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `codenames-1.2.3/codenames.egg-info/SOURCES.txt` & `codenames-1.2.4/codenames.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/pyproject.toml` & `codenames-1.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/setup.py` & `codenames-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "beautifultable~=1.0",
 ]
 WEB_DEPS = ["selenium~=4.1"]
 ALL_DEPS = BASE_DEPS + WEB_DEPS
 
 setup(
     name="codenames",
-    version="1.2.3",
+    version="1.2.4",
     description="Codenames board game logic implementation in python.",
     author="Asaf Kali",
     author_email="akali93@gmail.com",
     url="https://github.com/asaf-kali/codenames",
     install_requires=BASE_DEPS,
     extras_require={
         "all": ALL_DEPS,
```

### Comparing `codenames-1.2.3/tests/board_test.py` & `codenames-1.2.4/tests/board_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/tests/card_test.py` & `codenames-1.2.4/tests/card_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/tests/flows_test.py` & `codenames-1.2.4/tests/flows_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/tests/game_runner_test.py` & `codenames-1.2.4/tests/game_runner_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/tests/game_state_test.py` & `codenames-1.2.4/tests/game_state_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/tests/serialization_test.py` & `codenames-1.2.4/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/tests/utils/constants.py` & `codenames-1.2.4/tests/utils/constants.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/tests/utils/hooks.py` & `codenames-1.2.4/tests/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.3/tests/utils/testing_players.py` & `codenames-1.2.4/tests/utils/testing_players.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Iterable, List, NamedTuple, Tuple
+from typing import Dict, Iterable, List, NamedTuple, Optional, Tuple
 
 from codenames.game import (
     Guess,
     Guesser,
     GuesserGameState,
     Hint,
     Hinter,
@@ -20,17 +20,18 @@
 
 
 class TestHinter(Hinter):
     def __init__(
         self,
         hints: Iterable[Hint],
         name: str = "Test Hinter",
+        team_color: Optional[TeamColor] = None,
         auto_quit: bool = False,
     ):
-        super().__init__(name=name)
+        super().__init__(name=name, team_color=team_color)
         self.hints = list(hints)
         self.current_index = 0
         self.auto_quit = auto_quit
 
     def pick_hint(self, game_state: HinterGameState) -> Hint:
         if self.current_index >= len(self.hints):
             if self.auto_quit:
@@ -42,17 +43,18 @@
 
 
 class TestGuesser(Guesser):
     def __init__(
         self,
         guesses: Iterable[Guess],
         name: str = "Test Guesser",
+        team_color: Optional[TeamColor] = None,
         auto_quit: bool = False,
     ):
-        super().__init__(name=name)
+        super().__init__(name=name, team_color=team_color)
         self.guesses = list(guesses)
         self.current_index = 0
         self.auto_quit = auto_quit
 
     def guess(self, game_state: GuesserGameState) -> Guess:
         if self.current_index >= len(self.guesses):
             if self.auto_quit:
```

