# Comparing `tmp/cybersailor-0.1.3.tar.gz` & `tmp/cybersailor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybersailor-0.1.3.tar", last modified: Sun Apr 14 04:03:31 2024, max compression
+gzip compressed data, was "cybersailor-0.1.4.tar", last modified: Thu May 30 07:07:50 2024, max compression
```

## Comparing `cybersailor-0.1.3.tar` & `cybersailor-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-14 04:03:31.589696 cybersailor-0.1.3/
--rw-r--r--   0 wanglei    (501) staff       (20)      372 2024-04-14 04:03:31.589276 cybersailor-0.1.3/PKG-INFO
--rw-r--r--   0 wanglei    (501) staff       (20)       11 2024-03-19 04:35:41.000000 cybersailor-0.1.3/README.md
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-14 04:03:31.586070 cybersailor-0.1.3/cybersailor/
--rw-r--r--   0 wanglei    (501) staff       (20)       50 2024-03-19 06:42:00.000000 cybersailor-0.1.3/cybersailor/__init__.py
--rw-r--r--   0 wanglei    (501) staff       (20)      533 2024-03-20 02:22:34.000000 cybersailor-0.1.3/cybersailor/logger.py
--rw-r--r--   0 wanglei    (501) staff       (20)     5736 2024-04-14 04:01:04.000000 cybersailor-0.1.3/cybersailor/sdk.py
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-14 04:03:31.588823 cybersailor-0.1.3/cybersailor.egg-info/
--rw-r--r--   0 wanglei    (501) staff       (20)      372 2024-04-14 04:03:31.000000 cybersailor-0.1.3/cybersailor.egg-info/PKG-INFO
--rw-r--r--   0 wanglei    (501) staff       (20)      257 2024-04-14 04:03:31.000000 cybersailor-0.1.3/cybersailor.egg-info/SOURCES.txt
--rw-r--r--   0 wanglei    (501) staff       (20)        1 2024-04-14 04:03:31.000000 cybersailor-0.1.3/cybersailor.egg-info/dependency_links.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       34 2024-04-14 04:03:31.000000 cybersailor-0.1.3/cybersailor.egg-info/requires.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       12 2024-04-14 04:03:31.000000 cybersailor-0.1.3/cybersailor.egg-info/top_level.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       38 2024-04-14 04:03:31.589788 cybersailor-0.1.3/setup.cfg
--rw-r--r--   0 wanglei    (501) staff       (20)      562 2024-04-14 04:01:40.000000 cybersailor-0.1.3/setup.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-05-30 07:07:50.095258 cybersailor-0.1.4/
+-rw-r--r--   0 wanglei    (501) staff       (20)      372 2024-05-30 07:07:50.095079 cybersailor-0.1.4/PKG-INFO
+-rw-r--r--   0 wanglei    (501) staff       (20)       11 2024-05-30 07:03:15.000000 cybersailor-0.1.4/README.md
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-05-30 07:07:50.094293 cybersailor-0.1.4/cybersailor/
+-rw-r--r--   0 wanglei    (501) staff       (20)       50 2024-03-19 06:42:00.000000 cybersailor-0.1.4/cybersailor/__init__.py
+-rw-r--r--   0 wanglei    (501) staff       (20)      533 2024-03-20 02:22:34.000000 cybersailor-0.1.4/cybersailor/logger.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     5995 2024-05-30 07:02:04.000000 cybersailor-0.1.4/cybersailor/sdk.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-05-30 07:07:50.094903 cybersailor-0.1.4/cybersailor.egg-info/
+-rw-r--r--   0 wanglei    (501) staff       (20)      372 2024-05-30 07:07:50.000000 cybersailor-0.1.4/cybersailor.egg-info/PKG-INFO
+-rw-r--r--   0 wanglei    (501) staff       (20)      257 2024-05-30 07:07:50.000000 cybersailor-0.1.4/cybersailor.egg-info/SOURCES.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)        1 2024-05-30 07:07:50.000000 cybersailor-0.1.4/cybersailor.egg-info/dependency_links.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       34 2024-05-30 07:07:50.000000 cybersailor-0.1.4/cybersailor.egg-info/requires.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       12 2024-05-30 07:07:50.000000 cybersailor-0.1.4/cybersailor.egg-info/top_level.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       38 2024-05-30 07:07:50.095293 cybersailor-0.1.4/setup.cfg
+-rw-r--r--   0 wanglei    (501) staff       (20)      562 2024-05-30 07:03:35.000000 cybersailor-0.1.4/setup.py
```

### Comparing `cybersailor-0.1.3/cybersailor/logger.py` & `cybersailor-0.1.4/cybersailor/logger.py`

 * *Files identical despite different names*

### Comparing `cybersailor-0.1.3/cybersailor/sdk.py` & `cybersailor-0.1.4/cybersailor/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from typing import Any
 from carthooks import Client
 from .logger import Logger
+import traceback
 import os
 import time
 
 class Task:
     def __init__(self, handler, app_id, collection_id, 
                 trigger="pulling_items", 
                 filter=None, 
                 pagelimit=1,
                 include_locked=False,
                 sort=['created'], 
                 pulling_interval=30):
         self.handler = handler
         self.trigger = trigger
         self.last_pull = 0
+        self.last_pull_items = 0
         self.pulling_options = {
             "app_id": app_id,
             "collection_id": collection_id,
             "filter": filter,
             "sort": sort,
             "pulling_interval": pulling_interval,
             "pagelimit": pagelimit,
             "include_locked": include_locked
         }
     
     def pulling_now(self):
         self.last_pull = time.time()
 
     def is_pull_able(self):
+        if self.last_pull_items > 0:
+            return True
         return time.time() - self.last_pull > self.pulling_options["pulling_interval"]
 
 class Record:
     def __init__(self, sailor, app_id, collection_id, item_id, data):
         self.sailor = sailor
         self.app_id = app_id
         self.collection_id = collection_id
@@ -95,36 +99,36 @@
         return self.client.lockItem(record.app_id, record.collection_id, record.item_id, lock_timeout=lock_timeout, lock_id=self.sailor_id, subject=subject)
 
     def unlock(self, record):
         self.logger.debug(f"Unlocking task: {record}")
         return self.client.unlockItem(record.app_id, record.collection_id, record.item_id, lock_id=self.sailor_id)
 
     def update(self, task, map):
-        self.logger.debug(f"Updating task: {task} with map: {map}")
+        self.logger.info(f"Updating task: {task} with map: {map}")
         return self.client.updateItem(task.app_id, task.collection_id, task.item_id, map)
 
     def create(self, app_id, collection_id, data):
-        self.logger.debug(f"Creating record in app_id: {app_id}, collection_id: {collection_id} with data: {data}")
+        self.logger.info(f"Creating record in app_id: {app_id}, collection_id: {collection_id} with data: {data}")
         result = self.client.createItem(app_id, collection_id, data)
         return result
 
     def run(self):
         self.logger.debug("Running...")
 
         while True:
             for task in self.tasks:
                 if task.trigger == "pulling_items" and task.is_pull_able():
                     self.pull(task)
-            time.sleep(1)
+            time.sleep(0.1)
 
     def pull(self,task):
         try:
             app_id = task.pulling_options["app_id"]
             collection_id = task.pulling_options["collection_id"]
-            self.logger.debug(f"Pulling items from app_id: {app_id}, collection_id: {collection_id}")
+            self.logger.info(f"Pulling items from app_id: {app_id}, collection_id: {collection_id}")
 
             options = {
                 "limit": task.pulling_options["pagelimit"],
             }
 
             if task.pulling_options["sort"] != None:
                 options["sort"] = task.pulling_options["sort"]
@@ -136,23 +140,26 @@
 
             if task.pulling_options["include_locked"] == False:
                 options["unlockedOrLockedBy"] = self.sailor_id
 
             # print(options)
 
             result = self.client.getItems(app_id, collection_id, **options)
+            self.logger.debug(f"Result: {result}")
             
             items = result.data
             task.pulling_now()
+            task.last_pull_items = items.__len__()
             if items.__len__() > 0:
                 context = Context(sailor=self, task=task, logger=self.logger)
                 for item in items:
-                    self.logger.debug(f"Handling item: {item['id']}")
+                    self.logger.info(f"Handling item: {item['id']}")
                     record = Record(sailor=self, app_id=app_id, collection_id=collection_id, item_id=item['id'], data=item)
                     self.logger.debug(f"Record: {record}")
                     try:
                         task.handler(context, record)
                     except Exception as e:
-                        self.logger.error(f"Error: {e}")
+                        traceback.print_exc()
+                        # self.logger.error(f"Error: {e}")
         except Exception as e:
             self.logger.error(f"Error: {e}")
             time.sleep(5)
```

### Comparing `cybersailor-0.1.3/setup.py` & `cybersailor-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cybersailor',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     description='Cybersailor Python SDK',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Carthooks',
     author_email='developer@carthooks.com',
     license='MIT',
```

