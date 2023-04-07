# Comparing `tmp/search_string_overvaagning-0.3.3-py3-none-any.whl.zip` & `tmp/search_string_overvaagning-0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 17060 bytes, number of entries: 12
--rw-r--r--  2.0 unx      239 b- defN 23-Apr-02 20:27 search_string/__init__.py
--rw-r--r--  2.0 unx      382 b- defN 23-Apr-02 20:27 search_string/constants.py
--rw-r--r--  2.0 unx     2708 b- defN 23-Apr-02 20:27 search_string/linked_list.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 20:27 search_string/py.typed
--rw-r--r--  2.0 unx    21846 b- defN 23-Apr-02 20:27 search_string/search_string.py
--rw-r--r--  2.0 unx    11434 b- defN 23-Apr-02 20:27 search_string/search_string_collection.py
--rw-r--r--  2.0 unx       58 b- defN 23-Apr-02 20:27 search_string/version.py
--rw-r--r--  2.0 unx     4074 b- defN 23-Apr-02 20:27 search_string_overvaagning-0.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    10196 b- defN 23-Apr-02 20:27 search_string_overvaagning-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-02 20:27 search_string_overvaagning-0.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-02 20:27 search_string_overvaagning-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1072 b- defN 23-Apr-02 20:27 search_string_overvaagning-0.3.3.dist-info/RECORD
-12 files, 52115 bytes uncompressed, 15226 bytes compressed:  70.8%
+Zip file size: 16236 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      239 b- defN 23-Apr-07 16:29 search_string/__init__.py
+-rw-r--r--  2.0 unx      382 b- defN 23-Apr-07 16:29 search_string/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-07 16:29 search_string/py.typed
+-rw-r--r--  2.0 unx    21846 b- defN 23-Apr-07 16:29 search_string/search_string.py
+-rw-r--r--  2.0 unx    11786 b- defN 23-Apr-07 16:29 search_string/search_string_collection.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Apr-07 16:29 search_string/version.py
+-rw-r--r--  2.0 unx     4074 b- defN 23-Apr-07 16:29 search_string_overvaagning-0.3.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10197 b- defN 23-Apr-07 16:29 search_string_overvaagning-0.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 16:29 search_string_overvaagning-0.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-07 16:29 search_string_overvaagning-0.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      987 b- defN 23-Apr-07 16:29 search_string_overvaagning-0.3.5.dist-info/RECORD
+11 files, 49675 bytes uncompressed, 14534 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -1,37 +1,34 @@
 Filename: search_string/__init__.py
 Comment: 
 
 Filename: search_string/constants.py
 Comment: 
 
-Filename: search_string/linked_list.py
-Comment: 
-
 Filename: search_string/py.typed
 Comment: 
 
 Filename: search_string/search_string.py
 Comment: 
 
 Filename: search_string/search_string_collection.py
 Comment: 
 
 Filename: search_string/version.py
 Comment: 
 
-Filename: search_string_overvaagning-0.3.3.dist-info/LICENSE
+Filename: search_string_overvaagning-0.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: search_string_overvaagning-0.3.3.dist-info/METADATA
+Filename: search_string_overvaagning-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: search_string_overvaagning-0.3.3.dist-info/WHEEL
+Filename: search_string_overvaagning-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: search_string_overvaagning-0.3.3.dist-info/top_level.txt
+Filename: search_string_overvaagning-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: search_string_overvaagning-0.3.3.dist-info/RECORD
+Filename: search_string_overvaagning-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## search_string/search_string_collection.py

```diff
@@ -4,49 +4,68 @@
 from collections.abc import Generator
 from collections.abc import Iterable
 from copy import deepcopy
 from typing import Generic
 
 import search_string.constants as const
 from search_string.constants import Data
-from search_string.linked_list import LinkedList
-from search_string.linked_list import Node
 from search_string.search_string import SearchString
 
 
 class Trie(Generic[Data]):
-    __slots__ = ('trie', 'end_tokens')
+    __slots__ = ('sub_tries', 'end_tokens')
 
-    def __init__(self) -> None:
-        self.trie: dict[str, Trie] = {}
-        self.end_tokens: set[tuple[Data, int]] | None = None
+    def __init__(
+        self,
+        sub_tries: dict[str, Trie[Data]] | None = None,
+        end_tokens: set[tuple[Data, int]] | None = None,
+    ) -> None:
+        self.sub_tries: dict[str, Trie[Data]] = sub_tries or {}
+        self.end_tokens: set[tuple[Data, int]] | None = end_tokens
+
+    def __reduce__(self) -> tuple[type[Trie[Data]], tuple[dict[str, Trie[Data]], set[tuple[Data, int]] | None]]:
+        return self.__class__, (self.sub_tries, self.end_tokens)
 
     def __getitem__(self, key: str) -> Trie:
-        return self.trie[key]
+        return self.sub_tries[key]
 
     def __setitem__(self, key: str, value: Trie) -> None:
-        self.trie[key] = value
+        self.sub_tries[key] = value
 
     def __contains__(self, char: str) -> bool:
-        return char in self.trie
+        return char in self.sub_tries
+
+    def __eq__(self, other: object) -> bool:
+        return (
+            isinstance(other, Trie)
+            and self.sub_tries == other.sub_tries
+            and self.end_tokens == other.end_tokens
+        )
+
+    def get_or_insert(self, key: str) -> Trie[Data]:
+        return self.sub_tries.setdefault(key, Trie())
 
     @property
     def has_children(self) -> bool:
-        return len(self.trie) > 0
+        return len(self.sub_tries) > 0
 
 
 class SearchStringCollection(Generic[Data]):
     __slots__ = ('search_strings', 'trie')
 
-    def __init__(self, search_strings: Iterable[SearchString[Data]]) -> None:
+    def __init__(
+        self,
+        search_strings: Iterable[SearchString[Data]],
+        trie: Trie[Data] | None = None,
+    ) -> None:
         self.search_strings = self._build_search_string_dict(search_strings)
-        self.trie: Trie[Data] = self._build_trie()
+        self.trie: Trie[Data] = trie or self._build_trie()
 
-    def __reduce__(self) -> tuple[type[SearchStringCollection[Data]], tuple[list[SearchString[Data]]]]:
-        return self.__class__, (list(self.search_strings.values()),)
+    def __reduce__(self) -> tuple[type[SearchStringCollection[Data]], tuple[list[SearchString[Data]], Trie[Data]]]:
+        return self.__class__, (list(self), self.trie)
 
     def __iter__(self) -> Generator[SearchString[Data], None, None]:
         yield from self.search_strings.values()
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
         n = len(self.search_strings)
@@ -109,20 +128,19 @@
         part_id: int,
         part_str: str,
         cur_trie: Trie[Data],
     ) -> None:
         if not part_str:
             if cur_trie.end_tokens is None:
                 cur_trie.end_tokens = set()
-
             cur_trie.end_tokens.add((ss_id, part_id))
             return
 
         cur_char, next_chars = part_str[0], part_str[1:]
-        next_trie = cur_trie.trie.setdefault(cur_char, Trie())
+        next_trie = cur_trie.get_or_insert(cur_char)
         self._add_part_to_trie(ss_id, part_id, next_chars, next_trie)
 
     def _build_trie(self) -> Trie[Data]:
         trie: Trie[Data] = Trie()
         for ss in self:
             for part_id, part_str in ss._raw_parts():
                 for splitted_part in self._split_part(part_str):
@@ -140,38 +158,32 @@
         yield '\n'  # Strings that matched the end and need one more char to get added
 
     def _match_single_text(self, text: str) -> set[tuple[Data, int]]:
         """
         Matches a single text against the search strings and returns a set of
         tuples of the form (search_string_id, part_id).
         """
-        active_nodes: LinkedList[Trie] = LinkedList()
+        cur_positions: list[Trie[Data]] = []
         matched: set[tuple[Data, int]] = set()
         for char in self._text_yielder(text):
             is_wb = char in const.WORD_BREAK_CHARS
-            active_nodes.append(Node(self.trie))
-            for node in list(active_nodes):
-                if is_wb and const.WORD_BOUNDARY_CHAR in node.value:
-                    new_trie = node.value[const.WORD_BOUNDARY_CHAR]
-                    if new_trie.end_tokens is not None:
-                        matched.update(new_trie.end_tokens)
-                        if new_trie.has_children:
-                            active_nodes.append(Node(new_trie))
-                    else:
-                        active_nodes.append(Node(new_trie))
-
-                if char not in node.value:
-                    active_nodes.remove(node)
-                else:
-                    new_trie = node.value[char]
-                    node.value = new_trie
+            chars_to_check = [char, const.WORD_BOUNDARY_CHAR] if is_wb else [char]
+            new_positions: list[Trie[Data]] = []
+            cur_positions.append(self.trie)
+            for char_to_check in chars_to_check:
+                for cur_position in cur_positions:
+                    if char_to_check not in cur_position:
+                        continue
+
+                    new_trie = cur_position[char_to_check]
+                    if new_trie.has_children:
+                        new_positions.append(new_trie)
                     if new_trie.end_tokens is not None:
                         matched.update(new_trie.end_tokens)
-                        if not new_trie.has_children:
-                            active_nodes.remove(node)
+            cur_positions = new_positions
         return matched
 
     def _match_sentence(self, sentence: str) -> list[SearchString[Data]]:
         """
         Match the search strings against the text and return a list of
         SearchString objects that matched the text.
         """
```

## search_string/version.py

```diff
@@ -1,3 +1,3 @@
 from __future__ import annotations
 
-__version__ = '0.3.3'
+__version__ = '0.3.5'
```

## Comparing `search_string_overvaagning-0.3.3.dist-info/LICENSE` & `search_string_overvaagning-0.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `search_string_overvaagning-0.3.3.dist-info/METADATA` & `search_string_overvaagning-0.3.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: search-string-overvaagning
-Version: 0.3.3
+Version: 0.3.5
 Summary: SearchString is a custom implementation for searching strings for overvaagning.app.
 Home-page: https://github.com/kaas-mulvad/search-string
 Author: Søren Mulvad
 Author-email: Soeren Mulvad <post@kaasogmulvad.dk>
 License: End-User License Agreement (EULA) of SearchString
         
         This End-User License Agreement ("EULA") is a legal agreement between you and Kaas & Mulvad. Our EULA was created by EULA Template for SearchString.
@@ -73,15 +73,15 @@
 
 You can install `search-string` from [PyPI][pypi]:
 
 ```bash
 $ pip install search-string-overvaagning
 ```
 
-The package is supported on Python 3.9+.
+The package is supported on Python 3.10+.
 
 ## About
 
 This package implements the search string object that is used across [overvaagning.app](https://overvaagning.app/) for different types of surveillance.
 
 It is used for searching a text. For something to be deemed a match, the text must match the `first_str` and if the `second_str` is not empty, the text must also match the `second_str`. If the `not_str` is not empty, the text must *not* match the `not_str`. A logical AND is used between the three conditions. The three strings can each be a collection of strings separated by semicolons wherein a match is deemed by logical OR. You can use '~' to make a word boundary. Finally, you can use `!global` at the end of a string to signal that that part should check globally.
```

## Comparing `search_string_overvaagning-0.3.3.dist-info/RECORD` & `search_string_overvaagning-0.3.5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 search_string/__init__.py,sha256=L1sA0kHPqU2plluuMF75eGANNBM6JKbMm_V3Bkuujbw,239
 search_string/constants.py,sha256=usqtRup-oXpd86ucEopd8ghWdcwl6yDX8Bxjy5nRiFY,382
-search_string/linked_list.py,sha256=8nOqh-W1uLwgBjRrq8s6nxPiFmqCSRB7DFwEQ0lcxy0,2708
 search_string/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 search_string/search_string.py,sha256=MWUWqlV_QMcFE9_TQHgP7ztNIUGbl-d4KRI1eURhJsc,21846
-search_string/search_string_collection.py,sha256=DiK18kynDNQ8cGOjQuyLL7aHE_MRboFEx5pg4z7PP5U,11434
-search_string/version.py,sha256=999F9pn78OrJszoS1jtrrSiBmXoAyebwmScDKc5XyGc,58
-search_string_overvaagning-0.3.3.dist-info/LICENSE,sha256=xYX49IgOmQdnmBwaNYTW43N4YAiyfzwNr367kxWn2-s,4074
-search_string_overvaagning-0.3.3.dist-info/METADATA,sha256=NxzL-wSLGUuhfwVLJoXDiU--t1aWUnv1ikOTrKqgjm0,10196
-search_string_overvaagning-0.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-search_string_overvaagning-0.3.3.dist-info/top_level.txt,sha256=66CcfMgUUyQ2MQT4Se3Eit8Zr5agt6PT-YqoodkXGgA,14
-search_string_overvaagning-0.3.3.dist-info/RECORD,,
+search_string/search_string_collection.py,sha256=Y0TfcfMHOBvQf9NpEHLfgGCXwj5I2jed3iK5L9UAU88,11786
+search_string/version.py,sha256=GlEqBXfQJ0ivG1fjTckhSM8J7k20FRpPPJh55xVOr5A,58
+search_string_overvaagning-0.3.5.dist-info/LICENSE,sha256=xYX49IgOmQdnmBwaNYTW43N4YAiyfzwNr367kxWn2-s,4074
+search_string_overvaagning-0.3.5.dist-info/METADATA,sha256=eqiGEhG8qYafb9L_4F-zlAHVTAs7Z3MI67h5bw6bn5o,10197
+search_string_overvaagning-0.3.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+search_string_overvaagning-0.3.5.dist-info/top_level.txt,sha256=66CcfMgUUyQ2MQT4Se3Eit8Zr5agt6PT-YqoodkXGgA,14
+search_string_overvaagning-0.3.5.dist-info/RECORD,,
```

