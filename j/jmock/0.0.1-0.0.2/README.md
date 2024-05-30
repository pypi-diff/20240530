# Comparing `tmp/jmock-0.0.1.tar.gz` & `tmp/jmock-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmock-0.0.1.tar", last modified: Thu May 30 08:43:13 2024, max compression
+gzip compressed data, was "jmock-0.0.2.tar", last modified: Thu May 30 08:57:06 2024, max compression
```

## Comparing `jmock-0.0.1.tar` & `jmock-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 08:43:13.237536 jmock-0.0.1/
--rw-rw-rw-   0        0        0      342 2024-05-30 08:43:13.235375 jmock-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-30 08:43:13.201499 jmock-0.0.1/jmock/
--rw-rw-rw-   0        0        0       48 2024-05-30 07:53:39.000000 jmock-0.0.1/jmock/__init__.py
--rw-rw-rw-   0        0        0     3339 2024-05-30 08:31:09.000000 jmock-0.0.1/jmock/aiFunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:43:13.228467 jmock-0.0.1/jmock.egg-info/
--rw-rw-rw-   0        0        0      342 2024-05-30 08:43:13.000000 jmock-0.0.1/jmock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2024-05-30 08:43:13.000000 jmock-0.0.1/jmock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 08:43:13.000000 jmock-0.0.1/jmock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-30 08:43:13.000000 jmock-0.0.1/jmock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-30 08:43:13.000000 jmock-0.0.1/jmock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 08:43:13.237536 jmock-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      626 2024-05-30 08:43:07.000000 jmock-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:57:06.283434 jmock-0.0.2/
+-rw-rw-rw-   0        0        0      342 2024-05-30 08:57:06.281434 jmock-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 08:57:06.257970 jmock-0.0.2/jmock/
+-rw-rw-rw-   0        0        0       48 2024-05-30 07:53:39.000000 jmock-0.0.2/jmock/__init__.py
+-rw-rw-rw-   0        0        0     3339 2024-05-30 08:31:09.000000 jmock-0.0.2/jmock/aiFunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:57:06.279437 jmock-0.0.2/jmock.egg-info/
+-rw-rw-rw-   0        0        0      342 2024-05-30 08:57:06.000000 jmock-0.0.2/jmock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-05-30 08:57:06.000000 jmock-0.0.2/jmock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:57:06.000000 jmock-0.0.2/jmock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 08:57:06.000000 jmock-0.0.2/jmock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 08:57:06.000000 jmock-0.0.2/jmock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 08:57:06.284434 jmock-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      626 2024-05-30 08:56:50.000000 jmock-0.0.2/setup.py
```

### Comparing `jmock-0.0.1/jmock/aiFunctions.py` & `jmock-0.0.2/jmock/aiFunctions.py`

 * *Files identical despite different names*

### Comparing `jmock-0.0.1/setup.py` & `jmock-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = "Joe's Synthetic Data Generator"
 LONG_DESCRIPTION = "AI Package to generate synthetic data using Google's gemini AI"
 REQUIRED_PACKAGES = [
   "langchain",
 "python-dotenv",
 "langchain_google_genai"
 ]
```

