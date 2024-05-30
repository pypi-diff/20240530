# Comparing `tmp/corallium-1.0.0.tar.gz` & `tmp/corallium-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corallium-1.0.0.tar", max compression
+gzip compressed data, was "corallium-1.0.2.tar", max compression
```

## Comparing `corallium-1.0.0.tar` & `corallium-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-04-16 12:38:46.672808 corallium-1.0.0/LICENSE
--rw-r--r--   0        0        0     1850 2024-04-16 12:55:16.353486 corallium-1.0.0/corallium/__init__.py
--rw-r--r--   0        0        0     8684 2023-12-10 17:52:22.388535 corallium-1.0.0/corallium/file_helpers.py
--rw-r--r--   0        0        0     3756 2023-12-10 17:52:47.559820 corallium-1.0.0/corallium/log.py
--rw-r--r--   0        0        0        0 2023-02-23 12:18:48.616595 corallium-1.0.0/corallium/loggers/__init__.py
--rw-r--r--   0        0        0      494 2023-06-21 07:55:37.168870 corallium-1.0.0/corallium/loggers/plain_printer.py
--rw-r--r--   0        0        0     2114 2023-12-10 16:26:52.360419 corallium-1.0.0/corallium/loggers/rich_printer.py
--rw-r--r--   0        0        0      274 2023-04-22 04:52:34.549543 corallium-1.0.0/corallium/loggers/structlog_logger/__init__.py
--rw-r--r--   0        0        0      758 2023-04-22 04:57:25.576582 corallium-1.0.0/corallium/loggers/structlog_logger/_structlog_logger.py
--rw-r--r--   0        0        0     2094 2023-09-12 23:27:54.142142 corallium-1.0.0/corallium/loggers/styles.py
--rw-r--r--   0        0        0     4234 2023-12-10 17:57:10.741345 corallium-1.0.0/corallium/pretty_process.py
--rw-r--r--   0        0        0     3749 2024-04-16 12:40:28.343049 corallium-1.0.0/corallium/shell.py
--rw-r--r--   0        0        0      218 2023-12-10 17:58:03.509787 corallium-1.0.0/corallium/tomllib.py
--rw-r--r--   0        0        0     2833 2024-04-16 12:55:20.846119 corallium-1.0.0/docs/README.md
--rw-r--r--   0        0        0     1677 2024-04-16 12:55:16.369150 corallium-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 corallium-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-18 09:50:09.156598 corallium-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1850 2024-05-30 01:28:25.967050 corallium-1.0.2/corallium/__init__.py
+-rw-r--r--   0        0        0     8687 2024-04-17 15:26:30.023370 corallium-1.0.2/corallium/file_helpers.py
+-rw-r--r--   0        0        0     3756 2023-12-10 17:52:47.559820 corallium-1.0.2/corallium/log.py
+-rw-r--r--   0        0        0        0 2023-02-23 12:18:48.616595 corallium-1.0.2/corallium/loggers/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-21 07:55:37.168870 corallium-1.0.2/corallium/loggers/plain_printer.py
+-rw-r--r--   0        0        0     2114 2023-12-10 16:26:52.360419 corallium-1.0.2/corallium/loggers/rich_printer.py
+-rw-r--r--   0        0        0      274 2023-04-22 04:52:34.549543 corallium-1.0.2/corallium/loggers/structlog_logger/__init__.py
+-rw-r--r--   0        0        0      758 2023-04-22 04:57:25.576582 corallium-1.0.2/corallium/loggers/structlog_logger/_structlog_logger.py
+-rw-r--r--   0        0        0     2097 2024-05-30 00:10:41.836868 corallium-1.0.2/corallium/loggers/styles.py
+-rw-r--r--   0        0        0     4234 2023-12-10 17:57:10.741345 corallium-1.0.2/corallium/pretty_process.py
+-rw-r--r--   0        0        0     3749 2024-04-16 12:40:28.343049 corallium-1.0.2/corallium/shell.py
+-rw-r--r--   0        0        0      218 2023-12-10 17:58:03.509787 corallium-1.0.2/corallium/tomllib.py
+-rw-r--r--   0        0        0     2833 2024-05-30 01:28:29.774038 corallium-1.0.2/docs/README.md
+-rw-r--r--   0        0        0     1687 2024-05-30 01:28:25.978138 corallium-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3980 1970-01-01 00:00:00.000000 corallium-1.0.2/PKG-INFO
```

### Comparing `corallium-1.0.0/LICENSE` & `corallium-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corallium-1.0.0/corallium/__init__.py` & `corallium-1.0.2/corallium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from warnings import filterwarnings
 
 from beartype import BeartypeConf
 from beartype.claw import beartype_this_package
 from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
 from typing_extensions import Self
 
-__version__ = '1.0.0'
+__version__ = '1.0.2'
 __pkg_name__ = 'corallium'
 
 
 class _RuntimeTypeCheckingModes(Enum):
     """Supported global runtime type checking modes."""
 
     ERROR = 'ERROR'
```

### Comparing `corallium-1.0.0/corallium/file_helpers.py` & `corallium-1.0.2/corallium/file_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     """Read the 'pyproject.toml' file once."""
     toml_path = find_in_parents(name='pyproject.toml', cwd=cwd)
     try:
         pyproject_txt = toml_path.read_text(encoding='utf-8')
     except Exception as exc:
         msg = f'Could not locate: {toml_path}'
         raise RuntimeError(msg) from exc
-    return tomllib.loads(pyproject_txt)  # pyright: ignore[reportGeneralTypeIssues]
+    return tomllib.loads(pyproject_txt)  # pyright: ignore[reportAttributeAccessIssue]
 
 
 @lru_cache(maxsize=5)
 def read_package_name(cwd: Optional[Path] = None) -> str:
     """Read the package name once."""
     poetry_config = read_pyproject(cwd=cwd)
     return str(poetry_config['tool']['poetry']['name'])
```

### Comparing `corallium-1.0.0/corallium/log.py` & `corallium-1.0.2/corallium/log.py`

 * *Files identical despite different names*

### Comparing `corallium-1.0.0/corallium/loggers/rich_printer.py` & `corallium-1.0.2/corallium/loggers/rich_printer.py`

 * *Files identical despite different names*

### Comparing `corallium-1.0.0/corallium/loggers/structlog_logger/_structlog_logger.py` & `corallium-1.0.2/corallium/loggers/structlog_logger/_structlog_logger.py`

 * *Files identical despite different names*

### Comparing `corallium-1.0.0/corallium/loggers/styles.py` & `corallium-1.0.2/corallium/loggers/styles.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Styles."""
 
 import logging
+from dataclasses import dataclass
 
 from beartype import beartype
-from pydantic import BaseModel
 
 
-class Styles(BaseModel):
+@dataclass
+class Styles:
     """Inspired by `loguru` and `structlog` and used in `tail-jsonl`.
 
     https://rich.readthedocs.io/en/latest/style.html
 
     Inspired by: https://github.com/Delgan/loguru/blob/07f94f3c8373733119f85aa8b9ca05ace3325a4b/loguru/_defaults.py#L31-L73
 
     And: https://github.com/hynek/structlog/blob/bcfc7f9e60640c150bffbdaeed6328e582f93d1e/src/structlog/dev.py#L126-L141
```

### Comparing `corallium-1.0.0/corallium/pretty_process.py` & `corallium-1.0.2/corallium/pretty_process.py`

 * *Files identical despite different names*

### Comparing `corallium-1.0.0/corallium/shell.py` & `corallium-1.0.2/corallium/shell.py`

 * *Files identical despite different names*

### Comparing `corallium-1.0.0/docs/README.md` & `corallium-1.0.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `corallium-1.0.0/pyproject.toml` & `corallium-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.0.0"
+version = "1.0.2"
 version_files = ["corallium/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
@@ -21,25 +21,25 @@
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "corallium"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/corallium"
-version = "1.0.0"
+version = "1.0.2"
 
 [tool.poetry.dependencies]
 python = "^3.9.13"
 beartype = ">=0.18.2"
-pydantic = ">=2.7.0"
 rich = ">=13.7.1"
 tomli = {markers = "python_version < '3.11'", version = ">=2.0.1"}
+typing-extensions = ">=4.12.0"
 
 [tool.poetry.group.dev.dependencies]
-calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=2.0.4"}
+calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=2.1.0"}
 pytest-asyncio = ">=0.23.6"
 pytest-structlog = ">=0.8" # Provides pytest fixture 'log'
 pytest-subprocess = ">=1.5.0"
 structlog = ">=24.1.0"
 types-pyyaml = ">=6.0.12.8"
 
 [tool.poetry.urls]
```

### Comparing `corallium-1.0.0/PKG-INFO` & `corallium-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corallium
-Version: 1.0.0
+Version: 1.0.2
 Summary: Shared functionality for the calcipy-ecosystem
 Home-page: https://github.com/kyleking/corallium
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -12,17 +12,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beartype (>=0.18.2)
-Requires-Dist: pydantic (>=2.7.0)
 Requires-Dist: rich (>=13.7.1)
 Requires-Dist: tomli (>=2.0.1) ; python_version < "3.11"
+Requires-Dist: typing-extensions (>=4.12.0)
 Project-URL: Bug Tracker, https://github.com/kyleking/corallium/issues
 Project-URL: Changelog, https://github.com/kyleking/corallium/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://corallium.kyleking.me
 Project-URL: Repository, https://github.com/kyleking/corallium
 Description-Content-Type: text/markdown
 
 # corallium
```

