# Comparing `tmp/hashtag_utils-0.3.tar.gz` & `tmp/hashtag_utils-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashtag_utils-0.3.tar", last modified: Thu May 30 20:49:48 2024, max compression
+gzip compressed data, was "hashtag_utils-0.4.tar", last modified: Thu May 30 20:53:55 2024, max compression
```

## Comparing `hashtag_utils-0.3.tar` & `hashtag_utils-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:49:48.084974 hashtag_utils-0.3/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.3/LICENSE
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1482 2024-05-30 20:49:48.084350 hashtag_utils-0.3/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1005 2024-05-30 20:47:35.000000 hashtag_utils-0.3/README.md
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:49:48.080901 hashtag_utils-0.3/hashtag_utils/
--rw-r--r--   0 aditya.patange   (502) staff       (20)      369 2024-05-30 20:06:44.000000 hashtag_utils-0.3/hashtag_utils/__init__.py
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1142 2024-05-30 20:32:27.000000 hashtag_utils-0.3/hashtag_utils/hashtag_generator.py
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:49:48.083731 hashtag_utils-0.3/hashtag_utils.egg-info/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1482 2024-05-30 20:49:48.000000 hashtag_utils-0.3/hashtag_utils.egg-info/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)      235 2024-05-30 20:49:48.000000 hashtag_utils-0.3/hashtag_utils.egg-info/SOURCES.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 20:49:48.000000 hashtag_utils-0.3/hashtag_utils.egg-info/dependency_links.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 20:49:48.000000 hashtag_utils-0.3/hashtag_utils.egg-info/top_level.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 20:49:48.085042 hashtag_utils-0.3/setup.cfg
--rw-r--r--   0 aditya.patange   (502) staff       (20)      628 2024-05-30 20:49:44.000000 hashtag_utils-0.3/setup.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:53:55.946855 hashtag_utils-0.4/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.4/LICENSE
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1543 2024-05-30 20:53:55.946445 hashtag_utils-0.4/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1066 2024-05-30 20:53:45.000000 hashtag_utils-0.4/README.md
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:53:55.943853 hashtag_utils-0.4/hashtag_utils/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      369 2024-05-30 20:06:44.000000 hashtag_utils-0.4/hashtag_utils/__init__.py
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1142 2024-05-30 20:32:27.000000 hashtag_utils-0.4/hashtag_utils/hashtag_generator.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:53:55.946013 hashtag_utils-0.4/hashtag_utils.egg-info/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1543 2024-05-30 20:53:55.000000 hashtag_utils-0.4/hashtag_utils.egg-info/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      235 2024-05-30 20:53:55.000000 hashtag_utils-0.4/hashtag_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 20:53:55.000000 hashtag_utils-0.4/hashtag_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 20:53:55.000000 hashtag_utils-0.4/hashtag_utils.egg-info/top_level.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 20:53:55.946918 hashtag_utils-0.4/setup.cfg
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      628 2024-05-30 20:53:52.000000 hashtag_utils-0.4/setup.py
```

### Comparing `hashtag_utils-0.3/LICENSE` & `hashtag_utils-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.3/PKG-INFO` & `hashtag_utils-0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: hashtag_utils
-Version: 0.3
+Version: 0.4
 Summary: Simple LLM-powered hashtag utilities.
 Home-page: http://github.com/AdiPat/hashtag_utils
 Author: Aditya Patange
 Author-email: contact.adityapatange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Hashtag Utilities
+# Hashtag Utilities 🏷️
 
-An LLM-powered multi-purpose hashtag utilities library written in Python. 🏷️
+An LLM-powered multi-purpose hashtag utilities library written in Python. 
 
-![Hashtag Utilities Hero](images/hero.png)
+![Hashtag Utilities Hero](https://raw.githubusercontent.com/AdiPat/hashtag_utils/main/images/hero.png)
 
 Hashtags are used on almost every content platform today. This makes it a vital tool for creating & analyzing content. 
 This utilities library makes it easy to do things with hashtags. Ideally, this module is intended to be used within a larger system where more specific problems are solved. 
 
 **Feel free to suggest features, ideas and improvements! If you want to contribute, feel free to fork and send a Pull Request. I'm actively working on this project.**
 
 ## Features
```

### Comparing `hashtag_utils-0.3/README.md` & `hashtag_utils-0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Hashtag Utilities
+# Hashtag Utilities 🏷️
 
-An LLM-powered multi-purpose hashtag utilities library written in Python. 🏷️
+An LLM-powered multi-purpose hashtag utilities library written in Python. 
 
-![Hashtag Utilities Hero](images/hero.png)
+![Hashtag Utilities Hero](https://raw.githubusercontent.com/AdiPat/hashtag_utils/main/images/hero.png)
 
 Hashtags are used on almost every content platform today. This makes it a vital tool for creating & analyzing content. 
 This utilities library makes it easy to do things with hashtags. Ideally, this module is intended to be used within a larger system where more specific problems are solved. 
 
 **Feel free to suggest features, ideas and improvements! If you want to contribute, feel free to fork and send a Pull Request. I'm actively working on this project.**
 
 ## Features
```

### Comparing `hashtag_utils-0.3/hashtag_utils/hashtag_generator.py` & `hashtag_utils-0.4/hashtag_utils/hashtag_generator.py`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.3/hashtag_utils.egg-info/PKG-INFO` & `hashtag_utils-0.4/hashtag_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: hashtag_utils
-Version: 0.3
+Version: 0.4
 Summary: Simple LLM-powered hashtag utilities.
 Home-page: http://github.com/AdiPat/hashtag_utils
 Author: Aditya Patange
 Author-email: contact.adityapatange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Hashtag Utilities
+# Hashtag Utilities 🏷️
 
-An LLM-powered multi-purpose hashtag utilities library written in Python. 🏷️
+An LLM-powered multi-purpose hashtag utilities library written in Python. 
 
-![Hashtag Utilities Hero](images/hero.png)
+![Hashtag Utilities Hero](https://raw.githubusercontent.com/AdiPat/hashtag_utils/main/images/hero.png)
 
 Hashtags are used on almost every content platform today. This makes it a vital tool for creating & analyzing content. 
 This utilities library makes it easy to do things with hashtags. Ideally, this module is intended to be used within a larger system where more specific problems are solved. 
 
 **Feel free to suggest features, ideas and improvements! If you want to contribute, feel free to fork and send a Pull Request. I'm actively working on this project.**
 
 ## Features
```

### Comparing `hashtag_utils-0.3/setup.py` & `hashtag_utils-0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hashtag_utils",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     author="Aditya Patange",
     author_email="contact.adityapatange@gmail.com",
     description="Simple LLM-powered hashtag utilities.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/AdiPat/hashtag_utils",
```

