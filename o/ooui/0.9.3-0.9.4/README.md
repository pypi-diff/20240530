# Comparing `tmp/ooui-0.9.3.tar.gz` & `tmp/ooui-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooui-0.9.3.tar", last modified: Wed May 15 08:19:28 2024, max compression
+gzip compressed data, was "ooui-0.9.4.tar", last modified: Wed May 15 09:12:03 2024, max compression
```

## Comparing `ooui-0.9.3.tar` & `ooui-0.9.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:19:28.419839 ooui-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-15 08:19:20.000000 ooui-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 08:19:20.000000 ooui-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 08:19:28.419839 ooui-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 08:19:20.000000 ooui-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:19:28.415838 ooui-0.9.3/ooui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:19:28.419839 ooui-0.9.3/ooui/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/graph/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/graph/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/graph/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/graph/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/graph/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/graph/timerange.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:19:28.419839 ooui-0.9.3/ooui/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/helpers/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-15 08:19:20.000000 ooui-0.9.3/ooui/helpers/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:19:28.419839 ooui-0.9.3/ooui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 08:19:28.000000 ooui-0.9.3/ooui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-15 08:19:28.000000 ooui-0.9.3/ooui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:19:28.000000 ooui-0.9.3/ooui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 08:19:28.000000 ooui-0.9.3/ooui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 08:19:28.000000 ooui-0.9.3/ooui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 08:19:20.000000 ooui-0.9.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 08:19:20.000000 ooui-0.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:19:28.419839 ooui-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-15 08:19:20.000000 ooui-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:12:03.011498 ooui-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-15 09:11:54.000000 ooui-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 09:11:54.000000 ooui-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 09:12:03.011498 ooui-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 09:11:54.000000 ooui-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:12:03.011498 ooui-0.9.4/ooui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:12:03.011498 ooui-0.9.4/ooui/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/graph/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/graph/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/graph/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/graph/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/graph/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/graph/timerange.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:12:03.011498 ooui-0.9.4/ooui/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/helpers/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-15 09:11:54.000000 ooui-0.9.4/ooui/helpers/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:12:03.011498 ooui-0.9.4/ooui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 09:12:03.000000 ooui-0.9.4/ooui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-15 09:12:03.000000 ooui-0.9.4/ooui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:12:03.000000 ooui-0.9.4/ooui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 09:12:03.000000 ooui-0.9.4/ooui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 09:12:03.000000 ooui-0.9.4/ooui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 09:11:54.000000 ooui-0.9.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 09:11:54.000000 ooui-0.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 09:12:03.011498 ooui-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-15 09:11:54.000000 ooui-0.9.4/setup.py
```

### Comparing `ooui-0.9.3/LICENSE` & `ooui-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/ooui/graph/__init__.py` & `ooui-0.9.4/ooui/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/ooui/graph/axis.py` & `ooui-0.9.4/ooui/graph/axis.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/ooui/graph/base.py` & `ooui-0.9.4/ooui/graph/base.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/ooui/graph/chart.py` & `ooui-0.9.4/ooui/graph/chart.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/ooui/graph/fields.py` & `ooui-0.9.4/ooui/graph/fields.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/ooui/graph/indicator.py` & `ooui-0.9.4/ooui/graph/indicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,22 +48,24 @@
 
     def process(self, value, total=0):
         res = {
             'value': value,
             'total': total,
             'type': self.type,
         }
+        if total:
+            res['percent'] = round_number(value / total * 100)
         if self.suffix:
             res['suffix'] = self.suffix
-        if self.show_percent:
-            res['percent'] = round_number(value / total * 100)
         if self.color:
             res['color'] = self.color.eval(res)
         if self.icon:
             res['icon'] = self.icon.eval(res)
+        if not self.show_percent:
+            res.pop('percent', None)
         return res
 
 
 class GraphIndicatorField(GraphIndicator):
 
     def __init__(self, graph_type, element):
         super(GraphIndicatorField, self).__init__(graph_type, element)
```

### Comparing `ooui-0.9.3/ooui/graph/processor.py` & `ooui-0.9.4/ooui/graph/processor.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/ooui/graph/timerange.py` & `ooui-0.9.4/ooui/graph/timerange.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/ooui/helpers/__init__.py` & `ooui-0.9.4/ooui/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/ooui/helpers/conditions.py` & `ooui-0.9.4/ooui/helpers/conditions.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/ooui/helpers/domain.py` & `ooui-0.9.4/ooui/helpers/domain.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.3/setup.py` & `ooui-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
     name='ooui',
     description='Open Object User Interface',
     author='GISCE',
     author_email='devel@gisce.net',
     url='https://github.com/gisce/python-ooui',
-    version='0.9.3',
+    version='0.9.4',
     license='MIT',
     long_description='''Open Object User Interface for GISCE-ERP''',
     provides=['ooui'],
     install_requires=requirements,
     tests_require=requirements_dev,
     packages=find_packages()
 )
```

