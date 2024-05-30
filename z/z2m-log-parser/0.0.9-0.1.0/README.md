# Comparing `tmp/z2m_log_parser-0.0.9.tar.gz` & `tmp/z2m_log_parser-0.1.0.tar.gz`

## Comparing `z2m_log_parser-0.0.9.tar` & `z2m_log_parser-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/src/z2m_log_parser/__init__.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/src/z2m_log_parser/z2m_log_parser.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/src/z2m_log_parser/__init__.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/src/z2m_log_parser/z2m_log_parser.py
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/tests/test_z2m_log_parser.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/README.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 z2m_log_parser-0.1.0/PKG-INFO
```

### Comparing `z2m_log_parser-0.0.9/.github/workflows/python-publish.yml` & `z2m_log_parser-0.1.0/.github/workflows/python-publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -28,11 +28,13 @@
       uses: actions/setup-python@v3
       with:
         python-version: '3.12.2'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
+    - name: Run unit tests
+      run:  python -m unittest tests.test_z2m_log_parser
     - name: Build package
       run: python -m build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `z2m_log_parser-0.0.9/LICENSE` & `z2m_log_parser-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.0.9/pyproject.toml` & `z2m_log_parser-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "z2m_log_parser"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Stoyan Dimitrov", email="stdimitrov@gmail.com" },
 ]
 description = "Parser for Zigbee2Mqtt logs to python object for further processing"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

