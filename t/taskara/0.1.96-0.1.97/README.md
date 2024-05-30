# Comparing `tmp/taskara-0.1.96.tar.gz` & `tmp/taskara-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.96.tar", max compression
+gzip compressed data, was "taskara-0.1.97.tar", max compression
```

## Comparing `taskara-0.1.96.tar` & `taskara-0.1.97.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.96/LICENSE
--rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.96/README.md
--rw-r--r--   0        0        0     1171 2024-05-29 03:09:00.193396 taskara-0.1.96/pyproject.toml
--rw-r--r--   0        0        0      349 2024-05-28 21:17:06.610377 taskara-0.1.96/taskara/__init__.py
--rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.96/taskara/agent.py
--rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.96/taskara/auth/default.py
--rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.96/taskara/auth/key.py
--rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.96/taskara/auth/provider.py
--rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.96/taskara/auth/transport.py
--rw-r--r--   0        0        0    17809 2024-05-28 21:17:06.610669 taskara-0.1.96/taskara/benchmark.py
--rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.96/taskara/cli/main.py
--rw-r--r--   0        0        0      672 2024-05-23 03:23:29.445785 taskara-0.1.96/taskara/config.py
--rw-r--r--   0        0        0     2129 2024-05-28 21:17:06.610948 taskara-0.1.96/taskara/db/conn.py
--rw-r--r--   0        0        0     4040 2024-05-28 21:17:06.611322 taskara-0.1.96/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.96/taskara/env.py
--rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.96/taskara/metrics.py
--rw-r--r--   0        0        0    12137 2024-05-23 03:59:01.085005 taskara-0.1.96/taskara/runtime/base.py
--rw-r--r--   0        0        0    14316 2024-05-23 03:44:21.827171 taskara-0.1.96/taskara/runtime/docker.py
--rw-r--r--   0        0        0    30788 2024-05-28 21:17:06.611714 taskara-0.1.96/taskara/runtime/kube.py
--rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.96/taskara/runtime/load.py
--rw-r--r--   0        0        0    16258 2024-05-23 03:34:03.416381 taskara-0.1.96/taskara/runtime/process.py
--rw-r--r--   0        0        0     2340 2024-05-28 21:17:06.612057 taskara-0.1.96/taskara/server/app.py
--rw-r--r--   0        0        0     4143 2024-05-29 03:08:44.355605 taskara-0.1.96/taskara/server/models.py
--rw-r--r--   0        0        0     3703 2024-05-28 21:17:06.612655 taskara-0.1.96/taskara/server/router/benchmarks.py
--rw-r--r--   0        0        0     8554 2024-05-23 21:06:30.131717 taskara-0.1.96/taskara/server/router/tasks.py
--rw-r--r--   0        0        0    36744 2024-05-28 22:48:29.514940 taskara-0.1.96/taskara/task.py
--rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.96/taskara/util.py
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 taskara-0.1.96/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.97/LICENSE
+-rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.97/README.md
+-rw-r--r--   0        0        0     1193 2024-05-30 18:04:59.149675 taskara-0.1.97/pyproject.toml
+-rw-r--r--   0        0        0      349 2024-05-28 21:17:06.610377 taskara-0.1.97/taskara/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.97/taskara/agent.py
+-rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.97/taskara/auth/default.py
+-rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.97/taskara/auth/key.py
+-rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.97/taskara/auth/provider.py
+-rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.97/taskara/auth/transport.py
+-rw-r--r--   0        0        0    17891 2024-05-30 18:00:40.096971 taskara-0.1.97/taskara/benchmark.py
+-rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.97/taskara/cli/main.py
+-rw-r--r--   0        0        0      672 2024-05-23 03:23:29.445785 taskara-0.1.97/taskara/config.py
+-rw-r--r--   0        0        0     2129 2024-05-28 21:17:06.610948 taskara-0.1.97/taskara/db/conn.py
+-rw-r--r--   0        0        0     4040 2024-05-28 21:17:06.611322 taskara-0.1.97/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.97/taskara/env.py
+-rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.97/taskara/metrics.py
+-rw-r--r--   0        0        0    12137 2024-05-23 03:59:01.085005 taskara-0.1.97/taskara/runtime/base.py
+-rw-r--r--   0        0        0    14316 2024-05-23 03:44:21.827171 taskara-0.1.97/taskara/runtime/docker.py
+-rw-r--r--   0        0        0    30788 2024-05-28 21:17:06.611714 taskara-0.1.97/taskara/runtime/kube.py
+-rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.97/taskara/runtime/load.py
+-rw-r--r--   0        0        0    16258 2024-05-23 03:34:03.416381 taskara-0.1.97/taskara/runtime/process.py
+-rw-r--r--   0        0        0     2340 2024-05-28 21:17:06.612057 taskara-0.1.97/taskara/server/app.py
+-rw-r--r--   0        0        0     4143 2024-05-29 03:08:44.355605 taskara-0.1.97/taskara/server/models.py
+-rw-r--r--   0        0        0     3703 2024-05-28 21:17:06.612655 taskara-0.1.97/taskara/server/router/benchmarks.py
+-rw-r--r--   0        0        0     8554 2024-05-23 21:06:30.131717 taskara-0.1.97/taskara/server/router/tasks.py
+-rw-r--r--   0        0        0    36744 2024-05-28 22:48:29.514940 taskara-0.1.97/taskara/task.py
+-rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.97/taskara/util.py
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 taskara-0.1.97/PKG-INFO
```

### Comparing `taskara-0.1.96/LICENSE` & `taskara-0.1.97/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/README.md` & `taskara-0.1.97/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/pyproject.toml` & `taskara-0.1.97/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskara"
-version = "0.1.96"
+version = "0.1.97"
 description = "Task management for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -23,14 +23,15 @@
 skillpacks = "^0.1.31"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 flake8 = "^7.0.0"
 black = "^24.2.0"
 pytest-env = "^1.1.3"
+ipykernel = "^6.29.4"
 
 [tool.poetry.extras]
 runtime = ["kubernetes", "docker", "google-auth", "google-cloud-container"]
 cli = ["typer", "tabulate"]
 all = ["kubernetes", "docker", "google-auth", "google-cloud-container", "typer", "tabulate"]
 
 [build-system]
```

### Comparing `taskara-0.1.96/taskara/agent.py` & `taskara-0.1.97/taskara/agent.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/auth/key.py` & `taskara-0.1.97/taskara/auth/key.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/auth/provider.py` & `taskara-0.1.97/taskara/auth/provider.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/auth/transport.py` & `taskara-0.1.97/taskara/auth/transport.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/benchmark.py` & `taskara-0.1.97/taskara/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,15 +525,18 @@
             assigned_type=self._assigned_type,
             owner_id=self._owner_id,
         )
 
     @classmethod
     def from_v1(cls, v1: V1Eval, owner_id: Optional[str] = None) -> "Eval":
         benchmark = Benchmark.from_v1(v1.benchmark, owner_id=owner_id)
-        tasks = [Task.from_v1(task) for task in v1.tasks]
+        tasks = [
+            Task.from_v1(task, owner_id=owner_id if owner_id else v1.owner_id)
+            for task in v1.tasks
+        ]
 
         obj = cls.__new__(cls)
         obj._id = v1.id if v1.id else shortuuid.uuid()
         obj._benchmark = benchmark
         obj._tasks = tasks
         obj._owner_id = owner_id if owner_id else v1.owner_id
         obj._assigned_to = v1.assigned_to
```

### Comparing `taskara-0.1.96/taskara/cli/main.py` & `taskara-0.1.97/taskara/cli/main.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/config.py` & `taskara-0.1.97/taskara/config.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/db/conn.py` & `taskara-0.1.97/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/db/models.py` & `taskara-0.1.97/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/metrics.py` & `taskara-0.1.97/taskara/metrics.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/runtime/base.py` & `taskara-0.1.97/taskara/runtime/base.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/runtime/docker.py` & `taskara-0.1.97/taskara/runtime/docker.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/runtime/kube.py` & `taskara-0.1.97/taskara/runtime/kube.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/runtime/load.py` & `taskara-0.1.97/taskara/runtime/load.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/runtime/process.py` & `taskara-0.1.97/taskara/runtime/process.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/server/app.py` & `taskara-0.1.97/taskara/server/app.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/server/models.py` & `taskara-0.1.97/taskara/server/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/server/router/benchmarks.py` & `taskara-0.1.97/taskara/server/router/benchmarks.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/server/router/tasks.py` & `taskara-0.1.97/taskara/server/router/tasks.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/task.py` & `taskara-0.1.97/taskara/task.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/taskara/util.py` & `taskara-0.1.97/taskara/util.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.96/PKG-INFO` & `taskara-0.1.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.96
+Version: 0.1.97
 Summary: Task management for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskara Version: 0.1.96 Summary: Task management
+Metadata-Version: 2.1 Name: taskara Version: 0.1.97 Summary: Task management
 for AI agents License: MIT Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: cli Provides-
 Extra: runtime Requires-Dist: devicebay (>=0.1.25,<0.2.0) Requires-Dist: docker
 (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all" Requires-Dist: google-
```

