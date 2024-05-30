# Comparing `tmp/sakura_fm-0.0.7.tar.gz` & `tmp/sakura_fm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sakura_fm-0.0.7.tar", last modified: Thu May 30 06:07:07 2024, max compression
+gzip compressed data, was "sakura_fm-0.0.8.tar", last modified: Thu May 30 06:31:40 2024, max compression
```

## Comparing `sakura_fm-0.0.7.tar` & `sakura_fm-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 06:07:07.755248 sakura_fm-0.0.7/
--rw-rw-rw-   0        0        0     1083 2024-05-24 09:50:28.000000 sakura_fm-0.0.7/LICENCE
--rw-rw-rw-   0        0        0     2193 2024-05-30 06:07:07.752242 sakura_fm-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1756 2024-05-24 09:46:07.000000 sakura_fm-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 06:07:07.687365 sakura_fm-0.0.7/sakura/
--rw-rw-rw-   0        0        0       26 2024-05-24 08:11:31.000000 sakura_fm-0.0.7/sakura/__init__.py
--rw-rw-rw-   0        0        0     1891 2024-05-24 09:44:39.000000 sakura_fm-0.0.7/sakura/client.py
--rw-rw-rw-   0        0        0      980 2024-05-24 09:28:13.000000 sakura_fm-0.0.7/sakura/db.py
--rw-rw-rw-   0        0        0     4506 2024-05-24 08:34:13.000000 sakura_fm-0.0.7/sakura/sakura.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:07:07.749242 sakura_fm-0.0.7/sakura_fm.egg-info/
--rw-rw-rw-   0        0        0     2193 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 06:07:07.756244 sakura_fm-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      900 2024-05-30 06:05:16.000000 sakura_fm-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:31:40.327200 sakura_fm-0.0.8/
+-rw-rw-rw-   0        0        0     1083 2024-05-24 09:50:28.000000 sakura_fm-0.0.8/LICENCE
+-rw-rw-rw-   0        0        0     2190 2024-05-30 06:31:40.324849 sakura_fm-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1753 2024-05-30 06:23:33.000000 sakura_fm-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 06:31:40.279692 sakura_fm-0.0.8/sakura/
+-rw-rw-rw-   0        0        0       26 2024-05-24 08:11:31.000000 sakura_fm-0.0.8/sakura/__init__.py
+-rw-rw-rw-   0        0        0     1891 2024-05-24 09:44:39.000000 sakura_fm-0.0.8/sakura/client.py
+-rw-rw-rw-   0        0        0      980 2024-05-24 09:28:13.000000 sakura_fm-0.0.8/sakura/db.py
+-rw-rw-rw-   0        0        0     4506 2024-05-24 08:34:13.000000 sakura_fm-0.0.8/sakura/sakura.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:31:40.322581 sakura_fm-0.0.8/sakura_fm.egg-info/
+-rw-rw-rw-   0        0        0     2190 2024-05-30 06:31:40.000000 sakura_fm-0.0.8/sakura_fm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-05-30 06:31:40.000000 sakura_fm-0.0.8/sakura_fm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:31:40.000000 sakura_fm-0.0.8/sakura_fm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-30 06:31:40.000000 sakura_fm-0.0.8/sakura_fm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-05-30 06:31:40.000000 sakura_fm-0.0.8/sakura_fm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 06:31:40.000000 sakura_fm-0.0.8/sakura_fm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:31:40.328470 sakura_fm-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      900 2024-05-30 06:22:57.000000 sakura_fm-0.0.8/setup.py
```

### Comparing `sakura_fm-0.0.7/LICENCE` & `sakura_fm-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.7/PKG-INFO` & `sakura_fm-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sakura-fm
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple scraper package for chatting with bots from sakura.fm
 Home-page: https://github.com/awesome-Tofu/sakura_fm
 Author: Aditya
 Author-email: adityaraj6311@gmail.com
 Keywords: sakura,sakura.fm,sakura scraper,sakurai
 Description-Content-Type: text/markdown
 License-File: LICENCE
@@ -17,23 +17,23 @@
 This is a Python client for the Sakura API. It provides methods to authenticate, send messages, get selfies, and more.
 
 ## Installation
 
 You can install the Sakura Python Client using pip:
 
 ```bash
-pip install sakura_fm
+pip install sakura-fm
 ```
 
 ## Usage
 
 First, import the `Client` class from the `sakura` package:
 
 ```python
-from sakura_fm import Client
+from sakura import Client
 ```
 
 Next, create an instance of the `Client` class, passing your Sakura username, password and mongo uri to the constructor:
 
 ```python
 client = Client(
     username = "your_username",
```

### Comparing `sakura_fm-0.0.7/README.md` & `sakura_fm-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 This is a Python client for the Sakura API. It provides methods to authenticate, send messages, get selfies, and more.
 
 ## Installation
 
 You can install the Sakura Python Client using pip:
 
 ```bash
-pip install sakura_fm
+pip install sakura-fm
 ```
 
 ## Usage
 
 First, import the `Client` class from the `sakura` package:
 
 ```python
-from sakura_fm import Client
+from sakura import Client
 ```
 
 Next, create an instance of the `Client` class, passing your Sakura username, password and mongo uri to the constructor:
 
 ```python
 client = Client(
     username = "your_username",
```

### Comparing `sakura_fm-0.0.7/sakura/client.py` & `sakura_fm-0.0.8/sakura/client.py`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.7/sakura/db.py` & `sakura_fm-0.0.8/sakura/db.py`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.7/sakura/sakura.py` & `sakura_fm-0.0.8/sakura/sakura.py`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.7/sakura_fm.egg-info/PKG-INFO` & `sakura_fm-0.0.8/sakura_fm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sakura-fm
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple scraper package for chatting with bots from sakura.fm
 Home-page: https://github.com/awesome-Tofu/sakura_fm
 Author: Aditya
 Author-email: adityaraj6311@gmail.com
 Keywords: sakura,sakura.fm,sakura scraper,sakurai
 Description-Content-Type: text/markdown
 License-File: LICENCE
@@ -17,23 +17,23 @@
 This is a Python client for the Sakura API. It provides methods to authenticate, send messages, get selfies, and more.
 
 ## Installation
 
 You can install the Sakura Python Client using pip:
 
 ```bash
-pip install sakura_fm
+pip install sakura-fm
 ```
 
 ## Usage
 
 First, import the `Client` class from the `sakura` package:
 
 ```python
-from sakura_fm import Client
+from sakura import Client
 ```
 
 Next, create an instance of the `Client` class, passing your Sakura username, password and mongo uri to the constructor:
 
 ```python
 client = Client(
     username = "your_username",
```

### Comparing `sakura_fm-0.0.7/setup.py` & `sakura_fm-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 
 def get_long_description():
     with open("README.md", encoding="UTF-8") as f:
         long_description = f.read()
         return long_description
 
 setup(
```

