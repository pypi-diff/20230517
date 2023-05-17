# Comparing `tmp/py-bigquery-mock-0.2.1.tar.gz` & `tmp/py-bigquery-mock-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-bigquery-mock-0.2.1.tar", last modified: Wed May 17 18:22:49 2023, max compression
+gzip compressed data, was "py-bigquery-mock-0.2.2.tar", last modified: Wed May 17 21:33:56 2023, max compression
```

## Comparing `py-bigquery-mock-0.2.1.tar` & `py-bigquery-mock-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 18:22:49.937161 py-bigquery-mock-0.2.1/
--rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.2.1/LICENSE
--rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-17 18:22:49.937038 py-bigquery-mock-0.2.1/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305      464 2023-05-16 19:55:28.000000 py-bigquery-mock-0.2.1/README.md
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 18:22:49.936041 py-bigquery-mock-0.2.1/bigquery_mock/
--rw-r--r--   0 phtremblay (2028354092) 932231305       52 2023-05-17 18:20:55.000000 py-bigquery-mock-0.2.1/bigquery_mock/__init__.py
--rw-r--r--   0 phtremblay (2028354092) 932231305     3195 2023-05-16 20:40:11.000000 py-bigquery-mock-0.2.1/bigquery_mock/bigquery_mock.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 18:22:49.936879 py-bigquery-mock-0.2.1/py_bigquery_mock.egg-info/
--rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-17 18:22:49.000000 py-bigquery-mock-0.2.1/py_bigquery_mock.egg-info/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305      243 2023-05-17 18:22:49.000000 py-bigquery-mock-0.2.1/py_bigquery_mock.egg-info/SOURCES.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-17 18:22:49.000000 py-bigquery-mock-0.2.1/py_bigquery_mock.egg-info/dependency_links.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       14 2023-05-17 18:22:49.000000 py-bigquery-mock-0.2.1/py_bigquery_mock.egg-info/top_level.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-17 18:22:49.937201 py-bigquery-mock-0.2.1/setup.cfg
--rw-r--r--   0 phtremblay (2028354092) 932231305      407 2023-05-17 18:20:35.000000 py-bigquery-mock-0.2.1/setup.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 21:33:56.226072 py-bigquery-mock-0.2.2/
+-rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.2.2/LICENSE
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-17 21:33:56.225896 py-bigquery-mock-0.2.2/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305      464 2023-05-16 19:55:28.000000 py-bigquery-mock-0.2.2/README.md
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 21:33:56.225156 py-bigquery-mock-0.2.2/bigquery_mock/
+-rw-r--r--   0 phtremblay (2028354092) 932231305       52 2023-05-17 20:43:14.000000 py-bigquery-mock-0.2.2/bigquery_mock/__init__.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305     3195 2023-05-16 20:40:11.000000 py-bigquery-mock-0.2.2/bigquery_mock/bigquery_mock.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 21:33:56.225276 py-bigquery-mock-0.2.2/bigquery_mock/scripts/
+-rw-r--r--   0 phtremblay (2028354092) 932231305     1856 2023-05-17 20:17:35.000000 py-bigquery-mock-0.2.2/bigquery_mock/scripts/mkmock.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 21:33:56.225750 py-bigquery-mock-0.2.2/py_bigquery_mock.egg-info/
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-17 21:33:56.000000 py-bigquery-mock-0.2.2/py_bigquery_mock.egg-info/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305      275 2023-05-17 21:33:56.000000 py-bigquery-mock-0.2.2/py_bigquery_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-17 21:33:56.000000 py-bigquery-mock-0.2.2/py_bigquery_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       14 2023-05-17 21:33:56.000000 py-bigquery-mock-0.2.2/py_bigquery_mock.egg-info/top_level.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-17 21:33:56.226112 py-bigquery-mock-0.2.2/setup.cfg
+-rw-r--r--   0 phtremblay (2028354092) 932231305      456 2023-05-17 20:45:23.000000 py-bigquery-mock-0.2.2/setup.py
```

### Comparing `py-bigquery-mock-0.2.1/LICENSE` & `py-bigquery-mock-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-bigquery-mock-0.2.1/bigquery_mock/bigquery_mock.py` & `py-bigquery-mock-0.2.2/bigquery_mock/bigquery_mock.py`

 * *Files identical despite different names*

