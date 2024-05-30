# Comparing `tmp/odoo_addons_oca_product_attribute-16.0.20240511.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_product_attribute-16.0.20240517.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2040 bytes, number of entries: 4
--rw-r--r--  2.0 unx     5364 b- defN 24-May-12 05:41 odoo_addons_oca_product_attribute-16.0.20240511.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 05:41 odoo_addons_oca_product_attribute-16.0.20240511.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-12 05:41 odoo_addons_oca_product_attribute-16.0.20240511.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      441 b- defN 24-May-12 05:41 odoo_addons_oca_product_attribute-16.0.20240511.0.dist-info/RECORD
-4 files, 5898 bytes uncompressed, 1170 bytes compressed:  80.2%
+Zip file size: 2063 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     5505 b- defN 24-May-18 05:48 odoo_addons_oca_product_attribute-16.0.20240517.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-18 05:48 odoo_addons_oca_product_attribute-16.0.20240517.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-18 05:48 odoo_addons_oca_product_attribute-16.0.20240517.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      441 b- defN 24-May-18 05:48 odoo_addons_oca_product_attribute-16.0.20240517.1.dist-info/RECORD
+4 files, 6039 bytes uncompressed, 1193 bytes compressed:  80.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_product_attribute-16.0.20240511.0.dist-info/METADATA
+Filename: odoo_addons_oca_product_attribute-16.0.20240517.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_product_attribute-16.0.20240511.0.dist-info/WHEEL
+Filename: odoo_addons_oca_product_attribute-16.0.20240517.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_product_attribute-16.0.20240511.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_product_attribute-16.0.20240517.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_product_attribute-16.0.20240511.0.dist-info/RECORD
+Filename: odoo_addons_oca_product_attribute-16.0.20240517.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_product_attribute-16.0.20240511.0.dist-info/METADATA` & `odoo_addons_oca_product_attribute-16.0.20240517.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-product-attribute
-Version: 16.0.20240511.0
+Version: 16.0.20240517.1
 Summary: Meta package for oca-product-attribute Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -31,14 +31,15 @@
 Requires-Dist: odoo-addon-product-get-price-helper <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-logistics-uom <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-lot-sequence <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-manufacturer <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-multi-category <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-net-weight <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-optional-product-quantity <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-product-origin <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-packaging-container-deposit <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-packaging-dimension <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-packaging-level <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-packaging-level-purchasable <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-packaging-level-salable <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-pricelist-alternative <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-pricelist-direct-print <16.1dev,>=16.0dev
@@ -55,14 +56,15 @@
 Requires-Dist: odoo-addon-product-product-template-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-profile <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-route-mto <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-sale-description <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-secondary-unit <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-sequence <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-set <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-product-standard-price-tax-included <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-state <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-stock-state <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-supplierinfo-archive <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-supplierinfo-code <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-supplierinfo-for-customer <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-supplierinfo-revision <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-supplierinfo-stock-picking-type <16.1dev,>=16.0dev
```

