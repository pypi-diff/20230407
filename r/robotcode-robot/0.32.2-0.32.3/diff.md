# Comparing `tmp/robotcode_robot-0.32.2.tar.gz` & `tmp/robotcode_robot-0.32.3.tar.gz`

## Comparing `robotcode_robot-0.32.2.tar` & `robotcode_robot-0.32.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    79577 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/LICENSE.txt
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/README.md
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/pyproject.toml
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 robotcode_robot-0.32.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    77296 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/LICENSE.txt
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/README.md
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/pyproject.toml
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 robotcode_robot-0.32.3/PKG-INFO
```

### Comparing `robotcode_robot-0.32.2/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.32.3/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.32.2/src/robotcode/robot/config/model.py` & `robotcode_robot-0.32.3/src/robotcode/robot/config/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -354,15 +354,14 @@
         description="""\
             Use colors on console output or not.
             auto: use colors when output not redirected (default)
             on:   always use colors
             ansi: like `on` but use ANSI colors also on Windows
             off:  disable colors altogether
 
-            ---
             corresponds to the `-C --consolecolors auto|on|ansi|off` option of _robot_
             """,
         robot_name="consolecolors",
         robot_priority=500,
         robot_short_name="C",
     )
     doc: Optional[Union[str, StringExpression]] = field(
@@ -376,56 +375,51 @@
             Examples:
 
             ```
             --doc "Very *good* example"
             --doc doc_from_file.txt
             ```
 
-            ---
             corresponds to the `-D --doc documentation` option of _robot_
             """,
         robot_name="doc",
         robot_priority=500,
         robot_short_name="D",
     )
     excludes: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Select test cases not to run by tag. These tests are
             not run even if included with --include. Tags are
             matched using same rules as with --include.
 
-            ---
             corresponds to the `-e --exclude tag *` option of _robot_
             """,
         robot_name="exclude",
         robot_priority=500,
         robot_short_name="e",
     )
-    expand_keywords: Optional[List[Union[NamePattern, TagPattern]]] = field(
+    expand_keywords: Optional[List[Union[str, NamePattern, TagPattern]]] = field(
         description="""\
             Matching keywords will be automatically expanded in
             the log file. Matching against keyword name or tags
             work using same rules as with --removekeywords.
 
             Examples:
 
             ```
             --expandkeywords name:BuiltIn.Log
             --expandkeywords tag:expand
             ```
 
-            ---
             corresponds to the `--expandkeywords name:<pattern>|tag:<pattern> *` option of _robot_
             """,
         robot_name="expandkeywords",
         robot_priority=500,
     )
-    flatten_keywords: Optional[
-        Optional[List[Union[str, Literal["for", "while", "iteration"], NamePattern, TagPattern]]]
-    ] = field(
+    flatten_keywords: Optional[List[Union[str, Literal["for", "while", "iteration"], NamePattern, TagPattern]]] = field(
         description="""\
             Flattens matching keywords in the generated log file.
             Matching keywords get all log messages from their
             child keywords and children are discarded otherwise.
             for:     flatten FOR loops fully
             while:   flatten WHILE loops fully
             iteration: flatten FOR/WHILE loop iterations
@@ -433,15 +427,14 @@
             name:<pattern>:  flatten matched keywords using same
             matching rules as with
             `--removekeywords name:<pattern>`
             tag:<pattern>:  flatten matched keywords using same
             matching rules as with
             `--removekeywords tag:<pattern>`
 
-            ---
             corresponds to the `--flattenkeywords for|while|iteration|name:<pattern>|tag:<pattern> *` option of _robot_
             """,
         robot_name="flattenkeywords",
         robot_priority=500,
     )
     includes: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
@@ -454,15 +447,14 @@
             Examples:
 
             ```
             --include foo --include bar*
             --include fooANDbar*
             ```
 
-            ---
             corresponds to the `-i --include tag *` option of _robot_
             """,
         robot_name="include",
         robot_priority=500,
         robot_short_name="i",
     )
     log: Optional[Union[str, StringExpression]] = field(
@@ -472,90 +464,83 @@
 
             Examples:
 
             ```
             `--log mylog.html`, `-l NONE`
             ```
 
-            ---
             corresponds to the `-l --log file` option of _robot_
             """,
         robot_name="log",
         robot_priority=500,
         robot_short_name="l",
     )
     log_title: Optional[Union[str, StringExpression]] = field(
         description="""\
             Title for the generated log file. The default title
             is `<SuiteName> Log`.
 
-            ---
             corresponds to the `--logtitle title` option of _robot_
             """,
         robot_name="logtitle",
         robot_priority=500,
     )
     metadata: Optional[Dict[str, Union[str, StringExpression]]] = field(
         description="""\
             Set metadata of the top level suite. Value can
             contain formatting and be read from a file similarly
             as --doc. Example: --metadata Version:1.2
 
-            ---
             corresponds to the `-M --metadata name:value *` option of _robot_
             """,
         robot_name="metadata",
         robot_priority=500,
         robot_short_name="M",
     )
     name: Optional[Union[str, StringExpression]] = field(
         description="""\
             Set the name of the top level suite. By default the
             name is created based on the executed file or
             directory.
 
-            ---
             corresponds to the `-N --name name` option of _robot_
             """,
         robot_name="name",
         robot_priority=500,
         robot_short_name="N",
     )
     no_status_rc: Union[bool, Flag, None] = field(
         description="""\
             Sets the return code to zero regardless of failures
             in test cases. Error codes are returned normally.
 
-            ---
             corresponds to the `--nostatusrc` option of _robot_
             """,
         robot_name="statusrc",
         robot_priority=500,
         robot_is_flag=True,
         robot_flag_default=False,
     )
     output_dir: Optional[Union[str, StringExpression]] = field(
         description="""\
             Where to create output files. The default is the
             directory where tests are run from and the given path
             is considered relative to that unless it is absolute.
 
-            ---
             corresponds to the `-d --outputdir dir` option of _robot_
             """,
         robot_name="outputdir",
         robot_priority=500,
         robot_short_name="d",
     )
     pre_rebot_modifiers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Class to programmatically modify the result
             model before creating reports and logs.
 
-            ---
             corresponds to the `--prerebotmodifier class *` option of _robot_
             """,
         robot_name="prerebotmodifier",
         robot_priority=500,
     )
     python_path: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
@@ -569,22 +554,23 @@
             Examples:
 
             ```
             --pythonpath libs/
             --pythonpath /opt/libs:libraries.zip
             ```
 
-            ---
             corresponds to the `-P --pythonpath path *` option of _robot_
             """,
         robot_name="pythonpath",
         robot_priority=500,
         robot_short_name="P",
     )
-    remove_keywords: Optional[List[Union[Literal["all", "passed", "for", "wuks"], NamePattern, TagPattern]]] = field(
+    remove_keywords: Optional[
+        List[Union[str, Literal["all", "passed", "for", "wuks"], NamePattern, TagPattern]]
+    ] = field(
         description="""\
             Remove keyword data from the generated log file.
             Keywords containing warnings are not removed except
             in the `all` mode.
             all:     remove data from all keywords
             passed:  remove data only from keywords in passed
             test cases and suites
@@ -617,26 +603,24 @@
             Examples:
 
             ```
             --removekeywords foo
             --removekeywords fooANDbar*
             ```
 
-            ---
             corresponds to the `--removekeywords all|passed|for|wuks|name:<pattern>|tag:<pattern> *` option of _robot_
             """,
         robot_name="removekeywords",
         robot_priority=500,
     )
     report: Optional[Union[str, StringExpression]] = field(
         description="""\
             HTML report file. Can be disabled with `NONE`
             similarly as --log. Default: report.html
 
-            ---
             corresponds to the `-r --report file` option of _robot_
             """,
         robot_name="report",
         robot_priority=500,
         robot_short_name="r",
     )
     report_background: Optional[Union[str, StringExpression]] = field(
@@ -649,62 +633,57 @@
             Examples:
 
             ```
             --reportbackground green:red:yellow
             --reportbackground #00E:#E00
             ```
 
-            ---
             corresponds to the `--reportbackground colors` option of _robot_
             """,
         robot_name="reportbackground",
         robot_priority=500,
     )
     report_title: Optional[Union[str, StringExpression]] = field(
         description="""\
             Title for the generated report file. The default
             title is `<SuiteName> Report`.
 
-            ---
             corresponds to the `--reporttitle title` option of _robot_
             """,
         robot_name="reporttitle",
         robot_priority=500,
     )
     rpa: Union[bool, Flag, None] = field(
         description="""\
             Turn on the generic automation mode. Mainly affects
             terminology so that "test" is replaced with "task"
             in logs and reports. By default the mode is got
             from test/task header in data files.
 
-            ---
             corresponds to the `--rpa` option of _robot_
             """,
         robot_name="rpa",
         robot_priority=500,
         robot_is_flag=True,
     )
     set_tag: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Sets given tag(s) to all executed tests.
 
-            ---
             corresponds to the `-G --settag tag *` option of _robot_
             """,
         robot_name="settag",
         robot_priority=500,
         robot_short_name="G",
     )
     split_log: Union[bool, Flag, None] = field(
         description="""\
             Split the log file into smaller pieces that open in
             browsers transparently.
 
-            ---
             corresponds to the `--splitlog` option of _robot_
             """,
         robot_name="splitlog",
         robot_priority=500,
         robot_is_flag=True,
     )
     suites: Optional[List[Union[str, StringExpression]]] = field(
@@ -713,28 +692,26 @@
             --test, --include or --exclude, only tests in
             matching suites and also matching other filtering
             criteria are selected. Name can be a simple pattern
             similarly as with --test and it can contain parent
             name separated with a dot. For example, `-s X.Y`
             selects suite `Y` only if its parent is `X`.
 
-            ---
             corresponds to the `-s --suite name *` option of _robot_
             """,
         robot_name="suite",
         robot_priority=500,
         robot_short_name="s",
     )
     suite_stat_level: Optional[int] = field(
         description="""\
             How many levels to show in `Statistics by Suite`
             in log and report. By default all suite levels are
             shown. Example:  --suitestatlevel 3
 
-            ---
             corresponds to the `--suitestatlevel level` option of _robot_
             """,
         robot_name="suitestatlevel",
         robot_priority=500,
     )
     tag_doc: Optional[Dict[str, Union[str, StringExpression]]] = field(
         description="""\
@@ -747,15 +724,14 @@
             Examples:
 
             ```
             --tagdoc mytag:Example
             --tagdoc "owner-*:Original author"
             ```
 
-            ---
             corresponds to the `--tagdoc pattern:doc *` option of _robot_
             """,
         robot_name="tagdoc",
         robot_priority=500,
     )
     tag_stat_combine: Optional[List[Union[str, Dict[str, str]]]] = field(
         description="""\
@@ -768,39 +744,36 @@
             Examples:
 
             ```
             --tagstatcombine requirement-*
             --tagstatcombine tag1ANDtag2:My_name
             ```
 
-            ---
             corresponds to the `--tagstatcombine tags:name *` option of _robot_
             """,
         robot_name="tagstatcombine",
         robot_priority=500,
     )
     tag_stat_exclude: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Exclude matching tags from `Statistics by Tag`.
             This option can be used with --tagstatinclude
             similarly as --exclude is used with --include.
 
-            ---
             corresponds to the `--tagstatexclude tag *` option of _robot_
             """,
         robot_name="tagstatexclude",
         robot_priority=500,
     )
     tag_stat_include: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Include only matching tags in `Statistics by Tag`
             in log and report. By default all tags are shown.
             Given tag can be a pattern like with --include.
 
-            ---
             corresponds to the `--tagstatinclude tag *` option of _robot_
             """,
         robot_name="tagstatinclude",
         robot_priority=500,
     )
     tag_stat_link: Optional[Dict[str, Union[str, StringExpression]]] = field(
         description="""\
@@ -813,40 +786,37 @@
             Examples:
 
             ```
             --tagstatlink mytag:http://my.domain:Title
             --tagstatlink "bug-*:http://url/id=%1:Issue Tracker"
             ```
 
-            ---
             corresponds to the `--tagstatlink pattern:link:title *` option of _robot_
             """,
         robot_name="tagstatlink",
         robot_priority=500,
     )
     tasks: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Alias to --test. Especially applicable with --rpa.
 
-            ---
             corresponds to the `--task name *` option of _robot_
             """,
         robot_name="task",
         robot_priority=500,
     )
     tests: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Select tests by name or by long name containing also
             parent suite name like `Parent.Test`. Name is case
             and space insensitive and it can also be a simple
             pattern where `*` matches anything, `?` matches any
             single character, and `[chars]` matches one character
             in brackets.
 
-            ---
             corresponds to the `-t --test name *` option of _robot_
             """,
         robot_name="test",
         robot_priority=500,
         robot_short_name="t",
     )
     timestamp_outputs: Union[bool, Flag, None] = field(
@@ -854,28 +824,26 @@
             When this option is used, timestamp in a format
             `YYYYMMDD-hhmmss` is added to all generated output
             files between their basename and extension. For
             example `-T -o output.xml -r report.html -l none`
             creates files like `output-20070503-154410.xml` and
             `report-20070503-154410.html`.
 
-            ---
             corresponds to the `-T --timestampoutputs` option of _robot_
             """,
         robot_name="timestampoutputs",
         robot_priority=500,
         robot_short_name="T",
         robot_is_flag=True,
     )
     xunit: Optional[Union[str, StringExpression]] = field(
         description="""\
             xUnit compatible result file. Not created unless this
             option is specified.
 
-            ---
             corresponds to the `-x --xunit file` option of _robot_
             """,
         robot_name="xunit",
         robot_priority=500,
         robot_short_name="x",
     )
 
@@ -884,153 +852,130 @@
 class CommonExtraOptions(BaseOptions):
     """Extra common options for all _robot_ commands."""
 
     extra_excludes: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --exclude option.
 
-            ---
-
             Select test cases not to run by tag. These tests are
             not run even if included with --include. Tags are
             matched using same rules as with --include.
 
-            ---
             corresponds to the `-e --exclude tag *` option of _robot_
             """,
     )
-    extra_expand_keywords: Optional[List[Union[NamePattern, TagPattern]]] = field(
+    extra_expand_keywords: Optional[List[Union[str, NamePattern, TagPattern]]] = field(
         description="""\
             Appends entries to the --expandkeywords option.
 
-            ---
-
             Matching keywords will be automatically expanded in
             the log file. Matching against keyword name or tags
             work using same rules as with --removekeywords.
 
             Examples:
 
             ```
             --expandkeywords name:BuiltIn.Log
             --expandkeywords tag:expand
             ```
 
-            ---
             corresponds to the `--expandkeywords name:<pattern>|tag:<pattern> *` option of _robot_
             """,
     )
     extra_flatten_keywords: Optional[
-        Optional[List[Union[str, Literal["for", "while", "iteration"], NamePattern, TagPattern]]]
+        List[Union[str, Literal["for", "while", "iteration"], NamePattern, TagPattern]]
     ] = field(
         description="""\
             Appends entries to the --flattenkeywords option.
 
-            ---
-
             Flattens matching keywords in the generated log file.
             Matching keywords get all log messages from their
             child keywords and children are discarded otherwise.
             for:     flatten FOR loops fully
             while:   flatten WHILE loops fully
             iteration: flatten FOR/WHILE loop iterations
             foritem: deprecated alias for `iteration`
             name:<pattern>:  flatten matched keywords using same
             matching rules as with
             `--removekeywords name:<pattern>`
             tag:<pattern>:  flatten matched keywords using same
             matching rules as with
             `--removekeywords tag:<pattern>`
 
-            ---
             corresponds to the `--flattenkeywords for|while|iteration|name:<pattern>|tag:<pattern> *` option of _robot_
             """,
     )
     extra_includes: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --include option.
 
-            ---
-
             Select tests by tag. Similarly as name with --test,
             tag is case and space insensitive and it is possible
             to use patterns with `*`, `?` and `[]` as wildcards.
             Tags and patterns can also be combined together with
             `AND`, `OR`, and `NOT` operators.
 
             Examples:
 
             ```
             --include foo --include bar*
             --include fooANDbar*
             ```
 
-            ---
             corresponds to the `-i --include tag *` option of _robot_
             """,
     )
     extra_metadata: Optional[Dict[str, Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --metadata option.
 
-            ---
-
             Set metadata of the top level suite. Value can
             contain formatting and be read from a file similarly
             as --doc. Example: --metadata Version:1.2
 
-            ---
             corresponds to the `-M --metadata name:value *` option of _robot_
             """,
     )
     extra_pre_rebot_modifiers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Appends entries to the --prerebotmodifier option.
 
-            ---
-
             Class to programmatically modify the result
             model before creating reports and logs.
 
-            ---
             corresponds to the `--prerebotmodifier class *` option of _robot_
             """,
     )
     extra_python_path: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --pythonpath option.
 
-            ---
-
             Additional locations (directories, ZIPs) where to
             search libraries and other extensions when they are
             imported. Multiple paths can be given by separating
             them with a colon (`:`) or by using this option
             several times. Given path can also be a glob pattern
             matching multiple paths.
 
             Examples:
 
             ```
             --pythonpath libs/
             --pythonpath /opt/libs:libraries.zip
             ```
 
-            ---
             corresponds to the `-P --pythonpath path *` option of _robot_
             """,
     )
     extra_remove_keywords: Optional[
-        List[Union[Literal["all", "passed", "for", "wuks"], NamePattern, TagPattern]]
+        List[Union[str, Literal["all", "passed", "for", "wuks"], NamePattern, TagPattern]]
     ] = field(
         description="""\
             Appends entries to the --removekeywords option.
 
-            ---
-
             Remove keyword data from the generated log file.
             Keywords containing warnings are not removed except
             in the `all` mode.
             all:     remove data from all keywords
             passed:  remove data only from keywords in passed
             test cases and suites
             for:     remove passed iterations from for loops
@@ -1062,171 +1007,143 @@
             Examples:
 
             ```
             --removekeywords foo
             --removekeywords fooANDbar*
             ```
 
-            ---
             corresponds to the `--removekeywords all|passed|for|wuks|name:<pattern>|tag:<pattern> *` option of _robot_
             """,
     )
     extra_set_tag: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --settag option.
 
-            ---
-
             Sets given tag(s) to all executed tests.
 
-            ---
             corresponds to the `-G --settag tag *` option of _robot_
             """,
     )
     extra_suites: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --suite option.
 
-            ---
-
             Select suites by name. When this option is used with
             --test, --include or --exclude, only tests in
             matching suites and also matching other filtering
             criteria are selected. Name can be a simple pattern
             similarly as with --test and it can contain parent
             name separated with a dot. For example, `-s X.Y`
             selects suite `Y` only if its parent is `X`.
 
-            ---
             corresponds to the `-s --suite name *` option of _robot_
             """,
     )
     extra_tag_doc: Optional[Dict[str, Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --tagdoc option.
 
-            ---
-
             Add documentation to tags matching the given
             pattern. Documentation is shown in `Test Details` and
             also as a tooltip in `Statistics by Tag`. Pattern can
             use `*`, `?` and `[]` as wildcards like --test.
             Documentation can contain formatting like --doc.
 
             Examples:
 
             ```
             --tagdoc mytag:Example
             --tagdoc "owner-*:Original author"
             ```
 
-            ---
             corresponds to the `--tagdoc pattern:doc *` option of _robot_
             """,
     )
     extra_tag_stat_combine: Optional[List[Union[str, Dict[str, str]]]] = field(
         description="""\
             Appends entries to the --tagstatcombine option.
 
-            ---
-
             Create combined statistics based on tags.
             These statistics are added into `Statistics by Tag`.
             If the optional `name` is not given, name of the
             combined tag is got from the specified tags. Tags are
             matched using the same rules as with --include.
 
             Examples:
 
             ```
             --tagstatcombine requirement-*
             --tagstatcombine tag1ANDtag2:My_name
             ```
 
-            ---
             corresponds to the `--tagstatcombine tags:name *` option of _robot_
             """,
     )
     extra_tag_stat_exclude: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --tagstatexclude option.
 
-            ---
-
             Exclude matching tags from `Statistics by Tag`.
             This option can be used with --tagstatinclude
             similarly as --exclude is used with --include.
 
-            ---
             corresponds to the `--tagstatexclude tag *` option of _robot_
             """,
     )
     extra_tag_stat_include: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --tagstatinclude option.
 
-            ---
-
             Include only matching tags in `Statistics by Tag`
             in log and report. By default all tags are shown.
             Given tag can be a pattern like with --include.
 
-            ---
             corresponds to the `--tagstatinclude tag *` option of _robot_
             """,
     )
     extra_tag_stat_link: Optional[Dict[str, Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --tagstatlink option.
 
-            ---
-
             Add external links into `Statistics by
             Tag`. Pattern can use `*`, `?` and `[]` as wildcards
             like --test. Characters matching to `*` and `?`
             wildcards can be used in link and title with syntax
             %N, where N is index of the match (starting from 1).
 
             Examples:
 
             ```
             --tagstatlink mytag:http://my.domain:Title
             --tagstatlink "bug-*:http://url/id=%1:Issue Tracker"
             ```
 
-            ---
             corresponds to the `--tagstatlink pattern:link:title *` option of _robot_
             """,
     )
     extra_tasks: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --task option.
 
-            ---
-
             Alias to --test. Especially applicable with --rpa.
 
-            ---
             corresponds to the `--task name *` option of _robot_
             """,
     )
     extra_tests: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --test option.
 
-            ---
-
             Select tests by name or by long name containing also
             parent suite name like `Parent.Test`. Name is case
             and space insensitive and it can also be a simple
             pattern where `*` matches anything, `?` matches any
             single character, and `[chars]` matches one character
             in brackets.
 
-            ---
             corresponds to the `-t --test name *` option of _robot_
             """,
     )
 
 
 @dataclass
 class RobotOptions(BaseOptions):
@@ -1237,97 +1154,89 @@
             How to report execution on the console.
             verbose:  report every suite and test (default)
             dotted:   only show `.` for passed test, `s` for
             skipped tests, and `F` for failed tests
             quiet:    no output except for errors and warnings
             none:     no output whatsoever
 
-            ---
             corresponds to the `--console type` option of _robot_
             """,
         robot_name="console",
         robot_priority=500,
     )
     console_markers: Optional[Literal["auto", "on", "off"]] = field(
         description="""\
             Show markers on the console when top level
             keywords in a test case end. Values have same
             semantics as with --consolecolors.
 
-            ---
             corresponds to the `-K --consolemarkers auto|on|off` option of _robot_
             """,
         robot_name="consolemarkers",
         robot_priority=500,
         robot_short_name="K",
     )
     console_width: Optional[int] = field(
         description="""\
             Width of the console output. Default is 78.
 
-            ---
             corresponds to the `-W --consolewidth chars` option of _robot_
             """,
         robot_name="consolewidth",
         robot_priority=500,
         robot_short_name="W",
     )
     debug_file: Optional[Union[str, StringExpression]] = field(
         description="""\
             Debug file written during execution. Not created
             unless this option is specified.
 
-            ---
             corresponds to the `-b --debugfile file` option of _robot_
             """,
         robot_name="debugfile",
         robot_priority=500,
         robot_short_name="b",
     )
     dotted: Union[bool, Flag, None] = field(
         description="""\
             Shortcut for `--console dotted`.
 
-            ---
             corresponds to the `-. --dotted` option of _robot_
             """,
         robot_name="dotted",
         robot_priority=500,
         robot_short_name=".",
         robot_is_flag=True,
     )
     dry_run: Union[bool, Flag, None] = field(
         description="""\
             Verifies test data and runs tests so that library
             keywords are not executed.
 
-            ---
             corresponds to the `--dryrun` option of _robot_
             """,
         robot_name="dryrun",
         robot_priority=500,
         robot_is_flag=True,
     )
     exit_on_error: Union[bool, Flag, None] = field(
         description="""\
             Stops test execution if any error occurs when parsing
             test data, importing libraries, and so on.
 
-            ---
             corresponds to the `--exitonerror` option of _robot_
             """,
         robot_name="exitonerror",
         robot_priority=500,
         robot_is_flag=True,
     )
     exit_on_failure: Union[bool, Flag, None] = field(
         description="""\
             Stops test execution if any test fails.
 
-            ---
             corresponds to the `-X --exitonfailure` option of _robot_
             """,
         robot_name="exitonfailure",
         robot_priority=500,
         robot_short_name="X",
         robot_is_flag=True,
     )
@@ -1343,28 +1252,26 @@
             ```
             `--extension txt`, `--extension robot:txt`
             ```
 
 
             Only `*.robot` files are parsed by default.
 
-            ---
             corresponds to the `-F --extension value` option of _robot_
             """,
         robot_name="extension",
         robot_priority=500,
         robot_short_name="F",
     )
     languages: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Activate localization. `lang` can be a name or a code
             of a built-in language, or a path or a module name of
             a custom language file.
 
-            ---
             corresponds to the `--language lang *` option of _robot_
             """,
         robot_name="language",
         robot_priority=500,
     )
     listeners: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
@@ -1376,15 +1283,14 @@
             Examples:
 
             ```
             --listener MyListenerClass
             --listener path/to/Listener.py:arg1:arg2
             ```
 
-            ---
             corresponds to the `--listener class *` option of _robot_
             """,
         robot_name="listener",
         robot_priority=500,
     )
     log_level: Optional[Union[str, StringExpression]] = field(
         description="""\
@@ -1396,41 +1302,38 @@
             Examples:
 
             ```
             --loglevel DEBUG
             --loglevel DEBUG:INFO
             ```
 
-            ---
             corresponds to the `-L --loglevel level` option of _robot_
             """,
         robot_name="loglevel",
         robot_priority=500,
         robot_short_name="L",
     )
     max_assign_length: Optional[int] = field(
         description="""\
             Maximum number of characters to show in log
             when variables are assigned. Zero or negative values
             can be used to avoid showing assigned values at all.
             Default is 200.
 
-            ---
             corresponds to the `--maxassignlength characters` option of _robot_
             """,
         robot_name="maxassignlength",
         robot_priority=500,
     )
     max_error_lines: Optional[int] = field(
         description="""\
             Maximum number of error message lines to show in
             report when tests fail. Default is 40, minimum is 10
             and `NONE` can be used to show the full message.
 
-            ---
             corresponds to the `--maxerrorlines lines` option of _robot_
             """,
         robot_name="maxerrorlines",
         robot_priority=500,
     )
     output: Optional[Union[str, StringExpression]] = field(
         description="""\
@@ -1439,37 +1342,34 @@
             relative to --outputdir unless given as an absolute
             path. Other output files are created based on XML
             output files after the test execution and XML outputs
             can also be further processed with Rebot tool. Can be
             disabled by giving a special value `NONE`.
             Default: output.xml
 
-            ---
             corresponds to the `-o --output file` option of _robot_
             """,
         robot_name="output",
         robot_priority=500,
         robot_short_name="o",
     )
     pre_run_modifiers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Class to programmatically modify the suite
             structure before execution.
 
-            ---
             corresponds to the `--prerunmodifier class *` option of _robot_
             """,
         robot_name="prerunmodifier",
         robot_priority=500,
     )
     quiet: Union[bool, Flag, None] = field(
         description="""\
             Shortcut for `--console quiet`.
 
-            ---
             corresponds to the `--quiet` option of _robot_
             """,
         robot_name="quiet",
         robot_priority=500,
         robot_is_flag=True,
     )
     randomize: Optional[Union[str, Literal["all", "suites", "tests", "none"]]] = field(
@@ -1485,86 +1385,79 @@
             Examples:
 
             ```
             --randomize all
             --randomize tests:1234
             ```
 
-            ---
             corresponds to the `--randomize all|suites|tests|none` option of _robot_
             """,
         robot_name="randomize",
         robot_priority=500,
     )
     re_run_failed: Optional[Union[str, StringExpression]] = field(
         description="""\
             Select failed tests from an earlier output file to be
             re-executed. Equivalent to selecting same tests
             individually using --test.
 
-            ---
             corresponds to the `-R --rerunfailed output` option of _robot_
             """,
         robot_name="rerunfailed",
         robot_priority=500,
         robot_short_name="R",
     )
     re_run_failed_suites: Optional[Union[str, StringExpression]] = field(
         description="""\
             Select failed suites from an earlier output
             file to be re-executed.
 
-            ---
             corresponds to the `-S --rerunfailedsuites output` option of _robot_
             """,
         robot_name="rerunfailedsuites",
         robot_priority=500,
         robot_short_name="S",
     )
     run_empty_suite: Union[bool, Flag, None] = field(
         description="""\
             Executes suite even if it contains no tests. Useful
             e.g. with --include/--exclude when it is not an error
             that no test matches the condition.
 
-            ---
             corresponds to the `--runemptysuite` option of _robot_
             """,
         robot_name="runemptysuite",
         robot_priority=500,
         robot_is_flag=True,
     )
     skip: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Tests having given tag will be skipped. Tag can be
             a pattern.
 
-            ---
             corresponds to the `--skip tag *` option of _robot_
             """,
         robot_name="skip",
         robot_priority=500,
     )
     skip_on_failure: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Tests having given tag will be skipped if they fail.
             Tag can be a pattern
 
-            ---
             corresponds to the `--skiponfailure tag *` option of _robot_
             """,
         robot_name="skiponfailure",
         robot_priority=500,
     )
     skip_teardown_on_exit: Union[bool, Flag, None] = field(
         description="""\
             Causes teardowns to be skipped if test execution is
             stopped prematurely.
 
-            ---
             corresponds to the `--skipteardownonexit` option of _robot_
             """,
         robot_name="skipteardownonexit",
         robot_priority=500,
         robot_is_flag=True,
     )
     variables: Optional[Dict[str, Union[str, StringExpression]]] = field(
@@ -1578,15 +1471,14 @@
 
             ```
             --variable str:Hello       =>  ${str} = `Hello`
             -v hi:Hi_World -E space:_  =>  ${hi} = `Hi World`
             -v x: -v y:42              =>  ${x} = ``, ${y} = `42`
             ```
 
-            ---
             corresponds to the `-v --variable name:value *` option of _robot_
             """,
         robot_name="variable",
         robot_priority=500,
         robot_short_name="v",
     )
     variable_files: Optional[List[Union[str, StringExpression]]] = field(
@@ -1598,15 +1490,14 @@
             Examples:
 
             ```
             --variablefile path/vars.yaml
             --variablefile environment.py:testing
             ```
 
-            ---
             corresponds to the `-V --variablefile path *` option of _robot_
             """,
         robot_name="variablefile",
         robot_priority=500,
         robot_short_name="V",
     )
 
@@ -1615,127 +1506,106 @@
 class RobotExtraOptions(BaseOptions):
     """Extra options for _robot_ command."""
 
     extra_languages: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --language option.
 
-            ---
-
             Activate localization. `lang` can be a name or a code
             of a built-in language, or a path or a module name of
             a custom language file.
 
-            ---
-            corresponds to the `--language lang *` option of _robot_
+            corresponds to the `--language lang *` option of _rebot_
             """,
     )
     extra_listeners: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Appends entries to the --listener option.
 
-            ---
-
             A class for monitoring test execution. Gets
             notifications e.g. when tests start and end.
             Arguments to the listener class can be given after
             the name using a colon or a semicolon as a separator.
 
             Examples:
 
             ```
             --listener MyListenerClass
             --listener path/to/Listener.py:arg1:arg2
             ```
 
-            ---
-            corresponds to the `--listener class *` option of _robot_
+            corresponds to the `--listener class *` option of _rebot_
             """,
     )
     extra_pre_run_modifiers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Appends entries to the --prerunmodifier option.
 
-            ---
-
             Class to programmatically modify the suite
             structure before execution.
 
-            ---
-            corresponds to the `--prerunmodifier class *` option of _robot_
+            corresponds to the `--prerunmodifier class *` option of _rebot_
             """,
     )
     extra_skip: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --skip option.
 
-            ---
-
             Tests having given tag will be skipped. Tag can be
             a pattern.
 
-            ---
-            corresponds to the `--skip tag *` option of _robot_
+            corresponds to the `--skip tag *` option of _rebot_
             """,
     )
     extra_skip_on_failure: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --skiponfailure option.
 
-            ---
-
             Tests having given tag will be skipped if they fail.
             Tag can be a pattern
 
-            ---
-            corresponds to the `--skiponfailure tag *` option of _robot_
+            corresponds to the `--skiponfailure tag *` option of _rebot_
             """,
     )
     extra_variables: Optional[Dict[str, Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --variable option.
 
-            ---
-
             Set variables in the test data. Only scalar
             variables with string value are supported and name is
             given without `${}`. See --variablefile for a more
             powerful variable setting mechanism.
 
             Examples:
 
             ```
             --variable str:Hello       =>  ${str} = `Hello`
             -v hi:Hi_World -E space:_  =>  ${hi} = `Hi World`
             -v x: -v y:42              =>  ${x} = ``, ${y} = `42`
             ```
 
-            ---
-            corresponds to the `-v --variable name:value *` option of _robot_
+            corresponds to the `-v --variable name:value *` option of _rebot_
             """,
     )
     extra_variable_files: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --variablefile option.
 
-            ---
-
             Python or YAML file file to read variables from.
             Possible arguments to the variable file can be given
             after the path using colon or semicolon as separator.
 
             Examples:
 
             ```
             --variablefile path/vars.yaml
             --variablefile environment.py:testing
             ```
 
-            ---
-            corresponds to the `-V --variablefile path *` option of _robot_
+            corresponds to the `-V --variablefile path *` option of _rebot_
             """,
     )
 
 
 @dataclass
 class RebotOptions(BaseOptions):
     """Options for _rebot_ command."""
@@ -1744,16 +1614,15 @@
         description="""\
             Same as --starttime but for end time. If both options
             are used, elapsed time of the suite is calculated
             based on them. For combined suites, it is otherwise
             calculated by adding elapsed times of the combined
             suites together.
 
-            ---
-            corresponds to the `--endtime timestamp` option of _robot_
+            corresponds to the `--endtime timestamp` option of _rebot_
             """,
         robot_name="endtime",
         robot_priority=500,
     )
     log_level: Optional[Union[str, StringExpression]] = field(
         description="""\
             Threshold for selecting messages. Available levels:
@@ -1764,58 +1633,54 @@
             Examples:
 
             ```
             --loglevel DEBUG
             --loglevel DEBUG:INFO
             ```
 
-            ---
-            corresponds to the `-L --loglevel level` option of _robot_
+            corresponds to the `-L --loglevel level` option of _rebot_
             """,
         robot_name="loglevel",
         robot_priority=500,
         robot_short_name="L",
     )
     merge: Union[bool, Flag, None] = field(
         description="""\
             When combining results, merge outputs together
             instead of putting them under a new top level suite.
             Example: rebot --merge orig.xml rerun.xml
 
-            ---
-            corresponds to the `-R --merge` option of _robot_
+            corresponds to the `-R --merge` option of _rebot_
             """,
         robot_name="merge",
         robot_priority=500,
         robot_short_name="R",
         robot_is_flag=True,
     )
     output: Optional[Union[str, StringExpression]] = field(
         description="""\
             XML output file. Not created unless this option is
             specified. Given path, similarly as paths given to
             --log, --report and --xunit, is relative to
             --outputdir unless given as an absolute path.
 
-            ---
-            corresponds to the `-o --output file` option of _robot_
+            corresponds to the `-o --output file` option of _rebot_
             """,
         robot_name="output",
         robot_priority=500,
         robot_short_name="o",
     )
     process_empty_suite: Union[bool, Flag, None] = field(
         description="""\
             Processes output also if the top level suite is
             empty. Useful e.g. with --include/--exclude when it
             is not an error that there are no matches.
             Use --skiponfailure when starting execution instead.
 
-            ---
-            corresponds to the `--processemptysuite` option of _robot_
+            corresponds to the `--processemptysuite` option of _rebot_
             """,
         robot_name="processemptysuite",
         robot_priority=500,
         robot_is_flag=True,
     )
     start_time: Optional[Union[str, StringExpression]] = field(
         description="""\
@@ -1824,16 +1689,15 @@
             are optional (e.g. `20071001151242268` is ok too) and
             parts from milliseconds to hours can be omitted if
             they are zero (e.g. `2007-10-01`). This can be used
             to override start time of a single suite or to set
             start time for a combined suite, which would
             otherwise be `N/A`.
 
-            ---
-            corresponds to the `--starttime timestamp` option of _robot_
+            corresponds to the `--starttime timestamp` option of _rebot_
             """,
         robot_name="starttime",
         robot_priority=500,
     )
 
 
 @dataclass
@@ -1844,220 +1708,201 @@
         description="""\
             Specifies the source documentation format. Possible
             values are Robot Framework's documentation format,
             HTML, plain text, and reStructuredText. The default
             value can be specified in library source code and
             the initial default value is ROBOT.
 
-            ---
-            corresponds to the `-F --docformat ROBOT|HTML|TEXT|REST` option of _robot_
+            corresponds to the `-F --docformat ROBOT|HTML|TEXT|REST` option of _libdoc_
             """,
         robot_name="docformat",
         robot_priority=500,
         robot_short_name="F",
     )
     format: Optional[Literal["HTML", "XML", "JSON", "LIBSPEC"]] = field(
         description="""\
             Specifies whether to generate an HTML output for
             humans or a machine readable spec file in XML or JSON
             format. The LIBSPEC format means XML spec with
             documentations converted to HTML. The default format
             is got from the output file extension.
 
-            ---
-            corresponds to the `-f --format HTML|XML|JSON|LIBSPEC` option of _robot_
+            corresponds to the `-f --format HTML|XML|JSON|LIBSPEC` option of _libdoc_
             """,
         robot_name="format",
         robot_priority=500,
         robot_short_name="f",
     )
     name: Optional[Union[str, StringExpression]] = field(
         description="""\
             Sets the name of the documented library or resource.
 
-            ---
-            corresponds to the `-n --name name` option of _robot_
+            corresponds to the `-n --name name` option of _libdoc_
             """,
         robot_name="name",
         robot_priority=500,
         robot_short_name="n",
     )
     python_path: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Additional locations where to search for libraries
             and resources.
 
-            ---
-            corresponds to the `-P --pythonpath path *` option of _robot_
+            corresponds to the `-P --pythonpath path *` option of _libdoc_
             """,
         robot_name="pythonpath",
         robot_priority=500,
         robot_short_name="P",
     )
     quiet: Union[bool, Flag, None] = field(
         description="""\
             Do not print the path of the generated output file
             to the console. New in RF 4.0.
 
-            ---
-            corresponds to the `--quiet` option of _robot_
+            corresponds to the `--quiet` option of _libdoc_
             """,
         robot_name="quiet",
         robot_priority=500,
         robot_is_flag=True,
     )
     spec_doc_format: Optional[Literal["RAW", "HTML"]] = field(
         description="""\
             Specifies the documentation format used with XML and
             JSON spec files. RAW means preserving the original
             documentation format and HTML means converting
             documentation to HTML. The default is RAW with XML
             spec files and HTML with JSON specs and when using
             the special LIBSPEC format. New in RF 4.0.
 
-            ---
-            corresponds to the `-s --specdocformat RAW|HTML` option of _robot_
+            corresponds to the `-s --specdocformat RAW|HTML` option of _libdoc_
             """,
         robot_name="specdocformat",
         robot_priority=500,
         robot_short_name="s",
     )
     theme: Optional[Literal["DARK", "LIGHT", "NONE"]] = field(
         description="""\
             Use dark or light HTML theme. If this option is not
             used, or the value is NONE, the theme is selected
             based on the browser color scheme. New in RF 6.0.
 
-            ---
-            corresponds to the `--theme DARK|LIGHT|NONE` option of _robot_
+            corresponds to the `--theme DARK|LIGHT|NONE` option of _libdoc_
             """,
         robot_name="theme",
         robot_priority=500,
     )
 
 
 @dataclass
 class LibDocExtraOptions(BaseOptions):
     """Extra options for _libdoc_ command."""
 
     extra_python_path: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --pythonpath option.
 
-            ---
-
             Additional locations where to search for libraries
             and resources.
 
-            ---
-            corresponds to the `-P --pythonpath path *` option of _robot_
+            corresponds to the `-P --pythonpath path *` option of _libdoc_
             """,
     )
 
 
 @dataclass
 class TestDocOptions(BaseOptions):
     """Options for _testdoc_ command."""
 
     doc: Optional[Union[str, StringExpression]] = field(
         description="""\
             Override the documentation of the top level suite.
 
-            ---
-            corresponds to the `-D --doc document` option of _robot_
+            corresponds to the `-D --doc document` option of _testdoc_
             """,
         robot_name="doc",
         robot_priority=500,
         robot_short_name="D",
     )
     excludes: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Exclude tests by tags.
 
-            ---
-            corresponds to the `-e --exclude tag *` option of _robot_
+            corresponds to the `-e --exclude tag *` option of _testdoc_
             """,
         robot_name="exclude",
         robot_priority=500,
         robot_short_name="e",
     )
     includes: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Include tests by tags.
 
-            ---
-            corresponds to the `-i --include tag *` option of _robot_
+            corresponds to the `-i --include tag *` option of _testdoc_
             """,
         robot_name="include",
         robot_priority=500,
         robot_short_name="i",
     )
     metadata: Optional[Dict[str, Union[str, StringExpression]]] = field(
         description="""\
             Set/override metadata of the top level suite.
 
-            ---
-            corresponds to the `-M --metadata name:value *` option of _robot_
+            corresponds to the `-M --metadata name:value *` option of _testdoc_
             """,
         robot_name="metadata",
         robot_priority=500,
         robot_short_name="M",
     )
     name: Optional[Union[str, StringExpression]] = field(
         description="""\
             Override the name of the top level suite.
 
-            ---
-            corresponds to the `-N --name name` option of _robot_
+            corresponds to the `-N --name name` option of _testdoc_
             """,
         robot_name="name",
         robot_priority=500,
         robot_short_name="N",
     )
     set_tag: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Set given tag(s) to all test cases.
 
-            ---
-            corresponds to the `-G --settag tag *` option of _robot_
+            corresponds to the `-G --settag tag *` option of _testdoc_
             """,
         robot_name="settag",
         robot_priority=500,
         robot_short_name="G",
     )
     suites: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Include suites by name.
 
-            ---
-            corresponds to the `-s --suite name *` option of _robot_
+            corresponds to the `-s --suite name *` option of _testdoc_
             """,
         robot_name="suite",
         robot_priority=500,
         robot_short_name="s",
     )
     tests: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Include tests by name.
 
-            ---
-            corresponds to the `-t --test name *` option of _robot_
+            corresponds to the `-t --test name *` option of _testdoc_
             """,
         robot_name="test",
         robot_priority=500,
         robot_short_name="t",
     )
     title: Optional[Union[str, StringExpression]] = field(
         description="""\
             Set the title of the generated documentation.
             Underscores in the title are converted to spaces.
             The default title is the name of the top level suite.
 
-            ---
-            corresponds to the `-T --title title` option of _robot_
+            corresponds to the `-T --title title` option of _testdoc_
             """,
         robot_name="title",
         robot_priority=500,
         robot_short_name="T",
     )
 
 
@@ -2065,80 +1910,62 @@
 class TestDocExtraOptions(BaseOptions):
     """Extra options for _testdoc_ command."""
 
     extra_excludes: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --exclude option.
 
-            ---
-
             Exclude tests by tags.
 
-            ---
-            corresponds to the `-e --exclude tag *` option of _robot_
+            corresponds to the `-e --exclude tag *` option of _testdoc_
             """,
     )
     extra_includes: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --include option.
 
-            ---
-
             Include tests by tags.
 
-            ---
-            corresponds to the `-i --include tag *` option of _robot_
+            corresponds to the `-i --include tag *` option of _testdoc_
             """,
     )
     extra_metadata: Optional[Dict[str, Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --metadata option.
 
-            ---
-
             Set/override metadata of the top level suite.
 
-            ---
-            corresponds to the `-M --metadata name:value *` option of _robot_
+            corresponds to the `-M --metadata name:value *` option of _testdoc_
             """,
     )
     extra_set_tag: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --settag option.
 
-            ---
-
             Set given tag(s) to all test cases.
 
-            ---
-            corresponds to the `-G --settag tag *` option of _robot_
+            corresponds to the `-G --settag tag *` option of _testdoc_
             """,
     )
     extra_suites: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --suite option.
 
-            ---
-
             Include suites by name.
 
-            ---
-            corresponds to the `-s --suite name *` option of _robot_
+            corresponds to the `-s --suite name *` option of _testdoc_
             """,
     )
     extra_tests: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --test option.
 
-            ---
-
             Include tests by name.
 
-            ---
-            corresponds to the `-t --test name *` option of _robot_
+            corresponds to the `-t --test name *` option of _testdoc_
             """,
     )
 
 
 # end generated code
 
 
@@ -2178,15 +2005,14 @@
             If no paths are given at the command line this value is used.
 
             Examples:
             ```toml
             paths = ["tests"]
             ```
 
-            ---
             Corresponds to the `paths` argument of __robot__.
             """
     )
     env: Optional[Dict[str, str]] = field(
         description="""\
             Define environment variables to be set before running tests.
```

### Comparing `robotcode_robot-0.32.2/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.32.3/src/robotcode/robot/config/utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.32.2/.gitignore` & `robotcode_robot-0.32.3/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.32.2/LICENSE.txt` & `robotcode_robot-0.32.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.32.2/README.md` & `robotcode_robot-0.32.3/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.32.2/pyproject.toml` & `robotcode_robot-0.32.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.32.2/PKG-INFO` & `robotcode_robot-0.32.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-robot
-Version: 0.32.2
+Version: 0.32.3
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
```

