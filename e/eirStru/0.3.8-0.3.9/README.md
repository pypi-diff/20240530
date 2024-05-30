# Comparing `tmp/eirStru-0.3.8.tar.gz` & `tmp/eirStru-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.3.8.tar", last modified: Sun Apr 21 17:25:26 2024, max compression
+gzip compressed data, was "eirStru-0.3.9.tar", last modified: Sun Apr 21 17:43:57 2024, max compression
```

## Comparing `eirStru-0.3.8.tar` & `eirStru-0.3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:25:26.552600 eirStru-0.3.8/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.8/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.8/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 17:25:26.552342 eirStru-0.3.8/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.8/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:25:26.551733 eirStru-0.3.8/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.8/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.8/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.8/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    17773 2024-04-21 17:25:16.000000 eirStru-0.3.8/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.8/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.8/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.8/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.8/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.8/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.8/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:25:26.552154 eirStru-0.3.8/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 17:25:26.000000 eirStru-0.3.8/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 17:25:26.000000 eirStru-0.3.8/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 17:25:26.000000 eirStru-0.3.8/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 17:25:26.000000 eirStru-0.3.8/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 17:25:26.552642 eirStru-0.3.8/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 17:25:25.000000 eirStru-0.3.8/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:43:57.633756 eirStru-0.3.9/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.9/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.9/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 17:43:57.633540 eirStru-0.3.9/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.9/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:43:57.632931 eirStru-0.3.9/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.9/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.9/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.9/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    17828 2024-04-21 17:43:55.000000 eirStru-0.3.9/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.9/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.9/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.9/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.9/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.9/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.9/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:43:57.633374 eirStru-0.3.9/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 17:43:57.000000 eirStru-0.3.9/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 17:43:57.000000 eirStru-0.3.9/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 17:43:57.000000 eirStru-0.3.9/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 17:43:57.000000 eirStru-0.3.9/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 17:43:57.633804 eirStru-0.3.9/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 17:43:55.000000 eirStru-0.3.9/setup.py
```

### Comparing `eirStru-0.3.8/LICENSE` & `eirStru-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.8/PKG-INFO` & `eirStru-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.8
+Version: 0.3.9
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.8/README.md` & `eirStru-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.8/eirStru/aiomysql_helper.py` & `eirStru-0.3.9/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.8/eirStru/common.py` & `eirStru-0.3.9/eirStru/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,25 +310,25 @@
 
         for item in ctntypedigit_dict.values():
             item.ctn_digit = item.ctn_digit or item.ctn_list_count
 
             # 本次打印量=min(已申请量-已打印量,箱量)
             item.ctn_digit_for_print = min(item.ctn_digit_applied - item.ctn_digit_printed, item.ctn_digit)
 
-            # 总申请量=0 本次申请量=箱量-可打印量
-            if item.ctn_digit_need_apply == 0:
-                if self.ctntype_id:
-                    if item.ctn_digit > item.ctn_digit_applied - item.ctn_digit_printed:
-                        item.ctn_digit_for_apply = item.ctn_digit - item.ctn_digit_applied + item.ctn_digit_printed
-                else:
-                    item.ctn_digit_for_apply = item.ctn_list_count - item.ctn_digit_applied
-            # 总申请量>0 本次需申请量=总申请量-已申请量
+            # 非msk,cma;
+            if self.carrier_id not in ['MSK-EIR', 'CMA-EIR']:
+                # 非msk，cma因为有集装箱列表，所以只需考虑可申请数量
+                max_apply_count = item.ctn_list_count - item.ctn_digit_applied
+                item.ctn_digit_for_apply = min(item.ctn_digit, max_apply_count)
             elif item.ctn_digit_need_apply > item.ctn_digit_applied:
+                # cma统一申请模式
                 item.ctn_digit_for_apply = item.ctn_digit_need_apply - item.ctn_digit_applied
-
+            elif item.ctn_digit > item.ctn_digit_applied - item.ctn_digit_printed:
+                # msk模式
+                item.ctn_digit_for_apply = item.ctn_digit - item.ctn_digit_applied + item.ctn_digit_printed
         self.ctntypedigit_list = list(ctntypedigit_dict.values())
 
     def check_completed(self):
         """
         不需要申请，不需要打印
         """
         return not (self.need_apply or self.need_print)
```

### Comparing `eirStru-0.3.8/eirStru/eirjob_intf.py` & `eirStru-0.3.9/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.8/eirStru/eirlogin_intf.py` & `eirStru-0.3.9/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.8/eirStru/redis_utils.py` & `eirStru-0.3.9/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.8/eirStru/utils.py` & `eirStru-0.3.9/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.8/eirStru/wx_push.py` & `eirStru-0.3.9/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.8/eirStru.egg-info/PKG-INFO` & `eirStru-0.3.9/eirStru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.8
+Version: 0.3.9
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.8/setup.py` & `eirStru-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'eirStru'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.8'
+VERSION = '0.3.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

