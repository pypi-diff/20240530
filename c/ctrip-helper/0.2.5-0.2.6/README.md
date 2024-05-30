# Comparing `tmp/ctrip-helper-0.2.5.tar.gz` & `tmp/ctrip-helper-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.2.5.tar", last modified: Thu May 30 17:30:41 2024, max compression
+gzip compressed data, was "ctrip-helper-0.2.6.tar", last modified: Thu May 30 17:56:37 2024, max compression
```

## Comparing `ctrip-helper-0.2.5.tar` & `ctrip-helper-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:30:41.943812 ctrip-helper-0.2.5/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 17:30:41.942815 ctrip-helper-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 17:30:41.927864 ctrip-helper-0.2.5/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.5/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:30:41.939822 ctrip-helper-0.2.5/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.5/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30280 2024-05-30 17:30:24.000000 ctrip-helper-0.2.5/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.5/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.5/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.5/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.5/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.5/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:30:41.941817 ctrip-helper-0.2.5/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 17:30:41.000000 ctrip-helper-0.2.5/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 17:30:41.000000 ctrip-helper-0.2.5/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:30:41.000000 ctrip-helper-0.2.5/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 17:30:41.000000 ctrip-helper-0.2.5/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 17:30:41.000000 ctrip-helper-0.2.5/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 17:30:41.943812 ctrip-helper-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 17:30:36.000000 ctrip-helper-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:56:37.479001 ctrip-helper-0.2.6/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 17:56:37.478003 ctrip-helper-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:56:37.466069 ctrip-helper-0.2.6/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.6/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:56:37.476009 ctrip-helper-0.2.6/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.6/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30744 2024-05-30 17:56:16.000000 ctrip-helper-0.2.6/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.6/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.6/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.6/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.6/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.6/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:56:37.477006 ctrip-helper-0.2.6/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 17:56:37.000000 ctrip-helper-0.2.6/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 17:56:37.000000 ctrip-helper-0.2.6/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:56:37.000000 ctrip-helper-0.2.6/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 17:56:37.000000 ctrip-helper-0.2.6/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 17:56:37.000000 ctrip-helper-0.2.6/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:56:37.479998 ctrip-helper-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 17:56:32.000000 ctrip-helper-0.2.6/setup.py
```

### Comparing `ctrip-helper-0.2.5/LICENSE` & `ctrip-helper-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.5/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.2.6/ctrip_helper/api/desktop_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,19 +322,30 @@
         )
         if got_it_button:
             return True
         else:
             return False
 
     @classmethod
+    def get_safe_payment_home_page(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> tuple:
+        current_url = ""
+        for _ in range(loop):
+            current_url = driver.current_url
+            if current_url.startswith(url_map.get("safe_payment_home")) is True:
+                return True, current_url
+            if sleep > 0:
+                time.sleep(sleep)
+        return False, current_url
+
+    @classmethod
     def get_order_amount_with_safe_payment_home(cls, driver: webdriver, loop: int = 1, sleep: float = 0,
                                                 **kwargs) -> Decimal:
         order_payment_amount = "0.00"
-        current_url = driver.current_url
-        if current_url.startswith(url_map.get("safe_payment_home")) is True:
+        is_success, current_url = cls.get_safe_payment_home_page(driver=driver, loop=loop, sleep=sleep)
+        if is_success is True:
             order_payment_amount_element = get_element(
                 driver=driver, locator=UILocatorRegx.order_payment_amount.value.get("locator"),
                 regx=UILocatorRegx.order_payment_amount.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if order_payment_amount_element:
                 order_payment_amount = order_payment_amount_element.text.strip()
                 logger.info("获取订单的支付金额为：{}".format(order_payment_amount))
```

### Comparing `ctrip-helper-0.2.5/ctrip_helper/api/http_api.py` & `ctrip-helper-0.2.6/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.5/ctrip_helper/config.py` & `ctrip-helper-0.2.6/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.5/ctrip_helper/http_client.py` & `ctrip-helper-0.2.6/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.5/ctrip_helper/libs.py` & `ctrip-helper-0.2.6/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.5/ctrip_helper/utils.py` & `ctrip-helper-0.2.6/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.5/setup.py` & `ctrip-helper-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.2.5',
+    version='0.2.6',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

