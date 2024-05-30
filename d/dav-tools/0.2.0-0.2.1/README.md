# Comparing `tmp/dav_tools-0.2.0.tar.gz` & `tmp/dav_tools-0.2.1.tar.gz`

## Comparing `dav_tools-0.2.0.tar` & `dav_tools-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 dav_tools-0.2.0/Makefile
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.2.0/docs/Makefile
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.2.0/docs/conf.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.2.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.2.0/docs/make.bat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.2.0/docs/requirements.txt
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/__init__.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/_arg_parser.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/_text_format.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/commands.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/database.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/devtools.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/messages.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/requirements.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/text_format.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dav_tools-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dav_tools-0.2.0/tests/test_messages.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dav_tools-0.2.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.2.0/LICENSE
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 dav_tools-0.2.0/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dav_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 dav_tools-0.2.1/Makefile
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.2.1/docs/conf.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.2.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.2.1/docs/requirements.txt
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.2.1/src/dav_tools/__init__.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 dav_tools-0.2.1/src/dav_tools/_arg_parser.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dav_tools-0.2.1/src/dav_tools/_text_format.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 dav_tools-0.2.1/src/dav_tools/commands.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 dav_tools-0.2.1/src/dav_tools/database.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.2.1/src/dav_tools/devtools.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 dav_tools-0.2.1/src/dav_tools/messages.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 dav_tools-0.2.1/src/dav_tools/requirements.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 dav_tools-0.2.1/src/dav_tools/text_format.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dav_tools-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dav_tools-0.2.1/tests/test_messages.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dav_tools-0.2.1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.2.1/LICENSE
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 dav_tools-0.2.1/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 dav_tools-0.2.1/PKG-INFO
```

### Comparing `dav_tools-0.2.0/.readthedocs.yaml` & `dav_tools-0.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/Makefile` & `dav_tools-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/docs/Makefile` & `dav_tools-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/docs/conf.py` & `dav_tools-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/docs/index.rst` & `dav_tools-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/docs/make.bat` & `dav_tools-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/src/dav_tools/_arg_parser.py` & `dav_tools-0.2.1/src/dav_tools/_arg_parser.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/src/dav_tools/_text_format.py` & `dav_tools-0.2.1/src/dav_tools/_text_format.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/src/dav_tools/commands.py` & `dav_tools-0.2.1/src/dav_tools/commands.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/src/dav_tools/database.py` & `dav_tools-0.2.1/src/dav_tools/database.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/src/dav_tools/devtools.py` & `dav_tools-0.2.1/src/dav_tools/devtools.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/src/dav_tools/messages.py` & `dav_tools-0.2.1/src/dav_tools/messages.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/src/dav_tools/requirements.py` & `dav_tools-0.2.1/src/dav_tools/requirements.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/src/dav_tools/text_format.py` & `dav_tools-0.2.1/src/dav_tools/text_format.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/tests/test_messages.py` & `dav_tools-0.2.1/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/LICENSE` & `dav_tools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dav_tools-0.2.0/pyproject.toml` & `dav_tools-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dav_tools"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Davide Ponzini", email="davide.ponzini95@gmail.com" },
 ]
 description = "Various utilies to aid in program development."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dav_tools-0.2.0/PKG-INFO` & `dav_tools-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dav_tools
-Version: 0.2.0
+Version: 0.2.1
 Summary: Various utilies to aid in program development.
 Project-URL: Repository, https://github.com/DavidePonzini/dav-utils
 Project-URL: Documentation, https://dav-tools.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/DavidePonzini/dav-utils/issues
 Author-email: Davide Ponzini <davide.ponzini95@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,15 +19,24 @@
 Personal Python library to aid in software development
 
 ## Installation
 ```bash
 $ pip install dav-tools
 ```
 
-## Usage
+## Usage on python programs
 `dav-tools` contains a variety of diffent submodules, each with its own set of functionalities.
 
 Importing is done in the form of
 ```python
 from dav_tools import <submodule>
 ```
 since it usually doesn't make sense to import the whole library.
+
+## Usage on non-python programs
+Some modules can also be executed in other scripts, using:
+```bash
+python -m dav_tools.modulename [options]
+```
+
+Only basic functionalities are available.
+Error management requires the original program to exit if a subcommand exits with an error code.
```

