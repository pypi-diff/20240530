# Comparing `tmp/abcdict-0.0.2.tar.gz` & `tmp/abcdict-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abcdict-0.0.2.tar", last modified: Thu Apr 18 12:19:16 2024, max compression
+gzip compressed data, was "abcdict-0.0.5.tar", last modified: Thu May 30 10:47:36 2024, max compression
```

## Comparing `abcdict-0.0.2.tar` & `abcdict-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tudou      (501) staff       (20)        0 2024-04-18 12:19:16.590995 abcdict-0.0.2/
--rw-r--r--   0 tudou      (501) staff       (20)     1062 2024-04-18 12:15:37.000000 abcdict-0.0.2/LICENSE
--rw-r--r--   0 tudou      (501) staff       (20)      450 2024-04-18 12:19:16.590774 abcdict-0.0.2/PKG-INFO
--rw-r--r--   0 tudou      (501) staff       (20)       10 2024-04-18 12:15:37.000000 abcdict-0.0.2/README.md
--rw-r--r--   0 tudou      (501) staff       (20)      547 2024-04-18 12:15:37.000000 abcdict-0.0.2/pyproject.toml
--rw-r--r--   0 tudou      (501) staff       (20)       38 2024-04-18 12:19:16.591037 abcdict-0.0.2/setup.cfg
-drwxr-xr-x   0 tudou      (501) staff       (20)        0 2024-04-18 12:19:16.589866 abcdict-0.0.2/src/
--rw-r--r--   0 tudou      (501) staff       (20)       28 2024-04-18 12:15:37.000000 abcdict-0.0.2/src/__init__.py
-drwxr-xr-x   0 tudou      (501) staff       (20)        0 2024-04-18 12:19:16.590565 abcdict-0.0.2/src/abcDict.egg-info/
--rw-r--r--   0 tudou      (501) staff       (20)      450 2024-04-18 12:19:16.000000 abcdict-0.0.2/src/abcDict.egg-info/PKG-INFO
--rw-r--r--   0 tudou      (501) staff       (20)      215 2024-04-18 12:19:16.000000 abcdict-0.0.2/src/abcDict.egg-info/SOURCES.txt
--rw-r--r--   0 tudou      (501) staff       (20)        1 2024-04-18 12:19:16.000000 abcdict-0.0.2/src/abcDict.egg-info/dependency_links.txt
--rw-r--r--   0 tudou      (501) staff       (20)       22 2024-04-18 12:19:16.000000 abcdict-0.0.2/src/abcDict.egg-info/top_level.txt
--rw-r--r--   0 tudou      (501) staff       (20)     3305 2024-04-18 12:15:37.000000 abcdict-0.0.2/src/abcdict.py
--rw-r--r--   0 tudou      (501) staff       (20)       75 2024-04-18 12:15:37.000000 abcdict-0.0.2/src/util.py
+drwxr-xr-x   0 tudou      (501) staff       (20)        0 2024-05-30 10:47:36.388014 abcdict-0.0.5/
+-rw-r--r--   0 tudou      (501) staff       (20)     1062 2024-04-18 12:15:37.000000 abcdict-0.0.5/LICENSE
+-rw-r--r--   0 tudou      (501) staff       (20)      450 2024-05-30 10:47:36.387799 abcdict-0.0.5/PKG-INFO
+-rw-r--r--   0 tudou      (501) staff       (20)       10 2024-04-18 12:15:37.000000 abcdict-0.0.5/README.md
+-rw-r--r--   0 tudou      (501) staff       (20)      547 2024-05-30 10:47:03.000000 abcdict-0.0.5/pyproject.toml
+-rw-r--r--   0 tudou      (501) staff       (20)       38 2024-05-30 10:47:36.388053 abcdict-0.0.5/setup.cfg
+drwxr-xr-x   0 tudou      (501) staff       (20)        0 2024-05-30 10:47:36.386699 abcdict-0.0.5/src/
+-rw-r--r--   0 tudou      (501) staff       (20)      167 2024-05-30 10:47:03.000000 abcdict-0.0.5/src/__init__.py
+drwxr-xr-x   0 tudou      (501) staff       (20)        0 2024-05-30 10:47:36.387611 abcdict-0.0.5/src/abcDict.egg-info/
+-rw-r--r--   0 tudou      (501) staff       (20)      450 2024-05-30 10:47:36.000000 abcdict-0.0.5/src/abcDict.egg-info/PKG-INFO
+-rw-r--r--   0 tudou      (501) staff       (20)      218 2024-05-30 10:47:36.000000 abcdict-0.0.5/src/abcDict.egg-info/SOURCES.txt
+-rw-r--r--   0 tudou      (501) staff       (20)        1 2024-05-30 10:47:36.000000 abcdict-0.0.5/src/abcDict.egg-info/dependency_links.txt
+-rw-r--r--   0 tudou      (501) staff       (20)       25 2024-05-30 10:47:36.000000 abcdict-0.0.5/src/abcDict.egg-info/top_level.txt
+-rw-r--r--   0 tudou      (501) staff       (20)     2784 2024-05-30 10:47:03.000000 abcdict-0.0.5/src/abcdict.py
+-rw-r--r--   0 tudou      (501) staff       (20)     1914 2024-05-30 10:47:03.000000 abcdict-0.0.5/src/abcutil.py
```

### Comparing `abcdict-0.0.2/LICENSE` & `abcdict-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `abcdict-0.0.2/pyproject.toml` & `abcdict-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "PyYAML>=5.4.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "abcDict"
-version = "0.0.2"
+version = "0.0.5"
 authors = [
     { name="msbrm", email="cuihaniss@gmail.com" },
 ]
 description = "use yaml config easy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `abcdict-0.0.2/src/abcdict.py` & `abcdict-0.0.5/src/abcdict.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,38 @@
-import os
 import json
 from pathlib import Path
 
 import yaml
 
+from .abcutil import replace_env_variables
+
 
 class AbcDict(dict):
+    __charset__ = 'UTF-8'
+
     __k_keylist__ = [
         'update',
         'pop',
         'merge',
         'deep_merge',
         'dump'
     ]
 
+    __env_reType_dict__ = {
+        'int': int,
+        'float': float,
+        'str': str
+    }
+
     def __init__(self, d=None, **kwargs):
         d = self.__load__(d, **kwargs)
         for k, v in d.items():
             if isinstance(v, str):
-                if v.startswith('${') and v.endswith('}'):
-                    type_dict = {
-                        'int': int,
-                        'float': float,
-                        'str': str
-                    }
-                    env_k = v[2: -1]
-                    v_default, v_type = None, None
-                    if '|' in env_k:
-                        key_item = env_k.split('|')
-                        for info in key_item[1:]:
-                            if info.startswith('default:'):
-                                v_default = info.strip().replace('default:', '')
-                            if info.startswith('type:'):
-                                v_type = info.strip().replace('type:', '')
-                        env_k = key_item[0]
-                    v = os.getenv(env_k, v_default)
-                    if v_type in type_dict:
-                        v = type_dict[v_type](v)
+                if '${' in v:
+                    v = replace_env_variables(v)
             setattr(self, k, v)
 
         for k in self.__class__.__dict__.keys():
             if (
                 not (k.startswith('__') and k.endswith('__'))
                 and k not in (self.__k_keylist__)
             ):
@@ -66,15 +58,15 @@
             # d = {} if d is None else self.__load__(d)
             if d:
                 assert (
                     (isStr := isinstance(d, str)) or isinstance(d, Path)
                 ), f'parameter {d} error'
                 _d = Path(d) if isStr else d
                 assert _d.exists(), f'{d} not find'
-                d = yaml.safe_load(_d.open('r').read())
+                d = yaml.safe_load(_d.open('r', encoding=self.__charset__).read())
             else:
                 d = {}
         if kwargs:
             d.update(**kwargs)
         return d
 
     def update(self, e=None, **f):
@@ -83,22 +75,26 @@
         for k in d:
             setattr(self, k, d[k])
 
     def pop(self, k, d=None):
         delattr(self, k)
         return super(AbcDict, self).pop(k, d)
 
-    def merge(self, d):
+    def merge(self, d, **kwargs):
         self.__init__(d)
 
     def deep_merge(self, d=None, **kwargs):
         # d = self.__load__(d, **kwargs)
         # for k, v in d.items():
         #     setattr(self, k, v)
         # TODO deep merge
         pass
 
     def dump(self, save_path):
         if isinstance(save_path, str):
             save_path = Path(save_path)
-        jsons = json.loads(str(self).replace("'", '"'))
-        yaml.safe_dump(jsons, save_path.open('w'))
+        jsons = json.loads(str(self).replace("'", '"').replace(' None', ' null'))
+        yaml.safe_dump(
+            jsons,
+            save_path.open('w', encoding=self.__charset__),
+            allow_unicode=True
+        )
```

