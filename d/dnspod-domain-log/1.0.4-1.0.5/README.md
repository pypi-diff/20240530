# Comparing `tmp/dnspod_domain_log-1.0.4.tar.gz` & `tmp/dnspod_domain_log-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dnspod_domain_log-1.0.4.tar", last modified: Mon Mar  4 03:41:42 2024, max compression
+gzip compressed data, was "dist/dnspod_domain_log-1.0.5.tar", last modified: Thu May 30 02:25:10 2024, max compression
```

## Comparing `dnspod_domain_log-1.0.4.tar` & `dnspod_domain_log-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:41:42.434146 dnspod_domain_log-1.0.4/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1339 2024-03-04 03:41:42.433515 dnspod_domain_log-1.0.4/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      340 2024-03-01 06:24:28.000000 dnspod_domain_log-1.0.4/README.rst
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:41:42.430113 dnspod_domain_log-1.0.4/dnspod_domain_log/
--rw-r--r--   0 xiaofeng   (502) staff       (20)      124 2024-03-01 06:45:32.000000 dnspod_domain_log-1.0.4/dnspod_domain_log/__init__.py
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1275 2024-03-01 06:24:28.000000 dnspod_domain_log-1.0.4/dnspod_domain_log/check_domain_log.py
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:41:42.432832 dnspod_domain_log-1.0.4/dnspod_domain_log.egg-info/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1339 2024-03-04 03:41:42.000000 dnspod_domain_log-1.0.4/dnspod_domain_log.egg-info/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      291 2024-03-04 03:41:42.000000 dnspod_domain_log-1.0.4/dnspod_domain_log.egg-info/SOURCES.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)        1 2024-03-04 03:41:42.000000 dnspod_domain_log-1.0.4/dnspod_domain_log.egg-info/dependency_links.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       51 2024-03-04 03:41:42.000000 dnspod_domain_log-1.0.4/dnspod_domain_log.egg-info/requires.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       18 2024-03-04 03:41:42.000000 dnspod_domain_log-1.0.4/dnspod_domain_log.egg-info/top_level.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       38 2024-03-04 03:41:42.434311 dnspod_domain_log-1.0.4/setup.cfg
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1470 2024-03-04 03:41:31.000000 dnspod_domain_log-1.0.4/setup.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-30 02:25:10.000000 dnspod_domain_log-1.0.5/
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-30 02:25:10.000000 dnspod_domain_log-1.0.5/DNSPOD_Domain_Log/
+-rw-r--r--   0 xf.shen    (502) staff       (20)      124 2024-05-30 01:56:01.000000 dnspod_domain_log-1.0.5/DNSPOD_Domain_Log/__init__.py
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1426 2024-05-30 02:24:16.000000 dnspod_domain_log-1.0.5/DNSPOD_Domain_Log/check_domain_log.py
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1358 2024-05-30 02:25:10.000000 dnspod_domain_log-1.0.5/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      340 2024-05-30 01:56:01.000000 dnspod_domain_log-1.0.5/README.rst
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-30 02:25:10.000000 dnspod_domain_log-1.0.5/dnspod_domain_log.egg-info/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1358 2024-05-30 02:25:10.000000 dnspod_domain_log-1.0.5/dnspod_domain_log.egg-info/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      291 2024-05-30 02:25:10.000000 dnspod_domain_log-1.0.5/dnspod_domain_log.egg-info/SOURCES.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)        1 2024-05-30 02:25:10.000000 dnspod_domain_log-1.0.5/dnspod_domain_log.egg-info/dependency_links.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       74 2024-05-30 02:25:10.000000 dnspod_domain_log-1.0.5/dnspod_domain_log.egg-info/requires.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       18 2024-05-30 02:25:10.000000 dnspod_domain_log-1.0.5/dnspod_domain_log.egg-info/top_level.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       38 2024-05-30 02:25:10.000000 dnspod_domain_log-1.0.5/setup.cfg
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1496 2024-05-30 02:21:50.000000 dnspod_domain_log-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dnspod_domain_log-1.0.4/PKG-INFO` & `dnspod_domain_log-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: dnspod_domain_log
-Version: 1.0.4
+Version: 1.0.5
 Summary: return the log for dns resolution
 Home-page: https://github.com/hanyan007/DNSPOD_Domain_Log.git
 Author: hanyan_news
 Author-email: hanyan0572@gmail.com
 License: BSD License
 Project-URL: Source, https://github.com/hanyan007/DNSPOD_Domain_Log.git
+Description: 
+        ========
+        工程说明
+        ========
+        
+        DNSPod 提供域名一站式服务，包括域名注册、DNS 管理、SSL 证书、网站备案等，您都可以在这方便、快捷的管理这一切，而且大部分服务是免费的。
+        
+        - 链接 https://www.dnspod.cn/
+        
+        - 本工程提供实时解析日志服务。
+        
+        - 默认最多返回20条数据。
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: package-tea-hanyan==1.0.3
-Requires-Dist: package-tea-seven==1.0.0
-
-
-========
-工程说明
-========
-
-DNSPod 提供域名一站式服务，包括域名注册、DNS 管理、SSL 证书、网站备案等，您都可以在这方便、快捷的管理这一切，而且大部分服务是免费的。
-
-- 链接 https://www.dnspod.cn/
-
-- 本工程提供实时解析日志服务。
-
-- 默认最多返回20条数据。
```

### Comparing `dnspod_domain_log-1.0.4/dnspod_domain_log/check_domain_log.py` & `dnspod_domain_log-1.0.5/DNSPOD_Domain_Log/check_domain_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 reload(sys)
 sys.setdefaultencoding('utf-8')
 app = Flask(__name__)
 
 @app.route('/')
 def welcome():
     lt= [] #将结果导入list
-    posturl = 'https://dnsapi.cn/Domain.Log'  #dnspod接口
+    posturl = 'https://dnsapi.cn/Domain.Log'  #本接口 Domain.Log 用于获取域名信息。
+    #example curl -X POST https://dnsapi.cn/Domain.Log  -d 'login_token=LOGIN_TOKEN&format=json&domain_id=2059079'
     postdata = {'login_token':'10xxxxxxxxxxxxxx','format':'json','domain':'keabc.com','length':'20'}#json格式的请求参数
     req = urllib2.Request(posturl)
     data = urllib.urlencode(postdata) #post数据需要urlencode()下，将字典转换成“data1=value1&data2=value2”的格式
     opener = urllib2.build_opener(urllib2.HTTPCookieProcessor())
     response = opener.open(req,data)
     result = response.read()
     list = eval(result)  #将str返回为list
```

### Comparing `dnspod_domain_log-1.0.4/dnspod_domain_log.egg-info/PKG-INFO` & `dnspod_domain_log-1.0.5/dnspod_domain_log.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-Metadata-Version: 2.1
-Name: dnspod_domain_log
-Version: 1.0.4
+Metadata-Version: 1.1
+Name: dnspod-domain-log
+Version: 1.0.5
 Summary: return the log for dns resolution
 Home-page: https://github.com/hanyan007/DNSPOD_Domain_Log.git
 Author: hanyan_news
 Author-email: hanyan0572@gmail.com
 License: BSD License
 Project-URL: Source, https://github.com/hanyan007/DNSPOD_Domain_Log.git
+Description: 
+        ========
+        工程说明
+        ========
+        
+        DNSPod 提供域名一站式服务，包括域名注册、DNS 管理、SSL 证书、网站备案等，您都可以在这方便、快捷的管理这一切，而且大部分服务是免费的。
+        
+        - 链接 https://www.dnspod.cn/
+        
+        - 本工程提供实时解析日志服务。
+        
+        - 默认最多返回20条数据。
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: package-tea-hanyan==1.0.3
-Requires-Dist: package-tea-seven==1.0.0
-
-
-========
-工程说明
-========
-
-DNSPod 提供域名一站式服务，包括域名注册、DNS 管理、SSL 证书、网站备案等，您都可以在这方便、快捷的管理这一切，而且大部分服务是免费的。
-
-- 链接 https://www.dnspod.cn/
-
-- 本工程提供实时解析日志服务。
-
-- 默认最多返回20条数据。
```

### Comparing `dnspod_domain_log-1.0.4/setup.py` & `dnspod_domain_log-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 
 setup(name='dnspod_domain_log',  # 包名
-      version='1.0.4',  # 版本号
+      version='1.0.5',  # 版本号
       description='return the log for dns resolution',
       long_description=long_description,
       author='hanyan_news',
       author_email='hanyan0572@gmail.com',
       url='https://github.com/hanyan007/DNSPOD_Domain_Log.git',
       project_urls={  # Optional
           "Source": 'https://github.com/hanyan007/DNSPOD_Domain_Log.git',
       },
-      install_requires=["package-tea-hanyan==1.0.3", "package-tea-seven==1.0.0"],
+      install_requires=["package-tea-hanyan==1.0.3", "package-tea-seven==1.0.0", "package-tea-six==1.0.0"],
       license='BSD License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
           'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'Natural Language :: Chinese (Simplified)',
```

