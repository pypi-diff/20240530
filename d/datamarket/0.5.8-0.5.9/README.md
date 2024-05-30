# Comparing `tmp/datamarket-0.5.8.tar.gz` & `tmp/datamarket-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.5.8.tar", last modified: Mon Apr 29 18:07:28 2024, max compression
+gzip compressed data, was "datamarket-0.5.9.tar", last modified: Thu May 23 08:09:16 2024, max compression
```

## Comparing `datamarket-0.5.8.tar` & `datamarket-0.5.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 18:07:28.873674 datamarket-0.5.8/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)    35149 2024-04-29 13:44:53.000000 datamarket-0.5.8/LICENSE
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1692 2024-04-29 18:07:28.872674 datamarket-0.5.8/PKG-INFO
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      934 2024-04-29 13:44:53.000000 datamarket-0.5.8/README.md
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       38 2024-04-29 18:07:28.873674 datamarket-0.5.8/setup.cfg
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1080 2024-04-29 18:06:46.000000 datamarket-0.5.8/setup.py
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 18:07:28.862673 datamarket-0.5.8/src/
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 18:07:28.863674 datamarket-0.5.8/src/datamarket/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       12 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/__init__.py
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 18:07:28.869674 datamarket-0.5.8/src/datamarket/interfaces/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/interfaces/__init__.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     4214 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/interfaces/alchemy.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1252 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/interfaces/aws.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2915 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/interfaces/drive.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1344 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/interfaces/ftp.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     3330 2024-04-29 17:59:33.000000 datamarket-0.5.8/src/datamarket/interfaces/nominatim.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2913 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/interfaces/proxy.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2565 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/interfaces/tinybird.py
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 18:07:28.870674 datamarket-0.5.8/src/datamarket/params/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/params/__init__.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1143 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/params/nominatim.py
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 18:07:28.871674 datamarket-0.5.8/src/datamarket/utils/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       20 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/utils/__init__.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      635 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/utils/alchemy.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2270 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/utils/main.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2499 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/utils/selenium.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      941 2024-04-29 13:44:53.000000 datamarket-0.5.8/src/datamarket/utils/soda.py
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 18:07:28.872674 datamarket-0.5.8/src/datamarket.egg-info/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1692 2024-04-29 18:07:28.000000 datamarket-0.5.8/src/datamarket.egg-info/PKG-INFO
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      755 2024-04-29 18:07:28.000000 datamarket-0.5.8/src/datamarket.egg-info/SOURCES.txt
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        1 2024-04-29 18:07:28.000000 datamarket-0.5.8/src/datamarket.egg-info/dependency_links.txt
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       86 2024-04-29 18:07:28.000000 datamarket-0.5.8/src/datamarket.egg-info/requires.txt
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       11 2024-04-29 18:07:28.000000 datamarket-0.5.8/src/datamarket.egg-info/top_level.txt
+drwxr-xr-x   0 chicken   (1000) datamarket   (777)        0 2024-05-23 08:09:16.235913 datamarket-0.5.9/
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)    35149 2024-04-02 06:30:33.000000 datamarket-0.5.9/LICENSE
+-rw-r--r--   0 chicken   (1000) datamarket   (777)     1692 2024-05-23 08:09:16.231913 datamarket-0.5.9/PKG-INFO
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)      934 2024-04-02 06:30:33.000000 datamarket-0.5.9/README.md
+-rw-r--r--   0 chicken   (1000) datamarket   (777)       38 2024-05-23 08:09:16.235913 datamarket-0.5.9/setup.cfg
+-rw-r--r--   0 chicken   (1000) datamarket   (777)     1080 2024-05-23 08:09:10.000000 datamarket-0.5.9/setup.py
+drwxr-xr-x   0 chicken   (1000) datamarket   (777)        0 2024-05-23 08:09:16.207913 datamarket-0.5.9/src/
+drwxr-xr-x   0 chicken   (1000) datamarket   (777)        0 2024-05-23 08:09:16.219913 datamarket-0.5.9/src/datamarket/
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)       12 2024-04-02 06:30:33.000000 datamarket-0.5.9/src/datamarket/__init__.py
+drwxr-xr-x   0 chicken   (1000) datamarket   (777)        0 2024-05-23 08:09:16.227913 datamarket-0.5.9/src/datamarket/interfaces/
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)        0 2024-04-02 06:30:33.000000 datamarket-0.5.9/src/datamarket/interfaces/__init__.py
+-rw-r--r--   0 chicken   (1000) datamarket   (777)     4214 2024-05-23 08:09:04.000000 datamarket-0.5.9/src/datamarket/interfaces/alchemy.py
+-rw-r--r--   0 chicken   (1000) datamarket   (777)     1252 2024-04-02 07:42:08.000000 datamarket-0.5.9/src/datamarket/interfaces/aws.py
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)     2915 2024-05-23 07:03:31.000000 datamarket-0.5.9/src/datamarket/interfaces/drive.py
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)     1344 2024-04-02 06:30:33.000000 datamarket-0.5.9/src/datamarket/interfaces/ftp.py
+-rw-r--r--   0 chicken   (1000) datamarket   (777)     3330 2024-05-23 08:09:04.000000 datamarket-0.5.9/src/datamarket/interfaces/nominatim.py
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)     2913 2024-04-02 06:30:33.000000 datamarket-0.5.9/src/datamarket/interfaces/proxy.py
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)     2565 2024-04-02 06:30:33.000000 datamarket-0.5.9/src/datamarket/interfaces/tinybird.py
+drwxr-xr-x   0 chicken   (1000) datamarket   (777)        0 2024-05-23 08:09:16.227913 datamarket-0.5.9/src/datamarket/params/
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)        0 2024-04-02 06:30:33.000000 datamarket-0.5.9/src/datamarket/params/__init__.py
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)     1143 2024-04-02 06:30:33.000000 datamarket-0.5.9/src/datamarket/params/nominatim.py
+drwxr-xr-x   0 chicken   (1000) datamarket   (777)        0 2024-05-23 08:09:16.231913 datamarket-0.5.9/src/datamarket/utils/
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)       20 2024-04-02 06:30:33.000000 datamarket-0.5.9/src/datamarket/utils/__init__.py
+-rw-r--r--   0 chicken   (1000) datamarket   (777)      635 2024-05-23 08:09:04.000000 datamarket-0.5.9/src/datamarket/utils/alchemy.py
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)     2794 2024-05-23 08:03:57.000000 datamarket-0.5.9/src/datamarket/utils/main.py
+-rw-rw-r--   0 chicken   (1000) datamarket   (777)     2499 2024-04-02 06:30:33.000000 datamarket-0.5.9/src/datamarket/utils/selenium.py
+-rw-r--r--   0 chicken   (1000) datamarket   (777)      941 2024-05-23 08:09:04.000000 datamarket-0.5.9/src/datamarket/utils/soda.py
+drwxr-xr-x   0 chicken   (1000) datamarket   (777)        0 2024-05-23 08:09:16.231913 datamarket-0.5.9/src/datamarket.egg-info/
+-rw-r--r--   0 chicken   (1000) datamarket   (777)     1692 2024-05-23 08:09:16.000000 datamarket-0.5.9/src/datamarket.egg-info/PKG-INFO
+-rw-r--r--   0 chicken   (1000) datamarket   (777)      755 2024-05-23 08:09:16.000000 datamarket-0.5.9/src/datamarket.egg-info/SOURCES.txt
+-rw-r--r--   0 chicken   (1000) datamarket   (777)        1 2024-05-23 08:09:16.000000 datamarket-0.5.9/src/datamarket.egg-info/dependency_links.txt
+-rw-r--r--   0 chicken   (1000) datamarket   (777)       86 2024-05-23 08:09:16.000000 datamarket-0.5.9/src/datamarket.egg-info/requires.txt
+-rw-r--r--   0 chicken   (1000) datamarket   (777)       11 2024-05-23 08:09:16.000000 datamarket-0.5.9/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.5.8/LICENSE` & `datamarket-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/PKG-INFO` & `datamarket-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.5.8
+Version: 0.5.9
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.5.8/README.md` & `datamarket-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/setup.py` & `datamarket-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "undetected_chromedriver",
     "pendulum",
     "boto3",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.5.8",
+    version="0.5.9",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.5.8/src/datamarket/interfaces/alchemy.py` & `datamarket-0.5.9/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket/interfaces/aws.py` & `datamarket-0.5.9/src/datamarket/interfaces/aws.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket/interfaces/drive.py` & `datamarket-0.5.9/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket/interfaces/ftp.py` & `datamarket-0.5.9/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket/interfaces/nominatim.py` & `datamarket-0.5.9/src/datamarket/interfaces/nominatim.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket/interfaces/proxy.py` & `datamarket-0.5.9/src/datamarket/interfaces/proxy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket/interfaces/tinybird.py` & `datamarket-0.5.9/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket/params/nominatim.py` & `datamarket-0.5.9/src/datamarket/params/nominatim.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket/utils/alchemy.py` & `datamarket-0.5.9/src/datamarket/utils/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket/utils/main.py` & `datamarket-0.5.9/src/datamarket/utils/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,31 +24,27 @@
 
 
 def set_logger(level):
     log = logging.getLogger()
     log.setLevel(logging.DEBUG)
     ch = logging.StreamHandler()
     ch.setLevel(level.upper())
-    formatter = logging.Formatter(
-        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    )
+    formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
     ch.setFormatter(formatter)
     log.addHandler(ch)
 
 
 def ban_sleep(max_time, min_time=0):
     sleep_time = int(random.uniform(min_time, max_time))
     logger.info(f"sleeping for {sleep_time} seconds...")
     time.sleep(sleep_time)
 
 
 def run_bash_command(command):
-    p = subprocess.Popen(
-        shlex.split(command), stdout=subprocess.PIPE, stderr=subprocess.STDOUT
-    )
+    p = subprocess.Popen(shlex.split(command), stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
     text_lines = []
     for line_b in iter(p.stdout.readline, ""):
         line_str = line_b.decode().strip()
 
         if not line_str:
             break
@@ -60,17 +56,15 @@
 
 
 def text_to_int(text):
     max_int32 = 2147483647
     try:
         num = int(re.sub(r"[^\d-]", "", text))
 
-        if (
-                -max_int32 < num < max_int32
-        ):  # max integer value (in order to avoid problems on database insertion)
+        if -max_int32 < num < max_int32:  # max integer value (in order to avoid problems on database insertion)
             return num
 
     except ValueError:
         logger.warning(f"unable to parse {text} as integer")
 
 
 def sleep_out_interval(from_h, to_h, tz="Europe/Madrid", seconds=1800):
@@ -79,7 +73,22 @@
         ban_sleep(seconds, seconds)
 
 
 def sleep_in_interval(from_h, to_h, tz="Europe/Madrid", seconds=1800):
     while from_h <= pendulum.now(tz=tz).hour < to_h:
         logger.warning("time to sleep and not scrape anything...")
         ban_sleep(seconds, seconds)
+
+
+def parse_field(dict_struct, field_path, format_method=None):
+    if not isinstance(field_path, list):
+        raise ValueError("Argument field_path must be of type list")
+
+    field_value = dict_struct
+    for field in field_path:
+        if isinstance(field_value, dict):
+            field_value = field_value.get(field)
+        elif isinstance(field_value, list):
+            field_value = field_value[field] if len(field_value) > field else None
+        if field_value is None:
+            return None
+    return format_method(field_value) if format_method else field_value
```

### Comparing `datamarket-0.5.8/src/datamarket/utils/selenium.py` & `datamarket-0.5.9/src/datamarket/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket/utils/soda.py` & `datamarket-0.5.9/src/datamarket/utils/soda.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.8/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.5.9/src/datamarket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.5.8
+Version: 0.5.9
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.5.8/src/datamarket.egg-info/SOURCES.txt` & `datamarket-0.5.9/src/datamarket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

