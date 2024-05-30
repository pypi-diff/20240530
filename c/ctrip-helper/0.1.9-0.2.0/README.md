# Comparing `tmp/ctrip-helper-0.1.9.tar.gz` & `tmp/ctrip-helper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.1.9.tar", last modified: Thu May 30 10:17:59 2024, max compression
+gzip compressed data, was "ctrip-helper-0.2.0.tar", last modified: Thu May 30 10:28:37 2024, max compression
```

## Comparing `ctrip-helper-0.1.9.tar` & `ctrip-helper-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 10:17:59.884139 ctrip-helper-0.1.9/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 10:17:59.883142 ctrip-helper-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 10:17:59.867185 ctrip-helper-0.1.9/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.9/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:17:59.880150 ctrip-helper-0.1.9/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.9/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30232 2024-05-30 10:16:18.000000 ctrip-helper-0.1.9/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.9/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.1.9/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.9/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4575 2024-05-30 10:17:44.000000 ctrip-helper-0.1.9/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.9/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:17:59.882145 ctrip-helper-0.1.9/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 10:17:59.000000 ctrip-helper-0.1.9/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 10:17:59.000000 ctrip-helper-0.1.9/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 10:17:59.000000 ctrip-helper-0.1.9/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 10:17:59.000000 ctrip-helper-0.1.9/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 10:17:59.000000 ctrip-helper-0.1.9/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 10:17:59.884139 ctrip-helper-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 10:17:53.000000 ctrip-helper-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:28:37.305697 ctrip-helper-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 10:28:37.304700 ctrip-helper-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 10:28:37.288744 ctrip-helper-0.2.0/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.0/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:28:37.301707 ctrip-helper-0.2.0/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.0/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30232 2024-05-30 10:16:18.000000 ctrip-helper-0.2.0/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.0/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.0/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.0/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4682 2024-05-30 10:28:17.000000 ctrip-helper-0.2.0/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.0/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:28:37.302705 ctrip-helper-0.2.0/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 10:28:37.000000 ctrip-helper-0.2.0/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 10:28:37.000000 ctrip-helper-0.2.0/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 10:28:37.000000 ctrip-helper-0.2.0/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 10:28:37.000000 ctrip-helper-0.2.0/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 10:28:37.000000 ctrip-helper-0.2.0/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 10:28:37.305697 ctrip-helper-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 10:28:31.000000 ctrip-helper-0.2.0/setup.py
```

### Comparing `ctrip-helper-0.1.9/LICENSE` & `ctrip-helper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.9/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.2.0/ctrip_helper/api/desktop_ui.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.9/ctrip_helper/api/http_api.py` & `ctrip-helper-0.2.0/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.9/ctrip_helper/config.py` & `ctrip-helper-0.2.0/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.9/ctrip_helper/http_client.py` & `ctrip-helper-0.2.0/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.9/ctrip_helper/libs.py` & `ctrip-helper-0.2.0/ctrip_helper/libs.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,32 +41,33 @@
             return None
 
     @classmethod
     def items(cls) -> t.List:
         return [(x.name, x.value) for x in cls]
 
 
-class Locator(EnumMetaClass):
+class Locator(Enum):
     id = By.ID
     name = By.NAME
     xpath = By.XPATH
     tag_name = By.TAG_NAME
     link_text = By.LINK_TEXT
     class_name = By.CLASS_NAME
     css_selector = By.CSS_SELECTOR
     partial_link_text = By.PARTIAL_LINK_TEXT
 
 
 def is_exist_element(driver: webdriver, locator: str, regx: str, loop: int, sleep: float,
                      is_ignore: bool = True, is_log_output: bool = True) -> bool:
     is_exist = False
+    locator = getattr(getattr(Locator, locator, object), "value", "")
     for i in range(loop):
         try:
             # 根据实际情况定位按钮元素
-            element = driver.find_element(Locator.get(locator), regx)
+            element = driver.find_element(locator, regx)
             if element:
                 is_exist = True
                 break
         except (NoSuchElementException,):
             if is_log_output is True:
                 logger.error("Element Not Found")
             if is_ignore is False:
@@ -91,18 +92,19 @@
     return is_exist
 
 
 def get_element(driver: webdriver, locator: str, regx: str, loop: int, sleep: float, **kwargs) -> WebElement:
     element = None
     is_ignore = kwargs.get("is_ignore", True)
     is_log_output = kwargs.get("is_log_output", True)
+    locator = getattr(getattr(Locator, locator, object), "value", "")
     for i in range(loop):
         try:
             # 根据实际情况定位按钮元素
-            element = driver.find_element(Locator.get(locator), regx)
+            element = driver.find_element(locator, regx)
             if element:
                 return element
         except (NoSuchElementException,):
             if is_log_output is True:
                 logger.error("Element Not Found")
             if is_ignore is False:
                 raise NoSuchElementException()
```

### Comparing `ctrip-helper-0.1.9/ctrip_helper/utils.py` & `ctrip-helper-0.2.0/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.9/setup.py` & `ctrip-helper-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.1.9',
+    version='0.2.0',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

