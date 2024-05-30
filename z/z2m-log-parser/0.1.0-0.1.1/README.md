# Comparing `tmp/z2m_log_parser-0.1.0.tar.gz` & `tmp/z2m_log_parser-0.1.1.tar.gz`

## Comparing `z2m_log_parser-0.1.0.tar` & `z2m_log_parser-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/src/z2m_log_parser/__init__.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/src/z2m_log_parser/z2m_log_parser.py
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/tests/test_z2m_log_parser.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/LICENSE
--rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.1/src/z2m_log_parser/__init__.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.1/src/z2m_log_parser/z2m_log_parser.py
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.1/tests/test_z2m_log_parser.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.1/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.1/PKG-INFO
```

### Comparing `z2m_log_parser-0.1.0/.github/workflows/python-publish.yml` & `z2m_log_parser-0.1.1/.github/workflows/python-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     permissions:
       id-token: write
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
-        python-version: '3.12.2'
+        python-version: '3.9'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Run unit tests
       run:  python -m unittest tests.test_z2m_log_parser
     - name: Build package
```

### Comparing `z2m_log_parser-0.1.0/src/z2m_log_parser/z2m_log_parser.py` & `z2m_log_parser-0.1.1/src/z2m_log_parser/z2m_log_parser.py`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.1.0/tests/test_z2m_log_parser.py` & `z2m_log_parser-0.1.1/tests/test_z2m_log_parser.py`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.1.0/LICENSE` & `z2m_log_parser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.1.0/README.md` & `z2m_log_parser-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.1.0/pyproject.toml` & `z2m_log_parser-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "z2m_log_parser"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Stoyan Dimitrov", email="stdimitrov@gmail.com" },
 ]
 description = "Parser for Zigbee2Mqtt logs to python object for further processing"
 readme = "README.md"
-requires-python = ">=3.12"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `z2m_log_parser-0.1.0/PKG-INFO` & `z2m_log_parser-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: z2m_log_parser
-Version: 0.1.0
+Version: 0.1.1
 Summary: Parser for Zigbee2Mqtt logs to python object for further processing
 Project-URL: Homepage, https://github.com/st0yanDimitrov/z2m_log_parser
 Project-URL: Issues, https://github.com/st0yanDimitrov/z2m_log_parser/issues
 Author-email: Stoyan Dimitrov <stdimitrov@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # zigbee2mqtt log parser
 
 A simple module for parsing of zigbee2mqtt logs into Python object for further processing.
 
 ## How to install:
```

