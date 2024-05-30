# Comparing `tmp/booktest-0.3.7.tar.gz` & `tmp/booktest-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "booktest-0.3.7.tar", max compression
+gzip compressed data, was "booktest-0.3.8.tar", max compression
```

## Comparing `booktest-0.3.7.tar` & `booktest-0.3.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1296 2023-10-25 19:25:11.461339 booktest-0.3.7/LICENSE
--rw-r--r--   0        0        0      817 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/__init__.py
--rw-r--r--   0        0        0       69 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/__main__.py
--rw-r--r--   0        0        0      578 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/booktest.py
--rw-r--r--   0        0        0     1301 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/cache.py
--rw-r--r--   0        0        0     3685 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/cli.py
--rw-r--r--   0        0        0     1317 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/config.py
--rw-r--r--   0        0        0     1491 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/dependencies.py
--rw-r--r--   0        0        0     1694 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/detection.py
--rw-r--r--   0        0        0     1859 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/naming.py
--rw-r--r--   0        0        0     3459 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/reports.py
--rw-r--r--   0        0        0     8057 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/review.py
--rw-r--r--   0        0        0     5573 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/runs.py
--rw-r--r--   0        0        0     2504 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/testbook.py
--rw-r--r--   0        0        0    17637 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/testcaserun.py
--rw-r--r--   0        0        0     5741 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/testrun.py
--rw-r--r--   0        0        0    13808 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/tests.py
--rw-r--r--   0        0        0     1010 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/testsuite.py
--rw-r--r--   0        0        0     2270 2023-10-25 19:25:11.465339 booktest-0.3.7/booktest/tokenizer.py
--rw-r--r--   0        0        0      863 2023-10-25 19:25:11.465339 booktest-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    10627 2023-10-25 19:25:11.465339 booktest-0.3.7/readme.md
--rw-r--r--   0        0        0    11514 1970-01-01 00:00:00.000000 booktest-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1296 2023-11-17 20:24:24.620041 booktest-0.3.8/LICENSE
+-rw-r--r--   0        0        0      817 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/__init__.py
+-rw-r--r--   0        0        0       69 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/__main__.py
+-rw-r--r--   0        0        0      578 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/booktest.py
+-rw-r--r--   0        0        0     1301 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/cache.py
+-rw-r--r--   0        0        0     1255 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/cli.py
+-rw-r--r--   0        0        0     1317 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/config.py
+-rw-r--r--   0        0        0     1491 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/dependencies.py
+-rw-r--r--   0        0        0     1694 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/detection.py
+-rw-r--r--   0        0        0     1859 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/naming.py
+-rw-r--r--   0        0        0     3459 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/reports.py
+-rw-r--r--   0        0        0     8057 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/review.py
+-rw-r--r--   0        0        0     5573 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/runs.py
+-rw-r--r--   0        0        0     2216 2023-11-17 20:24:24.620041 booktest-0.3.8/booktest/setup.py
+-rw-r--r--   0        0        0     2504 2023-11-17 20:24:24.624040 booktest-0.3.8/booktest/testbook.py
+-rw-r--r--   0        0        0    17637 2023-11-17 20:24:24.624040 booktest-0.3.8/booktest/testcaserun.py
+-rw-r--r--   0        0        0     5741 2023-11-17 20:24:24.624040 booktest-0.3.8/booktest/testrun.py
+-rw-r--r--   0        0        0    14095 2023-11-17 20:24:24.624040 booktest-0.3.8/booktest/tests.py
+-rw-r--r--   0        0        0     1010 2023-11-17 20:24:24.624040 booktest-0.3.8/booktest/testsuite.py
+-rw-r--r--   0        0        0     2270 2023-11-17 20:24:24.624040 booktest-0.3.8/booktest/tokenizer.py
+-rw-r--r--   0        0        0      864 2023-11-17 20:24:24.624040 booktest-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     9131 2023-11-17 20:24:24.624040 booktest-0.3.8/readme.md
+-rw-r--r--   0        0        0    10070 1970-01-01 00:00:00.000000 booktest-0.3.8/PKG-INFO
```

### Comparing `booktest-0.3.7/LICENSE` & `booktest-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/__init__.py` & `booktest-0.3.8/booktest/__init__.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/booktest.py` & `booktest-0.3.8/booktest/booktest.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/cache.py` & `booktest-0.3.8/booktest/cache.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/config.py` & `booktest-0.3.8/booktest/config.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/dependencies.py` & `booktest-0.3.8/booktest/dependencies.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/detection.py` & `booktest-0.3.8/booktest/detection.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/naming.py` & `booktest-0.3.8/booktest/naming.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/reports.py` & `booktest-0.3.8/booktest/reports.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/review.py` & `booktest-0.3.8/booktest/review.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/runs.py` & `booktest-0.3.8/booktest/runs.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/testbook.py` & `booktest-0.3.8/booktest/testbook.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/testcaserun.py` & `booktest-0.3.8/booktest/testcaserun.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/testrun.py` & `booktest-0.3.8/booktest/testrun.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/tests.py` & `booktest-0.3.8/booktest/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from coverage import Coverage
 
 from booktest.cache import LruCache
 from booktest.review import run_tool, review
 from booktest.runs import parallel_run_tests, run_tests
 from booktest.config import get_default_config
+import booktest.setup
 
 
 class Tests:
     def __init__(self, cases):
         self.cases = cases
 
     def is_selected(self, test_name, selection):
@@ -165,15 +166,21 @@
         )
         parser.add_argument(
             '-l',
             action='store_const',
             dest='cmd',
             const="-l",
             help="lists the selected test cases")
-
+        parser.add_argument(
+            "--setup",
+            action='store_const',
+            dest='cmd',
+            const="--setup",
+            help="setups booktest"
+        )
         parser.add_argument(
             '--garbage',
             action='store_const',
             dest='cmd',
             const="--garbage",
             help="prints the garbage files")
 
@@ -324,15 +331,17 @@
         if test_cases == "*":
             test_cases = config.get("default_tests", "test,book").split(",")
 
         cases = self.selected_names(test_cases, cache_out_dir)
 
         cmd = parsed.cmd
 
-        if cmd == '--config':
+        if cmd == '--setup':
+            return booktest.setup.setup_booktest()
+        elif cmd == '--config':
             for key, value in config.items():
                 print(f"{key}={value}")
             return 0
         elif cmd == '--garbage':
             for p in garbage():
                 print(f"{p}")
             return 0
```

### Comparing `booktest-0.3.7/booktest/testsuite.py` & `booktest-0.3.8/booktest/testsuite.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/booktest/tokenizer.py` & `booktest-0.3.8/booktest/tokenizer.py`

 * *Files identical despite different names*

### Comparing `booktest-0.3.7/pyproject.toml` & `booktest-0.3.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "booktest"
-version = "0.3.7"
-authors = ["Antt Rauhala <antti@lumoa.io>"]
+version = "0.3.8"
+authors = ["Antti Rauhala <antti@lumoa.me>"]
 description = "Booktest is a snapshot testing library for review driven testing."
 readme = "readme.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent"
```

### Comparing `booktest-0.3.7/readme.md` & `booktest-0.3.8/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -95,19 +95,19 @@
 uses default directory paths for looking up tests, for storing the books and for
 storing caches and the output. 
 
 These tools depend on the OS, environment and user preferences. 
 To choose tools that work for you, you can run the setup script:
 
 ```bash
-booktest setup
+booktest --setup
 ```
 
 NOTE: that this operation will create a .booktest file in the local directory. You
-can edit the file by hand safely. Rerunning `booktest setup` will read the configuration
+can edit the file by hand safely. Rerunning `booktest --setup` will read the configuration
 and propose existing as defaults.
 
 NOTE that you can also store a .booktest file in your home directory to provide cross-project 
 default settings. These settings will be overriden by project specific .booktest or 
 environment variables of form BOOKTEST_VARIABLE_NAME. E.g. BOOKTEST_MD_VIEWER will 
 override .booktest file md_viewer configuration.
 
@@ -224,66 +224,14 @@
 - booktest || booktest -w -v -c
 ```
 
 `booktest` will run all test cases and `booktest -w -v -c` 
 print verbose review of all failed test cases, if the 
 run failed.
 
-## Tips and tricks
-
-### Enable autocomplete
-
-To enable the autocomplete, run the following in bash:
-
-```bash
-eval "$(register-python-argcomplete booktest)"
-```
-
-### Integrating booktest to CLI interface using argparse
-
-It often helps both the developer workflow and introducing other people 
-into the project, if you provide a simple developer CLI interface for
-running common tasks in the project. 
-
-This CLI interface may include commands for e.g. linting the code, 
-deploying pypi packages or running tests.
-
-As long your CLI interface uses the Python argparse, integrating the 
-booktest should be easy. You can follow the example in the `do.py` and 
-`do` scripts in this project:
-
-```python
-import argparse
-import argcomplete
-import sys
-import test.tests as tests
-
-parser = argparse.ArgumentParser()
-
-subparsers = parser.add_subparsers(help='sub-command help')
-
-# TODO: add your own parsers
-tests_parser = subparsers.add_parser("test")
-tests.setup_parser(tests_parser)
-tests_parser.set_defaults(
-    exec=lambda parsed:
-    tests.exec_parsed("books/test",
-                      parsed))
-
-argcomplete.autocomplete(parser)
-parsed = parser.parse_args(sys.args)
-
-exit(parsed.exec(parsed))
-```
-
-After the integration, you can run the test cases with:
-
-```
-./do test examples/hello
-```
 
 ### Tests and runs
 
 In data science, there are often 2 different needs related to booktest:
 
  - Regression testing, which is run in CI and run locally to assert
    quality. Regression testing should always use public data, and 
@@ -296,43 +244,28 @@
    data, the data or test results cannot maintained in Git.
    
 Booktest can help maintaining and rerunning the real world tests, which 
 may still be necessary for asserting the system real word performance and 
 quality and for doing exploratory analysis. 
 
 You may want to save the run data separately and supply separate method
-for loading test data.
-
-```
-./do load-run-data
-```
-
-After this, you can create a separate test suite for the runs with 
-separate integration
-
-```
-runs_parser = subparsers.add_parser("run")
-runs.setup_parser(tests_parser)
-runs_parser.set_defaults(
-    exec=lambda parsed:
-        runs.exec_parsed("books/runs",
-                         parsed))
-```
+for loading test data. After this, you can create a separate test suite for 
+the runs in a separate directory called 'run'.
 
 After this, the runs can be executed with:
 
 ```bash
-./do run -v -i real-world-case
+booktest -v -i run/real-world-case
 ```
 
 Similar integrations can be done for e.g. performance testing, which 
 may be slow enough to be maintained and run non-regularly and outside CI:
 
 ```bash
-./do perf -v -i slow-perfomance-test
+booktest -v -i perf/slow-perfomance-test
 ```
 
 # Developing booktest
 
 This guides through the basic steps of building booktest locally and 
 running it's tests.
```

### Comparing `booktest-0.3.7/PKG-INFO` & `booktest-0.3.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: booktest
-Version: 0.3.7
+Version: 0.3.8
 Summary: Booktest is a snapshot testing library for review driven testing.
 Home-page: https://github.com/lumoa-oss/booktest
-Author: Antt Rauhala
-Author-email: antti@lumoa.io
+Author: Antti Rauhala
+Author-email: antti@lumoa.me
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argcomplete (>=2.0.0,<3.0.0)
 Requires-Dist: coverage (>=6.5.0,<7.0.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/lumoa-oss/booktest
 Description-Content-Type: text/markdown
 
 # Booktest
@@ -117,19 +118,19 @@
 uses default directory paths for looking up tests, for storing the books and for
 storing caches and the output. 
 
 These tools depend on the OS, environment and user preferences. 
 To choose tools that work for you, you can run the setup script:
 
 ```bash
-booktest setup
+booktest --setup
 ```
 
 NOTE: that this operation will create a .booktest file in the local directory. You
-can edit the file by hand safely. Rerunning `booktest setup` will read the configuration
+can edit the file by hand safely. Rerunning `booktest --setup` will read the configuration
 and propose existing as defaults.
 
 NOTE that you can also store a .booktest file in your home directory to provide cross-project 
 default settings. These settings will be overriden by project specific .booktest or 
 environment variables of form BOOKTEST_VARIABLE_NAME. E.g. BOOKTEST_MD_VIEWER will 
 override .booktest file md_viewer configuration.
 
@@ -246,66 +247,14 @@
 - booktest || booktest -w -v -c
 ```
 
 `booktest` will run all test cases and `booktest -w -v -c` 
 print verbose review of all failed test cases, if the 
 run failed.
 
-## Tips and tricks
-
-### Enable autocomplete
-
-To enable the autocomplete, run the following in bash:
-
-```bash
-eval "$(register-python-argcomplete booktest)"
-```
-
-### Integrating booktest to CLI interface using argparse
-
-It often helps both the developer workflow and introducing other people 
-into the project, if you provide a simple developer CLI interface for
-running common tasks in the project. 
-
-This CLI interface may include commands for e.g. linting the code, 
-deploying pypi packages or running tests.
-
-As long your CLI interface uses the Python argparse, integrating the 
-booktest should be easy. You can follow the example in the `do.py` and 
-`do` scripts in this project:
-
-```python
-import argparse
-import argcomplete
-import sys
-import test.tests as tests
-
-parser = argparse.ArgumentParser()
-
-subparsers = parser.add_subparsers(help='sub-command help')
-
-# TODO: add your own parsers
-tests_parser = subparsers.add_parser("test")
-tests.setup_parser(tests_parser)
-tests_parser.set_defaults(
-    exec=lambda parsed:
-    tests.exec_parsed("books/test",
-                      parsed))
-
-argcomplete.autocomplete(parser)
-parsed = parser.parse_args(sys.args)
-
-exit(parsed.exec(parsed))
-```
-
-After the integration, you can run the test cases with:
-
-```
-./do test examples/hello
-```
 
 ### Tests and runs
 
 In data science, there are often 2 different needs related to booktest:
 
  - Regression testing, which is run in CI and run locally to assert
    quality. Regression testing should always use public data, and 
@@ -318,43 +267,28 @@
    data, the data or test results cannot maintained in Git.
    
 Booktest can help maintaining and rerunning the real world tests, which 
 may still be necessary for asserting the system real word performance and 
 quality and for doing exploratory analysis. 
 
 You may want to save the run data separately and supply separate method
-for loading test data.
-
-```
-./do load-run-data
-```
-
-After this, you can create a separate test suite for the runs with 
-separate integration
-
-```
-runs_parser = subparsers.add_parser("run")
-runs.setup_parser(tests_parser)
-runs_parser.set_defaults(
-    exec=lambda parsed:
-        runs.exec_parsed("books/runs",
-                         parsed))
-```
+for loading test data. After this, you can create a separate test suite for 
+the runs in a separate directory called 'run'.
 
 After this, the runs can be executed with:
 
 ```bash
-./do run -v -i real-world-case
+booktest -v -i run/real-world-case
 ```
 
 Similar integrations can be done for e.g. performance testing, which 
 may be slow enough to be maintained and run non-regularly and outside CI:
 
 ```bash
-./do perf -v -i slow-perfomance-test
+booktest -v -i perf/slow-perfomance-test
 ```
 
 # Developing booktest
 
 This guides through the basic steps of building booktest locally and 
 running it's tests.
```

