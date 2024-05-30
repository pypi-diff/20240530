# Comparing `tmp/codebleu-0.6.1.tar.gz` & `tmp/codebleu-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebleu-0.6.1.tar", last modified: Tue May 14 20:48:54 2024, max compression
+gzip compressed data, was "codebleu-0.7.0.tar", last modified: Thu May 30 10:31:55 2024, max compression
```

## Comparing `codebleu-0.6.1.tar` & `codebleu-0.7.0.tar`

### file list

```diff
@@ -1,47 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.146776 codebleu-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-14 20:48:19.000000 codebleu-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:19.000000 codebleu-0.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)   157835 2024-05-14 20:48:19.000000 codebleu-0.6.1/CodeBLEU.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-14 20:48:19.000000 codebleu-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-14 20:48:19.000000 codebleu-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-14 20:48:54.146776 codebleu-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-14 20:48:19.000000 codebleu-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 20:48:19.000000 codebleu-0.6.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.142776 codebleu-0.6.1/codebleu/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21713 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/codebleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/dataflow_match.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.142776 codebleu-0.6.1/codebleu/keywords/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/c.txt
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/c_sharp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/cpp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/go.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/java.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/javascript.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/php.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/python.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/ruby.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/rust.txt
--rwxr-xr-x   0 runner    (1001) docker     (127) 12698456 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu/my-languages.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.146776 codebleu-0.6.1/codebleu/parser/
--rw-r--r--   0 runner    (1001) docker     (127)    62313 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/parser/DFG.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/syntax_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18970 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/weighted_ngram_match.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.146776 codebleu-0.6.1/codebleu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-14 20:48:19.000000 codebleu-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:48:54.146776 codebleu-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-14 20:48:19.000000 codebleu-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.146776 codebleu-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-05-14 20:48:19.000000 codebleu-0.6.1/tests/test_codebleu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:31:55.172808 codebleu-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-30 10:31:44.000000 codebleu-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:31:44.000000 codebleu-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)   157835 2024-05-30 10:31:44.000000 codebleu-0.7.0/CodeBLEU.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-30 10:31:44.000000 codebleu-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 10:31:44.000000 codebleu-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-30 10:31:55.172808 codebleu-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-30 10:31:44.000000 codebleu-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 10:31:44.000000 codebleu-0.7.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:31:55.164807 codebleu-0.7.0/codebleu/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21713 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/codebleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/dataflow_match.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:31:55.168808 codebleu-0.7.0/codebleu/keywords/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/keywords/c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/keywords/c_sharp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/keywords/cpp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/keywords/go.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/keywords/java.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/keywords/javascript.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/keywords/php.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/keywords/python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/keywords/ruby.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/keywords/rust.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:31:55.168808 codebleu-0.7.0/codebleu/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)    62313 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/parser/DFG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/syntax_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18970 2024-05-30 10:31:44.000000 codebleu-0.7.0/codebleu/weighted_ngram_match.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:31:55.168808 codebleu-0.7.0/codebleu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-30 10:31:55.000000 codebleu-0.7.0/codebleu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-30 10:31:55.000000 codebleu-0.7.0/codebleu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:31:55.000000 codebleu-0.7.0/codebleu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 10:31:55.000000 codebleu-0.7.0/codebleu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-30 10:31:55.000000 codebleu-0.7.0/codebleu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 10:31:55.000000 codebleu-0.7.0/codebleu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-30 10:31:44.000000 codebleu-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:31:55.172808 codebleu-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:31:55.168808 codebleu-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-05-30 10:31:44.000000 codebleu-0.7.0/tests/test_codebleu.py
```

### Comparing `codebleu-0.6.1/.gitignore` & `codebleu-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/CodeBLEU.jpg` & `codebleu-0.7.0/CodeBLEU.jpg`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/LICENSE` & `codebleu-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/PKG-INFO` & `codebleu-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 Metadata-Version: 2.1
 Name: codebleu
-Version: 0.6.1
+Version: 0.7.0
 Summary: Unofficial CodeBLEU implementation that supports Linux, MacOS and Windows available on PyPI.
-Author-email: Konstantin Chernyshev <kdchernyshev@gmail.com>
+Author-email: Konstantin Chernyshev <kdchernyshev+github@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/k4black/codebleu
 Keywords: codebleu,code,bleu,nlp,natural language processing,programming,evaluate,evaluation,code generation,metrics
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tree-sitter<0.22.0,>=0.20.0
+Requires-Dist: tree-sitter<0.23.0,>=0.22.0
 Requires-Dist: setuptools>=61.0.0
+Provides-Extra: all
+Requires-Dist: tree-sitter-python~=0.21; extra == "all"
+Requires-Dist: tree-sitter-go~=0.21; extra == "all"
+Requires-Dist: tree-sitter-javascript~=0.21; extra == "all"
+Requires-Dist: tree-sitter-ruby~=0.21; extra == "all"
+Requires-Dist: tree-sitter-php~=0.22; extra == "all"
+Requires-Dist: tree-sitter-java~=0.21; extra == "all"
+Requires-Dist: tree-sitter-c-sharp~=0.21; extra == "all"
+Requires-Dist: tree-sitter-c~=0.21; extra == "all"
+Requires-Dist: tree-sitter-cpp~=0.22; extra == "all"
+Requires-Dist: tree-sitter-rust~=0.21; extra == "all"
 Provides-Extra: test
 Requires-Dist: pytest<9.0.0,>=7.0.0; extra == "test"
 Requires-Dist: pytest-cov<6.0.0,>=4.0.0; extra == "test"
 Requires-Dist: pytest-mock<4.0.0,>=3.0.0; extra == "test"
 Requires-Dist: pytest-timeout<3.0.0,>=2.0.0; extra == "test"
 Requires-Dist: black==24.4.0; extra == "test"
 Requires-Dist: mypy<2.0.0,>=1.0.0; extra == "test"
@@ -65,14 +76,28 @@
 pip install codebleu
 ```
 or directly from git repo (require internet connection to download tree-sitter):
 ```bash
 pip install git+https://github.com/k4black/codebleu.git
 ```
 
+Also you have to install tree-sitter language you need (e.g. python, rust, etc):
+```bash
+pip install tree-sitter-python
+```
+Or you can install all languages:
+```bash
+pip install codebleu[all]
+```
+
+Note: At the moment (May 2024) precompiled languages are NOT available for arm64 (M1) MacOS, so you have to install and build tree-sitter languages manually, for example:
+```bash
+pip install pip install git+https://github.com/tree-sitter/tree-sitter-python.git
+```
+
 
 ## Usage 
 
 ```python
 from codebleu import calc_codebleu
 
 prediction = "def add ( a , b ) :\n return a + b"
@@ -122,19 +147,19 @@
 If you have any questions, suggestions, or bug reports, please open an issue on GitHub.
 
 Make your own fork and clone it:
 ```bash
 git clone https://github.com/k4black/codebleu
 ```
 
-For development, you need to install library (for so file to compile) with `test` extra:  
+For development, you need to install library with `all` precompiled languages and `test` extra:  
 (require internet connection to download tree-sitter)
 ```bash
-python -m pip install -e .[test]
-python -m pip install -e .\[test\]  # for macos
+python -m pip install -e .[all,test]
+python -m pip install -e .\[all,test\]  # for macos
 ```
 
 For testing just run pytest:
 ```bash
 python -m pytest
 ```
```

### Comparing `codebleu-0.6.1/README.md` & `codebleu-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,28 @@
 pip install codebleu
 ```
 or directly from git repo (require internet connection to download tree-sitter):
 ```bash
 pip install git+https://github.com/k4black/codebleu.git
 ```
 
+Also you have to install tree-sitter language you need (e.g. python, rust, etc):
+```bash
+pip install tree-sitter-python
+```
+Or you can install all languages:
+```bash
+pip install codebleu[all]
+```
+
+Note: At the moment (May 2024) precompiled languages are NOT available for arm64 (M1) MacOS, so you have to install and build tree-sitter languages manually, for example:
+```bash
+pip install pip install git+https://github.com/tree-sitter/tree-sitter-python.git
+```
+
 
 ## Usage 
 
 ```python
 from codebleu import calc_codebleu
 
 prediction = "def add ( a , b ) :\n return a + b"
@@ -92,19 +106,19 @@
 If you have any questions, suggestions, or bug reports, please open an issue on GitHub.
 
 Make your own fork and clone it:
 ```bash
 git clone https://github.com/k4black/codebleu
 ```
 
-For development, you need to install library (for so file to compile) with `test` extra:  
+For development, you need to install library with `all` precompiled languages and `test` extra:  
 (require internet connection to download tree-sitter)
 ```bash
-python -m pip install -e .[test]
-python -m pip install -e .\[test\]  # for macos
+python -m pip install -e .[all,test]
+python -m pip install -e .\[all,test\]  # for macos
 ```
 
 For testing just run pytest:
 ```bash
 python -m pytest
 ```
```

### Comparing `codebleu-0.6.1/codebleu/__main__.py` & `codebleu-0.7.0/codebleu/__main__.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/codebleu/bleu.py` & `codebleu-0.7.0/codebleu/bleu.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/codebleu/codebleu.py` & `codebleu-0.7.0/codebleu/codebleu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 # Copyright (c) Microsoft Corporation.
 # Copyright (c) 2023 Konstantin Chernyshev.
 # Licensed under the MIT license.
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 from . import bleu, dataflow_match, syntax_match, weighted_ngram_match
+from .utils import AVAILABLE_LANGS, get_tree_sitter_language
 
 PACKAGE_DIR = Path(__file__).parent
-AVAILABLE_LANGS = [
-    "java",
-    "javascript",
-    "c_sharp",
-    "php",
-    "c",
-    "cpp",
-    "python",
-    "go",
-    "ruby",
-    "rust",
-]  # keywords available
 
 
 def calc_codebleu(
     references: Union[List[str], List[List[str]]],
     predictions: List[str],
     lang: str,
     weights: Tuple[float, float, float, float] = (0.25, 0.25, 0.25, 0.25),
     tokenizer: Optional[Callable] = None,
     keywords_dir: Path = PACKAGE_DIR / "keywords",
-    lang_so_file: Path = PACKAGE_DIR / "my-languages.so",
 ) -> Dict[str, float]:
     """Calculate CodeBLEU score
 
     Args:
         predictions: list of predictions
         references: list of lists with references
         lang: input language, one of AVAILABLE_LANGS
@@ -44,15 +32,17 @@
     Return:
         Scores dict
     """
     assert len(references) == len(predictions), "Number of references and predictions should be the same"
     assert lang in AVAILABLE_LANGS, f"Language {lang} is not supported (yet). Available languages: {AVAILABLE_LANGS}"
     assert len(weights) == 4, "weights should be a tuple of 4 floats (alpha, beta, gamma, theta)"
     assert keywords_dir.exists(), f"keywords_dir {keywords_dir} does not exist"
-    assert lang_so_file.exists(), f"lang_so_file {lang_so_file} does not exist"
+
+    # get the tree-sitter language for a given language
+    tree_sitter_language = get_tree_sitter_language(lang)
 
     # preprocess inputs
     references = [[x.strip() for x in ref] if isinstance(ref, list) else [ref.strip()] for ref in references]
     hypothesis = [x.strip() for x in predictions]
 
     # calculate ngram match (BLEU)
     if tokenizer is None:
@@ -76,18 +66,22 @@
         [[reference_tokens, make_weights(reference_tokens, keywords)] for reference_tokens in reference]
         for reference in tokenized_refs
     ]
 
     weighted_ngram_match_score = weighted_ngram_match.corpus_bleu(tokenized_refs_with_weights, tokenized_hyps)
 
     # calculate syntax match
-    syntax_match_score = syntax_match.corpus_syntax_match(references, hypothesis, lang, str(lang_so_file))
+    syntax_match_score = syntax_match.corpus_syntax_match(
+        references, hypothesis, lang, tree_sitter_language=tree_sitter_language
+    )
 
     # calculate dataflow match
-    dataflow_match_score = dataflow_match.corpus_dataflow_match(references, hypothesis, lang, str(lang_so_file))
+    dataflow_match_score = dataflow_match.corpus_dataflow_match(
+        references, hypothesis, lang, tree_sitter_language=tree_sitter_language
+    )
 
     alpha, beta, gamma, theta = weights
     code_bleu_score = (
         alpha * ngram_match_score
         + beta * weighted_ngram_match_score
         + gamma * syntax_match_score
         + theta * (dataflow_match_score or 1)
```

### Comparing `codebleu-0.6.1/codebleu/dataflow_match.py` & `codebleu-0.7.0/codebleu/dataflow_match.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 import logging
 
-from tree_sitter import Language, Parser
+from tree_sitter import Parser
 
 from .parser import (
     DFG_csharp,
     DFG_go,
     DFG_java,
     DFG_javascript,
     DFG_php,
     DFG_python,
     DFG_ruby,
     DFG_rust,
     index_to_code_token,
     remove_comments_and_docstrings,
     tree_to_token_index,
 )
+from .utils import get_tree_sitter_language
 
 dfg_function = {
     "python": DFG_python,
     "java": DFG_java,
     "ruby": DFG_ruby,
     "go": DFG_go,
     "php": DFG_php,
@@ -32,18 +33,20 @@
 }
 
 
 def calc_dataflow_match(references, candidate, lang, langso_so_file):
     return corpus_dataflow_match([references], [candidate], lang, langso_so_file)
 
 
-def corpus_dataflow_match(references, candidates, lang, langso_so_file):
-    LANGUAGE = Language(langso_so_file, lang)
+def corpus_dataflow_match(references, candidates, lang, tree_sitter_language=None):
+    if not tree_sitter_language:
+        tree_sitter_language = get_tree_sitter_language(lang)
+
     parser = Parser()
-    parser.set_language(LANGUAGE)
+    parser.language = tree_sitter_language
     parser = [parser, dfg_function[lang]]
     match_count = 0
     total_count = 0
 
     for i in range(len(candidates)):
         references_sample = references[i]
         candidate = candidates[i]
```

### Comparing `codebleu-0.6.1/codebleu/keywords/c_sharp.txt` & `codebleu-0.7.0/codebleu/keywords/c_sharp.txt`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/codebleu/keywords/cpp.txt` & `codebleu-0.7.0/codebleu/keywords/cpp.txt`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/codebleu/parser/DFG.py` & `codebleu-0.7.0/codebleu/parser/DFG.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/codebleu/parser/__init__.py` & `codebleu-0.7.0/codebleu/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/codebleu/parser/utils.py` & `codebleu-0.7.0/codebleu/parser/utils.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/codebleu/syntax_match.py` & `codebleu-0.7.0/codebleu/syntax_match.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
-from tree_sitter import Language, Parser
+from tree_sitter import Parser
 
 from .parser import (
     DFG_csharp,
     DFG_go,
     DFG_java,
     DFG_javascript,
     DFG_php,
     DFG_python,
     DFG_ruby,
     remove_comments_and_docstrings,
 )
+from .utils import get_tree_sitter_language
 
 dfg_function = {
     "python": DFG_python,
     "java": DFG_java,
     "ruby": DFG_ruby,
     "go": DFG_go,
     "php": DFG_php,
     "javascript": DFG_javascript,
     "c_sharp": DFG_csharp,
 }
 
 
-def calc_syntax_match(references, candidate, lang, lang_so_file):
-    return corpus_syntax_match([references], [candidate], lang, lang_so_file)
+def calc_syntax_match(references, candidate, lang):
+    return corpus_syntax_match([references], [candidate], lang)
 
 
-def corpus_syntax_match(references, candidates, lang, lang_so_file):
-    tree_sitter_language = Language(lang_so_file, lang)
+def corpus_syntax_match(references, candidates, lang, tree_sitter_language=None):
+    if not tree_sitter_language:
+        tree_sitter_language = get_tree_sitter_language(lang)
+
     parser = Parser()
-    parser.set_language(tree_sitter_language)
+    parser.language = tree_sitter_language
     match_count = 0
     match_count_candidate_to_reference = 0
     total_count = 0
 
     for i in range(len(candidates)):
         references_sample = references[i]
         candidate = candidates[i]
@@ -57,15 +60,15 @@
             def get_all_sub_trees(root_node):
                 node_stack = []
                 sub_tree_sexp_list = []
                 depth = 1
                 node_stack.append([root_node, depth])
                 while len(node_stack) != 0:
                     cur_node, cur_depth = node_stack.pop()
-                    sub_tree_sexp_list.append([cur_node.sexp(), cur_depth])
+                    sub_tree_sexp_list.append([str(cur_node), cur_depth])
                     for child_node in cur_node.children:
                         if len(child_node.children) != 0:
                             depth = cur_depth + 1
                             node_stack.append([child_node, depth])
                 return sub_tree_sexp_list
 
             cand_sexps = [x[0] for x in get_all_sub_trees(candidate_tree)]
```

### Comparing `codebleu-0.6.1/codebleu/weighted_ngram_match.py` & `codebleu-0.7.0/codebleu/weighted_ngram_match.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.1/codebleu.egg-info/PKG-INFO` & `codebleu-0.7.0/codebleu.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 Metadata-Version: 2.1
 Name: codebleu
-Version: 0.6.1
+Version: 0.7.0
 Summary: Unofficial CodeBLEU implementation that supports Linux, MacOS and Windows available on PyPI.
-Author-email: Konstantin Chernyshev <kdchernyshev@gmail.com>
+Author-email: Konstantin Chernyshev <kdchernyshev+github@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/k4black/codebleu
 Keywords: codebleu,code,bleu,nlp,natural language processing,programming,evaluate,evaluation,code generation,metrics
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tree-sitter<0.22.0,>=0.20.0
+Requires-Dist: tree-sitter<0.23.0,>=0.22.0
 Requires-Dist: setuptools>=61.0.0
+Provides-Extra: all
+Requires-Dist: tree-sitter-python~=0.21; extra == "all"
+Requires-Dist: tree-sitter-go~=0.21; extra == "all"
+Requires-Dist: tree-sitter-javascript~=0.21; extra == "all"
+Requires-Dist: tree-sitter-ruby~=0.21; extra == "all"
+Requires-Dist: tree-sitter-php~=0.22; extra == "all"
+Requires-Dist: tree-sitter-java~=0.21; extra == "all"
+Requires-Dist: tree-sitter-c-sharp~=0.21; extra == "all"
+Requires-Dist: tree-sitter-c~=0.21; extra == "all"
+Requires-Dist: tree-sitter-cpp~=0.22; extra == "all"
+Requires-Dist: tree-sitter-rust~=0.21; extra == "all"
 Provides-Extra: test
 Requires-Dist: pytest<9.0.0,>=7.0.0; extra == "test"
 Requires-Dist: pytest-cov<6.0.0,>=4.0.0; extra == "test"
 Requires-Dist: pytest-mock<4.0.0,>=3.0.0; extra == "test"
 Requires-Dist: pytest-timeout<3.0.0,>=2.0.0; extra == "test"
 Requires-Dist: black==24.4.0; extra == "test"
 Requires-Dist: mypy<2.0.0,>=1.0.0; extra == "test"
@@ -65,14 +76,28 @@
 pip install codebleu
 ```
 or directly from git repo (require internet connection to download tree-sitter):
 ```bash
 pip install git+https://github.com/k4black/codebleu.git
 ```
 
+Also you have to install tree-sitter language you need (e.g. python, rust, etc):
+```bash
+pip install tree-sitter-python
+```
+Or you can install all languages:
+```bash
+pip install codebleu[all]
+```
+
+Note: At the moment (May 2024) precompiled languages are NOT available for arm64 (M1) MacOS, so you have to install and build tree-sitter languages manually, for example:
+```bash
+pip install pip install git+https://github.com/tree-sitter/tree-sitter-python.git
+```
+
 
 ## Usage 
 
 ```python
 from codebleu import calc_codebleu
 
 prediction = "def add ( a , b ) :\n return a + b"
@@ -122,19 +147,19 @@
 If you have any questions, suggestions, or bug reports, please open an issue on GitHub.
 
 Make your own fork and clone it:
 ```bash
 git clone https://github.com/k4black/codebleu
 ```
 
-For development, you need to install library (for so file to compile) with `test` extra:  
+For development, you need to install library with `all` precompiled languages and `test` extra:  
 (require internet connection to download tree-sitter)
 ```bash
-python -m pip install -e .[test]
-python -m pip install -e .\[test\]  # for macos
+python -m pip install -e .[all,test]
+python -m pip install -e .\[all,test\]  # for macos
 ```
 
 For testing just run pytest:
 ```bash
 python -m pytest
 ```
```

### Comparing `codebleu-0.6.1/codebleu.egg-info/SOURCES.txt` & `codebleu-0.7.0/codebleu.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 pyproject.toml
-setup.py
 ./.gitignore
 ./CHANGELOG.md
 ./CodeBLEU.jpg
 ./LICENSE
 ./MANIFEST.in
 ./README.md
 ./VERSION
 ./pyproject.toml
-./setup.py
 ./codebleu/__init__.py
 ./codebleu/__main__.py
 ./codebleu/bleu.py
 ./codebleu/codebleu.py
 ./codebleu/dataflow_match.py
-./codebleu/my-languages.so
 ./codebleu/py.typed
 ./codebleu/syntax_match.py
 ./codebleu/utils.py
 ./codebleu/weighted_ngram_match.py
 ./codebleu/keywords/c.txt
 ./codebleu/keywords/c_sharp.txt
 ./codebleu/keywords/cpp.txt
@@ -34,15 +31,14 @@
 ./codebleu/keywords/ruby.txt
 ./codebleu/keywords/rust.txt
 codebleu/__init__.py
 codebleu/__main__.py
 codebleu/bleu.py
 codebleu/codebleu.py
 codebleu/dataflow_match.py
-codebleu/my-languages.so
 codebleu/py.typed
 codebleu/syntax_match.py
 codebleu/utils.py
 codebleu/weighted_ngram_match.py
 codebleu.egg-info/PKG-INFO
 codebleu.egg-info/SOURCES.txt
 codebleu.egg-info/dependency_links.txt
```

### Comparing `codebleu-0.6.1/tests/test_codebleu.py` & `codebleu-0.7.0/tests/test_codebleu.py`

 * *Files identical despite different names*

