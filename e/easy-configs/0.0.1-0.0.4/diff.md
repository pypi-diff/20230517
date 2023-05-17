# Comparing `tmp/easy-configs-0.0.1.tar.gz` & `tmp/easy-configs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-configs-0.0.1.tar", last modified: Wed May 17 10:39:45 2023, max compression
+gzip compressed data, was "easy-configs-0.0.4.tar", last modified: Wed May 17 14:38:55 2023, max compression
```

## Comparing `easy-configs-0.0.1.tar` & `easy-configs-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 10:39:45.073018 easy-configs-0.0.1/
--rw-rw-rw-   0        0        0      603 2023-05-17 10:39:45.072437 easy-configs-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 10:39:45.055961 easy-configs-0.0.1/configs/
--rw-rw-rw-   0        0        0       19 2023-05-17 10:19:48.000000 easy-configs-0.0.1/configs/__init__.py
--rw-rw-rw-   0        0        0     7408 2023-05-17 10:19:35.000000 easy-configs-0.0.1/configs/main.py
-drwxrwxrwx   0        0        0        0 2023-05-17 10:39:45.070438 easy-configs-0.0.1/easy_configs.egg-info/
--rw-rw-rw-   0        0        0      603 2023-05-17 10:39:44.000000 easy-configs-0.0.1/easy_configs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-05-17 10:39:44.000000 easy-configs-0.0.1/easy_configs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 10:39:44.000000 easy-configs-0.0.1/easy_configs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 10:39:44.000000 easy-configs-0.0.1/easy_configs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 10:39:45.073931 easy-configs-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-05-17 10:39:40.000000 easy-configs-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:38:55.905130 easy-configs-0.0.4/
+-rw-rw-rw-   0        0        0      603 2023-05-17 14:38:55.905130 easy-configs-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 14:38:55.882547 easy-configs-0.0.4/configs/
+-rw-rw-rw-   0        0        0       19 2023-05-17 10:19:48.000000 easy-configs-0.0.4/configs/__init__.py
+-rw-rw-rw-   0        0        0     7412 2023-05-17 14:36:44.000000 easy-configs-0.0.4/configs/main.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:38:55.903688 easy-configs-0.0.4/easy_configs.egg-info/
+-rw-rw-rw-   0        0        0      603 2023-05-17 14:38:55.000000 easy-configs-0.0.4/easy_configs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-05-17 14:38:55.000000 easy-configs-0.0.4/easy_configs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:38:55.000000 easy-configs-0.0.4/easy_configs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 14:38:55.000000 easy-configs-0.0.4/easy_configs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 14:38:55.906293 easy-configs-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-05-17 14:38:50.000000 easy-configs-0.0.4/setup.py
```

### Comparing `easy-configs-0.0.1/PKG-INFO` & `easy-configs-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-configs
-Version: 0.0.1
+Version: 0.0.4
 Summary: A python package to make configs easier!
 Home-page: UNKNOWN
 Author: tntgamer685347
 Author-email: gamer@fampl.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `easy-configs-0.0.1/configs/main.py` & `easy-configs-0.0.4/configs/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,16 +179,16 @@
             f.write(f'<{name}>{values[i]}</{name}>\n')
             written.append(f'<{name}>{values[i]}</{name}>\n')
         
         return written
 
     def create_basic(filename):
         f = open(filename, 'w')
-        f.write('<Version>1.0</Version>')
-        return '<Version>1.0</Version>'
+        f.write('<Version>1.0</Version>\n')
+        return '<Version>1.0</Version>\n'
 
 if __name__ == '__main__':
     file = open('config.config', 'w+') # open config file.
     config = Reader.load(f=file) # one way is the load function it uses an file object and then reads the config from there.
     print(config)
     # or:
     # text = file.read()
```

### Comparing `easy-configs-0.0.1/easy_configs.egg-info/PKG-INFO` & `easy-configs-0.0.4/easy_configs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-configs
-Version: 0.0.1
+Version: 0.0.4
 Summary: A python package to make configs easier!
 Home-page: UNKNOWN
 Author: tntgamer685347
 Author-email: gamer@fampl.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `easy-configs-0.0.1/setup.py` & `easy-configs-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.1'
+VERSION = '0.0.4'
 DESCRIPTION = 'A python package to make configs easier!'
 LONG_DESCRIPTION = 'A package that allows to read and write to configs.'
 
 setup(
     name="easy-configs",
     version=VERSION,
     author="tntgamer685347",
```

