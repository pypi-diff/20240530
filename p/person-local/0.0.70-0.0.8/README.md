# Comparing `tmp/person_local-0.0.70.tar.gz` & `tmp/person-local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "person_local-0.0.70.tar", last modified: Thu May 30 21:25:53 2024, max compression
+gzip compressed data, was "person-local-0.0.8.tar", last modified: Mon Aug 21 07:54:00 2023, max compression
```

## Comparing `person_local-0.0.70.tar` & `person-local-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:25:53.316617 person_local-0.0.70/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-30 21:25:53.316617 person_local-0.0.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-30 21:25:32.000000 person_local-0.0.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:25:53.312617 person_local-0.0.70/person_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:25:53.316617 person_local-0.0.70/person_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:25:32.000000 person_local-0.0.70/person_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-30 21:25:32.000000 person_local-0.0.70/person_local/src/person.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-30 21:25:32.000000 person_local-0.0.70/person_local/src/persons_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:25:53.316617 person_local-0.0.70/person_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-30 21:25:53.000000 person_local-0.0.70/person_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-30 21:25:53.000000 person_local-0.0.70/person_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:25:53.000000 person_local-0.0.70/person_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 21:25:53.000000 person_local-0.0.70/person_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 21:25:53.000000 person_local-0.0.70/person_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-30 21:25:38.000000 person_local-0.0.70/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:25:53.316617 person_local-0.0.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-30 21:25:32.000000 person_local-0.0.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:54:00.712449 person-local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-21 07:54:00.712449 person-local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-21 07:53:31.000000 person-local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:54:00.712449 person-local-0.0.8/person_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-21 07:54:00.000000 person-local-0.0.8/person_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-21 07:54:00.000000 person-local-0.0.8/person_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 07:54:00.000000 person-local-0.0.8/person_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-21 07:54:00.000000 person-local-0.0.8/person_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:54:00.712449 person-local-0.0.8/person_local_python_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 07:53:31.000000 person-local-0.0.8/person_local_python_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:54:00.712449 person-local-0.0.8/person_local_python_package/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 07:53:31.000000 person-local-0.0.8/person_local_python_package/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-21 07:53:31.000000 person-local-0.0.8/person_local_python_package/src/delete_person_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-21 07:53:31.000000 person-local-0.0.8/person_local_python_package/src/insert_person_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-08-21 07:53:31.000000 person-local-0.0.8/person_local_python_package/src/update_person_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-21 07:53:31.000000 person-local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 07:54:00.712449 person-local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-21 07:53:31.000000 person-local-0.0.8/setup.py
```

### Comparing `person_local-0.0.70/README.md` & `person-local-0.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,43 @@
 # python-package-template
-
 To create local package and remote package layers (not to create GraphQL and REST-API layers)
 
 # directory structure
-
-Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e.
-location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br>
+Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e. location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br> 
 /location_local<br>
 /location_local/get_country_name<br>
 /location_local/get_country_name/src<br>
 /location_local/get_country_name/src/get_country_name.py<br>
 /location_local/get_country_name/tests<br>
 /location_local/get_country_name/tests/test_get_country_name.py<br>
 
 # database Python scripts in /db folder
-
 Please place <table-name>.py in /db<br>
 No need for seperate file for _ml table<br>
 Please delete the example file if not needed<br>
-
+  
 # Create the files to create the database schema, tables, view and populate Meta Data and Test Date
-
 /db/<table-name>.py - CREATE SCHEMA ... CREATE TABLE ... CREATE VIEW ...<br>
 /db/<table-name>_insert.py to create records
 
 # Update the setup.py (i.e.name, version)
-
+ 
 # Please create test directory inside the directory of the project i.e. /<project-name>/tests
 
 # Update the serverless.yml in the root directory
-
 provider:
-stage: play1
-
+  stage: play1
+  
 Update the endpoints in serverless.yml
 
 # Working with VS Code
-
 Please make sure you push to the repo launch.json fie that enables to run and debug the code<br>
 
 # Unit-Test
-
 We prefer using pytest and not unittest package<br>
 
 Please create pytest.init in the project directory and not in the root directory
-
 ```
 [pytest]
 markers =
     test: custom mark for tests
 ```
```

### Comparing `person_local-0.0.70/pyproject.toml` & `person-local-0.0.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 
-name = "person-local"
+name = "person-local-python-package"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.71" # https://pypi.org/project/<project-name> i.e. https://pypi.org/project/storage-local/
+version = "0.0.1" # https://pypi.org/project/<project-name> i.e. https://pypi.org/project/storage-local/
 description = "person-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `person_local-0.0.70/setup.py` & `person-local-0.0.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 import setuptools
-
-PACKAGE_NAME = "person-local"
-package_dir = PACKAGE_NAME.replace("-", "_")
-
+# Each Python project should have pyproject.toml or setup.py
+# used by python -m build
+# ```python -m build``` needs pyproject.toml or setup.py
+# The need for setup.py is changing as of poetry 1.1.0 (including current pre-release) as we have moved away from needing to generate a setup.py file to enable editable installs - We might able to delete this file in the near future
 setuptools.setup(
-    name=PACKAGE_NAME,
-    version='0.0.70',  # https://pypi.org/project/person-local/
-    author="Circles",
-    author_email="info@circles.ai",
-    description="PyPI Package for Circles person Local Python",
-    long_description="This is a package for sharing common XXX function used in different repositories",
-    long_description_content_type="text/markdown",
-    url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
-    packages=[package_dir],
-    package_dir={package_dir: f'{package_dir}/src'},
-    package_data={package_dir: ['*.py']},
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: Other/Proprietary License",
-        "Operating System :: OS Independent",
-    ],
-    install_requires=[
-        "database-infrastructure-local>=0.0.24",
-        "database-mysql-local>=0.0.290",
-        "email-address-local>=0.0.40",
-        "language-remote>=0.0.20",
-        "logger-local>=0.0.135",
-        "user-context-remote>=0.0.75",
-        "people-local>=0.0.17"
-    ]
-)
+     name='person-local',  
+     version='0.0.8', # https://pypi.org/project/<project-name>/
+     author="Circles",
+     author_email="info@circles.life",
+     description="PyPI Package for Circles person Local Python", 
+     long_description="This is a package for sharing common XXX function used in different repositories",
+     long_description_content_type="text/markdown",
+     url="https://github.com/circles-zone/person-local-python-package",
+     packages=setuptools.find_packages(),
+     classifiers=[
+         "Programming Language :: Python :: 3",
+         "License :: Other/Proprietary License",
+         "Operating System :: OS Independent",
+     ],
+ )
```

