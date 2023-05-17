# Comparing `tmp/cloud-mappings-2.0.0a0.tar.gz` & `tmp/cloud-mappings-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cloud-mappings/cloud-mappings/dist/.tmp-6y3loxyk/cloud-mappings-2.0.0a0.tar", last modified: Fri May 12 03:32:19 2023, max compression
+gzip compressed data, was "/home/runner/work/cloud-mappings/cloud-mappings/dist/.tmp-p6odatm3/cloud-mappings-2.0.1.tar", last modified: Wed May 17 14:44:47 2023, max compression
```

## Comparing `cloud-mappings-2.0.0a0.tar` & `cloud-mappings-2.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloudmappings/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_cloudmappinginternal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/awss3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/azureblobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/azuretablestorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/googlecloudstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/cloudmapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/cloudstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/storageprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloudmappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_cloudmappinginternal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/awss3storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/azureblobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/azuretablestorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/googlecloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/cloudmapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/cloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloudmappings/serialisers/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/serialisers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/serialisers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/serialisers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/serialisers/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/storageprovider.py
```

### Comparing `cloud-mappings-2.0.0a0/LICENSE` & `cloud-mappings-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.0a0/PKG-INFO` & `cloud-mappings-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-mappings
-Version: 2.0.0a0
+Version: 2.0.1
 Summary: MutableMapping interfaces for common cloud storage providers
 Home-page: https://github.com/JJ11teen/cloud-mappings
 Author: Lucas Sargent
 Author-email: lucas.sargent@outlook.com
 Project-URL: Bug Tracker, https://github.com/JJ11teen/cloud-mappings/issues
 Keywords: mutable dict aws s3 azure gcp
 Classifier: Programming Language :: Python :: 3
@@ -262,10 +262,10 @@
 * Azure Blob: `AZURE_TENANT_ID`, `AZURE_CLIENT_ID`, `AZURE_CLIENT_SECRET`, `AZURE_BLOB_STORAGE_ACCOUNT_URL`, `AZURE_BLOB_STORAGE_HIERARCHICAL_ACCOUNT_URL` (the tests assume the same secret is used for both)
 * Azure Table: `AZURE_TABLE_STORAGE_CONNECTION_STRING`
 * GCP Storage: `GOOGLE_APPLICATION_CREDENTIALS` (path to credentials file), `GOOGLE_CLOUD_STORAGE_PROJECT`
 * AWS S3: `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`
 
 Run tests with:
 ```bash
-pytest --test_container_id <container-suffix-to-use-for-tests>
+pytest --test-container-id <container-suffix-to-use-for-tests>
 ```
 The testing container will be prefixed by "pytest", and the commit sha is used within build & release workflows. Note that if the container specified already exists one test will fail.
```

### Comparing `cloud-mappings-2.0.0a0/README.md` & `cloud-mappings-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -241,10 +241,10 @@
 * Azure Blob: `AZURE_TENANT_ID`, `AZURE_CLIENT_ID`, `AZURE_CLIENT_SECRET`, `AZURE_BLOB_STORAGE_ACCOUNT_URL`, `AZURE_BLOB_STORAGE_HIERARCHICAL_ACCOUNT_URL` (the tests assume the same secret is used for both)
 * Azure Table: `AZURE_TABLE_STORAGE_CONNECTION_STRING`
 * GCP Storage: `GOOGLE_APPLICATION_CREDENTIALS` (path to credentials file), `GOOGLE_CLOUD_STORAGE_PROJECT`
 * AWS S3: `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`
 
 Run tests with:
 ```bash
-pytest --test_container_id <container-suffix-to-use-for-tests>
+pytest --test-container-id <container-suffix-to-use-for-tests>
 ```
 The testing container will be prefixed by "pytest", and the commit sha is used within build & release workflows. Note that if the container specified already exists one test will fail.
```

### Comparing `cloud-mappings-2.0.0a0/setup.cfg` & `cloud-mappings-2.0.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 python_requires = >=3.7
 
 [options.extras_require]
 azureblob = azure-identity==1.12.0; azure-storage-blob==12.16.0
 azuretable = azure-identity==1.12.0; azure-data-tables==12.4.2
 gcpstorage = google-cloud-storage==2.9.0
 awss3 = boto3==1.26.129
-tests = pytest==7.1.2
+tests = pytest==7.1.2; pytest-mock==3.1.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/PKG-INFO` & `cloud-mappings-2.0.1/src/cloud_mappings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-mappings
-Version: 2.0.0a0
+Version: 2.0.1
 Summary: MutableMapping interfaces for common cloud storage providers
 Home-page: https://github.com/JJ11teen/cloud-mappings
 Author: Lucas Sargent
 Author-email: lucas.sargent@outlook.com
 Project-URL: Bug Tracker, https://github.com/JJ11teen/cloud-mappings/issues
 Keywords: mutable dict aws s3 azure gcp
 Classifier: Programming Language :: Python :: 3
@@ -262,10 +262,10 @@
 * Azure Blob: `AZURE_TENANT_ID`, `AZURE_CLIENT_ID`, `AZURE_CLIENT_SECRET`, `AZURE_BLOB_STORAGE_ACCOUNT_URL`, `AZURE_BLOB_STORAGE_HIERARCHICAL_ACCOUNT_URL` (the tests assume the same secret is used for both)
 * Azure Table: `AZURE_TABLE_STORAGE_CONNECTION_STRING`
 * GCP Storage: `GOOGLE_APPLICATION_CREDENTIALS` (path to credentials file), `GOOGLE_CLOUD_STORAGE_PROJECT`
 * AWS S3: `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`
 
 Run tests with:
 ```bash
-pytest --test_container_id <container-suffix-to-use-for-tests>
+pytest --test-container-id <container-suffix-to-use-for-tests>
 ```
 The testing container will be prefixed by "pytest", and the commit sha is used within build & release workflows. Note that if the container specified already exists one test will fail.
```

### Comparing `cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/SOURCES.txt` & `cloud-mappings-2.0.1/src/cloud_mappings.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 src/cloudmappings/__init__.py
 src/cloudmappings/_cloudmappinginternal.py
 src/cloudmappings/cloudmapping.py
 src/cloudmappings/cloudstorage.py
 src/cloudmappings/errors.py
 src/cloudmappings/storageprovider.py
 src/cloudmappings/_storageproviders/__init__.py
-src/cloudmappings/_storageproviders/awss3.py
+src/cloudmappings/_storageproviders/awss3storage.py
 src/cloudmappings/_storageproviders/azureblobstorage.py
 src/cloudmappings/_storageproviders/azuretablestorage.py
 src/cloudmappings/_storageproviders/googlecloudstorage.py
 src/cloudmappings/serialisers/__init__.py
 src/cloudmappings/serialisers/core.py
 src/cloudmappings/serialisers/pandas.py
 src/cloudmappings/serialisers/serialisation.py
```

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/_cloudmappinginternal.py` & `cloud-mappings-2.0.1/src/cloudmappings/_cloudmappinginternal.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,15 +69,18 @@
     def __delitem__(self, key: str) -> None:
         if key not in self._etags:
             raise KeyError(key)
         self._storage_provider.delete_data(key=self._encode_key(key), etag=self._etags[key])
         del self._etags[key]
 
     def __contains__(self, key: str) -> bool:
-        return key in self._etags
+        if not self.read_blindly:
+            return key in self._etags
+        encoded_key = self._encode_key(key)
+        return encoded_key in self._storage_provider.list_keys_and_etags(encoded_key)
 
     def keys(self) -> Iterator[str]:
         return iter(self._etags.keys())
 
     __iter__ = keys
 
     def __len__(self) -> int:
```

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/awss3.py` & `cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/awss3storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from cloudmappings.storageprovider import StorageProvider
 
 logger = logging.getLogger(__name__)
 
 _metadata_etag_key = "cloud-mappings-etag"
 
 
-class AWSS3Provider(StorageProvider):
+class AWSS3StorageProvider(StorageProvider):
     def __init__(
         self,
         bucket_name: str,
         silence_warning: bool = False,
     ) -> None:
         self._client = boto3.client("s3")
         self._bucket_name = bucket_name
```

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/azureblobstorage.py` & `cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/azureblobstorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from cloudmappings.storageprovider import StorageProvider
 
 
 class AzureBlobStorageProvider(StorageProvider):
     def __init__(
         self,
         container_name: str,
-        credential: Any,
+        credential: Any = None,
         account_url: str = None,
         connection_string: str = None,
         create_container_metadata=None,
     ) -> None:
         if connection_string:
             self._container_client = ContainerClient.from_connection_string(
                 conn_str=connection_string, container_name=container_name
```

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/azuretablestorage.py` & `cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/azuretablestorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return b"".join([v for k, v in entity.items() if k.startswith("d_")])
 
 
 class AzureTableStorageProvider(StorageProvider):
     def __init__(
         self,
         table_name: str,
-        credential: Any,
+        credential: Any = None,
         endpoint: str = None,
         connection_string: str = None,
     ) -> None:
         if connection_string is not None:
             self._table_client = TableClient.from_connection_string(conn_str=connection_string, table_name=table_name)
         else:
             self._table_client = TableClient(
```

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/googlecloudstorage.py` & `cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/googlecloudstorage.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/cloudmapping.py` & `cloud-mappings-2.0.1/src/cloudmappings/cloudmapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         When `read_blindly=True`, a `CloudMapping` will directly query the cloud for any key
         accessed, regardless of if it has previously written a value to that key. It will always get
         the latest value from the cloud, and never raise a `cloudmappings.errors.KeySyncError` for
         read operations. If there is no value for a key in the cloud, and `read_blindly_error=True`, a
         `KeyError` will be raised. If there is no value for a key in the cloud and
         `read_blindly_error=False`, `read_blindly_default` will be returned.
 
+        Read blindly only impacts __get__ (`d[key]`) and __contains__ (`in`) operations.
+
         By default a `CloudMapping` is instantiated with read blindly set to `False`.
     """
 
     read_blindly_error: bool
     """ Whether to raise a `KeyValue` error when `read_blindly=True` and a key does not have
         a value in the cloud. If `True`, this takes prescedence over `read_blindly_default`.
     """
```

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/cloudstorage.py` & `cloud-mappings-2.0.1/src/cloudmappings/cloudstorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,21 +72,24 @@
         return mapping
 
 
 class AzureBlobStorage(CloudStorage):
     def __init__(
         self,
         container_name: str,
-        credential: Any,
+        credential: Any = None,
         account_url: str = None,
         connection_string: str = None,
         create_container_metadata=None,
     ) -> None:
         """A cloud-mapping backed by an Azure Blob Storage Container
 
+        Note that if you're using hierarchical namespace, directories and blobs cannot share the
+        same key.
+
         Parameters
         ----------
         container_name : str
             The name of the Azure Storage Blob Container to use within the Azure Storage Account
         credential : Any
             A credential object from `azure.identity`
         account_url : str, default=None
@@ -114,15 +117,15 @@
         )
 
 
 class AzureTableStorage(CloudStorage):
     def __init__(
         self,
         table_name: str,
-        credential: Any,
+        credential: Any = None,
         endpoint: str = None,
         connection_string: str = None,
     ) -> None:
         """A cloud-mapping backed by an Azure Table Storage Table
 
         Note that Azure Table Storage has a 1MB size limit per entity. This mapping distributes
         bytes across dummy attributes within an entity to ensure attribute level limits are not
@@ -208,10 +211,10 @@
         silence_warning : bool, default=False
             Whether to silence the warning logged about using S3 backed cloud-mappings concurrently
 
         See Also
         --------
         cloud-mapping : `CloudMapping`
         """
-        from cloudmappings._storageproviders.awss3 import AWSS3Provider
+        from cloudmappings._storageproviders.awss3storage import AWSS3StorageProvider
 
-        super().__init__(AWSS3Provider(bucket_name=bucket_name, silence_warning=silence_warning))
+        super().__init__(AWSS3StorageProvider(bucket_name=bucket_name, silence_warning=silence_warning))
```

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/errors.py` & `cloud-mappings-2.0.1/src/cloudmappings/errors.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/core.py` & `cloud-mappings-2.0.1/src/cloudmappings/serialisers/core.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/pandas.py` & `cloud-mappings-2.0.1/src/cloudmappings/serialisers/pandas.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/serialisation.py` & `cloud-mappings-2.0.1/src/cloudmappings/serialisers/serialisation.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.0a0/src/cloudmappings/storageprovider.py` & `cloud-mappings-2.0.1/src/cloudmappings/storageprovider.py`

 * *Files identical despite different names*

