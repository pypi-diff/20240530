# Comparing `tmp/pp_weight_estimation-1.1.26.tar.gz` & `tmp/pp_weight_estimation-1.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pp_weight_estimation-1.1.26.tar", last modified: Wed May 29 19:51:12 2024, max compression
+gzip compressed data, was "pp_weight_estimation-1.1.27.tar", last modified: Thu May 30 01:40:58 2024, max compression
```

## Comparing `pp_weight_estimation-1.1.26.tar` & `pp_weight_estimation-1.1.27.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.26/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.287520 pp_weight_estimation-1.1.26/pp_weight_estimation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/pp_weight_estimation/core/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/core/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     9537 2024-05-29 19:11:15.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/core/function_test.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6712 2024-05-29 12:30:55.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/core/get_weight.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/core/gpt_support.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1643 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/core/s3_io.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/pp_weight_estimation/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/utils/slack_connect.py
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/utils/visulizer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-29 19:51:00.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/version.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-29 19:51:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-05-29 19:51:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-29 19:51:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-29 19:51:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-05-29 19:51:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.26/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.287520 pp_weight_estimation-1.1.26/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.26/scripts/weight_pred.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.26/setup.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/tests/
--rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.26/tests/test_function_test.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.324910 pp_weight_estimation-1.1.27/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.27/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/pp_weight_estimation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/pp_weight_estimation/core/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/core/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     9537 2024-05-30 01:40:37.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/core/function_test.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6712 2024-05-29 12:30:55.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/core/get_weight.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/core/gpt_support.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1643 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/core/s3_io.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/pp_weight_estimation/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/utils/slack_connect.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/utils/visulizer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-30 01:40:49.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/version.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-30 01:40:58.000000 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-05-30 01:40:58.000000 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-30 01:40:58.000000 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-30 01:40:58.000000 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-05-30 01:40:58.000000 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.27/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.27/scripts/weight_pred.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-30 01:40:58.324910 pp_weight_estimation-1.1.27/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.27/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/tests/
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.27/tests/test_function_test.py
```

### Comparing `pp_weight_estimation-1.1.26/pp_weight_estimation/core/function_test.py` & `pp_weight_estimation-1.1.27/pp_weight_estimation/core/function_test.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.26/pp_weight_estimation/core/get_weight.py` & `pp_weight_estimation-1.1.27/pp_weight_estimation/core/get_weight.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.26/pp_weight_estimation/core/gpt_support.py` & `pp_weight_estimation-1.1.27/pp_weight_estimation/core/gpt_support.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.26/pp_weight_estimation/core/s3_io.py` & `pp_weight_estimation-1.1.27/pp_weight_estimation/core/s3_io.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.26/pp_weight_estimation/utils/slack_connect.py` & `pp_weight_estimation-1.1.27/pp_weight_estimation/utils/slack_connect.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/SOURCES.txt` & `pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.26/setup.py` & `pp_weight_estimation-1.1.27/setup.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.26/tests/test_function_test.py` & `pp_weight_estimation-1.1.27/tests/test_function_test.py`

 * *Files identical despite different names*

