# Comparing `tmp/phones_local-0.0.35.tar.gz` & `tmp/phones_local-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.35.tar", last modified: Tue May 28 17:24:29 2024, max compression
+gzip compressed data, was "phones_local-0.0.36.tar", last modified: Wed May 29 19:24:13 2024, max compression
```

## Comparing `phones_local-0.0.35.tar` & `phones_local-0.0.36.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:24:29.387309 phones_local-0.0.35/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 17:24:29.387309 phones_local-0.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-28 17:23:53.000000 phones_local-0.0.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:24:29.383309 phones_local-0.0.35/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:24:29.387309 phones_local-0.0.35/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:23:53.000000 phones_local-0.0.35/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 17:23:53.000000 phones_local-0.0.35/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-05-28 17:23:53.000000 phones_local-0.0.35/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:24:29.387309 phones_local-0.0.35/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 17:24:29.000000 phones_local-0.0.35/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-28 17:24:29.000000 phones_local-0.0.35/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:24:29.000000 phones_local-0.0.35/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 17:24:29.000000 phones_local-0.0.35/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 17:24:29.000000 phones_local-0.0.35/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-28 17:23:59.000000 phones_local-0.0.35/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:24:29.387309 phones_local-0.0.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 17:23:53.000000 phones_local-0.0.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:13.944059 phones_local-0.0.36/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 19:24:13.944059 phones_local-0.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-29 19:23:43.000000 phones_local-0.0.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:13.940059 phones_local-0.0.36/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:13.944059 phones_local-0.0.36/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:43.000000 phones_local-0.0.36/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-29 19:23:43.000000 phones_local-0.0.36/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-29 19:23:43.000000 phones_local-0.0.36/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:13.944059 phones_local-0.0.36/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 19:24:13.000000 phones_local-0.0.36/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-29 19:24:13.000000 phones_local-0.0.36/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:24:13.000000 phones_local-0.0.36/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-29 19:24:13.000000 phones_local-0.0.36/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 19:24:13.000000 phones_local-0.0.36/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-29 19:23:50.000000 phones_local-0.0.36/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:24:13.944059 phones_local-0.0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 19:23:43.000000 phones_local-0.0.36/setup.py
```

### Comparing `phones_local-0.0.35/PKG-INFO` & `phones_local-0.0.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.35
+Version: 0.0.36
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.35/README.md` & `phones_local-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.35/phones_local/src/phone_local_constans.py` & `phones_local-0.0.36/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.35/phones_local/src/phones_local.py` & `phones_local-0.0.36/phones_local/src/phones_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
             "full_number_normalized": "+972549338666"
         }
         """
         try:
             parsed_number = parse(original_number, region)
             international_code = parsed_number.country_code
             full_number_normalized = format_number(parsed_number, PhoneNumberFormat.E164)
-            # if full_number_normalized.startswith("+"):
-            #     full_number_normalized = full_number_normalized[1:]
+            if full_number_normalized.startswith("+"):
+                full_number_normalized = full_number_normalized[1:]
             # parsed_number example: original_number='0687473298' -> PhoneNumber(country_code=972, national_number=687473298, extension=None, italian_leading_zero=None, number_of_leading_zeros=None, country_code_source=0, preferred_domestic_carrier_code=None)
             # TODO: Shall we add area_code? what shall it be? How can we do it?
             # TODO Can we move number_info to data member in PhoneLocal class
             number_info = {
                 "number_original": original_number,
                 "international_code": international_code,
                 "full_number_normalized": full_number_normalized,
@@ -208,10 +208,10 @@
             'extension': number_original[3],
         }
         test_phone_id = self.insert_phone(phone_data=phone_data)
         return test_phone_id
 
     @staticmethod
     def generate_fake_phone_number(prefix: str = "05", length: int = 8) -> str:
-        remaining_digits = ''.join(random.choices(string.digits, k=length - len(prefix)))
+        remaining_digits = ''.join(random.choices(string.digits, k=length))
         fake_phone_number = prefix + remaining_digits
-        return fake_phone_number
+        return fake_phone_number
```

### Comparing `phones_local-0.0.35/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.36/phones_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.35
+Version: 0.0.36
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.35/pyproject.toml` & `phones_local-0.0.36/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.35/setup.py` & `phones_local-0.0.36/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.35',  # https://pypi.org/project/phones-local/
+    version='0.0.36',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

