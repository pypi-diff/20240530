# Comparing `tmp/ctrip-helper-0.1.2.tar.gz` & `tmp/ctrip-helper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.1.2.tar", last modified: Wed May 29 18:49:02 2024, max compression
+gzip compressed data, was "ctrip-helper-0.1.3.tar", last modified: Thu May 30 02:24:34 2024, max compression
```

## Comparing `ctrip-helper-0.1.2.tar` & `ctrip-helper-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 18:49:02.560474 ctrip-helper-0.1.2/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-29 18:49:02.559473 ctrip-helper-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 18:49:02.547505 ctrip-helper-0.1.2/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.2/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 18:49:02.556489 ctrip-helper-0.1.2/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.2/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    24596 2024-05-29 18:48:23.000000 ctrip-helper-0.1.2/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.2/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.1.2/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.2/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4575 2024-05-29 18:45:32.000000 ctrip-helper-0.1.2/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.2/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 18:49:02.557478 ctrip-helper-0.1.2/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-29 18:49:02.000000 ctrip-helper-0.1.2/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-29 18:49:02.000000 ctrip-helper-0.1.2/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 18:49:02.000000 ctrip-helper-0.1.2/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 18:49:02.000000 ctrip-helper-0.1.2/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 18:49:02.000000 ctrip-helper-0.1.2/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 18:49:02.560474 ctrip-helper-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-29 18:48:57.000000 ctrip-helper-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:24:34.420196 ctrip-helper-0.1.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 02:24:34.419199 ctrip-helper-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 02:24:34.405238 ctrip-helper-0.1.3/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.3/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:24:34.416208 ctrip-helper-0.1.3/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.3/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    25870 2024-05-30 02:24:05.000000 ctrip-helper-0.1.3/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.3/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.1.3/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.3/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4575 2024-05-29 18:45:32.000000 ctrip-helper-0.1.3/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.3/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:24:34.418201 ctrip-helper-0.1.3/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 02:24:34.000000 ctrip-helper-0.1.3/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 02:24:34.000000 ctrip-helper-0.1.3/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 02:24:34.000000 ctrip-helper-0.1.3/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 02:24:34.000000 ctrip-helper-0.1.3/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 02:24:34.000000 ctrip-helper-0.1.3/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 02:24:34.421193 ctrip-helper-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 02:24:30.000000 ctrip-helper-0.1.3/setup.py
```

### Comparing `ctrip-helper-0.1.2/LICENSE` & `ctrip-helper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.2/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.1.3/ctrip_helper/api/desktop_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,19 +51,45 @@
                                 "regx": '//div[@class="verify-password-box"]//div[@class="inputBox"]//div[1]'}
     yeepay2b_accout_input_box = {"locator": "xpath",
                                  "regx": '//div[@class="account-pay-main"]//input[@name="userAccount"]'}
     yeepay2b_password_input_box = {"locator": "xpath",
                                    "regx": '//div[@class="account-pay-main"]//input[@name="tradePassword"]'}
     yeepay2b_payment_next_button = {"locator": "xpath",
                                     "regx": '//div[@class="account-pay-main"]//button[@id="passPayButton"]'}
+    is_login_button = {
+        "locator": "xpath",
+        "regx": '//div[@class="tl_nfes_home_header_login_wrapper_siwkn"]//button[contains(@aria-label, "我的账户")]'
+    }
+    is_login_span = {"locator": "xpath", "regx": '//div[@class="loginbar"]//span[@class="ctrip-username"]'}
 
 
 class SeleniumApi(object):
 
     @classmethod
+    def is_login(cls, driver: webdriver, username: str, platform: str, loop: int = 1, sleep: float = 0,
+                 **kwargs) -> bool:
+        """是否已登录"""
+        is_login_button = get_element(
+            driver=driver, locator=UILocatorRegx.get("is_login_button").get("locator"),
+            regx=UILocatorRegx.get("is_login_button").get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if is_login_button:
+            logger.info("{}平台用户<{}>已登录".format(platform, username))
+            return True
+        is_login_span = get_element(
+            driver=driver, locator=UILocatorRegx.get("is_login_span").get("locator"),
+            regx=UILocatorRegx.get("is_login_span").get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if is_login_span:
+            logger.info("{}平台用户<{}>已登录".format(platform, username))
+            return True
+        else:
+            return False
+
+    @classmethod
     def open_order_query_home_with_flight(cls, driver: webdriver, sleep: float = 0) -> None:
         driver.get(url_map.get_url('order_query_home_with_flight'))
         if sleep > 0:
             time.sleep(sleep)
         logger.info("打开机票订单查询首页")
 
     @classmethod
```

### Comparing `ctrip-helper-0.1.2/ctrip_helper/api/http_api.py` & `ctrip-helper-0.1.3/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.2/ctrip_helper/config.py` & `ctrip-helper-0.1.3/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.2/ctrip_helper/http_client.py` & `ctrip-helper-0.1.3/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.2/ctrip_helper/libs.py` & `ctrip-helper-0.1.3/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.2/ctrip_helper/utils.py` & `ctrip-helper-0.1.3/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.2/setup.py` & `ctrip-helper-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.1.2',
+    version='0.1.3',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

