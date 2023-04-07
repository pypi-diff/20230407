# Comparing `tmp/interval_sdk-1.0.1.tar.gz` & `tmp/interval_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval_sdk-1.0.1.tar", max compression
+gzip compressed data, was "interval_sdk-1.0.2.tar", max compression
```

## Comparing `interval_sdk-1.0.1.tar` & `interval_sdk-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2968 2023-02-09 22:23:52.939868 interval_sdk-1.0.1/README.md
--rw-r--r--   0        0        0     1890 2023-04-03 21:01:39.156787 interval_sdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/classes/__init__.py
--rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/classes/action.py
--rw-r--r--   0        0        0     6840 2023-03-27 15:09:45.569464 interval_sdk-1.0.1/src/interval_sdk/classes/component.py
--rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/classes/interval_file.py
--rw-r--r--   0        0        0    57515 2023-03-01 18:41:20.060651 interval_sdk-1.0.1/src/interval_sdk/classes/io.py
--rw-r--r--   0        0        0     7892 2023-03-27 15:09:45.569464 interval_sdk-1.0.1/src/interval_sdk/classes/io_client.py
--rw-r--r--   0        0        0      348 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/classes/io_error.py
--rw-r--r--   0        0        0    29240 2023-03-27 15:09:45.572798 interval_sdk-1.0.1/src/interval_sdk/classes/io_promise.py
--rw-r--r--   0        0        0     7753 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/classes/isocket.py
--rw-r--r--   0        0        0     1755 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/classes/layout.py
--rw-r--r--   0        0        0     3458 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/classes/logger.py
--rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/classes/page.py
--rw-r--r--   0        0        0     6060 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/classes/rpc.py
--rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.0.1/src/interval_sdk/classes/transaction_loading_state.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/components/__init__.py
--rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/components/grid.py
--rw-r--r--   0        0        0     6090 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/components/table.py
--rw-r--r--   0        0        0      771 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/handlers.py
--rw-r--r--   0        0        0    13507 2023-04-03 20:55:58.909284 interval_sdk-1.0.1/src/interval_sdk/internal_rpc_schema.py
--rw-r--r--   0        0        0    27054 2023-03-27 15:09:45.572798 interval_sdk-1.0.1/src/interval_sdk/io_schema.py
--rw-r--r--   0        0        0    55173 2023-03-24 17:27:13.924931 interval_sdk-1.0.1/src/interval_sdk/main.py
--rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/superjson/__init__.py
--rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/superjson/main.py
--rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/superjson/plainer.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/superjson/tests/__init__.py
--rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/superjson/tests/node-only-types.js
--rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/superjson/tests/round-trip-superjson.js
--rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/superjson/tests/test_superjson.py
--rw-r--r--   0        0        0     5790 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/superjson/transformer.py
--rw-r--r--   0        0        0     1982 2023-02-09 22:23:52.943201 interval_sdk-1.0.1/src/interval_sdk/types.py
--rw-r--r--   0        0        0     6996 2023-03-02 17:09:53.415870 interval_sdk-1.0.1/src/interval_sdk/util.py
--rw-r--r--   0        0        0     4207 1970-01-01 00:00:00.000000 interval_sdk-1.0.1/setup.py
--rw-r--r--   0        0        0     4051 1970-01-01 00:00:00.000000 interval_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2968 2023-02-09 22:23:52.939868 interval_sdk-1.0.2/README.md
+-rw-r--r--   0        0        0     1890 2023-04-07 20:59:55.559775 interval_sdk-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/__init__.py
+-rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/action.py
+-rw-r--r--   0        0        0     7024 2023-04-07 20:59:44.056525 interval_sdk-1.0.2/src/interval_sdk/classes/component.py
+-rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/interval_file.py
+-rw-r--r--   0        0        0    57515 2023-03-01 18:41:20.060651 interval_sdk-1.0.2/src/interval_sdk/classes/io.py
+-rw-r--r--   0        0        0     8151 2023-04-07 20:59:44.056525 interval_sdk-1.0.2/src/interval_sdk/classes/io_client.py
+-rw-r--r--   0        0        0      348 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/io_error.py
+-rw-r--r--   0        0        0    35098 2023-04-07 20:59:44.056525 interval_sdk-1.0.2/src/interval_sdk/classes/io_promise.py
+-rw-r--r--   0        0        0     7766 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/classes/isocket.py
+-rw-r--r--   0        0        0     1290 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/classes/layout.py
+-rw-r--r--   0        0        0     3458 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/logger.py
+-rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/page.py
+-rw-r--r--   0        0        0     6040 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/classes/rpc.py
+-rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.0.2/src/interval_sdk/classes/transaction_loading_state.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/components/__init__.py
+-rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/components/grid.py
+-rw-r--r--   0        0        0     6090 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/components/table.py
+-rw-r--r--   0        0        0      771 2023-04-06 18:28:22.682795 interval_sdk-1.0.2/src/interval_sdk/handlers.py
+-rw-r--r--   0        0        0    13565 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/internal_rpc_schema.py
+-rw-r--r--   0        0        0    25561 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/io_schema.py
+-rw-r--r--   0        0        0    55271 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/main.py
+-rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/__init__.py
+-rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/main.py
+-rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/plainer.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/tests/__init__.py
+-rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/tests/node-only-types.js
+-rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/tests/round-trip-superjson.js
+-rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/tests/test_superjson.py
+-rw-r--r--   0        0        0     5790 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/transformer.py
+-rw-r--r--   0        0        0     4550 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/types.py
+-rw-r--r--   0        0        0     7193 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/util.py
+-rw-r--r--   0        0        0     4207 1970-01-01 00:00:00.000000 interval_sdk-1.0.2/setup.py
+-rw-r--r--   0        0        0     4051 1970-01-01 00:00:00.000000 interval_sdk-1.0.2/PKG-INFO
```

### Comparing `interval_sdk-1.0.1/README.md` & `interval_sdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/pyproject.toml` & `interval_sdk-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interval-sdk"
-version = "1.0.1"
+version = "1.0.2"
 description = "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more."
 authors = [
 	"Jacob Mischka <jacob@interval.com>",
 	"Ryan Coppolo <ryan@interval.com>",
 ]
 maintainers = [
 	"Jacob Mischka <jacob@interval.com>",
```

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/component.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from pydantic import parse_obj_as, ValidationError, BaseModel as PydanticBaseModel
 
 from interval_sdk import superjson
 
 from ..io_schema import (
     ChoiceButtonConfig,
+    ChoiceReturn,
     ComponentMultipleProps,
     MethodDef,
     MN,
     io_schema,
     ComponentRenderInfo,
     resolves_immediately,
 )
@@ -33,14 +34,18 @@
 
 IOPromiseValidator: TypeAlias = Callable[
     [Output_co], Union[Awaitable[Optional[str]], str, None]
 ]
 IOGroupPromiseValidator: TypeAlias = Callable[
     [Unpack[GroupOutput]], Union[Awaitable[Optional[str]], str, None]
 ]
+WithChoicesIOGroupPromiseValidator: TypeAlias = Callable[
+    [ChoiceReturn[Output_co]],
+    Union[Awaitable[Optional[str]], str, None],
+]
 
 StateModel_co = TypeVar(
     "StateModel_co", bound=Union[PydanticBaseModel, None], covariant=True
 )
 PropsModel_co = TypeVar(
     "PropsModel_co", bound=Union[PydanticBaseModel, None], covariant=True
 )
@@ -195,12 +200,12 @@
             multiple_props=self.instance.multiple_props,
         )
 
 
 ComponentRenderer: TypeAlias = Callable[
     [
         list[Component],
-        Optional[IOPromiseValidator],
+        Optional[WithChoicesIOGroupPromiseValidator[list[Any]]],
         Optional[list[ChoiceButtonConfig]],
     ],
     Awaitable[tuple[list[Any], Optional[str]]],
 ]
```

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/interval_file.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/interval_file.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/io.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/io.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/io_client.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/io_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from uuid import UUID, uuid4
 
 from typing_extensions import TypeAlias, TypeVar, Any, Awaitable
 
 from .. import superjson
 from ..io_schema import (
     ChoiceButtonConfig,
+    ChoiceReturn,
     MethodName,
     IORender,
     IOResponse,
 )
-from .component import Component, IOPromiseValidator
+from .component import Component, WithChoicesIOGroupPromiseValidator
 from .io_error import IOError
 from .io import IO
 from .logger import Logger
 
 
 MN = TypeVar("MN", bound=MethodName)
 
@@ -75,15 +76,15 @@
             self._logger.error(
                 "No response handler defined for input group key", input_group_key
             )
 
     async def render_components(
         self,
         components: list[Component],
-        group_validator: Optional[IOPromiseValidator] = None,
+        group_validator: Optional[WithChoicesIOGroupPromiseValidator] = None,
         choice_buttons: Optional[list[ChoiceButtonConfig]] = None,
     ) -> tuple[list[Any], Optional[str]]:
         if self._is_canceled:
             raise IOError("TRANSACTION_CLOSED")
 
         validation_error_message: Optional[str] = None
 
@@ -155,15 +156,20 @@
 
                 if group_validator is not None:
                     # we check that these are valid above, if any are invalid we wouldn't make it this far
                     parsed_values = [
                         components[i].parse_return_value(val)
                         for i, val in enumerate(response.values)
                     ]
-                    resp = group_validator(parsed_values)
+                    resp = group_validator(
+                        ChoiceReturn(
+                            choice=cast(str, response.choice),
+                            return_value=cast(tuple[Any], parsed_values),
+                        )
+                    )
                     validation_error_message = cast(
                         Optional[str], await resp if inspect.isawaitable(resp) else resp
                     )
 
                     if validation_error_message is not None:
                         task = loop.create_task(render())
                         task.add_done_callback(self._logger.handle_task_exceptions)
```

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/io_promise.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/io_promise.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .component import (
     Component,
     ComponentRenderer,
     GroupOutput,
     IOGroupPromiseValidator,
     Output_co,
     IOPromiseValidator,
+    WithChoicesIOGroupPromiseValidator,
 )
 from ..io_schema import (
     ButtonTheme,
     ComponentMultipleProps,
     input_schema,
     ChoiceReturn,
     ChoiceButton,
@@ -227,16 +228,22 @@
                 )
                 for item in choices
             ],
             get_value=self._value_getter,
         )
 
 
+WithChoicesOptionalIOPromiseSelf = TypeVar(
+    "WithChoicesOptionalIOPromiseSelf", bound="WithChoicesOptionalIOPromise"
+)
+
+
 class WithChoicesOptionalIOPromise(OptionalIOPromise[Input_MN_co, Output_co]):
     _choice_buttons: list[ChoiceButtonConfig]
+    _validator: Optional[WithChoicesIOGroupPromiseValidator[Optional[Output_co]]]
 
     def __init__(
         self,
         component: Component,
         renderer: ComponentRenderer,
         choices: list[ChoiceButtonConfig],
         get_value: Optional[Callable[[Any], Output_co]] = None,
@@ -249,15 +256,15 @@
             get_value=get_value,
         )
         self._choice_buttons = choices
 
     @override
     def __await__(self) -> Generator[Any, None, ChoiceReturn[Optional[Output_co]]]:
         return_values, choice = yield from self._renderer(
-            [self._component], None, self._choice_buttons
+            [self._component], self._handle_validation, self._choice_buttons
         ).__await__()
         return ChoiceReturn(
             choice=cast(str, choice),
             return_value=self._get_value(return_values[0]),
         )
 
     def _get_value(self, val: Any) -> Optional[Output_co]:
@@ -274,14 +281,42 @@
             ChoiceButtonConfig.parse_obj(
                 {"label": item, "value": item} if isinstance(item, str) else item
             )
             for item in choices
         ]
         return self
 
+    @override
+    def validate(
+        self: WithChoicesOptionalIOPromiseSelf,
+        validator: Optional[WithChoicesIOGroupPromiseValidator[Optional[Output_co]]],
+    ) -> WithChoicesOptionalIOPromiseSelf:
+        self._component.validator = None
+        self._validator = validator
+        return self
+
+    async def _handle_validation(self, ret: ChoiceReturn[list[Any]]):
+        if self._validator is None:
+            return None
+
+        value = (
+            self._get_value(ret.return_value[0])
+            if self._value_getter is not None
+            else ret.return_value[0]
+        )
+
+        validate_ret = self._validator(
+            ChoiceReturn(choice=ret.choice, return_value=value)
+        )
+
+        return cast(
+            Optional[str],
+            await validate_ret if inspect.isawaitable(validate_ret) else validate_ret,
+        )
+
 
 DefaultValue = TypeVar("DefaultValue")
 
 
 class MultipleableIOPromise(
     Generic[Multipleable_MN_co, Output_co, DefaultValue],
     InputIOPromise[Multipleable_MN_co, Output_co],
@@ -503,14 +538,15 @@
 WithChoicesInputIOPromiseSelf = TypeVar(
     "WithChoicesInputIOPromiseSelf", bound="WithChoicesInputIOPromise"
 )
 
 
 class WithChoicesInputIOPromise(InputIOPromise[Input_MN_co, Output_co]):
     _choice_buttons: list[ChoiceButtonConfig]
+    _validator: Optional[WithChoicesIOGroupPromiseValidator[Output_co]] = None
 
     def __init__(
         self,
         component: Component,
         renderer: ComponentRenderer,
         choices: list[ChoiceButtonConfig],
         get_value: Optional[Callable[[Any], Output_co]] = None,
@@ -521,15 +557,15 @@
             get_value=get_value,
         )
         self._choice_buttons = choices
 
     @override
     def __await__(self) -> Generator[Any, None, ChoiceReturn[Output_co]]:
         return_values, choice = yield from self._renderer(
-            [self._component], None, self._choice_buttons
+            [self._component], self._handle_validation, self._choice_buttons
         ).__await__()
         return ChoiceReturn(
             choice=cast(str, choice),
             return_value=self._get_value(return_values[0]),
         )
 
     @overload
@@ -564,19 +600,53 @@
                 choices=self._choice_buttons,
                 get_value=self._value_getter,
             )
             if optional
             else self
         )
 
+    @override
+    def validate(
+        self: WithChoicesInputIOPromiseSelf,
+        validator: Optional[WithChoicesIOGroupPromiseValidator[Output_co]],
+    ) -> WithChoicesInputIOPromiseSelf:
+        self._component.validator = None
+        self._validator = validator
+        return self
+
+    async def _handle_validation(self, ret: ChoiceReturn[list[Any]]):
+        if self._validator is None:
+            return None
+
+        value = (
+            self._get_value(ret.return_value[0])
+            if self._value_getter is not None
+            else ret.return_value[0]
+        )
+
+        validate_ret = self._validator(
+            ChoiceReturn(choice=ret.choice, return_value=value)
+        )
+
+        return cast(
+            Optional[str],
+            await validate_ret if inspect.isawaitable(validate_ret) else validate_ret,
+        )
+
+
+WithChoicesMultipleableIOPromiseSelf = TypeVar(
+    "WithChoicesMultipleableIOPromiseSelf", bound="WithChoicesMultipleableIOPromise"
+)
+
 
 class WithChoicesMultipleableIOPromise(
     MultipleableIOPromise[Multipleable_MN_co, Output_co, DefaultValue]
 ):
     _choice_buttons: list[ChoiceButtonConfig]
+    _validator: Optional[WithChoicesIOGroupPromiseValidator[Output_co]] = None
 
     def __init__(
         self,
         component: Component,
         renderer: ComponentRenderer,
         choices: list[ChoiceButtonConfig],
         get_value: Optional[Callable[[Any], Output_co]] = None,
@@ -587,15 +657,15 @@
             get_value=get_value,
         )
         self._choice_buttons = parse_obj_as(list[ChoiceButtonConfig], choices)
 
     @override
     def __await__(self) -> Generator[Any, None, ChoiceReturn[Output_co]]:
         return_values, choice = yield from self._renderer(
-            [self._component], None, self._choice_buttons
+            [self._component], self._handle_validation, self._choice_buttons
         ).__await__()
         return ChoiceReturn(
             choice=cast(str, choice),
             return_value=self._get_value(return_values[0]),
         )
 
     def multiple(self, *, default_value: Optional[Iterable[DefaultValue]] = None):
@@ -605,19 +675,53 @@
         ](
             component=multiple_io_promise._component,
             renderer=multiple_io_promise._renderer,
             get_value=self._value_getter,
             choices=self._choice_buttons,
         )
 
+    @override
+    def validate(
+        self: WithChoicesMultipleableIOPromiseSelf,
+        validator: Optional[WithChoicesIOGroupPromiseValidator[Output_co]],
+    ) -> WithChoicesMultipleableIOPromiseSelf:
+        self._component.validator = None
+        self._validator = validator
+        return self
+
+    async def _handle_validation(self, ret: ChoiceReturn[list[Any]]):
+        if self._validator is None:
+            return None
+
+        value = (
+            self._get_value(ret.return_value[0])
+            if self._value_getter is not None
+            else ret.return_value[0]
+        )
+
+        validate_ret = self._validator(
+            ChoiceReturn(choice=ret.choice, return_value=value)
+        )
+
+        return cast(
+            Optional[str],
+            await validate_ret if inspect.isawaitable(validate_ret) else validate_ret,
+        )
+
+
+WithChoicesMultipleIOPromiseSelf = TypeVar(
+    "WithChoicesMultipleIOPromiseSelf", bound="WithChoicesMultipleIOPromise"
+)
+
 
 class WithChoicesMultipleIOPromise(
     MultipleIOPromise[Multipleable_MN_co, Output_co, DefaultValue]
 ):
     _choice_buttons: list[ChoiceButtonConfig]
+    _validator: Optional[WithChoicesIOGroupPromiseValidator[list[Output_co]]] = None
 
     def __init__(
         self,
         component: Component,
         renderer: ComponentRenderer,
         choices: list[ChoiceButtonConfig],
         get_value: Optional[Callable[[Any], Output_co]] = None,
@@ -628,21 +732,49 @@
             get_value=get_value,
         )
         self._choice_buttons = choices
 
     @override
     def __await__(self) -> Generator[Any, None, ChoiceReturn[list[Output_co]]]:
         return_values, choice = yield from self._renderer(
-            [self._component], None, self._choice_buttons
+            [self._component], self._handle_validation, self._choice_buttons
         ).__await__()
         return ChoiceReturn(
             choice=cast(str, choice),
             return_value=self._get_value(return_values[0]),
         )
 
+    @override
+    def validate(
+        self: WithChoicesMultipleIOPromiseSelf,
+        validator: Optional[WithChoicesIOGroupPromiseValidator[list[Output_co]]],
+    ) -> WithChoicesMultipleIOPromiseSelf:
+        self._component.validator = None
+        self._validator = validator
+        return self
+
+    async def _handle_validation(self, ret: ChoiceReturn[list[Any]]):
+        if self._validator is None:
+            return None
+
+        value = (
+            self._get_value(ret.return_value[0])
+            if self._value_getter is not None
+            else ret.return_value[0]
+        )
+
+        validate_ret = self._validator(
+            ChoiceReturn(choice=ret.choice, return_value=value)
+        )
+
+        return cast(
+            Optional[str],
+            await validate_ret if inspect.isawaitable(validate_ret) else validate_ret,
+        )
+
 
 IOGroupPromiseSelf = TypeVar("IOGroupPromiseSelf", bound="IOGroupPromise")
 
 
 class KeyedIONamespace(Mapping):
     __items: dict[str, Any] = {}
 
@@ -724,30 +856,30 @@
                 tuple[Unpack[GroupOutput]],
                 [
                     self._io_promises[i]._get_value(val)
                     for (i, val) in enumerate(return_values)
                 ],
             )
 
-    async def _handle_validation(self, return_values: list[Any]) -> Optional[str]:
+    async def _handle_validation(self, ret: ChoiceReturn[list[Any]]) -> Optional[str]:
         if self._validator is None:
             return None
 
         if self._kw_io_promises is not None and len(self._kw_io_promises) > 0:
             io_promises = list(self._kw_io_promises.values())
             values = {
-                key: io_promises[index]._get_value(return_values[index])
+                key: io_promises[index]._get_value(ret.return_value[index])
                 for index, key in enumerate(self._kw_io_promises.keys())
             }
             ret = self._validator(**values)  # type: ignore
         else:
             io_promises = self._io_promises
             values = [
                 io_promises[index]._get_value(v)
-                for index, v in enumerate(return_values)
+                for index, v in enumerate(ret.return_value)
             ]
             ret = self._validator(*values)  # type: ignore
         return cast(Optional[str], await ret if inspect.isawaitable(ret) else ret)
 
     @overload
     def validate(
         self: "IOGroupPromise[KeyedIONamespace]",
@@ -798,23 +930,34 @@
             ],
         )
 
 
 class WithChoicesIOGroupPromise(Generic[Unpack[GroupOutput]]):
     _inner_promise: IOGroupPromise[Unpack[GroupOutput]]
     _choice_buttons: Optional[list[ChoiceButtonConfig]] = None
+    _validator: Optional[
+        WithChoicesIOGroupPromiseValidator[tuple[Unpack[GroupOutput]]]
+    ] = None
 
     def __init__(
         self,
         inner_promise: IOGroupPromise[Unpack[GroupOutput]],
         choices: list[ChoiceButtonConfig],
+        validator: "Optional[IOGroupPromiseValidator[Unpack[GroupOutput]]]" = None,
     ):
         self._inner_promise = inner_promise
         self._choice_buttons = choices
 
+        if validator is not None:
+
+            def new_validator(ret: ChoiceReturn[tuple[Unpack[GroupOutput]]]):
+                return validator(*ret.return_value)
+
+            self._validator = new_validator
+
     @overload
     def __await__(
         self: "WithChoicesIOGroupPromise[KeyedIONamespace]",
     ) -> Generator[Any, None, ChoiceReturn[KeyedIONamespace]]:
         """Fallback typing for calls with keyword arguments."""
         ...
 
@@ -834,29 +977,29 @@
     def __await__(self) -> Generator[Any, None, ChoiceReturn[Union[tuple[Unpack[GroupOutput]], KeyedIONamespace]]]:  # type: ignore
         if (
             self._inner_promise._kw_io_promises is not None
             and len(self._inner_promise._kw_io_promises) > 0
         ):
             return_values, choice = yield from self._inner_promise._renderer(
                 [p._component for p in self._inner_promise._kw_io_promises.values()],
-                self._inner_promise._handle_validation,
+                self._handle_validation,
                 self._choice_buttons,
             ).__await__()
             res_dict = {
                 key: return_values[i]
                 for i, key in enumerate(self._inner_promise._kw_io_promises.keys())
             }
             return ChoiceReturn(
                 choice=cast(str, choice),
                 return_value=KeyedIONamespace(**res_dict),
             )
         else:
             return_values, choice = yield from self._inner_promise._renderer(
                 [p._component for p in self._inner_promise._io_promises],
-                self._inner_promise._handle_validation,
+                self._handle_validation,
                 self._choice_buttons,
             ).__await__()
             return ChoiceReturn(
                 choice=cast(str, choice),
                 return_value=cast(
                     tuple[Unpack[GroupOutput]],
                     [
@@ -864,37 +1007,63 @@
                         for (i, val) in enumerate(return_values)
                     ],
                 ),
             )
 
     @overload
     def validate(
-        self: "IOGroupPromise[KeyedIONamespace]",
+        self: "WithChoicesIOGroupPromise[KeyedIONamespace]",
         validator: "Callable[..., Optional[Union[str, Awaitable[Optional[str]]]]]",
-    ) -> "IOGroupPromise[Unpack[GroupOutput]]":
+    ) -> "WithChoicesIOGroupPromise[Unpack[GroupOutput]]":
         ...
 
     @overload
     def validate(
-        self: "IOGroupPromise[Unpack[GroupOutput]]",
-        validator: "Optional[IOGroupPromiseValidator[Unpack[GroupOutput]]]",
-    ) -> "IOGroupPromise[Unpack[GroupOutput]]":
+        self: "WithChoicesIOGroupPromise[Unpack[GroupOutput]]",
+        validator: "Optional[WithChoicesIOGroupPromiseValidator[tuple[Unpack[GroupOutput]]]]",
+    ) -> "WithChoicesIOGroupPromise[Unpack[GroupOutput]]":
         ...
 
     def validate(  # type: ignore
         self: "WithChoicesIOGroupPromise[Unpack[GroupOutput]]",
-        validator: "Optional[IOGroupPromiseValidator[Unpack[GroupOutput]]]",
+        validator: "Optional[WithChoicesIOGroupPromiseValidator[tuple[Unpack[GroupOutput]]]]",
     ) -> "WithChoicesIOGroupPromise[Unpack[GroupOutput]]":
-        self._inner_promise._validator = validator
+        self._validator = validator
         return self
 
     def with_choices(
         self: "WithChoicesIOGroupPromise[Unpack[GroupOutput]]",
         choices: Iterable[Union[ChoiceButton, str]],
     ) -> "WithChoicesIOGroupPromise[Unpack[GroupOutput]]":
         self._choice_buttons = [
             ChoiceButtonConfig.parse_obj(
                 {"label": item, "value": item} if isinstance(item, str) else item
             )
             for item in choices
         ]
         return self
+
+    async def _handle_validation(self, ret: ChoiceReturn[list[Any]]) -> Optional[str]:
+        if self._validator is None:
+            return None
+
+        if (
+            self._inner_promise._kw_io_promises is not None
+            and len(self._inner_promise._kw_io_promises) > 0
+        ):
+            io_promises = list(self._inner_promise._kw_io_promises.values())
+            values = {
+                key: io_promises[index]._get_value(ret.return_value[index])
+                for index, key in enumerate(self._inner_promise._kw_io_promises.keys())
+            }
+            validate_ret = self._validator(ChoiceReturn(choice=ret.choice, return_value=values))  # type: ignore
+        else:
+            io_promises = self._inner_promise._io_promises
+            values = [
+                io_promises[index]._get_value(v)
+                for index, v in enumerate(ret.return_value)
+            ]
+            validate_ret = self._validator(ChoiceReturn(choice=ret.choice, return_value=values))  # type: ignore
+        return cast(
+            Optional[str],
+            await validate_ret if inspect.isawaitable(validate_ret) else validate_ret,
+        )
```

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/isocket.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/isocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         self, ws: websockets.client.WebSocketClientProtocol
     ) -> None:
 
         while True:
             try:
                 message = await self._out_queue.get()
                 try:
-                    await ws.send(message.json())
+                    await ws.send(message.json(by_alias=True))
                 except websockets.exceptions.ConnectionClosed as e:
                     await self._handle_close(e.code, e.reason)
                 except asyncio.exceptions.TimeoutError:
                     # No need to put back in queue, we'll try resending again
                     pass
                 except Exception as e:
                     self._logger.error("Error in producer handler", e)
```

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/layout.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/layout.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing_extensions import Literal, TypeAlias, Awaitable
 
 from pydantic import Field
 
 from ..classes.io_promise import DisplayIOPromise
 from ..types import BaseModel
-from ..io_schema import ButtonItem, ButtonItemModel, IORender, dump_io_render
+from ..io_schema import ButtonItem, ButtonItemModel, IORender
 from ..util import dump_snake_obj, json_loads_camel, snake_to_camel
 
 PageLayoutKey = Literal["title", "description", "children", "menuItems"]
 
 
 class PageError(BaseModel):
     layout_key: PageLayoutKey
@@ -33,29 +33,14 @@
     children: Optional[list[DisplayIOPromise]] = None
     menu_items: Optional[list[ButtonItem]] = None
 
 
 Layout: TypeAlias = BasicLayout
 
 
-def json_dumps_basic_layout_model(layout: dict[str, Any], *args, **kwargs) -> str:
-    obj = {}
-    for key, val in layout.items():
-        if key == "children":
-            obj[snake_to_camel(key)] = dump_io_render(val)
-        else:
-            obj[snake_to_camel(key)] = dump_snake_obj(val)
-
-    return json.dumps(obj, *args, **kwargs)
-
-
 class BasicLayoutModel(BaseModel):
     kind: Literal["BASIC"]
     title: Optional[str] = None
     description: Optional[str] = None
     children: Optional[IORender] = None
     menu_items: Optional[list[ButtonItemModel]] = None
     errors: list[PageError] = Field(default_factory=list)
-
-    class Config:
-        json_dumps = json_dumps_basic_layout_model
-        json_loads = json_loads_camel
```

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/logger.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/logger.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/page.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/page.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/rpc.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/rpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from typing_extensions import TypeVar, TypeAlias, Awaitable
 from pydantic import ValidationError, parse_obj_as
 
 from .logger import LogLevel, Logger
 from ..internal_rpc_schema import AnyRPCSchemaMethodName, DuplexMessage, RPCMethod
 from .isocket import ISocket
-from ..util import dict_keys_to_camel
 
 CallerSchemaMethodName = TypeVar("CallerSchemaMethodName", bound=AnyRPCSchemaMethodName)
 ResponderSchemaMethodName = TypeVar(
     "ResponderSchemaMethodName", bound=AnyRPCSchemaMethodName
 )
 
 id_count = 0
@@ -127,28 +126,29 @@
         message = DuplexMessage(
             id=parsed.id,
             method_name=method_name,
             data=return_value,
             kind="RESPONSE",
         )
         prepared_response_text = message.json()
+        print(prepared_response_text)
 
         try:
             await self._communicator.send(prepared_response_text)
         except Exception as err:
             self._logger.error("Failed sending response", message, err)
             self._logger.print_exception(err)
             raise err
 
     async def send(self, method_name: CallerSchemaMethodName, inputs: dict[str, Any]):
         id = generate_id()
 
         message = DuplexMessage(
             id=id,
-            data=dict_keys_to_camel(inputs),
+            data=inputs,
             method_name=method_name,
             kind="CALL",
         )
 
         loop = asyncio.get_running_loop()
         fut = loop.create_future()
         self._pending_calls[id] = fut
```

### Comparing `interval_sdk-1.0.1/src/interval_sdk/classes/transaction_loading_state.py` & `interval_sdk-1.0.2/src/interval_sdk/classes/transaction_loading_state.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/components/grid.py` & `interval_sdk-1.0.2/src/interval_sdk/components/grid.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/components/table.py` & `interval_sdk-1.0.2/src/interval_sdk/components/table.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/handlers.py` & `interval_sdk-1.0.2/src/interval_sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/internal_rpc_schema.py` & `interval_sdk-1.0.2/src/interval_sdk/internal_rpc_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from .classes.logger import Logger, SdkAlert
 from .classes.transaction_loading_state import LoadingState, TransactionLoadingState
 
-from .util import SerializableRecord, isoformat_datetime, json_dumps_strip_none
+from .util import (
+    SerializableRecord,
+    isoformat_datetime,
+)
 from .types import BaseModel, GenericModel
 
 
 ActionEnvironment: TypeAlias = Union[Literal["production", "development"], str]
 
 
 @base_dataclass
@@ -76,17 +79,14 @@
     method: NotRequired[Literal["EMAIL", "SLACK"]]
 
 
 class DeliveryInstructionModel(BaseModel):
     to: str
     method: Optional[Literal["EMAIL", "SLACK"]] = None
 
-    class Config:
-        json_dumps = json_dumps_strip_none
-
 
 class NotifyInputs(BaseModel):
     message: str
     transaction_id: Optional[str] = None
     title: Optional[str] = None
     idempotency_key: Optional[str] = None
     delivery_instructions: Optional[list[DeliveryInstructionModel]] = None
@@ -372,14 +372,20 @@
 @dataclass
 class ContextUser:
     email: str
     first_name: Optional[str] = None
     last_name: Optional[str] = None
 
 
+class ContextUserModel(BaseModel):
+    email: str
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+
+
 @dataclass
 class ActionInfo:
     slug: str
     url: str
 
 
 class ActionContext:
@@ -492,15 +498,15 @@
 
 
 class StartTransactionInputs(BaseModel):
     transaction_id: str
     display_resolves_immediately: bool = False
     action: ActionInfo
     environment: ActionEnvironment
-    user: ContextUser
+    user: ContextUserModel
     params: SerializableRecord
     params_meta: Optional[Any] = None
 
 
 class CloseTransactionInputs(BaseModel):
     transaction_id: str
```

### Comparing `interval_sdk-1.0.1/src/interval_sdk/io_schema.py` & `interval_sdk-1.0.2/src/interval_sdk/io_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Generic,
     TypeVar,
     Mapping,
     Type,
 )
 from datetime import date, time, datetime
 from uuid import UUID
-import io, json, sys
+import io, sys
 from typing_extensions import NotRequired, TypedDict, TypeAlias, override
 from pydantic import (
     BaseModel as PydanticBaseModel,
     Field,
     NonNegativeInt,
     PositiveFloat,
     PositiveInt,
@@ -33,21 +33,16 @@
 
 from .types import (
     BaseModel,
     GenericModel,
 )
 from .util import (
     ObjectLiteral,
-    dict_strip_none,
-    json_dumps_snake_strip_none,
-    json_loads_snake_strip_none,
-    snake_to_camel,
-    dict_keys_to_camel,
-    json_dumps_some_snake,
-    json_loads_some_snake,
+    json_dumps_strip_none,
+    json_loads_strip_none,
     Serializable,
     SerializableRecord,
 )
 
 # TODO: Try generating most of this with datamode-code-generator
 # https://github.com/koxudaxi/datamodel-code-generator/
 
@@ -106,16 +101,16 @@
     is_stateful: bool
     is_optional: bool
     is_multiple: bool
     validation_error_message: Optional[str] = None
     multiple_props: Optional[ComponentMultipleProps] = None
 
     class Config:
-        json_loads = json_loads_snake_strip_none
-        json_dumps = json_dumps_snake_strip_none
+        json_loads = json_loads_strip_none
+        json_dumps = json_dumps_strip_none
 
 
 TypeValue = Literal[
     "string",
     "string?",
     "number",
     "number?",
@@ -331,17 +326,14 @@
 
 class ActionResult(BaseModel):
     schema_version: Literal[0, 1] = 1
     status: Literal["SUCCESS", "FAILURE"]
     data: IOFunctionReturnModel
     meta: Optional[Any] = None
 
-    class Config:
-        json_dumps = json.dumps
-
 
 TableRowValuePrimitive: TypeAlias = Union[
     StrictInt, StrictFloat, StrictBool, date, datetime, None, str, Any
 ]
 
 SearchResultValuePrimitive: TypeAlias = Union[
     StrictInt, StrictFloat, StrictBool, date, datetime, None, str
@@ -954,73 +946,35 @@
 ) -> bool:
     if display_resolves_immediately and method_name.startswith("DISPLAY_"):
         return True
 
     return io_schema[method_name].immediate
 
 
-def dump_io_render(io_render: dict[str, Any]) -> dict[str, Any]:
-    obj = {}
-    for key, val in io_render.items():
-        if key == "to_render":
-            obj[snake_to_camel(key)] = [
-                dict_keys_to_camel(dict_strip_none(info)) for info in val
-            ]
-        elif key == "validation_error_message" and val is None:
-            pass
-        elif key == "continue_button":
-            if val is None:
-                continue
-            obj[snake_to_camel(key)] = dict_keys_to_camel(dict_strip_none(val))
-        elif key == "choice_buttons":
-            if val is None:
-                continue
-            obj[snake_to_camel(key)] = [
-                dict_keys_to_camel(dict_strip_none(info)) for info in val
-            ]
-        else:
-            obj[snake_to_camel(key)] = val
-
-    return obj
-
-
-def json_dumps_io_render(io_render: dict[str, Any], *args, **kwargs) -> str:
-    # we don't want to clobber any user-provided keys in props
-    return json.dumps(dump_io_render(io_render), *args, **kwargs)
-
-
 class IORender(BaseModel):
     id: UUID
     input_group_key: UUID
     to_render: list[ComponentRenderInfo]
     kind: Literal["RENDER"] = "RENDER"
     validation_error_message: Optional[str] = None
     choice_buttons: Optional[list[ChoiceButtonConfig]] = None
 
     class Config:
-        json_dumps = json_dumps_io_render
+        json_dumps = json_dumps_strip_none
 
 
-class IOResponse(PydanticBaseModel):
+class IOResponse(BaseModel):
     id: Union[UUID, Literal["UNKNOWN"]]
     input_group_key: Optional[Union[UUID, Literal["UNKNOWN"]]] = None
     transaction_id: str
     kind: Literal["RETURN", "SET_STATE", "CANCELED"]
     values: list[Any]
     values_meta: Optional[Any] = None
     choice: Optional[str] = None
 
-    class Config:
-        json_loads = json_loads_some_snake(
-            "transaction_id", "input_group_key", "values_meta"
-        )
-        json_dumps = json_dumps_some_snake(
-            "transaction_id", "input_group_key", "values_meta"
-        )
-
 
 def dump_method(method_name: MethodName) -> str:
     method_def = io_schema[method_name]
     props = method_def.props
     pieces = method_name.split("_", maxsplit=1)
     if len(pieces) > 1:
         [namespace, fn_name] = pieces
```

### Comparing `interval_sdk-1.0.1/src/interval_sdk/main.py` & `interval_sdk-1.0.2/src/interval_sdk/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from .internal_rpc_schema import (
     AccessControlDefinition,
     ActionContext,
     ActionDefinition,
     ActionEnvironment,
     ClosePageInputs,
     CloseTransactionInputs,
+    ContextUser,
     DeliveryInstruction,
     DeliveryInstructionModel,
     EnqueueActionInputs,
     EnqueueActionReturns,
     DequeueActionInputs,
     DequeueActionReturns,
     HostSchemaMethodName,
@@ -831,15 +832,15 @@
             handler = self._action_handlers.get(slug, None)
 
             if handler is None:
                 self._log.debug("No handler", slug)
                 return
 
             async def send(instruction: IORender):
-                io_call = instruction.json(exclude_unset=True)
+                io_call = instruction.json()
                 self._pending_io_calls[inputs.transaction_id] = io_call
                 await self._send(
                     "SEND_IO_CALL",
                     SendIOCallInputs(
                         transaction_id=inputs.transaction_id,
                         io_call=io_call,
                     ).dict(),
@@ -866,15 +867,15 @@
             params = inputs.params
             if params is not None and inputs.params_meta is not None:
                 params = superjson.deserialize(params, inputs.params_meta)
 
             action_ctx = ActionContext(
                 transaction_id=inputs.transaction_id,
                 logger=self._logger,
-                user=inputs.user,
+                user=ContextUser(**inputs.user.dict(by_alias=False)),
                 params=deserialize_dates(params),
                 environment=inputs.environment,
                 organization=self.organization,
                 action=inputs.action,
                 send_log=self._send_log,
                 send_redirect=self._send_redirect,
                 notify=self._notify,
@@ -1058,15 +1059,17 @@
                         page_layout.children = render_instruction
 
                     if menu_items is not None:
                         page_layout.menu_items = menu_items
 
                     for _ in range(MAX_PAGE_RETRIES):
                         try:
-                            serialized_page = page_layout.json(exclude_unset=True)
+                            serialized_page = page_layout.json(
+                                exclude_unset=True,
+                            )
                             self._pending_page_layouts[
                                 inputs.page_key
                             ] = serialized_page
                             await self._send(
                                 "SEND_PAGE",
                                 SendPageInputs(
                                     page_key=inputs.page_key,
```

### Comparing `interval_sdk-1.0.1/src/interval_sdk/superjson/main.py` & `interval_sdk-1.0.2/src/interval_sdk/superjson/main.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/superjson/plainer.py` & `interval_sdk-1.0.2/src/interval_sdk/superjson/plainer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/superjson/tests/test_superjson.py` & `interval_sdk-1.0.2/src/interval_sdk/superjson/tests/test_superjson.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/superjson/transformer.py` & `interval_sdk-1.0.2/src/interval_sdk/superjson/transformer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.1/src/interval_sdk/util.py` & `interval_sdk-1.0.2/src/interval_sdk/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,22 @@
         *args,
         **kwargs,
         object_pairs_hook=load_snake_pairs,
         parse_constant=deserialize_date,
     )
 
 
-def dump_snake_obj(obj: Any) -> Any:
+def dump_snake_obj(obj: Any, recurse=False) -> Any:
     if isinstance(obj, dict):
-        obj = {snake_to_camel(key): dump_snake_obj(val) for (key, val) in obj.items()}
+        obj = {
+            snake_to_camel(key): dump_snake_obj(val) if recurse else val
+            for (key, val) in obj.items()
+        }
     elif isinstance(obj, list):
-        obj = [dump_snake_obj(item) for item in obj]
+        obj = [dump_snake_obj(item) if recurse else item for item in obj]
     elif isinstance(obj, str):
         try:
             return datetime.fromisoformat(obj)
         except:
             pass
 
     return obj
@@ -141,35 +144,40 @@
     return json.dumps(dump_snake_obj(obj), *args, **kwargs)
 
 
 def json_dumps_some_snake(
     *keys_to_include: str,
 ):
     def json_dumps(obj: Mapping[str, Any], *args, **kwargs) -> str:
-        obj = {}
+        ret = {}
         for key, val in obj.items():
             if key in keys_to_include:
-                obj[key] = val
+                ret[snake_to_camel(key)] = val
             else:
-                obj[snake_to_camel(key)] = dump_snake_obj(val)
+                ret[key] = val
 
-        return json.dumps(obj, *args, **kwargs)
+        return json.dumps(ret, *args, **kwargs)
 
     return json_dumps
 
 
 def json_dumps_snake_strip_none(obj: Any, *args, **kwargs) -> str:
     return json.dumps(dict_keys_to_snake(dict_strip_none(obj)), *args, **kwargs)
 
 
 def json_loads_snake_strip_none(*args, **kwargs) -> Any:
     obj = json.loads(*args, **kwargs)
     return dict_keys_to_snake(dict_strip_none(obj))
 
 
+def json_loads_strip_none(*args, **kwargs) -> Any:
+    obj = json.loads(*args, **kwargs)
+    return dict_strip_none(obj)
+
+
 Deserializable: TypeAlias = Union[int, float, bool, None, str]
 DeserializableRecord: TypeAlias = Mapping[str, Deserializable]
 Serializable: TypeAlias = Union[bool, int, float, datetime, date, time, str, None]
 SerializableRecord: TypeAlias = Mapping[str, Serializable]
 
 ObjectLiteral: TypeAlias = Union[
     StrictInt, StrictFloat, StrictBool, datetime, date, time, None, str
```

### Comparing `interval_sdk-1.0.1/setup.py` & `interval_sdk-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['aiohttp>=3.8.1,<4.0.0',
  'pydantic>=1.9.0,<2.0.0',
  'typing-extensions>=4.4.0,<5.0.0',
  'websockets>=10.1,<11.0']
 
 setup_kwargs = {
     'name': 'interval-sdk',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.",
     'long_description': '# interval-sdk\n\n## Installation\n\nInstall using pip, (or your python package manager of choice):\n\n```\npip install interval-sdk\n```\n\n## API\n\n*Note:* Proper documentation is in progress!\n\nSee `src/demos/basic.py` and `src/tests` for a better overview, but in short:\n\n```python\nfrom interval_sdk import Interval, IO\n\n# Initialize Interval\ninterval = Interval("API_KEY")\n\n# Add an action using the function name as the slug\n@interval.action\nasync def hello_interval():\n    return {"hello": "from python!"}\n\n# Add an action using a custom slug (can contain hyphens) and additional configuration\n@interval.action(slug=\'echo-message\', unlisted=True)\nasync def echo_message(io: IO):\n    [message] = await io.group(io.input.text("Hello!", help_text="From python!"))\n\n    return {"message": message}\n\n\n# Synchronously listen, blocking forever\ninterval.listen()\n```\n\nTo not block, interval can also be run asynchronously using\n`interval.listen_async()`. You must provide your own event loop.\n\nThe task will complete as soon as connection to Interval completes, so you\nlikely want to run forever or run alongside another permanent task.\n\n```python\nimport asyncio\n\n# This is what synchronous `listen()` does under the hood\nloop = asyncio.get_event_loop()\ntask = loop.create_task(interval.listen_async())\ndef handle_done(task: asyncio.Task[None]):\n    try:\n        task.result()\n    except:\n        loop.stop()\n\ntask.add_done_callback(handle_done)\nloop.run_forever()\n```\n\nIf you are using `run_forever()`, you\'ll probably want to add signal handlers\nto close the loop gracefully on process termination:\n\n```python\nimport asyncio, signal\n\nloop = asyncio.get_event_loop()\ntask = loop.create_task(interval.listen_async())\ndef handle_done(task: asyncio.Task[None]):\n    try:\n        task.result()\n    except:\n        loop.stop()\n\ntask.add_done_callback(handle_done)\nfor sig in {signal.SIGINT, signal.SIGTERM}:\n    loop.add_signal_handler(sig, loop.stop)\nloop.run_forever()\n```\n\n\n## Contributing\n\nThis project uses [Poetry](https://python-poetry.org/) for dependency\nmanagement\n\n1. `poetry install` to install dependencies\n2. `poetry shell` to activate the virtual environment\n\nTasks are configured using [poethepoet](https://github.com/nat-n/poethepoet)\n(installed as a dev dependency).\n\n- `poe demo [demo_name]` to run a demo (`basic` by default if `demo_name` omitted)\n- `poe test` to run `pytest` (can also run `pytest` directly in virtual env)\n\nCode is formatted using [Black](https://github.com/psf/black). Please configure\nyour editor to format on save using Black, or run `poe format` to format the\ncode before committing changes.\n\n## Tests\n\n*Note:* Tests currently require a local instance of the Interval backend.\n\nTests use [pytest](https://docs.pytest.org/en/7.1.x/) and\n[playwright](https://playwright.dev/python/).\n\nCurrently assumes the `test-runner@interval.com` user exists already.\nRun `yarn test` in the `web` directory at least once to create it before\nrunning these.\n',
     'author': 'Jacob Mischka',
     'author_email': 'jacob@interval.com',
     'maintainer': 'Jacob Mischka',
     'maintainer_email': 'jacob@interval.com',
     'url': 'https://interval.com',
```

### Comparing `interval_sdk-1.0.1/PKG-INFO` & `interval_sdk-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interval-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.
 Home-page: https://interval.com
 Keywords: internal tool,app,ui,ui builder
 Author: Jacob Mischka
 Author-email: jacob@interval.com
 Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com
```

