# Comparing `tmp/pysqream_sqlalchemy-1.1.tar.gz` & `tmp/pysqream_sqlalchemy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqream_sqlalchemy-1.1.tar", last modified: Thu Mar 14 11:51:11 2024, max compression
+gzip compressed data, was "pysqream_sqlalchemy-1.2.tar", last modified: Thu May 30 12:27:34 2024, max compression
```

## Comparing `pysqream_sqlalchemy-1.1.tar` & `pysqream_sqlalchemy-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:51:11.479302 pysqream_sqlalchemy-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-14 11:51:11.479302 pysqream_sqlalchemy-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-03-14 11:50:59.000000 pysqream_sqlalchemy-1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:51:11.479302 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 11:50:59.000000 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27207 2024-03-14 11:50:59.000000 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-03-14 11:50:59.000000 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:51:11.479302 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-14 11:51:11.000000 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-14 11:51:11.000000 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 11:51:11.000000 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-14 11:51:11.000000 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-14 11:51:11.000000 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-14 11:51:11.000000 pysqream_sqlalchemy-1.1/pysqream_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 11:51:11.479302 pysqream_sqlalchemy-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-14 11:50:59.000000 pysqream_sqlalchemy-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:27:34.568464 pysqream_sqlalchemy-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-30 12:27:34.568464 pysqream_sqlalchemy-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-30 12:27:25.000000 pysqream_sqlalchemy-1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:27:34.568464 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:27:25.000000 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27207 2024-05-30 12:27:25.000000 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-05-30 12:27:25.000000 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:27:34.568464 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-30 12:27:34.000000 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 12:27:34.000000 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 12:27:34.000000 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 12:27:34.000000 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 12:27:34.000000 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 12:27:34.000000 pysqream_sqlalchemy-1.2/pysqream_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 12:27:34.568464 pysqream_sqlalchemy-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-30 12:27:25.000000 pysqream_sqlalchemy-1.2/setup.py
```

### Comparing `pysqream_sqlalchemy-1.1/PKG-INFO` & `pysqream_sqlalchemy-1.2/pysqream_sqlalchemy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pysqream_sqlalchemy
-Version: 1.1
+Name: pysqream-sqlalchemy
+Version: 1.2
 Summary: SQLAlchemy dialect for SQreamDB
 Home-page: https://github.com/SQream/pysqream_sqlalchemy
 Author: SQream
 Author-email: info@sqream.com
 License: UNKNOWN
 Keywords: database sqlalchemy sqream sqreamdb
 Platform: UNKNOWN
@@ -16,17 +16,18 @@
 **********************************
 SQLAlchemy Dialect for SQream DB
 **********************************
 
 Prerequisites
 ================
 
-* Python > 3.9+
-* SQLAlchemy = 2.0.27
-* SQream DB-API Connector = 3.2.5
+* SQream => 4.5.6
+* Python == 3.9
+* SQLAlchemy == 2.0.27
+* SQream DB-API Connector == 3.2.5
 * Cython (optional - improves performance)
 
 Installing SQream SQLAlchemy
 =============================
 
 .. code-block:: shell
```

### Comparing `pysqream_sqlalchemy-1.1/README.rst` & `pysqream_sqlalchemy-1.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 **********************************
 SQLAlchemy Dialect for SQream DB
 **********************************
 
 Prerequisites
 ================
 
-* Python > 3.9+
-* SQLAlchemy = 2.0.27
-* SQream DB-API Connector = 3.2.5
+* SQream => 4.5.6
+* Python == 3.9
+* SQLAlchemy == 2.0.27
+* SQream DB-API Connector == 3.2.5
 * Cython (optional - improves performance)
 
 Installing SQream SQLAlchemy
 =============================
 
 .. code-block:: shell
```

### Comparing `pysqream_sqlalchemy-1.1/pysqream_sqlalchemy/base.py` & `pysqream_sqlalchemy-1.2/pysqream_sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `pysqream_sqlalchemy-1.1/pysqream_sqlalchemy/dialect.py` & `pysqream_sqlalchemy-1.2/pysqream_sqlalchemy/dialect.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,16 +126,20 @@
         return schema_name in schemas
 
     def get_view_names(self, connection, schema=None, **kw):
         schema = connection.dialect.default_schema_name if schema is None else schema
         # 0,public.fuzz
         return [schema_view.split(".", 1)[1] for idx, schema_view in connection.execute(text("select get_views()")).fetchall() if schema_view.split(".", 1)[0] == schema]
 
-    def has_table(self, connection, table_name, schema=None, info_cache=None):
-        return table_name in self.get_table_names(connection, schema, info_cache=None)
+    def has_table(self, connection, table_name, schema=None, info_cache=None) -> bool:
+        if schema is None:
+            schema = connection.dialect.default_schema_name
+        query = text(f"select is_table_exists('{schema}','{table_name}')")
+        is_table_exists = connection.execute(query).first()
+        return is_table_exists[0]
 
     def get_columns(self, connection, table_name, schema=None, **kwargs):
         """
             Used by SQLAlchemy's Table() which is called by Superset's get_table()
             when trying to add a new table to the sources
         """
```

### Comparing `pysqream_sqlalchemy-1.1/pysqream_sqlalchemy.egg-info/PKG-INFO` & `pysqream_sqlalchemy-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pysqream-sqlalchemy
-Version: 1.1
+Name: pysqream_sqlalchemy
+Version: 1.2
 Summary: SQLAlchemy dialect for SQreamDB
 Home-page: https://github.com/SQream/pysqream_sqlalchemy
 Author: SQream
 Author-email: info@sqream.com
 License: UNKNOWN
 Keywords: database sqlalchemy sqream sqreamdb
 Platform: UNKNOWN
@@ -16,17 +16,18 @@
 **********************************
 SQLAlchemy Dialect for SQream DB
 **********************************
 
 Prerequisites
 ================
 
-* Python > 3.9+
-* SQLAlchemy = 2.0.27
-* SQream DB-API Connector = 3.2.5
+* SQream => 4.5.6
+* Python == 3.9
+* SQLAlchemy == 2.0.27
+* SQream DB-API Connector == 3.2.5
 * Cython (optional - improves performance)
 
 Installing SQream SQLAlchemy
 =============================
 
 .. code-block:: shell
```

### Comparing `pysqream_sqlalchemy-1.1/setup.py` & `pysqream_sqlalchemy-1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 from setuptools import setup
 
 
 setup_params = dict(
+    name='pysqream_sqlalchemy',
+    version='1.2',
+    description='SQLAlchemy dialect for SQreamDB',
+    long_description=open("README.rst", "r").read() + '\n\n',
+    url="https://github.com/SQream/pysqream_sqlalchemy",
     
-    name =             'pysqream_sqlalchemy',
-    version =          '1.1',
-    description =      'SQLAlchemy dialect for SQreamDB', 
-    long_description = open("README.rst", "r").read() + '\n\n',
-    url=               "https://github.com/SQream/pysqream_sqlalchemy",
+    author='SQream',
+    author_email='info@sqream.com',
     
-    author =           'SQream',
-    author_email =     'info@sqream.com',
-    
-    classifiers =      [
+    classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
-    keywords = 'database sqlalchemy sqream sqreamdb',
+    keywords='database sqlalchemy sqream sqreamdb',
 
-    python_requires =  '>=3.9',
+    python_requires='>=3.9',
     
-    install_requires = ['sqlalchemy==2.0.27',
-                        'pysqream==3.2.5',
-                        'setuptools>=57.4.0',
-                        'pandas==2.2.1',
-                        'numpy>=1.20',
-                        'alembic>=1.10.2'],
+    install_requires=['sqlalchemy==2.0.27',
+                      'pysqream==3.2.5',
+                      'setuptools>=57.4.0',
+                      'pandas==2.2.1',
+                      'numpy>=1.20',
+                      'alembic>=1.10.2'],
     
-    packages         = ['pysqream_sqlalchemy'], 
+    packages=['pysqream_sqlalchemy'],
     
-    entry_points =     {'sqlalchemy.dialects': 
-        ['sqream = pysqream_sqlalchemy.dialect:SqreamDialect']
-    },
+    entry_points={'sqlalchemy.dialects': ['sqream = pysqream_sqlalchemy.dialect:SqreamDialect']},
     # sqream://sqream:sqream@localhost/master
 )
 
 
 if __name__ == '__main__':
     setup(**setup_params)
```

