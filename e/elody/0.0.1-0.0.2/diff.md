# Comparing `tmp/elody-0.0.1.tar.gz` & `tmp/elody-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elody-0.0.1.tar", last modified: Wed May 17 14:26:47 2023, max compression
+gzip compressed data, was "elody-0.0.2.tar", last modified: Wed May 17 14:42:40 2023, max compression
```

## Comparing `elody-0.0.1.tar` & `elody-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:26:47.033868 elody-0.0.1/
--rw-r--r--   0 booster   (1000) booster   (1000)    18092 2023-05-17 14:21:56.000000 elody-0.0.1/LICENSE
--rw-r--r--   0 booster   (1000) booster   (1000)    22518 2023-05-17 14:26:47.033868 elody-0.0.1/PKG-INFO
--rw-r--r--   0 booster   (1000) booster   (1000)     1263 2023-05-17 14:21:56.000000 elody-0.0.1/README.md
--rw-r--r--   0 booster   (1000) booster   (1000)      714 2023-05-17 14:21:56.000000 elody-0.0.1/pyproject.toml
--rw-r--r--   0 booster   (1000) booster   (1000)       38 2023-05-17 14:26:47.033868 elody-0.0.1/setup.cfg
-drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:26:47.030534 elody-0.0.1/src/
-drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:26:47.030534 elody-0.0.1/src/elody/
--rw-r--r--   0 booster   (1000) booster   (1000)       22 2023-05-17 14:21:56.000000 elody-0.0.1/src/elody/__init__.py
--rw-r--r--   0 booster   (1000) booster   (1000)     3932 2023-05-17 14:21:56.000000 elody-0.0.1/src/elody/client.py
--rw-r--r--   0 booster   (1000) booster   (1000)      209 2023-05-17 14:21:56.000000 elody-0.0.1/src/elody/exceptions.py
-drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:26:47.030534 elody-0.0.1/src/elody.egg-info/
--rw-r--r--   0 booster   (1000) booster   (1000)    22518 2023-05-17 14:26:47.000000 elody-0.0.1/src/elody.egg-info/PKG-INFO
--rw-r--r--   0 booster   (1000) booster   (1000)      262 2023-05-17 14:26:47.000000 elody-0.0.1/src/elody.egg-info/SOURCES.txt
--rw-r--r--   0 booster   (1000) booster   (1000)        1 2023-05-17 14:26:47.000000 elody-0.0.1/src/elody.egg-info/dependency_links.txt
--rw-r--r--   0 booster   (1000) booster   (1000)       86 2023-05-17 14:26:47.000000 elody-0.0.1/src/elody.egg-info/requires.txt
--rw-r--r--   0 booster   (1000) booster   (1000)        6 2023-05-17 14:26:47.000000 elody-0.0.1/src/elody.egg-info/top_level.txt
+drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:42:40.395948 elody-0.0.2/
+-rw-r--r--   0 booster   (1000) booster   (1000)    18092 2023-05-17 14:21:56.000000 elody-0.0.2/LICENSE
+-rw-r--r--   0 booster   (1000) booster   (1000)    22518 2023-05-17 14:42:40.395948 elody-0.0.2/PKG-INFO
+-rw-r--r--   0 booster   (1000) booster   (1000)     1263 2023-05-17 14:21:56.000000 elody-0.0.2/README.md
+-rw-r--r--   0 booster   (1000) booster   (1000)      714 2023-05-17 14:41:40.000000 elody-0.0.2/pyproject.toml
+-rw-r--r--   0 booster   (1000) booster   (1000)       38 2023-05-17 14:42:40.395948 elody-0.0.2/setup.cfg
+drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:42:40.395948 elody-0.0.2/src/
+drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:42:40.395948 elody-0.0.2/src/elody/
+-rw-r--r--   0 booster   (1000) booster   (1000)       22 2023-05-17 14:21:56.000000 elody-0.0.2/src/elody/__init__.py
+-rw-r--r--   0 booster   (1000) booster   (1000)     3937 2023-05-17 14:40:43.000000 elody-0.0.2/src/elody/client.py
+-rw-r--r--   0 booster   (1000) booster   (1000)      209 2023-05-17 14:21:56.000000 elody-0.0.2/src/elody/exceptions.py
+drwxr-xr-x   0 booster   (1000) booster   (1000)        0 2023-05-17 14:42:40.395948 elody-0.0.2/src/elody.egg-info/
+-rw-r--r--   0 booster   (1000) booster   (1000)    22518 2023-05-17 14:42:40.000000 elody-0.0.2/src/elody.egg-info/PKG-INFO
+-rw-r--r--   0 booster   (1000) booster   (1000)      262 2023-05-17 14:42:40.000000 elody-0.0.2/src/elody.egg-info/SOURCES.txt
+-rw-r--r--   0 booster   (1000) booster   (1000)        1 2023-05-17 14:42:40.000000 elody-0.0.2/src/elody.egg-info/dependency_links.txt
+-rw-r--r--   0 booster   (1000) booster   (1000)       86 2023-05-17 14:42:40.000000 elody-0.0.2/src/elody.egg-info/requires.txt
+-rw-r--r--   0 booster   (1000) booster   (1000)        6 2023-05-17 14:42:40.000000 elody-0.0.2/src/elody.egg-info/top_level.txt
```

### Comparing `elody-0.0.1/LICENSE` & `elody-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elody-0.0.1/PKG-INFO` & `elody-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.1
+Version: 0.0.2
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `elody-0.0.1/README.md` & `elody-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `elody-0.0.1/pyproject.toml` & `elody-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elody"
-version = "0.0.1"
+version = "0.0.2"
 description = "elody SDK for Python"
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Intended Audience :: Developers",
```

### Comparing `elody-0.0.1/src/elody/client.py` & `elody-0.0.2/src/elody/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .exceptions import NonUniqueException, NotFoundException
 
 
 class Client:
     def __init__(self, elody_collection_url=None, static_jwt=None):
         self.elody_collection_url = elody_collection_url or os.environ.get("ELODY_COLLECTION_URL", None)
         self.static_jwt = static_jwt or os.environ.get("STATIC_JWT", None)
-        self.headers = {"Authorization": f"Bearer {static_jwt}"}
+        self.headers = {"Authorization": f"Bearer {self.static_jwt}"}
 
     def __create_mediafile(self, entity_id, mediafile):
         url = f"{self.elody_collection_url}/entities/{entity_id}/mediafiles"
         headers = {**self.headers, **{"Accept": "text/uri-list"}}
         response = requests.post(url, json=mediafile, headers=headers)
         return self.__handle_response(
             response, "Failed to create mediafile", "text"
```

### Comparing `elody-0.0.1/src/elody.egg-info/PKG-INFO` & `elody-0.0.2/src/elody.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.1
+Version: 0.0.2
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

