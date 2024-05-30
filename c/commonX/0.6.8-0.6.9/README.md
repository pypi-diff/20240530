# Comparing `tmp/commonX-0.6.8.tar.gz` & `tmp/commonX-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonX-0.6.8.tar", last modified: Mon Feb 19 17:44:19 2024, max compression
+gzip compressed data, was "commonX-0.6.9.tar", last modified: Tue Feb 20 07:25:15 2024, max compression
```

## Comparing `commonX-0.6.8.tar` & `commonX-0.6.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:44:19.964599 commonX-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-19 17:44:19.964599 commonX-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-19 17:44:14.000000 commonX-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:44:19.956599 commonX-0.6.8/common/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-19 17:44:14.000000 commonX-0.6.8/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:44:19.956599 commonX-0.6.8/common/base/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-19 17:44:14.000000 commonX-0.6.8/common/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-19 17:44:14.000000 commonX-0.6.8/common/base/genor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-19 17:44:14.000000 commonX-0.6.8/common/base/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-02-19 17:44:14.000000 commonX-0.6.8/common/base/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-02-19 17:44:14.000000 commonX-0.6.8/common/base/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-02-19 17:44:14.000000 commonX-0.6.8/common/base/multi_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-02-19 17:44:14.000000 commonX-0.6.8/common/base/packer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-19 17:44:14.000000 commonX-0.6.8/common/base/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:44:19.960599 commonX-0.6.8/common/ext/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-19 17:44:14.000000 commonX-0.6.8/common/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-02-19 17:44:14.000000 commonX-0.6.8/common/ext/cookie_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-19 17:44:14.000000 commonX-0.6.8/common/ext/iphone_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-19 17:44:14.000000 commonX-0.6.8/common/ext/ocr_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-02-19 17:44:14.000000 commonX-0.6.8/common/ext/qq_email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:44:19.960599 commonX-0.6.8/common/postman/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-19 17:44:14.000000 commonX-0.6.8/common/postman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-02-19 17:44:14.000000 commonX-0.6.8/common/postman/postman_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-02-19 17:44:14.000000 commonX-0.6.8/common/postman/postman_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-02-19 17:44:14.000000 commonX-0.6.8/common/postman/postman_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:44:19.960599 commonX-0.6.8/common/util/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/args_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/assert_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/decorator_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/exception_utll.py
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/image_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/json_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/requests_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/sys_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-19 17:44:14.000000 commonX-0.6.8/common/util/typing_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:44:19.960599 commonX-0.6.8/commonX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-19 17:44:19.000000 commonX-0.6.8/commonX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-19 17:44:19.000000 commonX-0.6.8/commonX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 17:44:19.000000 commonX-0.6.8/commonX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-19 17:44:19.000000 commonX-0.6.8/commonX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 17:44:19.964599 commonX-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-19 17:44:14.000000 commonX-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 07:25:15.839231 commonX-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-20 07:25:15.839231 commonX-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-20 07:25:10.000000 commonX-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 07:25:15.835231 commonX-0.6.9/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-20 07:25:10.000000 commonX-0.6.9/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 07:25:15.835231 commonX-0.6.9/common/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-20 07:25:10.000000 commonX-0.6.9/common/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-20 07:25:10.000000 commonX-0.6.9/common/base/genor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-20 07:25:10.000000 commonX-0.6.9/common/base/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-02-20 07:25:10.000000 commonX-0.6.9/common/base/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-02-20 07:25:10.000000 commonX-0.6.9/common/base/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-02-20 07:25:10.000000 commonX-0.6.9/common/base/multi_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-02-20 07:25:10.000000 commonX-0.6.9/common/base/packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-02-20 07:25:10.000000 commonX-0.6.9/common/base/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 07:25:15.835231 commonX-0.6.9/common/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-20 07:25:10.000000 commonX-0.6.9/common/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-02-20 07:25:10.000000 commonX-0.6.9/common/ext/cookie_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-20 07:25:10.000000 commonX-0.6.9/common/ext/iphone_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-20 07:25:10.000000 commonX-0.6.9/common/ext/ocr_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-02-20 07:25:10.000000 commonX-0.6.9/common/ext/qq_email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 07:25:15.839231 commonX-0.6.9/common/postman/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-20 07:25:10.000000 commonX-0.6.9/common/postman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-02-20 07:25:10.000000 commonX-0.6.9/common/postman/postman_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-02-20 07:25:10.000000 commonX-0.6.9/common/postman/postman_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-02-20 07:25:10.000000 commonX-0.6.9/common/postman/postman_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 07:25:15.839231 commonX-0.6.9/common/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/args_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/assert_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/decorator_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/exception_utll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/image_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/requests_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/sys_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-20 07:25:10.000000 commonX-0.6.9/common/util/typing_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 07:25:15.839231 commonX-0.6.9/commonX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-20 07:25:15.000000 commonX-0.6.9/commonX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-20 07:25:15.000000 commonX-0.6.9/commonX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 07:25:15.000000 commonX-0.6.9/commonX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-20 07:25:15.000000 commonX-0.6.9/commonX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 07:25:15.839231 commonX-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-20 07:25:10.000000 commonX-0.6.9/setup.py
```

### Comparing `commonX-0.6.8/PKG-INFO` & `commonX-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.6.8
+Version: 0.6.9
 Summary: python common toolkit
 Home-page: https://github.com/hect0x7/common
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `commonX-0.6.8/common/base/__init__.py` & `commonX-0.6.9/common/base/__init__.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/base/genor.py` & `commonX-0.6.9/common/base/genor.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/base/hook.py` & `commonX-0.6.9/common/base/hook.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/base/logger.py` & `commonX-0.6.9/common/base/logger.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/base/mapper.py` & `commonX-0.6.9/common/base/mapper.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/base/multi_task.py` & `commonX-0.6.9/common/base/multi_task.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/base/packer.py` & `commonX-0.6.9/common/base/packer.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/ext/cookie_parser.py` & `commonX-0.6.9/common/ext/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/ext/iphone_client.py` & `commonX-0.6.9/common/ext/iphone_client.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/ext/qq_email.py` & `commonX-0.6.9/common/ext/qq_email.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/postman/postman_api.py` & `commonX-0.6.9/common/postman/postman_api.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/postman/postman_impl.py` & `commonX-0.6.9/common/postman/postman_impl.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/postman/postman_proxy.py` & `commonX-0.6.9/common/postman/postman_proxy.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/args_util.py` & `commonX-0.6.9/common/util/args_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/assert_util.py` & `commonX-0.6.9/common/util/assert_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/decorator_util.py` & `commonX-0.6.9/common/util/decorator_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/exception_utll.py` & `commonX-0.6.9/common/util/exception_utll.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/file_util.py` & `commonX-0.6.9/common/util/file_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/image_util.py` & `commonX-0.6.9/common/util/image_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/json_util.py` & `commonX-0.6.9/common/util/json_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/requests_util.py` & `commonX-0.6.9/common/util/requests_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/sys_util.py` & `commonX-0.6.9/common/util/sys_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/time_util.py` & `commonX-0.6.9/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/common/util/typing_util.py` & `commonX-0.6.9/common/util/typing_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/commonX.egg-info/PKG-INFO` & `commonX-0.6.9/commonX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.6.8
+Version: 0.6.9
 Summary: python common toolkit
 Home-page: https://github.com/hect0x7/common
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `commonX-0.6.8/commonX.egg-info/SOURCES.txt` & `commonX-0.6.9/commonX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonX-0.6.8/setup.py` & `commonX-0.6.9/setup.py`

 * *Files identical despite different names*

