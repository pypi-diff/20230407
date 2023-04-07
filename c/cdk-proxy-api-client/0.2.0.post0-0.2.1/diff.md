# Comparing `tmp/cdk_proxy_api_client-0.2.0.post0.tar.gz` & `tmp/cdk_proxy_api_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_proxy_api_client-0.2.0.post0.tar", max compression
+gzip compressed data, was "cdk_proxy_api_client-0.2.1.tar", max compression
```

## Comparing `cdk_proxy_api_client-0.2.0.post0.tar` & `cdk_proxy_api_client-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-0.2.0.post0/LICENSE
--rw-r--r--   0        0        0     4404 2023-03-26 16:28:29.410881 cdk_proxy_api_client-0.2.0.post0/README.md
--rw-r--r--   0        0        0      187 2023-03-26 17:00:38.310248 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/__init__.py
--rw-r--r--   0        0        0     1163 2023-03-26 16:47:51.442956 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/admin_auth/__init__.py
--rw-r--r--   0        0        0      133 2023-03-10 11:53:55.066691 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/admin_auth/exceptions.py
--rw-r--r--   0        0        0     4420 2023-03-26 16:47:14.023503 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/cli/__init__.py
--rw-r--r--   0        0        0     4095 2023-03-26 16:43:16.290623 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/cli/main_parser.py
--rw-r--r--   0        0        0     5728 2023-03-14 12:38:20.148498 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/client_wrapper.py
--rw-r--r--   0        0        0      601 2023-03-08 21:22:30.578973 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/common/__init__.py
--rw-r--r--   0        0        0     1174 2023-03-26 16:44:44.959697 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/common/logging.py
--rw-r--r--   0        0        0     3012 2023-03-10 11:34:33.523871 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/errors.py
--rw-r--r--   0        0        0       93 2023-03-08 21:22:30.582973 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/models/__init__.py
--rw-r--r--   0        0        0     1467 2023-03-08 10:34:32.551495 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/models/v1b1.py
--rw-r--r--   0        0        0     1400 2023-03-26 16:47:51.434956 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/proxy_api.py
--rw-r--r--   0        0        0        0 2023-03-14 12:46:32.223933 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/specs/__init__.py
--rw-r--r--   0        0        0     3585 2023-03-26 16:47:16.372532 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/specs/tenant_mappings-input.json
--rw-r--r--   0        0        0     2930 2023-03-26 16:47:51.457956 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/tenant_mappings/__init__.py
--rw-r--r--   0        0        0      414 2023-03-10 12:11:17.799028 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/tenant_mappings/exceptions.py
--rw-r--r--   0        0        0      800 2023-03-26 16:00:22.879474 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/tools/__init__.py
--rw-r--r--   0        0        0     9938 2023-03-26 16:36:20.532587 cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/tools/import_tenants_mappings.py
--rw-r--r--   0        0        0     2444 2023-03-26 17:00:38.309248 cdk_proxy_api_client-0.2.0.post0/pyproject.toml
--rw-r--r--   0        0        0     5916 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.0.post0/setup.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.0.post0/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4404 2023-03-26 16:28:29.410881 cdk_proxy_api_client-0.2.1/README.md
+-rw-r--r--   0        0        0      181 2023-04-07 15:31:20.720589 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/__init__.py
+-rw-r--r--   0        0        0     1163 2023-03-26 16:47:51.442956 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/admin_auth/__init__.py
+-rw-r--r--   0        0        0      133 2023-03-10 11:53:55.066691 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/admin_auth/exceptions.py
+-rw-r--r--   0        0        0     4492 2023-03-30 12:32:52.183010 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/cli/__init__.py
+-rw-r--r--   0        0        0     4062 2023-03-30 15:55:35.980876 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/cli/main_parser.py
+-rw-r--r--   0        0        0     5728 2023-03-14 12:38:20.148498 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/client_wrapper.py
+-rw-r--r--   0        0        0      601 2023-03-08 21:22:30.578973 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/common/__init__.py
+-rw-r--r--   0        0        0     1174 2023-03-26 16:44:44.959697 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/common/logging.py
+-rw-r--r--   0        0        0     3012 2023-03-10 11:34:33.523871 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/errors.py
+-rw-r--r--   0        0        0       93 2023-03-08 21:22:30.582973 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1467 2023-03-08 10:34:32.551495 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/models/v1b1.py
+-rw-r--r--   0        0        0     1400 2023-03-26 16:47:51.434956 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/proxy_api.py
+-rw-r--r--   0        0        0        0 2023-03-14 12:46:32.223933 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/specs/__init__.py
+-rw-r--r--   0        0        0     3825 2023-04-04 16:14:07.707858 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/specs/tenant_mappings-input.json
+-rw-r--r--   0        0        0     2930 2023-04-04 15:57:38.770731 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tenant_mappings/__init__.py
+-rw-r--r--   0        0        0      414 2023-03-10 12:11:17.799028 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tenant_mappings/exceptions.py
+-rw-r--r--   0        0        0      800 2023-03-26 16:00:22.879474 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tools/__init__.py
+-rw-r--r--   0        0        0    11030 2023-04-07 15:30:59.300327 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tools/import_tenants_mappings.py
+-rw-r--r--   0        0        0     2430 2023-04-07 15:31:20.720589 cdk_proxy_api_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5902 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.1/setup.py
+-rw-r--r--   0        0        0     6035 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.1/PKG-INFO
```

### Comparing `cdk_proxy_api_client-0.2.0.post0/LICENSE` & `cdk_proxy_api_client-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/README.md` & `cdk_proxy_api_client-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/admin_auth/__init__.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/admin_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/cli/__init__.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import yaml
 
 try:
     from yaml import Dumper
 except ImportError:
     from yaml import CDumper as Dumper
 
+from compose_x_common.compose_x_common import set_else_none
+
 from cdk_proxy_api_client.admin_auth import AdminAuth
 from cdk_proxy_api_client.cli.main_parser import set_parser
 from cdk_proxy_api_client.common.logging import LOG
 from cdk_proxy_api_client.proxy_api import ApiClient, Multitenancy, ProxyClient
 from cdk_proxy_api_client.tenant_mappings import TenantTopicMappings
 from cdk_proxy_api_client.tools import load_config_file
 from cdk_proxy_api_client.tools.import_tenants_mappings import import_tenants_mappings
@@ -46,15 +48,15 @@
     if action == "list":
         return multitenancy.list_tenants(as_list=True)
 
 
 def tenant_mappings_actions(proxy: ProxyClient, action: str, **kwargs):
     """Manages actions for TenantMappings"""
     tenants_mappings = TenantTopicMappings(proxy)
-    tenant_name = kwargs.pop("tenant_name")
+    tenant_name = set_else_none("tenant_name", kwargs)
     if action == "list":
         return tenants_mappings.list_tenant_topics_mappings(tenant_name).json()
     elif action == "import-from-tenants-config":
         content = load_config_file(path.abspath(kwargs["import_config_file"]))
         topics_mappings = import_tenants_mappings(proxy, content, tenant_name)
         return topics_mappings
     elif action == "import-from-tenant":
```

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/cli/main_parser.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/cli/main_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         name="create",
         help="Create a new tenant mapping",
         parents=[TENANT_PARSER],
     )
     import_from_tenants_parser = mappings_subparser.add_parser(
         name="import-from-tenants-config",
         help="Create topic mappings from existing tenants",
-        parents=[TENANT_PARSER],
     )
     import_from_tenants_parser.add_argument(
         "-f",
         "--import-config-file",
         dest="import_config_file",
         help="Path to the mappings import file",
         required=True,
```

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/client_wrapper.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/common/__init__.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/common/logging.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/common/logging.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/errors.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/models/v1b1.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/models/v1b1.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/proxy_api.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/proxy_api.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/specs/tenant_mappings-input.json` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/specs/tenant_mappings-input.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999218750000001%*

 * *Differences: {"'definitions'": "{'TenantMappingImportItem': {'oneOf': {1: {'properties': {'grant_write_access': "*

 * *                  "OrderedDict([('type', 'boolean'), ('description', 'On import, matched topics "*

 * *                  "will be available in the tenant with write access. NOT RECOMMENDED'), "*

 * *                  "('default', False)])}}}}}"}*

```diff
@@ -27,14 +27,19 @@
                 {
                     "description": "Regular expression",
                     "type": "string"
                 },
                 {
                     "additionalProperties": false,
                     "properties": {
+                        "grant_write_access": {
+                            "default": false,
+                            "description": "On import, matched topics will be available in the tenant with write access. NOT RECOMMENDED",
+                            "type": "boolean"
+                        },
                         "import_prefix": {
                             "description": "Optional - When creating the mapping, adds a prefix to the logical topic name",
                             "type": "string"
                         },
                         "logical_topics_exclude_regexes": {
                             "description": "List of regex to match tenant logical topics to exclude in mapping",
                             "items": {
```

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/tenant_mappings/__init__.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tenant_mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/tools/__init__.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.0.post0/cdk_proxy_api_client/tools/import_tenants_mappings.py` & `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tools/import_tenants_mappings.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 from json import loads
 
 from compose_x_common.compose_x_common import keyisset, set_else_none
 from importlib_resources import files as pkg_files
 from jsonschema import validate
 
-from cdk_proxy_api_client.errors import ProxyGenericException
+from cdk_proxy_api_client.common.logging import LOG
+from cdk_proxy_api_client.errors import ProxyApiException, ProxyGenericException
 from cdk_proxy_api_client.proxy_api import ApiClient, Multitenancy, ProxyClient
 from cdk_proxy_api_client.tenant_mappings import TenantTopicMappings
 
 DEFAULT_SCHEMA_PATH = pkg_files("cdk_proxy_api_client").joinpath(
     "specs/tenant_mappings-input.json"
 )
 
@@ -113,76 +114,97 @@
     topics_exclude_patterns: list[re.Pattern] = []
     topics_include_patterns: list[re.Pattern] = []
     if topics_exclude_pattern_regexes:
         for _exclude_pattern in topics_exclude_pattern_regexes:
             try:
                 topics_exclude_patterns.append(re.compile(_exclude_pattern))
             except Exception as error:
-                print(error)
-                print(
+                LOG.exception(error)
+                LOG.error(
                     "logical_topics_exclude_regexes",
                     _exclude_pattern,
                     "Not a valid regex. Skipping",
                 )
                 return
     if topics_include_pattern_regexes:
         for _include_pattern in topics_include_pattern_regexes:
             try:
                 topics_include_patterns.append(re.compile(_include_pattern))
             except Exception as error:
-                print(error)
-                print(
+                LOG.exception(error)
+                LOG.error(
                     "logical_topics_include_regexes",
                     _include_pattern,
                     "Not a valid regex. Skipping",
                 )
                 return
 
     tenant_mappings = TenantTopicMappings(proxy)
     for _tenant in tenants:
         if _pattern.match(_tenant):
             if process_once and _tenant in processed_tenants:
-                print(
-                    f"Tenant {_tenant} was already processed. Skipping",
-                    processed_tenants,
+                LOG.debug(
+                    "Tenant {} was already processed. Skipping {}".format(
+                        _tenant, processed_tenants
+                    ),
                 )
                 continue
             else:
                 processed_tenants.append(_tenant)
+        else:
+            LOG.debug(f"Skipping tenant {_tenant}")
+            continue
         tenant_topics: list[dict] = get_tenant_logical_topics(proxy, _tenant)
         topics_to_import: list[dict] = deepcopy(tenant_topics)
-        print(
-            f"Tenant {_tenant} topics:",
-            [_t["logicalTopicName"] for _t in tenant_topics],
-        )
         for _import_tenant_topic in tenant_topics:
             for _exclude_pattern in topics_exclude_patterns:
                 if (
                     _exclude_pattern.match(_import_tenant_topic["logicalTopicName"])
                     and _import_tenant_topic["logicalTopicName"] in topics_to_import
                 ):
                     topics_to_import.remove(_import_tenant_topic)
-                    print(
-                        "Topic",
-                        _import_tenant_topic["logicalTopicName"],
-                        "matched against exclude regex",
-                        _exclude_pattern.pattern,
+                    LOG.debug(
+                        "Topic: {} matched against exclude regex: {}".format(
+                            _import_tenant_topic["logicalTopicName"],
+                            _exclude_pattern.pattern,
+                        ),
                     )
-        print(
+        LOG.debug(
             "Topics post exclude", [_t["logicalTopicName"] for _t in topics_to_import]
         )
+        final_topics_import: list[dict] = []
         for _import_tenant_topic in topics_to_import:
             for _include_pattern in topics_include_patterns:
-                if not _include_pattern.match(_import_tenant_topic["logicalTopicName"]):
-                    continue
+                if (
+                    _include_pattern.match(_import_tenant_topic["logicalTopicName"])
+                    and _import_tenant_topic not in final_topics_import
+                ):
+                    final_topics_import.append(_import_tenant_topic)
+                    break
+        LOG.debug(f"Tenant:{_tenant} - Final topic list:{final_topics_import}")
+        grant_write_access = keyisset("grant_write_access", mapping_import_config)
+        for topic_mapping in final_topics_import:
+            try:
                 tenant_mappings.create_tenant_topic_mapping(
                     tenant_name,
-                    _import_tenant_topic["logicalTopicName"],
-                    _import_tenant_topic["physicalTopicName"],
-                    read_only=True,
+                    topic_mapping["logicalTopicName"],
+                    topic_mapping["physicalTopicName"],
+                    read_only=not grant_write_access,
+                )
+                if grant_write_access:
+                    LOG.warn(
+                        "{}:{} - Granting write access.".format(
+                            _tenant, topic_mapping["physicalTopicName"]
+                        )
+                    )
+            except ProxyApiException:
+                print(
+                    "Failed to create mapping from {}: {} does not seem to exist.".format(
+                        _tenant, topic_mapping["physicalTopicName"]
+                    )
                 )
 
 
 def import_from_other_tenants(
     proxy: ProxyClient, import_config: dict, tenant_name: str
 ) -> None:
     """Allows to import existing topics from other tenants in read-only"""
@@ -198,15 +220,14 @@
             _pattern = re.compile(_regex)
             for _tenant in tenants:
                 if _pattern.match(_tenant):
                     tenants.remove(_tenant)
         except Exception as error:
             print(error)
             print(_regex, "not a valid regex. Ignoring")
-
     for _include_item in include_list:
         if isinstance(_include_item, str):
             import_from_tenants_include_string(
                 proxy,
                 _include_item,
                 tenant_name,
                 tenants,
```

### Comparing `cdk_proxy_api_client-0.2.0.post0/pyproject.toml` & `cdk_proxy_api_client-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cdk-proxy-api-client"
 description = "Conduktor Proxy API Client"
-version = "0.2.0.post0"
+version = "0.2.1"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.md"
 license = "LICENSE"
 packages = [{include = "cdk_proxy_api_client"}]
 keywords = ["compose-x", "conduktor", "kafka", "proxy"]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
@@ -30,15 +30,15 @@
 "Source (GitHub)" = "https://github.com/JohnPreston/cdk-proxy-api-client"
 "Source (CodeBerg)" = "https://codeberg.org/JohnPreston/cdk-proxy-api-client"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.2"
 jsonschema = {version = "^4.17.3", optional = true }
-compose-x-common = {version = "^1.2.8", optional = true }
+compose-x-common = {version = "^1.2", optional = true }
 importlib-resources = {version = "^5.12.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 black = "^23.1.0"
 isort = "^5.12.0"
 openapi-python-client = "^0.13.1"
@@ -55,15 +55,15 @@
 cdk-cli = "cdk_proxy_api_client.cli:main"
 
 
 [tool.tbump]
 github_url = "https://codeberg.org/JohnPreston/cdk-proxy-api-client"
 
 [tool.tbump.version]
-current = "0.2.0.post0"
+current = "0.2.1"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `cdk_proxy_api_client-0.2.0.post0/setup.py` & `cdk_proxy_api_client-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 extras_require = \
 {'cli': ['jsonschema>=4.17.3,<5.0.0',
-         'compose-x-common>=1.2.8,<2.0.0',
+         'compose-x-common>=1.2,<2.0',
          'importlib-resources>=5.12.0,<6.0.0'],
  'tools': ['jsonschema>=4.17.3,<5.0.0',
-           'compose-x-common>=1.2.8,<2.0.0',
+           'compose-x-common>=1.2,<2.0',
            'importlib-resources>=5.12.0,<6.0.0']}
 
 entry_points = \
 {'console_scripts': ['cdk-cli = cdk_proxy_api_client.cli:main']}
 
 setup_kwargs = {
     'name': 'cdk-proxy-api-client',
-    'version': '0.2.0.post0',
+    'version': '0.2.1',
     'description': 'Conduktor Proxy API Client',
     'long_description': '# cdk-proxy-api-client\n\nAPI Client library to interact with Conduktor Proxy\n\nCurrent version: v1beta1\n\n\n## Getting started\n\nFirst, create a Proxy Client\n\n```python\nfrom cdk_proxy_api_client.proxy_api import ApiClient, ProxyClient\n\napi = ApiClient("localhost", port=8888, username="superUser", password="superUser")\nproxy_client = ProxyClient(api)\n```\n\n### Features\n\nNote: we assume you are re-using the ``proxy_client`` as shown above.\n\n* Create new Token for a tenant\n\n```python\nfrom cdk_proxy_api_client.admin_auth import AdminAuth\n\nadmin = AdminAuth(proxy_client)\nadmin.create_tenant_credentials("a_tenant_name")\n```\n\n* List all topic mappings for a tenant\n\n```python\nfrom cdk_proxy_api_client.proxy_api import Multitenancy\n\ntenants_mgmt = Multitenancy(proxy_client)\ntenants = tenants_mgmt.list_tenants(as_list=True)\n```\n\n* Create a new mapping for a tenant\n* Delete a tenant - topic mapping\n* Delete all topic mappings for a tenant\n\n```python\nfrom cdk_proxy_api_client.tenant_mappings import TenantTopicMappings\n\ntenant_mappings_mgmt = TenantTopicMappings(proxy_client)\ntenant_mappings_mgmt.create_tenant_topic_mapping(\n    "tenant_name", "logical_name", "real_name"\n)\ntenant_mappings_mgmt.delete_tenant_topic_mapping("tenant_name", "logical_name")\n```\n\n## Testing\nThe testing is for now very manual. See ``e2e_testing.py``\n\nPytest will be added later on\n\n\n## Tools & CLI\n\nTo simplify the usage of the client, you can use some CLI commands\n\n```shell\nusage: CDK Proxy CLI [-h] [--format OUTPUT_FORMAT] --username USERNAME --password PASSWORD --url URL {auth,tenant-topic-mappings,tenants} ...\n\npositional arguments:\n  {auth,tenant-topic-mappings,tenants}\n                        Resources to manage\n    auth                Manages proxy tenant token\n    tenant-topic-mappings\n                        Manages tenant mappings\n    tenants             Manage tenants\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --format OUTPUT_FORMAT, --output-format OUTPUT_FORMAT\n                        output format\n  --username USERNAME\n  --password PASSWORD\n  --url URL\n\n```\n\n### cdk-cli tenant-topic-mappings\n\n```shell\nusage: CDK Proxy CLI tenant-topic-mappings [-h] {list,create,import-from-tenants-config,import-from-tenant,delete-all-mappings,delete-topic-mapping} ...\n\npositional arguments:\n  {list,create,import-from-tenants-config,import-from-tenant,delete-all-mappings,delete-topic-mapping}\n                        Mappings management\n    list                List tenant mappings\n    create              Create a new tenant mapping\n    import-from-tenants-config\n                        Create topic mappings from existing tenants\n    import-from-tenant  Import all topics from a existing tenant\n    delete-all-mappings\n                        Delete all topics mappings for a given tenant\n    delete-topic-mapping\n                        Delete a topic mapping for a given tenant\n\noptional arguments:\n  -h, --help            show this help message and exit\n```\n\n#### import-from-tenants-config\n\nThis command uses a configuration file that will be used to propagate mappings from one/multiple existing tenants to another.\n\nexample file:\n\n```yaml\n---\n# example.config.yaml\n\ntenant_name: application-01\nignore_duplicates_conflict: true\nmappings:\n  - logicalTopicName: data.stock\n    physicalTopicName: data.stock\n    readOnly: true\n```\n\n```shell\ncdk-cli --username ${PROXY_USERNAME} \\\n        --password ${PROXY_PASSWORD} \\\n        --url ${PROXY_URL} \\\n        tenant-topic-mappings import-from-tenants-config -f example.config.yaml\n```\n\n### cdk-cli auth\n\n```shell\ncdk-cli auth --help\nusage: CDK Proxy CLI auth [-h] {create} ...\n\npositional arguments:\n  {create}    Token actions to execute\n    create    Create a new tenant proxy JWT Token\n\noptional arguments:\n  -h, --help  show this help message and exit\n```\n\n#### cdk-cli-create-tenant-token\n\nCreate a new user tenant token\n\n```shell\ncdk-cli \\\n        --username ${PROXY_USERNAME} \\\n        --password ${PROXY_PASSWORD} \\\n        --url ${PROXY_URL} \\\n        auth create \\\n        --lifetime-in-seconds 3600  \\\n        --tenant-name js-fin-panther-stg\n```\n\n### cdk-cli tenants\n\nManage tenants\n\n```shell\ncdk-cli tenants --help\nusage: CDK Proxy CLI tenants [-h] {list} ...\n\npositional arguments:\n  {list}      Manage tenants\n    list      List tenants\n\noptional arguments:\n  -h, --help  show this help message and exit\n```\n',
     'author': 'John "Preston" Mille',
     'author_email': 'john@ews-network.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cdk_proxy_api_client-0.2.0.post0/PKG-INFO` & `cdk_proxy_api_client-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-proxy-api-client
-Version: 0.2.0.post0
+Version: 0.2.1
 Summary: Conduktor Proxy API Client
 License: LICENSE
 Keywords: compose-x,conduktor,kafka,proxy
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: cli
 Provides-Extra: tools
-Requires-Dist: compose-x-common (>=1.2.8,<2.0.0) ; extra == "tools" or extra == "cli"
+Requires-Dist: compose-x-common (>=1.2,<2.0) ; extra == "tools" or extra == "cli"
 Requires-Dist: importlib-resources (>=5.12.0,<6.0.0) ; extra == "tools" or extra == "cli"
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0) ; extra == "tools" or extra == "cli"
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/JohnPreston/cdk-proxy-api-client/issues
 Project-URL: Source (GitHub), https://github.com/JohnPreston/cdk-proxy-api-client
 Project-URL: Source (CodeBerg), https://codeberg.org/JohnPreston/cdk-proxy-api-client
 Description-Content-Type: text/markdown
```

