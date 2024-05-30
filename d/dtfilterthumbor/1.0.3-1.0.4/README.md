# Comparing `tmp/dtfilterthumbor-1.0.3.tar.gz` & `tmp/dtfilterthumbor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfilterthumbor-1.0.3.tar", last modified: Wed May 29 07:57:25 2024, max compression
+gzip compressed data, was "dtfilterthumbor-1.0.4.tar", last modified: Thu May 30 01:57:31 2024, max compression
```

## Comparing `dtfilterthumbor-1.0.3.tar` & `dtfilterthumbor-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:57:25.388073 dtfilterthumbor-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1123 2024-05-29 07:57:25.388073 dtfilterthumbor-1.0.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      333 2022-08-18 11:31:44.000000 dtfilterthumbor-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:57:25.386073 dtfilterthumbor-1.0.3/dtfilterthumbor/
--rw-rw-r--   0 root         (0) root         (0)      322 2024-05-29 07:56:52.000000 dtfilterthumbor-1.0.3/dtfilterthumbor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7395 2022-08-18 11:31:44.000000 dtfilterthumbor-1.0.3/dtfilterthumbor/dtwatermark.py
--rw-rw-r--   0 root         (0) root         (0)     7429 2024-05-29 07:56:52.000000 dtfilterthumbor-1.0.3/dtfilterthumbor/watermarkdt2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:57:25.388073 dtfilterthumbor-1.0.3/dtfilterthumbor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1123 2024-05-29 07:57:25.000000 dtfilterthumbor-1.0.3/dtfilterthumbor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      265 2024-05-29 07:57:25.000000 dtfilterthumbor-1.0.3/dtfilterthumbor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 07:57:25.000000 dtfilterthumbor-1.0.3/dtfilterthumbor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-29 07:57:25.000000 dtfilterthumbor-1.0.3/dtfilterthumbor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 07:57:25.388073 dtfilterthumbor-1.0.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1289 2024-05-29 07:56:52.000000 dtfilterthumbor-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:57:31.173248 dtfilterthumbor-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-30 01:57:31.172248 dtfilterthumbor-1.0.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      333 2022-08-18 11:31:44.000000 dtfilterthumbor-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:57:31.169248 dtfilterthumbor-1.0.4/dtfilterthumbor/
+-rw-rw-r--   0 root         (0) root         (0)      322 2024-05-30 01:56:40.000000 dtfilterthumbor-1.0.4/dtfilterthumbor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7416 2024-05-30 01:56:40.000000 dtfilterthumbor-1.0.4/dtfilterthumbor/watermarkdt.py
+-rw-rw-r--   0 root         (0) root         (0)     7399 2024-05-30 01:54:55.000000 dtfilterthumbor-1.0.4/dtfilterthumbor/watermarkdt2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:57:31.171248 dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-30 01:57:31.000000 dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      265 2024-05-30 01:57:31.000000 dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 01:57:31.000000 dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-30 01:57:31.000000 dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 01:57:31.173248 dtfilterthumbor-1.0.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1289 2024-05-30 01:56:53.000000 dtfilterthumbor-1.0.4/setup.py
```

### Comparing `dtfilterthumbor-1.0.3/PKG-INFO` & `dtfilterthumbor-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfilterthumbor
-Version: 1.0.3
+Version: 1.0.4
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

### Comparing `dtfilterthumbor-1.0.3/dtfilterthumbor/dtwatermark.py` & `dtfilterthumbor-1.0.4/dtfilterthumbor/watermarkdt.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         self.x = str(math.ceil(watermark_sz[1]/2));
         self.y = "-"+str(math.ceil(watermark_sz[1]/2));
 
         #self.x = self.detect_and_get_ratio_position(self.x, image_size[0])
         #self.y = self.detect_and_get_ratio_position(self.y, image_size[1])
 
         mos_x = self.x == "repeat"
+        mos_x = True
         mos_y = self.y == "repeat"
         center_x = self.x == "center"
         center_y = self.y == "center"
         if not center_x and not mos_x:
             inv_x = self.x[0] == "-"
             x = int(self.x)
         if not center_y and not mos_y:
```

### Comparing `dtfilterthumbor-1.0.3/dtfilterthumbor/watermarkdt2.py` & `dtfilterthumbor-1.0.4/dtfilterthumbor/watermarkdt2.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,21 +75,19 @@
 
 
         #if self.w_ratio or self.h_ratio:
         #    watermark_sz = self.calc_watermark_size(
         #        image_size, watermark_sz, self.w_ratio, self.h_ratio
         #    )
         self.watermark_engine.resize(watermark_sz[0], watermark_sz[1])
-        self.x = str(math.ceil(watermark_sz[1]/2));
+        self.x =  True;
         self.y = "-"+str(math.ceil(watermark_sz[1]/2));
-
         #self.x = self.detect_and_get_ratio_position(self.x, image_size[0])
         #self.y = self.detect_and_get_ratio_position(self.y, image_size[1])
-
-        mos_x = self.x == "repeat"
+        mos_x = True
         mos_y = self.y == "repeat"
         center_x = self.x == "center"
         center_y = self.y == "center"
         if not center_x and not mos_x:
             inv_x = self.x[0] == "-"
             x = int(self.x)
         if not center_y and not mos_y:
@@ -121,17 +119,16 @@
             if image_size[1] * 1.0 / watermark_sz[1] < 2:
                 repeat_y = (
                     math.ceil(image_size[1] * 1.0 / watermark_sz[1]),
                     10,
                 )
                 space_y = 10
 
-        print ("change mose y")
         if not mos_x and not mos_y:
-            self.engine.paste(self.watermark_engine, (x, y), merge=True)
+            self.engine.paste(self.watermark_engine, (x, y), merge=True)     
         elif mos_x and mos_y:
             if (repeat_x[0] * repeat_y[0]) > 100:
                 tmpRepeatX = min(6, repeat_x[0])
                 tmpRepeatY = min(6, repeat_y[0])
                 repeat_x = (
                     tmpRepeatX,
                     image_size[0] - tmpRepeatX * watermark_sz[0],
@@ -146,27 +143,29 @@
                 x = i * space_x + i * watermark_sz[0]
                 for j in range(int(repeat_y[0])):
                     y = j * space_y + j * watermark_sz[1]
                     self.engine.paste(
                         self.watermark_engine, (x, y), merge=True
                     )
         elif mos_x:
+            # repeart by X axis
             space_x = repeat_x[1] // (max(repeat_x[0], 2) - 1)
             for i in range(int(repeat_x[0])):
                 x = i * space_x + i * watermark_sz[0]
                 self.engine.paste(self.watermark_engine, (x, y), merge=True)
         else:
             space_y = repeat_y[1] // (max(repeat_y[0], 2) - 1)
             for j in range(int(repeat_y[0])):
                 y = j * space_y + j * watermark_sz[1]
                 self.engine.paste(self.watermark_engine, (x, y), merge=True)
 
     @filter_method(
         BaseFilter.String,
-        BaseFilter.PositiveNumber
+        BaseF
+        ilter.PositiveNumber
     )
 
     async def watermarkdt2(self, url, alpha):
         self.url = url
         self.alpha = alpha
         self.watermark_engine = self.context.modules.engine.__class__(
             self.context
```

### Comparing `dtfilterthumbor-1.0.3/dtfilterthumbor.egg-info/PKG-INFO` & `dtfilterthumbor-1.0.4/dtfilterthumbor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfilterthumbor
-Version: 1.0.3
+Version: 1.0.4
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

### Comparing `dtfilterthumbor-1.0.3/setup.py` & `dtfilterthumbor-1.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="dtfilterthumbor",
-    version="1.0.3",
+    version="1.0.4",
     description="dan tri filter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://medium-multiply.readthedocs.io/",
     author="xuantrangk54",
     author_email="xuantrangk54@gmail.com",
     license="MIT",
```

