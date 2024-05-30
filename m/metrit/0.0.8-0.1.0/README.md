# Comparing `tmp/metrit-0.0.8.tar.gz` & `tmp/metrit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrit-0.0.8.tar", last modified: Wed May 29 15:05:55 2024, max compression
+gzip compressed data, was "metrit-0.1.0.tar", last modified: Thu May 30 16:42:14 2024, max compression
```

## Comparing `metrit-0.0.8.tar` & `metrit-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.336684 metrit-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.332684 metrit-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.332684 metrit-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-29 15:05:49.000000 metrit-0.0.8/.github/workflows/push_to_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-29 15:05:49.000000 metrit-0.0.8/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-29 15:05:49.000000 metrit-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 15:05:49.000000 metrit-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-29 15:05:49.000000 metrit-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-05-29 15:05:55.336684 metrit-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 15:05:49.000000 metrit-0.0.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)    26374 2024-05-29 15:05:49.000000 metrit-0.0.8/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-29 15:05:49.000000 metrit-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.332684 metrit-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-29 15:05:49.000000 metrit-0.0.8/examples/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.336684 metrit-0.0.8/metrit/
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/Monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/StatCollector.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/Stats.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.336684 metrit-0.0.8/metrit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-05-29 15:05:55.000000 metrit-0.0.8/metrit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-29 15:05:55.000000 metrit-0.0.8/metrit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:05:55.000000 metrit-0.0.8/metrit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 15:05:55.000000 metrit-0.0.8/metrit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 15:05:55.000000 metrit-0.0.8/metrit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-29 15:05:49.000000 metrit-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:05:55.336684 metrit-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.336684 metrit-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/test_StatsCollector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/test_metrit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/test_metrit_deactivated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/test_metrit_with_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:14.195147 metrit-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:14.191147 metrit-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:14.191147 metrit-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-30 16:42:05.000000 metrit-0.1.0/.github/workflows/push_to_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-30 16:42:05.000000 metrit-0.1.0/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-30 16:42:05.000000 metrit-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-30 16:42:05.000000 metrit-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-30 16:42:05.000000 metrit-0.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12806 2024-05-30 16:42:14.195147 metrit-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 16:42:05.000000 metrit-0.1.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    26374 2024-05-30 16:42:05.000000 metrit-0.1.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-05-30 16:42:05.000000 metrit-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:14.191147 metrit-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-30 16:42:05.000000 metrit-0.1.0/examples/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:14.195147 metrit-0.1.0/metrit/
+-rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-05-30 16:42:05.000000 metrit-0.1.0/metrit/Monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-05-30 16:42:05.000000 metrit-0.1.0/metrit/StatCollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-30 16:42:05.000000 metrit-0.1.0/metrit/Stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 16:42:05.000000 metrit-0.1.0/metrit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-30 16:42:05.000000 metrit-0.1.0/metrit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-30 16:42:05.000000 metrit-0.1.0/metrit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:14.195147 metrit-0.1.0/metrit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12806 2024-05-30 16:42:14.000000 metrit-0.1.0/metrit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-30 16:42:14.000000 metrit-0.1.0/metrit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:42:14.000000 metrit-0.1.0/metrit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 16:42:14.000000 metrit-0.1.0/metrit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 16:42:14.000000 metrit-0.1.0/metrit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-30 16:42:05.000000 metrit-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:42:14.195147 metrit-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:14.195147 metrit-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:05.000000 metrit-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-30 16:42:05.000000 metrit-0.1.0/tests/test_StatsCollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-30 16:42:05.000000 metrit-0.1.0/tests/test_metrit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-30 16:42:05.000000 metrit-0.1.0/tests/test_metrit_deactivated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-30 16:42:05.000000 metrit-0.1.0/tests/test_metrit_with_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-30 16:42:05.000000 metrit-0.1.0/tests/test_utils.py
```

### Comparing `metrit-0.0.8/.github/workflows/push_to_main.yml` & `metrit-0.1.0/.github/workflows/push_to_main.yml`

 * *Files identical despite different names*

### Comparing `metrit-0.0.8/.github/workflows/pypi_release.yml` & `metrit-0.1.0/.github/workflows/pypi_release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,14 @@
         python-version: 3.x
 
     - name: Install pypa/build
       run: |
         python -m pip install --upgrade pip
         pip install build
 
-    #- name: Extract tag name
-    #  id: tag
-    #  run: echo "TAG_NAME=${{ github.ref_name }}" >> $GITHUB_ENV
-
-    #- name: Update version in setup.py
-    #  env:
-    #    TAG_NAME: ${{ env.TAG_NAME }}
-    #  run: sed -i "s/{{VERSION_PLACEHOLDER}}/${{ env.TAG_NAME }}/g" setup.py
-
     - name: Build a binary wheel
       run: python -m build
 
     - name: Store the distribution packages
       uses: actions/upload-artifact@v4
       with:
         name: python-package-distributions
```

### Comparing `metrit-0.0.8/LICENSE` & `metrit-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metrit-0.0.8/Makefile` & `metrit-0.1.0/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	VENV_ACTIVATE = . .venv/bin/activate &
 	PYTHON = python3
 	RM = rm -f
 	RMDIR = rm -rf
 
 endif
 
-.PHONY: install build example test check clean upload_pypi upload-testpypi
+.PHONY: install build example test clean upload_pypi upload-testpypi
 
 install:
 	$(info Installing the repo)
 ifeq ($(OS),Windows_NT)
 	@if not exist .venv mkdir .venv
 else
 	@mkdir -p .venv
@@ -42,29 +42,30 @@
 	$(RMDIR) build
 	$(RMDIR) dist
 	$(RMDIR) .eggs
 	$(RMDIR) metrit.egg-info
 endif
 
 build:
+# Use it only to check the version before uploading
 	$(VENV_ACTIVATE) $(PYTHON) -m build
 
-check:
-	$(VENV_ACTIVATE) $(PYTHON) setup.py check
-
 
 upload-pypi: clean install test build check
-# Don't use this method,
+# DEPRECATED
 # Instead use tags and the pypi_release.yml will upload the Github release and pypi
 # git tag 0.0.1 # or whatever version needed
 # git push origin --tags
+
 # Upload to PyPI. Make sure you have in your ~/.pypirc file in home directory
 	$(VENV_ACTIVATE) $(PYTHON) -m twine upload dist/*
 
 upload-testpypi: clean install test build check
+# DEPRECATED
+
 # Upload to TestPyPI. Make sure you have in your ~/.pypirc file in home directory
 # Use $(PYTHON) -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ tempit
 # for installing the testpypi version
 # or use pipenv install tempit -i https://test.pypi.org/simple
 	$(VENV_ACTIVATE) $(PYTHON) -m twine upload --repository testpypi dist/*
```

### Comparing `metrit-0.0.8/PKG-INFO` & `metrit-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrit
-Version: 0.0.8
+Version: 0.1.0
 Summary: A dead simple resources monitoring decorator
 Author-email: Mario Crespo <info@mariocrespo.es>
 License: MIT License
         
         Copyright (c) 2024 Mario Crespo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -137,86 +137,98 @@
 - Automatic recursion detection.
 
 ## Parameters
 
 Using the decorator `@metrit` without any parameters executes the function once and displays the resources. However, you can enhance the experience using the following arguments:
 
 - `find_children` (bool, optional): Specifies if the monitoring system should look for children processes as well. Defaults to False.
-- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to False.
+- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to True.
 - `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
 
 ## Best Practices
 
 The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
 
 - For more precise measurements, it is recommended to set `isolate` to `True`. Please see the [Isolate](#isolate) section to understand the limitations of this approach.
 
 - Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more.
 
 - Decorating classes will return the class unmodified and will not be decorated. For more information about this decision, see the [Why is class decoration bypassed](#why-is-class-decoration-bypassed) in the [Limitations](#limitations) section.
 
 ## Recursive Functions
 
-Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended [encapsulating the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` will not trigger the automatic recursion checker, making bad measurements, slowing time and making a too verbose output.
+Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended to [encapsulate the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` is still in beta and could lead to inaccurate measurements.
 
 ### Using the Auto-Recursion Feature
 
 The auto-recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the measures taken to run the appropriate function, plus a small overhead. It is not recommended to rely on this feature intentionally since the collected data might not be as accurate.
 
 This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
 
 ```python
 @metrit
 def recursive_func(n):
-    if n == 0:
-        return 0
-    else:
-        return n + recursive_func(n - 1)
+    if n < 2:
+        return n
+    return recursive_func(n - 2) + recursive_func(n - 1)
 
 
 # This will trigger the auto-recursion feature
 result = recursive_func(3)
 ```
 
+The result for this function could be something like:
+
+```text
+Function 'recursive_func'  50.86KB avg of memory    54.46% avg of CPU   4.22KB IO reads   5.63KB IO writes
+```
+
 ### Encapsulating the Recursive Function
 
 The recommended option is to encapsulate the recursive function within another function and then, decorate and call the parent function. Here's an example:
 
 ```python
 @metrit
 def encapsulated_recursive_function(n):
     """A non-verbose wrapper for the recursive function."""
     def recursive_func(n):
-        if n == 0:
-            return 0
-        else:
-            return n + recursive_func(n - 1)
+        if n < 2:
+            return n
+        return recursive_func(n - 2) + recursive_func(n - 1)
 
     return recursive_func(n)
 
 # Encapsulating the recursive function
 result = encapsulated_recursive_function(3)
 ```
 
-This approach enhances readability without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
+This approach enhances speed and measurement precision without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
+
+The result for this function could be something like:
+
+```text
+Function 'encapsulated_recursive_function'  40.00KB avg of memory     0.00% avg of CPU     238B IO reads   2.01KB IO writes
+```
+
+Both examples are valid for comparisons between similar circumstances, but the latter is preferred.
 
 ## Isolate
 
 The isolation feature works by encapsulating the decorated function in a separate process and then monitoring that process from another process to avoid interfering with the function's execution. If any part of this process fails, `metrit` will retry running the function in the original process.
 
 ## Limitations
 
 While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `metrit` decorator could lead to unexpected behavior.
 
 ### Isolate Limitations
 
 While the `isolate` feature is powerful and recommended for precise measurements, it can lead to unexpected results. Here are the main limitations:
 
-- Using it in a non-wrapped recursive function will generate a process for each recursive call, wasting resources, performing inaccurate measurements, and generating verbose output. Ensure you are not using it directly with a recursive function.
-- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
+- Using it in a non-wrapped recursive function will generate one process for the parent call and use multiprocess queues to pass the call stack. Isolating non-wrapped recursive functions is still in beta and could lead to inaccurate measurements and other possible issues. If any issues arise using this approach, feel free to open a GitHub issue.
+- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to several issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
 
 ### Why is Class Decoration Bypassed?
 
 When a class is decorated using `metrit`, it remains unmodified and is not decorated. If the user intends to measure the time of `__init__` or any other constructor, it can be done directly on those methods.
 
 This design decision was made due to a potential issue that arises when a decorated class is used in conjunction with spawning a new process. Specifically, if a class decorated with `metrit` is pickled for use in a separate process and then a method is called within that new process, it may result in a `PicklingError`.
 
@@ -236,15 +248,14 @@
 ### Errors
 
 If an error occurs while executing the decorated function in non-isolated mode or within a recursively decorated function, the error will be propagated to the user's function.
 
 ### Warnings
 
 - Deprecation warnings will be added before removing a feature.
-- If recursion is detected, a warning will be prompted. In such cases, refer to the [Recursive functions](#recursive-functions) section.
 
 ## Contributing
 
 Contributions are welcome! Please follow these guidelines when contributing:
 
 1. Fork the repository.
 2. Use `make install` to install all dependencies.
```

### Comparing `metrit-0.0.8/Pipfile.lock` & `metrit-0.1.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `metrit-0.0.8/README.md` & `metrit-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -98,86 +98,98 @@
 - Automatic recursion detection.
 
 ## Parameters
 
 Using the decorator `@metrit` without any parameters executes the function once and displays the resources. However, you can enhance the experience using the following arguments:
 
 - `find_children` (bool, optional): Specifies if the monitoring system should look for children processes as well. Defaults to False.
-- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to False.
+- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to True.
 - `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
 
 ## Best Practices
 
 The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
 
 - For more precise measurements, it is recommended to set `isolate` to `True`. Please see the [Isolate](#isolate) section to understand the limitations of this approach.
 
 - Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more.
 
 - Decorating classes will return the class unmodified and will not be decorated. For more information about this decision, see the [Why is class decoration bypassed](#why-is-class-decoration-bypassed) in the [Limitations](#limitations) section.
 
 ## Recursive Functions
 
-Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended [encapsulating the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` will not trigger the automatic recursion checker, making bad measurements, slowing time and making a too verbose output.
+Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended to [encapsulate the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` is still in beta and could lead to inaccurate measurements.
 
 ### Using the Auto-Recursion Feature
 
 The auto-recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the measures taken to run the appropriate function, plus a small overhead. It is not recommended to rely on this feature intentionally since the collected data might not be as accurate.
 
 This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
 
 ```python
 @metrit
 def recursive_func(n):
-    if n == 0:
-        return 0
-    else:
-        return n + recursive_func(n - 1)
+    if n < 2:
+        return n
+    return recursive_func(n - 2) + recursive_func(n - 1)
 
 
 # This will trigger the auto-recursion feature
 result = recursive_func(3)
 ```
 
+The result for this function could be something like:
+
+```text
+Function 'recursive_func'  50.86KB avg of memory    54.46% avg of CPU   4.22KB IO reads   5.63KB IO writes
+```
+
 ### Encapsulating the Recursive Function
 
 The recommended option is to encapsulate the recursive function within another function and then, decorate and call the parent function. Here's an example:
 
 ```python
 @metrit
 def encapsulated_recursive_function(n):
     """A non-verbose wrapper for the recursive function."""
     def recursive_func(n):
-        if n == 0:
-            return 0
-        else:
-            return n + recursive_func(n - 1)
+        if n < 2:
+            return n
+        return recursive_func(n - 2) + recursive_func(n - 1)
 
     return recursive_func(n)
 
 # Encapsulating the recursive function
 result = encapsulated_recursive_function(3)
 ```
 
-This approach enhances readability without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
+This approach enhances speed and measurement precision without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
+
+The result for this function could be something like:
+
+```text
+Function 'encapsulated_recursive_function'  40.00KB avg of memory     0.00% avg of CPU     238B IO reads   2.01KB IO writes
+```
+
+Both examples are valid for comparisons between similar circumstances, but the latter is preferred.
 
 ## Isolate
 
 The isolation feature works by encapsulating the decorated function in a separate process and then monitoring that process from another process to avoid interfering with the function's execution. If any part of this process fails, `metrit` will retry running the function in the original process.
 
 ## Limitations
 
 While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `metrit` decorator could lead to unexpected behavior.
 
 ### Isolate Limitations
 
 While the `isolate` feature is powerful and recommended for precise measurements, it can lead to unexpected results. Here are the main limitations:
 
-- Using it in a non-wrapped recursive function will generate a process for each recursive call, wasting resources, performing inaccurate measurements, and generating verbose output. Ensure you are not using it directly with a recursive function.
-- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
+- Using it in a non-wrapped recursive function will generate one process for the parent call and use multiprocess queues to pass the call stack. Isolating non-wrapped recursive functions is still in beta and could lead to inaccurate measurements and other possible issues. If any issues arise using this approach, feel free to open a GitHub issue.
+- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to several issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
 
 ### Why is Class Decoration Bypassed?
 
 When a class is decorated using `metrit`, it remains unmodified and is not decorated. If the user intends to measure the time of `__init__` or any other constructor, it can be done directly on those methods.
 
 This design decision was made due to a potential issue that arises when a decorated class is used in conjunction with spawning a new process. Specifically, if a class decorated with `metrit` is pickled for use in a separate process and then a method is called within that new process, it may result in a `PicklingError`.
 
@@ -197,15 +209,14 @@
 ### Errors
 
 If an error occurs while executing the decorated function in non-isolated mode or within a recursively decorated function, the error will be propagated to the user's function.
 
 ### Warnings
 
 - Deprecation warnings will be added before removing a feature.
-- If recursion is detected, a warning will be prompted. In such cases, refer to the [Recursive functions](#recursive-functions) section.
 
 ## Contributing
 
 Contributions are welcome! Please follow these guidelines when contributing:
 
 1. Fork the repository.
 2. Use `make install` to install all dependencies.
```

### Comparing `metrit-0.0.8/examples/examples.py` & `metrit-0.1.0/examples/examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # Simulate some work
     for _ in range(10):
         for _ in range(10_000_000):
             pass  #
     return a + b
 
 
-@metrit
+@metrit(isolate=True)
 def recursive_func(n):
     if n < 2:
         return n
     return recursive_func(n - 2) + recursive_func(n - 1)
 
 
 def fib(n):
@@ -88,16 +88,17 @@
 
     with open(file, "rb") as f:
         f.read()
     os.remove(file)
     return num_writes + data_size
 
 
-@metrit(verbose=True, find_children=True, isolate=True)
+# @metrit(verbose=True, find_children=True, isolate=True)
 def main():
+
     print("---CLASS EXAMPLES---")
     test_class_args = MeasureTestClassWithArgs(3, b=6)
     if test_class_args.sum != 9:
         print("test_class_args.sum != 9")
         exit()
 
     test_class = MeasureTestClass()
@@ -114,16 +115,17 @@
     class_name, result = test_class.class_method(3, b=4)
     if result != 7 or class_name != "MeasureTestClass":
         print("test_class.class_method() != ('MeasureTestClass', 7)")
         exit()
     print("---END CLASS EXAMPLES---\n")
 
     print("---RECURSIVE EXAMPLES---")
+
     wrapped_recursive_func(21)
-    recursive_func(12)
+    recursive_func(21)
 
     print("---END RECURSIVE EXAMPLES---\n")
 
     print("---OTHER EXAMPLES---")
 
     fill_ram(100, duration_in_seconds=2)  # 100MB
     cpu_intensive(3, b=4)
```

### Comparing `metrit-0.0.8/metrit/Monitoring.py` & `metrit-0.1.0/metrit/Monitoring.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 from sys import platform
 from typing import Dict, Self
 
-from multiprocess import Process, Queue, current_process
+from multiprocess import Process, Queue, current_process  # type: ignore
 
 from .StatCollector import StatCollector
 from .Stats import RawStats, Stats
 from .utils import format_size
 
 
 class Monitoring:
```

### Comparing `metrit-0.0.8/metrit/StatCollector.py` & `metrit-0.1.0/metrit/StatCollector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from statistics import mean
 from sys import platform
 from typing import Dict, Tuple
 
 import psutil
-from multiprocess import Queue, current_process
+from multiprocess import Queue, current_process  # type: ignore
 
 from .Stats import RawStats, Stats
 
 
 class StatCollector:
     def __init__(self, pid):
         """
```

### Comparing `metrit-0.0.8/metrit/Stats.py` & `metrit-0.1.0/metrit/Stats.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.8/metrit/core.py` & `metrit-0.1.0/metrit/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 import inspect
 from collections import deque
 from functools import partial, wraps
 from typing import Any, Callable, Dict, Tuple
 
+from multiprocess import Queue  # type: ignore
+
 from metrit.Monitoring import Monitoring
 from metrit.utils import check_is_recursive_func, extract_callable_and_args_if_method
 
 
 class MetritConfig:
     ACTIVE: bool = True
 
 
-def metrit(*args: Any, verbose: bool = False, find_children: bool = False, isolate: bool = False) -> Callable:
+called_isolated_func_queue = Queue()
+
+
+def metrit(*args: Any, verbose: bool = False, find_children: bool = False, isolate: bool = True) -> Callable:
     """
     Decorator function that measures the cpu, ram and io footprint of a given function in the current process. It can be called like @metrit or using arguments @metrit(...)
 
     Args:
         args: contains the function to be decorated if no arguments are provided when calling the decorator
         verbose (bool, optional): Whether to print detailed information after execution. Defaults to False.
-        isolate (bool, optional): If True, encapsulates the function in its own process. Defaults to False.
+        isolate (bool, optional): If True, tries to encapsulate the function in its own process. Defaults to True.
 
     Returns:
         Callable: The decorated function if arguments are provided, otherwise a partial function.
                     If the callable is a class it will be returned unmodified and will not be decorated.
                     If the MetritConfig ACTIVE flag is set to false, the callable will be returned without modification and will not be decorated.
 
     Raises:
         Exception: If the function crashes, it will raise the exception given by the user's function.
 
     Notes:
         - Processes spawned inside the decorated function won't be measured
         - This decorator also checks for recursion automatically even though is better to wrap the recursive function in another function and apply the @metrit decorator to the new function.
-        - Recursive functions shouldn't use the isolate argument since recursion cannot be measured.
         - Classes will be returned unmodified and will not be decorated.
-        - If the function is a methods won't be isolated.
+        - If the function is a method, it won't be isolated.
         - If isolate==True and it crashes in the process, it will be tried again in the main process.
 
 
 
     Example:
         @metrit(verbose=True)
         def my_function(arg1, arg2):
@@ -58,78 +62,87 @@
             return lambda f: f
     if args:  # If arguments are provided, return the decorated function
         return _decorator(*args)
     else:
         return partial(_decorator, verbose=verbose, find_children=find_children, isolate=isolate)
 
 
-def _decorator(func: Callable, verbose: bool = False, find_children: bool = False, isolate: bool = False) -> Callable:
+def _decorator(func: Callable, verbose: bool = False, find_children: bool = False, isolate: bool = True) -> Callable:
     """
     Decorator function that measures the memory and time of a given function.
     Args:
         func (Callable): The function to be decorated.
         verbose (bool, optional): If True, prints detailed information about the function execution. Defaults to False.
         find_children (bool, optional): If True, measures the memory and time of all child processes spawned by the function. Defaults to False.
-        isolate (bool, optional): If True, encapsulates the function in its own process. Defaults to False.
+        isolate (bool, optional): If True, encapsulates the function in its own process. Defaults to True.
 
     Returns:
         Callable: The decorated function.
     Raises:
         Exception: If the function crashes, it will raise the exception given by the user's function.
     """
     if inspect.isclass(func):
         # If a class is found, return the class inmediatly since it could raise an exception if triggered from other processes
         return func
 
-    potential_recursion_func_stack: deque[Callable] = deque()
+    called_func_stack: deque[Callable] = deque()
 
     @wraps(func)
     def metrit_wrapper(*args: Tuple, **kwargs: Dict) -> Any:
-        nonlocal potential_recursion_func_stack
-        is_recursive: bool = check_is_recursive_func(func, potential_recursion_func_stack)
+        nonlocal called_func_stack
+        global called_isolated_func_queue
+
+        is_recursive: bool = check_is_recursive_func(func, called_func_stack, called_isolated_func_queue)
 
         callable_func, args, args_to_print, is_method = extract_callable_and_args_if_method(func, *args)
         if is_recursive:
-            return handle_recursive_call(callable_func, potential_recursion_func_stack, *args, **kwargs)
+            return handle_recursive_call(callable_func, called_func_stack, called_isolated_func_queue, *args, **kwargs)
 
         crashed: bool = False
-        # Get the memory footprint before the function is called
         if isolate and not is_method:
             try:
                 result, pool_monitor_data = isolate_function(find_children, callable_func, *args, **kwargs)
             except Exception:
                 crashed = True
 
         if crashed or not isolate or is_method:
             result, pool_monitor_data = call_func(find_children, callable_func, *args, **kwargs)
 
-        potential_recursion_func_stack.pop()
-        if not potential_recursion_func_stack:
+        called_func_stack.pop()
+        if not called_isolated_func_queue.empty():
+            called_isolated_func_queue.get()  # Consume the queue
+
+        if not called_func_stack and called_isolated_func_queue.empty():
             pool_monitor_data.print(verbose, callable_func.__name__, args_to_print, kwargs)
 
         return result
 
     return metrit_wrapper
 
 
-def handle_recursive_call(func: Callable, potential_recursion_func_stack: deque, *args: Tuple, **kwargs: Dict) -> Any:
+def handle_recursive_call(
+    func: Callable, called_func_stack: deque, called_isolated_func_queue: Queue, *args: Tuple, **kwargs: Dict
+) -> Any:
     """
     Handle a recursive call by executing the given function with the provided arguments and keyword arguments.
 
     Parameters:
         func (Callable): The function to be executed.
-        potential_recursion_func_stack (deque): A stack of potential recursive functions.
+        called_func_stack (deque): A stack of potential recursive functions.
         *args: Variable length argument list.
         **kwargs: Arbitrary keyword arguments.
 
     Returns:
         Any: The result of executing the function.
     """
     result: Any = func(*args, **kwargs)
-    potential_recursion_func_stack.pop()
+
+    called_func_stack.pop()
+    if not called_isolated_func_queue.empty():
+        called_isolated_func_queue.get()  # Consume one element of the queue
     return result
 
 
 def call_func(find_children: bool, func: Callable, *args: Tuple, **kwargs: Dict) -> Tuple[Any, Monitoring]:
     """
     Calls the given function with the provided arguments and keyword arguments.
     Monitor the resources used by the function.
@@ -177,19 +190,20 @@
         **kwargs: Arbitrary keyword arguments.
     Returns:
         Tuple[Any, Monitoring]: A tuple containing the result of the function and the monitoring data.
     Raises:
         Exception: If an exception occurs during the execution of the function.
         This exception will be handled in the main process and try again the execution and measurement of the function in the main process.
     """
-    from multiprocess import Process, Queue
+    from multiprocess import Process  # type: ignore
 
     data_queue = Queue()
     result_queue = Queue()
     error_queue = Queue()
+
     try:
 
         func_process: Process = Process(
             target=call_func_isolated,
             args=(find_children, func, data_queue, result_queue, error_queue, args),
             kwargs=kwargs,
         )
@@ -210,15 +224,21 @@
         func_process.join()
         func_process.terminate()
         print("Error trying to isolate the process. Trying it again in main process:", e)
         raise e
 
 
 def call_func_isolated(
-    find_children: bool, func: Callable, data_queue, result_queue, error_queue, args: Tuple, **kwargs: Dict
+    find_children: bool,
+    func: Callable,
+    data_queue: Queue,
+    result_queue: Queue,
+    error_queue: Queue,
+    args: Tuple,
+    **kwargs: Dict,
 ):
     """
     Executes the given function in a separate process and monitors its resource usage.
 
     Args:
         find_children (bool): Whether to find child processes.
         func (Callable): The function to be executed.
@@ -232,23 +252,26 @@
         None
 
     Raises:
         Exception: If an exception occurs during the execution of the function.
             The exception is put into the error_queue.
 
     """
+    global called_isolated_func_queue
+    called_isolated_func_queue.put(func)
     pre_monitor_data = Monitoring(find_children=find_children)
     pre_monitor_data.take_snapshot()
     pool_monitor_data = Monitoring(find_children=find_children)
     pool_monitor_data.start_monitoring()
 
     try:
         result: Any = func(*args, **kwargs)
     except Exception as e:
         pool_monitor_data.stop_monitoring()
+        called_isolated_func_queue.get()
         error_queue.put(e)
         return
 
     pool_monitor_data.stop_monitoring()
     pool_monitor_data.calculate_delta(pre_monitor_data)
     data_queue.put(pool_monitor_data)
     result_queue.put(result)
```

### Comparing `metrit-0.0.8/metrit/utils.py` & `metrit-0.1.0/metrit/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections import deque
 from typing import Callable, Tuple
-from warnings import warn
+
+from multiprocess import Queue  # type: ignore
 
 
 def format_size(bytes_size: int | float) -> str:
     """
     Converts a size in bytes to a human-readable format.
     Parameters:
         bytes_size (int | float): The size in bytes to be converted.
@@ -41,27 +42,40 @@
             args = (args[0].__class__,) + args[1:]  # type: ignore
             callable_func = func.__func__
         elif isinstance(func, staticmethod):
             args = args[1:]
     return callable_func, args, args_to_print, is_method
 
 
-def check_is_recursive_func(func: Callable, potential_recursion_func_stack: deque[Callable]) -> bool:
+def check_is_recursive_func(
+    func: Callable, called_func_stack: deque[Callable], called_isolated_func_queue: Queue
+) -> bool:
     """
     Checks if the function is being called recursively by checking the stack of called functions.
     It will send a warning if the function is being called recursively.
     Args:
         func (Callable): The function to check for recursion.
-        potential_recursion_func_stack (deque[Callable]): A stack of potential recursive functions.
+        called_func_stack (deque[Callable]): A stack of potential recursive functions.
     Returns:
         bool: True if the function is being called recursively, False otherwise.
 
     """
+    is_recursive = False
+    if not called_isolated_func_queue.empty():
+
+        prev_func = called_isolated_func_queue.get()
+        called_isolated_func_queue.put(prev_func)
+        if (
+            (prev_func.__name__ == func.__name__)
+            and (prev_func.__module__ == func.__module__)  # noqa: W503
+            and (prev_func.__code__.co_code == func.__code__.co_code)  # noqa: W503
+        ):
+            is_recursive = True
+
+    if called_func_stack and called_func_stack[-1] == func:
+        if is_recursive:
+            # This means that it is recursive and it has been called from another process (isolate) so we need to append the same function again
+            called_func_stack.append(func)
+        is_recursive = True
 
-    if potential_recursion_func_stack and potential_recursion_func_stack[-1] == func:
-        potential_recursion_func_stack.append(func)
-        # Check if the function is being called recursively by checking the object identity. This is way faster than using getFrameInfo
-        warning_msg = "Recursive function detected. This process may be slow. Consider wrapping the recursive function in another function and applying the @metrit decorator to the new function."
-        warn(warning_msg, stacklevel=3)
-        return True
-    potential_recursion_func_stack.append(func)
-    return False
+    called_func_stack.append(func)
+    return is_recursive
```

### Comparing `metrit-0.0.8/metrit.egg-info/PKG-INFO` & `metrit-0.1.0/metrit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrit
-Version: 0.0.8
+Version: 0.1.0
 Summary: A dead simple resources monitoring decorator
 Author-email: Mario Crespo <info@mariocrespo.es>
 License: MIT License
         
         Copyright (c) 2024 Mario Crespo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -137,86 +137,98 @@
 - Automatic recursion detection.
 
 ## Parameters
 
 Using the decorator `@metrit` without any parameters executes the function once and displays the resources. However, you can enhance the experience using the following arguments:
 
 - `find_children` (bool, optional): Specifies if the monitoring system should look for children processes as well. Defaults to False.
-- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to False.
+- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to True.
 - `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
 
 ## Best Practices
 
 The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
 
 - For more precise measurements, it is recommended to set `isolate` to `True`. Please see the [Isolate](#isolate) section to understand the limitations of this approach.
 
 - Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more.
 
 - Decorating classes will return the class unmodified and will not be decorated. For more information about this decision, see the [Why is class decoration bypassed](#why-is-class-decoration-bypassed) in the [Limitations](#limitations) section.
 
 ## Recursive Functions
 
-Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended [encapsulating the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` will not trigger the automatic recursion checker, making bad measurements, slowing time and making a too verbose output.
+Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended to [encapsulate the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` is still in beta and could lead to inaccurate measurements.
 
 ### Using the Auto-Recursion Feature
 
 The auto-recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the measures taken to run the appropriate function, plus a small overhead. It is not recommended to rely on this feature intentionally since the collected data might not be as accurate.
 
 This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
 
 ```python
 @metrit
 def recursive_func(n):
-    if n == 0:
-        return 0
-    else:
-        return n + recursive_func(n - 1)
+    if n < 2:
+        return n
+    return recursive_func(n - 2) + recursive_func(n - 1)
 
 
 # This will trigger the auto-recursion feature
 result = recursive_func(3)
 ```
 
+The result for this function could be something like:
+
+```text
+Function 'recursive_func'  50.86KB avg of memory    54.46% avg of CPU   4.22KB IO reads   5.63KB IO writes
+```
+
 ### Encapsulating the Recursive Function
 
 The recommended option is to encapsulate the recursive function within another function and then, decorate and call the parent function. Here's an example:
 
 ```python
 @metrit
 def encapsulated_recursive_function(n):
     """A non-verbose wrapper for the recursive function."""
     def recursive_func(n):
-        if n == 0:
-            return 0
-        else:
-            return n + recursive_func(n - 1)
+        if n < 2:
+            return n
+        return recursive_func(n - 2) + recursive_func(n - 1)
 
     return recursive_func(n)
 
 # Encapsulating the recursive function
 result = encapsulated_recursive_function(3)
 ```
 
-This approach enhances readability without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
+This approach enhances speed and measurement precision without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
+
+The result for this function could be something like:
+
+```text
+Function 'encapsulated_recursive_function'  40.00KB avg of memory     0.00% avg of CPU     238B IO reads   2.01KB IO writes
+```
+
+Both examples are valid for comparisons between similar circumstances, but the latter is preferred.
 
 ## Isolate
 
 The isolation feature works by encapsulating the decorated function in a separate process and then monitoring that process from another process to avoid interfering with the function's execution. If any part of this process fails, `metrit` will retry running the function in the original process.
 
 ## Limitations
 
 While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `metrit` decorator could lead to unexpected behavior.
 
 ### Isolate Limitations
 
 While the `isolate` feature is powerful and recommended for precise measurements, it can lead to unexpected results. Here are the main limitations:
 
-- Using it in a non-wrapped recursive function will generate a process for each recursive call, wasting resources, performing inaccurate measurements, and generating verbose output. Ensure you are not using it directly with a recursive function.
-- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
+- Using it in a non-wrapped recursive function will generate one process for the parent call and use multiprocess queues to pass the call stack. Isolating non-wrapped recursive functions is still in beta and could lead to inaccurate measurements and other possible issues. If any issues arise using this approach, feel free to open a GitHub issue.
+- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to several issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
 
 ### Why is Class Decoration Bypassed?
 
 When a class is decorated using `metrit`, it remains unmodified and is not decorated. If the user intends to measure the time of `__init__` or any other constructor, it can be done directly on those methods.
 
 This design decision was made due to a potential issue that arises when a decorated class is used in conjunction with spawning a new process. Specifically, if a class decorated with `metrit` is pickled for use in a separate process and then a method is called within that new process, it may result in a `PicklingError`.
 
@@ -236,15 +248,14 @@
 ### Errors
 
 If an error occurs while executing the decorated function in non-isolated mode or within a recursively decorated function, the error will be propagated to the user's function.
 
 ### Warnings
 
 - Deprecation warnings will be added before removing a feature.
-- If recursion is detected, a warning will be prompted. In such cases, refer to the [Recursive functions](#recursive-functions) section.
 
 ## Contributing
 
 Contributions are welcome! Please follow these guidelines when contributing:
 
 1. Fork the repository.
 2. Use `make install` to install all dependencies.
```

### Comparing `metrit-0.0.8/metrit.egg-info/SOURCES.txt` & `metrit-0.1.0/metrit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metrit-0.0.8/pyproject.toml` & `metrit-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -20,13 +20,10 @@
         "Intended Audience :: Developers",
     ]
 
 [project.urls]
 Repository = "https://github.com/mcrespoae/metrit"
 
 
-#[tool.setuptools.dynamic]
-#version = {attr = "metrit.__version__"}
-
 [tool.setuptools_scm]
 version_scheme = "guess-next-dev"
 local_scheme = "no-local-version"
```

### Comparing `metrit-0.0.8/tests/test_StatsCollector.py` & `metrit-0.1.0/tests/test_StatsCollector.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.8/tests/test_metrit.py` & `metrit-0.1.0/tests/test_metrit.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.8/tests/test_metrit_deactivated.py` & `metrit-0.1.0/tests/test_metrit_deactivated.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.8/tests/test_metrit_with_args.py` & `metrit-0.1.0/tests/test_metrit_with_args.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,71 +6,71 @@
 
 IN_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
 MetritConfig.ACTIVE = True
 
 
 @metrit(verbose=True)
 class MetritTestClassWithArgs:
-    @metrit(verbose=True, find_children=True, isolate=True)
+    @metrit(verbose=True, find_children=True, isolate=False)
     def __init__(self, a: int = 1, b: int = 2):
         self.sum = a + b
 
 
-@metrit(verbose=True, find_children=True, isolate=True)
+@metrit(verbose=True, find_children=True, isolate=False)
 class MetritTestClass:
-    @metrit(verbose=True, find_children=True, isolate=True)
+    @metrit(verbose=True, find_children=True, isolate=False)
     def metrit_basic(self, a: int = 1, b: int = 2):
         return a + b
 
-    @metrit(verbose=True, find_children=True, isolate=True)
+    @metrit(verbose=True, find_children=True, isolate=False)
     @staticmethod
     def static_method(a: int = 1, b: int = 2):
         return a + b
 
-    @metrit(verbose=True, find_children=True, isolate=True)
+    @metrit(verbose=True, find_children=True, isolate=False)
     @classmethod
     def class_method(cls, a: int = 1, b: int = 2):
         return cls.__name__, a + b
 
 
-@metrit(verbose=True, find_children=True, isolate=True)
+@metrit(verbose=True, find_children=True, isolate=False)
 def fill_ram(size_in_mb, duration_in_seconds):
     size_in_bytes = int(size_in_mb * 1024 * 1024)
     _ = bytearray(size_in_bytes)
     sleep(duration_in_seconds)
     return 1 + 2
 
 
-@metrit(verbose=True, find_children=True, isolate=True)
+@metrit(verbose=True, find_children=True, isolate=False)
 def cpu_intensive(a: int = 1, b: int = 2) -> int:
     for _ in range(2):
         for _ in range(1_000):
             pass  # Simulate some work
     return a + b
 
 
-@metrit(verbose=True, find_children=True, isolate=True)
+@metrit(verbose=True, find_children=True, isolate=False)
 def recursive_func(n):
     if n < 2:
         return n
     return recursive_func(n - 2) + recursive_func(n - 1)
 
 
 def fib(n):
     if n < 2:
         return n
     return fib(n - 2) + fib(n - 1)
 
 
-@metrit(verbose=True, find_children=True, isolate=True)
+@metrit(verbose=True, find_children=True, isolate=False)
 def wrapped_recursive_func(n):
     return fib(n)
 
 
-@metrit(verbose=True, find_children=True, isolate=True)
+@metrit(verbose=True, find_children=True, isolate=False)
 def simulate_writes_and_reads(num_writes=5_000, data_size=1024):
     file = ".temp_file"
     with open(file, "wb") as f:
         for _ in range(num_writes):
             f.write(b"a" * data_size)
             f.flush()
```

### Comparing `metrit-0.0.8/tests/test_utils.py` & `metrit-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

