# Comparing `tmp/bodosdk-1.3.1.tar.gz` & `tmp/bodosdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodosdk-1.3.1.tar", last modified: Wed May 10 04:20:48 2023, max compression
+gzip compressed data, was "bodosdk-1.3.2.tar", last modified: Wed May 17 14:40:47 2023, max compression
```

## Comparing `bodosdk-1.3.1.tar` & `bodosdk-1.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.287792 bodosdk-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-05-10 04:20:40.000000 bodosdk-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-10 04:20:40.000000 bodosdk-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-10 04:20:48.287792 bodosdk-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    35454 2023-05-10 04:20:40.000000 bodosdk-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.287792 bodosdk-1.3.1/bodosdk/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-10 04:20:48.287792 bodosdk-1.3.1/bodosdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.279792 bodosdk-1.3.1/bodosdk/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     8160 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    13724 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.283792 bodosdk-1.3.1/bodosdk/client/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    12094 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.287792 bodosdk-1.3.1/bodosdk/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    14687 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.275792 bodosdk-1.3.1/bodosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-10 04:20:48.000000 bodosdk-1.3.1/bodosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-10 04:20:48.000000 bodosdk-1.3.1/bodosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 04:20:48.000000 bodosdk-1.3.1/bodosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-10 04:20:48.000000 bodosdk-1.3.1/bodosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-10 04:20:48.000000 bodosdk-1.3.1/bodosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-10 04:20:48.287792 bodosdk-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-05-10 04:20:40.000000 bodosdk-1.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-05-10 04:20:40.000000 bodosdk-1.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.969244 bodosdk-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-05-17 14:40:41.000000 bodosdk-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-17 14:40:41.000000 bodosdk-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-17 14:40:47.969244 bodosdk-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    35454 2023-05-17 14:40:41.000000 bodosdk-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.969244 bodosdk-1.3.2/bodosdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-17 14:40:47.969244 bodosdk-1.3.2/bodosdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.965243 bodosdk-1.3.2/bodosdk/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8160 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13828 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.969244 bodosdk-1.3.2/bodosdk/client/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12094 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.969244 bodosdk-1.3.2/bodosdk/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3729 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14489 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.965243 bodosdk-1.3.2/bodosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-17 14:40:47.000000 bodosdk-1.3.2/bodosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-17 14:40:47.000000 bodosdk-1.3.2/bodosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 14:40:47.000000 bodosdk-1.3.2/bodosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-17 14:40:47.000000 bodosdk-1.3.2/bodosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-17 14:40:47.000000 bodosdk-1.3.2/bodosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-17 14:40:47.969244 bodosdk-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-05-17 14:40:41.000000 bodosdk-1.3.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-05-17 14:40:41.000000 bodosdk-1.3.2/versioneer.py
```

### Comparing `bodosdk-1.3.1/LICENSE` & `bodosdk-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/PKG-INFO` & `bodosdk-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: Bodo Platform SDK
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodosdk-1.3.1/README.md` & `bodosdk-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/api/auth.py` & `bodosdk-1.3.2/bodosdk/api/auth.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/api/base.py` & `bodosdk-1.3.2/bodosdk/api/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/api/catalog.py` & `bodosdk-1.3.2/bodosdk/api/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/api/cloud_config.py` & `bodosdk-1.3.2/bodosdk/api/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/api/cluster.py` & `bodosdk-1.3.2/bodosdk/api/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/api/instance_role.py` & `bodosdk-1.3.2/bodosdk/api/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/api/job.py` & `bodosdk-1.3.2/bodosdk/api/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,22 +216,26 @@
         json_data = resp.json()
         return BatchJobDefinitionResponse(**json_data)
 
     @validate_arguments
     def get_batch_job_definition_by_name(self, name: str) -> BatchJobDefinitionResponse:
         headers = self.get_auth_header()
         resp = self._requests.get(
-            f"{self.get_resource_url()}/batch_job_def/name/{name}", headers=headers
+            f"{self.get_resource_url()}/batch_job_def?name={name}", headers=headers
         )
         if resp.status_code == 404:
             raise ResourceNotFound
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
-        json_data = resp.json()
-        return BatchJobDefinitionResponse(**json_data)
+
+        # Based on DB criteria there can be only one element
+        for json_data in resp.json():
+            return BatchJobDefinitionResponse(**json_data)
+
+        raise ResourceNotFound
 
     @validate_arguments
     def update_batch_job_definition(
         self, uuid: UUID, config_override: JobConfigOverride
     ) -> BatchJobDefinitionResponse:
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
```

### Comparing `bodosdk-1.3.1/bodosdk/api/request_wrapper.py` & `bodosdk-1.3.2/bodosdk/api/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/api/secret_group.py` & `bodosdk-1.3.2/bodosdk/api/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/api/secrets.py` & `bodosdk-1.3.2/bodosdk/api/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/api/workspace.py` & `bodosdk-1.3.2/bodosdk/api/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/client/base.py` & `bodosdk-1.3.2/bodosdk/client/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/client/catalog.py` & `bodosdk-1.3.2/bodosdk/client/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/client/cloud_config.py` & `bodosdk-1.3.2/bodosdk/client/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/client/cluster.py` & `bodosdk-1.3.2/bodosdk/client/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/client/instance_role.py` & `bodosdk-1.3.2/bodosdk/client/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/client/job.py` & `bodosdk-1.3.2/bodosdk/client/job.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/client/secret_group.py` & `bodosdk-1.3.2/bodosdk/client/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/client/secrets.py` & `bodosdk-1.3.2/bodosdk/client/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/client/workspace.py` & `bodosdk-1.3.2/bodosdk/client/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/models/__init__.py` & `bodosdk-1.3.2/bodosdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/models/base.py` & `bodosdk-1.3.2/bodosdk/models/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/models/catalog.py` & `bodosdk-1.3.2/bodosdk/models/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/models/cloud_config.py` & `bodosdk-1.3.2/bodosdk/models/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk/models/cluster.py` & `bodosdk-1.3.2/bodosdk/models/cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     bodo_version: str = Field(..., alias="bodoVersion")
     description: Optional[str] = None
     accelerated_networking: Optional[bool] = Field(False, alias="acceleratedNetworking")
     is_job_dedicated: Optional[bool] = Field(False, alias="isJobDedicated")
     availability_zone: Optional[str] = Field(None, alias="availabilityZone")
     aws_deployment_subnet_id: Optional[str] = Field(None, alias="awsDeploymentSubnetId")
     instance_role_uuid: Optional[str] = Field(None, alias="instanceRoleUUID")
+    autoresume: Optional[bool] = Field(True, alias="autoresume")
 
 
 class ClusterResponse(CamelCaseBase):
     name: str
     uuid: Union[str, UUID]
     status: ClusterStatus
     description: Optional[str] = ""
@@ -67,14 +68,15 @@
     last_asg_activity_id: Optional[str] = Field(None, alias="lastAsgActivityId")
     created_at: str = Field(..., alias="createdAt")
     is_job_dedicated: bool = Field(..., alias="isJobDedicated")
     last_known_activity: Optional[str] = Field(None, alias="lastKnownActivity")
     aws_deployment_subnet_id: Optional[str] = Field(None, alias="awsDeploymentSubnetId")
     node_metadata: Optional[object] = Field(None, alias="nodeMetadata")
     asg_metadata: Optional[object] = Field(None, alias="asgMetadata")
+    autoresume: Optional[bool] = Field(True, alias="autoresume")
     workspace: Any
 
 
 class ClusterTaskInfo(CamelCaseBase):
     uuid: str
     status: str
     task_type: str = Field(..., alias="taskType")
@@ -88,7 +90,8 @@
 
 class ModifyCluster(CamelCaseBase):
     uuid: Union[str, UUID]
     auto_shutdown: Optional[int] = Field(None, alias="autoshutdown")
     auto_pause: Optional[int] = Field(None, alias="autopause")
     description: Optional[str] = Field(None, alias="description")
     workers_quantity: Optional[int] = Field(-1, alias="workersQuantity")
+    autoresume: Optional[bool] = Field(True, alias="autoresume")
```

### Comparing `bodosdk-1.3.1/bodosdk/models/job.py` & `bodosdk-1.3.2/bodosdk/models/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,23 +361,22 @@
 
     config: JobConfig
         Job configuration.
 
     cluster_config: JobClusterDefinition
         Job cluster configuration.
 
-    clusterUUID: Optional[str]
-        Job cluster.
     """
 
     name: str
     description: str
     config: JobConfig
-    cluster_config: JobClusterDefinition = Field(default=None, alias="clusterConfig")
-    clusterUUID: Optional[Union[str, UUID]] = None  # Todo(Ritwika): Confirm
+    cluster_config: Optional[JobClusterDefinition] = Field(
+        default=None, alias="clusterConfig"
+    )
 
 
 class JobRunType(str, enum.Enum):
     BATCH = "BATCH"
     INTERACTIVE = "INTERACTIVE"
 
 
@@ -492,31 +491,29 @@
 
     description: str
         Job definition description.
 
     config: JobConfig
         Job configuration.
 
-    clusterConfig: JobClusterDefinition
+    cluster_config: JobClusterDefinition
         Job cluster configuration.
 
-    clusterUUID: Optional[str]
-        Job cluster UUID.
-
     created_by: str
         Job definition creator.
 
     """
 
     uuid: UUID
     name: str
     description: str
     config: JobConfig
-    clusterConfig: JobClusterDefinition = Field(..., alias="clusterConfig")
-    clusterUUID: Optional[Union[UUID, str]]  # Todo(Ritwika): Confirm
+    cluster_config: Optional[JobClusterDefinition] = Field(
+        default=None, alias="clusterConfig"
+    )
     created_by: Optional[str] = Field(alias="createdBy")
     job_runs: List[JobRunResponse] = Field(default_factory=list, alias="jobRuns")
     # Run related fields
     # Rules related fields
 
 
 class CreateJobRun(CamelCaseBase):
```

### Comparing `bodosdk-1.3.1/bodosdk/models/workspace.py` & `bodosdk-1.3.2/bodosdk/models/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/bodosdk.egg-info/PKG-INFO` & `bodosdk-1.3.2/bodosdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: Bodo Platform SDK
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodosdk-1.3.1/bodosdk.egg-info/SOURCES.txt` & `bodosdk-1.3.2/bodosdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/setup.py` & `bodosdk-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.1/versioneer.py` & `bodosdk-1.3.2/versioneer.py`

 * *Files identical despite different names*

