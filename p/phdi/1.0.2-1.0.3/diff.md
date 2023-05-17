# Comparing `tmp/phdi-1.0.2.tar.gz` & `tmp/phdi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdi-1.0.2.tar", max compression
+gzip compressed data, was "phdi-1.0.3.tar", max compression
```

## Comparing `phdi-1.0.2.tar` & `phdi-1.0.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     7048 2023-05-09 16:54:17.546780 phdi-1.0.2/LICENSE.md
--rw-r--r--   0        0        0    11787 2023-05-09 16:54:17.546780 phdi-1.0.2/README.md
--rw-r--r--   0        0        0       27 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/__init__.py
--rw-r--r--   0        0        0      223 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/cloud/README.md
--rw-r--r--   0        0        0        0 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/cloud/__init__.py
--rw-r--r--   0        0        0     8647 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/cloud/azure.py
--rw-r--r--   0        0        0     2516 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/cloud/core.py
--rw-r--r--   0        0        0     6055 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/cloud/gcp.py
--rw-r--r--   0        0        0      163 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/containers/README.md
--rw-r--r--   0        0        0        0 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/containers/__init__.py
--rw-r--r--   0        0        0     2760 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/containers/base_service.py
--rw-r--r--   0        0        0        0 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/__init__.py
--rw-r--r--   0        0        0      292 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/cloud/README.md
--rw-r--r--   0        0        0      119 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/cloud/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/cloud/azure.py
--rw-r--r--   0        0        0      311 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/conversion/README.md
--rw-r--r--   0        0        0       89 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/conversion/__init__.py
--rw-r--r--   0        0        0     8026 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/conversion/convert.py
--rw-r--r--   0        0        0      808 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/geospatial/README.md
--rw-r--r--   0        0        0      294 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/geospatial/__init__.py
--rw-r--r--   0        0        0     3494 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/geospatial/census.py
--rw-r--r--   0        0        0     4521 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/geospatial/core.py
--rw-r--r--   0        0        0     3587 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/geospatial/smarty.py
--rw-r--r--   0        0        0      890 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/harmonization/README.md
--rw-r--r--   0        0        0      335 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/harmonization/__init__.py
--rw-r--r--   0        0        0    11809 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/harmonization/standardization.py
--rw-r--r--   0        0        0      179 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/linkage/__init__.py
--rw-r--r--   0        0        0     3591 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/linkage/link.py
--rw-r--r--   0        0        0      412 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/tabulation/README.md
--rw-r--r--   0        0        0      367 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/tabulation/__init__.py
--rw-r--r--   0        0        0    27459 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/tabulation/tables.py
--rw-r--r--   0        0        0      397 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/transport/README.md
--rw-r--r--   0        0        0      327 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/transport/__init__.py
--rw-r--r--   0        0        0     7383 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/transport/export.py
--rw-r--r--   0        0        0     6822 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/transport/http.py
--rw-r--r--   0        0        0     7005 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/utils.py
--rw-r--r--   0        0        0      881 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/geospatial/README.md
--rw-r--r--   0        0        0      291 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/geospatial/__init__.py
--rw-r--r--   0        0        0     9294 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/geospatial/census.py
--rw-r--r--   0        0        0     2697 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/geospatial/core.py
--rw-r--r--   0        0        0     5911 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/geospatial/smarty.py
--rw-r--r--   0        0        0     1027 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/README.md
--rw-r--r--   0        0        0      869 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/__init__.py
--rw-r--r--   0        0        0    28162 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/double_metaphone.py
--rw-r--r--   0        0        0    10909 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/hl7.py
--rw-r--r--   0        0        0    36359 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/phdi_nicknames.csv
--rw-r--r--   0        0        0    11999 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/standardization.py
--rw-r--r--   0        0        0     1952 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/utils.py
--rw-r--r--   0        0        0      255 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/README.md
--rw-r--r--   0        0        0     1869 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/__init__.py
--rw-r--r--   0        0        0     1948 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/algorithms.py
--rw-r--r--   0        0        0     2288 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/core.py
--rw-r--r--   0        0        0    56924 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/link.py
--rw-r--r--   0        0        0    10976 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/postgres.py
--rw-r--r--   0        0        0     2667 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/seed.py
--rw-r--r--   0        0        0      399 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/tables.ddl
--rw-r--r--   0        0        0      225 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/tabulation/README.md
--rw-r--r--   0        0        0      134 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/tabulation/__init__.py
--rw-r--r--   0        0        0    11839 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/tabulation/tables.py
--rw-r--r--   0        0        0     2881 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/tabulation/validation_schema.json
--rw-r--r--   0        0        0      225 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/transport/README.md
--rw-r--r--   0        0        0       81 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/transport/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-09 16:54:18.030780 phdi-1.0.2/phdi/transport/http.py
--rw-r--r--   0        0        0     1244 2023-05-09 16:54:18.030780 phdi-1.0.2/phdi/validation/__init__.py
--rw-r--r--   0        0        0     6260 2023-05-09 16:54:18.030780 phdi-1.0.2/phdi/validation/validation.py
--rw-r--r--   0        0        0    17870 2023-05-09 16:54:18.030780 phdi-1.0.2/phdi/validation/xml_utils.py
--rw-r--r--   0        0        0     1820 2023-05-09 16:54:18.038780 phdi-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    13589 1970-01-01 00:00:00.000000 phdi-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-05-17 19:05:06.580801 phdi-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0    11787 2023-05-17 19:05:06.580801 phdi-1.0.3/README.md
+-rw-r--r--   0        0        0       27 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/cloud/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/cloud/__init__.py
+-rw-r--r--   0        0        0     9436 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/cloud/azure.py
+-rw-r--r--   0        0        0     2516 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/cloud/core.py
+-rw-r--r--   0        0        0     6055 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/cloud/gcp.py
+-rw-r--r--   0        0        0      163 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/containers/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/containers/__init__.py
+-rw-r--r--   0        0        0     2776 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/containers/base_service.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/cloud/README.md
+-rw-r--r--   0        0        0      119 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/cloud/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/cloud/azure.py
+-rw-r--r--   0        0        0      311 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/conversion/README.md
+-rw-r--r--   0        0        0       89 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/conversion/__init__.py
+-rw-r--r--   0        0        0     8026 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/conversion/convert.py
+-rw-r--r--   0        0        0      808 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/geospatial/README.md
+-rw-r--r--   0        0        0      294 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/geospatial/__init__.py
+-rw-r--r--   0        0        0     3494 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/geospatial/census.py
+-rw-r--r--   0        0        0     4521 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/geospatial/core.py
+-rw-r--r--   0        0        0     3587 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/geospatial/smarty.py
+-rw-r--r--   0        0        0      890 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/harmonization/README.md
+-rw-r--r--   0        0        0      335 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/harmonization/__init__.py
+-rw-r--r--   0        0        0    11809 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/harmonization/standardization.py
+-rw-r--r--   0        0        0      179 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/linkage/__init__.py
+-rw-r--r--   0        0        0     3591 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/linkage/link.py
+-rw-r--r--   0        0        0      412 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/tabulation/README.md
+-rw-r--r--   0        0        0      367 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/tabulation/__init__.py
+-rw-r--r--   0        0        0    27459 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/tabulation/tables.py
+-rw-r--r--   0        0        0      397 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/transport/README.md
+-rw-r--r--   0        0        0      327 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/transport/__init__.py
+-rw-r--r--   0        0        0     7383 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/transport/export.py
+-rw-r--r--   0        0        0     6822 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/transport/http.py
+-rw-r--r--   0        0        0     7005 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/fhir/utils.py
+-rw-r--r--   0        0        0      881 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/geospatial/README.md
+-rw-r--r--   0        0        0      291 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/geospatial/__init__.py
+-rw-r--r--   0        0        0     9294 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/geospatial/census.py
+-rw-r--r--   0        0        0     2697 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/geospatial/core.py
+-rw-r--r--   0        0        0     5911 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/geospatial/smarty.py
+-rw-r--r--   0        0        0     1027 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/harmonization/README.md
+-rw-r--r--   0        0        0      869 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/harmonization/__init__.py
+-rw-r--r--   0        0        0    28162 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/harmonization/double_metaphone.py
+-rw-r--r--   0        0        0    10909 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/harmonization/hl7.py
+-rw-r--r--   0        0        0    36359 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/harmonization/phdi_nicknames.csv
+-rw-r--r--   0        0        0    11999 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/harmonization/standardization.py
+-rw-r--r--   0        0        0     1952 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/harmonization/utils.py
+-rw-r--r--   0        0        0      255 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/linkage/README.md
+-rw-r--r--   0        0        0     1869 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/linkage/__init__.py
+-rw-r--r--   0        0        0     1948 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/linkage/algorithms.py
+-rw-r--r--   0        0        0     2288 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/linkage/core.py
+-rw-r--r--   0        0        0    57120 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/linkage/link.py
+-rw-r--r--   0        0        0    11316 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/linkage/postgres.py
+-rw-r--r--   0        0        0     2667 2023-05-17 19:05:07.060797 phdi-1.0.3/phdi/linkage/seed.py
+-rw-r--r--   0        0        0      399 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/linkage/tables.ddl
+-rw-r--r--   0        0        0      225 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/tabulation/README.md
+-rw-r--r--   0        0        0      134 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/tabulation/__init__.py
+-rw-r--r--   0        0        0    11839 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/tabulation/tables.py
+-rw-r--r--   0        0        0     2046 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/tabulation/validation_schema.json
+-rw-r--r--   0        0        0      225 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/transport/README.md
+-rw-r--r--   0        0        0       81 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/transport/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/transport/http.py
+-rw-r--r--   0        0        0     1244 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/validation/__init__.py
+-rw-r--r--   0        0        0     6260 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/validation/validation.py
+-rw-r--r--   0        0        0    17870 2023-05-17 19:05:07.064797 phdi-1.0.3/phdi/validation/xml_utils.py
+-rw-r--r--   0        0        0     1820 2023-05-17 19:05:07.072797 phdi-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    13589 1970-01-01 00:00:00.000000 phdi-1.0.3/PKG-INFO
```

### Comparing `phdi-1.0.2/LICENSE.md` & `phdi-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/README.md` & `phdi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/cloud/azure.py` & `phdi-1.0.3/phdi/cloud/azure.py`

 * *Files 6% similar despite different names*

```diff
@@ -215,7 +215,24 @@
         blob_properties_generator = container_client.list_blobs(name_starts_with=prefix)
 
         blob_name_list = []
         for blob_propreties in blob_properties_generator:
             blob_name_list.append(blob_propreties.name)
 
         return blob_name_list
+
+    def blob_exists(self, container_name: str, filename: str) -> bool:
+        """
+        Check if a blob exists within a container given its name and the name of the
+        container.
+
+        :param container_name: The name of the container to look for the blob in.
+        :param filename: The name of the blob to check the existence of.
+        :param prefix: Filter the objects returned to filenames beginning
+          with this value.
+        :return: A boolean of true if the file exists and false if it does not.
+        """
+
+        container_location = f"{self.storage_account_url}/{container_name}"
+        container_client = self._get_container_client(container_location)
+        blob_client = container_client.get_blob_client(filename)
+        return blob_client.exists()
```

### Comparing `phdi-1.0.2/phdi/cloud/core.py` & `phdi-1.0.3/phdi/cloud/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/cloud/gcp.py` & `phdi-1.0.3/phdi/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/containers/base_service.py` & `phdi-1.0.3/phdi/containers/base_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 from fastapi import FastAPI
+from pydantic import BaseModel
 from pathlib import Path
-from enum import Enum
 from importlib import metadata
+from typing import Literal
 
 
 # create a class with the DIBBs default Creative Commons Zero v1.0 and
 # MIT license to be used by the BaseService class
-class LicenseType(Enum):
-    CreativeCommonsZero = {
+LICENSES = {
+    "CreativeCommonsZero": {
         "name": "Creative Commons Zero v1.0 Universal",
         "url": "https://creativecommons.org/publicdomain/zero/1.0/",
-    }
-    MIT = {"name": "The MIT License", "url": "https://mit-license.org/"}
+    },
+    "MIT": {"name": "The MIT License", "url": "https://mit-license.org/"},
+}
 
+DIBBS_CONTACT = {
+    "name": "CDC Public Health Data Infrastructure",
+    "url": "https://cdcgov.github.io/phdi-site/",
+    "email": "dmibuildingblocks@cdc.gov",
+}
 
-class BaseService:
+
+STATUS_OK = {"status": "OK"}
+
+
+class StatusResponse(BaseModel):
     """
-    Base class for all DIBBs services. This class provides a FastAPI instance with DIBBs
-    metadata and optionally a health check endpoint.
+    The schema for the response from the health check endpoint.
     """
 
-    LICENSE_INFO = LicenseType.CreativeCommonsZero
-    DIBBS_CONTACT = {
-        "name": "CDC Public Health Data Infrastructure",
-        "url": "https://cdcgov.github.io/phdi-site/",
-        "email": "dmibuildingblocks@cdc.gov",
-    }
+    status: Literal["OK"]
+
 
+class BaseService:
     def __init__(
         self,
         service_name: str,
         description_path: str,
         include_health_check_endpoint: bool = True,
-        license_info: LicenseType = LICENSE_INFO,
+        license_info: Literal["CreativeCommonsZero", "MIT"] = "CreativeCommonsZero",
     ):
         """
         Initialize a BaseService instance.
 
         :param service_name: The name of the service.
         :param description_path: The path to a markdown file containing a description of
             the service.
@@ -47,27 +54,27 @@
             MIT license.
         """
         description = Path(description_path).read_text(encoding="utf-8")
         self.include_health_check_endpoint = include_health_check_endpoint
         self.app = FastAPI(
             title=service_name,
             version=metadata.version("phdi"),
-            contact=self.DIBBS_CONTACT,
-            license_info=license_info,
+            contact=DIBBS_CONTACT,
+            license_info=LICENSES[license_info],
             description=description,
         )
 
     def add_health_check_endpoint(self):
         @self.app.get("/")
-        async def health_check() -> dict:
+        async def health_check() -> StatusResponse:
             """
             Check service status. If an HTTP 200 status code is returned along with
             '{"status": "OK"}' then the service is available and running properly.
             """
-            return {"status": "OK"}
+            return STATUS_OK
 
     def start(self) -> FastAPI:
         """
         Return a FastAPI instance with DIBBs metadata set. If
         `include_health_check_endpoint` is True, then the health check endpoint
         will be added.
```

### Comparing `phdi-1.0.2/phdi/fhir/cloud/azure.py` & `phdi-1.0.3/phdi/fhir/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/conversion/convert.py` & `phdi-1.0.3/phdi/fhir/conversion/convert.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/geospatial/README.md` & `phdi-1.0.3/phdi/fhir/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/geospatial/census.py` & `phdi-1.0.3/phdi/fhir/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/geospatial/core.py` & `phdi-1.0.3/phdi/fhir/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/geospatial/smarty.py` & `phdi-1.0.3/phdi/fhir/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/harmonization/README.md` & `phdi-1.0.3/phdi/fhir/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/harmonization/standardization.py` & `phdi-1.0.3/phdi/fhir/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/linkage/link.py` & `phdi-1.0.3/phdi/fhir/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/tabulation/tables.py` & `phdi-1.0.3/phdi/fhir/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/transport/export.py` & `phdi-1.0.3/phdi/fhir/transport/export.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/transport/http.py` & `phdi-1.0.3/phdi/fhir/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/fhir/utils.py` & `phdi-1.0.3/phdi/fhir/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/geospatial/README.md` & `phdi-1.0.3/phdi/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/geospatial/census.py` & `phdi-1.0.3/phdi/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/geospatial/core.py` & `phdi-1.0.3/phdi/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/geospatial/smarty.py` & `phdi-1.0.3/phdi/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/harmonization/README.md` & `phdi-1.0.3/phdi/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/harmonization/__init__.py` & `phdi-1.0.3/phdi/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/harmonization/double_metaphone.py` & `phdi-1.0.3/phdi/harmonization/double_metaphone.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/harmonization/hl7.py` & `phdi-1.0.3/phdi/harmonization/hl7.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/harmonization/phdi_nicknames.csv` & `phdi-1.0.3/phdi/harmonization/phdi_nicknames.csv`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/harmonization/standardization.py` & `phdi-1.0.3/phdi/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/harmonization/utils.py` & `phdi-1.0.3/phdi/harmonization/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/linkage/__init__.py` & `phdi-1.0.3/phdi/linkage/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/linkage/algorithms.py` & `phdi-1.0.3/phdi/linkage/algorithms.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/linkage/core.py` & `phdi-1.0.3/phdi/linkage/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/linkage/link.py` & `phdi-1.0.3/phdi/linkage/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,14 +599,18 @@
             blocked_record = data_block[i]
             for j in range(len(blocked_record)):
                 # patient_id, person_id not included in idx->col mapping
                 if j < 2:
                     continue
                 if idx_to_col[j - 2] != "first_name" and idx_to_col[j - 2] != "address":
                     while type(blocked_record[j]) == list:
+                        # Handle empty list edge case.
+                        if len(blocked_record[j]) == 0:
+                            blocked_record[j] = ""
+                            break
                         blocked_record[j] = blocked_record[j][0]
 
         clusters = _group_patient_block_by_person(data_block)
 
         # Check if incoming record should belong to one of the person clusters
         kwargs = linkage_pass.get("kwargs", {})
         for person in clusters:
```

### Comparing `phdi-1.0.2/phdi/linkage/postgres.py` & `phdi-1.0.3/phdi/linkage/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Dict, Union, Tuple
 from phdi.linkage.core import BaseMPIConnectorClient
 import psycopg2
 from psycopg2.sql import Identifier, SQL
 from psycopg2.extensions import connection, cursor
 import json
+import logging
 
 
 class DIBBsConnectorClient(BaseMPIConnectorClient):
     """
     Represents a Postgres-specific Master Patient Index (MPI) connector
     client for the DIBBs implementation of the record linkage building
     block. Callers should use the provided interface functions (e.g.,
@@ -156,15 +157,21 @@
                         "(patient_id, person_id, patient_resource) VALUES (%s, %s, %s);"
                     ).format(patient_table=Identifier(self.patient_table))
                     data = [
                         patient_resource.get("id"),
                         person_id,
                         json.dumps(patient_resource),
                     ]
-                    db_cursor.execute(insert_new_patient, data)
+                    try:
+                        db_cursor.execute(insert_new_patient, data)
+                    except psycopg2.errors.UniqueViolation:
+                        logging.warning(
+                            f"Patient with ID {patient_resource.get('id')} already "
+                            "exists in the MPI. The patient table was not updated."
+                        )
 
         except Exception as error:  # pragma: no cover
             raise ValueError(f"{error}")
 
         finally:
             self._close_connections(db_conn=db_conn, db_cursor=db_cursor)
```

### Comparing `phdi-1.0.2/phdi/linkage/seed.py` & `phdi-1.0.3/phdi/linkage/seed.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/tabulation/tables.py` & `phdi-1.0.3/phdi/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/tabulation/validation_schema.json` & `phdi-1.0.3/phdi/tabulation/validation_schema.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 1% similar despite different names*

```diff
@@ -1,181 +1,128 @@
-00000000: 7b0a 2020 2020 2274 7970 6522 3a20 226f  {.    "type": "o
-00000010: 626a 6563 7422 2c0a 2020 2020 2270 726f  bject",.    "pro
-00000020: 7065 7274 6965 7322 3a20 7b0a 2020 2020  perties": {.    
-00000030: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
-00000040: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
-00000050: 7970 6522 3a20 226f 626a 6563 7422 2c0a  ype": "object",.
-00000060: 2020 2020 2020 2020 2020 2020 2270 726f              "pro
-00000070: 7065 7274 6965 7322 3a20 7b0a 2020 2020  perties": {.    
-00000080: 2020 2020 2020 2020 2020 2020 2273 6368              "sch
-00000090: 656d 615f 6e61 6d65 223a 207b 0a20 2020  ema_name": {.   
-000000a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000000b0: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
-000000c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000000d0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-000000e0: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-000000f0: 7265 7175 6972 6564 223a 205b 0a20 2020  required": [.   
-00000100: 2020 2020 2020 2020 2020 2020 2022 7363               "sc
-00000110: 6865 6d61 5f6e 616d 6522 0a20 2020 2020  hema_name".     
-00000120: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00000130: 207d 2c0a 2020 2020 2020 2020 2274 6162   },.        "tab
-00000140: 6c65 7322 3a20 7b0a 2020 2020 2020 2020  les": {.        
-00000150: 2020 2020 2224 7265 6622 3a20 2223 2f24      "$ref": "#/$
-00000160: 6465 6673 2f74 6162 6c65 7322 0a20 2020  defs/tables".   
-00000170: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
-00000180: 2020 2272 6571 7569 7265 6422 3a20 5b0a    "required": [.
-00000190: 2020 2020 2020 2020 2274 6162 6c65 7322          "tables"
-000001a0: 0a20 2020 205d 2c0a 2020 2020 2224 6465  .    ],.    "$de
-000001b0: 6673 223a 207b 0a20 2020 2020 2020 2022  fs": {.        "
-000001c0: 7461 626c 6573 223a 207b 0a20 2020 2020  tables": {.     
-000001d0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-000001e0: 6f62 6a65 6374 222c 0a20 2020 2020 2020  object",.       
-000001f0: 2020 2020 2022 7061 7474 6572 6e50 726f       "patternPro
-00000200: 7065 7274 6965 7322 3a20 7b0a 2020 2020  perties": {.    
-00000210: 2020 2020 2020 2020 2020 2020 222e 223a              ".":
-00000220: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000230: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00000240: 696f 6e22 3a20 2254 6865 2075 7365 7227  ion": "The user'
-00000250: 7320 7461 626c 6520 6e61 6d65 222c 0a20  s table name",. 
-00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000270: 2020 2022 7479 7065 223a 2022 6f62 6a65     "type": "obje
-00000280: 6374 222c 0a20 2020 2020 2020 2020 2020  ct",.           
-00000290: 2020 2020 2020 2020 2022 7072 6f70 6572           "proper
-000002a0: 7469 6573 223a 207b 0a20 2020 2020 2020  ties": {.       
-000002b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002c0: 2022 7265 736f 7572 6365 5f74 7970 6522   "resource_type"
-000002d0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000002e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002f0: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-00000300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000310: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000330: 2020 2020 2265 6172 6c69 6573 745f 7570      "earliest_up
-00000340: 6461 7465 5f64 6174 6574 696d 6522 3a20  date_datetime": 
-00000350: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000360: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00000370: 7970 6522 3a20 2273 7472 696e 6722 0a20  ype": "string". 
-00000380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000390: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000003a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003b0: 2020 2263 6f6c 756d 6e73 223a 207b 0a20    "columns": {. 
-000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003d0: 2020 2020 2020 2020 2020 2022 2472 6566             "$ref
-000003e0: 223a 2022 232f 2464 6566 732f 636f 6c75  ": "#/$defs/colu
-000003f0: 6d6e 7322 0a20 2020 2020 2020 2020 2020  mns".           
-00000400: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000420: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00000430: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
-00000440: 7265 6422 3a20 5b0a 2020 2020 2020 2020  red": [.        
-00000450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000460: 2272 6573 6f75 7263 655f 7479 7065 222c  "resource_type",
-00000470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000480: 2020 2020 2020 2020 2022 636f 6c75 6d6e           "column
-00000490: 7322 0a20 2020 2020 2020 2020 2020 2020  s".             
-000004a0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-000004b0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-000004c0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000004d0: 207d 2c0a 2020 2020 2020 2020 2263 6f6c   },.        "col
-000004e0: 756d 6e73 223a 207b 0a20 2020 2020 2020  umns": {.       
-000004f0: 2020 2020 2022 7479 7065 223a 2022 6f62       "type": "ob
-00000500: 6a65 6374 222c 0a20 2020 2020 2020 2020  ject",.         
-00000510: 2020 2022 7061 7474 6572 6e50 726f 7065     "patternPrope
-00000520: 7274 6965 7322 3a20 7b0a 2020 2020 2020  rties": {.      
-00000530: 2020 2020 2020 2020 2020 222e 223a 207b            ".": {
-00000540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000550: 2020 2020 2022 2472 6566 223a 2022 232f       "$ref": "#/
-00000560: 2464 6566 732f 7369 6e67 6c65 5f63 6f6c  $defs/single_col
-00000570: 756d 6e22 0a20 2020 2020 2020 2020 2020  umn".           
-00000580: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00000590: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
-000005a0: 2020 2020 2020 2020 2273 696e 676c 655f          "single_
-000005b0: 636f 6c75 6d6e 223a 207b 0a20 2020 2020  column": {.     
-000005c0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-000005d0: 696f 6e22 3a20 2254 6865 2075 7365 7227  ion": "The user'
-000005e0: 7320 636f 6c75 6d6e 206e 616d 6522 2c0a  s column name",.
-000005f0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00000600: 6522 3a20 226f 626a 6563 7422 2c0a 2020  e": "object",.  
-00000610: 2020 2020 2020 2020 2020 2270 726f 7065            "prope
-00000620: 7274 6965 7322 3a20 7b0a 2020 2020 2020  rties": {.      
-00000630: 2020 2020 2020 2020 2020 2266 6869 725f            "fhir_
-00000640: 7061 7468 223a 207b 0a20 2020 2020 2020  path": {.       
-00000650: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-00000660: 7065 223a 2022 7374 7269 6e67 220a 2020  pe": "string".  
-00000670: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00000680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000690: 2022 696e 7661 6c69 645f 7661 6c75 6573   "invalid_values
-000006a0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000006b0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-000006c0: 2022 6172 7261 7922 2c0a 2020 2020 2020   "array",.      
-000006d0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-000006e0: 7465 6d73 223a 207b 0a20 2020 2020 2020  tems": {.       
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000700: 2022 7479 7065 223a 205b 0a20 2020 2020   "type": [.     
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 2020 2020 2022 7374 7269 6e67 222c         "string",
-00000730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000740: 2020 2020 2020 2020 2020 2020 2022 626f               "bo
-00000750: 6f6c 6561 6e22 2c0a 2020 2020 2020 2020  olean",.        
-00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000770: 2020 2020 226e 756c 6c22 2c0a 2020 2020      "null",.    
-00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 2020 2020 2020 2020 226e 756d 6265 7222          "number"
-000007a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007b0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007d0: 2020 2020 2275 6e69 7175 6549 7465 6d73      "uniqueItems
-000007e0: 223a 2074 7275 650a 2020 2020 2020 2020  ": true.        
-000007f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000800: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00000810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000820: 2022 7365 6c65 6374 696f 6e5f 6372 6974   "selection_crit
-00000830: 6572 6961 223a 207b 0a20 2020 2020 2020  eria": {.       
-00000840: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-00000850: 7065 223a 2022 7374 7269 6e67 222c 0a20  pe": "string",. 
-00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000870: 2020 2022 656e 756d 223a 205b 0a20 2020     "enum": [.   
-00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000890: 2020 2020 2022 6669 7273 7422 2c0a 2020       "first",.  
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 2020 2020 2020 226c 6173 7422 2c0a 2020        "last",.  
-000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008d0: 2020 2020 2020 2272 616e 646f 6d22 2c0a        "random",.
-000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 2020 2020 2020 2261 6c6c 220a 2020          "all".  
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
-00000920: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00000930: 2020 2020 2020 2022 6461 7461 5f74 7970         "data_typ
-00000940: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
-00000950: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00000960: 3a20 2273 7472 696e 6722 2c0a 2020 2020  : "string",.    
-00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 2265 6e75 6d22 3a20 5b0a 2020 2020 2020  "enum": [.      
-00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009a0: 2020 2273 7472 696e 6722 2c0a 2020 2020    "string",.    
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 2020 226e 756d 6265 7222 2c0a 2020      "number",.  
-000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009e0: 2020 2020 2020 2262 6f6f 6c65 616e 220a        "boolean".
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-00000a10: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00000a20: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00000a30: 2020 2022 7061 7474 6572 6e50 726f 7065     "patternPrope
-00000a40: 7274 6965 7322 3a20 7b0a 2020 2020 2020  rties": {.      
-00000a50: 2020 2020 2020 2020 2020 2272 6566 6572            "refer
-00000a60: 656e 6365 5f6c 6f63 6174 696f 6e22 3a20  ence_location": 
-00000a70: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000a80: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
-00000a90: 7472 696e 6722 2c0a 2020 2020 2020 2020  tring",.        
-00000aa0: 2020 2020 2020 2020 2020 2020 2270 6174              "pat
-00000ab0: 7465 726e 223a 2022 5e66 6f72 7761 7264  tern": "^forward
-00000ac0: 7c5e 7265 7665 7273 6522 0a20 2020 2020  |^reverse".     
-00000ad0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00000ae0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00000af0: 2020 2020 2020 2020 2272 6571 7569 7265          "require
-00000b00: 6422 3a20 5b0a 2020 2020 2020 2020 2020  d": [.          
-00000b10: 2020 2020 2020 2266 6869 725f 7061 7468        "fhir_path
-00000b20: 220a 2020 2020 2020 2020 2020 2020 5d0a  ".            ].
-00000b30: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
-00000b40: 7d                                       }
+00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
+00000010: 6563 7422 2c0a 2020 2270 726f 7065 7274  ect",.  "propert
+00000020: 6965 7322 3a20 7b0a 2020 2020 226d 6574  ies": {.    "met
+00000030: 6164 6174 6122 3a20 7b0a 2020 2020 2020  adata": {.      
+00000040: 2274 7970 6522 3a20 226f 626a 6563 7422  "type": "object"
+00000050: 2c0a 2020 2020 2020 2270 726f 7065 7274  ,.      "propert
+00000060: 6965 7322 3a20 7b0a 2020 2020 2020 2020  ies": {.        
+00000070: 2273 6368 656d 615f 6e61 6d65 223a 207b  "schema_name": {
+00000080: 0a20 2020 2020 2020 2020 2022 7479 7065  .          "type
+00000090: 223a 2022 7374 7269 6e67 220a 2020 2020  ": "string".    
+000000a0: 2020 2020 7d0a 2020 2020 2020 7d2c 0a20      }.      },. 
+000000b0: 2020 2020 2022 7265 7175 6972 6564 223a       "required":
+000000c0: 205b 0a20 2020 2020 2020 2022 7363 6865   [.        "sche
+000000d0: 6d61 5f6e 616d 6522 0a20 2020 2020 205d  ma_name".      ]
+000000e0: 0a20 2020 207d 2c0a 2020 2020 2274 6162  .    },.    "tab
+000000f0: 6c65 7322 3a20 7b0a 2020 2020 2020 2224  les": {.      "$
+00000100: 7265 6622 3a20 2223 2f24 6465 6673 2f74  ref": "#/$defs/t
+00000110: 6162 6c65 7322 0a20 2020 207d 0a20 207d  ables".    }.  }
+00000120: 2c0a 2020 2272 6571 7569 7265 6422 3a20  ,.  "required": 
+00000130: 5b0a 2020 2020 2274 6162 6c65 7322 0a20  [.    "tables". 
+00000140: 205d 2c0a 2020 2224 6465 6673 223a 207b   ],.  "$defs": {
+00000150: 0a20 2020 2022 7461 626c 6573 223a 207b  .    "tables": {
+00000160: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
+00000170: 6f62 6a65 6374 222c 0a20 2020 2020 2022  object",.      "
+00000180: 7061 7474 6572 6e50 726f 7065 7274 6965  patternPropertie
+00000190: 7322 3a20 7b0a 2020 2020 2020 2020 222e  s": {.        ".
+000001a0: 223a 207b 0a20 2020 2020 2020 2020 2022  ": {.          "
+000001b0: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
+000001c0: 6865 2075 7365 7227 7320 7461 626c 6520  he user's table 
+000001d0: 6e61 6d65 222c 0a20 2020 2020 2020 2020  name",.         
+000001e0: 2022 7479 7065 223a 2022 6f62 6a65 6374   "type": "object
+000001f0: 222c 0a20 2020 2020 2020 2020 2022 7072  ",.          "pr
+00000200: 6f70 6572 7469 6573 223a 207b 0a20 2020  operties": {.   
+00000210: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
+00000220: 6365 5f74 7970 6522 3a20 7b0a 2020 2020  ce_type": {.    
+00000230: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00000240: 3a20 2273 7472 696e 6722 0a20 2020 2020  : "string".     
+00000250: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00000260: 2020 2020 2020 2265 6172 6c69 6573 745f        "earliest_
+00000270: 7570 6461 7465 5f64 6174 6574 696d 6522  update_datetime"
+00000280: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00000290: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+000002a0: 6722 0a20 2020 2020 2020 2020 2020 207d  g".            }
+000002b0: 2c0a 2020 2020 2020 2020 2020 2020 2263  ,.            "c
+000002c0: 6f6c 756d 6e73 223a 207b 0a20 2020 2020  olumns": {.     
+000002d0: 2020 2020 2020 2020 2022 2472 6566 223a           "$ref":
+000002e0: 2022 232f 2464 6566 732f 636f 6c75 6d6e   "#/$defs/column
+000002f0: 7322 0a20 2020 2020 2020 2020 2020 207d  s".            }
+00000300: 0a20 2020 2020 2020 2020 207d 2c0a 2020  .          },.  
+00000310: 2020 2020 2020 2020 2272 6571 7569 7265          "require
+00000320: 6422 3a20 5b0a 2020 2020 2020 2020 2020  d": [.          
+00000330: 2020 2272 6573 6f75 7263 655f 7479 7065    "resource_type
+00000340: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00000350: 636f 6c75 6d6e 7322 0a20 2020 2020 2020  columns".       
+00000360: 2020 205d 0a20 2020 2020 2020 207d 0a20     ].        }. 
+00000370: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
+00000380: 2020 2263 6f6c 756d 6e73 223a 207b 0a20    "columns": {. 
+00000390: 2020 2020 2022 7479 7065 223a 2022 6f62       "type": "ob
+000003a0: 6a65 6374 222c 0a20 2020 2020 2022 7061  ject",.      "pa
+000003b0: 7474 6572 6e50 726f 7065 7274 6965 7322  tternProperties"
+000003c0: 3a20 7b0a 2020 2020 2020 2020 222e 223a  : {.        ".":
+000003d0: 207b 0a20 2020 2020 2020 2020 2022 2472   {.          "$r
+000003e0: 6566 223a 2022 232f 2464 6566 732f 7369  ef": "#/$defs/si
+000003f0: 6e67 6c65 5f63 6f6c 756d 6e22 0a20 2020  ngle_column".   
+00000400: 2020 2020 207d 0a20 2020 2020 207d 0a20       }.      }. 
+00000410: 2020 207d 2c0a 2020 2020 2273 696e 676c     },.    "singl
+00000420: 655f 636f 6c75 6d6e 223a 207b 0a20 2020  e_column": {.   
+00000430: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00000440: 3a20 2254 6865 2075 7365 7227 7320 636f  : "The user's co
+00000450: 6c75 6d6e 206e 616d 6522 2c0a 2020 2020  lumn name",.    
+00000460: 2020 2274 7970 6522 3a20 226f 626a 6563    "type": "objec
+00000470: 7422 2c0a 2020 2020 2020 2270 726f 7065  t",.      "prope
+00000480: 7274 6965 7322 3a20 7b0a 2020 2020 2020  rties": {.      
+00000490: 2020 2266 6869 725f 7061 7468 223a 207b    "fhir_path": {
+000004a0: 0a20 2020 2020 2020 2020 2022 7479 7065  .          "type
+000004b0: 223a 2022 7374 7269 6e67 220a 2020 2020  ": "string".    
+000004c0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+000004d0: 696e 7661 6c69 645f 7661 6c75 6573 223a  invalid_values":
+000004e0: 207b 0a20 2020 2020 2020 2020 2022 7479   {.          "ty
+000004f0: 7065 223a 2022 6172 7261 7922 2c0a 2020  pe": "array",.  
+00000500: 2020 2020 2020 2020 2269 7465 6d73 223a          "items":
+00000510: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000520: 7479 7065 223a 205b 0a20 2020 2020 2020  type": [.       
+00000530: 2020 2020 2020 2022 7374 7269 6e67 222c         "string",
+00000540: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00000550: 626f 6f6c 6561 6e22 2c0a 2020 2020 2020  boolean",.      
+00000560: 2020 2020 2020 2020 226e 756c 6c22 2c0a          "null",.
+00000570: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00000580: 756d 6265 7222 0a20 2020 2020 2020 2020  umber".         
+00000590: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+000005a0: 2020 2275 6e69 7175 6549 7465 6d73 223a    "uniqueItems":
+000005b0: 2074 7275 650a 2020 2020 2020 2020 2020   true.          
+000005c0: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
+000005d0: 2020 2020 2022 7365 6c65 6374 696f 6e5f       "selection_
+000005e0: 6372 6974 6572 6961 223a 207b 0a20 2020  criteria": {.   
+000005f0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00000600: 7374 7269 6e67 222c 0a20 2020 2020 2020  string",.       
+00000610: 2020 2022 656e 756d 223a 205b 0a20 2020     "enum": [.   
+00000620: 2020 2020 2020 2020 2022 6669 7273 7422           "first"
+00000630: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
+00000640: 6173 7422 2c0a 2020 2020 2020 2020 2020  ast",.          
+00000650: 2020 2272 616e 646f 6d22 2c0a 2020 2020    "random",.    
+00000660: 2020 2020 2020 2020 2261 6c6c 220a 2020          "all".  
+00000670: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00000680: 2020 7d2c 0a20 2020 2020 2020 2022 6461    },.        "da
+00000690: 7461 5f74 7970 6522 3a20 7b0a 2020 2020  ta_type": {.    
+000006a0: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+000006b0: 7472 696e 6722 2c0a 2020 2020 2020 2020  tring",.        
+000006c0: 2020 2265 6e75 6d22 3a20 5b0a 2020 2020    "enum": [.    
+000006d0: 2020 2020 2020 2020 2273 7472 696e 6722          "string"
+000006e0: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+000006f0: 756d 6265 7222 2c0a 2020 2020 2020 2020  umber",.        
+00000700: 2020 2020 2262 6f6f 6c65 616e 220a 2020      "boolean".  
+00000710: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00000720: 2020 7d0a 2020 2020 2020 7d2c 0a20 2020    }.      },.   
+00000730: 2020 2022 7061 7474 6572 6e50 726f 7065     "patternPrope
+00000740: 7274 6965 7322 3a20 7b0a 2020 2020 2020  rties": {.      
+00000750: 2020 2272 6566 6572 656e 6365 5f6c 6f63    "reference_loc
+00000760: 6174 696f 6e22 3a20 7b0a 2020 2020 2020  ation": {.      
+00000770: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+00000780: 696e 6722 2c0a 2020 2020 2020 2020 2020  ing",.          
+00000790: 2270 6174 7465 726e 223a 2022 5e66 6f72  "pattern": "^for
+000007a0: 7761 7264 7c5e 7265 7665 7273 6522 0a20  ward|^reverse". 
+000007b0: 2020 2020 2020 207d 0a20 2020 2020 207d         }.      }
+000007c0: 2c0a 2020 2020 2020 2272 6571 7569 7265  ,.      "require
+000007d0: 6422 3a20 5b0a 2020 2020 2020 2020 2266  d": [.        "f
+000007e0: 6869 725f 7061 7468 220a 2020 2020 2020  hir_path".      
+000007f0: 5d0a 2020 2020 7d0a 2020 7d0a 7d0a       ].    }.  }.}.
```

### Comparing `phdi-1.0.2/phdi/transport/http.py` & `phdi-1.0.3/phdi/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/validation/__init__.py` & `phdi-1.0.3/phdi/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/validation/validation.py` & `phdi-1.0.3/phdi/validation/validation.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/phdi/validation/xml_utils.py` & `phdi-1.0.3/phdi/validation/xml_utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.2/pyproject.toml` & `phdi-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phdi"
-version = "v1.0.2"
+version = "v1.0.3"
 description = "Public health data infrastructure Building Blocks is a library to help public health departments work with their data"
 authors = ["Kenneth Chow <kenneth@skylight.digital>", "Brandon Mader <brandon@skylight.digital>", "Spencer Kathol <spencer@skylight.digital>", "Nick Clyde <nclyde@skylight.digital", "Dan Paseltiner <dan@skylight.digital>", "Brady Fausett <brady@skylight.digital>", "Marcelle Goggins <marcelle@skylight.digital", "Nick Bristow <nick@skylight.digital>", "Bryan Britten <bryan@skylight.digital>", "Emma Stephenson <emma@skylight.digital>" , "Gordon Farrell <gordon@skylight.digital>", "Robert Mitchell <rmitchell@skylight.digital>"]
 homepage = "https://github.com/CDCgov/phdi"
 repository = "https://github.com/CDCgov/phdi"
 documentation = "https://cdcgov.github.io/phdi"
 readme = "README.md"
```

### Comparing `phdi-1.0.2/PKG-INFO` & `phdi-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Public health data infrastructure Building Blocks is a library to help public health departments work with their data
 Home-page: https://github.com/CDCgov/phdi
 Author: Kenneth Chow
 Author-email: kenneth@skylight.digital
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

