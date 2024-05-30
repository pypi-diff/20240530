# Comparing `tmp/ctrip-helper-0.2.4.tar.gz` & `tmp/ctrip-helper-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.2.4.tar", last modified: Thu May 30 17:19:39 2024, max compression
+gzip compressed data, was "ctrip-helper-0.2.5.tar", last modified: Thu May 30 17:30:41 2024, max compression
```

## Comparing `ctrip-helper-0.2.4.tar` & `ctrip-helper-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:19:39.825246 ctrip-helper-0.2.4/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 17:19:39.823253 ctrip-helper-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 17:19:39.808291 ctrip-helper-0.2.4/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.4/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:19:39.820260 ctrip-helper-0.2.4/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.4/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30280 2024-05-30 17:19:26.000000 ctrip-helper-0.2.4/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.4/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.4/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.4/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.4/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.4/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:19:39.822255 ctrip-helper-0.2.4/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 17:19:39.000000 ctrip-helper-0.2.4/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 17:19:39.000000 ctrip-helper-0.2.4/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:19:39.000000 ctrip-helper-0.2.4/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 17:19:39.000000 ctrip-helper-0.2.4/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 17:19:39.000000 ctrip-helper-0.2.4/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 17:19:39.825246 ctrip-helper-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 17:19:33.000000 ctrip-helper-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:30:41.943812 ctrip-helper-0.2.5/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 17:30:41.942815 ctrip-helper-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:30:41.927864 ctrip-helper-0.2.5/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.5/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:30:41.939822 ctrip-helper-0.2.5/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.5/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30280 2024-05-30 17:30:24.000000 ctrip-helper-0.2.5/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.5/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.5/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.5/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.5/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.5/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:30:41.941817 ctrip-helper-0.2.5/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 17:30:41.000000 ctrip-helper-0.2.5/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 17:30:41.000000 ctrip-helper-0.2.5/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:30:41.000000 ctrip-helper-0.2.5/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 17:30:41.000000 ctrip-helper-0.2.5/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 17:30:41.000000 ctrip-helper-0.2.5/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:30:41.943812 ctrip-helper-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 17:30:36.000000 ctrip-helper-0.2.5/setup.py
```

### Comparing `ctrip-helper-0.2.4/LICENSE` & `ctrip-helper-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.4/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.2.5/ctrip_helper/api/desktop_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         if current_url.startswith(local_url) is True:
             to_payment_button = get_element(
                 driver=driver, locator=UILocatorRegx.order_to_payment.value.get("locator"),
                 regx=UILocatorRegx.order_to_payment.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if to_payment_button:
                 to_payment_button.click()
-                logger.info("点击【去支付】，进入订单支付界面")
+                logger.info("点击【去支付】，进入安全支付界面")
                 return True
             else:
                 return False
         else:
             logger.warn("当前订单详情页面: {}，不是本次要支付的订单: {} 的详情页".format(current_url, order_id))
             return False
```

### Comparing `ctrip-helper-0.2.4/ctrip_helper/api/http_api.py` & `ctrip-helper-0.2.5/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.4/ctrip_helper/config.py` & `ctrip-helper-0.2.5/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.4/ctrip_helper/http_client.py` & `ctrip-helper-0.2.5/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.4/ctrip_helper/libs.py` & `ctrip-helper-0.2.5/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.4/ctrip_helper/utils.py` & `ctrip-helper-0.2.5/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.4/setup.py` & `ctrip-helper-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.2.4',
+    version='0.2.5',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

