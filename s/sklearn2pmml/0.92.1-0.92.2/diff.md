# Comparing `tmp/sklearn2pmml-0.92.1.tar.gz` & `tmp/sklearn2pmml-0.92.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sklearn2pmml-0.92.1.tar", last modified: Mon May  1 06:30:20 2023, max compression
+gzip compressed data, was "dist/sklearn2pmml-0.92.2.tar", last modified: Wed May 17 06:59:33 2023, max compression
```

## Comparing `sklearn2pmml-0.92.1.tar` & `sklearn2pmml-0.92.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.1/setup.cfg
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.1/LICENSE.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-03-03 19:54:54.000000 sklearn2pmml-0.92.1/setup.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/PKG-INFO
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2022-11-15 10:41:18.000000 sklearn2pmml-0.92.1/sklearn2pmml/h2o.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/ruleset/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-02-25 19:29:33.000000 sklearn2pmml-0.92.1/sklearn2pmml/ruleset/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/pipeline/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2022-12-20 20:55:09.000000 sklearn2pmml-0.92.1/sklearn2pmml/pipeline/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-04-30 07:17:22.000000 sklearn2pmml-0.92.1/sklearn2pmml/tpot.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    11627 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.1/sklearn2pmml/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/decoration/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16904 2023-01-03 17:06:18.000000 sklearn2pmml-0.92.1/sklearn2pmml/decoration/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/neural_network/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2022-12-11 13:16:56.000000 sklearn2pmml-0.92.1/sklearn2pmml/neural_network/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2022-12-07 19:44:36.000000 sklearn2pmml-0.92.1/sklearn2pmml/pycaret.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/util/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-04-29 08:24:42.000000 sklearn2pmml-0.92.1/sklearn2pmml/util/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-01-30 14:56:55.000000 sklearn2pmml-0.92.1/sklearn2pmml/xgboost.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_extraction/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_extraction/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_extraction/text/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2021-01-09 09:21:36.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_extraction/text/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/ensemble/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     9179 2023-02-25 19:29:33.000000 sklearn2pmml-0.92.1/sklearn2pmml/ensemble/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     3237 2023-03-15 18:26:47.000000 sklearn2pmml-0.92.1/sklearn2pmml/statsmodels.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_selection/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2022-04-01 09:50:44.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_selection/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/postprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1628 2022-12-11 13:56:03.000000 sklearn2pmml-0.92.1/sklearn2pmml/postprocessing/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5098 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6333 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2020-07-25 07:02:00.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7976 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jcommander-1.72.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    84321 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-model-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    54279 2022-06-05 15:53:19.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pickle-1.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7312 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   432826 2023-05-01 06:26:58.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-converter-1.5.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/guava-21.0.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    27449 2023-03-28 18:11:11.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-statsmodels-1.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   466289 2023-04-01 19:15:11.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/ubjson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   198275 2023-03-11 19:58:17.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-python-1.1.14.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    46362 2022-08-31 13:41:52.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-h2o-1.2.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-05-01 06:28:14.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/classpath.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-05-01 06:26:58.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5703 2023-05-01 06:28:15.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    68186 2022-08-31 09:48:33.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-lightgbm-1.4.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/serpent-1.40.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/gson-2.10.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-05-01 06:28:05.000000 sklearn2pmml-0.92.1/sklearn2pmml/metadata.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2022-04-15 15:03:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/h2o.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16202 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/xgboost.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/lightgbm.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/tree/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2022-12-19 19:21:40.000000 sklearn2pmml-0.92.1/sklearn2pmml/tree/chaid.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2022-06-06 08:17:18.000000 sklearn2pmml-0.92.1/sklearn2pmml/tree/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/expression/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-03-03 19:54:59.000000 sklearn2pmml-0.92.1/sklearn2pmml/expression/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.2/setup.cfg
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.2/LICENSE.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-03-03 19:54:54.000000 sklearn2pmml-0.92.2/setup.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/PKG-INFO
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2022-11-15 10:41:18.000000 sklearn2pmml-0.92.2/sklearn2pmml/h2o.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/ruleset/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-02-25 19:29:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/ruleset/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/pipeline/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2022-12-20 20:55:09.000000 sklearn2pmml-0.92.2/sklearn2pmml/pipeline/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-04-30 07:17:22.000000 sklearn2pmml-0.92.2/sklearn2pmml/tpot.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    11627 2023-05-17 05:52:06.000000 sklearn2pmml-0.92.2/sklearn2pmml/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/decoration/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16904 2023-01-03 17:06:18.000000 sklearn2pmml-0.92.2/sklearn2pmml/decoration/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/neural_network/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2022-12-11 13:16:56.000000 sklearn2pmml-0.92.2/sklearn2pmml/neural_network/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2022-12-07 19:44:36.000000 sklearn2pmml-0.92.2/sklearn2pmml/pycaret.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/util/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-04-29 08:24:42.000000 sklearn2pmml-0.92.2/sklearn2pmml/util/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-01-30 14:56:55.000000 sklearn2pmml-0.92.2/sklearn2pmml/xgboost.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_extraction/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_extraction/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_extraction/text/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2021-01-09 09:21:36.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_extraction/text/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/ensemble/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     9179 2023-02-25 19:29:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/ensemble/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     3237 2023-03-15 18:26:47.000000 sklearn2pmml-0.92.2/sklearn2pmml/statsmodels.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_selection/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2022-04-01 09:50:44.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_selection/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/postprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1628 2022-12-11 13:56:03.000000 sklearn2pmml-0.92.2/sklearn2pmml/postprocessing/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jaxb-core-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     5099 2023-05-17 06:50:31.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.28.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2020-07-25 07:02:00.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/slf4j-api-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jcommander-1.72.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-model-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    54279 2022-06-05 15:53:19.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pickle-1.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   432826 2023-05-01 06:26:58.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-converter-1.5.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7977 2023-05-17 06:50:31.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.28.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/guava-21.0.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    27449 2023-03-28 18:11:11.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-statsmodels-1.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/ubjson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   198275 2023-03-11 19:58:17.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-python-1.1.14.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   466641 2023-05-17 06:50:30.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-1.7.28.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    46362 2022-08-31 13:41:52.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-h2o-1.2.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    84308 2023-05-17 06:50:30.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-extension-1.7.28.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-05-17 06:56:56.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/classpath.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-05-01 06:26:58.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     5703 2023-05-17 06:56:57.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6332 2023-05-17 06:50:31.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.28.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/serpent-1.40.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7312 2023-05-17 06:50:31.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.28.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/gson-2.10.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-05-17 06:56:45.000000 sklearn2pmml-0.92.2/sklearn2pmml/metadata.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2022-04-15 15:03:20.000000 sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/h2o.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16202 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/xgboost.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/lightgbm.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/tree/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2022-12-19 19:21:40.000000 sklearn2pmml-0.92.2/sklearn2pmml/tree/chaid.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2022-06-06 08:17:18.000000 sklearn2pmml-0.92.2/sklearn2pmml/tree/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/expression/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-03-03 19:54:59.000000 sklearn2pmml-0.92.2/sklearn2pmml/expression/__init__.py
```

### Comparing `sklearn2pmml-0.92.1/LICENSE.txt` & `sklearn2pmml-0.92.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/setup.py` & `sklearn2pmml-0.92.2/setup.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/PKG-INFO` & `sklearn2pmml-0.92.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sklearn2pmml
-Version: 0.92.1
+Version: 0.92.2
 Summary: Python library for converting Scikit-Learn pipelines to PMML
 Home-page: https://github.com/jpmml/sklearn2pmml
 Author: Villu Ruusmann
 Author-email: villu.ruusmann@gmail.com
 License: GNU Affero General Public License (AGPL) version 3.0
-Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.92.1.tar.gz
+Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.92.2.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/h2o.py` & `sklearn2pmml-0.92.2/sklearn2pmml/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/ruleset/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/pipeline/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/tpot.py` & `sklearn2pmml-0.92.2/sklearn2pmml/tpot.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,25 +345,25 @@
 
 	"""
 	mapping = dict()
 	processor = lambda x: mapping.update(_expand_mapping(_parse_properties(x.readlines())))
 	_process_classpath("META-INF/sklearn2pmml.properties", processor, user_classpath)
 	return mapping
 
-def make_class_mapping_jar(path, mapping):
+def make_class_mapping_jar(mapping, path):
 	"""Generates a class mapping JAR file.
 
 	Parameters:
 	----------
-	path: string
-		The path to output JAR file.
-
 	mapping: dict of strings
 		Mapping from Python class names to Java converter class names.
 
+	path: string
+		The path to output JAR file.
+
 	"""
 	lines = _format_properties(mapping)
 
 	with ZipFile(path, mode = "w") as zipfile:
 		zipfile.writestr("META-INF/sklearn2pmml.properties", "".join(lines))
 
 def _strip_module(name):
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/decoration/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/decoration/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/neural_network/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/neural_network/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/pycaret.py` & `sklearn2pmml-0.92.2/sklearn2pmml/pycaret.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/util/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/xgboost.py` & `sklearn2pmml-0.92.2/sklearn2pmml/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/feature_extraction/text/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/feature_extraction/text/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/ensemble/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/statsmodels.py` & `sklearn2pmml-0.92.2/sklearn2pmml/statsmodels.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/feature_selection/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/postprocessing/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/jaxb-core-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.27.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.28.jar`

 * *Files 25% similar despite different names*

#### zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 5098 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Apr-01 22:15 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/statsmodels/
--rw-rw-r--  2.0 unx       96 b- defN 23-Apr-01 22:15 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     1515 b- defN 23-Apr-01 22:15 sklearn2pmml/statsmodels/StatsModelsClassifier.class
--rw-rw-r--  2.0 unx     1920 b- defN 23-Apr-01 22:15 sklearn2pmml/statsmodels/StatsModelsUtil.class
--rw-rw-r--  2.0 unx     1511 b- defN 23-Apr-01 22:15 sklearn2pmml/statsmodels/StatsModelsRegressor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
--rw-rw-r--  2.0 unx     1331 b- defN 23-Apr-01 22:14 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
--rw-rw-r--  2.0 unx      120 b- defN 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
-13 files, 6623 bytes uncompressed, 3170 bytes compressed:  52.1%
+Zip file size: 5099 bytes, number of entries: 13
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/statsmodels/
+-rw-rw-r--  2.0 unx       96 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     1515 b- defN 23-May-17 09:50 sklearn2pmml/statsmodels/StatsModelsClassifier.class
+-rw-rw-r--  2.0 unx     1920 b- defN 23-May-17 09:50 sklearn2pmml/statsmodels/StatsModelsUtil.class
+-rw-rw-r--  2.0 unx     1511 b- defN 23-May-17 09:50 sklearn2pmml/statsmodels/StatsModelsRegressor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
+-rw-rw-r--  2.0 unx     1331 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
+-rw-rw-r--  2.0 unx      120 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
+13 files, 6623 bytes uncompressed, 3171 bytes compressed:  52.1%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.27</version>
+    <version>1.7.28</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-statsmodels</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn StatsModels converter</name>
   <description>JPMML Scikit-Learn StatsModels to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sat Apr 01 22:15:12 EEST 2023
-version=1.7.27
+#Wed May 17 09:50:31 EEST 2023
+version=1.7.28
 groupId=org.jpmml
 artifactId=pmml-sklearn-statsmodels
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.27.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.28.jar`

 * *Files 22% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 6333 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Apr-01 22:15 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 h2o/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 h2o/estimators/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/preprocessing/h2o/
--rw-rw-r--  2.0 unx      679 b- defN 23-Apr-01 22:15 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     5710 b- defN 23-Apr-01 22:15 h2o/estimators/H2OEstimator.class
--rw-rw-r--  2.0 unx     1694 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
--rw-rw-r--  2.0 unx     1305 b- defN 23-Apr-01 22:14 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
--rw-rw-r--  2.0 unx      112 b- defN 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
-15 files, 9630 bytes uncompressed, 4317 bytes compressed:  55.2%
+Zip file size: 6332 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 h2o/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 h2o/estimators/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/preprocessing/h2o/
+-rw-rw-r--  2.0 unx      679 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     5710 b- defN 23-May-17 09:50 h2o/estimators/H2OEstimator.class
+-rw-rw-r--  2.0 unx     1694 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
+-rw-rw-r--  2.0 unx     1305 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
+-rw-rw-r--  2.0 unx      112 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
+15 files, 9630 bytes uncompressed, 4316 bytes compressed:  55.2%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.27</version>
+    <version>1.7.28</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-h2o</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn H2O.ai converter</name>
   <description>JPMML Scikit-Learn H2O.ai to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sat Apr 01 22:15:12 EEST 2023
-version=1.7.27
+#Wed May 17 09:50:31 EEST 2023
+version=1.7.28
 groupId=org.jpmml
 artifactId=pmml-sklearn-h2o
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.27.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.28.jar`

 * *Files 19% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7976 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Apr-01 22:15 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 xgboost/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 xgboost/sklearn/
--rw-rw-r--  2.0 unx      364 b- defN 23-Apr-01 22:15 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      168 b- defN 23-Apr-01 22:15 xgboost/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     2270 b- defN 23-Apr-01 22:15 xgboost/sklearn/XGBClassifier.class
--rw-rw-r--  2.0 unx     2210 b- defN 23-Apr-01 22:15 xgboost/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2246 b- defN 23-Apr-01 22:15 xgboost/sklearn/XGBRegressor.class
--rw-rw-r--  2.0 unx     4204 b- defN 23-Apr-01 22:15 xgboost/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
--rw-rw-r--  2.0 unx     1453 b- defN 23-Apr-01 22:14 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
--rw-rw-r--  2.0 unx      116 b- defN 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
-15 files, 13161 bytes uncompressed, 5920 bytes compressed:  55.0%
+Zip file size: 7977 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 xgboost/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 xgboost/sklearn/
+-rw-rw-r--  2.0 unx      364 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      168 b- defN 23-May-17 09:50 xgboost/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2270 b- defN 23-May-17 09:50 xgboost/sklearn/XGBClassifier.class
+-rw-rw-r--  2.0 unx     2210 b- defN 23-May-17 09:50 xgboost/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2246 b- defN 23-May-17 09:50 xgboost/sklearn/XGBRegressor.class
+-rw-rw-r--  2.0 unx     4204 b- defN 23-May-17 09:50 xgboost/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
+-rw-rw-r--  2.0 unx     1453 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
+-rw-rw-r--  2.0 unx      116 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
+15 files, 13161 bytes uncompressed, 5921 bytes compressed:  55.0%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.27</version>
+    <version>1.7.28</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-xgboost</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn XGBoost converter</name>
   <description>JPMML Scikit-Learn XGBoost to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sat Apr 01 22:15:12 EEST 2023
-version=1.7.27
+#Wed May 17 09:50:31 EEST 2023
+version=1.7.28
 groupId=org.jpmml
 artifactId=pmml-sklearn-xgboost
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/slf4j-api-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/jackson-annotations-2.13.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/jcommander-1.72.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/jcommander-1.72.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.27.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-extension-1.7.28.jar`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,69 +1,69 @@
-Zip file size: 84321 bytes, number of entries: 67
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Apr-01 22:15 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 mlxtend/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 mlxtend/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 pycaret/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 pycaret/preprocess/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 tpot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 tpot/builtins/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 optbinning/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 optbinning/scorecard/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 imblearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 category_encoders/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklego/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklego/meta/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklego/preprocessing/
--rw-rw-r--  2.0 unx      913 b- defN 23-Apr-01 22:15 mlxtend/preprocessing/DenseTransformer.class
--rw-rw-r--  2.0 unx     4244 b- defN 23-Apr-01 22:15 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      898 b- defN 23-Apr-01 22:15 pycaret/preprocess/FixImbalancer.class
--rw-rw-r--  2.0 unx     2818 b- defN 23-Apr-01 22:15 pycaret/preprocess/RemoveMulticollinearity.class
--rw-rw-r--  2.0 unx      907 b- defN 23-Apr-01 22:15 pycaret/preprocess/CleanColumnNames.class
--rw-rw-r--  2.0 unx     4017 b- defN 23-Apr-01 22:15 pycaret/preprocess/RareCategoryGrouping.class
--rw-rw-r--  2.0 unx     7434 b- defN 23-Apr-01 22:15 pycaret/preprocess/TransformerWrapper.class
--rw-rw-r--  2.0 unx     4951 b- defN 23-Apr-01 22:15 pycaret/preprocess/TransformerWrapperWithInverse.class
--rw-rw-r--  2.0 unx      720 b- defN 23-Apr-01 22:15 tpot/builtins/StackingEstimator$1.class
--rw-rw-r--  2.0 unx     4530 b- defN 23-Apr-01 22:15 tpot/builtins/StackingEstimator.class
--rw-rw-r--  2.0 unx     2433 b- defN 23-Apr-01 22:15 optbinning/BinnedFeature.class
--rw-rw-r--  2.0 unx     8560 b- defN 23-Apr-01 22:15 optbinning/scorecard/Scorecard.class
--rw-rw-r--  2.0 unx     2133 b- defN 23-Apr-01 22:15 optbinning/OptimalBinningUtil.class
--rw-rw-r--  2.0 unx     6372 b- defN 23-Apr-01 22:15 optbinning/BinningProcess.class
--rw-rw-r--  2.0 unx     2274 b- defN 23-Apr-01 22:15 optbinning/ContinuousOptimalBinning.class
--rw-rw-r--  2.0 unx     3917 b- defN 23-Apr-01 22:15 optbinning/MulticlassOptimalBinning.class
--rw-rw-r--  2.0 unx     1242 b- defN 23-Apr-01 22:15 optbinning/BinningProcess$1.class
--rw-rw-r--  2.0 unx    14050 b- defN 23-Apr-01 22:15 optbinning/OptimalBinning.class
--rw-rw-r--  2.0 unx      860 b- defN 23-Apr-01 22:15 imblearn/Sampler.class
--rw-rw-r--  2.0 unx     1916 b- defN 23-Apr-01 22:15 category_encoders/MapEncoder.class
--rw-rw-r--  2.0 unx     8449 b- defN 23-Apr-01 22:15 category_encoders/MapFeature.class
--rw-rw-r--  2.0 unx      527 b- defN 23-Apr-01 22:15 category_encoders/TargetEncoder.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Apr-01 22:15 category_encoders/CountEncoder$1.class
--rw-rw-r--  2.0 unx      515 b- defN 23-Apr-01 22:15 category_encoders/WOEEncoder.class
--rw-rw-r--  2.0 unx     9124 b- defN 23-Apr-01 22:15 category_encoders/MeanEncoder.class
--rw-rw-r--  2.0 unx     8520 b- defN 23-Apr-01 22:15 category_encoders/CountEncoder.class
--rw-rw-r--  2.0 unx    12815 b- defN 23-Apr-01 22:15 category_encoders/BaseNFeature.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-Apr-01 22:15 category_encoders/MeanEncoder$2.class
--rw-rw-r--  2.0 unx     1481 b- defN 23-Apr-01 22:15 category_encoders/OrdinalMapEncoder$1.class
--rw-rw-r--  2.0 unx     1445 b- defN 23-Apr-01 22:15 category_encoders/MeanEncoder$1.class
--rw-rw-r--  2.0 unx     2119 b- defN 23-Apr-01 22:15 category_encoders/OrdinalEncoder$Mapping.class
--rw-rw-r--  2.0 unx     1323 b- defN 23-Apr-01 22:15 category_encoders/LeaveOneOutEncoder$1.class
--rw-rw-r--  2.0 unx     7967 b- defN 23-Apr-01 22:15 category_encoders/OrdinalMapEncoder.class
--rw-rw-r--  2.0 unx     9241 b- defN 23-Apr-01 22:15 category_encoders/BaseNEncoder.class
--rw-rw-r--  2.0 unx     1334 b- defN 23-Apr-01 22:15 category_encoders/BinaryEncoder.class
--rw-rw-r--  2.0 unx     3547 b- defN 23-Apr-01 22:15 category_encoders/OneHotEncoder.class
--rw-rw-r--  2.0 unx     1325 b- defN 23-Apr-01 22:15 category_encoders/CatBoostEncoder.class
--rw-rw-r--  2.0 unx     2062 b- defN 23-Apr-01 22:15 category_encoders/CategoryEncoderUtil.class
--rw-rw-r--  2.0 unx     1564 b- defN 23-Apr-01 22:15 category_encoders/OrdinalEncoder$1.class
--rw-rw-r--  2.0 unx     1047 b- defN 23-Apr-01 22:15 category_encoders/LeaveOneOutEncoder.class
--rw-rw-r--  2.0 unx     4690 b- defN 23-Apr-01 22:15 category_encoders/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      742 b- defN 23-Apr-01 22:15 category_encoders/MeanEncoder$MeanFunction.class
--rw-rw-r--  2.0 unx     1378 b- defN 23-Apr-01 22:15 category_encoders/CatBoostEncoder$1.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Apr-01 22:15 category_encoders/CategoryEncoder.class
--rw-rw-r--  2.0 unx      725 b- defN 23-Apr-01 22:15 sklego/meta/EstimatorTransformer$1.class
--rw-rw-r--  2.0 unx     7306 b- defN 23-Apr-01 22:15 sklego/meta/EstimatorTransformer.class
--rw-rw-r--  2.0 unx      920 b- defN 23-Apr-01 22:15 sklego/preprocessing/IdentityTransformer.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn-extension/
--rw-rw-r--  2.0 unx     1226 b- defN 23-Apr-01 22:14 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
--rw-rw-r--  2.0 unx      118 b- defN 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
-67 files, 171565 bytes uncompressed, 74755 bytes compressed:  56.4%
+Zip file size: 84308 bytes, number of entries: 67
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 mlxtend/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 mlxtend/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 pycaret/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 pycaret/preprocess/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 tpot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 tpot/builtins/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 optbinning/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 optbinning/scorecard/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 imblearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 category_encoders/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklego/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklego/meta/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklego/preprocessing/
+-rw-rw-r--  2.0 unx      913 b- defN 23-May-17 09:50 mlxtend/preprocessing/DenseTransformer.class
+-rw-rw-r--  2.0 unx     4244 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      898 b- defN 23-May-17 09:50 pycaret/preprocess/FixImbalancer.class
+-rw-rw-r--  2.0 unx     2818 b- defN 23-May-17 09:50 pycaret/preprocess/RemoveMulticollinearity.class
+-rw-rw-r--  2.0 unx      907 b- defN 23-May-17 09:50 pycaret/preprocess/CleanColumnNames.class
+-rw-rw-r--  2.0 unx     4017 b- defN 23-May-17 09:50 pycaret/preprocess/RareCategoryGrouping.class
+-rw-rw-r--  2.0 unx     7434 b- defN 23-May-17 09:50 pycaret/preprocess/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     4951 b- defN 23-May-17 09:50 pycaret/preprocess/TransformerWrapperWithInverse.class
+-rw-rw-r--  2.0 unx      720 b- defN 23-May-17 09:50 tpot/builtins/StackingEstimator$1.class
+-rw-rw-r--  2.0 unx     4530 b- defN 23-May-17 09:50 tpot/builtins/StackingEstimator.class
+-rw-rw-r--  2.0 unx     2433 b- defN 23-May-17 09:50 optbinning/BinnedFeature.class
+-rw-rw-r--  2.0 unx     8560 b- defN 23-May-17 09:50 optbinning/scorecard/Scorecard.class
+-rw-rw-r--  2.0 unx     2133 b- defN 23-May-17 09:50 optbinning/OptimalBinningUtil.class
+-rw-rw-r--  2.0 unx     6372 b- defN 23-May-17 09:50 optbinning/BinningProcess.class
+-rw-rw-r--  2.0 unx     2274 b- defN 23-May-17 09:50 optbinning/ContinuousOptimalBinning.class
+-rw-rw-r--  2.0 unx     3917 b- defN 23-May-17 09:50 optbinning/MulticlassOptimalBinning.class
+-rw-rw-r--  2.0 unx     1242 b- defN 23-May-17 09:50 optbinning/BinningProcess$1.class
+-rw-rw-r--  2.0 unx    14050 b- defN 23-May-17 09:50 optbinning/OptimalBinning.class
+-rw-rw-r--  2.0 unx      860 b- defN 23-May-17 09:50 imblearn/Sampler.class
+-rw-rw-r--  2.0 unx     1916 b- defN 23-May-17 09:50 category_encoders/MapEncoder.class
+-rw-rw-r--  2.0 unx     8449 b- defN 23-May-17 09:50 category_encoders/MapFeature.class
+-rw-rw-r--  2.0 unx      527 b- defN 23-May-17 09:50 category_encoders/TargetEncoder.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-May-17 09:50 category_encoders/CountEncoder$1.class
+-rw-rw-r--  2.0 unx      515 b- defN 23-May-17 09:50 category_encoders/WOEEncoder.class
+-rw-rw-r--  2.0 unx     9124 b- defN 23-May-17 09:50 category_encoders/MeanEncoder.class
+-rw-rw-r--  2.0 unx     8520 b- defN 23-May-17 09:50 category_encoders/CountEncoder.class
+-rw-rw-r--  2.0 unx    12815 b- defN 23-May-17 09:50 category_encoders/BaseNFeature.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-May-17 09:50 category_encoders/MeanEncoder$2.class
+-rw-rw-r--  2.0 unx     1481 b- defN 23-May-17 09:50 category_encoders/OrdinalMapEncoder$1.class
+-rw-rw-r--  2.0 unx     1445 b- defN 23-May-17 09:50 category_encoders/MeanEncoder$1.class
+-rw-rw-r--  2.0 unx     2119 b- defN 23-May-17 09:50 category_encoders/OrdinalEncoder$Mapping.class
+-rw-rw-r--  2.0 unx     1323 b- defN 23-May-17 09:50 category_encoders/LeaveOneOutEncoder$1.class
+-rw-rw-r--  2.0 unx     7967 b- defN 23-May-17 09:50 category_encoders/OrdinalMapEncoder.class
+-rw-rw-r--  2.0 unx     9241 b- defN 23-May-17 09:50 category_encoders/BaseNEncoder.class
+-rw-rw-r--  2.0 unx     1334 b- defN 23-May-17 09:50 category_encoders/BinaryEncoder.class
+-rw-rw-r--  2.0 unx     3547 b- defN 23-May-17 09:50 category_encoders/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     1325 b- defN 23-May-17 09:50 category_encoders/CatBoostEncoder.class
+-rw-rw-r--  2.0 unx     2062 b- defN 23-May-17 09:50 category_encoders/CategoryEncoderUtil.class
+-rw-rw-r--  2.0 unx     1564 b- defN 23-May-17 09:50 category_encoders/OrdinalEncoder$1.class
+-rw-rw-r--  2.0 unx     1047 b- defN 23-May-17 09:50 category_encoders/LeaveOneOutEncoder.class
+-rw-rw-r--  2.0 unx     4690 b- defN 23-May-17 09:50 category_encoders/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      742 b- defN 23-May-17 09:50 category_encoders/MeanEncoder$MeanFunction.class
+-rw-rw-r--  2.0 unx     1378 b- defN 23-May-17 09:50 category_encoders/CatBoostEncoder$1.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-May-17 09:50 category_encoders/CategoryEncoder.class
+-rw-rw-r--  2.0 unx      725 b- defN 23-May-17 09:50 sklego/meta/EstimatorTransformer$1.class
+-rw-rw-r--  2.0 unx     7272 b- defN 23-May-17 09:50 sklego/meta/EstimatorTransformer.class
+-rw-rw-r--  2.0 unx      920 b- defN 23-May-17 09:50 sklego/preprocessing/IdentityTransformer.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-extension/
+-rw-rw-r--  2.0 unx     1226 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
+-rw-rw-r--  2.0 unx      118 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
+67 files, 171531 bytes uncompressed, 74742 bytes compressed:  56.4%
```

#### sklego/meta/EstimatorTransformer.class

##### procyon -ec {}

```diff
@@ -10,15 +10,15 @@
 import org.jpmml.converter.TypeUtil;
 import org.dmg.pmml.DataType;
 import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.ResultFeature;
 import org.dmg.pmml.DerivedField;
 import com.google.common.collect.Iterables;
 import org.jpmml.converter.ContinuousFeature;
-import sklearn.isotonic.IsotonicRegression;
+import sklearn.Calibrator;
 import org.dmg.pmml.OutputField;
 import org.dmg.pmml.Output;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import sklearn.EstimatorUtil;
 import sklearn.tree.HasTreeOptions;
 import org.jpmml.sklearn.SkLearnEncoder;
@@ -116,15 +116,15 @@
             default: {
                 throw new IllegalArgumentException(predictFunc);
             }
         }
     }
     
     private List<Feature> encodePostProcessor(List<Feature> features, final SkLearnEncoder encoder) {
-        final IsotonicRegression estimator = (IsotonicRegression)this.getEstimator((Class<? extends IsotonicRegression>)IsotonicRegression.class);
+        final Calibrator estimator = (Calibrator)this.getEstimator((Class<? extends Calibrator>)Calibrator.class);
         final String predictFunc2;
         final String predictFunc = predictFunc2 = this.getPredictFunc();
         int n = -1;
         switch (predictFunc2.hashCode()) {
             case -318720807: {
                 if (predictFunc2.equals("predict")) {
                     n = 0;
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.27</version>
+    <version>1.7.28</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-extension</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn extensions converter</name>
   <description>JPMML Scikit-Learn extension packages to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sat Apr 01 22:15:12 EEST 2023
-version=1.7.27
+#Wed May 17 09:50:30 EEST 2023
+version=1.7.28
 groupId=org.jpmml
 artifactId=pmml-sklearn-extension
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-model-1.6.4.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-model-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pickle-1.3.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pickle-1.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.27.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.28.jar`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 7312 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Apr-01 22:15 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 lightgbm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 lightgbm/sklearn/
--rw-rw-r--  2.0 unx      177 b- defN 23-Apr-01 22:15 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      170 b- defN 23-Apr-01 22:15 lightgbm/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     1953 b- defN 23-Apr-01 22:15 lightgbm/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2102 b- defN 23-Apr-01 22:15 lightgbm/sklearn/LGBMRegressor.class
--rw-rw-r--  2.0 unx     2126 b- defN 23-Apr-01 22:15 lightgbm/sklearn/LGBMClassifier.class
--rw-rw-r--  2.0 unx     3298 b- defN 23-Apr-01 22:15 lightgbm/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
--rw-rw-r--  2.0 unx     1319 b- defN 23-Apr-01 22:14 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
--rw-rw-r--  2.0 unx      117 b- defN 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 lightgbm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 lightgbm/sklearn/
+-rw-rw-r--  2.0 unx      177 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      170 b- defN 23-May-17 09:50 lightgbm/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     1953 b- defN 23-May-17 09:50 lightgbm/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2102 b- defN 23-May-17 09:50 lightgbm/sklearn/LGBMRegressor.class
+-rw-rw-r--  2.0 unx     2126 b- defN 23-May-17 09:50 lightgbm/sklearn/LGBMClassifier.class
+-rw-rw-r--  2.0 unx     3298 b- defN 23-May-17 09:50 lightgbm/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
+-rw-rw-r--  2.0 unx     1319 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
+-rw-rw-r--  2.0 unx      117 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
 15 files, 11392 bytes uncompressed, 5232 bytes compressed:  54.1%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.27</version>
+    <version>1.7.28</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-lightgbm</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn LightGBM converter</name>
   <description>JPMML Scikit-Learn LightGBM to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sat Apr 01 22:15:12 EEST 2023
-version=1.7.27
+#Wed May 17 09:50:31 EEST 2023
+version=1.7.28
 groupId=org.jpmml
 artifactId=pmml-sklearn-lightgbm
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-converter-1.5.4.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-converter-1.5.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/ubjson-gson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/guava-21.0.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/guava-21.0.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-statsmodels-1.0.2.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-statsmodels-1.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-1.7.27.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-1.7.28.jar`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,404 +1,405 @@
-Zip file size: 466289 bytes, number of entries: 402
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/
--rw-r--r--  2.0 unx      159 b- defN 23-Apr-01 22:15 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn_pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 chaid/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 stop_words/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/calibration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/dummy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/svm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/impute/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/naive_bayes/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/linear_model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/linear_model/logistic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/linear_model/ridge/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/linear_model/glm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/linear_model/stochastic_gradient/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/compose/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/model_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/decomposition/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/neighbors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/multioutput/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/isotonic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/ensemble/bagging/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/ensemble/stacking/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/ensemble/forest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/ensemble/iforest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/ensemble/voting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/ensemble/weight_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/loss/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/discriminant_analysis/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/tree/visitors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/cluster/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn/multiclass/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/ruleset/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/decoration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/util/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/postprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 sklearn2pmml/expression/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 org/jpmml/sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 org/jpmml/sklearn/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn/
--rw-rw-r--  2.0 unx    16829 b- defN 23-Apr-01 22:15 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2287 b- defN 23-Apr-01 22:15 sklearn_pandas/CategoricalImputer.class
--rw-rw-r--  2.0 unx      656 b- defN 23-Apr-01 22:15 sklearn_pandas/TransformerPipeline.class
--rw-rw-r--  2.0 unx     1154 b- defN 23-Apr-01 22:15 sklearn_pandas/DataFrameMapper$2.class
--rw-rw-r--  2.0 unx     6280 b- defN 23-Apr-01 22:15 sklearn_pandas/DataFrameMapper.class
--rw-rw-r--  2.0 unx     1126 b- defN 23-Apr-01 22:15 sklearn_pandas/DataFrameMapper$1.class
--rw-rw-r--  2.0 unx      609 b- defN 23-Apr-01 22:15 chaid/ContinuousColumn.class
--rw-rw-r--  2.0 unx      925 b- defN 23-Apr-01 22:15 chaid/Node.class
--rw-rw-r--  2.0 unx      467 b- defN 23-Apr-01 22:15 chaid/Column.class
--rw-rw-r--  2.0 unx     3283 b- defN 23-Apr-01 22:15 chaid/Split.class
--rw-rw-r--  2.0 unx      401 b- defN 23-Apr-01 22:15 chaid/InvalidSplitReason.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Apr-01 22:15 chaid/NominalColumn.class
--rw-rw-r--  2.0 unx     1912 b- defN 23-Apr-01 22:15 stop_words/english.txt
--rw-rw-r--  2.0 unx      147 b- defN 23-Apr-01 22:15 sklearn/HasHead.class
--rw-rw-r--  2.0 unx     1728 b- defN 23-Apr-01 22:15 sklearn/StepUtil.class
--rw-rw-r--  2.0 unx    11796 b- defN 23-Apr-01 22:15 sklearn/calibration/CalibratedClassifier.class
--rw-rw-r--  2.0 unx     3213 b- defN 23-Apr-01 22:15 sklearn/calibration/SigmoidCalibration.class
--rw-rw-r--  2.0 unx      683 b- defN 23-Apr-01 22:15 sklearn/calibration/CalibratedClassifier$1.class
--rw-rw-r--  2.0 unx     1475 b- defN 23-Apr-01 22:15 sklearn/calibration/CalibratedClassifierCV.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Apr-01 22:15 sklearn/pipeline/PipelineTransformer.class
--rw-rw-r--  2.0 unx     1671 b- defN 23-Apr-01 22:15 sklearn/pipeline/Pipeline$2.class
--rw-rw-r--  2.0 unx     2536 b- defN 23-Apr-01 22:15 sklearn/pipeline/FeatureUnion.class
--rw-rw-r--  2.0 unx     5062 b- defN 23-Apr-01 22:15 sklearn/pipeline/Pipeline.class
--rw-rw-r--  2.0 unx     2003 b- defN 23-Apr-01 22:15 sklearn/pipeline/PipelineRegressor.class
--rw-rw-r--  2.0 unx     1773 b- defN 23-Apr-01 22:15 sklearn/pipeline/Pipeline$1.class
--rw-rw-r--  2.0 unx     1111 b- defN 23-Apr-01 22:15 sklearn/pipeline/PipelineUtil.class
--rw-rw-r--  2.0 unx     2298 b- defN 23-Apr-01 22:15 sklearn/pipeline/PipelineClassifier.class
--rw-rw-r--  2.0 unx     4973 b- defN 23-Apr-01 22:15 sklearn/dummy/DummyClassifier.class
--rw-rw-r--  2.0 unx     2055 b- defN 23-Apr-01 22:15 sklearn/dummy/DummyRegressor.class
--rw-rw-r--  2.0 unx      454 b- defN 23-Apr-01 22:15 sklearn/SkLearnFields.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-Apr-01 22:15 sklearn/SkLearnOutlierTransformation.class
--rw-rw-r--  2.0 unx      240 b- defN 23-Apr-01 22:15 sklearn/HasEstimator.class
--rw-rw-r--  2.0 unx     1182 b- defN 23-Apr-01 22:15 sklearn/HasMultiApplyField.class
--rw-rw-r--  2.0 unx      908 b- defN 23-Apr-01 22:15 sklearn/None.class
--rw-rw-r--  2.0 unx     2393 b- defN 23-Apr-01 22:15 sklearn/svm/SupportVectorMachineUtil.class
--rw-rw-r--  2.0 unx     2052 b- defN 23-Apr-01 22:15 sklearn/svm/OneClassSVMUtil.class
--rw-rw-r--  2.0 unx     1439 b- defN 23-Apr-01 22:15 sklearn/svm/OneClassSVMUtil$1.class
--rw-rw-r--  2.0 unx     1109 b- defN 23-Apr-01 22:15 sklearn/svm/LinearSVC.class
--rw-rw-r--  2.0 unx     5037 b- defN 23-Apr-01 22:15 sklearn/svm/LibSVMClassifier.class
--rw-rw-r--  2.0 unx      966 b- defN 23-Apr-01 22:15 sklearn/svm/SupportVectorMachineUtil$1.class
--rw-rw-r--  2.0 unx     1274 b- defN 23-Apr-01 22:15 sklearn/svm/OneClassSVM.class
--rw-rw-r--  2.0 unx     3594 b- defN 23-Apr-01 22:15 sklearn/svm/LibSVMRegressor.class
--rw-rw-r--  2.0 unx     4114 b- defN 23-Apr-01 22:15 sklearn/InitializerUtil$1.class
--rw-rw-r--  2.0 unx      735 b- defN 23-Apr-01 22:15 sklearn/Estimator$1.class
--rw-rw-r--  2.0 unx      214 b- defN 23-Apr-01 22:15 sklearn/HasNumberOfFeatures.class
--rw-rw-r--  2.0 unx      660 b- defN 23-Apr-01 22:15 sklearn/MultiTransformer.class
--rw-rw-r--  2.0 unx     2110 b- defN 23-Apr-01 22:15 sklearn/neural_network/MLPRegressor.class
--rw-rw-r--  2.0 unx     2633 b- defN 23-Apr-01 22:15 sklearn/neural_network/MLPClassifier.class
--rw-rw-r--  2.0 unx      759 b- defN 23-Apr-01 22:15 sklearn/neural_network/MultilayerPerceptronUtil$1.class
--rw-rw-r--  2.0 unx    11996 b- defN 23-Apr-01 22:15 sklearn/neural_network/MultilayerPerceptronUtil.class
--rw-rw-r--  2.0 unx     1880 b- defN 23-Apr-01 22:15 sklearn/Step.class
--rw-rw-r--  2.0 unx      168 b- defN 23-Apr-01 22:15 sklearn/HasDefaultValue.class
--rw-rw-r--  2.0 unx     2936 b- defN 23-Apr-01 22:15 sklearn/impute/MissingIndicator.class
--rw-rw-r--  2.0 unx     4027 b- defN 23-Apr-01 22:15 sklearn/impute/ImputerUtil.class
--rw-rw-r--  2.0 unx     5703 b- defN 23-Apr-01 22:15 sklearn/impute/SimpleImputer.class
--rw-rw-r--  2.0 unx     7021 b- defN 23-Apr-01 22:15 sklearn/naive_bayes/GaussianNB.class
--rw-rw-r--  2.0 unx     4460 b- defN 23-Apr-01 22:15 sklearn/linear_model/LinearRegressor.class
--rw-rw-r--  2.0 unx     4715 b- defN 23-Apr-01 22:15 sklearn/linear_model/LinearClassifier.class
--rw-rw-r--  2.0 unx     7535 b- defN 23-Apr-01 22:15 sklearn/linear_model/logistic/LogisticRegression.class
--rw-rw-r--  2.0 unx     1042 b- defN 23-Apr-01 22:15 sklearn/linear_model/ridge/RidgeClassifier.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Apr-01 22:15 sklearn/linear_model/glm/DistributionBoundary.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Apr-01 22:15 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Apr-01 22:15 sklearn/linear_model/stochastic_gradient/Hinge.class
--rw-rw-r--  2.0 unx     2449 b- defN 23-Apr-01 22:15 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
--rw-rw-r--  2.0 unx      461 b- defN 23-Apr-01 22:15 sklearn/linear_model/stochastic_gradient/LossFunction.class
--rw-rw-r--  2.0 unx      452 b- defN 23-Apr-01 22:15 sklearn/linear_model/stochastic_gradient/Log.class
--rw-rw-r--  2.0 unx     1165 b- defN 23-Apr-01 22:15 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
--rw-rw-r--  2.0 unx      482 b- defN 23-Apr-01 22:15 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
--rw-rw-r--  2.0 unx      932 b- defN 23-Apr-01 22:15 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
--rw-rw-r--  2.0 unx     1720 b- defN 23-Apr-01 22:15 sklearn/compose/ColumnTransformer$1.class
--rw-rw-r--  2.0 unx     3239 b- defN 23-Apr-01 22:15 sklearn/compose/TransformedTargetRegressor.class
--rw-rw-r--  2.0 unx     3649 b- defN 23-Apr-01 22:15 sklearn/compose/ColumnTransformer.class
--rw-rw-r--  2.0 unx     1534 b- defN 23-Apr-01 22:15 sklearn/compose/TransformedTargetRegressor$1.class
--rw-rw-r--  2.0 unx     2825 b- defN 23-Apr-01 22:15 sklearn/Classifier.class
--rw-rw-r--  2.0 unx     1457 b- defN 23-Apr-01 22:15 sklearn/model_selection/EstimatorSearcher.class
--rw-rw-r--  2.0 unx     1685 b- defN 23-Apr-01 22:15 sklearn/Selector.class
--rw-rw-r--  2.0 unx      419 b- defN 23-Apr-01 22:15 sklearn/decomposition/IncrementalPCA.class
--rw-rw-r--  2.0 unx     3471 b- defN 23-Apr-01 22:15 sklearn/decomposition/TruncatedSVD.class
--rw-rw-r--  2.0 unx     4759 b- defN 23-Apr-01 22:15 sklearn/decomposition/PCA.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Apr-01 22:15 sklearn/decomposition/BasePCA.class
--rw-rw-r--  2.0 unx      336 b- defN 23-Apr-01 22:15 sklearn/HasPredictField.class
--rw-rw-r--  2.0 unx     3018 b- defN 23-Apr-01 22:15 sklearn/neighbors/NearestNeighbors.class
--rw-rw-r--  2.0 unx     4505 b- defN 23-Apr-01 22:15 sklearn/neighbors/KNeighborsClassifier.class
--rw-rw-r--  2.0 unx     3794 b- defN 23-Apr-01 22:15 sklearn/neighbors/NearestCentroid.class
--rw-rw-r--  2.0 unx     2025 b- defN 23-Apr-01 22:15 sklearn/neighbors/BinaryTree.class
--rw-rw-r--  2.0 unx     1266 b- defN 23-Apr-01 22:15 sklearn/neighbors/KNeighborsUtil$1.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Apr-01 22:15 sklearn/neighbors/HasMetric.class
--rw-rw-r--  2.0 unx    10748 b- defN 23-Apr-01 22:15 sklearn/neighbors/KNeighborsUtil.class
--rw-rw-r--  2.0 unx     4387 b- defN 23-Apr-01 22:15 sklearn/neighbors/KNeighborsRegressor.class
--rw-rw-r--  2.0 unx     1032 b- defN 23-Apr-01 22:15 sklearn/neighbors/DistanceMetric.class
--rw-rw-r--  2.0 unx      351 b- defN 23-Apr-01 22:15 sklearn/neighbors/HasTrainingData.class
--rw-rw-r--  2.0 unx      176 b- defN 23-Apr-01 22:15 sklearn/neighbors/HasNumberOfNeighbors.class
--rw-rw-r--  2.0 unx     2235 b- defN 23-Apr-01 22:15 sklearn/multioutput/MultiOutputUtil.class
--rw-rw-r--  2.0 unx     3383 b- defN 23-Apr-01 22:15 sklearn/multioutput/ChainUtil.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Apr-01 22:15 sklearn/multioutput/RegressorChain.class
--rw-rw-r--  2.0 unx     1316 b- defN 23-Apr-01 22:15 sklearn/multioutput/MultiOutputClassifier.class
--rw-rw-r--  2.0 unx     1310 b- defN 23-Apr-01 22:15 sklearn/multioutput/MultiOutputRegressor.class
--rw-rw-r--  2.0 unx     1745 b- defN 23-Apr-01 22:15 sklearn/multioutput/ClassifierChain.class
--rw-rw-r--  2.0 unx     5923 b- defN 23-Apr-01 22:15 sklearn/isotonic/IsotonicRegression.class
--rw-rw-r--  2.0 unx      326 b- defN 23-Apr-01 22:15 sklearn/HasApplyField.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Apr-01 22:15 sklearn/HasEstimatorEnsemble.class
--rw-rw-r--  2.0 unx     1929 b- defN 23-Apr-01 22:15 sklearn/Transformer$1.class
--rw-rw-r--  2.0 unx      953 b- defN 23-Apr-01 22:15 sklearn/LabelEncoderClassifier.class
--rw-rw-r--  2.0 unx      937 b- defN 23-Apr-01 22:15 sklearn/PassThrough.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Apr-01 22:15 sklearn/HasPriorProbability.class
--rw-rw-r--  2.0 unx     5693 b- defN 23-Apr-01 22:15 sklearn/feature_extraction/text/TfidfVectorizer.class
--rw-rw-r--  2.0 unx      809 b- defN 23-Apr-01 22:15 sklearn/feature_extraction/text/TfidfVectorizer$1.class
--rw-rw-r--  2.0 unx      675 b- defN 23-Apr-01 22:15 sklearn/feature_extraction/text/Tokenizer.class
--rw-rw-r--  2.0 unx    13329 b- defN 23-Apr-01 22:15 sklearn/feature_extraction/text/CountVectorizer.class
--rw-rw-r--  2.0 unx     2129 b- defN 23-Apr-01 22:15 sklearn/feature_extraction/text/CountVectorizer$1.class
--rw-rw-r--  2.0 unx     1433 b- defN 23-Apr-01 22:15 sklearn/feature_extraction/text/TfidfTransformer.class
--rw-rw-r--  2.0 unx     4031 b- defN 23-Apr-01 22:15 sklearn/feature_extraction/DictVectorizer.class
--rw-rw-r--  2.0 unx      762 b- defN 23-Apr-01 22:15 sklearn/Clusterer.class
--rw-rw-r--  2.0 unx     1375 b- defN 23-Apr-01 22:15 sklearn/metrics/DistanceMetric.class
--rw-rw-r--  2.0 unx     1069 b- defN 23-Apr-01 22:15 sklearn/ensemble/EnsembleUtil.class
--rw-rw-r--  2.0 unx     2112 b- defN 23-Apr-01 22:15 sklearn/ensemble/bagging/BaggingRegressor.class
--rw-rw-r--  2.0 unx     3293 b- defN 23-Apr-01 22:15 sklearn/ensemble/bagging/BaggingUtil.class
--rw-rw-r--  2.0 unx     3083 b- defN 23-Apr-01 22:15 sklearn/ensemble/bagging/BaggingClassifier.class
--rw-rw-r--  2.0 unx     1409 b- defN 23-Apr-01 22:15 sklearn/ensemble/EnsembleRegressor.class
--rw-rw-r--  2.0 unx     3485 b- defN 23-Apr-01 22:15 sklearn/ensemble/stacking/StackingClassifier.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Apr-01 22:15 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
--rw-rw-r--  2.0 unx     3109 b- defN 23-Apr-01 22:15 sklearn/ensemble/stacking/StackingRegressor.class
--rw-rw-r--  2.0 unx     3706 b- defN 23-Apr-01 22:15 sklearn/ensemble/stacking/StackingUtil.class
--rw-rw-r--  2.0 unx     4851 b- defN 23-Apr-01 22:15 sklearn/ensemble/stacking/StackingClassifier$1.class
--rw-rw-r--  2.0 unx     2254 b- defN 23-Apr-01 22:15 sklearn/ensemble/stacking/StackingRegressor$1.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
--rw-rw-r--  2.0 unx     1440 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
--rw-rw-r--  2.0 unx     2563 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
--rw-rw-r--  2.0 unx      858 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/LossFunction.class
--rw-rw-r--  2.0 unx     1588 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
--rw-rw-r--  2.0 unx     1317 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
--rw-rw-r--  2.0 unx     7718 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
--rw-rw-r--  2.0 unx      960 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/MeanEstimator.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
--rw-rw-r--  2.0 unx     1578 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
--rw-rw-r--  2.0 unx      811 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
--rw-rw-r--  2.0 unx     3003 b- defN 23-Apr-01 22:15 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
--rw-rw-r--  2.0 unx     1148 b- defN 23-Apr-01 22:15 sklearn/ensemble/EnsembleUtil$1.class
--rw-rw-r--  2.0 unx     3059 b- defN 23-Apr-01 22:15 sklearn/ensemble/forest/ForestUtil.class
--rw-rw-r--  2.0 unx     2558 b- defN 23-Apr-01 22:15 sklearn/ensemble/forest/ForestRegressor.class
--rw-rw-r--  2.0 unx     3078 b- defN 23-Apr-01 22:15 sklearn/ensemble/forest/ForestClassifier.class
--rw-rw-r--  2.0 unx     1752 b- defN 23-Apr-01 22:15 sklearn/ensemble/iforest/IsolationForest$3.class
--rw-rw-r--  2.0 unx     2206 b- defN 23-Apr-01 22:15 sklearn/ensemble/iforest/IsolationForest$1.class
--rw-rw-r--  2.0 unx     2050 b- defN 23-Apr-01 22:15 sklearn/ensemble/iforest/IsolationForest$4.class
--rw-rw-r--  2.0 unx     1716 b- defN 23-Apr-01 22:15 sklearn/ensemble/iforest/IsolationForest$2.class
--rw-rw-r--  2.0 unx     8150 b- defN 23-Apr-01 22:15 sklearn/ensemble/iforest/IsolationForest.class
--rw-rw-r--  2.0 unx     4981 b- defN 23-Apr-01 22:15 sklearn/ensemble/voting/VotingClassifier.class
--rw-rw-r--  2.0 unx     3716 b- defN 23-Apr-01 22:15 sklearn/ensemble/voting/VotingRegressor.class
--rw-rw-r--  2.0 unx     2814 b- defN 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
--rw-rw-r--  2.0 unx     1247 b- defN 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
--rw-rw-r--  2.0 unx     3041 b- defN 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
--rw-rw-r--  2.0 unx     6152 b- defN 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
--rw-rw-r--  2.0 unx      505 b- defN 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
--rw-rw-r--  2.0 unx      490 b- defN 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
--rw-rw-r--  2.0 unx     1572 b- defN 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
--rw-rw-r--  2.0 unx     6118 b- defN 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     8868 b- defN 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
--rw-rw-r--  2.0 unx      441 b- defN 23-Apr-01 22:15 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
--rw-rw-r--  2.0 unx     1418 b- defN 23-Apr-01 22:15 sklearn/ensemble/EnsembleClassifier.class
--rw-rw-r--  2.0 unx     3564 b- defN 23-Apr-01 22:15 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
--rw-rw-r--  2.0 unx     5361 b- defN 23-Apr-01 22:15 sklearn/Transformer.class
--rw-rw-r--  2.0 unx      859 b- defN 23-Apr-01 22:15 sklearn/Transformer$1$1.class
--rw-rw-r--  2.0 unx      981 b- defN 23-Apr-01 22:15 sklearn/Drop.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Apr-01 22:15 sklearn/feature_selection/SelectKBest$Entry.class
--rw-rw-r--  2.0 unx     3486 b- defN 23-Apr-01 22:15 sklearn/feature_selection/SelectFromModel.class
--rw-rw-r--  2.0 unx     2922 b- defN 23-Apr-01 22:15 sklearn/feature_selection/SelectKBest.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Apr-01 22:15 sklearn/feature_selection/PySelector.class
--rw-rw-r--  2.0 unx      607 b- defN 23-Apr-01 22:15 sklearn/Transformer$2.class
--rw-rw-r--  2.0 unx     2216 b- defN 23-Apr-01 22:15 sklearn/SkLearnUtil.class
--rw-rw-r--  2.0 unx      412 b- defN 23-Apr-01 22:15 sklearn/loss/HalfMultinomialLoss.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Apr-01 22:15 sklearn/loss/CyLossFunction.class
--rw-rw-r--  2.0 unx      403 b- defN 23-Apr-01 22:15 sklearn/loss/HalfBinomialLoss.class
--rw-rw-r--  2.0 unx      387 b- defN 23-Apr-01 22:15 sklearn/loss/BaseLoss.class
--rw-rw-r--  2.0 unx      381 b- defN 23-Apr-01 22:15 sklearn/HasDecisionFunctionField.class
--rw-rw-r--  2.0 unx      338 b- defN 23-Apr-01 22:15 sklearn/SkLearnMethods.class
--rw-rw-r--  2.0 unx     3091 b- defN 23-Apr-01 22:15 sklearn/ScalarLabelUtil.class
--rw-rw-r--  2.0 unx      195 b- defN 23-Apr-01 22:15 sklearn/HasClasses.class
--rw-rw-r--  2.0 unx     4524 b- defN 23-Apr-01 22:15 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
--rw-rw-r--  2.0 unx      696 b- defN 23-Apr-01 22:15 sklearn/EstimatorUtil$1.class
--rw-rw-r--  2.0 unx     3311 b- defN 23-Apr-01 22:15 sklearn/Composite.class
--rw-rw-r--  2.0 unx     1194 b- defN 23-Apr-01 22:15 sklearn/preprocessing/KBinsDiscretizer$1.class
--rw-rw-r--  2.0 unx     4567 b- defN 23-Apr-01 22:15 sklearn/preprocessing/PowerTransformer.class
--rw-rw-r--  2.0 unx     2381 b- defN 23-Apr-01 22:15 sklearn/preprocessing/LabelEncoder.class
--rw-rw-r--  2.0 unx     4924 b- defN 23-Apr-01 22:15 sklearn/preprocessing/LabelBinarizer.class
--rw-rw-r--  2.0 unx      729 b- defN 23-Apr-01 22:15 sklearn/preprocessing/EncoderUtil$3.class
--rw-rw-r--  2.0 unx      389 b- defN 23-Apr-01 22:15 sklearn/preprocessing/Scaler.class
--rw-rw-r--  2.0 unx     3242 b- defN 23-Apr-01 22:15 sklearn/preprocessing/MaxAbsScaler.class
--rw-rw-r--  2.0 unx     2948 b- defN 23-Apr-01 22:15 sklearn/preprocessing/FunctionTransformer.class
--rw-rw-r--  2.0 unx     3291 b- defN 23-Apr-01 22:15 sklearn/preprocessing/BaseEncoder.class
--rw-rw-r--  2.0 unx     1270 b- defN 23-Apr-01 22:15 sklearn/preprocessing/EncoderUtil$1.class
--rw-rw-r--  2.0 unx     4549 b- defN 23-Apr-01 22:15 sklearn/preprocessing/StandardScaler.class
--rw-rw-r--  2.0 unx     6971 b- defN 23-Apr-01 22:15 sklearn/preprocessing/EncoderUtil.class
--rw-rw-r--  2.0 unx     6343 b- defN 23-Apr-01 22:15 sklearn/preprocessing/PolynomialFeatures.class
--rw-rw-r--  2.0 unx     8486 b- defN 23-Apr-01 22:15 sklearn/preprocessing/KBinsDiscretizer.class
--rw-rw-r--  2.0 unx     4671 b- defN 23-Apr-01 22:15 sklearn/preprocessing/OneHotEncoder.class
--rw-rw-r--  2.0 unx     2553 b- defN 23-Apr-01 22:15 sklearn/preprocessing/Binarizer.class
--rw-rw-r--  2.0 unx     1054 b- defN 23-Apr-01 22:15 sklearn/preprocessing/EncoderUtil$2.class
--rw-rw-r--  2.0 unx     3595 b- defN 23-Apr-01 22:15 sklearn/preprocessing/MinMaxScaler.class
--rw-rw-r--  2.0 unx     4467 b- defN 23-Apr-01 22:15 sklearn/preprocessing/RobustScaler.class
--rw-rw-r--  2.0 unx     3740 b- defN 23-Apr-01 22:15 sklearn/preprocessing/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      957 b- defN 23-Apr-01 22:15 sklearn/preprocessing/Imputer.class
--rw-rw-r--  2.0 unx     2033 b- defN 23-Apr-01 22:15 sklearn/preprocessing/PolynomialFeatures$1.class
--rw-rw-r--  2.0 unx     7408 b- defN 23-Apr-01 22:15 sklearn/preprocessing/MultiOneHotEncoder.class
--rw-rw-r--  2.0 unx     2173 b- defN 23-Apr-01 22:15 sklearn/tree/TreeClassifier.class
--rw-rw-r--  2.0 unx     3111 b- defN 23-Apr-01 22:15 sklearn/tree/TreeUtil$1.class
--rw-rw-r--  2.0 unx     2664 b- defN 23-Apr-01 22:15 sklearn/tree/TreeUtil$4.class
--rw-rw-r--  2.0 unx     4805 b- defN 23-Apr-01 22:15 sklearn/tree/visitors/TreeModelFlattener.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Apr-01 22:15 sklearn/tree/visitors/TreeModelCompactor$1.class
--rw-rw-r--  2.0 unx     5431 b- defN 23-Apr-01 22:15 sklearn/tree/visitors/TreeModelCompactor.class
--rw-rw-r--  2.0 unx     2988 b- defN 23-Apr-01 22:15 sklearn/tree/visitors/TreeModelPruner.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Apr-01 22:15 sklearn/tree/visitors/TreeModelFlattener$1.class
--rw-rw-r--  2.0 unx      730 b- defN 23-Apr-01 22:15 sklearn/tree/visitors/TreeModelPruner$1.class
--rw-rw-r--  2.0 unx     1489 b- defN 23-Apr-01 22:15 sklearn/tree/TreeUtil$8.class
--rw-rw-r--  2.0 unx      879 b- defN 23-Apr-01 22:15 sklearn/tree/RegressionCriterion.class
--rw-rw-r--  2.0 unx     1151 b- defN 23-Apr-01 22:15 sklearn/tree/TreeUtil$5.class
--rw-rw-r--  2.0 unx      978 b- defN 23-Apr-01 22:15 sklearn/tree/PresortBestSplitter.class
--rw-rw-r--  2.0 unx      977 b- defN 23-Apr-01 22:15 sklearn/tree/TreeUtil$6.class
--rw-rw-r--  2.0 unx     1764 b- defN 23-Apr-01 22:15 sklearn/tree/TreeRegressor.class
--rw-rw-r--  2.0 unx     1589 b- defN 23-Apr-01 22:15 sklearn/tree/TreeUtil$7.class
--rw-rw-r--  2.0 unx    20190 b- defN 23-Apr-01 22:15 sklearn/tree/TreeUtil.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-Apr-01 22:15 sklearn/tree/TreeUtil$3.class
--rw-rw-r--  2.0 unx     1373 b- defN 23-Apr-01 22:15 sklearn/tree/HasTreeOptions.class
--rw-rw-r--  2.0 unx     2257 b- defN 23-Apr-01 22:15 sklearn/tree/Tree.class
--rw-rw-r--  2.0 unx      754 b- defN 23-Apr-01 22:15 sklearn/tree/TreeUtil$2.class
--rw-rw-r--  2.0 unx      150 b- defN 23-Apr-01 22:15 sklearn/tree/HasTree.class
--rw-rw-r--  2.0 unx     1967 b- defN 23-Apr-01 22:15 sklearn/InitializerUtil.class
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-01 22:15 sklearn/Regressor.class
--rw-rw-r--  2.0 unx      211 b- defN 23-Apr-01 22:15 sklearn/HasNumberOfOutputs.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Apr-01 22:15 sklearn/HasClassifierOptions.class
--rw-rw-r--  2.0 unx     6878 b- defN 23-Apr-01 22:15 sklearn/EstimatorUtil.class
--rw-rw-r--  2.0 unx      199 b- defN 23-Apr-01 22:15 sklearn/HasType.class
--rw-rw-r--  2.0 unx      678 b- defN 23-Apr-01 22:15 sklearn/cluster/MiniBatchKMeans.class
--rw-rw-r--  2.0 unx     5086 b- defN 23-Apr-01 22:15 sklearn/cluster/KMeans.class
--rw-rw-r--  2.0 unx     8327 b- defN 23-Apr-01 22:15 sklearn/Estimator.class
--rw-rw-r--  2.0 unx     1624 b- defN 23-Apr-01 22:15 sklearn/Initializer.class
--rw-rw-r--  2.0 unx     4598 b- defN 23-Apr-01 22:15 sklearn/multiclass/OneVsRestClassifier.class
--rw-rw-r--  2.0 unx     5157 b- defN 23-Apr-01 22:15 sklearn2pmml/ruleset/RuleSetClassifier.class
--rw-rw-r--  2.0 unx     1023 b- defN 23-Apr-01 22:15 sklearn2pmml/pipeline/PMMLPipeline$3.class
--rw-rw-r--  2.0 unx    28185 b- defN 23-Apr-01 22:15 sklearn2pmml/pipeline/PMMLPipeline.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Apr-01 22:15 sklearn2pmml/pipeline/PMMLPipeline$2.class
--rw-rw-r--  2.0 unx     1421 b- defN 23-Apr-01 22:15 sklearn2pmml/pipeline/PMMLPipeline$1.class
--rw-rw-r--  2.0 unx     1811 b- defN 23-Apr-01 22:15 sklearn2pmml/pipeline/Verification.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/MultiDomain.class
--rw-rw-r--  2.0 unx     1152 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/ContinuousDomainEraser.class
--rw-rw-r--  2.0 unx     1654 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/Alias.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/TemporalDomain.class
--rw-rw-r--  2.0 unx      779 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/ContinuousDomain$1.class
--rw-rw-r--  2.0 unx    11878 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/Domain.class
--rw-rw-r--  2.0 unx     1416 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/MultiAlias.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/DiscreteDomain.class
--rw-rw-r--  2.0 unx     1952 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/CategoricalDomain.class
--rw-rw-r--  2.0 unx     1453 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/DomainEraser.class
--rw-rw-r--  2.0 unx      613 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/DateTimeDomain.class
--rw-rw-r--  2.0 unx     7764 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/ContinuousDomain.class
--rw-rw-r--  2.0 unx     1083 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/DiscreteDomainEraser.class
--rw-rw-r--  2.0 unx     1590 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/TransformerWrapper.class
--rw-rw-r--  2.0 unx     1045 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/Domain$2.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/DateDomain.class
--rw-rw-r--  2.0 unx     3544 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/DomainUtil.class
--rw-rw-r--  2.0 unx     1033 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/Domain$1.class
--rw-rw-r--  2.0 unx     1577 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/OrdinalDomain.class
--rw-rw-r--  2.0 unx      672 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/Domain$4.class
--rw-rw-r--  2.0 unx      799 b- defN 23-Apr-01 22:15 sklearn2pmml/decoration/Domain$3.class
--rw-rw-r--  2.0 unx     7862 b- defN 23-Apr-01 22:15 sklearn2pmml/neural_network/MLPTransformer.class
--rw-rw-r--  2.0 unx      335 b- defN 23-Apr-01 22:15 sklearn2pmml/SkLearn2PMMLFields.class
--rw-rw-r--  2.0 unx     1160 b- defN 23-Apr-01 22:15 sklearn2pmml/util/Evaluatable.class
--rw-rw-r--  2.0 unx     1196 b- defN 23-Apr-01 22:15 sklearn2pmml/util/Expression.class
--rw-rw-r--  2.0 unx     1189 b- defN 23-Apr-01 22:15 sklearn2pmml/util/Predicate.class
--rw-rw-r--  2.0 unx     1434 b- defN 23-Apr-01 22:15 sklearn2pmml/util/Reshaper.class
--rw-rw-r--  2.0 unx     3392 b- defN 23-Apr-01 22:15 sklearn2pmml/util/EvaluatableUtil.class
--rw-rw-r--  2.0 unx     1658 b- defN 23-Apr-01 22:15 sklearn2pmml/util/Slicer.class
--rw-rw-r--  2.0 unx     2418 b- defN 23-Apr-01 22:15 sklearn2pmml/feature_extraction/text/Splitter.class
--rw-rw-r--  2.0 unx     3184 b- defN 23-Apr-01 22:15 sklearn2pmml/feature_extraction/text/Matcher.class
--rw-rw-r--  2.0 unx     1262 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/SelectFirstRegressor.class
--rw-rw-r--  2.0 unx     2083 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/GBDTUtil$2.class
--rw-rw-r--  2.0 unx     1134 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/EstimatorChain$1.class
--rw-rw-r--  2.0 unx     1934 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/GBDTLMRegressor.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/GBDTUtil$1.class
--rw-rw-r--  2.0 unx     7358 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/EstimatorChain.class
--rw-rw-r--  2.0 unx     6578 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/GBDTUtil.class
--rw-rw-r--  2.0 unx     3995 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/Link.class
--rw-rw-r--  2.0 unx     4360 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/SelectFirstUtil.class
--rw-rw-r--  2.0 unx     3773 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/GBDTLRClassifier.class
--rw-rw-r--  2.0 unx     2608 b- defN 23-Apr-01 22:15 sklearn2pmml/ensemble/SelectFirstClassifier.class
--rw-rw-r--  2.0 unx     1438 b- defN 23-Apr-01 22:15 sklearn2pmml/EstimatorProxy$1.class
--rw-rw-r--  2.0 unx      946 b- defN 23-Apr-01 22:15 sklearn2pmml/feature_selection/SelectUnique.class
--rw-rw-r--  2.0 unx     6477 b- defN 23-Apr-01 22:15 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
--rw-rw-r--  2.0 unx      791 b- defN 23-Apr-01 22:15 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
--rw-rw-r--  2.0 unx     1197 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/PatternTransformer.class
--rw-rw-r--  2.0 unx     2908 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/ReplaceTransformer.class
--rw-rw-r--  2.0 unx     1844 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/WordCountTransformer.class
--rw-rw-r--  2.0 unx      597 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/DateTimeFormatter.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
--rw-rw-r--  2.0 unx     4621 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/DurationTransformer.class
--rw-rw-r--  2.0 unx      444 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
--rw-rw-r--  2.0 unx     2777 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/FilterLookupTransformer.class
--rw-rw-r--  2.0 unx     2545 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/Formatter.class
--rw-rw-r--  2.0 unx     3341 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/CastTransformer.class
--rw-rw-r--  2.0 unx     2758 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/MatchesTransformer.class
--rw-rw-r--  2.0 unx      589 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/NumberFormatter.class
--rw-rw-r--  2.0 unx     4149 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/MultiLookupTransformer.class
--rw-rw-r--  2.0 unx     3871 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/StringNormalizer.class
--rw-rw-r--  2.0 unx     7145 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/ExpressionTransformer.class
--rw-rw-r--  2.0 unx      635 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
--rw-rw-r--  2.0 unx     3604 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/DataFrameConstructor.class
--rw-rw-r--  2.0 unx     2847 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/ConcatTransformer.class
--rw-rw-r--  2.0 unx     5993 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/CutTransformer.class
--rw-rw-r--  2.0 unx     7025 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/BSplineTransformer.class
--rw-rw-r--  2.0 unx     6410 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/LookupTransformer.class
--rw-rw-r--  2.0 unx     3236 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/SubstringTransformer.class
--rw-rw-r--  2.0 unx     3181 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
--rw-rw-r--  2.0 unx     2132 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
--rw-rw-r--  2.0 unx     3328 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/Aggregator.class
--rw-rw-r--  2.0 unx      647 b- defN 23-Apr-01 22:15 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
--rw-rw-r--  2.0 unx     1082 b- defN 23-Apr-01 22:15 sklearn2pmml/tree/CHAIDRegressor.class
--rw-rw-r--  2.0 unx    11309 b- defN 23-Apr-01 22:15 sklearn2pmml/tree/CHAIDUtil.class
--rw-rw-r--  2.0 unx     2019 b- defN 23-Apr-01 22:15 sklearn2pmml/tree/CHAIDClassifier.class
--rw-rw-r--  2.0 unx     1417 b- defN 23-Apr-01 22:15 sklearn2pmml/tree/CHAIDUtil$1.class
--rw-rw-r--  2.0 unx     3864 b- defN 23-Apr-01 22:15 sklearn2pmml/EstimatorProxy.class
--rw-rw-r--  2.0 unx     1458 b- defN 23-Apr-01 22:15 sklearn2pmml/SelectorProxy.class
--rw-rw-r--  2.0 unx     2046 b- defN 23-Apr-01 22:15 sklearn2pmml/expression/ExpressionUtil.class
--rw-rw-r--  2.0 unx     3799 b- defN 23-Apr-01 22:15 sklearn2pmml/expression/ExpressionRegressor.class
--rw-rw-r--  2.0 unx      990 b- defN 23-Apr-01 22:15 sklearn2pmml/expression/ExpressionClassifier$1.class
--rw-rw-r--  2.0 unx     8759 b- defN 23-Apr-01 22:15 sklearn2pmml/expression/ExpressionClassifier.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Apr-01 22:15 sklearn2pmml/expression/ExpressionUtil$1.class
--rw-rw-r--  2.0 unx     1774 b- defN 23-Apr-01 22:15 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     2764 b- defN 23-Apr-01 22:15 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
--rw-rw-r--  2.0 unx     3549 b- defN 23-Apr-01 22:15 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
--rw-rw-r--  2.0 unx    13598 b- defN 23-Apr-01 22:15 org/jpmml/sklearn/SkLearnEncoder.class
--rw-rw-r--  2.0 unx      194 b- defN 23-Apr-01 22:15 org/jpmml/sklearn/FieldNames.class
--rw-rw-r--  2.0 unx      171 b- defN 23-Apr-01 22:15 org/jpmml/sklearn/HasSkLearnOptions.class
--rw-rw-r--  2.0 unx     1030 b- defN 23-Apr-01 22:15 org/jpmml/sklearn/SkLearnEncoder$1.class
--rw-rw-r--  2.0 unx     1822 b- defN 23-Apr-01 22:14 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
--rw-rw-r--  2.0 unx       57 b- defN 23-Apr-01 22:15 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
-402 files, 916509 bytes uncompressed, 404555 bytes compressed:  55.9%
+Zip file size: 466641 bytes, number of entries: 403
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
+-rw-r--r--  2.0 unx      159 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn_pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 chaid/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 stop_words/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/calibration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/dummy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/svm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/impute/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/naive_bayes/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/linear_model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/linear_model/logistic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/linear_model/ridge/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/linear_model/glm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/compose/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/model_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/decomposition/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/neighbors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/multioutput/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/isotonic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/bagging/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/stacking/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/forest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/iforest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/voting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/weight_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/loss/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/discriminant_analysis/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/tree/visitors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/cluster/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/multiclass/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/ruleset/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/decoration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/util/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/postprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/expression/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 org/jpmml/sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 org/jpmml/sklearn/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn/
+-rw-rw-r--  2.0 unx    16829 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2287 b- defN 23-May-17 09:50 sklearn_pandas/CategoricalImputer.class
+-rw-rw-r--  2.0 unx      656 b- defN 23-May-17 09:50 sklearn_pandas/TransformerPipeline.class
+-rw-rw-r--  2.0 unx     1154 b- defN 23-May-17 09:50 sklearn_pandas/DataFrameMapper$2.class
+-rw-rw-r--  2.0 unx     6280 b- defN 23-May-17 09:50 sklearn_pandas/DataFrameMapper.class
+-rw-rw-r--  2.0 unx     1126 b- defN 23-May-17 09:50 sklearn_pandas/DataFrameMapper$1.class
+-rw-rw-r--  2.0 unx      609 b- defN 23-May-17 09:50 chaid/ContinuousColumn.class
+-rw-rw-r--  2.0 unx      925 b- defN 23-May-17 09:50 chaid/Node.class
+-rw-rw-r--  2.0 unx      467 b- defN 23-May-17 09:50 chaid/Column.class
+-rw-rw-r--  2.0 unx     3283 b- defN 23-May-17 09:50 chaid/Split.class
+-rw-rw-r--  2.0 unx      401 b- defN 23-May-17 09:50 chaid/InvalidSplitReason.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-May-17 09:50 chaid/NominalColumn.class
+-rw-rw-r--  2.0 unx     1912 b- defN 23-May-17 09:50 stop_words/english.txt
+-rw-rw-r--  2.0 unx      147 b- defN 23-May-17 09:50 sklearn/HasHead.class
+-rw-rw-r--  2.0 unx     1728 b- defN 23-May-17 09:50 sklearn/StepUtil.class
+-rw-rw-r--  2.0 unx    11436 b- defN 23-May-17 09:50 sklearn/calibration/CalibratedClassifier.class
+-rw-rw-r--  2.0 unx     2972 b- defN 23-May-17 09:50 sklearn/calibration/SigmoidCalibration.class
+-rw-rw-r--  2.0 unx      683 b- defN 23-May-17 09:50 sklearn/calibration/CalibratedClassifier$1.class
+-rw-rw-r--  2.0 unx     1475 b- defN 23-May-17 09:50 sklearn/calibration/CalibratedClassifierCV.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-May-17 09:50 sklearn/pipeline/PipelineTransformer.class
+-rw-rw-r--  2.0 unx     1671 b- defN 23-May-17 09:50 sklearn/pipeline/Pipeline$2.class
+-rw-rw-r--  2.0 unx     2536 b- defN 23-May-17 09:50 sklearn/pipeline/FeatureUnion.class
+-rw-rw-r--  2.0 unx     5062 b- defN 23-May-17 09:50 sklearn/pipeline/Pipeline.class
+-rw-rw-r--  2.0 unx     2003 b- defN 23-May-17 09:50 sklearn/pipeline/PipelineRegressor.class
+-rw-rw-r--  2.0 unx     1773 b- defN 23-May-17 09:50 sklearn/pipeline/Pipeline$1.class
+-rw-rw-r--  2.0 unx     1111 b- defN 23-May-17 09:50 sklearn/pipeline/PipelineUtil.class
+-rw-rw-r--  2.0 unx     2298 b- defN 23-May-17 09:50 sklearn/pipeline/PipelineClassifier.class
+-rw-rw-r--  2.0 unx     4973 b- defN 23-May-17 09:50 sklearn/dummy/DummyClassifier.class
+-rw-rw-r--  2.0 unx     2055 b- defN 23-May-17 09:50 sklearn/dummy/DummyRegressor.class
+-rw-rw-r--  2.0 unx      454 b- defN 23-May-17 09:50 sklearn/SkLearnFields.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-May-17 09:50 sklearn/SkLearnOutlierTransformation.class
+-rw-rw-r--  2.0 unx      240 b- defN 23-May-17 09:50 sklearn/HasEstimator.class
+-rw-rw-r--  2.0 unx     1182 b- defN 23-May-17 09:50 sklearn/HasMultiApplyField.class
+-rw-rw-r--  2.0 unx      908 b- defN 23-May-17 09:50 sklearn/None.class
+-rw-rw-r--  2.0 unx     2393 b- defN 23-May-17 09:50 sklearn/svm/SupportVectorMachineUtil.class
+-rw-rw-r--  2.0 unx     2052 b- defN 23-May-17 09:50 sklearn/svm/OneClassSVMUtil.class
+-rw-rw-r--  2.0 unx     1439 b- defN 23-May-17 09:50 sklearn/svm/OneClassSVMUtil$1.class
+-rw-rw-r--  2.0 unx     1109 b- defN 23-May-17 09:50 sklearn/svm/LinearSVC.class
+-rw-rw-r--  2.0 unx     5037 b- defN 23-May-17 09:50 sklearn/svm/LibSVMClassifier.class
+-rw-rw-r--  2.0 unx      966 b- defN 23-May-17 09:50 sklearn/svm/SupportVectorMachineUtil$1.class
+-rw-rw-r--  2.0 unx     1274 b- defN 23-May-17 09:50 sklearn/svm/OneClassSVM.class
+-rw-rw-r--  2.0 unx     3594 b- defN 23-May-17 09:50 sklearn/svm/LibSVMRegressor.class
+-rw-rw-r--  2.0 unx     4114 b- defN 23-May-17 09:50 sklearn/InitializerUtil$1.class
+-rw-rw-r--  2.0 unx      735 b- defN 23-May-17 09:50 sklearn/Estimator$1.class
+-rw-rw-r--  2.0 unx      214 b- defN 23-May-17 09:50 sklearn/HasNumberOfFeatures.class
+-rw-rw-r--  2.0 unx      660 b- defN 23-May-17 09:50 sklearn/MultiTransformer.class
+-rw-rw-r--  2.0 unx     2110 b- defN 23-May-17 09:50 sklearn/neural_network/MLPRegressor.class
+-rw-rw-r--  2.0 unx     2633 b- defN 23-May-17 09:50 sklearn/neural_network/MLPClassifier.class
+-rw-rw-r--  2.0 unx      759 b- defN 23-May-17 09:50 sklearn/neural_network/MultilayerPerceptronUtil$1.class
+-rw-rw-r--  2.0 unx    11996 b- defN 23-May-17 09:50 sklearn/neural_network/MultilayerPerceptronUtil.class
+-rw-rw-r--  2.0 unx     1880 b- defN 23-May-17 09:50 sklearn/Step.class
+-rw-rw-r--  2.0 unx      168 b- defN 23-May-17 09:50 sklearn/HasDefaultValue.class
+-rw-rw-r--  2.0 unx     2936 b- defN 23-May-17 09:50 sklearn/impute/MissingIndicator.class
+-rw-rw-r--  2.0 unx     4027 b- defN 23-May-17 09:50 sklearn/impute/ImputerUtil.class
+-rw-rw-r--  2.0 unx     5703 b- defN 23-May-17 09:50 sklearn/impute/SimpleImputer.class
+-rw-rw-r--  2.0 unx     7021 b- defN 23-May-17 09:50 sklearn/naive_bayes/GaussianNB.class
+-rw-rw-r--  2.0 unx     4460 b- defN 23-May-17 09:50 sklearn/linear_model/LinearRegressor.class
+-rw-rw-r--  2.0 unx     4715 b- defN 23-May-17 09:50 sklearn/linear_model/LinearClassifier.class
+-rw-rw-r--  2.0 unx     7535 b- defN 23-May-17 09:50 sklearn/linear_model/logistic/LogisticRegression.class
+-rw-rw-r--  2.0 unx     1042 b- defN 23-May-17 09:50 sklearn/linear_model/ridge/RidgeClassifier.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-May-17 09:50 sklearn/linear_model/glm/DistributionBoundary.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-May-17 09:50 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/Hinge.class
+-rw-rw-r--  2.0 unx     2449 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
+-rw-rw-r--  2.0 unx      461 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/LossFunction.class
+-rw-rw-r--  2.0 unx      452 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/Log.class
+-rw-rw-r--  2.0 unx     1165 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
+-rw-rw-r--  2.0 unx      482 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
+-rw-rw-r--  2.0 unx      932 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
+-rw-rw-r--  2.0 unx     1720 b- defN 23-May-17 09:50 sklearn/compose/ColumnTransformer$1.class
+-rw-rw-r--  2.0 unx     3239 b- defN 23-May-17 09:50 sklearn/compose/TransformedTargetRegressor.class
+-rw-rw-r--  2.0 unx     3649 b- defN 23-May-17 09:50 sklearn/compose/ColumnTransformer.class
+-rw-rw-r--  2.0 unx     1534 b- defN 23-May-17 09:50 sklearn/compose/TransformedTargetRegressor$1.class
+-rw-rw-r--  2.0 unx     2825 b- defN 23-May-17 09:50 sklearn/Classifier.class
+-rw-rw-r--  2.0 unx     1457 b- defN 23-May-17 09:50 sklearn/model_selection/EstimatorSearcher.class
+-rw-rw-r--  2.0 unx     1685 b- defN 23-May-17 09:50 sklearn/Selector.class
+-rw-rw-r--  2.0 unx      419 b- defN 23-May-17 09:50 sklearn/decomposition/IncrementalPCA.class
+-rw-rw-r--  2.0 unx     3471 b- defN 23-May-17 09:50 sklearn/decomposition/TruncatedSVD.class
+-rw-rw-r--  2.0 unx     4759 b- defN 23-May-17 09:50 sklearn/decomposition/PCA.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-May-17 09:50 sklearn/decomposition/BasePCA.class
+-rw-rw-r--  2.0 unx      336 b- defN 23-May-17 09:50 sklearn/HasPredictField.class
+-rw-rw-r--  2.0 unx     3018 b- defN 23-May-17 09:50 sklearn/neighbors/NearestNeighbors.class
+-rw-rw-r--  2.0 unx     4505 b- defN 23-May-17 09:50 sklearn/neighbors/KNeighborsClassifier.class
+-rw-rw-r--  2.0 unx     3794 b- defN 23-May-17 09:50 sklearn/neighbors/NearestCentroid.class
+-rw-rw-r--  2.0 unx     2025 b- defN 23-May-17 09:50 sklearn/neighbors/BinaryTree.class
+-rw-rw-r--  2.0 unx     1266 b- defN 23-May-17 09:50 sklearn/neighbors/KNeighborsUtil$1.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-May-17 09:50 sklearn/neighbors/HasMetric.class
+-rw-rw-r--  2.0 unx    10748 b- defN 23-May-17 09:50 sklearn/neighbors/KNeighborsUtil.class
+-rw-rw-r--  2.0 unx     4387 b- defN 23-May-17 09:50 sklearn/neighbors/KNeighborsRegressor.class
+-rw-rw-r--  2.0 unx     1032 b- defN 23-May-17 09:50 sklearn/neighbors/DistanceMetric.class
+-rw-rw-r--  2.0 unx      351 b- defN 23-May-17 09:50 sklearn/neighbors/HasTrainingData.class
+-rw-rw-r--  2.0 unx      176 b- defN 23-May-17 09:50 sklearn/neighbors/HasNumberOfNeighbors.class
+-rw-rw-r--  2.0 unx     2235 b- defN 23-May-17 09:50 sklearn/multioutput/MultiOutputUtil.class
+-rw-rw-r--  2.0 unx     3383 b- defN 23-May-17 09:50 sklearn/multioutput/ChainUtil.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-May-17 09:50 sklearn/multioutput/RegressorChain.class
+-rw-rw-r--  2.0 unx     1316 b- defN 23-May-17 09:50 sklearn/multioutput/MultiOutputClassifier.class
+-rw-rw-r--  2.0 unx     1310 b- defN 23-May-17 09:50 sklearn/multioutput/MultiOutputRegressor.class
+-rw-rw-r--  2.0 unx     1745 b- defN 23-May-17 09:50 sklearn/multioutput/ClassifierChain.class
+-rw-rw-r--  2.0 unx     4469 b- defN 23-May-17 09:50 sklearn/isotonic/IsotonicRegression.class
+-rw-rw-r--  2.0 unx      326 b- defN 23-May-17 09:50 sklearn/HasApplyField.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-May-17 09:50 sklearn/HasEstimatorEnsemble.class
+-rw-rw-r--  2.0 unx     1929 b- defN 23-May-17 09:50 sklearn/Transformer$1.class
+-rw-rw-r--  2.0 unx      953 b- defN 23-May-17 09:50 sklearn/LabelEncoderClassifier.class
+-rw-rw-r--  2.0 unx      937 b- defN 23-May-17 09:50 sklearn/PassThrough.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-May-17 09:50 sklearn/HasPriorProbability.class
+-rw-rw-r--  2.0 unx     5693 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/TfidfVectorizer.class
+-rw-rw-r--  2.0 unx      809 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/TfidfVectorizer$1.class
+-rw-rw-r--  2.0 unx      675 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/Tokenizer.class
+-rw-rw-r--  2.0 unx    13329 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/CountVectorizer.class
+-rw-rw-r--  2.0 unx     2129 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/CountVectorizer$1.class
+-rw-rw-r--  2.0 unx     1433 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/TfidfTransformer.class
+-rw-rw-r--  2.0 unx     4031 b- defN 23-May-17 09:50 sklearn/feature_extraction/DictVectorizer.class
+-rw-rw-r--  2.0 unx      762 b- defN 23-May-17 09:50 sklearn/Clusterer.class
+-rw-rw-r--  2.0 unx     1375 b- defN 23-May-17 09:50 sklearn/metrics/DistanceMetric.class
+-rw-rw-r--  2.0 unx     1069 b- defN 23-May-17 09:50 sklearn/ensemble/EnsembleUtil.class
+-rw-rw-r--  2.0 unx     2112 b- defN 23-May-17 09:50 sklearn/ensemble/bagging/BaggingRegressor.class
+-rw-rw-r--  2.0 unx     3293 b- defN 23-May-17 09:50 sklearn/ensemble/bagging/BaggingUtil.class
+-rw-rw-r--  2.0 unx     3083 b- defN 23-May-17 09:50 sklearn/ensemble/bagging/BaggingClassifier.class
+-rw-rw-r--  2.0 unx     1409 b- defN 23-May-17 09:50 sklearn/ensemble/EnsembleRegressor.class
+-rw-rw-r--  2.0 unx     3485 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingClassifier.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
+-rw-rw-r--  2.0 unx     3109 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingRegressor.class
+-rw-rw-r--  2.0 unx     3706 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingUtil.class
+-rw-rw-r--  2.0 unx     4851 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingClassifier$1.class
+-rw-rw-r--  2.0 unx     2254 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingRegressor$1.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
+-rw-rw-r--  2.0 unx     1440 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
+-rw-rw-r--  2.0 unx     2563 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx      858 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/LossFunction.class
+-rw-rw-r--  2.0 unx     1588 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
+-rw-rw-r--  2.0 unx     1317 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
+-rw-rw-r--  2.0 unx     7718 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
+-rw-rw-r--  2.0 unx      960 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/MeanEstimator.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
+-rw-rw-r--  2.0 unx     1578 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
+-rw-rw-r--  2.0 unx      811 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
+-rw-rw-r--  2.0 unx     3003 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
+-rw-rw-r--  2.0 unx     1148 b- defN 23-May-17 09:50 sklearn/ensemble/EnsembleUtil$1.class
+-rw-rw-r--  2.0 unx     3059 b- defN 23-May-17 09:50 sklearn/ensemble/forest/ForestUtil.class
+-rw-rw-r--  2.0 unx     2558 b- defN 23-May-17 09:50 sklearn/ensemble/forest/ForestRegressor.class
+-rw-rw-r--  2.0 unx     3078 b- defN 23-May-17 09:50 sklearn/ensemble/forest/ForestClassifier.class
+-rw-rw-r--  2.0 unx     1752 b- defN 23-May-17 09:50 sklearn/ensemble/iforest/IsolationForest$3.class
+-rw-rw-r--  2.0 unx     2206 b- defN 23-May-17 09:50 sklearn/ensemble/iforest/IsolationForest$1.class
+-rw-rw-r--  2.0 unx     2050 b- defN 23-May-17 09:50 sklearn/ensemble/iforest/IsolationForest$4.class
+-rw-rw-r--  2.0 unx     1716 b- defN 23-May-17 09:50 sklearn/ensemble/iforest/IsolationForest$2.class
+-rw-rw-r--  2.0 unx     8150 b- defN 23-May-17 09:50 sklearn/ensemble/iforest/IsolationForest.class
+-rw-rw-r--  2.0 unx     4981 b- defN 23-May-17 09:50 sklearn/ensemble/voting/VotingClassifier.class
+-rw-rw-r--  2.0 unx     3716 b- defN 23-May-17 09:50 sklearn/ensemble/voting/VotingRegressor.class
+-rw-rw-r--  2.0 unx     2814 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx     1247 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
+-rw-rw-r--  2.0 unx     3041 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
+-rw-rw-r--  2.0 unx     6152 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
+-rw-rw-r--  2.0 unx      490 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
+-rw-rw-r--  2.0 unx     1572 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
+-rw-rw-r--  2.0 unx     6118 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     8868 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
+-rw-rw-r--  2.0 unx     1418 b- defN 23-May-17 09:50 sklearn/ensemble/EnsembleClassifier.class
+-rw-rw-r--  2.0 unx     3564 b- defN 23-May-17 09:50 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
+-rw-rw-r--  2.0 unx     5361 b- defN 23-May-17 09:50 sklearn/Transformer.class
+-rw-rw-r--  2.0 unx      859 b- defN 23-May-17 09:50 sklearn/Transformer$1$1.class
+-rw-rw-r--  2.0 unx      981 b- defN 23-May-17 09:50 sklearn/Drop.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-May-17 09:50 sklearn/feature_selection/SelectKBest$Entry.class
+-rw-rw-r--  2.0 unx     3486 b- defN 23-May-17 09:50 sklearn/feature_selection/SelectFromModel.class
+-rw-rw-r--  2.0 unx     2922 b- defN 23-May-17 09:50 sklearn/feature_selection/SelectKBest.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-May-17 09:50 sklearn/feature_selection/PySelector.class
+-rw-rw-r--  2.0 unx      607 b- defN 23-May-17 09:50 sklearn/Transformer$2.class
+-rw-rw-r--  2.0 unx     2216 b- defN 23-May-17 09:50 sklearn/SkLearnUtil.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-May-17 09:50 sklearn/loss/HalfMultinomialLoss.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-May-17 09:50 sklearn/loss/CyLossFunction.class
+-rw-rw-r--  2.0 unx      403 b- defN 23-May-17 09:50 sklearn/loss/HalfBinomialLoss.class
+-rw-rw-r--  2.0 unx      387 b- defN 23-May-17 09:50 sklearn/loss/BaseLoss.class
+-rw-rw-r--  2.0 unx      381 b- defN 23-May-17 09:50 sklearn/HasDecisionFunctionField.class
+-rw-rw-r--  2.0 unx      338 b- defN 23-May-17 09:50 sklearn/SkLearnMethods.class
+-rw-rw-r--  2.0 unx     3091 b- defN 23-May-17 09:50 sklearn/ScalarLabelUtil.class
+-rw-rw-r--  2.0 unx      195 b- defN 23-May-17 09:50 sklearn/HasClasses.class
+-rw-rw-r--  2.0 unx     4524 b- defN 23-May-17 09:50 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
+-rw-rw-r--  2.0 unx      696 b- defN 23-May-17 09:50 sklearn/EstimatorUtil$1.class
+-rw-rw-r--  2.0 unx     3311 b- defN 23-May-17 09:50 sklearn/Composite.class
+-rw-rw-r--  2.0 unx     1194 b- defN 23-May-17 09:50 sklearn/preprocessing/KBinsDiscretizer$1.class
+-rw-rw-r--  2.0 unx     4567 b- defN 23-May-17 09:50 sklearn/preprocessing/PowerTransformer.class
+-rw-rw-r--  2.0 unx     2381 b- defN 23-May-17 09:50 sklearn/preprocessing/LabelEncoder.class
+-rw-rw-r--  2.0 unx     4924 b- defN 23-May-17 09:50 sklearn/preprocessing/LabelBinarizer.class
+-rw-rw-r--  2.0 unx      729 b- defN 23-May-17 09:50 sklearn/preprocessing/EncoderUtil$3.class
+-rw-rw-r--  2.0 unx      389 b- defN 23-May-17 09:50 sklearn/preprocessing/Scaler.class
+-rw-rw-r--  2.0 unx     3242 b- defN 23-May-17 09:50 sklearn/preprocessing/MaxAbsScaler.class
+-rw-rw-r--  2.0 unx     2948 b- defN 23-May-17 09:50 sklearn/preprocessing/FunctionTransformer.class
+-rw-rw-r--  2.0 unx     3291 b- defN 23-May-17 09:50 sklearn/preprocessing/BaseEncoder.class
+-rw-rw-r--  2.0 unx     1270 b- defN 23-May-17 09:50 sklearn/preprocessing/EncoderUtil$1.class
+-rw-rw-r--  2.0 unx     4549 b- defN 23-May-17 09:50 sklearn/preprocessing/StandardScaler.class
+-rw-rw-r--  2.0 unx     6971 b- defN 23-May-17 09:50 sklearn/preprocessing/EncoderUtil.class
+-rw-rw-r--  2.0 unx     6343 b- defN 23-May-17 09:50 sklearn/preprocessing/PolynomialFeatures.class
+-rw-rw-r--  2.0 unx     8486 b- defN 23-May-17 09:50 sklearn/preprocessing/KBinsDiscretizer.class
+-rw-rw-r--  2.0 unx     4671 b- defN 23-May-17 09:50 sklearn/preprocessing/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     2553 b- defN 23-May-17 09:50 sklearn/preprocessing/Binarizer.class
+-rw-rw-r--  2.0 unx     1054 b- defN 23-May-17 09:50 sklearn/preprocessing/EncoderUtil$2.class
+-rw-rw-r--  2.0 unx     3595 b- defN 23-May-17 09:50 sklearn/preprocessing/MinMaxScaler.class
+-rw-rw-r--  2.0 unx     4467 b- defN 23-May-17 09:50 sklearn/preprocessing/RobustScaler.class
+-rw-rw-r--  2.0 unx     3740 b- defN 23-May-17 09:50 sklearn/preprocessing/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      957 b- defN 23-May-17 09:50 sklearn/preprocessing/Imputer.class
+-rw-rw-r--  2.0 unx     2033 b- defN 23-May-17 09:50 sklearn/preprocessing/PolynomialFeatures$1.class
+-rw-rw-r--  2.0 unx     7408 b- defN 23-May-17 09:50 sklearn/preprocessing/MultiOneHotEncoder.class
+-rw-rw-r--  2.0 unx     2173 b- defN 23-May-17 09:50 sklearn/tree/TreeClassifier.class
+-rw-rw-r--  2.0 unx     3111 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$1.class
+-rw-rw-r--  2.0 unx     2664 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$4.class
+-rw-rw-r--  2.0 unx     4805 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelFlattener.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelCompactor$1.class
+-rw-rw-r--  2.0 unx     5431 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelCompactor.class
+-rw-rw-r--  2.0 unx     2988 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelPruner.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelFlattener$1.class
+-rw-rw-r--  2.0 unx      730 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelPruner$1.class
+-rw-rw-r--  2.0 unx     1489 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$8.class
+-rw-rw-r--  2.0 unx      879 b- defN 23-May-17 09:50 sklearn/tree/RegressionCriterion.class
+-rw-rw-r--  2.0 unx     1151 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$5.class
+-rw-rw-r--  2.0 unx      978 b- defN 23-May-17 09:50 sklearn/tree/PresortBestSplitter.class
+-rw-rw-r--  2.0 unx      977 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$6.class
+-rw-rw-r--  2.0 unx     1764 b- defN 23-May-17 09:50 sklearn/tree/TreeRegressor.class
+-rw-rw-r--  2.0 unx     1589 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$7.class
+-rw-rw-r--  2.0 unx    20190 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$3.class
+-rw-rw-r--  2.0 unx     1373 b- defN 23-May-17 09:50 sklearn/tree/HasTreeOptions.class
+-rw-rw-r--  2.0 unx     2257 b- defN 23-May-17 09:50 sklearn/tree/Tree.class
+-rw-rw-r--  2.0 unx      754 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$2.class
+-rw-rw-r--  2.0 unx      150 b- defN 23-May-17 09:50 sklearn/tree/HasTree.class
+-rw-rw-r--  2.0 unx     1967 b- defN 23-May-17 09:50 sklearn/InitializerUtil.class
+-rw-rw-r--  2.0 unx      570 b- defN 23-May-17 09:50 sklearn/Regressor.class
+-rw-rw-r--  2.0 unx      211 b- defN 23-May-17 09:50 sklearn/HasNumberOfOutputs.class
+-rw-rw-r--  2.0 unx     2366 b- defN 23-May-17 09:50 sklearn/Calibrator.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-May-17 09:50 sklearn/HasClassifierOptions.class
+-rw-rw-r--  2.0 unx     6878 b- defN 23-May-17 09:50 sklearn/EstimatorUtil.class
+-rw-rw-r--  2.0 unx      199 b- defN 23-May-17 09:50 sklearn/HasType.class
+-rw-rw-r--  2.0 unx      678 b- defN 23-May-17 09:50 sklearn/cluster/MiniBatchKMeans.class
+-rw-rw-r--  2.0 unx     5086 b- defN 23-May-17 09:50 sklearn/cluster/KMeans.class
+-rw-rw-r--  2.0 unx     8327 b- defN 23-May-17 09:50 sklearn/Estimator.class
+-rw-rw-r--  2.0 unx     1624 b- defN 23-May-17 09:50 sklearn/Initializer.class
+-rw-rw-r--  2.0 unx     4598 b- defN 23-May-17 09:50 sklearn/multiclass/OneVsRestClassifier.class
+-rw-rw-r--  2.0 unx     5157 b- defN 23-May-17 09:50 sklearn2pmml/ruleset/RuleSetClassifier.class
+-rw-rw-r--  2.0 unx     1023 b- defN 23-May-17 09:50 sklearn2pmml/pipeline/PMMLPipeline$3.class
+-rw-rw-r--  2.0 unx    28185 b- defN 23-May-17 09:50 sklearn2pmml/pipeline/PMMLPipeline.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-May-17 09:50 sklearn2pmml/pipeline/PMMLPipeline$2.class
+-rw-rw-r--  2.0 unx     1421 b- defN 23-May-17 09:50 sklearn2pmml/pipeline/PMMLPipeline$1.class
+-rw-rw-r--  2.0 unx     1811 b- defN 23-May-17 09:50 sklearn2pmml/pipeline/Verification.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-May-17 09:50 sklearn2pmml/decoration/MultiDomain.class
+-rw-rw-r--  2.0 unx     1152 b- defN 23-May-17 09:50 sklearn2pmml/decoration/ContinuousDomainEraser.class
+-rw-rw-r--  2.0 unx     1654 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Alias.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-May-17 09:50 sklearn2pmml/decoration/TemporalDomain.class
+-rw-rw-r--  2.0 unx      779 b- defN 23-May-17 09:50 sklearn2pmml/decoration/ContinuousDomain$1.class
+-rw-rw-r--  2.0 unx    11878 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Domain.class
+-rw-rw-r--  2.0 unx     1416 b- defN 23-May-17 09:50 sklearn2pmml/decoration/MultiAlias.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DiscreteDomain.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-May-17 09:50 sklearn2pmml/decoration/CategoricalDomain.class
+-rw-rw-r--  2.0 unx     1453 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DomainEraser.class
+-rw-rw-r--  2.0 unx      613 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DateTimeDomain.class
+-rw-rw-r--  2.0 unx     7764 b- defN 23-May-17 09:50 sklearn2pmml/decoration/ContinuousDomain.class
+-rw-rw-r--  2.0 unx     1083 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DiscreteDomainEraser.class
+-rw-rw-r--  2.0 unx     1590 b- defN 23-May-17 09:50 sklearn2pmml/decoration/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     1045 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Domain$2.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DateDomain.class
+-rw-rw-r--  2.0 unx     3544 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DomainUtil.class
+-rw-rw-r--  2.0 unx     1033 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Domain$1.class
+-rw-rw-r--  2.0 unx     1577 b- defN 23-May-17 09:50 sklearn2pmml/decoration/OrdinalDomain.class
+-rw-rw-r--  2.0 unx      672 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Domain$4.class
+-rw-rw-r--  2.0 unx      799 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Domain$3.class
+-rw-rw-r--  2.0 unx     7862 b- defN 23-May-17 09:50 sklearn2pmml/neural_network/MLPTransformer.class
+-rw-rw-r--  2.0 unx      335 b- defN 23-May-17 09:50 sklearn2pmml/SkLearn2PMMLFields.class
+-rw-rw-r--  2.0 unx     1160 b- defN 23-May-17 09:50 sklearn2pmml/util/Evaluatable.class
+-rw-rw-r--  2.0 unx     1196 b- defN 23-May-17 09:50 sklearn2pmml/util/Expression.class
+-rw-rw-r--  2.0 unx     1189 b- defN 23-May-17 09:50 sklearn2pmml/util/Predicate.class
+-rw-rw-r--  2.0 unx     1434 b- defN 23-May-17 09:50 sklearn2pmml/util/Reshaper.class
+-rw-rw-r--  2.0 unx     3392 b- defN 23-May-17 09:50 sklearn2pmml/util/EvaluatableUtil.class
+-rw-rw-r--  2.0 unx     1658 b- defN 23-May-17 09:50 sklearn2pmml/util/Slicer.class
+-rw-rw-r--  2.0 unx     2418 b- defN 23-May-17 09:50 sklearn2pmml/feature_extraction/text/Splitter.class
+-rw-rw-r--  2.0 unx     3184 b- defN 23-May-17 09:50 sklearn2pmml/feature_extraction/text/Matcher.class
+-rw-rw-r--  2.0 unx     1262 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/SelectFirstRegressor.class
+-rw-rw-r--  2.0 unx     2083 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/GBDTUtil$2.class
+-rw-rw-r--  2.0 unx     1134 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/EstimatorChain$1.class
+-rw-rw-r--  2.0 unx     1934 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/GBDTLMRegressor.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/GBDTUtil$1.class
+-rw-rw-r--  2.0 unx     7358 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/EstimatorChain.class
+-rw-rw-r--  2.0 unx     6578 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/GBDTUtil.class
+-rw-rw-r--  2.0 unx     3995 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/Link.class
+-rw-rw-r--  2.0 unx     4360 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/SelectFirstUtil.class
+-rw-rw-r--  2.0 unx     3773 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/GBDTLRClassifier.class
+-rw-rw-r--  2.0 unx     2608 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/SelectFirstClassifier.class
+-rw-rw-r--  2.0 unx     1438 b- defN 23-May-17 09:50 sklearn2pmml/EstimatorProxy$1.class
+-rw-rw-r--  2.0 unx      946 b- defN 23-May-17 09:50 sklearn2pmml/feature_selection/SelectUnique.class
+-rw-rw-r--  2.0 unx     6477 b- defN 23-May-17 09:50 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
+-rw-rw-r--  2.0 unx      791 b- defN 23-May-17 09:50 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
+-rw-rw-r--  2.0 unx     1197 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/PatternTransformer.class
+-rw-rw-r--  2.0 unx     2908 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/ReplaceTransformer.class
+-rw-rw-r--  2.0 unx     1844 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/WordCountTransformer.class
+-rw-rw-r--  2.0 unx      597 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/DateTimeFormatter.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
+-rw-rw-r--  2.0 unx     4621 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/DurationTransformer.class
+-rw-rw-r--  2.0 unx      444 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
+-rw-rw-r--  2.0 unx     2777 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/FilterLookupTransformer.class
+-rw-rw-r--  2.0 unx     2545 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/Formatter.class
+-rw-rw-r--  2.0 unx     3341 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/CastTransformer.class
+-rw-rw-r--  2.0 unx     2758 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/MatchesTransformer.class
+-rw-rw-r--  2.0 unx      589 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/NumberFormatter.class
+-rw-rw-r--  2.0 unx     4149 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/MultiLookupTransformer.class
+-rw-rw-r--  2.0 unx     3871 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/StringNormalizer.class
+-rw-rw-r--  2.0 unx     7145 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/ExpressionTransformer.class
+-rw-rw-r--  2.0 unx      635 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     3604 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/DataFrameConstructor.class
+-rw-rw-r--  2.0 unx     2847 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/ConcatTransformer.class
+-rw-rw-r--  2.0 unx     5993 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/CutTransformer.class
+-rw-rw-r--  2.0 unx     7025 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/BSplineTransformer.class
+-rw-rw-r--  2.0 unx     6410 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/LookupTransformer.class
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/SubstringTransformer.class
+-rw-rw-r--  2.0 unx     3181 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
+-rw-rw-r--  2.0 unx     2132 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
+-rw-rw-r--  2.0 unx     3328 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/Aggregator.class
+-rw-rw-r--  2.0 unx      647 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     1082 b- defN 23-May-17 09:50 sklearn2pmml/tree/CHAIDRegressor.class
+-rw-rw-r--  2.0 unx    11309 b- defN 23-May-17 09:50 sklearn2pmml/tree/CHAIDUtil.class
+-rw-rw-r--  2.0 unx     2019 b- defN 23-May-17 09:50 sklearn2pmml/tree/CHAIDClassifier.class
+-rw-rw-r--  2.0 unx     1417 b- defN 23-May-17 09:50 sklearn2pmml/tree/CHAIDUtil$1.class
+-rw-rw-r--  2.0 unx     3864 b- defN 23-May-17 09:50 sklearn2pmml/EstimatorProxy.class
+-rw-rw-r--  2.0 unx     1458 b- defN 23-May-17 09:50 sklearn2pmml/SelectorProxy.class
+-rw-rw-r--  2.0 unx     2046 b- defN 23-May-17 09:50 sklearn2pmml/expression/ExpressionUtil.class
+-rw-rw-r--  2.0 unx     3799 b- defN 23-May-17 09:50 sklearn2pmml/expression/ExpressionRegressor.class
+-rw-rw-r--  2.0 unx      990 b- defN 23-May-17 09:50 sklearn2pmml/expression/ExpressionClassifier$1.class
+-rw-rw-r--  2.0 unx     8759 b- defN 23-May-17 09:50 sklearn2pmml/expression/ExpressionClassifier.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-May-17 09:50 sklearn2pmml/expression/ExpressionUtil$1.class
+-rw-rw-r--  2.0 unx     1774 b- defN 23-May-17 09:50 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     2764 b- defN 23-May-17 09:50 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
+-rw-rw-r--  2.0 unx     3549 b- defN 23-May-17 09:50 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
+-rw-rw-r--  2.0 unx    13598 b- defN 23-May-17 09:50 org/jpmml/sklearn/SkLearnEncoder.class
+-rw-rw-r--  2.0 unx      194 b- defN 23-May-17 09:50 org/jpmml/sklearn/FieldNames.class
+-rw-rw-r--  2.0 unx      171 b- defN 23-May-17 09:50 org/jpmml/sklearn/HasSkLearnOptions.class
+-rw-rw-r--  2.0 unx     1030 b- defN 23-May-17 09:50 org/jpmml/sklearn/SkLearnEncoder$1.class
+-rw-rw-r--  2.0 unx     1822 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
+-rw-rw-r--  2.0 unx       57 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
+403 files, 916820 bytes uncompressed, 404783 bytes compressed:  55.8%
```

#### zipnote «TEMP»/diffoscope_ie8mbd0r_/tmpr0ptcg51_.zip

```diff
@@ -882,14 +882,17 @@
 
 Filename: sklearn/Regressor.class
 Comment: 
 
 Filename: sklearn/HasNumberOfOutputs.class
 Comment: 
 
+Filename: sklearn/Calibrator.class
+Comment: 
+
 Filename: sklearn/HasClassifierOptions.class
 Comment: 
 
 Filename: sklearn/EstimatorUtil.class
 Comment: 
 
 Filename: sklearn/HasType.class
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-SkLearn library
-Implementation-Version: 1.7.27
+Implementation-Version: 1.7.28
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.2.2
```

#### sklearn/calibration/CalibratedClassifier.class

##### procyon -ec {}

```diff
@@ -1,20 +1,19 @@
 
 package sklearn.calibration;
 
 import sklearn.Estimator;
 import org.dmg.pmml.DerivedField;
-import sklearn.isotonic.IsotonicRegression;
 import org.dmg.pmml.ResultFeature;
 import java.util.Iterator;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segmentation;
 import org.jpmml.converter.regression.RegressionModelUtil;
 import java.util.Collections;
-import sklearn.Regressor;
+import sklearn.Calibrator;
 import org.jpmml.converter.SchemaUtil;
 import java.util.List;
 import org.jpmml.converter.Label;
 import org.dmg.pmml.Output;
 import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.OpType;
@@ -42,15 +41,15 @@
 public class CalibratedClassifier extends Classifier implements HasEstimator<Classifier>
 {
     public CalibratedClassifier(final String module, final String name) {
         super(module, name);
     }
     
     public Model encodeModel(final Schema schema) {
-        final List<? extends Regressor> calibrators = this.getCalibrators();
+        final List<? extends Calibrator> calibrators = this.getCalibrators();
         final List<?> classes = this.getClasses();
         final Classifier estimator = this.getEstimator();
         final String method2;
         final String method = method2 = this.getMethod();
         int n = -1;
         switch (method2.hashCode()) {
             case 583579720: {
@@ -138,28 +137,28 @@
                         decisionFunctionFeatures = decisionFunctionFeatures.subList(1, 2);
                     }
                 }
                 SchemaUtil.checkSize(calibrators.size(), (List)decisionFunctionFeatures);
                 RegressionModel calibratorModel;
                 if (calibrators.size() == 1) {
                     SchemaUtil.checkSize(2, categoricalLabel);
-                    final Regressor calibrator = (Regressor)calibrators.get(0);
+                    final Calibrator calibrator = (Calibrator)calibrators.get(0);
                     final Model featureModel = (Model)models.get(0);
                     final Feature feature = (Feature)decisionFunctionFeatures.get(0);
                     final Feature calibratedFeature = calibrate(calibrator, featureModel, feature, encoder);
                     calibratorModel = RegressionModelUtil.createBinaryLogisticClassification((List)Collections.singletonList(calibratedFeature), (List)Collections.singletonList(Double.valueOf(1.0)), (Number)null, RegressionModel.NormalizationMethod.NONE, true, schema);
                 }
                 else {
                     if (calibrators.size() < 3) {
                         throw new IllegalArgumentException();
                     }
                     SchemaUtil.checkSize(calibrators.size(), categoricalLabel);
                     final List<RegressionTable> regressionTables = new ArrayList<RegressionTable>();
                     for (int i = 0; i < calibrators.size(); ++i) {
-                        final Regressor calibrator2 = (Regressor)calibrators.get(i);
+                        final Calibrator calibrator2 = (Calibrator)calibrators.get(i);
                         final Model featureModel2 = (models.size() == 1) ? ((Model)models.get(0)) : ((Model)models.get(i));
                         final Feature feature2 = (Feature)decisionFunctionFeatures.get(i);
                         final Feature calibratedFeature2 = calibrate(calibrator2, featureModel2, feature2, encoder);
                         final RegressionTable regressionTable2 = RegressionModelUtil.createRegressionTable((List)Collections.singletonList(calibratedFeature2), (List)Collections.singletonList(Double.valueOf(1.0)), (Number)null).setTargetCategory(categoricalLabel.getValue(i));
                         regressionTables.add(regressionTable2);
                     }
                     calibratorModel = new RegressionModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), (List)regressionTables).setNormalizationMethod(RegressionModel.NormalizationMethod.SIMPLEMAX).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, categoricalLabel));
@@ -173,39 +172,28 @@
         }
     }
     
     public List<?> getClasses() {
         return this.getListLike("classes");
     }
     
-    public List<? extends Regressor> getCalibrators() {
-        return this.getList("calibrators", (Class)Regressor.class);
+    public List<? extends Calibrator> getCalibrators() {
+        return this.getList("calibrators", (Class)Calibrator.class);
     }
     
     public Classifier getEstimator() {
         return (Classifier)this.get("estimator", (Class)Classifier.class);
     }
     
     public String getMethod() {
         return this.getString("method");
     }
     
-    private static Feature calibrate(final Regressor calibrator, final Model model, final Feature feature, final SkLearnEncoder encoder) {
+    private static Feature calibrate(final Calibrator calibrator, final Model model, final Feature feature, final SkLearnEncoder encoder) {
         encoder.export(model, feature.getName());
-        Feature calibratedFeature;
-        if (calibrator instanceof IsotonicRegression) {
-            final IsotonicRegression isotonicRegression = (IsotonicRegression)calibrator;
-            calibratedFeature = (Feature)Iterables.getOnlyElement((Iterable)isotonicRegression.encodeFeatures((List)Collections.singletonList(feature), encoder));
-        }
-        else {
-            if (!(calibrator instanceof SigmoidCalibration)) {
-                throw new IllegalArgumentException();
-            }
-            final SigmoidCalibration sigmoidCalibration = (SigmoidCalibration)calibrator;
-            calibratedFeature = (Feature)Iterables.getOnlyElement((Iterable)sigmoidCalibration.encodeFeatures((List)Collections.singletonList(feature), encoder));
-        }
+        final Feature calibratedFeature = (Feature)Iterables.getOnlyElement((Iterable)calibrator.encodeFeatures((List)Collections.singletonList(feature), encoder));
         DerivedField derivedField = encoder.removeDerivedField(calibratedFeature.getName());
         final OutputField outputField = new OutputField(derivedField.requireName(), derivedField.requireOpType(), derivedField.requireDataType()).setResultFeature(ResultFeature.TRANSFORMED_VALUE).setExpression(derivedField.requireExpression()).setFinalResult(Boolean.valueOf(false));
         derivedField = (DerivedField)encoder.createDerivedField(model, outputField, true);
         return (Feature)new ContinuousFeature((PMMLEncoder)encoder, (Field)derivedField);
     }
 }
```

#### sklearn/calibration/SigmoidCalibration.class

##### procyon -ec {}

```diff
@@ -12,28 +12,22 @@
 import java.util.Collections;
 import org.jpmml.converter.PMMLUtil;
 import org.dmg.pmml.Expression;
 import org.jpmml.converter.SchemaUtil;
 import org.jpmml.sklearn.SkLearnEncoder;
 import org.jpmml.converter.Feature;
 import java.util.List;
-import org.dmg.pmml.Model;
-import org.jpmml.converter.Schema;
-import sklearn.Regressor;
+import sklearn.Calibrator;
 
-public class SigmoidCalibration extends Regressor
+public class SigmoidCalibration extends Calibrator
 {
     public SigmoidCalibration(final String module, final String name) {
         super(module, name);
     }
     
-    public Model encodeModel(final Schema schema) {
-        throw new UnsupportedOperationException();
-    }
-    
     public List<Feature> encodeFeatures(final List<Feature> features, final SkLearnEncoder encoder) {
         final Number a = this.getA();
         final Number b = this.getB();
         SchemaUtil.checkSize(1, (List)features);
         final Feature feature = (Feature)features.get(0);
         Apply apply = PMMLUtil.createApply("*", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(-1)), (Expression)PMMLUtil.createApply("+", new Expression[] { (Expression)PMMLUtil.createApply("*", new Expression[] { (Expression)PMMLUtil.createConstant(a), (Expression)feature.ref() }), (Expression)PMMLUtil.createConstant(b) }) });
         apply = FunctionUtil.encodeScipyFunction("scipy.special", "expit", (List)Collections.singletonList(apply));
```

#### sklearn/calibration/CalibratedClassifier$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 2151dac637e6bf54dedf81cb9ebc5ba8eb1f85631163b24b207adbdb62a56dc0
+  SHA-256 checksum b89c1a7f33429046e53ef5fa587842c1d704630d209dc6feacf6f3f6ed2b91a1
   Compiled from "CalibratedClassifier.java"
 class sklearn.calibration.CalibratedClassifier$1
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #6                          // sklearn/calibration/CalibratedClassifier$1
   super_class: #7                         // java/lang/Object
@@ -67,15 +67,15 @@
         20: goto          24
         23: astore_0
         24: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 163: 0
+        line 162: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 2
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
 }
```

#### sklearn/isotonic/IsotonicRegression.class

##### procyon -ec {}

```diff
@@ -1,50 +1,35 @@
 
 package sklearn.isotonic;
 
-import org.dmg.pmml.Model;
 import org.dmg.pmml.DerivedField;
 import org.dmg.pmml.OutlierTreatmentMethod;
+import java.util.Collections;
 import org.dmg.pmml.Field;
+import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.converter.ContinuousFeature;
 import org.dmg.pmml.Expression;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.OpType;
 import org.dmg.pmml.LinearNorm;
 import org.dmg.pmml.NormContinuous;
 import org.jpmml.converter.SchemaUtil;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
-import org.jpmml.converter.Label;
-import org.jpmml.converter.PMMLEncoder;
-import org.jpmml.converter.regression.RegressionModelUtil;
-import java.util.Collections;
-import com.google.common.collect.Iterables;
+import org.jpmml.sklearn.SkLearnEncoder;
 import org.jpmml.converter.Feature;
 import java.util.List;
-import org.jpmml.sklearn.SkLearnEncoder;
-import org.dmg.pmml.regression.RegressionModel;
-import org.jpmml.converter.Schema;
-import sklearn.Regressor;
+import sklearn.Calibrator;
 
-public class IsotonicRegression extends Regressor
+public class IsotonicRegression extends Calibrator
 {
     public IsotonicRegression(final String module, final String name) {
         super(module, name);
     }
     
-    public RegressionModel encodeModel(final Schema schema) {
-        final PMMLEncoder encoder = schema.getEncoder();
-        final Label label = schema.getLabel();
-        List<? extends Feature> features = schema.getFeatures();
-        features = this.encodeFeatures((List<Feature>)features, (SkLearnEncoder)encoder);
-        final Feature feature = (Feature)Iterables.getOnlyElement((Iterable)features);
-        return RegressionModelUtil.createRegression((List)Collections.singletonList(feature), (List)Collections.singletonList(Double.valueOf(1.0)), (Number)Double.valueOf(0.0), RegressionModel.NormalizationMethod.NONE, schema);
-    }
-    
     public List<Feature> encodeFeatures(final List<Feature> features, final SkLearnEncoder encoder) {
         final List<? extends Number> xThresholds = this.getXThresholds();
         final List<? extends Number> yThresholds = this.getYThresholds();
         final String outOfBounds = this.getOutOfBounds();
         ClassDictUtil.checkSize(new Collection[] { xThresholds, yThresholds });
         SchemaUtil.checkSize(1, (List)features);
         final Feature feature = (Feature)features.get(0);
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.27</version>
+    <version>1.7.28</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn converter</name>
   <description>JPMML Scikit-Learn to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-sklearn
 groupId=org.jpmml
-version=1.7.27
+version=1.7.28
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/ubjson-0.1.8.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/ubjson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-python-1.1.14.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-python-1.1.14.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-h2o-1.2.5.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-h2o-1.2.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/classpath.txt` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/classpath.txt`

 * *Files 25% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 jakarta.xml.bind-api-3.0.1.jar
 jaxb-core-3.0.2.jar
 jaxb-runtime-3.0.2.jar
 jcommander-1.72.jar
 pickle-1.3.jar
 pmml-converter-1.5.4.jar
 pmml-h2o-1.2.5.jar
-pmml-lightgbm-1.4.4.jar
+pmml-lightgbm-1.4.5.jar
 pmml-model-1.6.4.jar
 pmml-model-metro-1.6.4.jar
 pmml-python-1.1.14.jar
-pmml-sklearn-1.7.27.jar
-pmml-sklearn-extension-1.7.27.jar
-pmml-sklearn-h2o-1.7.27.jar
-pmml-sklearn-lightgbm-1.7.27.jar
-pmml-sklearn-statsmodels-1.7.27.jar
-pmml-sklearn-xgboost-1.7.27.jar
+pmml-sklearn-1.7.28.jar
+pmml-sklearn-extension-1.7.28.jar
+pmml-sklearn-h2o-1.7.28.jar
+pmml-sklearn-lightgbm-1.7.28.jar
+pmml-sklearn-statsmodels-1.7.28.jar
+pmml-sklearn-xgboost-1.7.28.jar
 pmml-statsmodels-1.0.2.jar
 pmml-xgboost-1.7.3.jar
 serpent-1.40.jar
 slf4j-api-1.7.36.jar
 slf4j-jdk14-1.7.36.jar
 ubjson-0.1.8.jar
 ubjson-gson-0.1.8.jar
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 5703 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 09:28 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-May-01 09:28 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-01 09:28 com/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-01 09:28 com/sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 09:28 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 09:28 META-INF/maven/com.sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 09:28 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
--rw-rw-r--  2.0 unx     3741 b- defN 23-May-01 09:28 com/sklearn2pmml/Main.class
--rw-rw-r--  2.0 unx     1200 b- defN 23-May-01 09:28 com/sklearn2pmml/Main$1.class
--rw-rw-r--  2.0 unx     7844 b- defN 23-Apr-02 08:05 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
--rw-rw-r--  2.0 unx       70 b- defN 23-May-01 09:28 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:56 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-May-17 09:56 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:56 com/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:56 com/sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:56 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:56 META-INF/maven/com.sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:56 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
+-rw-rw-r--  2.0 unx     3741 b- defN 23-May-17 09:56 com/sklearn2pmml/Main.class
+-rw-rw-r--  2.0 unx     1200 b- defN 23-May-17 09:56 com/sklearn2pmml/Main$1.class
+-rw-rw-r--  2.0 unx     7844 b- defN 23-May-17 09:56 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
+-rw-rw-r--  2.0 unx       70 b- defN 23-May-17 09:56 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
 11 files, 13013 bytes uncompressed, 4227 bytes compressed:  67.5%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: SkLearn2PMML package
-Implementation-Version: 0.92.1
+Implementation-Version: 0.92.2
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.2.2
```

#### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

##### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

```diff
@@ -24,15 +24,15 @@
     <tag>HEAD</tag>
   </scm>
   <issueManagement>
     <system>GitHub</system>
     <url>https://github.com/jpmml/sklearn2pmml/issues</url>
   </issueManagement>
   <properties>
-    <jpmml-sklearn.version>1.7.27</jpmml-sklearn.version>
+    <jpmml-sklearn.version>1.7.28</jpmml-sklearn.version>
   </properties>
   <dependencies>
     <dependency>
       <groupId>org.jpmml</groupId>
       <artifactId>pmml-sklearn</artifactId>
       <version>${jpmml-sklearn.version}</version>
       <exclusions>
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-lightgbm-1.4.4.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,48 +1,48 @@
-Zip file size: 68186 bytes, number of entries: 46
-drwxr-xr-x  2.0 unx        0 b- stor 22-Aug-31 12:48 META-INF/
--rw-r--r--  2.0 unx      159 b- defN 22-Aug-31 12:48 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 22-Aug-31 12:48 org/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Aug-31 12:48 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Aug-31 12:48 org/jpmml/lightgbm/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Aug-31 12:48 org/jpmml/lightgbm/testing/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Aug-31 12:48 org/jpmml/lightgbm/visitors/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Aug-31 12:48 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Aug-31 12:48 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Aug-31 12:48 META-INF/maven/org.jpmml/pmml-lightgbm/
--rw-rw-r--  2.0 unx     1264 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/Token.class
--rw-rw-r--  2.0 unx     2931 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/TokenMgrException.class
--rw-rw-r--  2.0 unx      817 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/PandasCategoricalParser$LookaheadSuccess.class
--rw-rw-r--  2.0 unx     4673 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/ObjectiveFunction.class
--rw-rw-r--  2.0 unx      839 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/BinaryCategoricalFeature.class
--rw-rw-r--  2.0 unx     2183 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/PoissonRegression.class
--rw-rw-r--  2.0 unx    18759 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/GBDT.class
--rw-rw-r--  2.0 unx     9950 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/LightGBMUtil.class
--rw-rw-r--  2.0 unx     1028 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/PandasCategoricalParserConstants.class
--rw-rw-r--  2.0 unx     1910 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/testing/LightGBMEncoderBatchTest.class
--rw-rw-r--  2.0 unx     4470 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/testing/LightGBMEncoderBatch.class
--rw-rw-r--  2.0 unx     1676 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/testing/LightGBMEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     4171 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/ParseException.class
--rw-rw-r--  2.0 unx    10481 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/PandasCategoricalParser.class
--rw-rw-r--  2.0 unx     1300 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/StreamProvider.class
--rw-rw-r--  2.0 unx     4456 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/visitors/TreeModelCompactor.class
--rw-rw-r--  2.0 unx     6672 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/SimpleCharStream.class
--rw-rw-r--  2.0 unx    13950 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/PandasCategoricalParserTokenManager.class
--rw-rw-r--  2.0 unx     1123 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/StringProvider.class
--rw-rw-r--  2.0 unx      584 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/DirectCategoricalFeature.class
--rw-rw-r--  2.0 unx     5189 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/Section.class
--rw-rw-r--  2.0 unx     2172 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/Regression.class
--rw-rw-r--  2.0 unx     3846 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/GBDT$1.class
--rw-rw-r--  2.0 unx      324 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/LightGBMEncoder.class
--rw-rw-r--  2.0 unx      255 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/PandasCategoricalParser$1.class
--rw-rw-r--  2.0 unx      221 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/Provider.class
--rw-rw-r--  2.0 unx     3516 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/MultinomialLogisticRegression.class
--rw-rw-r--  2.0 unx      609 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/Tree$1.class
--rw-rw-r--  2.0 unx     2506 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/BinomialLogisticRegression.class
--rw-rw-r--  2.0 unx     1059 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/HasLightGBMOptions.class
--rw-rw-r--  2.0 unx      529 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/PandasCategoricalParser$JJCalls.class
--rw-rw-r--  2.0 unx      389 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/Lambdarank.class
--rw-rw-r--  2.0 unx     2325 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/Classification.class
--rw-rw-r--  2.0 unx    13878 b- defN 22-Aug-31 12:48 org/jpmml/lightgbm/Tree.class
--rw-rw-r--  2.0 unx     2484 b- defN 22-Aug-31 12:48 META-INF/maven/org.jpmml/pmml-lightgbm/pom.xml
--rw-rw-r--  2.0 unx       57 b- defN 22-Aug-31 12:48 META-INF/maven/org.jpmml/pmml-lightgbm/pom.properties
-46 files, 132755 bytes uncompressed, 61102 bytes compressed:  54.0%
+Zip file size: 68173 bytes, number of entries: 46
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-08 20:17 META-INF/
+-rw-r--r--  2.0 unx      159 b- defN 23-Apr-08 20:17 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-08 20:17 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-08 20:17 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-08 20:17 org/jpmml/lightgbm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-08 20:17 org/jpmml/lightgbm/testing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-08 20:17 org/jpmml/lightgbm/visitors/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-08 20:17 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-08 20:17 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-08 20:17 META-INF/maven/org.jpmml/pmml-lightgbm/
+-rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/Token.class
+-rw-rw-r--  2.0 unx     2931 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/TokenMgrException.class
+-rw-rw-r--  2.0 unx      817 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/PandasCategoricalParser$LookaheadSuccess.class
+-rw-rw-r--  2.0 unx     4673 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/ObjectiveFunction.class
+-rw-rw-r--  2.0 unx      839 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/BinaryCategoricalFeature.class
+-rw-rw-r--  2.0 unx     2183 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/PoissonRegression.class
+-rw-rw-r--  2.0 unx    18747 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/GBDT.class
+-rw-rw-r--  2.0 unx     9950 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/LightGBMUtil.class
+-rw-rw-r--  2.0 unx     1028 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/PandasCategoricalParserConstants.class
+-rw-rw-r--  2.0 unx     1910 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/testing/LightGBMEncoderBatchTest.class
+-rw-rw-r--  2.0 unx     4470 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/testing/LightGBMEncoderBatch.class
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/testing/LightGBMEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     4171 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/ParseException.class
+-rw-rw-r--  2.0 unx    10481 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/PandasCategoricalParser.class
+-rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/StreamProvider.class
+-rw-rw-r--  2.0 unx     4456 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/visitors/TreeModelCompactor.class
+-rw-rw-r--  2.0 unx     6672 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/SimpleCharStream.class
+-rw-rw-r--  2.0 unx    13950 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/PandasCategoricalParserTokenManager.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/StringProvider.class
+-rw-rw-r--  2.0 unx      584 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/DirectCategoricalFeature.class
+-rw-rw-r--  2.0 unx     5189 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/Section.class
+-rw-rw-r--  2.0 unx     2172 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/Regression.class
+-rw-rw-r--  2.0 unx     3846 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/GBDT$1.class
+-rw-rw-r--  2.0 unx      324 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/LightGBMEncoder.class
+-rw-rw-r--  2.0 unx      255 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/PandasCategoricalParser$1.class
+-rw-rw-r--  2.0 unx      221 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/Provider.class
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/MultinomialLogisticRegression.class
+-rw-rw-r--  2.0 unx      609 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/Tree$1.class
+-rw-rw-r--  2.0 unx     2506 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/BinomialLogisticRegression.class
+-rw-rw-r--  2.0 unx     1059 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/HasLightGBMOptions.class
+-rw-rw-r--  2.0 unx      529 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/PandasCategoricalParser$JJCalls.class
+-rw-rw-r--  2.0 unx      389 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/Lambdarank.class
+-rw-rw-r--  2.0 unx     2325 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/Classification.class
+-rw-rw-r--  2.0 unx    13878 b- defN 23-Apr-08 20:17 org/jpmml/lightgbm/Tree.class
+-rw-rw-r--  2.0 unx     2486 b- defN 23-Apr-08 20:17 META-INF/maven/org.jpmml/pmml-lightgbm/pom.xml
+-rw-rw-r--  2.0 unx       57 b- defN 23-Apr-08 20:17 META-INF/maven/org.jpmml/pmml-lightgbm/pom.properties
+46 files, 132745 bytes uncompressed, 61089 bytes compressed:  54.0%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-LightGBM library
-Implementation-Version: 1.4.4
+Implementation-Version: 1.4.5
 Build-Jdk-Spec: 1.8
-Created-By: Maven JAR Plugin 3.2.2
+Created-By: Maven JAR Plugin 3.3.0
```

#### org/jpmml/lightgbm/GBDT.class

##### procyon -ec {}

```diff
@@ -151,17 +151,14 @@
             throw new IllegalArgumentException();
         }
         for (int i = 0; i < featureNames.length; ++i) {
             final String featureName = featureNames[i];
             final String featureInfo = featureInfos[i];
             if (LightGBMUtil.isNone(featureInfo)) {
                 features.add(null);
-                if (hasPandasCategories) {
-                    ++pandasCategoryIndex;
-                }
             }
             else {
                 Boolean binary = this.isBinary(i);
                 if (binary == null) {
                     binary = Boolean.FALSE;
                 }
                 Boolean categorical = this.isCategorical(i);
```

#### org/jpmml/lightgbm/GBDT$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum c9d09a1ca7c92966710cff878b10fa35efb81ca08cd45f3e0041aa7aec44dbc4
+  SHA-256 checksum 4c8fc371f54c7e629b56e7fe35844f0d8eff3ffb7955ebbc109a2663fc64c055
   Compiled from "GBDT.java"
 class org.jpmml.lightgbm.GBDT$1 extends java.lang.Object implements java.util.function.Function<org.jpmml.converter.Feature, org.jpmml.converter.Feature>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #33                         // org/jpmml/lightgbm/GBDT$1
   super_class: #34                        // java/lang/Object
@@ -239,20 +239,20 @@
         63: getfield      #4                  // Field val$featureInfos:[Ljava/lang/String;
         66: arraylength
         67: aload_0
         68: getfield      #10                 // Field features:Ljava/util/List;
         71: invokestatic  #11                 // Method org/jpmml/converter/SchemaUtil.checkSize:(ILjava/util/List;)V
         74: return
       LineNumberTable:
-        line 310: 0
-        line 312: 25
-        line 314: 39
-        line 317: 50
-        line 318: 62
-        line 319: 74
+        line 306: 0
+        line 308: 25
+        line 310: 39
+        line 313: 50
+        line 314: 62
+        line 315: 74
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      75     0  this   Lorg/jpmml/lightgbm/GBDT$1;
             0      75     1 this$0   Lorg/jpmml/lightgbm/GBDT;
 
   public org.jpmml.converter.Feature apply(org.jpmml.converter.Feature);
     descriptor: (Lorg/jpmml/converter/Feature;)Lorg/jpmml/converter/Feature;
@@ -392,46 +392,46 @@
        268: astore        8
        270: aload         8
        272: areturn
        273: aload_1
        274: invokevirtual #30                 // Method org/jpmml/converter/Feature.toContinuousFeature:()Lorg/jpmml/converter/ContinuousFeature;
        277: areturn
       LineNumberTable:
-        line 323: 0
-        line 324: 11
-        line 325: 15
-        line 328: 23
-        line 329: 30
-        line 331: 38
-        line 332: 48
-        line 333: 53
-        line 336: 63
-        line 337: 70
-        line 339: 76
-        line 340: 86
-        line 341: 99
-        line 344: 102
-        line 345: 112
-        line 346: 125
-        line 348: 140
-        line 350: 143
-        line 352: 146
-        line 353: 153
-        line 355: 159
-        line 356: 169
-        line 357: 182
-        line 359: 185
-        line 361: 188
-        line 362: 195
-        line 364: 201
-        line 365: 211
-        line 366: 224
-        line 368: 251
-        line 370: 270
-        line 374: 273
+        line 319: 0
+        line 320: 11
+        line 321: 15
+        line 324: 23
+        line 325: 30
+        line 327: 38
+        line 328: 48
+        line 329: 53
+        line 332: 63
+        line 333: 70
+        line 335: 76
+        line 336: 86
+        line 337: 99
+        line 340: 102
+        line 341: 112
+        line 342: 125
+        line 344: 140
+        line 346: 143
+        line 348: 146
+        line 349: 153
+        line 351: 159
+        line 352: 169
+        line 353: 182
+        line 355: 185
+        line 357: 188
+        line 358: 195
+        line 360: 201
+        line 361: 211
+        line 362: 224
+        line 364: 251
+        line 366: 270
+        line 370: 273
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
           140       3     9 categoricalFeature   Lorg/jpmml/converter/CategoricalFeature;
            76      67     6 binaryFeature   Lorg/jpmml/converter/BinaryFeature;
            86      57     7 binary   Ljava/lang/Boolean;
           112      31     8 categorical   Ljava/lang/Boolean;
           159      26     6 categoricalFeature   Lorg/jpmml/converter/CategoricalFeature;
@@ -470,15 +470,15 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: checkcast     #31                 // class org/jpmml/converter/Feature
          5: invokevirtual #32                 // Method apply:(Lorg/jpmml/converter/Feature;)Lorg/jpmml/converter/Feature;
          8: areturn
       LineNumberTable:
-        line 310: 0
+        line 306: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lorg/jpmml/lightgbm/GBDT$1;
 }
 Signature: #83                          // Ljava/lang/Object;Ljava/util/function/Function<Lorg/jpmml/converter/Feature;Lorg/jpmml/converter/Feature;>;
 SourceFile: "GBDT.java"
 EnclosingMethod: #87.#88                // org.jpmml.lightgbm.GBDT.toLightGBMSchema
```

#### META-INF/maven/org.jpmml/pmml-lightgbm/pom.xml

##### META-INF/maven/org.jpmml/pmml-lightgbm/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-lightgbm</artifactId>
-    <version>1.4.4</version>
+    <version>1.4.5</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-lightgbm</artifactId>
   <packaging>jar</packaging>
   <name>JPMML LightGBM converter</name>
   <description>JPMML LightGBM to PMML converter</description>
   <licenses>
@@ -38,15 +38,15 @@
     </dependency>
   </dependencies>
   <build>
     <plugins>
       <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-jar-plugin</artifactId>
-        <version>3.2.2</version>
+        <version>3.3.0</version>
         <configuration>
           <archive>
             <manifestEntries>
               <Implementation-Title>JPMML-LightGBM library</Implementation-Title>
               <Implementation-Version>${project.version}</Implementation-Version>
             </manifestEntries>
           </archive>
@@ -59,15 +59,15 @@
           <javadocVersion>1.8</javadocVersion>
           <sourcepath>${basedir}/src/main/java</sourcepath>
         </configuration>
       </plugin>
       <plugin>
         <groupId>org.codehaus.mojo</groupId>
         <artifactId>javacc-maven-plugin</artifactId>
-        <version>2.6</version>
+        <version>3.0.1</version>
         <executions>
           <execution>
             <goals>
               <goal>javacc</goal>
             </goals>
           </execution>
         </executions>
```

#### META-INF/maven/org.jpmml/pmml-lightgbm/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-lightgbm
 groupId=org.jpmml
-version=1.4.4
+version=1.4.5
```

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/serpent-1.40.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/serpent-1.40.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/jakarta.activation-2.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/resources/gson-2.10.jar` & `sklearn2pmml-0.92.2/sklearn2pmml/resources/gson-2.10.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/h2o.py` & `sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/xgboost.py` & `sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/lightgbm.py` & `sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/tree/chaid.py` & `sklearn2pmml-0.92.2/sklearn2pmml/tree/chaid.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.1/sklearn2pmml/expression/__init__.py` & `sklearn2pmml-0.92.2/sklearn2pmml/expression/__init__.py`

 * *Files identical despite different names*

