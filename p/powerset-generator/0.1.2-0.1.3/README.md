# Comparing `tmp/powerset_generator-0.1.2.tar.gz` & `tmp/powerset_generator-0.1.3.tar.gz`

## Comparing `powerset_generator-0.1.2.tar` & `powerset_generator-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0   593705 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/..html
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/mypy.ini
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/requirements-dev.txt
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/requirements.txt
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/ruff.toml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.vscode/spellright.dict
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/make.bat
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/requirements.txt
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/source/conf.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/source/credits.rst
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/source/index.rst
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/source/usage.rst
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/source/yapp.rst
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/src/powerset_generator/__about__.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/src/powerset_generator/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/src/powerset_generator/py.typed
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/tests/test_powerset.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/LICENSE
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/README.md
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0   593705 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/..html
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/mypy.ini
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/requirements-dev.txt
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/ruff.toml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/.vscode/spellright.dict
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/docs/make.bat
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/docs/requirements.txt
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/docs/source/conf.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/docs/source/credits.rst
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/docs/source/index.rst
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/docs/source/usage.rst
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/docs/source/yapp.rst
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/src/powerset_generator/__about__.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/src/powerset_generator/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/src/powerset_generator/py.typed
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/tests/test_powerset.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/README.md
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 powerset_generator-0.1.3/PKG-INFO
```

### Comparing `powerset_generator-0.1.2/..html` & `powerset_generator-0.1.3/..html`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/CHANGELOG.md` & `powerset_generator-0.1.3/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## 0.1.3 - 2024-05-30
+
+### Improved
+
+    - README update
+
 ## 0.1.2 – 2024-05-18
 
 ### Fixed
 
     - Documentation correctly indicates that package is available.
 
 ### Updated
```

### Comparing `powerset_generator-0.1.2/ruff.toml` & `powerset_generator-0.1.3/ruff.toml`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/.github/workflows/lint.yml` & `powerset_generator-0.1.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/.github/workflows/test.yml` & `powerset_generator-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/docs/Makefile` & `powerset_generator-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/docs/make.bat` & `powerset_generator-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/docs/source/conf.py` & `powerset_generator-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/docs/source/index.rst` & `powerset_generator-0.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/docs/source/usage.rst` & `powerset_generator-0.1.3/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/docs/source/yapp.rst` & `powerset_generator-0.1.3/docs/source/yapp.rst`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/src/powerset_generator/__init__.py` & `powerset_generator-0.1.3/src/powerset_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/tests/test_powerset.py` & `powerset_generator-0.1.3/tests/test_powerset.py`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/.gitignore` & `powerset_generator-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/LICENSE` & `powerset_generator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/README.md` & `powerset_generator-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 # Python Power set generator
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[Documentation](https://jpgoldberg.github.io/powerset-generator/)
+[PyPi](https://pypi.org/project/powerset-generator/)
+
+---
+
+## Installation
+
+```console
+pip install powerset-generator
+```
+
+## Example
 
 ```python
 import powerset_generator
 
 for e in powerset_generator.subsets(["one", "two", "three", "three"]):
     print(e)
 ```
```

### Comparing `powerset_generator-0.1.2/pyproject.toml` & `powerset_generator-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.2/PKG-INFO` & `powerset_generator-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerset-generator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate the power set of a collection
 Project-URL: Documentation, https://jpgoldberg.github.io/powerset-generator/
 Project-URL: Issues, https://github.com/jpgoldberg/powerset-generator/issues
 Project-URL: Source, https://github.com/jpgoldberg/powerset-generator
 Project-URL: Changelog, https://github.com/jpgoldberg/powerset-generator/blob/main/CHANGELOG.md
 Author-email: Jeffrey Goldberg <jeffrey@goldmark.org>
 License: MIT Licesne
@@ -22,14 +22,26 @@
 Description-Content-Type: text/markdown
 
 # Python Power set generator
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[Documentation](https://jpgoldberg.github.io/powerset-generator/)
+[PyPi](https://pypi.org/project/powerset-generator/)
+
+---
+
+## Installation
+
+```console
+pip install powerset-generator
+```
+
+## Example
 
 ```python
 import powerset_generator
 
 for e in powerset_generator.subsets(["one", "two", "three", "three"]):
     print(e)
 ```
```

