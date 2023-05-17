# Comparing `tmp/etiq_spark-1.3.8b2-cp39-cp39-win_amd64.whl.zip` & `tmp/etiq_spark-1.3.8b3-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 347765 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  1065472 b- defN 23-Apr-26 20:57 etiq/spark.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1238 b- defN 23-Apr-26 20:57 etiq/spark.pyi
--rw-rw-rw-  2.0 fat     2041 b- defN 23-Apr-26 20:57 etiq_spark-1.3.8b2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-26 20:57 etiq_spark-1.3.8b2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-26 20:57 etiq_spark-1.3.8b2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      477 b- defN 23-Apr-26 20:57 etiq_spark-1.3.8b2.dist-info/RECORD
-6 files, 1069327 bytes uncompressed, 346905 bytes compressed:  67.6%
+Zip file size: 347764 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat  1065472 b- defN 23-Apr-27 15:01 etiq/spark.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1238 b- defN 23-Apr-27 15:01 etiq/spark.pyi
+-rw-rw-rw-  2.0 fat     2041 b- defN 23-Apr-27 15:01 etiq_spark-1.3.8b3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-27 15:01 etiq_spark-1.3.8b3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-27 15:01 etiq_spark-1.3.8b3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      477 b- defN 23-Apr-27 15:01 etiq_spark-1.3.8b3.dist-info/RECORD
+6 files, 1069327 bytes uncompressed, 346904 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: etiq/spark.cp39-win_amd64.pyd
 Comment: 
 
 Filename: etiq/spark.pyi
 Comment: 
 
-Filename: etiq_spark-1.3.8b2.dist-info/METADATA
+Filename: etiq_spark-1.3.8b3.dist-info/METADATA
 Comment: 
 
-Filename: etiq_spark-1.3.8b2.dist-info/WHEEL
+Filename: etiq_spark-1.3.8b3.dist-info/WHEEL
 Comment: 
 
-Filename: etiq_spark-1.3.8b2.dist-info/top_level.txt
+Filename: etiq_spark-1.3.8b3.dist-info/top_level.txt
 Comment: 
 
-Filename: etiq_spark-1.3.8b2.dist-info/RECORD
+Filename: etiq_spark-1.3.8b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `etiq_spark-1.3.8b2.dist-info/METADATA` & `etiq_spark-1.3.8b3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etiq-spark
-Version: 1.3.8b2
+Version: 1.3.8b3
 Summary: ETIQ.ai ML Testing library
 Home-page: https://etiq.ai/
 Author: ETIQ AI
 Author-email: devops@etiq.ai
 License: UNKNOWN
 Keywords: ai,bias,etiq,fairness
 Platform: UNKNOWN
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.6,<3.11
 Description-Content-Type: text/markdown
-Requires-Dist: etiq (==1.3.8b1)
+Requires-Dist: etiq (==1.3.8b3)
 Requires-Dist: pyspark
 
 
 # ETIQ AI
 
 Etiq helps companies test and monitor ML models. For data science & ML teams,
 Etiq tests ML algorithms, identifying issues and preventing accuracy loss in
```

