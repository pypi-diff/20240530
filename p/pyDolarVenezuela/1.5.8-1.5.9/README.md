# Comparing `tmp/pydolarvenezuela-1.5.8.tar.gz` & `tmp/pydolarvenezuela-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.5.8.tar", last modified: Mon May 20 18:40:53 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.5.9.tar", last modified: Thu May 30 05:02:13 2024, max compression
```

## Comparing `pydolarvenezuela-1.5.8.tar` & `pydolarvenezuela-1.5.9.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 18:40:53.067018 pydolarvenezuela-1.5.8/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.8/LICENSE
--rw-rw-rw-   0        0        0     7221 2024-05-20 18:40:53.050974 pydolarvenezuela-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     4830 2024-05-08 05:23:24.000000 pydolarvenezuela-1.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 18:40:52.765226 pydolarvenezuela-1.5.8/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2879 2024-05-20 18:40:00.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 18:40:52.823647 pydolarvenezuela-1.5.8/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-05-20 18:40:52.881963 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/images.py
--rw-rw-rw-   0        0        0      773 2024-05-20 18:37:09.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/monitor.py
--rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      740 2024-04-28 16:11:30.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-05-20 18:40:52.986001 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     5651 2024-05-20 18:32:08.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2328 2024-05-19 06:17:16.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2081 2024-05-19 06:50:07.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     2627 2024-05-19 05:56:01.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     1282 2024-05-04 08:02:51.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/italcambio.py
-drwxrwxrwx   0        0        0        0 2024-05-20 18:40:53.050974 pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0    12380 2024-05-19 06:16:03.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 18:40:53.050974 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     7221 2024-05-20 18:40:52.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      888 2024-05-20 18:40:52.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 18:40:52.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-20 18:40:52.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-20 18:40:52.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-05-20 18:40:16.000000 pydolarvenezuela-1.5.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 18:40:53.067018 pydolarvenezuela-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-05-20 18:40:10.000000 pydolarvenezuela-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.510912 pydolarvenezuela-1.5.9/
+-rw-rw-rw-   0        0        0    11547 2024-05-26 02:00:20.000000 pydolarvenezuela-1.5.9/LICENSE
+-rw-rw-rw-   0        0        0    19253 2024-05-30 05:02:13.501910 pydolarvenezuela-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4969 2024-05-30 04:08:53.000000 pydolarvenezuela-1.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.210913 pydolarvenezuela-1.5.9/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2794 2024-05-30 04:57:27.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.290931 pydolarvenezuela-1.5.9/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.331912 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/images.py
+-rw-rw-rw-   0        0        0      770 2024-05-30 04:34:11.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/monitor.py
+-rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      605 2024-05-30 03:42:26.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      860 2024-05-30 03:24:32.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.365912 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     5826 2024-05-30 04:51:43.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2689 2024-05-30 04:30:30.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/alcambio.py
+-rw-rw-rw-   0        0        0     2335 2024-05-25 22:27:08.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2088 2024-05-25 17:55:45.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     2648 2024-05-30 03:43:00.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     1289 2024-05-25 17:56:00.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/italcambio.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.464912 pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/calculator.py
+-rw-rw-rw-   0        0        0    12770 2024-05-30 04:23:51.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/extras.py
+-rw-rw-rw-   0        0        0     2457 2024-05-30 03:31:36.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/time.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:02:13.468912 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0    19253 2024-05-30 05:02:12.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2024-05-30 05:02:13.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 05:02:12.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-30 05:02:12.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-30 05:02:12.000000 pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-05-30 04:57:35.000000 pydolarvenezuela-1.5.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 05:02:13.510912 pydolarvenezuela-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-05-30 04:57:41.000000 pydolarvenezuela-1.5.9/setup.py
```

### Comparing `pydolarvenezuela-1.5.8/README.md` & `pydolarvenezuela-1.5.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,36 +4,37 @@
 
 | Página Web | URL | Estado
 |------------|-------------|-------------|
 | Exchange Monitor | https://exchangemonitor.net/dolar-venezuela | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | CriptoDolar | https://criptodolar.net/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | BCV (Banco Central de Venezuela) | http://www.bcv.org.ve/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | Italcambio | https://www.italcambio.com/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
+| AlCambio | https://alcambio.app/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 
 pyDolarVenezuela tiene como objetivo principal brindar una solución eficiente y confiable para acceder a información relevante sobre el valor del dólar en Venezuela, ofreciendo así una herramienta valiosa para desarrolladores interesados en trabajar en este ámbito.
 
 ## Instalación
 ``` sh
 pip install pyDolarVenezuela
 ```
 
 ## Uso
 Debes importar el módulo `pages`, donde encontrarás una variedad de atributos que contienen información sobre una página específica de la que deseas obtener los datos. Adicionalmente deberás importar la clase `Monitor`, cuyos parámetros será la página que deseas utilizar y la moneda en la que se expresarán los precios (`USD`, `EUR`).
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
+from pyDolarVenezuela.pages import AlCambio, BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 ```
 
 pyDolarVenezuela utiliza [Redis](https://github.com/redis/redis-py), un motor de base de datos en memoria, para almacenar y procesar datos. Esto nos ayuda para calcular el cambio, el porcentaje, el color y el símbolo, y se devuelven los datos actualizados.
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
+from pyDolarVenezuela.pages import AlCambio, BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor, Redis
 
 # Defecto
 db = Redis(
     host='localhost',
     port=6379
 )
@@ -67,15 +68,15 @@
 El método `get_value_monitors` se utiliza después de crear una instancia del objeto Monitor y permite el acceso a los datos almacenados en el diccionario. Los siguientes parámetros serían los siguientes:
 
 - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
 - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
 - `prettify`: Muestra los precios en formato de moneda con el símbolo de Bolívares. Por defecto es `False`.
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
+from pyDolarVenezuela.pages import AlCambio, BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 
 # Obtener los valores de todos los monitores
 valores_dolar = monitor.get_value_monitors()
 
@@ -84,15 +85,15 @@
 
 print(valor_dolar)
 ```
 
 La función `currency_converter` convierte una cantidad de dinero de una moneda a otra utilizando los datos de un monitor específico.
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
+from pyDolarVenezuela.pages import AlCambio, BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 from pyDolarVenezuela import currency_converter
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 
 information_dolar = monitor.get_value_monitors("enparalelovzla")
 price_in_dolares = currency_converter(
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 from typing import Literal
 from colorama import Fore
 
 from . import network
 from .models.pages import Page
 from .data.redis import Redis
-from .tools import get_time_zone as getdate, currency_converter
-from .provider import select_monitor
+from .utils import get_time_zone as getdate, currency_converter
+from .provider import Provider
 
-version = '1.5.8'
+version = '1.5.9'
 """
 Versión actual de la biblioteca    
 """
 
 class CheckVersion:
     """
     Verificar actualización de la biblioteca    
@@ -34,42 +34,37 @@
     def __init__(self, provider: Page, currency: Literal['USD', 'EUR'] = 'USD', db: Redis = None) -> None:
         """
         La clase `Monitor` proporciona funcionalidades para consultar los precios de diversos monitores en Venezuela.
 
         Parámetros:
         - `provider`: La página de la que se accederán los datos.
         - `currency`: La moneda en la que se expresarán los precios. Puede ser `USD` o `EUR`. Por defecto es `USD`.
+        - `db`: Base de datos con Redis. 
         """
 
         if CheckVersion.check:
             CheckVersion._check_dependence_version()
         if not isinstance(provider, Page):
             raise TypeError("The parameter must be an object of type Monitor.")
         
         self.provider = provider
         self.currency = currency.lower()
         self.db       = db
+        self.select_monitor = Provider(provider, currency, db)
     
     def get_all_monitors(self):
-        return select_monitor(
-            self.provider,
-            db=self.db,
-            currency=self.currency
-        )
+        return self.select_monitor._get_values_specifics()
 
-    def get_value_monitors(self, monitor_code: str = None, name_property: Literal['title', 'price', 'last_update'] = None, prettify: bool = False):
+    def get_value_monitors(self, type_monitor: str = None, property: Literal['title', 'price', 'last_update'] = None, prettify: bool = False):
         """
         El método `get_value_monitors` permite acceder a los datos extraídos de los monitores.
 
         Parámetros:
-        - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
-        - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
+        - `type_monitor`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
+        - `property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
         - `prettify`: Si es True, muestra los precios en formato de moneda con el símbolo de Bolívares. Por defecto es `False`.
         """ 
-        return select_monitor(
-            self.provider,
-            db=self.db,
-            currency=self.currency,
-            monitor_code=monitor_code,
-            name_property=name_property,
-            prettify=prettify
+        return self.select_monitor._get_values_specifics(
+            type_monitor,
+            property,
+            prettify
         )
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/models/monitor.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/models/monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional
 from dataclasses import dataclass
 
 @dataclass
-class MonitorDB:
+class Monitor:
     """
     MonitorDB instance
     """
     title: str  
     price: float  
     price_old: Optional[float] = None 
     last_update: Optional[str] = None  
-    percent: Optional[float] = None 
-    change: Optional[float] = None  
-    color: Optional[str] = None  
-    symbol: Optional[str] = None 
     image: Optional[str] = None  
+    percent: Optional[float] = 0.0
+    change: Optional[float] = 0.0  
+    color: Optional[str] = "neutral" 
+    symbol: Optional[str] = "" 
 
     def __str__(self):
         return f"{self.__class__.__name__}(title={self.title}, price={self.price}, price_old={self.price_old}, last_update={self.last_update}, percent={self.percent}, change={self.change}, color={self.color}, symbol={self.symbol}, image={self.image})"
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/pages.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,8 +18,14 @@
     currencies=['usd', 'eur']
 )
 
 Italcambio = Page(
     name="Italcambio",
     provider="https://www.italcambio.com/index.php",
     currencies=['usd', 'dkk', 'cop', 'nok', 'gbp', 'sek', 'clp', 'chf', 'hkd', 'twd', 'brl', 'cad', 'eur', 'bob', 'nio', 'ars', 'cny', 'ils', 'jpy', 'pen', 'dop', 'ttd', 'uyu', 'ang', 'aud']
+)
+
+AlCambio = Page(
+    name="Al Cambio",
+    provider="https://api.alcambio.app/graphql",
+    currencies=['usd']
 )
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,145 +1,139 @@
 import json
 from typing import Any
 from dataclasses import asdict
+from .alcambio import AlCambio
 from .bcv import BCV
 from .criptodolar import CriptoDolar
 from .exchangemonitor import ExchangeMonitor
 from .italcambio import Italcambio
 
 from ..data.redis import Cache
-from ..models.monitor import MonitorDB
+from ..models.monitor import Monitor
 from ..models.database import Redis
 from ..models.pages import Page
-from ..pages import BCV as B, CriptoDolar as C, ExchangeMonitor as E, Italcambio as I
-from ..utils import currencies_list
+from ..pages import AlCambio as A, BCV as B, CriptoDolar as C, ExchangeMonitor as E, Italcambio as I
 
-monitor_classes = [
-    {
-        B.name: {
-            'currency': B.currencies,
-            'provider': BCV
-        }
-    },
-    {
-        C.name: {
-            'currency': C.currencies,
-            'provider': CriptoDolar
-        }
-    },
-    {
-        E.name: {
-            'currency': E.currencies,
-            'provider': ExchangeMonitor
-        }
-    },
-    {
-        I.name: {
-            'currency': I.currencies,
-            'provider': Italcambio
-        }
-    }
-]
-
-def select_monitor(provider: Page, db: Redis, **kwargs):
-    global data
-        
-    currency = kwargs.get('currency', None)
-    monitor_code = kwargs.get('monitor_code', None)
-    name_property = kwargs.get('name_property', None)
-    prettify = kwargs.get('prettify', False)
-
-    if currency not in currencies_list:
-        raise ValueError(f"The currency type must be 'usd', 'eur'..., not {currency}")
-
-    def _get_values_specifics():
-        if not monitor_code:
-            return data
+monitor_classes = {
+    A.name: {'currency': A.currencies, 'provider': AlCambio},
+    B.name: {'currency': B.currencies, 'provider': BCV},
+    C.name: {'currency': C.currencies, 'provider': CriptoDolar},
+    E.name: {'currency': E.currencies, 'provider': ExchangeMonitor},
+    I.name: {'currency': I.currencies, 'provider': Italcambio},
+}
+
+class Provider:
+    def __init__(self,
+                page: Page, 
+                currency: str, 
+                db: Redis = None) -> None:
+        if currency.lower() not in page.currencies:
+            raise ValueError(f"The currency type must be 'usd', 'eur'..., not {currency}")
         
-        try:
-            monitor_data = data[monitor_code.lower()]
-            if name_property:
-                if name_property == 'last_update' and provider.name == B.name:
-                    return data[name_property]
-                value = monitor_data[name_property]
-                return f'Bs. {value}' if prettify and name_property == 'price' else value
-            return monitor_data
-        except KeyError:
-            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
-
-    def _update_item(existing_data_dict: dict, i: Any, last_data: dict):
-        structure_monitor = asdict(MonitorDB(**existing_data_dict[i]))
-        for key in list(existing_data_dict[i].keys()):
+        self.page = page
+        self.currency = currency.lower()
+        self.db = db
+
+        if self.db is not None:
+            self._redis = Cache(self.db)
+
+    def _load_data(self):
+        monitor_class = monitor_classes.get(self.page.name).get('provider')
+        values = monitor_class(url=self.page.provider, currency=self.currency).get_values()
+
+        if self.db is not None:
+            key = f'{self.currency}:{self.page.name}'
+            if not self._redis.get_data(key):
+                self._redis.set_data(key, json.dumps(values), self.db.ttl)
+
+            old_data = json.loads(self._redis.get_data(key))
+            for property in old_data:
+                if property not in ('banks', 'last_update'):
+                    try:
+                        self._update_item(old_data, values, property)
+                    except KeyError:
+                        pass
+                elif property == 'banks': # Comparación de propiedades de los datos BCV
+                    banks = values[property]
+                    for i, bank in enumerate(old_data[property]):
+                        if i < len(banks) and bank['title'] == banks[i]['title']:
+                            self._update_item(old_data[property], banks, i)
+                elif property == 'last_update':
+                    old_data[property] = values[property]
+
+            self._redis.set_data(key, json.dumps(old_data), self.db.ttl)
+            values = json.loads(self._redis.get_data(key))
+            
+        return values 
+    
+    def _update_item(self, old_data: dict, new_data: dict, i: Any):
+        """
+        Evalúa la estructura de cada monitor en `old_data`. Elimina los atributos que sean `None` (Cada estructura es diferente según el proveedor) y realiza los cálculos necesarios.
+
+        Estructura inicial (para la primera vez):
+        ```python
+        class Monitor:
+            title: str  
+            price: float  
+            price_old: Optional[float] = None 
+            last_update: Optional[str] = None  
+            image: Optional[str] = None  
+            percent: Optional[float] = 0.0
+            change: Optional[float] = 0.0  
+            color: Optional[str] = "neutral" 
+            symbol: Optional[str] = "" 
+        ```
+        """
+        structure_monitor = asdict(Monitor(**old_data[i]))
+        for key in list(old_data[i].keys()):
             if structure_monitor[key] is None:
-                del existing_data_dict[i][key]
+                del old_data[i][key]
         
-        if existing_data_dict[i]['price'] != last_data[i]['price']:
-            price = existing_data_dict[i]['price']
-            new_price = last_data[i]['price']
-            price_old = last_data[i].get('price_old', None)
-            change  = round(float(new_price - price), 2)
-            percent = float(f'{round(float((change / new_price) * 100 if price != 0 else 0), 2)}'.replace('-', ' '))
-            symbol  = "" if change == 0 else "▲" if change >= 0 else "▼"
-            color   = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
-            last_update = last_data[i].get('last_update', None)
+        if old_data[i]['price'] != new_data[i]['price']:
+            old_price = old_data[i]['price']
+            new_price = new_data[i]['price']
+            price_old = new_data[i].get('price_old', None) # Valor preciso
+            change    = round(float(new_price - old_price), 2)
+            percent   = float(f'{round(float((change / new_price) * 100 if old_price != 0 else 0), 2)}'.replace('-', ' '))
+            symbol    = "" if change == 0 else "▲" if change >= 0 else "▼"
+            color     = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
+            last_update = new_data[i].get('last_update', None)
+
             change = float(str(change).replace('-', ' '))
 
-            existing_data_dict[i].update({
-                    'price': new_price,
-                    'change': change,
-                    'percent': percent,
-                    'color': color,
-                    'symbol': symbol,
+            old_data[i].update({
+                'price': new_price,
+                'change': change,
+                'percent': percent,
+                'color': color,
+                'symbol': symbol,
             })
-    
-            if last_update and price_old is not None:
-                existing_data_dict[i].update({
+            
+            # Comprueba si los atributos tienen valor. se agregan y/o actualizan
+            if last_update and price_old:
+                old_data[i].update({
                     'price_old': price_old,
                     'last_update': last_update
                 })
-            elif last_update is not None:
-                existing_data_dict[i].update({
+                
+            elif last_update: 
+                old_data[i].update({
                     'last_update': last_update
                 })
 
-    try:
-        monitor_class = None
-
-        for monitor in monitor_classes:
-            if monitor.get(provider.name) and currency in monitor.get(provider.name)['currency']:
-                monitor_class = monitor[provider.name]['provider']
-
-        if monitor_class is not None:
-            data = monitor_class(url=provider.provider, currency=currency).get_values()
-            if db is not None:
-                key = f'{currency}:{provider.name}'
-                cache = Cache(db)
-                
-                existing_data = cache.get_data(key)
-
-                if not existing_data:
-                    cache.set_data(key, json.dumps(data), db.ttl)
-
-                existing_data_dict = json.loads(cache.get_data(key))
-                for name in existing_data_dict:
-                    if not name == 'last_update' and not name == 'banks':
-                        if name in existing_data_dict and name in data:
-                            _update_item(existing_data_dict, name, data)
-                    else:
-                        if name == 'banks':
-                            for i, bank in enumerate(existing_data_dict[name]):
-                                if i < len(data[name]) and bank['title'] == data[name][i]['title']:
-                                    _update_item(existing_data_dict[name], i, data[name])
-                        elif name == 'last_update':
-                            existing_data_dict[name] = data[name]
-                            
-                cache.set_data(key, json.dumps(existing_data_dict), db.ttl)
-                data = json.loads(
-                    cache.get_data(key)
-                )
-
-                return _get_values_specifics()
-            return _get_values_specifics()
-        else:
-            raise ValueError("Provider not supported")
-    except Exception as e:
-        raise e
+    def _get_values_specifics(self, type_monitor: str = None, property: str = None, prettify: bool = False):
+        data = self._load_data()
+        if not type_monitor:
+            return data
+        
+        try:
+            monitor_data = data[type_monitor.lower()]
+            if property:
+                if property == 'last_update' and self.page.name == B.name:
+                    return monitor_data[property]
+                value = monitor_data[property]
+                return f'Bs. {value}' if prettify and property == 'price' else value
+            return monitor_data
+        except KeyError:
+            raise KeyError('Property not found. https://github.com/fcoagz/pyDolarVenezuela')
+        except Exception as e:
+            raise e
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/bcv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bs4 import BeautifulSoup
 
 from ..network import requests, get
-from ..utils import currencies, list_monitors_images
+from ..utils.extras import currencies, list_monitors_images
 
 requests.packages.urllib3.disable_warnings()
 
 def _get_rate_by_id(tag_id: str, soup: BeautifulSoup):
     return float(soup.find(id=tag_id).find("strong").text.strip().replace(',', '.'))
 
 def _get_time(soup: BeautifulSoup):
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/criptodolar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from .. import network
-from ..tools import time
-from ..utils import list_monitors_images
+from ..utils import time
+from ..utils.extras import list_monitors_images
 
 def _convert_specific_format(text: str, character: str = '_') -> str:
     acentos = {'á': 'a', 'é': 'e', 'í': 'i', 'ó': 'o', 'ú': 'u'}
     for acento, sin_acento in acentos.items():
         text = text.lower().replace(acento, sin_acento).replace(' ', character)
     return text
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from bs4 import BeautifulSoup
 from .. import network
-from ..tools import time
-from ..utils import list_monitors_images
+from ..utils import time
+from ..utils.extras import list_monitors_images
 
 def _convert_specific_format(text: str, character: str = '_') -> str:
     acentos = {'á': 'a', 'é': 'e', 'í': 'i', 'ó': 'o', 'ú': 'u'}
     for acento, sin_acento in acentos.items():
         text = text.lower().replace(acento, sin_acento).replace(' ', character)
     return text
 
 def _get_values_monitors(soup: BeautifulSoup):
     return [value for value in soup]
 
 class ExchangeMonitor:
     def __init__(self, url: str, currency: str, **kwargs) -> None:
-        response = (network.curl(url + "dolar-venezuela") if currency == 'usd'
-                    else network.curl(url + "dolar-venezuela/EUR"))
+        response = (network.curl('GET', url + "dolar-venezuela") if currency == 'usd'
+                    else network.curl('GET', url + "dolar-venezuela/EUR"))
         self.soup = BeautifulSoup(response, "html.parser")
     
     def _load(self):
         section_dolar_venezuela = self.soup.find_all("div", "col-xs-12 col-sm-6 col-md-4 col-tabla")
         _scraping_monitors = _get_values_monitors(section_dolar_venezuela)
 
         self.data = {}
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/italcambio.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/provider/italcambio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from bs4 import BeautifulSoup
 from ..network import get
-from ..tools.time import standard_time_zone
-from ..utils import code_currencies
+from ..utils.time import standard_time_zone
+from ..utils.extras import code_currencies
 
 class Italcambio:
     def __init__(self, url: str, **kwargs) -> None:
         response = get(url)
         self.soup = BeautifulSoup(response, 'html.parser')
 
     def _load(self):
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/time.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from babel.dates import format_date, format_time
 from datetime import datetime, timedelta
 from pytz import timezone
 
-from pyDolarVenezuela.utils import time_units
+from .extras import time_units
 
 standard_time_zone = timezone('America/Caracas')
 
+def get_formatted_timestamp(date_timestamp_ms: int):
+    """
+    Formatear milisegundos a datetime string.
+    """
+    timestamp_s = date_timestamp_ms / 1000.0
+    datetime_obj = datetime.fromtimestamp(timestamp_s)
+    
+    return datetime_obj.strftime('%d/%m/%Y, %I:%M %p')
+
 def get_time(date_string: str):
     """
     Formatear datetime a string.
     """
     datetime_obj = datetime.strptime(date_string, '%Y-%m-%d %H:%M')
     
     return datetime_obj.strftime('%d/%m/%Y, %I:%M %p')
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela/utils.py` & `pydolarvenezuela-1.5.9/pyDolarVenezuela/utils/extras.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .models.images import Image
+from ..models.images import Image
 
 currencies = {
     "eur": {"name": "Euro", "id": "euro"},
     "cny": {"name": "Yuan chino", "id": "yuan"},
     "try": {"name": "Lira turca", "id": "lira"},
     "rub": {"name": "Rublo ruso", "id": "rublo"},
     "usd": {"name": "Dólar estadounidense", "id": "dolar"}
@@ -57,14 +57,24 @@
     "horas": "hours", "hora": "hours",
     "minutos": "minutes", "minuto": "minutes",
     "segundos": "seconds", "segundo": "seconds"
 }
 
 path_images = [
     {
+        "title": "bcv",
+        "image": "https://res.cloudinary.com/dcpyfqx87/image/upload/v1717042862/alcambio/pff3ahlx2ilvcf48ijne.png",
+        "provider": "alcambio"
+    },
+    {
+        "title": "enparalelovzla",
+        "image": "https://res.cloudinary.com/dcpyfqx87/image/upload/v1717042885/alcambio/pzlgnhggdwgkzzg3ndfs.png",
+        "provider": "alcambio"
+    },
+    {
         "title": "usd",
         "image": "https://res.cloudinary.com/dcpyfqx87/image/upload/v1716093823/bcv/uppdtt4fzbhnwq5cu9br.png",
         "provider": "bcv"
     },
     {
         "title": "try",
         "image": "https://res.cloudinary.com/dcpyfqx87/image/upload/v1716099345/bcv/zowkdfsqlmiafsksgdwb.png",
```

### Comparing `pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.5.9/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 pyDolarVenezuela/__init__.py
 pyDolarVenezuela/network.py
 pyDolarVenezuela/pages.py
-pyDolarVenezuela/utils.py
 pyDolarVenezuela.egg-info/PKG-INFO
 pyDolarVenezuela.egg-info/SOURCES.txt
 pyDolarVenezuela.egg-info/dependency_links.txt
 pyDolarVenezuela.egg-info/requires.txt
 pyDolarVenezuela.egg-info/top_level.txt
 pyDolarVenezuela/data/__init__.py
 pyDolarVenezuela/data/redis.py
 pyDolarVenezuela/models/__init__.py
 pyDolarVenezuela/models/database.py
 pyDolarVenezuela/models/images.py
 pyDolarVenezuela/models/monitor.py
 pyDolarVenezuela/models/pages.py
 pyDolarVenezuela/provider/__init__.py
+pyDolarVenezuela/provider/alcambio.py
 pyDolarVenezuela/provider/bcv.py
 pyDolarVenezuela/provider/criptodolar.py
 pyDolarVenezuela/provider/exchangemonitor.py
 pyDolarVenezuela/provider/italcambio.py
-pyDolarVenezuela/tools/__init__.py
-pyDolarVenezuela/tools/calculator.py
-pyDolarVenezuela/tools/time.py
+pyDolarVenezuela/utils/__init__.py
+pyDolarVenezuela/utils/calculator.py
+pyDolarVenezuela/utils/extras.py
+pyDolarVenezuela/utils/time.py
```

### Comparing `pydolarvenezuela-1.5.8/pyproject.toml` & `pydolarvenezuela-1.5.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.5.8"
+version = "1.5.9"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.5.8/setup.py` & `pydolarvenezuela-1.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.5.8'
+VERSION = '1.5.9'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

