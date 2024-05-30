# Comparing `tmp/composio_autogen-0.3.1.tar.gz` & `tmp/composio_autogen-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.3.1.tar", last modified: Thu May 30 09:16:29 2024, max compression
+gzip compressed data, was "composio_autogen-0.3.2.tar", last modified: Thu May 30 15:25:19 2024, max compression
```

## Comparing `composio_autogen-0.3.1.tar` & `composio_autogen-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:16:29.870144 composio_autogen-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-30 09:16:29.870144 composio_autogen-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-30 09:16:14.000000 composio_autogen-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:16:29.866144 composio_autogen-0.3.1/composio_autogen/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-30 09:16:14.000000 composio_autogen-0.3.1/composio_autogen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-05-30 09:16:14.000000 composio_autogen-0.3.1/composio_autogen/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:16:29.870144 composio_autogen-0.3.1/composio_autogen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-30 09:16:29.000000 composio_autogen-0.3.1/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 09:16:29.000000 composio_autogen-0.3.1/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:16:29.000000 composio_autogen-0.3.1/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 09:16:29.000000 composio_autogen-0.3.1/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 09:16:29.000000 composio_autogen-0.3.1/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:16:29.870144 composio_autogen-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-30 09:16:14.000000 composio_autogen-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:25:19.080191 composio_autogen-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-30 15:25:19.080191 composio_autogen-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-30 15:24:51.000000 composio_autogen-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:25:19.080191 composio_autogen-0.3.2/composio_autogen/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-30 15:24:51.000000 composio_autogen-0.3.2/composio_autogen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-30 15:24:51.000000 composio_autogen-0.3.2/composio_autogen/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:25:19.080191 composio_autogen-0.3.2/composio_autogen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-30 15:25:19.000000 composio_autogen-0.3.2/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 15:25:19.000000 composio_autogen-0.3.2/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:25:19.000000 composio_autogen-0.3.2/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 15:25:19.000000 composio_autogen-0.3.2/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 15:25:19.000000 composio_autogen-0.3.2/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:25:19.080191 composio_autogen-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-30 15:24:51.000000 composio_autogen-0.3.2/setup.py
```

### Comparing `composio_autogen-0.3.1/PKG-INFO` & `composio_autogen-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Composio to get an array of tools with your Autogen agent.
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
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.3.1/README.md` & `composio_autogen-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.3.1/composio_autogen/toolset.py` & `composio_autogen-0.3.2/composio_autogen/toolset.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,24 @@
 
     def register_tools(
         self,
         tools: t.Sequence[App],
         caller: t.Optional[ConversableAgent] = None,
         executor: t.Optional[ConversableAgent] = None,
         tags: t.Optional[t.Sequence[Tag]] = None,
+        entity_id: t.Optional[str] = None,
     ) -> None:
         """
         Register tools to the proxy agents.
 
         :param tools: List of tools to register.
         :param caller: Caller agent.
         :param executor: Executor agent.
         :param tags: Filter by the list of given Tags.
+        :param entity_id: Entity ID to use for executing function calls.
         """
         if isinstance(tools, App):
             tools = [tools]
 
         caller = caller or self.caller
         if caller is None:
             raise RuntimeError("Please provide `caller` agent")
@@ -75,28 +77,31 @@
                 schema=schema.model_dump(
                     exclude_defaults=True,
                     exclude_none=True,
                     exclude_unset=True,
                 ),
                 caller=caller,
                 executor=executor,
+                entity_id=entity_id or self.entity_id,
             )
 
     def register_actions(
         self,
         actions: t.Sequence[Action],
         caller: t.Optional[ConversableAgent] = None,
         executor: t.Optional[ConversableAgent] = None,
+        entity_id: t.Optional[str] = None,
     ):
         """
         Register tools to the proxy agents.
 
         :param actions: List of tools to register.
         :param caller: Caller agent.
         :param executor: Executor agent.
+        :param entity_id: Entity ID to use for executing function calls.
         """
 
         caller = caller or self.caller
         if caller is None:
             raise RuntimeError("Please provide `caller` agent")
 
         executor = executor or self.executor
@@ -109,14 +114,15 @@
                 schema=schema.model_dump(
                     exclude_defaults=True,
                     exclude_none=True,
                     exclude_unset=True,
                 ),
                 caller=caller,
                 executor=executor,
+                entity_id=entity_id or self.entity_id,
             )
 
     def _process_function_name_for_registration(
         self,
         input_string: str,
         max_allowed_length: int = 64,
         num_hash_char: int = 10,
@@ -130,28 +136,30 @@
         return processed_name
 
     def _register_schema_to_autogen(
         self,
         schema: t.Dict,
         caller: ConversableAgent,
         executor: ConversableAgent,
-    ):
+        entity_id: t.Optional[str] = None,
+    ) -> None:
+        """Register action schema to autogen registry."""
         name = schema["name"]
         appName = schema["appName"]
         description = schema["description"]
 
         def execute_action(**kwargs: t.Any) -> t.Dict:
             """Placeholder function for executing action."""
             return self.execute_action(
                 action=Action.from_app_and_action(
                     app=appName,
                     name=name,
                 ),
                 params=kwargs,
-                entity_id=self.entity_id,
+                entity_id=entity_id or self.entity_id,
             )
 
         function = types.FunctionType(
             code=execute_action.__code__,
             globals=globals(),
             name=self._process_function_name_for_registration(
                 input_string=name,
```

### Comparing `composio_autogen-0.3.1/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.3.2/composio_autogen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Composio to get an array of tools with your Autogen agent.
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
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.3.1/setup.py` & `composio_autogen-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_autogen",
-    version="0.3.1",
+    version="0.3.2",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_core===0.3.1", "pyautogen>=0.2.19"],
+    install_requires=["composio_core===0.3.2", "pyautogen>=0.2.19"],
     include_package_data=True,
 )
```

