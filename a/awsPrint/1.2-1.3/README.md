# Comparing `tmp/awsPrint-1.2.tar.gz` & `tmp/awsPrint-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsPrint-1.2.tar", last modified: Fri May 24 22:16:37 2024, max compression
+gzip compressed data, was "awsPrint-1.3.tar", last modified: Thu May 30 00:46:52 2024, max compression
```

## Comparing `awsPrint-1.2.tar` & `awsPrint-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 22:16:37.925972 awsPrint-1.2/
--rw-rw-rw-   0        0        0      527 2024-05-24 22:16:37.925228 awsPrint-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-24 22:16:37.918575 awsPrint-1.2/awsPrint/
--rw-rw-rw-   0        0        0     2847 2024-05-24 21:35:07.000000 awsPrint-1.2/awsPrint/__init__.py
--rw-rw-rw-   0        0        0      398 2024-05-24 20:26:31.000000 awsPrint-1.2/awsPrint/awsPrint.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:16:37.924224 awsPrint-1.2/awsPrint.egg-info/
--rw-rw-rw-   0        0        0      527 2024-05-24 22:16:37.000000 awsPrint-1.2/awsPrint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-24 22:16:37.000000 awsPrint-1.2/awsPrint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 22:16:37.000000 awsPrint-1.2/awsPrint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-24 22:16:37.000000 awsPrint-1.2/awsPrint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 22:16:37.000000 awsPrint-1.2/awsPrint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 22:16:37.925972 awsPrint-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1286 2024-05-24 22:16:34.000000 awsPrint-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:46:52.790506 awsPrint-1.3/
+-rw-rw-rw-   0        0        0      527 2024-05-30 00:46:52.790506 awsPrint-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 00:46:52.786137 awsPrint-1.3/awsPrint/
+-rw-rw-rw-   0        0        0     2909 2024-05-30 00:44:09.000000 awsPrint-1.3/awsPrint/__init__.py
+-rw-rw-rw-   0        0        0      398 2024-05-24 20:26:31.000000 awsPrint-1.3/awsPrint/awsPrint.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:46:52.789505 awsPrint-1.3/awsPrint.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-05-30 00:46:52.000000 awsPrint-1.3/awsPrint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-30 00:46:52.000000 awsPrint-1.3/awsPrint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 00:46:52.000000 awsPrint-1.3/awsPrint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-30 00:46:52.000000 awsPrint-1.3/awsPrint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 00:46:52.000000 awsPrint-1.3/awsPrint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 00:46:52.790506 awsPrint-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2024-05-30 00:44:09.000000 awsPrint-1.3/setup.py
```

### Comparing `awsPrint-1.2/awsPrint/__init__.py` & `awsPrint-1.3/awsPrint/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-"""https://github.com/Gorkor227/color_print"""
+"""https://github.com/Gorkor227/awsPrint"""
 from .awsPrint import cp, sepLine
 from typing import Union
 from typing_extensions import Self
 
+__VERSION__ = '1.3'
+
 
 class FontColor:
     black = '\x1b[30m'
     red = '\x1b[31m'
     green = '\x1b[32m'
     yellow = '\x1b[33m'
     blue = '\x1b[34m'
@@ -83,8 +85,10 @@
     :param sep: same as print()
     :param end: same as print()
     :param file: same as print()
     :param color: Yellow  --> FontColor's attr
     :param isFormat: False   --> By pprint.pformat
     :return: Self
     """
+    if not values:
+        values = '',
     return CPrint()(*values, sep=sep, end=end, file=file, isFormat=isFormat, color=color or FontColor.YELLOW)
```

### Comparing `awsPrint-1.2/setup.py` & `awsPrint-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='awsPrint',  # 包名
-    version='1.2',  # 版本
+    version='1.3',  # 版本
     description="colorful print",  # 包简介
     # long_description=open('README.md', 'r', encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='Gorkor',  # 作者
     author_email='2226750760@qq.com',  # 作者邮件
     maintainer='Gorkor',  # 维护者
     maintainer_email='2226750760@qq.com',  # 维护者邮件
```

