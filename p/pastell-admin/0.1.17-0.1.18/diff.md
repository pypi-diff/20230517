# Comparing `tmp/pastell-admin-0.1.17.tar.gz` & `tmp/pastell-admin-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastell-admin-0.1.17.tar", last modified: Thu May  4 08:11:01 2023, max compression
+gzip compressed data, was "pastell-admin-0.1.18.tar", last modified: Wed May 17 15:12:12 2023, max compression
```

## Comparing `pastell-admin-0.1.17.tar` & `pastell-admin-0.1.18.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/src/pastell_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/src/pastelladmin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/src/pastelladmin/api/
--rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/delete_any.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_associations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15496 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_connector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1990 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_connector_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_docs_delete_from_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_find.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3213 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_matrice_roles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2540 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_org.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/src/pastelladmin/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/shared/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:12.749566 pastell-admin-0.1.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-05-17 15:12:12.749566 pastell-admin-0.1.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:12:12.749566 pastell-admin-0.1.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:12.745566 pastell-admin-0.1.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:12.749566 pastell-admin-0.1.18/src/pastell_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-05-17 15:12:12.000000 pastell-admin-0.1.18/src/pastell_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-17 15:12:12.000000 pastell-admin-0.1.18/src/pastell_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:12:12.000000 pastell-admin-0.1.18/src/pastell_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-17 15:12:12.000000 pastell-admin-0.1.18/src/pastell_admin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 15:12:12.000000 pastell-admin-0.1.18/src/pastell_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 15:12:12.000000 pastell-admin-0.1.18/src/pastell_admin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:12.749566 pastell-admin-0.1.18/src/pastelladmin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:12.749566 pastell-admin-0.1.18/src/pastelladmin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    20794 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/delete_any.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/pastell_associations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15496 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/pastell_connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1990 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/pastell_connector_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/pastell_docs_delete_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/pastell_find.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3213 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/pastell_matrice_roles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2540 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/pastell_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/pastell_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:12.749566 pastell-admin-0.1.18/src/pastelladmin/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-17 15:12:03.000000 pastell-admin-0.1.18/src/pastelladmin/shared/configuration.py
```

### Comparing `pastell-admin-0.1.17/LICENSE` & `pastell-admin-0.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.17/PKG-INFO` & `pastell-admin-0.1.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastell-admin
-Version: 0.1.17
+Version: 0.1.18
 Author-email: Sebastien Pelhate <sebastien.pelhate@megalis.bretagne.bzh>, Yann Guenneugues <yann.guenneugues@sib.fr>
 Project-URL: Homepage, https://github.com/megalis-bretagne/scripts-pastell
 Project-URL: Bug Tracker, https://github.com/megalis-bretagne/scripts-pastell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,22 +17,22 @@
 
 
 # Installation
 
 Pour la version stable :
 
 ```
-pip install pastell-admin==0.1.17
+pip install pastell-admin==0.1.18
 ```
 
 Pour la version de dev :
 
 ```
 pip install requests
-pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.17
+pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.18
 ```
 # Développement
 
 ```
 git clone git@github.com:megalis-bretagne/scripts-pastell.git
 cd scripts-pastell
 python3 -m venv .venv
```

### Comparing `pastell-admin-0.1.17/README.md` & `pastell-admin-0.1.18/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 
 # Installation
 
 Pour la version stable :
 
 ```
-pip install pastell-admin==0.1.17
+pip install pastell-admin==0.1.18
 ```
 
 Pour la version de dev :
 
 ```
 pip install requests
-pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.17
+pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.18
 ```
 # Développement
 
 ```
 git clone git@github.com:megalis-bretagne/scripts-pastell.git
 cd scripts-pastell
 python3 -m venv .venv
```

### Comparing `pastell-admin-0.1.17/pyproject.toml` & `pastell-admin-0.1.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pastell-admin"
-version = "0.1.17"
+version = "0.1.18"
 authors = [
   { name="Sebastien Pelhate", email="sebastien.pelhate@megalis.bretagne.bzh"}, {name ="Yann Guenneugues" ,email="yann.guenneugues@sib.fr"  }
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pastell-admin-0.1.17/src/pastell_admin.egg-info/PKG-INFO` & `pastell-admin-0.1.18/src/pastell_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastell-admin
-Version: 0.1.17
+Version: 0.1.18
 Author-email: Sebastien Pelhate <sebastien.pelhate@megalis.bretagne.bzh>, Yann Guenneugues <yann.guenneugues@sib.fr>
 Project-URL: Homepage, https://github.com/megalis-bretagne/scripts-pastell
 Project-URL: Bug Tracker, https://github.com/megalis-bretagne/scripts-pastell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,22 +17,22 @@
 
 
 # Installation
 
 Pour la version stable :
 
 ```
-pip install pastell-admin==0.1.17
+pip install pastell-admin==0.1.18
 ```
 
 Pour la version de dev :
 
 ```
 pip install requests
-pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.17
+pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.18
 ```
 # Développement
 
 ```
 git clone git@github.com:megalis-bretagne/scripts-pastell.git
 cd scripts-pastell
 python3 -m venv .venv
```

### Comparing `pastell-admin-0.1.17/src/pastell_admin.egg-info/SOURCES.txt` & `pastell-admin-0.1.18/src/pastell_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.17/src/pastelladmin/api/client.py` & `pastell-admin-0.1.18/src/pastelladmin/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -531,15 +531,39 @@
             success = True
         else:
             result = request.text
             success = False
 
         return Result(success, result)
 
+    def update(self, id_e, id_d, data):
+        url = f"https://{self.server}/api/v2/entite/{id_e}/document/{id_d}"
+        request = requests.patch(url, auth=self.auth, data=data)
+        success = None
+        if request.status_code == 200:
+            result = json.loads(request.text)
+            success = True
+        else:
+            result = request.text
+            success = False
+
+        return Result(success, result)
 
+    def action(self, id_e, id_d, action):
+        url = f"https://{self.server}/api/v2/entite/{id_e}/document/{id_d}/action/{action}"
+        request = requests.post(url, auth=self.auth)
+        success = None
+        if request.status_code == 201:
+            result = json.loads(request.text)
+            success = True
+        else:
+            result = request.text
+            success = False
+
+        return Result(success, result)
 
     def getByFilter(self, id_e, dossier=None, status=None, start=None, end=None, transit=False, pagination=1000 ):
         #check types
         date_format = "%Y-%m-%d"
         for date in (start, end):
             if date:
                 assert datetime.strptime(date, date_format)
```

### Comparing `pastell-admin-0.1.17/src/pastelladmin/delete_any.py` & `pastell-admin-0.1.18/src/pastelladmin/delete_any.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.17/src/pastelladmin/pastell_associations.py` & `pastell-admin-0.1.18/src/pastelladmin/pastell_associations.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.17/src/pastelladmin/pastell_connector.py` & `pastell-admin-0.1.18/src/pastelladmin/pastell_connector.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.17/src/pastelladmin/pastell_connector_instances.py` & `pastell-admin-0.1.18/src/pastelladmin/pastell_connector_instances.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.17/src/pastelladmin/pastell_docs_delete_from_list.py` & `pastell-admin-0.1.18/src/pastelladmin/pastell_docs_delete_from_list.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.17/src/pastelladmin/pastell_find.py` & `pastell-admin-0.1.18/src/pastelladmin/pastell_find.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.17/src/pastelladmin/pastell_matrice_roles.py` & `pastell-admin-0.1.18/src/pastelladmin/pastell_matrice_roles.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.17/src/pastelladmin/pastell_org.py` & `pastell-admin-0.1.18/src/pastelladmin/pastell_org.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.17/src/pastelladmin/pastell_stats.py` & `pastell-admin-0.1.18/src/pastelladmin/pastell_stats.py`

 * *Files identical despite different names*

