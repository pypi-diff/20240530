# Comparing `tmp/catenp-0.0.7.tar.gz` & `tmp/catenp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catenp-0.0.7.tar", last modified: Fri Jun  9 13:52:28 2023, max compression
+gzip compressed data, was "catenp-0.0.9.tar", last modified: Thu Jun 22 12:08:20 2023, max compression
```

## Comparing `catenp-0.0.7.tar` & `catenp-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:52:28.669808 catenp-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     1173 2023-06-09 13:52:28.665359 catenp-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-09 11:05:06.000000 catenp-0.0.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:52:28.588952 catenp-0.0.7/catenp/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-06-09 09:37:10.000000 catenp-0.0.7/catenp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10052 2023-06-09 09:37:58.000000 catenp-0.0.7/catenp/catenumpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:52:28.654511 catenp-0.0.7/catenp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1173 2023-06-09 13:52:28.000000 catenp-0.0.7/catenp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      213 2023-06-09 13:52:28.000000 catenp-0.0.7/catenp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:52:28.000000 catenp-0.0.7/catenp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 13:52:28.000000 catenp-0.0.7/catenp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-09 13:52:28.000000 catenp-0.0.7/catenp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      668 2023-06-09 13:52:18.000000 catenp-0.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 13:52:28.672468 catenp-0.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:08:20.531267 catenp-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-06-22 12:08:20.527023 catenp-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      655 2023-06-22 12:06:00.000000 catenp-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:08:20.437611 catenp-0.0.9/catenp/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-06-09 09:37:10.000000 catenp-0.0.9/catenp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10052 2023-06-09 09:37:58.000000 catenp-0.0.9/catenp/catenumpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:08:20.514601 catenp-0.0.9/catenp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-06-22 12:08:20.000000 catenp-0.0.9/catenp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-06-22 12:08:20.000000 catenp-0.0.9/catenp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 12:08:20.000000 catenp-0.0.9/catenp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-22 12:08:20.000000 catenp-0.0.9/catenp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 12:08:20.000000 catenp-0.0.9/catenp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      675 2023-06-22 12:08:08.000000 catenp-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 12:08:20.535137 catenp-0.0.9/setup.cfg
```

### Comparing `catenp-0.0.7/README.rst` & `catenp-0.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,34 @@
------------
+
 DESCRIPTION
------------
+===========
 
 Python client for extracting data from CATE archives to numpy arrays
 
-------------
 INSTALLATION
 ------------
 
-::
 
-   pip install catenp
+    pip install catenp
 
 
------
 USAGE
 -----
 
 See also `catenp.catenumpy.Example`
 
-::
 
-   from catenp import Authenticate,DatabaseInfo,GetData
+    from catenp import Authenticate,DatabaseInfo,GetData
    
-   # Authenticate to the server
-   tk = Authenticate(serverAddress,serverPort,cateUserName,catePassword)
+    # Authenticate to the server
+    tk = Authenticate(serverAddress,serverPort,cateUserName,catePassword)
    
-   # (Optional) get server/ data info
-   info = DatabaseInfo(serverAddress,serverPort,cateUserName)
-   print("Info: ")
-   for kk in info: print("  ",kk,":",info[kk])
-
+    # (Optional) get server/ data info
+    info = DatabaseInfo(serverAddress,serverPort,cateUserName)
+    print("Info: ")
+    for kk in info: print("  ",kk,":",info[kk])
 
-   # Extract some data    
-   arr=GetData(serverAddress,serverPort,cateUserName,tstart,tstop,cstart,cstop)
+    # Extract some data    
+    arr=GetData(serverAddress,serverPort,cateUserName,tstart,tstop,cstart,cstop)
```

### Comparing `catenp-0.0.7/catenp/__init__.py` & `catenp-0.0.9/catenp/__init__.py`

 * *Files identical despite different names*

### Comparing `catenp-0.0.7/catenp/catenumpy.py` & `catenp-0.0.9/catenp/catenumpy.py`

 * *Files identical despite different names*

### Comparing `catenp-0.0.7/pyproject.toml` & `catenp-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=59.6.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "catenp"
-version = "0.0.7"
+version = "0.0.9"
 authors = [
-  { name="Motion Signal Technologies", email="info@motionsignaltechnologies.com" },
+  { name="Motion Signal Technologies", email="kit.chambers@motionsignaltechnologies.com" },
 ]
 description = "Python client for extracting data from CATE archives to numpy arrays"
-readme = "README.rst"
+readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent"
 ]
 dependencies = ["numpy>=1.24.3",
```

