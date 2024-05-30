# Comparing `tmp/jmpy4-1.0.8.tar.gz` & `tmp/jmpy4-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmpy4-1.0.8.tar", last modified: Wed May 29 12:36:09 2024, max compression
+gzip compressed data, was "jmpy4-1.0.9.tar", last modified: Thu May 30 01:56:18 2024, max compression
```

## Comparing `jmpy4-1.0.8.tar` & `jmpy4-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 12:36:09.723052 jmpy4-1.0.8/
--rw-rw-rw-   0        0        0     1103 2024-05-28 13:12:38.000000 jmpy4-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       61 2020-12-29 07:22:13.000000 jmpy4-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      929 2024-05-29 12:36:09.717048 jmpy4-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      573 2024-05-29 09:12:59.000000 jmpy4-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 12:36:09.652050 jmpy4-1.0.8/jmpy/
--rw-rw-rw-   0        0        0      109 2020-12-29 07:22:13.000000 jmpy4-1.0.8/jmpy/__init__.py
--rw-rw-rw-   0        0        0     2248 2024-05-28 14:16:29.000000 jmpy4-1.0.8/jmpy/cmdline.py
--rw-rw-rw-   0        0        0     6756 2024-05-29 12:35:09.000000 jmpy4-1.0.8/jmpy/encrypt_py.py
--rw-rw-rw-   0        0        0      531 2020-12-29 07:22:13.000000 jmpy4-1.0.8/jmpy/log.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:36:09.711048 jmpy4-1.0.8/jmpy4.egg-info/
--rw-rw-rw-   0        0        0      929 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 12:36:09.724048 jmpy4-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1137 2024-05-29 09:22:53.000000 jmpy4-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:36:09.701047 jmpy4-1.0.8/tests/
--rw-rw-rw-   0        0        0      402 2024-05-29 12:16:32.000000 jmpy4-1.0.8/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-30 01:56:18.300782 jmpy4-1.0.9/
+-rw-rw-rw-   0        0        0     1103 2024-05-28 13:12:38.000000 jmpy4-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       61 2020-12-29 07:22:13.000000 jmpy4-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      929 2024-05-30 01:56:18.296782 jmpy4-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2024-05-29 09:12:59.000000 jmpy4-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 01:56:18.233792 jmpy4-1.0.9/jmpy/
+-rw-rw-rw-   0        0        0      109 2020-12-29 07:22:13.000000 jmpy4-1.0.9/jmpy/__init__.py
+-rw-rw-rw-   0        0        0     2248 2024-05-28 14:16:29.000000 jmpy4-1.0.9/jmpy/cmdline.py
+-rw-rw-rw-   0        0        0     6864 2024-05-30 01:48:34.000000 jmpy4-1.0.9/jmpy/encrypt_py.py
+-rw-rw-rw-   0        0        0      531 2020-12-29 07:22:13.000000 jmpy4-1.0.9/jmpy/log.py
+drwxrwxrwx   0        0        0        0 2024-05-30 01:56:18.291780 jmpy4-1.0.9/jmpy4.egg-info/
+-rw-rw-rw-   0        0        0      929 2024-05-30 01:56:17.000000 jmpy4-1.0.9/jmpy4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-05-30 01:56:17.000000 jmpy4-1.0.9/jmpy4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 01:56:17.000000 jmpy4-1.0.9/jmpy4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-30 01:56:17.000000 jmpy4-1.0.9/jmpy4.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 01:56:17.000000 jmpy4-1.0.9/jmpy4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-30 01:56:17.000000 jmpy4-1.0.9/jmpy4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 01:56:18.300782 jmpy4-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1137 2024-05-29 09:22:53.000000 jmpy4-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 01:56:18.282786 jmpy4-1.0.9/tests/
+-rw-rw-rw-   0        0        0      391 2024-05-30 01:47:18.000000 jmpy4-1.0.9/tests/test.py
```

### Comparing `jmpy4-1.0.8/LICENSE` & `jmpy4-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jmpy4-1.0.8/PKG-INFO` & `jmpy4-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmpy4
-Version: 1.0.8
+Version: 1.0.9
 Summary: python代码一键加密
 Home-page: https://github.com/shenny520/jmpy-plus.git
 Author: Shenny
 Author-email: shenny520@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `jmpy4-1.0.8/README.md` & `jmpy4-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jmpy4-1.0.8/jmpy/cmdline.py` & `jmpy4-1.0.9/jmpy/cmdline.py`

 * *Files identical despite different names*

### Comparing `jmpy4-1.0.8/jmpy/encrypt_py.py` & `jmpy4-1.0.9/jmpy/encrypt_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,21 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         shutil.rmtree(self.name)
 
 
 def search(content, regexs):
     content = content.replace('\\', '/')
-    regexs = regexs.replace('\\', '/')
+
     if isinstance(regexs, str):
+        regexs = regexs.replace('\\', '/')
         return re.search(regexs, content)
 
     for regex in regexs:
+        regex = regex.replace('\\', '/')
         if re.search(regex, content):
             return True
 
 
 def walk_file(file_path):
     if os.path.isdir(file_path):
         for current_path, sub_folders, files_name in os.walk(file_path):
@@ -137,14 +139,15 @@
         if os.path.exists(temp_c):
             os.remove(temp_c)
 
 
 def encrypt_py(py_files: list, worker_num: int = 1):
     total = len(py_files)
     complete = 0
+    print('*' * 20, f'【{complete}/{total}】', '*' * 20)
 
     def show_progress(*args):
         nonlocal complete
         complete += 1
         print('*' * 20, f'【{complete}/{total}】', '*' * 20)
 
     pool = Pool(worker_num)
```

### Comparing `jmpy4-1.0.8/jmpy/log.py` & `jmpy4-1.0.9/jmpy/log.py`

 * *Files identical despite different names*

### Comparing `jmpy4-1.0.8/jmpy4.egg-info/PKG-INFO` & `jmpy4-1.0.9/jmpy4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmpy4
-Version: 1.0.8
+Version: 1.0.9
 Summary: python代码一键加密
 Home-page: https://github.com/shenny520/jmpy-plus.git
 Author: Shenny
 Author-email: shenny520@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `jmpy4-1.0.8/setup.py` & `jmpy4-1.0.9/setup.py`

 * *Files identical despite different names*

