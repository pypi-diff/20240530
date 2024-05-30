# Comparing `tmp/ctrip-helper-0.2.2.tar.gz` & `tmp/ctrip-helper-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.2.2.tar", last modified: Thu May 30 17:09:12 2024, max compression
+gzip compressed data, was "ctrip-helper-0.2.3.tar", last modified: Thu May 30 17:14:13 2024, max compression
```

## Comparing `ctrip-helper-0.2.2.tar` & `ctrip-helper-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:09:12.686440 ctrip-helper-0.2.2/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 17:09:12.685464 ctrip-helper-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 17:09:12.670482 ctrip-helper-0.2.2/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.2/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:09:12.682450 ctrip-helper-0.2.2/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.2/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30276 2024-05-30 17:08:52.000000 ctrip-helper-0.2.2/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.2/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.2/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.2/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.2/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.2/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:09:12.684445 ctrip-helper-0.2.2/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 17:09:12.000000 ctrip-helper-0.2.2/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 17:09:12.000000 ctrip-helper-0.2.2/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:09:12.000000 ctrip-helper-0.2.2/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 17:09:12.000000 ctrip-helper-0.2.2/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 17:09:12.000000 ctrip-helper-0.2.2/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 17:09:12.687462 ctrip-helper-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 17:09:07.000000 ctrip-helper-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:14:13.036250 ctrip-helper-0.2.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 17:14:13.035248 ctrip-helper-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:14:13.021285 ctrip-helper-0.2.3/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.3/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:14:13.031258 ctrip-helper-0.2.3/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.3/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30286 2024-05-30 17:14:04.000000 ctrip-helper-0.2.3/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.3/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.3/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.3/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.3/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.3/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:14:13.033263 ctrip-helper-0.2.3/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 17:14:12.000000 ctrip-helper-0.2.3/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 17:14:12.000000 ctrip-helper-0.2.3/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:14:12.000000 ctrip-helper-0.2.3/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 17:14:12.000000 ctrip-helper-0.2.3/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 17:14:12.000000 ctrip-helper-0.2.3/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:14:13.036250 ctrip-helper-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 17:14:08.000000 ctrip-helper-0.2.3/setup.py
```

### Comparing `ctrip-helper-0.2.2/LICENSE` & `ctrip-helper-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.2/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.2.3/ctrip_helper/api/desktop_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,16 +265,16 @@
 
     @classmethod
     def click_to_payment(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         current_url = driver.current_url
         local_url = "{}?oid={}".format(url_map.get("flight_order_details"), order_id)
         if current_url.startswith(local_url) is True:
             to_payment_button = get_element(
-                driver=driver, locator=UILocatorRegx.order_price.value.get("locator"),
-                regx=UILocatorRegx.order_price.value.get("regx"), loop=loop, sleep=sleep, **kwargs
+                driver=driver, locator=UILocatorRegx.order_to_payment.value.get("locator"),
+                regx=UILocatorRegx.order_to_payment.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if to_payment_button:
                 to_payment_button.click()
                 logger.info("点击【去支付】，进入订单支付界面")
                 return True
             else:
                 return False
```

### Comparing `ctrip-helper-0.2.2/ctrip_helper/api/http_api.py` & `ctrip-helper-0.2.3/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.2/ctrip_helper/config.py` & `ctrip-helper-0.2.3/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.2/ctrip_helper/http_client.py` & `ctrip-helper-0.2.3/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.2/ctrip_helper/libs.py` & `ctrip-helper-0.2.3/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.2/ctrip_helper/utils.py` & `ctrip-helper-0.2.3/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.2/setup.py` & `ctrip-helper-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.2.2',
+    version='0.2.3',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

