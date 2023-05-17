# Comparing `tmp/img-prediction-0.0.5.tar.gz` & `tmp/img-prediction-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img-prediction-0.0.5.tar", last modified: Wed May 17 11:58:41 2023, max compression
+gzip compressed data, was "img-prediction-0.0.6.tar", last modified: Wed May 17 12:13:53 2023, max compression
```

## Comparing `img-prediction-0.0.5.tar` & `img-prediction-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lzw        (501) staff       (20)        0 2023-05-17 11:58:41.671103 img-prediction-0.0.5/
--rw-r--r--   0 lzw        (501) staff       (20)     1065 2023-05-17 02:01:39.000000 img-prediction-0.0.5/LICENSE
--rw-r--r--   0 lzw        (501) staff       (20)     1966 2023-05-17 11:58:41.670625 img-prediction-0.0.5/PKG-INFO
--rw-r--r--   0 lzw        (501) staff       (20)     1360 2023-05-17 11:57:15.000000 img-prediction-0.0.5/README.md
-drwxr-xr-x   0 lzw        (501) staff       (20)        0 2023-05-17 11:58:41.670218 img-prediction-0.0.5/img_prediction.egg-info/
--rw-r--r--   0 lzw        (501) staff       (20)     1966 2023-05-17 11:58:41.000000 img-prediction-0.0.5/img_prediction.egg-info/PKG-INFO
--rw-r--r--   0 lzw        (501) staff       (20)      270 2023-05-17 11:58:41.000000 img-prediction-0.0.5/img_prediction.egg-info/SOURCES.txt
--rw-r--r--   0 lzw        (501) staff       (20)        1 2023-05-17 11:58:41.000000 img-prediction-0.0.5/img_prediction.egg-info/dependency_links.txt
--rw-r--r--   0 lzw        (501) staff       (20)       44 2023-05-17 11:58:41.000000 img-prediction-0.0.5/img_prediction.egg-info/entry_points.txt
--rw-r--r--   0 lzw        (501) staff       (20)       47 2023-05-17 11:58:41.000000 img-prediction-0.0.5/img_prediction.egg-info/requires.txt
--rw-r--r--   0 lzw        (501) staff       (20)       11 2023-05-17 11:58:41.000000 img-prediction-0.0.5/img_prediction.egg-info/top_level.txt
--rw-r--r--   0 lzw        (501) staff       (20)     4246 2023-05-17 11:55:36.000000 img-prediction-0.0.5/prediction.py
--rw-r--r--   0 lzw        (501) staff       (20)       38 2023-05-17 11:58:41.671228 img-prediction-0.0.5/setup.cfg
--rw-r--r--   0 lzw        (501) staff       (20)     1126 2023-05-17 11:57:59.000000 img-prediction-0.0.5/setup.py
+drwxr-xr-x   0 lzw        (501) staff       (20)        0 2023-05-17 12:13:53.727218 img-prediction-0.0.6/
+-rw-r--r--   0 lzw        (501) staff       (20)     1065 2023-05-17 02:01:39.000000 img-prediction-0.0.6/LICENSE
+-rw-r--r--   0 lzw        (501) staff       (20)     1966 2023-05-17 12:13:53.726939 img-prediction-0.0.6/PKG-INFO
+-rw-r--r--   0 lzw        (501) staff       (20)     1360 2023-05-17 11:57:15.000000 img-prediction-0.0.6/README.md
+drwxr-xr-x   0 lzw        (501) staff       (20)        0 2023-05-17 12:13:53.726533 img-prediction-0.0.6/img_prediction.egg-info/
+-rw-r--r--   0 lzw        (501) staff       (20)     1966 2023-05-17 12:13:53.000000 img-prediction-0.0.6/img_prediction.egg-info/PKG-INFO
+-rw-r--r--   0 lzw        (501) staff       (20)      270 2023-05-17 12:13:53.000000 img-prediction-0.0.6/img_prediction.egg-info/SOURCES.txt
+-rw-r--r--   0 lzw        (501) staff       (20)        1 2023-05-17 12:13:53.000000 img-prediction-0.0.6/img_prediction.egg-info/dependency_links.txt
+-rw-r--r--   0 lzw        (501) staff       (20)       44 2023-05-17 12:13:53.000000 img-prediction-0.0.6/img_prediction.egg-info/entry_points.txt
+-rw-r--r--   0 lzw        (501) staff       (20)       63 2023-05-17 12:13:53.000000 img-prediction-0.0.6/img_prediction.egg-info/requires.txt
+-rw-r--r--   0 lzw        (501) staff       (20)       11 2023-05-17 12:13:53.000000 img-prediction-0.0.6/img_prediction.egg-info/top_level.txt
+-rw-r--r--   0 lzw        (501) staff       (20)     4246 2023-05-17 11:55:36.000000 img-prediction-0.0.6/prediction.py
+-rw-r--r--   0 lzw        (501) staff       (20)       38 2023-05-17 12:13:53.727298 img-prediction-0.0.6/setup.cfg
+-rw-r--r--   0 lzw        (501) staff       (20)     1126 2023-05-17 12:13:25.000000 img-prediction-0.0.6/setup.py
```

### Comparing `img-prediction-0.0.5/LICENSE` & `img-prediction-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `img-prediction-0.0.5/PKG-INFO` & `img-prediction-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img-prediction
-Version: 0.0.5
+Version: 0.0.6
 Summary: Predict the location of the instance in the picture and Mosaic it
 Author: LiuZhiwei
 Author-email: 1129459766@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `img-prediction-0.0.5/README.md` & `img-prediction-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `img-prediction-0.0.5/img_prediction.egg-info/PKG-INFO` & `img-prediction-0.0.6/img_prediction.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img-prediction
-Version: 0.0.5
+Version: 0.0.6
 Summary: Predict the location of the instance in the picture and Mosaic it
 Author: LiuZhiwei
 Author-email: 1129459766@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `img-prediction-0.0.5/prediction.py` & `img-prediction-0.0.6/prediction.py`

 * *Files identical despite different names*

### Comparing `img-prediction-0.0.5/setup.py` & `img-prediction-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     a.strip()
     for a in read('requirements.txt').splitlines()
     if a.strip() and not a.startswith(('#', '-'))
 ]
 
 setup(
     name='img-prediction',
-    version='0.0.5',
+    version='0.0.6',
     description='Predict the location of the instance in the picture and Mosaic it',
     author='LiuZhiwei',
     author_email='1129459766@qq.com',
     license='MIT',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

