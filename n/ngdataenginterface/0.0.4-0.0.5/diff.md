# Comparing `tmp/ngdataenginterface-0.0.4.tar.gz` & `tmp/ngdataenginterface-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdataenginterface-0.0.4.tar", max compression
+gzip compressed data, was "ngdataenginterface-0.0.5.tar", max compression
```

## Comparing `ngdataenginterface-0.0.4.tar` & `ngdataenginterface-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1486 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/README.md
--rw-r--r--   0        0        0      142 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/__init__.py
--rw-r--r--   0        0        0       81 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/analytical/__init__.py
--rw-r--r--   0        0        0     2429 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/analytical/core.py
--rw-r--r--   0        0        0      320 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/aws_interface.py
--rw-r--r--   0        0        0     1558 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/partition.py
--rw-r--r--   0        0        0     5627 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/read.py
--rw-r--r--   0        0        0     2787 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/schema.py
--rw-r--r--   0        0        0     6726 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/utils_emr.py
--rw-r--r--   0        0        0     1424 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/core/validations.py
--rw-r--r--   0        0        0     4362 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/core/write.py
--rw-r--r--   0        0        0      174 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/process/__init__.py
--rw-r--r--   0        0        0     4027 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/process/cleansing.py
--rw-r--r--   0        0        0      408 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/process/export_redshift.py
--rw-r--r--   0        0        0     6859 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/process/pismo.py
--rw-r--r--   0        0        0      399 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2934 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/README.md
+-rw-r--r--   0        0        0      142 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/__init__.py
+-rw-r--r--   0        0        0       81 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/analytical/__init__.py
+-rw-r--r--   0        0        0     2429 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/analytical/core.py
+-rw-r--r--   0        0        0      320 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/aws_interface.py
+-rw-r--r--   0        0        0     1558 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/partition.py
+-rw-r--r--   0        0        0     5627 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/read.py
+-rw-r--r--   0        0        0     2787 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/schema.py
+-rw-r--r--   0        0        0     6726 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/utils_emr.py
+-rw-r--r--   0        0        0     1424 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/validations.py
+-rw-r--r--   0        0        0     4362 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/write.py
+-rw-r--r--   0        0        0      174 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/process/__init__.py
+-rw-r--r--   0        0        0     4027 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/process/cleansing.py
+-rw-r--r--   0        0        0      408 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/process/export_redshift.py
+-rw-r--r--   0        0        0     6859 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/process/pismo.py
+-rw-r--r--   0        0        0      395 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.5/PKG-INFO
```

### Comparing `ngdataenginterface-0.0.4/ngdataenginterface/analytical/core.py` & `ngdataenginterface-0.0.5/ngdataenginterface/analytical/core.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.4/ngdataenginterface/core/aws_interface.py` & `ngdataenginterface-0.0.5/ngdataenginterface/core/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.4/ngdataenginterface/core/partition.py` & `ngdataenginterface-0.0.5/ngdataenginterface/core/partition.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.4/ngdataenginterface/core/read.py` & `ngdataenginterface-0.0.5/ngdataenginterface/core/read.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.4/ngdataenginterface/core/schema.py` & `ngdataenginterface-0.0.5/ngdataenginterface/core/schema.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.4/ngdataenginterface/core/utils_emr.py` & `ngdataenginterface-0.0.5/ngdataenginterface/core/utils_emr.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.4/ngdataenginterface/core/validations.py` & `ngdataenginterface-0.0.5/ngdataenginterface/core/validations.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.4/ngdataenginterface/core/write.py` & `ngdataenginterface-0.0.5/ngdataenginterface/core/write.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.4/ngdataenginterface/process/cleansing.py` & `ngdataenginterface-0.0.5/ngdataenginterface/process/cleansing.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.4/ngdataenginterface/process/pismo.py` & `ngdataenginterface-0.0.5/ngdataenginterface/process/pismo.py`

 * *Files identical despite different names*

