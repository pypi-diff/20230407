# Comparing `tmp/pysignalr-0.1.2.tar.gz` & `tmp/pysignalr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysignalr-0.1.2.tar", max compression
+gzip compressed data, was "pysignalr-0.2.0.tar", max compression
```

## Comparing `pysignalr-0.1.2.tar` & `pysignalr-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1127 2022-05-24 12:04:31.198099 pysignalr-0.1.2/LICENSE
--rw-r--r--   0        0        0     1670 2022-05-24 12:04:31.198099 pysignalr-0.1.2/README.md
--rw-r--r--   0        0        0     1505 2022-05-24 12:04:31.198099 pysignalr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1985 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/__init__.py
--rw-r--r--   0        0        0     7722 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/client.py
--rw-r--r--   0        0        0      351 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/exceptions.py
--rw-r--r--   0        0        0     7244 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/messages.py
--rw-r--r--   0        0        0        0 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/protocol/__init__.py
--rw-r--r--   0        0        0     1014 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/protocol/abstract.py
--rw-r--r--   0        0        0     3738 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/protocol/json.py
--rw-r--r--   0        0        0     5369 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/protocol/messagepack.py
--rw-r--r--   0        0        0        0 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/py.typed
--rw-r--r--   0        0        0        0 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/transport/__init__.py
--rw-r--r--   0        0        0      545 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/transport/abstract.py
--rw-r--r--   0        0        0     7875 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/transport/websocket.py
--rw-r--r--   0        0        0     1254 2022-05-24 12:04:31.198099 pysignalr-0.1.2/src/pysignalr/utils.py
--rw-r--r--   0        0        0     2570 2022-05-24 12:05:28.612886 pysignalr-0.1.2/setup.py
--rw-r--r--   0        0        0     2456 2022-05-24 12:05:28.613314 pysignalr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1127 2023-04-07 18:24:13.314662 pysignalr-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2644 2023-04-07 18:24:13.314662 pysignalr-0.2.0/README.md
+-rw-r--r--   0        0        0     2275 2023-04-07 18:24:13.314662 pysignalr-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2202 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/__init__.py
+-rw-r--r--   0        0        0     7978 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/client.py
+-rw-r--r--   0        0        0      351 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/exceptions.py
+-rw-r--r--   0        0        0     7118 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/messages.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/protocol/__init__.py
+-rw-r--r--   0        0        0     1014 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/protocol/abstract.py
+-rw-r--r--   0        0        0     3738 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/protocol/json.py
+-rw-r--r--   0        0        0     5376 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/protocol/messagepack.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/py.typed
+-rw-r--r--   0        0        0        0 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/transport/__init__.py
+-rw-r--r--   0        0        0      545 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/transport/abstract.py
+-rw-r--r--   0        0        0     7870 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/transport/websocket.py
+-rw-r--r--   0        0        0     1282 2023-04-07 18:24:13.318662 pysignalr-0.2.0/src/pysignalr/utils.py
+-rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 pysignalr-0.2.0/setup.py
+-rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 pysignalr-0.2.0/PKG-INFO
```

### Comparing `pysignalr-0.1.2/LICENSE` & `pysignalr-0.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Lev Gorodetskiy, Baking Bad
+Copyright (c) 2021 Lev Gorodetskii, Baking Bad
 Copyright (c) 2019 Andrés Baamonde Lozano
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `pysignalr-0.1.2/src/pysignalr/__init__.py` & `pysignalr-0.2.0/src/pysignalr/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-__version__ = '0.1.2'
+import importlib.metadata
+
+__version__ = importlib.metadata.version('pysignalr')
 
 import asyncio
 import random
 from http import HTTPStatus
 from typing import AsyncIterator
 
 import websockets.legacy.client
@@ -11,48 +13,51 @@
 
 class NegotiationTimeout(Exception):
     """Connection URL generated during negotiation is no longer valid"""
 
     pass
 
 
-async def __aiter__(self) -> AsyncIterator[websockets.legacy.client.WebSocketClientProtocol]:
+async def __aiter__(
+    self: websockets.legacy.client.Connect,
+) -> AsyncIterator[websockets.legacy.client.WebSocketClientProtocol]:
     backoff_delay = self.BACKOFF_MIN
     while True:
         try:
             async with self as protocol:
                 yield protocol
 
+        # NOTE: The following block was added to the original code to handle expired connection URLs.
         except InvalidStatusCode as e:
             if e.status_code == HTTPStatus.NOT_FOUND:
                 raise NegotiationTimeout from e
         except asyncio.TimeoutError as e:
             raise NegotiationTimeout from e
 
         except Exception:
             # Add a random initial delay between 0 and 5 seconds.
             # See 7.2.3. Recovering from Abnormal Closure in RFC 6544.
             if backoff_delay == self.BACKOFF_MIN:
                 initial_delay = random.random() * self.BACKOFF_INITIAL
                 self.logger.info(
-                    "! connect failed; reconnecting in %.1f seconds",
+                    '! connect failed; reconnecting in %.1f seconds',
                     initial_delay,
                     exc_info=True,
                 )
                 await asyncio.sleep(initial_delay)
             else:
                 self.logger.info(
-                    "! connect failed again; retrying in %d seconds",
+                    '! connect failed again; retrying in %d seconds',
                     int(backoff_delay),
                     exc_info=True,
                 )
                 await asyncio.sleep(int(backoff_delay))
             # Increase delay with truncated exponential backoff.
             backoff_delay = backoff_delay * self.BACKOFF_FACTOR
             backoff_delay = min(backoff_delay, self.BACKOFF_MAX)
             continue
         else:
             # Connection succeeded - reset backoff delay
             backoff_delay = self.BACKOFF_MIN
 
 
-websockets.legacy.client.Connect.__aiter__ = __aiter__  # type: ignore
+websockets.legacy.client.Connect.__aiter__ = __aiter__  # type: ignore[method-assign]
```

### Comparing `pysignalr-0.1.2/src/pysignalr/client.py` & `pysignalr-0.2.0/src/pysignalr/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,36 +27,41 @@
 from pysignalr.protocol.json import JSONProtocol
 from pysignalr.transport.abstract import Transport
 from pysignalr.transport.websocket import DEFAULT_CONNECTION_TIMEOUT
 from pysignalr.transport.websocket import DEFAULT_MAX_SIZE
 from pysignalr.transport.websocket import DEFAULT_PING_INTERVAL
 from pysignalr.transport.websocket import WebsocketTransport
 
+EmptyCallback = Callable[[], Awaitable[None]]
+AnyCallback = Callable[[Any], Awaitable[None]]
+MessageCallback = Callable[[Message], Awaitable[None]]
+CompletionMessageCallback = Callable[[CompletionMessage], Awaitable[None]]
+
 
 class ClientStream:
     """Client to server streaming
     https://docs.microsoft.com/en-gb/aspnet/core/signalr/streaming?view=aspnetcore-5.0#client-to-server-streaming
     """
 
     def __init__(self, transport: Transport, target: str) -> None:
         self.transport: Transport = transport
         self.target: str = target
         self.invocation_id: str = str(uuid.uuid4())
 
     async def send(self, item: Any) -> None:
         """Send next item to the server"""
-        self.transport.send(StreamItemMessage(self.invocation_id, item))
+        await self.transport.send(StreamItemMessage(self.invocation_id, item))
 
     async def invoke(self) -> None:
         """Start streaming"""
-        self.transport.send(InvocationClientStreamMessage([self.invocation_id], self.target, []))
+        await self.transport.send(InvocationClientStreamMessage([self.invocation_id], self.target, []))
 
     async def complete(self) -> None:
         """Finish streaming"""
-        self.transport.send(CompletionClientStreamMessage(self.invocation_id))
+        await self.transport.send(CompletionClientStreamMessage(self.invocation_id))
 
 
 class SignalRClient:
     def __init__(
         self,
         url: str,
         protocol: Optional[Protocol] = None,
@@ -65,67 +70,69 @@
         connection_timeout: int = DEFAULT_CONNECTION_TIMEOUT,
         max_size: Optional[int] = DEFAULT_MAX_SIZE,
     ) -> None:
         self._url = url
         self._protocol = protocol or JSONProtocol()
         self._headers = headers or {}
 
-        self._message_handlers: DefaultDict[str, List[Optional[Callable]]] = defaultdict(list)
-        self._stream_handlers: Dict[str, Tuple[Optional[Callable], Optional[Callable], Optional[Callable]]] = {}
-        self._invocation_handlers: Dict[str, Optional[Callable]] = {}
+        self._message_handlers: DefaultDict[str, List[Optional[MessageCallback]]] = defaultdict(list)
+        self._stream_handlers: Dict[
+            str, Tuple[Optional[MessageCallback], Optional[MessageCallback], Optional[CompletionMessageCallback]]
+        ] = {}
+        self._invocation_handlers: Dict[str, Optional[MessageCallback]] = {}
 
         self._transport = WebsocketTransport(
             url=self._url,
             protocol=self._protocol,
             callback=self._on_message,
             headers=self._headers,
             ping_interval=ping_interval,
             connection_timeout=connection_timeout,
             max_size=max_size,
         )
-        self._error_callback: Optional[Callable[[CompletionMessage], Awaitable[None]]] = None
+        self._error_callback: Optional[CompletionMessageCallback] = None
 
     async def run(self) -> None:
         await self._transport.run()
 
-    def on(self, event: str, callback: Callable[..., Awaitable[None]]) -> None:
+    def on(self, event: str, callback: AnyCallback) -> None:
         """Register a callback on the specified event"""
         self._message_handlers[event].append(callback)
 
-    def on_open(self, callback: Callable[[], Awaitable[None]]) -> None:
+    def on_open(self, callback: EmptyCallback) -> None:
         """Register a callback on successful connection"""
         self._transport.on_open(callback)
 
-    def on_close(self, callback: Callable[[], Awaitable[None]]) -> None:
+    def on_close(self, callback: EmptyCallback) -> None:
         """Register a callback on connection close"""
         self._transport.on_close(callback)
 
-    def on_error(self, callback: Callable[[CompletionMessage], Awaitable[None]]) -> None:
+    def on_error(self, callback: CompletionMessageCallback) -> None:
         """Register a callback on error"""
         self._error_callback = callback
 
     async def send(
         self,
         method: str,
         arguments: List[Dict[str, Any]],
-        on_invocation: Optional[Callable[[CompletionMessage], Awaitable[None]]] = None,
+        on_invocation: Optional[MessageCallback] = None,
     ) -> None:
         """Send a message to the server"""
         invocation_id = str(uuid.uuid4())
         message = InvocationMessage(invocation_id, method, arguments, self._headers)
         self._invocation_handlers[invocation_id] = on_invocation
         await self._transport.send(message)
 
     async def stream(
         self,
         event: str,
         event_params: List[str],
-        on_next: Optional[Callable] = None,
-        on_complete: Optional[Callable] = None,
-        on_error: Optional[Callable] = None,
+        on_next: Optional[MessageCallback] = None,
+        on_complete: Optional[MessageCallback] = None,
+        on_error: Optional[CompletionMessageCallback] = None,
     ) -> None:
         """Invoke stream on the specified event"""
         invocation_id = str(uuid.uuid4())
         message = StreamInvocationMessage(invocation_id, event, event_params, self._headers)
         self._stream_handlers[invocation_id] = (on_next, on_complete, on_error)
         await self._transport.send(message)
 
@@ -135,15 +142,15 @@
         stream = ClientStream(self._transport, target)
         await stream.invoke()
         yield stream
         await stream.complete()
 
     async def _on_message(self, message: Message) -> None:
         # TODO: https://github.com/aspnet/SignalR/blob/master/clients/java/signalr/src/main/java/com/microsoft/signalr/InvocationBindingFailureMessage.java
-        if message.type == MessageType.invocation_binding_failure:  # type: ignore
+        if message.type == MessageType.invocation_binding_failure:  # type: ignore[attr-defined]
             raise ServerError(str(message))
 
         elif isinstance(message, PingMessage):
             pass
 
         elif isinstance(message, InvocationMessage):
             await self._on_invocation_message(message)
@@ -185,12 +192,12 @@
         callback, _, _ = self._stream_handlers[message.invocation_id]
         if callback:
             await callback(message.item)
 
     async def _on_cancel_invocation_message(self, message: CancelInvocationMessage) -> None:
         _, _, callback = self._stream_handlers[message.invocation_id]
         if callback:
-            await callback(message)
+            await callback(message)  # type: ignore[arg-type]
 
     async def _on_close_message(self, message: CloseMessage) -> None:
         if message.error:
             raise ServerError(message.error)
```

### Comparing `pysignalr-0.1.2/src/pysignalr/messages.py` & `pysignalr-0.2.0/src/pysignalr/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,41 +20,37 @@
 
 @dataclass
 class HandshakeResponseMessage(HandshakeMessage):
     error: Optional[str]
 
 
 class MessageType(IntEnum):
-    value: int
-
     _ = 9999
     invocation = 1
     stream_item = 2
     completion = 3
     stream_invocation = 4
     cancel_invocation = 5
     ping = 6
     close = 7
     invocation_binding_failure = -1
 
 
 @dataclass
 class Message:
     def __init_subclass__(cls, type_: MessageType) -> None:
-        # FIXME: https://github.com/samuelcolvin/pydantic/issues/288
-        cls.type = type_  # type: ignore
+        cls.type = type_  # type: ignore[attr-defined]
 
     def dump(self) -> Dict[str, Any]:
         data = self.__dict__
 
         invocation_id = data.pop('invocation_id', None)
         stream_ids = data.pop('stream_ids', None)
 
-        # FIXME: https://github.com/samuelcolvin/pydantic/issues/288
-        data['type'] = self.type  # type: ignore
+        data['type'] = self.type  # type: ignore[attr-defined]
         if invocation_id is not None:
             data['invocationId'] = invocation_id
         if stream_ids is not None:
             data['streamIds'] = stream_ids
 
         return data
```

### Comparing `pysignalr-0.1.2/src/pysignalr/protocol/abstract.py` & `pysignalr-0.2.0/src/pysignalr/protocol/abstract.py`

 * *Files identical despite different names*

### Comparing `pysignalr-0.1.2/src/pysignalr/protocol/json.py` & `pysignalr-0.2.0/src/pysignalr/protocol/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if isinstance(raw_message, bytes):
             raw_message = raw_message.decode()
 
         raw_messages = raw_message.split(self.record_separator)
         messages: List[Message] = []
 
         for item in raw_messages:
-            if item in ("", self.record_separator):
+            if item in ('', self.record_separator):
                 continue
 
             dict_message = json.loads(item)
             if dict_message:
                 messages.append(self.parse_message(dict_message))
 
         return messages
@@ -65,34 +65,34 @@
 
         # TODO: Cleanup
         messages = raw_message.split(self.record_separator)
         messages = list(filter(bool, messages))
         data = json.loads(messages[0])
         idx = raw_message.index(self.record_separator)
         return (
-            HandshakeResponseMessage(data.get("error", None)),
+            HandshakeResponseMessage(data.get('error', None)),
             self.decode(raw_message[idx + 1 :]) if len(messages) > 1 else [],
         )
 
     @staticmethod
     def parse_message(dict_message: Dict[str, Any]) -> Message:
         message_type = MessageType(dict_message.pop('type', 'close'))
 
         if message_type is MessageType.invocation:
-            dict_message["invocation_id"] = dict_message.pop("invocationId", None)
+            dict_message['invocation_id'] = dict_message.pop('invocationId', None)
             return InvocationMessage(**dict_message)
         elif message_type is MessageType.stream_item:
             return StreamItemMessage(**dict_message)
         elif message_type is MessageType.completion:
-            dict_message["invocation_id"] = dict_message.pop("invocationId", None)
+            dict_message['invocation_id'] = dict_message.pop('invocationId', None)
             return CompletionMessage(**dict_message)
         elif message_type is MessageType.stream_invocation:
             return StreamInvocationMessage(**dict_message)
         elif message_type is MessageType.cancel_invocation:
             return CancelInvocationMessage(**dict_message)
         elif message_type is MessageType.ping:
             return PingMessage()
         elif message_type is MessageType.close:
-            dict_message["allow_reconnect"] = dict_message.pop("allowReconnect", None)
+            dict_message['allow_reconnect'] = dict_message.pop('allowReconnect', None)
             return CloseMessage(**dict_message)
         else:
             raise NotImplementedError
```

### Comparing `pysignalr-0.1.2/src/pysignalr/protocol/messagepack.py` & `pysignalr-0.2.0/src/pysignalr/protocol/messagepack.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Iterable
 from typing import List
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from typing import cast
 
-import msgpack  # type: ignore
+import msgpack  # type: ignore[import]
 
 from pysignalr.messages import CancelInvocationMessage
 from pysignalr.messages import CloseMessage
 from pysignalr.messages import CompletionMessage
 from pysignalr.messages import HandshakeRequestMessage
 from pysignalr.messages import HandshakeResponseMessage
 from pysignalr.messages import InvocationClientStreamMessage
@@ -125,15 +125,14 @@
         else:
             raise NotImplementedError
 
     def _to_varint(self, value: int) -> bytes:
         buffer = b''
 
         while True:
-
             byte = value & 0x7F
             value >>= 7
 
             if value:
                 buffer += bytes((byte | 0x80,))
             else:
                 buffer += bytes((byte,))
```

### Comparing `pysignalr-0.1.2/src/pysignalr/transport/abstract.py` & `pysignalr-0.2.0/src/pysignalr/transport/abstract.py`

 * *Files identical despite different names*

### Comparing `pysignalr-0.1.2/src/pysignalr/transport/websocket.py` & `pysignalr-0.2.0/src/pysignalr/transport/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from typing import Union
 
 from aiohttp import ClientSession
 from aiohttp import ClientTimeout
 from aiohttp import ServerConnectionError
 from websockets.client import WebSocketClientProtocol
 from websockets.client import connect
+from websockets.connection import State
 from websockets.exceptions import ConnectionClosed
-from websockets.legacy.protocol import State
 
 import pysignalr.exceptions as exceptions
 from pysignalr import NegotiationTimeout
 from pysignalr.messages import CompletionMessage
 from pysignalr.messages import Message
 from pysignalr.messages import PingMessage
 from pysignalr.protocol.abstract import Protocol
```

### Comparing `pysignalr-0.1.2/src/pysignalr/utils.py` & `pysignalr-0.2.0/src/pysignalr/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import urllib.parse as parse
 from contextlib import suppress
 from typing import List
 
 http_schemas = ('http', 'https')
 websocket_schemas = ('ws', 'wss')
-http_to_ws = {k: v for k, v in zip(http_schemas, websocket_schemas)}
-ws_to_http = {k: v for k, v in zip(websocket_schemas, http_schemas)}
+http_to_ws = {k: v for k, v in zip(http_schemas, websocket_schemas)}  # noqa: C416
+ws_to_http = {k: v for k, v in zip(websocket_schemas, http_schemas)}  # noqa: C416
 
 
 def replace_scheme(url: str, ws: bool) -> str:
     scheme, netloc, path, query, fragment = parse.urlsplit(url)
 
     with suppress(KeyError):
         mapping = http_to_ws if ws else ws_to_http
```

