# Comparing `tmp/xm_ai-0.5-py3-none-any.whl.zip` & `tmp/xm_ai-0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5771 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-May-15 21:17 xm_ai/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 23-May-15 21:17 xm_ai/aws_utils.py
--rw-r--r--  2.0 unx     2290 b- defN 23-May-15 21:17 xm_ai/database_utils.py
--rw-r--r--  2.0 unx     2211 b- defN 23-May-15 21:17 xm_ai/email_utils.py
--rw-r--r--  2.0 unx      238 b- defN 23-May-15 21:17 xm_ai/excel_utils.py
--rw-r--r--  2.0 unx     2199 b- defN 23-May-15 21:17 xm_ai/query_utils.py
--rw-r--r--  2.0 unx      134 b- defN 23-May-15 21:17 xm_ai/syntax_utils.py
--rw-r--r--  2.0 unx      600 b- defN 23-May-15 21:17 xm_ai/time_utils.py
--rw-r--r--  2.0 unx      471 b- defN 23-May-15 21:17 xm_ai-0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 21:17 xm_ai-0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-15 21:17 xm_ai-0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      888 b- defN 23-May-15 21:17 xm_ai-0.5.dist-info/RECORD
-12 files, 10329 bytes uncompressed, 4297 bytes compressed:  58.4%
+Zip file size: 5732 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-May-16 22:24 xm_ai/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 23-May-16 22:24 xm_ai/aws_utils.py
+-rw-r--r--  2.0 unx     2213 b- defN 23-May-16 22:24 xm_ai/database_utils.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-May-16 22:24 xm_ai/email_utils.py
+-rw-r--r--  2.0 unx      238 b- defN 23-May-16 22:24 xm_ai/excel_utils.py
+-rw-r--r--  2.0 unx     2199 b- defN 23-May-16 22:24 xm_ai/query_utils.py
+-rw-r--r--  2.0 unx      134 b- defN 23-May-16 22:24 xm_ai/syntax_utils.py
+-rw-r--r--  2.0 unx      600 b- defN 23-May-16 22:24 xm_ai/time_utils.py
+-rw-r--r--  2.0 unx      471 b- defN 23-May-16 22:24 xm_ai-0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-16 22:24 xm_ai-0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-16 22:24 xm_ai-0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      888 b- defN 23-May-16 22:24 xm_ai-0.6.dist-info/RECORD
+12 files, 10252 bytes uncompressed, 4258 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: xm_ai/syntax_utils.py
 Comment: 
 
 Filename: xm_ai/time_utils.py
 Comment: 
 
-Filename: xm_ai-0.5.dist-info/METADATA
+Filename: xm_ai-0.6.dist-info/METADATA
 Comment: 
 
-Filename: xm_ai-0.5.dist-info/WHEEL
+Filename: xm_ai-0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xm_ai-0.5.dist-info/top_level.txt
+Filename: xm_ai-0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xm_ai-0.5.dist-info/RECORD
+Filename: xm_ai-0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xm_ai/database_utils.py

```diff
@@ -39,15 +39,14 @@
     else:
         raise ValueError("Invalid Option Selected")
 
     try:
         db = MongoClient(connstring)[database_name]
         try:
             db.templates.find_one({})
-            global db  # make this accessible by any function in this module
             return db
         except pymongo.errors.ServerSelectionTimeoutError as error:
             print(error)
             print("This connection string likely does not have access to the database")
             raise pymongo.errors.ServerSelectionTimeoutError
 
     except EndpointConnectionError as error:
```

## Comparing `xm_ai-0.5.dist-info/RECORD` & `xm_ai-0.6.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 xm_ai/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 xm_ai/aws_utils.py,sha256=BZ8lqidsBhckW2Jy6-eJVbomt5yyo7LWqmKuGu2Ewe0,1200
-xm_ai/database_utils.py,sha256=Xu68_OPiRSnXnkMJWeBWc224fjs04QkMl_Nzzdo7l70,2290
+xm_ai/database_utils.py,sha256=0hClNv1-yfiKuRb0re95s05ylZJVqMxeE3m3Sg46Y30,2213
 xm_ai/email_utils.py,sha256=N0xmFD5eD3nG8nVejh9uF5w__XYHD9JSNTOVEAEHcrU,2211
 xm_ai/excel_utils.py,sha256=xafW_NtNMq6qETFisMDPohPfs34BbekUdyM1qQefr7o,238
 xm_ai/query_utils.py,sha256=-6rvNWf3-lrbfgqhRriIUPFP8f4ojcrn2-y25pP7LNo,2199
 xm_ai/syntax_utils.py,sha256=aWGhKkLLZQSOO4_gee_9EGO1b1KI8-KXZd45Ts2jNj4,134
 xm_ai/time_utils.py,sha256=qEsWIjq3GRG3a4L8yxQe2b_gJszsmXRDSsBZKR4b9cs,600
-xm_ai-0.5.dist-info/METADATA,sha256=sAQ80Bj0uo_C5d6PAVHL6IA-vQgvHxf35blI_oeBLJ4,471
-xm_ai-0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xm_ai-0.5.dist-info/top_level.txt,sha256=0tH-EgTFu93crY6L8lAB9az_LQotSkuUdG1rObgP0iA,6
-xm_ai-0.5.dist-info/RECORD,,
+xm_ai-0.6.dist-info/METADATA,sha256=d_VfJ-Jp-awRJBIP82rH_Bxr9ecYkB91Oiy-0V6rLeo,471
+xm_ai-0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+xm_ai-0.6.dist-info/top_level.txt,sha256=0tH-EgTFu93crY6L8lAB9az_LQotSkuUdG1rObgP0iA,6
+xm_ai-0.6.dist-info/RECORD,,
```

