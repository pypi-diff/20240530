# Comparing `tmp/injector_collections-0.0.6.tar.gz` & `tmp/injector_collections-0.0.7.tar.gz`

## Comparing `injector_collections-0.0.6.tar` & `injector_collections-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 injector_collections-0.0.6/src/injector_collections/Collection.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.6/src/injector_collections/CollectionItem.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 injector_collections-0.0.6/src/injector_collections/Generator.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 injector_collections-0.0.6/src/injector_collections/__init__.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 injector_collections-0.0.6/src/injector_collections/collections.jinja
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.6/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.6/LICENSE
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 injector_collections-0.0.6/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 injector_collections-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 injector_collections-0.0.7/src/injector_collections/Collection.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.7/src/injector_collections/CollectionItem.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 injector_collections-0.0.7/src/injector_collections/Generator.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 injector_collections-0.0.7/src/injector_collections/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 injector_collections-0.0.7/src/injector_collections/collections.jinja
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.7/LICENSE
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 injector_collections-0.0.7/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 injector_collections-0.0.7/PKG-INFO
```

### Comparing `injector_collections-0.0.6/src/injector_collections/CollectionItem.py` & `injector_collections-0.0.7/src/injector_collections/CollectionItem.py`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.6/src/injector_collections/Generator.py` & `injector_collections-0.0.7/src/injector_collections/Generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,14 @@
             pass
 
         collectionMetadata = self.gatherCollectionMetadata(scannedModules)
 
         with open(f'{collectionModuleDirectory}/{self.generatedCollectionsFileName}', 'w') as f:
             f.write(self.renderCollectionsTemplate(inject, collectionMetadata))
 
-        # reload the collections module to make generated collections
-        # visible when using import from other places
-        # collectionModule = importlib.import_module(collectionModule)
-        # importlib.reload(collectionModule.generated)
-        # importlib.reload(collectionModule)
-
     def getModuleDirectory(self, module: str|ModuleType) -> str:
         if isinstance(module, str):
             moduleSpec = util.find_spec(module)
             modulePath = moduleSpec.origin
         else:
             modulePath = module.__file__
         assert(modulePath is not None)
```

### Comparing `injector_collections-0.0.6/src/injector_collections/collections.jinja` & `injector_collections-0.0.7/src/injector_collections/collections.jinja`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 {%- for collection, citems in collectionItems|items %}
 {%- for (key, className) in citems %}
 from {{ className.__module__ }} import {{ className.__name__ }}
 {%- endfor %}
 {%- endfor %}
 
 {%- for collection, citems in collectionItems|items %}
+{% if True %}{% endif %}
 class {{ collection.__name__ }}(Collection):
     @{{ inject.__name__ }}
     def __init__(
             self,
             {%- for (key, className) in citems %}
             v{{ className.__name__ }}: {{ className.__name__ }},
             {%- endfor %}
```

### Comparing `injector_collections-0.0.6/LICENSE` & `injector_collections-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.6/README.md` & `injector_collections-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.6/pyproject.toml` & `injector_collections-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "injector_collections"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Benjamin Schnitzler", email="regenbogenbauer@web.de" },
 ]
 description = "Collections for the Injector Package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `injector_collections-0.0.6/PKG-INFO` & `injector_collections-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: injector_collections
-Version: 0.0.6
+Version: 0.0.7
 Summary: Collections for the Injector Package
 Project-URL: Homepage, https://github.com/bschnitz/injector_collections
 Project-URL: Issues, https://github.com/bschnitz/injector_collections/issues
 Author-email: Benjamin Schnitzler <regenbogenbauer@web.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

