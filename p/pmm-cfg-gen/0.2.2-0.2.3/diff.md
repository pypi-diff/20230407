# Comparing `tmp/pmm_cfg_gen-0.2.2.tar.gz` & `tmp/pmm_cfg_gen-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmm_cfg_gen-0.2.2.tar", max compression
+gzip compressed data, was "pmm_cfg_gen-0.2.3.tar", max compression
```

## Comparing `pmm_cfg_gen-0.2.2.tar` & `pmm_cfg_gen-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0    35149 2023-04-01 09:59:32.119583 pmm_cfg_gen-0.2.2/LICENSE
--rw-r--r--   0        0        0     1167 2023-04-04 21:44:17.290489 pmm_cfg_gen-0.2.2/README.md
--rw-r--r--   0        0        0     1179 2023-04-06 15:20:00.388829 pmm_cfg_gen-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       29 2023-04-04 21:44:17.290489 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/.gitignore
--rw-r--r--   0        0        0      726 2023-04-05 16:55:25.750443 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/__init__.py
--rw-r--r--   0        0        0      964 2023-04-05 14:36:56.540712 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/config_default.yaml
--rw-r--r--   0        0        0     1375 2023-04-05 12:16:46.728346 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/logging.yaml
--rw-r--r--   0        0        0       40 2023-04-04 21:44:17.294489 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/library.json.j2
--rw-r--r--   0        0        0       37 2023-04-04 21:44:17.294489 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/movies.collection.json.j2
--rw-r--r--   0        0        0      622 2023-04-04 23:11:00.595590 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/movies.collection.yml.j2
--rw-r--r--   0        0        0      124 2023-04-04 21:44:17.294489 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/movies.metadata.json.j2
--rw-r--r--   0        0        0      724 2023-04-04 21:44:17.294489 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/movies.metadata.yml.j2
--rw-r--r--   0        0        0     1392 2023-04-06 13:30:45.584955 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/thePosterDatabase.html.j2
--rw-r--r--   0        0        0       44 2023-04-06 13:30:45.584955 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/thePosterDatabase.json.j2
--rw-r--r--   0        0        0       37 2023-04-04 21:44:17.294489 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/tvshows.collection.json.j2
--rw-r--r--   0        0        0      577 2023-04-04 23:10:39.119521 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/tvshows.collection.yml.j2
--rw-r--r--   0        0        0      124 2023-04-04 21:44:17.294489 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/tvshows.metadata.json.j2
--rw-r--r--   0        0        0      777 2023-04-03 22:53:32.103146 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/tvshows.metadata.yml.j2
--rw-r--r--   0        0        0        0 2023-04-03 13:48:27.869541 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/__init__.py
--rw-r--r--   0        0        0     1223 2023-04-04 21:44:17.294489 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/cli_args.py
--rw-r--r--   0        0        0     1194 2023-04-05 11:47:03.681025 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/fileutils.py
--rw-r--r--   0        0        0     1578 2023-04-05 23:36:11.177668 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/logging.py
--rw-r--r--   0        0        0    15312 2023-04-06 15:19:24.396656 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/plex.py
--rw-r--r--   0        0        0     2256 2023-04-06 13:30:10.400820 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/plex_stats.py
--rw-r--r--   0        0        0     1950 2023-04-05 11:47:03.677025 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/plex_utils.py
--rw-r--r--   0        0        0     2735 2023-04-06 13:30:45.588955 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/pmm_cfg_manager.py
--rw-r--r--   0        0        0    11214 2023-04-05 23:36:11.177668 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/settings_yml.py
--rw-r--r--   0        0        0     4666 2023-04-06 13:30:45.588955 pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/template_manager.py
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 pmm_cfg_gen-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-01 09:59:32.119583 pmm_cfg_gen-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1167 2023-04-04 21:44:17.290489 pmm_cfg_gen-0.2.3/README.md
+-rw-r--r--   0        0        0     1182 2023-04-07 18:07:58.094977 pmm_cfg_gen-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-04-04 21:44:17.290489 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/.gitignore
+-rw-r--r--   0        0        0     1183 2023-04-06 17:50:16.037839 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/__init__.py
+-rw-r--r--   0        0        0      956 2023-04-06 15:40:40.048972 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/config_default.yaml
+-rw-r--r--   0        0        0     1375 2023-04-05 12:16:46.728346 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/logging.yaml
+-rw-r--r--   0        0        0       27 2023-04-07 02:15:04.147528 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/library.json.j2
+-rw-r--r--   0        0        0       24 2023-04-07 01:57:28.613322 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/movies.collection.json.j2
+-rw-r--r--   0        0        0      662 2023-04-07 02:15:57.419845 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/movies.collection.yml.j2
+-rw-r--r--   0        0        0      111 2023-04-07 01:57:33.917353 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/movies.metadata.json.j2
+-rw-r--r--   0        0        0      724 2023-04-04 21:44:17.294489 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/movies.metadata.yml.j2
+-rw-r--r--   0        0        0     1392 2023-04-06 13:30:45.584955 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/thePosterDatabase.html.j2
+-rw-r--r--   0        0        0      142 2023-04-06 18:10:09.861502 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/thePosterDatabase.json.j2
+-rw-r--r--   0        0        0       24 2023-04-07 01:57:43.117406 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/tvshows.collection.json.j2
+-rw-r--r--   0        0        0      617 2023-04-07 02:16:07.491905 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/tvshows.collection.yml.j2
+-rw-r--r--   0        0        0      111 2023-04-07 01:57:47.097429 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/tvshows.metadata.json.j2
+-rw-r--r--   0        0        0      777 2023-04-03 22:53:32.103146 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/tvshows.metadata.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-03 13:48:27.869541 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/__init__.py
+-rw-r--r--   0        0        0     1408 2023-04-06 17:50:16.029839 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/cli_args.py
+-rw-r--r--   0        0        0     1194 2023-04-05 11:47:03.681025 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/fileutils.py
+-rw-r--r--   0        0        0     1578 2023-04-05 23:36:11.177668 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/logging.py
+-rw-r--r--   0        0        0    17405 2023-04-07 17:13:05.095676 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/plex.py
+-rw-r--r--   0        0        0     1992 2023-04-07 17:07:15.268609 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/plex_stats.py
+-rw-r--r--   0        0        0     2653 2023-04-07 12:49:38.861227 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/plex_utils.py
+-rw-r--r--   0        0        0     2735 2023-04-06 13:30:45.588955 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/pmm_cfg_manager.py
+-rw-r--r--   0        0        0    11455 2023-04-06 17:50:16.313841 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/settings_yml.py
+-rw-r--r--   0        0        0     5211 2023-04-07 02:13:17.834897 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/template_manager.py
+-rwxr-xr-x   0        0        0     4019 2023-04-07 19:44:51.546772 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/time_span.py
+-rw-r--r--   0        0        0     2663 2023-04-07 18:44:27.163668 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/timer.py
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 pmm_cfg_gen-0.2.3/PKG-INFO
```

### Comparing `pmm_cfg_gen-0.2.2/LICENSE` & `pmm_cfg_gen-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.2/README.md` & `pmm_cfg_gen-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.2/pyproject.toml` & `pmm_cfg_gen-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pmm-cfg-gen"
-version = "0.2.2"
+version = "0.2.3"
 description = "A script to help automatically generate Plex Meta Manager configuration files for your libraries"
 license = "GPL-3.0-or-later"
 authors = ["Shawn Anderson <sanderson@eye-catcher.com>"]
 readme = "README.md"
 homepage = "https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator"
 repository = "https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator"
 keywords = [ "pmm", "plex-meta-manager", "plex" ]
@@ -20,17 +20,17 @@
 jsonpickle = "*"
 plexapi = "*"
 jinja2 = "*"
 ruamel-yaml = "^0.17.21"
 expandvars = "^0.9.0"
 python-dotenv = "^1.0.0"
 confuse = "^2.0.1"
-click = "^8.1.3"
 importlib-resources = "^5.12.0"
 coloredlogs = "^15.0.1"
+readchar = "^4.0.5"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.1"
 scriv = {extras = ["toml"], version = "^1.2.1"}
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/config_default.yaml` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/config_default.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 plex:
   serverUrl: ${PLEX_SERVER:-https://plex.ravenwolf.org:32400}
   token: ${PLEX_TOKEN}
 thePosterDatabase:
-  dataFile: theposterdbsearch.json
   searchUrl: https://theposterdb.com/search/advanced/results
   dbAssetUrl: https://theposterdb.com/api/assets/
 templates:
   collections:
     movies:
       yamlFileName: movies.collection.yml.j2
       jsonFileName: movies.collection.json.j2
@@ -26,8 +25,9 @@
     jsonFileName: thePosterDatabase.json.j2
     htmlFileName: thePosterDatabase.html.j2
 output:
   path: "./data"
   pathFormat: "{{libraryTitle}}"
 generate:
   enableJson: False
-  enablePmm: True
+  enableYaml: True
+  enableThePosterDb: True
```

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/logging.yaml` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/logging.yaml`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/movies.collection.yml.j2` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/movies.collection.yml.j2`

 * *Files 14% similar despite different names*

```diff
@@ -17,10 +17,10 @@
     url_poster: <<poster>>
     sort_title: <<collection_name>>
 
 collections:
   "{{ item.title }}":
     template: {name: tmdbTemplate, collection: "", movie: "", poster: https://theposterdb.com/api/assets/ }
     # {{ item | generateTpDbUrl }}
-    # collection_mode: hide
+    {% if item.childCount != 1 %}# {% endif %}collection_mode: hide
     # trakt_list:
     #  -
```

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/movies.metadata.yml.j2` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/movies.metadata.yml.j2`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/thePosterDatabase.html.j2` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/thePosterDatabase.html.j2`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/tvshows.collection.yml.j2` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/tvshows.collection.yml.j2`

 * *Files 14% similar despite different names*

```diff
@@ -16,10 +16,10 @@
     url_poster: <<poster>>
 
 collections:
   "{{ item.title }}":
     template: { name: tvdbTemplate, list: "", show: "", poster: https://theposterdb.com/api/assets/ }
     summary: {{ item.title }}
     # {{ item | generateTpDbUrl }}
-    # collection_mode: hide
+    {% if item.childCount != 1 %}# {% endif %}collection_mode: hide
     # trakt_list:
     #  -
```

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/templates/tvshows.metadata.yml.j2` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/tvshows.metadata.yml.j2`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/cli_args.py` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/cli_args.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 globalArgParser.add_argument(
     "--generate.enableJson",
     action="store_true",
     default=False,
     help="Enabled generating json files for each item processed (default: %(default)s)",
 )
 globalArgParser.add_argument(
+    "--generate.enableThePosterDb",
+    action="store_true",
+    default=False,
+    help="Enabled generating thePosterDb files (default: %(default)s)",
+)
+
+globalArgParser.add_argument(
     "--logLevel",
     choices=["INFO", "WARN", "DEBUG", "CRITICAL"],
     default="INFO",
     help="Logging Level (default: %(default)s)",
 )
 
 ###################################################################################################
```

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/fileutils.py` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/logging.py` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/plex.py` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/plex.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,332 +1,248 @@
 #!/usr/bin/env python3
 ###################################################################################################
 
 import json
 import logging
 import os
-import time
 from pathlib import Path
 
 import jsonpickle
 import requests
 
-# the following two lines disable InsecureRequestWarning
 import urllib3
 import urllib3.exceptions
 from plexapi.library import LibrarySection
 from plexapi.server import PlexServer
 
-from pmm_cfg_gen.utils.fileutils import formatLibraryItemPath, writeFile
+from pmm_cfg_gen.utils.fileutils import formatLibraryItemPath
 from pmm_cfg_gen.utils.plex_stats import (
-    PlexStats,
-    PlexStatsLibraryTotals,
-    PlexStatsTimer,
-    PlexStatsTotals,
+    PlexStats
 )
-from pmm_cfg_gen.utils.plex_utils import _cleanTitle, isPMMItem
+from pmm_cfg_gen.utils.plex_utils import _cleanTitle, isPMMItem, _formatItemTitle
 from pmm_cfg_gen.utils.settings_yml import globalSettingsMgr
 from pmm_cfg_gen.utils.template_manager import TemplateManager, generateTpDbUrl
 
 ###################################################################################################
 
+# the following two lines disable InsecureRequestWarning
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 ###################################################################################################
 class PlexLibraryProcessor:
     _logger: logging.Logger
+    _itemProcessedCache: dict[str,list]
 
     __session: requests.Session
 
     __stats: PlexStats
 
     templateManager: TemplateManager
 
     plexServer: PlexServer
     plexLibrary: LibrarySection
     plexLibraryName: str
 
     pathLibrary: Path
 
-    thePostDbSearchCache: dict
 
     ###############################################################################################
     def __init__(self) -> None:
         self._logger = logging.getLogger("pmm_cfg_gen")
         self._displayHeader()
 
         self.__stats = PlexStats()
 
+        self._itemProcessedCache = dict()
+
         self.templateManager = TemplateManager(
             globalSettingsMgr.settings.templates.getTemplateRootPath()
         )
 
+    ###############################################################################################
+
     def process(self):
         self.__stats.timerProgram.start()
 
-        self.connectToServer()
+        self._connectToServer()
 
+        
         if globalSettingsMgr.settings.plex.libraries is None:
-            self._logger.warn(
-                "No plex libraries defined to process.  Please check your configuration"
+            self._logger.debug(
+                "Loading Library list from plex."
             )
-            return
+            globalSettingsMgr.settings.plex.libraries = sorted([str(x.title) for x in self.plexServer.library.sections() if x.type == "movie" or x.type == "show"])
 
-        self._logger.debug(
+        self._logger.info(
             "Libraries to process: {}".format(
                 ",".join(globalSettingsMgr.settings.plex.libraries)
             )
         )
         for libraryName in globalSettingsMgr.settings.plex.libraries:
             self._processLibrary(libraryName)
 
-        self.__stats.timerProgram.end()
+        self.__stats.timerProgram.stop()
         self.__stats.calcTotals()
 
         self._displayStats()
 
-    def connectToServer(self):
+    ###############################################################################################
+    def _connectToServer(self):
         self._logger.info(
             "Connection to plex server: {}".format(
                 globalSettingsMgr.settings.plex.serverUrl
             )
         )
 
         self.__session = requests.Session()
         self.__session.verify = False
         self.plexServer = PlexServer(
             globalSettingsMgr.settings.plex.serverUrl,
             globalSettingsMgr.settings.plex.token,
             session=self.__session,
         )
 
-    ###############################################################################################
     def _loadLibrary(self, libraryName: str) -> LibrarySection:
         self._logger.debug("Loading plex library: {}".format(libraryName))
 
         self.plexLibrary = self.plexServer.library.section(libraryName)
         self.plexLibraryName = libraryName
 
         self.pathLibrary = formatLibraryItemPath(
             globalSettingsMgr.settings.output, self.plexLibrary
         )
         self.pathLibrary.mkdir(parents=True, exist_ok=True)
 
         self._logger.debug("Library Path: '{}'".format(self.pathLibrary))
 
-        tplFiles = globalSettingsMgr.settings.templates.metadata.getByItemType(
-            "library"
-        )
-
-        fileNameJson = Path(self.pathLibrary, "{}.json".format(libraryName))
-
-        if (
-            tplFiles.jsonFileName is not None
-            and globalSettingsMgr.settings.generate.enableJson
-        ):
-            self.templateManager.renderAndSave(
-                tplFiles.jsonFileName, fileNameJson, {"library": self.plexLibrary}
+        if globalSettingsMgr.settings.generate.enableJson:
+            tplFiles = globalSettingsMgr.settings.templates.metadata.getByItemType(
+                "library"
             )
 
-        return self.plexLibrary
-
-    def _saveThePosterDbSeachCache(self, fileName: str | Path):
-        self._logger.info("Saving ThePosterDb Search Data")
-
-        tplFiles = globalSettingsMgr.settings.templates.thePosterDatabase
-        if tplFiles is None:
-            self._logger.warn("No PosterDatabase Templates specifed")
-            return
-
-        try:
-            for key in self.thePostDbSearchCache:
-                self.thePostDbSearchCache[key] = sorted(
-                    self.thePostDbSearchCache[key], key=lambda x: x["title"]
-                )
-
-                fileNameHtml = Path(
-                    self.pathLibrary,
-                    "{}.{}.html".format("thePosterDatabaseSearch", key),
-                )
-                fileNameJson = Path(
-                    self.pathLibrary,
-                    "{}.{}.json".format("thePosterDatabaseSearch", key),
-                )
-                fileNameYaml = Path(
-                    self.pathLibrary,
-                    "{}.{}.yaml".format("thePosterDatabaseSearch", key),
+            fileNameJson = Path(self.pathLibrary, "{}.json".format(libraryName))
+
+            if (
+                tplFiles.jsonFileName is not None
+                and globalSettingsMgr.settings.generate.enableJson
+            ):
+                self.templateManager.renderAndSave(
+                    tplFiles.jsonFileName, fileNameJson, {"library": self.plexLibrary}
                 )
 
-                if tplFiles.jsonFileName is not None and len(tplFiles.jsonFileName) > 0:
-                    self.templateManager.renderAndSave(
-                        tplFiles.jsonFileName,
-                        fileNameJson,
-                        tplArgs={"items": self.thePostDbSearchCache[key]},
-                    )
-
-                if tplFiles.htmlFileName is not None and len(tplFiles.htmlFileName) > 0:
-                    self.templateManager.renderAndSave(
-                        tplFiles.htmlFileName,
-                        fileNameHtml,
-                        tplArgs={"items": self.thePostDbSearchCache[key]},
-                    )
-
-                if tplFiles.yamlFileName is not None and len(tplFiles.yamlFileName) > 0:
-                    self.templateManager.renderAndSave(
-                        tplFiles.yamlFileName,
-                        fileNameYaml,
-                        tplArgs={"items": self.thePostDbSearchCache[key]},
-                    )
-        except:
-            self._logger.exception("Failed storing the posterdatabase cache")
-
-    def _addItemToThePosterDbSearchCache(self, item):
-        ids = [o.id for o in item.guids]
-
-        tpdbEntry = {
-            "title": item.title,
-            "searchUrl": generateTpDbUrl(item),
-            "ids": ids,
-        }
-
-        if self.plexLibrary.type not in self.thePostDbSearchCache.keys():
-            self.thePostDbSearchCache[self.plexLibrary.type] = []
-
-        it = next(
-            (
-                x
-                for x in self.thePostDbSearchCache[self.plexLibrary.type]
-                if x["title"] == item.title
-            ),
-            None,
-        )
-        if it is None:
-            self.thePostDbSearchCache[self.plexLibrary.type].append(tpdbEntry)
+        return self.plexLibrary
 
     def _processLibrary(self, libraryName: str):
         self._logger.info("-" * 50)
         self._logger.info("Started Processing Library: '{}'".format(libraryName))
 
         self.__stats.initLibrary(libraryName)
+        self._itemProcessedCache.update({ libraryName : list() })
 
         self.__stats.timerLibraries[libraryName].start()
 
-        self.thePostDbSearchCache = dict()
-
         self._loadLibrary(libraryName)
 
         self._logger.info("Processing Library Collections")
         collections = self.plexLibrary.collections()
 
         self.__stats.countsLibraries[libraryName].collections.total = len(collections)
+        self.__stats.countsLibraries[libraryName].collections.processed = 0
 
         for collection in collections:
-            self.__stats.countsLibraries[libraryName].collections.processed += 1
-            if not isPMMItem(collection) and collection.childCount > 0:
-                try:
-                    self._processCollection(collection.title, collection)
-                except:
-                    self._logger.exception(
-                        "Error Processing Collection: {}".format(collection.title)
-                    )
-            else:
-                self._logger.info(
-                    "  Skipping Dynamic Collecton: {}".format(collection.title)
+            try:
+                self._processCollection(collection.title, collection)
+            except:
+                self._logger.exception(
+                    "Error Processing Collection: {}".format(collection.title)
                 )
 
         self._logger.info("Processing Library Items")
         items = self.plexLibrary.all()
 
         self.__stats.countsLibraries[libraryName].items.total = len(items)
+        self.__stats.countsLibraries[libraryName].items.processed = 0
+        self.__stats.countsLibraries[libraryName].calcTotals()
 
         for item in items:
-            self.__stats.countsLibraries[libraryName].items.processed += 1
-
-            if len(item.collections) == 0:
-                self._logger.info(
-                    "Skipping '{}' Metdata for {} ({}). Member of a collection".format(
-                        item.type, item.title, item.year
-                    )
-                )
-            elif isPMMItem(item):
-                self._logger.info(
-                    "Skipping '{}' Metdata for {} ({}). Dynamic item".format(
-                        item.type, item.title, item.year
-                    )
+            try:
+                self._processMetadata(item.title, [item])
+            except:
+                self._logger.exception(
+                    "Error Processing Item: {}".format(item.title)
                 )
-            else:
-                try:
-                    self._processMetadata(item.title, [item])
-                except:
-                    self._logger.exception(
-                        "Error Processing Item: {}".format(item.title)
-                    )
 
-        self._saveThePosterDbSeachCache(
-            Path(
-                self.pathLibrary, globalSettingsMgr.settings.thePosterDatabase.dataFile
-            ).resolve()
-        )
+        self.__stats.timerLibraries[libraryName].stop()
 
-        self.__stats.timerLibraries[libraryName].end()
+        self.__stats.countsLibraries[libraryName].calcTotals()
+        self._saveThePosterDbSeachCache()
 
     def _processCollection(self, itemTitle: str, item):
-        title = _cleanTitle(itemTitle)
+        self.__stats.countsLibraries[self.plexLibraryName].collections.processed += 1
 
-        fileName = Path(self.pathLibrary, "collections", "{}.yml".format(title))
-        fileNameJson = Path(
-            self.pathLibrary, "collections/json", "{}.json".format(title)
-        )
+        title = _cleanTitle(itemTitle)
 
+        if isPMMItem(item) or item.childCount == 0:
+            self._logger.info(
+                "[{}/{}] Skipping Dynamic/Empty Collecton: {}".format(
+                    self.__stats.countsLibraries[self.plexLibraryName].collections.processed,
+                    self.__stats.countsLibraries[self.plexLibraryName].collections.total,
+                    item.title)
+            )
+            return 
+        
         self._logger.info(
             "[{}/{}] Processing Collection: {}".format(
-                self.__stats.countsLibraries[
-                    self.plexLibraryName
-                ].collections.processed,
+                self.__stats.countsLibraries[self.plexLibraryName].collections.processed,
                 self.__stats.countsLibraries[self.plexLibraryName].collections.total,
                 itemTitle,
             )
         )
 
         tplFiles = globalSettingsMgr.settings.templates.collections.getByItemType(
             self.plexLibrary.type
         )
         self._logger.debug(
             "tplFiles: {}".format(jsonpickle.dumps(tplFiles, unpicklable=False))
         )
 
-        self._logger.debug("tplFileNameYaml: {}".format(tplFiles.yamlFileName))
+        fileName = Path(self.pathLibrary, "collections", "{}.yml".format(title))
         if (
             not os.path.exists(fileName)
             and tplFiles.yamlFileName is not None
             and globalSettingsMgr.settings.generate.enableYaml
         ):
-            self._logger.info("  Generating Collection file")
+            self._logger.debug("  Generating Collection file")
+            
             self.templateManager.renderAndSave(
                 tplFiles.yamlFileName, fileName, tplArgs={"item": item}
             )
             # elif os.path.exists(fileName):
             # Do we want to try to merge here?
             # pmmCfgMgr = PlexMetaManager(self.pathLibrary)
 
             # pmmCfgMgr.mergeCollection(itemTitle, item)
             pass
+        elif not globalSettingsMgr.settings.generate.enableYaml:
+            self._logger.debug("  Skipping Generating Collection yaml file")
         else:
             self._logger.warn("  Collection File Exists")
 
-        self._logger.debug("tplFileNameJson: {}".format(tplFiles.jsonFileName))
+        fileNameJson = Path(self.pathLibrary, "collections/json", "{}.json".format(title))
         if (
             tplFiles.jsonFileName is not None
             and globalSettingsMgr.settings.generate.enableJson
         ):
-            self._logger.info("  Generating json file")
+            self._logger.debug("  Generating json file")
             self.templateManager.renderAndSave(
                 tplFiles.jsonFileName, fileNameJson, tplArgs={"item": item}
             )
+        elif not globalSettingsMgr.settings.generate.enableJson:
+            self._logger.debug("  Skipping Geerating json file")
 
         childItems = item.items()
         if len(childItems) > 0:
             self.__stats.countsLibraries[self.plexLibraryName].items.total = len(
                 childItems
             )
             self.__stats.countsLibraries[self.plexLibraryName].items.processed = 0
@@ -338,75 +254,177 @@
 
         fileName = Path(self.pathLibrary, "metadata", "{}.yml".format(title))
         fileNameJson = Path(self.pathLibrary, "metadata/json", "{}.json".format(title))
 
         tplFiles = globalSettingsMgr.settings.templates.metadata.getByItemType(
             self.plexLibrary.type
         )
-
+        
         itemsWithExtras = []
         for item in items:
             self.__stats.countsLibraries[self.plexLibraryName].items.processed += 1
-            self._logger.info(
-                "[{}/{}] Processing {}: {} ({})".format(
-                    self.__stats.countsLibraries[self.plexLibraryName].items.processed,
-                    self.__stats.countsLibraries[self.plexLibraryName].items.total,
-                    item.type,
-                    item.title,
-                    item.year,
+
+            if isPMMItem(item):
+                self._logger.info(
+                    "[{}/{}] Skipping '{}': {}. Dynamic item".format(
+                        self.__stats.countsLibraries[self.plexLibraryName].items.processed,
+                        self.__stats.countsLibraries[self.plexLibraryName].items.total,
+                        item.type, _formatItemTitle(item)
+                    )
+                )
+            elif self._isItemProcessed(item):                                 
+                self._logger.info(
+                    "[{}/{}] Skipping {}: {}. Already Processed".format(
+                        self.__stats.countsLibraries[self.plexLibraryName].items.processed,
+                        self.__stats.countsLibraries[self.plexLibraryName].items.total,
+                        item.type,
+                        _formatItemTitle(item)
+                    )
+                )
+            else:
+                self._logger.info(
+                    "[{}/{}] Processing {}: {}".format(
+                        self.__stats.countsLibraries[self.plexLibraryName].items.processed,
+                        self.__stats.countsLibraries[self.plexLibraryName].items.total,
+                        item.type,
+                        _formatItemTitle(item)
+                    )
                 )
-            )
 
-            self._addItemToThePosterDbSearchCache(item)
+                self._adItemToProcessedCache(item)
 
-            seasons = []
-            if "childCount" in item.__dict__:
-                self._logger.info("  Loading Seasons...")
-                seasons = item.seasons()
+                seasons = []
+                if "childCount" in item.__dict__:
+                    self._logger.debug("  Loading Seasons...")
+                    seasons = item.seasons()
 
-            itemsWithExtras.append({"metadata": item, "seasons": seasons})
+                itemsWithExtras.append({"metadata": item, "seasons": seasons})
 
         if (
             not os.path.exists(fileName)
             and tplFiles.yamlFileName is not None
             and globalSettingsMgr.settings.generate.enableYaml
         ):
-            self._logger.info("  Generating Metdata file")
+            self._logger.debug("  Generating Metdata file")
             self.templateManager.renderAndSave(
                 tplFiles.yamlFileName, fileName, tplArgs={"items": itemsWithExtras}
             )
         # elif os.path.exists(fileName):
         #     # Do we want to try to merge here?
         #     pass
         else:
-            self._logger.warn("  Metadata File Exists")
+            self._logger.debug("  Metadata File Exists")
 
         if (
             tplFiles.jsonFileName is not None
             and globalSettingsMgr.settings.generate.enableJson
         ):
-            self._logger.info("  Generating json file")
+            self._logger.debug("  Generating json file")
             self.templateManager.renderAndSave(
                 tplFiles.jsonFileName, fileNameJson, tplArgs={"items": itemsWithExtras}
             )
 
+    def _isItemProcessed(self, item) -> bool:
+        it = next(
+            (
+                x
+                for x in self._itemProcessedCache[self.plexLibraryName]
+                if x["title"] ==  _formatItemTitle(item)
+            ),
+            None,
+        )
+
+        return it is not None 
+            
+    def _adItemToProcessedCache(self, item):
+        ids = [o.id for o in item.guids]
+
+        if self.plexLibraryName not in self._itemProcessedCache.keys():
+            self._itemProcessedCache[self.plexLibraryName] = []
+
+        if not self._isItemProcessed(item):
+            tpdbEntry = {
+                "title":  _formatItemTitle(item),
+                "searchUrl": generateTpDbUrl(item),
+                "ids": ids,
+            }
+
+            self._itemProcessedCache[self.plexLibraryName].append(tpdbEntry)
+
+    def _saveThePosterDbSeachCache(self):
+        if not globalSettingsMgr.settings.generate.enaleThePosterDb:
+            self._logger.debug("Skipping Saving ThPosterDb Search Data...")
+            return
+
+        self._logger.info("Saving ThePosterDb Search Data")
+
+        tplFiles = globalSettingsMgr.settings.templates.thePosterDatabase
+        if tplFiles is None:
+            self._logger.warn("No PosterDatabase Templates specifed")
+            return
+
+        try:
+            self._itemProcessedCache[self.plexLibraryName] = sorted(
+                self._itemProcessedCache[self.plexLibraryName], key=lambda x: x["title"]
+            )
+
+            fileNameJson = Path(self.pathLibrary, "{}.json".format(globalSettingsMgr.settings.thePosterDatabase.baseFileName) )
+            if tplFiles.jsonFileName is not None and len(tplFiles.jsonFileName) > 0:
+                self.templateManager.renderAndSave(
+                    tplFiles.jsonFileName,
+                    fileNameJson,
+                    tplArgs={
+                        "items": self._itemProcessedCache[self.plexLibraryName],
+                        "stats": json.loads(str(jsonpickle.dumps(self.__stats.countsLibraries[self.plexLibraryName], unpicklable=False))),
+                        "processingTime": self.__stats.timerLibraries[self.plexLibraryName].to_dict()
+                    }
+                )
+
+            fileNameHtml = Path(self.pathLibrary, "{}.html".format(globalSettingsMgr.settings.thePosterDatabase.baseFileName) )
+            if tplFiles.htmlFileName is not None and len(tplFiles.htmlFileName) > 0:
+                self.templateManager.renderAndSave(
+                    tplFiles.htmlFileName,
+                    fileNameHtml,
+                    tplArgs={
+                        "items": self._itemProcessedCache[self.plexLibraryName],
+                        "stats": json.loads(str(jsonpickle.dumps(self.__stats.countsLibraries[self.plexLibraryName], unpicklable=False))),
+                        "processingTime": self.__stats.timerLibraries[self.plexLibraryName].to_dict()
+                    }
+                )
+
+            fileNameYaml = Path(self.pathLibrary, "{}.yaml".format(globalSettingsMgr.settings.thePosterDatabase.baseFileName) )
+            if tplFiles.yamlFileName is not None and len(tplFiles.yamlFileName) > 0:
+                self.templateManager.renderAndSave(
+                    tplFiles.yamlFileName,
+                    fileNameYaml,
+                    tplArgs={
+                        "items": self._itemProcessedCache[self.plexLibraryName],
+                        "stats": json.loads(str(jsonpickle.dumps(self.__stats.countsLibraries[self.plexLibraryName], unpicklable=False))),
+                        "processingTime": self.__stats.timerLibraries[self.plexLibraryName].to_dict()
+                    }
+                )
+        except:
+            self._logger.exception("Failed storing the posterdatabase cache")
+
     def _displayHeader(self):
         self._logger.info("-" * 50)
         self._logger.info("Please Meta Manager Configuration File Generator")
         self._logger.info("-" * 50)
 
     def _displayStats(self):
         # self._logger.debug(json.dumps(self.__timers, indent=4, unpicklable=False))
 
         self._logger.info("-" * 50)
 
         self._logger.info("Overall Statistics")
 
         self._logger.info(
-            "  Processing Time: {:.2f} seconds".format(self.__stats.timerProgram.delta)
+            "  Total Processing Time: {}".format(
+                    self.__stats.timerProgram.elapsed_time_ts.to_str() 
+                )            
         )
         self._logger.info(
             "  Collections Processed: {}".format(
                 self.__stats.countsProgram.collections.total
             )
         )
         self._logger.info(
@@ -416,16 +434,17 @@
         for libraryName in self.__stats.timerLibraries.keys():
             libraryTimer = self.__stats.timerLibraries[libraryName]
             libaryCounts = self.__stats.countsLibraries[libraryName]
 
             self._logger.info("Statistics for Library: '{}'".format(libraryName))
 
             self._logger.info(
-                "  Processing Time: '{}'. Total Time: {:.2f} seconds".format(
-                    libraryName, libraryTimer.delta
+                "  Processing Time: '{}'. Total Time: {}".format(
+                    libraryName, 
+                    libraryTimer.elapsed_time_ts.to_str()
                 )
             )
 
             self._logger.info(
                 "  Collections: {}".format(libaryCounts.collections.total)
             )
```

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/plex_stats.py` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/plex_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,28 @@
 #!/usr/bin/env python3
 ###################################################################################################
 
-import time
+# from datetime import timedelta
+# import time
+from pmm_cfg_gen.utils.timer import timer
 
 ###################################################################################################
 
-
-class PlexStatsTimer:
-    __timerStart: float
-    __timerEnd: float
-
-    def start(self):
-        self.__timerStart = time.perf_counter()
-
-    def end(self):
-        self.__timerEnd = time.perf_counter()
-
-    @property
-    def delta(self) -> float:
-        return self.__timerEnd - self.__timerStart
-
-
 class PlexStatsTotals:
     total: int
     processed: int
 
     def __init__(self) -> None:
         self.total = 0
         self.processed = 0
 
     def _addStats(self, stats):
         self.total += stats.total
         self.processed += stats.processed
 
-
 class PlexStatsLibraryTotals:
     totals: PlexStatsTotals
 
     collections: PlexStatsTotals
     items: PlexStatsTotals
 
     def __init__(self) -> None:
@@ -45,31 +30,30 @@
         self.collections = PlexStatsTotals()
         self.items = PlexStatsTotals()
 
     def calcTotals(self):
         self.totals.total = self.collections.total + self.items.total
         self.totals.processed = self.collections.processed + self.items.processed
 
-
 class PlexStats:
-    timerProgram: PlexStatsTimer
-    timerLibraries: dict[str, PlexStatsTimer]
+    timerProgram: timer
+    timerLibraries: dict[str, timer]
 
     countsProgram: PlexStatsLibraryTotals
     countsLibraries: dict[str, PlexStatsLibraryTotals]
 
     def __init__(self) -> None:
-        self.timerProgram = PlexStatsTimer()
+        self.timerProgram = timer()
         self.timerLibraries = {}
 
         self.countsProgram = PlexStatsLibraryTotals()
         self.countsLibraries = {}
 
     def initLibrary(self, libraryName: str):
-        self.timerLibraries[libraryName] = PlexStatsTimer()
+        self.timerLibraries[libraryName] = timer()
         self.countsLibraries[libraryName] = PlexStatsLibraryTotals()
 
     def calcTotals(self):
         # for libraryName in self.timerLibraries.keys():
         #     pass
 
         for libraryName in self.countsLibraries.keys():
```

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/pmm_cfg_manager.py` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/pmm_cfg_manager.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/settings_yml.py` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/settings_yml.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,33 +103,41 @@
                 importlib_resources.files("pmm_cfg_gen").joinpath("templates")
             )
 
         return Path(self.templatePath).resolve()
 
 
 class SettingsThePosterDatabase:
-    dataFile: str
+    baseFileName: str
     searchUrl: str
     dbAssetUrl: str
 
-    def __init__(self, searchUrl: str, dbAssetUrl: str, dataFile: str) -> None:
+    def __init__(self, searchUrl: str, dbAssetUrl: str, baseFileName: str) -> None:
         self.searchUrl = searchUrl
         self.dbAssetUrl = dbAssetUrl
-        self.dataFile = dataFile
+        self.baseFileName = baseFileName
 
 
 class SettingsGenerate:
     enableJson: bool
     enableYaml: bool
     enableHtml: bool
+    enaleThePosterDb: bool
 
-    def __init__(self, enableJson: bool, enableYaml: bool, enableHtml: bool) -> None:
+    def __init__(
+        self,
+        enableJson: bool,
+        enableYaml: bool,
+        enableHtml: bool,
+        enableThePosterDb: bool,
+    ) -> None:
         self.enableJson = enableJson
         self.enableYaml = enableYaml
         self.enableHtml = enableHtml
+        self.enaleThePosterDb = enableThePosterDb
 
 
 class Settings:
     plex: SettingsPlex
     thePosterDatabase: SettingsThePosterDatabase
     templates: SettingsTemplates
     output: SettingsOutput
@@ -183,15 +191,14 @@
 
         if cmdLineArgs is not None:
             self._logger.debug("Loading Configuration from Command Line")
             self._config.set_args(cmdLineArgs, dots=True)
 
         self._config.set_redaction("plex.token", True)
 
-        self._logger.debug(self._config.dump())
         self._logger.debug(
             "Configuration Directory: {}".format(self._config.config_dir())
         )
         self._logger.debug(
             "User Configuration Path: {}".format(self._config.user_config_path())
         )
 
@@ -204,20 +211,19 @@
             thePosterDatabase=SettingsThePosterDatabase(
                 searchUrl=expandvars(
                     self._config["thePosterDatabase"]["searchUrl"].as_str()
                 ),
                 dbAssetUrl=expandvars(
                     self._config["thePosterDatabase"]["dbAssetUrl"].as_str()
                 ),
-                dataFile=str(self._config["thePosterDatabase"]["dataFile"].as_str()),
-                # templates=SettingsTemplateFiles(
-                #     yamlFileName=,
-                #     jsonFileName=,
-                #     htmlFileName=
-                # )
+                baseFileName=str(
+                    self._config["thePosterDatabase"]["baseFileName"].get(
+                        confuse.Optional("thePosterDatabase")
+                    )
+                ),
             ),
             templates=SettingsTemplates(
                 collections=SettingsTemplateFileGroup(
                     movies=SettingsTemplateFiles(
                         yamlFileName=str(
                             self._config["templates"]["collections"]["movies"][
                                 "yamlFileName"
@@ -302,16 +308,18 @@
                 path=str(self._config["output"]["path"].as_str()),
                 pathFormat=str(self._config["output"]["pathFormat"].as_str()),
             ),
             generate=SettingsGenerate(
                 enableHtml=self._config["generate"]["enableHtml"].get(confuse.Optional(False)),  # type: ignore
                 enableJson=self._config["generate"]["enableJson"].get(confuse.Optional(False)),  # type: ignore
                 enableYaml=self._config["generate"]["enableYaml"].get(confuse.Optional(True)),  # type: ignore
+                enableThePosterDb=self._config["generate"]["enableThePosterDb"].get(confuse.Optional(True)),  # type: ignore
             ),
         )
 
-        # self._logger.debug(jsonpickle.dumps(self.settings, indent=4))
+        self._logger.debug("Active Settings:")
+        self._logger.debug(jsonpickle.dumps(self.settings, unpicklable=False))
 
 
 #######################################################################
 
 globalSettingsMgr = SettingsManager()
```

### Comparing `pmm_cfg_gen-0.2.2/src/pmm_cfg_gen/utils/template_manager.py` & `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/template_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,49 +21,56 @@
 def itemToJson(item):
     str = jsonpickle.encode(item, unpicklable=False)
 
     return str
 
 
 def formatJson(data):
-    return jsonpickle.dumps(data, indent=4)
+    return jsonpickle.dumps(data, indent=4, unpicklable=False)
 
 
 def generateTpDbUrl(item, baseUrl=None) -> str:
     if baseUrl is None:
         baseUrl = globalSettingsMgr.settings.thePosterDatabase.searchUrl
 
     urlParms = {}
 
-    if item.type == "movie":
+    if item.type == "collection":
+        if item.metadataType == "movie":
+            urlParms.update({"category": "Movies"})
+            urlParms.update({"term": "{}{}".format(item.title, " collection" if "collection" not in item.title else "")})
+        elif item.metadataType == "show":
+            urlParms.update({"category": "Shows"})
+            urlParms.update({"term": "{}{}".format(item.title, " collection" if "collection" not in item.title else "")})
+    elif item.type == "movie":
         urlParms.update({"category": "Movies"})
         urlParms.update({"term": item.title})
         urlParms.update({"year_filter": "equals"})
         urlParms.update({"yone": item.year})
-
-    if item.type == "show":
+    elif item.type == "show":
         urlParms.update({"category": "Shows"})
         urlParms.update({"term": item.title})
         urlParms.update({"year_filter": "equals"})
         urlParms.update({"yone": item.year})
-
-    if item.type == "season":
+    elif item.type == "season":
         urlParms.update({"category": "Shows"})
         urlParms.update({"term": "{} {}".format(item.title, item.parentTitle)})
 
     if "guids" in item.__dict__:
         ids = dict(o.id.split("://") for o in item.guids)
 
         if "tmdb" in ids.keys():
             urlParms.update({"tmdb_id": ids["tmdb"]})
         if "imdb" in ids.keys():
             urlParms.update({"imdb_id": ids["imdb"]})
         if "tvdb" in ids.keys():
             urlParms.update({"tvdb_id": ids["tvdb"]})
 
+    #logging.getLogger("pmm-cfg-gen").info(urlParms)
+    
     urlQS = urllib.parse.urlencode(urlParms)
 
     req = requests.PreparedRequest()
     req.prepare_url(baseUrl, urlQS)
 
     return str(req.url)
```

### Comparing `pmm_cfg_gen-0.2.2/PKG-INFO` & `pmm_cfg_gen-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pmm-cfg-gen
-Version: 0.2.2
+Version: 0.2.3
 Summary: A script to help automatically generate Plex Meta Manager configuration files for your libraries
 Home-page: https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator
 License: GPL-3.0-or-later
 Keywords: pmm,plex-meta-manager,plex
 Author: Shawn Anderson
 Author-email: sanderson@eye-catcher.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: confuse (>=2.0.1,<3.0.0)
 Requires-Dist: expandvars (>=0.9.0,<0.10.0)
 Requires-Dist: importlib-resources (>=5.12.0,<6.0.0)
 Requires-Dist: jinja2
 Requires-Dist: jsonpickle
 Requires-Dist: plexapi
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: readchar (>=4.0.5,<5.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Project-URL: Repository, https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator
 Description-Content-Type: text/markdown
 
 # Plex-Meta-Mnager-Config-Generator
 A python script to automatically generate Plex Meta Manager configuration files based on your plex libraries.
```

