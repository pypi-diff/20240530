# Comparing `tmp/easypedidoapi-0.0.8.tar.gz` & `tmp/easypedidoapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easypedidoapi-0.0.8.tar", last modified: Wed Mar  8 00:07:28 2023, max compression
+gzip compressed data, was "dist/easypedidoapi-0.0.9.tar", last modified: Thu May 30 06:17:04 2024, max compression
```

## Comparing `easypedidoapi-0.0.8.tar` & `easypedidoapi-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ampamo     (501) staff       (20)        0 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/
--rw-r--r--   0 ampamo     (501) staff       (20)      275 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/PKG-INFO
--rw-r--r--   0 ampamo     (501) staff       (20)      724 2023-03-07 23:50:06.000000 easypedidoapi-0.0.8/setup.py
-drwxr-xr-x   0 ampamo     (501) staff       (20)        0 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/easypedidoapi/
--rw-r--r--   0 ampamo     (501) staff       (20)       48 2023-03-01 19:02:00.000000 easypedidoapi-0.0.8/easypedidoapi/__init__.py
--rw-r--r--   0 ampamo     (501) staff       (20)     2778 2023-03-07 23:51:04.000000 easypedidoapi-0.0.8/easypedidoapi/base.py
-drwxr-xr-x   0 ampamo     (501) staff       (20)        0 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/easypedidoapi/interfaces/
--rw-r--r--   0 ampamo     (501) staff       (20)       36 2023-03-02 20:53:42.000000 easypedidoapi-0.0.8/easypedidoapi/interfaces/__init__.py
--rw-r--r--   0 ampamo     (501) staff       (20)     8084 2023-03-07 23:51:04.000000 easypedidoapi-0.0.8/easypedidoapi/interfaces/adatec.py
--rw-r--r--   0 ampamo     (501) staff       (20)       38 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/setup.cfg
-drwxr-xr-x   0 ampamo     (501) staff       (20)        0 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/easypedidoapi.egg-info/
--rw-r--r--   0 ampamo     (501) staff       (20)      275 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/easypedidoapi.egg-info/PKG-INFO
--rw-r--r--   0 ampamo     (501) staff       (20)      312 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/easypedidoapi.egg-info/SOURCES.txt
--rw-r--r--   0 ampamo     (501) staff       (20)       16 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/easypedidoapi.egg-info/requires.txt
--rw-r--r--   0 ampamo     (501) staff       (20)       14 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/easypedidoapi.egg-info/top_level.txt
--rw-r--r--   0 ampamo     (501) staff       (20)        1 2023-03-08 00:07:28.000000 easypedidoapi-0.0.8/easypedidoapi.egg-info/dependency_links.txt
+drwxr-xr-x   0 ampamo     (501) staff       (20)        0 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/
+-rw-r--r--   0 ampamo     (501) staff       (20)      275 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/PKG-INFO
+-rw-r--r--   0 ampamo     (501) staff       (20)      724 2024-05-30 06:11:09.000000 easypedidoapi-0.0.9/setup.py
+drwxr-xr-x   0 ampamo     (501) staff       (20)        0 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/easypedidoapi/
+-rw-r--r--   0 ampamo     (501) staff       (20)       48 2023-09-13 20:44:37.000000 easypedidoapi-0.0.9/easypedidoapi/__init__.py
+-rw-r--r--   0 ampamo     (501) staff       (20)     2793 2024-05-30 06:11:09.000000 easypedidoapi-0.0.9/easypedidoapi/base.py
+drwxr-xr-x   0 ampamo     (501) staff       (20)        0 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/easypedidoapi/interfaces/
+-rw-r--r--   0 ampamo     (501) staff       (20)       36 2023-09-13 20:44:37.000000 easypedidoapi-0.0.9/easypedidoapi/interfaces/__init__.py
+-rw-r--r--   0 ampamo     (501) staff       (20)     8456 2024-05-30 06:11:09.000000 easypedidoapi-0.0.9/easypedidoapi/interfaces/adatec.py
+-rw-r--r--   0 ampamo     (501) staff       (20)       38 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/setup.cfg
+drwxr-xr-x   0 ampamo     (501) staff       (20)        0 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/easypedidoapi.egg-info/
+-rw-r--r--   0 ampamo     (501) staff       (20)      275 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/easypedidoapi.egg-info/PKG-INFO
+-rw-r--r--   0 ampamo     (501) staff       (20)      312 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/easypedidoapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ampamo     (501) staff       (20)       16 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/easypedidoapi.egg-info/requires.txt
+-rw-r--r--   0 ampamo     (501) staff       (20)       14 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/easypedidoapi.egg-info/top_level.txt
+-rw-r--r--   0 ampamo     (501) staff       (20)        1 2024-05-30 06:17:04.000000 easypedidoapi-0.0.9/easypedidoapi.egg-info/dependency_links.txt
```

### Comparing `easypedidoapi-0.0.8/setup.py` & `easypedidoapi-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Package which helps to consume EasyPedido API'
 
 setup(
     name='easypedidoapi',
     version=VERSION,
     author='Andrés Palacio',
     author_email='ampamo9@gmail.com',
```

### Comparing `easypedidoapi-0.0.8/easypedidoapi/base.py` & `easypedidoapi-0.0.9/easypedidoapi/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,15 @@
                 "key_field_name": key_field_name,
                 "content": content
             }
             headers = {
                 'X-Requested-With': 'XMLHttpRequest',
             }
 
-            response = requests.post(self.get_url(self.variants_update_url), data=data, headers=headers)
+            response = requests.post(self.get_url(
+                self.variants_update_url), data=data, headers=headers)
             if response.status_code == 200:
                 res = json.loads(response.content)
                 if res.get('success'):
                     self.mark_variants_as_updated()
 
             return response.content
-
-
```

### Comparing `easypedidoapi-0.0.8/easypedidoapi/interfaces/adatec.py` & `easypedidoapi-0.0.9/easypedidoapi/interfaces/adatec.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 
     # Querys
     query_get_products_to_update = (
         "SELECT "
         "   P.PRODUCTO_CODIGO, "
         "   INV.UBICACION, "
         "   PR.LISTA_CODIGO, "
-        "   PR.PRECIO, " 
+        "   PR.PRECIO, "
         "   INV.DISPONIBLE, "
         "   P.PROCESO AS P_PROC, "
         "   PR.PROCESO AS PR_PROC, "
-        "   INV.PROCESO AS INV_PROC "
+        "   INV.PROCESO AS INV_PROC, "
+        "   P.PRODUCTO_IMPUESTO AS IMPUESTO_PORCENTAJE "
         "FROM PRODUCTOS P INNER JOIN PRECIOS PR ON ( "
         "   P.EMPRESA_CODIGO = PR.EMPRESA_CODIGO "
         "   AND P.PRODUCTO_CODIGO = PR.PRODUCTO_CODIGO "
         ") INNER JOIN INVENTARIO INV ON( "
         "   P.EMPRESA_CODIGO = INV.EMPRESA_CODIGO "
         "   AND P.PRODUCTO_CODIGO = INV.PRODUCTO_CODIGO "
         ") "
@@ -104,16 +105,18 @@
         self.updated_products_by_location_code = {}
 
         cursor = self.connect_to_db()
         cursor.execute('EXEC AllMerge @LOG_ID=NULL')
         cursor.commit()
         cursor.execute(self.query_get_products_to_update.format(
             company_code=self.company_code,
-            location_codes=','.join(["'{}'".format(code) for code in location_codes]),
-            price_list_codes=','.join(["'{}'".format(code) for code in price_list_codes]),
+            location_codes=','.join(["'{}'".format(code)
+                                    for code in location_codes]),
+            price_list_codes=','.join(["'{}'".format(code)
+                                      for code in price_list_codes]),
         ))
 
         db_results = cursor.fetchall()
         cursor.close()
 
         results = {}
         for db_result in db_results:
@@ -121,34 +124,38 @@
             if db_result[2] not in self.updated_products_by_price_code:
                 codes = set()
                 codes.add(db_result[0])
                 self.updated_products_by_price_code.update({
                     db_result[2]: codes
                 })
             else:
-                self.updated_products_by_price_code.get(db_result[2]).add(db_result[0])
+                self.updated_products_by_price_code.get(
+                    db_result[2]).add(db_result[0])
 
             # prepare location data to mark as updated
             if db_result[1] not in self.updated_products_by_location_code:
                 codes = set()
                 codes.add(db_result[0])
                 self.updated_products_by_location_code.update({
                     db_result[1]: codes
                 })
             else:
-                self.updated_products_by_location_code.get(db_result[1]).add(db_result[0])
+                self.updated_products_by_location_code.get(
+                    db_result[1]).add(db_result[0])
 
             # prepare result
             product_code = db_result[0]
             price = str(db_result[3])
             is_active = 'true' if db_result[4] == 'Y' else 'false'
-            product_key = '{product_code};{price};{is_active}'.format(
+            tax_percentage = str(db_result[8])
+            product_key = '{product_code};{price};{is_active};{tax_percentage}'.format(
                 product_code=product_code,
                 price=price,
-                is_active=is_active
+                is_active=is_active,
+                tax_percentage=tax_percentage
             )
 
             if product_key not in results:
                 trade_ids = set()
                 trade_ids.add(self.get_trade_id(db_result[1]))
                 results.update({
                     product_key: trade_ids
@@ -157,24 +164,25 @@
                 results.get(product_key).add(self.get_trade_id(db_result[1]))
 
         serialized_data = []
         for product_key in results:
             item = product_key.split(';')
             serialized_data.append(
                 '[TRADE_IDS];[KEY_FIELD_VALUE];[NAME];[DESCRIPTION];[CURRENCY];[PRICE];'
-                '[TRACK_INVENTORY];[STOCK];[IS_ACTIVE]'
+                '[TRACK_INVENTORY];[STOCK];[IS_ACTIVE];[TAX_PERCENTAGE]'
                 .replace('[TRADE_IDS]', ','.join(results[product_key]))
                 .replace('[KEY_FIELD_VALUE]', item[0])
                 .replace('[NAME]', '')
                 .replace('[DESCRIPTION]', '')
                 .replace('[CURRENCY]', '')
                 .replace('[PRICE]', item[1])
                 .replace('[TRACK_INVENTORY]', '')
                 .replace('[STOCK]', '')
                 .replace('[IS_ACTIVE]', item[2])
+                .replace('[TAX_PERCENTAGE]', item[3])
             )
 
         return '|'.join(serialized_data) if len(serialized_data) > 0 else None
 
     def mark_variants_as_updated(self):
         cursor = self.connect_to_db()
         # Update prices
@@ -198,15 +206,16 @@
         cursor.commit()
         cursor.close()
 
     def get_trade_id(self, location_code):
         if location_code in self.trade_ids_by_location_code:
             return self.trade_ids_by_location_code.get(location_code)
         else:
-            raise Exception('trade_id to location code {} not found'.format(location_code))
+            raise Exception(
+                'trade_id to location code {} not found'.format(location_code))
 
     def update_variants(self, key_field_name, location_codes=None, price_list_codes=None):
         content = self.get_variants_content(location_codes, price_list_codes)
         if content:
             return self.send_updated_variants(key_field_name, content)
         else:
             return 'No hay productos para actualizar'
```

