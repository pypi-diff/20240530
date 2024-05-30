# Comparing `tmp/xtn-tools-pro-1.0.0.1.8.tar.gz` & `tmp/xtn-tools-pro-1.0.0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtn-tools-pro-1.0.0.1.8.tar", last modified: Thu May 23 09:55:56 2024, max compression
+gzip compressed data, was "dist\xtn-tools-pro-1.0.0.1.9.tar", last modified: Thu May 30 00:07:05 2024, max compression
```

## Comparing `xtn-tools-pro-1.0.0.1.8.tar` & `xtn-tools-pro-1.0.0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.1.8/LICENSE
--rw-rw-rw-   0        0        0      287 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1289 2024-05-23 09:52:07.000000 xtn-tools-pro-1.0.0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/
--rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/db/
--rw-rw-rw-   0        0        0     5573 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/db/MongoDB.py
--rw-rw-rw-   0        0        0    13373 2024-05-12 14:20:54.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/db/MysqlDB.py
--rw-rw-rw-   0        0        0     6228 2024-05-23 09:54:54.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/db/RedisDB.py
--rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/proxy/
--rw-rw-rw-   0        0        0    11049 2024-05-16 00:39:58.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/proxy/XiaoXiangProxy.py
--rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/proxy/__init__.py
--rw-rw-rw-   0        0        0     8703 2024-05-13 14:02:38.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/proxy/proxy.py
--rw-rw-rw-   0        0        0      542 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/
--rw-rw-rw-   0        0        0      418 2024-05-12 04:02:30.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/__init__.py
--rw-rw-rw-   0        0        0     3190 2024-05-15 08:10:00.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/crypto.py
--rw-rw-rw-   0        0        0     1509 2024-05-12 16:32:12.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/file_utils.py
--rw-rw-rw-   0        0        0     3812 2024-05-15 15:46:10.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/helpers.py
--rw-rw-rw-   0        0        0     8139 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/log.py
--rw-rw-rw-   0        0        0     1657 2024-05-12 12:05:16.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/retry.py
--rw-rw-rw-   0        0        0     6263 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/sql.py
--rw-rw-rw-   0        0        0     4859 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/time_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro.egg-info/
--rw-rw-rw-   0        0        0      287 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 09:55:56.000000 xtn-tools-pro-1.0.0.1.8/xtn_tools_pro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      287 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1289 2024-05-30 00:03:32.000000 xtn-tools-pro-1.0.0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/
+-rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/db/
+-rw-rw-rw-   0        0        0     5573 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/db/MongoDB.py
+-rw-rw-rw-   0        0        0    13373 2024-05-12 14:20:54.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/db/MysqlDB.py
+-rw-rw-rw-   0        0        0     6466 2024-05-30 00:06:22.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/db/RedisDB.py
+-rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/proxy/
+-rw-rw-rw-   0        0        0    11049 2024-05-16 00:39:58.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/proxy/XiaoXiangProxy.py
+-rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/proxy/__init__.py
+-rw-rw-rw-   0        0        0     8703 2024-05-13 14:02:38.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/proxy/proxy.py
+-rw-rw-rw-   0        0        0      542 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/
+-rw-rw-rw-   0        0        0      418 2024-05-12 04:02:30.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/__init__.py
+-rw-rw-rw-   0        0        0     3190 2024-05-15 08:10:00.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/crypto.py
+-rw-rw-rw-   0        0        0     1509 2024-05-12 16:32:12.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/file_utils.py
+-rw-rw-rw-   0        0        0     3812 2024-05-15 15:46:10.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/helpers.py
+-rw-rw-rw-   0        0        0     8139 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/log.py
+-rw-rw-rw-   0        0        0     1657 2024-05-12 12:05:16.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/retry.py
+-rw-rw-rw-   0        0        0     6263 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/sql.py
+-rw-rw-rw-   0        0        0     4859 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/time_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 00:07:04.000000 xtn-tools-pro-1.0.0.1.9/xtn_tools_pro.egg-info/top_level.txt
```

### Comparing `xtn-tools-pro-1.0.0.1.8/setup.py` & `xtn-tools-pro-1.0.0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtn-tools-pro",  # 模块名称
-    version="1.0.0.1.8",  # 版本
+    version="1.0.0.1.9",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/db/MongoDB.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/db/MongoDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/db/MysqlDB.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/db/MysqlDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/db/RedisDB.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/db/RedisDB.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,14 +117,25 @@
         """
             从集合中弹出元素
         :param table:
         :return:
         """
         return self._redis.spop(table)
 
+    def sget_count(self, table):
+        """
+            获取无序集合数量
+        :param table:
+        :return:
+        """
+        return self._redis.scard(table)
+
+    def get_redis(self):
+        return self._redis
+
     def incr(self, key):
         """
             对一个键的值进行自增操作
         :param key: 需要自增的key
         :return:
         """
         return self._redis.incr(key)
```

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/proxy/XiaoXiangProxy.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/proxy/XiaoXiangProxy.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/proxy/proxy.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/tools.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/tools.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/crypto.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/file_utils.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/helpers.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/log.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/log.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/retry.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/retry.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/sql.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/sql.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro/utils/time_utils.py` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.8/xtn_tools_pro.egg-info/SOURCES.txt` & `xtn-tools-pro-1.0.0.1.9/xtn_tools_pro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

