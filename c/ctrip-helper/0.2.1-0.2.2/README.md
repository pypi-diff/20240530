# Comparing `tmp/ctrip-helper-0.2.1.tar.gz` & `tmp/ctrip-helper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.2.1.tar", last modified: Thu May 30 16:54:08 2024, max compression
+gzip compressed data, was "ctrip-helper-0.2.2.tar", last modified: Thu May 30 17:09:12 2024, max compression
```

## Comparing `ctrip-helper-0.2.1.tar` & `ctrip-helper-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 16:54:08.212754 ctrip-helper-0.2.1/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 16:54:08.210761 ctrip-helper-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 16:54:08.193806 ctrip-helper-0.2.1/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.1/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:54:08.206771 ctrip-helper-0.2.1/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.1/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30232 2024-05-30 10:16:18.000000 ctrip-helper-0.2.1/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.1/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.1/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.1/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.1/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.1/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:54:08.208765 ctrip-helper-0.2.1/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 16:54:08.000000 ctrip-helper-0.2.1/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 16:54:08.000000 ctrip-helper-0.2.1/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 16:54:08.000000 ctrip-helper-0.2.1/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 16:54:08.000000 ctrip-helper-0.2.1/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 16:54:08.000000 ctrip-helper-0.2.1/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 16:54:08.212754 ctrip-helper-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 16:54:03.000000 ctrip-helper-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:09:12.686440 ctrip-helper-0.2.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 17:09:12.685464 ctrip-helper-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:09:12.670482 ctrip-helper-0.2.2/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.2/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:09:12.682450 ctrip-helper-0.2.2/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.2/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30276 2024-05-30 17:08:52.000000 ctrip-helper-0.2.2/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.2/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.2/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.2/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.2/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.2/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:09:12.684445 ctrip-helper-0.2.2/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 17:09:12.000000 ctrip-helper-0.2.2/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 17:09:12.000000 ctrip-helper-0.2.2/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:09:12.000000 ctrip-helper-0.2.2/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 17:09:12.000000 ctrip-helper-0.2.2/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 17:09:12.000000 ctrip-helper-0.2.2/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:09:12.687462 ctrip-helper-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 17:09:07.000000 ctrip-helper-0.2.2/setup.py
```

### Comparing `ctrip-helper-0.2.1/LICENSE` & `ctrip-helper-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.1/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.2.2/ctrip_helper/api/desktop_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,17 +411,18 @@
                 if is_later is False:
                     flag = True
                     remark = "支付时间少于{}分钟".format(minutes)
                     logger.warning(remark)
                     return flag, remark
             else:
                 remark = "从文案<{}>中没有获取订单过期时间".format(sub_title_text)
+                logger.warning(remark)
         else:
             remark = "从订单详情页面中未找到订单过期时间元素"
-        logger.warning(remark)
+            logger.warning(remark)
         return flag, remark
 
     @classmethod
     def is_wallet_disable(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         wallet_disable_element = get_element(
             driver=driver, locator=UILocatorRegx.wallet_disable.value.get("locator"),
             regx=UILocatorRegx.wallet_disable.value.get("regx"), loop=loop, sleep=sleep, **kwargs
```

### Comparing `ctrip-helper-0.2.1/ctrip_helper/api/http_api.py` & `ctrip-helper-0.2.2/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.1/ctrip_helper/config.py` & `ctrip-helper-0.2.2/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.1/ctrip_helper/http_client.py` & `ctrip-helper-0.2.2/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.1/ctrip_helper/libs.py` & `ctrip-helper-0.2.2/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.1/ctrip_helper/utils.py` & `ctrip-helper-0.2.2/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.1/setup.py` & `ctrip-helper-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.2.1',
+    version='0.2.2',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

