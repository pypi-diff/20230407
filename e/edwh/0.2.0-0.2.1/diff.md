# Comparing `tmp/edwh-0.2.0.tar.gz` & `tmp/edwh-0.2.1.tar.gz`

## Comparing `edwh-0.2.0.tar` & `edwh-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 edwh-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 edwh-0.2.0/.idea/edwh.iml
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 edwh-0.2.0/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.2.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 edwh-0.2.0/.idea/vcs.xml
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 edwh-0.2.0/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.2.0/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.2.0/src/edwh/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 edwh-0.2.0/src/edwh/cli.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 edwh-0.2.0/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 edwh-0.2.0/README.md
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 edwh-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 edwh-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 edwh-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 edwh-0.2.1/.idea/edwh.iml
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 edwh-0.2.1/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.2.1/.idea/modules.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh-0.2.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 edwh-0.2.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.2.1/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.2.1/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 edwh-0.2.1/src/edwh/cli.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 edwh-0.2.1/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 edwh-0.2.1/README.md
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 edwh-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 edwh-0.2.1/PKG-INFO
```

### Comparing `edwh-0.2.0/.idea/workspace.xml` & `edwh-0.2.1/.idea/workspace.xml`

 * *Files 10% similar despite different names*

#### Comparing `edwh-0.2.0/.idea/workspace.xml` & `edwh-0.2.1/.idea/workspace.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="c3c9037f-3cb1-45bc-b93c-f432a2ce3ac3" name="Changes" comment="fix: removed CHANGELOG.txt and reduced semantic-versioning responsibilities">
-      <change beforePath="$PROJECT_DIR$/src/edwh/tasks.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/edwh/tasks.py" afterDir="false"/>
+    <list default="true" id="c3c9037f-3cb1-45bc-b93c-f432a2ce3ac3" name="Changes" comment="">
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -17,35 +17,36 @@
   </component>
   <component name="ProjectId" id="2O74kfRWAJGgKwua6ELxsHqOzz2"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showExcludedFiles" value="false"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "WebServerToolWindowFactoryState": "false",
-    "git-widget-placeholder": "main",
-    "node.js.detected.package.eslint": "true",
-    "node.js.selected.package.eslint": "(autodetect)",
-    "nodejs_package_manager_path": "npm",
-    "settings.editor.selected.configurable": "preferences.lookFeel",
-    "vue.rearranger.settings.migration": "true"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;WebServerToolWindowFactoryState&quot;: &quot;false&quot;,
+    &quot;git-widget-placeholder&quot;: &quot;main&quot;,
+    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
+    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
+    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;preferences.pluginManager&quot;,
+    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
   }
-}]]></component>
+}</component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="c3c9037f-3cb1-45bc-b93c-f432a2ce3ac3" name="Changes" comment=""/>
       <created>1680898430790</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1680898430790</updated>
-      <workItem from="1680898432130" duration="1860000"/>
+      <workItem from="1680898432130" duration="2391000"/>
+      <workItem from="1680900842047" duration="26000"/>
     </task>
     <task id="LOCAL-00001" summary="feat: changelog management using semantic-versioning added">
       <created>1680898686723</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1680898686723</updated>
@@ -53,19 +54,27 @@
     <task id="LOCAL-00002" summary="fix: removed CHANGELOG.txt and reduced semantic-versioning responsibilities">
       <created>1680900056423</created>
       <option name="number" value="00002"/>
       <option name="presentableId" value="LOCAL-00002"/>
       <option name="project" value="LOCAL"/>
       <updated>1680900056423</updated>
     </task>
-    <option name="localTasksCounter" value="3"/>
+    <task id="LOCAL-00003" summary="feat: removed old redundant demo methods and added `zen`">
+      <created>1680900327108</created>
+      <option name="number" value="00003"/>
+      <option name="presentableId" value="LOCAL-00003"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1680900327108</updated>
+    </task>
+    <option name="localTasksCounter" value="4"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="feat: changelog management using semantic-versioning added"/>
     <MESSAGE value="fix: removed CHANGELOG.txt and reduced semantic-versioning responsibilities"/>
-    <option name="LAST_COMMIT_MESSAGE" value="fix: removed CHANGELOG.txt and reduced semantic-versioning responsibilities"/>
+    <MESSAGE value="feat: removed old redundant demo methods and added `zen`"/>
+    <option name="LAST_COMMIT_MESSAGE" value="feat: removed old redundant demo methods and added `zen`"/>
   </component>
 </project>
```

### Comparing `edwh-0.2.0/src/edwh/cli.py` & `edwh-0.2.1/src/edwh/cli.py`

 * *Files identical despite different names*

### Comparing `edwh-0.2.0/LICENSE.txt` & `edwh-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.2.0/pyproject.toml` & `edwh-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -63,18 +63,24 @@
 [tool.hatch.version]
 path = "src/edwh/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  'python-semantic-release'
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
+publish = [
+  'semantic-release publish',
+  'hatch build -c',
+  'hatch publish',
+]
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
```

### Comparing `edwh-0.2.0/PKG-INFO` & `edwh-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.2.0
+Version: 0.2.1
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

