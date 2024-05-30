# Comparing `tmp/grimo-0.1.1.tar.gz` & `tmp/grimo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimo-0.1.1.tar", last modified: Thu May 30 19:34:33 2024, max compression
+gzip compressed data, was "grimo-0.1.2.tar", last modified: Thu May 30 19:39:13 2024, max compression
```

## Comparing `grimo-0.1.1.tar` & `grimo-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:34:33.485037 grimo-0.1.1/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1071 2024-05-30 19:18:47.000000 grimo-0.1.1/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11794 2024-05-30 19:34:33.484857 grimo-0.1.1/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11137 2024-05-30 19:30:03.000000 grimo-0.1.1/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:34:33.483066 grimo-0.1.1/grimo/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4292 2024-05-30 19:30:03.000000 grimo-0.1.1/grimo/README_USAGE.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3695 2024-05-30 19:30:03.000000 grimo-0.1.1/grimo/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11250 2024-05-30 19:30:03.000000 grimo-0.1.1/grimo/cli.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5637 2024-05-30 19:30:03.000000 grimo-0.1.1/grimo/core.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4938 2024-05-30 19:30:03.000000 grimo-0.1.1/grimo/package.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      309 2024-05-30 19:30:03.000000 grimo-0.1.1/grimo/req_cli.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      366 2024-05-30 19:30:03.000000 grimo-0.1.1/grimo/req_readme.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5993 2024-05-30 19:30:03.000000 grimo-0.1.1/grimo/storage.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1549 2024-05-30 19:30:03.000000 grimo-0.1.1/grimo/utils.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:34:33.483998 grimo-0.1.1/grimo.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11794 2024-05-30 19:34:33.000000 grimo-0.1.1/grimo.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      438 2024-05-30 19:34:33.000000 grimo-0.1.1/grimo.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-30 19:34:33.000000 grimo-0.1.1/grimo.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       41 2024-05-30 19:34:33.000000 grimo-0.1.1/grimo.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       54 2024-05-30 19:34:33.000000 grimo-0.1.1/grimo.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        6 2024-05-30 19:34:33.000000 grimo-0.1.1/grimo.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-30 19:34:33.485073 grimo-0.1.1/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1257 2024-05-30 19:32:04.000000 grimo-0.1.1/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:34:33.484612 grimo-0.1.1/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3528 2024-05-30 19:30:03.000000 grimo-0.1.1/tests/test_core.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3159 2024-05-30 19:30:03.000000 grimo-0.1.1/tests/test_package.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2993 2024-05-30 19:30:03.000000 grimo-0.1.1/tests/test_storage.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3283 2024-05-30 19:30:03.000000 grimo-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:39:13.663411 grimo-0.1.2/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1071 2024-05-30 19:18:47.000000 grimo-0.1.2/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11818 2024-05-30 19:39:13.663101 grimo-0.1.2/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11161 2024-05-30 19:36:35.000000 grimo-0.1.2/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:39:13.661581 grimo-0.1.2/grimo/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4292 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/README_USAGE.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3695 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11250 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/cli.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5637 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/core.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4938 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/package.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      309 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/req_cli.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      366 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/req_readme.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5993 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/storage.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1549 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/utils.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:39:13.662315 grimo-0.1.2/grimo.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11818 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      438 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       41 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       54 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        6 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-30 19:39:13.663452 grimo-0.1.2/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1257 2024-05-30 19:38:02.000000 grimo-0.1.2/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:39:13.662859 grimo-0.1.2/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3528 2024-05-30 19:30:03.000000 grimo-0.1.2/tests/test_core.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3159 2024-05-30 19:30:03.000000 grimo-0.1.2/tests/test_package.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2993 2024-05-30 19:30:03.000000 grimo-0.1.2/tests/test_storage.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3283 2024-05-30 19:30:03.000000 grimo-0.1.2/tests/test_utils.py
```

### Comparing `grimo-0.1.1/LICENSE` & `grimo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/PKG-INFO` & `grimo-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Abstract Programming Language Package Manager
 Home-page: https://github.com/dai-motoki/grimo
 Author: dai motoki
 Author-email: dai.motoki@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,46 +20,52 @@
 
 ### ゴール: 抽象プログラミング言語パッケージマネージャー「grimo」をPythonで作成
 
 
 ## 0. 利用方法
 
 ### コマンドラインオプション
+```
                         利用可能なサブコマンド
     install             パッケージをインストールする（利用可）
     upload              パッケージをアップロードする（利用可）
     search              パッケージを検索する（未開発）
     update              パッケージをアップデートする（未開発）
     uninstall           パッケージをアンインストールする（未開発）
+```
 
 ### パッケージのアップロード
 
+```
 grimo upload .
 
 project/
 ├── metadata.json # パッケージのメタデータ
 ├── package_name/
 │   ├── def.md # パッケージの定義
 │   ├── util.md # パッケージのユーティリティ
 │   ├── var.md # パッケージの変数
 │   └── ...
+```
 
 ### パッケージのインストール
 
+```
 grimo install package_name
 
 project/
 ├── grimoires/
 │   ├── package_name/
 │   │   ├── metadata.json # パッケージのメタデータ
 │   │   ├── def.md # パッケージの定義
 │   │   ├── util.md # パッケージのユーティリティ
 │   │   ├── var.md # パッケージの変数
 │   │   └── ...
 
+```
 
 ## 1. 目的
 
 多様なプログラミング言語のパッケージを一元管理できる、強力かつユーザーフレンドリーな抽象プログラミング言語パッケージマネージャー「grimo」をPythonで実装する。grimoは、プログラミング言語に依存せず、あらゆるパッケージの検索、インストール、アップグレードをシームレスに実行できるツールを目指します。
 
 ## 2. パッケージの基本構造
```

### Comparing `grimo-0.1.1/README.md` & `grimo-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,46 +2,52 @@
 
 ### ゴール: 抽象プログラミング言語パッケージマネージャー「grimo」をPythonで作成
 
 
 ## 0. 利用方法
 
 ### コマンドラインオプション
+```
                         利用可能なサブコマンド
     install             パッケージをインストールする（利用可）
     upload              パッケージをアップロードする（利用可）
     search              パッケージを検索する（未開発）
     update              パッケージをアップデートする（未開発）
     uninstall           パッケージをアンインストールする（未開発）
+```
 
 ### パッケージのアップロード
 
+```
 grimo upload .
 
 project/
 ├── metadata.json # パッケージのメタデータ
 ├── package_name/
 │   ├── def.md # パッケージの定義
 │   ├── util.md # パッケージのユーティリティ
 │   ├── var.md # パッケージの変数
 │   └── ...
+```
 
 ### パッケージのインストール
 
+```
 grimo install package_name
 
 project/
 ├── grimoires/
 │   ├── package_name/
 │   │   ├── metadata.json # パッケージのメタデータ
 │   │   ├── def.md # パッケージの定義
 │   │   ├── util.md # パッケージのユーティリティ
 │   │   ├── var.md # パッケージの変数
 │   │   └── ...
 
+```
 
 ## 1. 目的
 
 多様なプログラミング言語のパッケージを一元管理できる、強力かつユーザーフレンドリーな抽象プログラミング言語パッケージマネージャー「grimo」をPythonで実装する。grimoは、プログラミング言語に依存せず、あらゆるパッケージの検索、インストール、アップグレードをシームレスに実行できるツールを目指します。
 
 ## 2. パッケージの基本構造
```

### Comparing `grimo-0.1.1/grimo/README_USAGE.md` & `grimo-0.1.2/grimo/README_USAGE.md`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/grimo/__init__.py` & `grimo-0.1.2/grimo/__init__.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/grimo/cli.py` & `grimo-0.1.2/grimo/cli.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/grimo/core.py` & `grimo-0.1.2/grimo/core.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/grimo/package.py` & `grimo-0.1.2/grimo/package.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/grimo/storage.py` & `grimo-0.1.2/grimo/storage.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/grimo/utils.py` & `grimo-0.1.2/grimo/utils.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/grimo.egg-info/PKG-INFO` & `grimo-0.1.2/grimo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Abstract Programming Language Package Manager
 Home-page: https://github.com/dai-motoki/grimo
 Author: dai motoki
 Author-email: dai.motoki@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,46 +20,52 @@
 
 ### ゴール: 抽象プログラミング言語パッケージマネージャー「grimo」をPythonで作成
 
 
 ## 0. 利用方法
 
 ### コマンドラインオプション
+```
                         利用可能なサブコマンド
     install             パッケージをインストールする（利用可）
     upload              パッケージをアップロードする（利用可）
     search              パッケージを検索する（未開発）
     update              パッケージをアップデートする（未開発）
     uninstall           パッケージをアンインストールする（未開発）
+```
 
 ### パッケージのアップロード
 
+```
 grimo upload .
 
 project/
 ├── metadata.json # パッケージのメタデータ
 ├── package_name/
 │   ├── def.md # パッケージの定義
 │   ├── util.md # パッケージのユーティリティ
 │   ├── var.md # パッケージの変数
 │   └── ...
+```
 
 ### パッケージのインストール
 
+```
 grimo install package_name
 
 project/
 ├── grimoires/
 │   ├── package_name/
 │   │   ├── metadata.json # パッケージのメタデータ
 │   │   ├── def.md # パッケージの定義
 │   │   ├── util.md # パッケージのユーティリティ
 │   │   ├── var.md # パッケージの変数
 │   │   └── ...
 
+```
 
 ## 1. 目的
 
 多様なプログラミング言語のパッケージを一元管理できる、強力かつユーザーフレンドリーな抽象プログラミング言語パッケージマネージャー「grimo」をPythonで実装する。grimoは、プログラミング言語に依存せず、あらゆるパッケージの検索、インストール、アップグレードをシームレスに実行できるツールを目指します。
 
 ## 2. パッケージの基本構造
```

### Comparing `grimo-0.1.1/setup.py` & `grimo-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='grimo',
-    version='0.1.1',
+    version='0.1.2',
     description='Abstract Programming Language Package Manager',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',  # 追加: long_descriptionの形式を指定
     author='dai motoki',
     author_email='dai.motoki@gmail.com',
     url='https://github.com/dai-motoki/grimo',
     packages=find_packages(exclude=['tests']),
```

### Comparing `grimo-0.1.1/tests/test_core.py` & `grimo-0.1.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/tests/test_package.py` & `grimo-0.1.2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/tests/test_storage.py` & `grimo-0.1.2/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.1/tests/test_utils.py` & `grimo-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

