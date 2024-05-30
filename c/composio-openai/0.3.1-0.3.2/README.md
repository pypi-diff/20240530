# Comparing `tmp/composio_openai-0.3.1.tar.gz` & `tmp/composio_openai-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_openai-0.3.1.tar", last modified: Thu May 30 09:23:04 2024, max compression
+gzip compressed data, was "composio_openai-0.3.2.tar", last modified: Thu May 30 15:31:53 2024, max compression
```

## Comparing `composio_openai-0.3.1.tar` & `composio_openai-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:23:04.435749 composio_openai-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-30 09:23:04.435749 composio_openai-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-30 09:22:43.000000 composio_openai-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:23:04.435749 composio_openai-0.3.1/composio_openai/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 09:22:43.000000 composio_openai-0.3.1/composio_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-30 09:22:43.000000 composio_openai-0.3.1/composio_openai/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:23:04.435749 composio_openai-0.3.1/composio_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-30 09:23:04.000000 composio_openai-0.3.1/composio_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 09:23:04.000000 composio_openai-0.3.1/composio_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:23:04.000000 composio_openai-0.3.1/composio_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 09:23:04.000000 composio_openai-0.3.1/composio_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 09:23:04.000000 composio_openai-0.3.1/composio_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:23:04.435749 composio_openai-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-30 09:22:43.000000 composio_openai-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:31:53.784224 composio_openai-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-30 15:31:53.784224 composio_openai-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-30 15:31:37.000000 composio_openai-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:31:53.780224 composio_openai-0.3.2/composio_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 15:31:37.000000 composio_openai-0.3.2/composio_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-05-30 15:31:37.000000 composio_openai-0.3.2/composio_openai/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:31:53.784224 composio_openai-0.3.2/composio_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-30 15:31:53.000000 composio_openai-0.3.2/composio_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 15:31:53.000000 composio_openai-0.3.2/composio_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:31:53.000000 composio_openai-0.3.2/composio_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:31:53.000000 composio_openai-0.3.2/composio_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 15:31:53.000000 composio_openai-0.3.2/composio_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:31:53.784224 composio_openai-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-30 15:31:37.000000 composio_openai-0.3.2/setup.py
```

### Comparing `composio_openai-0.3.1/PKG-INFO` & `composio_openai-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.3.1
+Requires-Dist: composio_core===0.3.2
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.3.1/README.md` & `composio_openai-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `composio_openai-0.3.1/composio_openai/toolset.py` & `composio_openai-0.3.2/composio_openai/toolset.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,87 +146,95 @@
             )
             for schema in self.client.actions.get(apps=apps, tags=tags)
         ]
 
     def execute_tool_call(
         self,
         tool_call: ChatCompletionMessageToolCall,
-        entity_id: str = DEFAULT_ENTITY_ID,
+        entity_id: t.Optional[str] = None,
     ) -> t.Dict:
         """
         Execute a tool call.
 
         :param tool_call: Tool call metadata.
-        :param entity_id: Entity ID.
+        :param entity_id: Entity ID to use for executing the function call.
         :return: Object containing output data from the tool call.
         """
         return self.execute_action(
             action=Action.from_action(name=tool_call.function.name),
             params=json.loads(tool_call.function.arguments),
-            entity_id=entity_id,
+            entity_id=entity_id or self.entity_id,
         )
 
     def handle_tool_calls(
         self,
         response: ChatCompletion,
-        entity_id: str = DEFAULT_ENTITY_ID,
+        entity_id: t.Optional[str] = None,
     ) -> t.List[t.Dict]:
         """
         Handle tool calls from OpenAI chat completion object.
 
         :param response: Chat completion object from
                         openai.OpenAI.chat.completions.create function call
-        :param entity_id: Entity ID.
+        :param entity_id: Entity ID to use for executing the function call.
         :return: A list of output objects from the function calls.
         """
-        entity_id = self.validate_entity_id(entity_id)
+        entity_id = self.validate_entity_id(entity_id or self.entity_id)
         outputs = []
         if response.choices:
             for choice in response.choices:
                 if choice.message.tool_calls:
                     for tool_call in choice.message.tool_calls:
                         outputs.append(
                             self.execute_tool_call(
                                 tool_call=tool_call,
-                                entity_id=entity_id,
+                                entity_id=entity_id or self.entity_id,
                             )
                         )
         return outputs
 
-    def handle_assistant_tool_calls(self, run: Run) -> t.List:
+    def handle_assistant_tool_calls(
+        self,
+        run: Run,
+        entity_id: t.Optional[str] = None,
+    ) -> t.List:
         """Wait and handle assisant function calls"""
         tool_outputs = []
         for tool_call in t.cast(
             RequiredAction, run.required_action
         ).submit_tool_outputs.tool_calls:
             tool_response = self.execute_tool_call(
                 tool_call=t.cast(ChatCompletionMessageToolCall, tool_call),
-                entity_id=self.entity_id,
+                entity_id=entity_id or self.entity_id,
             )
             tool_output = {
                 "tool_call_id": tool_call.id,
                 "output": json.dumps(tool_response),
             }
             tool_outputs.append(tool_output)
         return tool_outputs
 
     def wait_and_handle_assistant_tool_calls(
         self,
         client: Client,
         run: Run,
         thread: Thread,
+        entity_id: t.Optional[str] = None,
     ) -> Run:
         """Wait and handle assisant function calls"""
         thread_object = thread
         while run.status in ("queued", "in_progress", "requires_action"):
             if run.status == "requires_action":
                 run = client.beta.threads.runs.submit_tool_outputs(
                     thread_id=thread_object.id,
                     run_id=run.id,
-                    tool_outputs=self.handle_assistant_tool_calls(run),
+                    tool_outputs=self.handle_assistant_tool_calls(
+                        run=run,
+                        entity_id=entity_id or self.entity_id,
+                    ),
                 )
             else:
                 run = client.beta.threads.runs.retrieve(
                     thread_id=thread_object.id,
                     run_id=run.id,
                 )
                 time.sleep(0.5)
```

### Comparing `composio_openai-0.3.1/composio_openai.egg-info/PKG-INFO` & `composio_openai-0.3.2/composio_openai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.3.1
+Requires-Dist: composio_core===0.3.2
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

