# Comparing `tmp/pytest_dashboard-0.1.0.tar.gz` & `tmp/pytest_dashboard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dashboard-0.1.0.tar", max compression
+gzip compressed data, was "pytest_dashboard-0.1.1.tar", max compression
```

## Comparing `pytest_dashboard-0.1.0.tar` & `pytest_dashboard-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1495 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/LICENSE
--rw-r--r--   0        0        0     1642 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/README.md
--rw-r--r--   0        0        0      770 2024-05-29 06:12:47.703161 pytest_dashboard-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       21 2024-05-29 06:12:47.703161 pytest_dashboard-0.1.0/pytest_dashboard/__init__.py
--rw-r--r--   0        0        0     4183 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/pytest_dashboard/_tally_progresses.py
--rw-r--r--   0        0        0      216 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/pytest_dashboard/config.py
--rw-r--r--   0        0        0     2184 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/pytest_dashboard/conftest.py
--rw-r--r--   0        0        0      165 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/pytest_dashboard/tally.py
--rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 pytest_dashboard-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1495 2024-05-29 07:32:46.165117 pytest_dashboard-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1728 2024-05-29 07:32:46.165117 pytest_dashboard-0.1.1/README.md
+-rw-r--r--   0        0        0      770 2024-05-29 07:32:59.820996 pytest_dashboard-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-29 07:32:59.820996 pytest_dashboard-0.1.1/pytest_dashboard/__init__.py
+-rw-r--r--   0        0        0     4327 2024-05-29 07:32:46.165117 pytest_dashboard-0.1.1/pytest_dashboard/_tally_progresses.py
+-rw-r--r--   0        0        0      216 2024-05-29 07:32:46.165117 pytest_dashboard-0.1.1/pytest_dashboard/config.py
+-rw-r--r--   0        0        0     2184 2024-05-29 07:32:46.165117 pytest_dashboard-0.1.1/pytest_dashboard/conftest.py
+-rw-r--r--   0        0        0      165 2024-05-29 07:32:46.165117 pytest_dashboard-0.1.1/pytest_dashboard/tally.py
+-rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 pytest_dashboard-0.1.1/PKG-INFO
```

### Comparing `pytest_dashboard-0.1.0/LICENSE` & `pytest_dashboard-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_dashboard-0.1.0/README.md` & `pytest_dashboard-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,34 +7,50 @@
     - You will get a `sample-progress.yaml` file.
 - Run pytest dashboard
     - i.e.) `tally-pytest <path_to_project>\sample-tests`
     - You will get a `entire-progress.yaml` file in working folder.
 
 ## usage
 `pytest`
-by this command, you get `[datetime]-progress.yaml` file on working directory as realtime pytest progress report.
+
+By this command, you get `[datetime]-progress.yaml` file on working directory as realtime pytest progress report.
+
+---
 
 `pytest --progress-path=[path/to/some-progress.yaml]`
-by this command, you get `path/to/some-progress.yaml` file.
+
+By this command, you get `path/to/some-progress.yaml` file.
 The value should end with `-progress.yaml`.
 
+---
+
 `tally-pytest PROGRESSES_DIR --entire_progress_path=[path/to/entire-progress.yaml]`
-by this command, you get started to monitor changes of
+
+By this command, you get started to monitor changes of
 the progress files (ends with `-progress.yaml`)
 inside `PROGRESS_DIR` and save the state summary
 to `path/to/entire-progress.yaml`.
 
 So it is necessary to set `--progress-path` option of pytest
 ending with `-progress.yaml`.
 For example, `2024-04-22-progress.yaml`,
 
-> **Note**
+> [!NOTE]
 > if your `entire_progress_path` is ends with `-progress.yaml`,
 > you cannot save the entire progress file to
 > the same directory with each progress file.
 
+---
+
 `tally-pytest PROGRESS_DIR --notification=True`
+
 By this command, you will get mail notification when entire progress is finished.
-> **Note**
+> [!NOTE]
 > Please implement pytest_dashboard.config
 > that contains information abaout mail address and SMTP server.
 > This command works with powershell `Send-MailMessage` command.
+
+---
+
+`tally-pytest PROGRESS_DIR --dashboart=True`
+
+Not implemented!
```

### Comparing `pytest_dashboard-0.1.0/pyproject.toml` & `pytest_dashboard-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-dashboard"
-version = "0.1.0"  # ignored by versioning plugin
+version = "0.1.1"  # ignored by versioning plugin
 description = ""
 authors = ["kazuma.naito <kazuma.naito@murata.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/pyfemtet/pytest-dashboard"
 
 [tool.poetry.dependencies]
```

### Comparing `pytest_dashboard-0.1.0/pytest_dashboard/_tally_progresses.py` & `pytest_dashboard-0.1.1/pytest_dashboard/_tally_progresses.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,24 +22,27 @@
 
 
 def _progress_passed(data) -> bool:
     # if empty, return False
     if data is None:
         return False
 
+    # if not started, return False
+    if data['results'] is None:
+        return False
+
     # if all(results), return True
     passed_list = []
     for result in data['results']:
         name = result['name']
         setup = result['setup'] if 'setup' in result.keys() else None
         call = result['call'] if 'call' in result.keys() else None
         teardown = result['teardown'] if 'teardown' in result.keys() else None
         passed = True
         if setup is not None:
-
             passed = passed * (setup == 'passed')
         if call is not None:
             passed = passed * (call == 'passed')
         if teardown is not None:
             passed = passed * (teardown == 'passed')
         passed_list.append(passed)
     return all(passed_list)
@@ -47,19 +50,20 @@
 
 def _progress_state(data) -> str:
     # if empty, not started
     if data is None:
         return 'not started'
 
     # if len(items) == len(results) and data['results'][-1] has the key 'teardown', finished
-    if (
-            len(data['items']) == len(data['results'])
-            and 'teardown' in data['results'][-1].keys()
-    ):
-        return 'finished'
+    if data['results'] is not None:
+        if (
+                len(data['items']) == len(data['results'])
+                and 'teardown' in data['results'][-1].keys()
+        ):
+            return 'finished'
 
     # else, ongoing
     return 'ongoing'
 
 
 def _check_notification(data):
```

### Comparing `pytest_dashboard-0.1.0/pytest_dashboard/conftest.py` & `pytest_dashboard-0.1.1/pytest_dashboard/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_dashboard-0.1.0/PKG-INFO` & `pytest_dashboard-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dashboard
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/pyfemtet/pytest-dashboard
 License: BSD-3-Clause
 Author: kazuma.naito
 Author-email: kazuma.naito@murata.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
@@ -28,35 +28,51 @@
     - You will get a `sample-progress.yaml` file.
 - Run pytest dashboard
     - i.e.) `tally-pytest <path_to_project>\sample-tests`
     - You will get a `entire-progress.yaml` file in working folder.
 
 ## usage
 `pytest`
-by this command, you get `[datetime]-progress.yaml` file on working directory as realtime pytest progress report.
+
+By this command, you get `[datetime]-progress.yaml` file on working directory as realtime pytest progress report.
+
+---
 
 `pytest --progress-path=[path/to/some-progress.yaml]`
-by this command, you get `path/to/some-progress.yaml` file.
+
+By this command, you get `path/to/some-progress.yaml` file.
 The value should end with `-progress.yaml`.
 
+---
+
 `tally-pytest PROGRESSES_DIR --entire_progress_path=[path/to/entire-progress.yaml]`
-by this command, you get started to monitor changes of
+
+By this command, you get started to monitor changes of
 the progress files (ends with `-progress.yaml`)
 inside `PROGRESS_DIR` and save the state summary
 to `path/to/entire-progress.yaml`.
 
 So it is necessary to set `--progress-path` option of pytest
 ending with `-progress.yaml`.
 For example, `2024-04-22-progress.yaml`,
 
-> **Note**
+> [!NOTE]
 > if your `entire_progress_path` is ends with `-progress.yaml`,
 > you cannot save the entire progress file to
 > the same directory with each progress file.
 
+---
+
 `tally-pytest PROGRESS_DIR --notification=True`
+
 By this command, you will get mail notification when entire progress is finished.
-> **Note**
+> [!NOTE]
 > Please implement pytest_dashboard.config
 > that contains information abaout mail address and SMTP server.
 > This command works with powershell `Send-MailMessage` command.
 
+---
+
+`tally-pytest PROGRESS_DIR --dashboart=True`
+
+Not implemented!
+
```

