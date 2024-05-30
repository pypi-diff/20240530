# Comparing `tmp/ctrip-helper-0.1.6.tar.gz` & `tmp/ctrip-helper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.1.6.tar", last modified: Thu May 30 05:29:06 2024, max compression
+gzip compressed data, was "ctrip-helper-0.1.7.tar", last modified: Thu May 30 07:10:13 2024, max compression
```

## Comparing `ctrip-helper-0.1.6.tar` & `ctrip-helper-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 05:29:06.890752 ctrip-helper-0.1.6/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 05:29:06.889755 ctrip-helper-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 05:29:06.874797 ctrip-helper-0.1.6/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.6/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 05:29:06.886763 ctrip-helper-0.1.6/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.6/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30297 2024-05-30 05:28:53.000000 ctrip-helper-0.1.6/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.6/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.1.6/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.6/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4575 2024-05-29 18:45:32.000000 ctrip-helper-0.1.6/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.6/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 05:29:06.887760 ctrip-helper-0.1.6/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 05:29:06.000000 ctrip-helper-0.1.6/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 05:29:06.000000 ctrip-helper-0.1.6/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 05:29:06.000000 ctrip-helper-0.1.6/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 05:29:06.000000 ctrip-helper-0.1.6/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 05:29:06.000000 ctrip-helper-0.1.6/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 05:29:06.890752 ctrip-helper-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 05:29:00.000000 ctrip-helper-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:10:13.091901 ctrip-helper-0.1.7/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 07:10:13.090904 ctrip-helper-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 07:10:13.076940 ctrip-helper-0.1.7/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.7/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:10:13.087912 ctrip-helper-0.1.7/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.7/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30297 2024-05-30 05:28:53.000000 ctrip-helper-0.1.7/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.7/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.1.7/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.7/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4805 2024-05-30 07:06:35.000000 ctrip-helper-0.1.7/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.7/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:10:13.089906 ctrip-helper-0.1.7/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 07:10:12.000000 ctrip-helper-0.1.7/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 07:10:12.000000 ctrip-helper-0.1.7/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:10:12.000000 ctrip-helper-0.1.7/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 07:10:12.000000 ctrip-helper-0.1.7/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 07:10:12.000000 ctrip-helper-0.1.7/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:10:13.091901 ctrip-helper-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 07:07:02.000000 ctrip-helper-0.1.7/setup.py
```

### Comparing `ctrip-helper-0.1.6/LICENSE` & `ctrip-helper-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.6/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.1.7/ctrip_helper/api/desktop_ui.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.6/ctrip_helper/api/http_api.py` & `ctrip-helper-0.1.7/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.6/ctrip_helper/config.py` & `ctrip-helper-0.1.7/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.6/ctrip_helper/http_client.py` & `ctrip-helper-0.1.7/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.6/ctrip_helper/libs.py` & `ctrip-helper-0.1.7/ctrip_helper/libs.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,32 +21,34 @@
 logger = logging.getLogger("root")
 
 
 class EnumMetaClass(Enum):
 
     @classmethod
     def values(cls) -> list:
-        return [x.value for x in cls]
+        return [x.value[0] if isinstance(x.value, tuple) else x.value for x in cls]
 
     @classmethod
     def keys(cls) -> list:
         return [x.name for x in cls]
 
     @classmethod
     def get(cls, key: str) -> t.Any:
         if key.upper() in cls.keys():
-            return getattr(cls, key.upper()).value
+            value = getattr(cls, key.upper()).value
+            return value[0] if isinstance(value, tuple) else value
         elif key.lower() in cls.keys():
-            return getattr(cls, key.lower()).value
+            value = getattr(cls, key.upper()).value
+            return value[0] if isinstance(value, tuple) else value
         else:
             return None
 
     @classmethod
     def items(cls) -> t.List:
-        return [(x.name, x.value) for x in cls]
+        return [(x.name, x.value[0] if isinstance(x.value, tuple) else x.value) for x in cls]
 
 
 class Locator(EnumMetaClass):
     id = By.ID
     name = By.NAME
     xpath = By.XPATH
     tag_name = By.TAG_NAME
```

### Comparing `ctrip-helper-0.1.6/ctrip_helper/utils.py` & `ctrip-helper-0.1.7/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.6/setup.py` & `ctrip-helper-0.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.1.6',
+    version='0.1.7',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

