# Comparing `tmp/pytest_custom_outputs-0.1.0.tar.gz` & `tmp/pytest_custom_outputs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_custom_outputs-0.1.0.tar", last modified: Wed May 29 23:12:50 2024, max compression
+gzip compressed data, was "pytest_custom_outputs-0.1.1.tar", last modified: Thu May 30 00:54:14 2024, max compression
```

## Comparing `pytest_custom_outputs-0.1.0.tar` & `pytest_custom_outputs-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-29 23:12:50.670858 pytest_custom_outputs-0.1.0/
--rw-r--r--   0 user      (1000) vboxusers   (136)     1501 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.1.0/LICENSE
--rw-r--r--   0 user      (1000) vboxusers   (136)     9681 2024-05-29 23:12:50.670858 pytest_custom_outputs-0.1.0/PKG-INFO
--rw-r--r--   0 user      (1000) vboxusers   (136)     6685 2024-05-29 23:07:14.000000 pytest_custom_outputs-0.1.0/README.rst
--rw-r--r--   0 user      (1000) vboxusers   (136)     1490 2024-05-29 23:12:23.000000 pytest_custom_outputs-0.1.0/pyproject.toml
--rw-r--r--   0 user      (1000) vboxusers   (136)       38 2024-05-29 23:12:50.670858 pytest_custom_outputs-0.1.0/setup.cfg
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-29 23:12:50.670858 pytest_custom_outputs-0.1.0/src/
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-29 23:12:50.670858 pytest_custom_outputs-0.1.0/src/pytest_custom_outputs/
--rw-r--r--   0 user      (1000) vboxusers   (136)        0 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.1.0/src/pytest_custom_outputs/__init__.py
--rw-r--r--   0 user      (1000) vboxusers   (136)     2390 2024-04-09 23:37:27.000000 pytest_custom_outputs-0.1.0/src/pytest_custom_outputs/custom_outputs.py
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-29 23:12:50.670858 pytest_custom_outputs-0.1.0/src/pytest_custom_outputs.egg-info/
--rw-r--r--   0 user      (1000) vboxusers   (136)     9681 2024-05-29 23:12:50.000000 pytest_custom_outputs-0.1.0/src/pytest_custom_outputs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) vboxusers   (136)      411 2024-05-29 23:12:50.000000 pytest_custom_outputs-0.1.0/src/pytest_custom_outputs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)        1 2024-05-29 23:12:50.000000 pytest_custom_outputs-0.1.0/src/pytest_custom_outputs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       65 2024-05-29 23:12:50.000000 pytest_custom_outputs-0.1.0/src/pytest_custom_outputs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       14 2024-05-29 23:12:50.000000 pytest_custom_outputs-0.1.0/src/pytest_custom_outputs.egg-info/requires.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       22 2024-05-29 23:12:50.000000 pytest_custom_outputs-0.1.0/src/pytest_custom_outputs.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/
+-rw-r--r--   0 user      (1000) vboxusers   (136)     1501 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.1.1/LICENSE
+-rw-r--r--   0 user      (1000) vboxusers   (136)     9671 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/PKG-INFO
+-rw-r--r--   0 user      (1000) vboxusers   (136)     6675 2024-05-30 00:52:21.000000 pytest_custom_outputs-0.1.1/README.rst
+-rw-r--r--   0 user      (1000) vboxusers   (136)     1490 2024-05-30 00:52:45.000000 pytest_custom_outputs-0.1.1/pyproject.toml
+-rw-r--r--   0 user      (1000) vboxusers   (136)       38 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/setup.cfg
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/src/
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs/
+-rw-r--r--   0 user      (1000) vboxusers   (136)        0 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs/__init__.py
+-rw-r--r--   0 user      (1000) vboxusers   (136)     2390 2024-04-09 23:37:27.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs/custom_outputs.py
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/
+-rw-r--r--   0 user      (1000) vboxusers   (136)     9671 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) vboxusers   (136)      411 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)        1 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       65 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       14 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       22 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/top_level.txt
```

### Comparing `pytest_custom_outputs-0.1.0/LICENSE` & `pytest_custom_outputs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_custom_outputs-0.1.0/PKG-INFO` & `pytest_custom_outputs-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-custom_outputs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A plugin that allows users to create and use custom outputs instead of the standard Pass and Fail
 Author-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 Maintainer-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 License: 
         Copyright (c) 2024, Babak Michael Engheta
         All rights reserved.
         
@@ -50,51 +50,56 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest>=6.2.0
 
-=====================
 pytest-custom_outputs
-=====================
+
+Overview
+--------
+
+Enhance Your Pytest Reporting with Customizable Test Outputs
+
+Tired of the standard pass/fail binary in pytest? With pytest-custom_outputs, you can create expressive and informative custom test results that go beyond the ordinary.  Tailor your reports to provide deeper insights into your test scenarios.
+
+Useful for if you want more than just the default Pass, Fail, and Skip outcomes.
+
 
 Features
 --------
 
-- Useful for if you want more than just the default Pass, Fail, and Skip outcomes.
-- Allows for the creation and usage of custom outputs.
-- Custom outputs are filled out in a file called "pytest_custom_outputs.json".
-- Custom outputs are customizable in their name, description, result code, tag, and color.
-- Supports the creation of an unknown output. If no result matches a default or custom output, then it will be categorized as an unknown output.
-- Unknown outputs are also fully customizable.
+- Flexible Output Types: Define new outcome types like "unimplemented", "soft_fail"," "inconclusive," or any custom label that suits your testing needs.
+- Fully Customizeable: Custom outputs are customizable in their name, description, result code, tag, and color.
+- Seamless Integration: Easily incorporate custom outputs into your existing pytest test suites.
+- Terminal and File Reporting: View your custom outputs in both your terminal output and pytest file reports.
 
 
 Requirements
 ------------
 
 None
 
 
 Installation
 ------------
 
-You can install "pytest-custom_outputs" via `pip`_ from `PyPI`_::
-
-    $ pip install pytest-custom_outputs
+pip install pytest-custom_outputs
 
 
 Usage
 -----
 
 In the directory where you will be running your pytest, create a file called "pytest_custom_outputs.json".
 You will use this file to create your own custom outputs.
+Feel free to copy and paste the below json file into yours and edit from there.
 
 EXAMPLE FILE:
-###STARTS HERE###
+```python
 {
         "use_unknown_if_no_match": true,
         "unknown": {
                 "attribute":"_unknown",
                 "status": {
                         "desc":"unknown",
                         "code":"?",
@@ -169,68 +174,74 @@
                                         "tag":"SKIPPED",
                                         "color":"yellow"
                                 }
                         }
                 }
         }
 }
-###ENDS HERE###
+```
+
+
+use_unknown_if_no_match
+ - If True, use the unknown output below if there is no match. Otherwise, use standard skip
 
+unknown
+ - The output to use if a test's result is not in default or custom outputs 
+
+custom_outputs
+ - A dictionary with all the custom outputs you write inside of it. You can edit, delete, and add new outputs here.
 
-use_unknown_if_no_match -> If True, use the unknown output below if there is no match. Otherwise, use standard skip
-unknown -> The output to use if a test's result is not in default or custom outputs 
-custom_outputs -> A dictionary with all the custom outputs you write inside of it. You can edit, delete, and add new outputs here.
 
 Each custom output is denoted by a name. The name is also the key for that output
 For example, in the above example file, "Pass_with_exception" and "Fatal_failed" are the names for their respective output.
 Names are also how we determine the result of a test case. 
 This is done by using skip followed by the name in the parameter.
 
 For example:
-        import pytest
-        from pytest import skip
-
-        def test_1():
-                skip("Pass_with_exception")
-
+```python
+import pytest
+from pytest import skip
+
+def test_1():
+    skip("Pass_with_exception")
+```
 
 In the example above, test_1 will result in "passed_with_exception".
 Because the name overrides the outcome, it will not result in a skip.
-We use the keyword skip as a means to obtaining out desired outcome.
+We use the keyword skip as a means to obtaining our desired outcome.
 
 If we put a name that is not in our custom output in the skip parameter,
-then
-        if we set unknown to True in the json, we will use the unknown outcome
-        else we will use the default skip and pass the name as a message (Standard skip behavior)
+then the following occurs:
+ - if we set unknown to True in the json, we will use the unknown outcome
+ - else we will use the default skip and pass the name as a message (Standard skip behavior)
+
 
+The rest of the information in the json file can be edited and customized to your liking.
 
-The rest of the information in the json file can be edited and customized to your liking. 
+
+Why pytest-custom_outputs?
+--------------------------
+
+- Improved Communication: Get more informative insights from your test runs
+- Focus on Key Areas: Prioritize test cases that require attention
+- Tailored for Your Needs: Adapt outcomes and messages to your project's specific requirements
 
 
 Contributing
 ------------
+
 Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
+
 License
 -------
 
 Distributed under the terms of the `BSD-3`_ license, "pytest-custom_outputs" is free and open source software
 
 
 Issues
 ------
 
 If you encounter any problems, please `file an issue`_ along with a detailed description.
 
-.. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
-.. _`@hackebrot`: https://github.com/hackebrot
-.. _`MIT`: https://opensource.org/licenses/MIT
-.. _`BSD-3`: https://opensource.org/licenses/BSD-3-Clause
-.. _`GNU GPL v3.0`: https://www.gnu.org/licenses/gpl-3.0.txt
-.. _`Apache Software License 2.0`: https://www.apache.org/licenses/LICENSE-2.0
-.. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 .. _`file an issue`: https://github.com/MichaelE55/pytest-custom_outputs/issues
-.. _`pytest`: https://github.com/pytest-dev/pytest
-.. _`tox`: https://tox.readthedocs.io/en/latest/
-.. _`pip`: https://pypi.org/project/pip/
-.. _`PyPI`: https://pypi.org/project
```

### Comparing `pytest_custom_outputs-0.1.0/README.rst` & `pytest_custom_outputs-0.1.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-=====================
 pytest-custom_outputs
-=====================
+
+Overview
+--------
+
+Enhance Your Pytest Reporting with Customizable Test Outputs
+
+Tired of the standard pass/fail binary in pytest? With pytest-custom_outputs, you can create expressive and informative custom test results that go beyond the ordinary.  Tailor your reports to provide deeper insights into your test scenarios.
+
+Useful for if you want more than just the default Pass, Fail, and Skip outcomes.
+
 
 Features
 --------
 
-- Useful for if you want more than just the default Pass, Fail, and Skip outcomes.
-- Allows for the creation and usage of custom outputs.
-- Custom outputs are filled out in a file called "pytest_custom_outputs.json".
-- Custom outputs are customizable in their name, description, result code, tag, and color.
-- Supports the creation of an unknown output. If no result matches a default or custom output, then it will be categorized as an unknown output.
-- Unknown outputs are also fully customizable.
+- Flexible Output Types: Define new outcome types like "unimplemented", "soft_fail"," "inconclusive," or any custom label that suits your testing needs.
+- Fully Customizeable: Custom outputs are customizable in their name, description, result code, tag, and color.
+- Seamless Integration: Easily incorporate custom outputs into your existing pytest test suites.
+- Terminal and File Reporting: View your custom outputs in both your terminal output and pytest file reports.
 
 
 Requirements
 ------------
 
 None
 
 
 Installation
 ------------
 
-You can install "pytest-custom_outputs" via `pip`_ from `PyPI`_::
-
-    $ pip install pytest-custom_outputs
+pip install pytest-custom_outputs
 
 
 Usage
 -----
 
 In the directory where you will be running your pytest, create a file called "pytest_custom_outputs.json".
 You will use this file to create your own custom outputs.
+Feel free to copy and paste the below json file into yours and edit from there.
 
 EXAMPLE FILE:
-###STARTS HERE###
+```python
 {
         "use_unknown_if_no_match": true,
         "unknown": {
                 "attribute":"_unknown",
                 "status": {
                         "desc":"unknown",
                         "code":"?",
@@ -113,68 +118,74 @@
                                         "tag":"SKIPPED",
                                         "color":"yellow"
                                 }
                         }
                 }
         }
 }
-###ENDS HERE###
+```
+
+
+use_unknown_if_no_match
+ - If True, use the unknown output below if there is no match. Otherwise, use standard skip
 
+unknown
+ - The output to use if a test's result is not in default or custom outputs 
+
+custom_outputs
+ - A dictionary with all the custom outputs you write inside of it. You can edit, delete, and add new outputs here.
 
-use_unknown_if_no_match -> If True, use the unknown output below if there is no match. Otherwise, use standard skip
-unknown -> The output to use if a test's result is not in default or custom outputs 
-custom_outputs -> A dictionary with all the custom outputs you write inside of it. You can edit, delete, and add new outputs here.
 
 Each custom output is denoted by a name. The name is also the key for that output
 For example, in the above example file, "Pass_with_exception" and "Fatal_failed" are the names for their respective output.
 Names are also how we determine the result of a test case. 
 This is done by using skip followed by the name in the parameter.
 
 For example:
-        import pytest
-        from pytest import skip
-
-        def test_1():
-                skip("Pass_with_exception")
-
+```python
+import pytest
+from pytest import skip
+
+def test_1():
+    skip("Pass_with_exception")
+```
 
 In the example above, test_1 will result in "passed_with_exception".
 Because the name overrides the outcome, it will not result in a skip.
-We use the keyword skip as a means to obtaining out desired outcome.
+We use the keyword skip as a means to obtaining our desired outcome.
 
 If we put a name that is not in our custom output in the skip parameter,
-then
-        if we set unknown to True in the json, we will use the unknown outcome
-        else we will use the default skip and pass the name as a message (Standard skip behavior)
+then the following occurs:
+ - if we set unknown to True in the json, we will use the unknown outcome
+ - else we will use the default skip and pass the name as a message (Standard skip behavior)
+
 
+The rest of the information in the json file can be edited and customized to your liking.
 
-The rest of the information in the json file can be edited and customized to your liking. 
+
+Why pytest-custom_outputs?
+--------------------------
+
+- Improved Communication: Get more informative insights from your test runs
+- Focus on Key Areas: Prioritize test cases that require attention
+- Tailored for Your Needs: Adapt outcomes and messages to your project's specific requirements
 
 
 Contributing
 ------------
+
 Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
+
 License
 -------
 
 Distributed under the terms of the `BSD-3`_ license, "pytest-custom_outputs" is free and open source software
 
 
 Issues
 ------
 
 If you encounter any problems, please `file an issue`_ along with a detailed description.
 
-.. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
-.. _`@hackebrot`: https://github.com/hackebrot
-.. _`MIT`: https://opensource.org/licenses/MIT
-.. _`BSD-3`: https://opensource.org/licenses/BSD-3-Clause
-.. _`GNU GPL v3.0`: https://www.gnu.org/licenses/gpl-3.0.txt
-.. _`Apache Software License 2.0`: https://www.apache.org/licenses/LICENSE-2.0
-.. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 .. _`file an issue`: https://github.com/MichaelE55/pytest-custom_outputs/issues
-.. _`pytest`: https://github.com/pytest-dev/pytest
-.. _`tox`: https://tox.readthedocs.io/en/latest/
-.. _`pip`: https://pypi.org/project/pip/
-.. _`PyPI`: https://pypi.org/project
```

### Comparing `pytest_custom_outputs-0.1.0/pyproject.toml` & `pytest_custom_outputs-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-custom_outputs"
 description = "A plugin that allows users to create and use custom outputs instead of the standard Pass and Fail"
-version = "0.1.0"
+version = "0.1.1"
 readme = {file = "README.rst", content-type = "text/markdown"}
 requires-python = ">=3.8"
 authors = [
     { name = "Babak Michael Engheta", email = "michaelengheta55@gmail.com" },
 ]
 maintainers = [
     { name = "Babak Michael Engheta", email = "michaelengheta55@gmail.com" },
```

### Comparing `pytest_custom_outputs-0.1.0/src/pytest_custom_outputs/custom_outputs.py` & `pytest_custom_outputs-0.1.1/src/pytest_custom_outputs/custom_outputs.py`

 * *Files identical despite different names*

### Comparing `pytest_custom_outputs-0.1.0/src/pytest_custom_outputs.egg-info/PKG-INFO` & `pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-custom_outputs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A plugin that allows users to create and use custom outputs instead of the standard Pass and Fail
 Author-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 Maintainer-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 License: 
         Copyright (c) 2024, Babak Michael Engheta
         All rights reserved.
         
@@ -50,51 +50,56 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest>=6.2.0
 
-=====================
 pytest-custom_outputs
-=====================
+
+Overview
+--------
+
+Enhance Your Pytest Reporting with Customizable Test Outputs
+
+Tired of the standard pass/fail binary in pytest? With pytest-custom_outputs, you can create expressive and informative custom test results that go beyond the ordinary.  Tailor your reports to provide deeper insights into your test scenarios.
+
+Useful for if you want more than just the default Pass, Fail, and Skip outcomes.
+
 
 Features
 --------
 
-- Useful for if you want more than just the default Pass, Fail, and Skip outcomes.
-- Allows for the creation and usage of custom outputs.
-- Custom outputs are filled out in a file called "pytest_custom_outputs.json".
-- Custom outputs are customizable in their name, description, result code, tag, and color.
-- Supports the creation of an unknown output. If no result matches a default or custom output, then it will be categorized as an unknown output.
-- Unknown outputs are also fully customizable.
+- Flexible Output Types: Define new outcome types like "unimplemented", "soft_fail"," "inconclusive," or any custom label that suits your testing needs.
+- Fully Customizeable: Custom outputs are customizable in their name, description, result code, tag, and color.
+- Seamless Integration: Easily incorporate custom outputs into your existing pytest test suites.
+- Terminal and File Reporting: View your custom outputs in both your terminal output and pytest file reports.
 
 
 Requirements
 ------------
 
 None
 
 
 Installation
 ------------
 
-You can install "pytest-custom_outputs" via `pip`_ from `PyPI`_::
-
-    $ pip install pytest-custom_outputs
+pip install pytest-custom_outputs
 
 
 Usage
 -----
 
 In the directory where you will be running your pytest, create a file called "pytest_custom_outputs.json".
 You will use this file to create your own custom outputs.
+Feel free to copy and paste the below json file into yours and edit from there.
 
 EXAMPLE FILE:
-###STARTS HERE###
+```python
 {
         "use_unknown_if_no_match": true,
         "unknown": {
                 "attribute":"_unknown",
                 "status": {
                         "desc":"unknown",
                         "code":"?",
@@ -169,68 +174,74 @@
                                         "tag":"SKIPPED",
                                         "color":"yellow"
                                 }
                         }
                 }
         }
 }
-###ENDS HERE###
+```
+
+
+use_unknown_if_no_match
+ - If True, use the unknown output below if there is no match. Otherwise, use standard skip
 
+unknown
+ - The output to use if a test's result is not in default or custom outputs 
+
+custom_outputs
+ - A dictionary with all the custom outputs you write inside of it. You can edit, delete, and add new outputs here.
 
-use_unknown_if_no_match -> If True, use the unknown output below if there is no match. Otherwise, use standard skip
-unknown -> The output to use if a test's result is not in default or custom outputs 
-custom_outputs -> A dictionary with all the custom outputs you write inside of it. You can edit, delete, and add new outputs here.
 
 Each custom output is denoted by a name. The name is also the key for that output
 For example, in the above example file, "Pass_with_exception" and "Fatal_failed" are the names for their respective output.
 Names are also how we determine the result of a test case. 
 This is done by using skip followed by the name in the parameter.
 
 For example:
-        import pytest
-        from pytest import skip
-
-        def test_1():
-                skip("Pass_with_exception")
-
+```python
+import pytest
+from pytest import skip
+
+def test_1():
+    skip("Pass_with_exception")
+```
 
 In the example above, test_1 will result in "passed_with_exception".
 Because the name overrides the outcome, it will not result in a skip.
-We use the keyword skip as a means to obtaining out desired outcome.
+We use the keyword skip as a means to obtaining our desired outcome.
 
 If we put a name that is not in our custom output in the skip parameter,
-then
-        if we set unknown to True in the json, we will use the unknown outcome
-        else we will use the default skip and pass the name as a message (Standard skip behavior)
+then the following occurs:
+ - if we set unknown to True in the json, we will use the unknown outcome
+ - else we will use the default skip and pass the name as a message (Standard skip behavior)
+
 
+The rest of the information in the json file can be edited and customized to your liking.
 
-The rest of the information in the json file can be edited and customized to your liking. 
+
+Why pytest-custom_outputs?
+--------------------------
+
+- Improved Communication: Get more informative insights from your test runs
+- Focus on Key Areas: Prioritize test cases that require attention
+- Tailored for Your Needs: Adapt outcomes and messages to your project's specific requirements
 
 
 Contributing
 ------------
+
 Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
+
 License
 -------
 
 Distributed under the terms of the `BSD-3`_ license, "pytest-custom_outputs" is free and open source software
 
 
 Issues
 ------
 
 If you encounter any problems, please `file an issue`_ along with a detailed description.
 
-.. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
-.. _`@hackebrot`: https://github.com/hackebrot
-.. _`MIT`: https://opensource.org/licenses/MIT
-.. _`BSD-3`: https://opensource.org/licenses/BSD-3-Clause
-.. _`GNU GPL v3.0`: https://www.gnu.org/licenses/gpl-3.0.txt
-.. _`Apache Software License 2.0`: https://www.apache.org/licenses/LICENSE-2.0
-.. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 .. _`file an issue`: https://github.com/MichaelE55/pytest-custom_outputs/issues
-.. _`pytest`: https://github.com/pytest-dev/pytest
-.. _`tox`: https://tox.readthedocs.io/en/latest/
-.. _`pip`: https://pypi.org/project/pip/
-.. _`PyPI`: https://pypi.org/project
```

