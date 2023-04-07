# Comparing `tmp/robotframework-tidy-4.0.1.tar.gz` & `tmp/robotframework-tidy-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-tidy-4.0.1.tar", last modified: Mon Apr  3 12:45:40 2023, max compression
+gzip compressed data, was "robotframework-tidy-4.1.0.tar", last modified: Fri Apr  7 18:36:45 2023, max compression
```

## Comparing `robotframework-tidy-4.0.1.tar` & `robotframework-tidy-4.1.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:45:40.409738 robotframework-tidy-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-03 12:45:40.409738 robotframework-tidy-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:45:40.393737 robotframework-tidy-4.0.1/robotframework_tidy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-03 12:45:40.000000 robotframework-tidy-4.0.1/robotframework_tidy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-03 12:45:40.000000 robotframework-tidy-4.0.1/robotframework_tidy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 12:45:40.000000 robotframework-tidy-4.0.1/robotframework_tidy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-03 12:45:40.000000 robotframework-tidy-4.0.1/robotframework_tidy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-03 12:45:40.000000 robotframework-tidy-4.0.1/robotframework_tidy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-03 12:45:40.000000 robotframework-tidy-4.0.1/robotframework_tidy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:45:40.401738 robotframework-tidy-4.0.1/robotidy/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:45:40.401738 robotframework-tidy-4.0.1/robotidy/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-03 12:45:40.000000 robotframework-tidy-4.0.1/robotidy/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-03 12:45:40.000000 robotframework-tidy-4.0.1/robotidy/__pycache__/version.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    19101 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/rich_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:45:40.409738 robotframework-tidy-4.0.1/robotidy/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/AddMissingEnd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/AlignKeywordsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/AlignSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/AlignTemplatedTestCases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/AlignTestCasesSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/AlignVariablesSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/DiscardEmptySections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/GenerateDocumentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/IndentNestedKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/InlineIf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/MergeAndOrderSections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/NormalizeAssignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/NormalizeComments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/NormalizeNewLines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/NormalizeSectionHeaderName.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/NormalizeSeparators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/NormalizeSettingName.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/NormalizeTags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/OrderSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/OrderSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/OrderTags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/RemoveEmptySettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/RenameKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/RenameTestCases.py
--rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/RenameVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/ReplaceBreakContinue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/ReplaceEmptyValues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/ReplaceReturns.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/ReplaceRunKeywordIf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/SmartSortKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/SplitTooLongLine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/Translate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19572 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23237 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/aligners_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/transformers/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    13418 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/robotidy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 12:45:40.409738 robotframework-tidy-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-03 12:45:25.000000 robotframework-tidy-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:36:45.826517 robotframework-tidy-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-07 18:36:45.826517 robotframework-tidy-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:36:45.818516 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:36:45.822517 robotframework-tidy-4.1.0/robotidy/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:36:45.822517 robotframework-tidy-4.1.0/robotidy/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotidy/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotidy/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19515 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/rich_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:36:45.826517 robotframework-tidy-4.1.0/robotidy/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AddMissingEnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AlignKeywordsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AlignSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AlignTemplatedTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AlignTestCasesSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AlignVariablesSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/DiscardEmptySections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/GenerateDocumentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/IndentNestedKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/InlineIf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/MergeAndOrderSections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeAssignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeComments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeNewLines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSectionHeaderName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSeparators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSettingName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeTags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/OrderSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/OrderSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/OrderTags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/RemoveEmptySettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/RenameKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/RenameTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/RenameVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/ReplaceBreakContinue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/ReplaceEmptyValues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/ReplaceReturns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/ReplaceRunKeywordIf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/SmartSortKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/SplitTooLongLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/Translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19572 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23237 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/aligners_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13418 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 18:36:45.826517 robotframework-tidy-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/setup.py
```

### Comparing `robotframework-tidy-4.0.1/LICENSE` & `robotframework-tidy-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/PKG-INFO` & `robotframework-tidy-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-tidy
-Version: 4.0.1
+Version: 4.1.0
 Summary: Code autoformatter for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-tidy
 Author: MarketSquare - Robot Framework community
 Author-email: bartek.hirsz@gmail.com
 License: Apache License 2.0
 Keywords: robotframework
 Platform: any
```

### Comparing `robotframework-tidy-4.0.1/README.md` & `robotframework-tidy-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotframework_tidy.egg-info/PKG-INFO` & `robotframework-tidy-4.1.0/robotframework_tidy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-tidy
-Version: 4.0.1
+Version: 4.1.0
 Summary: Code autoformatter for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-tidy
 Author: MarketSquare - Robot Framework community
 Author-email: bartek.hirsz@gmail.com
 License: Apache License 2.0
 Keywords: robotframework
 Platform: any
```

### Comparing `robotframework-tidy-4.0.1/robotframework_tidy.egg-info/SOURCES.txt` & `robotframework-tidy-4.1.0/robotframework_tidy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/api.py` & `robotframework-tidy-4.1.0/robotidy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
             TransformConfig(
                 tr, force_include=force_included, custom_transformer=custom_transformer, is_config=is_config
             )
             for tr in config.get(param_name, ())
         ]
 
     # TODO Refactor - Config should be read in one place both for API and CLI
-    # TODO Remove kwargs usage - other SDKs are not using this feature
-    config = files.find_and_read_config((src,))
+    ignore_git_dir = kwargs.get("ignore_git_dir", False)
+    config = files.find_and_read_config((src,), ignore_git_dir)
     config = {k: str(v) if not isinstance(v, (list, dict)) else v for k, v in config.items()}
     transformer_list = convert_transformers_config("transform", config, force_included=True)
     custom_transformers = convert_transformers_config("load-transformers", config, custom_transformer=True)
     configurations = convert_transformers_config("configure", config, is_config=True)
     transformer_config = TransformConfigMap(transformer_list, custom_transformers, configurations)
     formatting_config = get_formatting_config(config, kwargs)
     exclude = config.get("exclude", None)
```

### Comparing `robotframework-tidy-4.0.1/robotidy/app.py` & `robotframework-tidy-4.1.0/robotidy/app.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/cli.py` & `robotframework-tidy-4.1.0/robotidy/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,17 @@
 
 
 def read_config(ctx: click.Context, param: click.Parameter, value: Optional[str]) -> Optional[str]:
     # if --config was not used, try to find pyproject.toml or robotidy.toml file
     if value:
         config = files.read_pyproject_config(value)
     else:
-        config = files.find_and_read_config(ctx.params["src"] or (str(Path(".").resolve()),))
+        src = ctx.params["src"] or (str(Path(".").resolve()),)
+        ignore_git_dir = ctx.params["ignore_git_dir"]
+        config = files.find_and_read_config(src, ignore_git_dir)
     if not config:
         return
     # Sanitize the values to be Click friendly. For more information please see:
     # https://github.com/psf/black/issues/1458
     # https://github.com/pallets/click/issues/1567
     config = {k: str(v) if not isinstance(v, (list, dict)) else v for k, v in config.items()}
     if "src" in config:
@@ -287,14 +289,22 @@
 @click.option(
     "--skip-gitignore",
     is_flag=True,
     show_default=True,
     help="Skip **.gitignore** files and do not ignore files listed inside.",
 )
 @click.option(
+    "--ignore-git-dir",
+    is_flag=True,
+    is_eager=True,
+    help="Ignore .git directories when searching for the default configuration file. "
+    "By default first parent directory with .git directory is returned and this flag disables this behaviour.",
+    show_default=True,
+)
+@click.option(
     "--config",
     type=click.Path(
         exists=True,
         file_okay=True,
         dir_okay=False,
         readable=True,
         allow_dash=False,
@@ -505,14 +515,15 @@
     list_transformers: str,
     desc: Optional[str],
     output: Optional[Path],
     force_order: bool,
     target_version: int,
     language: Optional[List[str]],
     reruns: int,
+    ignore_git_dir: bool,
     skip_comments: bool,
     skip_documentation: bool,
     skip_return_values: bool,
     skip_keyword_call: List[str],
     skip_keyword_call_pattern: List[str],
     skip_settings: bool,
     skip_arguments: bool,
```

### Comparing `robotframework-tidy-4.0.1/robotidy/config.py` & `robotframework-tidy-4.1.0/robotidy/config.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/decorators.py` & `robotframework-tidy-4.1.0/robotidy/decorators.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/disablers.py` & `robotframework-tidy-4.1.0/robotidy/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/exceptions.py` & `robotframework-tidy-4.1.0/robotidy/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/files.py` & `robotframework-tidy-4.1.0/robotidy/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pathspec import PathSpec
 
 DEFAULT_EXCLUDES = r"/(\.direnv|\.eggs|\.git|\.hg|\.nox|\.tox|\.venv|venv|\.svn)/"
 INCLUDE_EXT = (".robot", ".resource")
 
 
 @lru_cache()
-def find_project_root(srcs: Iterable[str]) -> Path:
+def find_project_root(srcs: Iterable[str], ignore_git_dir: bool = False) -> Path:
     """Return a directory containing .git, or robotidy.toml.
     That directory will be a common parent of all files and directories
     passed in `srcs`.
     If no directory in the tree contains a marker that would specify it's the
     project root, the root of the file system is returned.
     """
     if not srcs:
@@ -33,28 +33,28 @@
 
     common_base = max(
         set.intersection(*(set(parents) for parents in src_parents)),
         key=lambda path: path.parts,
     )
 
     for directory in (common_base, *common_base.parents):
-        if (directory / ".git").exists():
+        if not ignore_git_dir and (directory / ".git").exists():
             return directory
 
         if (directory / "robotidy.toml").is_file():
             return directory
 
         if (directory / "pyproject.toml").is_file():
             return directory
 
     return directory
 
 
-def find_and_read_config(src_paths: Iterable[str]) -> Dict[str, Any]:
-    project_root = find_project_root(src_paths)
+def find_and_read_config(src_paths: Iterable[str], ignore_git_dir: bool = False) -> Dict[str, Any]:
+    project_root = find_project_root(src_paths, ignore_git_dir)
     config_path = project_root / "robotidy.toml"
     if config_path.is_file():
         return read_pyproject_config(str(config_path))
     pyproject_path = project_root / "pyproject.toml"
     if pyproject_path.is_file():
         return read_pyproject_config(str(pyproject_path))
     return {}
```

### Comparing `robotframework-tidy-4.0.1/robotidy/skip.py` & `robotframework-tidy-4.1.0/robotidy/skip.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/AddMissingEnd.py` & `robotframework-tidy-4.1.0/robotidy/transformers/AddMissingEnd.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/AlignKeywordsSection.py` & `robotframework-tidy-4.1.0/robotidy/transformers/AlignKeywordsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/AlignSettingsSection.py` & `robotframework-tidy-4.1.0/robotidy/transformers/AlignSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/AlignTemplatedTestCases.py` & `robotframework-tidy-4.1.0/robotidy/transformers/AlignTemplatedTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/AlignTestCasesSection.py` & `robotframework-tidy-4.1.0/robotidy/transformers/AlignTestCasesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/AlignVariablesSection.py` & `robotframework-tidy-4.1.0/robotidy/transformers/AlignVariablesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/DiscardEmptySections.py` & `robotframework-tidy-4.1.0/robotidy/transformers/DiscardEmptySections.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/GenerateDocumentation.py` & `robotframework-tidy-4.1.0/robotidy/transformers/GenerateDocumentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/IndentNestedKeywords.py` & `robotframework-tidy-4.1.0/robotidy/transformers/IndentNestedKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/InlineIf.py` & `robotframework-tidy-4.1.0/robotidy/transformers/InlineIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/MergeAndOrderSections.py` & `robotframework-tidy-4.1.0/robotidy/transformers/MergeAndOrderSections.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/NormalizeAssignments.py` & `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeAssignments.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/NormalizeComments.py` & `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeComments.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/NormalizeNewLines.py` & `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeNewLines.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/NormalizeSectionHeaderName.py` & `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSectionHeaderName.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/NormalizeSeparators.py` & `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSeparators.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/NormalizeSettingName.py` & `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSettingName.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/NormalizeTags.py` & `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/OrderSettings.py` & `robotframework-tidy-4.1.0/robotidy/transformers/OrderSettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/OrderSettingsSection.py` & `robotframework-tidy-4.1.0/robotidy/transformers/OrderSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/OrderTags.py` & `robotframework-tidy-4.1.0/robotidy/transformers/OrderTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/RemoveEmptySettings.py` & `robotframework-tidy-4.1.0/robotidy/transformers/RemoveEmptySettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/RenameKeywords.py` & `robotframework-tidy-4.1.0/robotidy/transformers/RenameKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/RenameTestCases.py` & `robotframework-tidy-4.1.0/robotidy/transformers/RenameTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/RenameVariables.py` & `robotframework-tidy-4.1.0/robotidy/transformers/RenameVariables.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/ReplaceBreakContinue.py` & `robotframework-tidy-4.1.0/robotidy/transformers/ReplaceBreakContinue.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/ReplaceEmptyValues.py` & `robotframework-tidy-4.1.0/robotidy/transformers/ReplaceEmptyValues.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/ReplaceReturns.py` & `robotframework-tidy-4.1.0/robotidy/transformers/ReplaceReturns.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/ReplaceRunKeywordIf.py` & `robotframework-tidy-4.1.0/robotidy/transformers/ReplaceRunKeywordIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/SmartSortKeywords.py` & `robotframework-tidy-4.1.0/robotidy/transformers/SmartSortKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/SplitTooLongLine.py` & `robotframework-tidy-4.1.0/robotidy/transformers/SplitTooLongLine.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/Translate.py` & `robotframework-tidy-4.1.0/robotidy/transformers/Translate.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/__init__.py` & `robotframework-tidy-4.1.0/robotidy/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/aligners_core.py` & `robotframework-tidy-4.1.0/robotidy/transformers/aligners_core.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/transformers/run_keywords.py` & `robotframework-tidy-4.1.0/robotidy/transformers/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/robotidy/utils.py` & `robotframework-tidy-4.1.0/robotidy/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.0.1/setup.py` & `robotframework-tidy-4.1.0/setup.py`

 * *Files identical despite different names*

