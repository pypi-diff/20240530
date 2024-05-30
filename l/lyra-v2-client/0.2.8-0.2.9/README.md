# Comparing `tmp/lyra_v2_client-0.2.8.tar.gz` & `tmp/lyra_v2_client-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyra_v2_client-0.2.8.tar", max compression
+gzip compressed data, was "lyra_v2_client-0.2.9.tar", max compression
```

## Comparing `lyra_v2_client-0.2.8.tar` & `lyra_v2_client-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      814 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/README.md
--rw-r--r--   0        0        0       74 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/__init__.py
--rw-r--r--   0        0        0     1715 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/analyser.py
--rw-r--r--   0        0        0    10361 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/async_client.py
--rw-r--r--   0        0        0    29601 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/base_client.py
--rw-r--r--   0        0        0    13530 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/cli.py
--rw-r--r--   0        0        0     2806 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/constants.py
--rw-r--r--   0        0        0     1224 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/enums.py
--rw-r--r--   0        0        0      637 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/http_client.py
--rw-r--r--   0        0        0      677 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/lyra.py
--rw-r--r--   0        0        0      762 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/utils.py
--rw-r--r--   0        0        0      793 2024-04-14 10:24:48.090497 lyra_v2_client-0.2.8/lyra/ws_client.py
--rw-r--r--   0        0        0     1481 2024-04-14 10:24:48.098497 lyra_v2_client-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 lyra_v2_client-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      814 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/README.md
+-rw-r--r--   0        0        0       74 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/__init__.py
+-rw-r--r--   0        0        0     1715 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/analyser.py
+-rw-r--r--   0        0        0    11394 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/async_client.py
+-rw-r--r--   0        0        0    29601 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/base_client.py
+-rw-r--r--   0        0        0    13530 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/cli.py
+-rw-r--r--   0        0        0     2806 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/constants.py
+-rw-r--r--   0        0        0     1224 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/enums.py
+-rw-r--r--   0        0        0      637 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/http_client.py
+-rw-r--r--   0        0        0      677 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/lyra.py
+-rw-r--r--   0        0        0      762 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/utils.py
+-rw-r--r--   0        0        0      793 2024-05-30 08:50:49.283726 lyra_v2_client-0.2.9/lyra/ws_client.py
+-rw-r--r--   0        0        0     1388 2024-05-30 08:50:49.291726 lyra_v2_client-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 lyra_v2_client-0.2.9/PKG-INFO
```

### Comparing `lyra_v2_client-0.2.8/README.md` & `lyra_v2_client-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.8/lyra/analyser.py` & `lyra_v2_client-0.2.9/lyra/analyser.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.8/lyra/async_client.py` & `lyra_v2_client-0.2.9/lyra/async_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     We us the ws client to make async requests to the lyra ws API
     """
 
     current_subscriptions = {}
 
     listener = None
     subscribing = False
+    _ws = None
 
     def __init__(
         self,
         private_key: str = TEST_PRIVATE_KEY,
         env: Environment = Environment.TEST,
         logger=None,
         verbose=False,
@@ -49,21 +50,33 @@
         print(f"Signing address: {self.signer.address}")
         if wallet:
             print(f"Using wallet: {wallet}")
         self.subaccount_id = subaccount_id
         print(f"Using subaccount id: {self.subaccount_id}")
         self.message_queues = {}
         self.connecting = False
+        # we make sure to get the event loop
+
+    @property
+    async def ws(self):
+        if self._ws is None:
+            self._ws = await self.connect_ws()
+        if not self._ws.connected:
+            self._ws = await self.connect_ws()
+        return self._ws
 
     async def fetch_ticker(self, instrument_name: str):
         """
         Fetch the ticker for a symbol
         """
         id = str(int(time.time()))
         payload = {"instrument_name": instrument_name}
+        if not self.ws:
+            await self.connect_ws()
+
         self.ws.send(json.dumps({"method": "public/get_ticker", "params": payload, "id": id}))
 
         # we now wait for the response
         while True:
             response = self.ws.recv()
             response = json.loads(response)
             if response["id"] == id:
@@ -91,15 +104,15 @@
             await asyncio.sleep(0.01)
         return self.current_subscriptions[instrument_name]
 
     async def connect_ws(self):
         self.connecting = True
         session = aiohttp.ClientSession()
         ws = await session.ws_connect(self.contracts['WS_ADDRESS'])
-        self.ws = ws
+        self._ws = ws
         self.connecting = False
         return ws
 
     async def listen_for_messages(
         self,
     ):
         while True:
@@ -128,16 +141,16 @@
         self,
     ):
         login_request = {
             'method': 'public/login',
             'params': self.sign_authentication_header(),
             'id': str(int(time.time())),
         }
-        await self.ws.send_json(login_request)
-        async for data in self.ws:
+        await self._ws.send_json(login_request)
+        async for data in self._ws:
             message = json.loads(data.data)
             if message['id'] == login_request['id']:
                 if "result" not in message:
                     raise Exception(f"Unable to login {message}")
                 break
 
     def handle_message(self, subscription, data):
@@ -206,33 +219,49 @@
         self.ws.close()
 
     async def fetch_tickers(
         self,
         instrument_type: InstrumentType = InstrumentType.OPTION,
         currency: UnderlyingCurrency = UnderlyingCurrency.BTC,
     ):
+        if not self._ws:
+            await self.connect_ws()
         instruments = await self.fetch_instruments(instrument_type=instrument_type, currency=currency)
         instrument_names = [i['instrument_name'] for i in instruments]
         id_base = str(int(time.time()))
         ids_to_instrument_names = {
             f'{id_base}_{enumerate}': instrument_name for enumerate, instrument_name in enumerate(instrument_names)
         }
         for id, instrument_name in ids_to_instrument_names.items():
             payload = {"instrument_name": instrument_name}
-            self.ws.send(json.dumps({'method': 'public/get_ticker', 'params': payload, 'id': id}))
-            await asyncio.sleep(0.05)  # otherwise we get rate limited...
+            await self._ws.send_json({'method': 'public/get_ticker', 'params': payload, 'id': id})
+            await asyncio.sleep(0.1)  # otherwise we get rate limited...
         results = {}
         while ids_to_instrument_names:
-            message = json.loads(self.ws.recv())
+            message = await self._ws.receive()
+            if message is None:
+                continue
+            if 'error' in message:
+                raise Exception(f"Error fetching ticker {message}")
+            if message.type == aiohttp.WSMsgType.CLOSED:
+                # we try to reconnect
+                print(f"Erorr fetching ticker {message}...")
+                self._ws = await self.connect_ws()
+                return await self.fetch_tickers(instrument_type, currency)
+            message = json.loads(message.data)
             if message['id'] in ids_to_instrument_names:
-                results[message['result']['instrument_name']] = message['result']
+                try:
+                    results[message['result']['instrument_name']] = message['result']
+                except KeyError:
+                    print(f"Error fetching ticker {message}")
                 del ids_to_instrument_names[message['id']]
         return results
 
     async def get_collaterals(self):
+        breakpoint()
         return super().get_collaterals()
 
     async def get_positions(self, currency: UnderlyingCurrency = UnderlyingCurrency.BTC):
         return super().get_positions()
 
     async def get_open_orders(self, status, currency: UnderlyingCurrency = UnderlyingCurrency.BTC):
         return super().fetch_orders(
```

### Comparing `lyra_v2_client-0.2.8/lyra/base_client.py` & `lyra_v2_client-0.2.9/lyra/base_client.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.8/lyra/cli.py` & `lyra_v2_client-0.2.9/lyra/cli.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.8/lyra/constants.py` & `lyra_v2_client-0.2.9/lyra/constants.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.8/lyra/enums.py` & `lyra_v2_client-0.2.9/lyra/enums.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.8/lyra/http_client.py` & `lyra_v2_client-0.2.9/lyra/http_client.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.8/lyra/lyra.py` & `lyra_v2_client-0.2.9/lyra/lyra.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.8/lyra/utils.py` & `lyra_v2_client-0.2.9/lyra/utils.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.8/lyra/ws_client.py` & `lyra_v2_client-0.2.9/lyra/ws_client.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.8/pyproject.toml` & `lyra_v2_client-0.2.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [tool.poetry]
 name = "lyra-v2-client"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["8baller <8ball030@gmail.com>"]
 readme = "README.md"
 packages = [{include = "lyra"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<=3.11.7"
-requests = "^2.31.0"
-web3 = "^5"
+python = ">=3.8.1,<=3.11.9"
+requests = "^2"
+web3 = "^6"
 websocket-client = ">=0.32.0,<1"
 setuptools = "^68.2.2"
 rich-click = "^1.7.1"
 python-dotenv = ">=0.14.0,<0.18.0"
 pandas = "~1"
-websockets = "9.1"
-python-socketio = {extras = ["asyncio-client"], version = "^5.11.2"}
 
 
 [tool.poetry.scripts]
 lyra= "lyra.cli:cli"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `lyra_v2_client-0.2.8/PKG-INFO` & `lyra_v2_client-0.2.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: lyra-v2-client
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: 8baller
 Author-email: 8ball030@gmail.com
-Requires-Python: >=3.8.1,<=3.11.7
+Requires-Python: >=3.8.1,<=3.11.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=1,<2)
 Requires-Dist: python-dotenv (>=0.14.0,<0.18.0)
-Requires-Dist: python-socketio[asyncio-client] (>=5.11.2,<6.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2,<3)
 Requires-Dist: rich-click (>=1.7.1,<2.0.0)
 Requires-Dist: setuptools (>=68.2.2,<69.0.0)
-Requires-Dist: web3 (>=5,<6)
+Requires-Dist: web3 (>=6,<7)
 Requires-Dist: websocket-client (>=0.32.0,<1)
-Requires-Dist: websockets (==9.1)
 Description-Content-Type: text/markdown
 
 # Lyra V2 Python Client.
 
 This repo provides a unified interface for the Lyra V2 Exchange.
 
 Please checkout the [examples](./examples) directory for usage.
```

