# Comparing `tmp/clickzetta-sqlalchemy-0.6.6.tar.gz` & `tmp/clickzetta-sqlalchemy-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-sqlalchemy-0.6.6.tar", last modified: Tue May 16 13:55:00 2023, max compression
+gzip compressed data, was "clickzetta-sqlalchemy-0.6.7.tar", last modified: Wed May 17 03:05:00 2023, max compression
```

## Comparing `clickzetta-sqlalchemy-0.6.6.tar` & `clickzetta-sqlalchemy-0.6.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-16 13:55:00.333506 clickzetta-sqlalchemy-0.6.6/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      423 2023-05-16 13:55:00.333386 clickzetta-sqlalchemy-0.6.6/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-16 13:55:00.331759 clickzetta-sqlalchemy-0.6.6/clickzetta_sqlalchemy.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      423 2023-05-16 13:55:00.000000 clickzetta-sqlalchemy-0.6.6/clickzetta_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)      560 2023-05-16 13:55:00.000000 clickzetta-sqlalchemy-0.6.6/clickzetta_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-16 13:55:00.000000 clickzetta-sqlalchemy-0.6.6/clickzetta_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-16 13:55:00.000000 clickzetta-sqlalchemy-0.6.6/clickzetta_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-16 13:55:00.000000 clickzetta-sqlalchemy-0.6.6/clickzetta_sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      633 2023-05-16 13:55:00.000000 clickzetta-sqlalchemy-0.6.6/clickzetta_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       22 2023-05-16 13:55:00.000000 clickzetta-sqlalchemy-0.6.6/clickzetta_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-16 13:55:00.333546 clickzetta-sqlalchemy-0.6.6/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1868 2023-05-16 13:54:03.000000 clickzetta-sqlalchemy-0.6.6/setup.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-16 13:55:00.333233 clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      499 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1079 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/_helpers.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1626 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/_types.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    20343 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/base.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1146 2023-02-24 06:29:49.000000 clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/parse_url.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2742 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/requirements.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-16 13:54:03.000000 clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/version.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-17 03:05:00.795879 clickzetta-sqlalchemy-0.6.7/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      423 2023-05-17 03:05:00.795707 clickzetta-sqlalchemy-0.6.7/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-17 03:05:00.793652 clickzetta-sqlalchemy-0.6.7/clickzetta_sqlalchemy.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      423 2023-05-17 03:05:00.000000 clickzetta-sqlalchemy-0.6.7/clickzetta_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      560 2023-05-17 03:05:00.000000 clickzetta-sqlalchemy-0.6.7/clickzetta_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-17 03:05:00.000000 clickzetta-sqlalchemy-0.6.7/clickzetta_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-17 03:05:00.000000 clickzetta-sqlalchemy-0.6.7/clickzetta_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-17 03:05:00.000000 clickzetta-sqlalchemy-0.6.7/clickzetta_sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      633 2023-05-17 03:05:00.000000 clickzetta-sqlalchemy-0.6.7/clickzetta_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       22 2023-05-17 03:05:00.000000 clickzetta-sqlalchemy-0.6.7/clickzetta_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-17 03:05:00.796082 clickzetta-sqlalchemy-0.6.7/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1868 2023-05-17 03:04:04.000000 clickzetta-sqlalchemy-0.6.7/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-17 03:05:00.795503 clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      499 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1123 2023-05-17 01:41:53.000000 clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/_helpers.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1626 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/_types.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    20451 2023-05-17 01:54:46.000000 clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/base.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1226 2023-05-17 01:54:46.000000 clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/parse_url.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2742 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/requirements.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-17 03:04:04.000000 clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/version.py
```

### Comparing `clickzetta-sqlalchemy-0.6.6/clickzetta_sqlalchemy.egg-info/SOURCES.txt` & `clickzetta-sqlalchemy-0.6.7/clickzetta_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.6.6/clickzetta_sqlalchemy.egg-info/requires.txt` & `clickzetta-sqlalchemy-0.6.7/clickzetta_sqlalchemy.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 proto-plus<2.0.0dev,>=1.22.0
 packaging<24.0.0dev,>=14.3
 protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 python-dateutil<3.0dev,>=2.7.2
 requests<3.0.0dev,>=2.21.0
 sqlalchemy==2.0.6
 future
-clickzetta-connector==0.6.6
+clickzetta-connector==0.6.7
 
 [all]
 pandas>=1.0.0
 db-dtypes<2.0.0dev,>=0.3.0
 ipywidgets==7.7.1
 geopandas<1.0dev,>=0.9.0
 Shapely<2.0dev,>=1.6.0
```

### Comparing `clickzetta-sqlalchemy-0.6.6/setup.py` & `clickzetta-sqlalchemy-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "proto-plus >= 1.22.0, <2.0.0dev",
     "packaging >= 14.3, <24.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "python-dateutil >= 2.7.2, <3.0dev",
     "requests >= 2.21.0, < 3.0.0dev",
     "sqlalchemy==2.0.6",
     "future",
-    'clickzetta-connector==0.6.6',
+    'clickzetta-connector==0.6.7',
 ]
 extras = {
     "pandas": ["pandas>=1.0.0", "db-dtypes>=0.3.0,<2.0.0dev"],
     "ipywidgets": ["ipywidgets==7.7.1"],
     "geopandas": ["geopandas>=0.9.0, <1.0dev", "Shapely>=1.6.0, <2.0dev"],
     "ipython": ["ipython>=7.0.1,!=8.1.0"],
     "tqdm": ["tqdm >= 4.7.4, <5.0.0dev"],
```

### Comparing `clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/_helpers.py` & `clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 def create_clickzetta_client(
         username=None,
         password=None,
         instance_name=None,
         workspace=None,
         vc_name=None,
         base_url=None,
+        schema=None,
 
 ):
     login_params = LoginParams(username, password, instance_name)
     return Client(
         login_params=login_params,
         workspace=workspace,
         instance_name=instance_name,
         vc_name=vc_name,
         base_url=base_url,
+        schema=schema,
     )
 
 
 def substitute_re_method(r, flags=0, repl=None):
     if repl is None:
         return lambda f: substitute_re_method(r, flags, f)
```

### Comparing `clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/_types.py` & `clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/_types.py`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/base.py` & `clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,46 +513,50 @@
         self.host = None
         self.username = None
         self.driver_name = None
         self.pwd = None
         self.instance_name = None
         self.workspace = None
         self.vc_name = None
+        self.schema = None
 
     @classmethod
     def dbapi(cls):
         return dbapi
 
     def create_connect_args(self, url):
         (
             host,
             username,
             driver_name,
             pwd,
             instance_name,
             workspace,
             vc_name,
+            schema,
         ) = parse_url(url)
 
         self.host = host
         self.arraysize = self.arraysize
         self.username = username
         self.driver_name = driver_name
         self.pwd = pwd
         self.instance_name = instance_name
         self.workspace = workspace
         self.vc_name = vc_name
+        self.schema = schema
 
         client = _helpers.create_clickzetta_client(
             username=self.username,
             password=self.pwd,
             instance_name=self.instance_name,
             workspace=self.workspace,
             vc_name=self.vc_name,
             base_url=self.host,
+            schema=self.schema,
         )
         return ([], {"client": client})
 
     def do_rollback(self, dbapi_connection):
         pass
 
     def get_foreign_keys(self, connection, table_name, schema=None, **kw):
```

### Comparing `clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/parse_url.py` & `clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/parse_url.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,16 +32,20 @@
         if 'virtualcluster' in query:
             vc_name = query.pop('virtualcluster')
         elif 'virtualCluster' in query:
             vc_name = query.pop('virtualCluster')
     else:
         raise ValueError('url must have `virtualcluster` parameter.')
 
+    if 'schema' in query:
+        schema = query.pop('schema')
+
     return (
         host,
         username,
         driver_name,
         pwd,
         instance_name,
         workspace,
         vc_name,
+        schema,
     )
```

### Comparing `clickzetta-sqlalchemy-0.6.6/sqlalchemy_clickzetta/requirements.py` & `clickzetta-sqlalchemy-0.6.7/sqlalchemy_clickzetta/requirements.py`

 * *Files identical despite different names*

