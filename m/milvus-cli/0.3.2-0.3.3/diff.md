# Comparing `tmp/milvus_cli-0.3.2.tar.gz` & `tmp/milvus_cli-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus_cli-0.3.2.tar", last modified: Mon Jan  9 12:06:53 2023, max compression
+gzip compressed data, was "milvus_cli-0.3.3.tar", last modified: Wed May 17 02:34:14 2023, max compression
```

## Comparing `milvus_cli-0.3.2.tar` & `milvus_cli-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-01-09 12:06:53.542685 milvus_cli-0.3.2/
--rw-r--r--   0 nameczz    (501) staff       (20)    11357 2022-07-27 10:33:17.000000 milvus_cli-0.3.2/LICENSE
--rw-r--r--   0 nameczz    (501) staff       (20)     4639 2023-01-09 12:06:53.542344 milvus_cli-0.3.2/PKG-INFO
--rw-r--r--   0 nameczz    (501) staff       (20)     4346 2023-01-09 12:00:52.000000 milvus_cli-0.3.2/README.md
-drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-01-09 12:06:53.524793 milvus_cli-0.3.2/examples/
-drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-01-09 12:06:53.529911 milvus_cli-0.3.2/examples/import_csv/
--rw-r--r--   0 nameczz    (501) staff       (20)      367 2022-07-27 10:33:17.000000 milvus_cli-0.3.2/examples/import_csv/generate_vectors.py
-drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-01-09 12:06:53.534433 milvus_cli-0.3.2/milvus_cli/
--rw-r--r--   0 nameczz    (501) staff       (20)     3976 2022-07-27 10:33:17.000000 milvus_cli-0.3.2/milvus_cli/Fs.py
--rw-r--r--   0 nameczz    (501) staff       (20)     2384 2022-12-14 07:33:01.000000 milvus_cli-0.3.2/milvus_cli/Types.py
--rw-r--r--   0 nameczz    (501) staff       (20)    10464 2022-12-14 07:33:01.000000 milvus_cli-0.3.2/milvus_cli/Validation.py
--rw-r--r--   0 nameczz    (501) staff       (20)        0 2022-07-27 10:33:17.000000 milvus_cli-0.3.2/milvus_cli/__init__.py
--rw-r--r--   0 nameczz    (501) staff       (20)        0 2022-07-27 10:33:17.000000 milvus_cli-0.3.2/milvus_cli/main.py
-drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-01-09 12:06:53.541129 milvus_cli-0.3.2/milvus_cli/scripts/
--rw-r--r--   0 nameczz    (501) staff       (20)        0 2022-07-27 10:33:17.000000 milvus_cli-0.3.2/milvus_cli/scripts/__init__.py
--rw-r--r--   0 nameczz    (501) staff       (20)    56484 2023-01-09 11:59:36.000000 milvus_cli-0.3.2/milvus_cli/scripts/milvus_cli.py
--rw-r--r--   0 nameczz    (501) staff       (20)    29738 2023-01-09 11:59:36.000000 milvus_cli-0.3.2/milvus_cli/utils.py
-drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-01-09 12:06:53.539452 milvus_cli-0.3.2/milvus_cli.egg-info/
--rw-r--r--   0 nameczz    (501) staff       (20)     4639 2023-01-09 12:06:53.000000 milvus_cli-0.3.2/milvus_cli.egg-info/PKG-INFO
--rw-r--r--   0 nameczz    (501) staff       (20)      460 2023-01-09 12:06:53.000000 milvus_cli-0.3.2/milvus_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nameczz    (501) staff       (20)        1 2023-01-09 12:06:53.000000 milvus_cli-0.3.2/milvus_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nameczz    (501) staff       (20)       74 2023-01-09 12:06:53.000000 milvus_cli-0.3.2/milvus_cli.egg-info/entry_points.txt
--rw-r--r--   0 nameczz    (501) staff       (20)       62 2023-01-09 12:06:53.000000 milvus_cli-0.3.2/milvus_cli.egg-info/requires.txt
--rw-r--r--   0 nameczz    (501) staff       (20)       41 2023-01-09 12:06:53.000000 milvus_cli-0.3.2/milvus_cli.egg-info/top_level.txt
--rw-r--r--   0 nameczz    (501) staff       (20)       38 2023-01-09 12:06:53.542775 milvus_cli-0.3.2/setup.cfg
--rw-r--r--   0 nameczz    (501) staff       (20)      840 2023-01-09 11:59:36.000000 milvus_cli-0.3.2/setup.py
+drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-05-17 02:34:14.412932 milvus_cli-0.3.3/
+-rw-r--r--   0 nameczz    (501) staff       (20)    11357 2022-07-28 13:55:46.000000 milvus_cli-0.3.3/LICENSE
+-rw-r--r--   0 nameczz    (501) staff       (20)     4639 2023-05-17 02:34:14.412633 milvus_cli-0.3.3/PKG-INFO
+-rw-r--r--   0 nameczz    (501) staff       (20)     4346 2023-04-23 03:11:44.000000 milvus_cli-0.3.3/README.md
+drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-05-17 02:34:14.401221 milvus_cli-0.3.3/examples/
+drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-05-17 02:34:14.403934 milvus_cli-0.3.3/examples/import_csv/
+-rw-r--r--   0 nameczz    (501) staff       (20)      367 2022-07-28 13:55:46.000000 milvus_cli-0.3.3/examples/import_csv/generate_vectors.py
+drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-05-17 02:34:14.407029 milvus_cli-0.3.3/milvus_cli/
+-rw-r--r--   0 nameczz    (501) staff       (20)     3976 2022-07-28 13:55:46.000000 milvus_cli-0.3.3/milvus_cli/Fs.py
+-rw-r--r--   0 nameczz    (501) staff       (20)     2385 2023-05-17 01:36:50.000000 milvus_cli-0.3.3/milvus_cli/Types.py
+-rw-r--r--   0 nameczz    (501) staff       (20)    10517 2023-05-17 01:36:50.000000 milvus_cli-0.3.3/milvus_cli/Validation.py
+-rw-r--r--   0 nameczz    (501) staff       (20)        0 2022-07-28 13:55:46.000000 milvus_cli-0.3.3/milvus_cli/__init__.py
+-rw-r--r--   0 nameczz    (501) staff       (20)        0 2022-07-28 13:55:46.000000 milvus_cli-0.3.3/milvus_cli/main.py
+drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-05-17 02:34:14.411428 milvus_cli-0.3.3/milvus_cli/scripts/
+-rw-r--r--   0 nameczz    (501) staff       (20)        0 2022-07-28 13:55:46.000000 milvus_cli-0.3.3/milvus_cli/scripts/__init__.py
+-rw-r--r--   0 nameczz    (501) staff       (20)    56484 2023-04-23 03:11:44.000000 milvus_cli-0.3.3/milvus_cli/scripts/milvus_cli.py
+-rw-r--r--   0 nameczz    (501) staff       (20)    30017 2023-05-17 01:36:50.000000 milvus_cli-0.3.3/milvus_cli/utils.py
+drwxr-xr-x   0 nameczz    (501) staff       (20)        0 2023-05-17 02:34:14.410585 milvus_cli-0.3.3/milvus_cli.egg-info/
+-rw-r--r--   0 nameczz    (501) staff       (20)     4639 2023-05-17 02:34:14.000000 milvus_cli-0.3.3/milvus_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nameczz    (501) staff       (20)      460 2023-05-17 02:34:14.000000 milvus_cli-0.3.3/milvus_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nameczz    (501) staff       (20)        1 2023-05-17 02:34:14.000000 milvus_cli-0.3.3/milvus_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nameczz    (501) staff       (20)       74 2023-05-17 02:34:14.000000 milvus_cli-0.3.3/milvus_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nameczz    (501) staff       (20)       62 2023-05-17 02:34:14.000000 milvus_cli-0.3.3/milvus_cli.egg-info/requires.txt
+-rw-r--r--   0 nameczz    (501) staff       (20)       47 2023-05-17 02:34:14.000000 milvus_cli-0.3.3/milvus_cli.egg-info/top_level.txt
+-rw-r--r--   0 nameczz    (501) staff       (20)       38 2023-05-17 02:34:14.413015 milvus_cli-0.3.3/setup.cfg
+-rw-r--r--   0 nameczz    (501) staff       (20)      840 2023-05-17 01:36:50.000000 milvus_cli-0.3.3/setup.py
```

### Comparing `milvus_cli-0.3.2/LICENSE` & `milvus_cli-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `milvus_cli-0.3.2/PKG-INFO` & `milvus_cli-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milvus_cli
-Version: 0.3.2
+Version: 0.3.3
 Summary: CLI for Milvus
 Home-page: https://github.com/zilliztech/milvus_cli
 Author: Milvus Team
 Author-email: milvus-team@zilliz.com
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -38,15 +38,15 @@
 
 #### Prerequisites
 
 Python >= 3.8.5
 
 #### Install from PyPI (Recommended)
 
-Run `pip install milvus-cli==0.3.1`
+Run `pip install milvus-cli==0.3.2`
 
 #### Install from a tarball
 
 1. Download the [latest release](https://github.com/zilliztech/milvus_cli/releases/latest) of ` milvus_cli-<version>.tar.gz`.
 2. Run `pip install milvus_cli-<version>.tar.gz`.
 
 #### Install from source code
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: milvus_cli Version: 0.3.2 Summary: CLI for Milvus
+Metadata-Version: 2.1 Name: milvus_cli Version: 0.3.3 Summary: CLI for Milvus
 Home-page: https://github.com/zilliztech/milvus_cli Author: Milvus Team Author-
 email: milvus-team@zilliz.com License: Apache-2.0 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE # Milvus_CLIð
 ![GitHub release (latest by date including pre-releases)](https://
 img.shields.io/github/v/release/zilliztech/milvus_cli?include_prereleases) !
 [PyPI](https://img.shields.io/pypi/v/milvus-cli) ![PyPI - Downloads](https://
 img.shields.io/pypi/dm/milvus_cli?label=PYPI%20downloads) ![GitHub release
@@ -14,15 +14,15 @@
 //img.shields.io/pypi/l/milvus-cli) ## Overview [Milvus](https://github.com/
 milvus-io/milvus) Command Line Interface based on [Milvus Python SDK](https://
 github.com/milvus-io/pymilvus). - Applicable to most platforms: MS Windows,
 macOS, Ubuntu - Support pip install & offline installation package - Support
 single executable file - Milvus Python SDK full function coverage - Built-in
 help function - Support auto completion ## Installation methods ### ðInstall
 in a Python environment #### Prerequisites Python >= 3.8.5 #### Install from
-PyPI (Recommended) Run `pip install milvus-cli==0.3.1` #### Install from a
+PyPI (Recommended) Run `pip install milvus-cli==0.3.2` #### Install from a
 tarball 1. Download the [latest release](https://github.com/zilliztech/
 milvus_cli/releases/latest) of ` milvus_cli-.tar.gz`. 2. Run `pip install
 milvus_cli-.tar.gz`. #### Install from source code 1. Run `git clone https://
 github.com/zilliztech/milvus_cli.git`. 2. Run `cd milvus_cli`. 3. Run `pip
 install --editable .` ### Install from an executable file #### Windows .exe
 file Download the [latest release](https://github.com/zilliztech/milvus_cli/
 releases/latest) of `milvus_cli.exe` and run it. #### Ubuntu executable file 1.
```

### Comparing `milvus_cli-0.3.2/README.md` & `milvus_cli-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 #### Prerequisites
 
 Python >= 3.8.5
 
 #### Install from PyPI (Recommended)
 
-Run `pip install milvus-cli==0.3.1`
+Run `pip install milvus-cli==0.3.2`
 
 #### Install from a tarball
 
 1. Download the [latest release](https://github.com/zilliztech/milvus_cli/releases/latest) of ` milvus_cli-<version>.tar.gz`.
 2. Run `pip install milvus_cli-<version>.tar.gz`.
 
 #### Install from source code
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
 License](https://img.shields.io/pypi/l/milvus-cli) ## Overview [Milvus](https:/
 /github.com/milvus-io/milvus) Command Line Interface based on [Milvus Python
 SDK](https://github.com/milvus-io/pymilvus). - Applicable to most platforms: MS
 Windows, macOS, Ubuntu - Support pip install & offline installation package -
 Support single executable file - Milvus Python SDK full function coverage -
 Built-in help function - Support auto completion ## Installation methods ###
 ðInstall in a Python environment #### Prerequisites Python >= 3.8.5 ####
-Install from PyPI (Recommended) Run `pip install milvus-cli==0.3.1` ####
+Install from PyPI (Recommended) Run `pip install milvus-cli==0.3.2` ####
 Install from a tarball 1. Download the [latest release](https://github.com/
 zilliztech/milvus_cli/releases/latest) of ` milvus_cli-.tar.gz`. 2. Run `pip
 install milvus_cli-.tar.gz`. #### Install from source code 1. Run `git clone
 https://github.com/zilliztech/milvus_cli.git`. 2. Run `cd milvus_cli`. 3. Run
 `pip install --editable .` ### Install from an executable file #### Windows
 .exe file Download the [latest release](https://github.com/zilliztech/
 milvus_cli/releases/latest) of `milvus_cli.exe` and run it. #### Ubuntu
```

### Comparing `milvus_cli-0.3.2/milvus_cli/Fs.py` & `milvus_cli-0.3.3/milvus_cli/Fs.py`

 * *Files identical despite different names*

### Comparing `milvus_cli-0.3.2/milvus_cli/Types.py` & `milvus_cli-0.3.3/milvus_cli/Types.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "BOOL",
     "INT8",
     "INT16",
     "INT32",
     "INT64",
     "FLOAT",
     "DOUBLE",
-    "STRING",
+    "VARCHAR",
     "BINARY_VECTOR",
     "FLOAT_VECTOR",
 ]
 
 IndexTypes = [
     "FLAT",
     "IVF_FLAT",
```

### Comparing `milvus_cli-0.3.2/milvus_cli/Validation.py` & `milvus_cli-0.3.3/milvus_cli/Validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,22 +28,23 @@
     for field in fields:
         fieldList = field.split(":")
         if not (len(fieldList) == 3):
             raise ParameterException(
                 'Field should contain three parameters concatenated by ":".'
             )
         [fieldName, fieldType, fieldData] = fieldList
+        upperFieldType = fieldType.upper()
         fieldNames.append(fieldName)
-        if fieldType not in FiledDataTypes:
+        if upperFieldType not in FiledDataTypes:
             raise ParameterException(
                 "Invalid field data type, should be one of {}".format(
                     str(FiledDataTypes)
                 )
             )
-        if fieldType in ["BINARY_VECTOR", "FLOAT_VECTOR"]:
+        if upperFieldType in ["BINARY_VECTOR", "FLOAT_VECTOR"]:
             try:
                 int(fieldData)
             except ValueError as e:
                 raise ParameterException("""Vector's dim should be int.""")
     # Dedup field name.
     newNames = list(set(fieldNames))
     if not (len(newNames) == len(fieldNames)):
```

### Comparing `milvus_cli-0.3.2/milvus_cli/scripts/milvus_cli.py` & `milvus_cli-0.3.3/milvus_cli/scripts/milvus_cli.py`

 * *Files identical despite different names*

### Comparing `milvus_cli-0.3.2/milvus_cli/utils.py` & `milvus_cli-0.3.3/milvus_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,24 +345,29 @@
     def createCollection(self, collectionName, primaryField, autoId,
                          description, fields):
         from pymilvus import Collection, DataType, FieldSchema, CollectionSchema
 
         fieldList = []
         for field in fields:
             [fieldName, fieldType, fieldData] = field.split(":")
-            isVector = False
-            if fieldType in ["BINARY_VECTOR", "FLOAT_VECTOR"]:
+            upperFieldType= fieldType.upper()
+            if upperFieldType in ["BINARY_VECTOR", "FLOAT_VECTOR"]:
                 fieldList.append(
                     FieldSchema(name=fieldName,
-                                dtype=DataType[fieldType],
+                                dtype=DataType[upperFieldType],
                                 dim=int(fieldData)))
+            elif upperFieldType == 'VARCHAR':
+                fieldList.append(
+                    FieldSchema(name=fieldName,
+                                dtype=DataType[upperFieldType],
+                                max_length=fieldData))
             else:
                 fieldList.append(
                     FieldSchema(name=fieldName,
-                                dtype=DataType[fieldType],
+                                dtype=DataType[upperFieldType],
                                 description=fieldData))
         schema = CollectionSchema(
             fields=fieldList,
             primary_field=primaryField,
             auto_id=autoId,
             description=description,
         )
```

### Comparing `milvus_cli-0.3.2/milvus_cli.egg-info/PKG-INFO` & `milvus_cli-0.3.3/milvus_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milvus-cli
-Version: 0.3.2
+Version: 0.3.3
 Summary: CLI for Milvus
 Home-page: https://github.com/zilliztech/milvus_cli
 Author: Milvus Team
 Author-email: milvus-team@zilliz.com
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -38,15 +38,15 @@
 
 #### Prerequisites
 
 Python >= 3.8.5
 
 #### Install from PyPI (Recommended)
 
-Run `pip install milvus-cli==0.3.1`
+Run `pip install milvus-cli==0.3.2`
 
 #### Install from a tarball
 
 1. Download the [latest release](https://github.com/zilliztech/milvus_cli/releases/latest) of ` milvus_cli-<version>.tar.gz`.
 2. Run `pip install milvus_cli-<version>.tar.gz`.
 
 #### Install from source code
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: milvus-cli Version: 0.3.2 Summary: CLI for Milvus
+Metadata-Version: 2.1 Name: milvus-cli Version: 0.3.3 Summary: CLI for Milvus
 Home-page: https://github.com/zilliztech/milvus_cli Author: Milvus Team Author-
 email: milvus-team@zilliz.com License: Apache-2.0 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE # Milvus_CLIð
 ![GitHub release (latest by date including pre-releases)](https://
 img.shields.io/github/v/release/zilliztech/milvus_cli?include_prereleases) !
 [PyPI](https://img.shields.io/pypi/v/milvus-cli) ![PyPI - Downloads](https://
 img.shields.io/pypi/dm/milvus_cli?label=PYPI%20downloads) ![GitHub release
@@ -14,15 +14,15 @@
 //img.shields.io/pypi/l/milvus-cli) ## Overview [Milvus](https://github.com/
 milvus-io/milvus) Command Line Interface based on [Milvus Python SDK](https://
 github.com/milvus-io/pymilvus). - Applicable to most platforms: MS Windows,
 macOS, Ubuntu - Support pip install & offline installation package - Support
 single executable file - Milvus Python SDK full function coverage - Built-in
 help function - Support auto completion ## Installation methods ### ðInstall
 in a Python environment #### Prerequisites Python >= 3.8.5 #### Install from
-PyPI (Recommended) Run `pip install milvus-cli==0.3.1` #### Install from a
+PyPI (Recommended) Run `pip install milvus-cli==0.3.2` #### Install from a
 tarball 1. Download the [latest release](https://github.com/zilliztech/
 milvus_cli/releases/latest) of ` milvus_cli-.tar.gz`. 2. Run `pip install
 milvus_cli-.tar.gz`. #### Install from source code 1. Run `git clone https://
 github.com/zilliztech/milvus_cli.git`. 2. Run `cd milvus_cli`. 3. Run `pip
 install --editable .` ### Install from an executable file #### Windows .exe
 file Download the [latest release](https://github.com/zilliztech/milvus_cli/
 releases/latest) of `milvus_cli.exe` and run it. #### Ubuntu executable file 1.
```

### Comparing `milvus_cli-0.3.2/setup.py` & `milvus_cli-0.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="milvus_cli",
-    version="v0.3.2",
+    version="v0.3.3",
     author="Milvus Team",
     author_email="milvus-team@zilliz.com",
     url="https://github.com/zilliztech/milvus_cli",
     description="CLI for Milvus",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache-2.0",
```

