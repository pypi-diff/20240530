# Comparing `tmp/xingpyc-0.2.5.tar.gz` & `tmp/xingpyc-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.2.5.tar", last modified: Wed May 29 11:12:36 2024, max compression
+gzip compressed data, was "xingpyc-0.2.6.tar", last modified: Thu May 30 07:16:51 2024, max compression
```

## Comparing `xingpyc-0.2.5.tar` & `xingpyc-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-29 11:12:36.785244 xingpyc-0.2.5/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-29 11:12:36.785044 xingpyc-0.2.5/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.5/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-29 11:12:27.000000 xingpyc-0.2.5/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-29 11:12:36.785284 xingpyc-0.2.5/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-29 11:12:36.783440 xingpyc-0.2.5/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-29 11:12:36.783980 xingpyc-0.2.5/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     9148 2024-05-27 20:22:50.000000 xingpyc-0.2.5/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.5/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-29 11:12:36.784833 xingpyc-0.2.5/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-29 11:12:36.000000 xingpyc-0.2.5/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-29 11:12:36.000000 xingpyc-0.2.5/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-29 11:12:36.000000 xingpyc-0.2.5/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-29 11:12:36.000000 xingpyc-0.2.5/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-29 11:12:36.000000 xingpyc-0.2.5/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-29 11:12:36.784691 xingpyc-0.2.5/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.5/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:16:51.095384 xingpyc-0.2.6/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-30 07:16:51.095133 xingpyc-0.2.6/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.6/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-30 07:16:40.000000 xingpyc-0.2.6/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-30 07:16:51.095439 xingpyc-0.2.6/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:16:51.093523 xingpyc-0.2.6/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:16:51.094075 xingpyc-0.2.6/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)    10113 2024-05-30 07:16:44.000000 xingpyc-0.2.6/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.6/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:16:51.094933 xingpyc-0.2.6/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-30 07:16:51.000000 xingpyc-0.2.6/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-30 07:16:51.000000 xingpyc-0.2.6/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-30 07:16:51.000000 xingpyc-0.2.6/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-30 07:16:51.000000 xingpyc-0.2.6/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-30 07:16:51.000000 xingpyc-0.2.6/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:16:51.094767 xingpyc-0.2.6/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.6/tests/test1.py
```

### Comparing `xingpyc-0.2.5/PKG-INFO` & `xingpyc-0.2.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.2.5
+Version: 0.2.6
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.2.5/pyproject.toml` & `xingpyc-0.2.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.2.5/src/xingpyc/__init__.py` & `xingpyc-0.2.6/src/xingpyc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class XClient:
     def __init__(self,funcs,mode: str, ip=None, portOrInfo=None):
         '''
         init a ComClient with AI functions
         funcs: a list of AI functions
         '''
         self.cloudClient = None
-
+        self.incomingMsg = []
 
         self.clients = {}
         self.blockbuffers = {}
         
         #tasks folder is for placing incoming commands
         if not os.path.exists("tasks"):
             os.mkdir("tasks")
@@ -36,125 +36,112 @@
         #results folder is for placing results from various AI functions, no matter binded to XClient or not
         if not os.path.exists("results"):
             os.mkdir("results")
         results = os.listdir("results")
         for result in results:
             os.remove(f"results/{result}")
 
-        #for functions registered with XClient, create a process for each processor that will automatically listen according to there function name
-        #e.g. if there is a function named "i2i" in the list, a process will be created to listen for "i2i" header tasks in the tasks folder
-        for func in funcs:
-            Process(target=add_listener, args=(func,)).start()
-        #sending
-        asyncio.get_event_loop().create_task(self.global_send())
+
+        #message loop
+        asyncio.get_event_loop().create_task(self.message_loop())
 
         #listening
         if(mode == "server"):
             print("\033[93m Server started on "+ip+":"+str(portOrInfo)+" \033[0m")
-            asyncio.get_event_loop().run_until_complete(serve(self.asServer_onRecv, ip, portOrInfo))
+            asyncio.get_event_loop().run_until_complete(serve(self.asServer_listening, ip, portOrInfo))
 
         #for client mode, connect to the cloud server, use sync websocket, async one is not working well for now
         elif(mode == "client"):
             print("\033[93m Client started \033[0m")
             self.cloudClient = WebSocket()
             self.cloudClient.connect(ip)
             self.cloudClient.send_bytes(("login     "+"0000000000"+portOrInfo).encode("utf-8"))
             login_res = self.cloudClient.recv()
             if login_res == b"login success":
                 print("\033[95m===========         Login Success         ============\033[0m")
             
-            Thread(target=self.connect_cloud, args=()).start()
+            Thread(target=self.asClient_listening, args=()).start()
             #asyncio.get_event_loop().create_task(self.connect_cloud(ip,portOrInfo))
-        
-        asyncio.get_event_loop().run_forever()
-
-
-
-
-    def connect_cloud(self):
-        try:
-            while True:
-                message = self.cloudClient.recv()
-                ###### -1 should be client id, change it later
-                self.global_onRecv(-1, message)
-        except Exception as e:
-            print("Connection closed by the server")
 
+        #for functions registered with XClient, create a process for each processor that will automatically listen according to there function name
+        #e.g. if there is a function named "i2i" in the list, a process will be created to listen for "i2i" header tasks in the tasks folder
+        for func in funcs:
+            Process(target=add_listener, args=(func,)).start()
+            
+        asyncio.get_event_loop().run_forever()
 
-    async def asServer_onRecv(self, websocket):
-
-        client_id = id(websocket)
-        print(f"Client {client_id} connected")
-        try:
-            async for message in websocket:
-                self.clients[client_id] = websocket
-                self.global_onRecv(client_id, message)
-
-        except Exception as e:
-            print(f"Error in websocket communication: {e}")
-
-    def global_onRecv(self, client_id, message):
+    async def message_loop(self, blocksize=100000):
         '''
-        WebSocket Object should NOT go inside here, only client_id and message
-        
+        the looping function for sending and receiving messages
         '''
-        print(
-            "\033[93mheader:"+
-            message[:10].replace(b" ", b"").decode()+
-            "   id:"+
-            message[10:20].decode()+
-            "   length:"+
-            str(len(message[20:]))+
-            "\033[0m"
-        )
-        # connect client and save client id
-
-        header = message[:10].replace(b" ", b"").decode()
-        task_id = message[10:20]
-
-        if client_id not in self.blockbuffers:
-            self.blockbuffers[client_id] = []
-
-        content = message[20:]
-        
-        try:
-            if header == "check":
-                print("connect check received")
-                return
-
-            if header == "block":
-                # if block, save it to buffer
-                self.blockbuffers[client_id].append(content)
-                print(len(self.blockbuffers[client_id]), "blocks received")
-                return
-
-            if client_id in self.blockbuffers:
-                # if there is a block buffer, concat it
-                self.blockbuffers[client_id].append(content)
-                content = b"".join(self.blockbuffers[client_id])
-
-                #finally write the file to tasks folder for processing from other processes
-                with open(f"tasks/{client_id}.{task_id.decode()}.{header}", "wb") as f:
-                    print("place task: "+f"{client_id}.{task_id.decode()}.{header}")
-                    f.write(content)
-                del self.blockbuffers[client_id] # clean buffer
-
-        except Exception as e:
-            print(f"Error in websocket communication: {e}")
-            return
-
-    async def global_send(self, blocksize=100000):
-        print("start result->sender loop")
+        print("=== message loop started ===")
+        print("=== message loop started ===")
+        print("=== message loop started ===")
         loopCount = 0
         while True:
             loopCount += 1
             if loopCount % 50 == 0 and self.cloudClient is not None:
                 self.cloudClient.send_bytes("check     0000000000")
                 print("check to cloud")
 
+            ### here starts the incoming message processing
+            ### here starts the incoming message processing
+            ### here starts the incoming message processing
+            currentMsg = self.incomingMsg
+            self.incomingMsg = []
+            for client_id, message in currentMsg:
+                print(
+                    "\033[93mheader:"+
+                    message[:10].replace(b" ", b"").decode()+
+                    "   id:"+
+                    message[10:20].decode()+
+                    "   length:"+
+                    str(len(message[20:]))+
+                    "\033[0m"
+                )
+                # connect client and save client id
+
+                header = message[:10].replace(b" ", b"").decode()
+                task_id = message[10:20]
+
+                if client_id not in self.blockbuffers:
+                    self.blockbuffers[client_id] = []
+
+                content = message[20:]
+                
+                try:
+                    if header == "check":
+                        print("connect check received")
+                        return
+
+                    if header == "block":
+                        # if block, save it to buffer
+                        self.blockbuffers[client_id].append(content)
+                        print(len(self.blockbuffers[client_id]), "blocks received")
+                        return
+
+                    if client_id in self.blockbuffers:
+                        # if there is a block buffer, concat it
+                        self.blockbuffers[client_id].append(content)
+                        content = b"".join(self.blockbuffers[client_id])
+
+                        #finally write the file to tasks folder for processing from other processes
+                        with open(f"tasks/{client_id}.{task_id.decode()}.{header}", "wb") as f:
+                            print("place task: "+f"{client_id}.{task_id.decode()}.{header}")
+                            f.write(content)
+                        del self.blockbuffers[client_id] # clean buffer
+
+                except Exception as e:
+                    print(f"Error in websocket communication: {e}")
+                    return
+                
+            ### here starts the result sending
+            ### here starts the result sending
+            ### here starts the result sending
+
             if len(os.listdir("results")) > 0:
                 for file in os.listdir("results"):
                     try:
                         with open(f"results/{file}", "rb") as f:
                             result_data = f.read()
                         os.remove(f"results/{file}")
                         content = result_data
@@ -179,33 +166,54 @@
                                 content = content[blocksize:]
                                 print(f"sent block {count}/{totalblocks}")
                                 count += 1
 
                             self.cloudClient.send_bytes(header + task_id + content)
                             print("sent to cloud")
                         else:
-                            await self.asServer_send(client_id, header, task_id, content)
+                            
+                            websocket = self.clients.get(client_id)
+                            while len(content) > 0:
+                                if len(content) > blocksize:
+                                    await websocket.send(b"block     " + task_id + content[0:blocksize])
+                                    content = content[blocksize:]
+                                else:
+                                    await websocket.send(header + task_id + content)
+                                    content = b""
+                                await asyncio.sleep(0.01)
+                            await asyncio.sleep(0.01)
 
                         break # only send one result at a time
                     except Exception as e:
                         print(f"Error in sending message to websocket: {e}")
             else:
                 await asyncio.sleep(0.1)
 
-    async def asServer_send(self, client_id, header, task_id, content):
-        websocket = self.clients.get(client_id)
-        while len(content) > 0:
-            if len(content) > 100000:
-                await websocket.send(b"block     " + task_id + content[0:100000])
-                content = content[100000:]
-            else:
-                await websocket.send(header + task_id + content)
-                content = b""
-            await asyncio.sleep(0.01)
-        await asyncio.sleep(0.01)
+    
+    def asClient_listening(self):
+        try:
+            while True:
+                message = self.cloudClient.recv()
+                ###### -1 should be client id, change it later
+                self.incomingMsg.append((-1, message))
+        except Exception as e:
+            print("Connection closed by the server")
+
+
+    async def asServer_listening(self, websocket):
+
+        client_id = id(websocket)
+        print(f"Client {client_id} connected")
+        try:
+            async for message in websocket:
+                self.clients[client_id] = websocket
+                self.incomingMsg.append((client_id, message))
+
+        except Exception as e:
+            print(f"Error in websocket communication: {e}")
 
 
 
 def add_listener(callback, interval=0.1):
     while True:
         taskfiles = os.listdir("tasks")
         time.sleep(interval)
@@ -223,17 +231,19 @@
                     os.remove("tasks/"+file)
         except Exception as e:
             print(f"Error in interpreting task of {callback.__name__}: {e}")
 
 
 
 def i2i(file):
+    #for testing
     print("i2i task received, file:",file)
     return b"i2i"
 
 def config(file):
+    #for testing
     print("config task received, file:",file)
     return b"hello from com test"
 
 if __name__ == "__main__":
     
     XClient([i2i,config],"client", "wss://xing.art/com/","testuser.testuser")
```

### Comparing `xingpyc-0.2.5/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.2.6/src/xingpyc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.2.5
+Version: 0.2.6
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

