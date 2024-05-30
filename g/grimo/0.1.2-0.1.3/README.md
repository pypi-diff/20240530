# Comparing `tmp/grimo-0.1.2.tar.gz` & `tmp/grimo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimo-0.1.2.tar", last modified: Thu May 30 19:39:13 2024, max compression
+gzip compressed data, was "grimo-0.1.3.tar", last modified: Thu May 30 19:53:31 2024, max compression
```

## Comparing `grimo-0.1.2.tar` & `grimo-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:39:13.663411 grimo-0.1.2/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1071 2024-05-30 19:18:47.000000 grimo-0.1.2/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11818 2024-05-30 19:39:13.663101 grimo-0.1.2/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11161 2024-05-30 19:36:35.000000 grimo-0.1.2/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:39:13.661581 grimo-0.1.2/grimo/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4292 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/README_USAGE.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3695 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11250 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/cli.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5637 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/core.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4938 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/package.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      309 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/req_cli.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      366 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/req_readme.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5993 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/storage.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1549 2024-05-30 19:30:03.000000 grimo-0.1.2/grimo/utils.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:39:13.662315 grimo-0.1.2/grimo.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11818 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      438 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       41 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       54 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        6 2024-05-30 19:39:13.000000 grimo-0.1.2/grimo.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-30 19:39:13.663452 grimo-0.1.2/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1257 2024-05-30 19:38:02.000000 grimo-0.1.2/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:39:13.662859 grimo-0.1.2/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3528 2024-05-30 19:30:03.000000 grimo-0.1.2/tests/test_core.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3159 2024-05-30 19:30:03.000000 grimo-0.1.2/tests/test_package.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2993 2024-05-30 19:30:03.000000 grimo-0.1.2/tests/test_storage.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3283 2024-05-30 19:30:03.000000 grimo-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:53:31.187903 grimo-0.1.3/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1071 2024-05-30 19:18:47.000000 grimo-0.1.3/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    12510 2024-05-30 19:53:31.187696 grimo-0.1.3/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11853 2024-05-30 19:50:11.000000 grimo-0.1.3/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:53:31.185952 grimo-0.1.3/grimo/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4292 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/README_USAGE.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3695 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11250 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/cli.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5637 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/core.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4938 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/package.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      309 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/req_cli.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      366 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/req_readme.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5993 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/storage.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1549 2024-05-30 19:30:03.000000 grimo-0.1.3/grimo/utils.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:53:31.186709 grimo-0.1.3/grimo.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    12510 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      438 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       41 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       54 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        6 2024-05-30 19:53:31.000000 grimo-0.1.3/grimo.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-30 19:53:31.187949 grimo-0.1.3/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1257 2024-05-30 19:52:53.000000 grimo-0.1.3/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-30 19:53:31.187384 grimo-0.1.3/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3528 2024-05-30 19:30:03.000000 grimo-0.1.3/tests/test_core.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3159 2024-05-30 19:30:03.000000 grimo-0.1.3/tests/test_package.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2993 2024-05-30 19:30:03.000000 grimo-0.1.3/tests/test_storage.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3283 2024-05-30 19:30:03.000000 grimo-0.1.3/tests/test_utils.py
```

### Comparing `grimo-0.1.2/LICENSE` & `grimo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/PKG-INFO` & `grimo-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,77 @@
-Metadata-Version: 2.1
-Name: grimo
-Version: 0.1.2
-Summary: Abstract Programming Language Package Manager
-Home-page: https://github.com/dai-motoki/grimo
-Author: dai motoki
-Author-email: dai.motoki@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# 抽象プログラミング言語パッケージマネージャー「grimo」
 
-## Pythonパッケージ開発のための要件定義書
 
-### ゴール: 抽象プログラミング言語パッケージマネージャー「grimo」をPythonで作成
+## 0. 利用方法
+＊ 現在パッケージマネージャーは各々ご自身のAWSアカウントにおけるS3バケットに格納する形になっています。
+バージョンアップに従って、全員共有バケットにする予定です。
 
 
-## 0. 利用方法
+1. grimo install
+```
+pip install grimo
+```
+
+2. AWSのバケットとしてgrimoを作成
+
+3. AWSのローカル設定を行う
+```
+export AWS_SECRET_ACCESS_KEY=xxx
+export AWS_ACCESS_KEY_ID=xxx
+```
 
 ### コマンドラインオプション
 ```
                         利用可能なサブコマンド
     install             パッケージをインストールする（利用可）
     upload              パッケージをアップロードする（利用可）
     search              パッケージを検索する（未開発）
     update              パッケージをアップデートする（未開発）
     uninstall           パッケージをアンインストールする（未開発）
 ```
 
 ### パッケージのアップロード
 
 ```
-grimo upload .
 
 project/
 ├── metadata.json # パッケージのメタデータ
 ├── package_name/
 │   ├── def.md # パッケージの定義
 │   ├── util.md # パッケージのユーティリティ
 │   ├── var.md # パッケージの変数
 │   └── ...
+
+```
+
+```metadata.json
+
+{
+  "name": "package_name",
+  "version": "1.0.0",
+  "language": "python",
+  "description": "package_description",
+  "category": "ai",
+  "tags": [
+    "tool",
+    "development"
+  ]
+}
+```
+
+project ディレクトリ内で
+```
+grimo upload .
+
 ```
 
 ### パッケージのインストール
 
+インストールされたファイルはgrimoiresディレクトリに格納されます。
+
 ```
 grimo install package_name
 
 project/
 ├── grimoires/
 │   ├── package_name/
 │   │   ├── metadata.json # パッケージのメタデータ
@@ -315,8 +334,8 @@
 - チームで開発を行う場合は、GitHub Flow などの開発フローを定義し、円滑な開発を進める
 
 ## 15. 今後の展望
 
 - パッケージの依存関係解決機能の追加
 - 仮想環境管理機能の追加
 - GUIクライアントの開発
-- プラグイン機構による拡張性の向上
+- プラグイン機構による拡張性の向上
```

### Comparing `grimo-0.1.2/README.md` & `grimo-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,95 @@
-## Pythonパッケージ開発のための要件定義書
+Metadata-Version: 2.1
+Name: grimo
+Version: 0.1.3
+Summary: Abstract Programming Language Package Manager
+Home-page: https://github.com/dai-motoki/grimo
+Author: dai motoki
+Author-email: dai.motoki@gmail.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-### ゴール: 抽象プログラミング言語パッケージマネージャー「grimo」をPythonで作成
+# 抽象プログラミング言語パッケージマネージャー「grimo」
 
 
 ## 0. 利用方法
+＊ 現在パッケージマネージャーは各々ご自身のAWSアカウントにおけるS3バケットに格納する形になっています。
+バージョンアップに従って、全員共有バケットにする予定です。
+
+
+1. grimo install
+```
+pip install grimo
+```
+
+2. AWSのバケットとしてgrimoを作成
+
+3. AWSのローカル設定を行う
+```
+export AWS_SECRET_ACCESS_KEY=xxx
+export AWS_ACCESS_KEY_ID=xxx
+```
 
 ### コマンドラインオプション
 ```
                         利用可能なサブコマンド
     install             パッケージをインストールする（利用可）
     upload              パッケージをアップロードする（利用可）
     search              パッケージを検索する（未開発）
     update              パッケージをアップデートする（未開発）
     uninstall           パッケージをアンインストールする（未開発）
 ```
 
 ### パッケージのアップロード
 
 ```
-grimo upload .
 
 project/
 ├── metadata.json # パッケージのメタデータ
 ├── package_name/
 │   ├── def.md # パッケージの定義
 │   ├── util.md # パッケージのユーティリティ
 │   ├── var.md # パッケージの変数
 │   └── ...
+
+```
+
+```metadata.json
+
+{
+  "name": "package_name",
+  "version": "1.0.0",
+  "language": "python",
+  "description": "package_description",
+  "category": "ai",
+  "tags": [
+    "tool",
+    "development"
+  ]
+}
+```
+
+project ディレクトリ内で
+```
+grimo upload .
+
 ```
 
 ### パッケージのインストール
 
+インストールされたファイルはgrimoiresディレクトリに格納されます。
+
 ```
 grimo install package_name
 
 project/
 ├── grimoires/
 │   ├── package_name/
 │   │   ├── metadata.json # パッケージのメタデータ
@@ -297,8 +352,8 @@
 - チームで開発を行う場合は、GitHub Flow などの開発フローを定義し、円滑な開発を進める
 
 ## 15. 今後の展望
 
 - パッケージの依存関係解決機能の追加
 - 仮想環境管理機能の追加
 - GUIクライアントの開発
-- プラグイン機構による拡張性の向上
+- プラグイン機構による拡張性の向上
```

### Comparing `grimo-0.1.2/grimo/README_USAGE.md` & `grimo-0.1.3/grimo/README_USAGE.md`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/grimo/__init__.py` & `grimo-0.1.3/grimo/__init__.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/grimo/cli.py` & `grimo-0.1.3/grimo/cli.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/grimo/core.py` & `grimo-0.1.3/grimo/core.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/grimo/package.py` & `grimo-0.1.3/grimo/package.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/grimo/storage.py` & `grimo-0.1.3/grimo/storage.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/grimo/utils.py` & `grimo-0.1.3/grimo/utils.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/grimo.egg-info/PKG-INFO` & `grimo-0.1.3/grimo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Abstract Programming Language Package Manager
 Home-page: https://github.com/dai-motoki/grimo
 Author: dai motoki
 Author-email: dai.motoki@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,47 +12,84 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Pythonパッケージ開発のための要件定義書
-
-### ゴール: 抽象プログラミング言語パッケージマネージャー「grimo」をPythonで作成
+# 抽象プログラミング言語パッケージマネージャー「grimo」
 
 
 ## 0. 利用方法
+＊ 現在パッケージマネージャーは各々ご自身のAWSアカウントにおけるS3バケットに格納する形になっています。
+バージョンアップに従って、全員共有バケットにする予定です。
+
+
+1. grimo install
+```
+pip install grimo
+```
+
+2. AWSのバケットとしてgrimoを作成
+
+3. AWSのローカル設定を行う
+```
+export AWS_SECRET_ACCESS_KEY=xxx
+export AWS_ACCESS_KEY_ID=xxx
+```
 
 ### コマンドラインオプション
 ```
                         利用可能なサブコマンド
     install             パッケージをインストールする（利用可）
     upload              パッケージをアップロードする（利用可）
     search              パッケージを検索する（未開発）
     update              パッケージをアップデートする（未開発）
     uninstall           パッケージをアンインストールする（未開発）
 ```
 
 ### パッケージのアップロード
 
 ```
-grimo upload .
 
 project/
 ├── metadata.json # パッケージのメタデータ
 ├── package_name/
 │   ├── def.md # パッケージの定義
 │   ├── util.md # パッケージのユーティリティ
 │   ├── var.md # パッケージの変数
 │   └── ...
+
+```
+
+```metadata.json
+
+{
+  "name": "package_name",
+  "version": "1.0.0",
+  "language": "python",
+  "description": "package_description",
+  "category": "ai",
+  "tags": [
+    "tool",
+    "development"
+  ]
+}
+```
+
+project ディレクトリ内で
+```
+grimo upload .
+
 ```
 
 ### パッケージのインストール
 
+インストールされたファイルはgrimoiresディレクトリに格納されます。
+
 ```
 grimo install package_name
 
 project/
 ├── grimoires/
 │   ├── package_name/
 │   │   ├── metadata.json # パッケージのメタデータ
```

### Comparing `grimo-0.1.2/setup.py` & `grimo-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='grimo',
-    version='0.1.2',
+    version='0.1.3',
     description='Abstract Programming Language Package Manager',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',  # 追加: long_descriptionの形式を指定
     author='dai motoki',
     author_email='dai.motoki@gmail.com',
     url='https://github.com/dai-motoki/grimo',
     packages=find_packages(exclude=['tests']),
```

### Comparing `grimo-0.1.2/tests/test_core.py` & `grimo-0.1.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/tests/test_package.py` & `grimo-0.1.3/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/tests/test_storage.py` & `grimo-0.1.3/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `grimo-0.1.2/tests/test_utils.py` & `grimo-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

