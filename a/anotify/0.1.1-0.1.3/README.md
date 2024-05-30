# Comparing `tmp/anotify-0.1.1.tar.gz` & `tmp/anotify-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anotify-0.1.1.tar", last modified: Thu May 30 02:27:52 2024, max compression
+gzip compressed data, was "anotify-0.1.3.tar", last modified: Thu May 30 02:49:43 2024, max compression
```

## Comparing `anotify-0.1.1.tar` & `anotify-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:27:52.559372 anotify-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:27:52.555372 anotify-0.1.1/ANotify/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Nanpush.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Ndingtalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Nemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Nfeishu.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Niyuu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Npushplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Nserverchan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Ntelegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Nwecom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-30 02:27:45.000000 anotify-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-30 02:27:52.559372 anotify-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-30 02:27:45.000000 anotify-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:27:52.559372 anotify-0.1.1/anotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-30 02:27:52.000000 anotify-0.1.1/anotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 02:27:52.000000 anotify-0.1.1/anotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 02:27:52.000000 anotify-0.1.1/anotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 02:27:52.000000 anotify-0.1.1/anotify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 02:27:52.000000 anotify-0.1.1/anotify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 02:27:52.559372 anotify-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 02:27:45.000000 anotify-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:49:43.734739 anotify-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:49:43.730739 anotify-0.1.3/ANotify/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 02:49:35.000000 anotify-0.1.3/ANotify/Nanpush.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-30 02:49:35.000000 anotify-0.1.3/ANotify/Ndingtalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-30 02:49:35.000000 anotify-0.1.3/ANotify/Nemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-30 02:49:35.000000 anotify-0.1.3/ANotify/Nfeishu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 02:49:35.000000 anotify-0.1.3/ANotify/Niyuu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-30 02:49:35.000000 anotify-0.1.3/ANotify/Npushplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-30 02:49:35.000000 anotify-0.1.3/ANotify/Nserverchan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-30 02:49:35.000000 anotify-0.1.3/ANotify/Ntelegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-05-30 02:49:35.000000 anotify-0.1.3/ANotify/Nwecom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-30 02:49:35.000000 anotify-0.1.3/ANotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-30 02:49:35.000000 anotify-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-30 02:49:43.734739 anotify-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-30 02:49:35.000000 anotify-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:49:43.734739 anotify-0.1.3/anotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-30 02:49:43.000000 anotify-0.1.3/anotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 02:49:43.000000 anotify-0.1.3/anotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 02:49:43.000000 anotify-0.1.3/anotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 02:49:43.000000 anotify-0.1.3/anotify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 02:49:43.000000 anotify-0.1.3/anotify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 02:49:43.734739 anotify-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-30 02:49:35.000000 anotify-0.1.3/setup.py
```

### Comparing `anotify-0.1.1/ANotify/Nanpush.py` & `anotify-0.1.3/ANotify/Nanpush.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.1/ANotify/Ndingtalk.py` & `anotify-0.1.3/ANotify/Ndingtalk.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.1/ANotify/Nemail.py` & `anotify-0.1.3/ANotify/Nemail.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.1/ANotify/Nfeishu.py` & `anotify-0.1.3/ANotify/Nfeishu.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.1/ANotify/Npushplus.py` & `anotify-0.1.3/ANotify/Npushplus.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.1/ANotify/Nserverchan.py` & `anotify-0.1.3/ANotify/Nserverchan.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.1/ANotify/Ntelegram.py` & `anotify-0.1.3/ANotify/Ntelegram.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.1/ANotify/Nwecom.py` & `anotify-0.1.3/ANotify/Nwecom.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,16 @@
             "enable_duplicate_check": 0,
             "duplicate_check_interval": 1800
         }
         resp = requests.post(url, data=json.dumps(payload))
         resp.raise_for_status()
         return resp.json()
 
-    # 发送 Markdown 消息
-    def send_msg_mardown(self, text):
+    # 发送 Markdown 文本消息
+    def send_msg_markdown(self, text):
         url = 'https://qyapi.weixin.qq.com/cgi-bin/message/send?access_token=' + self.access_token
         payload = {
             "touser": "@all",
             "msgtype": "markdown",
             "agentid": self.agentid,
             "text": {
                 "content": text
```

### Comparing `anotify-0.1.1/ANotify/__init__.py` & `anotify-0.1.3/ANotify/__init__.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.1/LICENSE` & `anotify-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anotify-0.1.1/PKG-INFO` & `anotify-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.1.1
-Summary: Send notifications by multiple channels.
+Version: 0.1.3
+Summary: Send notifications by multiple channels
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.1.1 Summary: Send notifications
-by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
+Metadata-Version: 2.1 Name: anotify Version: 0.1.3 Summary: Send notifications
+by multiple channels Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: requests>=2.15.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
 å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½](https://work.weixin.qq.com/)
```

### Comparing `anotify-0.1.1/README.md` & `anotify-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `anotify-0.1.1/anotify.egg-info/PKG-INFO` & `anotify-0.1.3/anotify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.1.1
-Summary: Send notifications by multiple channels.
+Version: 0.1.3
+Summary: Send notifications by multiple channels
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.1.1 Summary: Send notifications
-by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
+Metadata-Version: 2.1 Name: anotify Version: 0.1.3 Summary: Send notifications
+by multiple channels Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: requests>=2.15.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
 å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½](https://work.weixin.qq.com/)
```

### Comparing `anotify-0.1.1/setup.py` & `anotify-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='anotify',
-    version='0.1.1',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'requests>=2.15.1',
     ],
     author='7ommy',
     author_email='tommymerlin0920@gmail.com',
-    description='Send notifications by multiple channels.',
+    description='Send notifications by multiple channels',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/TommyMerlin/ANotify',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

