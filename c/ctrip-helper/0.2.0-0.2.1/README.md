# Comparing `tmp/ctrip-helper-0.2.0.tar.gz` & `tmp/ctrip-helper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.2.0.tar", last modified: Thu May 30 10:28:37 2024, max compression
+gzip compressed data, was "ctrip-helper-0.2.1.tar", last modified: Thu May 30 16:54:08 2024, max compression
```

## Comparing `ctrip-helper-0.2.0.tar` & `ctrip-helper-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 10:28:37.305697 ctrip-helper-0.2.0/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 10:28:37.304700 ctrip-helper-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 10:28:37.288744 ctrip-helper-0.2.0/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.0/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:28:37.301707 ctrip-helper-0.2.0/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.0/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30232 2024-05-30 10:16:18.000000 ctrip-helper-0.2.0/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.0/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.0/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.0/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4682 2024-05-30 10:28:17.000000 ctrip-helper-0.2.0/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.0/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:28:37.302705 ctrip-helper-0.2.0/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 10:28:37.000000 ctrip-helper-0.2.0/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 10:28:37.000000 ctrip-helper-0.2.0/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 10:28:37.000000 ctrip-helper-0.2.0/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 10:28:37.000000 ctrip-helper-0.2.0/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 10:28:37.000000 ctrip-helper-0.2.0/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 10:28:37.305697 ctrip-helper-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 10:28:31.000000 ctrip-helper-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:54:08.212754 ctrip-helper-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 16:54:08.210761 ctrip-helper-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 16:54:08.193806 ctrip-helper-0.2.1/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.1/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:54:08.206771 ctrip-helper-0.2.1/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.1/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30232 2024-05-30 10:16:18.000000 ctrip-helper-0.2.1/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.1/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.1/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.1/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.1/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.1/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:54:08.208765 ctrip-helper-0.2.1/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 16:54:08.000000 ctrip-helper-0.2.1/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 16:54:08.000000 ctrip-helper-0.2.1/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 16:54:08.000000 ctrip-helper-0.2.1/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 16:54:08.000000 ctrip-helper-0.2.1/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 16:54:08.000000 ctrip-helper-0.2.1/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 16:54:08.212754 ctrip-helper-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 16:54:03.000000 ctrip-helper-0.2.1/setup.py
```

### Comparing `ctrip-helper-0.2.0/LICENSE` & `ctrip-helper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.0/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.2.1/ctrip_helper/api/desktop_ui.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.0/ctrip_helper/api/http_api.py` & `ctrip-helper-0.2.1/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.0/ctrip_helper/config.py` & `ctrip-helper-0.2.1/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.0/ctrip_helper/http_client.py` & `ctrip-helper-0.2.1/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.0/ctrip_helper/libs.py` & `ctrip-helper-0.2.1/ctrip_helper/libs.py`

 * *Files 15% similar despite different names*

```diff
@@ -122,7 +122,21 @@
             if is_log_output is True:
                 logger.error(err_str)
             if is_ignore is False:
                 raise OverflowError("Element found failed, reason: {}".format(err_str))
         if sleep > 0:
             time.sleep(sleep)
     return element
+
+
+def switch_to_window(driver: webdriver, origin_windows: list, loop: int, sleep: float) -> bool:
+    for i in range(loop):
+        # 获取所有的窗口句柄
+        all_windows = driver.window_handles
+        diff = set(all_windows).difference(set(origin_windows))
+        if len(diff) > 0:
+            new_window = diff.pop()
+            driver.switch_to.window(new_window)
+            return True
+        if sleep > 0:
+            time.sleep(sleep)
+    return False
```

### Comparing `ctrip-helper-0.2.0/ctrip_helper/utils.py` & `ctrip-helper-0.2.1/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.0/setup.py` & `ctrip-helper-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.2.0',
+    version='0.2.1',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

