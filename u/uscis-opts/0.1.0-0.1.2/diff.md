# Comparing `tmp/uscis-opts-0.1.0.tar.gz` & `tmp/uscis-opts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uscis-opts-0.1.0.tar", last modified: Mon Mar 27 19:25:04 2023, max compression
+gzip compressed data, was "uscis-opts-0.1.2.tar", last modified: Fri Apr  7 19:29:23 2023, max compression
```

## Comparing `uscis-opts-0.1.0.tar` & `uscis-opts-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 19:25:04.631582 uscis-opts-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-01-12 21:23:52.000000 uscis-opts-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       32 2023-01-13 16:58:41.000000 uscis-opts-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-03-27 19:25:04.630583 uscis-opts-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-01-05 18:01:03.000000 uscis-opts-0.1.0/README.md
--rw-rw-rw-   0        0        0      795 2023-03-27 19:24:11.000000 uscis-opts-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-27 19:25:04.632583 uscis-opts-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-27 19:25:04.509254 uscis-opts-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-27 19:25:04.554276 uscis-opts-0.1.0/src/opts/
--rw-rw-rw-   0        0        0     3069 2023-03-27 18:59:31.000000 uscis-opts-0.1.0/src/opts/ArcherAuth.py
--rw-rw-rw-   0        0        0    10517 2023-03-27 18:59:09.000000 uscis-opts-0.1.0/src/opts/ArcherServerClient.py
--rw-rw-rw-   0        0        0      311 2023-01-24 15:59:21.000000 uscis-opts-0.1.0/src/opts/ContextError.py
--rw-rw-rw-   0        0        0      381 2023-01-05 18:01:03.000000 uscis-opts-0.1.0/src/opts/SigningError.py
--rw-rw-rw-   0        0        0        0 2023-01-06 17:11:22.000000 uscis-opts-0.1.0/src/opts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 19:25:04.578462 uscis-opts-0.1.0/src/opts/templates/
--rw-rw-rw-   0        0        0      488 2023-02-03 15:15:04.000000 uscis-opts-0.1.0/src/opts/templates/ExecuteSearch.xml
--rw-rw-rw-   0        0        0      409 2023-02-02 14:28:02.000000 uscis-opts-0.1.0/src/opts/templates/GetReports.xml
--rw-rw-rw-   0        0        0      478 2023-02-02 17:54:44.000000 uscis-opts-0.1.0/src/opts/templates/GetSearchOptionsByGuid.xml
--rw-rw-rw-   0        0        0        0 2023-01-06 17:11:22.000000 uscis-opts-0.1.0/src/opts/templates/__init__.py
--rw-rw-rw-   0        0        0      287 2023-01-05 18:01:03.000000 uscis-opts-0.1.0/src/opts/templates/template.xml
-drwxrwxrwx   0        0        0        0 2023-03-27 19:25:04.624909 uscis-opts-0.1.0/src/uscis_opts.egg-info/
--rw-rw-rw-   0        0        0      579 2023-03-27 19:25:04.000000 uscis-opts-0.1.0/src/uscis_opts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2023-03-27 19:25:04.000000 uscis-opts-0.1.0/src/uscis_opts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 19:25:04.000000 uscis-opts-0.1.0/src/uscis_opts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-03-27 19:25:04.000000 uscis-opts-0.1.0/src/uscis_opts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-27 19:25:04.000000 uscis-opts-0.1.0/src/uscis_opts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-07 19:29:23.709810 uscis-opts-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2023-01-12 21:23:52.000000 uscis-opts-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-01-13 16:58:41.000000 uscis-opts-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2737 2023-04-07 19:29:23.708809 uscis-opts-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2170 2023-04-07 18:05:55.000000 uscis-opts-0.1.2/README.md
+-rw-rw-rw-   0        0        0      795 2023-04-07 19:19:08.000000 uscis-opts-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-07 19:29:23.710810 uscis-opts-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-07 19:29:23.600813 uscis-opts-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-07 19:29:23.639810 uscis-opts-0.1.2/src/opts/
+-rw-rw-rw-   0        0        0     3069 2023-04-07 19:28:34.000000 uscis-opts-0.1.2/src/opts/ArcherAuth.py
+-rw-rw-rw-   0        0        0    11205 2023-04-07 19:18:20.000000 uscis-opts-0.1.2/src/opts/ArcherServerClient.py
+-rw-rw-rw-   0        0        0      311 2023-01-24 15:59:21.000000 uscis-opts-0.1.2/src/opts/ContextError.py
+-rw-rw-rw-   0        0        0      381 2023-01-05 18:01:03.000000 uscis-opts-0.1.2/src/opts/SigningError.py
+-rw-rw-rw-   0        0        0        0 2023-01-06 17:11:22.000000 uscis-opts-0.1.2/src/opts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:29:23.660811 uscis-opts-0.1.2/src/opts/templates/
+-rw-rw-rw-   0        0        0      488 2023-02-03 15:15:04.000000 uscis-opts-0.1.2/src/opts/templates/ExecuteSearch.xml
+-rw-rw-rw-   0        0        0      409 2023-02-02 14:28:02.000000 uscis-opts-0.1.2/src/opts/templates/GetReports.xml
+-rw-rw-rw-   0        0        0      478 2023-02-02 17:54:44.000000 uscis-opts-0.1.2/src/opts/templates/GetSearchOptionsByGuid.xml
+-rw-rw-rw-   0        0        0        0 2023-01-06 17:11:22.000000 uscis-opts-0.1.2/src/opts/templates/__init__.py
+-rw-rw-rw-   0        0        0      287 2023-01-05 18:01:03.000000 uscis-opts-0.1.2/src/opts/templates/template.xml
+drwxrwxrwx   0        0        0        0 2023-04-07 19:29:23.702813 uscis-opts-0.1.2/src/uscis_opts.egg-info/
+-rw-rw-rw-   0        0        0     2737 2023-04-07 19:29:23.000000 uscis-opts-0.1.2/src/uscis_opts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2023-04-07 19:29:23.000000 uscis-opts-0.1.2/src/uscis_opts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 19:29:23.000000 uscis-opts-0.1.2/src/uscis_opts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-07 19:29:23.000000 uscis-opts-0.1.2/src/uscis_opts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-07 19:29:23.000000 uscis-opts-0.1.2/src/uscis_opts.egg-info/top_level.txt
```

### Comparing `uscis-opts-0.1.0/LICENSE` & `uscis-opts-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uscis-opts-0.1.0/pyproject.toml` & `uscis-opts-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uscis-opts"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
   { name="Joshua Davis", email="Joshua.C.Davis@uscis.dhs.gov" },
 ]
 description = "A python module to simplify RSA Archer API calls."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `uscis-opts-0.1.0/src/opts/ArcherAuth.py` & `uscis-opts-0.1.2/src/opts/ArcherAuth.py`

 * *Files identical despite different names*

### Comparing `uscis-opts-0.1.0/src/opts/ArcherServerClient.py` & `uscis-opts-0.1.2/src/opts/ArcherServerClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from . import templates
 
 class ArcherServerClient:
   """
   ArcherAPI.ArcherServerClient
 
   A wrapper class to simplify Archer API calls. The different Archer APIs do NOT
-  have feature parity. You will see calls to different Archer APIs in this class.
+  have feature parity. You will see calls to different Archer APIs in this
+  class.
 
   Methods that a user interacts with currently return the following types:
   -- str
   -- pandas.DataFrame
 
   Types to avoid returning:
   -- xml.etree.* (I personally do not find xml or this module intuitive.
@@ -83,15 +84,15 @@
 
     # Map report name to GUID and lookup by name.
     try:
       guid = {element.find('ReportName').text: element.find('ReportGUID').text
               for element
               in root.findall('ReportValue')}[name]
     except KeyError:
-      raise ValueError('Invalid Report Name.')
+      raise ValueError('Invalid name.')
     
     return guid
 
   def get_search_options(self, guid: str) -> ET.Element:
     """
     Get search options for Execute Search. Requires report GUID.
     Use get_report_guid if report name is known, but GUID is not.
@@ -246,14 +247,15 @@
     Positional arguments:
     id -- Tracking ID of record to query for history log data.
     """
     url = f'{self.auth.base_url}/platformapi/core/content/history/{id}'
     headers = {'X-Http-Method-Override': 'GET'}
   
     response = self.auth.session.post(url, headers = headers)
+
     history_audits = response.json()[0]['RequestedObject']['HistoryAudits']
 
     for audit in history_audits:
       temp = []
       for field in audit['FieldHistory']:
         temp.append(audit['FieldHistory'][field])
       audit['FieldHistory'] = temp
@@ -301,15 +303,15 @@
     """
     report_guid = self.get_report_guid(report_name)
     search_options = self.get_search_options(report_guid)
 
     self.context = pd.DataFrame(self.exec_search(search_options))
     self.contextualized = True
 
-  def get_endpoints(self) -> dict:
+  def get_endpoints(self) -> list:
     """
     Get Content API endpoints. Returned to user and used to validate future
     Content API queries.
 
     API Used: Content
     """
     url = f'{self.auth.base_url}/contentapi'
@@ -323,52 +325,73 @@
     endpoints = {}
 
     for endpoint in response.json()['value']:
       if endpoint['kind'] == 'EntitySet':
         endpoints[endpoint['name']] = endpoint['url']
       else:
         # Please file a bug report if you recieve this warning.
-        warnings.warn("Non-EntitySet found in endpoints.", Warning)
+        warnings.warn('Non-EntitySet found in endpoints.', Warning)
 
     self.endpoints = endpoints
     self.last_refresh = datetime.datetime.now()
 
-    return endpoints
+    return list(endpoints.keys())
   
   def get_level_metadata(self, level_alias: str) -> list:
     """
     Query Content API. Max 1000 contents per API call. This function returns
-    all contents.
+    all contents as a json array.
 
     API Used: Content
+
+    Positional arguments:
+    level_alias -- Level alias returned by get_endpoints()
     """
     try:
       if self.last_refresh is None:
         self.get_endpoints()
       url = f'{self.auth.base_url}/contentapi/{self.endpoints[level_alias]}'
     except KeyError:
-      raise ValueError('Invalid Level Alias.')
+      raise ValueError('''Invalid level_alias. Please check your alias or call
+                       get_endpoints() to refresh the endpoints dictionary.''')
     
     headers = {'Cache-Control': 'no-cache'}
     params = {'skip': 0}
 
-    contents = []
+    content = []
 
-    while(params['skip'] == 0 or len(response.json()['value']) > 0):
+    while(True): # see PEP 315
       response = self.auth.session.get(
         url,
         headers = headers,
         params = params
       )
 
-      contents = contents + response.json()['value']
+      if len(response.json()['value']) == 0:
+        break
+
+      content = content + response.json()['value']
       params['skip'] = params['skip'] + len(response.json()['value'])
 
+    return content
+  
+  def get_levels_metadata(self, level_aliases: list) -> dict:
+    """
+    Get level metadata for a list of levels.
+
+    Positional arguments:
+    level_aliases -- Level aliases returned by get_endpoints()
+    """
+    contents = dict.fromkeys(level_aliases)
+
+    for alias in level_aliases:
+      contents[alias] = self.get_level_metadata(alias)
+
     return contents
 
   def __init__(self, auth: 'ArcherAuth') -> None:
     self.auth = auth
-    self.context = None
-    self.contextualized = False
-    self.endpoints = None
-    self.last_refresh = None
-    self.page_size = 1000
+    self.context = None # RESTful
+    self.contextualized = False # RESTful
+    self.endpoints = None # Content
+    self.last_refresh = None # Content
+    self.page_size = 1000 # Web Services
```

### Comparing `uscis-opts-0.1.0/src/uscis_opts.egg-info/SOURCES.txt` & `uscis-opts-0.1.2/src/uscis_opts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

