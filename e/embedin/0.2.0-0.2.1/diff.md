# Comparing `tmp/embedin-0.2.0.tar.gz` & `tmp/embedin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedin-0.2.0.tar", last modified: Sat May 13 23:59:15 2023, max compression
+gzip compressed data, was "embedin-0.2.1.tar", last modified: Wed May 17 03:02:11 2023, max compression
```

## Comparing `embedin-0.2.0.tar` & `embedin-0.2.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.205288 embedin-0.2.0/
--rw-r--r--   0 xchen375   (502) staff       (20)    11357 2023-04-10 04:12:37.000000 embedin-0.2.0/LICENSE
--rw-r--r--   0 xchen375   (502) staff       (20)     3655 2023-05-13 23:59:15.204888 embedin-0.2.0/PKG-INFO
--rw-r--r--   0 xchen375   (502) staff       (20)     3218 2023-05-13 23:56:49.000000 embedin-0.2.0/README.md
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.184662 embedin-0.2.0/embedin/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-09 17:01:17.000000 embedin-0.2.0/embedin/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.186886 embedin-0.2.0/embedin/client/
--rw-r--r--   0 xchen375   (502) staff       (20)     6524 2023-05-13 23:39:26.000000 embedin-0.2.0/embedin/client/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.188462 embedin-0.2.0/embedin/embedding/
--rw-r--r--   0 xchen375   (502) staff       (20)     1931 2023-05-13 23:39:26.000000 embedin-0.2.0/embedin/embedding/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      134 2023-05-13 23:39:26.000000 embedin-0.2.0/embedin/embedding/embedding_base.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1647 2023-05-13 23:39:26.000000 embedin-0.2.0/embedin/embedding/openai_embedding.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1927 2023-05-13 23:39:26.000000 embedin-0.2.0/embedin/embedding/sentence_transformer.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.190455 embedin-0.2.0/embedin/index/
--rw-r--r--   0 xchen375   (502) staff       (20)      693 2023-05-13 19:19:06.000000 embedin-0.2.0/embedin/index/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2317 2023-05-13 19:19:06.000000 embedin-0.2.0/embedin/index/flat_index.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2331 2023-05-13 19:19:06.000000 embedin-0.2.0/embedin/index/hnsw_index.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1373 2023-05-13 19:19:06.000000 embedin-0.2.0/embedin/index/index_base.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.191821 embedin-0.2.0/embedin/model/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/embedin/model/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      275 2023-04-22 15:16:27.000000 embedin-0.2.0/embedin/model/collection_model.py
--rw-r--r--   0 xchen375   (502) staff       (20)      610 2023-04-22 15:16:27.000000 embedin-0.2.0/embedin/model/embedding_model.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.193244 embedin-0.2.0/embedin/repository/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/embedin/repository/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2667 2023-04-22 22:11:55.000000 embedin-0.2.0/embedin/repository/collection_repository.py
--rw-r--r--   0 xchen375   (502) staff       (20)     3496 2023-04-22 22:11:55.000000 embedin-0.2.0/embedin/repository/embedding_repository.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.195504 embedin-0.2.0/embedin/service/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/embedin/service/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2258 2023-04-22 22:11:55.000000 embedin-0.2.0/embedin/service/collection_service.py
--rw-r--r--   0 xchen375   (502) staff       (20)     3978 2023-04-22 22:11:55.000000 embedin-0.2.0/embedin/service/embedding_service.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.196144 embedin-0.2.0/embedin/util/
--rw-r--r--   0 xchen375   (502) staff       (20)     1354 2023-05-13 19:19:06.000000 embedin-0.2.0/embedin/util/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.186505 embedin-0.2.0/embedin.egg-info/
--rw-r--r--   0 xchen375   (502) staff       (20)     3655 2023-05-13 23:59:15.000000 embedin-0.2.0/embedin.egg-info/PKG-INFO
--rw-r--r--   0 xchen375   (502) staff       (20)     1463 2023-05-13 23:59:15.000000 embedin-0.2.0/embedin.egg-info/SOURCES.txt
--rw-r--r--   0 xchen375   (502) staff       (20)        1 2023-05-13 23:59:15.000000 embedin-0.2.0/embedin.egg-info/dependency_links.txt
--rw-r--r--   0 xchen375   (502) staff       (20)      165 2023-05-13 23:59:15.000000 embedin-0.2.0/embedin.egg-info/requires.txt
--rw-r--r--   0 xchen375   (502) staff       (20)       14 2023-05-13 23:59:15.000000 embedin-0.2.0/embedin.egg-info/top_level.txt
--rw-r--r--   0 xchen375   (502) staff       (20)       38 2023-05-13 23:59:15.205399 embedin-0.2.0/setup.cfg
--rw-r--r--   0 xchen375   (502) staff       (20)      841 2023-05-13 23:58:06.000000 embedin-0.2.0/setup.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.196664 embedin-0.2.0/tests/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-10 19:13:54.000000 embedin-0.2.0/tests/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.196976 embedin-0.2.0/tests/client/
--rw-r--r--   0 xchen375   (502) staff       (20)     2163 2023-05-13 23:39:26.000000 embedin-0.2.0/tests/client/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.198465 embedin-0.2.0/tests/embedding/
--rw-r--r--   0 xchen375   (502) staff       (20)     1282 2023-05-13 23:39:26.000000 embedin-0.2.0/tests/embedding/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      296 2023-05-13 23:39:26.000000 embedin-0.2.0/tests/embedding/test_embedding_base.py
--rw-r--r--   0 xchen375   (502) staff       (20)      818 2023-05-13 23:39:26.000000 embedin-0.2.0/tests/embedding/test_openai_embedding.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1398 2023-05-13 23:39:26.000000 embedin-0.2.0/tests/embedding/test_sentence_transformer_embedding.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.199806 embedin-0.2.0/tests/index/
--rw-r--r--   0 xchen375   (502) staff       (20)     2065 2023-05-13 19:19:06.000000 embedin-0.2.0/tests/index/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2593 2023-05-13 19:19:06.000000 embedin-0.2.0/tests/index/test_flat_index.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2939 2023-05-13 19:19:06.000000 embedin-0.2.0/tests/index/test_hnsw_index.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.201147 embedin-0.2.0/tests/model/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/tests/model/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1938 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/model/test_collection_model.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2044 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/model/test_embedding_model.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.202544 embedin-0.2.0/tests/repository/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/tests/repository/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2479 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/repository/test_collection_repository.py
--rw-r--r--   0 xchen375   (502) staff       (20)     5427 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/repository/test_embedding_repository.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.203857 embedin-0.2.0/tests/service/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/tests/service/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1333 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/service/test_collection_service.py
--rw-r--r--   0 xchen375   (502) staff       (20)     3705 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/service/test_embedding_service.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.204300 embedin-0.2.0/tests/util/
--rw-r--r--   0 xchen375   (502) staff       (20)     1588 2023-05-13 19:19:06.000000 embedin-0.2.0/tests/util/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.636803 embedin-0.2.1/
+-rw-r--r--   0 xchen375   (502) staff       (20)    11357 2023-04-10 04:12:37.000000 embedin-0.2.1/LICENSE
+-rw-r--r--   0 xchen375   (502) staff       (20)     3492 2023-05-17 03:02:11.636191 embedin-0.2.1/PKG-INFO
+-rw-r--r--   0 xchen375   (502) staff       (20)     3055 2023-05-17 03:00:39.000000 embedin-0.2.1/README.md
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.609407 embedin-0.2.1/embedin/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-09 17:01:17.000000 embedin-0.2.1/embedin/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.611707 embedin-0.2.1/embedin/client/
+-rw-r--r--   0 xchen375   (502) staff       (20)     7381 2023-05-17 03:00:39.000000 embedin-0.2.1/embedin/client/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.613420 embedin-0.2.1/embedin/embedding/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1931 2023-05-15 01:03:38.000000 embedin-0.2.1/embedin/embedding/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      134 2023-05-13 23:39:26.000000 embedin-0.2.1/embedin/embedding/embedding_base.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1647 2023-05-13 23:39:26.000000 embedin-0.2.1/embedin/embedding/openai_embedding.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2043 2023-05-17 03:00:39.000000 embedin-0.2.1/embedin/embedding/sentence_transformer.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.616036 embedin-0.2.1/embedin/index/
+-rw-r--r--   0 xchen375   (502) staff       (20)      693 2023-05-13 19:19:06.000000 embedin-0.2.1/embedin/index/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2317 2023-05-13 19:19:06.000000 embedin-0.2.1/embedin/index/flat_index.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2331 2023-05-13 19:19:06.000000 embedin-0.2.1/embedin/index/hnsw_index.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1373 2023-05-13 19:19:06.000000 embedin-0.2.1/embedin/index/index_base.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.617686 embedin-0.2.1/embedin/model/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/embedin/model/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      275 2023-04-22 15:16:27.000000 embedin-0.2.1/embedin/model/collection_model.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      610 2023-04-22 15:16:27.000000 embedin-0.2.1/embedin/model/embedding_model.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.619385 embedin-0.2.1/embedin/repository/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/embedin/repository/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2667 2023-05-15 21:05:11.000000 embedin-0.2.1/embedin/repository/collection_repository.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     4381 2023-05-17 03:00:39.000000 embedin-0.2.1/embedin/repository/embedding_repository.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.620959 embedin-0.2.1/embedin/service/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/embedin/service/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2322 2023-05-17 03:00:39.000000 embedin-0.2.1/embedin/service/collection_service.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     4114 2023-05-17 03:00:39.000000 embedin-0.2.1/embedin/service/embedding_service.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.621618 embedin-0.2.1/embedin/util/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1354 2023-05-13 19:19:06.000000 embedin-0.2.1/embedin/util/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.611293 embedin-0.2.1/embedin.egg-info/
+-rw-r--r--   0 xchen375   (502) staff       (20)     3492 2023-05-17 03:02:11.000000 embedin-0.2.1/embedin.egg-info/PKG-INFO
+-rw-r--r--   0 xchen375   (502) staff       (20)     1463 2023-05-17 03:02:11.000000 embedin-0.2.1/embedin.egg-info/SOURCES.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)        1 2023-05-17 03:02:11.000000 embedin-0.2.1/embedin.egg-info/dependency_links.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)      170 2023-05-17 03:02:11.000000 embedin-0.2.1/embedin.egg-info/requires.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)       14 2023-05-17 03:02:11.000000 embedin-0.2.1/embedin.egg-info/top_level.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)       38 2023-05-17 03:02:11.636953 embedin-0.2.1/setup.cfg
+-rw-r--r--   0 xchen375   (502) staff       (20)      841 2023-05-17 03:00:33.000000 embedin-0.2.1/setup.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.622345 embedin-0.2.1/tests/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-10 19:13:54.000000 embedin-0.2.1/tests/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.622841 embedin-0.2.1/tests/client/
+-rw-r--r--   0 xchen375   (502) staff       (20)     2951 2023-05-17 03:00:39.000000 embedin-0.2.1/tests/client/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.625463 embedin-0.2.1/tests/embedding/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1282 2023-05-13 23:39:26.000000 embedin-0.2.1/tests/embedding/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      296 2023-05-13 23:39:26.000000 embedin-0.2.1/tests/embedding/test_embedding_base.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      818 2023-05-13 23:39:26.000000 embedin-0.2.1/tests/embedding/test_openai_embedding.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1398 2023-05-13 23:39:26.000000 embedin-0.2.1/tests/embedding/test_sentence_transformer_embedding.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.627848 embedin-0.2.1/tests/index/
+-rw-r--r--   0 xchen375   (502) staff       (20)     2065 2023-05-13 19:19:06.000000 embedin-0.2.1/tests/index/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2593 2023-05-13 19:19:06.000000 embedin-0.2.1/tests/index/test_flat_index.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2939 2023-05-13 19:19:06.000000 embedin-0.2.1/tests/index/test_hnsw_index.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.630258 embedin-0.2.1/tests/model/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/tests/model/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1938 2023-04-22 22:11:55.000000 embedin-0.2.1/tests/model/test_collection_model.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2044 2023-04-22 22:11:55.000000 embedin-0.2.1/tests/model/test_embedding_model.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.632527 embedin-0.2.1/tests/repository/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/tests/repository/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2479 2023-04-22 22:11:55.000000 embedin-0.2.1/tests/repository/test_collection_repository.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     7360 2023-05-17 03:00:39.000000 embedin-0.2.1/tests/repository/test_embedding_repository.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.634407 embedin-0.2.1/tests/service/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/tests/service/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1333 2023-04-22 22:11:55.000000 embedin-0.2.1/tests/service/test_collection_service.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     3752 2023-05-17 03:00:39.000000 embedin-0.2.1/tests/service/test_embedding_service.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.635237 embedin-0.2.1/tests/util/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1588 2023-05-13 19:19:06.000000 embedin-0.2.1/tests/util/__init__.py
```

### Comparing `embedin-0.2.0/LICENSE` & `embedin-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/PKG-INFO` & `embedin-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedin
-Version: 0.2.0
+Version: 0.2.1
 Summary: A lightweight vector database
 Home-page: https://github.com/EmbedInAI/EmbedInDB
 Author: EmbedInAI
 Author-email: EmbedInAI@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -23,54 +23,51 @@
 
 ## Installation
 ```bash
 pip install embedin
 ```
 
 ## Quick Start
-### Using memory DB
+### Using memory
 ```python
 from embedin.client import Client
 
-client = Client(collection_name="test_collection")
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
+print(result)
 ```
 
-### Using sqlite with local storage
+### Using Sqlite
 ```python
 from embedin.client import Client
 
 url = 'sqlite:///test.db'
-client = Client(collection_name="test_collection", url=url)
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using PostgreSQL
 ```python
 import os
 
 from embedin.client import Client
 
 url = os.getenv('EMBEDIN_POSGRES_URL', "postgresql+psycopg2://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", url=url)
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using MySQL
 ```python
 import os
 
 from embedin.client import Client
 
 url = os.getenv('EMBEDIN_MYSQL_URL', "mysql+pymysql://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", url=url)
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using MS-SQL
 ```python
 import os
```

### Comparing `embedin-0.2.0/README.md` & `embedin-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,54 +9,51 @@
 
 ## Installation
 ```bash
 pip install embedin
 ```
 
 ## Quick Start
-### Using memory DB
+### Using memory
 ```python
 from embedin.client import Client
 
-client = Client(collection_name="test_collection")
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
+print(result)
 ```
 
-### Using sqlite with local storage
+### Using Sqlite
 ```python
 from embedin.client import Client
 
 url = 'sqlite:///test.db'
-client = Client(collection_name="test_collection", url=url)
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using PostgreSQL
 ```python
 import os
 
 from embedin.client import Client
 
 url = os.getenv('EMBEDIN_POSGRES_URL', "postgresql+psycopg2://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", url=url)
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using MySQL
 ```python
 import os
 
 from embedin.client import Client
 
 url = os.getenv('EMBEDIN_MYSQL_URL', "mysql+pymysql://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", url=url)
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using MS-SQL
 ```python
 import os
```

### Comparing `embedin-0.2.0/embedin/client/__init__.py` & `embedin-0.2.1/embedin/client/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     def __init__(
         self,
         collection_name,
         url=None,
         embedding_fn="sentence_transformer",
         index_hint=None,
         debug=False,
+        **kwargs
     ):
         self.collection_id = None
 
         if callable(embedding_fn):
             self.embedding_fn = embedding_fn
         else:
             self.embedding_fn = Embedding.create_embedding(embedding_fn)
@@ -65,32 +66,53 @@
 
         session = sessionmaker(bind=engine)
         self.session = session()
 
         self.collection_service = CollectionService(self.session)
         self.embedding_service = EmbeddingService(self.session)
 
-        collection_id = self.create_or_get_collection(collection_name)
-        self.embedding_rows = self.embedding_service.get_by_collection_id(collection_id)
-        embeddings = [row.embedding_data for row in self.embedding_rows]
+        embeddings = kwargs.get("embeddings")
+        embeddings_meta = kwargs.get("meta")
+        texts = kwargs.get("texts")
+
+        self.collection_id = self.create_or_get_collection(collection_name)
+        self.embedding_rows = self.embedding_service.get_by_collection_id(
+            self.collection_id
+        )
+
+        # Insert user-provided texts and embeddings into the database
+        inserted_rows = []
+        if embeddings is not None and texts is not None:
+            # TODO validate embeddings' shape and dtype; validate text as well
+            inserted_rows = self.embedding_service.add_all(
+                self.collection_id, embeddings, texts, embeddings_meta
+            )
+        elif texts is not None:
+            embeddings = self.embedding_fn(texts)
+            inserted_rows = self.embedding_service.add_all(
+                self.collection_id, embeddings, texts, embeddings_meta
+            )
+
+        self.embedding_rows.extend(inserted_rows)
+        total_embeddings = [row.embedding_data for row in self.embedding_rows]
 
         self.index_hint = index_hint
         self.search_index = None
-        if embeddings:
-            self.search_index = Index(embeddings, self.index_hint)
+        if total_embeddings:
+            self.search_index = Index(total_embeddings, self.index_hint)
 
     def create_or_get_collection(self, name):
         """
         Get the ID of an existing collection or create a new one with the given name.
 
         Args:
             name (str): Name of the collection.
 
         Returns:
-            int: ID of the collection.
+            str: ID of the collection.
         """
         collection_id = self.get_collection(name)
         if not collection_id:
             collection_id = self.create_collection(name)
         self.collection_id = collection_id
         return collection_id
 
@@ -98,29 +120,29 @@
         """
         Create a new collection with the given name.
 
         Args:
             name (str): Name of the collection.
 
         Returns:
-            int: ID of the new collection.
+            str: ID of the new collection.
         """
         collection = self.collection_service.create(name)
         self.collection_id = collection.id
         return self.collection_id
 
     def get_collection(self, name):
         """
         Retrieve the ID of an existing collection with the given name.
 
         Args:
             name (str): Name of the collection.
 
         Returns:
-            int: ID of the collection, or None if no collection with the given name exists.
+            str: ID of the collection, or None if no collection with the given name exists.
         """
         collection = self.collection_service.get_by_name(name)
         if collection:
             self.collection_id = collection.id
             return self.collection_id
 
     def add_data(self, texts, meta_data=None):
@@ -131,20 +153,20 @@
             texts (list of str): List of text data to add to the collection.
             meta_data (list or None): List of associated metadata for the added text data (optional).
 
         Returns:
             None.
         """
         embeddings = self.embedding_fn(texts)
+        logger.info("Adding embedding to the database")
         inserted_data = self.embedding_service.add_all(
             self.collection_id, embeddings, texts, meta_data
         )
-        logger.info("inserted_data: %s", inserted_data)
 
-        self.embedding_rows += inserted_data
+        self.embedding_rows.extend(inserted_data)
 
         inserted_embeddings = [row.embedding_data for row in inserted_data]
 
         if self.search_index is None:
             self.search_index = Index(embeddings, self.index_hint)
         else:
             self.search_index.update_index(inserted_embeddings)
```

### Comparing `embedin-0.2.0/embedin/embedding/__init__.py` & `embedin-0.2.1/embedin/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/embedin/embedding/openai_embedding.py` & `embedin-0.2.1/embedin/embedding/openai_embedding.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/embedin/embedding/sentence_transformer.py` & `embedin-0.2.1/embedin/embedding/sentence_transformer.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 
         Returns:
         embeddings (list): A list of embeddings generated for the input text(s). Each embedding is a list of float values.
         """
         # Return it as a numpy array
         # Check if texts is a string
         if isinstance(texts, str):
-            return self.model.encode([texts], convert_to_numpy=True).tolist()
+            return self.model.encode(
+                [texts], convert_to_numpy=True, show_progress_bar=True
+            ).tolist()
         # Check if texts is a list of strings
         if isinstance(texts, list):
             if all(isinstance(text, str) for text in texts):
-                return self.model.encode(texts, convert_to_numpy=True).tolist()
+                return self.model.encode(
+                    texts, convert_to_numpy=True, show_progress_bar=True
+                ).tolist()
             raise TypeError("Input must be a string, a list of strings")
         raise TypeError("Input must be a string, a list of strings")
```

### Comparing `embedin-0.2.0/embedin/index/__init__.py` & `embedin-0.2.1/embedin/index/__init__.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/embedin/index/flat_index.py` & `embedin-0.2.1/embedin/index/flat_index.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/embedin/index/hnsw_index.py` & `embedin-0.2.1/embedin/index/hnsw_index.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/embedin/index/index_base.py` & `embedin-0.2.1/embedin/index/index_base.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/embedin/model/embedding_model.py` & `embedin-0.2.1/embedin/model/embedding_model.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/embedin/repository/collection_repository.py` & `embedin-0.2.1/embedin/repository/collection_repository.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/embedin/service/collection_service.py` & `embedin-0.2.1/embedin/service/collection_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,25 +12,25 @@
         get_by_name(name):
             Fetches a collection from the database by its name.
 
             Args:
                 name (str): The name of the collection to retrieve.
 
             Returns:
-                dict: A dictionary representing the row of the collection fetched from the database.
+                CollectionModel: A CollectionModel representing the row of the collection fetched from the database.
 
         create(name, get_if_exist=True):
             Creates a new collection in the database.
 
             Args:
                 name (str): The name of the new collection.
                 get_if_exist (bool): If True, return the existing collection if it already exists. If False, create a new collection with the given name.
 
             Returns:
-                dict: A dictionary representing the newly created collection.
+                CollectionModel: A CollectionModel representing the newly created collection.
     """
 
     def __init__(self, session):
         """
         Initializes a new instance of the CollectionService class.
 
         Args:
@@ -43,27 +43,27 @@
         """
         Fetches a collection from the database by its name.
 
         Args:
             name (str): The name of the collection to retrieve.
 
         Returns:
-            dict: A dictionary representing the row of the collection fetched from the database.
+            CollectionModel: A CollectionModel representing the row of the collection fetched from the database.
         """
 
         row = self.collection_repo.get_by_name(name)
         return row
 
     def create(self, name, get_if_exist=True):
         """
         Creates a new collection in the database.
 
         Args:
             name (str): The name of the new collection.
             get_if_exist (bool): If True, return the existing collection if it already exists. If False, create a new collection with the given name.
 
         Returns:
-            dict: A dictionary representing the newly created collection.
+            CollectionModel: A CollectionModel representing the newly created collection.
         """
 
         collection = self.collection_repo.create(name, get_if_exist)
         return collection
```

### Comparing `embedin-0.2.0/embedin/service/embedding_service.py` & `embedin-0.2.1/embedin/service/embedding_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,22 +59,26 @@
 
         Returns:
             list: A list of EmbeddingModel objects representing the newly created embeddings.
         """
 
         # Generate a list of Embedding objects
         rows = []
+        hash_value_set = set()
         for i, embedding in enumerate(embeddings):
             # Generate a UUID for the embedding
             emb_id = str(uuid.uuid4())
 
             meta_data = metadata_list[i] if metadata_list else None
             data = texts[i] + collection_id + json.dumps(meta_data)
 
             hashed = hashlib.sha256(data.encode()).hexdigest()
+            if hashed in hash_value_set:
+                continue
+            hash_value_set.add(hashed)
 
             # Construct an Embedding object
             # TODO: should not call model class directly in service class
             row = EmbeddingModel(
                 id=emb_id,
                 collection_id=collection_id,
                 text=texts[i],
```

### Comparing `embedin-0.2.0/embedin/util/__init__.py` & `embedin-0.2.1/embedin/util/__init__.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/embedin.egg-info/PKG-INFO` & `embedin-0.2.1/embedin.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedin
-Version: 0.2.0
+Version: 0.2.1
 Summary: A lightweight vector database
 Home-page: https://github.com/EmbedInAI/EmbedInDB
 Author: EmbedInAI
 Author-email: EmbedInAI@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -23,54 +23,51 @@
 
 ## Installation
 ```bash
 pip install embedin
 ```
 
 ## Quick Start
-### Using memory DB
+### Using memory
 ```python
 from embedin.client import Client
 
-client = Client(collection_name="test_collection")
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
+print(result)
 ```
 
-### Using sqlite with local storage
+### Using Sqlite
 ```python
 from embedin.client import Client
 
 url = 'sqlite:///test.db'
-client = Client(collection_name="test_collection", url=url)
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using PostgreSQL
 ```python
 import os
 
 from embedin.client import Client
 
 url = os.getenv('EMBEDIN_POSGRES_URL', "postgresql+psycopg2://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", url=url)
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using MySQL
 ```python
 import os
 
 from embedin.client import Client
 
 url = os.getenv('EMBEDIN_MYSQL_URL', "mysql+pymysql://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", url=url)
-client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
+client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using MS-SQL
 ```python
 import os
```

### Comparing `embedin-0.2.0/embedin.egg-info/SOURCES.txt` & `embedin-0.2.1/embedin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/setup.py` & `embedin-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         os.path.join(os.path.dirname(__file__), fname), "r", encoding="utf-8"
     ) as fh:
         return fh.read()
 
 
 setuptools.setup(
     name="embedin",
-    version="0.2.0",
+    version="0.2.1",
     author="EmbedInAI",
     author_email="EmbedInAI@gmail.com",
     description="A lightweight vector database",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/EmbedInAI/EmbedInDB",
     packages=setuptools.find_packages(exclude=["tests"]),
```

### Comparing `embedin-0.2.0/tests/client/__init__.py` & `embedin-0.2.1/tests/repository/test_collection_repository.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-import unittest
-from unittest.mock import MagicMock
+from unittest import TestCase, mock
+from unittest.mock import Mock, patch
 
-from embedin.client import Client
+from embedin.model.collection_model import CollectionModel
+from embedin.repository.collection_repository import CollectionRepository
 
 
-class TestClient(unittest.TestCase):
+class TestCollectionRepository(TestCase):
     def setUp(self):
-        self.client = Client("test_collection")
+        self.session_mock = Mock()
+        self.repo = CollectionRepository(self.session_mock)
 
-    def test_create_or_get_collection(self):
+    def test_get_by_name(self):
+        # Mocking a CollectionModel object
+        collection = CollectionModel(id="123", name="test_collection")
+        self.session_mock.query.return_value.filter_by.return_value.first.return_value = (
+            collection
+        )
+
+        # Call the method and assert the result
+        result = self.repo.get_by_name("test_collection")
+        self.assertEqual(result, collection)
+
+        # Verify that the query was executed with the correct arguments
+        self.session_mock.query.assert_called_once_with(CollectionModel)
+        self.session_mock.query.return_value.filter_by.assert_called_once_with(
+            name="test_collection"
+        )
+        self.session_mock.query.return_value.filter_by.return_value.first.assert_called_once()
+
+    def test_create(self):
+        # call create method
         name = "test_collection"
-        collection_id = self.client.create_or_get_collection(name)
-        self.assertIsNotNone(collection_id)
-        self.assertEqual(self.client.collection_id, collection_id)
-
-    def test_create_collection(self):
-        # Test that a collection is created with the given name
-        name = "new_collection"
-        collection_id = self.client.create_collection(name)
-        self.assertIsNotNone(collection_id)
-        self.assertEqual(self.client.collection_id, collection_id)
-
-    def test_get_collection(self):
-        # Test that a collection is retrieved with the given name
-        collection_name = "new_collection"
-        self.client.create_collection(collection_name)
-        collection_id = self.client.get_collection(collection_name)
-        self.assertIsNotNone(collection_id)
-        self.assertEqual(self.client.collection_id, collection_id)
-
-    def test_add_data(self):
-        # Test that data is added to the collection
-        texts = ["text1", "text2"]
-        meta_data = [{"meta1": "value1"}, {"meta2": "value2"}]
-
-        self.client.embedding_fn = MagicMock(return_value=[[1, 2, 3], [4, 5, 6]])
-        self.client.add_data(texts, meta_data)
-
-        self.client.embedding_fn.assert_called_once_with(texts)
-        self.assertEqual(len(self.client.embedding_rows), 2)
-
-    def test_query(self):
-        # Test that queries return the expected results
-        self.client.embedding_fn = MagicMock(return_value=[[1, 2, 3], [4, 5, 6]])
-        self.client.add_data(["test", "text"])
-
-        self.client.embedding_fn = MagicMock(return_value=[[1, 2, 3]])
-        result = self.client.query("test", top_k=1)
-        expected_result = [{"text": "test", "meta_data": None}]
-        self.assertEqual(result, expected_result)
-
-    def tearDown(self):
-        # Clean up any resources created by the test
-        pass
 
+        # mock the get_by_name method
+        with patch.object(self.repo, "get_by_name", return_value=None):
+            collection = self.repo.create(name)
+            self.assertIsNotNone(collection)
+            self.assertEqual(collection.name, name)
+            self.assertIsInstance(collection.id, str)
+
+    def test_create_raise_exception(self):
+        # call create method
+        name = "test_collection"
+        # Mocking a CollectionModel object
+        mock_collection = CollectionModel(id="123", name=name)
+        with patch.object(self.repo, "get_by_name", return_value=mock_collection):
+            with self.assertRaises(ValueError):
+                self.repo.create(name, get_if_exist=False)
+
+    def test_create_already_exists(self):
+        # call create method
+        name = "test_collection"
 
-if __name__ == "__main__":
-    unittest.main()
+        # Mocking a CollectionModel object
+        mock_collection = CollectionModel(id="123", name=name)
+        with patch.object(self.repo, "get_by_name", return_value=mock_collection):
+            collection = self.repo.create(name)
+            self.assertIsNotNone(collection)
+            self.assertEqual(collection.name, mock_collection.name)
+            self.assertEqual(collection.id, mock_collection.id)
```

### Comparing `embedin-0.2.0/tests/embedding/__init__.py` & `embedin-0.2.1/tests/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/tests/embedding/test_openai_embedding.py` & `embedin-0.2.1/tests/embedding/test_openai_embedding.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/tests/embedding/test_sentence_transformer_embedding.py` & `embedin-0.2.1/tests/embedding/test_sentence_transformer_embedding.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/tests/index/__init__.py` & `embedin-0.2.1/tests/index/__init__.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/tests/index/test_flat_index.py` & `embedin-0.2.1/tests/index/test_flat_index.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/tests/index/test_hnsw_index.py` & `embedin-0.2.1/tests/index/test_hnsw_index.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/tests/model/test_collection_model.py` & `embedin-0.2.1/tests/model/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/tests/model/test_embedding_model.py` & `embedin-0.2.1/tests/model/test_embedding_model.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/tests/repository/test_embedding_repository.py` & `embedin-0.2.1/tests/repository/test_embedding_repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,66 @@
 
     def tearDown(self):
         self.session.rollback()
         # Close the session and drop the in-memory database after testing
         self.session.close()
         Base.metadata.drop_all(engine)
 
+    def test_add_rows_one_by_one(self):
+        self.assertEqual(len(self.session.query(EmbeddingModel).all()), 0)
+        self.repository._add_rows_one_by_one(self.embeddings)
+        self.assertEqual(len(self.session.query(EmbeddingModel).all()), 2)
+
+        self.assertEqual(
+            self.session.query(EmbeddingModel).filter_by(id="id1").first().text,
+            "some text",
+        )
+        self.assertEqual(
+            self.session.query(EmbeddingModel).filter_by(id="id2").first().text,
+            "some other text",
+        )
+
+    def test__add_rows_one_by_one(self):
+        self.repository.add_all(self.embeddings)
+        # Test adding duplicate embeddings
+        duplicate_embeddings = [
+            EmbeddingModel(
+                id="id3",
+                collection_id="collection1",
+                text="some text",
+                embedding_data=[1.0, 2.0, 3.0],
+                meta_data={"key1": "value1"},
+                hash="hash1",
+                created_at=datetime.now(),
+            ),
+            EmbeddingModel(
+                id="id4",
+                collection_id="collection1",
+                text="some new text",
+                embedding_data=[7.0, 8.0, 9.0],
+                meta_data={"key3": "value3"},
+                hash="hash4",
+                created_at=datetime.now(),
+            ),
+        ]
+        self.repository._add_rows_one_by_one(duplicate_embeddings)
+        self.assertEqual(len(self.session.query(EmbeddingModel).all()), 3)
+        self.assertEqual(
+            self.session.query(EmbeddingModel).filter_by(id="id1").first().text,
+            "some text",
+        )
+        self.assertEqual(
+            self.session.query(EmbeddingModel).filter_by(id="id2").first().text,
+            "some other text",
+        )
+        self.assertEqual(
+            self.session.query(EmbeddingModel).filter_by(id="id4").first().text,
+            "some new text",
+        )
+
     def test_add_all(self):
         self.assertEqual(len(self.session.query(EmbeddingModel).all()), 0)
         self.repository.add_all(self.embeddings)
         self.assertEqual(len(self.session.query(EmbeddingModel).all()), 2)
 
         self.assertEqual(
             self.session.query(EmbeddingModel).filter_by(id="id1").first().text,
```

### Comparing `embedin-0.2.0/tests/service/test_collection_service.py` & `embedin-0.2.1/tests/service/test_collection_service.py`

 * *Files identical despite different names*

### Comparing `embedin-0.2.0/tests/service/test_embedding_service.py` & `embedin-0.2.1/tests/service/test_embedding_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
         self.embedding_repo = EmbeddingRepository(self.session)
         self.collection_repo = CollectionRepository(self.session)
         self.service = EmbeddingService(self.session)
 
     def test_add_all(self):
         # Define mock data
         collection_id = "test_collection"
-        embeddings = [[1, 2, 3], [4, 5, 6]]
-        texts = ["test_text_1", "test_text_2"]
-        metadata_list = [{"meta1": "value1"}, {"meta2": "value2"}]
+        embeddings = [[1, 2, 3], [4, 5, 6], [1, 2, 3]]
+        texts = ["test_text_1", "test_text_2", "test_text_1"]
+        metadata_list = [{"meta1": "value1"}, {"meta2": "value2"}, {"meta1": "value1"}]
         expected_rows = [
             EmbeddingModel(
                 id="test_id_1",
                 collection_id=collection_id,
                 text=texts[0],
                 embedding_data=[1, 2, 3],
                 meta_data=metadata_list[0],
```

### Comparing `embedin-0.2.0/tests/util/__init__.py` & `embedin-0.2.1/tests/util/__init__.py`

 * *Files identical despite different names*

