# Comparing `tmp/injector_collections-0.0.8.tar.gz` & `tmp/injector_collections-0.0.9.tar.gz`

## Comparing `injector_collections-0.0.8.tar` & `injector_collections-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 injector_collections-0.0.8/src/injector_collections/Collection.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.8/src/injector_collections/CollectionItem.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 injector_collections-0.0.8/src/injector_collections/Generator.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 injector_collections-0.0.8/src/injector_collections/__init__.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 injector_collections-0.0.8/src/injector_collections/collections.jinja
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.8/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.8/LICENSE
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 injector_collections-0.0.8/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 injector_collections-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 injector_collections-0.0.9/src/injector_collections/Collection.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.9/src/injector_collections/CollectionItem.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 injector_collections-0.0.9/src/injector_collections/Generator.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 injector_collections-0.0.9/src/injector_collections/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 injector_collections-0.0.9/src/injector_collections/collections.jinja
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 injector_collections-0.0.9/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 injector_collections-0.0.9/PKG-INFO
```

### Comparing `injector_collections-0.0.8/src/injector_collections/CollectionItem.py` & `injector_collections-0.0.9/src/injector_collections/CollectionItem.py`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.8/src/injector_collections/Generator.py` & `injector_collections-0.0.9/src/injector_collections/Generator.py`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.8/src/injector_collections/collections.jinja` & `injector_collections-0.0.9/src/injector_collections/collections.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 {%- for (className, class) in citems %}
 from {{ class.__module__ }} import {{ className }}
 {%- endfor %}
 {%- endfor %}
 
 {%- for collection, citems in collectionItems|items %}
 {% if True %}{% endif %}
-class {{ className }}(Collection):
+class {{ collection.__name__ }}(Collection):
     @{{ inject.__name__ }}
     def __init__(
             self,
             {%- for (className, class) in citems %}
             v{{ className }}: {{ className }},
             {%- endfor %}
             ) -> None:
```

### Comparing `injector_collections-0.0.8/LICENSE` & `injector_collections-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.8/README.md` & `injector_collections-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.8/pyproject.toml` & `injector_collections-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "injector_collections"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Benjamin Schnitzler", email="regenbogenbauer@web.de" },
 ]
 description = "Collections for the Injector Package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `injector_collections-0.0.8/PKG-INFO` & `injector_collections-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: injector_collections
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collections for the Injector Package
 Project-URL: Homepage, https://github.com/bschnitz/injector_collections
 Project-URL: Issues, https://github.com/bschnitz/injector_collections/issues
 Author-email: Benjamin Schnitzler <regenbogenbauer@web.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

