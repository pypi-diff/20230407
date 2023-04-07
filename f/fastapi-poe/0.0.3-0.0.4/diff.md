# Comparing `tmp/fastapi_poe-0.0.3.tar.gz` & `tmp/fastapi_poe-0.0.4.tar.gz`

## Comparing `fastapi_poe-0.0.3.tar` & `fastapi_poe-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_poe-0.0.3/src/fastapi_poe/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fastapi_poe-0.0.3/src/fastapi_poe/__main__.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 fastapi_poe-0.0.3/src/fastapi_poe/base.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 fastapi_poe-0.0.3/src/fastapi_poe/types.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 fastapi_poe-0.0.3/src/fastapi_poe/samples/catbot.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi_poe-0.0.3/src/fastapi_poe/samples/echo.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fastapi_poe-0.0.3/.gitignore
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 fastapi_poe-0.0.3/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastapi_poe-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fastapi_poe-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_poe-0.0.4/src/fastapi_poe/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fastapi_poe-0.0.4/src/fastapi_poe/__main__.py
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 fastapi_poe-0.0.4/src/fastapi_poe/base.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fastapi_poe-0.0.4/src/fastapi_poe/types.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 fastapi_poe-0.0.4/src/fastapi_poe/samples/catbot.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi_poe-0.0.4/src/fastapi_poe/samples/echo.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastapi_poe-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 fastapi_poe-0.0.4/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastapi_poe-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 fastapi_poe-0.0.4/PKG-INFO
```

### Comparing `fastapi_poe-0.0.3/src/fastapi_poe/types.py` & `fastapi_poe-0.0.4/src/fastapi_poe/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,25 +23,14 @@
     content_type: ContentType
     timestamp: int
     message_id: str
     message_type: Optional[str]
     feedback: List[MessageFeedback]
 
 
-class RawRequest(BaseModel):
-    """Raw request from Poe"""
-
-    version: str
-    type: str
-    conversation_id: str
-    user_id: str
-    message_id: str
-    query: List[ProtocolMessage]
-
-
 class BaseRequest(BaseModel):
     """Common data for all requests."""
 
     version: str
     type: Literal["query", "settings", "report_feedback", "report_error"]
```

### Comparing `fastapi_poe-0.0.3/src/fastapi_poe/samples/catbot.py` & `fastapi_poe-0.0.4/src/fastapi_poe/samples/catbot.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,15 +28,18 @@
     async def get_response(self, query: QueryRequest) -> AsyncIterable[ServerSentEvent]:
         """Return an async iterator of events to send to the user."""
         last_message = query.query[-1].content.lower()
         content_type: ContentType = (
             "text/plain" if "plain" in last_message else "text/markdown"
         )
         yield self.meta_event(
-            content_type=content_type, linkify=True, refetch_settings=False
+            content_type=content_type,
+            linkify=True,
+            refetch_settings=False,
+            suggested_replies="dog" not in last_message,
         )
         if "markdown" in last_message:
             yield self.text_event("# Heading 1\n\n")
             yield self.text_event("*Bold text* ")
             yield self.text_event("**More bold text**\n")
             yield self.text_event("\n")
             yield self.text_event("A list:\n")
@@ -70,14 +73,18 @@
         elif "cube" in last_message:
             yield self.error_event(
                 "Cube snacks are even less tasty.", allow_retry=False
             )
         elif "scratch" in last_message:
             # Note this is illegal according to the protocol
             yield ServerSentEvent(event="purr", data=json.dumps({"text": "purr"}))
+        elif "count" in last_message:
+            for i in range(1, 11):
+                yield self.replace_response_event(str(i))
+                await asyncio.sleep(1)
         else:
             yield self.text_event("zzz")
 
     async def on_feedback(self, feedback: ReportFeedbackRequest) -> None:
         """Called when we receive user feedback such as likes."""
         print(
             f"User {feedback.user_id} gave feedback on {feedback.conversation_id}"
```

### Comparing `fastapi_poe-0.0.3/src/fastapi_poe/samples/echo.py` & `fastapi_poe-0.0.4/src/fastapi_poe/samples/echo.py`

 * *Files identical despite different names*

### Comparing `fastapi_poe-0.0.3/pyproject.toml` & `fastapi_poe-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_poe"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Lida Li", email="lli@quora.com" },
 ]
 description = "A demonstration of the Poe protocol using FastAPI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `fastapi_poe-0.0.3/PKG-INFO` & `fastapi_poe-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_poe
-Version: 0.0.3
+Version: 0.0.4
 Summary: A demonstration of the Poe protocol using FastAPI
 Project-URL: Homepage, https://github.com/quora/poe-protocol
 Author-email: Lida Li <lli@quora.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -39,9 +39,22 @@
         last_message = query.query[-1].content
         yield self.text_event(last_message)
 
 if __name__ == "__main__":
     run(EchoHandler())
 ```
 
+## Enable authentication
+
+Poe servers send requests containing Authorization HTTP header in the format "Bearer
+<api_key>," where api_key is the API key configured in the bot settings. \
+
+To validate the requests are from Poe Servers, you can either set the environment
+variable POE_API_KEY or pass the parameter api_key in the run function like:
+
+```python
+if __name__ == "__main__":
+    run(EchoHandler(), api_key=<key>)
+```
+
 For a more advanced example that exercises more of the Poe protocol, see
 [Catbot](./src/fastapi_poe/samples/catbot.py).
```

