# Comparing `tmp/phones_local-0.0.37.tar.gz` & `tmp/phones_local-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.37.tar", last modified: Thu May 30 15:30:07 2024, max compression
+gzip compressed data, was "phones_local-0.0.38.tar", last modified: Thu May 30 16:30:38 2024, max compression
```

## Comparing `phones_local-0.0.37.tar` & `phones_local-0.0.38.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.197425 phones_local-0.0.37/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-30 15:30:07.197425 phones_local-0.0.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-30 15:29:23.000000 phones_local-0.0.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.193425 phones_local-0.0.37/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.197425 phones_local-0.0.37/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:29:23.000000 phones_local-0.0.37/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 15:29:23.000000 phones_local-0.0.37/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-05-30 15:29:23.000000 phones_local-0.0.37/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.197425 phones_local-0.0.37/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-30 15:30:07.000000 phones_local-0.0.37/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 15:30:07.000000 phones_local-0.0.37/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:30:07.000000 phones_local-0.0.37/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 15:30:07.000000 phones_local-0.0.37/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:30:07.000000 phones_local-0.0.37/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-30 15:29:43.000000 phones_local-0.0.37/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:30:07.197425 phones_local-0.0.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 15:29:23.000000 phones_local-0.0.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:30:38.114360 phones_local-0.0.38/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-30 16:30:38.114360 phones_local-0.0.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-30 16:30:10.000000 phones_local-0.0.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:30:38.114360 phones_local-0.0.38/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:30:38.114360 phones_local-0.0.38/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:30:10.000000 phones_local-0.0.38/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 16:30:10.000000 phones_local-0.0.38/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-05-30 16:30:10.000000 phones_local-0.0.38/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:30:38.114360 phones_local-0.0.38/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-30 16:30:38.000000 phones_local-0.0.38/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 16:30:38.000000 phones_local-0.0.38/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:30:38.000000 phones_local-0.0.38/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 16:30:38.000000 phones_local-0.0.38/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 16:30:38.000000 phones_local-0.0.38/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-30 16:30:17.000000 phones_local-0.0.38/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:30:38.114360 phones_local-0.0.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 16:30:10.000000 phones_local-0.0.38/setup.py
```

### Comparing `phones_local-0.0.37/PKG-INFO` & `phones_local-0.0.38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.37
+Version: 0.0.38
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.37/README.md` & `phones_local-0.0.38/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.37/phones_local/src/phone_local_constans.py` & `phones_local-0.0.38/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.37/phones_local/src/phones_local.py` & `phones_local-0.0.38/phones_local/src/phones_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,16 @@
             'international_code': normalized_phone_number['international_code'],
             'full_number_normalized': normalized_phone_number['full_number_normalized'],
             'local_number_normalized': int(str(normalized_phone_number['full_number_normalized'])
                                            .replace(str(normalized_phone_number['international_code']), '')),
             'created_user_id': logger.user_context.get_effective_user_id(),
         }
         phone_compare_data_dict = {
-            "number_original": phone_dict.get("number_original"),
             "full_number_normalized": phone_dict.get("full_number_normalized"),
-            "local_number_normalized": phone_dict.get("local_number_normalized"),
+            "full_number_normalized": '+' + phone_dict.get("full_number_normalized"),   # TODO: delete this line when we won't have '+' in any full_number_normalized entry
         }
         phone_id = self.upsert(data_dict=phone_dict, data_dict_compare=phone_compare_data_dict,
                                view_table_name="phone_view", table_name="phone_table",
                                compare_with_or=True)
 
         # link phone to profile
         if profile_id is not None:
```

### Comparing `phones_local-0.0.37/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.38/phones_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.37
+Version: 0.0.38
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.37/pyproject.toml` & `phones_local-0.0.38/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.37/setup.py` & `phones_local-0.0.38/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.37',  # https://pypi.org/project/phones-local/
+    version='0.0.38',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

