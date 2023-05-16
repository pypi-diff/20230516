# Comparing `tmp/odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230404.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2032 bytes, number of entries: 4
--rw-r--r--  2.0 unx     4531 b- defN 23-Apr-05 02:35 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230404.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-05 02:35 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230404.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-05 02:35 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230404.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      477 b- defN 23-Apr-05 02:35 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230404.0.dist-info/RECORD
-4 files, 5101 bytes uncompressed, 1090 bytes compressed:  78.6%
+Zip file size: 2046 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     4585 b- defN 23-May-16 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-16 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-16 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      477 b- defN 23-May-16 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/RECORD
+4 files, 5155 bytes uncompressed, 1104 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230404.0.dist-info/METADATA
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230404.0.dist-info/WHEEL
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230404.0.dist-info/top_level.txt
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230404.0.dist-info/RECORD
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230404.0.dist-info/METADATA` & `odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-shopinvader-odoo-shopinvader
-Version: 14.0.20230404.0
+Version: 14.0.20230515.0
 Summary: Meta package for shopinvader-odoo-shopinvader Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -48,14 +48,15 @@
 Requires-Dist: odoo14-addon-shopinvader-multi-category
 Requires-Dist: odoo14-addon-shopinvader-notification-default
 Requires-Dist: odoo14-addon-shopinvader-partner-firstname
 Requires-Dist: odoo14-addon-shopinvader-partner-vat
 Requires-Dist: odoo14-addon-shopinvader-pending-cart-reminder
 Requires-Dist: odoo14-addon-shopinvader-portal-mode
 Requires-Dist: odoo14-addon-shopinvader-pos
+Requires-Dist: odoo14-addon-shopinvader-price-per-qty
 Requires-Dist: odoo14-addon-shopinvader-product-attribute-set
 Requires-Dist: odoo14-addon-shopinvader-product-brand
 Requires-Dist: odoo14-addon-shopinvader-product-brand-image
 Requires-Dist: odoo14-addon-shopinvader-product-brand-tag
 Requires-Dist: odoo14-addon-shopinvader-product-manufactured-for
 Requires-Dist: odoo14-addon-shopinvader-product-media
 Requires-Dist: odoo14-addon-shopinvader-product-new
```

