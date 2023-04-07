# Comparing `tmp/meeple-cli-0.1.0b3.tar.gz` & `tmp/meeple-cli-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeple-cli-0.1.0b3.tar", last modified: Tue Apr  4 02:58:07 2023, max compression
+gzip compressed data, was "meeple-cli-0.1.0b4.tar", last modified: Fri Apr  7 19:59:06 2023, max compression
```

## Comparing `meeple-cli-0.1.0b3.tar` & `meeple-cli-0.1.0b4.tar`

### file list

```diff
@@ -1,42 +1,47 @@
--rw-r--r--   0        0        0       66 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/.flake8
--rw-r--r--   0        0        0     1146 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1035 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      279 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/.gitignore
--rw-r--r--   0        0        0      168 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/.markdownlint.yaml
--rw-r--r--   0        0        0     1174 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1071 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/LICENSE
--rw-r--r--   0        0        0     5322 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/README.md
--rw-r--r--   0        0        0     2690 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/docs/changelog.md
--rw-r--r--   0        0        0      876 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/justfile
--rw-r--r--   0        0        0     1014 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/src/meeple/__init__.py
--rw-r--r--   0        0        0      562 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/src/meeple/command/__init__.py
--rw-r--r--   0        0        0     1550 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/src/meeple/command/add.py
--rw-r--r--   0        0        0     2042 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/src/meeple/command/collections.py
--rw-r--r--   0        0        0     1293 2023-04-04 02:58:02.849422 meeple-cli-0.1.0b3/src/meeple/command/delete.py
--rw-r--r--   0        0        0     1541 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/drop.py
--rw-r--r--   0        0        0      634 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/hot.py
--rw-r--r--   0        0        0     1358 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/info.py
--rw-r--r--   0        0        0     3295 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/list.py
--rw-r--r--   0        0        0     2409 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/move.py
--rw-r--r--   0        0        0      664 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/new.py
--rw-r--r--   0        0        0     1312 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/open.py
--rw-r--r--   0        0        0     1081 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/rename.py
--rw-r--r--   0        0        0      971 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/search.py
--rw-r--r--   0        0        0     3292 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/stats.py
--rw-r--r--   0        0        0     2536 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/command/update.py
--rw-r--r--   0        0        0     1067 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/root.py
--rw-r--r--   0        0        0        0 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/type/__init__.py
--rw-r--r--   0        0        0      226 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/type/collection.py
--rw-r--r--   0        0        0     3807 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/type/item.py
--rw-r--r--   0        0        0        0 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/util/__init__.py
--rw-r--r--   0        0        0     1594 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/util/api_util.py
--rw-r--r--   0        0        0     1931 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/util/collection_util.py
--rw-r--r--   0        0        0     2596 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/util/data_util.py
--rw-r--r--   0        0        0      652 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/util/fs_util.py
--rw-r--r--   0        0        0      352 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/util/input_util.py
--rw-r--r--   0        0        0     2163 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/util/output_util.py
--rw-r--r--   0        0        0     1538 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/src/meeple/util/sort_util.py
--rw-r--r--   0        0        0        0 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/tests/__init__.py
--rw-r--r--   0        0        0      313 2023-04-04 02:58:02.853422 meeple-cli-0.1.0b3/tests/test_root.py
--rw-r--r--   0        0        0     6322 1970-01-01 00:00:00.000000 meeple-cli-0.1.0b3/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.flake8
+-rw-r--r--   0        0        0     1146 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1035 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      289 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.gitignore
+-rw-r--r--   0        0        0      168 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.markdownlint.yaml
+-rw-r--r--   0        0        0     1174 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/LICENSE
+-rw-r--r--   0        0        0     6207 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/README.md
+-rw-r--r--   0        0        0     4380 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/docs/changelog.md
+-rw-r--r--   0        0        0      876 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/justfile
+-rw-r--r--   0        0        0     1014 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/__init__.py
+-rw-r--r--   0        0        0      639 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/__init__.py
+-rw-r--r--   0        0        0     1498 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/add.py
+-rw-r--r--   0        0        0     2039 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/collections.py
+-rw-r--r--   0        0        0     1052 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/completions.py
+-rw-r--r--   0        0        0     1385 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/delete.py
+-rw-r--r--   0        0        0     1489 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/drop.py
+-rw-r--r--   0        0        0     5040 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/find.py
+-rw-r--r--   0        0        0      628 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/hot.py
+-rw-r--r--   0        0        0     1229 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/info.py
+-rw-r--r--   0        0        0     3357 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/list.py
+-rw-r--r--   0        0        0     2394 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/move.py
+-rw-r--r--   0        0        0      658 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/new.py
+-rw-r--r--   0        0        0     1158 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/open.py
+-rw-r--r--   0        0        0     1179 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/rename.py
+-rw-r--r--   0        0        0      966 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/search.py
+-rw-r--r--   0        0        0     3403 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/stats.py
+-rw-r--r--   0        0        0     2634 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/update.py
+-rw-r--r--   0        0        0     1153 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/root.py
+-rw-r--r--   0        0        0        0 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/type/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/type/collection.py
+-rw-r--r--   0        0        0     3977 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/type/item.py
+-rw-r--r--   0        0        0        0 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/__init__.py
+-rw-r--r--   0        0        0     1594 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/api_util.py
+-rw-r--r--   0        0        0      697 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/cmd_util.py
+-rw-r--r--   0        0        0     2024 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/collection_util.py
+-rw-r--r--   0        0        0      235 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/completion_util.py
+-rw-r--r--   0        0        0     2596 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/data_util.py
+-rw-r--r--   0        0        0      938 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/filter_util.py
+-rw-r--r--   0        0        0      652 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/fs_util.py
+-rw-r--r--   0        0        0      352 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/input_util.py
+-rw-r--r--   0        0        0     2549 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/output_util.py
+-rw-r--r--   0        0        0     1538 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/sort_util.py
+-rw-r--r--   0        0        0        0 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/tests/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/tests/test_root.py
+-rw-r--r--   0        0        0     7207 1970-01-01 00:00:00.000000 meeple-cli-0.1.0b4/PKG-INFO
```

### Comparing `meeple-cli-0.1.0b3/.github/workflows/python-publish.yml` & `meeple-cli-0.1.0b4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b3/.github/workflows/python-test.yml` & `meeple-cli-0.1.0b4/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b3/.pre-commit-config.yaml` & `meeple-cli-0.1.0b4/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-toml
       - id: check-added-large-files
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.260
+    rev: v0.0.261
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
```

### Comparing `meeple-cli-0.1.0b3/LICENSE` & `meeple-cli-0.1.0b4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MIT License
+# MIT License
 
 Copyright (c) 2023 Bradley Wojcik
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `meeple-cli-0.1.0b3/README.md` & `meeple-cli-0.1.0b4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # meeple-cli
 
 [![build status](https://img.shields.io/github/actions/workflow/status/boldandbrad/meeple-cli/python-test.yml?branch=main&logo=github)](https://github.com/boldandbrad/meeple-cli/actions/workflows/python-test.yml?query=branch%3Amain)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![pypi](https://img.shields.io/pypi/v/meeple-cli)](https://pypi.org/project/meeple-cli/)
-![downloads](https://img.shields.io/pypi/dm/meeple-cli)
+[![downloads](https://img.shields.io/pypi/dm/meeple-cli)](https://pypistats.org/packages/meeple-cli)
 
 <!-- [![codecov](https://codecov.io/gh/boldandbrad/meeple-cli/branch/main/graph/badge.svg)](https://codecov.io/gh/boldandbrad/meeple-cli) -->
 <!-- [![Docs](https://img.shields.io/website?down_message=down&label=docs&up_message=online&url=https%3A%2F%2Fboldandbrad.github.io%2Fmeeple-cli%2F)](https://boldandbrad.github.io/meeple-cli/) -->
 
-**Local board game collection manager. Powered by [BoardGameGeek](https://boardgamegeek.com).**
+**Local board game collection manager. Powered by
+[BoardGameGeek](https://boardgamegeek.com).**
 
-> `meeple-cli` allows you to create and manage _local_ board game collections
-> stored on your system. At this time the [BoardGameGeek API](https://boardgamegeek.com/wiki/page/BGG_XML_API2)
-> does not allow for creation nor modification of GeekLists directly. Nor is
-> `meeple-cli` affiliated with BoardGameGeek.
+## Disclaimer
+
+> Neither `meeple-cli` nor its maintainers are affiliated with
+> [BoardGameGeek](https://boardgamegeek.com).
 
 ## Install
 
 Global isolated install via [pipx](https://pypa.github.io/pipx/) (recommended):
 
 ```sh
 pipx install meeple-cli
@@ -30,64 +31,109 @@
 ```
 
 <!-- ```zsh
 brew tap boldandbrad/homebrew-tap
 brew install meeple-cli
 ```-->
 
-<!-- > For more details, read the **meeple-cli** [install guide](https://boldandbrad.github.io/meeple-cli/#/install). -->
+<!-- > For more details, read the **meeple-cli**
+> [install guide](https://boldandbrad.github.io/meeple-cli/#/install). -->
 
 ## Usage
 
-```sh
+```txt
 $ meeple --help
 Usage: meeple [OPTIONS] COMMAND [ARGS]...
 
   Local board game collection manager. Powered by BoardGameGeek.
 
 Options:
   -h, --help     Show this message and exit.
   -v, --version  Show the version and exit.
 
-Commands:
-  add          Add a board game/extension to a collection.
-  collections  List all local collections.
-  delete       Delete a local collection.
-  drop         Remove a board game/extension from a collection.
-  hot          Retrieve the current BoardGameGeek hotness list.
-  info         Print out the details of a board game or expansion.
-  list         List all board games/extensions in a collection.
-  move         Move a board game/extension from one collection to another.
-  new          Create a new local collection.
-  open         Open a board game or expansion on the BoardGameGeek website.
+Collection Commands:
+  add          Add an item to a collection.
+  collections  List all collections.
+  delete       Delete a collection.
+  drop         Remove an item from a collection.
+  find         Search collections for items.
+  list         List contents of a collection.
+  move         Move an item from one collection to another.
+  new          Create a new collection.
   rename       Rename a local collection.
-  search       Search BoardGameGeek for a board game or expansion.
-  stats        Print out the details of a local collection.
+  stats        Print out the details of a collection.
   update       Update local collection data.
+
+BoardGameGeek Commands:
+  hot     List current BoardGameGeek trending items.
+  info    Print out the details of an item.
+  open    Open an item on BoardGameGeek.
+  search  Search BoardGameGeek for items.
+
+Other Commands:
+  completions  Setup meeple shell completions.
+```
+
+<!-- > For more usage details, read the **meeple-cli**
+> [usage guide](https://boldandbrad.github.io/meeple-cli/#/usage). -->
+
+## Completions
+
+`meeple-cli` supports shell completions for `bash`, `zsh`, and `fish`. For
+setup, use `meeple completions <SHELL>`, or the following instructions:
+
+<details>
+<summary>bash</summary>
+
+Add the following to `~/.bashrc`:
+
+```sh
+eval "$(_MEEPLE_COMPLETE=bash_source meeple)"
+```
+
+</details>
+
+<details>
+<summary>zsh</summary>
+
+Add the following to `~/.zshrc`:
+
+```sh
+eval "$(_MEEPLE_COMPLETE=zsh_source meeple)"
+```
+
+</details>
+
+<details>
+<summary>fish</summary>
+
+Save the script to `~/.config/fish/completions/meeple.fish`:
+
+```sh
+_MEEPLE_COMPLETE=fish_source meeple > ~/.config/fish/completions/meeple.fish
 ```
 
-<!-- > For more usage details, read the **meeple-cli** [usage guide](https://boldandbrad.github.io/meeple-cli/#/usage). -->
+</details>
 
 ## Roadmap
 
-See a list of already implemented features/changes in the [Changelog](docs/changelog.md).
+See a list of already implemented features/changes in the
+[Changelog](docs/changelog.md).
 
 ### Planned Features
 
-- [ ] Find board games/expansions across local collections by attributes ->
-      `meeple find`
 - [ ] Verbose option on `meeple info` that includes additional info such as
       description, publishers, etc
-- [ ] Copy a local collection -> `meeple copy`
-- [ ] Export a local collection to csv or another format -> `meeple export`
-- [ ] Import a local collection from a variety of formats -> `meeple import`
-- [ ] Ability to assign and manage personal ratings of board games/expansions
+- [ ] Export a collection to csv or another format -> `meeple export`
+- [ ] Import a collection from a variety of formats -> `meeple import`
 
 ### Potential Features (May or may not happen)
 
+- [ ] Ability to assign and manage personal ratings of board games/expansions
+- [ ] Copy a collection -> `meeple copy`
 - [ ] Copy option `-c` on most commands that allows you to interactively select
       and copy text from the command output (for grabbing IDs) - similar to yank
 - [ ] Manage user preferences/configs -> `meeple config` stored at
       `~/.meeple/config.json` or something
   - [ ] Toggle colorized output
   - [ ] Set custom default output sorts
   - [ ] Set custom data location
@@ -103,21 +149,38 @@
         BoardGameGeek over time
 - [ ] Ability to record and manage plays of board games - would be nuts.
   - [ ] Ability to calculate and surface play statistics for a board game
 - [ ] Ability to interact with discord services to show that you are currently
       playing a board game?
 - [ ] Ability to actually interact with BoardGameGeek user
       profile/settings/collections (not all currently possible via the API)
-- [ ] Shell completions for common shells? For finding/searching.
 
 ### Other Todos
 
 - [ ] Unit tests
 - [ ] Documentation site (via vitepress?)
-- [ ] Homebrew formula (will be available [here](https://github.com/boldandbrad/homebrew-tap))
+- [ ] Homebrew formula (will be available
+      [here](https://github.com/boldandbrad/homebrew-tap))
 - [ ] Implement simple logging for debugging (local, not telemetry) (via
       loguru?)
 
+## FAQ
+
+### Why local only collections?
+
+Currently, the
+[BoardGameGeek Public API](https://boardgamegeek.com/wiki/page/BGG_XML_API2)
+provides limited _read-only_ data about user collections/GeekLists.
+
+While it is _technically_ feasible to interface with GeekLists via
+webscrapers/spiders, this kind of practice would be both complex and also
+violate [BoardGameGeek Terms of Service](https://boardgamegeek.com/terms#toc22).
+
+### Where does `meeple-cli` store data?
+
+`meeple-cli` stores collection data in `~/.meeple` and only makes network
+connections to retrieve data from the BoardGameGeek API.
+
 ## License
 
 Copyright (c) 2023 Bradley Wojcik. Released under the MIT License. See
 [LICENSE](LICENSE) for details.
```

### Comparing `meeple-cli-0.1.0b3/justfile` & `meeple-cli-0.1.0b4/justfile`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b3/pyproject.toml` & `meeple-cli-0.1.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/add.py` & `meeple-cli-0.1.0b4/src/meeple/command/add.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,34 +4,31 @@
 
 from meeple.util.api_util import get_bgg_item
 from meeple.util.collection_util import (
     is_collection,
     read_collection,
     update_collection,
 )
+from meeple.util.completion_util import complete_collections
 from meeple.util.output_util import print_error, print_info
 
 
 @click.command()
+@click.argument("collection", shell_complete=complete_collections)
+@click.argument("id", type=int)
 @click.help_option("-h", "--help")
-@click.argument("collection")
-@click.argument("id")
-def add(collection: str, id: str) -> None:
-    """Add a board game/extension to a collection.
+def add(collection: str, id: int) -> None:
+    """Add an item to a collection.
 
     - COLLECTION is the name of the intended destination collection.
 
     - ID is the BoardGameGeek ID of the board game/expansion to be added.
     """
-    # check that the given id is an integer
-    if not id.isdigit():
-        sys.exit(print_error("Provided ID must be an integer value"))
-    bgg_id = int(id)
-
     # check that the given id is a valid BoardGameGeek ID
+    bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
         sys.exit(print_error(f"'{bgg_id}' is not a valid BoardGameGeek ID"))
 
     # check that the given collection is a valid collection
     if not is_collection(collection):
         sys.exit(print_error(f"'{collection}' is not a valid collection"))
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/collections.py` & `meeple-cli-0.1.0b4/src/meeple/command/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from meeple.util.collection_util import get_collections
 from meeple.util.data_util import get_collection_data, last_updated
 from meeple.util.output_util import print_table, print_warning
 from meeple.util.sort_util import sort_collections
 
 
 @click.command()
-@click.help_option("-h", "--help")
 @click.option(
     "--sort",
     type=click.Choice(
         ["name", "boardgames", "expansions", "updated"], case_sensitive=False
     ),
     default="updated",
     show_default=True,
-    help="Sort output by a chosen column.",
+    help="Sort output by the provided column.",
 )
-@click.option("-v", "--verbose", is_flag=True, help="Display additional details.")
+@click.option("-v", "--verbose", is_flag=True, help="Output additional details.")
+@click.help_option("-h", "--help")
 def collections(sort: str, verbose: bool) -> None:
-    """List all local collections."""
+    """List all collections."""
     # attempt to retrieve collections
     collections = get_collections()
 
     # check that local collections exist
     if not collections:
         sys.exit(
             print_warning(
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/delete.py` & `meeple-cli-0.1.0b4/src/meeple/command/delete.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import sys
 
 import click
 
 from meeple.util.collection_util import delete_collection, is_collection
+from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import delete_collection_data, get_collection_data
 from meeple.util.input_util import bool_input
 from meeple.util.output_util import print_error, print_info
 
 
 @click.command()
-@click.help_option("-h", "--help")
-@click.argument("collection")
+@click.argument("collection", shell_complete=complete_collections)
 @click.option("-y", "--yes", is_flag=True, help="Dangerous - Bypass confirmation.")
+@click.help_option("-h", "--help")
 def delete(collection: str, yes: bool) -> None:
-    """Delete a local collection.
+    """Delete a collection.
 
     - COLLECTION is the name of the collection to be deleted.
     """
     # check that the given collection exists
     if not is_collection(collection):
         sys.exit(print_error(f"'{collection}' already does not exist"))
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/drop.py` & `meeple-cli-0.1.0b4/src/meeple/command/drop.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,34 +4,31 @@
 
 from meeple.util.api_util import get_bgg_item
 from meeple.util.collection_util import (
     is_collection,
     read_collection,
     update_collection,
 )
+from meeple.util.completion_util import complete_collections
 from meeple.util.output_util import print_error, print_info
 
 
 @click.command()
+@click.argument("collection", shell_complete=complete_collections)
+@click.argument("id", type=int)
 @click.help_option("-h", "--help")
-@click.argument("collection")
-@click.argument("id")
-def drop(collection: str, id: str) -> None:
-    """Remove a board game/extension from a collection.
+def drop(collection: str, id: int) -> None:
+    """Remove an item from a collection.
 
     - COLLECTION is the name of the collection to be modified.
 
     - ID is the BoardGameGeek ID of the board game/expansion to be removed.
     """
-    # check that the given ID is an integer
-    if not id.isdigit():
-        sys.exit(print_error("Provided ID must be an integer value"))
-    bgg_id = int(id)
-
     # check that the given id is a valid BoardGameGeek ID
+    bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
         sys.exit(print_error(f"'{bgg_id}' is not a valid BoardGameGeek ID"))
 
     # check that the given collection is a valid collection
     if not is_collection(collection):
         sys.exit(print_error(f"'{collection}' is not a valid collection"))
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/hot.py` & `meeple-cli-0.1.0b4/src/meeple/command/hot.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from meeple.util.output_util import print_table
 
 
 @click.command()
 @click.help_option("-h", "--help")
 # TODO: add verbosity flag to show more details for each item
 def hot() -> None:
-    """Retrieve the current BoardGameGeek hotness list."""
+    """List current BoardGameGeek trending items."""
     # retrieve hotness data from BoardGameGeek
     api_result = get_bgg_hot()
 
     # prepare table data
     headers = ["#", "ID", "Name"]
     rows = []
     for idx, item in enumerate(api_result):
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/info.py` & `meeple-cli-0.1.0b4/src/meeple/command/info.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,33 +5,30 @@
 from meeple.util.api_util import get_bgg_item
 from meeple.util.output_util import (
     fmt_players,
     fmt_playtime,
     fmt_rank,
     fmt_rating,
     fmt_weight,
+    fmt_year,
     print_error,
     print_table,
 )
 
 
 @click.command()
+@click.argument("id", type=int)
 @click.help_option("-h", "--help")
-@click.argument("id")
-def info(id: str) -> None:
-    """Print out the details of a board game or expansion.
+def info(id: int) -> None:
+    """Print out the details of an item.
 
     - ID is the BoardGameGeek ID of the board game/expansion to be detailed.
     """
-    # check that the given id is an integer
-    if not id.isdigit():
-        sys.exit(print_error("Provided ID must be an integer value"))
-    bgg_id = int(id)
-
     # check that the given id is a valid one
+    bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
         sys.exit(print_error(f"'{bgg_id}' is not a valid BoardGameGeek ID"))
 
     info_rows = [
         [
             f"Rating: {fmt_rating(bgg_item.rating)}",
@@ -40,9 +37,9 @@
         ],
         [
             f"Rank: {fmt_rank(bgg_item.rank)}",
             f"Time: {fmt_playtime(bgg_item.minplaytime, bgg_item.maxplaytime)}",
             f"Weight: {fmt_weight(bgg_item.weight)}",
         ],
     ]
-    print_table([[f"{bgg_item.id}", f"{bgg_item.name} ({bgg_item.year})"]])
+    print_table([[f"{bgg_item.id}", f"{bgg_item.name} ({fmt_year(bgg_item.year)})"]])
     print_table(info_rows, lines=True)
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/list.py` & `meeple-cli-0.1.0b4/src/meeple/command/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 import sys
 
 import click
 
 from meeple.util.collection_util import is_collection
+from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import get_collection_data
 from meeple.util.output_util import (
     fmt_players,
     fmt_playtime,
     fmt_rank,
     fmt_rating,
     fmt_weight,
+    fmt_year,
     print_error,
     print_table,
     print_warning,
 )
 from meeple.util.sort_util import sort_items
 
 
-@click.command()
-@click.help_option("-h", "--help")
-@click.argument("collection")
+@click.command(name="list")
+@click.argument("collection", shell_complete=complete_collections)
 @click.option(
     "-b",
     "--boardgames",
-    "only_include",
+    "item_type",
     is_flag=True,
     flag_value="bg",
-    help="Include only board games in output.",
+    help="Output only board games.",
 )
 @click.option(
     "-e",
     "--expansions",
-    "only_include",
+    "item_type",
     is_flag=True,
     flag_value="ex",
-    help="Include only expansions in output.",
+    help="Output only expansions.",
 )
 @click.option(
     "--sort",
     type=click.Choice(
         ["rank", "rating", "weight", "year", "name", "id"], case_sensitive=False
     ),
     default="rating",
     show_default=True,
-    help="Sort output by a chosen column.",
+    help="Sort output by the provided column.",
 )
-@click.option("-v", "--verbose", is_flag=True, help="Display additional details.")
+@click.option("-v", "--verbose", is_flag=True, help="Output additional details.")
+@click.help_option("-h", "--help")
 # TODO: add option to run update on the collection prior to list
 # TODO: add option to show grid lines or not in the table
 # TODO: implement paging/scrolling for long lists? not sure how rich will like that
-def list_collection(
-    collection: str, only_include: str, sort: str, verbose: bool
-) -> None:
-    """List all board games/extensions in a collection.
+def list_collection(collection: str, item_type: str, sort: str, verbose: bool) -> None:
+    """List contents of a collection.
 
     - COLLECTION is the name of the collection to be listed.
     """
     # check that the given collection is a valid collection
     if not is_collection(collection):
         sys.exit(print_error(f"'{collection}' is not a valid collection"))
 
@@ -67,38 +67,38 @@
         sys.exit(
             print_warning(
                 f"local data not found for '{collection}'. update with `meeple update {collection}`"
             )
         )
 
     # determine what to include in results depending on given flags
-    if only_include == "bg":
+    if item_type == "bg":
         out_list = boardgames
-    elif only_include == "ex":
+    elif item_type == "ex":
         out_list = expansions
     else:
         out_list = boardgames + expansions
 
     # sort output
     out_list = sort_items(out_list, sort)
 
     # prepare table data
     # TODO: add indicator to currently sorted by column
     headers = ["ID", "Name"]
     if verbose:
-        headers = ["ID", "Name", "Year", "Rank", "Rating", "Weight", "Players", "Time"]
+        headers.extend(["Year", "Rank", "Rating", "Weight", "Players", "Time"])
 
     rows = []
     for item in out_list:
         cols = [str(item.id), item.name]
         # include additional data if the user chose verbose output
         if verbose:
             cols.extend(
                 [
-                    str(item.year),
+                    fmt_year(item.year),
                     fmt_rank(str(item.rank)),
                     fmt_rating(item.rating),
                     fmt_weight(item.weight),
                     fmt_players(item.minplayers, item.maxplayers),
                     fmt_playtime(item.minplaytime, item.maxplaytime),
                 ]
             )
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/move.py` & `meeple-cli-0.1.0b4/src/meeple/util/collection_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,74 @@
-import sys
+from os import walk
+from os.path import join, splitext
+from pathlib import Path
+from typing import List
 
-import click
+import yaml
 
-from meeple.util.api_util import get_bgg_item
-from meeple.util.collection_util import (
-    is_collection,
-    read_collection,
-    update_collection,
-)
-from meeple.util.output_util import print_error, print_info
-
-
-@click.command()
-@click.help_option("-h", "--help")
-@click.argument("from_collection")
-@click.argument("to_collection")
-@click.argument("id")
-def move(from_collection: str, to_collection: str, id: str) -> None:
-    """Move a board game/extension from one collection to another.
-
-    - FROM_COLLECTION is the name of the intended source collection.
-
-    - TO_COLLECTION is the name of the intended destination collection.
-
-    - ID is the BoardGameGeek ID of the board game/expansion to be moved.
-    """
-    # check that the given id is an integer
-    if not id.isdigit():
-        sys.exit(print_error("Provided ID must be an integer value"))
-    bgg_id = int(id)
-
-    # check that the given id is a valid BoardGameGeek ID
-    bgg_item = get_bgg_item(bgg_id)
-    if not bgg_item:
-        sys.exit(print_error(f"'{bgg_id}' is not a valid BoardGameGeek ID"))
-
-    # check that the given collection is a valid collection
-    if not is_collection(from_collection):
-        sys.exit(print_error(f"'{from_collection}' is not a valid collection"))
-
-    # check that the given collection is a valid collection
-    if not is_collection(to_collection):
-        # TODO: offer to create the new collection
-        sys.exit(print_error(f"'{to_collection}' is not a valid collection"))
-
-    # TODO: refactor to avoid the following duplicated code
-    # remove the id from the source collection
-    from_bgg_ids = read_collection(from_collection)
-    if bgg_id not in from_bgg_ids:
-        # TODO: ask if they want to add it to the to collection anyway
-        sys.exit(
-            print_error(f"'{bgg_id}' already doesn't exist in '{from_collection}'")
-        )
-
-    from_bgg_ids.remove(bgg_id)
-
-    # add the id to the destination collection
-    to_bgg_ids = read_collection(to_collection)
-    if to_bgg_ids and bgg_id in to_bgg_ids:
-        sys.exit(print_error(f"'{bgg_id}' already exists in '{to_collection}'"))
-
-    to_bgg_ids.append(bgg_id)
-    to_bgg_ids.sort()
-
-    # save changes
-    update_collection(from_collection, from_bgg_ids)
-    update_collection(to_collection, to_bgg_ids)
-    print_info(f"Moved '{bgg_item.name}' from '{from_collection}' to '{to_collection}'")
+from meeple.util.fs_util import get_collection_dir
+
+IN_PATH = get_collection_dir()
+ID_LIST_KEY = "bgg-ids"
+
+
+def _collection_file(collection_name: str) -> str:
+    return join(IN_PATH, f"{collection_name}.yml")
+
+
+def get_collections() -> List[str]:
+    # create in_path dir and exit if it does not exist
+    if not Path(IN_PATH).exists():
+        Path(IN_PATH).mkdir(parents=True)
+
+    # retrieve collection source files from in_path
+    collection_files = next(walk(IN_PATH))[2]
+    collections = []
+    for collection_file in collection_files:
+        collection, ext = splitext(collection_file)
+        if ext == ".yml":
+            collections.append(collection)
+    return collections
+
+
+def is_collection(name: str) -> bool:
+    return name in get_collections()
+
+
+def are_collections(names: [str]) -> bool:
+    return set(names) <= set(get_collections())
+
+
+def read_collection(name: str) -> List[int]:
+    with open(_collection_file(name), "r") as f:
+        data = yaml.load(f, Loader=yaml.FullLoader)
+        if data and ID_LIST_KEY in data:
+            bgg_ids = data[ID_LIST_KEY]
+            if not bgg_ids:
+                return []
+
+            # remove non int values from list
+            for bgg_id in bgg_ids:
+                if not isinstance(bgg_id, int):
+                    bgg_ids.remove(bgg_id)
+            return bgg_ids
+        return []
+
+
+def create_collection(name: str) -> None:
+    data = {ID_LIST_KEY: []}
+    with open(_collection_file(name), "w") as f:
+        yaml.dump(data, f)
+
+
+def update_collection(name: str, ids: list) -> None:
+    data = {ID_LIST_KEY: ids}
+    with open(_collection_file(name), "w") as f:
+        yaml.dump(data, f)
+
+
+def rename_collection(current_name: str, new_name: str) -> None:
+    Path(_collection_file(current_name)).rename(join(IN_PATH, f"{new_name}.yml"))
+
+
+def delete_collection(name: str) -> None:
+    Path(_collection_file(name)).unlink()
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/new.py` & `meeple-cli-0.1.0b4/src/meeple/command/new.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import click
 
 from meeple.util.collection_util import create_collection, is_collection
 from meeple.util.output_util import print_error, print_info
 
 
 @click.command()
-@click.help_option("-h", "--help")
 @click.argument("collection")
+@click.help_option("-h", "--help")
 def new(collection: str) -> None:
-    """Create a new local collection.
+    """Create a new collection.
 
     - COLLECTION is the name of the collection to be created.
     """
     # check that the given collection doesn't already exist
     if is_collection(collection):
         sys.exit(print_error(f"'{collection}' already exists"))
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/open.py` & `meeple-cli-0.1.0b4/src/meeple/command/open.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,29 +4,25 @@
 import click
 
 from meeple.util.api_util import BGG_DOMAIN, get_bgg_items
 from meeple.util.input_util import bool_input
 from meeple.util.output_util import print_error, print_info
 
 
-@click.command()
+@click.command(name="open")
+@click.argument("id", type=int)
 @click.help_option("-h", "--help")
-@click.argument("id")
 # TODO: add -y option to automatically confirm opening on browser
-def open_on_bgg(id: str) -> None:
-    """Open a board game or expansion on the BoardGameGeek website.
+def open_on_bgg(id: int) -> None:
+    """Open an item on BoardGameGeek.
 
     - ID is the BoardGameGeek ID of the board game/expansion to be opened on boardgamegeek.com.
     """
-    # check that the given ID is an integer
-    if not id.isdigit():
-        sys.exit(print_error("Provided ID must be an integer value"))
-    bgg_id = int(id)
-
     # check that the given id is a valid BoardGameGeek ID
+    bgg_id = id
     api_result = get_bgg_items([bgg_id])
     if not api_result:
         sys.exit(print_error(f"Provided '{bgg_id}' is not a valid BoardGameGeek ID"))
 
     # confirm the user wants to open the board game/expansion on BoardGameGeek website
     item = api_result[0]
     url = f"https://{BGG_DOMAIN}/{item.type}/{bgg_id}"
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/rename.py` & `meeple-cli-0.1.0b4/src/meeple/command/rename.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import sys
 
 import click
 
 from meeple.util.collection_util import is_collection, rename_collection
+from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import rename_collection_data_dir
 from meeple.util.output_util import print_error, print_info
 
 
 @click.command()
-@click.help_option("-h", "--help")
-@click.argument("collection")
+@click.argument("collection", shell_complete=complete_collections)
 @click.argument("new_name")
+@click.help_option("-h", "--help")
 def rename(collection: str, new_name: str) -> None:
     """Rename a local collection.
 
     - COLLECTION is the name of the collection to be renamed.
     - NEW_NAME is the new name to assign to the collection.
     """
     # check that the given collection is a valid collection
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/search.py` & `meeple-cli-0.1.0b4/src/meeple/command/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import click
 
 from meeple.util.api_util import search_bgg
-from meeple.util.output_util import print_table
+from meeple.util.output_util import fmt_year, print_table
 
 
 @click.command()
-@click.help_option("-h", "--help")
 @click.argument("query")
+@click.help_option("-h", "--help")
 # TODO: add option to sort output by different columns
 # TODO: add verbosity flag to show more info about each result
 def search(query: str) -> None:
-    """Search BoardGameGeek for a board game or expansion.
+    """Search BoardGameGeek for items.
 
     - QUERY is the text to be searched for on BoardGameGeek. If searching multiple words, surround with quotes.
     """
     # search BoardGameGeek with user provided query
     api_result = search_bgg(query)
     api_result.sort(key=lambda x: x.id)
 
@@ -23,13 +23,13 @@
     rows = []
     for item in api_result:
         cols = []
         cols.extend(
             [
                 str(item.id),
                 item.name,
-                str(item.year),
+                fmt_year(item.year),
             ]
         )
         rows.append(cols)
 
     print_table(rows, headers)
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/stats.py` & `meeple-cli-0.1.0b4/src/meeple/command/stats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import sys
 
 import click
 
 from meeple.util.collection_util import is_collection
+from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import get_collection_data
 from meeple.util.output_util import (
     fmt_avg_rank,
     fmt_rating,
     fmt_weight,
     print_error,
     print_info,
     print_table,
     print_warning,
 )
 
 
 @click.command()
-@click.help_option("-h", "--help")
-@click.argument("collection")
+@click.argument("collection", shell_complete=complete_collections)
 @click.option(
     "-b",
     "--boardgames",
-    "type",
+    "item_type",
     is_flag=True,
-    flag_value="b",
-    help="Include only board games in output.",
+    flag_value="bg",
+    help="Output only board games.",
 )
 @click.option(
     "-e",
     "--expansions",
-    "type",
+    "item_type",
     is_flag=True,
-    flag_value="e",
-    help="Include only expansions in output.",
+    flag_value="ex",
+    help="Output only expansions.",
 )
-def stats(collection: str, type: str) -> None:
-    """Print out the details of a local collection.
+@click.help_option("-h", "--help")
+def stats(collection: str, item_type: str) -> None:
+    """Print out the details of a collection.
 
     - COLLECTION is the name of the collection to be detailed.
     """
     # check that the given collection is a valid collection
     if not is_collection(collection):
         sys.exit(print_error(f"'{collection}' is not a valid collection"))
 
@@ -50,17 +51,17 @@
         sys.exit(
             print_warning(
                 f"local data not found for '{collection}'. update with `meeple update {collection}`"
             )
         )
 
     # determine what to include in results depending on given flags
-    if type == "b":
+    if item_type == "bg":
         out_list = boardgames
-    elif type == "e":
+    elif item_type == "ex":
         out_list = expansions
     else:
         out_list = boardgames + expansions
 
     # calculate stats
     sum_ratings = (
         num_rated
@@ -91,17 +92,17 @@
         avg_rank = 0
     if num_weighted > 0:
         avg_weight = round(sum_weight / num_weighted, 2)
     else:
         avg_weight = 0
     avg_max_players = round(sum_players / len(out_list), 2)
 
-    if type == "b":
+    if item_type == "bg":
         header = f"{collection} ({len(boardgames)} Boardgames)"
-    elif type == "e":
+    elif item_type == "ex":
         header = f"{collection} ({len(expansions)} Expansions)"
     else:
         header = f"{collection} ({len(boardgames)} Board games | {len(expansions)} Expansions)"
 
     print_info(header)
     print_table(
         [
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/command/update.py` & `meeple-cli-0.1.0b4/src/meeple/command/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import sys
 
 import click
 
 from meeple.util.api_util import BOARDGAME_TYPE, EXPANSION_TYPE, get_bgg_items
 from meeple.util.collection_util import get_collections, is_collection, read_collection
+from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import write_collection_data
 from meeple.util.output_util import print_error, print_info, print_warning
 from meeple.util.sort_util import sort_items
 
 
 @click.command()
+@click.argument("collection", required=False, shell_complete=complete_collections)
 @click.help_option("-h", "--help")
-@click.argument("collection", required=False)
 def update(collection: str) -> None:
     """Update local collection data.
 
     - COLLECTION (optional) is the name of the collection to be updated. If not provided, update all collections.
     """
     print_info("Updating local data...")
     # update only a specific collection, if given
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/root.py` & `meeple-cli-0.1.0b4/src/meeple/root.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,64 @@
 import click
 
 from meeple.command import (
     add,
     collections,
+    completions,
     delete,
     drop,
+    find,
     hot,
     info,
     list_collection,
     move,
     new,
     open_on_bgg,
     rename,
     search,
     stats,
     update,
 )
+from meeple.util.cmd_util import SectionedHelpGroup
 
-
-@click.group(help="Local board game collection manager. Powered by BoardGameGeek.")
+commands = {
+    "Collection Commands": [
+        add,
+        collections,
+        delete,
+        drop,
+        find,
+        list_collection,
+        move,
+        new,
+        rename,
+        stats,
+        update,
+    ],
+    "BoardGameGeek Commands": [hot, info, open_on_bgg, search],
+    "Other Commands": [completions],
+}
+
+
+@click.group(
+    cls=SectionedHelpGroup,
+    help="Local board game collection manager. Powered by BoardGameGeek.",
+)
 @click.help_option("-h", "--help")
 @click.version_option(
     None,  # use version auto discovery
     "-v",
     "--version",
     package_name="meeple-cli",
     message="%(prog)s-cli, v%(version)s",
 )
 def cli() -> None:
     """Main 'meeple' command."""
     pass
 
 
-cli.add_command(add, "add")
-cli.add_command(collections, "collections")
-cli.add_command(delete, "delete")
-cli.add_command(drop, "drop")
-cli.add_command(info, "info")
-cli.add_command(hot, "hot")
-cli.add_command(list_collection, "list")
-cli.add_command(move, "move")
-cli.add_command(new, "new")
-cli.add_command(open_on_bgg, "open")
-cli.add_command(rename, "rename")
-cli.add_command(search, "search")
-cli.add_command(stats, "stats")
-cli.add_command(update, "update")
+for section, cmds in commands.items():
+    for cmd in cmds:
+        cli.add_command(cmd, section=section)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/type/item.py` & `meeple-cli-0.1.0b4/src/meeple/type/item.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,20 @@
 
     def __str__(self) -> str:
         return json.dumps(dict(self), ensure_ascii=False)
 
     def __repr__(self) -> str:
         return self.__str__()
 
+    def __eq__(self, other) -> bool:
+        return self.id == other.id
+
+    def __hash__(self):
+        return hash(("id", self.id))
+
     @staticmethod
     def from_json(json_dict):
         return Item(
             json_dict["id"],
             json_dict["name"],
             json_dict["type"],
             json_dict["year"],
@@ -99,14 +105,16 @@
         name = _grab_first(bgg_dict["name"])
         if bgg_dict.get("@type"):
             item_type = bgg_dict["@type"]
         else:
             item_type = None
         if bgg_dict.get("yearpublished"):
             year = bgg_dict["yearpublished"]["@value"]
+        else:
+            year = 0
         if bgg_dict.get("statistics"):
             stats_dict = bgg_dict["statistics"]["ratings"]
             rating = round(_parse_item_float_val(stats_dict["average"]), 2)
             weight = round(_parse_item_float_val(stats_dict["averageweight"]), 2)
             rank = _parse_item_rank(stats_dict["ranks"])
         if bgg_dict.get("minplayers"):
             minplayers = bgg_dict["minplayers"]["@value"]
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/util/api_util.py` & `meeple-cli-0.1.0b4/src/meeple/util/api_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b3/src/meeple/util/data_util.py` & `meeple-cli-0.1.0b4/src/meeple/util/data_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b3/src/meeple/util/fs_util.py` & `meeple-cli-0.1.0b4/src/meeple/util/fs_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b3/src/meeple/util/output_util.py` & `meeple-cli-0.1.0b4/src/meeple/util/output_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,83 @@
 import numbers
 
 from rich import box
 from rich.console import Console
 from rich.table import Table
 
+from meeple.util.api_util import BOARDGAME_TYPE, EXPANSION_TYPE
+
+NA = "[bright_black]NA[/bright_black]"
+
 
 def fmt_players(minplayers: str, maxplayers: str) -> str:
+    if int(minplayers) == int(maxplayers) == 0:
+        return NA
     return f"{minplayers}-{maxplayers}"
 
 
 def fmt_playtime(minplaytime: str, maxplaytime: str) -> str:
+    if int(minplaytime) == int(maxplaytime) == 0:
+        return NA
     return f"{minplaytime}-{maxplaytime} Min"
 
 
 def fmt_avg_rank(rank: str) -> str:
     if not isinstance(rank, numbers.Number) or int(rank) == 0:
-        return "[bright_black]NA[/bright_black]"
+        return NA
     rank_str = f"{rank:.2f}"
     return rank_str
 
 
 def fmt_rank(rank: str) -> str:
     if rank == "NA" or not rank.isdigit():
-        return "[bright_black]NA[/bright_black]"
+        return NA
     return rank
 
 
 def fmt_rating(rating: float) -> str:
     rating_str = f"{rating:.2f}"
     if rating >= 8:
         return f"[green]{rating_str}[/green]"
     if rating >= 7:
         return f"[blue]{rating_str}[/blue]"
     if rating > 6:
         return f"[magenta]{rating_str}[/magenta]"
     if rating == 0:
-        return "[bright_black]NA[/bright_black]"
+        return NA
     return f"[red]{rating_str}[/red]"
 
 
+def fmt_type(item_type: str) -> str:
+    if item_type == BOARDGAME_TYPE:
+        return "Board Game"
+    if item_type == EXPANSION_TYPE:
+        return "Expansion"
+    return NA
+
+
 def fmt_weight(weight: float) -> str:
     weight_str = f"{weight:.2f}"
     if weight >= 4:
         return f"[red]{weight_str}[/red]"
     if weight >= 3:
         return f"[yellow]{weight_str}[/yellow]"
     if weight >= 2:
         return f"[bright_yellow]{weight_str}[/bright_yellow]"
     if weight == 0:
-        return "[bright_black]NA[/bright_black]"
+        return NA
     return f"[green]{weight_str}[/green]"
 
 
+def fmt_year(year: str) -> str:
+    if int(year) == 0:
+        return NA
+    return year
+
+
 def print_error(message: str) -> None:
     print_table([["[red]Error[/red]", message]])
 
 
 def print_info(message: str) -> None:
     print_table([[message]])
```

### Comparing `meeple-cli-0.1.0b3/src/meeple/util/sort_util.py` & `meeple-cli-0.1.0b4/src/meeple/util/sort_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b3/PKG-INFO` & `meeple-cli-0.1.0b4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeple-cli
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: Local board game collection manager. Powered by BoardGameGeek.
 Author-email: Bradley Wojcik <bradleycwojcik@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: click >=8
 Requires-Dist: rich >=13
@@ -27,25 +27,26 @@
 Provides-Extra: test
 
 # meeple-cli
 
 [![build status](https://img.shields.io/github/actions/workflow/status/boldandbrad/meeple-cli/python-test.yml?branch=main&logo=github)](https://github.com/boldandbrad/meeple-cli/actions/workflows/python-test.yml?query=branch%3Amain)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![pypi](https://img.shields.io/pypi/v/meeple-cli)](https://pypi.org/project/meeple-cli/)
-![downloads](https://img.shields.io/pypi/dm/meeple-cli)
+[![downloads](https://img.shields.io/pypi/dm/meeple-cli)](https://pypistats.org/packages/meeple-cli)
 
 <!-- [![codecov](https://codecov.io/gh/boldandbrad/meeple-cli/branch/main/graph/badge.svg)](https://codecov.io/gh/boldandbrad/meeple-cli) -->
 <!-- [![Docs](https://img.shields.io/website?down_message=down&label=docs&up_message=online&url=https%3A%2F%2Fboldandbrad.github.io%2Fmeeple-cli%2F)](https://boldandbrad.github.io/meeple-cli/) -->
 
-**Local board game collection manager. Powered by [BoardGameGeek](https://boardgamegeek.com).**
+**Local board game collection manager. Powered by
+[BoardGameGeek](https://boardgamegeek.com).**
 
-> `meeple-cli` allows you to create and manage _local_ board game collections
-> stored on your system. At this time the [BoardGameGeek API](https://boardgamegeek.com/wiki/page/BGG_XML_API2)
-> does not allow for creation nor modification of GeekLists directly. Nor is
-> `meeple-cli` affiliated with BoardGameGeek.
+## Disclaimer
+
+> Neither `meeple-cli` nor its maintainers are affiliated with
+> [BoardGameGeek](https://boardgamegeek.com).
 
 ## Install
 
 Global isolated install via [pipx](https://pypa.github.io/pipx/) (recommended):
 
 ```sh
 pipx install meeple-cli
@@ -58,64 +59,109 @@
 ```
 
 <!-- ```zsh
 brew tap boldandbrad/homebrew-tap
 brew install meeple-cli
 ```-->
 
-<!-- > For more details, read the **meeple-cli** [install guide](https://boldandbrad.github.io/meeple-cli/#/install). -->
+<!-- > For more details, read the **meeple-cli**
+> [install guide](https://boldandbrad.github.io/meeple-cli/#/install). -->
 
 ## Usage
 
-```sh
+```txt
 $ meeple --help
 Usage: meeple [OPTIONS] COMMAND [ARGS]...
 
   Local board game collection manager. Powered by BoardGameGeek.
 
 Options:
   -h, --help     Show this message and exit.
   -v, --version  Show the version and exit.
 
-Commands:
-  add          Add a board game/extension to a collection.
-  collections  List all local collections.
-  delete       Delete a local collection.
-  drop         Remove a board game/extension from a collection.
-  hot          Retrieve the current BoardGameGeek hotness list.
-  info         Print out the details of a board game or expansion.
-  list         List all board games/extensions in a collection.
-  move         Move a board game/extension from one collection to another.
-  new          Create a new local collection.
-  open         Open a board game or expansion on the BoardGameGeek website.
+Collection Commands:
+  add          Add an item to a collection.
+  collections  List all collections.
+  delete       Delete a collection.
+  drop         Remove an item from a collection.
+  find         Search collections for items.
+  list         List contents of a collection.
+  move         Move an item from one collection to another.
+  new          Create a new collection.
   rename       Rename a local collection.
-  search       Search BoardGameGeek for a board game or expansion.
-  stats        Print out the details of a local collection.
+  stats        Print out the details of a collection.
   update       Update local collection data.
+
+BoardGameGeek Commands:
+  hot     List current BoardGameGeek trending items.
+  info    Print out the details of an item.
+  open    Open an item on BoardGameGeek.
+  search  Search BoardGameGeek for items.
+
+Other Commands:
+  completions  Setup meeple shell completions.
+```
+
+<!-- > For more usage details, read the **meeple-cli**
+> [usage guide](https://boldandbrad.github.io/meeple-cli/#/usage). -->
+
+## Completions
+
+`meeple-cli` supports shell completions for `bash`, `zsh`, and `fish`. For
+setup, use `meeple completions <SHELL>`, or the following instructions:
+
+<details>
+<summary>bash</summary>
+
+Add the following to `~/.bashrc`:
+
+```sh
+eval "$(_MEEPLE_COMPLETE=bash_source meeple)"
+```
+
+</details>
+
+<details>
+<summary>zsh</summary>
+
+Add the following to `~/.zshrc`:
+
+```sh
+eval "$(_MEEPLE_COMPLETE=zsh_source meeple)"
+```
+
+</details>
+
+<details>
+<summary>fish</summary>
+
+Save the script to `~/.config/fish/completions/meeple.fish`:
+
+```sh
+_MEEPLE_COMPLETE=fish_source meeple > ~/.config/fish/completions/meeple.fish
 ```
 
-<!-- > For more usage details, read the **meeple-cli** [usage guide](https://boldandbrad.github.io/meeple-cli/#/usage). -->
+</details>
 
 ## Roadmap
 
-See a list of already implemented features/changes in the [Changelog](docs/changelog.md).
+See a list of already implemented features/changes in the
+[Changelog](docs/changelog.md).
 
 ### Planned Features
 
-- [ ] Find board games/expansions across local collections by attributes ->
-      `meeple find`
 - [ ] Verbose option on `meeple info` that includes additional info such as
       description, publishers, etc
-- [ ] Copy a local collection -> `meeple copy`
-- [ ] Export a local collection to csv or another format -> `meeple export`
-- [ ] Import a local collection from a variety of formats -> `meeple import`
-- [ ] Ability to assign and manage personal ratings of board games/expansions
+- [ ] Export a collection to csv or another format -> `meeple export`
+- [ ] Import a collection from a variety of formats -> `meeple import`
 
 ### Potential Features (May or may not happen)
 
+- [ ] Ability to assign and manage personal ratings of board games/expansions
+- [ ] Copy a collection -> `meeple copy`
 - [ ] Copy option `-c` on most commands that allows you to interactively select
       and copy text from the command output (for grabbing IDs) - similar to yank
 - [ ] Manage user preferences/configs -> `meeple config` stored at
       `~/.meeple/config.json` or something
   - [ ] Toggle colorized output
   - [ ] Set custom default output sorts
   - [ ] Set custom data location
@@ -131,22 +177,39 @@
         BoardGameGeek over time
 - [ ] Ability to record and manage plays of board games - would be nuts.
   - [ ] Ability to calculate and surface play statistics for a board game
 - [ ] Ability to interact with discord services to show that you are currently
       playing a board game?
 - [ ] Ability to actually interact with BoardGameGeek user
       profile/settings/collections (not all currently possible via the API)
-- [ ] Shell completions for common shells? For finding/searching.
 
 ### Other Todos
 
 - [ ] Unit tests
 - [ ] Documentation site (via vitepress?)
-- [ ] Homebrew formula (will be available [here](https://github.com/boldandbrad/homebrew-tap))
+- [ ] Homebrew formula (will be available
+      [here](https://github.com/boldandbrad/homebrew-tap))
 - [ ] Implement simple logging for debugging (local, not telemetry) (via
       loguru?)
 
+## FAQ
+
+### Why local only collections?
+
+Currently, the
+[BoardGameGeek Public API](https://boardgamegeek.com/wiki/page/BGG_XML_API2)
+provides limited _read-only_ data about user collections/GeekLists.
+
+While it is _technically_ feasible to interface with GeekLists via
+webscrapers/spiders, this kind of practice would be both complex and also
+violate [BoardGameGeek Terms of Service](https://boardgamegeek.com/terms#toc22).
+
+### Where does `meeple-cli` store data?
+
+`meeple-cli` stores collection data in `~/.meeple` and only makes network
+connections to retrieve data from the BoardGameGeek API.
+
 ## License
 
 Copyright (c) 2023 Bradley Wojcik. Released under the MIT License. See
 [LICENSE](LICENSE) for details.
```

