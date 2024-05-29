# Comparing `tmp/virtool_workflow-6.0.0a9.tar.gz` & `tmp/virtool_workflow-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtool_workflow-6.0.0a9.tar", max compression
+gzip compressed data, was "virtool_workflow-7.0.0.tar", max compression
```

## Comparing `virtool_workflow-6.0.0a9.tar` & `virtool_workflow-7.0.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0     1097 2024-01-19 00:48:36.663114 virtool_workflow-6.0.0a9/LICENSE
--rw-r--r--   0        0        0     3430 2024-01-19 00:48:36.663114 virtool_workflow-6.0.0a9/README.md
--rw-r--r--   0        0        0     1433 2024-01-19 00:48:55.435255 virtool_workflow-6.0.0a9/pyproject.toml
--rw-r--r--   0        0        0      308 2024-01-19 00:48:37.771122 virtool_workflow-6.0.0a9/virtool_workflow/__init__.py
--rw-r--r--   0        0        0       57 2024-01-19 00:48:37.771122 virtool_workflow-6.0.0a9/virtool_workflow/analysis/__init__.py
--rw-r--r--   0        0        0    13149 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/analysis/fastqc.py
--rw-r--r--   0        0        0     7130 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/analysis/skewer.py
--rw-r--r--   0        0        0     1447 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/analysis/trimming.py
--rw-r--r--   0        0        0     1108 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/analysis/utils.py
--rw-r--r--   0        0        0        0 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/api/__init__.py
--rw-r--r--   0        0        0     2134 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/api/acquire.py
--rw-r--r--   0        0        0     4604 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/api/client.py
--rw-r--r--   0        0        0     3083 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/api/utils.py
--rw-r--r--   0        0        0     1441 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/cli.py
--rw-r--r--   0        0        0      610 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/data/__init__.py
--rw-r--r--   0        0        0     3117 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/data/analyses.py
--rw-r--r--   0        0        0     3234 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/data/hmms.py
--rw-r--r--   0        0        0     8997 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/data/indexes.py
--rw-r--r--   0        0        0     1667 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/data/jobs.py
--rw-r--r--   0        0        0     2190 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/data/ml.py
--rw-r--r--   0        0        0     4899 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/data/samples.py
--rw-r--r--   0        0        0     7242 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/data/subtractions.py
--rw-r--r--   0        0        0      905 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/data/uploads.py
--rw-r--r--   0        0        0     1274 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/decorators.py
--rw-r--r--   0        0        0     1152 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/errors.py
--rw-r--r--   0        0        0      384 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/files.py
--rw-r--r--   0        0        0     2683 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/hooks.py
--rw-r--r--   0        0        0      174 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/pytest_plugin/__init__.py
--rw-r--r--   0        0        0     5602 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/pytest_plugin/data.py
--rw-r--r--   0        0        0      229 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/pytest_plugin/subprocess.py
--rw-r--r--   0        0        0      211 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/pytest_plugin/utils.py
--rw-r--r--   0        0        0        0 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/__init__.py
--rw-r--r--   0        0        0      546 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/config.py
--rw-r--r--   0        0        0     2933 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/discover.py
--rw-r--r--   0        0        0      138 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/events.py
--rw-r--r--   0        0        0     4328 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/hook.py
--rw-r--r--   0        0        0      562 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/path.py
--rw-r--r--   0        0        0     1434 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/ping.py
--rw-r--r--   0        0        0     1601 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/redis.py
--rw-r--r--   0        0        0     8192 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/run.py
--rw-r--r--   0        0        0     4270 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/run_subprocess.py
--rw-r--r--   0        0        0      744 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/runtime/sentry.py
--rw-r--r--   0        0        0      818 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/utils.py
--rw-r--r--   0        0        0     2655 2024-01-19 00:48:37.775122 virtool_workflow-6.0.0a9/virtool_workflow/workflow.py
--rw-r--r--   0        0        0     4414 1970-01-01 00:00:00.000000 virtool_workflow-6.0.0a9/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-29 22:35:19.616876 virtool_workflow-7.0.0/LICENSE
+-rw-r--r--   0        0        0      969 2024-05-29 22:35:19.616876 virtool_workflow-7.0.0/README.md
+-rw-r--r--   0        0        0     1600 2024-05-29 22:35:44.804936 virtool_workflow-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0      308 2024-05-29 22:35:20.732878 virtool_workflow-7.0.0/virtool_workflow/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-29 22:35:20.732878 virtool_workflow-7.0.0/virtool_workflow/analysis/__init__.py
+-rw-r--r--   0        0        0    13149 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/analysis/fastqc.py
+-rw-r--r--   0        0        0     7130 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/analysis/skewer.py
+-rw-r--r--   0        0        0     1447 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/analysis/trimming.py
+-rw-r--r--   0        0        0     1108 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/analysis/utils.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/api/__init__.py
+-rw-r--r--   0        0        0     2134 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/api/acquire.py
+-rw-r--r--   0        0        0     4604 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/api/client.py
+-rw-r--r--   0        0        0     3083 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/api/utils.py
+-rw-r--r--   0        0        0     1441 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/cli.py
+-rw-r--r--   0        0        0      610 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/data/__init__.py
+-rw-r--r--   0        0        0     3117 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/data/analyses.py
+-rw-r--r--   0        0        0     3234 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/data/hmms.py
+-rw-r--r--   0        0        0     8997 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/data/indexes.py
+-rw-r--r--   0        0        0     1667 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/data/jobs.py
+-rw-r--r--   0        0        0     2190 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/data/ml.py
+-rw-r--r--   0        0        0     4899 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/data/samples.py
+-rw-r--r--   0        0        0     7242 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/data/subtractions.py
+-rw-r--r--   0        0        0      905 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/data/uploads.py
+-rw-r--r--   0        0        0     1274 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/decorators.py
+-rw-r--r--   0        0        0     1152 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/errors.py
+-rw-r--r--   0        0        0      384 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/files.py
+-rw-r--r--   0        0        0     2683 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/hooks.py
+-rw-r--r--   0        0        0      740 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0     5606 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/pytest_plugin/data.py
+-rw-r--r--   0        0        0      211 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/pytest_plugin/utils.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/__init__.py
+-rw-r--r--   0        0        0      546 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/config.py
+-rw-r--r--   0        0        0     2933 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/discover.py
+-rw-r--r--   0        0        0      138 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/events.py
+-rw-r--r--   0        0        0     4328 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/hook.py
+-rw-r--r--   0        0        0      562 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/path.py
+-rw-r--r--   0        0        0     1434 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/ping.py
+-rw-r--r--   0        0        0     1806 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/redis.py
+-rw-r--r--   0        0        0     8214 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/run.py
+-rw-r--r--   0        0        0     4757 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/run_subprocess.py
+-rw-r--r--   0        0        0      755 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/runtime/sentry.py
+-rw-r--r--   0        0        0     1089 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/utils.py
+-rw-r--r--   0        0        0     2655 2024-05-29 22:35:20.736878 virtool_workflow-7.0.0/virtool_workflow/workflow.py
+-rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 virtool_workflow-7.0.0/PKG-INFO
```

### Comparing `virtool_workflow-6.0.0a9/LICENSE` & `virtool_workflow-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/pyproject.toml` & `virtool_workflow-7.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,65 @@
 [tool.poetry]
 name = "virtool-workflow"
-version = "6.0.0-alpha.9"
+version = "7.0.0"
 description = "A framework for developing bioinformatics workflows for Virtool."
-authors = ["Ian Boyes", "Blake Smith", "Ryan Fang"]
+authors = [
+    "Ian Boyes",
+    "Blake Smith",
+    "Ryan Fang",
+    "Matt Curtis",
+    "Aman Monga",
+    "Bryce Davidson",
+    "Christine Wong Chong",
+    "Lilly Roberts",
+    "Markus Swoveland",
+    "Ryan Fang",
+]
 license = "MIT"
+maintainers = [
+    "Ian Boyes",
+    "Reece Hoffman"
+]
 readme = "README.md"
 repository = "https://github.com/virtool/virtool-workflow"
 classifiers = [
-    "Topic :: Software Development :: Libraries",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.12",
 ]
 packages = [
     { include = "virtool_workflow" },
 ]
 
 [tool.poetry.dependencies]
-python = "~3.10"
-click = "^8.1.7"
-aiohttp = "^3.8.1"
+python = "^3.10,<3.13"
 aiofiles = "^0.7.0"
-virtool-core = "^11.0.0"
-aioredis = "1.3.1"
-sentry-sdk = "^1.5.7"
-pyfixtures = "^1.0.0"
-orjson = "^3.9.9"
+aiohttp = "^3.8.1"
 biopython = "^1.81"
+click = "^8.1.7"
+orjson = "^3.9.9"
 pydantic-factories = "^1.17.3"
-
+pyfixtures = "^1.0.0"
+sentry-sdk = "^2.3.1"
+virtool-core = "^12.0.0"
 
 [tool.poetry.scripts]
 run-workflow = "virtool_workflow.cli:cli_main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 pytest-aiohttp = "^1.0.0"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.10.0"
-pre-commit = "^2.18.1"
 sphinx = "^4.0.2"
 syrupy = "^3.0.5"
 sphinx-autobuild = "^2021.3.14"
 sphinx-nameko-theme = "^0.0.3"
 pytest-structlog = "^0.6"
 sphinx-toolbox = "^3.5.0"
+ruff = "^0.4.6"
+piccolo-theme = "^0.22.0"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.ruff]
 exclude = [
     "docs",
```

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/analysis/fastqc.py` & `virtool_workflow-7.0.0/virtool_workflow/analysis/fastqc.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/analysis/skewer.py` & `virtool_workflow-7.0.0/virtool_workflow/analysis/skewer.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/analysis/trimming.py` & `virtool_workflow-7.0.0/virtool_workflow/analysis/trimming.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/analysis/utils.py` & `virtool_workflow-7.0.0/virtool_workflow/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/api/acquire.py` & `virtool_workflow-7.0.0/virtool_workflow/api/acquire.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/api/client.py` & `virtool_workflow-7.0.0/virtool_workflow/api/client.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/api/utils.py` & `virtool_workflow-7.0.0/virtool_workflow/api/utils.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/cli.py` & `virtool_workflow-7.0.0/virtool_workflow/cli.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/data/__init__.py` & `virtool_workflow-7.0.0/virtool_workflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/data/analyses.py` & `virtool_workflow-7.0.0/virtool_workflow/data/analyses.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/data/hmms.py` & `virtool_workflow-7.0.0/virtool_workflow/data/hmms.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/data/indexes.py` & `virtool_workflow-7.0.0/virtool_workflow/data/indexes.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/data/jobs.py` & `virtool_workflow-7.0.0/virtool_workflow/data/jobs.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/data/ml.py` & `virtool_workflow-7.0.0/virtool_workflow/data/ml.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/data/samples.py` & `virtool_workflow-7.0.0/virtool_workflow/data/samples.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/data/subtractions.py` & `virtool_workflow-7.0.0/virtool_workflow/data/subtractions.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/data/uploads.py` & `virtool_workflow-7.0.0/virtool_workflow/data/uploads.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/decorators.py` & `virtool_workflow-7.0.0/virtool_workflow/decorators.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/errors.py` & `virtool_workflow-7.0.0/virtool_workflow/errors.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/hooks.py` & `virtool_workflow-7.0.0/virtool_workflow/hooks.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/pytest_plugin/data.py` & `virtool_workflow-7.0.0/virtool_workflow/pytest_plugin/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 
     new_subtraction: Subtraction
     """An un-finalized subtraction for testing subtraction creation workflows."""
 
 
 @pytest.fixture()
 def data(
-    virtool_workflow_example_path: Path, static_datetime: datetime.datetime,
+    virtool_workflow_example_path: Path,
+    static_datetime: datetime.datetime,
 ) -> Data:
     class AnalysisFactory(ModelFactory):
         __model__ = Analysis
 
         created_at = Use(lambda: static_datetime)
         updated_at = Use(lambda: static_datetime)
```

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/runtime/config.py` & `virtool_workflow-7.0.0/virtool_workflow/runtime/config.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/runtime/discover.py` & `virtool_workflow-7.0.0/virtool_workflow/runtime/discover.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/runtime/hook.py` & `virtool_workflow-7.0.0/virtool_workflow/runtime/hook.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/runtime/path.py` & `virtool_workflow-7.0.0/virtool_workflow/runtime/path.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/runtime/ping.py` & `virtool_workflow-7.0.0/virtool_workflow/runtime/ping.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/runtime/run.py` & `virtool_workflow-7.0.0/virtool_workflow/runtime/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 import logging
 import signal
 import sys
 from asyncio import CancelledError
 from pathlib import Path
 from typing import Callable
 
-import pkg_resources
 import structlog
 from pyfixtures import FixtureScope, runs_in_new_fixture_context
 from structlog import get_logger
 from virtool_core.models.job import JobState
-from virtool_core.redis import configure_redis
+from virtool_core.redis import Redis
 
 from virtool_workflow.api.acquire import acquire_job_by_id
 from virtool_workflow.api.client import api_client
 from virtool_workflow.hooks import (
     cleanup_builtin_status_hooks,
     on_cancelled,
     on_error,
@@ -38,14 +37,15 @@
 from virtool_workflow.runtime.path import create_work_path
 from virtool_workflow.runtime.ping import ping_periodically
 from virtool_workflow.runtime.redis import (
     get_next_job_with_timeout,
     wait_for_cancellation,
 )
 from virtool_workflow.runtime.sentry import configure_sentry
+from virtool_workflow.utils import get_virtool_workflow_version
 from virtool_workflow.workflow import Workflow
 
 logger = get_logger("runtime")
 
 
 def configure_status_hooks():
     """Configure built-in job status hooks.
@@ -124,14 +124,16 @@
                 on_failure.trigger(scope),
             )
 
     except Exception as error:
         scope["_error"] = error
         scope["_state"] = JobState.ERROR
 
+        logger.exception(error)
+
         await asyncio.gather(on_error.trigger(scope), on_failure.trigger(scope))
 
         if isinstance(error, asyncio.CancelledError):
             raise
 
     else:
         scope["_state"] = JobState.COMPLETE
@@ -156,15 +158,17 @@
     configure_status_hooks()
 
     load_builtin_fixtures()
 
     job = await acquire_job_by_id(config.jobs_api_connection_string, job_id)
 
     async with api_client(
-        config.jobs_api_connection_string, job.id, job.key,
+        config.jobs_api_connection_string,
+        job.id,
+        job.key,
     ) as api, FixtureScope() as scope:
         # These fixtures should not be used directly by the workflow. They are used
         # by other built-in fixtures.
         scope["_api"] = api
         scope["_config"] = config
         scope["_error"] = None
         scope["_job"] = job
@@ -221,25 +225,25 @@
             structlog.processors.TimeStamper(fmt="%Y-%m-%d %H:%M.%S"),
             structlog.dev.ConsoleRenderer(colors=True, sort_keys=True),
         ],
     )
 
     logger.info(
         "found virtool-workflow",
-        version=pkg_resources.get_distribution("virtool-workflow").version,
+        version=get_virtool_workflow_version(),
     )
 
     workflow = workflow_loader()
 
     load_builtin_fixtures()
     load_custom_fixtures()
 
     configure_sentry(sentry_dsn)
 
-    async with configure_redis(redis_connection_string, timeout=15) as redis:
+    async with Redis(redis_connection_string) as redis:
         try:
             job_id = await get_next_job_with_timeout(redis_list_name, redis, timeout)
         except asyncio.TimeoutError:
             # This happens due to Kubernetes scheduling issues or job cancellations. It
             # is not an error.
             logger.warning("timed out while waiting for job id")
             return
@@ -269,15 +273,15 @@
     signal.signal(signal.SIGTERM, terminate_workflow)
 
     def cancel_workflow(*_):
         logger.info("received cancellation signal from redis")
         events.cancelled.set()
         run_workflow_task.cancel()
 
-    async with configure_redis(redis_connection_string) as redis:
+    async with Redis(redis_connection_string) as redis:
         cancellation_task = asyncio.create_task(
             wait_for_cancellation(redis, job_id, cancel_workflow),
         )
 
         await run_workflow_task
 
         cancellation_task.cancel()
```

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/runtime/run_subprocess.py` & `virtool_workflow-7.0.0/virtool_workflow/runtime/run_subprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Code for running and managing subprocesses."""
 import asyncio
 from asyncio.subprocess import Process
 from pathlib import Path
-from typing import Awaitable, Callable, Coroutine, Protocol
+from typing import Callable, Coroutine, Protocol
 
 from pyfixtures import fixture
 from structlog import get_logger
 from virtool_core.utils import timestamp
 
 from virtool_workflow.errors import SubprocessFailed
 
 logger = get_logger("subprocess")
 
 
 class LineOutputHandler(Protocol):
-    async def __call__(self, line: str):
+    async def __call__(self, line: bytes):
         """Handle input from stdin, or stderr, line by line.
 
         :param line: A line of output from the stream.
         """
         raise NotImplementedError
 
 
@@ -41,15 +41,16 @@
         :raise SubprocessFailed: The subprocess has exited with a non-zero exit code
         :return: An :class:`.Process` instance
         """
         raise NotImplementedError
 
 
 async def watch_pipe(
-    stream: asyncio.StreamReader, handler: Callable[[bytes], Awaitable[None]],
+    stream: asyncio.StreamReader,
+    handler: LineOutputHandler,
 ):
     """Watch the stdout or stderr stream and pass lines to the `handler` callback function.
 
     :param stream: a stdout or stderr file object
     :param handler: a handler coroutine for output lines
 
     """
@@ -58,33 +59,53 @@
 
         if not line:
             return
 
         await handler(line)
 
 
+def stderr_logger(line: bytes):
+    """Log a line of stderr output and try to decode it as UTF-8.
+
+    If the line is not decodable, log it as a string.
+
+    :param line: a line of stderr output
+    """
+    line = line.rstrip()
+
+    try:
+        logger.info("stderr", line=line.decode())
+    except UnicodeDecodeError:
+        logger.info("stderr", line=line)
+
+
 async def _run_subprocess(
     command: list[str],
     stdout_handler: LineOutputHandler | None = None,
     stderr_handler: Callable[[str], Coroutine] | None = None,
     env: dict | None = None,
     cwd: str | None = None,
 ) -> asyncio.subprocess.Process:
     """An implementation of :class:`RunSubprocess` using `asyncio.subprocess`."""
     log = logger.bind()
     log.info("running subprocess", command=command)
 
     stdout = asyncio.subprocess.PIPE if stdout_handler else asyncio.subprocess.DEVNULL
 
-    async def _stderr_handler(line):
-        logger.info("stderr", line=line.rstrip())
+    if stderr_handler:
 
-        if stderr_handler:
+        async def _stderr_handler(line):
+            stderr_logger(line)
             await stderr_handler(line)
 
+    else:
+
+        async def _stderr_handler(line):
+            stderr_logger(line)
+
     process = await asyncio.create_subprocess_exec(
         *(str(arg) for arg in command),
         cwd=cwd,
         env=env,
         limit=1024 * 1024 * 128,
         stderr=asyncio.subprocess.PIPE,
         stdout=stdout,
@@ -102,17 +123,20 @@
     try:
         await watcher_future
     except asyncio.CancelledError:
         logger.info("terminating subprocess")
 
         process.terminate()
 
-        # Have to do this to avoid Event loop closed error.
+        # Have to do this in Python 3.10 to avoid Event loop closed error.
         # https://github.com/python/cpython/issues/88050
-        process._transport.close()
+        try:
+            process._transport.close()
+        except AttributeError:
+            pass
 
         await process.wait()
         logger.info("subprocess exited", code=process.returncode)
 
         await watcher_future
 
         return process
```

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/utils.py` & `virtool_workflow-7.0.0/virtool_workflow/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import tarfile
 from collections.abc import Callable
 from functools import wraps
+from importlib import metadata
 from inspect import iscoroutinefunction
 from pathlib import Path
 
 
 def coerce_to_coroutine_function(func: Callable):
     """Wrap a non-async function in an async function."""
     if iscoroutinefunction(func):
@@ -14,14 +15,22 @@
     @wraps(func)
     async def _func(*args, **kwargs):
         return func(*args, **kwargs)
 
     return _func
 
 
+def get_virtool_workflow_version() -> str:
+    """Get the version of the installed virtool-workflow package."""
+    try:
+        return metadata.version("virtool-workflow")
+    except metadata.PackageNotFoundError:
+        return "0.0.0"
+
+
 async def make_directory(path: Path):
     await asyncio.to_thread(path.mkdir, exist_ok=True, parents=True)
 
 
 def untar(path: Path, target_path: Path):
     with tarfile.open(path, "r:gz") as tar:
         tar.extractall(target_path)
```

### Comparing `virtool_workflow-6.0.0a9/virtool_workflow/workflow.py` & `virtool_workflow-7.0.0/virtool_workflow/workflow.py`

 * *Files identical despite different names*

