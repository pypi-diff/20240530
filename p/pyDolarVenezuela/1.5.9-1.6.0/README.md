# Comparing `tmp/pydolarvenezuela-1.5.9.tar.gz` & `tmp/pydolarvenezuela-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.5.9.tar", last modified: Thu May 30 05:02:13 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.6.0.tar", last modified: Thu May 30 07:37:12 2024, max compression
```

## Comparing `pydolarvenezuela-1.5.9.tar` & `pydolarvenezuela-1.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.510912 pydolarvenezuela-1.5.9/
--rw-rw-rw-   0        0        0    11547 2024-05-26 02:00:20.000000 pydolarvenezuela-1.5.9/LICENSE
--rw-rw-rw-   0        0        0    19253 2024-05-30 05:02:13.501910 pydolarvenezuela-1.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2024-05-30 04:08:53.000000 pydolarvenezuela-1.5.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.210913 pydolarvenezuela-1.5.9/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2794 2024-05-30 04:57:27.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.290931 pydolarvenezuela-1.5.9/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.331912 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/images.py
--rw-rw-rw-   0        0        0      770 2024-05-30 04:34:11.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/monitor.py
--rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      605 2024-05-30 03:42:26.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      860 2024-05-30 03:24:32.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.365912 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     5826 2024-05-30 04:51:43.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2689 2024-05-30 04:30:30.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/alcambio.py
--rw-rw-rw-   0        0        0     2335 2024-05-25 22:27:08.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2088 2024-05-25 17:55:45.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     2648 2024-05-30 03:43:00.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     1289 2024-05-25 17:56:00.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/italcambio.py
-drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.464912 pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/calculator.py
--rw-rw-rw-   0        0        0    12770 2024-05-30 04:23:51.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/extras.py
--rw-rw-rw-   0        0        0     2457 2024-05-30 03:31:36.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/time.py
-drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.468912 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0    19253 2024-05-30 05:02:12.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      933 2024-05-30 05:02:13.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 05:02:12.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-30 05:02:12.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-30 05:02:12.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-05-30 04:57:35.000000 pydolarvenezuela-1.5.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 05:02:13.510912 pydolarvenezuela-1.5.9/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-05-30 04:57:41.000000 pydolarvenezuela-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:37:12.610080 pydolarvenezuela-1.6.0/
+-rw-rw-rw-   0        0        0    11547 2024-05-26 02:00:20.000000 pydolarvenezuela-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0    19253 2024-05-30 07:37:12.602072 pydolarvenezuela-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4969 2024-05-30 04:08:53.000000 pydolarvenezuela-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 07:37:11.970110 pydolarvenezuela-1.6.0/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2794 2024-05-30 07:34:20.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:37:12.214100 pydolarvenezuela-1.6.0/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:37:12.258094 pydolarvenezuela-1.6.0/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/models/images.py
+-rw-rw-rw-   0        0        0      770 2024-05-30 04:34:11.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/models/monitor.py
+-rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      605 2024-05-30 03:42:26.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      860 2024-05-30 03:24:32.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:37:12.435082 pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     5921 2024-05-30 07:30:50.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2689 2024-05-30 04:30:30.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/alcambio.py
+-rw-rw-rw-   0        0        0     2335 2024-05-25 22:27:08.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2088 2024-05-25 17:55:45.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     2648 2024-05-30 03:43:00.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     1289 2024-05-25 17:56:00.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/italcambio.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:37:12.585074 pydolarvenezuela-1.6.0/pyDolarVenezuela/utils/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/utils/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/utils/calculator.py
+-rw-rw-rw-   0        0        0    12770 2024-05-30 04:23:51.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/utils/extras.py
+-rw-rw-rw-   0        0        0     2457 2024-05-30 03:31:36.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela/utils/time.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:37:12.598074 pydolarvenezuela-1.6.0/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0    19253 2024-05-30 07:37:11.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2024-05-30 07:37:11.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:37:11.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-30 07:37:11.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-30 07:37:11.000000 pydolarvenezuela-1.6.0/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-05-30 07:34:31.000000 pydolarvenezuela-1.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:37:12.610080 pydolarvenezuela-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-05-30 07:35:58.000000 pydolarvenezuela-1.6.0/setup.py
```

### Comparing `pydolarvenezuela-1.5.9/LICENSE` & `pydolarvenezuela-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/PKG-INFO` & `pydolarvenezuela-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.9
+Version: 1.6.0
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pydolarvenezuela-1.5.9/README.md` & `pydolarvenezuela-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from . import network
 from .models.pages import Page
 from .data.redis import Redis
 from .utils import get_time_zone as getdate, currency_converter
 from .provider import Provider
 
-version = '1.5.9'
+version = '1.6.0'
 """
 Versión actual de la biblioteca    
 """
 
 class CheckVersion:
     """
     Verificar actualización de la biblioteca
```

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/models/monitor.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/models/monitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/network.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/network.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
     def _load_data(self):
         monitor_class = monitor_classes.get(self.page.name).get('provider')
         values = monitor_class(url=self.page.provider, currency=self.currency).get_values()
 
         if self.db is not None:
             key = f'{self.currency}:{self.page.name}'
+            self._redis.delete_data(key)
             if not self._redis.get_data(key):
                 self._redis.set_data(key, json.dumps(values), self.db.ttl)
 
             old_data = json.loads(self._redis.get_data(key))
             for property in old_data:
                 if property not in ('banks', 'last_update'):
                     try:
@@ -80,17 +81,18 @@
             percent: Optional[float] = 0.0
             change: Optional[float] = 0.0  
             color: Optional[str] = "neutral" 
             symbol: Optional[str] = "" 
         ```
         """
         structure_monitor = asdict(Monitor(**old_data[i]))
-        for key in list(old_data[i].keys()):
+        for key in list(structure_monitor.keys()):
             if structure_monitor[key] is None:
-                del old_data[i][key]
+                del structure_monitor[key]
+        old_data[i] = structure_monitor
         
         if old_data[i]['price'] != new_data[i]['price']:
             old_price = old_data[i]['price']
             new_price = new_data[i]['price']
             price_old = new_data[i].get('price_old', None) # Valor preciso
             change    = round(float(new_price - old_price), 2)
             percent   = float(f'{round(float((change / new_price) * 100 if old_price != 0 else 0), 2)}'.replace('-', ' '))
```

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/alcambio.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/alcambio.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/criptodolar.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/italcambio.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/provider/italcambio.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/calculator.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/utils/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/extras.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/utils/extras.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/time.py` & `pydolarvenezuela-1.6.0/pyDolarVenezuela/utils/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.6.0/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.9
+Version: 1.6.0
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.6.0/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.9/pyproject.toml` & `pydolarvenezuela-1.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.5.9"
+version = "1.6.0"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.5.9/setup.py` & `pydolarvenezuela-1.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.5.9'
+VERSION = '1.6.0'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

