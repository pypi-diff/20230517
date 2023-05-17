# Comparing `tmp/manifest-ml-0.1.5.tar.gz` & `tmp/manifest-ml-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifest-ml-0.1.5.tar", last modified: Thu May  4 04:44:00 2023, max compression
+gzip compressed data, was "manifest-ml-0.1.6.tar", last modified: Wed May 17 05:54:31 2023, max compression
```

## Comparing `manifest-ml-0.1.5.tar` & `manifest-ml-0.1.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.204735 manifest-ml-0.1.5/
--rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/LICENSE
--rw-r--r--   0 laurelorr   (501) staff       (20)    10682 2023-05-04 04:44:00.204545 manifest-ml-0.1.5/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     9994 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/README.md
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.195734 manifest-ml-0.1.5/manifest/
--rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.5/manifest/__init__.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.196379 manifest-ml-0.1.5/manifest/api/
--rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/api/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     8947 2023-04-16 20:56:11.000000 manifest-ml-0.1.5/manifest/api/app.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.197708 manifest-ml-0.1.5/manifest/api/models/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/api/models/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4383 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/manifest/api/models/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    23121 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/manifest/api/models/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2798 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/manifest/api/models/model.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3880 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/manifest/api/models/sentence_transformer.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1767 2023-04-17 05:07:52.000000 manifest-ml-0.1.5/manifest/api/response.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.199231 manifest-ml-0.1.5/manifest/caches/
--rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/caches/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/caches/array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4386 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/caches/cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/caches/noop.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.5/manifest/caches/postgres.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/caches/redis.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5997 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/caches/serializers.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/caches/sqlite.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.201139 manifest-ml-0.1.5/manifest/clients/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/clients/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3303 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/ai21.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    14386 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/clients/client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3461 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/cohere.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2821 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5717 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/clients/dummy.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3751 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/clients/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2336 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/huggingface_embedding.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4810 2023-04-24 19:18:15.000000 manifest-ml-0.1.5/manifest/clients/openai.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5782 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/clients/openai_chat.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     6560 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/openai_embedding.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5164 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/toma.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1940 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/toma_diffuser.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.201639 manifest-ml-0.1.5/manifest/connections/
--rw-r--r--   0 laurelorr   (501) staff       (20)       23 2023-04-17 05:07:52.000000 manifest-ml-0.1.5/manifest/connections/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     6196 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/connections/client_pool.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1227 2023-05-03 06:44:32.000000 manifest-ml-0.1.5/manifest/connections/scheduler.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    22429 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3135 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    10950 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-05-01 03:31:34.000000 manifest-ml-0.1.5/manifest/version.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.202342 manifest-ml-0.1.5/manifest_ml.egg-info/
--rw-r--r--   0 laurelorr   (501) staff       (20)    10682 2023-05-04 04:43:59.000000 manifest-ml-0.1.5/manifest_ml.egg-info/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     1568 2023-05-04 04:44:00.000000 manifest-ml-0.1.5/manifest_ml.egg-info/SOURCES.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-05-04 04:43:59.000000 manifest-ml-0.1.5/manifest_ml.egg-info/dependency_links.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)     1615 2023-05-04 04:44:00.000000 manifest-ml-0.1.5/manifest_ml.egg-info/requires.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-05-04 04:44:00.000000 manifest-ml-0.1.5/manifest_ml.egg-info/top_level.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)      786 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/pyproject.toml
--rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-05-04 04:44:00.204777 manifest-ml-0.1.5/setup.cfg
--rw-r--r--   0 laurelorr   (501) staff       (20)     5349 2023-04-12 20:13:43.000000 manifest-ml-0.1.5/setup.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.203918 manifest-ml-0.1.5/tests/
--rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/tests/test_array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     8152 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/tests/test_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2446 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/tests/test_client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2304 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/tests/test_client_pool.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     9132 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/tests/test_huggingface_api.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    38750 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/tests/test_manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.5/tests/test_request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    10431 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/tests/test_response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      769 2023-05-03 06:44:15.000000 manifest-ml-0.1.5/tests/test_scheduler.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1073 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/tests/test_serializer.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.204337 manifest-ml-0.1.5/web_app/
--rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/web_app/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1737 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/web_app/main.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/web_app/schemas.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 05:54:31.270943 manifest-ml-0.1.6/
+-rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/LICENSE
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10728 2023-05-17 05:54:31.270710 manifest-ml-0.1.6/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10040 2023-05-17 05:53:01.000000 manifest-ml-0.1.6/README.md
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 05:54:31.264022 manifest-ml-0.1.6/manifest/
+-rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.6/manifest/__init__.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 05:54:31.264436 manifest-ml-0.1.6/manifest/api/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/manifest/api/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8947 2023-04-16 20:56:11.000000 manifest-ml-0.1.6/manifest/api/app.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 05:54:31.265349 manifest-ml-0.1.6/manifest/api/models/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/manifest/api/models/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4383 2023-04-09 06:56:02.000000 manifest-ml-0.1.6/manifest/api/models/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    23667 2023-05-17 05:53:01.000000 manifest-ml-0.1.6/manifest/api/models/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2798 2023-04-09 06:56:02.000000 manifest-ml-0.1.6/manifest/api/models/model.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3880 2023-04-09 06:56:02.000000 manifest-ml-0.1.6/manifest/api/models/sentence_transformer.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1767 2023-04-17 05:07:52.000000 manifest-ml-0.1.6/manifest/api/response.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 05:54:31.266295 manifest-ml-0.1.6/manifest/caches/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/manifest/caches/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/manifest/caches/array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4386 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/manifest/caches/cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/manifest/caches/noop.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.6/manifest/caches/postgres.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/manifest/caches/redis.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5997 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/manifest/caches/serializers.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/manifest/caches/sqlite.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 05:54:31.267772 manifest-ml-0.1.6/manifest/clients/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/manifest/clients/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3303 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/manifest/clients/ai21.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    14412 2023-05-17 05:53:01.000000 manifest-ml-0.1.6/manifest/clients/client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3461 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/manifest/clients/cohere.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2821 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/manifest/clients/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5717 2023-05-04 04:43:35.000000 manifest-ml-0.1.6/manifest/clients/dummy.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3751 2023-05-04 04:43:35.000000 manifest-ml-0.1.6/manifest/clients/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2336 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/manifest/clients/huggingface_embedding.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4810 2023-04-24 19:18:15.000000 manifest-ml-0.1.6/manifest/clients/openai.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5801 2023-05-17 05:53:01.000000 manifest-ml-0.1.6/manifest/clients/openai_chat.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6560 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/manifest/clients/openai_embedding.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5164 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/manifest/clients/toma.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1940 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/manifest/clients/toma_diffuser.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 05:54:31.268132 manifest-ml-0.1.6/manifest/connections/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       23 2023-04-17 05:07:52.000000 manifest-ml-0.1.6/manifest/connections/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6196 2023-05-04 04:43:35.000000 manifest-ml-0.1.6/manifest/connections/client_pool.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1227 2023-05-03 06:44:32.000000 manifest-ml-0.1.6/manifest/connections/scheduler.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    24977 2023-05-17 05:53:01.000000 manifest-ml-0.1.6/manifest/manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3135 2023-05-04 04:43:35.000000 manifest-ml-0.1.6/manifest/request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10950 2023-05-04 04:43:35.000000 manifest-ml-0.1.6/manifest/response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-05-17 05:54:28.000000 manifest-ml-0.1.6/manifest/version.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 05:54:31.268712 manifest-ml-0.1.6/manifest_ml.egg-info/
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10728 2023-05-17 05:54:31.000000 manifest-ml-0.1.6/manifest_ml.egg-info/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1568 2023-05-17 05:54:31.000000 manifest-ml-0.1.6/manifest_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-05-17 05:54:31.000000 manifest-ml-0.1.6/manifest_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1653 2023-05-17 05:54:31.000000 manifest-ml-0.1.6/manifest_ml.egg-info/requires.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-05-17 05:54:31.000000 manifest-ml-0.1.6/manifest_ml.egg-info/top_level.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)      802 2023-05-17 05:53:01.000000 manifest-ml-0.1.6/pyproject.toml
+-rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-05-17 05:54:31.270994 manifest-ml-0.1.6/setup.cfg
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5379 2023-05-17 05:53:01.000000 manifest-ml-0.1.6/setup.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 05:54:31.270170 manifest-ml-0.1.6/tests/
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/tests/test_array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8152 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/tests/test_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2446 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/tests/test_client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2304 2023-05-04 04:43:35.000000 manifest-ml-0.1.6/tests/test_client_pool.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     9132 2023-04-09 06:56:02.000000 manifest-ml-0.1.6/tests/test_huggingface_api.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    38821 2023-05-17 05:53:01.000000 manifest-ml-0.1.6/tests/test_manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.6/tests/test_request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10431 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/tests/test_response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      769 2023-05-03 06:44:15.000000 manifest-ml-0.1.6/tests/test_scheduler.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1073 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/tests/test_serializer.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 05:54:31.270515 manifest-ml-0.1.6/web_app/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/web_app/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1737 2023-04-24 18:36:42.000000 manifest-ml-0.1.6/web_app/main.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.6/web_app/schemas.py
```

### Comparing `manifest-ml-0.1.5/LICENSE` & `manifest-ml-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/PKG-INFO` & `manifest-ml-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifest-ml
-Version: 0.1.5
+Version: 0.1.6
 Summary: Manifest for Prompting Foundation Models.
 Home-page: https://github.com/HazyResearch/manifest
 Author: Laurel Orr
 Author-email: laurel.orr@numbersstation.ai
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -238,23 +238,23 @@
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
 # Chat Models
-Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, you must use the `run_chat` command with an associated chat model such as `openaichat`.
+Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, use the `run` command with a list of dictionary inputs with `role` and `content` keys using an associated chat model such as `openaichat`.
 
 ```python
 manifest = Manifest(client_name="openaichat")
 dialogue = [
     {"role": "system", "content": "You are a helpful assistant who also responds in rhymes"},
     {"role": "user", "content": "What is the date?"},
 ]
-res = manifest.run_chat(dialogue, max_tokens=100)
+res = manifest.run(dialogue, max_tokens=100)
 ```
 
 # Embedding Models
 Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
 
 To use OpenAI's embedding models, simply run
 ```python
```

### Comparing `manifest-ml-0.1.5/README.md` & `manifest-ml-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -214,23 +214,23 @@
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
 # Chat Models
-Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, you must use the `run_chat` command with an associated chat model such as `openaichat`.
+Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, use the `run` command with a list of dictionary inputs with `role` and `content` keys using an associated chat model such as `openaichat`.
 
 ```python
 manifest = Manifest(client_name="openaichat")
 dialogue = [
     {"role": "system", "content": "You are a helpful assistant who also responds in rhymes"},
     {"role": "user", "content": "What is the date?"},
 ]
-res = manifest.run_chat(dialogue, max_tokens=100)
+res = manifest.run(dialogue, max_tokens=100)
 ```
 
 # Embedding Models
 Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
 
 To use OpenAI's embedding models, simply run
 ```python
```

### Comparing `manifest-ml-0.1.5/manifest/api/app.py` & `manifest-ml-0.1.6/manifest/api/app.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/api/models/diffuser.py` & `manifest-ml-0.1.6/manifest/api/models/diffuser.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/api/models/huggingface.py` & `manifest-ml-0.1.6/manifest/api/models/huggingface.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     BloomForCausalLM,
     CLIPModel,
     CLIPProcessor,
     GPT2LMHeadModel,
     GPTJForCausalLM,
     GPTNeoForCausalLM,
     GPTNeoXForCausalLM,
+    LlamaForCausalLM,
+    LlamaTokenizer,
     OPTForCausalLM,
     PreTrainedModel,
     PreTrainedTokenizer,
 )
 
 import deepspeed
 from manifest.api.models.model import Model
@@ -44,14 +46,15 @@
     "facebook/opt-30b": OPTForCausalLM,
     "gpt2": GPT2LMHeadModel,
     "openai/clip-vit-base-patch32": CLIPModel,
     "bigscience/bloom-560m": BloomForCausalLM,
     "bigscience/bloom-1b7": BloomForCausalLM,
     "bigscience/bloom-3b": BloomForCausalLM,
     "bigscience/bloom-7b1": BloomForCausalLM,
+    "chainyo/alpaca-lora-7b": LlamaForCausalLM,
     "bigscience/bloom": AutoModelForCausalLM,
     "bigscience/T0pp": AutoModelForSeq2SeqLM,
     "bigscience/T0_3B": AutoModelForSeq2SeqLM,
     "google/t5-small-lm-adapt": AutoModelForSeq2SeqLM,  # 220M
     "google/t5-l-lm-adapt": AutoModelForSeq2SeqLM,  # 800M
     "google/t5-xl-lm-adapt": AutoModelForSeq2SeqLM,  # 3B
     "google/t5-xxl-lm-adapt": AutoModelForSeq2SeqLM,  # 11B
@@ -61,14 +64,15 @@
     "google/flan-t5-l": AutoModelForSeq2SeqLM,  # 800M
     "google/flan-t5-xl": AutoModelForSeq2SeqLM,  # 3B
     "google/flan-t5-xxl": AutoModelForSeq2SeqLM,  # 11B
 }
 
 MODEL_GENTYPE_REGISTRY = {
     "text-generation": AutoModelForCausalLM,
+    "llama-text-generation": LlamaForCausalLM,
     "text2text-generation": AutoModelForSeq2SeqLM,
 }
 
 
 def get_max_memory(gpu_reduction: float) -> Dict[int, str]:
     """Get max memory in GB times reduction."""
     free_in_gb = int(torch.cuda.mem_get_info()[0] / 1024**3)  # type: ignore
@@ -148,25 +152,28 @@
             text,
             max_length=max_input_len,
             truncation=True,
             padding=True,
             return_tensors="pt",
         )
         encoded_prompt = encoded_prompt.to(self.device)
+        kwargs_to_pass = dict(
+            temperature=kwargs.get("temperature"),
+            top_k=kwargs.get("top_k"),
+            top_p=kwargs.get("top_p"),
+            repetition_penalty=kwargs.get("repetition_penalty"),
+            num_return_sequences=kwargs.get("num_return_sequences"),
+        )
+        kwargs_to_pass = {k: v for k, v in kwargs_to_pass.items() if v is not None}
         output_dict = self.model.generate(  # type: ignore
             **encoded_prompt,
+            **kwargs_to_pass,
             max_new_tokens=kwargs.get("max_new_tokens"),
-            temperature=kwargs.get("temperature", None),
-            top_k=kwargs.get("top_k", None),
-            top_p=kwargs.get("top_p", None),
-            repetition_penalty=kwargs.get("repetition_penalty", None),
-            do_sample=kwargs.get("do_sample", None) if not self.bitsandbytes else False,
             eos_token_id=self.tokenizer.eos_token_id,
             pad_token_id=self.tokenizer.pad_token_id,
-            num_return_sequences=kwargs.get("num_return_sequences", None),
             output_scores=True,
             return_dict_in_generate=True,
         )
         # logits/scores from the output always correspond to the generated tokens.
         # shape (num_tokens, num_return_sequences, vocab_size)
         logits = torch.stack(output_dict.scores)
         logits = torch.nn.functional.log_softmax(logits, dim=-1)
@@ -454,25 +461,33 @@
             use_accelerate,
             use_parallelize,
             use_bitsandbytes,
             use_deepspeed,
             perc_max_gpu_mem_red,
             use_fp16,
         )
-        try:
-            tokenizer = AutoTokenizer.from_pretrained(
-                self.model_name, truncation_side="left", padding_side="left"
-            )
-        except ValueError:
-            tokenizer = AutoTokenizer.from_pretrained(
-                self.model_name,
-                truncation_side="left",
-                padding_side="left",
-                use_fast=False,
+        if (
+            MODEL_REGISTRY.get(
+                self.model_name, MODEL_GENTYPE_REGISTRY.get(self.model_type, None)
             )
+            == LlamaForCausalLM
+        ):
+            tokenizer = LlamaTokenizer.from_pretrained(self.model_name)
+        else:
+            try:
+                tokenizer = AutoTokenizer.from_pretrained(
+                    self.model_name, truncation_side="left", padding_side="left"
+                )
+            except ValueError:
+                tokenizer = AutoTokenizer.from_pretrained(
+                    self.model_name,
+                    truncation_side="left",
+                    padding_side="left",
+                    use_fast=False,
+                )
         dtype = torch.float16 if use_fp16 else "auto"
         if use_bitsandbytes:
             print("WARNING!!! Cannot use sampling with bitsandbytes.")
             max_memory = get_max_memory(perc_max_gpu_mem_red)
             model = MODEL_REGISTRY.get(
                 self.model_name, MODEL_GENTYPE_REGISTRY.get(self.model_type, None)
             ).from_pretrained(  # type: ignore
@@ -497,19 +512,18 @@
                 model = MODEL_REGISTRY.get(
                     self.model_name, MODEL_GENTYPE_REGISTRY.get(self.model_type, None)
                 ).from_pretrained(  # type: ignore
                     self.model_path, cache_dir=cache_dir, torch_dtype=dtype
                 )
         model.eval()
         print(f"Loaded Model DType {model.dtype}")
-
         self.is_encdec = model.config.is_encoder_decoder
         if not self.is_encdec:
             tokenizer.pad_token = tokenizer.eos_token
-
+            tokenizer.pad_token_id = tokenizer.eos_token_id
         if not use_bitsandbytes:
             if use_accelerate:
                 self._dispatch_accelerate_model(model, perc_max_gpu_mem_red)
                 device = 0
             elif use_parallelize:
                 model.parallelize()
                 device = 0
```

### Comparing `manifest-ml-0.1.5/manifest/api/models/model.py` & `manifest-ml-0.1.6/manifest/api/models/model.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/api/models/sentence_transformer.py` & `manifest-ml-0.1.6/manifest/api/models/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/api/response.py` & `manifest-ml-0.1.6/manifest/api/response.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/caches/array_cache.py` & `manifest-ml-0.1.6/manifest/caches/array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/caches/cache.py` & `manifest-ml-0.1.6/manifest/caches/cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/caches/noop.py` & `manifest-ml-0.1.6/manifest/caches/noop.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/caches/postgres.py` & `manifest-ml-0.1.6/manifest/caches/postgres.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/caches/redis.py` & `manifest-ml-0.1.6/manifest/caches/redis.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/caches/serializers.py` & `manifest-ml-0.1.6/manifest/caches/serializers.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/caches/sqlite.py` & `manifest-ml-0.1.6/manifest/caches/sqlite.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/clients/ai21.py` & `manifest-ml-0.1.6/manifest/clients/ai21.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/clients/client.py` & `manifest-ml-0.1.6/manifest/clients/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 class Client(ABC):
     """Client class."""
 
     # Must be overridden by child class
     PARAMS: Dict[str, Tuple[str, Any]] = {}
     REQUEST_CLS = Request
     NAME: str = None
+    IS_CHAT: bool = False
 
     def __init__(
         self, connection_str: Optional[str] = None, client_args: Dict[str, Any] = {}
     ):
         """
         Initialize client.
```

### Comparing `manifest-ml-0.1.5/manifest/clients/cohere.py` & `manifest-ml-0.1.6/manifest/clients/cohere.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/clients/diffuser.py` & `manifest-ml-0.1.6/manifest/clients/diffuser.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/clients/dummy.py` & `manifest-ml-0.1.6/manifest/clients/dummy.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/clients/huggingface.py` & `manifest-ml-0.1.6/manifest/clients/huggingface.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/clients/huggingface_embedding.py` & `manifest-ml-0.1.6/manifest/clients/huggingface_embedding.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/clients/openai.py` & `manifest-ml-0.1.6/manifest/clients/openai.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/clients/openai_chat.py` & `manifest-ml-0.1.6/manifest/clients/openai_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         "top_p": ("top_p", 1.0),
         "stop_sequences": ("stop", None),  # OpenAI doesn't like empty lists
         "presence_penalty": ("presence_penalty", 0.0),
         "frequency_penalty": ("frequency_penalty", 0.0),
     }
     REQUEST_CLS = LMRequest
     NAME = "openaichat"
+    IS_CHAT = True
 
     def connect(
         self,
         connection_str: Optional[str] = None,
         client_args: Dict[str, Any] = {},
     ) -> None:
         """
```

### Comparing `manifest-ml-0.1.5/manifest/clients/openai_embedding.py` & `manifest-ml-0.1.6/manifest/clients/openai_embedding.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/clients/toma.py` & `manifest-ml-0.1.6/manifest/clients/toma.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/clients/toma_diffuser.py` & `manifest-ml-0.1.6/manifest/clients/toma_diffuser.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/connections/client_pool.py` & `manifest-ml-0.1.6/manifest/connections/client_pool.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/connections/scheduler.py` & `manifest-ml-0.1.6/manifest/connections/scheduler.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/manifest.py` & `manifest-ml-0.1.6/manifest/manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -283,37 +283,98 @@
             response_type=response_type,
             request_type=request_type,
         )
         return response_obj
 
     def run(
         self,
-        prompt: Union[str, List[str]],
+        prompt: Union[str, List[str], List[Dict[str, str]]],
         overwrite_cache: bool = False,
         stop_token: Optional[str] = None,
         return_response: bool = False,
         **kwargs: Any,
     ) -> Union[str, List[str], np.ndarray, List[np.ndarray], Response]:
         """
         Run the prompt.
 
+        Orchestrates between the standard run and chat run and batch run.
+
         Args:
             prompt: prompt(s) to run.
             overwrite_cache: whether to overwrite cache.
             stop_token: stop token for prompt generation.
                         Default is self.stop_token.
                         "" for no stop token.
             return_response: whether to return Response object.
 
         Returns:
             response from prompt.
         """
-        is_batch = isinstance(prompt, list)
+        if not isinstance(prompt, list) and not isinstance(prompt, str):
+            raise ValueError(
+                f"Invalid prompt type: {type(prompt)}. "
+                "Prompt must be a string or list of strings "
+                "or list of dicts."
+            )
+        if isinstance(prompt, list) and not prompt:
+            raise ValueError("Prompt cannot be empty list")
         # Get the client to run
         client = self.client_pool.get_next_client()
+        if isinstance(prompt, list) and isinstance(prompt[0], dict):
+            if not client.IS_CHAT:
+                raise ValueError(
+                    f"Client {client} does not support dict chat prompt. "
+                    "Please use a chat model."
+                )
+            if stop_token:
+                logger.warning(
+                    "stop_token is not supported for chat prompt. "
+                    "Ignoring stop_token."
+                )
+            return self._run_chat(
+                prompt=cast(List[Dict[str, str]], prompt),
+                client=client,
+                overwrite_cache=overwrite_cache,
+                return_response=return_response,
+            )
+        else:
+            return self._run(
+                prompt=cast(Union[str, List[str]], prompt),
+                client=client,
+                overwrite_cache=overwrite_cache,
+                stop_token=stop_token,
+                return_response=return_response,
+                **kwargs,
+            )
+
+    def _run(
+        self,
+        prompt: Union[str, List[str]],
+        client: Client,
+        overwrite_cache: bool = False,
+        stop_token: Optional[str] = None,
+        return_response: bool = False,
+        **kwargs: Any,
+    ) -> Union[str, List[str], np.ndarray, List[np.ndarray], Response]:
+        """
+        Run the prompt.
+
+        Args:
+            prompt: prompt(s) to run.
+            client: client to run.
+            overwrite_cache: whether to overwrite cache.
+            stop_token: stop token for prompt generation.
+                        Default is self.stop_token.
+                        "" for no stop token.
+            return_response: whether to return Response object.
+
+        Returns:
+            response from prompt.
+        """
+        is_batch = isinstance(prompt, list)
         stop_token = stop_token if stop_token is not None else self.stop_token
         # Must pass kwargs as dict for client "pop" methods removed used arguments
         request_params = client.get_request(prompt, kwargs)
         # Avoid nested list of results - enforce n = 1 for batch
         if is_batch and request_params.n > 1:
             raise ValueError("Batch mode does not support n > 1.")
         self._validate_kwargs(kwargs, request_params)
@@ -340,14 +401,75 @@
 
         # Extract text results
         if return_response:
             return final_response
         else:
             return final_response.get_response(stop_token, is_batch)
 
+    def _run_chat(
+        self,
+        prompt: List[Dict[str, str]],
+        client: Client,
+        overwrite_cache: bool = False,
+        return_response: bool = False,
+        **kwargs: Any,
+    ) -> Union[str, Response]:
+        """
+        Run the prompt.
+
+        Args:
+            prompt: prompt dictionary to run.
+            client: client to run.
+            overwrite_cache: whether to overwrite cache.
+            stop_token: stop token for prompt generation.
+                        Default is self.stop_token.
+                        "" for no stop token.
+            return_response: whether to return Response object.
+
+        Returns:
+            response from prompt.
+        """
+        is_batch = False
+        # Get a request for an empty prompt to handle all kwargs
+        request_params = client.get_request("", kwargs)
+        # Add prompt and cast as chat request
+        request_params_dict = request_params.to_dict()
+        request_params_dict["prompt"] = prompt
+        request_params_as_chat = LMChatRequest(**request_params_dict)
+        # Avoid nested list of results - enforce n = 1 for batch
+        if request_params_as_chat.n > 1:
+            raise ValueError("Chat mode does not support n > 1.")
+        self._validate_kwargs(kwargs, request_params_as_chat)
+
+        cached_idx_to_response, request_params_as_chat = self._split_cached_requests(  # type: ignore # noqa: E501
+            request_params_as_chat, client, overwrite_cache
+        )
+        # If not None value or empty list - run new request
+        if request_params_as_chat.prompt:
+            # Start timing metrics
+            self.client_pool.start_timer()
+            response = client.run_chat_request(request_params_as_chat)
+            self.client_pool.end_timer()
+        else:
+            # Nothing to run
+            response = None
+
+        final_response = self._stitch_responses_and_cache(
+            request=request_params_as_chat,
+            client=client,
+            response=response,
+            cached_idx_to_response=cached_idx_to_response,
+        )
+
+        # Extract text results
+        if return_response:
+            return final_response
+        else:
+            return cast(str, final_response.get_response("", is_batch))
+
     async def arun_batch(
         self,
         prompts: List[str],
         overwrite_cache: bool = False,
         stop_token: Optional[str] = None,
         return_response: bool = False,
         chunk_size: int = -1,
@@ -377,14 +499,21 @@
                 For a single manifest client, there is no impact to
                 setting chunk_size. For a client pool, chunk_size
                 can be used to distribute the load across the clients.
 
         Returns:
             response from prompt.
         """
+        if not isinstance(prompts, list):
+            raise ValueError("Prompts must be a list of strings.")
+        if not prompts:
+            raise ValueError("Prompts must not be empty.")
+        if not isinstance(prompts[0], str):
+            raise ValueError("Prompts must be a list of strings.")
+
         # Split the prompts into chunks
         prompt_chunks: List[Tuple[Client, List[str]]] = []
         if chunk_size > 0:
             for i in range(0, len(prompts), chunk_size):
                 prompt_chunks.append(
                     (self.client_pool.get_next_client(), prompts[i : i + chunk_size])
                 )
@@ -460,75 +589,14 @@
             request=request_params,
             client=client,
             response=response,
             cached_idx_to_response=cached_idx_to_response,
         )
         return final_response
 
-    def run_chat(
-        self,
-        prompt: List[Dict[str, str]],
-        overwrite_cache: bool = False,
-        return_response: bool = False,
-        **kwargs: Any,
-    ) -> Union[str, Response]:
-        """
-        Run the prompt.
-
-        Args:
-            prompt: prompt dictionary to run.
-            overwrite_cache: whether to overwrite cache.
-            stop_token: stop token for prompt generation.
-                        Default is self.stop_token.
-                        "" for no stop token.
-            return_response: whether to return Response object.
-
-        Returns:
-            response from prompt.
-        """
-        is_batch = False
-        # Get the client to run
-        client = self.client_pool.get_next_client()
-        # Get a request for an empty prompt to handle all kwargs
-        request_params = client.get_request("", kwargs)
-        # Add prompt and cast as chat request
-        request_params_dict = request_params.to_dict()
-        request_params_dict["prompt"] = prompt
-        request_params_as_chat = LMChatRequest(**request_params_dict)
-        # Avoid nested list of results - enforce n = 1 for batch
-        if request_params_as_chat.n > 1:
-            raise ValueError("Chat mode does not support n > 1.")
-        self._validate_kwargs(kwargs, request_params_as_chat)
-
-        cached_idx_to_response, request_params_as_chat = self._split_cached_requests(  # type: ignore # noqa: E501
-            request_params_as_chat, client, overwrite_cache
-        )
-        # If not None value or empty list - run new request
-        if request_params_as_chat.prompt:
-            # Start timing metrics
-            self.client_pool.start_timer()
-            response = client.run_chat_request(request_params_as_chat)
-            self.client_pool.end_timer()
-        else:
-            # Nothing to run
-            response = None
-
-        final_response = self._stitch_responses_and_cache(
-            request=request_params_as_chat,
-            client=client,
-            response=response,
-            cached_idx_to_response=cached_idx_to_response,
-        )
-
-        # Extract text results
-        if return_response:
-            return final_response
-        else:
-            return cast(str, final_response.get_response("", is_batch))
-
     def score_prompt(
         self,
         prompt: Union[str, List[str]],
         overwrite_cache: bool = False,
         **kwargs: Any,
     ) -> Dict:
         """
```

### Comparing `manifest-ml-0.1.5/manifest/request.py` & `manifest-ml-0.1.6/manifest/request.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest/response.py` & `manifest-ml-0.1.6/manifest/response.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest_ml.egg-info/PKG-INFO` & `manifest-ml-0.1.6/manifest_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifest-ml
-Version: 0.1.5
+Version: 0.1.6
 Summary: Manifest for Prompting Foundation Models.
 Home-page: https://github.com/HazyResearch/manifest
 Author: Laurel Orr
 Author-email: laurel.orr@numbersstation.ai
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -238,23 +238,23 @@
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
 # Chat Models
-Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, you must use the `run_chat` command with an associated chat model such as `openaichat`.
+Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, use the `run` command with a list of dictionary inputs with `role` and `content` keys using an associated chat model such as `openaichat`.
 
 ```python
 manifest = Manifest(client_name="openaichat")
 dialogue = [
     {"role": "system", "content": "You are a helpful assistant who also responds in rhymes"},
     {"role": "user", "content": "What is the date?"},
 ]
-res = manifest.run_chat(dialogue, max_tokens=100)
+res = manifest.run(dialogue, max_tokens=100)
 ```
 
 # Embedding Models
 Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
 
 To use OpenAI's embedding models, simply run
 ```python
```

### Comparing `manifest-ml-0.1.5/manifest_ml.egg-info/SOURCES.txt` & `manifest-ml-0.1.6/manifest_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/manifest_ml.egg-info/requires.txt` & `manifest-ml-0.1.6/manifest_ml.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,61 +5,63 @@
 aiohttp>=3.8.0
 sqlitedict>=2.0.0
 tenacity>=8.2.0
 tiktoken>=0.3.0
 xxhash>=3.0.0
 
 [all]
-deepspeed>=0.7.0
-pre-commit>=2.14.0
+accelerate>=0.10.0
 fastapi>=0.70.0
-sqlalchemy
-uvicorn>=0.18.0
-transformers<4.26.0,>=4.20.0
-diffusers>=0.6.0
+torch>=1.8.0
 types-PyYAML>=6.0.7
-types-redis>=4.2.6
+black>=22.3.0
+pg8000
+diffusers>=0.6.0
+sentence_transformers>=2.2.0
+deepspeed>=0.7.0
+cloud-sql-python-connector[pg8000]>=1.0.0
+sqlalchemy
+pytest>=7.0.0
+pytest-cov>=3.0.0
 pillow>=9.0.0
-docformatter>=1.4
-types-python-dateutil>=2.8.16
-python-dotenv>=0.20.0
-flake8>=4.0.0
-torch>=1.8.0
-types-protobuf>=3.19.21
+types-requests>=2.27.29
+uvicorn>=0.18.0
+isort>=5.9.3
 sphinx-autobuild
+mypy>=0.950
 sphinx-rtd-theme>=0.5.1
+types-redis>=4.2.6
+flake8>=4.0.0
 nbsphinx>=0.8.0
-black>=22.3.0
-recommonmark>=0.7.1
-types-xxhash>=3.0.0
-types-pillow>=9.0.0
+twine
 Flask>=2.1.2
-cloud-sql-python-connector[pg8000]>=1.0.0
-types-requests>=2.27.29
-sentence_transformers>=2.2.0
-isort>=5.9.3
+types-setuptools>=57.4.17
+types-xxhash>=3.0.0
+autopep8>=1.6.0
 flake8-docstrings>=1.6.0
-pytest>=7.0.0
+types-pillow>=9.0.0
+types-python-dateutil>=2.8.16
+python-dotenv>=0.20.0
+transformers<4.31.0,>=4.29.0
+pre-commit>=2.14.0
+types-protobuf>=3.19.21
+docformatter>=1.4
+recommonmark>=0.7.1
 pep8-naming>=0.12.1
-autopep8>=1.6.0
-pytest-cov>=3.0.0
-accelerate>=0.10.0
-types-setuptools>=57.4.17
-mypy>=0.950
-twine
-pg8000
+tokenizers>=0.13.3
 
 [api]
 accelerate>=0.10.0
 deepspeed>=0.7.0
 diffusers>=0.6.0
 Flask>=2.1.2
 sentence_transformers>=2.2.0
 torch>=1.8.0
-transformers<4.26.0,>=4.20.0
+transformers<4.31.0,>=4.29.0
+tokenizers>=0.13.3
 
 [app]
 fastapi>=0.70.0
 uvicorn>=0.18.0
 
 [dev]
 autopep8>=1.6.0
```

### Comparing `manifest-ml-0.1.5/pyproject.toml` & `manifest-ml-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ignore_missing_imports = true
 module = [
   "deepspeed",
   "numpy",
   "diffusers",
   "sentence_transformers",
   "sqlitedict",
+  "sqlalchemy",
   "dill",
   "accelerate",
   "accelerate.utils.modeling",
   "transformers",
   "flask",
   "torch",
   "pyChatGPT",
```

### Comparing `manifest-ml-0.1.5/setup.py` & `manifest-ml-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     "api": [
         "accelerate>=0.10.0",
         "deepspeed>=0.7.0",
         "diffusers>=0.6.0",
         "Flask>=2.1.2",
         "sentence_transformers>=2.2.0",
         "torch>=1.8.0",
-        "transformers>=4.20.0,<4.26.0",
+        "transformers>=4.29.0,<4.31.0",
+        "tokenizers>=0.13.3",
     ],
     "app": [
         "fastapi>=0.70.0",
         "uvicorn>=0.18.0",
     ],
     "diffusers": [
         "pillow>=9.0.0",
```

### Comparing `manifest-ml-0.1.5/tests/test_array_cache.py` & `manifest-ml-0.1.6/tests/test_array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/tests/test_cache.py` & `manifest-ml-0.1.6/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/tests/test_client.py` & `manifest-ml-0.1.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/tests/test_client_pool.py` & `manifest-ml-0.1.6/tests/test_client_pool.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/tests/test_huggingface_api.py` & `manifest-ml-0.1.6/tests/test_huggingface_api.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/tests/test_manifest.py` & `manifest-ml-0.1.6/tests/test_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,19 +395,21 @@
 def test_run_chat(sqlite_cache: str) -> None:
     """Test manifest run."""
     manifest = Manifest(
         client_name="dummy",
         cache_name="sqlite",
         cache_connection=sqlite_cache,
     )
+    # Set CHAT to be true for this model
+    manifest.client_pool.client_pool[0].IS_CHAT = True
 
     prompt = [
         {"role": "system", "content": "Hello."},
     ]
-    result = manifest.run_chat(prompt, return_response=False)
+    result = manifest.run(prompt, return_response=False)
     assert result == "Hello."
     assert (
         manifest.cache.get(
             {
                 "prompt": [{"content": "Hello.", "role": "system"}],
                 "engine": "dummy",
                 "num_results": 1,
@@ -417,15 +419,15 @@
         is not None
     )
 
     prompt = [
         {"role": "system", "content": "Hello."},
         {"role": "user", "content": "Goodbye?"},
     ]
-    result = manifest.run_chat(prompt, return_response=True)
+    result = manifest.run(prompt, return_response=True)
     assert isinstance(result, Response)
     result = cast(Response, result)
     assert len(result.get_usage_obj().usages) == len(result.get_response_obj().choices)
     res = result.get_response()
     assert res == "Hello."
     assert (
         manifest.cache.get(
@@ -845,29 +847,29 @@
         {"role": "user", "content": "Who won the world series in 2020?"},
         {
             "role": "assistant",
             "content": "The Los Angeles Dodgers won the World Series in 2020.",
         },
         {"role": "user", "content": "Where was it played?"},
     ]
-    res = client.run_chat(chat_dict)
+    res = client.run(chat_dict)
     assert isinstance(res, str) and len(res) > 0
-    response = cast(Response, client.run_chat(chat_dict, return_response=True))
+    response = cast(Response, client.run(chat_dict, return_response=True))
     assert response.is_cached() is True
     assert response.get_usage_obj().usages[0].total_tokens == 67
     chat_dict = [
         {"role": "system", "content": "You are a helpful assistanttttt."},
         {"role": "user", "content": "Who won the world series in 2020?"},
         {
             "role": "assistant",
             "content": "The Los Angeles Dodgers won the World Series in 2020.",
         },
         {"role": "user", "content": "Where was it played?"},
     ]
-    response = cast(Response, client.run_chat(chat_dict, return_response=True))
+    response = cast(Response, client.run(chat_dict, return_response=True))
     assert response.is_cached() is False
 
 
 @pytest.mark.skipif(not OPENAI_ALIVE, reason="No openai key set")
 @pytest.mark.usefixtures("sqlite_cache")
 def test_openaiembedding(sqlite_cache: str) -> None:
     """Test openaichat client."""
```

### Comparing `manifest-ml-0.1.5/tests/test_request.py` & `manifest-ml-0.1.6/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/tests/test_response.py` & `manifest-ml-0.1.6/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/tests/test_scheduler.py` & `manifest-ml-0.1.6/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/tests/test_serializer.py` & `manifest-ml-0.1.6/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/web_app/main.py` & `manifest-ml-0.1.6/web_app/main.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.5/web_app/schemas.py` & `manifest-ml-0.1.6/web_app/schemas.py`

 * *Files identical despite different names*

