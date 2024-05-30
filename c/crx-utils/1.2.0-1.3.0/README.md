# Comparing `tmp/crx_utils-1.2.0.tar.gz` & `tmp/crx_utils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crx_utils-1.2.0.tar", last modified: Sun May 26 12:51:13 2024, max compression
+gzip compressed data, was "crx_utils-1.3.0.tar", last modified: Thu May 30 12:59:33 2024, max compression
```

## Comparing `crx_utils-1.2.0.tar` & `crx_utils-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 12:51:13.203529 crx_utils-1.2.0/
--rw-rw-rw-   0        0        0       85 2024-05-26 10:32:30.000000 crx_utils-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      419 2024-05-26 12:51:13.202527 crx_utils-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-26 12:51:13.195527 crx_utils-1.2.0/crx/
--rw-rw-rw-   0        0        0      767 2024-05-26 12:50:07.000000 crx_utils-1.2.0/crx/Cogs.py
--rw-rw-rw-   0        0        0     1356 2024-05-26 00:54:31.000000 crx_utils-1.2.0/crx/Embed.py
--rw-rw-rw-   0        0        0     1154 2024-05-26 00:55:36.000000 crx_utils-1.2.0/crx/Loguru.py
--rw-rw-rw-   0        0        0     1507 2024-05-26 09:43:03.000000 crx_utils-1.2.0/crx/Reader.py
--rw-rw-rw-   0        0        0      754 2024-05-26 00:55:46.000000 crx_utils-1.2.0/crx/Tortoise.py
--rw-rw-rw-   0        0        0      238 2024-05-26 00:55:12.000000 crx_utils-1.2.0/crx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 12:51:13.201528 crx_utils-1.2.0/crx_utils.egg-info/
--rw-rw-rw-   0        0        0      419 2024-05-26 12:51:13.000000 crx_utils-1.2.0/crx_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-05-26 12:51:13.000000 crx_utils-1.2.0/crx_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 12:51:13.000000 crx_utils-1.2.0/crx_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2024-05-26 12:51:13.000000 crx_utils-1.2.0/crx_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-26 12:51:13.000000 crx_utils-1.2.0/crx_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      109 2024-05-26 10:36:41.000000 crx_utils-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-26 12:51:13.203529 crx_utils-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      568 2024-05-26 12:50:30.000000 crx_utils-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:33.924108 crx_utils-1.3.0/
+-rw-rw-rw-   0        0        0       85 2024-05-26 10:32:30.000000 crx_utils-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      496 2024-05-30 12:59:33.923108 crx_utils-1.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:33.910107 crx_utils-1.3.0/crx/
+-rw-rw-rw-   0        0        0      767 2024-05-26 12:50:07.000000 crx_utils-1.3.0/crx/Cogs.py
+-rw-rw-rw-   0        0        0     1356 2024-05-26 00:54:31.000000 crx_utils-1.3.0/crx/Embed.py
+-rw-rw-rw-   0        0        0     1154 2024-05-26 00:55:36.000000 crx_utils-1.3.0/crx/Loguru.py
+-rw-rw-rw-   0        0        0     1507 2024-05-26 09:43:03.000000 crx_utils-1.3.0/crx/Reader.py
+-rw-rw-rw-   0        0        0      119 2024-05-30 12:53:58.000000 crx_utils-1.3.0/crx/Restart.py
+-rw-rw-rw-   0        0        0      754 2024-05-26 00:55:46.000000 crx_utils-1.3.0/crx/Tortoise.py
+-rw-rw-rw-   0        0        0      266 2024-05-30 12:54:12.000000 crx_utils-1.3.0/crx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:33.923108 crx_utils-1.3.0/crx_utils.egg-info/
+-rw-rw-rw-   0        0        0      496 2024-05-30 12:59:33.000000 crx_utils-1.3.0/crx_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-05-30 12:59:33.000000 crx_utils-1.3.0/crx_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:59:33.000000 crx_utils-1.3.0/crx_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-05-30 12:59:33.000000 crx_utils-1.3.0/crx_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-30 12:59:33.000000 crx_utils-1.3.0/crx_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      109 2024-05-26 10:36:41.000000 crx_utils-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:59:33.924108 crx_utils-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      667 2024-05-30 12:56:40.000000 crx_utils-1.3.0/setup.py
```

### Comparing `crx_utils-1.2.0/crx/Cogs.py` & `crx_utils-1.3.0/crx/Cogs.py`

 * *Files identical despite different names*

### Comparing `crx_utils-1.2.0/crx/Embed.py` & `crx_utils-1.3.0/crx/Embed.py`

 * *Files identical despite different names*

### Comparing `crx_utils-1.2.0/crx/Loguru.py` & `crx_utils-1.3.0/crx/Loguru.py`

 * *Files identical despite different names*

### Comparing `crx_utils-1.2.0/crx/Reader.py` & `crx_utils-1.3.0/crx/Reader.py`

 * *Files identical despite different names*

### Comparing `crx_utils-1.2.0/crx/Tortoise.py` & `crx_utils-1.3.0/crx/Tortoise.py`

 * *Files identical despite different names*

### Comparing `crx_utils-1.2.0/setup.py` & `crx_utils-1.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="crx-utils",
-    version="1.2.0",
+    version="1.3.0",
     description="A collection of functions for creating Discord bots, works with nextcord.",
+    long_description="A collection of functions for creating Discord bots, works with nextcord.",
     url="https://discord.gg/EEp67FWQDP",
     author="CRX-DEV",
     author_email="cherniq66@gmail.com",
     license="MIT License",
     
 
     packages=find_packages(include=['crx', 'crx.*']),
```

