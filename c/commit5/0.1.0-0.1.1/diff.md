# Comparing `tmp/commit5-0.1.0.tar.gz` & `tmp/commit5-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commit5-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "commit5-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `commit5-0.1.0.tar` & `commit5-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1422 2023-05-17 18:16:48.603494 commit5-0.1.0/app.py
--rw-r--r--   0        0        0       73 2023-05-10 22:10:32.647649 commit5-0.1.0/docker/.dockerignore
--rw-r--r--   0        0        0      392 2023-05-17 17:42:51.849607 commit5-0.1.0/docker/Dockerfile
--rw-r--r--   0        0        0      521 2023-05-15 21:52:32.922662 commit5-0.1.0/docker/api.py
--rw-r--r--   0        0        0      151 2023-05-15 21:56:45.943497 commit5-0.1.0/docker/download_tokenizer.py
--rw-r--r--   0        0        0     1340 2023-05-15 19:43:38.753082 commit5-0.1.0/docker/generator.py
--rw-r--r--   0        0        0     1711 2023-05-17 05:43:27.192500 commit5-0.1.0/docker/requirements.txt
-drwxr-xr-x   0        0        0        0 2023-05-10 20:12:18.487785 commit5-0.1.0/fastT5/
--rw-r--r--   0        0        0      530 2023-05-17 21:21:33.681362 commit5-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      199 2023-05-16 20:12:41.896228 commit5-0.1.0/tests/test_generate.py
--rw-r--r--   0        0        0      201 2023-05-10 08:58:48.339406 commit5-0.1.0/tests/test_server.py
--rw-r--r--   0        0        0      368 1970-01-01 00:00:00.000000 commit5-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2560 2023-05-17 21:37:37.726918 commit5-0.1.1/README.md
+-rw-r--r--   0        0        0     1422 2023-05-17 18:16:48.603494 commit5-0.1.1/app.py
+-rw-r--r--   0        0        0       73 2023-05-10 22:10:32.647649 commit5-0.1.1/docker/.dockerignore
+-rw-r--r--   0        0        0      392 2023-05-17 17:42:51.849607 commit5-0.1.1/docker/Dockerfile
+-rw-r--r--   0        0        0      521 2023-05-15 21:52:32.922662 commit5-0.1.1/docker/api.py
+-rw-r--r--   0        0        0      151 2023-05-15 21:56:45.943497 commit5-0.1.1/docker/download_tokenizer.py
+-rw-r--r--   0        0        0     1340 2023-05-15 19:43:38.753082 commit5-0.1.1/docker/generator.py
+-rw-r--r--   0        0        0     1711 2023-05-17 05:43:27.192500 commit5-0.1.1/docker/requirements.txt
+drwxr-xr-x   0        0        0        0 2023-05-10 20:12:18.487785 commit5-0.1.1/fastT5/
+-rw-r--r--   0        0        0      551 2023-05-17 21:39:09.424722 commit5-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-05-16 20:12:41.896228 commit5-0.1.1/tests/test_generate.py
+-rw-r--r--   0        0        0      201 2023-05-10 08:58:48.339406 commit5-0.1.1/tests/test_server.py
+-rw-r--r--   0        0        0     2970 1970-01-01 00:00:00.000000 commit5-0.1.1/PKG-INFO
```

### Comparing `commit5-0.1.0/app.py` & `commit5-0.1.1/app.py`

 * *Files identical despite different names*

### Comparing `commit5-0.1.0/docker/api.py` & `commit5-0.1.1/docker/api.py`

 * *Files identical despite different names*

### Comparing `commit5-0.1.0/docker/generator.py` & `commit5-0.1.1/docker/generator.py`

 * *Files identical despite different names*

### Comparing `commit5-0.1.0/docker/requirements.txt` & `commit5-0.1.1/docker/requirements.txt`

 * *Files identical despite different names*

### Comparing `commit5-0.1.0/pyproject.toml` & `commit5-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [project]
 name = "commit5"
 description = "Locally generate commit messages using CodeTrans and FastT5"
-version = "0.1.0"
+readme = "README.md"
+version = "0.1.1"
 authors = [
     { name = "Kevin Lu", email = "kevinlu1248@gmail.com" }
 ]
 dependencies = [
     "docker",
     "typer",
     "requests"
```

