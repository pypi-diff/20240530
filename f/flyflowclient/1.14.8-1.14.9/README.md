# Comparing `tmp/flyflowclient-1.14.8.tar.gz` & `tmp/flyflowclient-1.14.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyflowclient-1.14.8.tar", last modified: Tue May 14 20:22:52 2024, max compression
+gzip compressed data, was "flyflowclient-1.14.9.tar", last modified: Sun May 19 02:26:36 2024, max compression
```

## Comparing `flyflowclient-1.14.8.tar` & `flyflowclient-1.14.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-14 20:22:52.460677 flyflowclient-1.14.8/
--rw-r--r--   0 carlcortright   (501) staff       (20)    11357 2024-05-12 23:23:34.000000 flyflowclient-1.14.8/LICENSE
--rw-r--r--   0 carlcortright   (501) staff       (20)     3817 2024-05-14 20:22:52.460409 flyflowclient-1.14.8/PKG-INFO
--rw-r--r--   0 carlcortright   (501) staff       (20)     3359 2024-05-13 01:08:29.000000 flyflowclient-1.14.8/README.md
-drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-14 20:22:52.457457 flyflowclient-1.14.8/flyflowclient/
--rw-r--r--   0 carlcortright   (501) staff       (20)       27 2024-05-13 00:56:24.000000 flyflowclient-1.14.8/flyflowclient/__init__.py
--rw-r--r--   0 carlcortright   (501) staff       (20)     3878 2024-05-14 20:21:47.000000 flyflowclient-1.14.8/flyflowclient/client.py
-drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-14 20:22:52.459585 flyflowclient-1.14.8/flyflowclient.egg-info/
--rw-r--r--   0 carlcortright   (501) staff       (20)     3817 2024-05-14 20:22:52.000000 flyflowclient-1.14.8/flyflowclient.egg-info/PKG-INFO
--rw-r--r--   0 carlcortright   (501) staff       (20)      260 2024-05-14 20:22:52.000000 flyflowclient-1.14.8/flyflowclient.egg-info/SOURCES.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)        1 2024-05-14 20:22:52.000000 flyflowclient-1.14.8/flyflowclient.egg-info/dependency_links.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)       17 2024-05-14 20:22:52.000000 flyflowclient-1.14.8/flyflowclient.egg-info/requires.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)       14 2024-05-14 20:22:52.000000 flyflowclient-1.14.8/flyflowclient.egg-info/top_level.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)       38 2024-05-14 20:22:52.460731 flyflowclient-1.14.8/setup.cfg
--rw-r--r--   0 carlcortright   (501) staff       (20)      634 2024-05-14 20:22:51.000000 flyflowclient-1.14.8/setup.py
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-19 02:26:36.606667 flyflowclient-1.14.9/
+-rw-r--r--   0 carlcortright   (501) staff       (20)    11357 2024-05-12 23:23:34.000000 flyflowclient-1.14.9/LICENSE
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3806 2024-05-19 02:26:36.606466 flyflowclient-1.14.9/PKG-INFO
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3348 2024-05-14 21:12:04.000000 flyflowclient-1.14.9/README.md
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-19 02:26:36.605406 flyflowclient-1.14.9/flyflowclient/
+-rw-r--r--   0 carlcortright   (501) staff       (20)       27 2024-05-13 00:56:24.000000 flyflowclient-1.14.9/flyflowclient/__init__.py
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3942 2024-05-19 02:23:40.000000 flyflowclient-1.14.9/flyflowclient/client.py
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-19 02:26:36.606255 flyflowclient-1.14.9/flyflowclient.egg-info/
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3806 2024-05-19 02:26:36.000000 flyflowclient-1.14.9/flyflowclient.egg-info/PKG-INFO
+-rw-r--r--   0 carlcortright   (501) staff       (20)      260 2024-05-19 02:26:36.000000 flyflowclient-1.14.9/flyflowclient.egg-info/SOURCES.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)        1 2024-05-19 02:26:36.000000 flyflowclient-1.14.9/flyflowclient.egg-info/dependency_links.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       17 2024-05-19 02:26:36.000000 flyflowclient-1.14.9/flyflowclient.egg-info/requires.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       14 2024-05-19 02:26:36.000000 flyflowclient-1.14.9/flyflowclient.egg-info/top_level.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       38 2024-05-19 02:26:36.606718 flyflowclient-1.14.9/setup.cfg
+-rw-r--r--   0 carlcortright   (501) staff       (20)      634 2024-05-19 02:26:35.000000 flyflowclient-1.14.9/setup.py
```

### Comparing `flyflowclient-1.14.8/LICENSE` & `flyflowclient-1.14.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flyflowclient-1.14.8/PKG-INFO` & `flyflowclient-1.14.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyflowclient
-Version: 1.14.8
+Version: 1.14.9
 Summary: A client library for the FlyFlow API
 Home-page: https://github.com/flyflow-devs/flyflow-python
 Author: Carl Cortright
 Author-email: carl@flyflow.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -48,23 +48,23 @@
 
 ### Agent Management
 
 #### Create an Agent
 
 ```python
 agent = client.create_agent(
-    name='Agent Name',
-    system_prompt='System prompt',
-    initial_message='Initial message',
-    llm_model='gpt-3.5-turbo',
-    voice_id='voice_id',
-    webhook='https://webhook-url.com',
-    tools=[],
-    filler_words=True,
-    area_code='123'
+   name='Agent Name',
+   system_prompt='System prompt',
+   initial_message='Initial message',
+   llm_model='gpt-3.5-turbo',
+   voice_id='voice_id',
+   webhook='https://webhook-url.com',
+   tools=[],
+   filler_words=True,
+   area_code='123'
 )
 ```
 
 #### Update an Agent
 
 ```python
 updated_agent = client.update_agent(
@@ -110,16 +110,16 @@
 call = client.get_call(call_id=call['id'])
 ```
 
 #### Set Call Context
 
 ```python
 updated_call = client.set_call_context(
-    call_id=call['id'],
-    context='Updated call context'
+   call_id=call['id'],
+   context='Updated call context'
 )
 ```
 
 #### List Calls
 
 ```python
 calls = client.list_calls(limit=10, agent_id=agent['id'])
```

### Comparing `flyflowclient-1.14.8/README.md` & `flyflowclient-1.14.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 
 ### Agent Management
 
 #### Create an Agent
 
 ```python
 agent = client.create_agent(
-    name='Agent Name',
-    system_prompt='System prompt',
-    initial_message='Initial message',
-    llm_model='gpt-3.5-turbo',
-    voice_id='voice_id',
-    webhook='https://webhook-url.com',
-    tools=[],
-    filler_words=True,
-    area_code='123'
+   name='Agent Name',
+   system_prompt='System prompt',
+   initial_message='Initial message',
+   llm_model='gpt-3.5-turbo',
+   voice_id='voice_id',
+   webhook='https://webhook-url.com',
+   tools=[],
+   filler_words=True,
+   area_code='123'
 )
 ```
 
 #### Update an Agent
 
 ```python
 updated_agent = client.update_agent(
@@ -96,16 +96,16 @@
 call = client.get_call(call_id=call['id'])
 ```
 
 #### Set Call Context
 
 ```python
 updated_call = client.set_call_context(
-    call_id=call['id'],
-    context='Updated call context'
+   call_id=call['id'],
+   context='Updated call context'
 )
 ```
 
 #### List Calls
 
 ```python
 calls = client.list_calls(limit=10, agent_id=agent['id'])
```

### Comparing `flyflowclient-1.14.8/flyflowclient/client.py` & `flyflowclient-1.14.9/flyflowclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,20 @@
             'id': call_id,
             'context': context
         }
         response = requests.post(f'{self.base_url}/call/context', json=payload, headers=self.headers)
         response.raise_for_status()
         return response.json()
 
-    def list_calls(self, cursor=None, limit=10, agent_id=None):
+    def list_calls(self, cursor=None, limit=10, agent_id=None, client_number=None):
         params = {
             'cursor': cursor,
             'limit': limit,
-            'agent_id': agent_id
+            'agent_id': agent_id,
+            'client_number': client_number
         }
         response = requests.get(f'{self.base_url}/calls', params=params, headers=self.headers)
         response.raise_for_status()
         return response.json()
 
     def create_agent(self, name=None, system_prompt=None, initial_message=None, voice_id=None, llm_model=None, webhook=None, tools=None, filler_words=None, filler_words_whitelist=None, area_code=None):
         payload = {
```

### Comparing `flyflowclient-1.14.8/flyflowclient.egg-info/PKG-INFO` & `flyflowclient-1.14.9/flyflowclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyflowclient
-Version: 1.14.8
+Version: 1.14.9
 Summary: A client library for the FlyFlow API
 Home-page: https://github.com/flyflow-devs/flyflow-python
 Author: Carl Cortright
 Author-email: carl@flyflow.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -48,23 +48,23 @@
 
 ### Agent Management
 
 #### Create an Agent
 
 ```python
 agent = client.create_agent(
-    name='Agent Name',
-    system_prompt='System prompt',
-    initial_message='Initial message',
-    llm_model='gpt-3.5-turbo',
-    voice_id='voice_id',
-    webhook='https://webhook-url.com',
-    tools=[],
-    filler_words=True,
-    area_code='123'
+   name='Agent Name',
+   system_prompt='System prompt',
+   initial_message='Initial message',
+   llm_model='gpt-3.5-turbo',
+   voice_id='voice_id',
+   webhook='https://webhook-url.com',
+   tools=[],
+   filler_words=True,
+   area_code='123'
 )
 ```
 
 #### Update an Agent
 
 ```python
 updated_agent = client.update_agent(
@@ -110,16 +110,16 @@
 call = client.get_call(call_id=call['id'])
 ```
 
 #### Set Call Context
 
 ```python
 updated_call = client.set_call_context(
-    call_id=call['id'],
-    context='Updated call context'
+   call_id=call['id'],
+   context='Updated call context'
 )
 ```
 
 #### List Calls
 
 ```python
 calls = client.list_calls(limit=10, agent_id=agent['id'])
```

### Comparing `flyflowclient-1.14.8/setup.py` & `flyflowclient-1.14.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="flyflowclient",
-    version="1.14.8",
+    version="1.14.9",
     packages=find_packages(),
     install_requires=[
         "requests>=2.25.1"
     ],
     author="Carl Cortright",
     author_email="carl@flyflow.dev",
     description="A client library for the FlyFlow API",
```

