# Comparing `tmp/python-eigen-ingenuity-0.4.7.tar.gz` & `tmp/python-eigen-ingenuity-0.4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-eigen-ingenuity-0.4.7.tar", last modified: Wed May 17 14:55:30 2023, max compression
+gzip compressed data, was "python-eigen-ingenuity-0.4.7.1.tar", last modified: Wed May 17 14:56:58 2023, max compression
```

## Comparing `python-eigen-ingenuity-0.4.7.tar` & `python-eigen-ingenuity-0.4.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:55:30.907409 python-eigen-ingenuity-0.4.7/
--rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7/LICENSE
--rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.7/MANIFEST.in
--rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-05-17 14:55:30.907205 python-eigen-ingenuity-0.4.7/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7/README.md
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:55:30.905934 python-eigen-ingenuity-0.4.7/eigeningenuity/
--rw-r--r--   0 berhic     (501) staff       (20)     1203 2023-04-06 15:03:48.000000 python-eigen-ingenuity-0.4.7/eigeningenuity/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)    15882 2023-05-17 13:44:01.000000 python-eigen-ingenuity-0.4.7/eigeningenuity/assetmodel.py
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:55:30.906261 python-eigen-ingenuity-0.4.7/eigeningenuity/core/
--rw-r--r--   0 berhic     (501) staff       (20)     7715 2023-04-06 10:18:46.000000 python-eigen-ingenuity-0.4.7/eigeningenuity/core/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7/eigeningenuity/core/debug.py
--rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.7/eigeningenuity/elastic.py
--rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.7/eigeningenuity/events.py
--rw-r--r--   0 berhic     (501) staff       (20)    36199 2023-05-17 13:47:31.000000 python-eigen-ingenuity-0.4.7/eigeningenuity/historian.py
--rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.7/eigeningenuity/smartdash.py
--rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.7/eigeningenuity/sql.py
--rw-r--r--   0 berhic     (501) staff       (20)    11846 2023-05-17 14:22:19.000000 python-eigen-ingenuity-0.4.7/eigeningenuity/util.py
--rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7/pyproject.toml
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:55:30.906998 python-eigen-ingenuity-0.4.7/python_eigen_ingenuity.egg-info/
--rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-05-17 14:55:30.000000 python-eigen-ingenuity-0.4.7/python_eigen_ingenuity.egg-info/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)      551 2023-05-17 14:55:30.000000 python-eigen-ingenuity-0.4.7/python_eigen_ingenuity.egg-info/SOURCES.txt
--rw-r--r--   0 berhic     (501) staff       (20)        1 2023-05-17 14:55:30.000000 python-eigen-ingenuity-0.4.7/python_eigen_ingenuity.egg-info/dependency_links.txt
--rw-r--r--   0 berhic     (501) staff       (20)       24 2023-05-17 14:55:30.000000 python-eigen-ingenuity-0.4.7/python_eigen_ingenuity.egg-info/requires.txt
--rw-r--r--   0 berhic     (501) staff       (20)       15 2023-05-17 14:55:30.000000 python-eigen-ingenuity-0.4.7/python_eigen_ingenuity.egg-info/top_level.txt
--rw-r--r--   0 berhic     (501) staff       (20)       38 2023-05-17 14:55:30.907456 python-eigen-ingenuity-0.4.7/setup.cfg
--rw-r--r--   0 berhic     (501) staff       (20)      689 2023-05-17 14:55:00.000000 python-eigen-ingenuity-0.4.7/setup.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:56:58.463388 python-eigen-ingenuity-0.4.7.1/
+-rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.1/LICENSE
+-rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.7.1/MANIFEST.in
+-rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-05-17 14:56:58.463167 python-eigen-ingenuity-0.4.7.1/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.1/README.md
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:56:58.461864 python-eigen-ingenuity-0.4.7.1/eigeningenuity/
+-rw-r--r--   0 berhic     (501) staff       (20)     1203 2023-04-06 15:03:48.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)    15882 2023-05-17 13:44:01.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/assetmodel.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:56:58.462176 python-eigen-ingenuity-0.4.7.1/eigeningenuity/core/
+-rw-r--r--   0 berhic     (501) staff       (20)     7715 2023-04-06 10:18:46.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/core/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/core/debug.py
+-rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/elastic.py
+-rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/events.py
+-rw-r--r--   0 berhic     (501) staff       (20)    36199 2023-05-17 13:47:31.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/historian.py
+-rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/smartdash.py
+-rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/sql.py
+-rw-r--r--   0 berhic     (501) staff       (20)    11952 2023-05-17 14:56:30.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/util.py
+-rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.1/pyproject.toml
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:56:58.462955 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/
+-rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-05-17 14:56:58.000000 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)      551 2023-05-17 14:56:58.000000 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/SOURCES.txt
+-rw-r--r--   0 berhic     (501) staff       (20)        1 2023-05-17 14:56:58.000000 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/dependency_links.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       24 2023-05-17 14:56:58.000000 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/requires.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       15 2023-05-17 14:56:58.000000 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/top_level.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       38 2023-05-17 14:56:58.463441 python-eigen-ingenuity-0.4.7.1/setup.cfg
+-rw-r--r--   0 berhic     (501) staff       (20)      691 2023-05-17 14:56:45.000000 python-eigen-ingenuity-0.4.7.1/setup.py
```

### Comparing `python-eigen-ingenuity-0.4.7/LICENSE` & `python-eigen-ingenuity-0.4.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/PKG-INFO` & `python-eigen-ingenuity-0.4.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.7
+Version: 0.4.7.1
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.7/README.md` & `python-eigen-ingenuity-0.4.7.1/README.md`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/eigeningenuity/__init__.py` & `python-eigen-ingenuity-0.4.7.1/eigeningenuity/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/eigeningenuity/assetmodel.py` & `python-eigen-ingenuity-0.4.7.1/eigeningenuity/assetmodel.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/eigeningenuity/core/__init__.py` & `python-eigen-ingenuity-0.4.7.1/eigeningenuity/core/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/eigeningenuity/core/debug.py` & `python-eigen-ingenuity-0.4.7.1/eigeningenuity/core/debug.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/eigeningenuity/elastic.py` & `python-eigen-ingenuity-0.4.7.1/eigeningenuity/elastic.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/eigeningenuity/events.py` & `python-eigen-ingenuity-0.4.7.1/eigeningenuity/events.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/eigeningenuity/historian.py` & `python-eigen-ingenuity-0.4.7.1/eigeningenuity/historian.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/eigeningenuity/smartdash.py` & `python-eigen-ingenuity-0.4.7.1/eigeningenuity/smartdash.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/eigeningenuity/sql.py` & `python-eigen-ingenuity-0.4.7.1/eigeningenuity/sql.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/eigeningenuity/util.py` & `python-eigen-ingenuity-0.4.7.1/eigeningenuity/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,16 +283,20 @@
     return x[1]
 
 def aggToDf(x):
     y = flattenList(list(map(aggMap,x.items())))
     cols = ["tag", "start", "end", "min", "max", "avg", "var", "stddev", "numgood", "numbad"]
     df = pd.DataFrame(y)
     df = df[cols]
-    df["start"] = pd.to_datetime(df["start"].apply(lambda s: s.split("+")[0]), unit="ms")
-    df["end"] = pd.to_datetime(df["end"].apply(lambda s: s.split("+")[0]), unit="ms")
+    try:
+        df["start"] = pd.to_datetime(df["start"], unit="ms")
+        df["end"] = pd.to_datetime(df["end"], unit="ms")
+    except ValueError:
+        df["start"] = pd.to_datetime(df["start"], format="ISO8601")
+        df["end"] = pd.to_datetime(df["end"], format="ISO8601")
     df.sort_values(by='start', inplace=True)
     return(df)
 
 def get_eigenserver(url):
     split_url = urlsplit(url)
     return split_url.scheme + "://" + split_url.netloc
```

### Comparing `python-eigen-ingenuity-0.4.7/python_eigen_ingenuity.egg-info/PKG-INFO` & `python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.7
+Version: 0.4.7.1
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.7/python_eigen_ingenuity.egg-info/SOURCES.txt` & `python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7/setup.py` & `python-eigen-ingenuity-0.4.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README = (HERE / "README.md").read_text()
 
 pkgname = 'python-eigen-ingenuity'
 
 # Invoke setup
 setup(
     name=pkgname,
-    version='0.4.7',
+    version='0.4.7.1',
     author='Murray Callander',
     author_email='info@eigen.co',
     url='https://www.eigen.co/',
     description="A python library used to query data from the Eigen Ingenuity system",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages("."),
```

