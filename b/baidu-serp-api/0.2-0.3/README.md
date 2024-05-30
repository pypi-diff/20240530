# Comparing `tmp/baidu_serp_api-0.2.tar.gz` & `tmp/baidu_serp_api-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baidu_serp_api-0.2.tar", last modified: Thu May 30 03:27:42 2024, max compression
+gzip compressed data, was "baidu_serp_api-0.3.tar", last modified: Thu May 30 03:55:42 2024, max compression
```

## Comparing `baidu_serp_api-0.2.tar` & `baidu_serp_api-0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:27:42.824005 baidu_serp_api-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 03:27:42.824005 baidu_serp_api-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:27:42.820004 baidu_serp_api-0.2/baidu_serp_api/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/baidu_serp_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/baidu_serp_api/baidu_mobile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/baidu_serp_api/baidu_pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/baidu_serp_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:27:42.824005 baidu_serp_api-0.2/baidu_serp_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 03:27:42.000000 baidu_serp_api-0.2/baidu_serp_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 03:27:42.000000 baidu_serp_api-0.2/baidu_serp_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:27:42.000000 baidu_serp_api-0.2/baidu_serp_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 03:27:42.000000 baidu_serp_api-0.2/baidu_serp_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 03:27:42.000000 baidu_serp_api-0.2/baidu_serp_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:27:42.824005 baidu_serp_api-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:27:42.824005 baidu_serp_api-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/tests/test_baidu_serp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/baidu_serp_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/baidu_serp_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/baidu_serp_api/baidu_mobile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/baidu_serp_api/baidu_pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/baidu_serp_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/baidu_serp_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 03:55:42.000000 baidu_serp_api-0.3/baidu_serp_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 03:55:42.000000 baidu_serp_api-0.3/baidu_serp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:55:42.000000 baidu_serp_api-0.3/baidu_serp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 03:55:42.000000 baidu_serp_api-0.3/baidu_serp_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 03:55:42.000000 baidu_serp_api-0.3/baidu_serp_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/tests/test_baidu_serp_api.py
```

### Comparing `baidu_serp_api-0.2/LICENSE.txt` & `baidu_serp_api-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.2/PKG-INFO` & `baidu_serp_api-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidu-serp-api
-Version: 0.2
+Version: 0.3
 Summary: A library to extract data from Baidu SERP and output it as JSON objects
 Home-page: https://github.com/ohblue/baidu-serp-api
 Author: Ben Chen
 Author-email: chan@live.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `baidu_serp_api-0.2/README.md` & `baidu_serp_api-0.3/README.md`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.2/baidu_serp_api/baidu_mobile.py` & `baidu_serp_api-0.3/baidu_serp_api/baidu_mobile.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             url = result.get('data-log')
             if url:
                 url = json.loads(url)['mu']
 
             description = ""
             date_time = ""
 
-            summary_element = result.find('div', {'data-module': 'summary'})
+            summary_element = result.find('div', class_=lambda x: x and 'summary-' in x)
             if summary_element:
                 description = clean_html_tags(summary_element.get_text().strip())
 
                 date_time_element = summary_element.find('span', class_='c-gap-right-small c-color-gray')
                 if date_time_element:
                     description = description.replace(date_time_element.get_text().strip(), '')
                     date_time = date_time_element.get_text().strip()
```

### Comparing `baidu_serp_api-0.2/baidu_serp_api/baidu_pc.py` & `baidu_serp_api-0.3/baidu_serp_api/baidu_pc.py`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.2/baidu_serp_api/util.py` & `baidu_serp_api-0.3/baidu_serp_api/util.py`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.2/baidu_serp_api.egg-info/PKG-INFO` & `baidu_serp_api-0.3/baidu_serp_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidu-serp-api
-Version: 0.2
+Version: 0.3
 Summary: A library to extract data from Baidu SERP and output it as JSON objects
 Home-page: https://github.com/ohblue/baidu-serp-api
 Author: Ben Chen
 Author-email: chan@live.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `baidu_serp_api-0.2/setup.py` & `baidu_serp_api-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='baidu-serp-api',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `baidu_serp_api-0.2/tests/test_baidu_serp_api.py` & `baidu_serp_api-0.3/tests/test_baidu_serp_api.py`

 * *Files identical despite different names*

