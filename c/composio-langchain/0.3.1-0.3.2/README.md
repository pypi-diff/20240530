# Comparing `tmp/composio_langchain-0.3.1.tar.gz` & `tmp/composio_langchain-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.3.1.tar", last modified: Thu May 30 09:20:41 2024, max compression
+gzip compressed data, was "composio_langchain-0.3.2.tar", last modified: Thu May 30 15:30:07 2024, max compression
```

## Comparing `composio_langchain-0.3.1.tar` & `composio_langchain-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:20:41.906838 composio_langchain-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-30 09:20:41.906838 composio_langchain-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-30 09:20:24.000000 composio_langchain-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:20:41.906838 composio_langchain-0.3.1/composio_langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 09:20:24.000000 composio_langchain-0.3.1/composio_langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-30 09:20:24.000000 composio_langchain-0.3.1/composio_langchain/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:20:41.906838 composio_langchain-0.3.1/composio_langchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-30 09:20:41.000000 composio_langchain-0.3.1/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-30 09:20:41.000000 composio_langchain-0.3.1/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:20:41.000000 composio_langchain-0.3.1/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 09:20:41.000000 composio_langchain-0.3.1/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 09:20:41.000000 composio_langchain-0.3.1/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:20:41.906838 composio_langchain-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-30 09:20:24.000000 composio_langchain-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.768839 composio_langchain-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-30 15:30:07.768839 composio_langchain-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-30 15:29:49.000000 composio_langchain-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.768839 composio_langchain-0.3.2/composio_langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 15:29:49.000000 composio_langchain-0.3.2/composio_langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-30 15:29:49.000000 composio_langchain-0.3.2/composio_langchain/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.768839 composio_langchain-0.3.2/composio_langchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-30 15:30:07.000000 composio_langchain-0.3.2/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-30 15:30:07.000000 composio_langchain-0.3.2/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:30:07.000000 composio_langchain-0.3.2/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 15:30:07.000000 composio_langchain-0.3.2/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 15:30:07.000000 composio_langchain-0.3.2/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:30:07.768839 composio_langchain-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-30 15:29:49.000000 composio_langchain-0.3.2/setup.py
```

### Comparing `composio_langchain-0.3.1/PKG-INFO` & `composio_langchain-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: langchainhub>=0.1.15
-Requires-Dist: composio_core===0.3.1
+Requires-Dist: composio_core===0.3.2
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.3.1/README.md` & `composio_langchain-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.3.1/composio_langchain/toolset.py` & `composio_langchain-0.3.2/composio_langchain/toolset.py`

 * *Files 20% similar despite different names*

```diff
@@ -71,28 +71,33 @@
         super().__init__(
             api_key=api_key,
             base_url=base_url,
             runtime="langchain",
             entity_id=entity_id,
         )
 
-    def _wrap_tool(self, schema: t.Dict[str, t.Any]) -> StructuredTool:
+    def _wrap_tool(
+        self,
+        schema: t.Dict[str, t.Any],
+        entity_id: t.Optional[str] = None,
+    ) -> StructuredTool:
         """Wraps composio tool as Langchain StructuredTool object."""
         app = schema["appName"]
         action = schema["name"]
         description = schema["description"]
 
         def function(**kwargs: t.Any) -> t.Dict:
             """Wrapper function for composio action."""
             return self.execute_action(
                 action=Action.from_app_and_action(
                     app=app,
                     name=action,
                 ),
                 params=kwargs,
+                entity_id=entity_id or self.entity_id,
             )
 
         parameters = json_schema_to_model(
             json_schema=schema["parameters"],
         )
         action_func = types.FunctionType(
             function.__code__,
@@ -110,37 +115,50 @@
             name=action,
             description=description,
             args_schema=parameters,
             return_schema=True,
             func=action_func,
         )
 
-    def get_actions(self, actions: t.Sequence[Action]) -> t.Sequence[StructuredTool]:
+    def get_actions(
+        self,
+        actions: t.Sequence[Action],
+        entity_id: t.Optional[str] = None,
+    ) -> t.Sequence[StructuredTool]:
         """
         Get composio tools wrapped as Langchain StructuredTool objects.
 
         :param actions: List of actions to wrap
+        :param entity_id: Entity ID to use for executing function calls.
         :return: Composio tools wrapped as `StructuredTool` objects
         """
 
         return [
-            self._wrap_tool(schema=tool.model_dump(exclude_none=True))
+            self._wrap_tool(
+                schema=tool.model_dump(exclude_none=True),
+                entity_id=entity_id or self.entity_id,
+            )
             for tool in self.client.actions.get(actions=actions)
         ]
 
     def get_tools(
         self,
         apps: t.Sequence[App],
         tags: t.Optional[t.List[t.Union[str, Tag]]] = None,
+        entity_id: t.Optional[str] = None,
     ) -> t.Sequence[StructuredTool]:
         """
         Get composio tools wrapped as Langchain StructuredTool objects.
 
         :param apps: List of apps to wrap
         :param tags: Filter the apps by given tags
+        :param entity_id: Entity ID to use for executing function calls.
         :return: Composio tools wrapped as `StructuredTool` objects
         """
 
         return [
-            self._wrap_tool(schema=tool.model_dump(exclude_none=True))
+            self._wrap_tool(
+                schema=tool.model_dump(exclude_none=True),
+                entity_id=entity_id or self.entity_id,
+            )
             for tool in self.client.actions.get(apps=apps, tags=tags)
         ]
```

### Comparing `composio_langchain-0.3.1/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.3.2/composio_langchain.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: langchainhub>=0.1.15
-Requires-Dist: composio_core===0.3.1
+Requires-Dist: composio_core===0.3.2
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.3.1/setup.py` & `composio_langchain-0.3.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_langchain",
-    version="0.3.1",
+    version="0.3.2",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
@@ -23,11 +23,11 @@
     ],
     python_requires=">=3.9,<4",
     install_requires=[
         "langchain>=0.1.0",
         "langchain-openai>=0.0.2.post1",
         "pydantic>=2.6.4",
         "langchainhub>=0.1.15",
-        "composio_core===0.3.1",
+        "composio_core===0.3.2",
     ],
     include_package_data=True,
 )
```

