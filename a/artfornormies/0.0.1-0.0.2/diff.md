# Comparing `tmp/artfornormies-0.0.1.tar.gz` & `tmp/artfornormies-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artfornormies-0.0.1.tar", last modified: Tue Feb 28 22:10:48 2023, max compression
+gzip compressed data, was "artfornormies-0.0.2.tar", last modified: Wed May 17 19:00:35 2023, max compression
```

## Comparing `artfornormies-0.0.1.tar` & `artfornormies-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 jonathanchan   (501) staff       (20)        0 2023-02-28 22:10:48.538399 artfornormies-0.0.1/
--rw-r--r--   0 jonathanchan   (501) staff       (20)     1069 2023-02-28 21:49:20.000000 artfornormies-0.0.1/LICENSE
--rw-r--r--   0 jonathanchan   (501) staff       (20)        0 2023-02-28 22:07:49.000000 artfornormies-0.0.1/MANIFEST.in
--rw-r--r--   0 jonathanchan   (501) staff       (20)      826 2023-02-28 22:10:48.538605 artfornormies-0.0.1/PKG-INFO
--rw-r--r--   0 jonathanchan   (501) staff       (20)      318 2023-02-28 21:46:50.000000 artfornormies-0.0.1/README.md
-drwxr-xr-x   0 jonathanchan   (501) staff       (20)        0 2023-02-28 22:10:48.534789 artfornormies-0.0.1/artfornormies/
--rw-r--r--   0 jonathanchan   (501) staff       (20)        0 2023-02-28 22:01:52.000000 artfornormies-0.0.1/artfornormies/__init__.py
--rw-r--r--   0 jonathanchan   (501) staff       (20)    14260 2023-01-16 18:15:03.000000 artfornormies-0.0.1/artfornormies/functions.py
-drwxr-xr-x   0 jonathanchan   (501) staff       (20)        0 2023-02-28 22:10:48.537888 artfornormies-0.0.1/artfornormies.egg-info/
--rw-r--r--   0 jonathanchan   (501) staff       (20)      826 2023-02-28 22:10:48.000000 artfornormies-0.0.1/artfornormies.egg-info/PKG-INFO
--rw-r--r--   0 jonathanchan   (501) staff       (20)      255 2023-02-28 22:10:48.000000 artfornormies-0.0.1/artfornormies.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanchan   (501) staff       (20)        1 2023-02-28 22:10:48.000000 artfornormies-0.0.1/artfornormies.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanchan   (501) staff       (20)       14 2023-02-28 22:10:48.000000 artfornormies-0.0.1/artfornormies.egg-info/top_level.txt
--rw-r--r--   0 jonathanchan   (501) staff       (20)      103 2023-02-28 21:48:12.000000 artfornormies-0.0.1/pyproject.toml
--rw-r--r--   0 jonathanchan   (501) staff       (20)      596 2023-02-28 22:10:48.539574 artfornormies-0.0.1/setup.cfg
+drwxr-xr-x   0 jonathanchan   (501) staff       (20)        0 2023-05-17 19:00:35.014294 artfornormies-0.0.2/
+-rw-r--r--   0 jonathanchan   (501) staff       (20)     1069 2023-02-28 21:49:20.000000 artfornormies-0.0.2/LICENSE
+-rw-r--r--   0 jonathanchan   (501) staff       (20)        0 2023-02-28 22:07:49.000000 artfornormies-0.0.2/MANIFEST.in
+-rw-r--r--   0 jonathanchan   (501) staff       (20)     1002 2023-05-17 19:00:35.014422 artfornormies-0.0.2/PKG-INFO
+-rw-r--r--   0 jonathanchan   (501) staff       (20)      493 2023-03-01 03:47:40.000000 artfornormies-0.0.2/README.md
+drwxr-xr-x   0 jonathanchan   (501) staff       (20)        0 2023-05-17 19:00:35.011711 artfornormies-0.0.2/artfornormies/
+-rw-r--r--   0 jonathanchan   (501) staff       (20)        0 2023-02-28 22:01:52.000000 artfornormies-0.0.2/artfornormies/__init__.py
+-rw-r--r--   0 jonathanchan   (501) staff       (20)    14260 2023-01-16 18:15:03.000000 artfornormies-0.0.2/artfornormies/functions.py
+drwxr-xr-x   0 jonathanchan   (501) staff       (20)        0 2023-05-17 19:00:35.014020 artfornormies-0.0.2/artfornormies.egg-info/
+-rw-r--r--   0 jonathanchan   (501) staff       (20)     1002 2023-05-17 19:00:34.000000 artfornormies-0.0.2/artfornormies.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanchan   (501) staff       (20)      291 2023-05-17 19:00:35.000000 artfornormies-0.0.2/artfornormies.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanchan   (501) staff       (20)        1 2023-05-17 19:00:35.000000 artfornormies-0.0.2/artfornormies.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanchan   (501) staff       (20)       15 2023-05-17 19:00:35.000000 artfornormies-0.0.2/artfornormies.egg-info/requires.txt
+-rw-r--r--   0 jonathanchan   (501) staff       (20)       14 2023-05-17 19:00:35.000000 artfornormies-0.0.2/artfornormies.egg-info/top_level.txt
+-rw-r--r--   0 jonathanchan   (501) staff       (20)      125 2023-05-17 18:30:30.000000 artfornormies-0.0.2/pyproject.toml
+-rw-r--r--   0 jonathanchan   (501) staff       (20)      631 2023-05-17 19:00:35.014968 artfornormies-0.0.2/setup.cfg
```

### Comparing `artfornormies-0.0.1/LICENSE` & `artfornormies-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `artfornormies-0.0.1/artfornormies/functions.py` & `artfornormies-0.0.2/artfornormies/functions.py`

 * *Files identical despite different names*

