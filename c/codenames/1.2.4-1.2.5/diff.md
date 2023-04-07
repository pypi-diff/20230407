# Comparing `tmp/codenames-1.2.4.tar.gz` & `tmp/codenames-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codenames-1.2.4.tar", last modified: Fri Apr  7 19:28:54 2023, max compression
+gzip compressed data, was "codenames-1.2.5.tar", last modified: Fri Apr  7 21:16:00 2023, max compression
```

## Comparing `codenames-1.2.4.tar` & `codenames-1.2.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.194429 codenames-1.2.4/
--rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-07 19:28:54.194429 codenames-1.2.4/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      469 2022-05-18 20:32:47.000000 codenames-1.2.4/README.md
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/__init__.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames/boards/
--rw-rw-r--   0 akali     (1000) akali     (1000)       31 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/boards/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1941 2023-04-07 13:09:58.000000 codenames-1.2.4/codenames/boards/builder.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6098 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/boards/english.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6979 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/boards/hebrew.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames/game/
--rw-rw-r--   0 akali     (1000) akali     (1000)      160 2022-05-18 21:36:58.000000 codenames-1.2.4/codenames/game/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     8034 2023-04-07 15:36:10.000000 codenames-1.2.4/codenames/game/base.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      470 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/game/exceptions.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2228 2023-04-07 19:26:56.000000 codenames-1.2.4/codenames/game/player.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     4575 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/game/runner.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     8881 2023-04-07 15:28:27.000000 codenames-1.2.4/codenames/game/state.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames/online/
--rw-rw-r--   0 akali     (1000) akali     (1000)       80 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/online/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)    12980 2023-04-07 13:09:56.000000 codenames-1.2.4/codenames/online/online_adapter.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7634 2023-04-07 13:09:28.000000 codenames-1.2.4/codenames/online/online_game_runner.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1038 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/online/online_players.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2105 2022-05-13 11:39:47.000000 codenames-1.2.4/codenames/online/utils.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames/utils/
--rw-rw-r--   0 akali     (1000) akali     (1000)       31 2022-05-18 19:59:48.000000 codenames-1.2.4/codenames/utils/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)       48 2022-05-18 19:59:50.000000 codenames-1.2.4/codenames/utils/logging.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.190429 codenames-1.2.4/codenames.egg-info/
--rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-07 19:28:54.000000 codenames-1.2.4/codenames.egg-info/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      991 2023-04-07 19:28:54.000000 codenames-1.2.4/codenames.egg-info/SOURCES.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-07 19:28:54.000000 codenames-1.2.4/codenames.egg-info/dependency_links.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      114 2023-04-07 19:28:54.000000 codenames-1.2.4/codenames.egg-info/requires.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       16 2023-04-07 19:28:54.000000 codenames-1.2.4/codenames.egg-info/top_level.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      538 2023-04-07 13:12:43.000000 codenames-1.2.4/pyproject.toml
--rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-07 19:28:54.194429 codenames-1.2.4/setup.cfg
--rw-rw-r--   0 akali     (1000) akali     (1000)      556 2023-04-07 19:28:26.000000 codenames-1.2.4/setup.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.194429 codenames-1.2.4/tests/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-18 20:04:04.000000 codenames-1.2.4/tests/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1631 2022-05-18 21:34:44.000000 codenames-1.2.4/tests/board_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      713 2022-05-18 21:34:41.000000 codenames-1.2.4/tests/card_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7925 2022-06-10 19:44:20.000000 codenames-1.2.4/tests/flows_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7931 2023-04-07 13:03:22.000000 codenames-1.2.4/tests/game_runner_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     4701 2023-04-07 12:57:13.000000 codenames-1.2.4/tests/game_state_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      783 2023-04-07 19:28:08.000000 codenames-1.2.4/tests/player_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      645 2022-04-23 20:19:49.000000 codenames-1.2.4/tests/serialization_test.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 19:28:54.194429 codenames-1.2.4/tests/utils/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-02-23 19:10:50.000000 codenames-1.2.4/tests/utils/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     3697 2022-05-18 21:34:41.000000 codenames-1.2.4/tests/utils/constants.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1124 2022-02-23 19:10:50.000000 codenames-1.2.4/tests/utils/hooks.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2729 2023-04-07 19:28:19.000000 codenames-1.2.4/tests/utils/testing_players.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 21:16:00.901917 codenames-1.2.5/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-07 21:16:00.901917 codenames-1.2.5/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      469 2022-05-18 20:32:47.000000 codenames-1.2.5/README.md
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 21:16:00.897917 codenames-1.2.5/codenames/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-13 11:39:47.000000 codenames-1.2.5/codenames/__init__.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 21:16:00.897917 codenames-1.2.5/codenames/boards/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       31 2022-05-13 11:39:47.000000 codenames-1.2.5/codenames/boards/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1941 2023-04-07 13:09:58.000000 codenames-1.2.5/codenames/boards/builder.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     6098 2022-05-13 11:39:47.000000 codenames-1.2.5/codenames/boards/english.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     6979 2022-05-13 11:39:47.000000 codenames-1.2.5/codenames/boards/hebrew.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 21:16:00.897917 codenames-1.2.5/codenames/game/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      160 2022-05-18 21:36:58.000000 codenames-1.2.5/codenames/game/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     8034 2023-04-07 15:36:10.000000 codenames-1.2.5/codenames/game/base.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      470 2022-05-13 11:39:47.000000 codenames-1.2.5/codenames/game/exceptions.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2228 2023-04-07 19:26:56.000000 codenames-1.2.5/codenames/game/player.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     4575 2022-05-13 11:39:47.000000 codenames-1.2.5/codenames/game/runner.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     8953 2023-04-07 21:15:10.000000 codenames-1.2.5/codenames/game/state.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 21:16:00.901917 codenames-1.2.5/codenames/online/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       80 2022-05-13 11:39:47.000000 codenames-1.2.5/codenames/online/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)    12980 2023-04-07 13:09:56.000000 codenames-1.2.5/codenames/online/online_adapter.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     7634 2023-04-07 13:09:28.000000 codenames-1.2.5/codenames/online/online_game_runner.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1038 2022-05-13 11:39:47.000000 codenames-1.2.5/codenames/online/online_players.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2105 2022-05-13 11:39:47.000000 codenames-1.2.5/codenames/online/utils.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 21:16:00.901917 codenames-1.2.5/codenames/utils/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       31 2022-05-18 19:59:48.000000 codenames-1.2.5/codenames/utils/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)       48 2022-05-18 19:59:50.000000 codenames-1.2.5/codenames/utils/logging.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 21:16:00.897917 codenames-1.2.5/codenames.egg-info/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-07 21:16:00.000000 codenames-1.2.5/codenames.egg-info/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      991 2023-04-07 21:16:00.000000 codenames-1.2.5/codenames.egg-info/SOURCES.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-07 21:16:00.000000 codenames-1.2.5/codenames.egg-info/dependency_links.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)      114 2023-04-07 21:16:00.000000 codenames-1.2.5/codenames.egg-info/requires.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)       16 2023-04-07 21:16:00.000000 codenames-1.2.5/codenames.egg-info/top_level.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)      538 2023-04-07 13:12:43.000000 codenames-1.2.5/pyproject.toml
+-rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-07 21:16:00.901917 codenames-1.2.5/setup.cfg
+-rw-rw-r--   0 akali     (1000) akali     (1000)      556 2023-04-07 21:15:27.000000 codenames-1.2.5/setup.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 21:16:00.901917 codenames-1.2.5/tests/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-18 20:04:04.000000 codenames-1.2.5/tests/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1631 2022-05-18 21:34:44.000000 codenames-1.2.5/tests/board_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      713 2022-05-18 21:34:41.000000 codenames-1.2.5/tests/card_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     7925 2022-06-10 19:44:20.000000 codenames-1.2.5/tests/flows_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     7931 2023-04-07 13:03:22.000000 codenames-1.2.5/tests/game_runner_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     4701 2023-04-07 12:57:13.000000 codenames-1.2.5/tests/game_state_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      783 2023-04-07 19:28:08.000000 codenames-1.2.5/tests/player_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      645 2022-04-23 20:19:49.000000 codenames-1.2.5/tests/serialization_test.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-07 21:16:00.901917 codenames-1.2.5/tests/utils/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-02-23 19:10:50.000000 codenames-1.2.5/tests/utils/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     3697 2022-05-18 21:34:41.000000 codenames-1.2.5/tests/utils/constants.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1124 2022-02-23 19:10:50.000000 codenames-1.2.5/tests/utils/hooks.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2729 2023-04-07 19:28:19.000000 codenames-1.2.5/tests/utils/testing_players.py
```

### Comparing `codenames-1.2.4/PKG-INFO` & `codenames-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codenames
-Version: 1.2.4
+Version: 1.2.5
 Summary: Codenames board game logic implementation in python.
 Home-page: https://github.com/asaf-kali/codenames
 Author: Asaf Kali
 Author-email: akali93@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `codenames-1.2.4/codenames/boards/builder.py` & `codenames-1.2.5/codenames/boards/builder.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/codenames/boards/english.py` & `codenames-1.2.5/codenames/boards/english.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/codenames/boards/hebrew.py` & `codenames-1.2.5/codenames/boards/hebrew.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/codenames/game/base.py` & `codenames-1.2.5/codenames/game/base.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/codenames/game/player.py` & `codenames-1.2.5/codenames/game/player.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/codenames/game/runner.py` & `codenames-1.2.5/codenames/game/runner.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/codenames/game/state.py` & `codenames-1.2.5/codenames/game/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,24 +102,25 @@
         values["score"] = score
         return values
 
     @property
     def hinter_state(self) -> "HinterGameState":
         return HinterGameState(
             board=self.board,
+            score=self.score,
             current_team_color=self.current_team_color,
             given_hints=self.given_hints,
             given_guesses=self.given_guesses,
         )
 
     @property
     def guesser_state(self) -> "GuesserGameState":
-        board = self.board.censured
         return GuesserGameState(
-            board=board,
+            board=self.board.censured,
+            score=self.score,
             current_team_color=self.current_team_color,
             given_hints=self.given_hints,
             given_guesses=self.given_guesses,
             left_guesses=self.left_guesses,
             bonus_given=self.bonus_given,
         )
 
@@ -229,14 +230,15 @@
         game_ended = self.score.add_point(score_team_color)
         if game_ended:
             self.winner = Winner(team_color=score_team_color, reason=WinningReason.TARGET_SCORE_REACHED)
 
 
 class HinterGameState(BaseModel):
     board: Board
+    score: Score
     current_team_color: TeamColor
     given_hints: List[GivenHint]
     given_guesses: List[GivenGuess]
 
     @cached_property
     def given_hint_words(self) -> WordGroup:
         return tuple(hint.formatted_word for hint in self.given_hints)
@@ -244,14 +246,15 @@
     @cached_property
     def illegal_words(self) -> WordGroup:
         return *self.board.all_words, *self.given_hint_words
 
 
 class GuesserGameState(BaseModel):
     board: Board
+    score: Score
     current_team_color: TeamColor
     given_hints: List[GivenHint]
     given_guesses: List[GivenGuess]
     left_guesses: int
     bonus_given: bool
 
     @cached_property
```

### Comparing `codenames-1.2.4/codenames/online/online_adapter.py` & `codenames-1.2.5/codenames/online/online_adapter.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/codenames/online/online_game_runner.py` & `codenames-1.2.5/codenames/online/online_game_runner.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/codenames/online/online_players.py` & `codenames-1.2.5/codenames/online/online_players.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/codenames/online/utils.py` & `codenames-1.2.5/codenames/online/utils.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/codenames.egg-info/PKG-INFO` & `codenames-1.2.5/codenames.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codenames
-Version: 1.2.4
+Version: 1.2.5
 Summary: Codenames board game logic implementation in python.
 Home-page: https://github.com/asaf-kali/codenames
 Author: Asaf Kali
 Author-email: akali93@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `codenames-1.2.4/codenames.egg-info/SOURCES.txt` & `codenames-1.2.5/codenames.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/pyproject.toml` & `codenames-1.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/setup.py` & `codenames-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "beautifultable~=1.0",
 ]
 WEB_DEPS = ["selenium~=4.1"]
 ALL_DEPS = BASE_DEPS + WEB_DEPS
 
 setup(
     name="codenames",
-    version="1.2.4",
+    version="1.2.5",
     description="Codenames board game logic implementation in python.",
     author="Asaf Kali",
     author_email="akali93@gmail.com",
     url="https://github.com/asaf-kali/codenames",
     install_requires=BASE_DEPS,
     extras_require={
         "all": ALL_DEPS,
```

### Comparing `codenames-1.2.4/tests/board_test.py` & `codenames-1.2.5/tests/board_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/tests/card_test.py` & `codenames-1.2.5/tests/card_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/tests/flows_test.py` & `codenames-1.2.5/tests/flows_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/tests/game_runner_test.py` & `codenames-1.2.5/tests/game_runner_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/tests/game_state_test.py` & `codenames-1.2.5/tests/game_state_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/tests/player_test.py` & `codenames-1.2.5/tests/player_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/tests/serialization_test.py` & `codenames-1.2.5/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/tests/utils/constants.py` & `codenames-1.2.5/tests/utils/constants.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/tests/utils/hooks.py` & `codenames-1.2.5/tests/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `codenames-1.2.4/tests/utils/testing_players.py` & `codenames-1.2.5/tests/utils/testing_players.py`

 * *Files identical despite different names*

