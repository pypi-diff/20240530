# Comparing `tmp/pynumint-0.0.9.tar.gz` & `tmp/pynumint-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumint-0.0.9.tar", last modified: Thu May 30 14:21:23 2024, max compression
+gzip compressed data, was "pynumint-0.1.0.tar", last modified: Thu May 30 14:24:13 2024, max compression
```

## Comparing `pynumint-0.0.9.tar` & `pynumint-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:21:23.591040 pynumint-0.0.9/
--rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     5453 2024-05-30 14:21:23.591040 pynumint-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4434 2024-05-30 13:47:32.000000 pynumint-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 14:21:23.561079 pynumint-0.0.9/pynumint/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:21:23.591040 pynumint-0.0.9/pynumint/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:21:23.581037 pynumint-0.0.9/pynumint/src/pynumint.egg-info/
--rw-rw-rw-   0        0        0     5453 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.0.9/pynumint/src/pynumint.py
--rw-rw-rw-   0        0        0       42 2024-05-30 14:21:23.591040 pynumint-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1856 2024-05-30 14:20:54.000000 pynumint-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:24:13.627863 pynumint-0.1.0/
+-rw-rw-rw-   0        0        0     1069 2024-05-30 14:23:16.000000 pynumint-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5454 2024-05-30 14:24:13.627863 pynumint-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4434 2024-05-30 13:47:32.000000 pynumint-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 14:24:13.597912 pynumint-0.1.0/pynumint/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:24:13.617918 pynumint-0.1.0/pynumint/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:24:13.617918 pynumint-0.1.0/pynumint/src/pynumint.egg-info/
+-rw-rw-rw-   0        0        0     5454 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.1.0/pynumint/src/pynumint.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:24:13.627863 pynumint-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1857 2024-05-30 14:24:10.000000 pynumint-0.1.0/setup.py
```

### Comparing `pynumint-0.0.9/LICENSE` & `pynumint-0.1.0/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2024 The Python Packaging Authority
+Copyright (c) 2024 pynumint
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pynumint-0.0.9/PKG-INFO` & `pynumint-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.9
-Summary: pynumint Test Package for Numerical Integration Demo
+Version: 0.1.0
+Summary: pynumint is a package for Numerical Integration tasks
 Home-page: https://github.com/CodeSleuthX/pynumint
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/CodeSleuthX/pynumint/issues
 Project-URL: Source, https://github.com/CodeSleuthX/pynumint
 Keywords: numerical integration mathematics science
```

### Comparing `pynumint-0.0.9/README.md` & `pynumint-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.9/pynumint/src/pynumint.egg-info/PKG-INFO` & `pynumint-0.1.0/pynumint/src/pynumint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.9
-Summary: pynumint Test Package for Numerical Integration Demo
+Version: 0.1.0
+Summary: pynumint is a package for Numerical Integration tasks
 Home-page: https://github.com/CodeSleuthX/pynumint
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/CodeSleuthX/pynumint/issues
 Project-URL: Source, https://github.com/CodeSleuthX/pynumint
 Keywords: numerical integration mathematics science
```

### Comparing `pynumint-0.0.9/pynumint/src/pynumint.py` & `pynumint-0.1.0/pynumint/src/pynumint.py`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.9/setup.py` & `pynumint-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 print("Installing pynumint...")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pynumint",
-    version="0.0.9",
+    version="0.1.0",
     author="Arjun Jagdale",
     author_email="arjunjagdale14@gmail.com",
-    description="pynumint Test Package for Numerical Integration Demo",
+    description="pynumint is a package for Numerical Integration tasks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CodeSleuthX/pynumint",
     packages=setuptools.find_packages(where='pynumint/src'),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

