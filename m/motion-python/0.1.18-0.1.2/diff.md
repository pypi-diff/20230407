# Comparing `tmp/motion_python-0.1.18.tar.gz` & `tmp/motion_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.18.tar", max compression
+gzip compressed data, was "motion_python-0.1.2.tar", max compression
```

## Comparing `motion_python-0.1.18.tar` & `motion_python-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,24 @@
--rw-r--r--   0        0        0     2819 2023-04-07 19:46:13.438624 motion_python-0.1.18/README.md
--rw-r--r--   0        0        0      641 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/api/__init__.py
--rw-r--r--   0        0        0     6702 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/api/models.py
--rw-r--r--   0        0        0     2582 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/cli.py
--rw-r--r--   0        0        0     6675 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/client.py
--rw-r--r--   0        0        0    21748 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/cursor.py
--rw-r--r--   0        0        0     8091 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1934 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      421 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1351 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4564 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     4754 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     1771 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/routing.py
--rw-r--r--   0        0        0     2671 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/schema.py
--rw-r--r--   0        0        0    14188 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/store.py
--rw-r--r--   0        0        0     3741 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/task.py
--rw-r--r--   0        0        0     5010 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/trigger.py
--rw-r--r--   0        0        0     1092 2023-04-07 19:46:13.442624 motion_python-0.1.18/motion/utils.py
--rw-r--r--   0        0        0     1416 2023-04-07 19:46:34.402934 motion_python-0.1.18/pyproject.toml
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.18/PKG-INFO
+-rw-r--r--   0        0        0     1640 2023-03-30 02:40:08.524296 motion_python-0.1.2/README.md
+-rw-r--r--   0        0        0      447 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/__init__.py
+-rw-r--r--   0        0        0       64 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/api/__init__.py
+-rw-r--r--   0        0        0     6610 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/api/api.py
+-rw-r--r--   0        0        0      652 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/api/models.py
+-rw-r--r--   0        0        0     3469 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/cli.py
+-rw-r--r--   0        0        0     6592 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/client.py
+-rw-r--r--   0        0        0    21058 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/cursor.py
+-rw-r--r--   0        0        0     6101 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/entry.py
+-rw-r--r--   0        0        0      374 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/exampleproj/mconfig.py
+-rw-r--r--   0        0        0       78 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/exampleproj/schemas/__init__.py
+-rw-r--r--   0        0        0      256 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/exampleproj/schemas/chat.py
+-rw-r--r--   0        0        0      993 2023-03-30 02:40:08.524296 motion_python-0.1.2/motion/exampleproj/test.py
+-rw-r--r--   0        0        0      141 2023-03-30 02:40:08.528296 motion_python-0.1.2/motion/exampleproj/triggers/__init__.py
+-rw-r--r--   0        0        0     1097 2023-03-30 02:40:08.528296 motion_python-0.1.2/motion/exampleproj/triggers/chatbot.py
+-rw-r--r--   0        0        0      604 2023-03-30 02:40:08.528296 motion_python-0.1.2/motion/exampleproj/triggers/generate.py
+-rw-r--r--   0        0        0     1348 2023-03-30 02:40:08.528296 motion_python-0.1.2/motion/routing.py
+-rw-r--r--   0        0        0     2875 2023-03-30 02:40:08.528296 motion_python-0.1.2/motion/schema.py
+-rw-r--r--   0        0        0    15277 2023-03-30 02:40:08.528296 motion_python-0.1.2/motion/store.py
+-rw-r--r--   0        0        0     3432 2023-03-30 02:40:08.528296 motion_python-0.1.2/motion/task.py
+-rw-r--r--   0        0        0     4362 2023-03-30 02:40:08.528296 motion_python-0.1.2/motion/trigger.py
+-rw-r--r--   0        0        0     1105 2023-03-30 02:40:08.528296 motion_python-0.1.2/motion/utils.py
+-rw-r--r--   0        0        0     1287 2023-03-30 02:40:38.752545 motion_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 motion_python-0.1.2/PKG-INFO
```

### Comparing `motion_python-0.1.18/motion/api/api.py` & `motion_python-0.1.2/motion/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import typing
 from io import BytesIO
 from urllib.parse import parse_qs
 
 import pandas as pd
 from fastapi import Depends, FastAPI, File, HTTPException, Request, Response, UploadFile
@@ -15,15 +17,15 @@
 def df_to_json_response(df: pd.DataFrame) -> Response:
     return Response(
         df.to_parquet(engine="pyarrow", index=False),
         media_type="application/octet-stream",
     )
 
 
-def create_fastapi_app(store: Store, testing: bool = False) -> FastAPI:
+def create_app(store: Store, testing: bool = False) -> FastAPI:
     # Security
     MOTION_API_TOKEN = os.environ.get("MOTION_API_TOKEN")
     if not MOTION_API_TOKEN:
         raise ValueError(
             "MOTION_API_TOKEN environment variable is not set. Please run `motion token` to generate a token, and export MOTION_API_TOKEN={result}."
         )
 
@@ -130,18 +132,14 @@
     async def root() -> dict:
         return {"message": "Hello World"}
 
     @app.get("/session_id/")
     async def session_id() -> typing.Any:
         return app.state.store.session_id
 
-    @app.post("/checkpoint/")
-    async def checkpoint() -> typing.Any:
-        return app.state.store.checkpoint_pa()
-
     @app.on_event("shutdown")
     async def shutdown() -> None:
         if not app.state.testing:
             app.state.store.stop()
 
     # JSON API
```

### Comparing `motion_python-0.1.18/motion/client.py` & `motion_python-0.1.2/motion/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import io
 import json
 import typing
 from enum import Enum
 
 import pandas as pd
 import requests
@@ -17,15 +19,15 @@
     Args:
         name (str): The name of the store.
     """
 
     def __init__(
         self,
         name: str,
-        server: typing.Union[str, FastAPI],
+        server: str | FastAPI,
         bearer_token: str,
     ) -> None:
         if not bearer_token:
             raise ConnectionError(
                 f"Could not find bearer token for {name}. Please set the MOTION_API_TOKEN environment variable, or pass in the token to the `motion.connect` function if you are using `motion.connect`."
             )
 
@@ -49,15 +51,15 @@
                 )
             self.session_id = requests.get(self.server + "/session_id/").json()  # type: ignore
 
     def addStore(self, store: Store) -> None:
         self.store = store
         self.session_id = self.store.session_id
 
-    def close(self, wait: bool = False) -> None:
+    def close(self, wait: bool = True) -> None:
         if isinstance(self.server, FastAPI):
             self.store.stop(wait=wait)
 
     def __del__(self) -> None:
         self.close(wait=False)
 
     def getWrapper(self, dest: str, **kwargs: typing.Any) -> typing.Any:
@@ -162,15 +164,15 @@
         return response
 
     def set(
         self,
         *,
         relation: str,
         identifier: str,
-        key_values: typing.Dict[str, typing.Any],
+        key_values: dict[str, typing.Any],
     ) -> typing.Any:
         # Convert enums to their values
 
         for key, value in key_values.items():
             if isinstance(value, Enum):
                 key_values.update({key: value.value})
 
@@ -205,10 +207,7 @@
 
     def duplicate(self, *, relation: str, identifier: str) -> typing.Any:
         data = json.dumps({"relation": relation, "identifier": identifier})
         return self.postWrapper(
             "/duplicate/",
             data=data,
         )
-
-    def checkpoint(self) -> typing.Any:
-        return self.postWrapper("/checkpoint/", data={})
```

### Comparing `motion_python-0.1.18/motion/cursor.py` & `motion_python-0.1.2/motion/cursor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Database connection, with functions that a users is allowed to
 call within trigger lifecycle methods.
 """
-
+from __future__ import annotations
 
 import collections
 import threading
 import typing
 import uuid
 from enum import Enum
 
@@ -19,26 +19,26 @@
 
 
 class Cursor:
     def __init__(
         self,
         *,
         name: str,
-        relations: typing.Dict[str, pa.Table],
+        relations: dict[str, pa.Table],
         log_table: pa.Table,
-        table_columns: typing.Dict[str, list[str]],
-        triggers: typing.Dict[str, list[TriggerFn]],
+        table_columns: dict[str, list[str]],
+        triggers: dict[str, list[TriggerFn]],
         write_lock: threading.Lock,
         session_id: str,
         wait_for_results: bool = False,
-        triggers_to_run_on_duplicate: typing.Dict[TriggerFn, TriggerElement] = {},
+        triggers_to_run_on_duplicate: dict[TriggerFn, TriggerElement] = {},
         spawned_by: TriggerElement = None,  # type: ignore
     ):
         self.name = name
-        self.relations: typing.Dict[str, pa.Table] = relations
+        self.relations: dict[str, pa.Table] = relations
         self.log_table = log_table
         self.table_columns = table_columns
         self.triggers = triggers
         self.write_lock = write_lock
         self.session_id = session_id
         self.wait_for_results = wait_for_results
         self.fit_events: list[threading.Event] = []
@@ -46,15 +46,14 @@
         self.spawned_by = spawned_by
 
     def __del__(self) -> None:
         if self.wait_for_results:
             self.waitForResults()
 
     def waitForResults(self) -> None:
-        """Waits for all fit events to finish."""
         for t in self.fit_events:
             t.wait()
         self.fit_events = []
 
     def getNewId(self, relation: str, key: str = "identifier") -> str:
         """Get a new id for a relation.
 
@@ -98,19 +97,19 @@
 
         return result
 
     def set(
         self,
         *,
         relation: str,
-        key_values: typing.Dict[str, typing.Any],
+        key_values: dict[str, typing.Any],
         identifier: str = "",
     ) -> str:
-        """Sets given key-value pairs for an identifier in a relation.
-        Overwrites existing values.
+        """Set multiple values for a key in a relation.
+        TODO(shreyashankar): Handle complex types.
 
         Args:
             relation (str): The relation to set the value in.
             identifier (str): The id of the record to set the value for.
             key_values (typing.Dict[str, typing.Any]): The key-value pairs to set.
 
         Returns:
@@ -173,159 +172,173 @@
                 new_row = pa.Table.from_pandas(row, schema=table.schema)
 
                 filtered_table = pc.filter(table, pc.invert(condition))
                 final_table = pa.concat_tables([filtered_table, new_row])
                 self.relations[relation] = final_table
 
         # Get all triggers to run
-        triggers_to_run: typing.Dict[TriggerFn, TriggerElement] = {}
+        triggers_to_run: dict[TriggerFn, TriggerElement] = {}
         for key, value in key_values.items():
             if f"{relation}.{key}" not in self.triggers:
                 continue
 
-            trigger_context = TriggerElement(
+            triggered_by = TriggerElement(
                 relation=relation,
                 identifier=identifier,
                 key=key,
                 value=value,
             )
             for trigger in self.triggers.get(f"{relation}.{key}", []):
                 if trigger in triggers_to_run.keys():
                     continue
 
-                triggers_to_run[trigger] = trigger_context
+                triggers_to_run[trigger] = triggered_by
 
         # Run triggers, passing in remainder of triggers_to_run
-        for trigger, trigger_context in triggers_to_run.items():
+        for trigger, triggered_by in triggers_to_run.items():
             other_triggers_to_run = {
                 k: triggers_to_run[k] for k in triggers_to_run if k != trigger
             }
             self.executeTrigger(
                 trigger=trigger,
-                trigger_context=trigger_context,
+                triggered_by=triggered_by,
                 triggers_to_run_on_duplicate=other_triggers_to_run,
             )
 
         return identifier
 
     def logTriggerExecution(
         self,
         trigger_name: str,
         trigger_version: int,
         trigger_action: str,
-        trigger_context: TriggerElement,
+        triggered_by: TriggerElement,
     ) -> None:
         """Logs a trigger execution.
 
         Args:
             trigger_name (str): The name of the trigger.
             trigger_version (int): The version of the trigger.
             trigger_action (str): The action of the trigger.
-            trigger_context (TriggerElement): The element that triggered the trigger.
+            triggered_by (TriggerElement): The element that triggered the trigger.
         """
 
         # Append to the log table
         new_row = {
             "executed_time": pd.Timestamp.now(),
             "session_id": self.session_id,
             "trigger_name": trigger_name,
             "trigger_version": trigger_version,
             "trigger_action": trigger_action,
-            "relation": trigger_context.relation,
-            "identifier": trigger_context.identifier,
-            "trigger_key": trigger_context.key,
+            "relation": triggered_by.relation,
+            "identifier": triggered_by.identifier,
+            "trigger_key": triggered_by.key,
         }
         new_row = pa.Table.from_pandas(
             pd.DataFrame(new_row, index=[0]), schema=self.log_table.schema
         )
 
         with self.write_lock:
             self.log_table = pa.concat_tables([self.log_table, new_row])
 
     def executeTrigger(
         self,
         *,
         trigger: TriggerFn,
-        trigger_context: TriggerElement,
-        triggers_to_run_on_duplicate: typing.Dict[TriggerFn, TriggerElement] = {},
+        triggered_by: TriggerElement,
+        triggers_to_run_on_duplicate: dict[TriggerFn, TriggerElement] = {},
     ) -> None:
         """Execute a trigger.
 
         Args:
             trigger (TriggerFn): The trigger to execute.
-            trigger_context (TriggerElement): The element that triggered the trigger.
+            triggered_by (TriggerElement): The element that triggered the trigger.
             triggers_to_run (typing.Dict[TriggerFn, TriggerElement], optional): The triggers to run whenever duplicate is called within a trigger. Defaults to {}.
         """
         try:
-            self._executeTrigger(trigger, trigger_context, triggers_to_run_on_duplicate)
+            self._executeTrigger(trigger, triggered_by, triggers_to_run_on_duplicate)
         except RecursionError:
             raise RecursionError(
                 f"Recursion error in trigger {trigger[0]}. Please make sure you do not have a cycle in your triggers."
             )
 
     def _executeTrigger(
         self,
         trigger: TriggerFn,
-        trigger_context: TriggerElement,
-        triggers_to_run_on_duplicate: typing.Dict[TriggerFn, TriggerElement] = {},
+        triggered_by: TriggerElement,
+        triggers_to_run_on_duplicate: dict[TriggerFn, TriggerElement] = {},
     ) -> None:
         """Execute a trigger.
 
         Args:
             trigger (TriggerFn): The trigger to execute.
-            trigger_context (TriggerElement): The element that triggered the trigger.
+            triggered_by (TriggerElement): The element that triggered the trigger.
             triggers_to_run (typing.Dict[TriggerFn, TriggerElement], optional): The triggers to run whenever duplicate is called within a trigger. Defaults to {}.
         """
-        trigger_name, trigger_fn = trigger
+        trigger_name, trigger_fn, isTransform = trigger
         logger.info(
-            f"Running trigger {trigger_name} for identifier {trigger_context.identifier}, key {trigger_context.key}..."
+            f"Running trigger {trigger_name} for identifier {triggered_by.identifier}, key {triggered_by.key}..."
         )
         new_connection = Cursor(
             name=self.name,
             relations=self.relations,
             log_table=self.log_table,
             table_columns=self.table_columns,
             triggers=self.triggers,
             write_lock=self.write_lock,
             session_id=self.session_id,
             wait_for_results=self.wait_for_results,
             triggers_to_run_on_duplicate=triggers_to_run_on_duplicate,
-            spawned_by=trigger_context,
+            spawned_by=triggered_by,
         )
 
-        # Get route for key
-        route = trigger_fn.route_map.get(
-            f"{trigger_context.relation}.{trigger_context.key}", None
-        )
-        if route is None:
-            raise NotImplementedError(
-                f"Route not found for {trigger_context.relation}.{trigger_context.key}."
+        if not isTransform:
+            trigger_fn(
+                new_connection,
+                triggered_by,
             )
+            # Log the trigger execution
+            self.logTriggerExecution(trigger_name, 0, "function", triggered_by)
 
-        # Execute the transform lifecycle: infer -> fit
-        infer_context = None
-        if route.infer is not None:
-            infer_context = route.infer(new_connection, trigger_context)
-            self.logTriggerExecution(
-                trigger_name, trigger_fn.version, "infer", trigger_context
+            logger.info(
+                f"Finished running trigger {trigger_name} for identifier {triggered_by.identifier}."
             )
 
-        # Fit is asynchronous
-        if route.fit is not None:
-            fit_thread = trigger_fn.fitWrapper(
-                new_connection, trigger_name, trigger_context, infer_context
-            )
-            self.fit_events.append(fit_thread)
         else:
-            logger.info(
-                f"Finished running trigger {trigger_name} for identifier {trigger_context.identifier}."
+            # Get route for key
+            route = trigger_fn.route_map.get(
+                f"{triggered_by.relation}.{triggered_by.key}", None
             )
+            if route is None:
+                raise NotImplementedError(
+                    f"Route not found for {triggered_by.relation}.{triggered_by.key}."
+                )
+
+            # Execute the transform lifecycle: infer -> fit
+            if route.infer is not None:
+                route.infer(new_connection, triggered_by)
+                self.logTriggerExecution(
+                    trigger_name, trigger_fn.version, "infer", triggered_by
+                )
+
+            # Fit is asynchronous
+            if route.fit is not None:
+                fit_thread = trigger_fn.fitWrapper(
+                    new_connection,
+                    trigger_name,
+                    triggered_by,
+                )
+                self.fit_events.append(fit_thread)
+            else:
+                logger.info(
+                    f"Finished running trigger {trigger_name} for identifier {triggered_by.identifier}."
+                )
 
     def duplicate(self, relation: str, identifier: str) -> str:
-        """Duplicates a record in a relation. Doesn't rerun any triggers for old keys on the new record.
+        """Duplicate a record in a relation. Doesn't run triggers.
 
         Args:
             relation (str): The relation to duplicate the record in.
             identifier (str): The identifier of the record to duplicate.
 
         Returns:
             str: The new identifier of the duplicated record.
@@ -354,49 +367,49 @@
         if (
             self.spawned_by is not None
             and self.spawned_by.identifier == identifier
             and self.spawned_by.relation == relation
         ):
             for (
                 trigger,
-                trigger_context,
+                triggered_by,
             ) in self.triggers_to_run_on_duplicate.items():
                 other_triggers_to_run = {
                     k: self.triggers_to_run_on_duplicate[k]
                     for k in self.triggers_to_run_on_duplicate
                     if k != trigger
                 }
-                new_trigger_context = trigger_context._replace(identifier=new_id)
+                new_triggered_by = triggered_by._replace(identifier=new_id)
                 self.executeTrigger(
                     trigger=trigger,
-                    trigger_context=new_trigger_context,
+                    triggered_by=new_triggered_by,
                     triggers_to_run_on_duplicate=other_triggers_to_run,
                 )
 
         return new_id
 
     def get(
         self,
         *,
         relation: str,
         identifier: str,
         keys: list[str],
         **kwargs: typing.Any,
     ) -> typing.Any:
-        """Get values for an identifier's keys in a relation. Can pass in ["*"] as the keys argument to get all keys.
+        """Get values for an identifier's keys in a relation.
+        TODO: Handle complex types.
 
         Args:
             relation (str): The relation to get the value from.
             identifier (str): The identifier of the record to get the value for.
             keys (typing.List[str]): The keys to get the values for.
 
         Keyword Args:
-            include_derived (bool, optional): Whether to include derived ids in the result. Defaults to False.
-            filter_null (bool, optional): Whether to filter out null values. Filters all records with any null walue for any of the keys requested. Only used in conjuction with include_derived. Defaults to True.
-            as_df (bool, optional): Whether to return the result as a pandas dataframe. Defaults to False.
+            include_derived (bool, optional): Whether to include derived ids. Defaults to False.
+            filter_null (bool, optional): Whether to filter out null values. Only used in conjuction with include_derived. Defaults to True.
 
         Returns:
             typing.Any: The values for the keys.
         """
 
         if not identifier:
             raise ValueError("Identifier cannot be empty.")
@@ -487,25 +500,22 @@
         self,
         *,
         relation: str,
         identifiers: list[str],
         keys: list[str],
         **kwargs: typing.Any,
     ) -> pd.DataFrame:
-        """Get values for a many identifiers' keys in a relation. Can pass in ["*"] as the keys argument to get all keys.
+        """Get multiple values for keys in a relation.
+        TODO: Handle complex types.
 
         Args:
             relation (str): The relation to get the value from.
             identifiers (typing.List[int]): The ids of the records to get the value for.
             keys (typing.List[str]): The keys to get the values for.
-
-        Keyword Args:
-            include_derived (bool, optional): Whether to include derived ids in the result. Defaults to False.
-            filter_null (bool, optional): Whether to filter out null values. Filters all records with any null walue for any of the keys requested. Only used in conjuction with include_derived. Defaults to True.
-            as_df (bool, optional): Whether to return the result as a pandas dataframe. Defaults to False.
+            filter_null (bool, optional): Whether to filter out null values.  Defaults to True.
 
 
         Returns:
             pd.DataFrame: The values for the key.
         """
 
         con = duckdb.connect()
@@ -573,23 +583,14 @@
         res = con.execute(
             f"SELECT identifier FROM scanner WHERE {key} = ?",
             (value,),
         ).fetchall()
         return [r[0] for r in res]
 
     def sql(self, query: str, as_df: bool = True) -> typing.Any:
-        """Executes a SQL query on the relations. Specify the relations as tables in the query.
-
-        Args:
-            query (str): SQL query to execute.
-            as_df (bool, optional): Whether to return the result as a pandas dataframe. Defaults to True.
-
-        Returns:
-            typing.Any: Pandas dataframe if as_df is True, else list of tuples.
-        """
         con = duckdb.connect()
 
         # Create a table for each relation
         for relation, table in self.relations.items():
             locals()[relation] = table
 
         return (
```

### Comparing `motion_python-0.1.18/motion/entry.py` & `motion_python-0.1.2/motion/entry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,30 @@
+from __future__ import annotations
+
 import logging
 import os
-import shutil
-import typing
 import uuid
 
 import colorlog
 import uvicorn
 
-from motion.api import create_fastapi_app
+from motion.api import create_app
 from motion.client import ClientConnection
 from motion.store import Store
-from motion.utils import PRODUCTION_SESSION_ID
 
 
 def create_token() -> str:
     """Create a token for the API.
 
     Returns:
         str: The token.
     """
     return str(uuid.uuid4())
 
 
-def create_example_app(name: str, author: str) -> None:
-    """Creates a motion app from examples."""
-    name = name.strip().lower()
-
-    if name == "cooking":
-        # Copy the example project
-        shutil.copytree(
-            os.path.join(os.path.dirname(__file__), f"examples/{name}"), name
-        )
-
-        # Create config
-        with open(os.path.join(name, "mconfig.py"), "w") as f:
-            f.write(
-                open(
-                    os.path.join(
-                        os.path.dirname(__file__),
-                        f"examples/{name}/mconfig.py",
-                    ),
-                )
-                .read()
-                .replace("{1}", author)
-            )
-
-    else:
-        raise ValueError(f"Example application {name} does not exist.")
-
-
-def create_app(name: str, author: str) -> None:
-    """Creates a motion app."""
-    name = name.strip().lower()
-    if len(name.split(" ")) > 1:
-        raise ValueError("Name cannot contain spaces.")
-
-    if os.path.exists(name):
-        raise ValueError(f"Directory {name} already exists.")
-
-    # Copy over the example project
-    shutil.copytree(os.path.join(os.path.dirname(__file__), "examples/basic"), name)
-
-    # Create store setup file
-    with open(os.path.join(name, "mconfig.py"), "w") as f:
-        f.write(
-            open(
-                os.path.join(
-                    os.path.dirname(__file__),
-                    "examples/basic/mconfig.py",
-                ),
-            )
-            .read()
-            .replace("{0}", name)
-            .replace("{1}", author)
-        )
-
-
 def init(
     mconfig: dict, disable_cron_triggers: bool = False, session_id: str = ""
 ) -> Store:
     """Initialize the motion store.
 
     Args:
         mconfig (dict): The motion configuration.
@@ -110,55 +55,63 @@
         session_id=session_id,
         datastore_prefix=os.path.join(MOTION_HOME, "datastores"),
         checkpoint=checkpoint,
         disable_cron_triggers=disable_cron_triggers,
     )
 
     # Create relations
-    for relation in mconfig["relations"]:
-        store.addrelation_pa(relation.__name__, relation)
+    for relation, schema in mconfig["relations"].items():
+        store.addrelation_pa(relation, schema)
 
     # Create triggers
-    for trigger in mconfig["triggers"]:
+    for trigger, keys in mconfig["triggers"].items():
         params = mconfig.get("trigger_params", {}).get(trigger, {})
 
         store.addTrigger(
             name=trigger.__name__,
+            keys=keys,
             trigger=trigger,
             params=params,
         )
 
     # Start store
     store.start()
 
     return store
 
 
 def serve(
     mconfig: dict,
     host: str = "0.0.0.0",
-    port: int = 5000,
+    port: int = 8000,
     motion_logging_level: str = "INFO",
 ) -> None:
-    """Serve a Motion application.
+    """Serve a motion application.
 
     Args:
         mconfig (dict): The motion configuration.
         host (str, optional): The host to serve on. Defaults to "0.0.0.0".
-        port (int, optional): The port to serve on. Defaults to 5000.
+        port (int, optional): The port to serve on. Defaults to 8000.
         motion_logging_level (str, optional): The logging level for motion.
     """
     configureLogging(motion_logging_level)
-    store = init(mconfig, session_id=PRODUCTION_SESSION_ID)
+    store = init(mconfig, session_id="PRODUCTION")
     serve_store(store, host, port)
 
 
 def serve_store(store: Store, host: str, port: int) -> None:
+    # Log that the server is running
+    MOTION_HOME = os.environ.get("MOTION_HOME", os.path.expanduser("~/.cache/motion"))
+
+    os.makedirs(os.path.join(MOTION_HOME, "logs"), exist_ok=True)
+    with open(os.path.join(MOTION_HOME, "logs", store.name), "a") as f:
+        f.write(f"Server running at {host}:{port}")
+
     # Start fastapi server
-    app = create_fastapi_app(store)
+    app = create_app(store)
     uvicorn.run(app, host=host, port=port)
 
 
 def configureLogging(level: str) -> None:
     handler = logging.StreamHandler()
 
     formatter = colorlog.ColoredFormatter(
@@ -175,42 +128,39 @@
     logger = logging.getLogger("motion")
     logger.addHandler(handler)
     logger.setLevel(level)
 
 
 def test(
     mconfig: dict,
-    wait_for_triggers: typing.List[str] = [],
+    wait_for_triggers: list = [],
     disable_cron_triggers: bool = False,
     motion_logging_level: str = "WARNING",
     session_id: str = "",
 ) -> ClientConnection:
-    """Creates a test connection to a Motion application, defined by a mconfig. This will run the application
+    """Test a motion application. This will run the application
     and then shut it down.
 
     Args:
-        mconfig (dict): Config for the Motion application.
-        wait_for_triggers (typing.List[str], optional): List of cron-scheduled trigger names to wait for a first completion of. Typically used to wait for a first scrape of data.
-        disable_cron_triggers (bool, optional): Whether cron triggers should be disabled for this session (can speed up testing some non-cron triggers). Defaults to False.
-        motion_logging_level (str, optional): Logging level for motion. Use "INFO" if you want to see all trigger execution logs.
-        session_id (str, optional): Session ID to use for this connection. Defaults to a random UUID if empty.
-
-    Returns:
-        connection: A cannection to the Motion application.
+        mconfig (dict): Config for the motion application.
+        wait_for_triggers (list, optional): Defaults to [].
+        disable_cron_triggers (bool, optional): Defaults to False.
+        motion_logging_level (str, optional): Defaults to "WARNING".
+        session_id (str, optional): Defaults to "".
     """
     if wait_for_triggers and disable_cron_triggers:
         raise ValueError("Cannot wait for triggers if cron triggers are disabled.")
 
     configureLogging(motion_logging_level)
     store = init(
         mconfig,
         disable_cron_triggers=disable_cron_triggers,
         session_id=session_id,
     )
-    app = create_fastapi_app(store, testing=True)
+    app = create_app(store, testing=True)
 
     connection = ClientConnection(
         mconfig["application"]["name"],
         server=app,
         bearer_token=os.environ.get("MOTION_API_TOKEN", ""),
     )
     connection.addStore(store)
@@ -219,35 +169,40 @@
         connection.waitForTrigger(trigger)
 
     return connection
 
 
 def connect(
     name: str,
-    host: str = "0.0.0.0",
-    port: int = 5000,
-    wait_for_triggers: typing.List[str] = [],
+    wait_for_triggers: list = [],
     motion_api_token: str = "",
 ) -> ClientConnection:
-    """Connects to a Motion application that is already being served.
+    """Connect to a motion application.
 
     Args:
-        name (str): The name of the Motion application.
-        host (str, optional): The host of the Motion application. Defaults to localhost.
-        port (int, optional): The port of the Motion application. Defaults to 5000.
-        wait_for_triggers (typing.List[str], optional): List of cron-scheduled trigger names to wait for a first completion of. Typically used to wait for a first scrape of data.
-        motion_api_token (str, optional): API token set as the environment variable on the host serving the Motion application. If not provided as an argument, the token will be read from environment (possibly throwing an error if the environment doesn't have an API token defined).
+        name (str): The qname of the store.
+        wait_for_triggers (list, optional): Defaults to [].
+        motion_api_token (str, optional): Defaults to "". If not provided, the token will be read from environment.
 
     Returns:
-        connection: A connection to the Motion application.
+        Store: The motion store.
     """
     #  Check logs
+    MOTION_HOME = os.environ.get("MOTION_HOME", os.path.expanduser("~/.cache/motion"))
     MOTION_API_TOKEN = (
         motion_api_token if motion_api_token else os.environ.get("MOTION_API_TOKEN", "")
     )
 
-    server = "http://" + host + ":" + str(port)
+    os.makedirs(os.path.join(MOTION_HOME, "logs"), exist_ok=True)
+    try:
+        with open(os.path.join(MOTION_HOME, "logs", name)) as f:
+            server = f.read().split(" ")[-1]
+    except FileNotFoundError:
+        raise Exception(
+            f"Could not find a server for {name}. Please run `motion serve` first."
+        )
+
     connection = ClientConnection(name, server, bearer_token=MOTION_API_TOKEN)
     for trigger in wait_for_triggers:
         connection.waitForTrigger(trigger)
 
     return connection
```

### Comparing `motion_python-0.1.18/motion/schema.py` & `motion_python-0.1.2/motion/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+from __future__ import annotations
+
 import inspect
 import typing
 from collections import namedtuple
 from datetime import date, datetime
 from enum import Enum
 
 import numpy as np
 import pyarrow as pa
 from pydantic import BaseModel, Extra
 
+
+class MEnum(Enum):
+    @classmethod
+    def list(cls) -> list:
+        return [e.value for e in cls]
+
+
 Field = namedtuple("Field", ["name", "type_"])
 
 
 def type_to_name(t: type) -> str:
     return t.__name__.split(".")[-1].upper()
 
 
@@ -26,15 +35,15 @@
 }
 
 
 def get_arrow_type(t: type) -> pa.DataType:
     if t in TYPE_TO_PA_TYPE.keys():
         return TYPE_TO_PA_TYPE[t]
 
-    elif inspect.isclass(t) and issubclass(t, Enum):
+    elif inspect.isclass(t) and issubclass(t, MEnum):
         # return pa_ext.EnumType.from_enum(t)
         return pa.string()
 
     elif typing.get_origin(t) == list:
         sub_t = typing.get_args(t)[0]
         return pa.list_(get_arrow_type(sub_t))
 
@@ -57,14 +66,17 @@
     create_at: datetime
     session_id: str
 
     @classmethod
     def formatPaSchema(cls, relation: str) -> pa.Schema:
         """Formats a pyarrow schema for the given relation.
 
+        Args:
+            table_name (str): Name of relation.
+
         Returns:
             pa.Schema: Schema for table based on annotations.
         """
 
         fields = [Field(key, val) for key, val in cls.__annotations__.items()]
         user_defined_fields = [
             f
```

### Comparing `motion_python-0.1.18/motion/store.py` & `motion_python-0.1.2/motion/store.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+import inspect
 import os
 import threading
 import typing
 
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.dataset as ds
@@ -45,19 +48,19 @@
             self.table_columns,
             self.log_table,
         ) = self.loadFromCheckpoint_pa()
         if self.log_table is None:
             self.addLogTable_pa()
 
         # Set up triggers
-        self.triggers: typing.Dict[str, list[TriggerFn]] = {}
-        self.cron_triggers: typing.Dict[str, list[TriggerFn]] = {}
-        self.cron_threads: typing.Dict[str, CronThread] = {}
-        self.trigger_names: typing.Dict[str, list[str]] = {}
-        self.trigger_fns: typing.Dict[str, Trigger] = {}
+        self.triggers: dict[str, list[TriggerFn]] = {}
+        self.cron_triggers: dict[str, list[TriggerFn]] = {}
+        self.cron_threads: dict[str, CronThread] = {}
+        self.trigger_names: dict[str, list[str]] = {}
+        self.trigger_fns: dict[str, typing.Callable] = {}
 
     def __del__(self) -> None:
         self.stop(wait=False)
 
     @property
     def listening(self) -> bool:
         return self._listening
@@ -198,14 +201,17 @@
                 self.relations[name].schema.names,
                 self.relations[name].schema.types,
             ):
                 if old_name == "session_id":
                     continue
                 name_idx = pa_schema_names.index(old_name)
                 if not old_type.equals(pa_schema_types[name_idx]):
+                    print(old_name)
+                    print(old_type)
+                    print(pa_schema_types[name_idx])
                     logger.error(
                         f"relation {name} already exists with a different schema. Please clear the data store with `motion clear {self.name}` and try again."
                     )
 
         else:
             logger.info(f"Adding relation {name} with schema {pa_schema}")
             self.relations[name] = pa_schema.empty_table()
@@ -213,48 +219,65 @@
             self.table_columns[name] = self.relations[name].schema.names
             self.table_columns[name].remove("identifier")
             self.table_columns[name].remove("derived_id")
 
     def addTrigger(
         self,
         name: str,
-        trigger: typing.Type[Trigger],
-        params: typing.Dict[str, typing.Any] = {},
+        keys: list[str],
+        trigger: typing.Callable | type,
+        params: dict[str, typing.Any] = {},
     ) -> None:
         """Adds a trigger to the store.
 
         Args:
             name (str): Trigger name.
-            trigger (Trigger): Trigger class to execute when trigger is fired. Must implement the Trigger interface.
+            keys (typing.List[str]): Names of the keys to triger on. Formatted
+            as "relation.key" or cron expression. Trigger executes if there is
+            a addition to any of the keys, or on the cron schedule.
+            trigger (typing.Union[typing.Callable, type]): Function or class to
+            execute when the trigger is fired. If function, must take in the id
+            of the row that triggered the trigger, a reference to the element
+            that triggered it, and a reference to the store object (in this
+            order). If class, must implement the Transform interface.
             params (typing.Dict[str, typing.Any], optional): Parameters to pass
 
         Raises:
             ValueError: If there is already a trigger with the given name.
         """
         if name in self.trigger_names:
             logger.warning(f"Trigger {name} already exists. Doing nothing.")
             return
 
-        # Check that the class implements the Trigger interface
-        if not issubclass(trigger, Trigger):
-            raise ValueError(f"Trigger class must implement the Trigger interface.")
+        if inspect.isfunction(trigger):
+            # Check that the function signature is correct
+            if len(inspect.signature(trigger).parameters) != 2:
+                raise ValueError(
+                    f"Trigger function must take in 2 arguments: cursor and triggered_by."
+                )
 
-        # Retrieve keys
-        keys = trigger.getRouteKeys()
+        elif inspect.isclass(trigger):
+            # Check that the class implements the Transform interface
+            if not issubclass(trigger, Trigger):
+                raise ValueError(f"Trigger class must implement the Trigger interface.")
+
+        else:
+            raise ValueError(
+                f"Trigger {name} must be a function or class. Got {type(trigger)}."
+            )
 
         # Check that keys are valid
         all_possible_keys = [
             f"{ns}.{key}" for ns in self.table_columns for key in self.table_columns[ns]
         ]
         cron_key_exists = False
-        for full_key in keys:
-            _, key = full_key.split(".")
-            if full_key not in all_possible_keys and not croniter.is_valid(key):
+        for key in keys:
+            if key not in all_possible_keys and not croniter.is_valid(key):
                 raise ValueError(
-                    f"Trigger {name} has invalid key {full_key}. Valid keys are {all_possible_keys} or a cron expression. If your schemas have changed, you may need to clear your application by running `motion clear {self.name}`."
+                    f"Trigger {name} has invalid key {key}. Valid keys are {all_possible_keys} or a cron expression. If your schemas have changed, you may need to clear your application by running `motion clear {self.name}`."
                 )
 
             if croniter.is_valid(key):
                 if cron_key_exists:
                     raise ValueError(
                         f"Trigger {name} has more than one cron key. Only one cron key is allowed per trigger."
                     )
@@ -269,29 +292,30 @@
                 self.log_table["trigger_version"],
                 pc.equal(self.log_table["trigger_name"], name),
             )
         ).as_py()
 
         version = version if version is not None else 0
 
-        trigger_exec = trigger(
-            self.cursor(bypass_listening=True), name, version, params
+        trigger_exec = (
+            trigger(self.cursor(bypass_listening=True), name, version, params)
+            if inspect.isclass(trigger)
+            else trigger
         )
         self.trigger_fns[name] = trigger_exec
 
-        for full_key in keys:
-            _, key = full_key.split(".")
+        for key in keys:
             if croniter.is_valid(key):
-                self.cron_triggers[full_key] = self.cron_triggers.get(full_key, []) + [
-                    TriggerFn(name, trigger_exec)
+                self.cron_triggers[key] = self.cron_triggers.get(key, []) + [
+                    TriggerFn(name, trigger_exec, inspect.isclass(trigger))
                 ]
 
             else:
-                self.triggers[full_key] = self.triggers.get(full_key, []) + [
-                    TriggerFn(name, trigger_exec)
+                self.triggers[key] = self.triggers.get(key, []) + [
+                    TriggerFn(name, trigger_exec, inspect.isclass(trigger))
                 ]
 
     def deleteTrigger(self, name: str) -> None:
         """Delete a trigger from the store.
 
         Args:
             name (str): The name of the trigger.
@@ -300,20 +324,22 @@
             raise ValueError(f"Trigger {name} does not exist.")
 
         # Remove the trigger from the store
         keys = self.trigger_names[name]
         fn = self.trigger_fns[name]
         for key in keys:
             if croniter.is_valid(key):
-                self.cron_triggers[key].remove(TriggerFn(name, fn))
+                self.cron_triggers[key].remove(
+                    TriggerFn(name, fn, isinstance(fn, Trigger))
+                )
                 self.cron_threads[name].stop()
                 self.cron_threads[name].join()
 
             else:
-                self.triggers[key].remove(TriggerFn(name, fn))
+                self.triggers[key].remove(TriggerFn(name, fn, isinstance(fn, Trigger)))
 
         del self.trigger_names[name]
         del self.trigger_fns[name]
 
     def getTriggersForKey(self, relation: str, key: str) -> list[str]:
         """Get the list of triggers for a given key.
 
@@ -323,15 +349,15 @@
 
         Returns:
             typing.List[str]: The list of triggers for the given key.
         """
         names_and_fns = self.triggers.get(f"{relation}.{key}", [])
         return [t[0] for t in names_and_fns]
 
-    def getTriggersForAllKeys(self) -> typing.Dict[str, list[str]]:
+    def getTriggersForAllKeys(self) -> dict[str, list[str]]:
         """Get the list of triggers for all keys.
 
         Returns:
             typing.Dict[str, typing.List[str]]: The list of triggers for all keys.
         """
         return {
             k: self.getTriggersForKey(k.split(".")[0], k.split(".")[1])
@@ -341,25 +367,23 @@
     def start(self) -> None:
         """Start the store."""
         # Start cron triggers
         self._listening = True
         self.cron_threads = {}
 
         if not self.disable_cron_triggers:
-            for full_key, triggers in self.cron_triggers.items():
-                _, cron_expression = full_key.split(".")
+            for cron_expression, triggers in self.cron_triggers.items():
                 for trigger_fn in triggers:
                     e = threading.Event()
                     t = CronThread(
                         cron_expression,
                         self.cursor(wait_for_results=True),
                         trigger_fn,
                         self.checkpoint_pa,
                         e,
-                        self.session_id,
                     )
                     self.cron_threads[trigger_fn.name] = t
                     t.start()
 
         # Start a thread to checkpoint the store every 5 minutes
         self.checkpoint_thread = CheckpointThread(
             self.name, self.checkpoint_pa, self.checkpoint_interval
```

### Comparing `motion_python-0.1.18/motion/task.py` & `motion_python-0.1.2/motion/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
+from __future__ import annotations
+
 import threading
 import time
 import typing
 from datetime import datetime
 
 from croniter import croniter
 
 from motion.cursor import Cursor
-from motion.utils import PRODUCTION_SESSION_ID, TriggerElement, TriggerFn, logger
+from motion.utils import TriggerElement, TriggerFn, logger
 
 
 class CronThread(threading.Thread):
     """Thread that executes a task on cron schedule."""
 
     def __init__(
         self,
         cron_expression: str,
         cursor: Cursor,
         trigger_fn: TriggerFn,
         checkpoint_fn: typing.Callable,
         first_run_event: threading.Event,
-        session_id: str,
     ) -> None:
         threading.Thread.__init__(self)
         self.daemon = True
         self.cron_expression = cron_expression
         self.cur = cursor
         self.trigger_fn = trigger_fn
         self.checkpoint_fn = checkpoint_fn
         self.running = True
         self.first_run = True
         self.first_run_event = first_run_event
-        self.session_id = session_id
 
     def run(self) -> None:
         while self.running:
             next_time = croniter(self.cron_expression, datetime.now()).get_next(
                 datetime
             )
             delay = (next_time - datetime.now()).total_seconds()
@@ -43,41 +43,34 @@
             if not self.first_run:
                 if delay > 0:
                     time.sleep(delay)
                 else:
                     continue
 
             # Run trigger
-            trigger_context = TriggerElement(
-                relation="_cron",
+            triggered_by = TriggerElement(
+                relation="SCHEDULED",
                 identifier="SCHEDULED",
                 key=self.cron_expression,
                 value=None,
             )
 
             try:
                 self.cur.executeTrigger(
                     trigger=self.trigger_fn,
-                    trigger_context=trigger_context,
+                    triggered_by=triggered_by,
                 )
 
                 self.cur.waitForResults()
                 logger.info(
                     f"Finished waiting for background task {self.trigger_fn.name}."
                 )
             except Exception as e:
-                if self.session_id == PRODUCTION_SESSION_ID:
-                    logger.error(
-                        f"Error while running task {self.trigger_fn.name}: {e}"
-                    )
-                    continue
-                else:
-                    if self.first_run:
-                        self.first_run_event.set()
-                    raise e
+                logger.error(f"Error while running task {self.trigger_fn.name}: {e}")
+                continue
 
             if self.first_run:
                 self.first_run_event.set()
                 self.first_run = False
 
             self.checkpoint_fn()
             logger.info(f"Checkpointed store from task {self.trigger_fn.name}.")
```

### Comparing `motion_python-0.1.18/motion/trigger.py` & `motion_python-0.1.2/motion/trigger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import inspect
 import sys
 import threading
 import typing
 from abc import ABC, abstractmethod
 from queue import SimpleQueue
 
@@ -27,22 +29,15 @@
         except KeyError:
             raise KeyError(
                 f"Key `{key}` not found in {self.dict_type} for trigger {self.trigger_name}."
             )
 
 
 class Trigger(ABC):
-    def __init__(
-        self,
-        cursor: Cursor,
-        name: str,
-        version: int,
-        params: dict = {},
-        routes_only: bool = False,
-    ):
+    def __init__(self, cursor: Cursor, name: str, version: int, params: dict = {}):
         self.name = name
 
         # Validate number of arguments in each trigger and set up routes
         route_list = self.routes()
         if not isinstance(route_list, list):
             raise TypeError(
                 f"routes() of trigger {name} should return a list of motion.Route objects."
@@ -53,24 +48,15 @@
             if f"{r.relation}.{r.key}" in seen_keys:
                 raise ValueError(
                     f"Duplicate route {r.relation}.{r.key} in trigger {name}."
                 )
 
             r.validateTrigger(self)
             seen_keys.add(f"{r.relation}.{r.key}")
-
-        self.route_map = {}
-        for r in self.routes():
-            if r.relation != "":
-                self.route_map[f"{r.relation}.{r.key}"] = r
-            else:
-                self.route_map[f"_cron.{r.key}"] = r
-
-        if routes_only:
-            return
+        self.route_map = {f"{r.relation}.{r.key}": r for r in self.routes()}
 
         # Set up params dictionary
         self._params = CustomDict(self.name, "params", params)
 
         # Set up initial state
         if len(inspect.signature(self.setUp).parameters) != 1:
             raise ValueError(f"setUp() of trigger {name} should have 1 argument")
@@ -89,27 +75,21 @@
         self._fit_thread = threading.Thread(
             target=self.processFitQueue,
             daemon=True,
             name=f"{name}_fit_thread",
         )
         self._fit_thread.start()
 
-    @classmethod
-    def getRouteKeys(cls) -> list:
-        obj: Trigger = cls(None, "", 0, routes_only=True)  # type: ignore
-
-        return list(obj.route_map.keys())
-
     @abstractmethod
     def routes(self) -> list:
         pass
 
     @abstractmethod
     def setUp(self, cursor: Cursor) -> dict:
-        raise TypeError(f"Please implement setUp() for trigger {self.name}.")
+        pass
 
     @property
     def params(self) -> dict:
         return self._params
 
     @property
     def state(self) -> dict:
@@ -129,48 +109,42 @@
             self._version += 1
 
     def processFitQueue(self) -> None:
         while True:
             (
                 cursor,
                 trigger_name,
-                trigger_context,
-                infer_context,
+                triggered_by,
                 fit_event,
             ) = self._fit_queue.get()
 
             new_state = self.route_map[
-                f"{trigger_context.relation}.{trigger_context.key}"
-            ].fit(cursor, trigger_context, infer_context)
+                f"{triggered_by.relation}.{triggered_by.key}"
+            ].fit(cursor, triggered_by)
 
             if not isinstance(new_state, dict):
                 fit_event.set()
                 raise TypeError(
                     f"fit() of trigger {self.name} should return a dict of state updates."
                 )
 
             old_version = self.version
             self.update(new_state)
 
             logger.info(
-                f"Finished running trigger {trigger_name} for identifier {trigger_context.identifier} and key {trigger_context.key}."
+                f"Finished running trigger {trigger_name} for identifier {triggered_by.identifier} and key {triggered_by.key}."
             )
 
-            cursor.logTriggerExecution(
-                trigger_name, old_version, "fit", trigger_context
-            )
+            cursor.logTriggerExecution(trigger_name, old_version, "fit", triggered_by)
 
             fit_event.set()
 
     def fitWrapper(
         self,
         cursor: Cursor,
         trigger_name: str,
-        trigger_context: TriggerElement,
-        infer_context: typing.Any,
+        triggered_by: TriggerElement,
     ) -> threading.Event:
         fit_event = threading.Event()
-        self._fit_queue.put(
-            (cursor, trigger_name, trigger_context, infer_context, fit_event)
-        )
+        self._fit_queue.put((cursor, trigger_name, triggered_by, fit_event))
 
         return fit_event
```

### Comparing `motion_python-0.1.18/motion/utils.py` & `motion_python-0.1.2/motion/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from __future__ import annotations
+
 import copy
 import logging
 from collections import namedtuple
 
 logger = logging.getLogger(__name__)
 
 TriggerElement = namedtuple(
     "TriggerElement", ["relation", "identifier", "key", "value"]
 )
-TriggerFn = namedtuple("TriggerFn", ["name", "fn"])
-
-PRODUCTION_SESSION_ID = "PRODUCTION"
+TriggerFn = namedtuple("TriggerFn", ["name", "fn", "isTransform"])
 
 
 def update_params(mconfig: dict, params: dict) -> dict:
     """Updates the mconfig with the new trigger params.
 
     Args:
         mconfig (dict): config dict in mconfig.py
```

### Comparing `motion_python-0.1.18/pyproject.toml` & `motion_python-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.18"
+version = "0.1.2"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -30,35 +30,30 @@
 poetry-types = "^0.3.5"
 pytest = "^7.2.2"
 mypy = "^1.1.1"
 coverage = "^7.2.2"
 pre-commit = "^3.2.1"
 types-requests = "^2.28.11.16"
 types-croniter = "^1.3.2.7"
-mkdocs = "^1.4.2"
-mkdocs-terminal = "^4.2.0"
-mkdocs-material = "^9.1.5"
-mkdocstrings = {version="^0.20.0", extras = ["python"] }
-pytkdocs = "^0.16.1"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.mypy]
 files = "motion"
 mypy_path = "motion"
 warn_return_any = true
 warn_unused_configs = true
 disallow_untyped_defs = true
-exclude = ['motion/tests*']
+exclude = ['motion/exampleproj*', 'motion/tests*']
 ignore_missing_imports = true
 show_error_codes = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:"
-]
+]
```

