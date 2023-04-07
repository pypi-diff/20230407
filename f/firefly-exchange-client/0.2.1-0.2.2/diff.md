# Comparing `tmp/firefly_exchange_client-0.2.1.tar.gz` & `tmp/firefly_exchange_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefly_exchange_client-0.2.1.tar", last modified: Mon Apr  3 19:30:51 2023, max compression
+gzip compressed data, was "firefly_exchange_client-0.2.2.tar", last modified: Fri Apr  7 20:13:11 2023, max compression
```

## Comparing `firefly_exchange_client-0.2.1.tar` & `firefly_exchange_client-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:30:51.438260 firefly_exchange_client-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-03 19:30:51.438260 firefly_exchange_client-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 19:30:51.438260 firefly_exchange_client-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:30:51.434260 firefly_exchange_client-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:30:51.438260 firefly_exchange_client-0.2.1/src/firefly_exchange_client/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    32123 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/contract_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/onboarding_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/order_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/socket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-03 19:30:34.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:30:51.438260 firefly_exchange_client-0.2.1/src/firefly_exchange_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-03 19:30:51.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-03 19:30:51.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 19:30:51.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-03 19:30:51.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-03 19:30:51.000000 firefly_exchange_client-0.2.1/src/firefly_exchange_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:13:11.053288 firefly_exchange_client-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-07 20:13:11.053288 firefly_exchange_client-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:13:11.053288 firefly_exchange_client-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:13:11.049288 firefly_exchange_client-0.2.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:13:11.049288 firefly_exchange_client-0.2.2/src/firefly_exchange_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32136 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/contract_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/onboarding_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/order_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/socket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:13:11.053288 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-07 20:13:11.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-07 20:13:11.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:13:11.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-07 20:13:11.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 20:13:11.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/top_level.txt
```

### Comparing `firefly_exchange_client-0.2.1/LICENSE` & `firefly_exchange_client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/PKG-INFO` & `firefly_exchange_client-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly_exchange_client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.2.1/README.md` & `firefly_exchange_client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/pyproject.toml` & `firefly_exchange_client-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "firefly_exchange_client"
-version = "0.2.1"
+version = "0.2.2"
 description = "Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["firefly", "exchange", "decentralized", "perpetuals", "blockchain"]
 dependencies = [
   'web3 ~= 5.31.3',
   'requests ~= 2.28.1',
```

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/api_service.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/api_service.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/client.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -702,15 +702,15 @@
         """
             Returns a list of orders.
             Inputs:
                 - params(GetOrderRequest): params required to query orders (e.g. symbol,statuses) 
             Returns:
                 - list: a list of orders 
         """
-        params = extract_enums(params,["symbol","statuses"])
+        params = extract_enums(params,["symbol","statuses", "orderType"])
 
         return await self.apis.get(
             SERVICE_URLS["USER"]["ORDERS"],
             params,
             True
         )
```

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/constants.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/constants.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/contract_abis.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/contract_abis.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/contracts.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/contracts.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/enumerations.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/enumerations.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/interfaces.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,15 +130,18 @@
   endTime: int
   pageSize: int
   pageNumber: int
   type: ORDER_TYPE
   parentAddress: str # (optional) should be provided by sub account
 
 class GetOrderRequest(GetTransactionHistoryRequest):
-  statuses:List[ORDER_STATUS] # status of orders to be fetched
+  statuses:List[ORDER_STATUS] # (optional) status of orders to be fetched
+  orderId: int #(optional) the id of order to be fetched
+  orderType: List[ORDER_TYPE]; # (optional) type of order Limit/Market
+  orderHashes: List[str] # (optional) hashes of order to be fetched
   parentAddress : str # (optional) should be provided by sub accounts
 
 class GetFundingHistoryRequest(TypedDict):
   symbol: MARKET_SYMBOLS  # will fetch orders of provided market
   pageSize: int  # will get only provided number of orders must be <= 50
   cursor: int  # will fetch particular page records. A single page contains 50 records.
   parentAddress: str # (optional) should be provided by a sub account
```

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/onboarding_signer.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/onboarding_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/order_signer.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/order_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/signer.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/socket_manager.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/socket_manager.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/sockets.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/sockets.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/utilities.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/utilities.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client/websocket_client.py` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client/websocket_client.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client.egg-info/PKG-INFO` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly-exchange-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.2.1/src/firefly_exchange_client.egg-info/SOURCES.txt` & `firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

