# Comparing `tmp/konfuzio_sdk-0.3.7.dev20240524130943.tar.gz` & `tmp/konfuzio_sdk-0.3.7.dev20240528095544.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konfuzio_sdk-0.3.7.dev20240524130943.tar", last modified: Sat May 25 03:30:27 2024, max compression
+gzip compressed data, was "konfuzio_sdk-0.3.7.dev20240528095544.tar", last modified: Wed May 29 03:29:22 2024, max compression
```

## Comparing `konfuzio_sdk-0.3.7.dev20240524130943.tar` & `konfuzio_sdk-0.3.7.dev20240528095544.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 03:30:27.551406 konfuzio_sdk-0.3.7.dev20240524130943/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-25 03:30:27.551406 konfuzio_sdk-0.3.7.dev20240524130943/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 03:30:27.543406 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   209636 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    27953 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/settings_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 03:30:27.543406 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/tokenizer/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 03:30:27.547406 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/document_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    51688 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/file_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/image.py
--rw-r--r--   0 runner    (1001) docker     (127)   102313 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/information_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 03:30:27.547406 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-25 03:30:27.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-25 03:30:27.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 03:30:27.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-25 03:30:27.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-25 03:30:27.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-25 03:30:27.000000 konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 03:30:27.551406 konfuzio_sdk-0.3.7.dev20240524130943/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 03:30:27.547406 konfuzio_sdk-0.3.7.dev20240524130943/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23654 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   169183 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/tests/test_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-05-25 03:30:19.000000 konfuzio_sdk-0.3.7.dev20240524130943/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:29:22.474626 konfuzio_sdk-0.3.7.dev20240528095544/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-29 03:29:22.474626 konfuzio_sdk-0.3.7.dev20240528095544/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:29:22.466626 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   209636 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27953 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/settings_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:29:22.466626 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/tokenizer/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:29:22.470625 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75855 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/document_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53090 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/file_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102313 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/information_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:29:22.470625 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-29 03:29:22.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-29 03:29:22.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:29:22.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 03:29:22.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 03:29:22.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 03:29:22.000000 konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:29:22.474626 konfuzio_sdk-0.3.7.dev20240528095544/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:29:22.470625 konfuzio_sdk-0.3.7.dev20240528095544/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23654 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169183 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/tests/test_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-05-29 03:29:14.000000 konfuzio_sdk-0.3.7.dev20240528095544/tests/test_utils.py
```

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/LICENSE.md` & `konfuzio_sdk-0.3.7.dev20240528095544/LICENSE.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/PKG-INFO` & `konfuzio_sdk-0.3.7.dev20240528095544/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.7.dev20240524130943
+Version: 0.3.7.dev20240528095544
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/README.md` & `konfuzio_sdk-0.3.7.dev20240528095544/README.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/api.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/cli.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/data.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/evaluate.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/extras.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/normalize.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/regex.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/samples.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/settings_importer.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/settings_importer.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/tokenizer/base.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/tokenizer/paragraph_and_sentence.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/tokenizer/paragraph_and_sentence.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/tokenizer/regex.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/tokenizer/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/base.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/document_categorization.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/document_categorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 from konfuzio_sdk.extras import (
     DataLoader,
     FloatTensor,
     LongTensor,
     Module,
     Optimizer,
     Tensor,
-    evaluate,
     timm,
     torch,
     torch_no_grad,
     torchvision,
     transformers,
 )
 from konfuzio_sdk.tokenizer.base import AbstractTokenizer, Vocab
 from konfuzio_sdk.tokenizer.regex import WhitespaceTokenizer
 from konfuzio_sdk.trainer.base import BaseModel
 from konfuzio_sdk.trainer.image import ImageDataAugmentation, ImagePreProcessing
 from konfuzio_sdk.trainer.tokenization import TransformersTokenizer
+from konfuzio_sdk.trainer.utils import load_metric
 from konfuzio_sdk.utils import get_timestamp
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractCategorizationAI(BaseModel, metaclass=abc.ABCMeta):
     """Abstract definition of a CategorizationAI."""
@@ -1294,16 +1294,18 @@
         train_losses = []
         patience_counter = 0
         loss_fn = torch.nn.CrossEntropyLoss()
         optimizer = get_optimizer(self.classifier, optimizer)
         scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=0, factor=lr_decay)
         temp_dir = tempfile.gettempdir()
         temp_filename = os.path.join(temp_dir, f'temp_{uuid.uuid4().hex}.pt')
-        f1_metric = evaluate.load('f1')
-        acc_metric = evaluate.load('accuracy')
+        # defining transformers cache location to load the metrics
+        transformers_cache_location = os.getenv('TRANSFORMERS_CACHE')
+        f1_metric = load_metric('f1', path=transformers_cache_location)
+        acc_metric = load_metric('accuracy', path=transformers_cache_location)
         logger.info('Begin fitting')
         best_valid_loss = float('inf')
         train_loss = float('inf')
         for epoch in range(n_epochs):
             train_loss, predictions_list, ground_truth_list = self._train(
                 train_examples, loss_fn, optimizer
             )  # train epoch
```

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/file_splitting.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/file_splitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 import numpy as np
 import pandas as pd
 import PIL
 from sklearn.utils.class_weight import compute_class_weight
 
 from konfuzio_sdk.data import Category, Document, Page
 from konfuzio_sdk.evaluate import FileSplittingEvaluation
-from konfuzio_sdk.extras import datasets, evaluate, mlflow, tensorflow as tf, torch, transformers
+from konfuzio_sdk.extras import datasets, mlflow, tensorflow as tf, torch, transformers
 from konfuzio_sdk.trainer.information_extraction import BaseModel
-from konfuzio_sdk.trainer.utils import BalancedLossTrainer, LoggerCallback
+from konfuzio_sdk.trainer.utils import BalancedLossTrainer, LoggerCallback, load_metric
 from konfuzio_sdk.utils import get_timestamp
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractFileSplittingModel(BaseModel, metaclass=abc.ABCMeta):
     """Abstract class for the File Splitting model."""
@@ -544,14 +544,39 @@
                     labels.append(1)
                 else:
                     labels.append(0)
         if return_images:
             return page_images, texts, labels
         return texts, labels
 
+    def _load_model_and_tokenizer(self, path: str):
+        """
+        Private method to load the model and tokenizer from the HuggingFace Cache.
+        If one of the model or it's tokenizer is not to be found in the cache, it will be downloaded from the HuggingFace Hub.
+
+        :param path: The path to the transformers cache.
+        :type path: str
+        :returns: The model and it's tokenizer.
+        """
+
+        # try to get the model & it's tokenizer from the transformers cache first
+        try:
+            transformers_tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_name, cache_dir=path)
+            model = transformers.AutoModelForSequenceClassification.from_pretrained(
+                self.model_name, cache_dir=path, num_labels=2
+            )
+            logger.info(f'Model and tokenizer {self.model_name} loaded successfully from the transformers cache.')
+        # if the model is not found in the cache, download it from the HuggingFace Hub
+        except OSError:
+            logger.warning('Could not find the model in the transformers cache. Downloading it from HuggingFace Hub.')
+            transformers_tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_name)
+            model = transformers.AutoModelForSequenceClassification.from_pretrained(self.model_name, num_labels=2)
+
+        return model, transformers_tokenizer
+
     def fit(
         self,
         epochs: int = 5,
         eval_batch_size: int = 8,
         train_batch_size: int = 8,
         device: str = 'cpu',
         *args,
@@ -596,18 +621,22 @@
             class_weights = compute_class_weight('balanced', classes=[0, 1], y=train_labels)
         except ValueError:
             logger.warning(
                 'Your Dataset is composed of only first pages! \
                 You are about to train a Splitting AI for a one class classification task!'
             )
             class_weights = [1, 1]
-        # defining tokenizer
-        self.transformers_tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_name)
+        # defining transformers cache location
+        transformers_cache_location = os.getenv('TRANSFORMERS_CACHE')
+        # defining model & tokenizer
+        self.model, self.transformers_tokenizer = self._load_model_and_tokenizer(path=transformers_cache_location)
+        # move model to device
+        self.model.to(device)
         # defining metric
-        metric = evaluate.load('f1')
+        metric = load_metric(metric_name='f1', path=transformers_cache_location)
 
         # functions to be used by transformers.trainer
         def tokenize_function(examples):
             return self.transformers_tokenizer(examples['text'], truncation=True, padding='max_length')
 
         def compute_metrics(eval_pred):
             predictions, labels = eval_pred
@@ -616,18 +645,14 @@
 
         logger.info('=' * 50)
         logger.info('Tokenizing datasets')
         train_dataset = train_dataset.map(tokenize_function, batched=True)
         test_dataset = test_dataset.map(tokenize_function, batched=True)
         logger.info('=' * 50)
         logger.info('Loading model')
-        # loading the transformers model and defining the training arguments
-        self.model = transformers.AutoModelForSequenceClassification.from_pretrained(self.model_name, num_labels=2)
-        # move model to device
-        self.model.to(device)
         # getting MLflow variables
         experiment_name = kwargs.get('experiment_name', None)
         tracking_uri = kwargs.get('tracking_uri', None)
         # check if both are not None then use MLflow
         self.use_mlflow = experiment_name is not None and tracking_uri is not None
         if self.use_mlflow:
             logger.info(
@@ -767,47 +792,47 @@
 
         This is needed for proper saving of the model in lz4 compressed format – if the dependencies are not removed,
         the resulting pickle will be impossible to load.
         """
         globals()['torch'] = None
         globals()['tf'] = None
         globals()['transformers'] = None
-        globals()['evaluate'] = None
+        globals()['load_metric'] = None
         globals()['datasets'] = None
         globals()['Trainer'] = None
         globals()['BalancedLossTrainer'] = None
         globals()['LoggerCallback'] = None
         globals()['mlflow'] = None
 
         del globals()['torch']
         del globals()['tf']
         del globals()['transformers']
-        del globals()['evaluate']
+        del globals()['load_metric']
         del globals()['datasets']
         del globals()['Trainer']
         del globals()['BalancedLossTrainer']
         del globals()['LoggerCallback']
         del globals()['mlflow']
 
     @staticmethod
     def restore_dependencies():
         """
         Restore removed dependencies after loading.
 
         This is needed for proper functioning of a loaded model because we have previously removed these dependencies
         upon saving the model.
         """
-        from konfuzio_sdk.extras import Trainer, datasets, evaluate, mlflow, tensorflow as tf, torch, transformers
-        from konfuzio_sdk.trainer.utils import BalancedLossTrainer, LoggerCallback
+        from konfuzio_sdk.extras import Trainer, datasets, mlflow, tensorflow as tf, torch, transformers
+        from konfuzio_sdk.trainer.utils import BalancedLossTrainer, LoggerCallback, load_metric
 
         globals()['torch'] = torch
         globals()['tf'] = tf
         globals()['transformers'] = transformers
         globals()['datasets'] = datasets
-        globals()['evalute'] = evaluate
+        globals()['load_metric'] = load_metric
         globals()['Trainer'] = Trainer
         globals()['BalancedLossTrainer'] = BalancedLossTrainer
         globals()['LoggerCallback'] = LoggerCallback
         globals()['mlflow'] = mlflow
 
     def check_is_ready(self):
         """
```

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/image.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/image.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/information_extraction.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/information_extraction.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/trainer/tokenization.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/trainer/tokenization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/urls.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk/utils.py` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk.egg-info/PKG-INFO` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.7.dev20240524130943
+Version: 0.3.7.dev20240528095544
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk.egg-info/SOURCES.txt` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/konfuzio_sdk.egg-info/requires.txt` & `konfuzio_sdk-0.3.7.dev20240528095544/konfuzio_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/setup.py` & `konfuzio_sdk-0.3.7.dev20240528095544/setup.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/tests/test_api.py` & `konfuzio_sdk-0.3.7.dev20240528095544/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/tests/test_cli.py` & `konfuzio_sdk-0.3.7.dev20240528095544/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/tests/test_data.py` & `konfuzio_sdk-0.3.7.dev20240528095544/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/tests/test_evaluate.py` & `konfuzio_sdk-0.3.7.dev20240528095544/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/tests/test_extras.py` & `konfuzio_sdk-0.3.7.dev20240528095544/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/tests/test_normalize.py` & `konfuzio_sdk-0.3.7.dev20240528095544/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/tests/test_regex.py` & `konfuzio_sdk-0.3.7.dev20240528095544/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/tests/test_samples.py` & `konfuzio_sdk-0.3.7.dev20240528095544/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/tests/test_urls.py` & `konfuzio_sdk-0.3.7.dev20240528095544/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.7.dev20240524130943/tests/test_utils.py` & `konfuzio_sdk-0.3.7.dev20240528095544/tests/test_utils.py`

 * *Files identical despite different names*

