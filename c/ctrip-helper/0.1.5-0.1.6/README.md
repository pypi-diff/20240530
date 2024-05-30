# Comparing `tmp/ctrip-helper-0.1.5.tar.gz` & `tmp/ctrip-helper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.1.5.tar", last modified: Thu May 30 03:21:10 2024, max compression
+gzip compressed data, was "ctrip-helper-0.1.6.tar", last modified: Thu May 30 05:29:06 2024, max compression
```

## Comparing `ctrip-helper-0.1.5.tar` & `ctrip-helper-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 03:21:10.183263 ctrip-helper-0.1.5/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 03:21:10.182266 ctrip-helper-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 03:21:10.168306 ctrip-helper-0.1.5/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.5/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:21:10.180271 ctrip-helper-0.1.5/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.5/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30309 2024-05-30 03:20:43.000000 ctrip-helper-0.1.5/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.5/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.1.5/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.5/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4575 2024-05-29 18:45:32.000000 ctrip-helper-0.1.5/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.5/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:21:10.181269 ctrip-helper-0.1.5/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 03:21:10.000000 ctrip-helper-0.1.5/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 03:21:10.000000 ctrip-helper-0.1.5/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 03:21:10.000000 ctrip-helper-0.1.5/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 03:21:10.000000 ctrip-helper-0.1.5/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 03:21:10.000000 ctrip-helper-0.1.5/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 03:21:10.184261 ctrip-helper-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 03:20:54.000000 ctrip-helper-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:29:06.890752 ctrip-helper-0.1.6/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 05:29:06.889755 ctrip-helper-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 05:29:06.874797 ctrip-helper-0.1.6/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.6/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:29:06.886763 ctrip-helper-0.1.6/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.6/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30297 2024-05-30 05:28:53.000000 ctrip-helper-0.1.6/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.6/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.1.6/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.6/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4575 2024-05-29 18:45:32.000000 ctrip-helper-0.1.6/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.6/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:29:06.887760 ctrip-helper-0.1.6/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 05:29:06.000000 ctrip-helper-0.1.6/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 05:29:06.000000 ctrip-helper-0.1.6/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 05:29:06.000000 ctrip-helper-0.1.6/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 05:29:06.000000 ctrip-helper-0.1.6/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 05:29:06.000000 ctrip-helper-0.1.6/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 05:29:06.890752 ctrip-helper-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 05:29:00.000000 ctrip-helper-0.1.6/setup.py
```

### Comparing `ctrip-helper-0.1.5/LICENSE` & `ctrip-helper-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.5/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.1.6/ctrip_helper/api/desktop_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,16 +91,16 @@
             logger.info("{}平台用户<{}>已登录".format(platform, username))
             return True
         else:
             return False
 
     @classmethod
     def open_login_page(cls, driver: webdriver, sleep: float = 0) -> None:
-        ctrip_login_prefix = url_map.get_url('ctrip_login_prefix')
-        ctrip_login_suffix = url_map.get_url('ctrip_login_suffix')
+        ctrip_login_prefix = url_map.get('ctrip_login_prefix')
+        ctrip_login_suffix = url_map.get('ctrip_login_suffix')
         login_url = "{}{}".format(ctrip_login_prefix, ctrip_login_suffix)
         driver.get(login_url)
         if sleep > 0:
             time.sleep(sleep)
         logger.info("打开携程网页版登录页")
 
     @classmethod
@@ -172,15 +172,15 @@
             logger.info("当前页面：{} 出现了滑块验证码".format(current_url))
             return True
         else:
             return False
 
     @classmethod
     def open_order_query_home_with_flight(cls, driver: webdriver, sleep: float = 0) -> None:
-        driver.get(url_map.get_url('order_query_home_with_flight'))
+        driver.get(url_map.get('order_query_home_with_flight'))
         if sleep > 0:
             time.sleep(sleep)
         logger.info("打开机票订单查询首页")
 
     @classmethod
     def click_more_filter_conditions(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         more_filter_expand = get_element(
```

### Comparing `ctrip-helper-0.1.5/ctrip_helper/api/http_api.py` & `ctrip-helper-0.1.6/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.5/ctrip_helper/config.py` & `ctrip-helper-0.1.6/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.5/ctrip_helper/http_client.py` & `ctrip-helper-0.1.6/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.5/ctrip_helper/libs.py` & `ctrip-helper-0.1.6/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.5/ctrip_helper/utils.py` & `ctrip-helper-0.1.6/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.5/setup.py` & `ctrip-helper-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.1.5',
+    version='0.1.6',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

