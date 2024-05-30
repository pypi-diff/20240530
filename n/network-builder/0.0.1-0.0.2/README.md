# Comparing `tmp/network_builder-0.0.1.tar.gz` & `tmp/network_builder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network_builder-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "network_builder-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `network_builder-0.0.1.tar` & `network_builder-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,7 @@
--rw-r--r--   0        0        0      842 2024-05-09 08:10:16.143702 network_builder-0.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      598 2024-05-09 08:10:16.143702 network_builder-0.0.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     3238 2024-05-09 08:10:16.143702 network_builder-0.0.1/.gitignore
--rw-r--r--   0        0        0     1083 2024-05-09 08:10:16.143702 network_builder-0.0.1/LICENSE
--rw-r--r--   0        0        0      971 2024-05-09 08:10:16.143702 network_builder-0.0.1/README.md
--rw-r--r--   0        0        0      295 2024-05-09 08:10:16.143702 network_builder-0.0.1/devices.json
--rw-r--r--   0        0        0      660 2024-05-09 08:10:16.143702 network_builder-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      169 2024-05-09 08:10:16.143702 network_builder-0.0.1/src/network_builder/__init__.py
--rw-r--r--   0        0        0      379 2024-05-09 08:10:16.143702 network_builder-0.0.1/src/network_builder/__main__.py
--rw-r--r--   0        0        0     4980 2024-05-09 08:10:16.143702 network_builder-0.0.1/src/network_builder/network_builder.py
--rw-r--r--   0        0        0      590 2024-05-09 08:10:16.143702 network_builder-0.0.1/tasks.json
--rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 network_builder-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-08 19:42:51.503140 network_builder-0.0.2/LICENSE
+-rw-r--r--   0        0        0      925 2024-05-08 19:42:51.503140 network_builder-0.0.2/README.md
+-rw-r--r--   0        0        0      544 2024-05-30 09:43:21.998207 network_builder-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      169 2024-05-08 20:01:58.008642 network_builder-0.0.2/src/network_builder/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-30 09:28:14.332399 network_builder-0.0.2/src/network_builder/__main__.py
+-rw-r--r--   0        0        0     6718 2024-05-30 09:27:54.409988 network_builder-0.0.2/src/network_builder/network_builder.py
+-rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 network_builder-0.0.2/PKG-INFO
```

### Comparing `network_builder-0.0.1/pyproject.toml` & `network_builder-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "Network_Builder"
-version = "0.0.1"
+name = "network_builder"
+version = "0.0.2"
 description = "Infrastructure as code network builder"
 authors = [
     { name = "Levy-Y", email = "21.hagymasi.levente.gyula@mechwart.com" }
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
@@ -15,14 +15,8 @@
 
 [project.urls]
 Homepage = "https://github.com/Levy-Y/Network-Builder/"
 Repository = "https://github.com/Levy-Y/Network-Builder/"
 
 [build-system]
 build-backend = "flit_core.buildapi"
-requires = ["flit_core >=3.2,<4"]
-
-[tool.flit.module]
-name = "network_builder"
-
-[tool.flit.sdist]
-include = ["src/network_builder/__init__.py"]
+requires = ["flit_core >=3.2,<4"]
```

### Comparing `network_builder-0.0.1/PKG-INFO` & `network_builder-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Network_Builder
-Version: 0.0.1
+Name: network_builder
+Version: 0.0.2
 Summary: Infrastructure as code network builder
 Author-email: Levy-Y <21.hagymasi.levente.gyula@mechwart.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: netmiko
 Project-URL: Homepage, https://github.com/Levy-Y/Network-Builder/
 Project-URL: Repository, https://github.com/Levy-Y/Network-Builder/
```

