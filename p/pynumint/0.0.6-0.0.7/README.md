# Comparing `tmp/pynumint-0.0.6.tar.gz` & `tmp/pynumint-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumint-0.0.6.tar", last modified: Thu May 30 08:47:40 2024, max compression
+gzip compressed data, was "pynumint-0.0.7.tar", last modified: Thu May 30 13:48:34 2024, max compression
```

## Comparing `pynumint-0.0.6.tar` & `pynumint-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 08:47:40.001984 pynumint-0.0.6/
--rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3978 2024-05-30 08:47:40.000359 pynumint-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3470 2024-05-30 07:34:52.000000 pynumint-0.0.6/README.md
--rw-rw-rw-   0        0        0      160 2024-05-30 08:34:23.000000 pynumint-0.0.6/post_install.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:47:39.795105 pynumint-0.0.6/pynumint/
-drwxrwxrwx   0        0        0        0 2024-05-30 08:47:39.982222 pynumint-0.0.6/pynumint/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 08:47:39.958217 pynumint-0.0.6/pynumint/src/pynumint.egg-info/
--rw-rw-rw-   0        0        0     3978 2024-05-30 08:47:39.000000 pynumint-0.0.6/pynumint/src/pynumint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-30 08:47:39.000000 pynumint-0.0.6/pynumint/src/pynumint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 08:47:39.000000 pynumint-0.0.6/pynumint/src/pynumint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 08:47:39.000000 pynumint-0.0.6/pynumint/src/pynumint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.0.6/pynumint/src/pynumint.py
--rw-rw-rw-   0        0        0       42 2024-05-30 08:47:40.001984 pynumint-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      982 2024-05-30 08:47:05.000000 pynumint-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:48:34.019258 pynumint-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4942 2024-05-30 13:48:34.019258 pynumint-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4434 2024-05-30 13:47:32.000000 pynumint-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 13:48:33.517269 pynumint-0.0.7/pynumint/
+drwxrwxrwx   0        0        0        0 2024-05-30 13:48:34.019258 pynumint-0.0.7/pynumint/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 13:48:33.968770 pynumint-0.0.7/pynumint/src/pynumint.egg-info/
+-rw-rw-rw-   0        0        0     4942 2024-05-30 13:48:33.000000 pynumint-0.0.7/pynumint/src/pynumint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2024-05-30 13:48:33.000000 pynumint-0.0.7/pynumint/src/pynumint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 13:48:33.000000 pynumint-0.0.7/pynumint/src/pynumint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-30 13:48:33.000000 pynumint-0.0.7/pynumint/src/pynumint.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 13:48:33.000000 pynumint-0.0.7/pynumint/src/pynumint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.0.7/pynumint/src/pynumint.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 13:48:34.019258 pynumint-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2024-05-30 13:47:48.000000 pynumint-0.0.7/setup.py
```

### Comparing `pynumint-0.0.6/LICENSE` & `pynumint-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.6/pynumint/src/pynumint.py` & `pynumint-0.0.7/pynumint/src/pynumint.py`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.6/setup.py` & `pynumint-0.0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 print("Installing pynumint...")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pynumint",
-    version="0.0.6",
+    version="0.0.7",
     author="Arjun Jagdale",
     author_email="arjunjagdale14@gmail.com",
     description="pynumint Test Package for Numerical Integration Demo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/pynumint/",
     packages=setuptools.find_packages(),
@@ -22,12 +22,16 @@
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     py_modules=["pynumint"],
     package_dir={'': 'pynumint/src'},
     install_requires=[],
 
-    scripts=['post_install.py'],
+    entry_points={
+        'console_scripts': [
+            'pynumint-post-install = post_install:print_word_star_pattern',
+        ],
+    },
 )
 
 # Print a completion message
 print("pynumint has been successfully installed!")
```

