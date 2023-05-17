# Comparing `tmp/pdtr-0.1.0.tar.gz` & `tmp/pdtr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdtr-0.1.0.tar", last modified: Wed May 17 14:12:50 2023, max compression
+gzip compressed data, was "pdtr-0.1.1.tar", last modified: Wed May 17 16:05:19 2023, max compression
```

## Comparing `pdtr-0.1.0.tar` & `pdtr-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-17 14:12:50.940846 pdtr-0.1.0/
--rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-12 08:26:44.000000 pdtr-0.1.0/LICENSE
--rw-r--r--   0 lubberit   (501) staff       (20)     8474 2023-05-17 14:12:50.940123 pdtr-0.1.0/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)     7748 2023-05-17 14:11:24.000000 pdtr-0.1.0/README.md
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-17 14:12:50.936676 pdtr-0.1.0/pdtr/
--rw-r--r--   0 lubberit   (501) staff       (20)      265 2023-05-17 13:55:01.000000 pdtr-0.1.0/pdtr/__init__.py
--rw-r--r--   0 lubberit   (501) staff       (20)    21376 2023-05-12 10:15:12.000000 pdtr-0.1.0/pdtr/excel_writer.py
--rw-r--r--   0 lubberit   (501) staff       (20)    14658 2023-05-17 13:54:39.000000 pdtr-0.1.0/pdtr/transforme.py
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-17 14:12:50.939399 pdtr-0.1.0/pdtr.egg-info/
--rw-r--r--   0 lubberit   (501) staff       (20)     8474 2023-05-17 14:12:50.000000 pdtr-0.1.0/pdtr.egg-info/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)      222 2023-05-17 14:12:50.000000 pdtr-0.1.0/pdtr.egg-info/SOURCES.txt
--rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-17 14:12:50.000000 pdtr-0.1.0/pdtr.egg-info/dependency_links.txt
--rw-r--r--   0 lubberit   (501) staff       (20)      168 2023-05-17 14:12:50.000000 pdtr-0.1.0/pdtr.egg-info/requires.txt
--rw-r--r--   0 lubberit   (501) staff       (20)        5 2023-05-17 14:12:50.000000 pdtr-0.1.0/pdtr.egg-info/top_level.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-17 14:12:50.940941 pdtr-0.1.0/setup.cfg
--rw-r--r--   0 lubberit   (501) staff       (20)     1632 2023-05-17 13:54:53.000000 pdtr-0.1.0/setup.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-17 16:05:19.927967 pdtr-0.1.1/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-12 08:26:44.000000 pdtr-0.1.1/LICENSE
+-rw-r--r--   0 lubberit   (501) staff       (20)     8477 2023-05-17 16:05:19.927685 pdtr-0.1.1/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)     7751 2023-05-17 14:15:07.000000 pdtr-0.1.1/README.md
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-17 16:05:19.925673 pdtr-0.1.1/pdtr/
+-rw-r--r--   0 lubberit   (501) staff       (20)      265 2023-05-17 16:05:07.000000 pdtr-0.1.1/pdtr/__init__.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    21376 2023-05-17 15:26:47.000000 pdtr-0.1.1/pdtr/excel_writer.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    25148 2023-05-17 15:58:18.000000 pdtr-0.1.1/pdtr/transforme.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-17 16:05:19.927294 pdtr-0.1.1/pdtr.egg-info/
+-rw-r--r--   0 lubberit   (501) staff       (20)     8477 2023-05-17 16:05:19.000000 pdtr-0.1.1/pdtr.egg-info/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)      222 2023-05-17 16:05:19.000000 pdtr-0.1.1/pdtr.egg-info/SOURCES.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-17 16:05:19.000000 pdtr-0.1.1/pdtr.egg-info/dependency_links.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)      199 2023-05-17 16:05:19.000000 pdtr-0.1.1/pdtr.egg-info/requires.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        5 2023-05-17 16:05:19.000000 pdtr-0.1.1/pdtr.egg-info/top_level.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-17 16:05:19.928071 pdtr-0.1.1/setup.cfg
+-rw-r--r--   0 lubberit   (501) staff       (20)     1632 2023-05-17 16:04:40.000000 pdtr-0.1.1/setup.py
```

### Comparing `pdtr-0.1.0/LICENSE` & `pdtr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdtr-0.1.0/PKG-INFO` & `pdtr-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdtr
-Version: 0.1.0
+Version: 0.1.1
 Summary: 自动决策树规则挖掘工具包
 Home-page: https://github.com/itlubber/pdtr
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -215,8 +215,9 @@
 
 `examples/决策树组合策略挖掘.xlsx`
 
 
 ## 参考
 
 > https://github.com/itlubber/LogisticRegressionPipeline
+> 
 > https://github.com/itlubber/itlubber-excel-writer
```

### Comparing `pdtr-0.1.0/README.md` & `pdtr-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,9 @@
 
 `examples/决策树组合策略挖掘.xlsx`
 
 
 ## 参考
 
 > https://github.com/itlubber/LogisticRegressionPipeline
+> 
 > https://github.com/itlubber/itlubber-excel-writer
```

### Comparing `pdtr-0.1.0/pdtr/excel_writer.py` & `pdtr-0.1.1/pdtr/excel_writer.py`

 * *Files identical despite different names*

### Comparing `pdtr-0.1.0/pdtr.egg-info/PKG-INFO` & `pdtr-0.1.1/pdtr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdtr
-Version: 0.1.0
+Version: 0.1.1
 Summary: 自动决策树规则挖掘工具包
 Home-page: https://github.com/itlubber/pdtr
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -215,8 +215,9 @@
 
 `examples/决策树组合策略挖掘.xlsx`
 
 
 ## 参考
 
 > https://github.com/itlubber/LogisticRegressionPipeline
+> 
 > https://github.com/itlubber/itlubber-excel-writer
```

### Comparing `pdtr-0.1.0/setup.py` & `pdtr-0.1.1/setup.py`

 * *Files identical despite different names*

