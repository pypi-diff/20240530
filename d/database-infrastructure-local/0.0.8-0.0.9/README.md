# Comparing `tmp/database-infrastructure-local-0.0.8.tar.gz` & `tmp/database-infrastructure-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-infrastructure-local-0.0.8.tar", last modified: Thu Aug 17 10:52:49 2023, max compression
+gzip compressed data, was "database-infrastructure-local-0.0.9.tar", last modified: Thu Aug 17 11:01:57 2023, max compression
```

## Comparing `database-infrastructure-local-0.0.8.tar` & `database-infrastructure-local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 10:52:49.515431 database-infrastructure-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-17 10:52:49.515431 database-infrastructure-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-17 10:52:19.000000 database-infrastructure-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 10:52:49.515431 database-infrastructure-local-0.0.8/circles_number_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-17 10:52:19.000000 database-infrastructure-local-0.0.8/circles_number_generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 10:52:49.515431 database-infrastructure-local-0.0.8/circles_number_generator/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-17 10:52:19.000000 database-infrastructure-local-0.0.8/circles_number_generator/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-08-17 10:52:19.000000 database-infrastructure-local-0.0.8/circles_number_generator/src/number_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 10:52:49.515431 database-infrastructure-local-0.0.8/database_infrastructure_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-17 10:52:49.000000 database-infrastructure-local-0.0.8/database_infrastructure_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-17 10:52:49.000000 database-infrastructure-local-0.0.8/database_infrastructure_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 10:52:49.000000 database-infrastructure-local-0.0.8/database_infrastructure_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-17 10:52:49.000000 database-infrastructure-local-0.0.8/database_infrastructure_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-17 10:52:19.000000 database-infrastructure-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-17 10:52:49.515431 database-infrastructure-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-17 10:52:19.000000 database-infrastructure-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 11:01:57.920092 database-infrastructure-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-17 11:01:57.920092 database-infrastructure-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-17 11:01:28.000000 database-infrastructure-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 11:01:57.920092 database-infrastructure-local-0.0.9/circles_number_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-17 11:01:28.000000 database-infrastructure-local-0.0.9/circles_number_generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 11:01:57.920092 database-infrastructure-local-0.0.9/circles_number_generator/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-17 11:01:28.000000 database-infrastructure-local-0.0.9/circles_number_generator/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-17 11:01:28.000000 database-infrastructure-local-0.0.9/circles_number_generator/src/number_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 11:01:57.920092 database-infrastructure-local-0.0.9/database_infrastructure_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-17 11:01:57.000000 database-infrastructure-local-0.0.9/database_infrastructure_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-17 11:01:57.000000 database-infrastructure-local-0.0.9/database_infrastructure_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 11:01:57.000000 database-infrastructure-local-0.0.9/database_infrastructure_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-17 11:01:57.000000 database-infrastructure-local-0.0.9/database_infrastructure_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-17 11:01:28.000000 database-infrastructure-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-17 11:01:57.920092 database-infrastructure-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-17 11:01:28.000000 database-infrastructure-local-0.0.9/setup.py
```

### Comparing `database-infrastructure-local-0.0.8/README.md` & `database-infrastructure-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `database-infrastructure-local-0.0.8/circles_number_generator/src/number_generator.py` & `database-infrastructure-local-0.0.9/circles_number_generator/src/number_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,16 +54,17 @@
         cursor = connection.cursor()
 
         successful = False
 
         while not successful:
             number = random.randint(1, sys.maxsize)
             logger.info(object = {"Random number generated": str(number)})
-
-            cursor.execute("SELECT %s FROM %s.%s WHERE `%s` = %s" % (self.id_column_name, self.number_column_name, self.schema, self.table, number))
+            
+            query_get = "SELECT %s FROM %s.%s WHERE `%s` = %s"
+            cursor.execute(query_get, (self.id_column_name, self.schema, self.table, self.number_column_name, number))
             if cursor.fetchone() == None:
                 successful = True
                 logger.info("Number does not already exist in database")
 
         connection.close()
         logger.end(GET_RANDOM_NUMBER_METHOD_NAME, object = {"number" : number})
         return number
```

### Comparing `database-infrastructure-local-0.0.8/pyproject.toml` & `database-infrastructure-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database-infrastructure-local-0.0.8/setup.py` & `database-infrastructure-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      name='database-infrastructure-local',  
-     version='0.0.8',
+     version='0.0.9',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Database Infrastructure Local Python",
      long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/circles",
      packages=setuptools.find_packages(),
```

