# Comparing `tmp/baidu_serp_api-0.3.tar.gz` & `tmp/baidu_serp_api-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baidu_serp_api-0.3.tar", last modified: Thu May 30 03:55:42 2024, max compression
+gzip compressed data, was "baidu_serp_api-0.4.tar", last modified: Thu May 30 06:59:39 2024, max compression
```

## Comparing `baidu_serp_api-0.3.tar` & `baidu_serp_api-0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/baidu_serp_api/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/baidu_serp_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/baidu_serp_api/baidu_mobile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/baidu_serp_api/baidu_pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/baidu_serp_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/baidu_serp_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 03:55:42.000000 baidu_serp_api-0.3/baidu_serp_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 03:55:42.000000 baidu_serp_api-0.3/baidu_serp_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:55:42.000000 baidu_serp_api-0.3/baidu_serp_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 03:55:42.000000 baidu_serp_api-0.3/baidu_serp_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 03:55:42.000000 baidu_serp_api-0.3/baidu_serp_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:42.742228 baidu_serp_api-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-30 03:55:38.000000 baidu_serp_api-0.3/tests/test_baidu_serp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:59:39.087936 baidu_serp_api-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 06:59:39.083936 baidu_serp_api-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:59:39.083936 baidu_serp_api-0.4/baidu_serp_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/baidu_serp_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/baidu_serp_api/baidu_mobile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/baidu_serp_api/baidu_pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/baidu_serp_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:59:39.083936 baidu_serp_api-0.4/baidu_serp_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 06:59:39.000000 baidu_serp_api-0.4/baidu_serp_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 06:59:39.000000 baidu_serp_api-0.4/baidu_serp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:59:39.000000 baidu_serp_api-0.4/baidu_serp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 06:59:39.000000 baidu_serp_api-0.4/baidu_serp_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 06:59:39.000000 baidu_serp_api-0.4/baidu_serp_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 06:59:39.087936 baidu_serp_api-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:59:39.083936 baidu_serp_api-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/tests/test_baidu_serp_api.py
```

### Comparing `baidu_serp_api-0.3/LICENSE.txt` & `baidu_serp_api-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.3/PKG-INFO` & `baidu_serp_api-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidu-serp-api
-Version: 0.3
+Version: 0.4
 Summary: A library to extract data from Baidu SERP and output it as JSON objects
 Home-page: https://github.com/ohblue/baidu-serp-api
 Author: Ben Chen
 Author-email: chan@live.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `baidu_serp_api-0.3/README.md` & `baidu_serp_api-0.4/README.md`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.3/baidu_serp_api/baidu_mobile.py` & `baidu_serp_api-0.4/baidu_serp_api/baidu_mobile.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,27 +20,32 @@
 
             url = result.get('data-log')
             if url:
                 url = json.loads(url)['mu']
 
             description = ""
             date_time = ""
+            source = ""
 
             summary_element = result.find('div', class_=lambda x: x and 'summary-' in x)
+
             if summary_element:
                 description = clean_html_tags(summary_element.get_text().strip())
 
                 date_time_element = summary_element.find('span', class_='c-gap-right-small c-color-gray')
                 if date_time_element:
                     description = description.replace(date_time_element.get_text().strip(), '')
                     date_time = date_time_element.get_text().strip()
+            source_element = result.find('div', class_=lambda x: x and '_text_' in x)
+            if source_element:
+                source = source_element.get_text().strip()
 
             if title_element and url:
                 title_text = clean_html_tags(title_element.get_text().strip())
-                search_data.append({'title': title_text, 'url': url, 'description': description, 'date_time': date_time})
+                search_data.append({'title': title_text, 'url': url, 'description': description, 'date_time': date_time, "source": source})
 
         return search_data
 
     def get_recommend(self, keyword, qid, proxies=None):
         url = 'https://m.baidu.com/rec'
         params = {
             'word': keyword,
```

### Comparing `baidu_serp_api-0.3/baidu_serp_api/baidu_pc.py` & `baidu_serp_api-0.4/baidu_serp_api/baidu_pc.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,31 @@
         for result in search_results:
             title_element = result.select_one('h3.c-title')
 
             url = result.get('mu')
 
             description = ""
             date_time = ""
+            source = ""
 
             summary_element = result.select_one('span[class^="content-right_"]')
             if summary_element:
                 description = clean_html_tags(summary_element.get_text().strip())
 
             date_time_element = result.select_one('span.c-color-gray2')
             if date_time_element:
                 date_time = date_time_element.get_text().strip()
 
+            source_element = result.select_one('span.c-color-gray')
+            if source_element:
+                source = source_element.get_text().strip()
+
             if title_element and url:
                 title_text = clean_html_tags(title_element.get_text().strip())
-                result_data.append({"title": title_text, "url": url, "description": description, "date_time": date_time})
+                result_data.append({"title": title_text, "url": url, "description": description, "date_time": date_time, "source": source})
 
         return result_data
 
     def get_recommend(self, html_content):
         # 找出所有 s-data 注释块
         pattern = r"<!--s-data:(.*?)-->"
         matches = re.findall(pattern, html_content, re.DOTALL)
```

### Comparing `baidu_serp_api-0.3/baidu_serp_api/util.py` & `baidu_serp_api-0.4/baidu_serp_api/util.py`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.3/baidu_serp_api.egg-info/PKG-INFO` & `baidu_serp_api-0.4/baidu_serp_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidu-serp-api
-Version: 0.3
+Version: 0.4
 Summary: A library to extract data from Baidu SERP and output it as JSON objects
 Home-page: https://github.com/ohblue/baidu-serp-api
 Author: Ben Chen
 Author-email: chan@live.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `baidu_serp_api-0.3/setup.py` & `baidu_serp_api-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='baidu-serp-api',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `baidu_serp_api-0.3/tests/test_baidu_serp_api.py` & `baidu_serp_api-0.4/tests/test_baidu_serp_api.py`

 * *Files identical despite different names*

