# Comparing `tmp/argendolar-2.1.1.tar.gz` & `tmp/argendolar-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argendolar-2.1.1.tar", last modified: Wed May 29 15:24:00 2024, max compression
+gzip compressed data, was "argendolar-2.2.1.tar", last modified: Wed May 29 15:46:03 2024, max compression
```

## Comparing `argendolar-2.1.1.tar` & `argendolar-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:24:00.636310 argendolar-2.1.1/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-2.1.1/LICENSE
--rw-r--r--   0 mgobea   (1218917679) 1010544492     5467 2024-05-29 15:24:00.636018 argendolar-2.1.1/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4783 2024-05-29 15:08:48.000000 argendolar-2.1.1/README.md
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:24:00.632864 argendolar-2.1.1/argendolar/
--rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-2.1.1/argendolar/__init__.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492    11171 2024-05-29 15:22:32.000000 argendolar-2.1.1/argendolar/argendolar.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-2.1.1/argendolar/tipo_dolares.py
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:24:00.635554 argendolar-2.1.1/argendolar.egg-info/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     5467 2024-05-29 15:24:00.000000 argendolar-2.1.1/argendolar.egg-info/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-29 15:24:00.000000 argendolar-2.1.1/argendolar.egg-info/SOURCES.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-29 15:24:00.000000 argendolar-2.1.1/argendolar.egg-info/dependency_links.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-29 15:24:00.000000 argendolar-2.1.1/argendolar.egg-info/requires.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-29 15:24:00.000000 argendolar-2.1.1/argendolar.egg-info/top_level.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-29 15:24:00.636382 argendolar-2.1.1/setup.cfg
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-29 15:22:49.000000 argendolar-2.1.1/setup.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:46:03.589735 argendolar-2.2.1/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-2.2.1/LICENSE
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     5467 2024-05-29 15:46:03.589494 argendolar-2.2.1/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4783 2024-05-29 15:08:48.000000 argendolar-2.2.1/README.md
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:46:03.587463 argendolar-2.2.1/argendolar/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-2.2.1/argendolar/__init__.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492    11268 2024-05-29 15:43:35.000000 argendolar-2.2.1/argendolar/argendolar.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-2.2.1/argendolar/tipo_dolares.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:46:03.589135 argendolar-2.2.1/argendolar.egg-info/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     5467 2024-05-29 15:46:03.000000 argendolar-2.2.1/argendolar.egg-info/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-29 15:46:03.000000 argendolar-2.2.1/argendolar.egg-info/SOURCES.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-29 15:46:03.000000 argendolar-2.2.1/argendolar.egg-info/dependency_links.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-29 15:46:03.000000 argendolar-2.2.1/argendolar.egg-info/requires.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-29 15:46:03.000000 argendolar-2.2.1/argendolar.egg-info/top_level.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-29 15:46:03.589789 argendolar-2.2.1/setup.cfg
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-29 15:44:54.000000 argendolar-2.2.1/setup.py
```

### Comparing `argendolar-2.1.1/LICENSE` & `argendolar-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argendolar-2.1.1/PKG-INFO` & `argendolar-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 2.1.1
+Version: 2.2.1
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `argendolar-2.1.1/README.md` & `argendolar-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `argendolar-2.1.1/argendolar/argendolar.py` & `argendolar-2.2.1/argendolar/argendolar.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,18 +283,21 @@
         """
         Get the currently daily fixed term rate for online placements of $100,000 within 30 days.
         :return: A Pandas DataFrame with the daily fixed term rate.
         """
         if not self.api_status():
             raise Exception("The API is not online.")
         else:
-            url = f"{self.base_url}/v1/tasas/plazo-fijo"
+            url = f"{self.historico_url}/v1/finanzas/tasas/plazoFijo"
+            print(url)
             response = requests.get(url)
+            print(response)
+            print(response.json())
             data = response.json()
-            df = pd.DataFrame([data])
+            df = pd.DataFrame(data)
             return df
 
     def get_tasa_promedio_plazo_fijo_historica(self) -> pd.DataFrame:
         """
         Get the historical average fixed term rate since 2000-01.
         :return: A Pandas DataFrame with the historical average fixed term rate since 2000.
         """
```

### Comparing `argendolar-2.1.1/argendolar.egg-info/PKG-INFO` & `argendolar-2.2.1/argendolar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 2.1.1
+Version: 2.2.1
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `argendolar-2.1.1/setup.py` & `argendolar-2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='argendolar',
-    version='2.1.1',
+    version='2.2.1',
     packages=find_packages(),
     install_requires=['pandas', 'requests'],
     author='Mariano Gobea Alcoba',
     author_email='gobeamariano@gmail.com',
     description='A package to get the exchange rates of the different types of dollars and others currencies in Argentina.',
     long_description=long_description,  # Usa el contenido del README.md como descripción larga
     long_description_content_type="text/markdown",  # Especifica el tipo de contenido como markdown
```

