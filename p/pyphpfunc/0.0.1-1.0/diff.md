# Comparing `tmp/pyphpfunc-0.0.1.tar.gz` & `tmp/pyphpfunc-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphpfunc-0.0.1.tar", last modified: Tue May 16 14:03:01 2023, max compression
+gzip compressed data, was "pyphpfunc-1.0.tar", last modified: Wed May 17 02:15:39 2023, max compression
```

## Comparing `pyphpfunc-0.0.1.tar` & `pyphpfunc-1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 14:03:01.425586 pyphpfunc-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-16 10:06:54.000000 pyphpfunc-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      327 2023-05-16 14:03:01.425586 pyphpfunc-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-05-16 10:03:04.000000 pyphpfunc-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 14:03:01.405579 pyphpfunc-0.0.1/pyphpfunc/
--rw-rw-rw-   0        0        0       23 2023-05-16 10:06:17.000000 pyphpfunc-0.0.1/pyphpfunc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:03:01.421575 pyphpfunc-0.0.1/pyphpfunc.egg-info/
--rw-rw-rw-   0        0        0      327 2023-05-16 14:03:01.000000 pyphpfunc-0.0.1/pyphpfunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-05-16 14:03:01.000000 pyphpfunc-0.0.1/pyphpfunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 14:03:01.000000 pyphpfunc-0.0.1/pyphpfunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 14:03:01.000000 pyphpfunc-0.0.1/pyphpfunc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 14:03:01.425586 pyphpfunc-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      474 2023-05-16 14:02:48.000000 pyphpfunc-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:15:39.306218 pyphpfunc-1.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-16 10:06:54.000000 pyphpfunc-1.0/LICENSE
+-rw-rw-rw-   0        0        0      325 2023-05-17 02:15:39.304720 pyphpfunc-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-05-16 10:03:04.000000 pyphpfunc-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 02:15:39.287653 pyphpfunc-1.0/pyphpfunc/
+-rw-rw-rw-   0        0        0       53 2023-05-17 02:07:17.000000 pyphpfunc-1.0/pyphpfunc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:15:39.302721 pyphpfunc-1.0/pyphpfunc.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-05-17 02:15:39.000000 pyphpfunc-1.0/pyphpfunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-05-17 02:15:39.000000 pyphpfunc-1.0/pyphpfunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 02:15:39.000000 pyphpfunc-1.0/pyphpfunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 02:15:39.000000 pyphpfunc-1.0/pyphpfunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 02:15:39.306218 pyphpfunc-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      472 2023-05-17 02:14:50.000000 pyphpfunc-1.0/setup.py
```

### Comparing `pyphpfunc-0.0.1/LICENSE` & `pyphpfunc-1.0/LICENSE`

 * *Files identical despite different names*

