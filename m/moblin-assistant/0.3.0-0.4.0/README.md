# Comparing `tmp/moblin_assistant-0.3.0.tar.gz` & `tmp/moblin_assistant-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moblin_assistant-0.3.0.tar", last modified: Sat May 25 17:40:10 2024, max compression
+gzip compressed data, was "moblin_assistant-0.4.0.tar", last modified: Thu May 30 03:54:26 2024, max compression
```

## Comparing `moblin_assistant-0.3.0.tar` & `moblin_assistant-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:40:10.427604 moblin_assistant-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-25 17:40:06.000000 moblin_assistant-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-25 17:40:10.427604 moblin_assistant-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-25 17:40:06.000000 moblin_assistant-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:40:10.427604 moblin_assistant-0.3.0/moblin_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-25 17:40:06.000000 moblin_assistant-0.3.0/moblin_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 17:40:10.427604 moblin_assistant-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-05-25 17:40:06.000000 moblin_assistant-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:54:26.084087 moblin_assistant-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-30 03:54:21.000000 moblin_assistant-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-30 03:54:26.084087 moblin_assistant-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-30 03:54:21.000000 moblin_assistant-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:54:26.084087 moblin_assistant-0.4.0/moblin_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-30 03:54:26.000000 moblin_assistant-0.4.0/moblin_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-30 03:54:26.000000 moblin_assistant-0.4.0/moblin_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:54:26.000000 moblin_assistant-0.4.0/moblin_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 03:54:26.000000 moblin_assistant-0.4.0/moblin_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 03:54:26.000000 moblin_assistant-0.4.0/moblin_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 03:54:26.000000 moblin_assistant-0.4.0/moblin_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-30 03:54:21.000000 moblin_assistant-0.4.0/moblin_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:54:26.084087 moblin_assistant-0.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-05-30 03:54:21.000000 moblin_assistant-0.4.0/setup.py
```

### Comparing `moblin_assistant-0.3.0/LICENSE` & `moblin_assistant-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moblin_assistant-0.3.0/PKG-INFO` & `moblin_assistant-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moblin_assistant
-Version: 0.3.0
+Version: 0.4.0
 Summary: Moblin remote control assistant
 Home-page: https://github.com/eerimoq/moblin_assistant
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -12,19 +12,15 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: websockets
 
 About
 =====
 
-Mangling of various file formats that conveys binary information
-(Motorola S-Record, Intel HEX, TI-TXT, Verilog VMEM, ELF and binary
-files).
-
-Project homepage: https://github.com/eerimoq/moblin_assistant
+A Moblin assistant in the terminal.
 
 Installation
 ============
 
 .. code-block:: python
 
     pip install moblin_assistant
```

### Comparing `moblin_assistant-0.3.0/moblin_assistant.egg-info/PKG-INFO` & `moblin_assistant-0.4.0/moblin_assistant.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moblin_assistant
-Version: 0.3.0
+Version: 0.4.0
 Summary: Moblin remote control assistant
 Home-page: https://github.com/eerimoq/moblin_assistant
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -12,19 +12,15 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: websockets
 
 About
 =====
 
-Mangling of various file formats that conveys binary information
-(Motorola S-Record, Intel HEX, TI-TXT, Verilog VMEM, ELF and binary
-files).
-
-Project homepage: https://github.com/eerimoq/moblin_assistant
+A Moblin assistant in the terminal.
 
 Installation
 ============
 
 .. code-block:: python
 
     pip install moblin_assistant
```

### Comparing `moblin_assistant-0.3.0/moblin_assistant.py` & `moblin_assistant-0.4.0/moblin_assistant.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import asyncio
 from aiohttp import web
 import aiohttp
 from websockets.sync.client import connect
 
 
 __author__ = 'Erik Moqvist'
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 DEFAULT_PORT = 2345
 API_VERSION = '0.1'
 
 
 def random_string():
     return random.randbytes(64).hex()
@@ -23,24 +23,26 @@
 
 class Assistant:
 
     def __init__(self, password):
         self.password = password
         self.challenge = None
         self.salt = None
+        self.identified = False
         self.streamer = None
         self.request_id = 0
         self.client_completions = {}
 
     async def handle_streamer(self, request):
         self.streamer = web.WebSocketResponse()
         await self.streamer.prepare(request)
 
         self.challenge = random_string()
         self.salt = random_string()
+        self.identified = False
         await self.send_to_streamer({
             'hello': {
                 'apiVersion': API_VERSION,
                 'authentication': {
                     'challenge': self.challenge,
                     'salt': self.salt
                 }
@@ -84,34 +86,43 @@
             concatenated.encode('utf-8')).digest()).decode('utf-8')
         concatenated = hash + self.challenge
 
         return b64encode(sha256(
             concatenated.encode('utf-8')).digest()).decode('utf-8')
 
     async def handle_identify(self, authentication):
-        if authentication == self.hash_password():
-            await self.send_to_streamer({
-                'identified': {
-                    'result': {
-                        'ok':{}
-                    }
-                }
-            })
+        if self.identified:
+            result = {'alreadyIdentified': {}}
+        elif authentication == self.hash_password():
+            self.identified = True
+            result = {'ok': {}}
         else:
-            print('identify failed')
+            self.identified = False
+            result = {'wrongPassword': {}}
+
+        await self.send_to_streamer({
+            'identified': {
+                'result': result
+            }
+        })
 
     async def handle_event(self, data):
+        if not self.identified:
+            return
+
         for kind, data in data.items():
             if kind == 'log':
                 print(data['entry'])
             else:
                 print('ignoring event', kind, data)
 
     async def handle_response(self, data):
-        print(data)
+        if not self.identified:
+            return
+
         try:
             request_id = data['id']
             queue = self.client_completions[request_id]
             await queue.put(data)
         except Exception:
             pass
 
@@ -120,34 +131,37 @@
         await client.prepare(request)
 
         async for message in client:
             if message.type == aiohttp.WSMsgType.TEXT:
                 message = json.loads(message.data)
 
                 if message['type'] == 'request':
-                    request_id = self.next_id()
-                    queue = asyncio.Queue()
-                    self.client_completions[request_id] = queue
-                    await self.send_to_streamer({
-                        'request': {
-                            'id': request_id,
-                            'data': message['data']
-                        }
-                    })
-                    await client.send_str(json.dumps({
-                        'type': 'response',
-                        'data': await queue.get()
-                    }))
+                    await self.handle_client_request(client, message)
                 else:
                     print('Not supported', message)
             else:
                 print('Ignoring', message)
 
         return client
 
+    async def handle_client_request(self, client, message):
+        request_id = self.next_id()
+        queue = asyncio.Queue()
+        self.client_completions[request_id] = queue
+        await self.send_to_streamer({
+            'request': {
+                'id': request_id,
+                'data': message['data']
+            }
+        })
+        await client.send_str(json.dumps({
+            'type': 'response',
+            'data': await queue.get()
+        }))
+
 
 def do_run(args):
     app = web.Application()
     assistant = Assistant(args.password)
     app.add_routes([web.get('/', assistant.handle_streamer)])
     app.add_routes([web.get('/client', assistant.handle_client)])
     web.run_app(app, port=args.port)
```

### Comparing `moblin_assistant-0.3.0/setup.py` & `moblin_assistant-0.4.0/setup.py`

 * *Files identical despite different names*

