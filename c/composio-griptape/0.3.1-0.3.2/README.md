# Comparing `tmp/composio_griptape-0.3.1.tar.gz` & `tmp/composio_griptape-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_griptape-0.3.1.tar", last modified: Thu May 30 09:18:55 2024, max compression
+gzip compressed data, was "composio_griptape-0.3.2.tar", last modified: Thu May 30 15:28:01 2024, max compression
```

## Comparing `composio_griptape-0.3.1.tar` & `composio_griptape-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:18:55.483942 composio_griptape-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-30 09:18:55.483942 composio_griptape-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-30 09:18:38.000000 composio_griptape-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:18:55.483942 composio_griptape-0.3.1/composio_griptape/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 09:18:38.000000 composio_griptape-0.3.1/composio_griptape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-30 09:18:38.000000 composio_griptape-0.3.1/composio_griptape/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:18:55.483942 composio_griptape-0.3.1/composio_griptape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-30 09:18:55.000000 composio_griptape-0.3.1/composio_griptape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-30 09:18:55.000000 composio_griptape-0.3.1/composio_griptape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:18:55.000000 composio_griptape-0.3.1/composio_griptape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 09:18:55.000000 composio_griptape-0.3.1/composio_griptape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 09:18:55.000000 composio_griptape-0.3.1/composio_griptape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:18:55.483942 composio_griptape-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-30 09:18:38.000000 composio_griptape-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:28:01.173902 composio_griptape-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-30 15:28:01.173902 composio_griptape-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-30 15:27:40.000000 composio_griptape-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:28:01.169902 composio_griptape-0.3.2/composio_griptape/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 15:27:40.000000 composio_griptape-0.3.2/composio_griptape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-30 15:27:40.000000 composio_griptape-0.3.2/composio_griptape/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:28:01.173902 composio_griptape-0.3.2/composio_griptape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-30 15:28:01.000000 composio_griptape-0.3.2/composio_griptape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-30 15:28:01.000000 composio_griptape-0.3.2/composio_griptape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:28:01.000000 composio_griptape-0.3.2/composio_griptape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 15:28:01.000000 composio_griptape-0.3.2/composio_griptape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:28:01.000000 composio_griptape-0.3.2/composio_griptape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:28:01.173902 composio_griptape-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-30 15:27:40.000000 composio_griptape-0.3.2/setup.py
```

### Comparing `composio_griptape-0.3.1/PKG-INFO` & `composio_griptape-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
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
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.3.1/README.md` & `composio_griptape-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `composio_griptape-0.3.1/composio_griptape/toolset.py` & `composio_griptape-0.3.2/composio_griptape/toolset.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,19 @@
         super().__init__(
             api_key=api_key,
             base_url=base_url,
             runtime="griptape",
             entity_id=entity_id,
         )
 
-    def _wrap_tool(self, schema: t.Dict) -> t.Type[BaseTool]:
+    def _wrap_tool(
+        self,
+        schema: t.Dict,
+        entity_id: t.Optional[str] = None,
+    ) -> BaseTool:
         """Wrap Composio tool as GripTape `BaseTool` object"""
         app = schema["appName"]
         name = schema["name"]
         description = schema["description"]
 
         schema_dict = {}
         for param_name, param_body in schema["parameters"]["properties"].items():
@@ -86,19 +90,19 @@
                 raise TypeError(
                     f"Some dtype of current schema are not handled yet. Current Schema: {param_body}"
                 )
 
             schema_dict[schema_key] = schema_dtype
 
         def _execute_task(params: t.Dict) -> t.Dict:
-            """Auxialiry method for executing task."""
+            """Placeholder method for executing task."""
             return self.execute_action(
                 action=Action.from_app_and_action(app=app, name=name),
                 params=params,
-                entity_id=self.entity_id,
+                entity_id=entity_id or self.entity_id,
             )
 
         class GripTapeTool(BaseTool):
             """
             Griptap tool wrapper for Composio tools.
             """
 
@@ -120,39 +124,53 @@
                     "name": name,
                     "description": description,
                     "contact_email": "hello@composio.dev",
                     "legal_info_url": "https://www.composio.dev/legal",
                 }
 
         name = "".join(map(lambda x: x.title(), name.split("_"))) + "Client"
-        return type(name, (GripTapeTool,), {})
+        cls = type(name, (GripTapeTool,), {})
+        return cls()
 
-    def get_actions(self, actions: t.Sequence[Action]) -> t.List[BaseTool]:
+    def get_actions(
+        self,
+        actions: t.Sequence[Action],
+        entity_id: t.Optional[str] = None,
+    ) -> t.List[BaseTool]:
         """
         Get composio tools wrapped as GripTape `BaseTool` type objects.
 
         :param actions: List of actions to wrap
+        :param entity_id: Entity ID to use for executing function calls.
         :return: Composio tools wrapped as `BaseTool` objects
         """
 
         return [
-            self._wrap_tool(schema=tool.model_dump(exclude_none=True))()
+            self._wrap_tool(
+                schema=tool.model_dump(exclude_none=True),
+                entity_id=entity_id,
+            )
             for tool in self.client.actions.get(actions=actions)
         ]
 
     def get_tools(
         self,
         apps: t.Sequence[App],
         tags: t.Optional[t.List[t.Union[str, Tag]]] = None,
+        entity_id: t.Optional[str] = None,
     ) -> t.List[BaseTool]:
         """
         Get composio tools wrapped as GripTape `BaseTool` type objects.
 
         :param apps: List of apps to wrap
         :param tags: Filter the apps by given tags
+        :param entity_id: Entity ID to use for executing function calls.
         :return: Composio tools wrapped as `BaseTool` objects
         """
 
         return [
-            self._wrap_tool(schema=tool.model_dump(exclude_none=True))()
+            self._wrap_tool(
+                schema=tool.model_dump(exclude_none=True),
+                entity_id=entity_id,
+            )
             for tool in self.client.actions.get(apps=apps, tags=tags)
         ]
```

### Comparing `composio_griptape-0.3.1/composio_griptape.egg-info/PKG-INFO` & `composio_griptape-0.3.2/composio_griptape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
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
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.3.1/setup.py` & `composio_griptape-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_griptape",
-    version="0.3.1",
+    version="0.3.2",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Griptape wokflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_core===0.3.1", "griptape>=0.24.2"],
+    install_requires=["composio_core===0.3.2", "griptape>=0.24.2"],
     include_package_data=True,
 )
```

