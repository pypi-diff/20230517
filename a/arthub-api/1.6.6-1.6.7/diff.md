# Comparing `tmp/arthub_api-1.6.6.tar.gz` & `tmp/arthub_api-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.6.6.tar", last modified: Tue May 16 11:29:27 2023, max compression
+gzip compressed data, was "arthub_api-1.6.7.tar", last modified: Wed May 17 11:52:05 2023, max compression
```

## Comparing `arthub_api-1.6.6.tar` & `arthub_api-1.6.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 11:29:27.454974 arthub_api-1.6.6/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.6/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-05-16 11:29:27.453976 arthub_api-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 11:29:27.431204 arthub_api-1.6.6/arthub_api/
--rw-rw-rw-   0        0        0      666 2023-05-15 09:23:22.000000 arthub_api-1.6.6/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     3483 2023-05-16 10:40:32.000000 arthub_api-1.6.6/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-05-16 11:28:34.000000 arthub_api-1.6.6/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.6/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.6/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.6/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    38387 2023-05-16 10:40:32.000000 arthub_api-1.6.6/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     1265 2023-05-16 10:40:32.000000 arthub_api-1.6.6/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    22945 2023-05-11 11:42:27.000000 arthub_api-1.6.6/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.6/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.6/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.6/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.6/arthub_api/models.py
--rw-rw-rw-   0        0        0    41857 2023-05-15 09:23:22.000000 arthub_api-1.6.6/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.6/arthub_api/storage.py
--rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.6/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:29:27.441876 arthub_api-1.6.6/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-05-16 11:29:27.000000 arthub_api-1.6.6/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-16 11:29:27.000000 arthub_api-1.6.6/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 11:29:27.000000 arthub_api-1.6.6/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-16 11:29:27.000000 arthub_api-1.6.6/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.6/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      108 2023-05-16 11:29:27.000000 arthub_api-1.6.6/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 11:29:27.000000 arthub_api-1.6.6/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.6/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 11:29:27.454974 arthub_api-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     2973 2023-05-16 11:29:25.000000 arthub_api-1.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:29:27.451991 arthub_api-1.6.6/tests/
--rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.6/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.6/tests/_utils.py
--rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.6/tests/conftest.py
--rw-rw-rw-   0        0        0     5924 2023-05-11 09:00:19.000000 arthub_api-1.6.6/tests/test_open_api.py
--rw-rw-rw-   0        0        0    17832 2023-05-16 10:40:32.000000 arthub_api-1.6.6/tests/test_open_api_blade.py
--rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.6/tests/test_storage.py
--rw-rw-rw-   0        0        0     3691 2023-05-11 11:42:27.000000 arthub_api-1.6.6/tests/test_storage_blade.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:52:05.013626 arthub_api-1.6.7/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.7/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-05-17 11:52:05.012629 arthub_api-1.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 11:52:04.989691 arthub_api-1.6.7/arthub_api/
+-rw-rw-rw-   0        0        0      666 2023-05-15 09:23:22.000000 arthub_api-1.6.7/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3483 2023-05-16 10:40:32.000000 arthub_api-1.6.7/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2023-05-17 11:50:58.000000 arthub_api-1.6.7/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.7/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.7/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.7/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    38742 2023-05-17 11:50:58.000000 arthub_api-1.6.7/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     2070 2023-05-17 11:50:58.000000 arthub_api-1.6.7/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    23614 2023-05-17 11:50:58.000000 arthub_api-1.6.7/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.7/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.7/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.7/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.7/arthub_api/models.py
+-rw-rw-rw-   0        0        0    42130 2023-05-17 11:50:58.000000 arthub_api-1.6.7/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.7/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.7/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:52:05.000660 arthub_api-1.6.7/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.7/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      108 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.7/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 11:52:05.013626 arthub_api-1.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     2973 2023-05-16 11:29:25.000000 arthub_api-1.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:52:05.011632 arthub_api-1.6.7/tests/
+-rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.7/tests/_utils.py
+-rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.7/tests/conftest.py
+-rw-rw-rw-   0        0        0     5924 2023-05-11 09:00:19.000000 arthub_api-1.6.7/tests/test_open_api.py
+-rw-rw-rw-   0        0        0    17832 2023-05-16 10:40:32.000000 arthub_api-1.6.7/tests/test_open_api_blade.py
+-rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.7/tests/test_storage.py
+-rw-rw-rw-   0        0        0     4290 2023-05-17 11:50:58.000000 arthub_api-1.6.7/tests/test_storage_blade.py
```

### Comparing `arthub_api-1.6.6/LICENSE` & `arthub_api-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/PKG-INFO` & `arthub_api-1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.6.6
+Version: 1.6.7
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.6/README.md` & `arthub_api-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/arthub_api/__init__.py` & `arthub_api-1.6.7/arthub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/arthub_api/__main__.py` & `arthub_api-1.6.7/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/arthub_api/_internal_utils.py` & `arthub_api-1.6.7/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/arthub_api/asset_matrix.py` & `arthub_api-1.6.7/arthub_api/asset_matrix.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/arthub_api/blade_api.py` & `arthub_api-1.6.7/arthub_api/blade_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,25 @@
         return "%s//%s/resolving/resolving/openapi/%s/core/%s" % (
             self.http_scheme, self.api_host, self._api_version_blade, api_method)
 
     def add_headers(self, headers):
         if self.blade_public_token != "":
             headers["blade-public-token"] = self.blade_public_token
 
+    def has_credential(self):
+        r"""Checks if credential is already set or not for Blade"""
+        # public_token from pan is not valid credential for blade
+        if self.blade_public_token:
+            return True
+        if self._cookies:
+            return True
+        if self._token:
+            return True
+        return False
+
     def set_blade_public_token(self, token):
         self.blade_public_token = token
 
     def clear_blade_public_token(self):
         self.blade_public_token = ""
 
     # root
```

### Comparing `arthub_api-1.6.6/arthub_api/blade_storage.py` & `arthub_api-1.6.7/arthub_api/blade_storage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,556 +1,559 @@
-# -*- coding:utf-8 -*-
-"""internal COS API can be used to upload and download files from COS."""
-
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
-# Import built-in modules
-import six
-import logging
-import socket
-import os
-import time
-import threading
-import requests
-import concurrent
-import json
-import warnings
-
-# Import third-party modules
-import requests
-
-# Import third-party modules
-from tenacity import retry as tenacity_retry
-from tenacity import retry_if_exception_type
-from tenacity import stop_after_attempt
-from tenacity import wait_fixed
-from tenacity import RetryError
-from xml.etree import ElementTree
-
-# Import local modules
-from arthub_api.__version__ import __title__
-from arthub_api.blade_api import BladeAPI
-import arthub_api.utils as utils
-import arthub_api._internal_utils as _internal_utils
-
-
-logger = logging.getLogger(__title__)
-
-if six.PY2:
-    class PermissionError(OSError):
-        pass
-    class FileNotFoundError(IOError):
-        pass
-
-class SignerError(RuntimeError):
-    pass
-
-# signer for blade api
-class RemoteSigner(object):    
-    def __init__(self, blade_backend, force=False):
-        self.cli = blade_backend
-        self.force = force
-        
-    @classmethod
-    def _remove_suffix(cls, s, sf):
-        if s.endswith(sf):
-            return s[:len(s)-len(sf)]
-        return s
-
-    @classmethod
-    def _key_to_pkg(cls, key):
-        if not key.startswith("pkg_distribution/7z/"):
-            return {}
-        result = key.split("/")
-        if len(result) < 5:
-            return {}
-        result[4] = cls._remove_suffix(result[4], ".7z")
-        if result[2] != result[4]:
-            return {}
-        return {"name": result[2], "version": result[3]}
-    
-    def _take_signed_url(self, arthub_response, type_of_sign=""):
-        if not arthub_response.is_succeeded():
-            raise SignerError("arthub api: {0}".format(str(arthub_response.errors)))
-        logger.debug('{0} sign-url rsp is {1}'.format(type_of_sign, arthub_response.result))
-        if len(arthub_response.result) == 0:
-            raise SignerError("arthub api: result is empty")
-        return "https:" + arthub_response.result[0].get('signed_url')
-        
-    # we use bucket + key to identify a file. 
-    # however bucket might be fixed for ArtHub condition, so bucket input is ignored
-    def _get_package_download_sign(self, bucket, key):
-        pkg = self._key_to_pkg(key)
-        # this will return a url expires in 10 minutes
-        signed = self.cli.blade_download_package([pkg])
-        if not signed.is_succeeded():
-            raise SignerError("arthub api: {0}".format(str(signed.errors)))
-        logger.debug("download sign-url rsp is {0}".format(signed.result))
-        return signed.result
-    
-    def get_download_url(self, bucket, key):
-        signed = self._get_package_download_sign(bucket, key)
-        if len(signed) == 0:
-            raise SignerError("arthub api: result is empty")
-        return "https:" + signed[0].get('signed_url')
-        
-    def get_file_size(self, bucket, key):
-        signed = self._get_package_download_sign(bucket, key)
-        if len(signed) == 0:
-            raise SignerError("arthub api: result is empty")
-        return signed[0].get('size')
-    
-    def get_upload_url(self, bucket, key):
-        pkg = self._key_to_pkg(key)
-        signed = self.cli.blade_upload_package([pkg], self.force)
-        return self._take_signed_url(signed, "upload")
-    
-    def get_begin_multipart_upload_url(self, bucket, key):
-        pkg = self._key_to_pkg(key)
-        signed = self.cli.blade_begin_multipart_package_upload([pkg], self.force)
-        return self._take_signed_url(signed, "begin multipart upload")
-    
-    def get_upload_part_url(self, bucket, key, upload_id, part_number):
-        pkg = self._key_to_pkg(key)
-        pkg.update({"upload_id": upload_id, "part_number": part_number})
-        signed = self.cli.blade_part_package_upload([pkg], self.force)
-        return self._take_signed_url(signed, "upload part")
-    
-    def get_complete_multipart_upload_url(self, bucket, key, upload_id):
-        pkg = self._key_to_pkg(key)
-        pkg.update({"upload_id": upload_id})
-        signed = self.cli.blade_complete_multipart_package_upload([pkg], self.force)
-        return self._take_signed_url(signed, "end multipart upload")
-
-
-class ProgressCallback():
-    def __init__(self, file_size, progress_callback):
-        self.__lock = threading.Lock()
-        self.__finished_size = 0
-        self.__file_size = file_size
-        self.__progress_callback = progress_callback
-
-    def report(self, size):
-        with self.__lock:
-            self.__finished_size += size
-            self.__progress_callback(self.__finished_size, self.__file_size)
-            
-    def get(self):
-        return self.__finished_size, self.__file_size
-            
-    def get_percent(self):
-        return self.__finished_size / self.__file_size
-
-
-class Client(object):
-    def __init__(self, signer=None):
-        if signer is None:
-            raise ReferenceError("signer is None: must provide signer arg")
-        self.remote_signer = signer
-        
-    def download_file(self, Bucket, Key, DestFilePath, PartSize=20, MAXThread=5, EnableCRC=False, progress_callback=None):
-        if EnableCRC:
-            warnings.warn("EnableCRC is not supported")
-        part_size = PartSize * 1024 * 1024
-        file_size = self.remote_signer.get_file_size(Bucket, Key)
-        if file_size is None:
-            raise RetryError('failed to get file_size for {0}, file might not exist'.format(Key))
-        callback = None
-        if progress_callback:
-            callback = ProgressCallback(file_size, progress_callback)
-        resumable_downloader = ResumableDownLoader(self.remote_signer, Bucket, Key, DestFilePath, file_size, part_size, MAXThread, callback)
-        if file_size < 20 * 1024 * 1024:
-            resumable_downloader.simple_download()
-            return
-            
-        resumable_downloader.download()
-        
-    def upload_file(self, Bucket, Key, LocalFilePath, PartSize=20, MAXThread=5, EnableCRC=False, progress_callback=None):
-        if EnableCRC:
-            warnings.warn("EnableCRC is not supported")
-        if not os.path.isfile(LocalFilePath):
-            raise OSError("not found file: {0}".format(LocalFilePath))
-        file_size = os.path.getsize(LocalFilePath)
-        part_size = PartSize * 1024 * 1024
-        callback = None
-        if progress_callback:
-            callback = ProgressCallback(file_size, progress_callback)
-        resumableUploader = ResumableUploader(self.remote_signer, Bucket, Key, LocalFilePath, file_size, part_size, MAXThread, callback)
-        if file_size < 20 * 1024 * 1024:
-            resumableUploader.simple_upload()
-            return
-            
-        resumableUploader.upload()
-
-    # check file exists with http-get method
-    def check_exists(self, bucket, key):
-        headers = {'Range': 'bytes=0-0'}
-        self.download_url = self.remote_signer.get_download_url(bucket, key)
-        response = requests.get(self.download_url, headers=headers)
-        if response.status_code == 404:
-            return False
-        if response.status_code == 416:
-            return True
-        response.raise_for_status()
-        return True
-
-
-class ResumableDownLoader(object):
-    def __init__(self, remote_signer, bucket, key, local_path, file_size, part_size=5*1024*1024, thread_num=4, progress_callback=None):
-        self.remote_signer = remote_signer
-        self.bucket = bucket
-        self.key = key
-        self.local_path = local_path
-        self.part_size = part_size
-        self.thread_num = thread_num
-        self.progress_callback = progress_callback
-        self.file_size = file_size
-        self.download_url = None
-        self.url_expire_time = None
-        self.tmp_file = '{0}_ahtmp'.format(local_path)
-        self.record_file = '{0}_dl_ahrecord'.format(local_path)
-
-    def _refresh_download_url(self):
-        current_time = time.time()
-        if self.download_url is None or current_time >= self.url_expire_time:
-            self.download_url = self.remote_signer.get_download_url(self.bucket, self.key)
-            self.url_expire_time = current_time + 10 * 60  # 10 minutes expiry time
-
-    def _load_progress(self):
-        if os.path.exists(self.record_file):
-            with open(self.record_file, 'r') as f:
-                return [tuple(map(int, line.strip().split('-'))) for line in f]
-        return []
-
-    def _save_progress(self, start, end):
-        with threading.Lock():  
-            with open(self.record_file, 'a') as f:
-                f.write('{start}-{end}-{part_size}\n'.format(start=start, end=end, part_size=self.part_size))  # Save part_size along with the progress, part_size is not current chunk_length
-
-    def _download_part(self, start, end):
-        self._refresh_download_url()
-        headers = {'Range': 'bytes={start}-{end}'.format(start=start, end=end)}
-        response = requests.get(self.download_url, headers=headers, stream=True)
-        with open(self.tmp_file, 'rb+') as f:
-            f.seek(start)
-            for chunk in response.iter_content(chunk_size=8192):
-                f.write(chunk)
-                if self.progress_callback:
-                    self.progress_callback.report(len(chunk))
-        self._save_progress(start, end)  # Save progress after part is downloaded
-
-    def simple_download(self):
-        self._refresh_download_url()
-        response = requests.get(self.download_url, stream=True)
-        response.raise_for_status()
-        with open(self.tmp_file, 'wb') as f:
-            for chunk in response.iter_content(chunk_size=8192):
-                f.write(chunk)
-                if self.progress_callback:
-                    self.progress_callback.report(len(chunk))
-        try:
-            os.remove(self.local_path)
-        except:
-            pass
-        os.rename(self.tmp_file, self.local_path)
-        if os.path.exists(self.record_file):  # Remove existing progress record file
-            os.remove(self.record_file)
-                    
-    def download(self):
-        self._refresh_download_url()
-        part_ranges = self._calculate_part_ranges()
-        progress_record = self._load_progress()
-        
-        # create if not exists
-        with open(self.tmp_file,"a+"):
-            pass
-            
-        # Call progress_callback with the existing progress if there is a progress record
-        if progress_record and self.progress_callback:
-            total_downloaded = sum(end - start + 1 for start, end, _ in progress_record)
-            self.progress_callback.report(total_downloaded)
-
-        # Use a ThreadPoolExecutor to limit the number of threads
-        with concurrent.futures.ThreadPoolExecutor(max_workers=self.thread_num) as executor:
-            # Submit download tasks to the thread pool
-            futures = [executor.submit(self._download_part, start, end) for start, end in part_ranges if (start, end, self.part_size) not in progress_record]
-
-            # Wait for all download tasks to complete, allowing KeyboardInterrupt (Ctrl-C) to stop the process
-            try:
-                for future in concurrent.futures.as_completed(futures):
-                    future.result()
-            except KeyboardInterrupt as e:
-                print("Download interrupted by user. Stopping...")
-                executor.shutdown(wait=False, cancel_futures=True)
-                raise e
-        try:
-            os.remove(self.local_path)
-        except:
-            pass
-        os.rename(self.tmp_file, self.local_path)
-        if os.path.exists(self.record_file):  # Remove existing progress record file
-            os.remove(self.record_file)
-
-    def _calculate_part_ranges(self):
-        part_ranges = []
-        num_parts = self.file_size // self.part_size
-        if self.file_size % self.part_size != 0:
-            num_parts += 1
-
-        for i in range(num_parts):
-            start = i * self.part_size
-            end = min((i + 1) * self.part_size - 1, self.file_size - 1)
-            part_ranges.append((start, end))
-
-        return part_ranges
-    
-
-class ResumableUploader(object):
-    def __init__(self, remote_signer, bucket, key, local_path, file_size, part_size=5*1024*1024, thread_num=4, progress_callback=None):
-        self.remote_signer = remote_signer
-        self.bucket = bucket
-        self.key = key
-        self.local_path = local_path
-        self.part_size = part_size
-        self.thread_num = thread_num
-        self.progress_callback = progress_callback
-        self.file_size = file_size
-        self.upload_url = None
-        self.url_expire_time = None
-        self.record_file = '{0}_ul_ahrecord'.format(local_path)
-        
-    def _begin_multipart_upload(self, bucket, key, file_name):
-        begin_url = self.remote_signer.get_begin_multipart_upload_url(bucket, key)
-        # req
-        try:
-            res = requests.post(begin_url,
-                                headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)})
-        except Exception as e:
-            error_message = "request S3 multipart by url %s upload id exception: %s" % (begin_url, e)
-            logging.error("[API] %s" % error_message)
-            raise
-        if not res or not res.ok:
-            error_message = "request S3 multipart upload id failed, url: %s, code: %d" % (begin_url, res.status_code)
-            logging.error("[API] %s" % error_message)
-            raise RuntimeError(error_message)
-        # parse
-        try:
-            xml_tree = ElementTree.fromstring(res.content)
-            upload_id = xml_tree.find("UploadId").text
-            logging.info("[API] get multipart upload id: %s" % upload_id)
-            return upload_id
-        except Exception as e:
-            error_message = "parsing S3 multipart upload id from \"%s\" exception, %s" % (res.text, e)
-            logging.error("[API] %s" % error_message)
-            raise RuntimeError(error_message)
-        
-    def _upload_part(self, bucket, key, start, end, upload_id, part_number, disable_record=False):
-        upload_url = self.remote_signer.get_upload_part_url(bucket, key, upload_id, part_number)
-        res = utils.upload_part_of_file(upload_url, self.local_path, start, end-start+1, self._report)
-        if not res.is_succeeded():
-            err = "upload \"{0}\"th part failed, {1}".format(part_number, res.error_message())
-            logging.error("[API] %s" % err)
-            raise RuntimeError(err)
-        etag = res.data.headers.get("etag").strip('"')
-        if not disable_record:
-            self._save_progress(start, end, upload_id, part_number, etag)  # Save progress after part is uploaded
-        return (part_number, etag)
-    
-    def _complete_multipart_upload(self, bucket, key, upload_id, etags):
-        complete_url = self.remote_signer.get_complete_multipart_upload_url(bucket, key, upload_id)
-        etag_data = self._generate_etags_xml(etags)
-        # req
-        try:
-            res = requests.post(complete_url,
-                                headers={"content-type": "application/xml"}, data=etag_data)
-        except Exception as e:
-            error_message = "request complete S3 multipart by url %s upload id exception: %s" % (complete_url, e)
-            logging.error("[API] %s" % error_message)
-            raise
-        if not res or not res.ok:
-            error_message = "request complete S3 multipart upload id failed, url: %s, code: %d" % (complete_url, res.status_code)
-            logging.error("[API] %s" % error_message)
-            raise RuntimeError(error_message)
-        return
-        
-    def _upload(self, bucket, key):
-        upload_url = self.remote_signer.get_upload_url(bucket, key)
-        res = utils.upload_file(upload_url, self.local_path, self._report)
-        if not res.is_succeeded():
-            err = "upload failed, {0}".format(res.error_message())
-            logging.error("[API] %s" % err)
-            raise RuntimeError(err)
-        return 
-        
-    def _report(self, new_read_size):
-        if self.progress_callback:
-            self.progress_callback.report(new_read_size)
-
-    def _load_progress(self):
-        parts = []
-        etags = []
-        final_upload_id = ""
-        if os.path.exists(self.record_file):
-            with open(self.record_file, 'r') as f:
-                for line in f:
-                    obj = json.loads(line)
-                    parts.append((obj.get("start"), obj.get("end"), obj.get("part_size"), obj.get("upload_id"), obj.get("part_number")))
-                    etags.append((obj.get("part_number"), obj.get("etag")))
-            # check
-            for start, end, part_size, upload_id, part_number in parts:
-                if final_upload_id == "":
-                    final_upload_id = upload_id
-                if final_upload_id != upload_id or part_size != self.part_size:
-                    os.remove(self.record_file)
-                    parts = []
-                    etags = []
-                    break
-        return parts, etags, final_upload_id
-
-    def _save_progress(self, start, end, upload_id, part_number, etag):
-        with threading.Lock():  
-            with open(self.record_file, 'a') as f:
-                line = json.dumps({"start":start, "end":end, "part_size":self.part_size, "upload_id":upload_id, "part_number":part_number, "etag":etag })
-                f.write("{0}\n".format(line))
-
-    def simple_upload(self):
-        if os.path.exists(self.record_file):  # Remove existing progress record file
-            os.remove(self.record_file)
-        self._upload(self.bucket, self.key)
-                    
-    def upload(self, disable_record=False):
-        part_ranges = self._calculate_part_ranges()
-        
-        progress_record = []
-        progress_etags = []
-        upload_id = ""
-        if not disable_record:
-            progress_record, progress_etags, upload_id = self._load_progress()
-            # Call progress_callback with the existing progress if there is a progress record
-            if progress_record and self.progress_callback:
-                total_uploaded = sum(end - start + 1 for start, end, _, _, _ in progress_record)
-                self.progress_callback.report(total_uploaded)
-        
-        # begin multipart upload
-        if not upload_id:
-            upload_id = self._begin_multipart_upload(self.bucket, self.key, self.local_path)
-
-        # Use a ThreadPoolExecutor to limit the number of threads
-        with concurrent.futures.ThreadPoolExecutor(max_workers=self.thread_num) as executor:
-            # Submit upload tasks to the thread pool
-            futures = []
-            for start, end, part_number in part_ranges:
-                if (start, end, self.part_size, upload_id, part_number) not in progress_record:
-                    futures.append(executor.submit(self._upload_part, self.bucket, self.key, start, end, upload_id, part_number, disable_record))
-
-            # Wait for all upload part tasks to complete, allowing KeyboardInterrupt (Ctrl-C) to stop the process
-            try:
-                for future in concurrent.futures.as_completed(futures):
-                    progress_etags.append(future.result())
-            except KeyboardInterrupt as e:
-                print("Upload interrupted by user. Stopping...")
-                executor.shutdown(wait=False, cancel_futures=True)
-                raise e
-            
-        # end multipart upload
-        self._complete_multipart_upload(self.bucket, self.key, upload_id, progress_etags)
-        
-        if os.path.exists(self.record_file):  # Remove existing progress record file
-            os.remove(self.record_file)
-
-    def _calculate_part_ranges(self):
-        part_ranges = []
-        num_parts = self.file_size // self.part_size
-        if self.file_size % self.part_size != 0:
-            num_parts += 1
-
-        for i in range(num_parts):
-            start = i * self.part_size
-            end = min((i + 1) * self.part_size - 1, self.file_size - 1)
-            part_ranges.append((start, end, i+1))
-
-        return part_ranges
-
-    def _generate_etags_xml(self, etags):
-        root = ElementTree.Element('CompleteMultipartUpload')
-        etags = sorted(etags, key=lambda x: x[0])
-        for item in etags:
-            part = ElementTree.SubElement(root, 'Part')
-            etag = ElementTree.SubElement(part, 'ETag')
-            etag.text = item[1]
-            part_number = ElementTree.SubElement(part, 'PartNumber')
-            part_number.text = str(item[0])
-        return ElementTree.tostring(root)
-
-class BladeCOSApi(object):
-    """API to access THM pipeline installers on Blade storage."""
-    # user input:
-    def __init__(self, api, force=False, retry=3, cli=None, signer=None):
-        self.api = api
-        self.force = force
-        self.retry = retry
-        self.signer = signer
-        self.cli = cli
-        self.logger = logging.getLogger(__name__)
-        if self.signer is None:
-            self.signer = RemoteSigner(self.api, self.force)
-        if self.cli is None:
-            self.cli = Client(self.signer)
-
-    def check_file_exist(self, server_path):
-        try:
-            return self.cli.check_exists("", server_path)
-        except ValueError:
-            return False
-
-    def get_download_url(self, server_path):
-        """Get current download URL by given server_path.
-
-        Args:
-            server_path: Relative path on COS.
-            expired_time: Expired timestamps.
-
-        Returns:
-            - Current download URL.
-
-        """
-        return self.cli.get_download_url(
-            Bucket="",
-            Key=server_path,
-        )
-
-    @tenacity_retry(
-        stop=stop_after_attempt(5),
-        wait=wait_fixed(0.5),
-        retry=retry_if_exception_type(OSError)
-        | retry_if_exception_type(PermissionError)
-        | retry_if_exception_type(FileNotFoundError)
-    )
-    def download_file(self, server_path, local_path, progress_callback=None):
-        """Download file by given server path."""
-        return self.cli.download_file(
-            Bucket="",
-            Key=server_path,
-            DestFilePath=local_path,
-            MAXThread=10,
-            progress_callback=progress_callback,
-        )
-
-    @tenacity_retry(
-        stop=stop_after_attempt(5),
-        wait=wait_fixed(0.5),
-        retry=retry_if_exception_type(OSError)
-        | retry_if_exception_type(PermissionError)
-        | retry_if_exception_type(FileNotFoundError)
-    )
-    def upload_file(self, server_path, local_path, progress_callback=None):
-        """Upload file by given server path."""
-        return self.cli.upload_file(
-            Bucket="",
-            Key=server_path,
-            LocalFilePath=local_path,
-            MAXThread=10,
-            progress_callback=progress_callback,
-        )
-        
+# -*- coding:utf-8 -*-
+"""internal COS API can be used to upload and download files from COS."""
+
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+# Import built-in modules
+import six
+import logging
+import socket
+import os
+import time
+import threading
+import requests
+import concurrent
+import json
+import warnings
+
+# Import third-party modules
+import requests
+
+# Import third-party modules
+from tenacity import retry as tenacity_retry
+from tenacity import retry_if_exception_type
+from tenacity import stop_after_attempt
+from tenacity import wait_fixed
+from tenacity import RetryError
+from xml.etree import ElementTree
+
+# Import local modules
+from arthub_api.__version__ import __title__
+from arthub_api.blade_api import BladeAPI
+import arthub_api.utils as utils
+import arthub_api._internal_utils as _internal_utils
+
+
+logger = logging.getLogger(__title__)
+
+if six.PY2:
+    class PermissionError(OSError):
+        pass
+    class FileNotFoundError(IOError):
+        pass
+
+class SignerError(RuntimeError):
+    pass
+
+# signer for blade api
+class RemoteSigner(object):    
+    def __init__(self, blade_backend, force=False):
+        self.cli = blade_backend
+        self.force = force
+        
+    @classmethod
+    def _remove_suffix(cls, s, sf):
+        if s.endswith(sf):
+            return s[:len(s)-len(sf)]
+        return s
+
+    @classmethod
+    def _key_to_pkg(cls, key):
+        if not key.startswith("pkg_distribution/7z/"):
+            return {}
+        result = key.split("/")
+        if len(result) < 5:
+            return {}
+        result[4] = cls._remove_suffix(result[4], ".7z")
+        if result[2] != result[4]:
+            return {}
+        return {"name": result[2], "version": result[3]}
+    
+    def _take_signed_url(self, arthub_response, type_of_sign=""):
+        if not arthub_response.is_succeeded():
+            raise SignerError("arthub api: {0}".format(str(arthub_response.errors)))
+        logger.debug('{0} sign-url rsp is {1}'.format(type_of_sign, arthub_response.result))
+        if len(arthub_response.result) == 0:
+            raise SignerError("arthub api: result is empty")
+        return "https:" + arthub_response.result[0].get('signed_url')
+        
+    # we use bucket + key to identify a file. 
+    # however bucket might be fixed for ArtHub condition, so bucket input is ignored
+    def _get_package_download_sign(self, bucket, key):
+        pkg = self._key_to_pkg(key)
+        # this will return a url expires in 10 minutes
+        signed = self.cli.blade_download_package([pkg])
+        if not signed.is_succeeded():
+            raise SignerError("arthub api: {0}".format(str(signed.errors)))
+        logger.debug("download sign-url rsp is {0}".format(signed.result))
+        return signed.result
+    
+    def get_download_url(self, bucket, key):
+        signed = self._get_package_download_sign(bucket, key)
+        if len(signed) == 0:
+            raise SignerError("arthub api: result is empty")
+        return "https:" + signed[0].get('signed_url')
+        
+    def get_file_size(self, bucket, key):
+        signed = self._get_package_download_sign(bucket, key)
+        if len(signed) == 0:
+            raise SignerError("arthub api: result is empty")
+        return signed[0].get('size')
+    
+    def get_upload_url(self, bucket, key):
+        pkg = self._key_to_pkg(key)
+        signed = self.cli.blade_upload_package([pkg], self.force)
+        return self._take_signed_url(signed, "upload")
+    
+    def get_begin_multipart_upload_url(self, bucket, key):
+        pkg = self._key_to_pkg(key)
+        signed = self.cli.blade_begin_multipart_package_upload([pkg], self.force)
+        return self._take_signed_url(signed, "begin multipart upload")
+    
+    def get_upload_part_url(self, bucket, key, upload_id, part_number):
+        pkg = self._key_to_pkg(key)
+        pkg.update({"upload_id": upload_id, "part_number": part_number})
+        signed = self.cli.blade_part_package_upload([pkg], self.force)
+        return self._take_signed_url(signed, "upload part")
+    
+    def get_complete_multipart_upload_url(self, bucket, key, upload_id):
+        pkg = self._key_to_pkg(key)
+        pkg.update({"upload_id": upload_id})
+        signed = self.cli.blade_complete_multipart_package_upload([pkg], self.force)
+        return self._take_signed_url(signed, "end multipart upload")
+
+
+class ProgressCallback():
+    def __init__(self, file_size, progress_callback):
+        self.__lock = threading.Lock()
+        self.__finished_size = 0
+        self.__file_size = file_size
+        self.__progress_callback = progress_callback
+
+    def report(self, size):
+        with self.__lock:
+            self.__finished_size += size
+            self.__progress_callback(self.__finished_size, self.__file_size)
+            
+    def get(self):
+        return self.__finished_size, self.__file_size
+            
+    def get_percent(self):
+        return self.__finished_size / self.__file_size
+
+
+class Client(object):
+    def __init__(self, signer=None):
+        if signer is None:
+            raise ReferenceError("signer is None: must provide signer arg")
+        self.remote_signer = signer
+        
+    def download_file(self, Bucket, Key, DestFilePath, PartSize=20, MAXThread=5, EnableCRC=False, progress_callback=None):
+        if EnableCRC:
+            warnings.warn("EnableCRC is not supported")
+        part_size = PartSize * 1024 * 1024
+        file_size = self.remote_signer.get_file_size(Bucket, Key)
+        if file_size is None:
+            raise RetryError('failed to get file_size for {0}, file might not exist'.format(Key))
+        callback = None
+        if progress_callback:
+            callback = ProgressCallback(file_size, progress_callback)
+        resumable_downloader = ResumableDownLoader(self.remote_signer, Bucket, Key, DestFilePath, file_size, part_size, MAXThread, callback)
+        if file_size < 20 * 1024 * 1024:
+            resumable_downloader.simple_download()
+            return
+            
+        resumable_downloader.download()
+        
+    def upload_file(self, Bucket, Key, LocalFilePath, PartSize=20, MAXThread=5, EnableCRC=False, progress_callback=None):
+        if EnableCRC:
+            warnings.warn("EnableCRC is not supported")
+        if not os.path.isfile(LocalFilePath):
+            raise OSError("not found file: {0}".format(LocalFilePath))
+        file_size = os.path.getsize(LocalFilePath)
+        part_size = PartSize * 1024 * 1024
+        callback = None
+        if progress_callback:
+            callback = ProgressCallback(file_size, progress_callback)
+        resumableUploader = ResumableUploader(self.remote_signer, Bucket, Key, LocalFilePath, file_size, part_size, MAXThread, callback)
+        if file_size < 20 * 1024 * 1024:
+            resumableUploader.simple_upload()
+            return
+            
+        resumableUploader.upload()
+
+    def get_download_url(self, Bucket, Key):
+        return self.remote_signer.get_download_url(Bucket, Key)
+
+    # check file exists with http-get method
+    def check_exists(self, bucket, key):
+        headers = {'Range': 'bytes=0-0'}
+        self.download_url = self.remote_signer.get_download_url(bucket, key)
+        response = requests.get(self.download_url, headers=headers)
+        if response.status_code == 404:
+            return False
+        if response.status_code == 416:
+            return True
+        response.raise_for_status()
+        return True
+
+
+class ResumableDownLoader(object):
+    def __init__(self, remote_signer, bucket, key, local_path, file_size, part_size=5*1024*1024, thread_num=4, progress_callback=None):
+        self.remote_signer = remote_signer
+        self.bucket = bucket
+        self.key = key
+        self.local_path = local_path
+        self.part_size = part_size
+        self.thread_num = thread_num
+        self.progress_callback = progress_callback
+        self.file_size = file_size
+        self.download_url = None
+        self.url_expire_time = None
+        self.tmp_file = '{0}_ahtmp'.format(local_path)
+        self.record_file = '{0}_dl_ahrecord'.format(local_path)
+
+    def _refresh_download_url(self):
+        current_time = time.time()
+        if self.download_url is None or current_time >= self.url_expire_time:
+            self.download_url = self.remote_signer.get_download_url(self.bucket, self.key)
+            self.url_expire_time = current_time + 10 * 60  # 10 minutes expiry time
+
+    def _load_progress(self):
+        if os.path.exists(self.record_file):
+            with open(self.record_file, 'r') as f:
+                return [tuple(map(int, line.strip().split('-'))) for line in f]
+        return []
+
+    def _save_progress(self, start, end):
+        with threading.Lock():  
+            with open(self.record_file, 'a') as f:
+                f.write('{start}-{end}-{part_size}\n'.format(start=start, end=end, part_size=self.part_size))  # Save part_size along with the progress, part_size is not current chunk_length
+
+    def _download_part(self, start, end):
+        self._refresh_download_url()
+        headers = {'Range': 'bytes={start}-{end}'.format(start=start, end=end)}
+        response = requests.get(self.download_url, headers=headers, stream=True)
+        with open(self.tmp_file, 'rb+') as f:
+            f.seek(start)
+            for chunk in response.iter_content(chunk_size=8192):
+                f.write(chunk)
+                if self.progress_callback:
+                    self.progress_callback.report(len(chunk))
+        self._save_progress(start, end)  # Save progress after part is downloaded
+
+    def simple_download(self):
+        self._refresh_download_url()
+        response = requests.get(self.download_url, stream=True)
+        response.raise_for_status()
+        with open(self.tmp_file, 'wb') as f:
+            for chunk in response.iter_content(chunk_size=8192):
+                f.write(chunk)
+                if self.progress_callback:
+                    self.progress_callback.report(len(chunk))
+        try:
+            os.remove(self.local_path)
+        except:
+            pass
+        os.rename(self.tmp_file, self.local_path)
+        if os.path.exists(self.record_file):  # Remove existing progress record file
+            os.remove(self.record_file)
+                    
+    def download(self):
+        self._refresh_download_url()
+        part_ranges = self._calculate_part_ranges()
+        progress_record = self._load_progress()
+        
+        # create if not exists
+        with open(self.tmp_file,"a+"):
+            pass
+            
+        # Call progress_callback with the existing progress if there is a progress record
+        if progress_record and self.progress_callback:
+            total_downloaded = sum(end - start + 1 for start, end, _ in progress_record)
+            self.progress_callback.report(total_downloaded)
+
+        # Use a ThreadPoolExecutor to limit the number of threads
+        with concurrent.futures.ThreadPoolExecutor(max_workers=self.thread_num) as executor:
+            # Submit download tasks to the thread pool
+            futures = [executor.submit(self._download_part, start, end) for start, end in part_ranges if (start, end, self.part_size) not in progress_record]
+
+            # Wait for all download tasks to complete, allowing KeyboardInterrupt (Ctrl-C) to stop the process
+            try:
+                for future in concurrent.futures.as_completed(futures):
+                    future.result()
+            except KeyboardInterrupt as e:
+                print("Download interrupted by user. Stopping...")
+                executor.shutdown(wait=False, cancel_futures=True)
+                raise e
+        try:
+            os.remove(self.local_path)
+        except:
+            pass
+        os.rename(self.tmp_file, self.local_path)
+        if os.path.exists(self.record_file):  # Remove existing progress record file
+            os.remove(self.record_file)
+
+    def _calculate_part_ranges(self):
+        part_ranges = []
+        num_parts = self.file_size // self.part_size
+        if self.file_size % self.part_size != 0:
+            num_parts += 1
+
+        for i in range(num_parts):
+            start = i * self.part_size
+            end = min((i + 1) * self.part_size - 1, self.file_size - 1)
+            part_ranges.append((start, end))
+
+        return part_ranges
+    
+
+class ResumableUploader(object):
+    def __init__(self, remote_signer, bucket, key, local_path, file_size, part_size=5*1024*1024, thread_num=4, progress_callback=None):
+        self.remote_signer = remote_signer
+        self.bucket = bucket
+        self.key = key
+        self.local_path = local_path
+        self.part_size = part_size
+        self.thread_num = thread_num
+        self.progress_callback = progress_callback
+        self.file_size = file_size
+        self.upload_url = None
+        self.url_expire_time = None
+        self.record_file = '{0}_ul_ahrecord'.format(local_path)
+        
+    def _begin_multipart_upload(self, bucket, key, file_name):
+        begin_url = self.remote_signer.get_begin_multipart_upload_url(bucket, key)
+        # req
+        try:
+            res = requests.post(begin_url,
+                                headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)})
+        except Exception as e:
+            error_message = "request S3 multipart by url %s upload id exception: %s" % (begin_url, e)
+            logging.error("[API] %s" % error_message)
+            raise
+        if not res or not res.ok:
+            error_message = "request S3 multipart upload id failed, url: %s, code: %d" % (begin_url, res.status_code)
+            logging.error("[API] %s" % error_message)
+            raise RuntimeError(error_message)
+        # parse
+        try:
+            xml_tree = ElementTree.fromstring(res.content)
+            upload_id = xml_tree.find("UploadId").text
+            logging.info("[API] get multipart upload id: %s" % upload_id)
+            return upload_id
+        except Exception as e:
+            error_message = "parsing S3 multipart upload id from \"%s\" exception, %s" % (res.text, e)
+            logging.error("[API] %s" % error_message)
+            raise RuntimeError(error_message)
+        
+    def _upload_part(self, bucket, key, start, end, upload_id, part_number, disable_record=False):
+        upload_url = self.remote_signer.get_upload_part_url(bucket, key, upload_id, part_number)
+        res = utils.upload_part_of_file(upload_url, self.local_path, start, end-start+1, self._report)
+        if not res.is_succeeded():
+            err = "upload \"{0}\"th part failed, {1}".format(part_number, res.error_message())
+            logging.error("[API] %s" % err)
+            raise RuntimeError(err)
+        etag = res.data.headers.get("etag").strip('"')
+        if not disable_record:
+            self._save_progress(start, end, upload_id, part_number, etag)  # Save progress after part is uploaded
+        return (part_number, etag)
+    
+    def _complete_multipart_upload(self, bucket, key, upload_id, etags):
+        complete_url = self.remote_signer.get_complete_multipart_upload_url(bucket, key, upload_id)
+        etag_data = self._generate_etags_xml(etags)
+        # req
+        try:
+            res = requests.post(complete_url,
+                                headers={"content-type": "application/xml"}, data=etag_data)
+        except Exception as e:
+            error_message = "request complete S3 multipart by url %s upload id exception: %s" % (complete_url, e)
+            logging.error("[API] %s" % error_message)
+            raise
+        if not res or not res.ok:
+            error_message = "request complete S3 multipart upload id failed, url: %s, code: %d" % (complete_url, res.status_code)
+            logging.error("[API] %s" % error_message)
+            raise RuntimeError(error_message)
+        return
+        
+    def _upload(self, bucket, key):
+        upload_url = self.remote_signer.get_upload_url(bucket, key)
+        res = utils.upload_file(upload_url, self.local_path, self._report)
+        if not res.is_succeeded():
+            err = "upload failed, {0}".format(res.error_message())
+            logging.error("[API] %s" % err)
+            raise RuntimeError(err)
+        return 
+        
+    def _report(self, new_read_size):
+        if self.progress_callback:
+            self.progress_callback.report(new_read_size)
+
+    def _load_progress(self):
+        parts = []
+        etags = []
+        final_upload_id = ""
+        if os.path.exists(self.record_file):
+            with open(self.record_file, 'r') as f:
+                for line in f:
+                    obj = json.loads(line)
+                    parts.append((obj.get("start"), obj.get("end"), obj.get("part_size"), obj.get("upload_id"), obj.get("part_number")))
+                    etags.append((obj.get("part_number"), obj.get("etag")))
+            # check
+            for start, end, part_size, upload_id, part_number in parts:
+                if final_upload_id == "":
+                    final_upload_id = upload_id
+                if final_upload_id != upload_id or part_size != self.part_size:
+                    os.remove(self.record_file)
+                    parts = []
+                    etags = []
+                    break
+        return parts, etags, final_upload_id
+
+    def _save_progress(self, start, end, upload_id, part_number, etag):
+        with threading.Lock():  
+            with open(self.record_file, 'a') as f:
+                line = json.dumps({"start":start, "end":end, "part_size":self.part_size, "upload_id":upload_id, "part_number":part_number, "etag":etag })
+                f.write("{0}\n".format(line))
+
+    def simple_upload(self):
+        if os.path.exists(self.record_file):  # Remove existing progress record file
+            os.remove(self.record_file)
+        self._upload(self.bucket, self.key)
+                    
+    def upload(self, disable_record=False):
+        part_ranges = self._calculate_part_ranges()
+        
+        progress_record = []
+        progress_etags = []
+        upload_id = ""
+        if not disable_record:
+            progress_record, progress_etags, upload_id = self._load_progress()
+            # Call progress_callback with the existing progress if there is a progress record
+            if progress_record and self.progress_callback:
+                total_uploaded = sum(end - start + 1 for start, end, _, _, _ in progress_record)
+                self.progress_callback.report(total_uploaded)
+        
+        # begin multipart upload
+        if not upload_id:
+            upload_id = self._begin_multipart_upload(self.bucket, self.key, self.local_path)
+
+        # Use a ThreadPoolExecutor to limit the number of threads
+        with concurrent.futures.ThreadPoolExecutor(max_workers=self.thread_num) as executor:
+            # Submit upload tasks to the thread pool
+            futures = []
+            for start, end, part_number in part_ranges:
+                if (start, end, self.part_size, upload_id, part_number) not in progress_record:
+                    futures.append(executor.submit(self._upload_part, self.bucket, self.key, start, end, upload_id, part_number, disable_record))
+
+            # Wait for all upload part tasks to complete, allowing KeyboardInterrupt (Ctrl-C) to stop the process
+            try:
+                for future in concurrent.futures.as_completed(futures):
+                    progress_etags.append(future.result())
+            except KeyboardInterrupt as e:
+                print("Upload interrupted by user. Stopping...")
+                executor.shutdown(wait=False, cancel_futures=True)
+                raise e
+            
+        # end multipart upload
+        self._complete_multipart_upload(self.bucket, self.key, upload_id, progress_etags)
+        
+        if os.path.exists(self.record_file):  # Remove existing progress record file
+            os.remove(self.record_file)
+
+    def _calculate_part_ranges(self):
+        part_ranges = []
+        num_parts = self.file_size // self.part_size
+        if self.file_size % self.part_size != 0:
+            num_parts += 1
+
+        for i in range(num_parts):
+            start = i * self.part_size
+            end = min((i + 1) * self.part_size - 1, self.file_size - 1)
+            part_ranges.append((start, end, i+1))
+
+        return part_ranges
+
+    def _generate_etags_xml(self, etags):
+        root = ElementTree.Element('CompleteMultipartUpload')
+        etags = sorted(etags, key=lambda x: x[0])
+        for item in etags:
+            part = ElementTree.SubElement(root, 'Part')
+            etag = ElementTree.SubElement(part, 'ETag')
+            etag.text = item[1]
+            part_number = ElementTree.SubElement(part, 'PartNumber')
+            part_number.text = str(item[0])
+        return ElementTree.tostring(root)
+
+class BladeCOSApi(object):
+    """API to access THM pipeline installers on Blade storage."""
+    # user input:
+    def __init__(self, api, force=False, retry=3, cli=None, signer=None):
+        self.api = api
+        self.force = force
+        self.retry = retry
+        self.signer = signer
+        self.cli = cli
+        self.logger = logging.getLogger(__name__)
+        if self.signer is None:
+            self.signer = RemoteSigner(self.api, self.force)
+        if self.cli is None:
+            self.cli = Client(self.signer)
+
+    def check_file_exist(self, server_path):
+        try:
+            return self.cli.check_exists("", server_path)
+        except ValueError:
+            return False
+
+    def get_download_url(self, server_path):
+        """Get current download URL by given server_path.
+
+        Args:
+            server_path: Relative path on COS.
+            expired_time: Expired timestamps.
+
+        Returns:
+            - Current download URL.
+
+        """
+        return self.cli.get_download_url(
+            Bucket="",
+            Key=server_path,
+        )
+
+    @tenacity_retry(
+        stop=stop_after_attempt(5),
+        wait=wait_fixed(0.5),
+        retry=retry_if_exception_type(OSError)
+        | retry_if_exception_type(PermissionError)
+        | retry_if_exception_type(FileNotFoundError)
+    )
+    def download_file(self, server_path, local_path, progress_callback=None):
+        """Download file by given server path."""
+        return self.cli.download_file(
+            Bucket="",
+            Key=server_path,
+            DestFilePath=local_path,
+            MAXThread=10,
+            progress_callback=progress_callback,
+        )
+
+    @tenacity_retry(
+        stop=stop_after_attempt(5),
+        wait=wait_fixed(0.5),
+        retry=retry_if_exception_type(OSError)
+        | retry_if_exception_type(PermissionError)
+        | retry_if_exception_type(FileNotFoundError)
+    )
+    def upload_file(self, server_path, local_path, progress_callback=None):
+        """Upload file by given server path."""
+        return self.cli.upload_file(
+            Bucket="",
+            Key=server_path,
+            LocalFilePath=local_path,
+            MAXThread=10,
+            progress_callback=progress_callback,
+        )
+
```

### Comparing `arthub_api-1.6.6/arthub_api/config.py` & `arthub_api-1.6.7/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/arthub_api/exception.py` & `arthub_api-1.6.7/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/arthub_api/models.py` & `arthub_api-1.6.7/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/arthub_api/open_api.py` & `arthub_api-1.6.7/arthub_api/open_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,14 +375,24 @@
         """
 
         if type(cookie) is str:
             self._cookies = utils.parse_cookies(cookie)
         elif type(cookie) is dict:
             self._cookies = cookie
 
+    def has_credential(self):
+        r"""Checks if credential is already set or not"""
+        if self._public_token:
+            return True
+        if self._cookies:
+            return True
+        if self._token:
+            return True
+        return False
+
     def reset_config(self, config):
         self._config = config
 
     def init_from_config(self):
         self.reset_config(utils.get_config_by_name(arthub_api_config.api_config_name, self.config))
 
     def _depot_url(self, asset_hub, api_method):
```

### Comparing `arthub_api-1.6.6/arthub_api/storage.py` & `arthub_api-1.6.7/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/arthub_api/utils.py` & `arthub_api-1.6.7/arthub_api/utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.6.7/arthub_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.6.6
+Version: 1.6.7
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.6/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.6.7/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/setup.py` & `arthub_api-1.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/tests/test_open_api.py` & `arthub_api-1.6.7/tests/test_open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/tests/test_open_api_blade.py` & `arthub_api-1.6.7/tests/test_open_api_blade.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.6/tests/test_storage.py` & `arthub_api-1.6.7/tests/test_storage.py`

 * *Files identical despite different names*

