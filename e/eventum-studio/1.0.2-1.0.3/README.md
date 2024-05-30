# Comparing `tmp/eventum_studio-1.0.2.tar.gz` & `tmp/eventum_studio-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventum_studio-1.0.2.tar", max compression
+gzip compressed data, was "eventum_studio-1.0.3.tar", max compression
```

## Comparing `eventum_studio-1.0.2.tar` & `eventum_studio-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-05-29 18:59:07.580389 eventum_studio-1.0.2/LICENSE
--rw-r--r--   0        0        0       46 2024-05-29 19:01:21.540375 eventum_studio-1.0.2/README.md
--rw-r--r--   0        0        0      112 2024-05-29 19:00:23.640392 eventum_studio-1.0.2/eventum_studio/.streamlit/config.toml
--rw-r--r--   0        0        0     1350 2024-05-29 21:38:29.198163 eventum_studio-1.0.2/eventum_studio/01_Time_distribution.py
--rw-r--r--   0        0        0        0 2024-05-29 19:00:23.640392 eventum_studio-1.0.2/eventum_studio/__init__.py
--rw-r--r--   0        0        0      396 2024-05-30 09:47:15.306755 eventum_studio-1.0.2/eventum_studio/__main__.py
--rw-r--r--   0        0        0     3174 2024-05-29 19:13:53.120193 eventum_studio-1.0.2/eventum_studio/components/component.py
--rw-r--r--   0        0        0     1530 2024-05-29 20:34:03.679067 eventum_studio-1.0.2/eventum_studio/components/sample_explorer.py
--rw-r--r--   0        0        0     1855 2024-05-29 20:16:13.529325 eventum_studio-1.0.2/eventum_studio/components/span_input.py
--rw-r--r--   0        0        0     2473 2024-05-29 20:36:59.119021 eventum_studio-1.0.2/eventum_studio/components/template_configuration_editor.py
--rw-r--r--   0        0        0     1601 2024-05-29 21:38:29.208163 eventum_studio-1.0.2/eventum_studio/components/template_editor.py
--rw-r--r--   0        0        0     5885 2024-05-29 20:37:43.669011 eventum_studio-1.0.2/eventum_studio/components/template_manager.py
--rw-r--r--   0        0        0     7205 2024-05-29 20:38:45.599000 eventum_studio-1.0.2/eventum_studio/components/template_renderer.py
--rw-r--r--   0        0        0     1547 2024-05-29 20:39:47.188987 eventum_studio-1.0.2/eventum_studio/components/template_state_viewer.py
--rw-r--r--   0        0        0    15180 2024-05-29 21:13:36.178516 eventum_studio-1.0.2/eventum_studio/components/time_pattern_configurator.py
--rw-r--r--   0        0        0     8672 2024-05-29 20:40:01.868985 eventum_studio-1.0.2/eventum_studio/components/time_pattern_configurator_list.py
--rw-r--r--   0        0        0     5231 2024-05-29 20:46:35.288886 eventum_studio-1.0.2/eventum_studio/components/time_pattern_distribution_histogram.py
--rw-r--r--   0        0        0      973 2024-05-29 19:00:23.650392 eventum_studio-1.0.2/eventum_studio/notifiers.py
--rw-r--r--   0        0        0     2455 2024-05-29 21:38:29.228163 eventum_studio-1.0.2/eventum_studio/pages/02_Event_template.py
--rw-r--r--   0        0        0        0 2024-05-29 19:05:13.340315 eventum_studio-1.0.2/eventum_studio/py.typed
--rw-r--r--   0        0        0    15406 2024-05-29 21:37:07.818185 eventum_studio-1.0.2/eventum_studio/static/favicon.ico
--rw-r--r--   0        0        0      285 2024-05-29 19:09:11.880258 eventum_studio-1.0.2/eventum_studio/theme.py
--rw-r--r--   0        0        0        0 2024-05-29 20:13:32.839354 eventum_studio-1.0.2/eventum_studio/utils/__init__.py
--rw-r--r--   0        0        0     1750 2024-05-29 20:44:15.698923 eventum_studio-1.0.2/eventum_studio/utils/relative_time.py
--rw-r--r--   0        0        0     1957 2024-05-29 20:15:17.739341 eventum_studio-1.0.2/eventum_studio/utils/tests/test_relative_time.py
--rw-r--r--   0        0        0      747 2024-05-29 19:35:37.879890 eventum_studio-1.0.2/eventum_studio/utils/validation_prettier.py
--rw-r--r--   0        0        0     2094 2024-05-29 19:00:23.660392 eventum_studio-1.0.2/eventum_studio/widget_management.py
--rw-r--r--   0        0        0     1360 2024-05-30 09:49:51.496716 eventum_studio-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 eventum_studio-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 18:59:07.580389 eventum_studio-1.0.3/LICENSE
+-rw-r--r--   0        0        0       46 2024-05-29 19:01:21.540375 eventum_studio-1.0.3/README.md
+-rw-r--r--   0        0        0      112 2024-05-29 19:00:23.640392 eventum_studio-1.0.3/eventum_studio/.streamlit/config.toml
+-rw-r--r--   0        0        0     1350 2024-05-29 21:38:29.198163 eventum_studio-1.0.3/eventum_studio/01_Time_distribution.py
+-rw-r--r--   0        0        0        0 2024-05-29 19:00:23.640392 eventum_studio-1.0.3/eventum_studio/__init__.py
+-rw-r--r--   0        0        0      397 2024-05-30 09:51:11.176690 eventum_studio-1.0.3/eventum_studio/__main__.py
+-rw-r--r--   0        0        0     3174 2024-05-29 19:13:53.120193 eventum_studio-1.0.3/eventum_studio/components/component.py
+-rw-r--r--   0        0        0     1530 2024-05-29 20:34:03.679067 eventum_studio-1.0.3/eventum_studio/components/sample_explorer.py
+-rw-r--r--   0        0        0     1855 2024-05-29 20:16:13.529325 eventum_studio-1.0.3/eventum_studio/components/span_input.py
+-rw-r--r--   0        0        0     2473 2024-05-29 20:36:59.119021 eventum_studio-1.0.3/eventum_studio/components/template_configuration_editor.py
+-rw-r--r--   0        0        0     1601 2024-05-29 21:38:29.208163 eventum_studio-1.0.3/eventum_studio/components/template_editor.py
+-rw-r--r--   0        0        0     5885 2024-05-29 20:37:43.669011 eventum_studio-1.0.3/eventum_studio/components/template_manager.py
+-rw-r--r--   0        0        0     7205 2024-05-29 20:38:45.599000 eventum_studio-1.0.3/eventum_studio/components/template_renderer.py
+-rw-r--r--   0        0        0     1547 2024-05-29 20:39:47.188987 eventum_studio-1.0.3/eventum_studio/components/template_state_viewer.py
+-rw-r--r--   0        0        0    15180 2024-05-29 21:13:36.178516 eventum_studio-1.0.3/eventum_studio/components/time_pattern_configurator.py
+-rw-r--r--   0        0        0     8672 2024-05-29 20:40:01.868985 eventum_studio-1.0.3/eventum_studio/components/time_pattern_configurator_list.py
+-rw-r--r--   0        0        0     5231 2024-05-29 20:46:35.288886 eventum_studio-1.0.3/eventum_studio/components/time_pattern_distribution_histogram.py
+-rw-r--r--   0        0        0      973 2024-05-29 19:00:23.650392 eventum_studio-1.0.3/eventum_studio/notifiers.py
+-rw-r--r--   0        0        0     2455 2024-05-29 21:38:29.228163 eventum_studio-1.0.3/eventum_studio/pages/02_Event_template.py
+-rw-r--r--   0        0        0        0 2024-05-29 19:05:13.340315 eventum_studio-1.0.3/eventum_studio/py.typed
+-rw-r--r--   0        0        0    15406 2024-05-29 21:37:07.818185 eventum_studio-1.0.3/eventum_studio/static/favicon.ico
+-rw-r--r--   0        0        0      285 2024-05-29 19:09:11.880258 eventum_studio-1.0.3/eventum_studio/theme.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:13:32.839354 eventum_studio-1.0.3/eventum_studio/utils/__init__.py
+-rw-r--r--   0        0        0     1750 2024-05-29 20:44:15.698923 eventum_studio-1.0.3/eventum_studio/utils/relative_time.py
+-rw-r--r--   0        0        0     1957 2024-05-29 20:15:17.739341 eventum_studio-1.0.3/eventum_studio/utils/tests/test_relative_time.py
+-rw-r--r--   0        0        0      747 2024-05-29 19:35:37.879890 eventum_studio-1.0.3/eventum_studio/utils/validation_prettier.py
+-rw-r--r--   0        0        0     2094 2024-05-29 19:00:23.660392 eventum_studio-1.0.3/eventum_studio/widget_management.py
+-rw-r--r--   0        0        0     1417 2024-05-30 10:25:37.456209 eventum_studio-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 eventum_studio-1.0.3/PKG-INFO
```

### Comparing `eventum_studio-1.0.2/LICENSE` & `eventum_studio-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/01_Time_distribution.py` & `eventum_studio-1.0.3/eventum_studio/01_Time_distribution.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/component.py` & `eventum_studio-1.0.3/eventum_studio/components/component.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/sample_explorer.py` & `eventum_studio-1.0.3/eventum_studio/components/sample_explorer.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/span_input.py` & `eventum_studio-1.0.3/eventum_studio/components/span_input.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/template_configuration_editor.py` & `eventum_studio-1.0.3/eventum_studio/components/template_configuration_editor.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/template_editor.py` & `eventum_studio-1.0.3/eventum_studio/components/template_editor.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/template_manager.py` & `eventum_studio-1.0.3/eventum_studio/components/template_manager.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/template_renderer.py` & `eventum_studio-1.0.3/eventum_studio/components/template_renderer.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/template_state_viewer.py` & `eventum_studio-1.0.3/eventum_studio/components/template_state_viewer.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/time_pattern_configurator.py` & `eventum_studio-1.0.3/eventum_studio/components/time_pattern_configurator.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/time_pattern_configurator_list.py` & `eventum_studio-1.0.3/eventum_studio/components/time_pattern_configurator_list.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/components/time_pattern_distribution_histogram.py` & `eventum_studio-1.0.3/eventum_studio/components/time_pattern_distribution_histogram.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/notifiers.py` & `eventum_studio-1.0.3/eventum_studio/notifiers.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/pages/02_Event_template.py` & `eventum_studio-1.0.3/eventum_studio/pages/02_Event_template.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/static/favicon.ico` & `eventum_studio-1.0.3/eventum_studio/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/utils/relative_time.py` & `eventum_studio-1.0.3/eventum_studio/utils/relative_time.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/utils/tests/test_relative_time.py` & `eventum_studio-1.0.3/eventum_studio/utils/tests/test_relative_time.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/utils/validation_prettier.py` & `eventum_studio-1.0.3/eventum_studio/utils/validation_prettier.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/eventum_studio/widget_management.py` & `eventum_studio-1.0.3/eventum_studio/widget_management.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.2/pyproject.toml` & `eventum_studio-1.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventum-studio"
-version = "1.0.2"
+version = "1.0.3"
 description = "Content designer for Eventum "
 license = "Apache-2.0"
 authors = ["Nikita Reznikov <nikita.reznikov.public@mail.ru>"]
 readme = "README.md"
 repository = "https://github.com/Eventum-Generatives/EventumStudio"
 documentation = "https://eventum-generatives.github.io/Website/"
 keywords = ["content", "IDE", "template", "visualization"]
@@ -14,15 +14,16 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3"
 ]
 packages = [
     {include = "eventum_studio"},
     {include = "eventum_studio/py.typed"},
-    {include = "eventum_studio/static/favicon.ico"}
+    {include = "eventum_studio/static/favicon.ico"},
+    {include = "eventum_studio/.streamlit/config.toml"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.6.2"
 streamlit = "==1.28.1"
 numpy = "^1.26.4"
```

### Comparing `eventum_studio-1.0.2/PKG-INFO` & `eventum_studio-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventum-studio
-Version: 1.0.2
+Version: 1.0.3
 Summary: Content designer for Eventum 
 Home-page: https://github.com/Eventum-Generatives/EventumStudio
 License: Apache-2.0
 Keywords: content,IDE,template,visualization
 Author: Nikita Reznikov
 Author-email: nikita.reznikov.public@mail.ru
 Requires-Python: >=3.11,<4.0
```

