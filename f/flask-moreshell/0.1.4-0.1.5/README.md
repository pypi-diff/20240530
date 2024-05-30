# Comparing `tmp/flask_moreshell-0.1.4.tar.gz` & `tmp/flask_moreshell-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_moreshell-0.1.4.tar", max compression
+gzip compressed data, was "flask_moreshell-0.1.5.tar", max compression
```

## Comparing `flask_moreshell-0.1.4.tar` & `flask_moreshell-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2024-02-11 11:58:06.568458 flask_moreshell-0.1.4/LICENSE
--rw-r--r--   0        0        0     3326 2024-02-11 11:58:06.568458 flask_moreshell-0.1.4/README.md
--rw-r--r--   0        0        0     2148 2024-02-11 11:58:17.176461 flask_moreshell-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       74 2024-02-11 11:58:06.576458 flask_moreshell-0.1.4/src/flask_moreshell/__init__.py
--rw-r--r--   0        0        0     1790 2024-02-11 11:58:17.176461 flask_moreshell-0.1.4/src/flask_moreshell/__main__.py
--rw-r--r--   0        0        0        0 2024-02-11 11:58:06.576458 flask_moreshell-0.1.4/src/flask_moreshell/py.typed
--rw-r--r--   0        0        0        0 2024-02-11 11:58:06.576458 flask_moreshell-0.1.4/src/flask_moreshell/shells/__init__.py
--rw-r--r--   0        0        0     1361 2024-02-11 11:58:06.576458 flask_moreshell-0.1.4/src/flask_moreshell/shells/base_shell.py
--rw-r--r--   0        0        0      542 2024-02-11 11:58:06.576458 flask_moreshell-0.1.4/src/flask_moreshell/shells/bpython_shell.py
--rw-r--r--   0        0        0     1140 2024-02-11 11:58:06.576458 flask_moreshell-0.1.4/src/flask_moreshell/shells/ipython_shell.py
--rw-r--r--   0        0        0      609 2024-02-11 11:58:06.576458 flask_moreshell-0.1.4/src/flask_moreshell/shells/ptpython_shell.py
--rw-r--r--   0        0        0      769 2024-02-11 11:58:06.576458 flask_moreshell-0.1.4/src/flask_moreshell/shells/python_shell.py
--rw-r--r--   0        0        0     4434 1970-01-01 00:00:00.000000 flask_moreshell-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-30 04:10:43.584325 flask_moreshell-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3326 2024-05-30 04:10:43.584325 flask_moreshell-0.1.5/README.md
+-rw-r--r--   0        0        0     2126 2024-05-30 04:10:54.200228 flask_moreshell-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-05-30 04:10:43.592325 flask_moreshell-0.1.5/src/flask_moreshell/__init__.py
+-rw-r--r--   0        0        0     1790 2024-05-30 04:10:43.592325 flask_moreshell-0.1.5/src/flask_moreshell/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:10:43.592325 flask_moreshell-0.1.5/src/flask_moreshell/py.typed
+-rw-r--r--   0        0        0        0 2024-05-30 04:10:43.592325 flask_moreshell-0.1.5/src/flask_moreshell/shells/__init__.py
+-rw-r--r--   0        0        0     1361 2024-05-30 04:10:43.592325 flask_moreshell-0.1.5/src/flask_moreshell/shells/base_shell.py
+-rw-r--r--   0        0        0      542 2024-05-30 04:10:43.592325 flask_moreshell-0.1.5/src/flask_moreshell/shells/bpython_shell.py
+-rw-r--r--   0        0        0     1140 2024-05-30 04:10:43.592325 flask_moreshell-0.1.5/src/flask_moreshell/shells/ipython_shell.py
+-rw-r--r--   0        0        0      609 2024-05-30 04:10:43.592325 flask_moreshell-0.1.5/src/flask_moreshell/shells/ptpython_shell.py
+-rw-r--r--   0        0        0      769 2024-05-30 04:10:43.592325 flask_moreshell-0.1.5/src/flask_moreshell/shells/python_shell.py
+-rw-r--r--   0        0        0     4304 1970-01-01 00:00:00.000000 flask_moreshell-0.1.5/PKG-INFO
```

### Comparing `flask_moreshell-0.1.4/LICENSE` & `flask_moreshell-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_moreshell-0.1.4/README.md` & `flask_moreshell-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `flask_moreshell-0.1.4/pyproject.toml` & `flask_moreshell-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-moreshell"
-version = "0.1.4"
+version = "0.1.5"
 description = "Flask Moreshell"
 authors = ["JAEGYUN JUNG <twicegoddessana1229@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tgoddessana/flask-moreshell"
 repository = "https://github.com/tgoddessana/flask-moreshell"
 documentation = "https://flask-moreshell.readthedocs.io"
@@ -14,17 +14,14 @@
 
 [tool.poetry.urls]
 Changelog = "https://github.com/tgoddessana/flask-moreshell/releases"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = ">=8.0.1"
-nox-poetry = "^1.0.3"
-nox = "^2023.4.22"
-furo = "^2023.9.10"
 
 [tool.poetry.extras]
 ipython = ["ipython"]
 ptpython = ["ptpython"]
 bpython = ["bpython"]
 all = ["ipython", "ptpython", "bpython"]
 
@@ -36,15 +33,14 @@
 black = ">=21.10b0"
 coverage = { extras = ["toml"], version = ">=6.2" }
 flake8 = ">=4.0.1"
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.5"
-furo = ">=2021.11.12"
 isort = ">=5.10.1"
 mypy = ">=0.930"
 pep8-naming = ">=0.12.1"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
 pytest = ">=6.2.5"
 pyupgrade = ">=2.29.1"
@@ -53,14 +49,17 @@
 sphinx-click = ">=3.0.2"
 xdoctest = { extras = ["colors"], version = ">=0.15.10" }
 myst-parser = { version = ">=0.16.1" }
 ipython = "^8.17.2"
 ptpython = "^3.0.23"
 bpython = "^0.24"
 flask = "^2.3"
+nox-poetry = "^1.0.3"
+nox = "^2023.4.22"
+furo = "^2023.9.10"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `flask_moreshell-0.1.4/src/flask_moreshell/__main__.py` & `flask_moreshell-0.1.5/src/flask_moreshell/__main__.py`

 * *Files identical despite different names*

### Comparing `flask_moreshell-0.1.4/src/flask_moreshell/shells/base_shell.py` & `flask_moreshell-0.1.5/src/flask_moreshell/shells/base_shell.py`

 * *Files identical despite different names*

### Comparing `flask_moreshell-0.1.4/src/flask_moreshell/shells/bpython_shell.py` & `flask_moreshell-0.1.5/src/flask_moreshell/shells/bpython_shell.py`

 * *Files identical despite different names*

### Comparing `flask_moreshell-0.1.4/src/flask_moreshell/shells/ipython_shell.py` & `flask_moreshell-0.1.5/src/flask_moreshell/shells/ipython_shell.py`

 * *Files identical despite different names*

### Comparing `flask_moreshell-0.1.4/src/flask_moreshell/shells/ptpython_shell.py` & `flask_moreshell-0.1.5/src/flask_moreshell/shells/ptpython_shell.py`

 * *Files identical despite different names*

### Comparing `flask_moreshell-0.1.4/src/flask_moreshell/shells/python_shell.py` & `flask_moreshell-0.1.5/src/flask_moreshell/shells/python_shell.py`

 * *Files identical despite different names*

### Comparing `flask_moreshell-0.1.4/PKG-INFO` & `flask_moreshell-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-moreshell
-Version: 0.1.4
+Version: 0.1.5
 Summary: Flask Moreshell
 Home-page: https://github.com/tgoddessana/flask-moreshell
 License: MIT
 Author: JAEGYUN JUNG
 Author-email: twicegoddessana1229@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,17 +15,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: bpython
 Provides-Extra: ipython
 Provides-Extra: ptpython
 Requires-Dist: click (>=8.0.1)
-Requires-Dist: furo (>=2023.9.10,<2024.0.0)
-Requires-Dist: nox (>=2023.4.22,<2024.0.0)
-Requires-Dist: nox-poetry (>=1.0.3,<2.0.0)
 Project-URL: Changelog, https://github.com/tgoddessana/flask-moreshell/releases
 Project-URL: Documentation, https://flask-moreshell.readthedocs.io
 Project-URL: Repository, https://github.com/tgoddessana/flask-moreshell
 Description-Content-Type: text/markdown
 
 <img src="https://github.com/TGoddessana/flask-moreshell/assets/88619089/804d2934-be56-4ea7-8ad8-9c787d5b2dd2" style="width: 40%">
```

