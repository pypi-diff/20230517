# Comparing `tmp/dcm-processor-1.0.5.tar.gz` & `tmp/dcm-processor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcm-processor-1.0.5.tar", last modified: Fri Apr 28 10:35:48 2023, max compression
+gzip compressed data, was "dcm-processor-1.1.0.tar", last modified: Wed May 17 12:42:37 2023, max compression
```

## Comparing `dcm-processor-1.0.5.tar` & `dcm-processor-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.782593 dcm-processor-1.0.5/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.0.5/LICENSE
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-28 10:35:48.784054 dcm-processor-1.0.5/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     5834 2023-04-17 10:06:58.000000 dcm-processor-1.0.5/README.md
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.230620 dcm-processor-1.0.5/dcm_processor/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.0.5/dcm_processor/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-04-15 09:02:58.000000 dcm-processor-1.0.5/dcm_processor/argparser.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    33102 2023-04-28 08:35:47.000000 dcm-processor-1.0.5/dcm_processor/files.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    46033 2023-04-19 12:36:49.000000 dcm-processor-1.0.5/dcm_processor/script.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.084754 dcm-processor-1.0.5/dcm_processor/services/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.080006 dcm-processor-1.0.5/dcm_processor/services/base/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.314612 dcm-processor-1.0.5/dcm_processor/services/base/module/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.556084 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/
--rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1551 2023-03-31 12:36:10.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.594050 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/config/
--rwxr-xr-x   0 giles     (1000) giles     (1000)    59497 2021-10-17 16:16:15.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
--rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/requirements.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/script.sh
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.621208 dcm-processor-1.0.5/dcm_processor/services/base/module/storageManager/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/storageManager/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       97 2021-10-17 16:16:20.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/storageManager/header_codes.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/storageManager/lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10198 2023-04-28 08:47:17.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/storageManager/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.650040 dcm-processor-1.0.5/dcm_processor/services/base/module/systemcleaner/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/systemcleaner/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3908 2023-04-28 08:48:28.000000 dcm-processor-1.0.5/dcm_processor/services/base/module/systemcleaner/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.655361 dcm-processor-1.0.5/dcm_processor/services/base/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      491 2023-04-28 08:35:17.000000 dcm-processor-1.0.5/dcm_processor/services/base/registry/__init__.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.092771 dcm-processor-1.0.5/dcm_processor/services/dcm2nii/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.762235 dcm-processor-1.0.5/dcm_processor/services/dcm2nii/module/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.0.5/dcm_processor/services/dcm2nii/module/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.0.5/dcm_processor/services/dcm2nii/module/dcm2niix
--rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.0.5/dcm_processor/services/dcm2nii/module/lib.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.778099 dcm-processor-1.0.5/dcm_processor/services/dcm2nii/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.0.5/dcm_processor/services/dcm2nii/registry/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)      288 2023-04-18 12:25:35.000000 dcm-processor-1.0.5/dcm_processor/services/dcm2nii/registry/settings.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6682 2023-04-21 16:23:38.000000 dcm-processor-1.0.5/dcm_processor/worker.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 10:35:48.283670 dcm-processor-1.0.5/dcm_processor.egg-info/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-28 10:35:42.000000 dcm-processor-1.0.5/dcm_processor.egg-info/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-04-28 10:35:46.000000 dcm-processor-1.0.5/dcm_processor.egg-info/SOURCES.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-04-28 10:35:42.000000 dcm-processor-1.0.5/dcm_processor.egg-info/dependency_links.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-04-28 10:35:42.000000 dcm-processor-1.0.5/dcm_processor.egg-info/entry_points.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-04-28 10:35:42.000000 dcm-processor-1.0.5/dcm_processor.egg-info/requires.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-04-28 10:35:42.000000 dcm-processor-1.0.5/dcm_processor.egg-info/top_level.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.0.5/pyproject.toml
--rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-04-28 10:35:48.789940 dcm-processor-1.0.5/setup.cfg
--rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.0.5/setup.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:37.149464 dcm-processor-1.1.0/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.1.0/LICENSE
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-05-17 12:42:37.150014 dcm-processor-1.1.0/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     5834 2023-04-17 10:06:58.000000 dcm-processor-1.1.0/README.md
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.720272 dcm-processor-1.1.0/dcm_processor/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.1.0/dcm_processor/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-04-15 09:02:58.000000 dcm-processor-1.1.0/dcm_processor/argparser.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    33214 2023-05-17 11:54:45.000000 dcm-processor-1.1.0/dcm_processor/files.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    46033 2023-04-19 12:36:49.000000 dcm-processor-1.1.0/dcm_processor/script.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.683831 dcm-processor-1.1.0/dcm_processor/services/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.681816 dcm-processor-1.1.0/dcm_processor/services/base/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.758424 dcm-processor-1.1.0/dcm_processor/services/base/module/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.966491 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1590 2023-05-12 10:21:10.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.976669 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/config/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    59797 2023-05-17 12:00:32.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/requirements.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/script.sh
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.991698 dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       95 2023-05-11 22:55:55.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/header_codes.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10622 2023-05-11 22:55:44.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:37.014549 dcm-processor-1.1.0/dcm_processor/services/base/module/systemcleaner/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/systemcleaner/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3908 2023-04-28 08:48:28.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/systemcleaner/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:37.019802 dcm-processor-1.1.0/dcm_processor/services/base/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      491 2023-04-28 08:35:17.000000 dcm-processor-1.1.0/dcm_processor/services/base/registry/__init__.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.686497 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:37.124060 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/dcm2niix
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/lib.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:37.145108 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/registry/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      288 2023-04-18 12:25:35.000000 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/registry/settings.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6682 2023-04-21 16:23:38.000000 dcm-processor-1.1.0/dcm_processor/worker.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.745532 dcm-processor-1.1.0/dcm_processor.egg-info/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-05-17 12:42:35.000000 dcm-processor-1.1.0/dcm_processor.egg-info/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-05-17 12:42:36.000000 dcm-processor-1.1.0/dcm_processor.egg-info/SOURCES.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-05-17 12:42:35.000000 dcm-processor-1.1.0/dcm_processor.egg-info/dependency_links.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-05-17 12:42:35.000000 dcm-processor-1.1.0/dcm_processor.egg-info/entry_points.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-05-17 12:42:35.000000 dcm-processor-1.1.0/dcm_processor.egg-info/requires.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-05-17 12:42:35.000000 dcm-processor-1.1.0/dcm_processor.egg-info/top_level.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.1.0/pyproject.toml
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-05-17 12:42:37.152834 dcm-processor-1.1.0/setup.cfg
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.1.0/setup.py
```

### Comparing `dcm-processor-1.0.5/LICENSE` & `dcm-processor-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/PKG-INFO` & `dcm-processor-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.0.5
+Version: 1.1.0
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dcm-processor-1.0.5/README.md` & `dcm-processor-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/argparser.py` & `dcm-processor-1.1.0/dcm_processor/argparser.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/files.py` & `dcm-processor-1.1.0/dcm_processor/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,22 +320,23 @@
 SCHEDULER_PORT=5000
 SCHEDULER_SETTINGS=/settings.json
 
 ORTHANC_REST_USERNAME=dcm-processor
 ORTHANC_REST_PASSWORD=dcm-processor
 ORTHANC_REST_URL=http://orthanc:8042
 ORTHANC_DEFUALT_STORE=pac
+ORTHANC_LOGLEVEL=2
 CLEAN_ORTHANC=0
 
 ORTHANC_DICOM_PORT=4242
 ORTHANC_BROWSER_PORT=8042
 DASHBOARD_PORT=5000
 SUPPORTED_MODALITY=CT,MR
-ACCEPTED_FILES=primary
-JUNK_FILES=sbi,surv,bersi,racker,ssde,results,mip,mono,spectal,scout,localizer,lokali,konturen,sectrareconstruction,zeffect,iodoinekein,smartplan,doseinf
+ACCEPTED_FILES=primary,original
+JUNK_FILES=derived,projection,sbi,surv,bersi,racker,ssde,results,mip,mono,spectal,scout,localizer,lokali,konturen,sectrareconstruction,zeffect,iodoinekein,smartplan,doseinf
 NO_PROXY=scheduler,orthanc,mongo,localhost,127.0.0.*
 
 JOBS_CONNECTION=mongodb://mongo:27017/
 JOBS_DBNAME=jobs
 JOBS_COLNAME=jobs
 DEFUALT_CHANNEL=default
 
@@ -430,27 +431,31 @@
     expose:
       - "4242"
       - "8042"
     ports:
       - ${ORTHANC_DICOM_PORT}:4242
       - ${ORTHANC_BROWSER_PORT}:8042
     volumes:
-      - orthanc-db:/var/lib/orthanc/db                # Persitent Orthanc DB
-      - orthanc-dblight:/var/lib/orthanc/dblight      # Persitent Orthanc DB
-      - ${BASEDIR}${DATA}:/tmp/nifti:rw               # Temp folder
+      - orthanc-db:/var/lib/orthanc/db
+      - orthanc-dblight:/var/lib/orthanc/dblight
+      - ${BASEDIR}${DATA}:/data:rw
+      - ${BASEDIR}${LOGS}:/logs:rw
     secrets:
       - orthanc.json
     environment:
       SCHEDULER_HOST: ${SCHEDULER_HOST}
       SCHEDULER_PORT: ${SCHEDULER_PORT}
       SUPPORTED_MODALITY: ${SUPPORTED_MODALITY}
       JUNK_FILES: ${JUNK_FILES}
       ACCEPTED_FILES: ${ACCEPTED_FILES}
       NO_PROXY: ${NO_PROXY}
       no_proxy: ${NO_PROXY}
+      DATA: /data
+      LOGS: /logs
+      LOGLEVEL: ${ORTHANC_LOGLEVEL}
 
 secrets:
   orthanc.json:
     file: ./orthanc.json
 """
 
 ORTHANC = """
@@ -495,17 +500,17 @@
   // Maximum number of patients that can be stored at a given time
   // in the storage (a value of "0" indicates no limit on the number
   // of patients)
   "MaximumPatientCount": 0,
 
   // List of paths to the custom Lua scripts that are to be loaded
   // into this instance of Orthanc
-
-  "PythonScript": "/scripts/Callback.py",
-  "PythonVerbose": false,
+  "LuaScripts": [
+    "/scripts/dicom_listener.lua"
+  ],
 
   // List of paths to the plugins that are to be loaded into this
   // instance of Orthanc (e.g. "./libPluginTest.so" for Linux, or
   // "./PluginTest.dll" for Windows). These paths can refer to
   // folders, in which case they will be scanned non-recursively to
   // find shared libraries. Backslashes must be either escaped by
   // doubling them, or replaced by forward slashes "/".
@@ -912,15 +917,16 @@
     // "7053,1003" : [ "ST", "Original Image Filename", 1, 1, "Philips PET Private Group" ]
     // "2001,5f" : [ "SQ", "StackSequence", 1, 1, "Philips Imaging DD 001" ]
     "0405,0010": ["LO", "Private data element", 1, 1, "DCM-PROCESSOR"],
     "0405,1001": ["ST", "Action", 1, 1, "DCM-PROCESSOR"],
     "0405,1003": ["ST", "ActionType", 1, 1, "DCM-PROCESSOR"],
     "0405,1005": ["ST", "ActionSource", 1, 1, "DCM-PROCESSOR"],
     "0405,1007": ["ST", "ActionDestination", 1, 1, "DCM-PROCESSOR"],
-    "0405,1009": ["ST", "ReferenceSeries", 1, 1, "DCM-PROCESSOR"]
+    "0405,1009": ["ST", "ReferenceSeries", 1, 1, "DCM-PROCESSOR"],
+    "0405,1011": ["ST", "DcmProcessorStatus", 1, 1, "DCM-PROCESSOR"]
   },
 
   // Whether to run DICOM C-Move operations synchronously. If set to
   // "false" (asynchronous mode), each incoming C-Move request results
   // in the creation of a new background job. Up to Orthanc 1.3.2, the
   // implicit behavior was to use synchronous C-Move ("true"). Between
   // Orthanc 1.4.0 and 1.4.2, the default behavior was set to
@@ -948,15 +954,15 @@
   "SaveJobs": true,
 
   // Specifies how Orthanc reacts when it receives a DICOM instance
   // whose SOPInstanceUID is already stored. If set to "true", the new
   // instance replaces the old one. If set to "false", the new
   // instance is discarded and the old one is kept. Up to Orthanc
   // 1.4.1, the implicit behavior corresponded to "false".
-  "OverwriteInstances": false,
+  "OverwriteInstances": true,
 
   // Maximum number of ZIP/media archives that are maintained by
   // Orthanc, as a response to the asynchronous creation of archives.
   // The least recently used archives get deleted as new archives are
   // generated. This option was introduced in Orthanc 1.5.0, and has
   // no effect on the synchronous generation of archives.
   "MediaArchiveSize": 1,
```

### Comparing `dcm-processor-1.0.5/dcm_processor/script.py` & `dcm-processor-1.1.0/dcm_processor/script.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 def anonymize(path, params=None):
   series = []
   for r, _, f in os.walk(path):
     for file in f:
       series.append(os.path.join(r,file))
 
+  if len(series) == 0:
+    return
+    
   ptid = pydicom.dcmread(series[0]).PatientID
   
   if os.path.isfile(pseudonyms_table):
     pseudonyms_dict = read_csv_table(pseudonyms_table)
       
   else:
     pseudonyms_dict = {}
```

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 <script>
  <p t="DATEINC">-137</p>
  <p t="PROFILENAME">DICOM-PS3.15E-Basic</p>
  <p t="PROJECTNAME">Project</p>
- <p t="SHORTNAME">Project</p>
+ <p t="SHORTNAME">DCM-Proc</p>
  <p t="SITEID">99</p>
- <p t="SITENAME">SiteName</p>
- <p t="TRIALNAME">Trial</p>
+ <p t="SITENAME">MRI</p>
+ <p t="TRIALNAME">NRAD</p>
  <p t="UIDROOT">9999</p>
  <e en="T" t="00080005" n="SpecificCharacterSet">@keep()</e>
- <e en="F" t="00080008" n="ImageType">@keep()</e>
+ <e en="F" t="00080008" n="ImageType"></e>
  <e en="T" t="00080012" n="InstanceCreationDate">@remove()</e>
  <e en="F" t="00080013" n="InstanceCreationTime"></e>
  <e en="T" t="00080014" n="InstanceCreatorUID">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="00080016" n="SOPClassUID">@keep()</e>
  <e en="T" t="00080018" n="SOPInstanceUID">@hashuid(@UIDROOT,this)</e>
- <e en="T" t="00080020" n="StudyDate">@modifydate(this,*,1,1)</e>
- <e en="T" t="00080021" n="SeriesDate">@modifydate(this,*,1,1)</e>
- <e en="T" t="00080022" n="AcquisitionDate">@modifydate(this,*,1,1)</e>
+ <e en="T" t="00080020" n="StudyDate">@keep()</e>
+ <e en="T" t="00080021" n="SeriesDate">@modifydate(this,*,*,1)</e>
+ <e en="T" t="00080022" n="AcquisitionDate">@modifydate(this,*,*,1)</e>
  <e en="T" t="00080023" n="ContentDate">@modifydate(this,*,1,1)</e>
  <e en="T" t="00080024" n="OverlayDate">@remove()</e>
  <e en="T" t="00080025" n="CurveDate">@remove()</e>
- <e en="T" t="0008002a" n="AcquisitionDatetime">@remove()</e>
- <e en="T" t="00080030" n="StudyTime">@empty()</e>
- <e en="T" t="00080031" n="SeriesTime">@remove()</e>
- <e en="T" t="00080032" n="AcquisitionTime">@remove()</e>
- <e en="T" t="00080033" n="ContentTime">@empty()</e>
- <e en="T" t="00080034" n="OverlayTime">@remove()</e>
- <e en="T" t="00080035" n="CurveTime">@remove()</e>
+ <e en="T" t="0008002a" n="AcquisitionDatetime">@modifydate(this,*,1,1)</e>
+ <e en="T" t="00080030" n="StudyTime">@remove()</e>
+ <e en="T" t="00080031" n="SeriesTime">@keep()</e>
+ <e en="T" t="00080032" n="AcquisitionTime">@keep()</e>
+ <e en="T" t="00080033" n="ContentTime">@keep()</e>
+ <e en="T" t="00080034" n="OverlayTime">@keep()</e>
+ <e en="T" t="00080035" n="CurveTime">@keep()</e>
  <e en="T" t="00080050" n="AccessionNumber">@hash(this,16)</e>
  <e en="F" t="00080052" n="QueryRetrieveLevel"></e>
  <e en="F" t="00080054" n="RetrieveAET"></e>
  <e en="F" t="00080056" n="InstanceAvailability"></e>
  <e en="T" t="00080058" n="FailedSOPInstanceUIDList">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="00080060" n="Modality">@require()</e>
  <e en="F" t="00080061" n="ModalitiesInStudy"></e>
@@ -179,19 +179,19 @@
  <e en="T" t="00120063" n="DeIdentificationMethod">@append(){CTP: @param(@PROFILENAME): @date():@time()}</e>
  <e en="F" t="00120064" n="DeIdentificationMethodCodeSeq"></e>
  <e en="T" t="00130010" n="BlockOwner">CTP</e>
  <e en="T" t="00131010" n="ProjectName">@param(@PROJECTNAME)</e>
  <e en="T" t="00131011" n="TrialName">@param(@TRIALNAME)</e>
  <e en="T" t="00131012" n="SiteName">@param(@SITENAME)</e>
  <e en="T" t="00131013" n="SiteID">@param(@SITEID)</e>
- <e en="T" t="00180010" n="ContrastBolusAgent">@empty()</e>
+ <e en="T" t="00180010" n="ContrastBolusAgent"></e>
  <e en="F" t="00180012" n="ContrastBolusAgentSeq"></e>
  <e en="F" t="00180014" n="ContrastBolusAdministrationRouteSeq"></e>
  <e en="T" t="00180015" n="BodyPartExamined">@require()</e>
- <e en="F" t="00180020" n="ScanningSeq"></e>
+ <e en="F" t="00180020" n="ScanningSeq">@keep()</e>
  <e en="F" t="00180021" n="SeqVariant"></e>
  <e en="F" t="00180022" n="ScanOptions"></e>
  <e en="F" t="00180023" n="MRAcquisitionType"></e>
  <e en="F" t="00180024" n="SequenceName"></e>
  <e en="F" t="00180025" n="AngioFlag"></e>
  <e en="F" t="00180026" n="InterventionDrugInformationSeq"></e>
  <e en="F" t="00180027" n="InterventionDrugStopTime"></e>
@@ -225,15 +225,15 @@
  <e en="F" t="00180088" n="SpacingBetweenSlices"></e>
  <e en="F" t="00180089" n="NumberOfPhaseEncodingSteps"></e>
  <e en="F" t="00180090" n="DataCollectionDiameter"></e>
  <e en="F" t="00180091" n="EchoTrainLength"></e>
  <e en="F" t="00180093" n="PercentSampling"></e>
  <e en="F" t="00180094" n="PercentPhaseFieldOfView"></e>
  <e en="F" t="00180095" n="PixelBandwidth"></e>
- <e en="T" t="00181000" n="DeviceSerialNumber">@remove()</e>
+ <e en="T" t="00181000" n="DeviceSerialNumber">@keep()</e>
  <e en="T" t="00181002" n="DeviceUID">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="00181004" n="PlateID">@remove()</e>
  <e en="T" t="00181005" n="GeneratorID">@remove()</e>
  <e en="T" t="00181007" n="CassetteID">@remove()</e>
  <e en="T" t="00181008" n="GantryID">@remove()</e>
  <e en="F" t="00181010" n="SecondaryCaptureDeviceID"></e>
  <e en="F" t="00181011" n="HardcopyCreationDeviceID"></e>
@@ -393,15 +393,15 @@
  <e en="F" t="00181702" n="CollimatorLeftVerticalEdge"></e>
  <e en="F" t="00181704" n="CollimatorRightVerticalEdge"></e>
  <e en="F" t="00181706" n="CollimatorUpperHorizontalEdge"></e>
  <e en="F" t="00181708" n="CollimatorLowerHorizontalEdge"></e>
  <e en="F" t="00181710" n="CenterOfCircularCollimator"></e>
  <e en="F" t="00181712" n="RadiusOfCircularCollimator"></e>
  <e en="F" t="00181720" n="VerticesOfPolygonalCollimator"></e>
- <e en="F" t="00181800" n="AcquisitionTimeSynchronized"></e>
+ <e en="F" t="00181800" n="AcquisitionTimeSynchronized">@modifydate(this,*,1,1)</e>
  <e en="F" t="00181801" n="TimeSource"></e>
  <e en="F" t="00181802" n="TimeDistributionProtocol"></e>
  <e en="T" t="00184000" n="AcquisitionComments">@remove()</e>
  <e en="F" t="00185000" n="OutputPower"></e>
  <e en="F" t="00185010" n="TransducerData"></e>
  <e en="F" t="00185012" n="FocusDepth"></e>
  <e en="F" t="00185020" n="ProcessingFunction"></e>
@@ -628,14 +628,16 @@
  <e en="F" t="00189231" n="MRAcquisitionPhaseEncodingStepsInPlane"></e>
  <e en="F" t="00189232" n="MRAcquisitionPhaseEncodingStepsOutOfPlane"></e>
  <e en="F" t="00189234" n="SpectroscopyAcquisitionPhaseColumns"></e>
  <e en="F" t="00189236" n="CardiacMotionStatus"></e>
  <e en="F" t="00189239" n="SpecificAbsorptionRateSeq"></e>
  <e en="T" t="00189424" n="AcquisitionProtocolDescription">@remove()</e>
  <e en="T" t="0018a003" n="ContributionDescription">@remove()</e>
+ <e en="T" t="00191092" n="OsteoRegressionLineSlope">@keep()</e>
+ <e en="T" t="00191093" n="OsteoRegressionLineIntercept">@keep()</e>
  <e en="T" t="0020000d" n="StudyInstanceUID">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="0020000e" n="SeriesInstanceUID">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="00200010" n="StudyID">@empty()</e>
  <e en="F" t="00200011" n="SeriesNumber"></e>
  <e en="F" t="00200012" n="AcquisitionNumber"></e>
  <e en="F" t="00200013" n="InstanceNumber"></e>
  <e en="F" t="00200019" n="ItemNumber"></e>
@@ -663,15 +665,15 @@
  <e en="F" t="00201204" n="NumberOfPatientRelatedInstances"></e>
  <e en="F" t="00201206" n="NumberOfStudyRelatedSeries"></e>
  <e en="F" t="00201208" n="NumberOfStudyRelatedInstances"></e>
  <e en="F" t="00201209" n="NumberOfSeriesRelatedInstances"></e>
  <e en="T" t="00203401" n="ModifyingDeviceID">@remove()</e>
  <e en="T" t="00203404" n="ModifyingDeviceManufacturer">@remove()</e>
  <e en="T" t="00203406" n="ModifiedImageDescription">@remove()</e>
- <e en="T" t="00204000" n="ImageComments">@remove()</e>
+ <e en="T" t="00204000" n="ImageComments"></e>
  <e en="F" t="00209056" n="StackID"></e>
  <e en="F" t="00209057" n="InStackPositionNumber"></e>
  <e en="F" t="00209071" n="FrameAnatomySeq"></e>
  <e en="F" t="00209072" n="FrameLaterality"></e>
  <e en="F" t="00209111" n="FrameContentSeq"></e>
  <e en="F" t="00209113" n="PlanePositionSeq"></e>
  <e en="F" t="00209116" n="PlaneOrientationSeq"></e>
@@ -796,15 +798,15 @@
  <e en="F" t="00321051" n="StudyCompletionTime"></e>
  <e en="F" t="00321055" n="StudyComponentStatusID"></e>
  <e en="T" t="00321060" n="RequestedProcedureDescription">@remove()</e>
  <e en="F" t="00321064" n="RequestedProcedureCodeSeq"></e>
  <e en="T" t="00321070" n="RequestedContrastAgent">@remove()</e>
  <e en="T" t="00324000" n="StudyComments">@remove()</e>
  <e en="F" t="00380004" n="RefPatientAliasSeq"></e>
- <e en="F" t="00380008" n="VisitStatusID"></e>
+ <e en="F" t="00380008" n="VisitStatusID">@remove()</e>
  <e en="T" t="00380010" n="AdmissionID">@remove()</e>
  <e en="T" t="00380011" n="IssuerOfAdmissionID">@remove()</e>
  <e en="F" t="00380016" n="RouteOfAdmissions"></e>
  <e en="T" t="0038001a" n="ScheduledAdmissionDate">@remove()</e>
  <e en="F" t="0038001b" n="ScheduledAdmissionTime"></e>
  <e en="T" t="0038001c" n="ScheduledDischargeDate">@remove()</e>
  <e en="F" t="0038001d" n="ScheduledDischargeTime"></e>
@@ -871,15 +873,15 @@
  <e en="T" t="00400244" n="PPSStartDate">@remove()</e>
  <e en="F" t="00400245" n="PPSStartTime"></e>
  <e en="T" t="00400248" n="PerformedStationNameCodeSeq">@remove()</e>
  <e en="T" t="00400250" n="PPSEndDate">@remove()</e>
  <e en="F" t="00400251" n="PPSEndTime"></e>
  <e en="F" t="00400252" n="PPSStatus"></e>
  <e en="T" t="00400253" n="PPSID">@remove()</e>
- <e en="T" t="00400254" n="PerformedProcedureStepDescription">@keep()</e>
+ <e en="T" t="00400254" n="PPSDescription">@remove()</e>
  <e en="F" t="00400255" n="PerformedProcedureTypeDescription"></e>
  <e en="F" t="00400260" n="PerformedProtocolCodeSeq"></e>
  <e en="F" t="00400270" n="ScheduledStepAttributesSeq"></e>
  <e en="T" t="00400275" n="RequestAttributesSeq">@remove()</e>
  <e en="T" t="00400280" n="PPSComments">@remove()</e>
  <e en="F" t="00400281" n="PPSDiscontinuationReasonCodeSeq"></e>
  <e en="F" t="00400293" n="QuantitySeq"></e>
@@ -1010,14 +1012,17 @@
  <e en="T" t="0070031a" n="FiducialUID">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="00880140" n="StorageMediaFilesetUID">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="00880200" n="IconImageSequence">@remove()</e>
  <e en="T" t="00880906" n="TopicSubject">@remove()</e>
  <e en="T" t="00880910" n="TopicAuthor">@remove()</e>
  <e en="T" t="00880912" n="TopicKeyWords">@remove()</e>
  <e en="T" t="04000100" n="DigitalSignatureUID">@hashuid(@UIDROOT,this)</e>
+ <e en="T" t="2005100c" n="PhilipsRescaleSlope">@keep()</e>
+ <e en="T" t="2005100d" n="PhilipsRescaleIntercept">@keep()</e>
+ <e en="T" t="2005100e" n="PhilipsScaleSlope">@keep()</e>
  <e en="T" t="20300020" n="TextString">@remove()</e>
  <e en="T" t="30060024" n="ReferencedFrameOfReferenceUID">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="300600c2" n="RelatedFrameOfReferenceUID">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="300a0013" n="DoseReferenceUID">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="40000010" n="Arbitrary">@remove()</e>
  <e en="T" t="40004000" n="TextComments">@remove()</e>
  <e en="T" t="40080042" n="ResultsIDIssuer">@remove()</e>
@@ -1039,8 +1044,8 @@
  <k en="T" t="0018">Keep group 0018</k>
  <k en="T" t="0020">Keep group 0020</k>
  <k en="T" t="0028">Keep group 0028</k>
  <r en="T" t="curves">Remove curves</r>
  <r en="T" t="overlays">Remove overlays</r>
  <r en="T" t="privategroups">Remove private groups</r>
  <r en="F" t="unspecifiedelements">Remove unchecked elements</r>
-</script>
+</script>
```

#### html2text {}

```diff
@@ -1 +0,0 @@
-
```

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/util.jar` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/util.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/DicomAnonymizerService/utils.py` & `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/utils.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/storageManager/lib.py` & `dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/storageManager/main.py` & `dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,27 +98,32 @@
         meta = requests.get(tag_url, auth=authOrthanc, headers=header)
         dicom_meta.append((str(tag).replace("-", "|"), meta.text))
         
       #Set Custom header
       dicom_meta += [("0405|0010", "DCM-PROCESSOR"), ("0405|1001", action), ("0405|1003", filefmt), ("0405|1005", "dcm-processor"), ("0405|1007", destination), ("0405|1009", seriesId)]
 
       #Set Series Description
-      dicom_meta.append(("0008|103e", "Processed Information"))
+      dicom_meta.append(("0008|103e", "dcm-processor-temp"))
+      actual_series_description = "Processed Information"
 
       h_codes = load_header_codes()
       for k in added_tags:
         if k in h_codes:
-          dicom_meta.append((h_codes[k], added_tags[k]))
+          if k == "SeriesDescription":
+            actual_series_description = added_tags[k]
+          else:
+            dicom_meta.append((h_codes[k], added_tags[k]))
+
 
       nifti_to_dicom(path, outpath ,dicom_meta)
 
       series_id = import_dicom_to_orthanc(outpath, url, ORTHANC_REST_USERNAME, ORTHANC_REST_PASSWORD)
       if (not series_id is None) and (not destination is None):
         time.sleep(2)
-        patch_series_private_meta(series_id, {"0405-0010": "DCM-PROCESSOR", "0405-1001": action, "0405-1003": filefmt, "0405-1005": "dcm-processor", "0405-1007": destination, "0405-1009": seriesId})
+        patch_series_private_meta(series_id, {"0405-0010": "DCM-PROCESSOR", "0405-1001": action, "0405-1003": filefmt, "0405-1005": "dcm-processor", "0405-1007": destination, "0405-1009": seriesId, "0008-103e": actual_series_description})
         
   os.system(f"rm -rf {outpath}")
 
 
 def post_dicom_to_orthanc(path, filefmt, destination ,added_tags, seriesId, base_folder, action="store-data"):
   header = {'content-type': 'application/json'}
   authOrthanc = (ORTHANC_REST_USERNAME, ORTHANC_REST_PASSWORD)
@@ -131,41 +136,47 @@
   if "Instances" in data:
     instances = data["Instances"]
     if len(instances) > 0:
       instanceId = str(instances[0])
       dicom_tags = requests.get(url + "/instances/" + instanceId + "/content", auth=authOrthanc, headers=header)
       tags = dicom_tags.json()
       dicom_meta = {}
+      
+      actual_series_description = ""
+
       for tag in tags:
         if tag not in COPY_TAGS:
           continue
 
         tag_url = f"{url}/instances/{instanceId}/content/{tag}"
         meta = requests.get(tag_url, auth=authOrthanc, headers=header)
         dicom_meta[str(tag)] = meta.text
 
       h_codes = load_header_codes()
       for k in added_tags:
         if k in h_codes:
           dicom_meta[h_codes[k]] = added_tags[k]
 
 
-      dicom_meta.update({"0405-0010": "DCM-PROCESSOR", "0405-1001": action, "0405-1003": filefmt, "0405-1005": "dcm-processor", "0405-1007": destination, "0405-1009": seriesId})
+      if "0008-103e" in dicom_meta:
+        actual_series_description = dicom_meta["0008-103e"]
+
+      dicom_meta.update({"0405-0010": "DCM-PROCESSOR", "0405-1001": action, "0405-1003": filefmt, "0405-1005": "dcm-processor", "0405-1007": destination, "0405-1009": seriesId, "0008-103e": "dcm-processor-temp"})
 
       output = os.path.join(base_folder, seriesId)
       os.system(f"mkdir -p {output}")
 
       load_and_update_meta(path, output, dicom_meta)
       series_id = import_dicom_to_orthanc(output, url, ORTHANC_REST_USERNAME, ORTHANC_REST_PASSWORD)
 
       os.system(f"rm -rf {output}")
 
       if (not series_id is None) and (not destination is None):
         time.sleep(2)
-        patch_series_private_meta(series_id, {"0405-0010": "DCM-PROCESSOR", "0405-1001": action, "0405-1003": filefmt, "0405-1005": "dcm-processor", "0405-1007": destination, "0405-1009": seriesId})
+        patch_series_private_meta(series_id, {"0405-0010": "DCM-PROCESSOR", "0405-1001": action, "0405-1003": filefmt, "0405-1005": "dcm-processor", "0405-1007": destination, "0405-1009": seriesId, "0008-103e": actual_series_description})
 
 
 def patch_series_private_meta(seriesId, tags):
   header = {'content-type': 'application/json'}
   authOrthanc = (ORTHANC_REST_USERNAME, ORTHANC_REST_PASSWORD)
   url = ORTHANC_REST_URL
```

### Comparing `dcm-processor-1.0.5/dcm_processor/services/base/module/systemcleaner/main.py` & `dcm-processor-1.1.0/dcm_processor/services/base/module/systemcleaner/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/dcm2nii/module/__init__.py` & `dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/dcm2nii/module/dcm2niix` & `dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/dcm2niix`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/services/dcm2nii/registry/__init__.py` & `dcm-processor-1.1.0/dcm_processor/services/dcm2nii/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor/worker.py` & `dcm-processor-1.1.0/dcm_processor/worker.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/dcm_processor.egg-info/PKG-INFO` & `dcm-processor-1.1.0/dcm_processor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.0.5
+Version: 1.1.0
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dcm-processor-1.0.5/dcm_processor.egg-info/SOURCES.txt` & `dcm-processor-1.1.0/dcm_processor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.5/setup.cfg` & `dcm-processor-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dcm-processor
-version = 1.0.5
+version = 1.1.0
 author = Giles Tetteh
 author_email = giles.tetteh@tum.de
 description = A Command line tool for the dicom processor library
 url = https://github.com/giesekow/dcm-processor-cli
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
```

