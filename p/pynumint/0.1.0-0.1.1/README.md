# Comparing `tmp/pynumint-0.1.0.tar.gz` & `tmp/pynumint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumint-0.1.0.tar", last modified: Thu May 30 14:24:13 2024, max compression
+gzip compressed data, was "pynumint-0.1.1.tar", last modified: Thu May 30 14:27:18 2024, max compression
```

## Comparing `pynumint-0.1.0.tar` & `pynumint-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:13.627863 pynumint-0.1.0/
--rw-rw-rw-   0        0        0     1069 2024-05-30 14:23:16.000000 pynumint-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5454 2024-05-30 14:24:13.627863 pynumint-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4434 2024-05-30 13:47:32.000000 pynumint-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:13.597912 pynumint-0.1.0/pynumint/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:13.617918 pynumint-0.1.0/pynumint/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:13.617918 pynumint-0.1.0/pynumint/src/pynumint.egg-info/
--rw-rw-rw-   0        0        0     5454 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 14:24:13.000000 pynumint-0.1.0/pynumint/src/pynumint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.1.0/pynumint/src/pynumint.py
--rw-rw-rw-   0        0        0       42 2024-05-30 14:24:13.627863 pynumint-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1857 2024-05-30 14:24:10.000000 pynumint-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:27:18.252876 pynumint-0.1.1/
+-rw-rw-rw-   0        0        0     1069 2024-05-30 14:23:16.000000 pynumint-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5454 2024-05-30 14:27:18.242918 pynumint-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4434 2024-05-30 13:47:32.000000 pynumint-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 14:27:18.222879 pynumint-0.1.1/pynumint/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:27:18.242918 pynumint-0.1.1/pynumint/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:27:18.242918 pynumint-0.1.1/pynumint/src/pynumint.egg-info/
+-rw-rw-rw-   0        0        0     5454 2024-05-30 14:27:18.000000 pynumint-0.1.1/pynumint/src/pynumint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-30 14:27:18.000000 pynumint-0.1.1/pynumint/src/pynumint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:27:18.000000 pynumint-0.1.1/pynumint/src/pynumint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-30 14:27:18.000000 pynumint-0.1.1/pynumint/src/pynumint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 14:27:18.000000 pynumint-0.1.1/pynumint/src/pynumint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.1.1/pynumint/src/pynumint.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:27:18.252876 pynumint-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1712 2024-05-30 14:27:00.000000 pynumint-0.1.1/setup.py
```

### Comparing `pynumint-0.1.0/LICENSE` & `pynumint-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumint-0.1.0/PKG-INFO` & `pynumint-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.1.0
+Version: 0.1.1
 Summary: pynumint is a package for Numerical Integration tasks
 Home-page: https://github.com/CodeSleuthX/pynumint
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/CodeSleuthX/pynumint/issues
 Project-URL: Source, https://github.com/CodeSleuthX/pynumint
```

### Comparing `pynumint-0.1.0/README.md` & `pynumint-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pynumint-0.1.0/pynumint/src/pynumint.egg-info/PKG-INFO` & `pynumint-0.1.1/pynumint/src/pynumint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.1.0
+Version: 0.1.1
 Summary: pynumint is a package for Numerical Integration tasks
 Home-page: https://github.com/CodeSleuthX/pynumint
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/CodeSleuthX/pynumint/issues
 Project-URL: Source, https://github.com/CodeSleuthX/pynumint
```

### Comparing `pynumint-0.1.0/pynumint/src/pynumint.py` & `pynumint-0.1.1/pynumint/src/pynumint.py`

 * *Files identical despite different names*

### Comparing `pynumint-0.1.0/setup.py` & `pynumint-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 print("Installing pynumint...")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pynumint",
-    version="0.1.0",
+    version="0.1.1",
     author="Arjun Jagdale",
     author_email="arjunjagdale14@gmail.com",
     description="pynumint is a package for Numerical Integration tasks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CodeSleuthX/pynumint",
     packages=setuptools.find_packages(where='pynumint/src'),
@@ -40,19 +40,15 @@
             'check-manifest',
             'flake8',
         ],
         'test': [
             'coverage',
         ],
     },
-    entry_points={
-        'console_scripts': [
-            'pynumint-post-install = post_install:print_word_star_pattern',
-        ],
-    },
+
     project_urls={
         'Bug Reports': 'https://github.com/CodeSleuthX/pynumint/issues',
         'Source': 'https://github.com/CodeSleuthX/pynumint',
     },
 )
 
 # Print a completion message
```

