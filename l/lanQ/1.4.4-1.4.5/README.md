# Comparing `tmp/lanQ-1.4.4.tar.gz` & `tmp/lanQ-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanQ-1.4.4.tar", last modified: Thu May 23 07:46:27 2024, max compression
+gzip compressed data, was "lanQ-1.4.5.tar", last modified: Thu May 30 09:22:44 2024, max compression
```

## Comparing `lanQ-1.4.4.tar` & `lanQ-1.4.5.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.812489 lanQ-1.4.4/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-05-23 07:46:27.812489 lanQ-1.4.4/PKG-INFO
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     9785 2024-05-20 03:00:14.000000 lanQ-1.4.4/README.md
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.808490 lanQ-1.4.4/convert/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      574 2024-05-22 10:16:37.000000 lanQ-1.4.4/convert/__init__.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      324 2024-05-22 10:18:04.000000 lanQ-1.4.4/convert/alpaca.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      300 2024-05-22 07:06:56.000000 lanQ-1.4.4/convert/audio_ar.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      357 2024-05-21 05:51:01.000000 lanQ-1.4.4/convert/json_file.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      305 2024-05-21 08:02:04.000000 lanQ-1.4.4/convert/json_line.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      291 2024-05-21 05:47:42.000000 lanQ-1.4.4/convert/string_line.py
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.808490 lanQ-1.4.4/lanQ.egg-info/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-05-23 07:46:27.000000 lanQ-1.4.4/lanQ.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      779 2024-05-23 07:46:27.000000 lanQ-1.4.4/lanQ.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        1 2024-05-23 07:46:27.000000 lanQ-1.4.4/lanQ.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       29 2024-05-23 07:46:27.000000 lanQ-1.4.4/lanQ.egg-info/top_level.txt
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.808490 lanQ-1.4.4/lanQ_model/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-18 10:56:29.000000 lanQ-1.4.4/lanQ_model/__init__.py
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.808490 lanQ-1.4.4/lanQ_model/base_func/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-18 10:56:29.000000 lanQ-1.4.4/lanQ_model/base_func/__init__.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    15911 2024-05-10 05:37:15.000000 lanQ-1.4.4/lanQ_model/base_func/base.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    15517 2024-05-10 05:37:15.000000 lanQ-1.4.4/lanQ_model/base_func/base_api.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     8630 2024-05-10 05:37:15.000000 lanQ-1.4.4/lanQ_model/base_func/openai_api.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     5611 2024-05-10 05:37:15.000000 lanQ-1.4.4/lanQ_model/base_func/turbomind_api.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1528 2024-05-22 07:08:13.000000 lanQ-1.4.4/lanQ_model/gpt.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     2757 2024-05-21 02:45:55.000000 lanQ-1.4.4/lanQ_model/llama3.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     2104 2024-05-20 08:56:37.000000 lanQ-1.4.4/lanQ_model/perspective.py
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.808490 lanQ-1.4.4/lanQ_rule/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-18 10:56:29.000000 lanQ-1.4.4/lanQ_rule/__init__.py
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.812489 lanQ-1.4.4/lanQ_rule/base_func/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 07:11:32.000000 lanQ-1.4.4/lanQ_rule/base_func/__init__.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     4593 2024-04-26 08:10:06.000000 lanQ-1.4.4/lanQ_rule/base_func/base.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    14875 2024-05-22 08:18:06.000000 lanQ-1.4.4/lanQ_rule/common_rule.py
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.812489 lanQ-1.4.4/lanQ_rule/config/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-20 06:41:14.000000 lanQ-1.4.4/lanQ_rule/config/__init__.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1852 2024-05-20 06:52:10.000000 lanQ-1.4.4/lanQ_rule/config/const.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      230 2024-04-30 03:33:52.000000 lanQ-1.4.4/lanQ_rule/config/customize.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1117 2024-05-20 06:09:13.000000 lanQ-1.4.4/lanQ_rule/config/rule_map.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      902 2024-05-20 06:54:36.000000 lanQ-1.4.4/lanQ_rule/model_rule.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1040 2024-05-20 06:54:36.000000 lanQ-1.4.4/lanQ_rule/prompt_rule.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       38 2024-05-23 07:46:27.812489 lanQ-1.4.4/setup.cfg
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      394 2024-05-23 07:46:01.000000 lanQ-1.4.4/setup.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-30 09:22:44.148225 lanQ-1.4.5/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-05-30 09:22:44.148225 lanQ-1.4.5/PKG-INFO
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     9785 2024-05-27 03:06:42.000000 lanQ-1.4.5/README.md
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-30 09:22:44.144225 lanQ-1.4.5/convert/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-27 03:06:42.000000 lanQ-1.4.5/convert/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     2679 2024-05-30 02:33:19.000000 lanQ-1.4.5/convert/data.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-30 09:22:44.144225 lanQ-1.4.5/lanQ.egg-info/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-05-30 09:22:44.000000 lanQ-1.4.5/lanQ.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      753 2024-05-30 09:22:44.000000 lanQ-1.4.5/lanQ.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        1 2024-05-30 09:22:44.000000 lanQ-1.4.5/lanQ.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       39 2024-05-30 09:22:44.000000 lanQ-1.4.5/lanQ.egg-info/top_level.txt
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-30 09:22:44.144225 lanQ-1.4.5/lanQ_model/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_model/__init__.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-30 09:22:44.144225 lanQ-1.4.5/lanQ_model/base_func/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_model/base_func/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    15911 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_model/base_func/base.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    15517 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_model/base_func/base_api.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     8630 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_model/base_func/openai_api.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     5611 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_model/base_func/turbomind_api.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1528 2024-05-29 10:49:21.000000 lanQ-1.4.5/lanQ_model/gpt.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     2757 2024-05-30 03:24:05.000000 lanQ-1.4.5/lanQ_model/llama3.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     2104 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_model/perspective.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-30 09:22:44.148225 lanQ-1.4.5/lanQ_rule/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_rule/__init__.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-30 09:22:44.148225 lanQ-1.4.5/lanQ_rule/base_func/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_rule/base_func/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     4593 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_rule/base_func/base.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    14875 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_rule/common_rule.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-30 09:22:44.148225 lanQ-1.4.5/lanQ_rule/config/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_rule/config/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1852 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_rule/config/const.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      230 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_rule/config/customize.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1457 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_rule/config/rule_map.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      902 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_rule/model_rule.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1040 2024-05-27 03:06:42.000000 lanQ-1.4.5/lanQ_rule/prompt_rule.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-30 09:22:44.148225 lanQ-1.4.5/run/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-27 03:06:42.000000 lanQ-1.4.5/run/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     7285 2024-05-30 02:32:19.000000 lanQ-1.4.5/run/run.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       38 2024-05-30 09:22:44.148225 lanQ-1.4.5/setup.cfg
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      394 2024-05-30 09:22:37.000000 lanQ-1.4.5/setup.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-30 09:22:44.148225 lanQ-1.4.5/spark/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-29 08:24:13.000000 lanQ-1.4.5/spark/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     3405 2024-05-30 09:00:11.000000 lanQ-1.4.5/spark/common.py
```

### Comparing `lanQ-1.4.4/README.md` & `lanQ-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ.egg-info/SOURCES.txt` & `lanQ-1.4.5/lanQ.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 README.md
 setup.py
 convert/__init__.py
-convert/alpaca.py
-convert/audio_ar.py
-convert/json_file.py
-convert/json_line.py
-convert/string_line.py
+convert/data.py
 lanQ.egg-info/PKG-INFO
 lanQ.egg-info/SOURCES.txt
 lanQ.egg-info/dependency_links.txt
 lanQ.egg-info/top_level.txt
 lanQ_model/__init__.py
 lanQ_model/gpt.py
 lanQ_model/llama3.py
@@ -24,8 +20,12 @@
 lanQ_rule/model_rule.py
 lanQ_rule/prompt_rule.py
 lanQ_rule/base_func/__init__.py
 lanQ_rule/base_func/base.py
 lanQ_rule/config/__init__.py
 lanQ_rule/config/const.py
 lanQ_rule/config/customize.py
-lanQ_rule/config/rule_map.py
+lanQ_rule/config/rule_map.py
+run/__init__.py
+run/run.py
+spark/__init__.py
+spark/common.py
```

### Comparing `lanQ-1.4.4/lanQ_model/base_func/base.py` & `lanQ-1.4.5/lanQ_model/base_func/base.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_model/base_func/base_api.py` & `lanQ-1.4.5/lanQ_model/base_func/base_api.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_model/base_func/openai_api.py` & `lanQ-1.4.5/lanQ_model/base_func/openai_api.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_model/base_func/turbomind_api.py` & `lanQ-1.4.5/lanQ_model/base_func/turbomind_api.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_model/gpt.py` & `lanQ-1.4.5/lanQ_model/gpt.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_model/llama3.py` & `lanQ-1.4.5/lanQ_model/llama3.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_model/perspective.py` & `lanQ-1.4.5/lanQ_model/perspective.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_rule/base_func/base.py` & `lanQ-1.4.5/lanQ_rule/base_func/base.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_rule/common_rule.py` & `lanQ-1.4.5/lanQ_rule/common_rule.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_rule/config/const.py` & `lanQ-1.4.5/lanQ_rule/config/const.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_rule/config/rule_map.py` & `lanQ-1.4.5/lanQ_rule/config/rule_map.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,7 +41,22 @@
     common_special_mark,
     common_joint_special_symbol,
     common_underscore_length,
     common_ellipsis_ratio,
     common_invalid_web,
     common_emoj_characters,
 ]
+arabic_all = [
+    common_enter_more,
+    common_content_null,
+    common_space_more,
+    common_url_only,
+    common_colon_end,
+    common_check_photo,
+    common_img_html_tag,
+    common_special_character,
+    common_enter_ratio_more,
+    common_doc_repeat,
+    common_html_entity,
+    common_invisible_char,
+    common_bracket_unmatch,
+]
```

### Comparing `lanQ-1.4.4/lanQ_rule/model_rule.py` & `lanQ-1.4.5/lanQ_rule/model_rule.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.4/lanQ_rule/prompt_rule.py` & `lanQ-1.4.5/lanQ_rule/prompt_rule.py`

 * *Files identical despite different names*

