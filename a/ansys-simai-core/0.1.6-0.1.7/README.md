# Comparing `tmp/ansys_simai_core-0.1.6.tar.gz` & `tmp/ansys_simai_core-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_simai_core-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_simai_core-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_simai_core-0.1.6.tar` & `ansys_simai_core-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1089 2024-04-29 16:23:44.826218 ansys_simai_core-0.1.6/LICENSE
--rw-r--r--   0        0        0     5009 2024-04-29 16:23:44.826218 ansys_simai_core-0.1.6/README.rst
--rw-r--r--   0        0        0     4796 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1532 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/__init__.py
--rw-r--r--   0        0        0     1146 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/__init__.py
--rw-r--r--   0        0        0     2202 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/client.py
--rw-r--r--   0        0        0     2397 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/design_of_experiments.py
--rw-r--r--   0        0        0     5852 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/geometry.py
--rw-r--r--   0        0        0    10158 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/mixin.py
--rw-r--r--   0        0        0     1975 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/optimization.py
--rw-r--r--   0        0        0     4901 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/post_processing.py
--rw-r--r--   0        0        0     2650 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/prediction.py
--rw-r--r--   0        0        0     3749 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/project.py
--rw-r--r--   0        0        0     6030 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/sse.py
--rw-r--r--   0        0        0     3134 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/training_data.py
--rw-r--r--   0        0        0     2456 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/training_data_part.py
--rw-r--r--   0        0        0     3818 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/workspace.py
--rw-r--r--   0        0        0    13489 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/client.py
--rw-r--r--   0        0        0     1146 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/__init__.py
--rw-r--r--   0        0        0    12193 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/base.py
--rw-r--r--   0        0        0     3158 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/design_of_experiments.py
--rw-r--r--   0        0        0     2638 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/downloads.py
--rw-r--r--   0        0        0    22009 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/geometries.py
--rw-r--r--   0        0        0    11257 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/geometry_utils.py
--rw-r--r--   0        0        0     4766 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/lists.py
--rw-r--r--   0        0        0     4318 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/models.py
--rw-r--r--   0        0        0    10812 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/optimizations.py
--rw-r--r--   0        0        0    30612 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/post_processings.py
--rw-r--r--   0        0        0     9794 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/predictions.py
--rw-r--r--   0        0        0     6826 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/projects.py
--rw-r--r--   0        0        0     7571 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/selection_post_processings.py
--rw-r--r--   0        0        0     9701 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/selections.py
--rw-r--r--   0        0        0    11994 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/training_data.py
--rw-r--r--   0        0        0     2137 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/training_data_parts.py
--rw-r--r--   0        0        0     9611 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/types.py
--rw-r--r--   0        0        0     6541 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/workspaces.py
--rw-r--r--   0        0        0     4108 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/errors.py
--rw-r--r--   0        0        0        0 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/py.typed
--rw-r--r--   0        0        0     1146 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/__init__.py
--rw-r--r--   0        0        0     9476 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/auth.py
--rw-r--r--   0        0        0     4522 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/config_file.py
--rw-r--r--   0        0        0     5970 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/configuration.py
--rw-r--r--   0        0        0     2761 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/files.py
--rw-r--r--   0        0        0     5041 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/grouping.py
--rw-r--r--   0        0        0     1627 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/misc.py
--rw-r--r--   0        0        0     4132 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/numerical.py
--rw-r--r--   0        0        0     3903 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/requests.py
--rw-r--r--   0        0        0     3084 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/sse_client.py
--rw-r--r--   0        0        0     1643 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/typing.py
--rw-r--r--   0        0        0     2118 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/validation.py
--rw-r--r--   0        0        0     6462 1970-01-01 00:00:00.000000 ansys_simai_core-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-30 15:07:22.418074 ansys_simai_core-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5010 2024-05-30 15:07:22.418074 ansys_simai_core-0.1.7/README.rst
+-rw-r--r--   0        0        0     4896 2024-05-30 15:07:22.418074 ansys_simai_core-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1532 2024-05-30 15:07:22.418074 ansys_simai_core-0.1.7/src/ansys/simai/core/__init__.py
+-rw-r--r--   0        0        0     1146 2024-05-30 15:07:22.418074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/__init__.py
+-rw-r--r--   0        0        0     2202 2024-05-30 15:07:22.418074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/client.py
+-rw-r--r--   0        0        0     2397 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/design_of_experiments.py
+-rw-r--r--   0        0        0     5852 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/geometry.py
+-rw-r--r--   0        0        0    10158 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/mixin.py
+-rw-r--r--   0        0        0     1975 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/optimization.py
+-rw-r--r--   0        0        0     4901 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/post_processing.py
+-rw-r--r--   0        0        0     2650 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/prediction.py
+-rw-r--r--   0        0        0     3749 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/project.py
+-rw-r--r--   0        0        0     6030 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/sse.py
+-rw-r--r--   0        0        0     3134 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/training_data.py
+-rw-r--r--   0        0        0     2456 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/training_data_part.py
+-rw-r--r--   0        0        0     3818 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/api/workspace.py
+-rw-r--r--   0        0        0    13489 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/client.py
+-rw-r--r--   0        0        0     1146 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/__init__.py
+-rw-r--r--   0        0        0    11888 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/base.py
+-rw-r--r--   0        0        0     3927 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/design_of_experiments.py
+-rw-r--r--   0        0        0     2638 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/downloads.py
+-rw-r--r--   0        0        0    22009 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/geometries.py
+-rw-r--r--   0        0        0    11257 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/geometry_utils.py
+-rw-r--r--   0        0        0     4766 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/lists.py
+-rw-r--r--   0        0        0    12407 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/models.py
+-rw-r--r--   0        0        0    10826 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/optimizations.py
+-rw-r--r--   0        0        0    31881 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/post_processings.py
+-rw-r--r--   0        0        0     9788 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/predictions.py
+-rw-r--r--   0        0        0     6835 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/projects.py
+-rw-r--r--   0        0        0     7571 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/selection_post_processings.py
+-rw-r--r--   0        0        0     9701 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/selections.py
+-rw-r--r--   0        0        0    11994 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/training_data.py
+-rw-r--r--   0        0        0     2137 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/training_data_parts.py
+-rw-r--r--   0        0        0     9770 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/types.py
+-rw-r--r--   0        0        0     6846 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/data/workspaces.py
+-rw-r--r--   0        0        0     4108 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/errors.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/py.typed
+-rw-r--r--   0        0        0     1146 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/__init__.py
+-rw-r--r--   0        0        0     9476 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/auth.py
+-rw-r--r--   0        0        0     4522 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/config_file.py
+-rw-r--r--   0        0        0     5970 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/configuration.py
+-rw-r--r--   0        0        0     2761 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/files.py
+-rw-r--r--   0        0        0     5041 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/grouping.py
+-rw-r--r--   0        0        0     1627 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/misc.py
+-rw-r--r--   0        0        0     4132 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/numerical.py
+-rw-r--r--   0        0        0     3903 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/requests.py
+-rw-r--r--   0        0        0     3084 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/sse_client.py
+-rw-r--r--   0        0        0     1643 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/typing.py
+-rw-r--r--   0        0        0     2118 2024-05-30 15:07:22.422074 ansys_simai_core-0.1.7/src/ansys/simai/core/utils/validation.py
+-rw-r--r--   0        0        0     6463 1970-01-01 00:00:00.000000 ansys_simai_core-0.1.7/PKG-INFO
```

### Comparing `ansys_simai_core-0.1.6/LICENSE` & `ansys_simai_core-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/README.rst` & `ansys_simai_core-0.1.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 As Makefile has rules, `tox`_ has environments. In fact, the tool creates its
 own virtual environment so anything being tested is isolated from the project in
 order to guarantee project's integrity. The following environments commands are provided:
 
 - **tox -e style**: will check for coding style quality.
 - **tox -e py**: checks for unit tests.
 - **tox -e py-coverage**: checks for unit testing and code coverage.
-- **tox -e doc**: checs for documentation building process.
+- **tox -e doc**: checks for documentation building process.
 
 
 Raw testing
 ^^^^^^^^^^^
 
 If required, you can always call the style commands (`ruff`_) or unit testing ones (`pytest`_) from the command line. However,
 this does not guarantee that your project is being tested in an isolated
```

### Comparing `ansys_simai_core-0.1.6/pyproject.toml` & `ansys_simai_core-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Using PDM with flit backend
 [build-system]
 requires = ["flit_core>=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-simai-core"
-version = "0.1.6"
+version = "0.1.7"
 description = "A python wrapper for Ansys SimAI"
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
     {name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com"},
 ]
@@ -32,15 +32,15 @@
 dependencies = [
     "requests>=2.31.0,<3",
     "requests_toolbelt>=1.0.0,<2",
     "tomli>=2.0.1,<3",
     "pydantic>=2.5.1,<3",
     "semver>=3.0.2",
     "sseclient-py>=1.8.0,<3",
-    "wakepy>=0.7.2",
+    "wakepy>=0.8.0",
     "tqdm>=4.66.1",
 ]
 
 [project.module]
 name = "ansys.simai.core"
 
 [tool.flit.module]
@@ -67,14 +67,15 @@
     "blacken-docs",
     "pre-commit"
 ]
 
 [tool.pdm.scripts]
 lint = "pre-commit run --all-files"
 test = "pytest --cov=ansys --cov-report=term --cov-report=html:./cov/html tests -vv"
+doc = "sphinx-build doc/source _build/html --color -vW -bhtml"
 
 [project.urls]
 Bugs = "https://github.com/ansys/pysimai/issues"
 Documentation = "https://simai.docs.pyansys.com"
 Source = "https://github.com/ansys/pysimai"
 Discussions = "https://github.com/ansys/pysimai/discussions"
 Releases = "https://github.com/ansys/pysimai/releases"
@@ -168,7 +169,8 @@
 known-first-party = ["ansys.simai.core"]
 
 [tool.coverage.run]
 source = ["ansys.simai.core"]
 
 [tool.coverage.report]
 show_missing = true
+exclude_also = ["if TYPE_CHECKING:"]
```

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/__init__.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/__init__.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/client.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/client.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/design_of_experiments.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/design_of_experiments.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/geometry.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/geometry.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/mixin.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/mixin.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/optimization.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/optimization.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/post_processing.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/post_processing.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/prediction.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/prediction.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/project.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/project.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/sse.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/sse.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/training_data.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/training_data.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/training_data_part.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/training_data_part.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/api/workspace.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/api/workspace.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/client.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/client.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/__init__.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/base.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,14 @@
         **kwargs,
     ):
         # Override id_key to configure the field to return with :py:meth:`Model.id`.
         self.id_key = "id"
         self.fields = fields or {}
         self._directory = directory
         self._client = client
-        if (
-            self.fields.get("workspace_id")
-            and self.fields["workspace_id"] != self._client.current_workspace.id
-        ):
-            logger.warning("The object does not belong to the currently configured workspace.")
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: {self.id}>"
 
     @property
     def id(self) -> str:
         """ID of the object on the server."""
@@ -231,19 +226,15 @@
             logger.error(self.fields.get("error"))
 
 
 DataModelType = TypeVar("DataModelType", bound=DataModel)
 
 
 class Directory(ABC, Generic[DataModelType]):
-    @classmethod
-    @property
-    @abstractmethod
-    def _data_model(cls) -> Type[DataModel]:
-        pass
+    _data_model: Type[DataModelType]
 
     def __init__(self, client: "ansys.simai.core.client.SimAIClient"):
         self._client = client
 
         # Registry for known objects of this type that have been created
         # locally. It is used to ensure that only one instance of a particular class
         # exists with a given ID.
@@ -255,16 +246,16 @@
         self._registry: Dict[str, DataModel] = {}
 
     @abstractmethod
     def get(self, id: str) -> DataModel:  # noqa: D102
         pass
 
     def _model_from(
-        self, data: dict, data_model: Optional[DataModel] = None, **kwargs
-    ) -> DataModel:
+        self, data: dict, data_model: Optional[DataModelType] = None, **kwargs
+    ) -> DataModelType:
         # _model_from overrides object data (fields),
         # thus it is, and should, only be called with
         # complete data from the server, such as from a GET request.
         if "id" not in data:
             raise ValueError("Cannot instantiate data object without an id")
         item_id = data["id"]
         if item_id in self._registry:
@@ -276,15 +267,15 @@
         else:
             constructor = data_model if data_model else self._data_model
             # item was unknown: create it and save it to the registry
             item = constructor(self._client, self, data, **kwargs)
             self._registry[item_id] = item
         return item
 
-    def _unregister_item(self, item: DataModel):
+    def _unregister_item(self, item: DataModelType):
         """Remove the item from the internal registry,
         mainly after a deletion.
         """
         self._unregister_item_with_id(item.id)
 
     def _unregister_item_with_id(self, item_id: str):
         """Remove the item from the internal registry,
```

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/design_of_experiments.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/design_of_experiments.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,63 +20,76 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import io
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, Union
 
+from ansys.simai.core.data.types import Identifiable, get_id_from_identifiable
+
 if TYPE_CHECKING:
-    import ansys.simai.core.client
+    from ansys.simai.core.client import SimAIClient
+    from ansys.simai.core.data.workspaces import Workspace
 
 
 class DesignOfExperimentsCollection:
     """Provides a collection of methods related to design of experiments.
 
     This class is accessed through ``client.design_of_experiments``.
     """
 
-    def __init__(self, client: "ansys.simai.core.client.SimAIClient"):
+    def __init__(self, client: "SimAIClient"):
         self._client = client
 
-    def download(self, file: Union[str, Path], format: str = "xlsx") -> None:
+    def download(
+        self,
+        file: Union[str, Path],
+        format: str = "xlsx",
+        workspace: Optional[Identifiable["Workspace"]] = None,
+    ) -> None:
         """Download the design of experiments data to the specified file or path.
 
         Args:
             file: Path of the file to put the content into.
             format: Expected format. The default is ``'xlsx'``. Options are ``'xlsx'``
                 and ``'csv'``.
+            workspace: Workspace to download the design of experiments from. If not
+                specified, the current workspace is used.
 
         Example:
             .. code-block:: python
 
                 import ansys.simai.core
 
                 simai = ansys.simai.core.from_config()
                 simai.design_of_experiments.download(file="~/exp_plan.xlsx", format="xlsx")
         """
-        self._client._api.download_design_of_experiments(
-            file, format, self._client.current_workspace.id
-        )
+        workspace_id = get_id_from_identifiable(workspace, default=self._client._current_workspace)
+        self._client._api.download_design_of_experiments(file, format, workspace_id)
 
-    def in_memory(self, format: Optional[str] = "csv") -> io.BytesIO:
+    def in_memory(
+        self, format: Optional[str] = "csv", workspace: Optional[Identifiable["Workspace"]] = None
+    ) -> io.BytesIO:
         """Load the design of experiments data in memory.
 
         Args:
             file: Path of the file to put the content into.
             format: Expected format. The default is ``'csv'``. Options are ``'xlsx'``
                 and ``'csv'``.
+            workspace: Workspace to download the design of experiments from. If not
+                specified, the current workspace is used.
 
         Returns:
             :class:`~io.BytesIO` object containing the design of experiments data.
 
         Example:
             .. code-block:: python
 
                 import ansys.simai.core
 
                 simai = ansys.simai.core.from_config()
-                data = simai.design_of_experiments.in_memory(format="csv")
+                workspace = simai.workspaces.list()[0]
+                data = simai.design_of_experiments.in_memory(format="csv", workspace=workspace)
                 # Read data with CSV reader, ...
         """
-        return self._client._api.download_design_of_experiments(
-            None, format, self._client.current_workspace.id
-        )
+        workspace_id = get_id_from_identifiable(workspace, default=self._client._current_workspace)
+        return self._client._api.download_design_of_experiments(None, format, workspace_id)
```

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/downloads.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/geometries.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/geometries.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/geometry_utils.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/lists.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/lists.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/optimizations.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/optimizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
             optimization = self._model_from(
                 self._client._api.define_optimization(workspace_id, optimization_parameters)
             )
             optimization.wait()
             geometry_parameters = optimization.fields["initial_geometry_parameters"]
             logger.debug("Optimization defined. Starting optimization loop.")
             iterations_results: List[Dict] = []
-            with keep.running() as k:
+            with keep.running(on_fail="warn") as k:
                 if not k.success:
                     logger.info("Failed to get sleep inhibition lock.")
                 while geometry_parameters:
                     logger.debug(f"Generating geometry with parameters {geometry_parameters}.")
                     progress_bar.set_description("Generating geometry.")
                     # TODO: Somehow keep session alive for long geometry generation
                     generated_geometry = geometry_generation_fn(**geometry_parameters)
```

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/post_processings.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/post_processings.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from ansys.simai.core.data.downloads import DownloadableResult
 from ansys.simai.core.data.types import Identifiable, get_id_from_identifiable
 from ansys.simai.core.errors import InvalidArguments, InvalidServerStateError
 from ansys.simai.core.utils.numerical import convert_axis_and_coordinate_to_plane_eq_coeffs
 
 if TYPE_CHECKING:
     from ansys.simai.core.data.predictions import Prediction
+    from ansys.simai.core.data.workspaces import Workspace
 
 
 logger = logging.getLogger(__name__)
 
 
 class PostProcessing(ComputableDataModel, ABC):
     """Provides the local representation of a ``PostProcessing`` object.
@@ -570,14 +571,27 @@
         if pp_class not in self._post_processings:
             self._post_processings[pp_class] = {}
         self._post_processings[pp_class][params_frozen] = post_processing
         for location, warning_message in post_processing.fields.get("warnings", {}).items():
             logger.warning(f"{location}: {warning_message}")
         return post_processing
 
+    def list(
+        self,
+        post_processing_type: Optional[Type[PostProcessing]] = None,
+    ) -> List[PostProcessing]:
+        """List the postprocessings associated with the prediction.
+
+        See :func:`post_processings.list<ansys.simai.core.data.post_processings.PostProcessingDirectory.list>`
+        """
+        return self._client.post_processings.list(
+            post_processing_type=post_processing_type,
+            prediction=self.prediction,
+        )
+
 
 class PostProcessingDirectory(Directory[PostProcessing]):
     _data_model = PostProcessing
 
     @classmethod
     def _data_model_for_type_name(cls, pp_type_name: str) -> Optional[Type[PostProcessing]]:
         return getattr(sys.modules[__name__], pp_type_name, None)
@@ -629,51 +643,63 @@
         data = self._client._api.get_post_processing_result(id)
         return self._model_from(data)
 
     def list(
         self,
         post_processing_type: Optional[Type[PostProcessing]] = None,
         prediction: Optional[Identifiable["Prediction"]] = None,
+        workspace: Optional[Identifiable["Workspace"]] = None,
     ) -> List[PostProcessing]:
         """List the postprocessings in the current workspace or associated with a prediction.
 
         Optionally you can choose to list only postprocessings of a specific type.
         For the name of the available postprocessings, see :ref:`available_pp`.
-        Note that the case must be respected.
 
         Args:
             post_processing_type: Type of postprocessing to list.
             prediction: ID or :class:`model <.predictions.Prediction>` of a prediction.
                 If a value is specified, only postprocessings associated with this prediction
                 are returned.
+            workspace: ID or :class:`model <.workspaces.Workspace>` of a workspace.
+                If a value is specified, only postprocessings associated with this workspace
+                are returned.
 
         Raises:
-            NotFoundError: Postprocessing type and/or the prediction ID are incorrect.
+            NotFoundError: Postprocessing type, prediction ID or workspace ID are incorrect.
+            InvalidArguments: If both prediction and workspace are specified.
+            InvalidClientStateError: Neither prediction nor workspace are defined, default
+                workspace is not set.
 
         Example:
             .. code-block:: python
 
                 import ansys.simai.core
 
                 simai = ansys.simai.core_from_config()
                 prediction = simai.predictions.list()[0]
                 post_processings = simai.post_processings.list(
                     ansys.simai.core.SurfaceEvol, prediction.id
                 )
         """
         pp_type_str = post_processing_type._api_name() if post_processing_type else None
-        prediction_id = get_id_from_identifiable(prediction, required=False)
-        if not prediction_id:
-            post_processings = self._client._api.get_post_processings_in_workspace(
-                self._client.current_workspace.id, pp_type_str
-            )
-        else:
+        if workspace and prediction:
+            raise InvalidArguments("Only one of Workspace or Prediction can be specified")
+        if prediction:
+            prediction_id = get_id_from_identifiable(prediction, required=False)
             post_processings = self._client._api.get_post_processings_for_prediction(
                 prediction_id, pp_type_str
             )
+        else:
+            if workspace:
+                workspace_id = get_id_from_identifiable(workspace, required=False)
+            else:
+                workspace_id = self._client.current_workspace.id
+            post_processings = self._client._api.get_post_processings_in_workspace(
+                workspace_id, pp_type_str
+            )
         return list(map(self._model_from, post_processings))
 
     def run(
         self,
         post_processing_type: Union[str, Type[PostProcessing]],
         prediction: Identifiable["Prediction"],
         parameters: Optional[Dict[str, Any]] = None,
```

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/predictions.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/predictions.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,20 +181,17 @@
     def list(self, workspace: Optional[Identifiable[Workspace]] = None) -> List[Prediction]:
         """List all predictions on the server that belong to the specified workspace or the configured one.
 
         Args:
             workspace: ID or :class:`model <.workspaces.Workspace>` of the workspace to list the predictions for.
                 This parameter is necessary if no workspace is set for the client.
         """
-        return [
-            self._model_from(prediction)
-            for prediction in self._client._api.predictions(
-                get_id_from_identifiable(workspace, default=self._client.current_workspace)
-            )
-        ]
+        workspace_id = get_id_from_identifiable(workspace, default=self._client.current_workspace)
+        raw_predictions = self._client._api.predictions(workspace_id)
+        return list(map(self._model_from, raw_predictions))
 
     def get(self, id: str) -> Prediction:
         """Get a specific prediction object from the server by ID.
 
         Args:
             id: ID of the prediction.
```

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/projects.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from typing import TYPE_CHECKING, List, NamedTuple, Optional
+from typing import TYPE_CHECKING, Dict, List, NamedTuple, Optional
 
 from ansys.simai.core.data.base import DataModel, Directory
 from ansys.simai.core.data.models import ModelConfiguration
 from ansys.simai.core.data.types import Identifiable, get_id_from_identifiable
 from ansys.simai.core.errors import InvalidArguments
 
 if TYPE_CHECKING:
@@ -122,15 +122,15 @@
         self._client._api.delete_project(self.id)
 
     def is_trainable(self) -> bool:
         """Check if the project meets the prerequisites to be trained."""
         tt = self._client._api.is_project_trainable(self.id)
         return IsTrainableInfo(**tt)
 
-    def get_variables(self) -> dict[str, list[str]] | None:
+    def get_variables(self) -> Optional[Dict[str, List[str]]]:
         """Get the available variables for the model's input/output."""
         if not self.sample:
             return None
 
         sample_metadata = self.sample.fields.get("extracted_metadata")
         data = {}
         for key, vals in sample_metadata.items():
```

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/selection_post_processings.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/selection_post_processings.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/selections.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/selections.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/training_data.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/training_data.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/training_data_parts.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/training_data_parts.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/types.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,26 @@
 
 import io
 import os
 import pathlib
 from contextlib import contextmanager
 from enum import Enum
 from numbers import Number
-from typing import Any, BinaryIO, Callable, Dict, Generator, List, Optional, Tuple, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    BinaryIO,
+    Callable,
+    Dict,
+    Generator,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
 
 from requests import Response
 
 from ansys.simai.core.data.base import DataModel, DataModelType, Directory
 from ansys.simai.core.errors import InvalidArguments
 from ansys.simai.core.utils.files import file_path_to_obj_file
 from ansys.simai.core.utils.numerical import (
@@ -84,14 +95,19 @@
 
 For uploads, the callback receives the number of bytes written each iteration.
 """
 
 Identifiable = Union[DataModelType, str]
 """Either a model or the string ID of an object of the same type."""
 
+if TYPE_CHECKING:
+    from typing import TypeVar
+
+    D = TypeVar("D", bound=DataModel)
+
 
 def build_boundary_conditions(boundary_conditions: Optional[Dict[str, Number]] = None, **kwargs):
     bc = boundary_conditions if boundary_conditions else {}
     bc.update(**kwargs)
     if bc is None:
         raise ValueError("No boundary condition was specified.")
     if not is_boundary_conditions(bc):
@@ -232,17 +248,17 @@
         yield file, obj_name, file_ext
     finally:
         if close_file is True:
             file.close()
 
 
 def get_id_from_identifiable(
-    identifiable: Optional[Identifiable] = None,
+    identifiable: Optional[Identifiable["D"]] = None,
     required: bool = True,
-    default: Optional[Identifiable] = None,
+    default: Optional[Identifiable["D"]] = None,
 ) -> Optional[str]:
     if isinstance(identifiable, DataModel):
         return identifiable.id
     elif isinstance(identifiable, str):
         return identifiable
     elif default:
         return get_id_from_identifiable(default, required)
```

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/data/workspaces.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/data/workspaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import warnings
 from pprint import pformat
 from typing import Any, BinaryIO, Dict, List, Optional, Union
 
 from ansys.simai.core.data.base import DataModel, Directory
 from ansys.simai.core.data.types import File, Identifiable, get_id_from_identifiable
 
 
@@ -63,15 +64,15 @@
 
     @property
     def physical_quantities(self) -> Dict[str, Any]:
         """Information on the physical quantities generated by the model. For example, the prediction's output."""
         return self._raw["physical_quantities"]
 
     @property
-    def post_processings(self) -> List[Dict[str, Any]]:
+    def post_processings(self) -> "List[Dict[str, Any]]":
         """Information on the postprocessings available for the model
         and the accepted parameters when relevant.
         """
         return self._raw["available-post-processings"]
 
 
 class Workspace(DataModel):
@@ -87,14 +88,22 @@
     @property
     def name(self) -> str:
         """Name of the workspace."""
         return self.fields["name"]
 
     @property
     def model(self) -> ModelManifest:
+        """Deprecated alias to :py:attr:`~model_manifest`."""
+        warnings.warn(
+            "workspace.model is deprecated, please use workspace.model_manifest", stacklevel=2
+        )
+        return self.model_manifest
+
+    @property
+    def model_manifest(self) -> ModelManifest:
         """:class:`~ansys.simai.core.data.workspaces.ModelManifest` instance containing
         information about the model associated with the workspace.
         """
         if self._model_manifest is None:
             self._model_manifest = ModelManifest(
                 self._client._api.get_workspace_model_manifest(self.id)
             )
```

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/errors.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/__init__.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/auth.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/config_file.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/config_file.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/configuration.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/files.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/grouping.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/grouping.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/misc.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/numerical.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/numerical.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/requests.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/requests.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/sse_client.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/typing.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/typing.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/validation.py` & `ansys_simai_core-0.1.7/src/ansys/simai/core/utils/validation.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.6/PKG-INFO` & `ansys_simai_core-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-simai-core
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python wrapper for Ansys SimAI
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests>=2.31.0,<3
 Requires-Dist: requests_toolbelt>=1.0.0,<2
 Requires-Dist: tomli>=2.0.1,<3
 Requires-Dist: pydantic>=2.5.1,<3
 Requires-Dist: semver>=3.0.2
 Requires-Dist: sseclient-py>=1.8.0,<3
-Requires-Dist: wakepy>=0.7.2
+Requires-Dist: wakepy>=0.8.0
 Requires-Dist: tqdm>=4.66.1
 Project-URL: Bugs, https://github.com/ansys/pysimai/issues
 Project-URL: Discussions, https://github.com/ansys/pysimai/discussions
 Project-URL: Documentation, https://simai.docs.pyansys.com
 Project-URL: Releases, https://github.com/ansys/pysimai/releases
 Project-URL: Source, https://github.com/ansys/pysimai
 
@@ -142,15 +142,15 @@
 As Makefile has rules, `tox`_ has environments. In fact, the tool creates its
 own virtual environment so anything being tested is isolated from the project in
 order to guarantee project's integrity. The following environments commands are provided:
 
 - **tox -e style**: will check for coding style quality.
 - **tox -e py**: checks for unit tests.
 - **tox -e py-coverage**: checks for unit testing and code coverage.
-- **tox -e doc**: checs for documentation building process.
+- **tox -e doc**: checks for documentation building process.
 
 
 Raw testing
 ^^^^^^^^^^^
 
 If required, you can always call the style commands (`ruff`_) or unit testing ones (`pytest`_) from the command line. However,
 this does not guarantee that your project is being tested in an isolated
```

