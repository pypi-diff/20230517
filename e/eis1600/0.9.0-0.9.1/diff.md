# Comparing `tmp/eis1600-0.9.0.tar.gz` & `tmp/eis1600-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.9.0.tar", last modified: Thu May 11 10:51:08 2023, max compression
+gzip compressed data, was "eis1600-0.9.1.tar", last modified: Wed May 17 10:40:47 2023, max compression
```

## Comparing `eis1600-0.9.0.tar` & `eis1600-0.9.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.308791 eis1600-0.9.0/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.0/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-05-11 10:51:08.308791 eis1600-0.9.0/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7640 2023-05-11 10:42:54.000000 eis1600-0.9.0/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.296791 eis1600-0.9.0/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.0/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.300792 eis1600-0.9.0/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.0/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.0/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.9.0/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.9.0/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.300792 eis1600-0.9.0/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.9.0/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5877 2023-05-05 07:34:23.000000 eis1600-0.9.0/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.0/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.300792 eis1600-0.9.0/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.0/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.0/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      482 2023-03-23 10:19:45.000000 eis1600-0.9.0/eis1600/gazetteers/data/regions_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.0/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   218682 2023-04-27 07:51:31.000000 eis1600-0.9.0/eis1600/gazetteers/data/toponyms.csv
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.304792 eis1600-0.9.0/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      730 2023-04-27 07:54:20.000000 eis1600-0.9.0/eis1600/helper/EntityTags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.0/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.0/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.0/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.304792 eis1600-0.9.0/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.0/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      256 2023-04-19 13:02:11.000000 eis1600-0.9.0/eis1600/helper/data/entity_tags.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.9.0/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.9.0/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.0/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3739 2023-04-20 08:46:34.000000 eis1600-0.9.0/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.0/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11231 2023-05-11 10:42:54.000000 eis1600-0.9.0/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      598 2023-04-26 15:20:40.000000 eis1600-0.9.0/eis1600/helper/yml_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1335 2023-05-11 10:36:39.000000 eis1600-0.9.0/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.304792 eis1600-0.9.0/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.0/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.0/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.9.0/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.9.0/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12991 2023-05-04 08:54:08.000000 eis1600-0.9.0/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.9.0/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.9.0/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.304792 eis1600-0.9.0/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.9.0/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8819 2023-05-10 14:51:01.000000 eis1600-0.9.0/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.0/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2778 2023-05-11 10:36:39.000000 eis1600-0.9.0/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.9.0/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.9.0/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7584 2023-05-10 14:48:27.000000 eis1600-0.9.0/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.308791 eis1600-0.9.0/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.0/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.9.0/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3682 2023-05-11 10:36:39.000000 eis1600-0.9.0/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.9.0/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.308791 eis1600-0.9.0/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.0/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1663 2023-05-11 10:36:39.000000 eis1600-0.9.0/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10489 2023-05-04 08:54:08.000000 eis1600-0.9.0/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.0/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.308791 eis1600-0.9.0/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.0/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.9.0/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-21 13:13:53.000000 eis1600-0.9.0/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.308791 eis1600-0.9.0/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.0/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.0/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.0/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.300792 eis1600-0.9.0/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1959 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-05-11 10:51:08.308791 eis1600-0.9.0/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2297 2023-05-11 10:50:52.000000 eis1600-0.9.0/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.856145 eis1600-0.9.1/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.1/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-05-17 10:40:47.856145 eis1600-0.9.1/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7640 2023-05-11 10:42:54.000000 eis1600-0.9.1/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.844145 eis1600-0.9.1/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.1/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.844145 eis1600-0.9.1/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.1/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.1/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.9.1/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.9.1/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.844145 eis1600-0.9.1/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.9.1/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5877 2023-05-05 07:34:23.000000 eis1600-0.9.1/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.1/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.848145 eis1600-0.9.1/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.1/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.1/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      482 2023-03-23 10:19:45.000000 eis1600-0.9.1/eis1600/gazetteers/data/regions_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.1/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   218682 2023-04-27 07:51:31.000000 eis1600-0.9.1/eis1600/gazetteers/data/toponyms.csv
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.848145 eis1600-0.9.1/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      730 2023-04-27 07:54:20.000000 eis1600-0.9.1/eis1600/helper/EntityTags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.1/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.1/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.1/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.848145 eis1600-0.9.1/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.1/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      256 2023-04-19 13:02:11.000000 eis1600-0.9.1/eis1600/helper/data/entity_tags.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.9.1/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.9.1/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.1/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3739 2023-04-20 08:46:34.000000 eis1600-0.9.1/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.1/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11231 2023-05-11 10:42:54.000000 eis1600-0.9.1/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      598 2023-04-26 15:20:40.000000 eis1600-0.9.1/eis1600/helper/yml_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1421 2023-05-17 10:37:30.000000 eis1600-0.9.1/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.852145 eis1600-0.9.1/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.1/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.1/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.9.1/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.9.1/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12991 2023-05-04 08:54:08.000000 eis1600-0.9.1/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.9.1/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.9.1/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.852145 eis1600-0.9.1/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-05-12 10:15:49.000000 eis1600-0.9.1/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8819 2023-05-12 10:15:37.000000 eis1600-0.9.1/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.1/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2786 2023-05-12 09:46:15.000000 eis1600-0.9.1/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.9.1/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.9.1/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7584 2023-05-10 14:48:27.000000 eis1600-0.9.1/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.852145 eis1600-0.9.1/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.1/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.9.1/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3690 2023-05-12 09:46:15.000000 eis1600-0.9.1/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.9.1/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.852145 eis1600-0.9.1/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.1/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1671 2023-05-12 09:46:15.000000 eis1600-0.9.1/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10489 2023-05-04 08:54:08.000000 eis1600-0.9.1/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.1/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.852145 eis1600-0.9.1/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.1/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.9.1/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-21 13:13:53.000000 eis1600-0.9.1/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.852145 eis1600-0.9.1/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.1/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.1/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.1/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:40:47.844145 eis1600-0.9.1/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-05-17 10:40:47.000000 eis1600-0.9.1/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1959 2023-05-17 10:40:47.000000 eis1600-0.9.1/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-05-17 10:40:47.000000 eis1600-0.9.1/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-05-17 10:40:47.000000 eis1600-0.9.1/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-05-17 10:40:47.000000 eis1600-0.9.1/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-05-17 10:40:47.000000 eis1600-0.9.1/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-05-17 10:40:47.856145 eis1600-0.9.1/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2297 2023-05-12 09:46:15.000000 eis1600-0.9.1/setup.py
```

### Comparing `eis1600-0.9.0/LICENSE` & `eis1600-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/PKG-INFO` & `eis1600-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.0
+Version: 0.9.1
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.9.0/README.md` & `eis1600-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/dates/Date.py` & `eis1600-0.9.1/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/dates/date_patterns.py` & `eis1600-0.9.1/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/dates/methods.py` & `eis1600-0.9.1/eis1600/dates/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/gazetteers/Onomastics.py` & `eis1600-0.9.1/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/gazetteers/Toponyms.py` & `eis1600-0.9.1/eis1600/gazetteers/Toponyms.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-0.9.1/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-0.9.1/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/gazetteers/data/toponyms.csv` & `eis1600-0.9.1/eis1600/gazetteers/data/toponyms.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/helper/EntityTags.py` & `eis1600-0.9.1/eis1600/helper/EntityTags.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/helper/Singleton.py` & `eis1600-0.9.1/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/helper/ar_normalization.py` & `eis1600-0.9.1/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.9.1/eis1600/helper/fix_miu_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/helper/markdown_methods.py` & `eis1600-0.9.1/eis1600/helper/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/helper/markdown_patterns.py` & `eis1600-0.9.1/eis1600/helper/markdown_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/helper/miu_random_revisions.py` & `eis1600-0.9.1/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/helper/repo.py` & `eis1600-0.9.1/eis1600/helper/repo.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/helper/yml_methods.py` & `eis1600-0.9.1/eis1600/helper/yml_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/helper/yml_to_json.py` & `eis1600-0.9.1/eis1600/helper/yml_to_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from pathlib import Path
 import jsonpickle
 from p_tqdm import p_uimap
 
 from eis1600.processing.preprocessing import get_yml
-from helper.repo import MC_REPO, TRAINING_DATA_REPO
+from eis1600.helper.repo import MC_REPO, TRAINING_DATA_REPO
 
 
 def main():
     arg_parser = ArgumentParser(
             prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to generate JSON from MIU YAMLHeaders.'''
     )
@@ -31,12 +31,15 @@
     else:
         res = p_uimap(get_yml, infiles)
 
     yml_dict = {}
     for path, yml in res:
         yml_dict[path] = yml.to_json()
 
+    print(yml_dict)
+
     with open(MC_REPO + 'masterchronicleapp/src/data.json', 'w', encoding='utf-8') as fh:
+        jsonpickle.set_encoder_options('json', indent=4)
         json_str = jsonpickle.encode(yml_dict, unpicklable=False)
         fh.write(json_str)
 
     print('Done')
```

### Comparing `eis1600-0.9.0/eis1600/markdown/UIDs.py` & `eis1600-0.9.1/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.9.1/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/markdown/insert_uids.py` & `eis1600-0.9.1/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/markdown/methods.py` & `eis1600-0.9.1/eis1600/markdown/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/markdown/update_uids.py` & `eis1600-0.9.1/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.9.1/eis1600/markdown/update_uids_old_process.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/miu/HeadingTracker.py` & `eis1600-0.9.1/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/miu/YAMLHandler.py` & `eis1600-0.9.1/eis1600/miu/YAMLHandler.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.9.1/eis1600/miu/disassemble_into_miu_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from p_tqdm import p_uimap
 from tqdm import tqdm
 
 from eis1600.helper.repo import get_path_to_other_repo, read_files_from_autoreport, get_files_from_eis1600_dir, \
     write_to_readme
 from eis1600.miu.methods import disassemble_text
-from helper.repo import TEXT_REPO
+from eis1600.helper.repo import TEXT_REPO
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
         if input_arg and os.path.isfile(input_arg):
             filepath, fileext = os.path.splitext(input_arg)
             if fileext != '.EIS1600':
```

### Comparing `eis1600-0.9.0/eis1600/miu/methods.py` & `eis1600-0.9.1/eis1600/miu/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.9.1/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/miu/yml_handling.py` & `eis1600-0.9.1/eis1600/miu/yml_handling.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/nlp/cameltools.py` & `eis1600-0.9.1/eis1600/nlp/cameltools.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.9.1/eis1600/nlp/ner_annotate_mius.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from eis1600.helper.logging import setup_logger
 from p_tqdm import p_uimap
 from tqdm import tqdm
 
 from eis1600.helper.repo import get_files_from_eis1600_dir, read_files_from_readme
 from eis1600.miu.methods import annotate_miu_file, get_mius
-from helper.repo import MIU_REPO
+from eis1600.helper.repo import MIU_REPO
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
         if input_arg and os.path.isfile(input_arg):
             filepath, fileext = os.path.splitext(input_arg)
             if fileext != '.IDs' and fileext != '.EIS1600':
```

### Comparing `eis1600-0.9.0/eis1600/nlp/utils.py` & `eis1600-0.9.1/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/onomastics/annotation.py` & `eis1600-0.9.1/eis1600/onomastics/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from functools import partial
 
 from eis1600.helper.logging import setup_logger
 from p_tqdm import p_uimap
 
 from eis1600.onomastics.methods import nasab_annotation
-from helper.repo import GAZETTEERS_REPO, TRAINING_DATA_REPO
+from eis1600.helper.repo import GAZETTEERS_REPO, TRAINING_DATA_REPO
 
 
 def main():
     arg_parser = ArgumentParser(
             prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to annotate onomastic information in gold-standard MIUs.'''
     )
```

### Comparing `eis1600-0.9.0/eis1600/onomastics/methods.py` & `eis1600-0.9.1/eis1600/onomastics/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/onomastics/re_pattern.py` & `eis1600-0.9.1/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/processing/postprocessing.py` & `eis1600-0.9.1/eis1600/processing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/processing/preprocessing.py` & `eis1600-0.9.1/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/stats/methods.py` & `eis1600-0.9.1/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600/stats/miu_stats.py` & `eis1600-0.9.1/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600.egg-info/PKG-INFO` & `eis1600-0.9.1/eis1600.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.0
+Version: 0.9.1
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.9.0/eis1600.egg-info/SOURCES.txt` & `eis1600-0.9.1/eis1600.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/eis1600.egg-info/entry_points.txt` & `eis1600-0.9.1/eis1600.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.0/setup.py` & `eis1600-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.9.0',
+      version='0.9.1',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
```

