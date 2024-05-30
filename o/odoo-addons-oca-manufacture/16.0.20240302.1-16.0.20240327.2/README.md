# Comparing `tmp/odoo_addons_oca_manufacture-16.0.20240302.1-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_manufacture-16.0.20240327.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1664 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2208 b- defN 24-Mar-03 05:25 odoo_addons_oca_manufacture-16.0.20240302.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-03 05:25 odoo_addons_oca_manufacture-16.0.20240302.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-03 05:25 odoo_addons_oca_manufacture-16.0.20240302.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      417 b- defN 24-Mar-03 05:25 odoo_addons_oca_manufacture-16.0.20240302.1.dist-info/RECORD
-4 files, 2718 bytes uncompressed, 842 bytes compressed:  69.0%
+Zip file size: 1700 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2443 b- defN 24-Mar-29 06:05 odoo_addons_oca_manufacture-16.0.20240327.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-29 06:05 odoo_addons_oca_manufacture-16.0.20240327.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Mar-29 06:05 odoo_addons_oca_manufacture-16.0.20240327.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      417 b- defN 24-Mar-29 06:05 odoo_addons_oca_manufacture-16.0.20240327.2.dist-info/RECORD
+4 files, 2953 bytes uncompressed, 878 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_manufacture-16.0.20240302.1.dist-info/METADATA
+Filename: odoo_addons_oca_manufacture-16.0.20240327.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_manufacture-16.0.20240302.1.dist-info/WHEEL
+Filename: odoo_addons_oca_manufacture-16.0.20240327.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_manufacture-16.0.20240302.1.dist-info/top_level.txt
+Filename: odoo_addons_oca_manufacture-16.0.20240327.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_manufacture-16.0.20240302.1.dist-info/RECORD
+Filename: odoo_addons_oca_manufacture-16.0.20240327.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_manufacture-16.0.20240302.1.dist-info/METADATA` & `odoo_addons_oca_manufacture-16.0.20240327.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-manufacture
-Version: 16.0.20240302.1
+Version: 16.0.20240327.2
 Summary: Meta package for oca-manufacture Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-account-move-line-mrp-info <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-attachment-mgmt <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-bom-component-menu <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-bom-hierarchy <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-mrp-bom-line-formula-quantity <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-bom-location <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-bom-tracking <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-default-workorder-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-lot-number-propagation <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-lot-production-date <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-multi-level <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-multi-level-estimate <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-packaging-default <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-planned-order-matrix <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-production-note <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-production-quant-manual-assign <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-restrict-lot <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-sale-info <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-mrp-subcontracting-bom-dual-use <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-subcontracting-inhibit <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-mrp-subcontracting-partner-management <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-subcontracting-purchase-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-subcontracting-skip-no-negative <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-tag <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-unbuild-move-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-warehouse-calendar <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-workcenter-cost <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mrp-workorder-lot-display <16.1dev,>=16.0dev
```

