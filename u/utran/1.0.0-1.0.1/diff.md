# Comparing `tmp/utran-1.0.0-py3-none-any.whl.zip` & `tmp/utran-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 32038 bytes, number of entries: 23
--rw-rw-rw-  2.0 fat      119 b- defN 23-Apr-07 16:18 utran/__init__.py
+Zip file size: 32065 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat      119 b- defN 23-Apr-07 17:06 utran/__init__.py
 -rw-rw-rw-  2.0 fat       56 b- defN 23-Mar-29 06:22 utran/__main__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-29 13:25 utran/application.py
 -rw-rw-rw-  2.0 fat     9798 b- defN 23-Apr-07 11:51 utran/handler.py
 -rw-rw-rw-  2.0 fat      540 b- defN 23-Apr-02 16:36 utran/log.py
 -rw-rw-rw-  2.0 fat    15004 b- defN 23-Apr-06 07:10 utran/object.py
 -rw-rw-rw-  2.0 fat    15495 b- defN 23-Apr-07 11:17 utran/register.py
 -rw-rw-rw-  2.0 fat     1318 b- defN 23-Apr-04 18:39 utran/runner.py
 -rw-rw-rw-  2.0 fat     5937 b- defN 23-Apr-05 16:38 utran/utils.py
 -rw-rw-rw-  2.0 fat       86 b- defN 23-Apr-04 18:45 utran/client/__init__.py
--rw-rw-rw-  2.0 fat    21255 b- defN 23-Apr-07 11:41 utran/client/baseclient.py
+-rw-rw-rw-  2.0 fat    21430 b- defN 23-Apr-07 17:03 utran/client/baseclient.py
 -rw-rw-rw-  2.0 fat     7196 b- defN 23-Apr-07 10:22 utran/client/client.py
 -rw-rw-rw-  2.0 fat     1828 b- defN 23-Apr-06 17:14 utran/client/que.py
 -rw-rw-rw-  2.0 fat      163 b- defN 23-Mar-29 16:26 utran/server/__init__.py
 -rw-rw-rw-  2.0 fat     2668 b- defN 23-Apr-07 11:49 utran/server/baseServer.py
 -rw-rw-rw-  2.0 fat     4897 b- defN 23-Apr-07 11:49 utran/server/rpcServer.py
 -rw-rw-rw-  2.0 fat     5522 b- defN 23-Apr-05 17:27 utran/server/server.py
 -rw-rw-rw-  2.0 fat     5631 b- defN 23-Apr-07 11:48 utran/server/webserver.py
--rw-rw-rw-  2.0 fat     1062 b- defN 23-Apr-07 16:30 utran-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      403 b- defN 23-Apr-07 16:30 utran-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-07 16:30 utran-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-07 16:30 utran-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1749 b- defN 23-Apr-07 16:30 utran-1.0.0.dist-info/RECORD
-23 files, 100825 bytes uncompressed, 29258 bytes compressed:  71.0%
+-rw-rw-rw-  2.0 fat     1062 b- defN 23-Apr-07 17:36 utran-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      403 b- defN 23-Apr-07 17:36 utran-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-07 17:36 utran-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-07 17:36 utran-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1749 b- defN 23-Apr-07 17:36 utran-1.0.1.dist-info/RECORD
+23 files, 101000 bytes uncompressed, 29285 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: utran/server/server.py
 Comment: 
 
 Filename: utran/server/webserver.py
 Comment: 
 
-Filename: utran-1.0.0.dist-info/LICENSE
+Filename: utran-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: utran-1.0.0.dist-info/METADATA
+Filename: utran-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: utran-1.0.0.dist-info/WHEEL
+Filename: utran-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: utran-1.0.0.dist-info/top_level.txt
+Filename: utran-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: utran-1.0.0.dist-info/RECORD
+Filename: utran-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## utran/__init__.py

```diff
@@ -1,5 +1,5 @@
 from utran.runner import run
 from utran.server import Server
 from utran.client import Client
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

## utran/client/baseclient.py

```diff
@@ -55,14 +55,21 @@
             self._timeoutTask.cancel()
 
         if self._pingTask:
             self._pingTask.cancel()
 
         self._pingTask = self._loop.call_later(self._ping_freq,self.__ping)
 
+    
+    def stop(self):
+        """停止"""
+        self._timeoutTask.cancel()
+        self._pingTask.cancel()
+
+
     def getResponseDelay(self)->float:
         """# 获取响应延迟时间，
         需要在收到服务器Pong响应时调用
 
         Returns:
             返回毫秒数，保留小数点后三位        
         """
@@ -221,14 +228,15 @@
     async def _ping(self):
         """向服务器发送ping"""
         try:
             await self._send(None,heartbeat=True)
         except ConnectionResetError as e:
             logger.error('发送PING时服务器错误，'+str(e))
 
+            
 
 
     async def _ping_timeout(self):
         """服务器响应超时，该方法会被执行"""
         logger.error("服务器响应超时，启动断线重连..")
         self._reconnectTask = asyncio.create_task(self._reconnecting())
 
@@ -443,15 +451,15 @@
                 # 本地等待超时，非断线原因
                 logger.warning(f'Local call timeout ({timeout}s):{request.to_dict()}')
                 await self.exit()
                 raise e
                 
 
     async def __receive(self):
-        print("启动接收任务")
+        # print("启动接收任务")
         while True:
             chunk = await self._reader.read(1024)
             if not chunk:
                 raise ConnectionError('Connection closed by server')
             
             self._heartbeatTimer.alive()
             # 心跳检测                      
@@ -499,10 +507,11 @@
         self._reader = None
         self._writer = None
 
     async def exit(self):
         """# 退出程序
         调用退出时，并不会立即退出，需要等run方法中指定的`main`入口函数执行完毕才会退出。
         """
+        self._heartbeatTimer.stop()
         self._topics_handler = None
         self._exitEvent.set()
```

## Comparing `utran-1.0.0.dist-info/LICENSE` & `utran-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `utran-1.0.0.dist-info/RECORD` & `utran-1.0.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-utran/__init__.py,sha256=vKl93Dt9UA1kuXcbA55UtRX_hB45UPQFvuD0wJSAb3E,119
+utran/__init__.py,sha256=Hvsxj7jF1NU5R3U45NYaWhszKTV4SZC03vLOETWItVo,119
 utran/__main__.py,sha256=iJDh2-BPQSCB63Vdx_oTisjzUZHGfG1yGBz2T-EUusY,56
 utran/application.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 utran/handler.py,sha256=ua0pmYJhZeCtJ-uZYvHQGOwwyVFbwkWkjTaQHxphE7c,9798
 utran/log.py,sha256=yV3OegWgMX4rzzJcBnBzvX5sqh4WFgFDKFTvNUAzPzo,540
 utran/object.py,sha256=_DfgGmDnm5vwPapevBX5pwExQapoccLV-ABQTgOiwhM,15004
 utran/register.py,sha256=BFnO84Mm3qmGcpDORhvzySoUHSVmLZ07873QI8ypbd0,15495
 utran/runner.py,sha256=MRyK9lwkcGCgQSJhZtcm7scvrPhry1jiNyDDSxNKiN0,1318
 utran/utils.py,sha256=hfcFvn2Yl0uwn1w8wnFe7FjCqkJxFsCZnngyiu8OMWM,5937
 utran/client/__init__.py,sha256=Kav3KmWiPhdMDjV7poRDaAM_XxBqbngvrH9nVaQd5fk,86
-utran/client/baseclient.py,sha256=aMZJLf_SRhrFEfkbnyKAroLpoEqJP-H7IV0HOfVN5_Q,21255
+utran/client/baseclient.py,sha256=_F5IUfc3yHC-5jVe931o-yER8PfUGesM_TQCGAZES3c,21430
 utran/client/client.py,sha256=oGCx2GSbX1aJ_1sOZ-SAh6vh_0z8gJrRE6oHWUVNk_M,7196
 utran/client/que.py,sha256=cgUmJ3Pz_1j3B0LnC4gx8PGqLC__c4f20qQuQXuLt0A,1828
 utran/server/__init__.py,sha256=S-DRV8KWrwO_4yM3vJWEkDfcJCyjwSlSHaDDk8UGl_Q,163
 utran/server/baseServer.py,sha256=URBy6NkEnXotpgI9atdcuhPecC9EasYjJQ7hLcokYu0,2668
 utran/server/rpcServer.py,sha256=rc9ht889j3nSrBh5A0zqBalVsjdcO9957gWCI0biwNE,4897
 utran/server/server.py,sha256=HQgDNLcvM2fvzMGI_it2z5MKyAU0kzE1WfPf9iOl-Y8,5522
 utran/server/webserver.py,sha256=0xMQ65cyKJxlOkYNk2N-NtwKE7VDObU4n2MRHw4PFb8,5631
-utran-1.0.0.dist-info/LICENSE,sha256=7HB3vUUZ3KdogFm8d92SgQCXP7uuE2kNYWGajh3eo4Y,1062
-utran-1.0.0.dist-info/METADATA,sha256=MgE-Ta1mwbiK_f5XBQ1DWmvJjzqa3wuQbhEfp2QQWE0,403
-utran-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-utran-1.0.0.dist-info/top_level.txt,sha256=kcB7HqGkubiQlKanIo6oNBlCUQJOy5zc_HSvHiaoOA8,6
-utran-1.0.0.dist-info/RECORD,,
+utran-1.0.1.dist-info/LICENSE,sha256=7HB3vUUZ3KdogFm8d92SgQCXP7uuE2kNYWGajh3eo4Y,1062
+utran-1.0.1.dist-info/METADATA,sha256=yEXHnUgE-glQCAr3snNexKmljYQr0j7NOH7ga5ytU0c,403
+utran-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+utran-1.0.1.dist-info/top_level.txt,sha256=kcB7HqGkubiQlKanIo6oNBlCUQJOy5zc_HSvHiaoOA8,6
+utran-1.0.1.dist-info/RECORD,,
```

