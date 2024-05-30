# Comparing `tmp/composio_claude-0.3.1.tar.gz` & `tmp/composio_claude-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_claude-0.3.1.tar", last modified: Thu May 30 09:17:18 2024, max compression
+gzip compressed data, was "composio_claude-0.3.2.tar", last modified: Thu May 30 15:26:13 2024, max compression
```

## Comparing `composio_claude-0.3.1.tar` & `composio_claude-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:17:18.023148 composio_claude-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-30 09:17:18.019147 composio_claude-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-30 09:17:03.000000 composio_claude-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:17:18.019147 composio_claude-0.3.1/composio_claude/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 09:17:03.000000 composio_claude-0.3.1/composio_claude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-30 09:17:03.000000 composio_claude-0.3.1/composio_claude/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:17:18.019147 composio_claude-0.3.1/composio_claude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-30 09:17:18.000000 composio_claude-0.3.1/composio_claude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 09:17:18.000000 composio_claude-0.3.1/composio_claude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:17:18.000000 composio_claude-0.3.1/composio_claude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 09:17:18.000000 composio_claude-0.3.1/composio_claude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 09:17:18.000000 composio_claude-0.3.1/composio_claude.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:17:18.023148 composio_claude-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-30 09:17:03.000000 composio_claude-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:26:13.883198 composio_claude-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-30 15:26:13.883198 composio_claude-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-30 15:25:52.000000 composio_claude-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:26:13.883198 composio_claude-0.3.2/composio_claude/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 15:25:52.000000 composio_claude-0.3.2/composio_claude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-05-30 15:25:52.000000 composio_claude-0.3.2/composio_claude/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:26:13.883198 composio_claude-0.3.2/composio_claude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-30 15:26:13.000000 composio_claude-0.3.2/composio_claude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 15:26:13.000000 composio_claude-0.3.2/composio_claude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:26:13.000000 composio_claude-0.3.2/composio_claude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 15:26:13.000000 composio_claude-0.3.2/composio_claude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 15:26:13.000000 composio_claude-0.3.2/composio_claude.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:26:13.883198 composio_claude-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-30 15:25:52.000000 composio_claude-0.3.2/setup.py
```

### Comparing `composio_claude-0.3.1/PKG-INFO` & `composio_claude-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_claude
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Composio to get an array of tools with your Claude LLMs.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.3.1
+Requires-Dist: composio_openai===0.3.2
 Requires-Dist: anthropic>=0.25.7
 
 ## 🚀🔗 Leveraging Claude with Composio
 
 Facilitate the integration of Claude with Composio to empower Claude models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_claude-0.3.1/README.md` & `composio_claude-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `composio_claude-0.3.1/composio_claude/toolset.py` & `composio_claude-0.3.2/composio_claude/toolset.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,46 +132,46 @@
             )
             for schema in self.client.actions.get(apps=apps, tags=tags)
         ]
 
     def execute_tool_call(
         self,
         tool_call: ToolUseBlock,
-        entity_id: str = DEFAULT_ENTITY_ID,
+        entity_id: t.Optional[str] = None,
     ) -> t.Dict:
         """
         Execute a tool call.
 
         :param tool_call: Tool call metadata.
-        :param entity_id: Entity ID.
+        :param entity_id: Entity ID to use for executing function calls.
         :return: Object containing output data from the tool call.
         """
         return self.execute_action(
             action=Action.from_action(name=tool_call.name),
             params=t.cast(t.Dict, tool_call.input),
-            entity_id=entity_id,
+            entity_id=entity_id or self.entity_id,
         )
 
     def handle_tool_calls(
         self,
         llm_response: ToolsBetaMessage,
-        entity_id: str = DEFAULT_ENTITY_ID,
+        entity_id: t.Optional[str] = None,
     ) -> t.List[t.Dict]:
         """
         Handle tool calls from OpenAI chat completion object.
 
         :param response: Chat completion object from
                         openai.OpenAI.chat.completions.create function call
-        :param entity_id: Entity ID.
+        :param entity_id: Entity ID to use for executing function calls.
         :return: A list of output objects from the function calls.
         """
-        entity_id = self.validate_entity_id(entity_id)
+        entity_id = self.validate_entity_id(entity_id or self.entity_id)
         outputs = []
         for content in llm_response.content:
             if isinstance(content, ToolUseBlock):
                 outputs.append(
                     self.execute_tool_call(
                         tool_call=content,
-                        entity_id=entity_id,
+                        entity_id=entity_id or self.entity_id,
                     )
                 )
         return outputs
```

### Comparing `composio_claude-0.3.1/composio_claude.egg-info/PKG-INFO` & `composio_claude-0.3.2/composio_claude.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_claude
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Composio to get an array of tools with your Claude LLMs.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.3.1
+Requires-Dist: composio_openai===0.3.2
 Requires-Dist: anthropic>=0.25.7
 
 ## 🚀🔗 Leveraging Claude with Composio
 
 Facilitate the integration of Claude with Composio to empower Claude models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_claude-0.3.1/setup.py` & `composio_claude-0.3.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_claude",
-    version="0.3.1",
+    version="0.3.2",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Claude LLMs.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_openai===0.3.1", "anthropic>=0.25.7"],
+    install_requires=["composio_openai===0.3.2", "anthropic>=0.25.7"],
     include_package_data=True,
 )
```

