# Comparing `tmp/odoo_addons_oca_wms-16.0.20240403.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_wms-16.0.20240405.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1565 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2337 b- defN 24-Apr-04 06:43 odoo_addons_oca_wms-16.0.20240403.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 06:43 odoo_addons_oca_wms-16.0.20240403.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-04 06:43 odoo_addons_oca_wms-16.0.20240403.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-Apr-04 06:43 odoo_addons_oca_wms-16.0.20240403.0.dist-info/RECORD
-4 files, 2815 bytes uncompressed, 807 bytes compressed:  71.3%
+Zip file size: 1570 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2437 b- defN 24-Apr-06 06:35 odoo_addons_oca_wms-16.0.20240405.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 06:35 odoo_addons_oca_wms-16.0.20240405.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-06 06:35 odoo_addons_oca_wms-16.0.20240405.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-Apr-06 06:35 odoo_addons_oca_wms-16.0.20240405.0.dist-info/RECORD
+4 files, 2915 bytes uncompressed, 812 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_wms-16.0.20240403.0.dist-info/METADATA
+Filename: odoo_addons_oca_wms-16.0.20240405.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240403.0.dist-info/WHEEL
+Filename: odoo_addons_oca_wms-16.0.20240405.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240403.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_wms-16.0.20240405.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240403.0.dist-info/RECORD
+Filename: odoo_addons_oca_wms-16.0.20240405.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_wms-16.0.20240403.0.dist-info/METADATA` & `odoo_addons_oca_wms-16.0.20240405.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-wms
-Version: 16.0.20240403.0
+Version: 16.0.20240405.0
 Summary: Meta package for oca-wms Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -24,14 +24,15 @@
 Requires-Dist: odoo-addon-stock-release-channel-partner-delivery-window <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-partner-public-holidays <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-plan <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-plan-process-end-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-process-end-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-propagate-channel-picking <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-shipment-advice <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-stock-release-channel-shipment-advice-process-end-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-shipment-lead-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-show-volume <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-show-weight <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-storage-type <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-storage-type-putaway-abc <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-warehouse-flow <16.1dev,>=16.0dev
```

