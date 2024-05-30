# Comparing `tmp/baidu_serp_api-0.1.tar.gz` & `tmp/baidu_serp_api-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baidu_serp_api-0.1.tar", last modified: Fri May 24 06:37:28 2024, max compression
+gzip compressed data, was "baidu_serp_api-0.2.tar", last modified: Thu May 30 03:27:42 2024, max compression
```

## Comparing `baidu_serp_api-0.1.tar` & `baidu_serp_api-0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:37:28.053629 baidu_serp_api-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-24 06:37:28.053629 baidu_serp_api-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-24 06:37:22.000000 baidu_serp_api-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:37:28.053629 baidu_serp_api-0.1/baidu_serp_api/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-24 06:37:22.000000 baidu_serp_api-0.1/baidu_serp_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-24 06:37:22.000000 baidu_serp_api-0.1/baidu_serp_api/baidu_mobile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-24 06:37:22.000000 baidu_serp_api-0.1/baidu_serp_api/baidu_pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-24 06:37:22.000000 baidu_serp_api-0.1/baidu_serp_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:37:28.053629 baidu_serp_api-0.1/baidu_serp_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-24 06:37:28.000000 baidu_serp_api-0.1/baidu_serp_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-24 06:37:28.000000 baidu_serp_api-0.1/baidu_serp_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 06:37:28.000000 baidu_serp_api-0.1/baidu_serp_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 06:37:28.000000 baidu_serp_api-0.1/baidu_serp_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 06:37:28.000000 baidu_serp_api-0.1/baidu_serp_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 06:37:28.053629 baidu_serp_api-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-24 06:37:22.000000 baidu_serp_api-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:37:28.053629 baidu_serp_api-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 06:37:22.000000 baidu_serp_api-0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-24 06:37:22.000000 baidu_serp_api-0.1/tests/test_baidu_serp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:27:42.824005 baidu_serp_api-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 03:27:42.824005 baidu_serp_api-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:27:42.820004 baidu_serp_api-0.2/baidu_serp_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/baidu_serp_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/baidu_serp_api/baidu_mobile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/baidu_serp_api/baidu_pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/baidu_serp_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:27:42.824005 baidu_serp_api-0.2/baidu_serp_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 03:27:42.000000 baidu_serp_api-0.2/baidu_serp_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 03:27:42.000000 baidu_serp_api-0.2/baidu_serp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:27:42.000000 baidu_serp_api-0.2/baidu_serp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 03:27:42.000000 baidu_serp_api-0.2/baidu_serp_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 03:27:42.000000 baidu_serp_api-0.2/baidu_serp_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:27:42.824005 baidu_serp_api-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:27:42.824005 baidu_serp_api-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-30 03:27:30.000000 baidu_serp_api-0.2/tests/test_baidu_serp_api.py
```

### Comparing `baidu_serp_api-0.1/PKG-INFO` & `baidu_serp_api-0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: baidu-serp-api
-Version: 0.1
-Summary: A library to extract data from Baidu SERP and output it as JSON objects
-Home-page: https://github.com/ohblue/baidu-serp-api
-Author: Ben Chen
-Author-email: chan@live.cn
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: beautifulsoup4
-
 [English](#baidu-serp-api) | [中文](#百度SERP-API)
 
 # Baidu SERP API
 
 A Python library to extract data from Baidu Search Engine Results Pages (SERP) and output it as JSON objects.
 
 ## Installation
@@ -44,22 +29,25 @@
 - `keyword`: The search keyword.
 - `date_range` (optional): Search for results within the specified date range. the format should be a time range string like `'20240501,20240531'`, representing searching results between May 1, 2024, and May 31, 2024. 
 - `pn` (optional): Search for results on the specified page.
 - `proxies` (optional): Use proxies for searching.
 
 ### Return Values
 
-- `{'code': 40001, 'msg': '百度安全验证'}`: Baidu security verification required.
-- `{'code': 40002, 'msg': '未找到相关结果'}`: No relevant results found.
-- `{'code': 40003, 'msg': '疑似违禁词'}`: Suspected prohibited word.
-- `{'code': 20000, 'msg': 'ok', 'data': {'results': [], 'recommend': [], last_page': True}}`: Successful response. 
+- `{'code': 500, 'msg': '网络请求错误'}`: Network request exception.
+- `{'code': 501, 'msg': '百度安全验证'}`: Baidu security verification required.
+- `{'code': 404, 'msg': '未找到相关结果'}`: No relevant results found.
+- `{'code': 403, 'msg': '疑似违禁词'}`: Suspected prohibited word.
+- `{'code': 200, 'msg': 'ok', 'data': {'results': [], 'recommend': [], last_page': True}}`: Successful response. 
     - `results` search results list.
     - `recommend` recommend keywords.
     - `last_page` indicates whether it's the last page.
 
+### Disclaimer
+This project is intended for educational purposes only and must not be used for commercial purposes or for large-scale scraping of Baidu data. This project is licensed under the GPLv3 open-source license. If other projects utilize the content of this project, they must be open-sourced and acknowledge the source. Additionally, the author of this project shall not be held responsible for any legal risks resulting from misuse. Violators will bear the consequences at their own risk.
 
 
 
 # 百度SERP API
 
 一个用于从百度搜索结果页面（SERP）提取数据并将其输出为JSON对象的Python库。
 
@@ -75,27 +63,32 @@
 from baidu_serp_api import BaiduPc, BaiduMobile
 
 pc_serp = BaiduPc()
 results = pc_serp.search('关键词', date_range='20240501,20240531', pn='2', proxies={'http': 'http://你的代理服务器:端口'})
 print(results)
 
 m_serp = BaiduMobile()
-results = m_serp.search('关键词', date_range='day', pn='2', proxies={'http': 'http://你的代理服务器:端口'})
+results = m_serp.search('关键词', date_range='20240501,20240531', pn='2', proxies={'http': 'http://你的代理服务器:端口'})
 print(results)
 ```
 
 ### 参数
 
 - `keyword`: 搜索关键词。
 - `date_range` (可选): 在指定日期范围内搜索结果。格式应为一个时间范围字符串，如 `'20240501,20240531'`，表示搜索2024年5月1日至2024年5月31日之间的结果。
 - `pn` (可选): 搜索指定页码的结果。
 - `proxies` (可选): 使用代理进行搜索。
 
 ### 返回值
 
-- `{'code': 40001, 'msg': '百度安全验证'}`: 需要进行百度安全验证。
-- `{'code': 40002, 'msg': '未找到相关结果'}`: 未找到相关结果。
-- `{'code': 40003, 'msg': '疑似违禁词'}`: 疑似违禁词。
-- `{'code': 20000, 'msg': 'ok', 'data': {'results': [], 'last_page': True}}`: 成功响应。
+- `{'code': 500, 'msg': '网络请求错误'}`: 网络请求失败需要重试。
+- `{'code': 502, 'msg': '百度安全验证'}`: 需要进行百度安全验证。
+- `{'code': 404, 'msg': '未找到相关结果'}`: 未找到相关结果。
+- `{'code': 403, 'msg': '疑似违禁词'}`: 疑似违禁词。
+- `{'code': 200, 'msg': 'ok', 'data': {'results': [], 'last_page': True}}`: 成功响应。
     - `results` 搜索结果列表。
     - `recommend` 推荐相关搜索词。
     - `last_page` 表示是否为最后一页。
+
+### 免责声明
+
+本项目仅供学习之用，不可用于商业目的或大规模爬取百度数据。本项目采用GPLv3开源许可，若涉及到其他项目使用本项目内容，需开源并注明来源。同时，本项目作者不对滥用行为可能导致的法律风险承担责任，违者自负后果。
```

### Comparing `baidu_serp_api-0.1/baidu_serp_api/baidu_mobile.py` & `baidu_serp_api-0.2/baidu_serp_api/baidu_mobile.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from bs4 import BeautifulSoup
 import json
 from datetime import datetime
 from .util import gen_random_params, clean_html_tags, logger
 
 class BaiduMobile:
     
-    random_params = gen_random_params()
-    recomment_list = []
+    def __init__(self):
+        self.random_params = gen_random_params()
+        self.keyword = None
+        self.recomment_list = []
 
     def extract_baidum_data(self, html_content):
         search_data = []
         soup = BeautifulSoup(html_content, 'html.parser')
         search_results = soup.find_all(class_='c-result result')
         for result in search_results:
             title_element = result.find('p', class_='cu-title')
@@ -72,15 +74,15 @@
                 down_values.extend(item['down'])
 
             # 排重并合并为新的列表
             recomment_list = list(set(up_values + down_values))
             logger.debug(len(recomment_list))
             return recomment_list
         except requests.exceptions.RequestException as e:
-            return {'code': 40000, 'msg': '网络请求错误'}
+            return {'code': 500, 'msg': '网络请求错误'}
 
     def get_baidum_serp(self, keyword, date_range=None, pn=None, proxies=None):
         url = 'https://m.baidu.com/s'
         params = {
             'word': keyword
         }
         if date_range:
@@ -108,25 +110,23 @@
         except requests.exceptions.RequestException as e:
             logger.error(f'{keyword}相关搜索词获取失败')
             return []
 
     def handle_response(self, response):
         if isinstance(response, str):
             if '百度安全验证' in response:
-                return {'code': 40001, 'msg': '百度安全验证'}
+                return {'code': 501, 'msg': '百度安全验证'}
             elif '未找到相关结果' in response:
-                return {'code': 40002, 'msg': '未找到相关结果'}
+                return {'code': 404, 'msg': '未找到相关结果'}
             else:
                 soup = BeautifulSoup(response, 'html.parser')
                 if not soup.find('p', class_='cu-title'):
-                    with open('tmp.html', 'w') as f:
-                        f.write(response)
-                    return {'code': 40003, 'msg': '疑似违禁词'}
+                    return {'code': 403, 'msg': '疑似违禁词'}
                 search_results = self.extract_baidum_data(response)
                 last_page = 'new-nextpage' not in response
-                return {'code': 20000, 'msg': 'ok', 'data': {'results': search_results, 'recomment': self.recomment_list, 'last_page': last_page}}
+                return {'code': 200, 'msg': 'ok', 'data': {'results': search_results, 'recomment': self.recomment_list, 'last_page': last_page}}
         else:
             return response
 
     def search(self, keyword, date_range=None, pn=None, proxies=None):
         html_content = self.get_baidum_serp(keyword, date_range, pn, proxies)
         return self.handle_response(html_content)
```

### Comparing `baidu_serp_api-0.1/baidu_serp_api/baidu_pc.py` & `baidu_serp_api-0.2/baidu_serp_api/baidu_pc.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from urllib.parse import quote
 from datetime import datetime
 from .util import gen_random_params, clean_html_tags, logger
 import re
 
 class BaiduPc:
 
-    random_params = gen_random_params()
+    def __init__(self):
+        self.random_params = gen_random_params()
+        self.keyword = None
 
     def extract_baidupc_data(self, html_content):
         soup = BeautifulSoup(html_content, 'html.parser')
         search_results = soup.select('div[tpl="se_com_default"]')
         result_data = []
         for result in search_results:
             title_element = result.select_one('h3.c-title')
@@ -134,28 +136,29 @@
         try:
             response = requests.get(url, headers=headers, params=params, proxies=proxies, timeout=10, allow_redirects=False)
             # logger.debug(response.url)
             response.raise_for_status()
             response.encoding = 'utf-8'
             return response.text
         except requests.exceptions.RequestException as e:
-            return {'code': 40000, 'msg': '网络请求失败'}
+            return {'code': 500, 'msg': '网络请求失败'}
 
     def handle_response(self, response):
         if isinstance(response, str):
             if '百度安全验证' in response or response.strip() == '':
-                return {'code': 40001, 'msg': '百度安全验证'}
+                return {'code': 501, 'msg': '百度安全验证'}
             elif '未找到相关结果' in response:
-                return {'code': 40002, 'msg': '未找到相关结果'}
-            # elif '相关搜索' not in response:
-            #     return {'code': 40003, 'msg': '疑似违禁词'}
+                return {'code': 404, 'msg': '未找到相关结果'}
+            elif '相关搜索' not in response and 'site:' not in self.keyword:
+                return {'code': 403, 'msg': '疑似违禁词'}
             else:
                 search_results = self.extract_baidupc_data(response)
                 recomment_list = self.get_recommend(response)
                 last_page = '下一页' not in response
-                return {'code': 20000, 'msg': 'ok', 'data': {'results': search_results, 'recommend':recomment_list, 'last_page': last_page}}
+                return {'code': 200, 'msg': 'ok', 'data': {'results': search_results, 'recommend':recomment_list, 'last_page': last_page}}
         else:
             return response
 
     def search(self, keyword, date_range=None, pn=None, proxies=None):
+        self.keyword = keyword
         html_content = self.get_baidupc_serp(keyword, date_range, pn, proxies)
         return self.handle_response(html_content)
```

### Comparing `baidu_serp_api-0.1/baidu_serp_api/util.py` & `baidu_serp_api-0.2/baidu_serp_api/util.py`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.1/tests/test_baidu_serp_api.py` & `baidu_serp_api-0.2/tests/test_baidu_serp_api.py`

 * *Files identical despite different names*

