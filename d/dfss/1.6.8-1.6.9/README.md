# Comparing `tmp/dfss-1.6.8.tar.gz` & `tmp/dfss-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfss-1.6.8.tar", last modified: Sat Mar 16 03:28:11 2024, max compression
+gzip compressed data, was "dfss-1.6.9.tar", last modified: Sat Mar 16 03:29:58 2024, max compression
```

## Comparing `dfss-1.6.8.tar` & `dfss-1.6.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zzt       (1000) zzt       (1000)        0 2024-03-16 03:28:11.673051 dfss-1.6.8/
--rw-r--r--   0 zzt       (1000) zzt       (1000)      293 2024-03-16 03:28:11.673051 dfss-1.6.8/PKG-INFO
--rw-r--r--   0 zzt       (1000) zzt       (1000)       91 2024-03-16 03:18:40.000000 dfss-1.6.8/README.md
-drwxr-xr-x   0 zzt       (1000) zzt       (1000)        0 2024-03-16 03:28:11.672051 dfss-1.6.8/dfss/
--rw-r--r--   0 zzt       (1000) zzt       (1000)        0 2022-05-18 10:40:46.000000 dfss-1.6.8/dfss/__init__.py
--rw-r--r--   0 zzt       (1000) zzt       (1000)     2592 2024-03-16 03:06:11.000000 dfss-1.6.8/dfss/__main__.py
--rw-r--r--   0 zzt       (1000) zzt       (1000)    16803 2024-03-16 03:27:45.000000 dfss-1.6.8/dfss/util.py
-drwxr-xr-x   0 zzt       (1000) zzt       (1000)        0 2024-03-16 03:28:11.673051 dfss-1.6.8/dfss.egg-info/
--rw-r--r--   0 zzt       (1000) zzt       (1000)      293 2024-03-16 03:28:11.000000 dfss-1.6.8/dfss.egg-info/PKG-INFO
--rw-r--r--   0 zzt       (1000) zzt       (1000)      214 2024-03-16 03:28:11.000000 dfss-1.6.8/dfss.egg-info/SOURCES.txt
--rw-r--r--   0 zzt       (1000) zzt       (1000)        1 2024-03-16 03:28:11.000000 dfss-1.6.8/dfss.egg-info/dependency_links.txt
--rw-r--r--   0 zzt       (1000) zzt       (1000)       55 2024-03-16 03:28:11.000000 dfss-1.6.8/dfss.egg-info/requires.txt
--rw-r--r--   0 zzt       (1000) zzt       (1000)        5 2024-03-16 03:28:11.000000 dfss-1.6.8/dfss.egg-info/top_level.txt
--rw-r--r--   0 zzt       (1000) zzt       (1000)       38 2024-03-16 03:28:11.673051 dfss-1.6.8/setup.cfg
--rw-r--r--   0 zzt       (1000) zzt       (1000)      370 2024-03-16 03:28:08.000000 dfss-1.6.8/setup.py
+drwxr-xr-x   0 zzt       (1000) zzt       (1000)        0 2024-03-16 03:29:58.215316 dfss-1.6.9/
+-rw-r--r--   0 zzt       (1000) zzt       (1000)      293 2024-03-16 03:29:58.215316 dfss-1.6.9/PKG-INFO
+-rw-r--r--   0 zzt       (1000) zzt       (1000)       91 2024-03-16 03:18:40.000000 dfss-1.6.9/README.md
+drwxr-xr-x   0 zzt       (1000) zzt       (1000)        0 2024-03-16 03:29:58.214316 dfss-1.6.9/dfss/
+-rw-r--r--   0 zzt       (1000) zzt       (1000)        0 2022-05-18 10:40:46.000000 dfss-1.6.9/dfss/__init__.py
+-rw-r--r--   0 zzt       (1000) zzt       (1000)     2592 2024-03-16 03:06:11.000000 dfss-1.6.9/dfss/__main__.py
+-rw-r--r--   0 zzt       (1000) zzt       (1000)    16870 2024-03-16 03:29:51.000000 dfss-1.6.9/dfss/util.py
+drwxr-xr-x   0 zzt       (1000) zzt       (1000)        0 2024-03-16 03:29:58.215316 dfss-1.6.9/dfss.egg-info/
+-rw-r--r--   0 zzt       (1000) zzt       (1000)      293 2024-03-16 03:29:58.000000 dfss-1.6.9/dfss.egg-info/PKG-INFO
+-rw-r--r--   0 zzt       (1000) zzt       (1000)      214 2024-03-16 03:29:58.000000 dfss-1.6.9/dfss.egg-info/SOURCES.txt
+-rw-r--r--   0 zzt       (1000) zzt       (1000)        1 2024-03-16 03:29:58.000000 dfss-1.6.9/dfss.egg-info/dependency_links.txt
+-rw-r--r--   0 zzt       (1000) zzt       (1000)       55 2024-03-16 03:29:58.000000 dfss-1.6.9/dfss.egg-info/requires.txt
+-rw-r--r--   0 zzt       (1000) zzt       (1000)        5 2024-03-16 03:29:58.000000 dfss-1.6.9/dfss.egg-info/top_level.txt
+-rw-r--r--   0 zzt       (1000) zzt       (1000)       38 2024-03-16 03:29:58.215316 dfss-1.6.9/setup.cfg
+-rw-r--r--   0 zzt       (1000) zzt       (1000)      370 2024-03-16 03:29:56.000000 dfss-1.6.9/setup.py
```

### Comparing `dfss-1.6.8/dfss/__main__.py` & `dfss-1.6.9/dfss/__main__.py`

 * *Files identical despite different names*

### Comparing `dfss-1.6.8/dfss/util.py` & `dfss-1.6.9/dfss/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,19 @@
     finally:
         try:
             transport.close()
         except Exception as e:
             print('Error: ', e)
     lock_output(False)
     lock_output_clear()
-    data_size = (file_content.getbuffer().nbytes / 1024 / (end_time - start_time))
-    return data_size if download_data_ok == 1 else 0
+    if download_data_ok == 1 and (end_time - start_time) != 0:
+        data_size = (file_content.getbuffer().nbytes / 1024 / (end_time - start_time))
+    else:
+        data_size = 0
+    return data_size
 
 def is_remote_directory(remote_path, sftp):
     try:
         remote_attributes = sftp.stat(remote_path)
         return stat.S_ISDIR(remote_attributes.st_mode)
     except Exception as e:
         print('Failed to determine directory:', str(e))
```

