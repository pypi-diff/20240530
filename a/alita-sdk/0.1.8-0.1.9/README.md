# Comparing `tmp/alita_sdk-0.1.8.tar.gz` & `tmp/alita_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_sdk-0.1.8.tar", last modified: Mon May 20 06:53:15 2024, max compression
+gzip compressed data, was "alita_sdk-0.1.9.tar", last modified: Mon May 20 09:44:00 2024, max compression
```

## Comparing `alita_sdk-0.1.8.tar` & `alita_sdk-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.563035 alita_sdk-0.1.8/
--rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.8/LICENSE
--rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-20 06:53:15.562800 alita_sdk-0.1.8/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.8/README.md
--rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-05-20 06:53:10.000000 alita_sdk-0.1.8/pyproject.toml
--rw-r--r--   0 arozumenko   (501) staff       (20)      175 2024-05-08 13:44:16.000000 alita_sdk-0.1.8/requirements.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-05-20 06:53:15.563084 alita_sdk-0.1.8/setup.cfg
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.558320 alita_sdk-0.1.8/src/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.8/src/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.558419 alita_sdk-0.1.8/src/alita_sdk/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.8/src/alita_sdk/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.559883 alita_sdk-0.1.8/src/alita_sdk/agents/
--rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.8/src/alita_sdk/agents/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3122 2024-04-30 17:52:10.000000 alita_sdk-0.1.8/src/alita_sdk/agents/alita_openai.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3135 2024-05-16 11:42:35.000000 alita_sdk-0.1.8/src/alita_sdk/agents/mixedAgentParser.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2380 2024-05-09 09:15:40.000000 alita_sdk-0.1.8/src/alita_sdk/agents/mixedAgentRenderes.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1151 2024-05-16 11:35:26.000000 alita_sdk-0.1.8/src/alita_sdk/agents/utils.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.560287 alita_sdk-0.1.8/src/alita_sdk/clients/
--rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.8/src/alita_sdk/clients/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    21902 2024-05-20 06:52:53.000000 alita_sdk-0.1.8/src/alita_sdk/clients/client.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.560825 alita_sdk-0.1.8/src/alita_sdk/llms/
--rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.8/src/alita_sdk/llms/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     8851 2024-05-02 10:28:32.000000 alita_sdk-0.1.8/src/alita_sdk/llms/alita.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.561405 alita_sdk-0.1.8/src/alita_sdk/toolkits/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.8/src/alita_sdk/toolkits/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      798 2024-05-08 13:59:31.000000 alita_sdk-0.1.8/src/alita_sdk/toolkits/application.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.8/src/alita_sdk/toolkits/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.8/src/alita_sdk/toolkits/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.561957 alita_sdk-0.1.8/src/alita_sdk/tools/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.8/src/alita_sdk/tools/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      530 2024-05-08 13:59:34.000000 alita_sdk-0.1.8/src/alita_sdk/tools/application.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.8/src/alita_sdk/tools/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-05-14 06:19:04.000000 alita_sdk-0.1.8/src/alita_sdk/tools/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.562181 alita_sdk-0.1.8/src/alita_sdk/utils/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.8/src/alita_sdk/utils/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.8/src/alita_sdk/utils/streamlit.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.562518 alita_sdk-0.1.8/src/alita_sdk.egg-info/
--rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-20 06:53:15.000000 alita_sdk-0.1.8/src/alita_sdk.egg-info/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)      923 2024-05-20 06:53:15.000000 alita_sdk-0.1.8/src/alita_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-05-20 06:53:15.000000 alita_sdk-0.1.8/src/alita_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)      176 2024-05-20 06:53:15.000000 alita_sdk-0.1.8/src/alita_sdk.egg-info/requires.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-05-20 06:53:15.000000 alita_sdk-0.1.8/src/alita_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 09:44:00.251835 alita_sdk-0.1.9/
+-rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.9/LICENSE
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-20 09:44:00.251595 alita_sdk-0.1.9/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.9/README.md
+-rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-05-20 09:43:36.000000 alita_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0 arozumenko   (501) staff       (20)      175 2024-05-08 13:44:16.000000 alita_sdk-0.1.9/requirements.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-05-20 09:44:00.251879 alita_sdk-0.1.9/setup.cfg
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 09:44:00.245116 alita_sdk-0.1.9/src/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.9/src/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 09:44:00.245219 alita_sdk-0.1.9/src/alita_sdk/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.9/src/alita_sdk/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 09:44:00.246927 alita_sdk-0.1.9/src/alita_sdk/agents/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.9/src/alita_sdk/agents/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3122 2024-04-30 17:52:10.000000 alita_sdk-0.1.9/src/alita_sdk/agents/alita_openai.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3135 2024-05-16 11:42:35.000000 alita_sdk-0.1.9/src/alita_sdk/agents/mixedAgentParser.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2380 2024-05-09 09:15:40.000000 alita_sdk-0.1.9/src/alita_sdk/agents/mixedAgentRenderes.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1151 2024-05-16 11:35:26.000000 alita_sdk-0.1.9/src/alita_sdk/agents/utils.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 09:44:00.247421 alita_sdk-0.1.9/src/alita_sdk/clients/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.9/src/alita_sdk/clients/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    21902 2024-05-20 09:43:18.000000 alita_sdk-0.1.9/src/alita_sdk/clients/client.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 09:44:00.248199 alita_sdk-0.1.9/src/alita_sdk/llms/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.9/src/alita_sdk/llms/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     8851 2024-05-02 10:28:32.000000 alita_sdk-0.1.9/src/alita_sdk/llms/alita.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 09:44:00.249271 alita_sdk-0.1.9/src/alita_sdk/toolkits/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.9/src/alita_sdk/toolkits/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      786 2024-05-20 09:41:16.000000 alita_sdk-0.1.9/src/alita_sdk/toolkits/application.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.9/src/alita_sdk/toolkits/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.9/src/alita_sdk/toolkits/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 09:44:00.250271 alita_sdk-0.1.9/src/alita_sdk/tools/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.9/src/alita_sdk/tools/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      530 2024-05-08 13:59:34.000000 alita_sdk-0.1.9/src/alita_sdk/tools/application.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.9/src/alita_sdk/tools/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-05-14 06:19:04.000000 alita_sdk-0.1.9/src/alita_sdk/tools/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 09:44:00.250614 alita_sdk-0.1.9/src/alita_sdk/utils/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.9/src/alita_sdk/utils/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.9/src/alita_sdk/utils/streamlit.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 09:44:00.251275 alita_sdk-0.1.9/src/alita_sdk.egg-info/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-20 09:44:00.000000 alita_sdk-0.1.9/src/alita_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)      923 2024-05-20 09:44:00.000000 alita_sdk-0.1.9/src/alita_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-05-20 09:44:00.000000 alita_sdk-0.1.9/src/alita_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)      176 2024-05-20 09:44:00.000000 alita_sdk-0.1.9/src/alita_sdk.egg-info/requires.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-05-20 09:44:00.000000 alita_sdk-0.1.9/src/alita_sdk.egg-info/top_level.txt
```

### Comparing `alita_sdk-0.1.8/LICENSE` & `alita_sdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/PKG-INFO` & `alita_sdk-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_sdk-0.1.8/README.md` & `alita_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/pyproject.toml` & `alita_sdk-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_sdk"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Artem Rozumenko", email="support@analysta.ai" },
 ]
 description = "SDK for building langchain agents using resouces from Alita"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `alita_sdk-0.1.8/src/alita_sdk/agents/__init__.py` & `alita_sdk-0.1.9/src/alita_sdk/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/agents/alita_openai.py` & `alita_sdk-0.1.9/src/alita_sdk/agents/alita_openai.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/agents/mixedAgentParser.py` & `alita_sdk-0.1.9/src/alita_sdk/agents/mixedAgentParser.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/agents/mixedAgentRenderes.py` & `alita_sdk-0.1.9/src/alita_sdk/agents/mixedAgentRenderes.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/agents/utils.py` & `alita_sdk-0.1.9/src/alita_sdk/agents/utils.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/clients/client.py` & `alita_sdk-0.1.9/src/alita_sdk/clients/client.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/llms/alita.py` & `alita_sdk-0.1.9/src/alita_sdk/llms/alita.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/toolkits/application.py` & `alita_sdk-0.1.9/src/alita_sdk/toolkits/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from langchain_core.tools import BaseTool
 from ..tools.application import Application, applicationToolSchema
 
 class ApplicationToolkit(BaseToolkit):
     tools: List[BaseTool] = []
     
     @classmethod
-    def get_toolkit(cls, client: Any, application_id: list[int], application_version_id: list[int], selected_tools: list[str] = [] ):
+    def get_toolkit(cls, client: Any, application_id: int, application_version_id: int, selected_tools: list[str] = [] ):
         app_details = client.get_app_details(application_id)
         app = client.application(application_id, application_version_id)
         return cls(tools=[Application(name=app_details.get("name"), description=app_details.get("description"), appliacation=app, args_schema=applicationToolSchema)])
             
     def get_tools(self):
         return self.tools
```

### Comparing `alita_sdk-0.1.8/src/alita_sdk/toolkits/datasource.py` & `alita_sdk-0.1.9/src/alita_sdk/toolkits/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/toolkits/prompt.py` & `alita_sdk-0.1.9/src/alita_sdk/toolkits/prompt.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/tools/application.py` & `alita_sdk-0.1.9/src/alita_sdk/tools/application.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/tools/datasource.py` & `alita_sdk-0.1.9/src/alita_sdk/tools/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk/utils/streamlit.py` & `alita_sdk-0.1.9/src/alita_sdk/utils/streamlit.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.8/src/alita_sdk.egg-info/PKG-INFO` & `alita_sdk-0.1.9/src/alita_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_sdk-0.1.8/src/alita_sdk.egg-info/SOURCES.txt` & `alita_sdk-0.1.9/src/alita_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

