# Comparing `tmp/azureml_featurestore-0.0.1-py3-none-any.whl.zip` & `tmp/azureml_featurestore-0.1.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,57 @@
-Zip file size: 2251 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      249 b- defN 20-Jun-24 20:49 azureml/__init__.py
--rw-rw-rw-  2.0 fat     1021 b- defN 22-Apr-06 23:47 azureml_featurestore-0.0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      390 b- defN 22-Apr-06 23:47 azureml_featurestore-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Apr-06 23:47 azureml_featurestore-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 22-Apr-06 23:47 azureml_featurestore-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      528 b- defN 22-Apr-06 23:47 azureml_featurestore-0.0.1.dist-info/RECORD
-6 files, 2288 bytes uncompressed, 1279 bytes compressed:  44.1%
+Zip file size: 66566 bytes, number of entries: 55
+-rw-rw-rw-  2.0 fat      267 b- defN 23-May-17 19:57 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      565 b- defN 23-May-17 19:57 azureml/featurestore/__init__.py
+-rw-rw-rw-  2.0 fat    21083 b- defN 23-May-17 19:57 azureml/featurestore/_feature_set.py
+-rw-rw-rw-  2.0 fat       21 b- defN 23-May-17 20:05 azureml/featurestore/_version.py
+-rw-rw-rw-  2.0 fat     1108 b- defN 23-May-17 19:57 azureml/featurestore/abstract_feature_store.py
+-rw-rw-rw-  2.0 fat    25597 b- defN 23-May-17 19:57 azureml/featurestore/feature_set_spec.py
+-rw-rw-rw-  2.0 fat    27132 b- defN 23-May-17 19:57 azureml/featurestore/feature_store_client.py
+-rw-rw-rw-  2.0 fat      410 b- defN 23-May-17 19:57 azureml/featurestore/_identity/__init__.py
+-rw-rw-rw-  2.0 fat     6332 b- defN 23-May-17 19:57 azureml/featurestore/_identity/aml_hobospark_on_behalf_of.py
+-rw-rw-rw-  2.0 fat      455 b- defN 23-May-17 19:57 azureml/featurestore/_offline_query/__init__.py
+-rw-rw-rw-  2.0 fat      401 b- defN 23-May-17 19:57 azureml/featurestore/_offline_query/offline_retrieval_job.py
+-rw-rw-rw-  2.0 fat    10924 b- defN 23-May-17 19:57 azureml/featurestore/_offline_query/point_at_time.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-May-17 19:57 azureml/featurestore/_utils/__init__.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 23-May-17 19:57 azureml/featurestore/_utils/_constants.py
+-rw-rw-rw-  2.0 fat      398 b- defN 23-May-17 19:57 azureml/featurestore/_utils/_preview_method.py
+-rw-rw-rw-  2.0 fat     7359 b- defN 23-May-17 19:57 azureml/featurestore/_utils/arm_id_utils.py
+-rw-rw-rw-  2.0 fat     5210 b- defN 23-May-17 19:57 azureml/featurestore/_utils/materialize.py
+-rw-rw-rw-  2.0 fat     9810 b- defN 23-May-17 19:57 azureml/featurestore/_utils/spark_utils.py
+-rw-rw-rw-  2.0 fat     2370 b- defN 23-May-17 19:57 azureml/featurestore/_utils/type_map.py
+-rw-rw-rw-  2.0 fat    15837 b- defN 23-May-17 19:57 azureml/featurestore/_utils/utils.py
+-rw-rw-rw-  2.0 fat      681 b- defN 23-May-17 19:57 azureml/featurestore/contracts/__init__.py
+-rw-rw-rw-  2.0 fat     1243 b- defN 23-May-17 19:57 azureml/featurestore/contracts/column.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-May-17 19:57 azureml/featurestore/contracts/datetimeoffset.py
+-rw-rw-rw-  2.0 fat     3593 b- defN 23-May-17 19:57 azureml/featurestore/contracts/feature.py
+-rw-rw-rw-  2.0 fat     9275 b- defN 23-May-17 19:57 azureml/featurestore/contracts/feature_retrieval_spec.py
+-rw-rw-rw-  2.0 fat     2846 b- defN 23-May-17 19:57 azureml/featurestore/contracts/feature_source.py
+-rw-rw-rw-  2.0 fat     2019 b- defN 23-May-17 19:57 azureml/featurestore/contracts/offline_store.py
+-rw-rw-rw-  2.0 fat      646 b- defN 23-May-17 19:57 azureml/featurestore/contracts/online_store.py
+-rw-rw-rw-  2.0 fat      694 b- defN 23-May-17 19:57 azureml/featurestore/contracts/partition.py
+-rw-rw-rw-  2.0 fat     1230 b- defN 23-May-17 19:57 azureml/featurestore/contracts/store_connection.py
+-rw-rw-rw-  2.0 fat      753 b- defN 23-May-17 19:57 azureml/featurestore/contracts/timestamp_column.py
+-rw-rw-rw-  2.0 fat     2578 b- defN 23-May-17 19:57 azureml/featurestore/contracts/transformation_code.py
+-rw-rw-rw-  2.0 fat      294 b- defN 23-May-17 19:57 azureml/featurestore/grpc/__init__.py
+-rw-rw-rw-  2.0 fat     1364 b- defN 23-May-17 19:57 azureml/featurestore/grpc/_flight_feature_retrieval_client.py
+-rw-rw-rw-  2.0 fat     3276 b- defN 23-May-17 19:57 azureml/featurestore/grpc/_flight_feature_retrieval_server.py
+-rw-rw-rw-  2.0 fat     5923 b- defN 23-May-17 19:57 azureml/featurestore/grpc/_flight_helper.py
+-rw-rw-rw-  2.0 fat      934 b- defN 23-May-17 19:57 azureml/featurestore/grpc/_inline_feature_retrieval_client.py
+-rw-rw-rw-  2.0 fat      391 b- defN 23-May-17 19:57 azureml/featurestore/offline_store/__init__.py
+-rw-rw-rw-  2.0 fat     9020 b- defN 23-May-17 19:57 azureml/featurestore/offline_store/azure_data_lake_offline_store.py
+-rw-rw-rw-  2.0 fat      367 b- defN 23-May-17 19:57 azureml/featurestore/offline_store/partition/__init__.py
+-rw-rw-rw-  2.0 fat     2381 b- defN 23-May-17 19:57 azureml/featurestore/offline_store/partition/timestamp_partition.py
+-rw-rw-rw-  2.0 fat      242 b- defN 23-May-17 19:57 azureml/featurestore/online/__init__.py
+-rw-rw-rw-  2.0 fat     5515 b- defN 23-May-17 19:57 azureml/featurestore/online/_online_feature_getter.py
+-rw-rw-rw-  2.0 fat     4492 b- defN 23-May-17 19:57 azureml/featurestore/online/_online_feature_materialization.py
+-rw-rw-rw-  2.0 fat     1669 b- defN 23-May-17 19:57 azureml/featurestore/online/_redis_client_pool.py
+-rw-rw-rw-  2.0 fat      643 b- defN 23-May-17 19:57 azureml/featurestore/online/_utils.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-May-17 19:57 azureml/featurestore/schema/__init__.py
+-rw-rw-rw-  2.0 fat     1655 b- defN 23-May-17 19:57 azureml/featurestore/schema/feature_retrieval_spec_schema.py
+-rw-rw-rw-  2.0 fat     5944 b- defN 23-May-17 19:57 azureml/featurestore/schema/feature_set_schema.py
+-rw-rw-rw-  2.0 fat      823 b- defN 23-May-17 20:08 azureml_featurestore-0.1.0b1.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat     1142 b- defN 23-May-17 20:08 azureml_featurestore-0.1.0b1.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-17 20:08 azureml_featurestore-0.1.0b1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-May-17 20:08 azureml_featurestore-0.1.0b1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1921 b- defN 23-May-17 20:08 azureml_featurestore-0.1.0b1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     5698 b- defN 23-May-17 20:08 azureml_featurestore-0.1.0b1.dist-info/RECORD
+55 files, 217777 bytes uncompressed, 57198 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -1,19 +1,166 @@
 Filename: azureml/__init__.py
 Comment: 
 
-Filename: azureml_featurestore-0.0.1.dist-info/LICENSE.txt
+Filename: azureml/featurestore/__init__.py
 Comment: 
 
-Filename: azureml_featurestore-0.0.1.dist-info/METADATA
+Filename: azureml/featurestore/_feature_set.py
 Comment: 
 
-Filename: azureml_featurestore-0.0.1.dist-info/WHEEL
+Filename: azureml/featurestore/_version.py
 Comment: 
 
-Filename: azureml_featurestore-0.0.1.dist-info/top_level.txt
+Filename: azureml/featurestore/abstract_feature_store.py
 Comment: 
 
-Filename: azureml_featurestore-0.0.1.dist-info/RECORD
+Filename: azureml/featurestore/feature_set_spec.py
+Comment: 
+
+Filename: azureml/featurestore/feature_store_client.py
+Comment: 
+
+Filename: azureml/featurestore/_identity/__init__.py
+Comment: 
+
+Filename: azureml/featurestore/_identity/aml_hobospark_on_behalf_of.py
+Comment: 
+
+Filename: azureml/featurestore/_offline_query/__init__.py
+Comment: 
+
+Filename: azureml/featurestore/_offline_query/offline_retrieval_job.py
+Comment: 
+
+Filename: azureml/featurestore/_offline_query/point_at_time.py
+Comment: 
+
+Filename: azureml/featurestore/_utils/__init__.py
+Comment: 
+
+Filename: azureml/featurestore/_utils/_constants.py
+Comment: 
+
+Filename: azureml/featurestore/_utils/_preview_method.py
+Comment: 
+
+Filename: azureml/featurestore/_utils/arm_id_utils.py
+Comment: 
+
+Filename: azureml/featurestore/_utils/materialize.py
+Comment: 
+
+Filename: azureml/featurestore/_utils/spark_utils.py
+Comment: 
+
+Filename: azureml/featurestore/_utils/type_map.py
+Comment: 
+
+Filename: azureml/featurestore/_utils/utils.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/__init__.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/column.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/datetimeoffset.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/feature.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/feature_retrieval_spec.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/feature_source.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/offline_store.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/online_store.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/partition.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/store_connection.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/timestamp_column.py
+Comment: 
+
+Filename: azureml/featurestore/contracts/transformation_code.py
+Comment: 
+
+Filename: azureml/featurestore/grpc/__init__.py
+Comment: 
+
+Filename: azureml/featurestore/grpc/_flight_feature_retrieval_client.py
+Comment: 
+
+Filename: azureml/featurestore/grpc/_flight_feature_retrieval_server.py
+Comment: 
+
+Filename: azureml/featurestore/grpc/_flight_helper.py
+Comment: 
+
+Filename: azureml/featurestore/grpc/_inline_feature_retrieval_client.py
+Comment: 
+
+Filename: azureml/featurestore/offline_store/__init__.py
+Comment: 
+
+Filename: azureml/featurestore/offline_store/azure_data_lake_offline_store.py
+Comment: 
+
+Filename: azureml/featurestore/offline_store/partition/__init__.py
+Comment: 
+
+Filename: azureml/featurestore/offline_store/partition/timestamp_partition.py
+Comment: 
+
+Filename: azureml/featurestore/online/__init__.py
+Comment: 
+
+Filename: azureml/featurestore/online/_online_feature_getter.py
+Comment: 
+
+Filename: azureml/featurestore/online/_online_feature_materialization.py
+Comment: 
+
+Filename: azureml/featurestore/online/_redis_client_pool.py
+Comment: 
+
+Filename: azureml/featurestore/online/_utils.py
+Comment: 
+
+Filename: azureml/featurestore/schema/__init__.py
+Comment: 
+
+Filename: azureml/featurestore/schema/feature_retrieval_spec_schema.py
+Comment: 
+
+Filename: azureml/featurestore/schema/feature_set_schema.py
+Comment: 
+
+Filename: azureml_featurestore-0.1.0b1.dist-info/DESCRIPTION.rst
+Comment: 
+
+Filename: azureml_featurestore-0.1.0b1.dist-info/metadata.json
+Comment: 
+
+Filename: azureml_featurestore-0.1.0b1.dist-info/top_level.txt
+Comment: 
+
+Filename: azureml_featurestore-0.1.0b1.dist-info/WHEEL
+Comment: 
+
+Filename: azureml_featurestore-0.1.0b1.dist-info/METADATA
+Comment: 
+
+Filename: azureml_featurestore-0.1.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/__init__.py

```diff
@@ -1,4 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
-__path__ = __import__('pkgutil').extend_path(__path__, __name__)
+
+__path__ = __import__("pkgutil").extend_path(__path__, __name__)  # type: ignore
```

