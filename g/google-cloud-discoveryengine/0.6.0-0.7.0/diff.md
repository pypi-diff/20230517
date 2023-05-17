# Comparing `tmp/google-cloud-discoveryengine-0.6.0.tar.gz` & `tmp/google-cloud-discoveryengine-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-discoveryengine-0.6.0.tar", last modified: Thu May  4 17:24:58 2023, max compression
+gzip compressed data, was "google-cloud-discoveryengine-0.7.0.tar", last modified: Wed May 17 17:31:17 2023, max compression
```

## Comparing `google-cloud-discoveryengine-0.6.0.tar` & `google-cloud-discoveryengine-0.7.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.482420 google-cloud-discoveryengine-0.6.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4587 2023-05-04 17:24:58.482420 google-cloud-discoveryengine-0.6.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3663 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.462418 google-cloud-discoveryengine-0.6.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.462418 google-cloud-discoveryengine-0.6.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.462418 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/
--rw-rw-r--   0 root         (0)     1003     5697 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.466419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003     4372 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     9266 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.466419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.466419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17110 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26203 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.466419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6711 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13616 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13824 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22544 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.466419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47829 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58424 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py
--rw-rw-r--   0 root         (0)     1003     5921 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.470419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10042 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23048 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    59724 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.470419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/
--rw-rw-r--   0 root         (0)     1003      797 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17422 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27322 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.470419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6712 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13617 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13829 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22701 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.470419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    38222 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    48529 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
--rw-rw-r--   0 root         (0)     1003     5829 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.470419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8553 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18711 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19114 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    48576 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.474419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17633 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28264 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py
--rw-rw-r--   0 root         (0)     1003     5757 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.474419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6603 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13401 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13619 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22431 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.474419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27473 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37338 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.474419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8165 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17230 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17568 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    40240 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.478420 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     3197 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5368 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/common.py
--rw-rw-r--   0 root         (0)     1003     4646 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/completion_service.py
--rw-rw-r--   0 root         (0)     1003     6373 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/document.py
--rw-rw-r--   0 root         (0)     1003     9481 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/document_service.py
--rw-rw-r--   0 root         (0)     1003    18586 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/import_config.py
--rw-rw-r--   0 root         (0)     1003     4085 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/purge_config.py
--rw-rw-r--   0 root         (0)     1003    10788 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
--rw-rw-r--   0 root         (0)     1003     2396 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/schema.py
--rw-rw-r--   0 root         (0)     1003     9031 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/schema_service.py
--rw-rw-r--   0 root         (0)     1003    35635 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/search_service.py
--rw-rw-r--   0 root         (0)     1003    27718 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/user_event.py
--rw-rw-r--   0 root         (0)     1003     3436 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.478420 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/
--rw-r--r--   0 root         (0)     1003     4587 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     6181 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-05-04 17:24:58.482420 google-cloud-discoveryengine-0.6.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2956 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.478420 google-cloud-discoveryengine-0.6.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.478420 google-cloud-discoveryengine-0.6.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.478420 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.482420 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    83584 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
--rw-rw-r--   0 root         (0)     1003   201685 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
--rw-rw-r--   0 root         (0)     1003    86195 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
--rw-rw-r--   0 root         (0)     1003   168594 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
--rw-rw-r--   0 root         (0)     1003    93887 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
--rw-rw-r--   0 root         (0)     1003   119713 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.078381 google-cloud-discoveryengine-0.7.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4587 2023-05-17 17:31:17.074379 google-cloud-discoveryengine-0.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3663 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.058371 google-cloud-discoveryengine-0.7.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.058371 google-cloud-discoveryengine-0.7.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.062373 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine/
+-rw-rw-r--   0 root         (0)     1003     5697 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine/__init__.py
+-rw-rw-r--   0 root         (0)     1003      653 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.062373 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003     4372 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9266 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.062373 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.062373 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17110 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26203 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.062373 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6711 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13616 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13824 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22544 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.062373 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47829 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58424 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5921 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.066375 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10042 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22600 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23048 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    59724 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.066375 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/
+-rw-rw-r--   0 root         (0)     1003      797 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17422 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27322 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.066375 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6712 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13617 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13829 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22701 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.066375 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38222 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48529 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5829 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.066375 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8553 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18711 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19114 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    48576 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.066375 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17633 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28264 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5757 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.070377 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6603 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13401 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13619 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22431 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.070377 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27473 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37338 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.070377 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8165 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17230 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17568 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    40240 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.074379 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     3197 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5368 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/common.py
+-rw-rw-r--   0 root         (0)     1003     4646 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003     6373 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/document.py
+-rw-rw-r--   0 root         (0)     1003     9481 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/document_service.py
+-rw-rw-r--   0 root         (0)     1003    18586 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/import_config.py
+-rw-rw-r--   0 root         (0)     1003     4085 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/purge_config.py
+-rw-rw-r--   0 root         (0)     1003    10788 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003     2396 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     9031 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/schema_service.py
+-rw-rw-r--   0 root         (0)     1003    37478 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/search_service.py
+-rw-rw-r--   0 root         (0)     1003    27718 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/user_event.py
+-rw-rw-r--   0 root         (0)     1003     3436 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.074379 google-cloud-discoveryengine-0.7.0/google_cloud_discoveryengine.egg-info/
+-rw-r--r--   0 root         (0)     1003     4587 2023-05-17 17:31:17.000000 google-cloud-discoveryengine-0.7.0/google_cloud_discoveryengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     6181 2023-05-17 17:31:17.000000 google-cloud-discoveryengine-0.7.0/google_cloud_discoveryengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-17 17:31:17.000000 google-cloud-discoveryengine-0.7.0/google_cloud_discoveryengine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-17 17:31:17.000000 google-cloud-discoveryengine-0.7.0/google_cloud_discoveryengine.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-17 17:31:17.000000 google-cloud-discoveryengine-0.7.0/google_cloud_discoveryengine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-05-17 17:31:17.000000 google-cloud-discoveryengine-0.7.0/google_cloud_discoveryengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-17 17:31:17.000000 google-cloud-discoveryengine-0.7.0/google_cloud_discoveryengine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-05-17 17:31:17.078381 google-cloud-discoveryengine-0.7.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2956 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.074379 google-cloud-discoveryengine-0.7.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.074379 google-cloud-discoveryengine-0.7.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.074379 google-cloud-discoveryengine-0.7.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:17.074379 google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83584 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
+-rw-rw-r--   0 root         (0)     1003   201685 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
+-rw-rw-r--   0 root         (0)     1003    86195 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003   168594 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
+-rw-rw-r--   0 root         (0)     1003    93887 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
+-rw-rw-r--   0 root         (0)     1003   119713 2023-05-17 17:28:51.000000 google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
```

### Comparing `google-cloud-discoveryengine-0.6.0/LICENSE` & `google-cloud-discoveryengine-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/MANIFEST.in` & `google-cloud-discoveryengine-0.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/PKG-INFO` & `google-cloud-discoveryengine-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.6.0
+Version: 0.7.0
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.6.0/README.rst` & `google-cloud-discoveryengine-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/gapic_version.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.6.0"  # {x-release-please-version}
+__version__ = "0.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/gapic_version.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.6.0"  # {x-release-please-version}
+__version__ = "0.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/__init__.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/common.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/completion_service.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/document.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/document_service.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/import_config.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/import_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/purge_config.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/purge_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/schema.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/schema_service.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/search_service.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/search_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,18 @@
             ordered by a field in an
             [Document][google.cloud.discoveryengine.v1beta.Document]
             object. Leave it unset if ordered by relevance. OrderBy
             expression is case-sensitive.
 
             If this field is unrecognizable, an ``INVALID_ARGUMENT`` is
             returned.
+        user_info (google.cloud.discoveryengine_v1beta.types.UserInfo):
+            Information about the end user. Highly recommended for
+            analytics. The user_agent string in UserInfo will be used to
+            deduce device_type for analytics.
         facet_specs (MutableSequence[google.cloud.discoveryengine_v1beta.types.SearchRequest.FacetSpec]):
             Facet specifications for faceted search. If empty, no facets
             are returned.
 
             A maximum of 100 values are allowed. Otherwise, an
             ``INVALID_ARGUMENT`` error is returned.
         boost_spec (google.cloud.discoveryengine_v1beta.types.SearchRequest.BoostSpec):
@@ -116,15 +120,15 @@
 
             -  ``user_country_code``: string. Default empty. If set to
                non-empty, results are restricted or boosted based on the
                location provided.
             -  ``search_type``: double. Default empty. Enables
                non-webpage searching depending on the value. The only
                valid non-default value is 1, which enables image
-               searching. This field is ignored for other verticals.
+               searching.
         query_expansion_spec (google.cloud.discoveryengine_v1beta.types.SearchRequest.QueryExpansionSpec):
             The query expansion specification that
             specifies the conditions under which query
             expansion will occur.
         spell_correction_spec (google.cloud.discoveryengine_v1beta.types.SearchRequest.SpellCorrectionSpec):
             The spell correction specification that
             specifies the mode under which spell correction
@@ -146,14 +150,39 @@
 
             The field must be a UTF-8 encoded string with a length limit
             of 128 characters. Otherwise, an ``INVALID_ARGUMENT`` error
             is returned.
         content_search_spec (google.cloud.discoveryengine_v1beta.types.SearchRequest.ContentSearchSpec):
             The content search spec that configs the
             desired behavior of content search.
+        safe_search (bool):
+            Whether to turn on safe search. This is only supported for
+            [ContentConfig.PUBLIC_WEBSITE][].
+        user_labels (MutableMapping[str, str]):
+            The user labels applied to a resource must meet the
+            following requirements:
+
+            -  Each resource can have multiple labels, up to a maximum
+               of 64.
+            -  Each label must be a key-value pair.
+            -  Keys have a minimum length of 1 character and a maximum
+               length of 63 characters and cannot be empty. Values can
+               be empty and have a maximum length of 63 characters.
+            -  Keys and values can contain only lowercase letters,
+               numeric characters, underscores, and dashes. All
+               characters must use UTF-8 encoding, and international
+               characters are allowed.
+            -  The key portion of a label must be unique. However, you
+               can use the same key with multiple resources.
+            -  Keys must start with a lowercase letter or international
+               character.
+
+            See `Google Cloud
+            Document <https://cloud.google.com/resource-manager/docs/creating-managing-labels#requirements>`__
+            for more details.
     """
 
     class FacetSpec(proto.Message):
         r"""A facet specification to perform faceted search.
 
         Attributes:
             facet_key (google.cloud.discoveryengine_v1beta.types.SearchRequest.FacetSpec.FacetKey):
@@ -585,14 +614,19 @@
         proto.STRING,
         number=7,
     )
     order_by: str = proto.Field(
         proto.STRING,
         number=8,
     )
+    user_info: common.UserInfo = proto.Field(
+        proto.MESSAGE,
+        number=21,
+        message=common.UserInfo,
+    )
     facet_specs: MutableSequence[FacetSpec] = proto.RepeatedField(
         proto.MESSAGE,
         number=9,
         message=FacetSpec,
     )
     boost_spec: BoostSpec = proto.Field(
         proto.MESSAGE,
@@ -620,14 +654,23 @@
         number=15,
     )
     content_search_spec: ContentSearchSpec = proto.Field(
         proto.MESSAGE,
         number=24,
         message=ContentSearchSpec,
     )
+    safe_search: bool = proto.Field(
+        proto.BOOL,
+        number=20,
+    )
+    user_labels: MutableMapping[str, str] = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=22,
+    )
 
 
 class SearchResponse(proto.Message):
     r"""Response message for
     [SearchService.Search][google.cloud.discoveryengine.v1beta.SearchService.Search]
     method.
```

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/user_event.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/user_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py` & `google-cloud-discoveryengine-0.7.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/PKG-INFO` & `google-cloud-discoveryengine-0.7.0/google_cloud_discoveryengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.6.0
+Version: 0.7.0
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/SOURCES.txt` & `google-cloud-discoveryengine-0.7.0/google_cloud_discoveryengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/setup.py` & `google-cloud-discoveryengine-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/tests/__init__.py` & `google-cloud-discoveryengine-0.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/tests/unit/__init__.py` & `google-cloud-discoveryengine-0.7.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/__init__.py` & `google-cloud-discoveryengine-0.7.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py` & `google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py` & `google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py` & `google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py` & `google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py` & `google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py` & `google-cloud-discoveryengine-0.7.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py`

 * *Files identical despite different names*

