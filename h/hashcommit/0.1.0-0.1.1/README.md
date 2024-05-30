# Comparing `tmp/hashcommit-0.1.0.tar.gz` & `tmp/hashcommit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashcommit-0.1.0.tar", last modified: Thu May 23 17:02:30 2024, max compression
+gzip compressed data, was "hashcommit-0.1.1.tar", last modified: Thu May 30 16:28:37 2024, max compression
```

## Comparing `hashcommit-0.1.0.tar` & `hashcommit-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:02:30.284669 hashcommit-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 17:02:22.000000 hashcommit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-23 17:02:30.284669 hashcommit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-23 17:02:22.000000 hashcommit-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:02:30.280669 hashcommit-0.1.0/hashcommit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:02:22.000000 hashcommit-0.1.0/hashcommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-23 17:02:22.000000 hashcommit-0.1.0/hashcommit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:02:30.280669 hashcommit-0.1.0/hashcommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-23 17:02:30.000000 hashcommit-0.1.0/hashcommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-23 17:02:30.000000 hashcommit-0.1.0/hashcommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:02:30.000000 hashcommit-0.1.0/hashcommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 17:02:30.000000 hashcommit-0.1.0/hashcommit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 17:02:30.000000 hashcommit-0.1.0/hashcommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:02:30.284669 hashcommit-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-23 17:02:22.000000 hashcommit-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:37.305824 hashcommit-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 16:28:29.000000 hashcommit-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-30 16:28:37.305824 hashcommit-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-30 16:28:29.000000 hashcommit-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:37.301824 hashcommit-0.1.1/hashcommit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:37.305824 hashcommit-0.1.1/hashcommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-30 16:28:37.000000 hashcommit-0.1.1/hashcommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 16:28:37.000000 hashcommit-0.1.1/hashcommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:28:37.000000 hashcommit-0.1.1/hashcommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 16:28:37.000000 hashcommit-0.1.1/hashcommit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 16:28:37.000000 hashcommit-0.1.1/hashcommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:28:37.305824 hashcommit-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-30 16:28:29.000000 hashcommit-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:37.305824 hashcommit-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-30 16:28:29.000000 hashcommit-0.1.1/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-30 16:28:29.000000 hashcommit-0.1.1/tests/test_empty_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-30 16:28:29.000000 hashcommit-0.1.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-30 16:28:29.000000 hashcommit-0.1.1/tests/test_existing_repo.py
```

### Comparing `hashcommit-0.1.0/LICENSE` & `hashcommit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.0/PKG-INFO` & `hashcommit-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,116 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hashcommit
 
-A tool to generate a Git commit with a specific hash prefix.
+A tool to generate a Git commit with a specific hash part.
 
 ## Installation
 
 You can install the package using pip:
 
 ```sh
 pip install hashcommit
 ```
 
 ## Usage
 
-By default, `hashcommit` will use the files that are staged (added using `git add`) to create a commit with a specific hash prefix. If no files are staged, it will create an empty commit.
+### Creating a New Commit
 
-To create a new commit with a specific hash prefix:
+To create a new commit with a specific hash part:
 
 ```sh
 hashcommit --hash <desired_hash_part> --message "<commit_message>"
 ```
 
-To overwrite the current commit with a specific hash prefix:
+### Overwriting the Last Commit
+
+To overwrite the last commit with a specific hash part:
 
 ```sh
 hashcommit --hash <desired_hash_part> --message "<commit_message>" --overwrite
 ```
 
+### Match Type
+
 You can also specify if the hash must begin with, contain, or end with the desired string using the `--match-type` option. The default is to match the beginning of the hash:
 
 ```sh
 hashcommit --hash <desired_hash_part> --message "<commit_message>" --match-type <begin|contain|end>
 ```
 
+### Example Usage
+
+To find and use a specific commit hash:
+
+```sh
+hashcommit --hash fff --match-type contain --message "foobar" ; git log -1 | cat
+```
+
+Example output:
+
+```
+Found matching commit hash: 93fffe4756192c250a7234c7c5fd81752c747091
+commit 93fffe4756192c250a7234c7c5fd81752c747091
+Author: Your Name <your-email@domain.com>
+Date:   Thu May 23 17:06:24 2024 +0000
+
+    foobar
+```
+
+### Author Preservation
+
+By default, the author is not preserved and gets overwritten when overwriting a commit. This feature will be implemented in the future.
+
+### Overwriting Commits in the Past
+
+Overwriting a particular commit in the past will be implemented in the future.
+
 ## Development
 
 To develop or contribute to this project, clone the repository and install the dependencies:
 
 ```sh
 git clone https://github.com/wozniakpl/hashcommit.git
 cd hashcommit
 pip install -e .
 ```
 
+### Running Locally
+
+You can run tests locally using tox or act:
+
+```sh
+# Using tox
+tox
+
+# Using act
+act
+```
+
+You can use the following command for simplicity of development. It formats the code, runs the checks, and the tests on one Python version:
+
+```sh
+tox -e format && tox -e checks && tox -e py311 --
+```
+
+To set up an environment with `hashcommit` installed and a git repository initialized in the `/repo` directory, use Docker Compose:
+
+```sh
+docker compose run --rm tests bash
+```
+
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `hashcommit-0.1.0/README.md` & `hashcommit-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,102 @@
 # hashcommit
 
-A tool to generate a Git commit with a specific hash prefix.
+A tool to generate a Git commit with a specific hash part.
 
 ## Installation
 
 You can install the package using pip:
 
 ```sh
 pip install hashcommit
 ```
 
 ## Usage
 
-By default, `hashcommit` will use the files that are staged (added using `git add`) to create a commit with a specific hash prefix. If no files are staged, it will create an empty commit.
+### Creating a New Commit
 
-To create a new commit with a specific hash prefix:
+To create a new commit with a specific hash part:
 
 ```sh
 hashcommit --hash <desired_hash_part> --message "<commit_message>"
 ```
 
-To overwrite the current commit with a specific hash prefix:
+### Overwriting the Last Commit
+
+To overwrite the last commit with a specific hash part:
 
 ```sh
 hashcommit --hash <desired_hash_part> --message "<commit_message>" --overwrite
 ```
 
+### Match Type
+
 You can also specify if the hash must begin with, contain, or end with the desired string using the `--match-type` option. The default is to match the beginning of the hash:
 
 ```sh
 hashcommit --hash <desired_hash_part> --message "<commit_message>" --match-type <begin|contain|end>
 ```
 
+### Example Usage
+
+To find and use a specific commit hash:
+
+```sh
+hashcommit --hash fff --match-type contain --message "foobar" ; git log -1 | cat
+```
+
+Example output:
+
+```
+Found matching commit hash: 93fffe4756192c250a7234c7c5fd81752c747091
+commit 93fffe4756192c250a7234c7c5fd81752c747091
+Author: Your Name <your-email@domain.com>
+Date:   Thu May 23 17:06:24 2024 +0000
+
+    foobar
+```
+
+### Author Preservation
+
+By default, the author is not preserved and gets overwritten when overwriting a commit. This feature will be implemented in the future.
+
+### Overwriting Commits in the Past
+
+Overwriting a particular commit in the past will be implemented in the future.
+
 ## Development
 
 To develop or contribute to this project, clone the repository and install the dependencies:
 
 ```sh
 git clone https://github.com/wozniakpl/hashcommit.git
 cd hashcommit
 pip install -e .
 ```
 
+### Running Locally
+
+You can run tests locally using tox or act:
+
+```sh
+# Using tox
+tox
+
+# Using act
+act
+```
+
+You can use the following command for simplicity of development. It formats the code, runs the checks, and the tests on one Python version:
+
+```sh
+tox -e format && tox -e checks && tox -e py311 --
+```
+
+To set up an environment with `hashcommit` installed and a git repository initialized in the `/repo` directory, use Docker Compose:
+
+```sh
+docker compose run --rm tests bash
+```
+
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `hashcommit-0.1.0/hashcommit.egg-info/PKG-INFO` & `hashcommit-0.1.1/hashcommit.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,116 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hashcommit
 
-A tool to generate a Git commit with a specific hash prefix.
+A tool to generate a Git commit with a specific hash part.
 
 ## Installation
 
 You can install the package using pip:
 
 ```sh
 pip install hashcommit
 ```
 
 ## Usage
 
-By default, `hashcommit` will use the files that are staged (added using `git add`) to create a commit with a specific hash prefix. If no files are staged, it will create an empty commit.
+### Creating a New Commit
 
-To create a new commit with a specific hash prefix:
+To create a new commit with a specific hash part:
 
 ```sh
 hashcommit --hash <desired_hash_part> --message "<commit_message>"
 ```
 
-To overwrite the current commit with a specific hash prefix:
+### Overwriting the Last Commit
+
+To overwrite the last commit with a specific hash part:
 
 ```sh
 hashcommit --hash <desired_hash_part> --message "<commit_message>" --overwrite
 ```
 
+### Match Type
+
 You can also specify if the hash must begin with, contain, or end with the desired string using the `--match-type` option. The default is to match the beginning of the hash:
 
 ```sh
 hashcommit --hash <desired_hash_part> --message "<commit_message>" --match-type <begin|contain|end>
 ```
 
+### Example Usage
+
+To find and use a specific commit hash:
+
+```sh
+hashcommit --hash fff --match-type contain --message "foobar" ; git log -1 | cat
+```
+
+Example output:
+
+```
+Found matching commit hash: 93fffe4756192c250a7234c7c5fd81752c747091
+commit 93fffe4756192c250a7234c7c5fd81752c747091
+Author: Your Name <your-email@domain.com>
+Date:   Thu May 23 17:06:24 2024 +0000
+
+    foobar
+```
+
+### Author Preservation
+
+By default, the author is not preserved and gets overwritten when overwriting a commit. This feature will be implemented in the future.
+
+### Overwriting Commits in the Past
+
+Overwriting a particular commit in the past will be implemented in the future.
+
 ## Development
 
 To develop or contribute to this project, clone the repository and install the dependencies:
 
 ```sh
 git clone https://github.com/wozniakpl/hashcommit.git
 cd hashcommit
 pip install -e .
 ```
 
+### Running Locally
+
+You can run tests locally using tox or act:
+
+```sh
+# Using tox
+tox
+
+# Using act
+act
+```
+
+You can use the following command for simplicity of development. It formats the code, runs the checks, and the tests on one Python version:
+
+```sh
+tox -e format && tox -e checks && tox -e py311 --
+```
+
+To set up an environment with `hashcommit` installed and a git repository initialized in the `/repo` directory, use Docker Compose:
+
+```sh
+docker compose run --rm tests bash
+```
+
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `hashcommit-0.1.0/setup.py` & `hashcommit-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from setuptools import setup, find_packages
-
-with open('VERSION') as version_file:
-    version = version_file.read().strip()
+from hashcommit.version import VERSION
 
 setup(
     name='hashcommit',
-    version=version,
+    version=VERSION,
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'hashcommit = hashcommit.main:main',
         ],
     },
     install_requires=[],
```

