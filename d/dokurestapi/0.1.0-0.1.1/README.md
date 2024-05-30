# Comparing `tmp/dokurestapi-0.1.0.tar.gz` & `tmp/dokurestapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dokurestapi-0.1.0.tar", last modified: Thu May 30 14:42:32 2024, max compression
+gzip compressed data, was "dist\dokurestapi-0.1.1.tar", last modified: Thu May 30 14:54:15 2024, max compression
```

## Comparing `dokurestapi-0.1.0.tar` & `dokurestapi-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/dokurestapi.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/dokurestapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4638 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/dokurestapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/dokurestapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0      238 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/dokurestapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/dokurestapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/Login/
--rw-rw-rw-   0        0        0     2177 2024-05-30 14:14:58.000000 dokurestapi-0.1.0/Login/__init__.py
--rw-rw-rw-   0        0        0     4638 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3221 2024-05-30 14:35:03.000000 dokurestapi-0.1.0/README.md
--rw-rw-rw-   0        0        0       86 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      767 2024-05-30 14:42:26.000000 dokurestapi-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:42:32.000000 dokurestapi-0.1.0/Users/
--rw-rw-rw-   0        0        0     9371 2024-05-30 14:13:27.000000 dokurestapi-0.1.0/Users/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/dokurestapi.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/dokurestapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4687 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/dokurestapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/dokurestapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      238 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/dokurestapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/dokurestapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/Login/
+-rw-rw-rw-   0        0        0     2177 2024-05-30 14:14:58.000000 dokurestapi-0.1.1/Login/__init__.py
+-rw-rw-rw-   0        0        0     4687 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3270 2024-05-30 14:51:32.000000 dokurestapi-0.1.1/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      767 2024-05-30 14:51:42.000000 dokurestapi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:54:15.000000 dokurestapi-0.1.1/Users/
+-rw-rw-rw-   0        0        0     9371 2024-05-30 14:13:27.000000 dokurestapi-0.1.1/Users/__init__.py
```

### Comparing `dokurestapi-0.1.0/dokurestapi.egg-info/PKG-INFO` & `dokurestapi-0.1.1/dokurestapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dokurestapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to interact with the DokuWiki REST API.
 Home-page: https://github.com/krowvin/dokurestapi
 Author: krowvin
 Author-email: charlie@krowvin.com
 License: MIT
 Description: # DokuRestAPI
         
         DokuRestAPI is a Python package that provides an easy-to-use interface for interacting with the DokuWiki web interface via its undocumented REST API. This package allows you to perform actions such as creating and deleting users, fetching user details, and managing other aspects of your DokuWiki instance programmatically.
         
-        If you would like to see other things added create an issue! I've just been adding things as I need them.
+        If you would like to see other things added [create an issue](https://github.com/krowvin/dokurestapi/issues)! I've just been adding things as I need them.
         
         ## Features
         
         - **User Management**: Create, delete, and fetch details of users.
         - **Session Management**: Login and maintain sessions to interact with the API.
         - **Integration**: Easily integrate with your DokuWiki instance using simple HTTP calls.
```

### Comparing `dokurestapi-0.1.0/Login/__init__.py` & `dokurestapi-0.1.1/Login/__init__.py`

 * *Files identical despite different names*

### Comparing `dokurestapi-0.1.0/PKG-INFO` & `dokurestapi-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dokurestapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to interact with the DokuWiki REST API.
 Home-page: https://github.com/krowvin/dokurestapi
 Author: krowvin
 Author-email: charlie@krowvin.com
 License: MIT
 Description: # DokuRestAPI
         
         DokuRestAPI is a Python package that provides an easy-to-use interface for interacting with the DokuWiki web interface via its undocumented REST API. This package allows you to perform actions such as creating and deleting users, fetching user details, and managing other aspects of your DokuWiki instance programmatically.
         
-        If you would like to see other things added create an issue! I've just been adding things as I need them.
+        If you would like to see other things added [create an issue](https://github.com/krowvin/dokurestapi/issues)! I've just been adding things as I need them.
         
         ## Features
         
         - **User Management**: Create, delete, and fetch details of users.
         - **Session Management**: Login and maintain sessions to interact with the API.
         - **Integration**: Easily integrate with your DokuWiki instance using simple HTTP calls.
```

### Comparing `dokurestapi-0.1.0/README.md` & `dokurestapi-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # DokuRestAPI
 
 DokuRestAPI is a Python package that provides an easy-to-use interface for interacting with the DokuWiki web interface via its undocumented REST API. This package allows you to perform actions such as creating and deleting users, fetching user details, and managing other aspects of your DokuWiki instance programmatically.
 
-If you would like to see other things added create an issue! I've just been adding things as I need them.
+If you would like to see other things added [create an issue](https://github.com/krowvin/dokurestapi/issues)! I've just been adding things as I need them.
 
 ## Features
 
 - **User Management**: Create, delete, and fetch details of users.
 - **Session Management**: Login and maintain sessions to interact with the API.
 - **Integration**: Easily integrate with your DokuWiki instance using simple HTTP calls.
```

### Comparing `dokurestapi-0.1.0/setup.py` & `dokurestapi-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="dokurestapi",
-    version="0.1.0",
+    version="0.1.1",
     author="krowvin",
     author_email="charlie@krowvin.com",
     description="A Python package to interact with the DokuWiki REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krowvin/dokurestapi",
     packages=find_packages(),
```

### Comparing `dokurestapi-0.1.0/Users/__init__.py` & `dokurestapi-0.1.1/Users/__init__.py`

 * *Files identical despite different names*

