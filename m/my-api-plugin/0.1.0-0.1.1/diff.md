# Comparing `tmp/my-api-plugin-0.1.0.tar.gz` & `tmp/my-api-plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-api-plugin-0.1.0.tar", last modified: Tue May 16 09:30:59 2023, max compression
+gzip compressed data, was "my-api-plugin-0.1.1.tar", last modified: Wed May 17 00:55:51 2023, max compression
```

## Comparing `my-api-plugin-0.1.0.tar` & `my-api-plugin-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-16 09:30:59.209321 my-api-plugin-0.1.0/
--rw-r--r--   0 wangchan   (501) staff       (20)      262 2023-05-16 09:30:59.209075 my-api-plugin-0.1.0/PKG-INFO
--rw-r--r--   0 wangchan   (501) staff       (20)        0 2023-05-16 08:39:47.000000 my-api-plugin-0.1.0/README.md
-drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-16 09:30:59.207139 my-api-plugin-0.1.0/my_api_plugin/
--rw-r--r--   0 wangchan   (501) staff       (20)       33 2023-05-16 09:27:54.000000 my-api-plugin-0.1.0/my_api_plugin/__init__.py
--rw-r--r--   0 wangchan   (501) staff       (20)     1613 2023-05-16 09:27:56.000000 my-api-plugin-0.1.0/my_api_plugin/api_client.py
-drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-16 09:30:59.208782 my-api-plugin-0.1.0/my_api_plugin.egg-info/
--rw-r--r--   0 wangchan   (501) staff       (20)      262 2023-05-16 09:30:59.000000 my-api-plugin-0.1.0/my_api_plugin.egg-info/PKG-INFO
--rw-r--r--   0 wangchan   (501) staff       (20)      256 2023-05-16 09:30:59.000000 my-api-plugin-0.1.0/my_api_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 wangchan   (501) staff       (20)        1 2023-05-16 09:30:59.000000 my-api-plugin-0.1.0/my_api_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 wangchan   (501) staff       (20)        9 2023-05-16 09:30:59.000000 my-api-plugin-0.1.0/my_api_plugin.egg-info/requires.txt
--rw-r--r--   0 wangchan   (501) staff       (20)       14 2023-05-16 09:30:59.000000 my-api-plugin-0.1.0/my_api_plugin.egg-info/top_level.txt
--rw-r--r--   0 wangchan   (501) staff       (20)       38 2023-05-16 09:30:59.209380 my-api-plugin-0.1.0/setup.cfg
--rw-r--r--   0 wangchan   (501) staff       (20)      347 2023-05-16 09:29:35.000000 my-api-plugin-0.1.0/setup.py
+drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-17 00:55:51.600656 my-api-plugin-0.1.1/
+-rw-r--r--   0 wangchan   (501) staff       (20)      262 2023-05-17 00:55:51.600462 my-api-plugin-0.1.1/PKG-INFO
+-rw-r--r--   0 wangchan   (501) staff       (20)        0 2023-05-16 08:39:47.000000 my-api-plugin-0.1.1/README.md
+drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-17 00:55:51.598766 my-api-plugin-0.1.1/my_api_plugin/
+-rw-r--r--   0 wangchan   (501) staff       (20)       33 2023-05-16 09:27:54.000000 my-api-plugin-0.1.1/my_api_plugin/__init__.py
+-rw-r--r--   0 wangchan   (501) staff       (20)     1613 2023-05-16 09:27:56.000000 my-api-plugin-0.1.1/my_api_plugin/api_client.py
+drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-17 00:55:51.600185 my-api-plugin-0.1.1/my_api_plugin.egg-info/
+-rw-r--r--   0 wangchan   (501) staff       (20)      262 2023-05-17 00:55:51.000000 my-api-plugin-0.1.1/my_api_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 wangchan   (501) staff       (20)      256 2023-05-17 00:55:51.000000 my-api-plugin-0.1.1/my_api_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 wangchan   (501) staff       (20)        1 2023-05-17 00:55:51.000000 my-api-plugin-0.1.1/my_api_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 wangchan   (501) staff       (20)        9 2023-05-17 00:55:51.000000 my-api-plugin-0.1.1/my_api_plugin.egg-info/requires.txt
+-rw-r--r--   0 wangchan   (501) staff       (20)       14 2023-05-17 00:55:51.000000 my-api-plugin-0.1.1/my_api_plugin.egg-info/top_level.txt
+-rw-r--r--   0 wangchan   (501) staff       (20)       38 2023-05-17 00:55:51.600736 my-api-plugin-0.1.1/setup.cfg
+-rw-r--r--   0 wangchan   (501) staff       (20)      347 2023-05-17 00:55:42.000000 my-api-plugin-0.1.1/setup.py
```

### Comparing `my-api-plugin-0.1.0/my_api_plugin/api_client.py` & `my-api-plugin-0.1.1/my_api_plugin/api_client.py`

 * *Files identical despite different names*

