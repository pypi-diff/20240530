# Comparing `tmp/provenaclient-0.1.0.tar.gz` & `tmp/provenaclient-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "provenaclient-0.1.0.tar", max compression
+gzip compressed data, was "provenaclient-0.2.0.tar", max compression
```

## Comparing `provenaclient-0.1.0.tar` & `provenaclient-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,31 @@
--rw-r--r--   0        0        0     1504 2024-04-05 05:09:54.124806 provenaclient-0.1.0/README.md
--rw-r--r--   0        0        0     1073 2024-04-05 05:09:54.128805 provenaclient-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      115 2024-04-05 05:09:54.128805 provenaclient-0.1.0/src/provenaclient/__init__.py
--rw-r--r--   0        0        0      228 2024-04-05 05:09:54.128805 provenaclient-0.1.0/src/provenaclient/main.py
--rw-r--r--   0        0        0      302 2024-04-05 05:09:54.128805 provenaclient-0.1.0/src/provenaclient/provena_client.py
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 provenaclient-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1867 2024-05-30 01:00:00.571279 provenaclient-0.2.0/README.md
+-rw-r--r--   0        0        0     1198 2024-05-30 01:00:00.575279 provenaclient-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      241 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/__init__.py
+-rw-r--r--   0        0        0      108 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/auth/__init__.py
+-rw-r--r--   0        0        0     2076 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/auth/helpers.py
+-rw-r--r--   0        0        0    19325 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/auth/implementations.py
+-rw-r--r--   0        0        0      784 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/auth/manager.py
+-rw-r--r--   0        0        0       32 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/clients/README.md
+-rw-r--r--   0        0        0      184 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/clients/__init__.py
+-rw-r--r--   0        0        0    12264 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/clients/auth_client.py
+-rw-r--r--   0        0        0     6887 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/clients/client_helpers.py
+-rw-r--r--   0        0        0     3721 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/clients/datastore_client.py
+-rw-r--r--   0        0        0     2094 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/clients/search_client.py
+-rw-r--r--   0        0        0     1380 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/clients/template_client.py
+-rw-r--r--   0        0        0       24 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/models/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/models/datastore.py
+-rw-r--r--   0        0        0       24 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/modules/README.md
+-rw-r--r--   0        0        0      145 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/modules/__init__.py
+-rw-r--r--   0        0        0     3055 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/modules/auth.py
+-rw-r--r--   0        0        0     4911 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/modules/datastore.py
+-rw-r--r--   0        0        0      349 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/modules/module_helpers.py
+-rw-r--r--   0        0        0     1291 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/modules/provena_client.py
+-rw-r--r--   0        0        0     1840 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/modules/search.py
+-rw-r--r--   0        0        0      963 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/modules/template_module.py
+-rw-r--r--   0        0        0       76 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/utils/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/utils/__init__.py
+-rw-r--r--   0        0        0     7350 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/utils/config.py
+-rw-r--r--   0        0        0     4509 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/utils/exceptions.py
+-rw-r--r--   0        0        0     8091 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/utils/helpers.py
+-rw-r--r--   0        0        0     3079 2024-05-30 01:00:00.575279 provenaclient-0.2.0/src/provenaclient/utils/http_client.py
+-rw-r--r--   0        0        0     2571 1970-01-01 00:00:00.000000 provenaclient-0.2.0/PKG-INFO
```

### Comparing `provenaclient-0.1.0/README.md` & `provenaclient-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,22 @@
 
 1) Run the Command: `curl -sSL https://install.python-poetry.org | python3 -`.
 2) Check if poetry was successfully installed by running `poetry --version`.
 3) You should now have be able to see your poetry version successfully. 
 4) Now run the command `poetry shell`. This  will activate the poetry virtual environment for you.
 5) Now finally run the command `poetry install`. This will install all dependencies defined within pyproject.toml.
 
+### Using local .venv
+
+1) Set poetry to use local `.venv` with `poetry config virtualenvs.in-project true`
+2) List and remove any existing venvs with `poetry env list` and `poetry env remove <name>`
+3) Install `poetry install`
+
+You can then make vs code use this environment easily with `ctrl + shift + p` select python interpreter choosing `.venv/bin/python`. 
+
 ### My Poetry Installation is not being detected?
 1) This means that your PATH variable does not include the Poetry directory. 
 2) Open your .bashrc file, using the command `nano ~/.bashrc`.
 3) Add the following line at the end of the file, `export PATH= "$HOME/.local/bin:$PATH"`.
 4) Reload your .bashrc file, using the command `source ~/.bashrc`.
 5) Verify that your poetry is now running, using the command `poetry --version`.
```

### Comparing `provenaclient-0.1.0/pyproject.toml` & `provenaclient-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 [tool.poetry]
 name = "provenaclient"
-version = "0.1.0"
+version = "0.2.0"
 description = "A client library for interfacing with a Provena instance."
 authors = ["RRAP <rrapisdev@gmail.com>"]
 license = "None"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
+httpx = "<0.27.0"
+pydantic = "<2.0"
+python-jose = "<3.3.0"
+provena-interfaces = "^2.6.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.9.0"
-pytest = "^8.1.1"
-python-semantic-release = "^9.4.0"
-pytest-cov = "^5.0.0"
+mypy = "<1.9.0"
+pytest = "<8.1.1"
+python-semantic-release = "<9.4.0"
+pytest-cov = "<5.0.0"
 myst-nb = "^1.0.0"
 sphinx-autoapi = "^3.0.0"
-sphinx-rtd-theme = "^2.0.0"
+sphinx-rtd-theme = "<2.0.0"
+types-requests = "^2.31.0.20240406"
 
 [tool.semantic_release]
 version_variable = [
     "src/provenaclient/__init__.py:__version__",
     "pyproject.toml:version"
 ]                                                   # version location
 branch = "main"                                      # branch to make releases of
```

### Comparing `provenaclient-0.1.0/PKG-INFO` & `provenaclient-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: provenaclient
-Version: 0.1.0
+Version: 0.2.0
 Summary: A client library for interfacing with a Provena instance.
 License: None
 Author: RRAP
 Author-email: rrapisdev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpx (<0.27.0)
+Requires-Dist: provena-interfaces (>=2.6.0,<3.0.0)
+Requires-Dist: pydantic (<2.0)
+Requires-Dist: python-jose (<3.3.0)
 Description-Content-Type: text/markdown
 
 # provenaclient
 
 A client library for interfacing with a Provena instance.
 
 ## Installation
@@ -30,14 +34,22 @@
 
 1) Run the Command: `curl -sSL https://install.python-poetry.org | python3 -`.
 2) Check if poetry was successfully installed by running `poetry --version`.
 3) You should now have be able to see your poetry version successfully. 
 4) Now run the command `poetry shell`. This  will activate the poetry virtual environment for you.
 5) Now finally run the command `poetry install`. This will install all dependencies defined within pyproject.toml.
 
+### Using local .venv
+
+1) Set poetry to use local `.venv` with `poetry config virtualenvs.in-project true`
+2) List and remove any existing venvs with `poetry env list` and `poetry env remove <name>`
+3) Install `poetry install`
+
+You can then make vs code use this environment easily with `ctrl + shift + p` select python interpreter choosing `.venv/bin/python`. 
+
 ### My Poetry Installation is not being detected?
 1) This means that your PATH variable does not include the Poetry directory. 
 2) Open your .bashrc file, using the command `nano ~/.bashrc`.
 3) Add the following line at the end of the file, `export PATH= "$HOME/.local/bin:$PATH"`.
 4) Reload your .bashrc file, using the command `source ~/.bashrc`.
 5) Verify that your poetry is now running, using the command `poetry --version`.
```

