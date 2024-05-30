# Comparing `tmp/understand_sdk-0.1.2.tar.gz` & `tmp/understand_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "understand_sdk-0.1.2.tar", max compression
+gzip compressed data, was "understand_sdk-0.1.3.tar", max compression
```

## Comparing `understand_sdk-0.1.2.tar` & `understand_sdk-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-02-26 13:16:17.048739 understand_sdk-0.1.2/LICENSE
--rw-r--r--   0        0        0     1022 2024-02-29 13:48:34.879359 understand_sdk-0.1.2/README.md
--rw-r--r--   0        0        0     1133 2024-03-06 10:51:46.324835 understand_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 13:19:46.316110 understand_sdk-0.1.2/understand_sdk/__init__.py
--rw-r--r--   0        0        0     3167 2024-03-06 10:49:50.830127 understand_sdk-0.1.2/understand_sdk/client.py
--rw-r--r--   0        0        0       46 2024-02-28 08:15:21.730498 understand_sdk-0.1.2/understand_sdk/const.py
--rw-r--r--   0        0        0        0 2024-02-27 13:06:42.041051 understand_sdk-0.1.2/understand_sdk/examples/__init__.py
--rw-r--r--   0        0        0    16802 2024-03-06 10:49:46.001232 understand_sdk-0.1.2/understand_sdk/examples/story.py
--rw-r--r--   0        0        0       96 2024-03-06 10:49:50.830414 understand_sdk-0.1.2/understand_sdk/exceptions.py
--rw-r--r--   0        0        0      197 2024-02-28 08:15:22.489243 understand_sdk-0.1.2/understand_sdk/model.py
--rw-r--r--   0        0        0     5814 2024-02-29 14:03:15.286643 understand_sdk-0.1.2/understand_sdk/story.py
--rw-r--r--   0        0        0      697 2024-02-28 08:15:23.195071 understand_sdk-0.1.2/understand_sdk/task.py
--rw-r--r--   0        0        0     1558 1970-01-01 00:00:00.000000 understand_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-02-26 13:16:17.048739 understand_sdk-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1022 2024-02-29 13:48:34.879359 understand_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0     1133 2024-05-30 12:36:57.691086 understand_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-26 13:19:46.316110 understand_sdk-0.1.3/understand_sdk/__init__.py
+-rw-r--r--   0        0        0     3167 2024-03-06 10:49:50.830127 understand_sdk-0.1.3/understand_sdk/client.py
+-rw-r--r--   0        0        0       46 2024-02-28 08:15:21.730498 understand_sdk-0.1.3/understand_sdk/const.py
+-rw-r--r--   0        0        0        0 2024-02-27 13:06:42.041051 understand_sdk-0.1.3/understand_sdk/examples/__init__.py
+-rw-r--r--   0        0        0    16403 2024-05-30 12:33:13.609831 understand_sdk-0.1.3/understand_sdk/examples/story.py
+-rw-r--r--   0        0        0       96 2024-03-06 10:49:50.830414 understand_sdk-0.1.3/understand_sdk/exceptions.py
+-rw-r--r--   0        0        0      197 2024-02-28 08:15:22.489243 understand_sdk-0.1.3/understand_sdk/model.py
+-rw-r--r--   0        0        0     5735 2024-05-30 12:28:30.003084 understand_sdk-0.1.3/understand_sdk/story.py
+-rw-r--r--   0        0        0      697 2024-02-28 08:15:23.195071 understand_sdk-0.1.3/understand_sdk/task.py
+-rw-r--r--   0        0        0     1558 1970-01-01 00:00:00.000000 understand_sdk-0.1.3/PKG-INFO
```

### Comparing `understand_sdk-0.1.2/LICENSE` & `understand_sdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `understand_sdk-0.1.2/README.md` & `understand_sdk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `understand_sdk-0.1.2/pyproject.toml` & `understand_sdk-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "understand-sdk"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python client for UnderstandLabs"
 authors = ["Understandlabs.com Team <it@understandlabs.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "understand_sdk"}]
 
 [tool.poetry.dependencies]
```

### Comparing `understand_sdk-0.1.2/understand_sdk/client.py` & `understand_sdk-0.1.3/understand_sdk/client.py`

 * *Files identical despite different names*

### Comparing `understand_sdk-0.1.2/understand_sdk/examples/story.py` & `understand_sdk-0.1.3/understand_sdk/examples/story.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     Slide,
     SlideLayout,
     Story,
     StoryWithChannels,
     TargetAttribute,
     TargetFillArea,
     Variance,
-    VarianceAttribute,
     XAttribute,
     YAttribute,
 )
 
 
 def create_story(dt: datetime) -> Story:
     title = "Example story"
@@ -276,24 +275,14 @@
                 ElementAttribute(field="Company name"),
                 YAttribute(field="Amount"),
                 TargetAttribute(field="Target"),
             ],
             data=EXAMPLE_DATA_LINE,
         ),
         LineSlide(
-            title="Line with custom variance",
-            settings=LineSlideSettings(variance=Variance.CUSTOM_BAR),
-            attributes=[
-                ElementAttribute(field="Company name"),
-                YAttribute(field="Amount"),
-                VarianceAttribute(field="Variance"),
-            ],
-            data=EXAMPLE_DATA_LINE,
-        ),
-        LineSlide(
             layout=SlideLayout.ROW,
             title="Line with row",
             description="**Markdown** description",
             attributes=[
                 ElementAttribute(field="Company name"),
                 YAttribute(field="Amount"),
             ],
```

### Comparing `understand_sdk-0.1.2/understand_sdk/story.py` & `understand_sdk-0.1.3/understand_sdk/story.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,16 +74,14 @@
 # Settings options
 #
 
 
 class Variance(str, Enum):
     ABSOLUTE = "absolute"
     RELATIVE = "relative"
-    CUSTOM_BAR = "customBar"
-    CUSTOM_DIVERGING_BARS = "customDivergingBars"
 
 
 class TargetFillArea(str, Enum):
     ABOVE = "above"
     BELOW = "below"
     BOTH = "both"
```

### Comparing `understand_sdk-0.1.2/understand_sdk/task.py` & `understand_sdk-0.1.3/understand_sdk/task.py`

 * *Files identical despite different names*

### Comparing `understand_sdk-0.1.2/PKG-INFO` & `understand_sdk-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understand-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client for UnderstandLabs
 License: MIT
 Author: Understandlabs.com Team
 Author-email: it@understandlabs.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

