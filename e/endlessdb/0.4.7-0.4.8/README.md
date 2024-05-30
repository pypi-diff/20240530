# Comparing `tmp/endlessdb-0.4.7.tar.gz` & `tmp/endlessdb-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endlessdb-0.4.7.tar", last modified: Wed May 29 20:05:44 2024, max compression
+gzip compressed data, was "endlessdb-0.4.8.tar", last modified: Wed May 29 21:28:31 2024, max compression
```

## Comparing `endlessdb-0.4.7.tar` & `endlessdb-0.4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 20:05:44.624713 endlessdb-0.4.7/
--rw-rw-rw-   0        0        0    11524 2024-05-20 13:50:18.000000 endlessdb-0.4.7/LICENSE.txt
--rw-rw-rw-   0        0        0    14363 2024-05-29 20:05:44.622710 endlessdb-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-05-29 01:30:15.000000 endlessdb-0.4.7/README.md
--rw-rw-rw-   0        0        0      886 2024-05-29 20:05:31.000000 endlessdb-0.4.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 20:05:44.625714 endlessdb-0.4.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-29 20:05:44.608300 endlessdb-0.4.7/src/
--rw-rw-rw-   0        0        0       23 2024-05-28 22:01:22.000000 endlessdb-0.4.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:05:44.621709 endlessdb-0.4.7/src/endlessdb.egg-info/
--rw-rw-rw-   0        0        0    14363 2024-05-29 20:05:44.000000 endlessdb-0.4.7/src/endlessdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-29 20:05:44.000000 endlessdb-0.4.7/src/endlessdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 20:05:44.000000 endlessdb-0.4.7/src/endlessdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-29 20:05:44.000000 endlessdb-0.4.7/src/endlessdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-29 20:05:44.000000 endlessdb-0.4.7/src/endlessdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    40991 2024-05-29 20:04:39.000000 endlessdb-0.4.7/src/endlessdb.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:05:44.619710 endlessdb-0.4.7/tests/
--rw-rw-rw-   0        0        0    10866 2024-05-29 18:55:49.000000 endlessdb-0.4.7/tests/test_endlessddb.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:28:31.663493 endlessdb-0.4.8/
+-rw-rw-rw-   0        0        0    11524 2024-05-20 13:50:18.000000 endlessdb-0.4.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    14363 2024-05-29 21:28:31.658492 endlessdb-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-05-29 01:30:15.000000 endlessdb-0.4.8/README.md
+-rw-rw-rw-   0        0        0      886 2024-05-29 21:28:18.000000 endlessdb-0.4.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 21:28:31.664492 endlessdb-0.4.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 21:28:31.569886 endlessdb-0.4.8/src/
+-rw-rw-rw-   0        0        0       23 2024-05-28 22:01:22.000000 endlessdb-0.4.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:28:31.652492 endlessdb-0.4.8/src/endlessdb.egg-info/
+-rw-rw-rw-   0        0        0    14363 2024-05-29 21:28:31.000000 endlessdb-0.4.8/src/endlessdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-29 21:28:31.000000 endlessdb-0.4.8/src/endlessdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 21:28:31.000000 endlessdb-0.4.8/src/endlessdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 21:28:31.000000 endlessdb-0.4.8/src/endlessdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-29 21:28:31.000000 endlessdb-0.4.8/src/endlessdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    40775 2024-05-29 21:27:06.000000 endlessdb-0.4.8/src/endlessdb.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:28:31.632331 endlessdb-0.4.8/tests/
+-rw-rw-rw-   0        0        0    10866 2024-05-29 18:55:49.000000 endlessdb-0.4.8/tests/test_endlessddb.py
```

### Comparing `endlessdb-0.4.7/LICENSE.txt` & `endlessdb-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `endlessdb-0.4.7/PKG-INFO` & `endlessdb-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endlessdb
-Version: 0.4.7
+Version: 0.4.8
 Summary: Endless Database with pyyaml and pymongo
 Author-email: Andrew Berlin <a.berlin@33solutions.company>
 Maintainer-email: Andrew Berlin <a.berlin@33solutions.company>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `endlessdb-0.4.7/pyproject.toml` & `endlessdb-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "endlessdb"
-version = "0.4.7"
+version = "0.4.8"
 requires-python = ">=3.8"
 description = "Endless Database with pyyaml and pymongo"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `endlessdb-0.4.7/src/endlessdb.egg-info/PKG-INFO` & `endlessdb-0.4.8/src/endlessdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endlessdb
-Version: 0.4.7
+Version: 0.4.8
 Summary: Endless Database with pyyaml and pymongo
 Author-email: Andrew Berlin <a.berlin@33solutions.company>
 Maintainer-email: Andrew Berlin <a.berlin@33solutions.company>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `endlessdb-0.4.7/src/endlessdb.py` & `endlessdb-0.4.8/src/endlessdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                     collection = self.collection()
                     collection().reload()
                     return                    
                 else:
                     obj = mongo.find_one({"_id": self._key})
                     if obj is None:
                         self.virtual = True
-                        return #raise Exception(f"Document {self._key} not found in collection {_parent}")
+                        return
                     else:
                         self.virtual = False                        
             else:
                 _parent()._reload(None)
                 return       
             
         if self._key is None:
@@ -206,24 +206,21 @@
                 self._key = int(path[-1])
                 pass
             except:
                 self._key = path[-1]
             
         virtual = self.virtual
                        
-        #self._key = path[len(path) - 1]
-        
         _keys  = self._keys.copy()
         self._keys.clear()
         _path = f"{self.path(True)}"
         _edb = self.edb()
         for _key in obj:
             value = obj[_key]
             self._keys.append(_key)  
-            #self.__slots__.append(key)
             
             if isinstance(value, bson.dbref.DBRef):
                 value = _edb[value.collection][value.id]                                
                 
             if self.descendant_expected is None:
                 if isinstance(value, EndlessDocument) or isinstance(value, dict):                
                     if self.static:                
@@ -498,30 +495,31 @@
         
     def repr(self, srepr = None):
         parent = self.parent()
         repr = ""
         if self.debug:
             repr += "🐞"
         
-        repr += "📚"
-        
-        if self.protected:
-            repr += "🔒"
-        else:
-            repr += "🔓"
-        
-        repr += f"{self._key}"
-        repr += "{" + f"ℓ{self.len()}" + "}"
+        if self._edb is None:
+            repr = f"⚓{self.path(True)}"
+        else:    
+            repr += "📚"
+            
+            if self.protected:
+                repr += "🔒"
+            else:
+                repr += "🔓"
+            
+            repr += f"{self._key}"
+            repr += "{" + f"ℓ{self.len()}" + "}"
             
         if srepr is not None:
             repr += f'/{srepr}'        
                
         if parent is None:
-            if self._edb is None:
-                return f"⚓{self.path(True)}"
             return repr           
         else:
             return parent().repr(repr)            
     
     def keys(self):
         if self._collection is None:
             return self._keys
@@ -1054,15 +1052,14 @@
         if collection is None:
             raise Exception(f"{self} is read-only")
         
         if isinstance(value, dict):
             collection.update_one({'_id': key }, {"$set": value}, upsert=True)            
             _path = f"{_self.path(True)}/{key}"
             documents = _self.edb()().documents()
-            #_path = f"{self._key}.{path}"
             if _path in documents:
                 documents[_path]().reload()                         
         else:
             raise Exception(f"You must pass dict value with filled _id pproperty {self}")
     
     def __getitem__(self, key):
         if key is None:
@@ -1076,15 +1073,14 @@
             key = int(key)
         except:
             pass
         
         if isinstance(key, int):
             return self.__getattr__(key)
         
-        #key = f"{_self.path()}/{key}"
         path = key.replace("/", ".").split(".", 1)
         if len(path) > 1:
             next_path = path[0]
             try:
                 next_path = int(next_path)
             except:
                 pass            
@@ -1232,9 +1228,8 @@
         if edb is None:
             edb = EndlessDatabase()
         self._edb = edb
         _config = self._edb().config()
         self._cfg = _config[config_key]
         self._log = Logger(__name__)
         self.DEBUG = self._cfg(False, create=True).debug
-        self._edb.load_defaults()
-        
+        self._edb().load_defaults()
```

### Comparing `endlessdb-0.4.7/tests/test_endlessddb.py` & `endlessdb-0.4.8/tests/test_endlessddb.py`

 * *Files identical despite different names*

