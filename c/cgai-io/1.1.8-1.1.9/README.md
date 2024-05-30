# Comparing `tmp/cgai_io-1.1.8.tar.gz` & `tmp/cgai_io-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgai_io-1.1.8.tar", last modified: Tue Apr 23 01:22:26 2024, max compression
+gzip compressed data, was "cgai_io-1.1.9.tar", last modified: Thu May 30 01:37:21 2024, max compression
```

## Comparing `cgai_io-1.1.8.tar` & `cgai_io-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 01:22:26.819719 cgai_io-1.1.8/
--rw-rw-rw-   0        0        0    35823 2024-04-23 01:15:31.000000 cgai_io-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     3831 2024-04-23 01:22:26.818721 cgai_io-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2967 2024-04-23 01:15:31.000000 cgai_io-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 01:22:26.816728 cgai_io-1.1.8/cgai_io/
--rw-rw-rw-   0        0        0     2912 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/Copy.py
--rw-rw-rw-   0        0        0     2606 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/Delete.py
--rw-rw-rw-   0        0        0      319 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/Info.py
--rw-rw-rw-   0        0        0      923 2024-04-23 01:12:13.000000 cgai_io-1.1.8/cgai_io/Move.py
--rw-rw-rw-   0        0        0      910 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/Name.py
--rw-rw-rw-   0        0        0      777 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/Pack.py
--rw-rw-rw-   0        0        0      408 2024-04-23 01:12:19.000000 cgai_io-1.1.8/cgai_io/__init__.py
--rw-rw-rw-   0        0        0      384 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/_util.py
-drwxrwxrwx   0        0        0        0 2024-04-23 01:22:26.818721 cgai_io-1.1.8/cgai_io.egg-info/
--rw-rw-rw-   0        0        0     3831 2024-04-23 01:22:26.000000 cgai_io-1.1.8/cgai_io.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-04-23 01:22:26.000000 cgai_io-1.1.8/cgai_io.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 01:22:26.000000 cgai_io-1.1.8/cgai_io.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 01:22:26.000000 cgai_io-1.1.8/cgai_io.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 01:22:26.819719 cgai_io-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1166 2024-04-23 01:11:09.000000 cgai_io-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 01:37:21.021377 cgai_io-1.1.9/
+-rw-rw-rw-   0        0        0    35823 2024-04-23 01:15:31.000000 cgai_io-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     5057 2024-05-30 01:37:21.021377 cgai_io-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2967 2024-04-23 01:15:31.000000 cgai_io-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 01:37:21.019384 cgai_io-1.1.9/cgai_io/
+-rw-rw-rw-   0        0        0     2912 2024-04-10 06:36:34.000000 cgai_io-1.1.9/cgai_io/Copy.py
+-rw-rw-rw-   0        0        0     2606 2024-04-10 06:36:34.000000 cgai_io-1.1.9/cgai_io/Delete.py
+-rw-rw-rw-   0        0        0      319 2024-04-10 06:36:34.000000 cgai_io-1.1.9/cgai_io/Info.py
+-rw-rw-rw-   0        0        0     1069 2024-05-30 01:22:31.000000 cgai_io-1.1.9/cgai_io/Move.py
+-rw-rw-rw-   0        0        0      910 2024-04-10 06:36:34.000000 cgai_io-1.1.9/cgai_io/Name.py
+-rw-rw-rw-   0        0        0      777 2024-04-10 06:36:34.000000 cgai_io-1.1.9/cgai_io/Pack.py
+-rw-rw-rw-   0        0        0      408 2024-05-30 01:29:01.000000 cgai_io-1.1.9/cgai_io/__init__.py
+-rw-rw-rw-   0        0        0      384 2024-04-10 06:36:34.000000 cgai_io-1.1.9/cgai_io/_util.py
+drwxrwxrwx   0        0        0        0 2024-05-30 01:37:21.020381 cgai_io-1.1.9/cgai_io.egg-info/
+-rw-rw-rw-   0        0        0     5057 2024-05-30 01:37:20.000000 cgai_io-1.1.9/cgai_io.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-30 01:37:21.000000 cgai_io-1.1.9/cgai_io.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 01:37:20.000000 cgai_io-1.1.9/cgai_io.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-30 01:37:20.000000 cgai_io-1.1.9/cgai_io.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 01:37:21.021377 cgai_io-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1166 2024-05-30 01:29:11.000000 cgai_io-1.1.9/setup.py
```

### Comparing `cgai_io-1.1.8/LICENSE` & `cgai_io-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.8/README.md` & `cgai_io-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.8/cgai_io/Copy.py` & `cgai_io-1.1.9/cgai_io/Copy.py`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.8/cgai_io/Delete.py` & `cgai_io-1.1.9/cgai_io/Delete.py`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.8/cgai_io/Move.py` & `cgai_io-1.1.9/cgai_io/Move.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 #-*- coding:utf-8 -*-
 """
 移动文件或目录
 """
+import subprocess
 from ._util import *
 
 
-def mv(src,des):
+def mv(src,des,wait=True):
     """
     移动文件或文件夹
     :param src: 源文件或目录
     :param des: 目标文件或目录
     :return:
     """
     if iswin():
-        os.popen('move {} {}'.format(src.replace('/', '\\'),des.replace('/', '\\')))
+        src_file = src.replace('/', '\\')
+        des_file = des.replace('/', '\\')
+        p = subprocess.Popen(['move',src_file,des_file],shell=True)
     else:
-        os.popen('mv {} {}'.format(src.replace('\\', '/'), des.replace('\\', '/')))
+        p = subprocess.Popen(['mv',src_file,des_file],shell=True)
 
-
-def mvfile(src,des):
+    if wait:
+        p.wait()
+    
+def mvfile(src,des,wait=True):
     """
     移动文件
     :param src: 源文件
     :param des: 目标文件
     :return: 
     """
     if isfile(src):
-        mv(src,des)
+        mv(src,des,wait)
     else:
         raise Exception("输入非文件")
 
-def mvdir(src,des):
+def mvdir(src,des,wait=True):
     """
     移动文件目录
     :param src: 源文件目录
     :param des: 目标文件目录
     :return:
     """
     if isdir(src):
-        mv(src,des)
+        mv(src,des,wait)
     else:
         raise Exception("输入非文件目录")
```

### Comparing `cgai_io-1.1.8/cgai_io/Name.py` & `cgai_io-1.1.9/cgai_io/Name.py`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.8/cgai_io/Pack.py` & `cgai_io-1.1.9/cgai_io/Pack.py`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.8/setup.py` & `cgai_io-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="cgai_io",
-    version="1.1.8",
+    version="1.1.9",
     author="Master Zhang",
     author_email="360014296@qq.com",
     description="A simple, light and fast data stream operation Python Library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zxzxde/cgai-io",
     packages=setuptools.find_packages(),
```

