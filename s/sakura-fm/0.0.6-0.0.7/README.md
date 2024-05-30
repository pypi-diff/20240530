# Comparing `tmp/sakura_fm-0.0.6.tar.gz` & `tmp/sakura_fm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sakura_fm-0.0.6.tar", last modified: Fri May 24 12:49:06 2024, max compression
+gzip compressed data, was "sakura_fm-0.0.7.tar", last modified: Thu May 30 06:07:07 2024, max compression
```

## Comparing `sakura_fm-0.0.6.tar` & `sakura_fm-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 12:49:06.516264 sakura_fm-0.0.6/
--rw-rw-rw-   0        0        0     1083 2024-05-24 09:50:28.000000 sakura_fm-0.0.6/LICENCE
--rw-rw-rw-   0        0        0     2193 2024-05-24 12:49:06.513286 sakura_fm-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1756 2024-05-24 09:46:07.000000 sakura_fm-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 12:49:06.486088 sakura_fm-0.0.6/sakura/
--rw-rw-rw-   0        0        0       26 2024-05-24 08:11:31.000000 sakura_fm-0.0.6/sakura/__init__.py
--rw-rw-rw-   0        0        0     1891 2024-05-24 09:44:39.000000 sakura_fm-0.0.6/sakura/client.py
--rw-rw-rw-   0        0        0      980 2024-05-24 09:28:13.000000 sakura_fm-0.0.6/sakura/db.py
--rw-rw-rw-   0        0        0     4506 2024-05-24 08:34:13.000000 sakura_fm-0.0.6/sakura/sakura.py
-drwxrwxrwx   0        0        0        0 2024-05-24 12:49:06.509872 sakura_fm-0.0.6/sakura_fm.egg-info/
--rw-rw-rw-   0        0        0     2193 2024-05-24 12:49:06.000000 sakura_fm-0.0.6/sakura_fm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-24 12:49:06.000000 sakura_fm-0.0.6/sakura_fm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 12:49:06.000000 sakura_fm-0.0.6/sakura_fm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-24 12:49:06.000000 sakura_fm-0.0.6/sakura_fm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-05-24 12:49:06.000000 sakura_fm-0.0.6/sakura_fm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-24 12:49:06.000000 sakura_fm-0.0.6/sakura_fm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 12:49:06.516264 sakura_fm-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      900 2024-05-24 12:42:14.000000 sakura_fm-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:07:07.755248 sakura_fm-0.0.7/
+-rw-rw-rw-   0        0        0     1083 2024-05-24 09:50:28.000000 sakura_fm-0.0.7/LICENCE
+-rw-rw-rw-   0        0        0     2193 2024-05-30 06:07:07.752242 sakura_fm-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1756 2024-05-24 09:46:07.000000 sakura_fm-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 06:07:07.687365 sakura_fm-0.0.7/sakura/
+-rw-rw-rw-   0        0        0       26 2024-05-24 08:11:31.000000 sakura_fm-0.0.7/sakura/__init__.py
+-rw-rw-rw-   0        0        0     1891 2024-05-24 09:44:39.000000 sakura_fm-0.0.7/sakura/client.py
+-rw-rw-rw-   0        0        0      980 2024-05-24 09:28:13.000000 sakura_fm-0.0.7/sakura/db.py
+-rw-rw-rw-   0        0        0     4506 2024-05-24 08:34:13.000000 sakura_fm-0.0.7/sakura/sakura.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:07:07.749242 sakura_fm-0.0.7/sakura_fm.egg-info/
+-rw-rw-rw-   0        0        0     2193 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 06:07:07.000000 sakura_fm-0.0.7/sakura_fm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:07:07.756244 sakura_fm-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      900 2024-05-30 06:05:16.000000 sakura_fm-0.0.7/setup.py
```

### Comparing `sakura_fm-0.0.6/LICENCE` & `sakura_fm-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.6/PKG-INFO` & `sakura_fm-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sakura_fm
-Version: 0.0.6
+Name: sakura-fm
+Version: 0.0.7
 Summary: A simple scraper package for chatting with bots from sakura.fm
 Home-page: https://github.com/awesome-Tofu/sakura_fm
 Author: Aditya
 Author-email: adityaraj6311@gmail.com
 Keywords: sakura,sakura.fm,sakura scraper,sakurai
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `sakura_fm-0.0.6/README.md` & `sakura_fm-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.6/sakura/client.py` & `sakura_fm-0.0.7/sakura/client.py`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.6/sakura/db.py` & `sakura_fm-0.0.7/sakura/db.py`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.6/sakura/sakura.py` & `sakura_fm-0.0.7/sakura/sakura.py`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.6/sakura_fm.egg-info/PKG-INFO` & `sakura_fm-0.0.7/sakura_fm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sakura_fm
-Version: 0.0.6
+Name: sakura-fm
+Version: 0.0.7
 Summary: A simple scraper package for chatting with bots from sakura.fm
 Home-page: https://github.com/awesome-Tofu/sakura_fm
 Author: Aditya
 Author-email: adityaraj6311@gmail.com
 Keywords: sakura,sakura.fm,sakura scraper,sakurai
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `sakura_fm-0.0.6/setup.py` & `sakura_fm-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 def get_long_description():
     with open("README.md", encoding="UTF-8") as f:
         long_description = f.read()
         return long_description
 
 setup(
-    name='sakura_fm',
+    name='sakura-fm',
     version=VERSION,
     packages=find_packages(),
     include_package_data=True,
     long_description_content_type='text/markdown',
     author='Aditya',
     author_email='adityaraj6311@gmail.com',
     url="https://github.com/awesome-Tofu/sakura_fm",
```

