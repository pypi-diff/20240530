# Comparing `tmp/ndpi_demerger-0.1.0.tar.gz` & `tmp/ndpi_demerger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndpi_demerger-0.1.0.tar", last modified: Thu May 30 17:42:06 2024, max compression
+gzip compressed data, was "ndpi_demerger-0.1.1.tar", last modified: Thu May 30 18:12:11 2024, max compression
```

## Comparing `ndpi_demerger-0.1.0.tar` & `ndpi_demerger-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:42:06.042856 ndpi_demerger-0.1.0/
--rw-rw-rw-   0        0        0      473 2024-05-30 17:42:06.041859 ndpi_demerger-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-30 17:42:06.037148 ndpi_demerger-0.1.0/ndpi_demerger/
--rw-rw-rw-   0        0        0      178 2024-05-30 17:12:19.000000 ndpi_demerger-0.1.0/ndpi_demerger/__init__.py
--rw-rw-rw-   0        0        0     6421 2024-05-30 17:08:10.000000 ndpi_demerger-0.1.0/ndpi_demerger/extract.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:42:06.041859 ndpi_demerger-0.1.0/ndpi_demerger.egg-info/
--rw-rw-rw-   0        0        0      473 2024-05-30 17:42:05.000000 ndpi_demerger-0.1.0/ndpi_demerger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-05-30 17:42:05.000000 ndpi_demerger-0.1.0/ndpi_demerger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:42:05.000000 ndpi_demerger-0.1.0/ndpi_demerger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-30 17:42:05.000000 ndpi_demerger-0.1.0/ndpi_demerger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-30 17:42:05.000000 ndpi_demerger-0.1.0/ndpi_demerger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 17:42:06.042856 ndpi_demerger-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      628 2024-05-30 17:14:34.000000 ndpi_demerger-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:12:11.456388 ndpi_demerger-0.1.1/
+-rw-rw-rw-   0        0        0     1058 2024-05-30 18:07:52.000000 ndpi_demerger-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      496 2024-05-30 18:12:11.455390 ndpi_demerger-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 18:12:11.447412 ndpi_demerger-0.1.1/ndpi_demerger/
+-rw-rw-rw-   0        0        0      147 2024-05-30 18:05:43.000000 ndpi_demerger-0.1.1/ndpi_demerger/__init__.py
+-rw-rw-rw-   0        0        0     5969 2024-05-30 18:11:40.000000 ndpi_demerger-0.1.1/ndpi_demerger/extract.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:12:11.454394 ndpi_demerger-0.1.1/ndpi_demerger.egg-info/
+-rw-rw-rw-   0        0        0      496 2024-05-30 18:12:11.000000 ndpi_demerger-0.1.1/ndpi_demerger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-30 18:12:11.000000 ndpi_demerger-0.1.1/ndpi_demerger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 18:12:11.000000 ndpi_demerger-0.1.1/ndpi_demerger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 18:12:11.000000 ndpi_demerger-0.1.1/ndpi_demerger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 18:12:11.000000 ndpi_demerger-0.1.1/ndpi_demerger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 18:12:11.456388 ndpi_demerger-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-05-30 18:03:28.000000 ndpi_demerger-0.1.1/setup.py
```

### Comparing `ndpi_demerger-0.1.0/ndpi_demerger/extract.py` & `ndpi_demerger-0.1.1/ndpi_demerger/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,17 +117,7 @@
         # 计算当前文件的处理时间
         current_file_elapsed_time = time.time() - current_file_start_time
         total_elapsed_time = time.time() - start_time
         print(f'已处理 {index + 1}/{total_files} 文件，占总进度的 {(index + 1) / total_files * 100:.2f}%，当前文件耗时 {current_file_elapsed_time:.2f} 秒，已运行时间 {total_elapsed_time:.2f} 秒。')
 
     total_elapsed_time = time.time() - start_time  # 计算总耗时
     print(f'所有文件已处理完成，总耗时 {total_elapsed_time / 60:.2f} 分钟。')
-
-# 配置基本路径和参数
-base_path = r'D:\科研\免疫\image'  # NDPI文件所在的基础路径
-output_base = r'D:\科研\免疫\extract'  # 输出基础路径
-threshold = 50  # patches饱和度阈值
-size = 512  # patches的大小
-magnification = 20  # 预设放大倍数
-
-# 调用函数以处理NDPI文件
-process_ndpi_files(base_path, output_base, saturation_threshold=threshold, patch_size=size, target_magnification=magnification)
```

### Comparing `ndpi_demerger-0.1.0/setup.py` & `ndpi_demerger-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='ndpi_demerger',
-    version='0.1.0',
+    version='0.1.1',
     description='A package for extracting patches from NDPI images',
     author='Thirteen',
     author_email='506607814@qq.com',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'openslide-python',
@@ -19,7 +19,9 @@
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
 )
+
+
```

