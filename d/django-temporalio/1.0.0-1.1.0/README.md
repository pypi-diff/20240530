# Comparing `tmp/django_temporalio-1.0.0.tar.gz` & `tmp/django_temporalio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_temporalio-1.0.0.tar", last modified: Thu May 16 16:14:35 2024, max compression
+gzip compressed data, was "django_temporalio-1.1.0.tar", last modified: Thu May 30 16:39:00 2024, max compression
```

## Comparing `django_temporalio-1.0.0.tar` & `django_temporalio-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:35.800871 django_temporalio-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-16 16:14:35.800871 django_temporalio-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:35.800871 django_temporalio-1.0.0/django_temporalio/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/django_temporalio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/django_temporalio/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/django_temporalio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/django_temporalio/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:35.800871 django_temporalio-1.0.0/django_temporalio/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/django_temporalio/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:35.800871 django_temporalio-1.0.0/django_temporalio/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/django_temporalio/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/django_temporalio/management/commands/show_temporalio_queue_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/django_temporalio/management/commands/start_temporalio_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/django_temporalio/management/commands/sync_temporalio_schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/django_temporalio/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:35.800871 django_temporalio-1.0.0/django_temporalio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-16 16:14:35.000000 django_temporalio-1.0.0/django_temporalio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-16 16:14:35.000000 django_temporalio-1.0.0/django_temporalio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:14:35.000000 django_temporalio-1.0.0/django_temporalio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 16:14:35.000000 django_temporalio-1.0.0/django_temporalio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 16:14:35.000000 django_temporalio-1.0.0/django_temporalio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 16:14:35.800871 django_temporalio-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-16 16:14:33.000000 django_temporalio-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:39:00.259482 django_temporalio-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-30 16:39:00.259482 django_temporalio-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:39:00.255482 django_temporalio-1.1.0/django_temporalio/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:39:00.255482 django_temporalio-1.1.0/django_temporalio/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:39:00.255482 django_temporalio-1.1.0/django_temporalio/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/management/commands/show_temporalio_queue_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/management/commands/start_temporalio_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/management/commands/sync_temporalio_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/django_temporalio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:39:00.259482 django_temporalio-1.1.0/django_temporalio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-30 16:39:00.000000 django_temporalio-1.1.0/django_temporalio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-30 16:39:00.000000 django_temporalio-1.1.0/django_temporalio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:39:00.000000 django_temporalio-1.1.0/django_temporalio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-30 16:39:00.000000 django_temporalio-1.1.0/django_temporalio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 16:39:00.000000 django_temporalio-1.1.0/django_temporalio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 16:39:00.259482 django_temporalio-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-30 16:38:57.000000 django_temporalio-1.1.0/setup.py
```

### Comparing `django_temporalio-1.0.0/LICENSE` & `django_temporalio-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_temporalio-1.0.0/PKG-INFO` & `django_temporalio-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-temporalio
-Version: 1.0.0
+Version: 1.1.0
 Summary: Temporal.io integration for Django
 Home-page: https://github.com/RegioHelden/django-temporalio
 Download-URL: 
 Author: RegioHelden GmbH
 Author-email: opensource@regiohelden.de
 License: MIT
 Keywords: django,temporal.io,temporal
@@ -54,32 +54,39 @@
 Add the following settings to your `settings.py`:
 
 ```python
 from temporalio.worker import WorkerConfig
 
 DJANGO_TEMPORALIO = {
     "URL": "localhost:7233",
+    "BASE_MODULE": "path.to.module",
     "WORKER_CONFIGS": {
         "main": WorkerConfig(
             task_queue="MAIN_TASK_QUEUE",
             ...
         ),
         ...
     },
 }
 ```
 
 ## Usage
 
+Activities, workflows and schedules should be placed inside the base module defined by the `BASE_MODULE` setting, 
+preferably outside of any Django application, in order to keep the uses of 
+the [imports_passed_through](https://python.temporal.io/temporalio.workflow.unsafe.html) context manager encapsulated 
+inside the module, along with Temporal.io related code.
+
 ### Workflow and Activity Registry
 
 The registry is a singleton that holds mappings between queue names and registered activities and workflows.
 You can register activities and workflows using the `register` method. 
 
-Activities and workflows should be declared in `workflows.py` and `activities.py` modules respectively. 
+Activities and workflows should be declared in modules matching the following patterns `*workflows*.py` and 
+`*activities*.py` respectively. 
 
 ```python
 from temporalio import activity, workflow
 from django_temporalio.registry import queue_activities, queue_workflows
 
 @queue_activities.register("HIGH_PRIORITY_TASK_QUEUE", "MAIN_TASK_QUEUE")
 @activity.defn
@@ -144,12 +151,13 @@
 
 DJANGO_TEMPORALIO: A dictionary containing the following keys:
 
 - URL: The Temporal.io host to connect to, defaults to `http://localhost:7233`
 - NAMESPACE: The Temporal.io namespace to use, defaults to `default`
 - WORKER_CONFIGS: A dictionary containing worker configurations. 
   The key is the worker name and the value is a `WorkerConfig` instance.
+- BASE_MODULE: A python module that holds workflows, activities and schedules, defaults to `None`
 
 
 ## 1.0.0 (2024-05-16)
 
 * Initial release
```

### Comparing `django_temporalio-1.0.0/README.md` & `django_temporalio-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -29,32 +29,39 @@
 Add the following settings to your `settings.py`:
 
 ```python
 from temporalio.worker import WorkerConfig
 
 DJANGO_TEMPORALIO = {
     "URL": "localhost:7233",
+    "BASE_MODULE": "path.to.module",
     "WORKER_CONFIGS": {
         "main": WorkerConfig(
             task_queue="MAIN_TASK_QUEUE",
             ...
         ),
         ...
     },
 }
 ```
 
 ## Usage
 
+Activities, workflows and schedules should be placed inside the base module defined by the `BASE_MODULE` setting, 
+preferably outside of any Django application, in order to keep the uses of 
+the [imports_passed_through](https://python.temporal.io/temporalio.workflow.unsafe.html) context manager encapsulated 
+inside the module, along with Temporal.io related code.
+
 ### Workflow and Activity Registry
 
 The registry is a singleton that holds mappings between queue names and registered activities and workflows.
 You can register activities and workflows using the `register` method. 
 
-Activities and workflows should be declared in `workflows.py` and `activities.py` modules respectively. 
+Activities and workflows should be declared in modules matching the following patterns `*workflows*.py` and 
+`*activities*.py` respectively. 
 
 ```python
 from temporalio import activity, workflow
 from django_temporalio.registry import queue_activities, queue_workflows
 
 @queue_activities.register("HIGH_PRIORITY_TASK_QUEUE", "MAIN_TASK_QUEUE")
 @activity.defn
@@ -119,7 +126,8 @@
 
 DJANGO_TEMPORALIO: A dictionary containing the following keys:
 
 - URL: The Temporal.io host to connect to, defaults to `http://localhost:7233`
 - NAMESPACE: The Temporal.io namespace to use, defaults to `default`
 - WORKER_CONFIGS: A dictionary containing worker configurations. 
   The key is the worker name and the value is a `WorkerConfig` instance.
+- BASE_MODULE: A python module that holds workflows, activities and schedules, defaults to `None`
```

### Comparing `django_temporalio-1.0.0/django_temporalio/conf.py` & `django_temporalio-1.1.0/django_temporalio/conf.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,17 +16,22 @@
 from django.dispatch import receiver
 
 SETTINGS_KEY = "DJANGO_TEMPORALIO"
 DEFAULTS = {
     "URL": "http://localhost:7233",
     "NAMESPACE": "default",
     "WORKER_CONFIGS": {},
+    "BASE_MODULE": None,
 }
 
 
+class SettingIsNotSetError(Exception):
+    pass
+
+
 class Settings:
     def __init__(self):
         self.defaults = DEFAULTS
 
     @property
     def user_settings(self):
         if not hasattr(self, "_user_settings"):
```

### Comparing `django_temporalio-1.0.0/django_temporalio/management/commands/show_temporalio_queue_registry.py` & `django_temporalio-1.1.0/django_temporalio/management/commands/show_temporalio_queue_registry.py`

 * *Files identical despite different names*

### Comparing `django_temporalio-1.0.0/django_temporalio/management/commands/start_temporalio_worker.py` & `django_temporalio-1.1.0/django_temporalio/management/commands/start_temporalio_worker.py`

 * *Files identical despite different names*

### Comparing `django_temporalio-1.0.0/django_temporalio/management/commands/sync_temporalio_schedules.py` & `django_temporalio-1.1.0/django_temporalio/management/commands/sync_temporalio_schedules.py`

 * *Files identical despite different names*

### Comparing `django_temporalio-1.0.0/django_temporalio/registry.py` & `django_temporalio-1.1.0/django_temporalio/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass, field
 from functools import wraps
 from typing import Callable, Sequence, Type
 
-from django.utils.module_loading import autodiscover_modules
 from temporalio.client import Schedule
 
+from django_temporalio.utils import autodiscover_modules
+
 
 class ScheduleRegistry:
     _registry: dict[str, Schedule]
 
     class AlreadyRegistered(Exception):
         pass
 
@@ -22,15 +23,15 @@
         if schedule_id in self._registry:
             raise self.AlreadyRegistered(
                 f"Schedule with ID '{schedule_id}' is already registered.",
             )
         self._registry[schedule_id] = schedule
 
     def get_registry(self):
-        autodiscover_modules("schedules")
+        autodiscover_modules("*schedules*")
         return self._registry
 
     def clear_registry(self):
         self._init_registry()
 
 
 class QueueRegistry:
@@ -81,16 +82,16 @@
 
     def get_registry(self):
         autodiscover_modules(self.module_name)
         return self._registry
 
 
 schedules = ScheduleRegistry()
-queue_workflows = QueueRegistry("workflows", "__temporal_workflow_definition")
-queue_activities = QueueRegistry("activities", "__temporal_activity_definition")
+queue_workflows = QueueRegistry("*workflows*", "__temporal_workflow_definition")
+queue_activities = QueueRegistry("*activities*", "__temporal_activity_definition")
 
 
 @dataclass
 class QueueRegistryItem:
     workflows: Sequence[Type] = field(default_factory=list)
     activities: Sequence[Callable] = field(default_factory=list)
```

### Comparing `django_temporalio-1.0.0/django_temporalio.egg-info/PKG-INFO` & `django_temporalio-1.1.0/django_temporalio.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-temporalio
-Version: 1.0.0
+Version: 1.1.0
 Summary: Temporal.io integration for Django
 Home-page: https://github.com/RegioHelden/django-temporalio
 Download-URL: 
 Author: RegioHelden GmbH
 Author-email: opensource@regiohelden.de
 License: MIT
 Keywords: django,temporal.io,temporal
@@ -54,32 +54,39 @@
 Add the following settings to your `settings.py`:
 
 ```python
 from temporalio.worker import WorkerConfig
 
 DJANGO_TEMPORALIO = {
     "URL": "localhost:7233",
+    "BASE_MODULE": "path.to.module",
     "WORKER_CONFIGS": {
         "main": WorkerConfig(
             task_queue="MAIN_TASK_QUEUE",
             ...
         ),
         ...
     },
 }
 ```
 
 ## Usage
 
+Activities, workflows and schedules should be placed inside the base module defined by the `BASE_MODULE` setting, 
+preferably outside of any Django application, in order to keep the uses of 
+the [imports_passed_through](https://python.temporal.io/temporalio.workflow.unsafe.html) context manager encapsulated 
+inside the module, along with Temporal.io related code.
+
 ### Workflow and Activity Registry
 
 The registry is a singleton that holds mappings between queue names and registered activities and workflows.
 You can register activities and workflows using the `register` method. 
 
-Activities and workflows should be declared in `workflows.py` and `activities.py` modules respectively. 
+Activities and workflows should be declared in modules matching the following patterns `*workflows*.py` and 
+`*activities*.py` respectively. 
 
 ```python
 from temporalio import activity, workflow
 from django_temporalio.registry import queue_activities, queue_workflows
 
 @queue_activities.register("HIGH_PRIORITY_TASK_QUEUE", "MAIN_TASK_QUEUE")
 @activity.defn
@@ -144,12 +151,13 @@
 
 DJANGO_TEMPORALIO: A dictionary containing the following keys:
 
 - URL: The Temporal.io host to connect to, defaults to `http://localhost:7233`
 - NAMESPACE: The Temporal.io namespace to use, defaults to `default`
 - WORKER_CONFIGS: A dictionary containing worker configurations. 
   The key is the worker name and the value is a `WorkerConfig` instance.
+- BASE_MODULE: A python module that holds workflows, activities and schedules, defaults to `None`
 
 
 ## 1.0.0 (2024-05-16)
 
 * Initial release
```

### Comparing `django_temporalio-1.0.0/django_temporalio.egg-info/SOURCES.txt` & `django_temporalio-1.1.0/django_temporalio.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 setup.py
 django_temporalio/__init__.py
 django_temporalio/apps.py
 django_temporalio/client.py
 django_temporalio/conf.py
 django_temporalio/registry.py
+django_temporalio/utils.py
 django_temporalio.egg-info/PKG-INFO
 django_temporalio.egg-info/SOURCES.txt
 django_temporalio.egg-info/dependency_links.txt
 django_temporalio.egg-info/requires.txt
 django_temporalio.egg-info/top_level.txt
 django_temporalio/management/__init__.py
 django_temporalio/management/commands/__init__.py
```

### Comparing `django_temporalio-1.0.0/setup.py` & `django_temporalio-1.1.0/setup.py`

 * *Files identical despite different names*

