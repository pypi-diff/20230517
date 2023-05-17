# Comparing `tmp/commonroad-openscenario-converter-0.0.2.tar.gz` & `tmp/commonroad-openscenario-converter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad-openscenario-converter-0.0.2.tar", last modified: Wed May 17 07:55:19 2023, max compression
+gzip compressed data, was "commonroad-openscenario-converter-0.0.3.tar", last modified: Wed May 17 13:36:37 2023, max compression
```

## Comparing `commonroad-openscenario-converter-0.0.2.tar` & `commonroad-openscenario-converter-0.0.3.tar`

### file list

```diff
@@ -1,54 +1,59 @@
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/LICENSE
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/PKG-INFO
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4237 2023-05-17 07:37:55.000000 commonroad-openscenario-converter-0.0.2/README.md
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-05-17 07:55:19.000000 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/PKG-INFO
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-05-17 07:55:19.000000 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-05-17 07:55:19.000000 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      181 2023-05-17 07:55:19.000000 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/requires.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       23 2023-05-17 07:55:19.000000 commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/top_level.txt
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4190 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/base.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1242 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/error.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      756 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/error_analyzer.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      482 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/result.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    18497 2023-05-09 11:24:57.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/analysis.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5787 2023-05-09 09:30:26.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/converter.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1375 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/base.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    22393 2023-05-10 07:31:51.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/osc2cr.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3076 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/result.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1872 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/serializable.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.595547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/udp_driver/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/udp_driver/__init__.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     4494 2023-05-17 07:35:27.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/udp_driver/common.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2836 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/abs_rel.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6758 2023-05-09 08:57:31.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/configuration.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1876 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/general.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3952 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/obstacle_info.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3610 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/pps.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      984 2023-05-09 08:11:46.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/statistics.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3455 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/visualization.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10620 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    14812 2023-05-16 09:23:37.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_wrapper.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4868 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      995 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/storyboard_element.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/setup.cfg
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1086 2023-05-17 07:43:14.000000 commonroad-openscenario-converter-0.0.2/setup.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 07:55:19.599547 commonroad-openscenario-converter-0.0.2/tests/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.2/tests/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1937 2023-05-09 12:06:26.000000 commonroad-openscenario-converter-0.0.2/tests/test_conversion.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      194 2023-05-16 14:12:02.000000 commonroad-openscenario-converter-0.0.2/tests/test_udp.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/LICENSE
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/PKG-INFO
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4237 2023-05-17 09:16:36.000000 commonroad-openscenario-converter-0.0.3/README.md
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.510572 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-05-17 13:36:37.000000 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1752 2023-05-17 13:36:37.000000 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-05-17 13:36:37.000000 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      181 2023-05-17 13:36:37.000000 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/requires.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       23 2023-05-17 13:36:37.000000 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/top_level.txt
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.510572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.510572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4190 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/base.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1242 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/error.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      756 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/error_analyzer.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      482 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/result.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.510572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    18497 2023-05-09 11:24:57.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/analysis.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5787 2023-05-09 09:30:26.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/converter.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1375 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/base.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    22393 2023-05-10 07:31:51.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/osc2cr.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3076 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/result.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1872 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/serializable.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/udp_driver/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/udp_driver/__init__.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     4494 2023-05-17 07:35:27.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/udp_driver/common.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2836 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/abs_rel.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6758 2023-05-09 08:57:31.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/configuration.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1876 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/general.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3952 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/obstacle_info.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3610 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/pps.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      984 2023-05-09 08:11:46.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/statistics.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3455 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/visualization.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      483 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/ending_cause.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5956 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/scenario_object.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3533 2023-05-09 08:11:46.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/sim_wrapper.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10620 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    14812 2023-05-16 09:23:37.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_wrapper.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4868 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      995 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/storyboard_element.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/setup.cfg
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1086 2023-05-17 13:32:43.000000 commonroad-openscenario-converter-0.0.3/setup.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/tests/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/tests/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1937 2023-05-09 12:06:26.000000 commonroad-openscenario-converter-0.0.3/tests/test_conversion.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      194 2023-05-16 14:12:02.000000 commonroad-openscenario-converter-0.0.3/tests/test_udp.py
```

### Comparing `commonroad-openscenario-converter-0.0.2/LICENSE` & `commonroad-openscenario-converter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/PKG-INFO` & `commonroad-openscenario-converter-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-openscenario-converter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Converter between OpenSCENARIO and CommonRoad formats
 Author: Yuanfei Lin, Michael Ratzel
 Author-email: yuanfei.lin@tum.de
 License: BSD 3-Clause
 Keywords: scenario description,autonomous driving
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `commonroad-openscenario-converter-0.0.2/README.md` & `commonroad-openscenario-converter-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 even if you mess something up, you can always have a safe and clean restart. 
 A guide for managing python environments with Anaconda can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
 
 - First, clone the repository. 
 - After installing Anaconda, create a new environment with (>=3.9) and enter it:
 ``` bash
 $ conda create -n commonroad-py39 python=3.9 -y
-$ conda activate commonroad-py37
+$ conda activate commonroad-py39
 or
-$ source activate commonroad-py37
+$ source activate commonroad-py39
 ```
 - Then, install the dependencies with:
 
 ```sh
 $ cd <path-to-this-repo>
 $ pip install .
 $ conda develop .
```

### Comparing `commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/PKG-INFO` & `commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-openscenario-converter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Converter between OpenSCENARIO and CommonRoad formats
 Author: Yuanfei Lin, Michael Ratzel
 Author-email: yuanfei.lin@tum.de
 License: BSD 3-Clause
 Keywords: scenario description,autonomous driving
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `commonroad-openscenario-converter-0.0.2/commonroad_openscenario_converter.egg-info/SOURCES.txt` & `commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 osc_cr_converter/utility/configuration.py
 osc_cr_converter/utility/general.py
 osc_cr_converter/utility/obstacle_info.py
 osc_cr_converter/utility/pps.py
 osc_cr_converter/utility/statistics.py
 osc_cr_converter/utility/visualization.py
 osc_cr_converter/wrapper/__init__.py
+osc_cr_converter/wrapper/base/__init__.py
+osc_cr_converter/wrapper/base/ending_cause.py
+osc_cr_converter/wrapper/base/scenario_object.py
+osc_cr_converter/wrapper/base/sim_wrapper.py
 osc_cr_converter/wrapper/esmini/__init__.py
 osc_cr_converter/wrapper/esmini/esmini_scenario_object.py
 osc_cr_converter/wrapper/esmini/esmini_wrapper.py
 osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py
 osc_cr_converter/wrapper/esmini/storyboard_element.py
 tests/__init__.py
 tests/test_conversion.py
```

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/base.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/error.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/error.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/analyzer/error_analyzer.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/error_analyzer.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/analysis.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/analysis.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/batch/converter.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/converter.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/base.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/base.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/osc2cr.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/osc2cr.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/result.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/result.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/converter/serializable.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/serializable.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/udp_driver/common.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/udp_driver/common.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/abs_rel.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/abs_rel.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/configuration.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/configuration.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/general.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/general.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/obstacle_info.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/obstacle_info.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/pps.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/pps.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/statistics.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/statistics.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/utility/visualization.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/visualization.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_wrapper.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/osc_cr_converter/wrapper/esmini/storyboard_element.py` & `commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/storyboard_element.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.2/setup.py` & `commonroad-openscenario-converter-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='commonroad-openscenario-converter',
-      version='0.0.2',
+      version='0.0.3',
       description='Converter between OpenSCENARIO and CommonRoad formats',
       keywords="scenario description, autonomous driving",
       author='Yuanfei Lin, Michael Ratzel',
       author_email='yuanfei.lin@tum.de',
       license='BSD 3-Clause',
       packages=find_packages(),
       install_requires=[
```

### Comparing `commonroad-openscenario-converter-0.0.2/tests/test_conversion.py` & `commonroad-openscenario-converter-0.0.3/tests/test_conversion.py`

 * *Files identical despite different names*

