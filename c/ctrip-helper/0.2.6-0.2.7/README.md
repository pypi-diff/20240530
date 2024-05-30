# Comparing `tmp/ctrip-helper-0.2.6.tar.gz` & `tmp/ctrip-helper-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.2.6.tar", last modified: Thu May 30 17:56:37 2024, max compression
+gzip compressed data, was "ctrip-helper-0.2.7.tar", last modified: Thu May 30 18:17:06 2024, max compression
```

## Comparing `ctrip-helper-0.2.6.tar` & `ctrip-helper-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:56:37.479001 ctrip-helper-0.2.6/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 17:56:37.478003 ctrip-helper-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 17:56:37.466069 ctrip-helper-0.2.6/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.6/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:56:37.476009 ctrip-helper-0.2.6/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.6/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30744 2024-05-30 17:56:16.000000 ctrip-helper-0.2.6/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.6/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.6/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.6/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.6/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.6/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:56:37.477006 ctrip-helper-0.2.6/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 17:56:37.000000 ctrip-helper-0.2.6/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 17:56:37.000000 ctrip-helper-0.2.6/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:56:37.000000 ctrip-helper-0.2.6/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 17:56:37.000000 ctrip-helper-0.2.6/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 17:56:37.000000 ctrip-helper-0.2.6/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 17:56:37.479998 ctrip-helper-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 17:56:32.000000 ctrip-helper-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:17:06.315632 ctrip-helper-0.2.7/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 18:17:06.313638 ctrip-helper-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 18:17:06.299675 ctrip-helper-0.2.7/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.7/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:17:06.310660 ctrip-helper-0.2.7/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.7/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30760 2024-05-30 18:16:43.000000 ctrip-helper-0.2.7/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.7/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.7/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.7/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.7/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.7/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:17:06.312641 ctrip-helper-0.2.7/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 18:17:06.000000 ctrip-helper-0.2.7/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 18:17:06.000000 ctrip-helper-0.2.7/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 18:17:06.000000 ctrip-helper-0.2.7/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 18:17:06.000000 ctrip-helper-0.2.7/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 18:17:06.000000 ctrip-helper-0.2.7/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 18:17:06.315632 ctrip-helper-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 18:17:02.000000 ctrip-helper-0.2.7/setup.py
```

### Comparing `ctrip-helper-0.2.6/LICENSE` & `ctrip-helper-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.6/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.2.7/ctrip_helper/api/desktop_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -470,15 +470,15 @@
         else:
             return False
 
     @classmethod
     def click_wallet_immediately_payment(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         immediately_payment_button = get_element(
             driver=driver, locator=UILocatorRegx.wallet_immediately_payment.value.get("locator"),
-            regx=UILocatorRegx.use_wallet.value.get("regx"), loop=loop, sleep=sleep, **kwargs
+            regx=UILocatorRegx.wallet_immediately_payment.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if immediately_payment_button:
             immediately_payment_button.click()
             logger.info("点击钱包【立即支付】")
             return True
         else:
             return False
```

### Comparing `ctrip-helper-0.2.6/ctrip_helper/api/http_api.py` & `ctrip-helper-0.2.7/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.6/ctrip_helper/config.py` & `ctrip-helper-0.2.7/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.6/ctrip_helper/http_client.py` & `ctrip-helper-0.2.7/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.6/ctrip_helper/libs.py` & `ctrip-helper-0.2.7/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.6/ctrip_helper/utils.py` & `ctrip-helper-0.2.7/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.6/setup.py` & `ctrip-helper-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.2.6',
+    version='0.2.7',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

