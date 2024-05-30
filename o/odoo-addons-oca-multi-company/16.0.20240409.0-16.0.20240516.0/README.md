# Comparing `tmp/odoo_addons_oca_multi_company-16.0.20240409.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_multi_company-16.0.20240516.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1606 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1918 b- defN 24-Apr-10 04:58 odoo_addons_oca_multi_company-16.0.20240409.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 04:58 odoo_addons_oca_multi_company-16.0.20240409.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-10 04:58 odoo_addons_oca_multi_company-16.0.20240409.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      425 b- defN 24-Apr-10 04:58 odoo_addons_oca_multi_company-16.0.20240409.0.dist-info/RECORD
-4 files, 2436 bytes uncompressed, 768 bytes compressed:  68.5%
+Zip file size: 1612 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1996 b- defN 24-May-17 05:16 odoo_addons_oca_multi_company-16.0.20240516.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-17 05:16 odoo_addons_oca_multi_company-16.0.20240516.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-17 05:16 odoo_addons_oca_multi_company-16.0.20240516.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      425 b- defN 24-May-17 05:16 odoo_addons_oca_multi_company-16.0.20240516.0.dist-info/RECORD
+4 files, 2514 bytes uncompressed, 774 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_multi_company-16.0.20240409.0.dist-info/METADATA
+Filename: odoo_addons_oca_multi_company-16.0.20240516.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_multi_company-16.0.20240409.0.dist-info/WHEEL
+Filename: odoo_addons_oca_multi_company-16.0.20240516.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_multi_company-16.0.20240409.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_multi_company-16.0.20240516.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_multi_company-16.0.20240409.0.dist-info/RECORD
+Filename: odoo_addons_oca_multi_company-16.0.20240516.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_multi_company-16.0.20240409.0.dist-info/METADATA` & `odoo_addons_oca_multi_company-16.0.20240516.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-multi-company
-Version: 16.0.20240409.0
+Version: 16.0.20240516.0
 Summary: Meta package for oca-multi-company Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -26,10 +26,11 @@
 Requires-Dist: odoo-addon-res-company-active <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-res-company-category <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-res-company-code <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-res-company-search-view <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-product-company <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-stock-warehouse-multicompany <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-intercompany <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-stock-intercompany-bidirectional <16.1dev,>=16.0dev
 
 UNKNOWN
```

