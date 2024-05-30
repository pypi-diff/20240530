# Comparing `tmp/dtfilterthumbor-1.0.4.tar.gz` & `tmp/dtfilterthumbor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfilterthumbor-1.0.4.tar", last modified: Thu May 30 01:57:31 2024, max compression
+gzip compressed data, was "dtfilterthumbor-1.0.5.tar", last modified: Thu May 30 02:43:12 2024, max compression
```

## Comparing `dtfilterthumbor-1.0.4.tar` & `dtfilterthumbor-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:57:31.173248 dtfilterthumbor-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     1123 2024-05-30 01:57:31.172248 dtfilterthumbor-1.0.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      333 2022-08-18 11:31:44.000000 dtfilterthumbor-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:57:31.169248 dtfilterthumbor-1.0.4/dtfilterthumbor/
--rw-rw-r--   0 root         (0) root         (0)      322 2024-05-30 01:56:40.000000 dtfilterthumbor-1.0.4/dtfilterthumbor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7416 2024-05-30 01:56:40.000000 dtfilterthumbor-1.0.4/dtfilterthumbor/watermarkdt.py
--rw-rw-r--   0 root         (0) root         (0)     7399 2024-05-30 01:54:55.000000 dtfilterthumbor-1.0.4/dtfilterthumbor/watermarkdt2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:57:31.171248 dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1123 2024-05-30 01:57:31.000000 dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      265 2024-05-30 01:57:31.000000 dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 01:57:31.000000 dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-30 01:57:31.000000 dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 01:57:31.173248 dtfilterthumbor-1.0.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1289 2024-05-30 01:56:53.000000 dtfilterthumbor-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:43:12.883268 dtfilterthumbor-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-30 02:43:12.882268 dtfilterthumbor-1.0.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      333 2022-08-18 11:31:44.000000 dtfilterthumbor-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:43:12.879268 dtfilterthumbor-1.0.5/dtfilterthumbor/
+-rw-rw-r--   0 root         (0) root         (0)      322 2024-05-30 01:56:40.000000 dtfilterthumbor-1.0.5/dtfilterthumbor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7416 2024-05-30 01:56:40.000000 dtfilterthumbor-1.0.5/dtfilterthumbor/watermarkdt.py
+-rw-rw-r--   0 root         (0) root         (0)     7389 2024-05-30 02:42:20.000000 dtfilterthumbor-1.0.5/dtfilterthumbor/watermarkdt2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:43:12.881268 dtfilterthumbor-1.0.5/dtfilterthumbor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-30 02:43:12.000000 dtfilterthumbor-1.0.5/dtfilterthumbor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      265 2024-05-30 02:43:12.000000 dtfilterthumbor-1.0.5/dtfilterthumbor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 02:43:12.000000 dtfilterthumbor-1.0.5/dtfilterthumbor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-30 02:43:12.000000 dtfilterthumbor-1.0.5/dtfilterthumbor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 02:43:12.883268 dtfilterthumbor-1.0.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1289 2024-05-30 02:42:20.000000 dtfilterthumbor-1.0.5/setup.py
```

### Comparing `dtfilterthumbor-1.0.4/PKG-INFO` & `dtfilterthumbor-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfilterthumbor
-Version: 1.0.4
+Version: 1.0.5
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

### Comparing `dtfilterthumbor-1.0.4/dtfilterthumbor/watermarkdt.py` & `dtfilterthumbor-1.0.5/dtfilterthumbor/watermarkdt.py`

 * *Files identical despite different names*

### Comparing `dtfilterthumbor-1.0.4/dtfilterthumbor/watermarkdt2.py` & `dtfilterthumbor-1.0.5/dtfilterthumbor/watermarkdt2.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,18 +156,16 @@
             space_y = repeat_y[1] // (max(repeat_y[0], 2) - 1)
             for j in range(int(repeat_y[0])):
                 y = j * space_y + j * watermark_sz[1]
                 self.engine.paste(self.watermark_engine, (x, y), merge=True)
 
     @filter_method(
         BaseFilter.String,
-        BaseF
-        ilter.PositiveNumber
+        BaseFilter.PositiveNumber
     )
-
     async def watermarkdt2(self, url, alpha):
         self.url = url
         self.alpha = alpha
         self.watermark_engine = self.context.modules.engine.__class__(
             self.context
         )
         self.storage = self.context.modules.storage
```

### Comparing `dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/PKG-INFO` & `dtfilterthumbor-1.0.5/dtfilterthumbor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfilterthumbor
-Version: 1.0.4
+Version: 1.0.5
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

### Comparing `dtfilterthumbor-1.0.4/setup.py` & `dtfilterthumbor-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="dtfilterthumbor",
-    version="1.0.4",
+    version="1.0.5",
     description="dan tri filter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://medium-multiply.readthedocs.io/",
     author="xuantrangk54",
     author_email="xuantrangk54@gmail.com",
     license="MIT",
```

