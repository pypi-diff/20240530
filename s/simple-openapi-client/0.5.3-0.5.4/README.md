# Comparing `tmp/simple_openapi_client-0.5.3.tar.gz` & `tmp/simple_openapi_client-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_openapi_client-0.5.3.tar", max compression
+gzip compressed data, was "simple_openapi_client-0.5.4.tar", max compression
```

## Comparing `simple_openapi_client-0.5.3.tar` & `simple_openapi_client-0.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1423 2022-12-18 02:39:16.255314 simple_openapi_client-0.5.3/README.md
--rw-r--r--   0        0        0      613 2023-11-14 19:27:44.492588 simple_openapi_client-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      161 2022-12-18 02:39:16.257314 simple_openapi_client-0.5.3/simple_openapi_client/__init__.py
--rw-r--r--   0        0        0      126 2022-12-18 02:39:16.257314 simple_openapi_client-0.5.3/simple_openapi_client/config.py
--rw-r--r--   0        0        0     5929 2022-12-18 02:39:16.257314 simple_openapi_client-0.5.3/simple_openapi_client/maker.py
--rw-r--r--   0        0        0       61 2022-12-18 02:39:16.258314 simple_openapi_client-0.5.3/simple_openapi_client/openapi/__init__.py
--rw-r--r--   0        0        0      560 2022-12-18 02:39:16.258314 simple_openapi_client-0.5.3/simple_openapi_client/openapi/document.py
--rw-r--r--   0        0        0      361 2022-12-18 02:39:16.258314 simple_openapi_client-0.5.3/simple_openapi_client/openapi/info.py
--rw-r--r--   0        0        0     3461 2022-12-18 02:39:16.258314 simple_openapi_client-0.5.3/simple_openapi_client/openapi/path.py
--rw-r--r--   0        0        0      451 2022-12-18 02:39:16.259314 simple_openapi_client-0.5.3/simple_openapi_client/parser.py
--rw-r--r--   0        0        0     7670 2023-08-29 21:00:38.318230 simple_openapi_client-0.5.3/simple_openapi_client/templates/async_client.jinja
--rw-r--r--   0        0        0     4030 2023-08-17 15:25:11.999920 simple_openapi_client-0.5.3/simple_openapi_client/templates/async_method.jinja
--rw-r--r--   0        0        0     7473 2023-08-18 18:12:18.626577 simple_openapi_client-0.5.3/simple_openapi_client/templates/client.jinja
--rw-r--r--   0        0        0     4010 2023-08-17 15:25:11.999920 simple_openapi_client-0.5.3/simple_openapi_client/templates/method.jinja
--rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 simple_openapi_client-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1423 2024-05-28 20:51:43.994319 simple_openapi_client-0.5.4/README.md
+-rw-r--r--   0        0        0      563 2024-05-30 13:16:01.216666 simple_openapi_client-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      161 2024-05-28 20:51:43.994319 simple_openapi_client-0.5.4/simple_openapi_client/__init__.py
+-rw-r--r--   0        0        0      126 2024-05-28 20:51:43.994319 simple_openapi_client-0.5.4/simple_openapi_client/config.py
+-rw-r--r--   0        0        0     5929 2024-05-29 18:36:17.139368 simple_openapi_client-0.5.4/simple_openapi_client/maker.py
+-rw-r--r--   0        0        0       61 2024-05-28 20:51:43.995319 simple_openapi_client-0.5.4/simple_openapi_client/openapi/__init__.py
+-rw-r--r--   0        0        0      560 2024-05-28 20:51:43.995319 simple_openapi_client-0.5.4/simple_openapi_client/openapi/document.py
+-rw-r--r--   0        0        0      361 2024-05-28 20:51:43.995319 simple_openapi_client-0.5.4/simple_openapi_client/openapi/info.py
+-rw-r--r--   0        0        0     3461 2024-05-28 20:51:43.995319 simple_openapi_client-0.5.4/simple_openapi_client/openapi/path.py
+-rw-r--r--   0        0        0      451 2024-05-29 18:09:28.299446 simple_openapi_client-0.5.4/simple_openapi_client/parser.py
+-rw-r--r--   0        0        0     7670 2024-05-28 20:51:43.995319 simple_openapi_client-0.5.4/simple_openapi_client/templates/async_client.jinja
+-rw-r--r--   0        0        0     4244 2024-05-30 13:16:01.216666 simple_openapi_client-0.5.4/simple_openapi_client/templates/async_method.jinja
+-rw-r--r--   0        0        0     7473 2024-05-28 20:51:43.995319 simple_openapi_client-0.5.4/simple_openapi_client/templates/client.jinja
+-rw-r--r--   0        0        0     4224 2024-05-30 13:16:01.216666 simple_openapi_client-0.5.4/simple_openapi_client/templates/method.jinja
+-rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 simple_openapi_client-0.5.4/PKG-INFO
```

### Comparing `simple_openapi_client-0.5.3/README.md` & `simple_openapi_client-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `simple_openapi_client-0.5.3/pyproject.toml` & `simple_openapi_client-0.5.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 [tool.poetry]
 name = "simple-openapi-client"
-version = "0.5.3"
+version = "0.5.4"
 description = "OpenAPI Python client generator that follows the KISS principle."
 authors = ["Gabriel Couture <gacou54@gmail.ca>"]
 license = "BSD-3-Clause"
 readme = 'README.md'
 homepage = 'https://github.com/gacou54/openapi-client'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0"
 Jinja2 = "^3.1.2"
-black = "^23.7.0"
-
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
+black = "^24.4.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `simple_openapi_client-0.5.3/simple_openapi_client/maker.py` & `simple_openapi_client-0.5.4/simple_openapi_client/maker.py`

 * *Files identical despite different names*

### Comparing `simple_openapi_client-0.5.3/simple_openapi_client/openapi/document.py` & `simple_openapi_client-0.5.4/simple_openapi_client/openapi/document.py`

 * *Files identical despite different names*

### Comparing `simple_openapi_client-0.5.3/simple_openapi_client/openapi/path.py` & `simple_openapi_client-0.5.4/simple_openapi_client/openapi/path.py`

 * *Files identical despite different names*

### Comparing `simple_openapi_client-0.5.3/simple_openapi_client/templates/async_client.jinja` & `simple_openapi_client-0.5.4/simple_openapi_client/templates/async_client.jinja`

 * *Files identical despite different names*

### Comparing `simple_openapi_client-0.5.3/simple_openapi_client/templates/async_method.jinja` & `simple_openapi_client-0.5.4/simple_openapi_client/templates/async_method.jinja`

 * *Files 15% similar despite different names*

```diff
@@ -18,72 +18,73 @@
             ) -> Union[Dict, List, str, bytes, int, httpx.Response]:
         """(async) {{ OPERATION.summary }}
 
         {{ OPERATION.description }}
         Tags: {{ ','.join(OPERATION.tags) }}
         {%- if OPERATION.externalDocs %}ExternaDocs: {{ OPERATION.externalDocs }}{% endif %}
 
+        {%- if PATH_PARAMETERS or REQUEST_BODY.json or REQUEST_BODY.files or REQUEST_BODY.data or QUERY_PARAMETERS or HEADERS %}
+
         Parameters
         ----------
-        {% if PATH_PARAMETERS -%}
-        {% for name, description in PATH_PARAMETERS.items() -%}
+        {%- if PATH_PARAMETERS %}
+        {%- for name, description in PATH_PARAMETERS.items() %}
         {{ name }}
             {{ description }}
-        {% endfor -%}
-        {% endif -%}
-
-        {% if REQUEST_BODY.json %}json
+        {%- endfor %}
+        {%- endif %}
+        {%- if REQUEST_BODY.json %}
+        json
         {%- for request_data in REQUEST_BODY.json %}
-            {% if request_data -%}
+            {%- if request_data %}
             Dictionary with the following keys:
             {%- for property_name, property in request_data.properties.items() %}
-            "{{ property_name }}": {{ property['description'] }}
+              "{{ property_name }}": {{ property['description'] }}
             {%- endfor %}
-            {%- endif -%}
+            {%- endif %}
         {% endfor -%}
-        {% endif -%}
-
-        {% if REQUEST_BODY.files %}files
+        {%- endif %}
+        {%- if REQUEST_BODY.files %}
+        files
         {%- for request_data in REQUEST_BODY.files %}
-            {% if request_data -%}Files:
+            {%- if request_data %}
+            Files:
             {%- for property_name, property in request_data.properties.items() %}
                 "{{ property_name }}": {{ property['description'] }}
             {%- endfor %}
-            {%- endif -%}
+            {%- endif %}
         {% endfor -%}
-        {% endif -%}
-
-        {% if REQUEST_BODY.data %}
+        {%- endif %}
+        {%- if REQUEST_BODY.data %}
         data
         {%- for request_data in REQUEST_BODY.data %}
             {{ request_data.description }}
-        {% endfor -%}
-        {% endif -%}
-
-        {% if REQUEST_BODY.content %}content
-        {%- for request_data in REQUEST_BODY.content %}
-            - (Content-Type: "{{ request_data.content_type }}") {{ request_data.description }}
-        {% endfor -%}
-        {% endif -%}
-
-        {% if QUERY_PARAMETERS -%}
+        {%- endfor -%}
+        {%- endif %}
+        {%- if REQUEST_BODY.content %}
+        content
+            {%- for request_data in REQUEST_BODY.content %}
+                - (Content-Type: "{{ request_data.content_type }}") {{ request_data.description }}
+            {%- endfor %}
+        {%- endif %}
+        {%- if QUERY_PARAMETERS %}
         params
             Dictionary of optional parameters:
-        {%- for name, query in QUERY_PARAMETERS.items() %}
-            "{{ name }}" ({{ query.type }}): {{ query.description }}
-        {%- endfor -%}
-        {% endif -%}
-
-        {% if HEADERS -%}
+            {%- for name, query in QUERY_PARAMETERS.items() %}
+                "{{ name }}" ({{ query.type }}): {{ query.description }}
+            {%- endfor %}
+        {%- endif %}
+        {%- if HEADERS %}
         headers
             Dictionary of optional headers:
-            {% for name, header in HEADERS.items() -%}
+            {%- for name, header in HEADERS.items() %}
                 "{{ name }}" ({{ header.type }}): {{ header.description }}
-            {% endfor -%}
-        {% endif %}
+            {%- endfor %}
+        {%- endif %}
+        {%- endif %}
 
         Returns
         -------
         Union[Dict, List, str, bytes, int, httpx.Response]
         {%- for response in RESPONSES %}
             {{ response.description }}
         {%- endfor %}
```

### Comparing `simple_openapi_client-0.5.3/simple_openapi_client/templates/client.jinja` & `simple_openapi_client-0.5.4/simple_openapi_client/templates/client.jinja`

 * *Files identical despite different names*

### Comparing `simple_openapi_client-0.5.3/simple_openapi_client/templates/method.jinja` & `simple_openapi_client-0.5.4/simple_openapi_client/templates/method.jinja`

 * *Files 21% similar despite different names*

```diff
@@ -18,72 +18,73 @@
             ) -> Union[Dict, List, str, bytes, int, httpx.Response]:
         """{{ OPERATION.summary }}
 
         {{ OPERATION.description }}
         Tags: {{ ','.join(OPERATION.tags) }}
         {%- if OPERATION.externalDocs %}ExternaDocs: {{ OPERATION.externalDocs }}{% endif %}
 
+        {%- if PATH_PARAMETERS or REQUEST_BODY.json or REQUEST_BODY.files or REQUEST_BODY.data or QUERY_PARAMETERS or HEADERS %}
+
         Parameters
         ----------
-        {% if PATH_PARAMETERS -%}
-        {% for name, description in PATH_PARAMETERS.items() -%}
+        {%- if PATH_PARAMETERS %}
+        {%- for name, description in PATH_PARAMETERS.items() %}
         {{ name }}
             {{ description }}
-        {% endfor -%}
-        {% endif -%}
-
-        {% if REQUEST_BODY.json %}json
+        {%- endfor %}
+        {%- endif %}
+        {%- if REQUEST_BODY.json %}
+        json
         {%- for request_data in REQUEST_BODY.json %}
-            {% if request_data -%}
+            {%- if request_data %}
             Dictionary with the following keys:
             {%- for property_name, property in request_data.properties.items() %}
-            "{{ property_name }}": {{ property['description'] }}
+              "{{ property_name }}": {{ property['description'] }}
             {%- endfor %}
-            {%- endif -%}
+            {%- endif %}
         {% endfor -%}
-        {% endif -%}
-
-        {% if REQUEST_BODY.files %}files
+        {%- endif %}
+        {%- if REQUEST_BODY.files %}
+        files
         {%- for request_data in REQUEST_BODY.files %}
-            {% if request_data -%}Files:
+            {%- if request_data %}
+            Files:
             {%- for property_name, property in request_data.properties.items() %}
                 "{{ property_name }}": {{ property['description'] }}
             {%- endfor %}
-            {%- endif -%}
+            {%- endif %}
         {% endfor -%}
-        {% endif -%}
-
-        {% if REQUEST_BODY.data %}
+        {%- endif %}
+        {%- if REQUEST_BODY.data %}
         data
         {%- for request_data in REQUEST_BODY.data %}
             {{ request_data.description }}
-        {% endfor -%}
-        {% endif -%}
-
-        {% if REQUEST_BODY.content %}content
-        {%- for request_data in REQUEST_BODY.content %}
-            - (Content-Type: "{{ request_data.content_type }}") {{ request_data.description }}
-        {% endfor -%}
-        {% endif -%}
-
-        {% if QUERY_PARAMETERS -%}
+        {%- endfor -%}
+        {%- endif %}
+        {%- if REQUEST_BODY.content %}
+        content
+            {%- for request_data in REQUEST_BODY.content %}
+                - (Content-Type: "{{ request_data.content_type }}") {{ request_data.description }}
+            {%- endfor %}
+        {%- endif %}
+        {%- if QUERY_PARAMETERS %}
         params
             Dictionary of optional parameters:
-        {%- for name, query in QUERY_PARAMETERS.items() %}
-            "{{ name }}" ({{ query.type }}): {{ query.description }}
-        {%- endfor -%}
-        {% endif -%}
-
-        {% if HEADERS -%}
+            {%- for name, query in QUERY_PARAMETERS.items() %}
+                "{{ name }}" ({{ query.type }}): {{ query.description }}
+            {%- endfor %}
+        {%- endif %}
+        {%- if HEADERS %}
         headers
             Dictionary of optional headers:
-            {% for name, header in HEADERS.items() -%}
+            {%- for name, header in HEADERS.items() %}
                 "{{ name }}" ({{ header.type }}): {{ header.description }}
-            {% endfor -%}
-        {% endif %}
+            {%- endfor %}
+        {%- endif %}
+        {%- endif %}
 
         Returns
         -------
         Union[Dict, List, str, bytes, int, httpx.Response]
         {%- for response in RESPONSES %}
             {{ response.description }}
         {%- endfor %}
```

### Comparing `simple_openapi_client-0.5.3/PKG-INFO` & `simple_openapi_client-0.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: simple-openapi-client
-Version: 0.5.3
+Version: 0.5.4
 Summary: OpenAPI Python client generator that follows the KISS principle.
 Home-page: https://github.com/gacou54/openapi-client
 License: BSD-3-Clause
 Author: Gabriel Couture
 Author-email: gacou54@gmail.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: black (>=23.7.0,<24.0.0)
+Requires-Dist: black (>=24.4.2,<25.0.0)
 Requires-Dist: httpx (>=0,<1)
 Description-Content-Type: text/markdown
 
 # Simple Open API Client generator
 
 This project was made to generate a simple client (async or not) from an openapi
 specifications (unlike other client generators, which typically produce
```

