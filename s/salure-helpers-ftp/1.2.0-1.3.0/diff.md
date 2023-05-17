# Comparing `tmp/salure_helpers_ftp-1.2.0.tar.gz` & `tmp/salure_helpers_ftp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_ftp-1.2.0.tar", last modified: Tue Jan 24 12:55:04 2023, max compression
+gzip compressed data, was "dist/salure_helpers_ftp-1.3.0.tar", last modified: Wed May 17 09:24:26 2023, max compression
```

## Comparing `salure_helpers_ftp-1.2.0.tar` & `salure_helpers_ftp-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      253 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/salure_helpers/ftp/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-01-24 12:54:52.000000 salure_helpers_ftp-1.2.0/salure_helpers/ftp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7491 2023-01-24 12:54:52.000000 salure_helpers_ftp-1.2.0/salure_helpers/ftp/ftps.py
--rw-rw-rw-   0 root         (0) root         (0)     6231 2023-01-24 12:54:52.000000 salure_helpers_ftp-1.2.0/salure_helpers/ftp/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/salure_helpers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      253 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/salure_helpers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/salure_helpers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/salure_helpers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/salure_helpers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       64 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/salure_helpers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/salure_helpers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-24 12:55:04.000000 salure_helpers_ftp-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-01-24 12:54:52.000000 salure_helpers_ftp-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/salure_helpers/ftp/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-17 09:24:11.000000 salure_helpers_ftp-1.3.0/salure_helpers/ftp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9010 2023-05-17 09:24:11.000000 salure_helpers_ftp-1.3.0/salure_helpers/ftp/ftps.py
+-rw-rw-rw-   0 root         (0) root         (0)     6231 2023-05-17 09:24:11.000000 salure_helpers_ftp-1.3.0/salure_helpers/ftp/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/salure_helpers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/salure_helpers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/salure_helpers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/salure_helpers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/salure_helpers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/salure_helpers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/salure_helpers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 09:24:26.000000 salure_helpers_ftp-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-05-17 09:24:11.000000 salure_helpers_ftp-1.3.0/setup.py
```

### Comparing `salure_helpers_ftp-1.2.0/salure_helpers/ftp/ftps.py` & `salure_helpers_ftp-1.3.0/salure_helpers/ftp/ftps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import os
 import ftplib
 import time
 from ftplib import FTP
 from salure_helpers.salureconnect import SalureConnect
 from typing import Union, List
+from tenacity import retry, stop_after_attempt, wait_exponential_jitter, retry_if_exception
+
+
+def is_ftp_exception(e: BaseException) -> bool:
+    if isinstance(e, ftplib.all_errors):
+        error = str(e)[:400].replace('\'', '').replace('\"', '')
+        print(f"{error}, retrying")
+        return True
+    else:
+        return False
 
 
 class FTPS(SalureConnect):
     def __init__(self, label: Union[str, List] = None, debug=False):
         super().__init__()
         if label is not None:
             credentials = self.get_system_credential(system='ftps', label=label)
@@ -18,14 +28,15 @@
             self.host = os.getenv("QLIK_HOST")
             self.username = os.getenv("QLIK_USER")
             self.password = os.getenv("QLIK_PASSWORD")
         else:
             raise ValueError("Set the environment variables QLIK_HOST, QLIK_USER and QLIK_PASSWORD or provide the label parameter for a credential from SalureConnect")
         self.debug = debug
 
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_ftp_exception), reraise=True)
     def upload_file(self, local_path, filename, remote_path):
         """
         Upload a file from the client to another client or server
         :param local_path: the path where the upload file is located
         :param filename: The file which should be uploaded
         :param remote_path: The path on the destination client where the file should be saved
         :return: a status if the upload is succesfull or not
@@ -44,14 +55,15 @@
                             continue
                         else:
                             raise
                     break
             ftp.close()
             return 'File is transferred'
 
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_ftp_exception), reraise=True)
     def upload_multiple_files(self, local_path, remote_path):
         """
         Upload all files in a directory from the client to another client or server
         :param local_path: the path from where all the files should be uploaded
         :param remote_path: The path on the destination client where the file should be saved
         :return: a status if the upload is succesfull or not
         """
@@ -74,14 +86,15 @@
                                 continue
                             else:
                                 raise
                         break
         ftp.close()
         return 'All files are transferred'
 
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_ftp_exception), reraise=True)
     def download_file(self, local_path, remote_path, filename, remove_after_download=False):
         """
         Returns a single file from a given remote path
         :param local_path: the folder where the downloaded file should be stored
         :param remote_path: the folder on the server where the file should be downloaded from
         :param filename: the filename itself
         :param remove_after_download: Should the file be removed on the server after the download or not
@@ -98,37 +111,40 @@
                         os.remove(f'{local_path}/{filename}')
                 else:
                     if remove_after_download:
                         ftp.delete(filename)
 
                 return res
 
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_ftp_exception), reraise=True)
     def make_dir(self, dir_name):
         """
         Create a directory on a remote machine
         :param dir_name: give the path name which should be created
         :return: the status if the creation is successfull or not
         """
         with FTP(host=self.host, user=self.username, passwd=self.password) as ftp:
             status = ftp.mkd(dir_name)
             return status
 
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_ftp_exception), reraise=True)
     def list_directories(self, remote_path=''):
         """
         Give a NoneType of directories and files in a given directory. This one is only for information. The Nonetype
         can't be iterated or something like that
         :param remote_path: give the folder where to start in
         :return: a NoneType with folders and files
         """
         with FTP(host=self.host, user=self.username, passwd=self.password) as ftp:
             ftp.cwd(remote_path)
             if self.debug:
                 print(ftp.dir())
             return ftp.dir()
 
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_ftp_exception), reraise=True)
     def make_dirs(self, filepath: str):
         """
         shadows os.makedirs but for ftp
         :param filepath: filepath that you want to create
         :return: nothing
         """
         filepath = filepath.split('/')
@@ -140,26 +156,28 @@
                     ftp.retrlines('NLST', file_list.append)
                     if subpath in file_list:
                         ftp.cwd(subpath)
                     else:
                         ftp.mkd(subpath)
                         ftp.cwd(subpath)
 
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_ftp_exception), reraise=True)
     def list_files(self, remote_path=''):
         """
         Give a list with files in a certain folder
         :param remote_path: give the folder where to look in
         :return: a list with files
         """
         with FTP(host=self.host, user=self.username, passwd=self.password) as ftp:
             ftp.cwd(remote_path)
             if self.debug:
                 print(ftp.nlst())
             return ftp.nlst()
 
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_ftp_exception), reraise=True)
     def remove_file(self, remote_filepath):
         """
         Remove a file on a remote location
         :param remote_file: the full path of the file that needs to be removed
         """
         with FTP(host=self.host, user=self.username, passwd=self.password) as ftp:
             ftp.delete(remote_filepath)
```

### Comparing `salure_helpers_ftp-1.2.0/salure_helpers/ftp/sftp.py` & `salure_helpers_ftp-1.3.0/salure_helpers/ftp/sftp.py`

 * *Files identical despite different names*

