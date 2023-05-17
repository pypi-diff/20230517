# Comparing `tmp/criptoMark-0.0.4.tar.gz` & `tmp/criptoMark-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criptoMark-0.0.4.tar", last modified: Tue May 16 00:09:51 2023, max compression
+gzip compressed data, was "criptoMark-0.0.5.tar", last modified: Wed May 17 00:29:44 2023, max compression
```

## Comparing `criptoMark-0.0.4.tar` & `criptoMark-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 00:09:51.505587 criptoMark-0.0.4/
--rw-rw-rw-   0        0        0      504 2023-05-16 00:09:51.504747 criptoMark-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 00:09:51.490575 criptoMark-0.0.4/criptoMark/
--rw-rw-rw-   0        0        0        0 2023-05-16 00:05:35.000000 criptoMark-0.0.4/criptoMark/__init__.py
--rw-rw-rw-   0        0        0     6990 2023-05-16 00:05:52.000000 criptoMark-0.0.4/criptoMark/requisicaocripto.py
-drwxrwxrwx   0        0        0        0 2023-05-16 00:09:51.500586 criptoMark-0.0.4/criptoMark.egg-info/
--rw-rw-rw-   0        0        0      504 2023-05-16 00:09:51.000000 criptoMark-0.0.4/criptoMark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-05-16 00:09:51.000000 criptoMark-0.0.4/criptoMark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 00:09:51.000000 criptoMark-0.0.4/criptoMark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 00:09:51.000000 criptoMark-0.0.4/criptoMark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 00:09:51.505587 criptoMark-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-05-16 00:09:43.000000 criptoMark-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:29:44.883817 criptoMark-0.0.5/
+-rw-rw-rw-   0        0        0      504 2023-05-17 00:29:44.883817 criptoMark-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 00:29:44.857743 criptoMark-0.0.5/criptoMark/
+-rw-rw-rw-   0        0        0        0 2023-05-16 00:05:35.000000 criptoMark-0.0.5/criptoMark/__init__.py
+-rw-rw-rw-   0        0        0     8559 2023-05-16 19:07:10.000000 criptoMark-0.0.5/criptoMark/binance_symbols.py
+-rw-rw-rw-   0        0        0     8631 2023-05-17 00:26:23.000000 criptoMark-0.0.5/criptoMark/requisicaocripto.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:29:44.881812 criptoMark-0.0.5/criptoMark.egg-info/
+-rw-rw-rw-   0        0        0      504 2023-05-17 00:29:44.000000 criptoMark-0.0.5/criptoMark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-05-17 00:29:44.000000 criptoMark-0.0.5/criptoMark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 00:29:44.000000 criptoMark-0.0.5/criptoMark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-17 00:29:44.000000 criptoMark-0.0.5/criptoMark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 00:29:44.883817 criptoMark-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-05-17 00:29:33.000000 criptoMark-0.0.5/setup.py
```

### Comparing `criptoMark-0.0.4/setup.py` & `criptoMark-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'Pacote de consultas'
 LONG_DESCRIPTION = 'Pacote de Consultas de cripto'
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
         name="criptoMark",
```

