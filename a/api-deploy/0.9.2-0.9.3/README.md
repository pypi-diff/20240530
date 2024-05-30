# Comparing `tmp/api-deploy-0.9.2.tar.gz` & `tmp/api-deploy-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-deploy-0.9.2.tar", last modified: Thu Nov  2 16:58:03 2023, max compression
+gzip compressed data, was "api-deploy-0.9.3.tar", last modified: Fri Nov  3 10:39:57 2023, max compression
```

## Comparing `api-deploy-0.9.2.tar` & `api-deploy-0.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-11-02 16:58:03.835997 api-deploy-0.9.2/
--rw-r--r--   0 fabian     (501) staff       (20)       42 2023-09-29 15:31:13.000000 api-deploy-0.9.2/MANIFEST.in
--rw-r--r--   0 fabian     (501) staff       (20)      740 2023-11-02 16:58:03.835802 api-deploy-0.9.2/PKG-INFO
--rw-r--r--   0 fabian     (501) staff       (20)       12 2022-12-17 05:34:22.000000 api-deploy-0.9.2/README.md
-drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-11-02 16:58:03.832010 api-deploy-0.9.2/api_deploy/
--rw-r--r--   0 fabian     (501) staff       (20)       18 2023-11-02 16:56:31.000000 api-deploy-0.9.2/api_deploy/__init__.py
--rw-r--r--   0 fabian     (501) staff       (20)     3228 2023-10-05 16:17:32.000000 api-deploy-0.9.2/api_deploy/cli.py
--rw-r--r--   0 fabian     (501) staff       (20)     2400 2023-05-09 14:47:12.000000 api-deploy-0.9.2/api_deploy/client.py
--rw-r--r--   0 fabian     (501) staff       (20)     1889 2023-11-02 11:58:11.000000 api-deploy-0.9.2/api_deploy/config.py
--rw-r--r--   0 fabian     (501) staff       (20)    18368 2023-11-02 12:06:55.000000 api-deploy-0.9.2/api_deploy/converters.py
-drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-11-02 16:58:03.834745 api-deploy-0.9.2/api_deploy/processors/
--rw-r--r--   0 fabian     (501) staff       (20)        0 2023-09-29 15:24:43.000000 api-deploy-0.9.2/api_deploy/processors/__init__.py
--rw-r--r--   0 fabian     (501) staff       (20)      308 2023-09-29 15:24:43.000000 api-deploy-0.9.2/api_deploy/processors/abstract_processor.py
--rw-r--r--   0 fabian     (501) staff       (20)     4975 2023-10-06 05:28:47.000000 api-deploy-0.9.2/api_deploy/processors/code_generator.py
--rw-r--r--   0 fabian     (501) staff       (20)     1548 2023-11-02 16:56:49.000000 api-deploy-0.9.2/api_deploy/processors/strict_processor.py
-drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-11-02 16:58:03.835398 api-deploy-0.9.2/api_deploy/processors/templates/
--rw-r--r--   0 fabian     (501) staff       (20)      329 2023-10-17 09:29:44.000000 api-deploy-0.9.2/api_deploy/processors/templates/typescript.jinja2
--rw-r--r--   0 fabian     (501) staff       (20)      619 2023-10-06 05:18:17.000000 api-deploy-0.9.2/api_deploy/processors/templates/typescript.object.jinja2
--rw-r--r--   0 fabian     (501) staff       (20)     1075 2023-10-05 13:44:18.000000 api-deploy-0.9.2/api_deploy/schema.py
-drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-11-02 16:58:03.833963 api-deploy-0.9.2/api_deploy.egg-info/
--rw-r--r--   0 fabian     (501) staff       (20)      740 2023-11-02 16:58:03.000000 api-deploy-0.9.2/api_deploy.egg-info/PKG-INFO
--rw-r--r--   0 fabian     (501) staff       (20)      665 2023-11-02 16:58:03.000000 api-deploy-0.9.2/api_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 fabian     (501) staff       (20)        1 2023-11-02 16:58:03.000000 api-deploy-0.9.2/api_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 fabian     (501) staff       (20)       44 2023-11-02 16:58:03.000000 api-deploy-0.9.2/api_deploy.egg-info/entry_points.txt
--rw-r--r--   0 fabian     (501) staff       (20)        1 2022-12-17 05:34:25.000000 api-deploy-0.9.2/api_deploy.egg-info/not-zip-safe
--rw-r--r--   0 fabian     (501) staff       (20)      102 2023-11-02 16:58:03.000000 api-deploy-0.9.2/api_deploy.egg-info/requires.txt
--rw-r--r--   0 fabian     (501) staff       (20)       11 2023-11-02 16:58:03.000000 api-deploy-0.9.2/api_deploy.egg-info/top_level.txt
--rw-r--r--   0 fabian     (501) staff       (20)       38 2023-11-02 16:58:03.836068 api-deploy-0.9.2/setup.cfg
--rw-r--r--   0 fabian     (501) staff       (20)     1428 2023-09-29 15:53:08.000000 api-deploy-0.9.2/setup.py
+drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-11-03 10:39:57.502077 api-deploy-0.9.3/
+-rw-r--r--   0 fabian     (501) staff       (20)       42 2023-09-29 15:31:13.000000 api-deploy-0.9.3/MANIFEST.in
+-rw-r--r--   0 fabian     (501) staff       (20)      740 2023-11-03 10:39:57.501953 api-deploy-0.9.3/PKG-INFO
+-rw-r--r--   0 fabian     (501) staff       (20)       12 2022-12-17 05:34:22.000000 api-deploy-0.9.3/README.md
+drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-11-03 10:39:57.499604 api-deploy-0.9.3/api_deploy/
+-rw-r--r--   0 fabian     (501) staff       (20)       18 2023-11-03 10:39:53.000000 api-deploy-0.9.3/api_deploy/__init__.py
+-rw-r--r--   0 fabian     (501) staff       (20)     3228 2023-10-05 16:17:32.000000 api-deploy-0.9.3/api_deploy/cli.py
+-rw-r--r--   0 fabian     (501) staff       (20)     2400 2023-05-09 14:47:12.000000 api-deploy-0.9.3/api_deploy/client.py
+-rw-r--r--   0 fabian     (501) staff       (20)     1889 2023-11-02 11:58:11.000000 api-deploy-0.9.3/api_deploy/config.py
+-rw-r--r--   0 fabian     (501) staff       (20)    18368 2023-11-02 12:06:55.000000 api-deploy-0.9.3/api_deploy/converters.py
+drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-11-03 10:39:57.501312 api-deploy-0.9.3/api_deploy/processors/
+-rw-r--r--   0 fabian     (501) staff       (20)        0 2023-09-29 15:24:43.000000 api-deploy-0.9.3/api_deploy/processors/__init__.py
+-rw-r--r--   0 fabian     (501) staff       (20)      308 2023-09-29 15:24:43.000000 api-deploy-0.9.3/api_deploy/processors/abstract_processor.py
+-rw-r--r--   0 fabian     (501) staff       (20)     4975 2023-10-06 05:28:47.000000 api-deploy-0.9.3/api_deploy/processors/code_generator.py
+-rw-r--r--   0 fabian     (501) staff       (20)     1548 2023-11-02 16:56:49.000000 api-deploy-0.9.3/api_deploy/processors/strict_processor.py
+drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-11-03 10:39:57.501688 api-deploy-0.9.3/api_deploy/processors/templates/
+-rw-r--r--   0 fabian     (501) staff       (20)      329 2023-10-17 09:29:44.000000 api-deploy-0.9.3/api_deploy/processors/templates/typescript.jinja2
+-rw-r--r--   0 fabian     (501) staff       (20)      784 2023-11-03 10:38:52.000000 api-deploy-0.9.3/api_deploy/processors/templates/typescript.object.jinja2
+-rw-r--r--   0 fabian     (501) staff       (20)     1075 2023-10-05 13:44:18.000000 api-deploy-0.9.3/api_deploy/schema.py
+drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-11-03 10:39:57.500563 api-deploy-0.9.3/api_deploy.egg-info/
+-rw-r--r--   0 fabian     (501) staff       (20)      740 2023-11-03 10:39:57.000000 api-deploy-0.9.3/api_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 fabian     (501) staff       (20)      665 2023-11-03 10:39:57.000000 api-deploy-0.9.3/api_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 fabian     (501) staff       (20)        1 2023-11-03 10:39:57.000000 api-deploy-0.9.3/api_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 fabian     (501) staff       (20)       44 2023-11-03 10:39:57.000000 api-deploy-0.9.3/api_deploy.egg-info/entry_points.txt
+-rw-r--r--   0 fabian     (501) staff       (20)        1 2022-12-17 05:34:25.000000 api-deploy-0.9.3/api_deploy.egg-info/not-zip-safe
+-rw-r--r--   0 fabian     (501) staff       (20)      102 2023-11-03 10:39:57.000000 api-deploy-0.9.3/api_deploy.egg-info/requires.txt
+-rw-r--r--   0 fabian     (501) staff       (20)       11 2023-11-03 10:39:57.000000 api-deploy-0.9.3/api_deploy.egg-info/top_level.txt
+-rw-r--r--   0 fabian     (501) staff       (20)       38 2023-11-03 10:39:57.502113 api-deploy-0.9.3/setup.cfg
+-rw-r--r--   0 fabian     (501) staff       (20)     1428 2023-09-29 15:53:08.000000 api-deploy-0.9.3/setup.py
```

### Comparing `api-deploy-0.9.2/PKG-INFO` & `api-deploy-0.9.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: api-deploy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Manage Amazon REST API Gateway deployments
 Home-page: https://github.com/fabfuel/api-deploy
 Author: Fabian Fuelling
 Author-email: pypi@fabfuel.de
 License: BSD-3-Clause
-Download-URL: https://github.com/fabfuel/api-deploy/archive/0.9.2.tar.gz
+Download-URL: https://github.com/fabfuel/api-deploy/archive/0.9.3.tar.gz
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
```

### Comparing `api-deploy-0.9.2/api_deploy/cli.py` & `api-deploy-0.9.3/api_deploy/cli.py`

 * *Files identical despite different names*

### Comparing `api-deploy-0.9.2/api_deploy/client.py` & `api-deploy-0.9.3/api_deploy/client.py`

 * *Files identical despite different names*

### Comparing `api-deploy-0.9.2/api_deploy/config.py` & `api-deploy-0.9.3/api_deploy/config.py`

 * *Files identical despite different names*

### Comparing `api-deploy-0.9.2/api_deploy/converters.py` & `api-deploy-0.9.3/api_deploy/converters.py`

 * *Files identical despite different names*

### Comparing `api-deploy-0.9.2/api_deploy/processors/code_generator.py` & `api-deploy-0.9.3/api_deploy/processors/code_generator.py`

 * *Files identical despite different names*

### Comparing `api-deploy-0.9.2/api_deploy/processors/strict_processor.py` & `api-deploy-0.9.3/api_deploy/processors/strict_processor.py`

 * *Files identical despite different names*

### Comparing `api-deploy-0.9.2/api_deploy/processors/templates/typescript.object.jinja2` & `api-deploy-0.9.3/api_deploy/processors/templates/typescript.object.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,25 @@
     * {{ property.name }}
 {%- if property.example %}
     * Example: {{ property.example }}
 {%- endif %}
     */
   {{ property.name }}{{ '?' if not property.required }}:
 
-{%- if property.types == ['object'] -%}
-    {% with properties=property.properties %}
-        {% include 'typescript.object.jinja2' %}
-    {%- endwith -%}
+{%- if 'object' in property.types -%}
+    {%- if property.properties -%}
+        {% with properties=property.properties %}
+            {% include 'typescript.object.jinja2' %}
+        {%- endwith -%}
+    {% else %}
+        object
+    {%  endif %}
+    {%- if 'null' in property.types -%}
+        | null
+    {%- endif -%}
 {%- else -%}
     {%- if property.enum -%}
         {{ property.enum|join(' | ') }}
     {%- else -%}
         {{ property.types|join(' | ') }}
     {%- endif -%}
 {%- endif -%}
```

### Comparing `api-deploy-0.9.2/api_deploy/schema.py` & `api-deploy-0.9.3/api_deploy/schema.py`

 * *Files identical despite different names*

### Comparing `api-deploy-0.9.2/api_deploy.egg-info/PKG-INFO` & `api-deploy-0.9.3/api_deploy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: api-deploy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Manage Amazon REST API Gateway deployments
 Home-page: https://github.com/fabfuel/api-deploy
 Author: Fabian Fuelling
 Author-email: pypi@fabfuel.de
 License: BSD-3-Clause
-Download-URL: https://github.com/fabfuel/api-deploy/archive/0.9.2.tar.gz
+Download-URL: https://github.com/fabfuel/api-deploy/archive/0.9.3.tar.gz
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
```

### Comparing `api-deploy-0.9.2/api_deploy.egg-info/SOURCES.txt` & `api-deploy-0.9.3/api_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `api-deploy-0.9.2/setup.py` & `api-deploy-0.9.3/setup.py`

 * *Files identical despite different names*

