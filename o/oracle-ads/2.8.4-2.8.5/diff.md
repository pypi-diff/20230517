# Comparing `tmp/oracle_ads-2.8.4.tar.gz` & `tmp/oracle_ads-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oracle_ads-2.8.4.tar", last modified: Fri May  5 18:10:05 2023, max compression
+gzip compressed data, was "oracle_ads-2.8.5.tar", last modified: Wed May 17 18:39:08 2023, max compression
```

## Comparing `oracle_ads-2.8.4.tar` & `oracle_ads-2.8.5.tar`

### file list

```diff
@@ -1,535 +1,533 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    48614 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/THIRD_PARTY_LICENSES.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.662151 oracle_ads-2.8.4/ads/
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/ads
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/ads_version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.662151 oracle_ads-2.8.4/ads/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/automl/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    35984 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/automl/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.662151 oracle_ads-2.8.4/ads/bds/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/bds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/bds/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/bds/big_data_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.662151 oracle_ads-2.8.4/ads/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60039 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/catalog/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/catalog/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/catalog/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/catalog/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/common/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/common/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/artifact/.model-ignore
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33843 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/card_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    20253 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/common/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/decorator/argument_to_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/decorator/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/decorator/runtime_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/decorator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/dsc_file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/extended_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/common/function/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/function/fn_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/function/func_conf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    72294 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/model_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/model_artifact_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/model_export_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/object_storage_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/oci_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/oci_datascience.py
--rw-r--r--   0 runner    (1001) docker     (123)    42155 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/oci_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    37213 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/oci_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/oci_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    16565 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    45941 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22306 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/word_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/data_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/data_labeling_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/data_labeling/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/interface/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/interface/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/interface/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/data_labeling/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/loader/file_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/data_labeling/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/mixin/data_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/data_labeling/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/parser/dls_record_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/parser/export_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/parser/export_record_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/data_labeling/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/dataset_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/dls_record_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/export_record_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/jsonl_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/metadata_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/record_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/data_labeling/visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/visualizer/image_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/visualizer/text_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/database/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/database/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65402 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataflow/dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataflow/dataflowsummary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17306 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/correlation_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/dask_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/dataframe_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    70924 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/dataset_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    38407 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/dataset_with_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    37220 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/feature_engineering_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/forecasting_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    26056 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/recommendation_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/regression_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    39503 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/sampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/target.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/dbmixin/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dbmixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dbmixin/db_pandas_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/environment/ml_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/evaluations/
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/evaluations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39617 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/evaluations/evaluation_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    53173 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/evaluations/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/evaluations/statistical_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/base_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    41704 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/mlx_global_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/mlx_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/mlx_local_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/mlx_whatif_explainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/accessor/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/dataframe_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/eda_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/eda_mixin_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/feature_types_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/series_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/adsimage/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsimage/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsimage/image_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/adsimage/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsimage/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsimage/interface/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/adsstring/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsstring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/adsstring/oci_language/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsstring/oci_language/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/adsstring/string/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsstring/string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/data_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.678151 oracle_ads-2.8.4/ads/feature_engineering/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1600358 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/dataset/zip_code_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/feature_engineering/feature_type/
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/address.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/oci_language.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/creditcard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/gis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/feature_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/feature_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address_v6.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/lat_long.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/ordinal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/unknown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/zip_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/ads_search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    57469 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/search_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/stopping_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/tuner_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/hpo/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_edf.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_intermediate_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_optimization_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_parallel_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_param_importances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/ads_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    35717 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    59213 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dsc_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    40623 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dsc_job_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/builders/runtimes/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/runtimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/runtimes/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/runtimes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/runtimes/container_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/runtimes/python_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/env_var_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/schema/infrastructure_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/schema/job_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/schema/runtime_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/schema/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/driver_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/driver_oci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/driver_python.py
--rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/driver_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.690152 oracle_ads-2.8.4/ads/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/artifact_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/artifact_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/base_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.690152 oracle_ads-2.8.4/ads/model/common/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/common/.model-ignore
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37764 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/datascience_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.690152 oracle_ads-2.8.4/ads/model/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.690152 oracle_ads-2.8.4/ads/model/deployment/common/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/model_deployer.py
--rw-r--r--   0 runner    (1001) docker     (123)    60706 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/model_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19761 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/model_deployment_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/model_deployment_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/model_deployment_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.690152 oracle_ads-2.8.4/ads/model/extractor/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/automl_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/huggingface_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/keras_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/lightgbm_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/model_info_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/model_info_extractor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/pytorch_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/sklearn_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/spark_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/tensorflow_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/xgboost_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/automl_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/huggingface_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/lightgbm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/pytorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/spark_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/tensorflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   131287 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/generic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/artifact_introspection_test/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/artifact_introspection_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    54236 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_metadata_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_version_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/env_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/model_deployment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/model_provenance_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/runtime_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/runtime/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/schemas/inference_env_info_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/schemas/model_provenance_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/schemas/training_env_info_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/serde/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/serde/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    43205 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/serde/model_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/service/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21239 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/service/oci_datascience_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/service/oci_datascience_model_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/service/oci_datascience_model_version_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/transformer/onnx_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/mysqldb/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/mysqldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/mysqldb/mysql_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/opctl/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/ads_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/ads_ml_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/ads_ml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/ads_model_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    33122 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28259 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/cmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/manifest_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/multipart_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/pack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/config/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/config/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/diagnostics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/config/diagnostics/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/versioner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/diagnostics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/diagnostics/check_distributed_job_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/diagnostics/check_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/diagnostics/requirement_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/cmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/distributed/common/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/abstract_cluster_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/abstract_framework_spec_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_provider_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/framework_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.gpu
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.job
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.job.gpu
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/cuda.repo
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/merge_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/index.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/model/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/model/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/model/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spark/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spark/cmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/spec/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spec/abstract_operator_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spec/operator_spec_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/templates/diagnostic_report_template.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/oracledb/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/oracledb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/oracledb/oracle_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84848 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/ads_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/ads_pipeline_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/ads_pipeline_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/pipeline/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/builders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/pipeline/builders/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/builders/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/builders/infrastructure/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/pipeline/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/pipeline/visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/visualizer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/visualizer/graph_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/visualizer/text_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.706152 oracle_ads-2.8.4/ads/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/auth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/big_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/oracledb.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.706152 oracle_ads-2.8.4/ads/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/telemetry/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.706152 oracle_ads-2.8.4/ads/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/dataflow_pyspark.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/dataflow_sparksql.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/func.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score-pkl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_generic.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_huggingface_pipeline.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_lightgbm.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_onnx.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_onnx_new.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_oracle_automl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_pyspark.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_pytorch.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_scikit-learn.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_tensorflow.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_xgboost.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.706152 oracle_ads-2.8.4/ads/text_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/udfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/ads/type_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/abstract_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/constant_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/continuous_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/credit_card_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/datetime_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/discrete_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/document_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/ip_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/latlon_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/phone_number_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/type_discovery_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/typed_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/unknown_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/zipcode_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/ads/vault/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/vault/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/oracle_ads.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-05 18:10:05.000000 oracle_ads-2.8.4/oracle_ads.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-05-05 18:10:05.000000 oracle_ads-2.8.4/oracle_ads.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:10:05.000000 oracle_ads-2.8.4/oracle_ads.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-05 18:10:05.000000 oracle_ads-2.8.4/oracle_ads.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 18:10:05.000000 oracle_ads-2.8.4/oracle_ads.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    48614 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/THIRD_PARTY_LICENSES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.134277 oracle_ads-2.8.5/ads/
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/ads
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/ads_version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.134277 oracle_ads-2.8.5/ads/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/automl/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35984 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/automl/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.134277 oracle_ads-2.8.5/ads/bds/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/bds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/bds/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/bds/big_data_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.134277 oracle_ads-2.8.5/ads/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60039 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/catalog/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/catalog/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/catalog/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/catalog/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/common/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/artifact/.model-ignore
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35972 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/card_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20253 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/common/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/decorator/argument_to_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/decorator/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/decorator/runtime_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/decorator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/dsc_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/extended_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/common/function/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/function/fn_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/function/func_conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72294 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/model_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/model_artifact_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/model_export_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/object_storage_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/oci_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/oci_datascience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42155 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/oci_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37213 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/oci_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/oci_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16565 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46073 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22306 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/word_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/data_labeling_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/interface/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/interface/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/interface/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/loader/file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/mixin/data_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/parser/dls_record_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/parser/export_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/parser/export_record_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/dls_record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/export_record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/jsonl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/metadata_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/visualizer/image_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/visualizer/text_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/database/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65402 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataflow/dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataflow/dataflowsummary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17306 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/correlation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/dask_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/dataframe_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72309 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/dataset_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38574 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/dataset_with_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37220 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/feature_engineering_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/forecasting_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/label_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/dataset/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/mixin/dataset_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26056 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22168 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/recommendation_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/regression_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39503 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/sampled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/dbmixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dbmixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dbmixin/db_pandas_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/environment/ml_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/evaluations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/evaluations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39617 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/evaluations/evaluation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53173 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/evaluations/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/evaluations/statistical_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/base_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41704 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/mlx_global_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/mlx_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/mlx_local_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/mlx_whatif_explainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/accessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/dataframe_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/eda_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/eda_mixin_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/feature_types_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/series_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/adsimage/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsimage/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsimage/image_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/adsimage/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsimage/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsimage/interface/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/adsstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsstring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/adsstring/oci_language/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsstring/oci_language/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/adsstring/string/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsstring/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/data_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1600358 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/dataset/zip_code_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.150278 oracle_ads-2.8.5/ads/feature_engineering/feature_type/
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/address.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.150278 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/oci_language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.150278 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/creditcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/gis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.150278 oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/feature_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/feature_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address_v6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/lat_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/ordinal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/zip_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.150278 oracle_ads-2.8.5/ads/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/ads_search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57469 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/stopping_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/tuner_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/hpo/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_edf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_intermediate_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_optimization_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_parallel_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_param_importances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/ads_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35717 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59213 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dsc_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40623 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dsc_job_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/builders/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/runtimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/runtimes/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/runtimes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/runtimes/container_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/runtimes/python_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/env_var_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/schema/infrastructure_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/schema/job_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/schema/runtime_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/schema/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/driver_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/driver_oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/driver_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/driver_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.158278 oracle_ads-2.8.5/ads/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/artifact_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/artifact_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/base_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.158278 oracle_ads-2.8.5/ads/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/common/.model-ignore
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37764 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/datascience_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.158278 oracle_ads-2.8.5/ads/model/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.158278 oracle_ads-2.8.5/ads/model/deployment/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/model_deployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60718 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19761 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/model_deployment_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/model_deployment_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/model_deployment_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.158278 oracle_ads-2.8.5/ads/model/extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/automl_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/huggingface_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/keras_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/lightgbm_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/model_info_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/model_info_extractor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/pytorch_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/sklearn_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/spark_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/tensorflow_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/xgboost_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/automl_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/huggingface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/lightgbm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/pytorch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/spark_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/tensorflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131281 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/generic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/artifact_introspection_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/artifact_introspection_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54236 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_metadata_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_version_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/env_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/model_deployment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/model_provenance_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/runtime_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/runtime/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/schemas/inference_env_info_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/schemas/model_provenance_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/schemas/training_env_info_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/serde/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/serde/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43205 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/serde/model_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21239 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/service/oci_datascience_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/service/oci_datascience_model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/service/oci_datascience_model_version_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/transformer/onnx_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/mysqldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/mysqldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/mysqldb/mysql_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/opctl/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/opctl/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/ads_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/ads_ml_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/ads_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/ads_model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33122 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28259 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/manifest_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/multipart_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/pack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/config/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/diagnostics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/config/diagnostics/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/versioner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/diagnostics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/diagnostics/check_distributed_job_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/diagnostics/check_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/diagnostics/requirement_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/distributed/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/abstract_cluster_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/abstract_framework_spec_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_provider_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/framework_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.gpu
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.job
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.job.gpu
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/cuda.repo
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/merge_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/model/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/model/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/spark/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/spark/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/opctl/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/templates/diagnostic_report_template.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/oracledb/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/oracledb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/oracledb/oracle_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84848 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/ads_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/ads_pipeline_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/ads_pipeline_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/pipeline/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/builders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/pipeline/builders/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/builders/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/builders/infrastructure/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/pipeline/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/pipeline/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/visualizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/visualizer/graph_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/visualizer/text_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/big_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/oracledb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/telemetry/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/dataflow_pyspark.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/dataflow_sparksql.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/func.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score-pkl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_generic.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_huggingface_pipeline.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_lightgbm.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_onnx.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_onnx_new.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_oracle_automl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_pyspark.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_pytorch.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_scikit-learn.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_tensorflow.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_xgboost.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/ads/text_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/udfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/ads/type_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/abstract_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/constant_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/continuous_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/credit_card_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/datetime_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/discrete_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/document_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/ip_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/latlon_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/phone_number_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/type_discovery_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/typed_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/unknown_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/zipcode_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/ads/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/vault/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/oracle_ads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-17 18:39:08.000000 oracle_ads-2.8.5/oracle_ads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-05-17 18:39:08.000000 oracle_ads-2.8.5/oracle_ads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:39:08.000000 oracle_ads-2.8.5/oracle_ads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-17 18:39:08.000000 oracle_ads-2.8.5/oracle_ads.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 18:39:08.000000 oracle_ads-2.8.5/oracle_ads.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-17 18:39:05.000000 oracle_ads-2.8.5/setup.py
```

### Comparing `oracle_ads-2.8.4/LICENSE.txt` & `oracle_ads-2.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/MANIFEST.in` & `oracle_ads-2.8.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/PKG-INFO` & `oracle_ads-2.8.5/oracle_ads.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oracle_ads
-Version: 2.8.4
+Name: oracle-ads
+Version: 2.8.5
 Summary: Oracle Accelerated Data Science SDK
 Home-page: https://docs.oracle.com/en-us/iaas/tools/ads-sdk/latest/index.html
 Author: Oracle Data Science
 License: Universal Permissive License 1.0
 Project-URL: Github, https://github.com/oracle/accelerated-data-science
 Project-URL: Documentation, https://accelerated-data-science.readthedocs.io/en/latest/index.html
 Keywords: Oracle Cloud Infrastructure,OCI,Machine Learning,ML,Artificial Intelligence,AI,Data Science,Cloud,Oracle
```

### Comparing `oracle_ads-2.8.4/README.md` & `oracle_ads-2.8.5/README.md`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/THIRD_PARTY_LICENSES.txt` & `oracle_ads-2.8.5/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/__init__.py` & `oracle_ads-2.8.5/ads/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/automl/driver.py` & `oracle_ads-2.8.5/ads/automl/driver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/automl/provider.py` & `oracle_ads-2.8.5/ads/automl/provider.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/bds/auth.py` & `oracle_ads-2.8.5/ads/bds/auth.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/bds/big_data_service.py` & `oracle_ads-2.8.5/ads/bds/big_data_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/catalog/model.py` & `oracle_ads-2.8.5/ads/catalog/model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/catalog/notebook.py` & `oracle_ads-2.8.5/ads/catalog/notebook.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/catalog/project.py` & `oracle_ads-2.8.5/ads/catalog/project.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/catalog/summary.py` & `oracle_ads-2.8.5/ads/catalog/summary.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/cli.py` & `oracle_ads-2.8.5/ads/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/analyzer.py` & `oracle_ads-2.8.5/ads/common/analyzer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/artifact/.model-ignore` & `oracle_ads-2.8.5/ads/common/artifact/.model-ignore`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/auth.py` & `oracle_ads-2.8.5/ads/common/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import copy
 import os
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional, Union
 
 import ads.telemetry
 import oci
 from ads.common import logger
 from ads.common.decorator.deprecate import deprecated
 from ads.common.extended_enum import ExtendedEnumMeta
 from oci.config import DEFAULT_LOCATION  # "~/.oci/config"
@@ -41,15 +41,15 @@
     set by use at any given time and can be provided by this class in any ADS module.
     """
 
     oci_iam_type: str = None
     oci_cli_auth: str = None
     oci_config_path: str = None
     oci_key_profile: str = None
-    oci_config: str = None
+    oci_config: Dict = None
     oci_signer: Any = None
     oci_signer_callable: Callable = None
     oci_signer_kwargs: Dict = None
     oci_client_kwargs: Dict = None
 
     def __post_init__(self):
         self.oci_iam_type = self.oci_iam_type or os.environ.get(
@@ -61,16 +61,14 @@
         self.oci_config_path = self.oci_config_path or os.environ.get(
             "OCI_CONFIG_LOCATION", DEFAULT_LOCATION
         )
         self.oci_key_profile = self.oci_key_profile or os.environ.get(
             "OCI_CONFIG_PROFILE", DEFAULT_PROFILE
         )
         self.oci_config = self.oci_config or {}
-        self.oci_signer = self.oci_signer
-        self.oci_signer_callable = self.oci_signer_callable
         self.oci_signer_kwargs = self.oci_signer_kwargs or {}
         self.oci_client_kwargs = self.oci_client_kwargs or {}
 
 
 def set_auth(
     auth: Optional[str] = AuthType.API_KEY,
     oci_config_location: Optional[str] = DEFAULT_LOCATION,
@@ -78,23 +76,22 @@
     config: Optional[Dict] = {},
     signer: Optional[Any] = None,
     signer_callable: Optional[Callable] = None,
     signer_kwargs: Optional[Dict] = {},
     client_kwargs: Optional[Dict] = {},
 ) -> None:
     """
-    Save type of authentication, profile, config location, config (keypair identity) or signer, which will be used
-    when actual creation of config or signer happens.
+    Sets the default authentication type.
 
     Parameters
     ----------
     auth: Optional[str], default 'api_key'
         'api_key', 'resource_principal' or 'instance_principal'. Enable/disable resource principal identity,
          instance principal or keypair identity in a notebook session
-    oci_config_location: Optional[str], default oci.config.DEFAULT_LOCATION, which is '~/.oci/config'
+    oci_config_location: Optional[str], default '~/.oci/config'
         config file location
     profile: Optional[str], default is DEFAULT_PROFILE, which is 'DEFAULT'
          profile name for api keys config file
     config: Optional[Dict], default {}
         created config dictionary
     signer: Optional[Any], default None
         created signer, can be resource principals signer, instance principal signer or other.
@@ -117,18 +114,54 @@
     >>> ads.set_auth("api_key", oci_config_location = "other_config_location") # use non-default oci_config_location
 
     >>> ads.set_auth("api_key", client_kwargs={"timeout": 60}) # default signer with connection and read timeouts set to 60 seconds for the client.
 
     >>> other_config = oci.config.from_file("other_config_location", "OTHER_PROFILE") # Create non-default config
     >>> ads.set_auth(config=other_config) # Set api keys type of authentication based on provided config
 
+    >>> config={
+    ...     user=ocid1.user.oc1..<unique_ID>,
+    ...     fingerprint=<fingerprint>,
+    ...     tenancy=ocid1.tenancy.oc1..<unique_ID>,
+    ...     region=us-ashburn-1,
+    ...     key_content=<private key content>,
+    ... }
+    >>> ads.set_auth(config=config) # Set api key authentication using private key content based on provided config
+
+    >>> config={
+    ...     user=ocid1.user.oc1..<unique_ID>,
+    ...     fingerprint=<fingerprint>,
+    ...     tenancy=ocid1.tenancy.oc1..<unique_ID>,
+    ...     region=us-ashburn-1,
+    ...     key_file=~/.oci/oci_api_key.pem,
+    ... }
+    >>> ads.set_auth(config=config) # Set api key authentication using private key file location based on provided config
+
     >>> ads.set_auth("resource_principal")  # Set resource principal authentication
 
     >>> ads.set_auth("instance_principal")  # Set instance principal authentication
 
+    >>> singer = oci.signer.Signer(
+    ...     user=ocid1.user.oc1..<unique_ID>,
+    ...     fingerprint=<fingerprint>,
+    ...     tenancy=ocid1.tenancy.oc1..<unique_ID>,
+    ...     region=us-ashburn-1,
+    ...     private_key_content=<private key content>,
+    ... )
+    >>> ads.set_auth(singer=singer) # Set api keys authentication with private key content based on provided signer
+
+    >>> singer = oci.signer.Signer(
+    ...     user=ocid1.user.oc1..<unique_ID>,
+    ...     fingerprint=<fingerprint>,
+    ...     tenancy=ocid1.tenancy.oc1..<unique_ID>,
+    ...     region=us-ashburn-1,
+    ...     private_key_file_location=<private key content>,
+    ... )
+    >>> ads.set_auth(singer=singer) # Set api keys authentication with private key file location based on provided signer
+
     >>> singer = oci.auth.signers.get_resource_principals_signer()
     >>> ads.auth.create_signer(config={}, singer=signer) # resource principals authentication dictionary created
 
     >>> signer_callable = oci.auth.signers.ResourcePrincipalsFederationSigner
     >>> ads.set_auth(signer_callable=signer_callable) # Set resource principal federation singer callable
 
     >>> signer_callable = oci.auth.signers.InstancePrincipalsSecurityTokenSigner
@@ -153,41 +186,34 @@
         raise ValueError(
             f"'config' and 'oci_config_location', 'profile' pair are mutually exclusive."
             f"Please specify 'config' OR 'oci_config_location', 'profile' pair."
         )
 
     auth_state.oci_config = config
     auth_state.oci_key_profile = profile
-    if auth == AuthType.API_KEY and not signer and not signer_callable:
-        if os.path.exists(os.path.expanduser(oci_config_location)):
-            auth_state.oci_config_path = oci_config_location
-        else:
-            raise ValueError(
-                f"{oci_config_location} path does not exist, please provide existing path to config file."
-            )
-
+    auth_state.oci_config_path = oci_config_location
     auth_state.oci_signer = signer
     auth_state.oci_signer_callable = signer_callable
     auth_state.oci_signer_kwargs = signer_kwargs
     auth_state.oci_client_kwargs = client_kwargs
 
 
 def api_keys(
-    oci_config: str = os.path.join(os.path.expanduser("~"), ".oci", "config"),
+    oci_config: Union[str, Dict] = os.path.expanduser(DEFAULT_LOCATION),
     profile: str = DEFAULT_PROFILE,
     client_kwargs: Dict = None,
 ) -> Dict:
     """
     Prepares authentication and extra arguments necessary for creating clients for different OCI services using API
     Keys.
 
     Parameters
     ----------
-    oci_config: Optional[str], default is $HOME/.oci/config
-        OCI authentication config file location.
+    oci_config: Optional[Union[str, Dict]], default is ~/.oci/config
+        OCI authentication config file location or a dictionary with config attributes.
     profile: Optional[str], is DEFAULT_PROFILE, which is 'DEFAULT'
         Profile name to select from the config file.
     client_kwargs: Optional[Dict], default None
         kwargs that are required to instantiate the Client if we need to override the defaults.
 
     Returns
     -------
@@ -201,15 +227,18 @@
     Examples
     --------
     >>> from ads.common import oci_client as oc
     >>> auth = ads.auth.api_keys(oci_config="/home/datascience/.oci/config", profile="TEST", client_kwargs={"timeout": 6000})
     >>> oc.OCIClientFactory(**auth).object_storage # Creates Object storage client with timeout set to 6000 using API Key authentication
     """
     signer_args = dict(
-        oci_config_location=oci_config,
+        oci_config=oci_config if isinstance(oci_config, Dict) else {},
+        oci_config_location=oci_config
+        if isinstance(oci_config, str)
+        else os.path.expanduser(DEFAULT_LOCATION),
         oci_key_profile=profile,
         client_kwargs=client_kwargs,
     )
     signer_generator = AuthFactory().signerGenerator(AuthType.API_KEY)
     return signer_generator(signer_args).create_signer()
 
 
@@ -287,14 +316,32 @@
     --------
     >>> import ads
     >>> auth = ads.auth.create_signer() # api_key type of authentication dictionary created with default config location and default profile
 
     >>> config = oci.config.from_file("other_config_location", "OTHER_PROFILE")
     >>> auth = ads.auth.create_signer(config=config) # api_key type of authentication dictionary created based on provided config
 
+    >>> config={
+    ...     user=ocid1.user.oc1..<unique_ID>,
+    ...     fingerprint=<fingerprint>,
+    ...     tenancy=ocid1.tenancy.oc1..<unique_ID>,
+    ...     region=us-ashburn-1,
+    ...     key_content=<private key content>,
+    ... }
+    >>> auth = ads.auth.create_signer(config=config) # api_key type of authentication dictionary with private key content created based on provided config
+
+    >>> config={
+    ...     user=ocid1.user.oc1..<unique_ID>,
+    ...     fingerprint=<fingerprint>,
+    ...     tenancy=ocid1.tenancy.oc1..<unique_ID>,
+    ...     region=us-ashburn-1,
+    ...     key_file=~/.oci/oci_api_key.pem,
+    ... }
+    >>> auth = ads.auth.create_signer(config=config) # api_key type of authentication dictionary with private key file location created based on provided config
+
     >>> singer = oci.auth.signers.get_resource_principals_signer()
     >>> auth = ads.auth.create_signer(config={}, signer=signer) # resource principals authentication dictionary created
 
     >>> auth = ads.auth.create_signer(auth_type='instance_principal') # instance principals authentication dictionary created
 
     >>> signer_callable = oci.auth.signers.InstancePrincipalsSecurityTokenSigner
     >>> signer_kwargs = dict(log_requests=True) # will log the request url and response data when retrieving
@@ -478,16 +525,16 @@
 
     def create_signer(self) -> Dict:
         """
         Creates api keys configuration and signer with extra arguments necessary for creating clients.
         Signer constructed from the `oci_config` provided. If not 'oci_config', configuration will be
         constructed from 'oci_config_location' and 'oci_key_profile' in place.
 
-        Resturns
-        --------
+        Returns
+        -------
         dict
             Contains keys - config, signer and client_kwargs.
 
             - config contains the configuration information
             - signer contains the signer object created. It is instantiated from signer_callable, or
             signer provided in args used, or instantiated in place
             - client_kwargs contains the `client_kwargs` that was passed in as input parameter
@@ -502,23 +549,26 @@
         """
         if self.oci_config:
             configuration = ads.telemetry.update_oci_client_config(self.oci_config)
         else:
             configuration = ads.telemetry.update_oci_client_config(
                 oci.config.from_file(self.oci_config_location, self.oci_key_profile)
             )
+
+        oci.config.validate_config(configuration)
         logger.info(f"Using 'api_key' authentication.")
         return {
             "config": configuration,
             "signer": oci.signer.Signer(
-                configuration["tenancy"],
-                configuration["user"],
-                configuration["fingerprint"],
-                configuration["key_file"],
-                configuration.get("pass_phrase"),
+                tenancy=configuration["tenancy"],
+                user=configuration["user"],
+                fingerprint=configuration["fingerprint"],
+                private_key_file_location=configuration.get("key_file"),
+                pass_phrase= configuration.get("pass_phrase"),
+                private_key_content=configuration.get("key_content")
             ),
             "client_kwargs": self.client_kwargs,
         }
 
 
 class ResourcePrincipal(AuthSignerGenerator):
     """
@@ -540,16 +590,16 @@
         """
         self.client_kwargs = args.get("client_kwargs")
 
     def create_signer(self) -> Dict:
         """
         Creates Resource Principal signer with extra arguments necessary for creating clients.
 
-        Resturns
-        --------
+        Returns
+        -------
         dict
             Contains keys - config, signer and client_kwargs.
 
             - config contains the configuration information
             - signer contains the signer object created. It is instantiated from signer_callable, or
             signer provided in args used, or instantiated in place
             - client_kwargs contains the `client_kwargs` that was passed in as input parameter
@@ -596,16 +646,16 @@
 
     def create_signer(self) -> Dict:
         """
         Creates Instance Principal signer with extra arguments necessary for creating clients.
         Signer instantiated from the `signer_callable` or if the `signer` provided is will be return by this method.
         If `signer_callable` or `signer` not provided new signer will be created in place.
 
-        Resturns
-        --------
+        Returns
+        -------
         dict
             Contains keys - config, signer and client_kwargs.
 
             - config contains the configuration information
             - signer contains the signer object created. It is instantiated from signer_callable, or
             signer provided in args used, or instantiated in place
             - client_kwargs contains the `client_kwargs` that was passed in as input parameter
```

### Comparing `oracle_ads-2.8.4/ads/common/card_identifier.py` & `oracle_ads-2.8.5/ads/common/card_identifier.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/config.py` & `oracle_ads-2.8.5/ads/common/config.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/data.py` & `oracle_ads-2.8.5/ads/common/data.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/decorator/argument_to_case.py` & `oracle_ads-2.8.5/ads/common/decorator/argument_to_case.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/decorator/deprecate.py` & `oracle_ads-2.8.5/ads/common/decorator/deprecate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/decorator/runtime_dependency.py` & `oracle_ads-2.8.5/ads/common/decorator/runtime_dependency.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/decorator/utils.py` & `oracle_ads-2.8.5/ads/common/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/dsc_file_system.py` & `oracle_ads-2.8.5/ads/common/dsc_file_system.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/error.py` & `oracle_ads-2.8.5/ads/common/error.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/extended_enum.py` & `oracle_ads-2.8.5/ads/common/extended_enum.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/function/fn_util.py` & `oracle_ads-2.8.5/ads/common/function/fn_util.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/function/func_conf.yaml` & `oracle_ads-2.8.5/ads/common/function/func_conf.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/ipython.py` & `oracle_ads-2.8.5/ads/common/ipython.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/model.py` & `oracle_ads-2.8.5/ads/common/model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/model_artifact.py` & `oracle_ads-2.8.5/ads/common/model_artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/model_artifact_schema.json` & `oracle_ads-2.8.5/ads/common/model_artifact_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/model_export_util.py` & `oracle_ads-2.8.5/ads/common/model_export_util.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/model_metadata.py` & `oracle_ads-2.8.5/ads/common/model_metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/object_storage_details.py` & `oracle_ads-2.8.5/ads/common/object_storage_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/oci_client.py` & `oracle_ads-2.8.5/ads/common/oci_client.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/oci_datascience.py` & `oracle_ads-2.8.5/ads/common/oci_datascience.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/oci_logging.py` & `oracle_ads-2.8.5/ads/common/oci_logging.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/oci_mixin.py` & `oracle_ads-2.8.5/ads/common/oci_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/oci_resource.py` & `oracle_ads-2.8.5/ads/common/oci_resource.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/serializer.py` & `oracle_ads-2.8.5/ads/common/serializer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/common/utils.py` & `oracle_ads-2.8.5/ads/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 # dimention of np array which can be converted to pd dataframe
 DIMENSION = 2
 
 # declare custom exception class
 
 
-class FileOverwriteError(Exception):   # pragma: no cover
+class FileOverwriteError(Exception):  # pragma: no cover
     pass
 
 
 def get_cpu_count():
     """
     Returns the number of CPUs available on this machine
     """
@@ -1299,14 +1299,16 @@
         Whether to overwrite existing files or not.
     auth: (Dict, optional). Defaults to None.
         The default authentication is set using `ads.set_auth` API. If you need to override the
         default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
         authentication signer and kwargs required to instantiate IdentityClient object.
     chunk_size: (int, optinal). Defaults to `DEFAULT_BUFFER_SIZE`
         How much data can be copied in one iteration.
+    progressbar_description: (str, optinal). Defaults to `"Copying `{uri_src}` to `{uri_dst}`"`.
+        Prefix for the progressbar.
 
     Returns
     -------
     str
         The path to the newly created file.
 
     Raises
```

### Comparing `oracle_ads-2.8.4/ads/common/word_lists.py` & `oracle_ads-2.8.5/ads/common/word_lists.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/config.py` & `oracle_ads-2.8.5/ads/config.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/__init__.py` & `oracle_ads-2.8.5/ads/data_labeling/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/boundingbox.py` & `oracle_ads-2.8.5/ads/data_labeling/boundingbox.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/constants.py` & `oracle_ads-2.8.5/ads/data_labeling/constants.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/data_labeling_service.py` & `oracle_ads-2.8.5/ads/data_labeling/data_labeling_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/interface/reader.py` & `oracle_ads-2.8.5/ads/data_labeling/interface/reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/loader/file_loader.py` & `oracle_ads-2.8.5/ads/data_labeling/loader/file_loader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/metadata.py` & `oracle_ads-2.8.5/ads/data_labeling/metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/mixin/data_labeling.py` & `oracle_ads-2.8.5/ads/data_labeling/mixin/data_labeling.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/ner.py` & `oracle_ads-2.8.5/ads/data_labeling/ner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/parser/dls_record_parser.py` & `oracle_ads-2.8.5/ads/data_labeling/parser/dls_record_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/parser/export_metadata_parser.py` & `oracle_ads-2.8.5/ads/data_labeling/parser/export_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/parser/export_record_parser.py` & `oracle_ads-2.8.5/ads/data_labeling/parser/export_record_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/reader/dataset_reader.py` & `oracle_ads-2.8.5/ads/data_labeling/reader/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/reader/dls_record_reader.py` & `oracle_ads-2.8.5/ads/data_labeling/reader/dls_record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/reader/export_record_reader.py` & `oracle_ads-2.8.5/ads/data_labeling/reader/export_record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/reader/jsonl_reader.py` & `oracle_ads-2.8.5/ads/data_labeling/reader/jsonl_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/reader/metadata_reader.py` & `oracle_ads-2.8.5/ads/data_labeling/reader/metadata_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/reader/record_reader.py` & `oracle_ads-2.8.5/ads/data_labeling/reader/record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/record.py` & `oracle_ads-2.8.5/ads/data_labeling/record.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/visualizer/image_visualizer.py` & `oracle_ads-2.8.5/ads/data_labeling/visualizer/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/data_labeling/visualizer/text_visualizer.py` & `oracle_ads-2.8.5/ads/data_labeling/visualizer/text_visualizer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/database/connection.py` & `oracle_ads-2.8.5/ads/database/connection.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataflow/dataflow.py` & `oracle_ads-2.8.5/ads/dataflow/dataflow.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataflow/dataflowsummary.py` & `oracle_ads-2.8.5/ads/dataflow/dataflowsummary.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/classification_dataset.py` & `oracle_ads-2.8.5/ads/dataset/classification_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/correlation.py` & `oracle_ads-2.8.5/ads/dataset/correlation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/correlation_plot.py` & `oracle_ads-2.8.5/ads/dataset/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/dask_series.py` & `oracle_ads-2.8.5/ads/dataset/dask_series.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/dataframe_transformer.py` & `oracle_ads-2.8.5/ads/dataset/dataframe_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/dataset.py` & `oracle_ads-2.8.5/ads/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             description=description,
             type_discovery=type_discovery,
             types=types,
             metadata=metadata,
             progress=progress,
             transformer_pipeline=transformer_pipeline,
             interactive=interactive,
-            **kwargs
+            **kwargs,
         )
 
     @property
     @deprecated(
         "2.5.2", details="The ddf attribute is deprecated. Use the df attribute."
     )
     def ddf(self):
@@ -1909,7 +1909,47 @@
 
         warningz.value = self._generate_warnings_html(
             is_wide_dataset, n_rows, n_columns, self.df_stats, warningz, accordion
         )
 
         if visualize_features and not is_wide_dataset:
             self._visualize_feature_distribution(features)
+
+    def get_recommendations(self, *args, **kwargs):  # real signature may change
+        """
+        Returns user-friendly error message to set target variable before invoking this API.
+
+        Parameters
+        ----------
+        kwargs
+
+        Returns
+        -------
+        NotImplementedError
+            raises NotImplementedError, if target parameter value not provided
+
+        """
+        raise NotImplementedError(
+            "Please set the target using set_target() before invoking this API. See "
+            "https://accelerated-data-science.readthedocs.io/en/latest/ads.dataset.html#ads.dataset.dataset.ADSDataset.set_target "
+            "for the API usage."
+        )
+
+    def suggest_recommendations(self, *args, **kwargs):  # real signature may change
+        """
+        Returns user-friendly error message to set target variable before invoking this API.
+
+        Parameters
+        ----------
+        kwargs
+
+        Returns
+        -------
+        NotImplementedError
+            raises NotImplementedError, if target parameter value not provided
+
+        """
+        raise NotImplementedError(
+            "Please set the target using set_target() before invoking this API. See "
+            "https://accelerated-data-science.readthedocs.io/en/latest/ads.dataset.html#ads.dataset.dataset.ADSDataset.set_target "
+            "for the API usage."
+        )
```

### Comparing `oracle_ads-2.8.4/ads/dataset/dataset_browser.py` & `oracle_ads-2.8.5/ads/dataset/dataset_browser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/dataset_with_target.py` & `oracle_ads-2.8.5/ads/dataset/dataset_with_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,19 @@
             sampled_df = generate_sample(
                 df,
                 (shape or df.shape)[0],
                 DatasetDefaults.sampling_confidence_level,
                 DatasetDefaults.sampling_confidence_interval,
                 **init_kwargs,
             )
+
+        if target not in df:
+            raise ValueError(
+                f"{target} column doesn't exist in data frame. Specify a valid one instead."
+            )
             
         if target_type is None:
             target_type = get_target_type(target, sampled_df, **init_kwargs)
 
         if len(df[target].dropna()) == 0:
             logger.warning(
                 "It is not recommended to use an empty column as the target variable."
```

### Comparing `oracle_ads-2.8.4/ads/dataset/exception.py` & `oracle_ads-2.8.5/ads/dataset/exception.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/factory.py` & `oracle_ads-2.8.5/ads/dataset/factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/feature_engineering_transformer.py` & `oracle_ads-2.8.5/ads/dataset/feature_engineering_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/feature_selection.py` & `oracle_ads-2.8.5/ads/dataset/feature_selection.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/forecasting_dataset.py` & `oracle_ads-2.8.5/ads/dataset/forecasting_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/helper.py` & `oracle_ads-2.8.5/ads/dataset/helper.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/label_encoder.py` & `oracle_ads-2.8.5/ads/dataset/label_encoder.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/pipeline.py` & `oracle_ads-2.8.5/ads/dataset/pipeline.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/plot.py` & `oracle_ads-2.8.5/ads/dataset/plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/progress.py` & `oracle_ads-2.8.5/ads/dataset/progress.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/recommendation.py` & `oracle_ads-2.8.5/ads/dataset/recommendation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/recommendation_transformer.py` & `oracle_ads-2.8.5/ads/dataset/recommendation_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,22 +249,23 @@
                     target_value_counts.iteritems(), key=lambda k: k[1]
                 )[1]
                 majority_class_len = max(
                     target_value_counts.iteritems(), key=lambda k: k[1]
                 )[1]
                 minor_majority_ratio = minority_class_len / majority_class_len
 
-                # Suggest down sampling if minor_majority_ratio is 1:1000
-                suggested_sampling = (
-                    "Do nothing"
-                    if len(df) <= utils.MAX_LEN_FOR_UP_SAMPLING
-                    else "Down-sample"
-                    if minor_majority_ratio >= utils.MIN_RATIO_FOR_DOWN_SAMPLING
-                    else "Do nothing"
-                )
+                # up-sample if length of dataframe is less than or equal to MAX_LEN_FOR_UP_SAMPLING = 5000
+                # down-sample if minor_majority_ratio is greater than or equal to MIN_RATIO_FOR_DOWN_SAMPLING = 1/20
+                if len(df) <= utils.MAX_LEN_FOR_UP_SAMPLING:
+                    suggested_sampling = "Up-sample"
+                elif minor_majority_ratio >= utils.MIN_RATIO_FOR_DOWN_SAMPLING:
+                    suggested_sampling = "Down-sample"
+                else:
+                    suggested_sampling = "Do nothing"
+
                 self._build_recommendation(
                     recommendations,
                     "fix_imbalance",
                     [self.target_],
                     "Imbalanced Target({0:.2%})".format(minor_majority_ratio),
                     ["Do nothing", "Down-sample", "Up-sample"],
                     suggested_sampling,
```

### Comparing `oracle_ads-2.8.4/ads/dataset/regression_dataset.py` & `oracle_ads-2.8.5/ads/dataset/regression_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/sampled_dataset.py` & `oracle_ads-2.8.5/ads/dataset/sampled_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/target.py` & `oracle_ads-2.8.5/ads/dataset/target.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dataset/timeseries.py` & `oracle_ads-2.8.5/ads/dataset/timeseries.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/dbmixin/db_pandas_accessor.py` & `oracle_ads-2.8.5/ads/dbmixin/db_pandas_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/environment/ml_runtime.py` & `oracle_ads-2.8.5/ads/environment/ml_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/evaluations/__init__.py` & `oracle_ads-2.8.5/ads/evaluations/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/evaluations/evaluation_plot.py` & `oracle_ads-2.8.5/ads/evaluations/evaluation_plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/evaluations/evaluator.py` & `oracle_ads-2.8.5/ads/evaluations/evaluator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/evaluations/statistical_metrics.py` & `oracle_ads-2.8.5/ads/evaluations/statistical_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,28 +194,35 @@
         self.metrics["recall"] = metrics.recall_score(
             self.y_true, self.y_pred, pos_label=self.positive_class
         )
         self.metrics["f1"] = metrics.f1_score(
             self.y_true, self.y_pred, pos_label=self.positive_class, average="binary"
         )
 
-        (
-            self.metrics["false_positive_rate"],
-            self.metrics["true_positive_rate"],
-            _,
-        ) = metrics.roc_curve(self.y_true, self.y_pred, pos_label=self.positive_class)
-        self.metrics["auc"] = metrics.auc(
-            self.metrics["false_positive_rate"], self.metrics["true_positive_rate"]
-        )
-
         if self.y_score is not None:
             if not all(0 >= x >= 1 for x in self.y_score):
                 self.y_score = np.asarray(
                     [0 if x < 0 else 1 if x > 1 else x for x in self.y_score]
                 )
+            if len(np.asarray(self.y_score).shape) > 1: 
+                # If the SKLearn classifier doesn't correctly identify the problem as 
+                # binary classification, y_score may be of shape (n_rows, 2) 
+                # instead of (n_rows,)
+                pos_class_idx = self.classes.index(self.positive_class)
+                positive_class_scores = self.y_score[:, pos_class_idx]
+            else:
+                positive_class_scores = self.y_score
+            (
+                self.metrics["false_positive_rate"],
+                self.metrics["true_positive_rate"],
+                _,
+            ) = metrics.roc_curve(y_true=self.y_true, y_score=positive_class_scores, pos_label=self.positive_class)
+            self.metrics["auc"] = metrics.auc(
+                self.metrics["false_positive_rate"], self.metrics["true_positive_rate"]
+            )
             self.y_score = list(self.y_score)
             self.metrics["youden_j"] = (
                 self.metrics["true_positive_rate"] - self.metrics["false_positive_rate"]
             )
             best_idx = np.argmax(self.metrics["youden_j"])
             self.metrics["roc_best_model_score"] = (
                 self.metrics["false_positive_rate"][best_idx],
```

### Comparing `oracle_ads-2.8.4/ads/explanations/base_explainer.py` & `oracle_ads-2.8.5/ads/explanations/base_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/explanations/explainer.py` & `oracle_ads-2.8.5/ads/explanations/explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/explanations/mlx_global_explainer.py` & `oracle_ads-2.8.5/ads/explanations/mlx_global_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/explanations/mlx_interface.py` & `oracle_ads-2.8.5/ads/explanations/mlx_interface.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/explanations/mlx_local_explainer.py` & `oracle_ads-2.8.5/ads/explanations/mlx_local_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/explanations/mlx_whatif_explainer.py` & `oracle_ads-2.8.5/ads/explanations/mlx_whatif_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/__init__.py` & `oracle_ads-2.8.5/ads/feature_engineering/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/accessor/dataframe_accessor.py` & `oracle_ads-2.8.5/ads/feature_engineering/accessor/dataframe_accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2021, 2022 Oracle and/or its affiliates.
+# Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 """
 The ADS accessor for the Pandas DataFrame.
 The accessor will be initialized with the pandas object the user is interacting with.
 
 Examples
@@ -37,27 +37,32 @@
 
 from typing import Any, Dict, List, Union
 
 import numpy as np
 import pandas as pd
 from ads.common.utils import DATA_SCHEMA_MAX_COL_NUM
 from ads.data_labeling.mixin.data_labeling import DataLabelingAccessMixin
+from ads.dataset.mixin.dataset_accessor import ADSDatasetAccessMixin
 from ads.dbmixin.db_pandas_accessor import DBAccessMixin
 from ads.feature_engineering import schema
 from ads.feature_engineering.accessor.mixin.eda_mixin import EDAMixin
 from ads.feature_engineering.accessor.mixin.feature_types_mixin import (
     ADSFeatureTypesMixin,
 )
 from ads.feature_engineering.feature_type.base import FeatureType
 from pandas.core.dtypes.common import is_list_like
 
 
 @pd.api.extensions.register_dataframe_accessor("ads")
 class ADSDataFrameAccessor(
-    ADSFeatureTypesMixin, EDAMixin, DBAccessMixin, DataLabelingAccessMixin
+    ADSFeatureTypesMixin,
+    EDAMixin,
+    DBAccessMixin,
+    DataLabelingAccessMixin,
+    ADSDatasetAccessMixin
 ):
     """ADS accessor for the Pandas DataFrame.
 
     Attributes
     ----------
     columns: List[str]
         The column labels of the DataFrame.
```

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/correlation.py` & `oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/correlation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/eda_mixin.py` & `oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/eda_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/eda_mixin_series.py` & `oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/eda_mixin_series.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/feature_types_mixin.py` & `oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/feature_types_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/utils.py` & `oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/accessor/series_accessor.py` & `oracle_ads-2.8.5/ads/feature_engineering/accessor/series_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/adsimage/image.py` & `oracle_ads-2.8.5/ads/feature_engineering/adsimage/image.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/adsimage/image_reader.py` & `oracle_ads-2.8.5/ads/feature_engineering/adsimage/image_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/data_schema.json` & `oracle_ads-2.8.5/ads/feature_engineering/data_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/dataset/zip_code_data.py` & `oracle_ads-2.8.5/ads/feature_engineering/dataset/zip_code_data.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/exceptions.py` & `oracle_ads-2.8.5/ads/feature_engineering/exceptions.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/__init__.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/address.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/address.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/oci_language.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/oci_language.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/base.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/string.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/string.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/base.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/boolean.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/boolean.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/category.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/category.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/constant.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/constant.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/continuous.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/continuous.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/creditcard.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/creditcard.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/datetime.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/datetime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/discrete.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/discrete.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/document.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/document.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/gis.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/gis.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/feature_validator.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/feature_validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/feature_warning.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/feature_warning.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/warnings.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/warnings.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/integer.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/integer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address_v4.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address_v4.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address_v6.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address_v6.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/lat_long.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/lat_long.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/object.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/object.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/ordinal.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/ordinal.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/phone_number.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/phone_number.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/string.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/string.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/text.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/text.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/unknown.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/unknown.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type/zip_code.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type/zip_code.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/feature_type_manager.py` & `oracle_ads-2.8.5/ads/feature_engineering/feature_type_manager.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/schema.py` & `oracle_ads-2.8.5/ads/feature_engineering/schema.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/feature_engineering/utils.py` & `oracle_ads-2.8.5/ads/feature_engineering/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/_imports.py` & `oracle_ads-2.8.5/ads/hpo/_imports.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/ads_search_space.py` & `oracle_ads-2.8.5/ads/hpo/ads_search_space.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/distributions.py` & `oracle_ads-2.8.5/ads/hpo/distributions.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/objective.py` & `oracle_ads-2.8.5/ads/hpo/objective.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/search_cv.py` & `oracle_ads-2.8.5/ads/hpo/search_cv.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/stopping_criterion.py` & `oracle_ads-2.8.5/ads/hpo/stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/tuner_artifact.py` & `oracle_ads-2.8.5/ads/hpo/tuner_artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/utils.py` & `oracle_ads-2.8.5/ads/hpo/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/validation.py` & `oracle_ads-2.8.5/ads/hpo/validation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/visualization/_contour.py` & `oracle_ads-2.8.5/ads/hpo/visualization/_contour.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/visualization/_edf.py` & `oracle_ads-2.8.5/ads/hpo/visualization/_edf.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/visualization/_intermediate_values.py` & `oracle_ads-2.8.5/ads/hpo/visualization/_intermediate_values.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/visualization/_optimization_history.py` & `oracle_ads-2.8.5/ads/hpo/visualization/_optimization_history.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/visualization/_parallel_coordinate.py` & `oracle_ads-2.8.5/ads/hpo/visualization/_parallel_coordinate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/hpo/visualization/_param_importances.py` & `oracle_ads-2.8.5/ads/hpo/visualization/_param_importances.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/__init__.py` & `oracle_ads-2.8.5/ads/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/ads_job.py` & `oracle_ads-2.8.5/ads/jobs/ads_job.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/builders/base.py` & `oracle_ads-2.8.5/ads/jobs/builders/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/builders/infrastructure/base.py` & `oracle_ads-2.8.5/ads/jobs/builders/infrastructure/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dataflow.py` & `oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dataflow.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dsc_job.py` & `oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dsc_job.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dsc_job_runtime.py` & `oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dsc_job_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/builders/infrastructure/utils.py` & `oracle_ads-2.8.5/ads/jobs/builders/infrastructure/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/builders/runtimes/artifact.py` & `oracle_ads-2.8.5/ads/jobs/builders/runtimes/artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/builders/runtimes/base.py` & `oracle_ads-2.8.5/ads/jobs/builders/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/builders/runtimes/container_runtime.py` & `oracle_ads-2.8.5/ads/jobs/builders/runtimes/container_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/builders/runtimes/python_runtime.py` & `oracle_ads-2.8.5/ads/jobs/builders/runtimes/python_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/cli.py` & `oracle_ads-2.8.5/ads/jobs/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/env_var_parser.py` & `oracle_ads-2.8.5/ads/jobs/env_var_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/extension.py` & `oracle_ads-2.8.5/ads/jobs/extension.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/schema/infrastructure_schema.json` & `oracle_ads-2.8.5/ads/jobs/schema/infrastructure_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/schema/job_schema.json` & `oracle_ads-2.8.5/ads/jobs/schema/job_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/schema/runtime_schema.json` & `oracle_ads-2.8.5/ads/jobs/schema/runtime_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/schema/validator.py` & `oracle_ads-2.8.5/ads/jobs/schema/validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/serializer.py` & `oracle_ads-2.8.5/ads/jobs/serializer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/templates/driver_notebook.py` & `oracle_ads-2.8.5/ads/jobs/templates/driver_notebook.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/templates/driver_oci.py` & `oracle_ads-2.8.5/ads/jobs/templates/driver_oci.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/templates/driver_python.py` & `oracle_ads-2.8.5/ads/jobs/templates/driver_python.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/templates/driver_utils.py` & `oracle_ads-2.8.5/ads/jobs/templates/driver_utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/jobs/utils.py` & `oracle_ads-2.8.5/ads/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/__init__.py` & `oracle_ads-2.8.5/ads/model/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/artifact.py` & `oracle_ads-2.8.5/ads/model/artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/artifact_downloader.py` & `oracle_ads-2.8.5/ads/model/artifact_downloader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/artifact_uploader.py` & `oracle_ads-2.8.5/ads/model/artifact_uploader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/base_properties.py` & `oracle_ads-2.8.5/ads/model/base_properties.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/common/.model-ignore` & `oracle_ads-2.8.5/ads/model/common/.model-ignore`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/common/utils.py` & `oracle_ads-2.8.5/ads/model/common/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/datascience_model.py` & `oracle_ads-2.8.5/ads/model/datascience_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/deployment/__init__.py` & `oracle_ads-2.8.5/ads/model/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/deployment/common/utils.py` & `oracle_ads-2.8.5/ads/model/deployment/common/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/deployment/model_deployer.py` & `oracle_ads-2.8.5/ads/model/deployment/model_deployer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/deployment/model_deployment.py` & `oracle_ads-2.8.5/ads/model/deployment/model_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         Loads model deployment instance from ocid
     sync()
         Updates the model deployment instance from backend
 
 
     Examples
     --------
-    Build model deployment from builder apis:
+    >>> # Build model deployment from builder apis:
     >>> ds_model_deployment = (ModelDeployment()
     ...    .with_display_name("TestModelDeployment")
     ...    .with_description("Testing the test model deployment")
     ...    .with_freeform_tags(tag1="val1", tag2="val2")
     ...    .with_infrastructure(
     ...        (ModelDeploymentInfrastructure()
     ...        .with_project_id(<project_id>)
@@ -207,15 +207,15 @@
     >>> ds_model_deployment.status
     >>> ds_model_deployment.with_display_name("new name").update()
     >>> ds_model_deployment.deactivate()
     >>> ds_model_deployment.sync()
     >>> ds_model_deployment.list(status="ACTIVE")
     >>> ds_model_deployment.delete()
 
-    Build model deployment from yaml
+    >>> # Build model deployment from yaml
     >>> ds_model_deployment = ModelDeployment.from_yaml(uri=<path_to_yaml>)
     """
 
     _PREFIX = "datascience_model_deployment"
 
     CONST_ID = "id"
     CONST_CREATED_BY = "createdBy"
```

### Comparing `oracle_ads-2.8.4/ads/model/deployment/model_deployment_infrastructure.py` & `oracle_ads-2.8.5/ads/model/deployment/model_deployment_infrastructure.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/deployment/model_deployment_properties.py` & `oracle_ads-2.8.5/ads/model/deployment/model_deployment_properties.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/deployment/model_deployment_runtime.py` & `oracle_ads-2.8.5/ads/model/deployment/model_deployment_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/automl_extractor.py` & `oracle_ads-2.8.5/ads/model/extractor/automl_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/huggingface_extractor.py` & `oracle_ads-2.8.5/ads/model/extractor/huggingface_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/keras_extractor.py` & `oracle_ads-2.8.5/ads/model/extractor/keras_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/lightgbm_extractor.py` & `oracle_ads-2.8.5/ads/model/extractor/lightgbm_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/model_info_extractor.py` & `oracle_ads-2.8.5/ads/model/extractor/model_info_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/model_info_extractor_factory.py` & `oracle_ads-2.8.5/ads/model/extractor/model_info_extractor_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/pytorch_extractor.py` & `oracle_ads-2.8.5/ads/model/extractor/pytorch_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/sklearn_extractor.py` & `oracle_ads-2.8.5/ads/model/extractor/sklearn_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/spark_extractor.py` & `oracle_ads-2.8.5/ads/model/extractor/spark_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/tensorflow_extractor.py` & `oracle_ads-2.8.5/ads/model/extractor/tensorflow_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/extractor/xgboost_extractor.py` & `oracle_ads-2.8.5/ads/model/extractor/xgboost_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/framework/automl_model.py` & `oracle_ads-2.8.5/ads/model/framework/automl_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/framework/huggingface_model.py` & `oracle_ads-2.8.5/ads/model/framework/huggingface_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/framework/lightgbm_model.py` & `oracle_ads-2.8.5/ads/model/framework/lightgbm_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/framework/pytorch_model.py` & `oracle_ads-2.8.5/ads/model/framework/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/framework/sklearn_model.py` & `oracle_ads-2.8.5/ads/model/framework/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/framework/spark_model.py` & `oracle_ads-2.8.5/ads/model/framework/spark_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/framework/tensorflow_model.py` & `oracle_ads-2.8.5/ads/model/framework/tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/framework/xgboost_model.py` & `oracle_ads-2.8.5/ads/model/framework/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/generic_model.py` & `oracle_ads-2.8.5/ads/model/generic_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1986,15 +1986,15 @@
         Deploys a model. The model needs to be saved to the model catalog at first. You can deploy the model
         on either conda or container runtime. The customized runtime allows you to bring your own service container.
         To deploy model on container runtime, make sure to build the container and push it to OCIR.
         For more information, see https://docs.oracle.com/en-us/iaas/data-science/using/mod-dep-byoc.htm.
 
         Example
         -------
-        # This is an example to deploy model on container runtime
+        >>> # This is an example to deploy model on container runtime
         >>> model = GenericModel(estimator=estimator, artifact_dir=tempfile.mkdtemp())
         >>> model.summary_status()
         >>> model.prepare(
         ...     model_file_name="toy_model.pkl",
         ...     ignore_conda_error=True, # set ignore_conda_error=True for container runtime
         ...     force_overwrite=True
         ... )
@@ -2847,18 +2847,19 @@
         """Uploads model artifacts to the provided `uri`.
         The artifacts will be zipped before uploading.
 
         Parameters
         ----------
         uri: str
             The destination location for the model artifacts, which can be a local path or
-            OCI object storage URI.
-            Examples:
+            OCI object storage URI. Examples:
+
             >>> upload_artifact(uri="/some/local/folder/")
             >>> upload_artifact(uri="oci://bucket@namespace/prefix/")
+
         auth: (Dict, optional). Defaults to `None`.
             The default authetication is set using `ads.set_auth` API. If you need to override the
             default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
             authentication signer and kwargs required to instantiate IdentityClient object.
         force_overwrite: bool
             Overwrite target_dir if exists.
         """
```

### Comparing `oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py` & `oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/score.py` & `oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/score.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/model_introspect.py` & `oracle_ads-2.8.5/ads/model/model_introspect.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/model_metadata.py` & `oracle_ads-2.8.5/ads/model/model_metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/model_metadata_mixin.py` & `oracle_ads-2.8.5/ads/model/model_metadata_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/model_properties.py` & `oracle_ads-2.8.5/ads/model/model_properties.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/model_version_set.py` & `oracle_ads-2.8.5/ads/model/model_version_set.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/runtime/env_info.py` & `oracle_ads-2.8.5/ads/model/runtime/env_info.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/runtime/model_deployment_details.py` & `oracle_ads-2.8.5/ads/model/runtime/model_deployment_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/runtime/model_provenance_details.py` & `oracle_ads-2.8.5/ads/model/runtime/model_provenance_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/runtime/runtime_info.py` & `oracle_ads-2.8.5/ads/model/runtime/runtime_info.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/runtime/schemas/model_provenance_schema.yaml` & `oracle_ads-2.8.5/ads/model/runtime/schemas/model_provenance_schema.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/runtime/utils.py` & `oracle_ads-2.8.5/ads/model/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/serde/common.py` & `oracle_ads-2.8.5/ads/model/serde/common.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/serde/model_input.py` & `oracle_ads-2.8.5/ads/model/serde/model_input.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/serde/model_serializer.py` & `oracle_ads-2.8.5/ads/model/serde/model_serializer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/service/oci_datascience_model.py` & `oracle_ads-2.8.5/ads/model/service/oci_datascience_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/service/oci_datascience_model_deployment.py` & `oracle_ads-2.8.5/ads/model/service/oci_datascience_model_deployment.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/service/oci_datascience_model_version_set.py` & `oracle_ads-2.8.5/ads/model/service/oci_datascience_model_version_set.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/model/transformer/onnx_transformer.py` & `oracle_ads-2.8.5/ads/model/transformer/onnx_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/mysqldb/mysql_db.py` & `oracle_ads-2.8.5/ads/mysqldb/mysql_db.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/backend/ads_dataflow.py` & `oracle_ads-2.8.5/ads/opctl/backend/ads_dataflow.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/backend/ads_ml_job.py` & `oracle_ads-2.8.5/ads/opctl/backend/ads_ml_job.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/backend/ads_ml_pipeline.py` & `oracle_ads-2.8.5/ads/opctl/backend/ads_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/backend/ads_model_deployment.py` & `oracle_ads-2.8.5/ads/opctl/backend/ads_model_deployment.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/backend/base.py` & `oracle_ads-2.8.5/ads/opctl/backend/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/backend/local.py` & `oracle_ads-2.8.5/ads/opctl/backend/local.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/cli.py` & `oracle_ads-2.8.5/ads/opctl/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/cmds.py` & `oracle_ads-2.8.5/ads/opctl/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/conda/cli.py` & `oracle_ads-2.8.5/ads/opctl/conda/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/conda/cmds.py` & `oracle_ads-2.8.5/ads/opctl/conda/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/conda/config.yaml` & `oracle_ads-2.8.5/ads/opctl/conda/config.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/conda/multipart_uploader.py` & `oracle_ads-2.8.5/ads/opctl/conda/multipart_uploader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/conda/pack.py` & `oracle_ads-2.8.5/ads/opctl/conda/pack.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/config/base.py` & `oracle_ads-2.8.5/ads/opctl/config/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml` & `oracle_ads-2.8.5/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/config/merger.py` & `oracle_ads-2.8.5/ads/opctl/config/merger.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/config/resolver.py` & `oracle_ads-2.8.5/ads/opctl/config/resolver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/config/utils.py` & `oracle_ads-2.8.5/ads/opctl/config/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/config/validator.py` & `oracle_ads-2.8.5/ads/opctl/config/validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/config/versioner.py` & `oracle_ads-2.8.5/ads/opctl/config/versioner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/base.py` & `oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py` & `oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/constants.py` & `oracle_ads-2.8.5/ads/opctl/constants.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/diagnostics/__main__.py` & `oracle_ads-2.8.5/ads/opctl/diagnostics/__main__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/diagnostics/check_distributed_job_requirements.py` & `oracle_ads-2.8.5/ads/opctl/diagnostics/check_distributed_job_requirements.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/diagnostics/check_requirements.py` & `oracle_ads-2.8.5/ads/opctl/diagnostics/check_requirements.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/distributed/certificates.py` & `oracle_ads-2.8.5/ads/opctl/distributed/certificates.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/distributed/cli.py` & `oracle_ads-2.8.5/ads/opctl/distributed/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/distributed/cmds.py` & `oracle_ads-2.8.5/ads/opctl/distributed/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/distributed/common/abstract_cluster_provider.py` & `oracle_ads-2.8.5/ads/opctl/distributed/common/abstract_cluster_provider.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/distributed/common/abstract_framework_spec_builder.py` & `oracle_ads-2.8.5/ads/opctl/distributed/common/abstract_framework_spec_builder.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_config_helper.py` & `oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_config_helper.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_provider_factory.py` & `oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_provider_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_runner.py` & `oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_runner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/distributed/common/framework_factory.py` & `oracle_ads-2.8.5/ads/opctl/distributed/common/framework_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/docker/Dockerfile` & `oracle_ads-2.8.5/ads/opctl/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.gpu` & `oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.gpu`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.job` & `oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.job`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.job.gpu` & `oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.job.gpu`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/docker/merge_dependencies.py` & `oracle_ads-2.8.5/ads/opctl/docker/merge_dependencies.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/model/cli.py` & `oracle_ads-2.8.5/ads/opctl/model/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/model/cmds.py` & `oracle_ads-2.8.5/ads/opctl/model/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/script.py` & `oracle_ads-2.8.5/ads/opctl/script.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/spark/cli.py` & `oracle_ads-2.8.5/ads/opctl/spark/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/spark/cmds.py` & `oracle_ads-2.8.5/ads/opctl/spark/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/templates/diagnostic_report_template.jinja2` & `oracle_ads-2.8.5/ads/opctl/templates/diagnostic_report_template.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/opctl/utils.py` & `oracle_ads-2.8.5/ads/opctl/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/oracledb/oracle_db.py` & `oracle_ads-2.8.5/ads/oracledb/oracle_db.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/pipeline/__init__.py` & `oracle_ads-2.8.5/ads/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/pipeline/ads_pipeline.py` & `oracle_ads-2.8.5/ads/pipeline/ads_pipeline.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/pipeline/ads_pipeline_run.py` & `oracle_ads-2.8.5/ads/pipeline/ads_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/pipeline/ads_pipeline_step.py` & `oracle_ads-2.8.5/ads/pipeline/ads_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/pipeline/builders/infrastructure/custom_script.py` & `oracle_ads-2.8.5/ads/pipeline/builders/infrastructure/custom_script.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/pipeline/cli.py` & `oracle_ads-2.8.5/ads/pipeline/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/pipeline/extension.py` & `oracle_ads-2.8.5/ads/pipeline/extension.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/pipeline/visualizer/base.py` & `oracle_ads-2.8.5/ads/pipeline/visualizer/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/pipeline/visualizer/graph_renderer.py` & `oracle_ads-2.8.5/ads/pipeline/visualizer/graph_renderer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/pipeline/visualizer/text_renderer.py` & `oracle_ads-2.8.5/ads/pipeline/visualizer/text_renderer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/secrets/adb.py` & `oracle_ads-2.8.5/ads/secrets/adb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/secrets/auth_token.py` & `oracle_ads-2.8.5/ads/secrets/auth_token.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/secrets/big_data_service.py` & `oracle_ads-2.8.5/ads/secrets/big_data_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/secrets/mysqldb.py` & `oracle_ads-2.8.5/ads/secrets/mysqldb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/secrets/oracledb.py` & `oracle_ads-2.8.5/ads/secrets/oracledb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/secrets/secrets.py` & `oracle_ads-2.8.5/ads/secrets/secrets.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/telemetry/telemetry.py` & `oracle_ads-2.8.5/ads/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score-pkl.jinja2` & `oracle_ads-2.8.5/ads/templates/score-pkl.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score.jinja2` & `oracle_ads-2.8.5/ads/templates/score.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_generic.jinja2` & `oracle_ads-2.8.5/ads/templates/score_generic.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_huggingface_pipeline.jinja2` & `oracle_ads-2.8.5/ads/templates/score_huggingface_pipeline.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_lightgbm.jinja2` & `oracle_ads-2.8.5/ads/templates/score_lightgbm.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_onnx.jinja2` & `oracle_ads-2.8.5/ads/templates/score_onnx.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_onnx_new.jinja2` & `oracle_ads-2.8.5/ads/templates/score_onnx_new.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_oracle_automl.jinja2` & `oracle_ads-2.8.5/ads/templates/score_oracle_automl.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_pyspark.jinja2` & `oracle_ads-2.8.5/ads/templates/score_pyspark.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_pytorch.jinja2` & `oracle_ads-2.8.5/ads/templates/score_pytorch.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_scikit-learn.jinja2` & `oracle_ads-2.8.5/ads/templates/score_scikit-learn.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_tensorflow.jinja2` & `oracle_ads-2.8.5/ads/templates/score_tensorflow.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/templates/score_xgboost.jinja2` & `oracle_ads-2.8.5/ads/templates/score_xgboost.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/text_dataset/backends.py` & `oracle_ads-2.8.5/ads/text_dataset/backends.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/text_dataset/dataset.py` & `oracle_ads-2.8.5/ads/text_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/text_dataset/extractor.py` & `oracle_ads-2.8.5/ads/text_dataset/extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/text_dataset/options.py` & `oracle_ads-2.8.5/ads/text_dataset/options.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/text_dataset/udfs.py` & `oracle_ads-2.8.5/ads/text_dataset/udfs.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/text_dataset/utils.py` & `oracle_ads-2.8.5/ads/text_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/abstract_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/abstract_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/constant_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/constant_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/continuous_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/continuous_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/credit_card_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/credit_card_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/datetime_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/datetime_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/discrete_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/discrete_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/document_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/document_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/ip_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/ip_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/latlon_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/latlon_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/phone_number_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/phone_number_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/type_discovery_driver.py` & `oracle_ads-2.8.5/ads/type_discovery/type_discovery_driver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/typed_feature.py` & `oracle_ads-2.8.5/ads/type_discovery/typed_feature.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/unknown_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/unknown_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/type_discovery/zipcode_detector.py` & `oracle_ads-2.8.5/ads/type_discovery/zipcode_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/ads/vault/vault.py` & `oracle_ads-2.8.5/ads/vault/vault.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.4/oracle_ads.egg-info/PKG-INFO` & `oracle_ads-2.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oracle-ads
-Version: 2.8.4
+Name: oracle_ads
+Version: 2.8.5
 Summary: Oracle Accelerated Data Science SDK
 Home-page: https://docs.oracle.com/en-us/iaas/tools/ads-sdk/latest/index.html
 Author: Oracle Data Science
 License: Universal Permissive License 1.0
 Project-URL: Github, https://github.com/oracle/accelerated-data-science
 Project-URL: Documentation, https://accelerated-data-science.readthedocs.io/en/latest/index.html
 Keywords: Oracle Cloud Infrastructure,OCI,Machine Learning,ML,Artificial Intelligence,AI,Data Science,Cloud,Oracle
```

### Comparing `oracle_ads-2.8.4/oracle_ads.egg-info/SOURCES.txt` & `oracle_ads-2.8.5/oracle_ads.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,16 @@
 ads/dataset/progress.py
 ads/dataset/recommendation.py
 ads/dataset/recommendation_transformer.py
 ads/dataset/regression_dataset.py
 ads/dataset/sampled_dataset.py
 ads/dataset/target.py
 ads/dataset/timeseries.py
+ads/dataset/mixin/__init__.py
+ads/dataset/mixin/dataset_accessor.py
 ads/dbmixin/__init__.py
 ads/dbmixin/db_pandas_accessor.py
 ads/environment/__init__.py
 ads/environment/ml_runtime.py
 ads/evaluations/__init__.py
 ads/evaluations/evaluation_plot.py
 ads/evaluations/evaluator.py
@@ -365,18 +367,14 @@
 ads/opctl/docker/merge_dependencies.py
 ads/opctl/model/__init__.py
 ads/opctl/model/cli.py
 ads/opctl/model/cmds.py
 ads/opctl/spark/__init__.py
 ads/opctl/spark/cli.py
 ads/opctl/spark/cmds.py
-ads/opctl/spec/__init__.py
-ads/opctl/spec/abstract_operator_spec.py
-ads/opctl/spec/operator_spec_factory.py
-ads/opctl/spec/utils.py
 ads/opctl/templates/diagnostic_report_template.jinja2
 ads/oracledb/__init__.py
 ads/oracledb/oracle_db.py
 ads/pipeline/__init__.py
 ads/pipeline/ads_pipeline.py
 ads/pipeline/ads_pipeline_run.py
 ads/pipeline/ads_pipeline_step.py
```

### Comparing `oracle_ads-2.8.4/oracle_ads.egg-info/requires.txt` & `oracle_ads-2.8.5/oracle_ads.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 cerberus>=1.3.4
 cloudpickle>=1.6.0
 fsspec>=0.8.7
 jinja2>=2.11.2
 gitpython>=3.1.2
 matplotlib>=3.1.3
 numpy>=1.19.2
-oci>=2.96.0
+oci>=2.102.0
 ocifs>=1.1.3
 pandas<1.6,>1.2.1
 python_jsonschema_objects>=0.3.13
 PyYAML<6,>=5.4
 requests
 scikit-learn<1.2,>=0.23.2
 tabulate>=0.8.9
```

### Comparing `oracle_ads-2.8.4/setup.py` & `oracle_ads-2.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "cerberus>=1.3.4",
     "cloudpickle>=1.6.0",
     "fsspec>=0.8.7",
     "jinja2>=2.11.2",
     "gitpython>=3.1.2",
     "matplotlib>=3.1.3",
     "numpy>=1.19.2",
-    "oci>=2.96.0",
+    "oci>=2.102.0",
     "ocifs>=1.1.3",
     "pandas>1.2.1,<1.6",
     "python_jsonschema_objects>=0.3.13",
     "PyYAML>=5.4,<6",
     "requests",
     "scikit-learn>=0.23.2,<1.2",
     "tabulate>=0.8.9",
```

