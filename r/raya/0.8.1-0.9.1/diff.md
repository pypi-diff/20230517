# Comparing `tmp/raya-0.8.1.tar.gz` & `tmp/raya-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raya-0.8.1.tar", last modified: Sun Aug 28 05:56:09 2022, max compression
+gzip compressed data, was "raya-0.9.1.tar", last modified: Tue Sep 20 14:52:31 2022, max compression
```

## Comparing `raya-0.8.1.tar` & `raya-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ofir      (1000) ofir      (1000)        0 2022-08-28 05:56:09.535325 raya-0.8.1/
--rw-rw-r--   0 ofir      (1000) ofir      (1000)     1069 2022-08-02 15:33:11.000000 raya-0.8.1/LICENSE
--rw-rw-r--   0 ofir      (1000) ofir      (1000)       35 2022-08-02 15:31:45.000000 raya-0.8.1/MANIFEST.in
--rw-rw-r--   0 ofir      (1000) ofir      (1000)      401 2022-08-28 05:56:09.539325 raya-0.8.1/PKG-INFO
--rw-rw-r--   0 ofir      (1000) ofir      (1000)      145 2022-08-28 05:55:25.000000 raya-0.8.1/README.md
-drwxrwxr-x   0 ofir      (1000) ofir      (1000)        0 2022-08-28 05:56:09.535325 raya-0.8.1/raya.egg-info/
--rw-rw-r--   0 ofir      (1000) ofir      (1000)      401 2022-08-28 05:56:09.000000 raya-0.8.1/raya.egg-info/PKG-INFO
--rw-rw-r--   0 ofir      (1000) ofir      (1000)      187 2022-08-28 05:56:09.000000 raya-0.8.1/raya.egg-info/SOURCES.txt
--rw-rw-r--   0 ofir      (1000) ofir      (1000)        1 2022-08-28 05:56:09.000000 raya-0.8.1/raya.egg-info/dependency_links.txt
--rw-rw-r--   0 ofir      (1000) ofir      (1000)        8 2022-08-28 05:56:09.000000 raya-0.8.1/raya.egg-info/requires.txt
--rw-rw-r--   0 ofir      (1000) ofir      (1000)        1 2022-08-28 05:56:09.000000 raya-0.8.1/raya.egg-info/top_level.txt
--rw-rw-r--   0 ofir      (1000) ofir      (1000)       38 2022-08-28 05:56:09.539325 raya-0.8.1/setup.cfg
--rw-rw-r--   0 ofir      (1000) ofir      (1000)      469 2022-08-28 05:55:33.000000 raya-0.8.1/setup.py
+drwxrwxr-x   0 ofir      (1000) ofir      (1000)        0 2022-09-20 14:52:31.484438 raya-0.9.1/
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)     1069 2022-08-02 15:33:11.000000 raya-0.9.1/LICENSE
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)       35 2022-08-02 15:31:45.000000 raya-0.9.1/MANIFEST.in
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)      401 2022-09-20 14:52:31.484438 raya-0.9.1/PKG-INFO
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)      145 2022-08-28 05:55:25.000000 raya-0.9.1/README.md
+drwxrwxr-x   0 ofir      (1000) ofir      (1000)        0 2022-09-20 14:52:31.484438 raya-0.9.1/raya.egg-info/
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)      401 2022-09-20 14:52:31.000000 raya-0.9.1/raya.egg-info/PKG-INFO
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)      187 2022-09-20 14:52:31.000000 raya-0.9.1/raya.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)        1 2022-09-20 14:52:31.000000 raya-0.9.1/raya.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)        8 2022-09-20 14:52:31.000000 raya-0.9.1/raya.egg-info/requires.txt
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)        1 2022-09-20 14:52:31.000000 raya-0.9.1/raya.egg-info/top_level.txt
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)       38 2022-09-20 14:52:31.484438 raya-0.9.1/setup.cfg
+-rw-rw-r--   0 ofir      (1000) ofir      (1000)      469 2022-09-20 14:52:26.000000 raya-0.9.1/setup.py
```

### Comparing `raya-0.8.1/LICENSE` & `raya-0.9.1/LICENSE`

 * *Files identical despite different names*

