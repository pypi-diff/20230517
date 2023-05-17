# Comparing `tmp/commonroad-openscenario-converter-0.0.1.tar.gz` & `tmp/commonroad-openscenario-converter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad-openscenario-converter-0.0.1.tar", last modified: Wed May 10 10:35:01 2023, max compression
+gzip compressed data, was "commonroad-openscenario-converter-0.0.2.tar", last modified: Wed May 17 07:55:19 2023, max compression
```

## Comparing `commonroad-openscenario-converter-0.0.1.tar` & `commonroad-openscenario-converter-0.0.2.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-10 10:35:01.879716 commonroad-openscenario-converter-0.0.1/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/LICENSE
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-05-10 10:35:01.879716 commonroad-openscenario-converter-0.0.1/PKG-INFO
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3512 2023-05-10 07:57:22.000000 commonroad-openscenario-converter-0.0.1/README.md
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-10 10:35:01.875716 commonroad-openscenario-converter-0.0.1/commonroad_openscenario_converter.egg-info/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-05-10 10:35:01.000000 commonroad-openscenario-converter-0.0.1/commonroad_openscenario_converter.egg-info/PKG-INFO
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1474 2023-05-10 10:35:01.000000 commonroad-openscenario-converter-0.0.1/commonroad_openscenario_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-05-10 10:35:01.000000 commonroad-openscenario-converter-0.0.1/commonroad_openscenario_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      166 2023-05-10 10:35:01.000000 commonroad-openscenario-converter-0.0.1/commonroad_openscenario_converter.egg-info/requires.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       23 2023-05-10 10:35:01.000000 commonroad-openscenario-converter-0.0.1/commonroad_openscenario_converter.egg-info/top_level.txt
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-10 10:35:01.875716 commonroad-openscenario-converter-0.0.1/osc_cr_converter/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-10 10:35:01.875716 commonroad-openscenario-converter-0.0.1/osc_cr_converter/analyzer/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/analyzer/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4190 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/analyzer/base.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1242 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/analyzer/error.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      756 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/analyzer/error_analyzer.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      482 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/analyzer/result.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-10 10:35:01.875716 commonroad-openscenario-converter-0.0.1/osc_cr_converter/batch/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/batch/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    18497 2023-05-09 11:24:57.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/batch/analysis.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5787 2023-05-09 09:30:26.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/batch/converter.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-10 10:35:01.879716 commonroad-openscenario-converter-0.0.1/osc_cr_converter/converter/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/converter/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1375 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/converter/base.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    22393 2023-05-10 07:31:51.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/converter/osc2cr.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3076 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/converter/result.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1872 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/converter/serializable.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-10 10:35:01.879716 commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2836 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/abs_rel.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6758 2023-05-09 08:57:31.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/configuration.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1876 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/general.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3952 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/obstacle_info.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3610 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/pps.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      984 2023-05-09 08:11:46.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/statistics.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3455 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/visualization.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-10 10:35:01.879716 commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-10 10:35:01.879716 commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/esmini/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/esmini/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10620 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    14758 2023-05-10 09:14:09.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/esmini/esmini_wrapper.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4868 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      995 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/esmini/storyboard_element.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-05-10 10:35:01.883716 commonroad-openscenario-converter-0.0.1/setup.cfg
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1059 2023-05-10 10:34:47.000000 commonroad-openscenario-converter-0.0.1/setup.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-10 10:35:01.879716 commonroad-openscenario-converter-0.0.1/tests/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.1/tests/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1937 2023-05-09 12:06:26.000000 commonroad-openscenario-converter-0.0.1/tests/test_conversion.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/LICENSE
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/PKG-INFO
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4237 2023-05-17 07:37:55.000000 commonroad-openscenario-converter-0.0.2/README.md
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-05-17 07:55:19.000000 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-05-17 07:55:19.000000 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-05-17 07:55:19.000000 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      181 2023-05-17 07:55:19.000000 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/requires.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       23 2023-05-17 07:55:19.000000 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/top_level.txt
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4190 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/base.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1242 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/error.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      756 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/error_analyzer.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      482 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/result.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    18497 2023-05-09 11:24:57.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/analysis.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5787 2023-05-09 09:30:26.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/converter.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1375 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/base.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    22393 2023-05-10 07:31:51.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/osc2cr.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3076 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/result.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1872 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/serializable.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/udp_driver/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/udp_driver/__init__.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     4494 2023-05-17 07:35:27.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/udp_driver/common.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2836 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/abs_rel.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6758 2023-05-09 08:57:31.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/configuration.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1876 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/general.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3952 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/obstacle_info.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3610 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/pps.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      984 2023-05-09 08:11:46.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/statistics.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3455 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/visualization.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10620 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    14812 2023-05-16 09:23:37.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_wrapper.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4868 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      995 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/storyboard_element.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/setup.cfg
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1086 2023-05-17 07:43:14.000000 commonroad-openscenario-converter-0.0.2/setup.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/tests/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/tests/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1937 2023-05-09 12:06:26.000000 commonroad-openscenario-converter-0.0.2/tests/test_conversion.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      194 2023-05-16 14:12:02.000000 commonroad-openscenario-converter-0.0.2/tests/test_udp.py
```

### Comparing `commonroad-openscenario-converter-0.0.1/LICENSE` & `commonroad-openscenario-converter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/PKG-INFO` & `commonroad-openscenario-converter-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-openscenario-converter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converter between OpenSCENARIO and CommonRoad formats
 Author: Yuanfei Lin, Michael Ratzel
 Author-email: yuanfei.lin@tum.de
 License: BSD 3-Clause
 Keywords: scenario description,autonomous driving
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `commonroad-openscenario-converter-0.0.1/README.md` & `commonroad-openscenario-converter-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 ![image info](./docs/figures/converter-banner.gif)
 
 Automatic Traffic Scenario Conversion between [OpenSCENARIO](https://www.asam.net/standards/detail/openscenario/)
 and [CommonRoad](commonroad.in.tum.de/). Currently, only the conversion from **O**pen**SC**ENARIO to **C**ommon**R**OAD (osc2cr) is developed.<br>
 [![Linux](https://svgshare.com/i/Zhy.svg?style=plastic)](https://svgshare.com/i/Zhy.svg)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/commonroad-openscenario-converter.svg)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)
 [![PyPI license](https://img.shields.io/pypi/l/commonroad-openscenario-converter.svg)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)
-[![PyPI version fury.io](https://badge.fury.io/py/commonroad-openscenario-converter.svg?style=plastic)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)<br>
+[![PyPI version fury.io](https://badge.fury.io/py/commonroad-openscenario-converter.svg)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)<br>
+[![PyPI download month](https://img.shields.io/pypi/dm/commonroad-openscenario-converter.svg?style=plastic&label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-openscenario-converter/) 
+[![PyPI download week](https://img.shields.io/pypi/dw/commonroad-openscenario-converter.svg?style=plastic&label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)<br>
+
 ### Using the Converter
 The recommended way of installation if you only want to use the OpenSCENARIO-CommonROAD Converter
 (i.e., you do not want to work with the code directly) is to use the PyPI package:
 ```bash
 pip install commonroad-openscenario-converter
 ```
 ### Development
@@ -35,14 +38,20 @@
 ```
 
 - To test the installition, run unittest:
 ```bash
 $ cd tests
 $ python -m unittest -v
 ```
+
+### Open Simulation Interface (OSI) and UDP Driver
+If you want to use the [esmini](https://github.com/esmini/esmini) UDPDriverController in combination with OSI for including
+external driver models or vehicle simulators, you need to install OSI manually, 
+see [here](https://github.com/OpenSimulationInterface/open-simulation-interface).
+
 ### Contributors (in alphabetical order by last name)
 - Yuanfei Lin
 - Michael Ratzel
 
 ### Acknowledgments
 We would like to extend our heartfelt gratitude to the team behind [esmini](https://github.com/esmini/esmini) for 
 their remarkable effort in developing the simulation tool. Specifically, we would like to express our sincere
```

### Comparing `commonroad-openscenario-converter-0.0.1/commonroad_openscenario_converter.egg-info/PKG-INFO` & `commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-openscenario-converter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converter between OpenSCENARIO and CommonRoad formats
 Author: Yuanfei Lin, Michael Ratzel
 Author-email: yuanfei.lin@tum.de
 License: BSD 3-Clause
 Keywords: scenario description,autonomous driving
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `commonroad-openscenario-converter-0.0.1/commonroad_openscenario_converter.egg-info/SOURCES.txt` & `commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 osc_cr_converter/batch/analysis.py
 osc_cr_converter/batch/converter.py
 osc_cr_converter/converter/__init__.py
 osc_cr_converter/converter/base.py
 osc_cr_converter/converter/osc2cr.py
 osc_cr_converter/converter/result.py
 osc_cr_converter/converter/serializable.py
+osc_cr_converter/udp_driver/__init__.py
+osc_cr_converter/udp_driver/common.py
 osc_cr_converter/utility/__init__.py
 osc_cr_converter/utility/abs_rel.py
 osc_cr_converter/utility/configuration.py
 osc_cr_converter/utility/general.py
 osc_cr_converter/utility/obstacle_info.py
 osc_cr_converter/utility/pps.py
 osc_cr_converter/utility/statistics.py
@@ -31,8 +33,9 @@
 osc_cr_converter/wrapper/__init__.py
 osc_cr_converter/wrapper/esmini/__init__.py
 osc_cr_converter/wrapper/esmini/esmini_scenario_object.py
 osc_cr_converter/wrapper/esmini/esmini_wrapper.py
 osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py
 osc_cr_converter/wrapper/esmini/storyboard_element.py
 tests/__init__.py
-tests/test_conversion.py
+tests/test_conversion.py
+tests/test_udp.py
```

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/analyzer/base.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/analyzer/error.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/error.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/analyzer/error_analyzer.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/error_analyzer.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/batch/analysis.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/analysis.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/batch/converter.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/converter.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/converter/base.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/base.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/converter/osc2cr.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/osc2cr.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/converter/result.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/result.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/converter/serializable.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/serializable.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/abs_rel.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/abs_rel.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/configuration.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/configuration.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/general.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/general.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/obstacle_info.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/obstacle_info.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/pps.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/pps.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/statistics.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/statistics.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/utility/visualization.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/visualization.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/esmini/esmini_wrapper.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
     @log_to_file.setter
     def log_to_file(self, new_log_to_file: Union[None, bool, str]):
         if new_log_to_file is None:
             self._log_to_file = None
         elif isinstance(new_log_to_file, bool):
             if new_log_to_file:
-                log_dir =  os.path.dirname(os.path.realpath(__file__)) + "/../../../output/log"
+                log_dir = os.path.dirname(os.path.realpath(__file__)) + "/../../../output/log"
                 os.makedirs(log_dir, exist_ok=True)  # create directory if it doesn't exist
                 self._log_to_file = os.path.join(log_dir,
                                                  "{}.txt".format(datetime.now().isoformat(sep="_", timespec="seconds")))
                 warnings.warn(f"Using default log file {self._log_to_file}")
             else:
                 self._log_to_file = None
         elif path.exists(path.dirname(new_log_to_file)):
@@ -293,14 +293,16 @@
             int(0)
         )
         if ret != 0:
             return False
 
         self.esmini_lib.SE_SetSeed(self.random_seed)
 
+        self.esmini_lib.SE_OpenOSISocket("127.0.0.1")
+
         self._callback_functor = ct.CFUNCTYPE(None, ct.c_char_p, ct.c_int, ct.c_int)(self.__state_change_callback)
         self.esmini_lib.SE_RegisterStoryBoardElementStateChangeCallback(self._callback_functor)
         self._scenario_engine_initialized = True
         return True
 
     def _set_set_window_size(self, window_size: EsminiParams.WindowSize):
         self.esmini_lib.SE_SetWindowPosAndSize(window_size.x, window_size.y, window_size.width, window_size.height)
```

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/osc_cr_converter/wrapper/esmini/storyboard_element.py` & `commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/storyboard_element.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.1/setup.py` & `commonroad-openscenario-converter-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='commonroad-openscenario-converter',
-      version='0.0.1',
+      version='0.0.2',
       description='Converter between OpenSCENARIO and CommonRoad formats',
       keywords="scenario description, autonomous driving",
       author='Yuanfei Lin, Michael Ratzel',
       author_email='yuanfei.lin@tum.de',
       license='BSD 3-Clause',
       packages=find_packages(),
       install_requires=[
           'commonroad-io>=2023.1',
           'commonroad-scenario-designer>=0.7.0',
           'matplotlib>=3.5.2',
           'imageio>=2.28.1',
           'numpy>=1.19.0',
           'tqdm>=4.65.0',
           'scenariogeneration>=0.9.0',
+          'protobuf>=3.19'
       ],
       extras_require={
           'tests': [
               'pytest>=7.1'
           ]
       },
       classifiers=[
```

### Comparing `commonroad-openscenario-converter-0.0.1/tests/test_conversion.py` & `commonroad-openscenario-converter-0.0.2/tests/test_conversion.py`

 * *Files identical despite different names*

