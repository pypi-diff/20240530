# Comparing `tmp/almax_common-0.9.0.tar.gz` & `tmp/almax_common-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-0.9.0.tar", last modified: Sun May 26 22:02:22 2024, max compression
+gzip compressed data, was "almax_common-0.9.1.tar", last modified: Wed May 29 21:12:31 2024, max compression
```

## Comparing `almax_common-0.9.0.tar` & `almax_common-0.9.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:02:22.502923 almax_common-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-26 22:02:22.502923 almax_common-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-26 22:01:53.000000 almax_common-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:02:22.502923 almax_common-0.9.0/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-26 22:02:22.000000 almax_common-0.9.0/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-26 22:02:22.000000 almax_common-0.9.0/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:02:22.000000 almax_common-0.9.0/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-26 22:02:22.000000 almax_common-0.9.0/almax_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:02:22.000000 almax_common-0.9.0/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 22:02:22.502923 almax_common-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-26 22:01:53.000000 almax_common-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:12:31.936332 almax_common-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 21:12:31.936332 almax_common-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 21:12:04.000000 almax_common-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:12:31.936332 almax_common-0.9.1/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 21:12:31.000000 almax_common-0.9.1/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 21:12:31.000000 almax_common-0.9.1/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:12:31.000000 almax_common-0.9.1/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:12:31.000000 almax_common-0.9.1/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:12:31.936332 almax_common-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 21:12:04.000000 almax_common-0.9.1/setup.py
```

### Comparing `almax_common-0.9.0/setup.py` & `almax_common-0.9.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,25 +4,16 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name='almax_common',
-    version='0.9.0',
+    version='0.9.1',
     description='A common library with some of my implementations',
     long_description='test',
     long_description_content_type='text/markdown',
     author='AlMax98',
     author_email='alihaider.maqsood@gmail.com',
     packages=find_packages(),
-    install_requires=[
-        'tkinter',
-        'logging',
-        'subprocess',
-        'reportlab',
-        'threading',
-        'datetime',
-        'os',
-        'sys'
-    ],
+    install_requires=[],
 );
```

