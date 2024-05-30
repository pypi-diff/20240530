# Comparing `tmp/unittestreport_yami-0.1.5.tar.gz` & `tmp/unittestreport_yami-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittestreport_yami-0.1.5.tar", last modified: Wed May 29 02:38:37 2024, max compression
+gzip compressed data, was "unittestreport_yami-0.1.6.tar", last modified: Thu May 30 04:55:52 2024, max compression
```

## Comparing `unittestreport_yami-0.1.5.tar` & `unittestreport_yami-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:37.118533 unittestreport_yami-0.1.5/
--rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2111 2024-05-29 02:38:37.115537 unittestreport_yami-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-29 02:38:37.119533 unittestreport_yami-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-05-29 02:38:08.000000 unittestreport_yami-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:37.026053 unittestreport_yami-0.1.5/unittestreport_yami/
--rw-rw-rw-   0        0        0      190 2024-05-29 02:14:58.000000 unittestreport_yami-0.1.5/unittestreport_yami/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:37.098532 unittestreport_yami-0.1.5/unittestreport_yami/core/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/__init__.py
--rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/dataDriver.py
--rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/parameterized.py
--rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/reRun.py
--rw-rw-rw-   0        0        0     4996 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/resultPush.py
--rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/sendEmail.py
--rw-rw-rw-   0        0        0     7279 2024-05-29 02:23:45.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/testResult.py
--rw-rw-rw-   0        0        0    12886 2024-05-29 01:16:12.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/testRunner.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:37.111533 unittestreport_yami-0.1.5/unittestreport_yami/templates/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/__init__.py
--rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/dingtalk.md
--rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/templates.html
--rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/templates03.html
--rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/templates2.html
--rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/templates3.html
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:37.081533 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/
--rw-rw-rw-   0        0        0     2111 2024-05-29 02:38:36.000000 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      859 2024-05-29 02:38:36.000000 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 02:38:36.000000 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-29 02:38:36.000000 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-29 02:38:36.000000 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 04:55:52.597001 unittestreport_yami-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2111 2024-05-30 04:55:52.589345 unittestreport_yami-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 04:55:52.597001 unittestreport_yami-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-30 04:50:12.000000 unittestreport_yami-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 04:55:52.292919 unittestreport_yami-0.1.6/unittestreport_yami/
+-rw-rw-rw-   0        0        0      190 2024-05-29 02:14:58.000000 unittestreport_yami-0.1.6/unittestreport_yami/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 04:55:52.571700 unittestreport_yami-0.1.6/unittestreport_yami/core/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.6/unittestreport_yami/core/__init__.py
+-rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.6/unittestreport_yami/core/dataDriver.py
+-rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.6/unittestreport_yami/core/parameterized.py
+-rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.6/unittestreport_yami/core/reRun.py
+-rw-rw-rw-   0        0        0     5549 2024-05-30 04:51:21.000000 unittestreport_yami-0.1.6/unittestreport_yami/core/resultPush.py
+-rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.6/unittestreport_yami/core/sendEmail.py
+-rw-rw-rw-   0        0        0     7279 2024-05-29 02:23:45.000000 unittestreport_yami-0.1.6/unittestreport_yami/core/testResult.py
+-rw-rw-rw-   0        0        0    13575 2024-05-30 04:55:11.000000 unittestreport_yami-0.1.6/unittestreport_yami/core/testRunner.py
+drwxrwxrwx   0        0        0        0 2024-05-30 04:55:52.583226 unittestreport_yami-0.1.6/unittestreport_yami/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.6/unittestreport_yami/templates/__init__.py
+-rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.6/unittestreport_yami/templates/dingtalk.md
+-rw-rw-rw-   0        0        0      410 2024-05-30 02:31:03.000000 unittestreport_yami-0.1.6/unittestreport_yami/templates/remote_report.md
+-rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.6/unittestreport_yami/templates/templates.html
+-rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.6/unittestreport_yami/templates/templates03.html
+-rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.6/unittestreport_yami/templates/templates2.html
+-rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.6/unittestreport_yami/templates/templates3.html
+drwxrwxrwx   0        0        0        0 2024-05-30 04:55:52.506010 unittestreport_yami-0.1.6/unittestreport_yami.egg-info/
+-rw-rw-rw-   0        0        0     2111 2024-05-30 04:55:52.000000 unittestreport_yami-0.1.6/unittestreport_yami.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      906 2024-05-30 04:55:52.000000 unittestreport_yami-0.1.6/unittestreport_yami.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 04:55:52.000000 unittestreport_yami-0.1.6/unittestreport_yami.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-30 04:55:52.000000 unittestreport_yami-0.1.6/unittestreport_yami.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-30 04:55:52.000000 unittestreport_yami-0.1.6/unittestreport_yami.egg-info/top_level.txt
```

### Comparing `unittestreport_yami-0.1.5/LICENSE` & `unittestreport_yami-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/PKG-INFO` & `unittestreport_yami-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittestreport_yami
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `unittestreport_yami-0.1.5/README.md` & `unittestreport_yami-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/setup.py` & `unittestreport_yami-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name="unittestreport_yami",
-    version="0.1.5",
+    version="0.1.6",
     author="Ethan",
     author_email="ethan.liu@yamibuy.com",
     url="https://github.com/EthanLiuInyami/UnitTestReport",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["Jinja2==3.1.2", "PyYAML==5.3.1", "requests==2.32.2"],
```

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/core/dataDriver.py` & `unittestreport_yami-0.1.6/unittestreport_yami/core/dataDriver.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/core/parameterized.py` & `unittestreport_yami-0.1.6/unittestreport_yami/core/parameterized.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/core/reRun.py` & `unittestreport_yami-0.1.6/unittestreport_yami/core/reRun.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/core/resultPush.py` & `unittestreport_yami-0.1.6/unittestreport_yami/core/resultPush.py`

 * *Files 18% similar despite different names*

```diff
@@ -107,39 +107,51 @@
 
 
 class WeiXin:
     """
     Enterprise wechat group notice
     """
 
-    base_url = "https://qyapi.weixin.qq.com/cgi-bin/appchat/send?access_token="
+    base_url = "https://qyapi.weixin.qq.com/cgi-bin/message/send?debug=1&access_token="
 
     def __init__(self, access_token=None, corpid=None, corpsecret=None):
         """
         :param corpid:wechat corpid
         :param corpsecret:Applied credential key
         """
         self.corpid = corpid
         self.corpsecret = corpsecret
         if access_token:
             self.access_token = access_token
         elif corpid and corpsecret:
             self.access_token = self.get_access_token()
         else:
-            raise ValueError(
-                "access_token and [corpid, corpsecret] cannot both be empty. At least one of them must be passed in"
-            )
+            self.access_token = None
 
     def get_access_token(self):
         """get access_token"""
         url = "https://qyapi.weixin.qq.com/cgi-bin/gettoken"
         params = {"corpid": self.corpid, "corpsecret": self.corpsecret}
         result = requests.get(url=url, params=params).json()
         if result["errcode"] != 0:
             raise ValueError(result["errmsg"])
         return result["access_token"]
 
     def send_info(self, data):
         """send info"""
+        if not self.access_token:
+            raise ValueError(
+                "access_token and [corpid, corpsecret] cannot both be empty. At least one of them must be passed in"
+            )
+
         url = self.base_url + self.access_token
         response = requests.post(url=url, json=data)
         return response
+
+    def send_to_bot(self, webhook, data):
+        """
+        企业微信通过机器人发送消息通知
+        webhook: 群消息机器人webhook地址
+        data: 要发送的数据， 例如：{"msgtype": "text", "text": {"content": "hello world"}}， 详细信息请查看企业微信相关文档： https://developer.work.weixin.qq.com/document/path/99110
+        """
+        response = requests.post(url=webhook, json=data)
+        return response
```

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/core/sendEmail.py` & `unittestreport_yami-0.1.6/unittestreport_yami/core/sendEmail.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/core/testResult.py` & `unittestreport_yami-0.1.6/unittestreport_yami/core/testResult.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/core/testRunner.py` & `unittestreport_yami-0.1.6/unittestreport_yami/core/testRunner.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         suite: unittest.TestSuite,
         filename="report.html",
         report_dir="./reports",
         title="测试报告",
         tester="测试员",
         desc="测试报告",
         templates=1,
+        report_url=None,
     ):
         """
         :param suites: test suite
         :param filename: Report file name
         :param report_dir:The path to the report file
         :param title:Test suite title
         :param templates: You can specify the style template for the report by parameter value 1 or 2. Currently, there are only two templates
@@ -66,14 +67,15 @@
         self.title = title
         self.tester = tester
         self.desc = desc
         self.templates = templates
         self.report_dir = report_dir
         self.result = []
         self.starttime = time.time()
+        self.report_url = report_url
 
     def __classification_suite(self):
         suites_list = []
 
         def wrapper(suite):
             for item in suite:
                 if isinstance(item, unittest.TestCase):
@@ -186,15 +188,22 @@
             json.dump(history, f, ensure_ascii=True)
         return history
 
     def __get_notice_content(self):
         """获取通知的内容"""
         template_path = os.path.join(os.path.dirname(__file__), "../templates")
         env = Environment(loader=FileSystemLoader(template_path))
-        res_text = env.get_template("dingtalk.md").render(self.test_result)
+        if self.report_url:
+            template = env.get_template("remote_report.md")
+            report_address = f"{self.report_url}/{self.filename}"
+            report_address = report_address.replace("\\", "/")
+            self.test_result["report_address"] = report_address
+        else:
+            template = env.get_template("dingtalk.md")
+        res_text = template.render(self.test_result)
         return res_text
 
     def run(self, thread_count=1, count=0, interval=2):
         """
         The entrance to running tests
         Note: if multiple test classes share a global variable, errors may occur due to resource competition
         :param thread_count:Number of threads. default 1
@@ -331,7 +340,16 @@
             "chatid": chatid,
             "msgtype": "markdown",
             "markdown": {"content": res_text},
         }
         wx = WeiXin(access_token=access_token, corpid=corpid, corpsecret=corpsecret)
         response = wx.send_info(data=data)
         return response
+
+    def weixin_robot_notice(self, webhook):
+        res_text = self.__get_notice_content()
+        data = {
+            "msgtype": "markdown",
+            "markdown": {"content": res_text},
+        }
+        response = WeiXin().send_to_robot(webhook, data)
+        return response
```

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/templates/templates.html` & `unittestreport_yami-0.1.6/unittestreport_yami/templates/templates.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/templates/templates03.html` & `unittestreport_yami-0.1.6/unittestreport_yami/templates/templates03.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/templates/templates2.html` & `unittestreport_yami-0.1.6/unittestreport_yami/templates/templates2.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami/templates/templates3.html` & `unittestreport_yami-0.1.6/unittestreport_yami/templates/templates3.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami.egg-info/PKG-INFO` & `unittestreport_yami-0.1.6/unittestreport_yami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittestreport-yami
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `unittestreport_yami-0.1.5/unittestreport_yami.egg-info/SOURCES.txt` & `unittestreport_yami-0.1.6/unittestreport_yami.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 unittestreport_yami/core/reRun.py
 unittestreport_yami/core/resultPush.py
 unittestreport_yami/core/sendEmail.py
 unittestreport_yami/core/testResult.py
 unittestreport_yami/core/testRunner.py
 unittestreport_yami/templates/__init__.py
 unittestreport_yami/templates/dingtalk.md
+unittestreport_yami/templates/remote_report.md
 unittestreport_yami/templates/templates.html
 unittestreport_yami/templates/templates03.html
 unittestreport_yami/templates/templates2.html
 unittestreport_yami/templates/templates3.html
```

