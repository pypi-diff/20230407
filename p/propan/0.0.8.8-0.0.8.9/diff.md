# Comparing `tmp/propan-0.0.8.8.tar.gz` & `tmp/propan-0.0.8.9.tar.gz`

## Comparing `propan-0.0.8.8.tar` & `propan-0.0.8.9.tar`

### file list

```diff
@@ -1,69 +1,73 @@
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 propan-0.0.8.8/CONTRIBUTING.md
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/1_basic_usage.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/5_publishing.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.8.8/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/__about__.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/cli/__init__.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/cli/app.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/cli/main.py
--rw-r--r--   0        0        0     5846 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/cli/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/cli/supervisors/watchgodreloader.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/log/__init__.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/log/formatter.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/log/logging.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/utils/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/utils/classes.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/utils/functions.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/utils/context/decorate.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/utils/context/main.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/utils/context/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/utils/types/__init__.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 propan-0.0.8.8/propan/utils/types/decorate.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.8.8/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.8.8/scripts/publish.sh
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 propan-0.0.8.8/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 propan-0.0.8.8/scripts/test.sh
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 propan-0.0.8.8/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.8.8/LICENSE
--rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 propan-0.0.8.8/README.md
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 propan-0.0.8.8/pyproject.toml
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 propan-0.0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 propan-0.0.8.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/5_publishing.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/__about__.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/__init__.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/app.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/main.py
+-rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/supervisors/watchgodreloader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/log/__init__.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/log/formatter.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/log/logging.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/classes.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/functions.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/context/decorate.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/context/main.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/context/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/types/__init__.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/types/decorate.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.8.9/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.8.9/scripts/publish.sh
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 propan-0.0.8.9/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 propan-0.0.8.9/scripts/test.sh
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 propan-0.0.8.9/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.8.9/LICENSE
+-rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 propan-0.0.8.9/README.md
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     8980 2020-02-02 00:00:00.000000 propan-0.0.8.9/PKG-INFO
```

### Comparing `propan-0.0.8.8/CONTRIBUTING.md` & `propan-0.0.8.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/3_lifespan_events.py` & `propan-0.0.8.9/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/4_cli_attributes_promotion.py` & `propan-0.0.8.9/examples/4_cli_attributes_promotion.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ... --env=.env
 ... -env=.env
 ... env=.env
 "=" is required
 
 Or you can pass a boolean flags
 ... --use-smth  # passes as use_smth=True
+... --no-use-smth  # passes as use_smth=False
 """
 from propan import Context, PropanApp
 from propan.brokers.rabbit import RabbitBroker
 from pydantic import BaseSettings
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
```

### Comparing `propan-0.0.8.8/examples/5_publishing.py` & `propan-0.0.8.9/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/6_arguments_casting.py` & `propan-0.0.8.9/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/7_handler_errors_processing.py` & `propan-0.0.8.9/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/dependencies/1_dependency_injection.py` & `propan-0.0.8.9/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/dependencies/2_dependency_declaration.py` & `propan-0.0.8.9/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.0.8.9/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/dependencies/5_dependency_nesting.py` & `propan-0.0.8.9/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/dependencies/6_dependecy_calling.py` & `propan-0.0.8.9/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/dependencies/7_annotated.py` & `propan-0.0.8.9/examples/dependencies/7_annotated.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 typing.Annotated class as a shortcut to Depends and Alias
 """
 import logging
 from typing import Annotated
 
 from propan import PropanApp
 from propan.brokers.rabbit import RabbitBroker
-from propan.utils import Depends, Alias, use_context
-
+from propan.utils import Alias, Depends, use_context
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 Logger = Annotated[logging.Logger, Alias("broker.logger")]
 
+
 @use_context
 async def async_dependency(body, logger: Logger):
     logger.info(f"Async calls with: {body}")
     return True
 
 
 Dependency = Annotated[bool, Depends(async_dependency)]
```

### Comparing `propan-0.0.8.8/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.0.8.9/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.0.8.9/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/http_frameworks_integrations/falcon.py` & `propan-0.0.8.9/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/http_frameworks_integrations/fastapi.py` & `propan-0.0.8.9/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/http_frameworks_integrations/quart.py` & `propan-0.0.8.9/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/http_frameworks_integrations/sanic.py` & `propan-0.0.8.9/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/examples/http_frameworks_integrations/tornado.py` & `propan-0.0.8.9/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/brokers/push_back_watcher.py` & `propan-0.0.8.9/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/brokers/model/broker_usecase.py` & `propan-0.0.8.9/propan/brokers/model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/brokers/model/schemas.py` & `propan-0.0.8.9/propan/brokers/model/schemas.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 class NameRequired(BaseModel):
     name: Optional[str] = Field(...)
 
     def __init__(self, name: str, **kwargs: Any):
         super().__init__(name=name, **kwargs)
 
     def __eq__(self, other: object) -> bool:
-        if not isinstance(other, NameRequired):
-            raise ValueError(f"{other} is not NameRequired type")
-        return self.name == other.name
+        return isinstance(other, NameRequired) and self.name == other.name
 
 
 class Queue(NameRequired):
     name: Optional[str] = Field(...)
 
     def __init__(self, name: str, **kwargs: Any):
         super().__init__(name=name, **kwargs)
```

### Comparing `propan-0.0.8.8/propan/brokers/nats/nats_broker.py` & `propan-0.0.8.9/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/brokers/nats/nats_broker.pyi` & `propan-0.0.8.9/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/brokers/nats/nats_js_broker.py` & `propan-0.0.8.9/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.0.8.9/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.0.8.9/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/brokers/rabbit/schemas.py` & `propan-0.0.8.9/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/cli/app.py` & `propan-0.0.8.9/propan/cli/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         )
         self.loop.run_forever()
 
     def _stop(self, log_level: int) -> None:
         self.logger.log(log_level, "Propan app shutting down...")
         self.loop.run_until_complete(self._shutdown())
         self.logger.log(log_level, "Propan app shut down gracefully.")
+        self.loop.close()
 
     async def _startup(self) -> None:
         for func in self._on_startup_calling:
             await call_or_await(func)
 
         if self.broker is not None:
             await self.broker.start()
```

### Comparing `propan-0.0.8.8/propan/cli/startproject.py` & `propan-0.0.8.9/propan/cli/startproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pathlib import Path
 
 
-def create(dirname: str, version: str) -> None:
-    project_dir = _create_project_dir(dirname, version)
+def create(project_dir: Path, version: str) -> Path:
+    project_dir = _create_project_dir(project_dir, version)
     app_dir = _create_app_dir(project_dir / "app")
     _create_config_dir(app_dir / "config")
     _create_core_dir(app_dir / "core")
     _create_apps_dir(app_dir / "apps")
-    exit()
+    return project_dir
 
 
-def _create_project_dir(dirname: str, version: str) -> Path:
-    project_dir = _touch_dir(Path.cwd() / dirname)
+def _create_project_dir(dirname: Path, version: str) -> Path:
+    project_dir = _touch_dir(dirname)
 
     if project_dir.exists() is False:
         project_dir.mkdir()
 
     _write_file(project_dir / "README.md")
 
     _write_file(
```

### Comparing `propan-0.0.8.8/propan/cli/supervisors/basereload.py` & `propan-0.0.8.9/propan/cli/supervisors/basereload.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,65 @@
 import os
 import threading
+from multiprocessing.context import SpawnProcess
 from typing import Any, Callable, Optional, Tuple
 
 from propan.cli.supervisors.utils import get_subprocess, set_exit
 from propan.log import logger
 
 
 class BaseReload:
+    _process: SpawnProcess
+    _target: Callable[..., Any]
+    _args: Tuple[Any, ...]
+
+    reload_delay: Optional[float]
+    should_exit: threading.Event
+    pid: int
+    reloader_name: str = ""
+
     def __init__(
         self,
         target: Callable[..., Any],
         args: Tuple[Any, ...],
         reload_delay: Optional[float] = 0.5,
     ) -> None:
-        self.target = target
+        self._target = target
+        self._args = args
+
         self.should_exit = threading.Event()
         self.pid = os.getpid()
-        self.reloader_name: Optional[str] = None
         self.reload_delay = reload_delay
-        self._args = args
+
+        set_exit(lambda *_: self.should_exit.set())
 
     def run(self) -> None:
         self.startup()
         while not self.should_exit.wait(self.reload_delay):
             if self.should_restart():
                 self.restart()
         self.shutdown()
 
     def startup(self) -> None:
         logger.info(f"Started reloader process [{self.pid}] using {self.reloader_name}")
-        set_exit(lambda *_: self.should_exit.set())
-        self._start_process()
+        self._process = self._start_process()
 
     def restart(self) -> None:
         self._stop_process()
         logger.info("Process successfully reloaded")
-        self._start_process()
+        self._process = self._start_process()
 
     def shutdown(self) -> None:
         self._stop_process()
         logger.info(f"Stopping reloader process [{self.pid}]")
 
     def _stop_process(self) -> None:
-        self.process.terminate()
-        self.process.join()
+        self._process.terminate()
+        self._process.join()
 
-    def _start_process(self) -> None:
-        self.process = get_subprocess(target=self.target, args=self._args)
-        self.process.start()
+    def _start_process(self) -> SpawnProcess:
+        process = get_subprocess(target=self._target, args=self._args)
+        process.start()
+        return process
 
     def should_restart(self) -> bool:
         raise NotImplementedError("Reload strategies should override should_restart()")
```

### Comparing `propan-0.0.8.8/propan/cli/supervisors/multiprocess.py` & `propan-0.0.8.9/propan/cli/supervisors/multiprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 import os
 import threading
 from multiprocessing.context import SpawnProcess
 from typing import Any, Callable, List, Tuple
 
+from propan.cli.supervisors.basereload import BaseReload
 from propan.cli.supervisors.utils import get_subprocess, set_exit
 from propan.log import logger
 
 
-class Multiprocess:
+class Multiprocess(BaseReload):
     def __init__(
-        self, target: Callable[..., Any], args: Tuple[Any, ...], workers: int
+        self,
+        target: Callable[..., Any],
+        args: Tuple[Any, ...],
+        workers: int
     ) -> None:
-        self._target = target
-        self._args = args
+        super().__init__(target, args, None)
 
         self.workers = workers
         self.processes: List[SpawnProcess] = []
 
-        self.should_exit = threading.Event()
-        self.pid = os.getpid()
-
-    def run(self) -> None:
-        self.startup()
-        self.should_exit.wait()
-        self.shutdown()
-
     def startup(self) -> None:
         logger.info(f"Started parent process [{self.pid}]")
 
-        set_exit(lambda *_: self.should_exit.set())
-
         for _ in range(self.workers):
-            process = get_subprocess(target=self._target, args=self._args)
-            process.start()
+            process = self._start_process()
             logger.info(f"Started child process [{process.pid}]")
             self.processes.append(process)
 
     def shutdown(self) -> None:
         for process in self.processes:
             process.terminate()
             logger.info(f"Stopping child process [{process.pid}]")
```

### Comparing `propan-0.0.8.8/propan/cli/supervisors/utils.py` & `propan-0.0.8.9/propan/cli/supervisors/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import multiprocessing
 import os
 import signal
 import sys
 from multiprocessing.context import SpawnProcess
 from pathlib import Path
 from types import FrameType
-from typing import Any, Callable, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, List, Optional, Sequence, Tuple, TypeVar, Union
 
 from propan.log import logger
 
 multiprocessing.allow_connection_pickling()
 spawn = multiprocessing.get_context("spawn")
 
 
 HANDLED_SIGNALS = (
     signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
     signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
 )
 
 
-DIR = Union[Path, str]
-DIRS = Union[Sequence[DIR], DIR, None]
+DIR = TypeVar("DIR", bound=Union[Path, str])
+DIRS = TypeVar("DIRS", bound=Union[Sequence[DIR], DIR, None])
 
 
 def set_exit(func: Callable[[int, Optional[FrameType]], Any]) -> None:
     for sig in HANDLED_SIGNALS:
         signal.signal(sig, func)
```

### Comparing `propan-0.0.8.8/propan/cli/supervisors/watchgodreloader.py` & `propan-0.0.8.9/propan/cli/supervisors/watchgodreloader.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/log/formatter.py` & `propan-0.0.8.9/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/log/logging.py` & `propan-0.0.8.9/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/utils/functions.py` & `propan-0.0.8.9/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/utils/context/decorate.py` & `propan-0.0.8.9/propan/utils/context/decorate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from functools import wraps
 from inspect import iscoroutinefunction, signature
-from typing import Any, Callable, Dict, List
+from typing import Any, Callable, Dict, List, TypeVar
 
 from propan.utils.context.main import context as global_context
 from propan.utils.context.types import Alias, Depends
 from propan.utils.functions import call_or_await, remove_useless_arguments
 
-FuncArgName = str
-AliasStr = str
+FuncArgName = TypeVar("FuncArgName", bound=str)
+AliasStr = TypeVar("AliasStr", bound=str)
 
 
 def use_context(func: Callable[..., Any]) -> Callable[..., Any]:
     sig = signature(func).parameters
 
     aliases: Dict[AliasStr, FuncArgName] = {}
     dependencies: Dict[FuncArgName, Callable[..., Any]] = {}
```

### Comparing `propan-0.0.8.8/propan/utils/context/main.py` & `propan-0.0.8.9/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/propan/utils/types/decorate.py` & `propan-0.0.8.9/propan/utils/types/decorate.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/LICENSE` & `propan-0.0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/README.md` & `propan-0.0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.8/pyproject.toml` & `propan-0.0.8.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
     "pydantic>=1.8",
     "watchgod",
-    "click",
+    "typer",
     "uvloop>=0.14.0,!=0.15.0,!=0.15.1; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/Lancetnik/Propan"
@@ -84,14 +84,15 @@
 dev = [
     "propan[test]",
 
     "mypy==1.1.1",
     "black==23.3.0",
     "isort==5.12.0",
     "ruff==0.0.261",
+    "typer[all]",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 allow-ambiguous-features = true
 
 [tool.hatch.version]
@@ -145,14 +146,15 @@
 known-third-party = ["propan", "pydantic", "aio-pika", "nats-py"]
 
 [tool.ruff.flake8-bugbear]
 extend-immutable-calls = [
     "propan.Depends", "propan.Alias",
     "propan.utils.Depends", "propan.utils.Alias",
     "propan.utils.context.Depends", "propan.utils.context.Alias",
+    "typer.Argument", "typer.Option",
 ]
 
 [tool.coverage.run]
 parallel = true
 source = [
     "propan",
     "tests"
```

### Comparing `propan-0.0.8.8/PKG-INFO` & `propan-0.0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.0.8.8
+Version: 0.0.8.9
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://github.com/Lancetnik/Propan
 Project-URL: Documentation, https://github.com/Lancetnik/Propan
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
@@ -32,29 +32,30 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
-Requires-Dist: click
 Requires-Dist: pydantic>=1.8
+Requires-Dist: typer
 Requires-Dist: uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')
 Requires-Dist: watchgod
 Provides-Extra: async_nats
 Requires-Dist: nats-py>=2; extra == 'async_nats'
 Provides-Extra: async_rabbit
 Requires-Dist: aio-pika>=9; extra == 'async_rabbit'
 Requires-Dist: pika-stubs; extra == 'async_rabbit'
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: isort==5.12.0; extra == 'dev'
 Requires-Dist: mypy==1.1.1; extra == 'dev'
 Requires-Dist: propan[test]; extra == 'dev'
 Requires-Dist: ruff==0.0.261; extra == 'dev'
+Requires-Dist: typer[all]; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage[toml]>=7.2; extra == 'test'
 Requires-Dist: propan[async-nats]; extra == 'test'
 Requires-Dist: propan[async-rabbit]; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.21; extra == 'test'
 Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
```

