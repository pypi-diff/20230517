# Comparing `tmp/odoo13_addons_oca_server_ux-13.0.20230228.0-py3-none-any.whl.zip` & `tmp/odoo13_addons_oca_server_ux-13.0.20230516.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1663 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1846 b- defN 23-Mar-01 08:16 odoo13_addons_oca_server_ux-13.0.20230228.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-01 08:16 odoo13_addons_oca_server_ux-13.0.20230228.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-01 08:16 odoo13_addons_oca_server_ux-13.0.20230228.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      417 b- defN 23-Mar-01 08:16 odoo13_addons_oca_server_ux-13.0.20230228.0.dist-info/RECORD
-4 files, 2356 bytes uncompressed, 841 bytes compressed:  64.3%
+Zip file size: 1681 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1953 b- defN 23-May-17 07:10 odoo13_addons_oca_server_ux-13.0.20230516.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 07:10 odoo13_addons_oca_server_ux-13.0.20230516.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-17 07:10 odoo13_addons_oca_server_ux-13.0.20230516.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      417 b- defN 23-May-17 07:10 odoo13_addons_oca_server_ux-13.0.20230516.0.dist-info/RECORD
+4 files, 2463 bytes uncompressed, 859 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo13_addons_oca_server_ux-13.0.20230228.0.dist-info/METADATA
+Filename: odoo13_addons_oca_server_ux-13.0.20230516.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo13_addons_oca_server_ux-13.0.20230228.0.dist-info/WHEEL
+Filename: odoo13_addons_oca_server_ux-13.0.20230516.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo13_addons_oca_server_ux-13.0.20230228.0.dist-info/top_level.txt
+Filename: odoo13_addons_oca_server_ux-13.0.20230516.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo13_addons_oca_server_ux-13.0.20230228.0.dist-info/RECORD
+Filename: odoo13_addons_oca_server_ux-13.0.20230516.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo13_addons_oca_server_ux-13.0.20230228.0.dist-info/METADATA` & `odoo13_addons_oca_server_ux-13.0.20230516.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: odoo13-addons-oca-server-ux
-Version: 13.0.20230228.0
+Version: 13.0.20230516.0
 Summary: Meta package for oca-server-ux Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 13.0
 Requires-Dist: odoo13-addon-announcement
 Requires-Dist: odoo13-addon-barcode-action
 Requires-Dist: odoo13-addon-base-action-visibility-restriction
+Requires-Dist: odoo13-addon-base-binary-url-import
 Requires-Dist: odoo13-addon-base-custom-filter
 Requires-Dist: odoo13-addon-base-duplicate-security-group
 Requires-Dist: odoo13-addon-base-export-manager
 Requires-Dist: odoo13-addon-base-field-deprecated
 Requires-Dist: odoo13-addon-base-import-security-group
 Requires-Dist: odoo13-addon-base-ir-actions-sequence
 Requires-Dist: odoo13-addon-base-menu-visibility-restriction
@@ -34,10 +35,11 @@
 Requires-Dist: odoo13-addon-document-quick-access-folder-auto-classification
 Requires-Dist: odoo13-addon-filter-multi-user
 Requires-Dist: odoo13-addon-mass-editing
 Requires-Dist: odoo13-addon-mass-operation-abstract
 Requires-Dist: odoo13-addon-multi-step-wizard
 Requires-Dist: odoo13-addon-sequence-check-digit
 Requires-Dist: odoo13-addon-sequence-reset-period
+Requires-Dist: odoo13-addon-test-base-binary-url-import
 
 UNKNOWN
```

