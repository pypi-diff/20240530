# Comparing `tmp/injector_collections-0.0.7.tar.gz` & `tmp/injector_collections-0.0.8.tar.gz`

## Comparing `injector_collections-0.0.7.tar` & `injector_collections-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 injector_collections-0.0.7/src/injector_collections/Collection.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.7/src/injector_collections/CollectionItem.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 injector_collections-0.0.7/src/injector_collections/Generator.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 injector_collections-0.0.7/src/injector_collections/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 injector_collections-0.0.7/src/injector_collections/collections.jinja
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.7/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.7/LICENSE
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 injector_collections-0.0.7/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 injector_collections-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 injector_collections-0.0.8/src/injector_collections/Collection.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.8/src/injector_collections/CollectionItem.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 injector_collections-0.0.8/src/injector_collections/Generator.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 injector_collections-0.0.8/src/injector_collections/__init__.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 injector_collections-0.0.8/src/injector_collections/collections.jinja
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.8/LICENSE
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 injector_collections-0.0.8/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 injector_collections-0.0.8/PKG-INFO
```

### Comparing `injector_collections-0.0.7/src/injector_collections/CollectionItem.py` & `injector_collections-0.0.8/src/injector_collections/CollectionItem.py`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.7/src/injector_collections/Generator.py` & `injector_collections-0.0.8/src/injector_collections/Generator.py`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.7/src/injector_collections/collections.jinja` & `injector_collections-0.0.8/src/injector_collections/collections.jinja`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from {{ inject.__module__ }} import {{ inject.__name__ }}
 from injector_collections import Collection
 {%- for collection, citems in collectionItems|items %}
-{%- for (key, className) in citems %}
-from {{ className.__module__ }} import {{ className.__name__ }}
+{%- for (className, class) in citems %}
+from {{ class.__module__ }} import {{ className }}
 {%- endfor %}
 {%- endfor %}
 
 {%- for collection, citems in collectionItems|items %}
 {% if True %}{% endif %}
-class {{ collection.__name__ }}(Collection):
+class {{ className }}(Collection):
     @{{ inject.__name__ }}
     def __init__(
             self,
-            {%- for (key, className) in citems %}
-            v{{ className.__name__ }}: {{ className.__name__ }},
+            {%- for (className, class) in citems %}
+            v{{ className }}: {{ className }},
             {%- endfor %}
             ) -> None:
         super().__init__()
-        {%- for (key, className) in citems %}
-        self[{{ key }}] = v{{ className.__name__ }}
+        {%- for (className, class) in citems %}
+        self[{{ className }}] = v{{ className }}
+        self.byClassname['{{ className }}'] = v{{ className }}
         {%- endfor %}
 {%- endfor %}
```

### Comparing `injector_collections-0.0.7/LICENSE` & `injector_collections-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.7/README.md` & `injector_collections-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.7/pyproject.toml` & `injector_collections-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "injector_collections"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Benjamin Schnitzler", email="regenbogenbauer@web.de" },
 ]
 description = "Collections for the Injector Package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `injector_collections-0.0.7/PKG-INFO` & `injector_collections-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: injector_collections
-Version: 0.0.7
+Version: 0.0.8
 Summary: Collections for the Injector Package
 Project-URL: Homepage, https://github.com/bschnitz/injector_collections
 Project-URL: Issues, https://github.com/bschnitz/injector_collections/issues
 Author-email: Benjamin Schnitzler <regenbogenbauer@web.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

