# Comparing `tmp/grimo-0.1.3.tar.gz` & `tmp/grimo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimo-0.1.3.tar", last modified: Thu May 30 19:53:31 2024, max compression
+gzip compressed data, was "grimo-0.1.4.tar", last modified: Thu May 30 19:55:10 2024, max compression
```

## Comparing `grimo-0.1.3.tar` & `grimo-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:53:31.187903 grimo-0.1.3/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1071 2024-05-30 19:18:47.000000 grimo-0.1.3/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    12510 2024-05-30 19:53:31.187696 grimo-0.1.3/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11853 2024-05-30 19:50:11.000000 grimo-0.1.3/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:53:31.185952 grimo-0.1.3/grimo/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4292 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/README_USAGE.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3695 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11250 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/cli.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5637 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/core.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4938 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/package.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      309 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/req_cli.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      366 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/req_readme.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5993 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/storage.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1549 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/utils.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:53:31.186709 grimo-0.1.3/grimo.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    12510 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      438 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       41 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       54 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        6 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-30 19:53:31.187949 grimo-0.1.3/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1257 2024-05-30 19:52:53.000000 grimo-0.1.3/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:53:31.187384 grimo-0.1.3/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3528 2024-05-30 19:30:03.000000 grimo-0.1.3/tests/test_core.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3159 2024-05-30 19:30:03.000000 grimo-0.1.3/tests/test_package.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2993 2024-05-30 19:30:03.000000 grimo-0.1.3/tests/test_storage.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3283 2024-05-30 19:30:03.000000 grimo-0.1.3/tests/test_utils.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:55:10.757571 grimo-0.1.4/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1071 2024-05-30 19:18:47.000000 grimo-0.1.4/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    12660 2024-05-30 19:55:10.757364 grimo-0.1.4/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    12003 2024-05-30 19:55:01.000000 grimo-0.1.4/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:55:10.756075 grimo-0.1.4/grimo/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4292 2024-05-30 19:30:03.000000 grimo-0.1.4/grimo/README_USAGE.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3695 2024-05-30 19:30:03.000000 grimo-0.1.4/grimo/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11250 2024-05-30 19:30:03.000000 grimo-0.1.4/grimo/cli.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5637 2024-05-30 19:30:03.000000 grimo-0.1.4/grimo/core.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4938 2024-05-30 19:30:03.000000 grimo-0.1.4/grimo/package.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      309 2024-05-30 19:30:03.000000 grimo-0.1.4/grimo/req_cli.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      366 2024-05-30 19:30:03.000000 grimo-0.1.4/grimo/req_readme.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5993 2024-05-30 19:30:03.000000 grimo-0.1.4/grimo/storage.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1549 2024-05-30 19:30:03.000000 grimo-0.1.4/grimo/utils.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:55:10.756651 grimo-0.1.4/grimo.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    12660 2024-05-30 19:55:10.000000 grimo-0.1.4/grimo.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      438 2024-05-30 19:55:10.000000 grimo-0.1.4/grimo.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-30 19:55:10.000000 grimo-0.1.4/grimo.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       41 2024-05-30 19:55:10.000000 grimo-0.1.4/grimo.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       54 2024-05-30 19:55:10.000000 grimo-0.1.4/grimo.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        6 2024-05-30 19:55:10.000000 grimo-0.1.4/grimo.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-30 19:55:10.757609 grimo-0.1.4/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1257 2024-05-30 19:55:08.000000 grimo-0.1.4/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:55:10.757077 grimo-0.1.4/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3528 2024-05-30 19:30:03.000000 grimo-0.1.4/tests/test_core.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3159 2024-05-30 19:30:03.000000 grimo-0.1.4/tests/test_package.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2993 2024-05-30 19:30:03.000000 grimo-0.1.4/tests/test_storage.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3283 2024-05-30 19:30:03.000000 grimo-0.1.4/tests/test_utils.py
```

### Comparing `grimo-0.1.3/LICENSE` & `grimo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/PKG-INFO` & `grimo-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Abstract Programming Language Package Manager
 Home-page: https://github.com/dai-motoki/grimo
 Author: dai motoki
 Author-email: dai.motoki@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -81,17 +81,18 @@
 grimo upload .
 
 ```
 
 ### パッケージのインストール
 
 インストールされたファイルはgrimoiresディレクトリに格納されます。
+-v でバージョン指定をお願いします（ここも何も指定がない場合最新を取得するようにする予定です）
 
 ```
-grimo install package_name
+grimo install package_name -v version
 
 project/
 ├── grimoires/
 │   ├── package_name/
 │   │   ├── metadata.json # パッケージのメタデータ
 │   │   ├── def.md # パッケージの定義
 │   │   ├── util.md # パッケージのユーティリティ
```

### Comparing `grimo-0.1.3/README.md` & `grimo-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,18 @@
 grimo upload .
 
 ```
 
 ### パッケージのインストール
 
 インストールされたファイルはgrimoiresディレクトリに格納されます。
+-v でバージョン指定をお願いします（ここも何も指定がない場合最新を取得するようにする予定です）
 
 ```
-grimo install package_name
+grimo install package_name -v version
 
 project/
 ├── grimoires/
 │   ├── package_name/
 │   │   ├── metadata.json # パッケージのメタデータ
 │   │   ├── def.md # パッケージの定義
 │   │   ├── util.md # パッケージのユーティリティ
```

### Comparing `grimo-0.1.3/grimo/README_USAGE.md` & `grimo-0.1.4/grimo/README_USAGE.md`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/grimo/__init__.py` & `grimo-0.1.4/grimo/__init__.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/grimo/cli.py` & `grimo-0.1.4/grimo/cli.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/grimo/core.py` & `grimo-0.1.4/grimo/core.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/grimo/package.py` & `grimo-0.1.4/grimo/package.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/grimo/storage.py` & `grimo-0.1.4/grimo/storage.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/grimo/utils.py` & `grimo-0.1.4/grimo/utils.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/grimo.egg-info/PKG-INFO` & `grimo-0.1.4/grimo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Abstract Programming Language Package Manager
 Home-page: https://github.com/dai-motoki/grimo
 Author: dai motoki
 Author-email: dai.motoki@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -81,17 +81,18 @@
 grimo upload .
 
 ```
 
 ### パッケージのインストール
 
 インストールされたファイルはgrimoiresディレクトリに格納されます。
+-v でバージョン指定をお願いします（ここも何も指定がない場合最新を取得するようにする予定です）
 
 ```
-grimo install package_name
+grimo install package_name -v version
 
 project/
 ├── grimoires/
 │   ├── package_name/
 │   │   ├── metadata.json # パッケージのメタデータ
 │   │   ├── def.md # パッケージの定義
 │   │   ├── util.md # パッケージのユーティリティ
```

### Comparing `grimo-0.1.3/setup.py` & `grimo-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='grimo',
-    version='0.1.3',
+    version='0.1.4',
     description='Abstract Programming Language Package Manager',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',  # 追加: long_descriptionの形式を指定
     author='dai motoki',
     author_email='dai.motoki@gmail.com',
     url='https://github.com/dai-motoki/grimo',
     packages=find_packages(exclude=['tests']),
```

### Comparing `grimo-0.1.3/tests/test_core.py` & `grimo-0.1.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/tests/test_package.py` & `grimo-0.1.4/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/tests/test_storage.py` & `grimo-0.1.4/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.3/tests/test_utils.py` & `grimo-0.1.4/tests/test_utils.py`

 * *Files identical despite different names*

