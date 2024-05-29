# Comparing `tmp/almax_common-0.9.2.tar.gz` & `tmp/almax_common-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-0.9.2.tar", last modified: Wed May 29 22:07:57 2024, max compression
+gzip compressed data, was "almax_common-0.9.3.tar", last modified: Wed May 29 22:22:15 2024, max compression
```

## Comparing `almax_common-0.9.2.tar` & `almax_common-0.9.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:07:57.508433 almax_common-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 22:07:57.508433 almax_common-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 22:07:33.000000 almax_common-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:07:57.508433 almax_common-0.9.2/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 22:07:57.000000 almax_common-0.9.2/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 22:07:57.000000 almax_common-0.9.2/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:07:57.000000 almax_common-0.9.2/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 22:07:57.000000 almax_common-0.9.2/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 22:07:57.508433 almax_common-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-29 22:07:33.000000 almax_common-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:22:15.894073 almax_common-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 22:22:15.894073 almax_common-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 22:21:51.000000 almax_common-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:22:15.894073 almax_common-0.9.3/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 22:22:15.000000 almax_common-0.9.3/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 22:22:15.000000 almax_common-0.9.3/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:22:15.000000 almax_common-0.9.3/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:22:15.000000 almax_common-0.9.3/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 22:22:15.894073 almax_common-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-29 22:21:51.000000 almax_common-0.9.3/setup.py
```

### Comparing `almax_common-0.9.2/setup.py` & `almax_common-0.9.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,17 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name='almax_common',
-    version='0.9.2',
+    version='0.9.3',
     description='A common library with some of my implementations',
     long_description='test',
     long_description_content_type='text/markdown',
     author='AlMax98',
     author_email='alihaider.maqsood@gmail.com',
-    packages=find_packages(),
-    install_requires=[],
-    py_modules=['Common']
+    packages=find_packages(where='.'),  # Ensure it finds the Common package
+    package_dir={'': '.'},  # Specify the root directory as the package directory
+    install_requires=[],  # Add any dependencies here
 );
```

