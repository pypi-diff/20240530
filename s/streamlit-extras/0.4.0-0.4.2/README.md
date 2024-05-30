# Comparing `tmp/streamlit_extras-0.4.0.tar.gz` & `tmp/streamlit_extras-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_extras-0.4.0.tar", max compression
+gzip compressed data, was "streamlit_extras-0.4.2.tar", max compression
```

## Comparing `streamlit_extras-0.4.0.tar` & `streamlit_extras-0.4.2.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0    11357 2024-02-05 09:58:41.784282 streamlit_extras-0.4.0/LICENSE
--rw-r--r--   0        0        0     2390 2024-02-05 09:58:41.784282 streamlit_extras-0.4.0/README.md
--rw-r--r--   0        0        0     2040 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1599 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/__init__.py
--rw-r--r--   0        0        0      929 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/add_vertical_space/__init__.py
--rw-r--r--   0        0        0    15616 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/altex/__init__.py
--rw-r--r--   0        0        0     1003 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/annotated_text/__init__.py
--rw-r--r--   0        0        0     1529 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/app_logo/__init__.py
--rw-r--r--   0        0        0     3657 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/badges/__init__.py
--rw-r--r--   0        0        0     2708 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/buy_me_a_coffee/__init__.py
--rw-r--r--   0        0        0      833 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/camera_input_live/__init__.py
--rw-r--r--   0        0        0    10002 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/capture/__init__.py
--rw-r--r--   0        0        0      699 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/card/__init__.py
--rw-r--r--   0        0        0     5365 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/chart_annotations/__init__.py
--rw-r--r--   0        0        0     5742 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/chart_container/__init__.py
--rw-r--r--   0        0        0     4982 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/colored_header/__init__.py
--rw-r--r--   0        0        0      875 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/customize_running/__init__.py
--rw-r--r--   0        0        0     8842 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/dataframe_explorer/__init__.py
--rw-r--r--   0        0        0     3119 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/echo_expander/__init__.py
--rw-r--r--   0        0        0     1732 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/embed_code/__init__.py
--rw-r--r--   0        0        0      721 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/faker/__init__.py
--rw-r--r--   0        0        0     4817 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/function_explorer/__init__.py
--rw-r--r--   0        0        0     5812 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/grid/__init__.py
--rw-r--r--   0        0        0      809 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/image_coordinates/__init__.py
--rw-r--r--   0        0        0     2731 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/image_in_tables/__init__.py
--rw-r--r--   0        0        0      773 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/jupyterlite/__init__.py
--rw-r--r--   0        0        0     1539 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/keyboard_text/__init__.py
--rw-r--r--   0        0        0     2336 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/keyboard_url/__init__.py
--rw-r--r--   0        0        0     5099 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/let_it_rain/__init__.py
--rw-r--r--   0        0        0     2800 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/mandatory_date_range/__init__.py
--rw-r--r--   0        0        0     1864 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/markdownlit/__init__.py
--rw-r--r--   0        0        0     3450 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/mention/__init__.py
--rw-r--r--   0        0        0     2326 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/metric_cards/__init__.py
--rw-r--r--   0        0        0     2651 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/no_default_selectbox/__init__.py
--rw-r--r--   0        0        0     4943 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/prometheus/__init__.py
--rw-r--r--   0        0        0      382 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/prometheus/example/README.md
--rw-r--r--   0        0        0      817 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/prometheus/example/app.py
--rw-r--r--   0        0        0      461 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/prometheus/example/metrics.py
--rw-r--r--   0        0        0     3336 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/row/__init__.py
--rw-r--r--   0        0        0     5269 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/sandbox/__init__.py
--rw-r--r--   0        0        0      927 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/st_keyup/__init__.py
--rw-r--r--   0        0        0     1389 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/stateful_button/__init__.py
--rw-r--r--   0        0        0     4355 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/stateful_chat/__init__.py
--rw-r--r--   0        0        0     2243 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/stodo/__init__.py
--rw-r--r--   0        0        0      997 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/stoggle/__init__.py
--rw-r--r--   0        0        0     4897 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/streaming_write/__init__.py
--rw-r--r--   0        0        0     2501 2024-02-05 09:58:41.788282 streamlit_extras-0.4.0/src/streamlit_extras/stylable_container/__init__.py
--rw-r--r--   0        0        0     1719 2024-02-05 09:58:41.792282 streamlit_extras-0.4.0/src/streamlit_extras/switch_page_button/__init__.py
--rw-r--r--   0        0        0     5816 2024-02-05 09:58:41.792282 streamlit_extras-0.4.0/src/streamlit_extras/tags/__init__.py
--rw-r--r--   0        0        0     1236 2024-02-05 09:58:41.792282 streamlit_extras-0.4.0/src/streamlit_extras/toggle_switch/__init__.py
--rw-r--r--   0        0        0     1077 2024-02-05 09:58:41.792282 streamlit_extras-0.4.0/src/streamlit_extras/vertical_slider/__init__.py
--rw-r--r--   0        0        0     2066 2024-02-05 09:58:41.792282 streamlit_extras-0.4.0/src/streamlit_extras/word_importances/__init__.py
--rw-r--r--   0        0        0     3792 1970-01-01 00:00:00.000000 streamlit_extras-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-04 12:54:34.306461 streamlit_extras-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2390 2024-04-04 12:54:34.306461 streamlit_extras-0.4.2/README.md
+-rw-r--r--   0        0        0     2065 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1599 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/add_vertical_space/__init__.py
+-rw-r--r--   0        0        0    15616 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/altex/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/annotated_text/__init__.py
+-rw-r--r--   0        0        0     1529 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/app_logo/__init__.py
+-rw-r--r--   0        0        0     3657 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/badges/__init__.py
+-rw-r--r--   0        0        0      922 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/bottom_container/__init__.py
+-rw-r--r--   0        0        0     2708 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/buy_me_a_coffee/__init__.py
+-rw-r--r--   0        0        0      833 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/camera_input_live/__init__.py
+-rw-r--r--   0        0        0    10002 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/capture/__init__.py
+-rw-r--r--   0        0        0      699 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/card/__init__.py
+-rw-r--r--   0        0        0     5365 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/chart_annotations/__init__.py
+-rw-r--r--   0        0        0     5742 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/chart_container/__init__.py
+-rw-r--r--   0        0        0     4982 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/colored_header/__init__.py
+-rw-r--r--   0        0        0      875 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/customize_running/__init__.py
+-rw-r--r--   0        0        0     8842 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/dataframe_explorer/__init__.py
+-rw-r--r--   0        0        0     3119 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/echo_expander/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/embed_code/__init__.py
+-rw-r--r--   0        0        0      721 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/faker/__init__.py
+-rw-r--r--   0        0        0     4817 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/function_explorer/__init__.py
+-rw-r--r--   0        0        0     5812 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/grid/__init__.py
+-rw-r--r--   0        0        0      809 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/image_coordinates/__init__.py
+-rw-r--r--   0        0        0     2731 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/image_in_tables/__init__.py
+-rw-r--r--   0        0        0      773 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/jupyterlite/__init__.py
+-rw-r--r--   0        0        0     1539 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/keyboard_text/__init__.py
+-rw-r--r--   0        0        0     2336 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/keyboard_url/__init__.py
+-rw-r--r--   0        0        0     5099 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/let_it_rain/__init__.py
+-rw-r--r--   0        0        0     2800 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/mandatory_date_range/__init__.py
+-rw-r--r--   0        0        0     1864 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/markdownlit/__init__.py
+-rw-r--r--   0        0        0     3450 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/mention/__init__.py
+-rw-r--r--   0        0        0     2326 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/metric_cards/__init__.py
+-rw-r--r--   0        0        0     2651 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/no_default_selectbox/__init__.py
+-rw-r--r--   0        0        0     4943 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/prometheus/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/prometheus/example/README.md
+-rw-r--r--   0        0        0      817 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/prometheus/example/app.py
+-rw-r--r--   0        0        0      461 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/prometheus/example/metrics.py
+-rw-r--r--   0        0        0     3336 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/row/__init__.py
+-rw-r--r--   0        0        0     5269 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/sandbox/__init__.py
+-rw-r--r--   0        0        0      927 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/st_keyup/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/stateful_button/__init__.py
+-rw-r--r--   0        0        0     4355 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/stateful_chat/__init__.py
+-rw-r--r--   0        0        0     2243 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/stodo/__init__.py
+-rw-r--r--   0        0        0      997 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/stoggle/__init__.py
+-rw-r--r--   0        0        0     4897 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/streaming_write/__init__.py
+-rw-r--r--   0        0        0     2501 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/stylable_container/__init__.py
+-rw-r--r--   0        0        0     1719 2024-04-04 12:54:34.310461 streamlit_extras-0.4.2/src/streamlit_extras/switch_page_button/__init__.py
+-rw-r--r--   0        0        0     5816 2024-04-04 12:54:34.314461 streamlit_extras-0.4.2/src/streamlit_extras/tags/__init__.py
+-rw-r--r--   0        0        0     1236 2024-04-04 12:54:34.314461 streamlit_extras-0.4.2/src/streamlit_extras/toggle_switch/__init__.py
+-rw-r--r--   0        0        0     1077 2024-04-04 12:54:34.314461 streamlit_extras-0.4.2/src/streamlit_extras/vertical_slider/__init__.py
+-rw-r--r--   0        0        0     2066 2024-04-04 12:54:34.314461 streamlit_extras-0.4.2/src/streamlit_extras/word_importances/__init__.py
+-rw-r--r--   0        0        0     3829 1970-01-01 00:00:00.000000 streamlit_extras-0.4.2/PKG-INFO
```

### Comparing `streamlit_extras-0.4.0/LICENSE` & `streamlit_extras-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/README.md` & `streamlit_extras-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/pyproject.toml` & `streamlit_extras-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "streamlit-extras"
-version = "0.4.0"
+version = "0.4.2"
 license = "Apache-2.0"
 description = "A library to discover, try, install and share Streamlit extras"
 authors = [
   "Arnaud Miribel <arnaudmiribel@gmail.com>",
   "Zachary Blackwood <zachary@streamlit.io>",
 ]
 readme = "README.md"
@@ -29,14 +29,15 @@
 htbuilder = ">=0.6.2"
 streamlit-faker = ">=0.0.2"
 streamlit-card = ">=0.0.4"
 markdownlit = ">=0.0.5"
 streamlit-image-coordinates = "^0.1.1"
 entrypoints = ">=0.4"
 prometheus-client = ">=0.14.0"
+validators = ">= 0.20.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^22.8.0"
 isort = "^5.10.1"
 mypy = "^0.971"
 streamlit = ">=1.12.2"
```

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/add_vertical_space/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/add_vertical_space/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/altex/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/altex/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/annotated_text/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/annotated_text/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/app_logo/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/app_logo/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/badges/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/badges/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/buy_me_a_coffee/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/buy_me_a_coffee/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/camera_input_live/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/camera_input_live/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/capture/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/capture/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/card/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/card/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/chart_annotations/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/chart_annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/chart_container/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/chart_container/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/colored_header/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/colored_header/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/customize_running/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/customize_running/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/dataframe_explorer/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/dataframe_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/echo_expander/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/echo_expander/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/embed_code/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/embed_code/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/faker/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/faker/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/function_explorer/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/function_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/grid/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/image_coordinates/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/image_coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/image_in_tables/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/image_in_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/jupyterlite/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/jupyterlite/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/keyboard_text/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/keyboard_text/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/keyboard_url/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/keyboard_url/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/let_it_rain/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/let_it_rain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/mandatory_date_range/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/mandatory_date_range/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/markdownlit/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/markdownlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/mention/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/mention/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/metric_cards/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/metric_cards/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/no_default_selectbox/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/no_default_selectbox/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/prometheus/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/prometheus/example/app.py` & `streamlit_extras-0.4.2/src/streamlit_extras/prometheus/example/app.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/row/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/row/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/sandbox/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/st_keyup/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/st_keyup/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/stateful_button/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/stateful_button/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import streamlit as st
 
+try:
+    from streamlit import rerun
+except ImportError:
+    from streamlit import experimental_rerun as rerun
+
 from .. import extra
 
 
 @extra
 def button(*args, key=None, **kwargs):
     """
     Works just like a normal streamlit button, but it remembers its state, so that
@@ -19,15 +24,15 @@
         st.session_state[key] = False
 
     if "type" not in kwargs:
         kwargs["type"] = "primary" if st.session_state[key] else "secondary"
 
     if st.button(*args, **kwargs):
         st.session_state[key] = not st.session_state[key]
-        st.experimental_rerun()
+        rerun()
 
     return st.session_state[key]
 
 
 def example():
     if button("Button 1", key="button1"):
         if button("Button 2", key="button2"):
```

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/stateful_chat/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/stateful_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/stodo/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/stodo/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/stoggle/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/stoggle/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/streaming_write/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/streaming_write/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/stylable_container/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/stylable_container/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/switch_page_button/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/switch_page_button/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/tags/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/toggle_switch/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/toggle_switch/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/vertical_slider/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/vertical_slider/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/src/streamlit_extras/word_importances/__init__.py` & `streamlit_extras-0.4.2/src/streamlit_extras/word_importances/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.4.0/PKG-INFO` & `streamlit_extras-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-extras
-Version: 0.4.0
+Version: 0.4.2
 Summary: A library to discover, try, install and share Streamlit extras
 License: Apache-2.0
 Keywords: python,streamlit,ui,data
 Author: Arnaud Miribel
 Author-email: arnaudmiribel@gmail.com
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,14 +25,15 @@
 Requires-Dist: streamlit-card (>=0.0.4)
 Requires-Dist: streamlit-embedcode (>=0.1.2)
 Requires-Dist: streamlit-faker (>=0.0.2)
 Requires-Dist: streamlit-image-coordinates (>=0.1.1,<0.2.0)
 Requires-Dist: streamlit-keyup (>=0.1.9)
 Requires-Dist: streamlit-toggle-switch (>=1.0.2)
 Requires-Dist: streamlit-vertical-slider (>=2.5.5)
+Requires-Dist: validators (>=0.20.0)
 Description-Content-Type: text/markdown
 
 
 <a href="https://extras.streamlitapp.com" title="Python Version"><img src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg"></a><br>
 <a href="https://github.com/arnaudmiribel/streamlit-extras/" title="Python Version"><img src="https://img.shields.io/badge/Python-3.9%2B-blue&style=flat"></a>
 <a href="https://badge.fury.io/py/streamlit-extras"><img src="https://badge.fury.io/py/streamlit-extras.svg" alt="PyPI version" height="18"></a>
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Farnaudmiribel%2Fstreamlit-extras&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=visits&edge_flat=false"/></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlit-extras Version: 0.4.0 Summary: A library
+Metadata-Version: 2.1 Name: streamlit-extras Version: 0.4.2 Summary: A library
 to discover, try, install and share Streamlit extras License: Apache-2.0
 Keywords: python,streamlit,ui,data Author: Arnaud Miribel Author-email:
 arnaudmiribel@gmail.com Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*,
 !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.* Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -11,17 +11,17 @@
 htbuilder (>=0.6.2) Requires-Dist: markdownlit (>=0.0.5) Requires-Dist:
 prometheus-client (>=0.14.0) Requires-Dist: protobuf (!=3.20.2) Requires-Dist:
 st-annotated-text (>=3.0.0) Requires-Dist: streamlit (>=1.0.0) Requires-Dist:
 streamlit-camera-input-live (>=0.2.0) Requires-Dist: streamlit-card (>=0.0.4)
 Requires-Dist: streamlit-embedcode (>=0.1.2) Requires-Dist: streamlit-faker
 (>=0.0.2) Requires-Dist: streamlit-image-coordinates (>=0.1.1,<0.2.0) Requires-
 Dist: streamlit-keyup (>=0.1.9) Requires-Dist: streamlit-toggle-switch
-(>=1.0.2) Requires-Dist: streamlit-vertical-slider (>=2.5.5) Description-
-Content-Type: text/markdown _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._s_t_r_e_a_m_l_i_t_._i_o_/_b_a_d_g_e_s_/
-_s_t_r_e_a_m_l_i_t___b_a_d_g_e___b_l_a_c_k___w_h_i_t_e_._s_v_g_]
+(>=1.0.2) Requires-Dist: streamlit-vertical-slider (>=2.5.5) Requires-Dist:
+validators (>=0.20.0) Description-Content-Type: text/markdown _[_h_t_t_p_s_:_/_/
+_s_t_a_t_i_c_._s_t_r_e_a_m_l_i_t_._i_o_/_b_a_d_g_e_s_/_s_t_r_e_a_m_l_i_t___b_a_d_g_e___b_l_a_c_k___w_h_i_t_e_._s_v_g_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_t_h_o_n_-_3_._9_%_2_B_-_b_l_u_e_&_s_t_y_l_e_=_f_l_a_t_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]
 _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_a_r_n_a_u_d_m_i_r_i_b_e_l_%_2_F_s_t_r_e_a_m_l_i_t_-
 _e_x_t_r_a_s_&_c_o_u_n_t___b_g_=_%_2_3_7_9_C_8_3_D_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_v_i_s_i_t_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]#
 ðª¢ streamlit-extras AA PPyytthhoonn lliibbrraarryy wwiitthh uusseeffuull SSttrreeaammlliitt eexxttrraass `streamlit-
 extras` is a Python library putting together useful Streamlit bits of code
 (eexxttrraass). ![CleanShot 2023-10-18 at 14 56 43](https://github.com/arnaudmiribel/
```

