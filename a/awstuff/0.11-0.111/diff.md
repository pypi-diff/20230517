# Comparing `tmp/awstuff-0.11.tar.gz` & `tmp/awstuff-0.111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awstuff-0.11.tar", last modified: Wed May 17 18:13:10 2023, max compression
+gzip compressed data, was "awstuff-0.111.tar", last modified: Wed May 17 19:21:09 2023, max compression
```

## Comparing `awstuff-0.11.tar` & `awstuff-0.111.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 18:13:10.310687 awstuff-0.11/
--rw-rw-rw-   0        0        0      237 2023-05-17 18:13:10.311687 awstuff-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 18:13:10.296688 awstuff-0.11/awstuff/
--rw-rw-rw-   0        0        0     3454 2023-05-17 18:09:00.000000 awstuff-0.11/awstuff/Functions.py
--rw-rw-rw-   0        0        0       33 2023-05-17 00:29:39.000000 awstuff-0.11/awstuff/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 18:13:10.309686 awstuff-0.11/awstuff.egg-info/
--rw-rw-rw-   0        0        0      237 2023-05-17 18:13:10.000000 awstuff-0.11/awstuff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-17 18:13:10.000000 awstuff-0.11/awstuff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 18:13:10.000000 awstuff-0.11/awstuff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 00:31:25.000000 awstuff-0.11/awstuff.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-05-17 18:13:10.000000 awstuff-0.11/awstuff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 18:13:10.312688 awstuff-0.11/setup.cfg
--rw-rw-rw-   0        0        0      256 2023-05-17 18:09:19.000000 awstuff-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:09.035664 awstuff-0.111/
+-rw-rw-rw-   0        0        0      238 2023-05-17 19:21:09.035664 awstuff-0.111/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:09.015665 awstuff-0.111/awstuff/
+-rw-rw-rw-   0        0        0     3459 2023-05-17 19:14:46.000000 awstuff-0.111/awstuff/Functions.py
+-rw-rw-rw-   0        0        0       33 2023-05-17 00:29:39.000000 awstuff-0.111/awstuff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:09.034663 awstuff-0.111/awstuff.egg-info/
+-rw-rw-rw-   0        0        0      238 2023-05-17 19:21:08.000000 awstuff-0.111/awstuff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-17 19:21:08.000000 awstuff-0.111/awstuff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 19:21:08.000000 awstuff-0.111/awstuff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 00:31:25.000000 awstuff-0.111/awstuff.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-05-17 19:21:08.000000 awstuff-0.111/awstuff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 19:21:09.040666 awstuff-0.111/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-05-17 19:21:02.000000 awstuff-0.111/setup.py
```

### Comparing `awstuff-0.11/awstuff/Functions.py` & `awstuff-0.111/awstuff/Functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         Args:
             s3 (boto3 resource): boto3 S3 resource
             source (S3 bucket): source S3 bucket
             source_prefix (String): prefix for objects in source
             dest (S3 bucket): destination S3 bucket
             dest_prefix (String): prefix for objects in destination
         """
-        missing_keys = self.diff_bucket_objs(s3, source, source_prefix, dest, dest_prefix)
+        missing_keys = Functions.diff_bucket_objs(s3, source, source_prefix, dest, dest_prefix)
         ct = 0
         for key in missing_keys:
             key_dict = {'Bucket' : source, 'Key': f'{source_prefix}{key}'}
             s3.Bucket(dest).copy(key_dict, f'{dest_prefix}{key}')
             print (f'Copied over: {key}')
             ct += 1
         print (f'Extraction complete, {dest_prefix} folder on destination bucket updated. {ct} objects copied over.')
```

