# Comparing `tmp/utubes-0.0.8.tar.gz` & `tmp/utubes-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utubes-0.0.8.tar", last modified: Tue Apr 16 20:21:51 2024, max compression
+gzip compressed data, was "utubes-0.0.9.tar", last modified: Tue Apr 16 20:55:26 2024, max compression
```

## Comparing `utubes-0.0.8.tar` & `utubes-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:51.458017 utubes-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 20:21:47.000000 utubes-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 20:21:51.458017 utubes-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-16 20:21:47.000000 utubes-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:51.458017 utubes-0.0.8/Utube/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:51.458017 utubes-0.0.8/Utube/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:51.458017 utubes-0.0.8/Utube/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:21:51.458017 utubes-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 20:21:47.000000 utubes-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:51.458017 utubes-0.0.8/utubes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 20:21:51.000000 utubes-0.0.8/utubes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-16 20:21:51.000000 utubes-0.0.8/utubes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:21:51.000000 utubes-0.0.8/utubes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:21:51.000000 utubes-0.0.8/utubes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 20:21:51.000000 utubes-0.0.8/utubes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:55:26.694682 utubes-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 20:55:22.000000 utubes-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 20:55:26.694682 utubes-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-16 20:55:22.000000 utubes-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:55:26.690681 utubes-0.0.9/Utube/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 20:55:22.000000 utubes-0.0.9/Utube/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:55:26.690681 utubes-0.0.9/Utube/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 20:55:22.000000 utubes-0.0.9/Utube/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-16 20:55:22.000000 utubes-0.0.9/Utube/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:55:26.690681 utubes-0.0.9/Utube/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 20:55:22.000000 utubes-0.0.9/Utube/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:55:22.000000 utubes-0.0.9/Utube/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 20:55:22.000000 utubes-0.0.9/Utube/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:55:26.694682 utubes-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 20:55:22.000000 utubes-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:55:26.694682 utubes-0.0.9/utubes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 20:55:26.000000 utubes-0.0.9/utubes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-16 20:55:26.000000 utubes-0.0.9/utubes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:55:26.000000 utubes-0.0.9/utubes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:55:26.000000 utubes-0.0.9/utubes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 20:55:26.000000 utubes-0.0.9/utubes.egg-info/top_level.txt
```

### Comparing `utubes-0.0.8/LICENSE` & `utubes-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `utubes-0.0.8/PKG-INFO` & `utubes-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.8
+Version: 0.0.9
 Summary: ㅤ
 Home-page: https://github.com/Monisha
 License: MIT
 Keywords: python,youtube,extension
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: utubes Version: 0.0.8 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: utubes Version: 0.0.9 Summary: ã¤ Home-page:
 https://github.com/Monisha License: MIT Keywords: python,youtube,extension
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
```

### Comparing `utubes-0.0.8/README.md` & `utubes-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `utubes-0.0.8/Utube/functions/function01.py` & `utubes-0.0.9/Utube/functions/function01.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,57 +5,66 @@
 
 class UDMessages:
     def __init__(self, **kwargs):
         self.status = kwargs.get('status', True)
         self.errors = kwargs.get('errors', None)
         self.result = kwargs.get('result', None)
 
-#==========================================================================
+#=====================================================================================================
 
 class UDownloader:
+    def __int__(self):
+        self.foold = Okeys.DATA01
+        self.looad = asyncio.get_event_loop()
 
-    async def metadata(link, command):
+#=====================================================================================================
+
+    def start(self, link, command, progress):
+        with YoutubeDL(command) as ydl:
+            try:
+                filelink = [link]
+                ydl.add_progress_hook(progress)
+                ydl.download(filelink)
+                return True, None
+            except DownloadError as errors:
+                return False, errors
+            except Exception as errors:
+                return False, errors
+
+#=====================================================================================================
+    
+    async def metadata(self, link, command):
         with YoutubeDL(command) as ydl:
             try:
                 moonus = ydl.extract_info(link, download=False)
                 return UDMessages(result=moonus)
             except Exception as errors:
                 return UDMessages(errors=errors)
 
-#==========================================================================
+#=====================================================================================================
 
-    async def extracts(link, command):
+    async def extracts(self, link, command):
         with YoutubeDL(command) as ydl:
             try:
                 moonus = ydl.extract_info(link, download=False)
                 return UDMessages(result=moonus)
             except Exception as errors:
                 return UDMessages(errors=errors)
 
-#==========================================================================
+#=====================================================================================================
 
-    async def filename(link, command):
+    async def filename(self, link, command):
         with YoutubeDL(command) as ydl:
             try:
-                mainos = Okeys.DATA01
                 metase = ydl.extract_info(link, download=False)
-                moonus = ydl.prepare_filename(metase, outtmpl=mainos)
+                moonus = ydl.prepare_filename(metase, outtmpl=self.foold)
                 return UDMessages(result=moonus)
             except Exception as errors:
                 return UDMessages(errors=errors)
 
-#==========================================================================
+#=====================================================================================================
 
-    async def download(link, command, progress):
-        loop = asyncio.get_event_loop()
-        with YoutubeDL(command) as ydl:
-            try:
-                filelink = [link]
-                ydl.add_progress_hook(progress)   
-                await loop.run_in_executor(None, ydl.download, filelink)
-                return UDMessages(status=True)
-            except DownloadError as errors:
-                return UDMessages(status=False, errors=errors)
-            except Exception as errors:
-                return UDMessages(status=False, errors=errors)
+    async def download(self, link, command, progress):
+        om, em = await self.looad.run_in_executor(None, self.start, link, command, progress)
+        return UDMessages(status=om, errors=em)
 
-#==========================================================================
+#=====================================================================================================
```

### Comparing `utubes-0.0.8/setup.py` & `utubes-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `utubes-0.0.8/utubes.egg-info/PKG-INFO` & `utubes-0.0.9/utubes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.8
+Version: 0.0.9
 Summary: ㅤ
 Home-page: https://github.com/Monisha
 License: MIT
 Keywords: python,youtube,extension
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: utubes Version: 0.0.8 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: utubes Version: 0.0.9 Summary: ã¤ Home-page:
 https://github.com/Monisha License: MIT Keywords: python,youtube,extension
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
```

