# Comparing `tmp/botxbingxuser-0.0.1.tar.gz` & `tmp/botxbingxuser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botxbingxuser-0.0.1.tar", last modified: Tue May 16 01:55:24 2023, max compression
+gzip compressed data, was "botxbingxuser-0.0.2.tar", last modified: Wed May 17 01:36:55 2023, max compression
```

## Comparing `botxbingxuser-0.0.1.tar` & `botxbingxuser-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 01:55:24.897079 botxbingxuser-0.0.1/
--rw-rw-rw-   0        0        0      566 2023-05-16 01:55:24.896076 botxbingxuser-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 01:55:24.890121 botxbingxuser-0.0.1/botxbingxuser.egg-info/
--rw-rw-rw-   0        0        0      566 2023-05-16 01:55:24.000000 botxbingxuser-0.0.1/botxbingxuser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-16 01:55:24.000000 botxbingxuser-0.0.1/botxbingxuser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 01:55:24.000000 botxbingxuser-0.0.1/botxbingxuser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-16 01:55:24.000000 botxbingxuser-0.0.1/botxbingxuser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 01:55:24.894076 botxbingxuser-0.0.1/botxbinxuser/
--rw-rw-rw-   0        0        0     6543 2023-05-16 01:23:08.000000 botxbingxuser-0.0.1/botxbinxuser/PrincipalMetodos.py
--rw-rw-rw-   0        0        0        0 2023-05-16 01:23:25.000000 botxbingxuser-0.0.1/botxbinxuser/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-16 01:55:24.897079 botxbingxuser-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1093 2023-05-16 01:55:07.000000 botxbingxuser-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 01:36:55.607119 botxbingxuser-0.0.2/
+-rw-rw-rw-   0        0        0      566 2023-05-17 01:36:55.606119 botxbingxuser-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 01:36:55.600102 botxbingxuser-0.0.2/botxbingxuser.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-05-17 01:36:55.000000 botxbingxuser-0.0.2/botxbingxuser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-17 01:36:55.000000 botxbingxuser-0.0.2/botxbingxuser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 01:36:55.000000 botxbingxuser-0.0.2/botxbingxuser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 01:36:55.000000 botxbingxuser-0.0.2/botxbingxuser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 01:36:55.604117 botxbingxuser-0.0.2/botxbinxuser/
+-rw-rw-rw-   0        0        0     4966 2023-05-17 01:36:05.000000 botxbingxuser-0.0.2/botxbinxuser/PrincipalMetodos.py
+-rw-rw-rw-   0        0        0        0 2023-05-16 01:23:25.000000 botxbingxuser-0.0.2/botxbinxuser/__init__.py
+-rw-rw-rw-   0        0        0      465 2023-05-17 01:33:16.000000 botxbingxuser-0.0.2/botxbinxuser/user.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 01:36:55.607119 botxbingxuser-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2023-05-17 01:34:24.000000 botxbingxuser-0.0.2/setup.py
```

### Comparing `botxbingxuser-0.0.1/PKG-INFO` & `botxbingxuser-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botxbingxuser
-Version: 0.0.1
+Version: 0.0.2
 Summary: API de acesso a Xbinx
 Author: Thiago Ventura
 Author-email: <tigoluthi@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `botxbingxuser-0.0.1/botxbingxuser.egg-info/PKG-INFO` & `botxbingxuser-0.0.2/botxbingxuser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botxbingxuser
-Version: 0.0.1
+Version: 0.0.2
 Summary: API de acesso a Xbinx
 Author: Thiago Ventura
 Author-email: <tigoluthi@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `botxbingxuser-0.0.1/setup.py` & `botxbingxuser-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'API de acesso a Xbinx'
 LONG_DESCRIPTION = """ API de acesso a corretora XBINGX
                         Para automatizar os traders"""
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
```

