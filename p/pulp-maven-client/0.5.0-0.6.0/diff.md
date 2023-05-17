# Comparing `tmp/pulp_maven-client-0.5.0.tar.gz` & `tmp/pulp_maven-client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_maven-client-0.5.0.tar", last modified: Fri Mar 17 10:20:09 2023, max compression
+gzip compressed data, was "pulp_maven-client-0.6.0.tar", last modified: Wed May 17 14:27:59 2023, max compression
```

## Comparing `pulp_maven-client-0.5.0.tar` & `pulp_maven-client-0.6.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:20:09.494586 pulp_maven-client-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-17 10:20:09.494586 pulp_maven-client-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:20:09.486586 pulp_maven-client-0.5.0/pulp_maven_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-17 10:20:09.000000 pulp_maven-client-0.5.0/pulp_maven_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-17 10:20:09.000000 pulp_maven-client-0.5.0/pulp_maven_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 10:20:09.000000 pulp_maven-client-0.5.0/pulp_maven_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-17 10:20:09.000000 pulp_maven-client-0.5.0/pulp_maven_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-17 10:20:09.000000 pulp_maven-client-0.5.0/pulp_maven_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:20:09.486586 pulp_maven-client-0.5.0/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:20:09.486586 pulp_maven-client-0.5.0/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:20:09.486586 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:20:09.486586 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21566 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/content_artifact_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/distributions_maven_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/pulp_maven_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42083 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/remotes_maven_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/repositories_maven_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32383 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/repositories_maven_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26284 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:20:09.490586 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_artifact_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    26038 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_artifact_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26347 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/repository_add_cached_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-17 10:20:09.494586 pulp_maven-client-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:20:09.494586 pulp_maven-client-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/test/test_content_artifact_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/test/test_distributions_maven_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_maven_maven_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_maven_maven_artifact_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_maven_maven_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_maven_maven_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_maven_maven_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_maven_maven_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_maven_maven_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_maven_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_maven_maven_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_paginatedmaven_maven_artifact_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_paginatedmaven_maven_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_paginatedmaven_maven_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_paginatedmaven_maven_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_patchedmaven_maven_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_patchedmaven_maven_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_patchedmaven_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/test/test_pulp_maven_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/test/test_remotes_maven_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/test/test_repositories_maven_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-17 10:20:08.000000 pulp_maven-client-0.5.0/test/test_repositories_maven_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_repository_add_cached_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-03-17 10:20:07.000000 pulp_maven-client-0.5.0/test/test_repository_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:27:59.091861 pulp_maven-client-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-17 14:27:59.091861 pulp_maven-client-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:27:59.083861 pulp_maven-client-0.6.0/pulp_maven_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulp_maven_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-17 14:27:59.000000 pulp_maven-client-0.6.0/pulp_maven_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulp_maven_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulp_maven_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulp_maven_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:27:59.083861 pulp_maven-client-0.6.0/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:27:59.083861 pulp_maven-client-0.6.0/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:27:59.083861 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:27:59.087861 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24074 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/content_artifact_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44907 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/distributions_maven_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/pulp_maven_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46819 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/remotes_maven_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54073 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/repositories_maven_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33732 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/repositories_maven_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26284 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:27:59.087861 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_artifact_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23603 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_artifact_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26625 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/repository_add_cached_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 14:27:59.091861 pulp_maven-client-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:27:59.091861 pulp_maven-client-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_content_artifact_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_distributions_maven_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_maven_maven_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_maven_maven_artifact_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_maven_maven_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_maven_maven_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_maven_maven_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_maven_maven_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_maven_maven_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_maven_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_maven_maven_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_paginatedmaven_maven_artifact_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_paginatedmaven_maven_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_paginatedmaven_maven_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_paginatedmaven_maven_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_patchedmaven_maven_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_patchedmaven_maven_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_patchedmaven_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/test/test_pulp_maven_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/test/test_remotes_maven_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/test/test_repositories_maven_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-17 14:27:58.000000 pulp_maven-client-0.6.0/test/test_repositories_maven_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_repository_add_cached_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-17 14:27:57.000000 pulp_maven-client-0.6.0/test/test_repository_version_response.py
```

### Comparing `pulp_maven-client-0.5.0/README.md` & `pulp_maven-client-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_maven-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 0.5.0
+- Package version: 0.6.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_maven-client-0.5.0/pulp_maven_client.egg-info/SOURCES.txt` & `pulp_maven-client-0.6.0/pulp_maven_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/__init__.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 # import apis into sdk package
 from pulpcore.client.pulp_maven.api.content_artifact_api import ContentArtifactApi
 from pulpcore.client.pulp_maven.api.distributions_maven_api import DistributionsMavenApi
 from pulpcore.client.pulp_maven.api.pulp_maven_api import PulpMavenApi
 from pulpcore.client.pulp_maven.api.remotes_maven_api import RemotesMavenApi
 from pulpcore.client.pulp_maven.api.repositories_maven_api import RepositoriesMavenApi
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/__init__.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/content_artifact_api.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/content_artifact_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,15 +166,17 @@
 
         :param async_req bool: execute request asynchronously
         :param str artifact_id: Filter results where artifact_id matches value
         :param str filename: Filter results where filename matches value
         :param str group_id: Filter results where group_id matches value
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `upstream_id` - Upstream id * `-upstream_id` - Upstream id (descending) * `timestamp_of_interest` - Timestamp of interest * `-timestamp_of_interest` - Timestamp of interest (descending) * `group_id` - Group id * `-group_id` - Group id (descending) * `artifact_id` - Artifact id * `-artifact_id` - Artifact id (descending) * `version` - Version * `-version` - Version (descending) * `filename` - Filename * `-filename` - Filename (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param str version: Filter results where version matches value
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -202,15 +204,17 @@
 
         :param async_req bool: execute request asynchronously
         :param str artifact_id: Filter results where artifact_id matches value
         :param str filename: Filter results where filename matches value
         :param str group_id: Filter results where group_id matches value
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `upstream_id` - Upstream id * `-upstream_id` - Upstream id (descending) * `timestamp_of_interest` - Timestamp of interest * `-timestamp_of_interest` - Timestamp of interest (descending) * `group_id` - Group id * `-group_id` - Group id (descending) * `artifact_id` - Artifact id * `-artifact_id` - Artifact id (descending) * `version` - Version * `-version` - Version (descending) * `filename` - Filename * `-filename` - Filename (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param str version: Filter results where version matches value
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
@@ -232,14 +236,16 @@
         all_params = [
             'artifact_id',
             'filename',
             'group_id',
             'limit',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'repository_version',
             'repository_version_added',
             'repository_version_removed',
             'version',
             'fields',
             'exclude_fields'
         ]
@@ -275,14 +281,20 @@
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'repository_version' in local_var_params and local_var_params['repository_version'] is not None:  # noqa: E501
             query_params.append(('repository_version', local_var_params['repository_version']))  # noqa: E501
         if 'repository_version_added' in local_var_params and local_var_params['repository_version_added'] is not None:  # noqa: E501
             query_params.append(('repository_version_added', local_var_params['repository_version_added']))  # noqa: E501
         if 'repository_version_removed' in local_var_params and local_var_params['repository_version_removed'] is not None:  # noqa: E501
             query_params.append(('repository_version_removed', local_var_params['repository_version_removed']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/distributions_maven_api.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/distributions_maven_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -286,15 +286,17 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `base_path` - Base path * `-base_path` - Base path (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param str repository: Filter results where repository matches value
         :param list[str] repository__in: Filter results where repository is in a comma-separated list of values
         :param str with_content: Filter distributions based on the content served by them
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -328,15 +330,17 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `base_path` - Base path * `-base_path` - Base path (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param str repository: Filter results where repository matches value
         :param list[str] repository__in: Filter results where repository is in a comma-separated list of values
         :param str with_content: Filter distributions based on the content served by them
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
@@ -364,14 +368,16 @@
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'pulp_label_select',
             'repository',
             'repository__in',
             'with_content',
             'fields',
             'exclude_fields'
         ]
@@ -421,14 +427,20 @@
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'pulp_label_select' in local_var_params and local_var_params['pulp_label_select'] is not None:  # noqa: E501
             query_params.append(('pulp_label_select', local_var_params['pulp_label_select']))  # noqa: E501
         if 'repository' in local_var_params and local_var_params['repository'] is not None:  # noqa: E501
             query_params.append(('repository', local_var_params['repository']))  # noqa: E501
         if 'repository__in' in local_var_params and local_var_params['repository__in'] is not None:  # noqa: E501
             query_params.append(('repository__in', local_var_params['repository__in']))  # noqa: E501
             collection_formats['repository__in'] = 'csv'  # noqa: E501
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/pulp_maven_api.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/pulp_maven_api.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/remotes_maven_api.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/remotes_maven_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -282,15 +282,17 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `url` - Url * `-url` - Url (descending) * `ca_cert` - Ca cert * `-ca_cert` - Ca cert (descending) * `client_cert` - Client cert * `-client_cert` - Client cert (descending) * `client_key` - Client key * `-client_key` - Client key (descending) * `tls_validation` - Tls validation * `-tls_validation` - Tls validation (descending) * `username` - Username * `-username` - Username (descending) * `password` - Password * `-password` - Password (descending) * `proxy_url` - Proxy url * `-proxy_url` - Proxy url (descending) * `proxy_username` - Proxy username * `-proxy_username` - Proxy username (descending) * `proxy_password` - Proxy password * `-proxy_password` - Proxy password (descending) * `download_concurrency` - Download concurrency * `-download_concurrency` - Download concurrency (descending) * `max_retries` - Max retries * `-max_retries` - Max retries (descending) * `policy` - Policy * `-policy` - Policy (descending) * `total_timeout` - Total timeout * `-total_timeout` - Total timeout (descending) * `connect_timeout` - Connect timeout * `-connect_timeout` - Connect timeout (descending) * `sock_connect_timeout` - Sock connect timeout * `-sock_connect_timeout` - Sock connect timeout (descending) * `sock_read_timeout` - Sock read timeout * `-sock_read_timeout` - Sock read timeout (descending) * `headers` - Headers * `-headers` - Headers (descending) * `rate_limit` - Rate limit * `-rate_limit` - Rate limit (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param datetime pulp_last_updated: Filter results where pulp_last_updated matches value
         :param datetime pulp_last_updated__gt: Filter results where pulp_last_updated is greater than value
         :param datetime pulp_last_updated__gte: Filter results where pulp_last_updated is greater than or equal to value
         :param datetime pulp_last_updated__lt: Filter results where pulp_last_updated is less than value
         :param datetime pulp_last_updated__lte: Filter results where pulp_last_updated is less than or equal to value
         :param list[datetime] pulp_last_updated__range: Filter results where pulp_last_updated is between two comma separated values
@@ -323,15 +325,17 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `url` - Url * `-url` - Url (descending) * `ca_cert` - Ca cert * `-ca_cert` - Ca cert (descending) * `client_cert` - Client cert * `-client_cert` - Client cert (descending) * `client_key` - Client key * `-client_key` - Client key (descending) * `tls_validation` - Tls validation * `-tls_validation` - Tls validation (descending) * `username` - Username * `-username` - Username (descending) * `password` - Password * `-password` - Password (descending) * `proxy_url` - Proxy url * `-proxy_url` - Proxy url (descending) * `proxy_username` - Proxy username * `-proxy_username` - Proxy username (descending) * `proxy_password` - Proxy password * `-proxy_password` - Proxy password (descending) * `download_concurrency` - Download concurrency * `-download_concurrency` - Download concurrency (descending) * `max_retries` - Max retries * `-max_retries` - Max retries (descending) * `policy` - Policy * `-policy` - Policy (descending) * `total_timeout` - Total timeout * `-total_timeout` - Total timeout (descending) * `connect_timeout` - Connect timeout * `-connect_timeout` - Connect timeout (descending) * `sock_connect_timeout` - Sock connect timeout * `-sock_connect_timeout` - Sock connect timeout (descending) * `sock_read_timeout` - Sock read timeout * `-sock_read_timeout` - Sock read timeout (descending) * `headers` - Headers * `-headers` - Headers (descending) * `rate_limit` - Rate limit * `-rate_limit` - Rate limit (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param datetime pulp_last_updated: Filter results where pulp_last_updated matches value
         :param datetime pulp_last_updated__gt: Filter results where pulp_last_updated is greater than value
         :param datetime pulp_last_updated__gte: Filter results where pulp_last_updated is greater than or equal to value
         :param datetime pulp_last_updated__lt: Filter results where pulp_last_updated is less than value
         :param datetime pulp_last_updated__lte: Filter results where pulp_last_updated is less than or equal to value
         :param list[datetime] pulp_last_updated__range: Filter results where pulp_last_updated is between two comma separated values
@@ -358,14 +362,16 @@
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'pulp_label_select',
             'pulp_last_updated',
             'pulp_last_updated__gt',
             'pulp_last_updated__gte',
             'pulp_last_updated__lt',
             'pulp_last_updated__lte',
             'pulp_last_updated__range',
@@ -409,14 +415,20 @@
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'pulp_label_select' in local_var_params and local_var_params['pulp_label_select'] is not None:  # noqa: E501
             query_params.append(('pulp_label_select', local_var_params['pulp_label_select']))  # noqa: E501
         if 'pulp_last_updated' in local_var_params and local_var_params['pulp_last_updated'] is not None:  # noqa: E501
             query_params.append(('pulp_last_updated', local_var_params['pulp_last_updated']))  # noqa: E501
         if 'pulp_last_updated__gt' in local_var_params and local_var_params['pulp_last_updated__gt'] is not None:  # noqa: E501
             query_params.append(('pulp_last_updated__gt', local_var_params['pulp_last_updated__gt']))  # noqa: E501
         if 'pulp_last_updated__gte' in local_var_params and local_var_params['pulp_last_updated__gte'] is not None:  # noqa: E501
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/repositories_maven_api.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/repositories_maven_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,32 +402,36 @@
         A ViewSet for MavenRemote.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param str latest_with_content: Content Unit referenced by HREF
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `description` - Description * `-description` - Description (descending) * `next_version` - Next version * `-next_version` - Next version (descending) * `retain_repo_versions` - Retain repo versions * `-retain_repo_versions` - Retain repo versions (descending) * `user_hidden` - User hidden * `-user_hidden` - User hidden (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param str remote: Foreign Key referenced by HREF
         :param int retain_repo_versions: Filter results where retain_repo_versions matches value
         :param int retain_repo_versions__gt: Filter results where retain_repo_versions is greater than value
         :param int retain_repo_versions__gte: Filter results where retain_repo_versions is greater than or equal to value
         :param bool retain_repo_versions__isnull: Filter results where retain_repo_versions has a null value
         :param int retain_repo_versions__lt: Filter results where retain_repo_versions is less than value
         :param int retain_repo_versions__lte: Filter results where retain_repo_versions is less than or equal to value
         :param int retain_repo_versions__ne: Filter results where retain_repo_versions not equal to value
         :param list[int] retain_repo_versions__range: Filter results where retain_repo_versions is between two comma separated values
+        :param str with_content: Content Unit referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -446,32 +450,36 @@
         A ViewSet for MavenRemote.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param str latest_with_content: Content Unit referenced by HREF
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `description` - Description * `-description` - Description (descending) * `next_version` - Next version * `-next_version` - Next version (descending) * `retain_repo_versions` - Retain repo versions * `-retain_repo_versions` - Retain repo versions (descending) * `user_hidden` - User hidden * `-user_hidden` - User hidden (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param str remote: Foreign Key referenced by HREF
         :param int retain_repo_versions: Filter results where retain_repo_versions matches value
         :param int retain_repo_versions__gt: Filter results where retain_repo_versions is greater than value
         :param int retain_repo_versions__gte: Filter results where retain_repo_versions is greater than or equal to value
         :param bool retain_repo_versions__isnull: Filter results where retain_repo_versions has a null value
         :param int retain_repo_versions__lt: Filter results where retain_repo_versions is less than value
         :param int retain_repo_versions__lte: Filter results where retain_repo_versions is less than or equal to value
         :param int retain_repo_versions__ne: Filter results where retain_repo_versions not equal to value
         :param list[int] retain_repo_versions__range: Filter results where retain_repo_versions is between two comma separated values
+        :param str with_content: Content Unit referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -483,32 +491,36 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
+            'latest_with_content',
             'limit',
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'pulp_label_select',
             'remote',
             'retain_repo_versions',
             'retain_repo_versions__gt',
             'retain_repo_versions__gte',
             'retain_repo_versions__isnull',
             'retain_repo_versions__lt',
             'retain_repo_versions__lte',
             'retain_repo_versions__ne',
             'retain_repo_versions__range',
+            'with_content',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -527,14 +539,16 @@
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'latest_with_content' in local_var_params and local_var_params['latest_with_content'] is not None:  # noqa: E501
+            query_params.append(('latest_with_content', local_var_params['latest_with_content']))  # noqa: E501
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
         if 'name' in local_var_params and local_var_params['name'] is not None:  # noqa: E501
             query_params.append(('name', local_var_params['name']))  # noqa: E501
         if 'name__contains' in local_var_params and local_var_params['name__contains'] is not None:  # noqa: E501
             query_params.append(('name__contains', local_var_params['name__contains']))  # noqa: E501
         if 'name__icontains' in local_var_params and local_var_params['name__icontains'] is not None:  # noqa: E501
@@ -545,14 +559,20 @@
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'pulp_label_select' in local_var_params and local_var_params['pulp_label_select'] is not None:  # noqa: E501
             query_params.append(('pulp_label_select', local_var_params['pulp_label_select']))  # noqa: E501
         if 'remote' in local_var_params and local_var_params['remote'] is not None:  # noqa: E501
             query_params.append(('remote', local_var_params['remote']))  # noqa: E501
         if 'retain_repo_versions' in local_var_params and local_var_params['retain_repo_versions'] is not None:  # noqa: E501
             query_params.append(('retain_repo_versions', local_var_params['retain_repo_versions']))  # noqa: E501
         if 'retain_repo_versions__gt' in local_var_params and local_var_params['retain_repo_versions__gt'] is not None:  # noqa: E501
@@ -566,14 +586,16 @@
         if 'retain_repo_versions__lte' in local_var_params and local_var_params['retain_repo_versions__lte'] is not None:  # noqa: E501
             query_params.append(('retain_repo_versions__lte', local_var_params['retain_repo_versions__lte']))  # noqa: E501
         if 'retain_repo_versions__ne' in local_var_params and local_var_params['retain_repo_versions__ne'] is not None:  # noqa: E501
             query_params.append(('retain_repo_versions__ne', local_var_params['retain_repo_versions__ne']))  # noqa: E501
         if 'retain_repo_versions__range' in local_var_params and local_var_params['retain_repo_versions__range'] is not None:  # noqa: E501
             query_params.append(('retain_repo_versions__range', local_var_params['retain_repo_versions__range']))  # noqa: E501
             collection_formats['retain_repo_versions__range'] = 'csv'  # noqa: E501
+        if 'with_content' in local_var_params and local_var_params['with_content'] is not None:  # noqa: E501
+            query_params.append(('with_content', local_var_params['with_content']))  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
             collection_formats['exclude_fields'] = 'multi'  # noqa: E501
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api/repositories_maven_versions_api.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api/repositories_maven_versions_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,21 +168,22 @@
         :param int number: Filter results where number matches value
         :param int number__gt: Filter results where number is greater than value
         :param int number__gte: Filter results where number is greater than or equal to value
         :param int number__lt: Filter results where number is less than value
         :param int number__lte: Filter results where number is less than or equal to value
         :param list[int] number__range: Filter results where number is between two comma separated values
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `number` - Number * `-number` - Number (descending) * `complete` - Complete * `-complete` - Complete (descending) * `info` - Info * `-info` - Info (descending) * `pk` - Pk * `-pk` - Pk (descending)
         :param datetime pulp_created: Filter results where pulp_created matches value
         :param datetime pulp_created__gt: Filter results where pulp_created is greater than value
         :param datetime pulp_created__gte: Filter results where pulp_created is greater than or equal to value
         :param datetime pulp_created__lt: Filter results where pulp_created is less than value
         :param datetime pulp_created__lte: Filter results where pulp_created is less than or equal to value
         :param list[datetime] pulp_created__range: Filter results where pulp_created is between two comma separated values
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -212,21 +213,22 @@
         :param int number: Filter results where number matches value
         :param int number__gt: Filter results where number is greater than value
         :param int number__gte: Filter results where number is greater than or equal to value
         :param int number__lt: Filter results where number is less than value
         :param int number__lte: Filter results where number is less than or equal to value
         :param list[int] number__range: Filter results where number is between two comma separated values
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `number` - Number * `-number` - Number (descending) * `complete` - Complete * `-complete` - Complete (descending) * `info` - Info * `-info` - Info (descending) * `pk` - Pk * `-pk` - Pk (descending)
         :param datetime pulp_created: Filter results where pulp_created matches value
         :param datetime pulp_created__gt: Filter results where pulp_created is greater than value
         :param datetime pulp_created__gte: Filter results where pulp_created is greater than or equal to value
         :param datetime pulp_created__lt: Filter results where pulp_created is less than value
         :param datetime pulp_created__lte: Filter results where pulp_created is less than or equal to value
         :param list[datetime] pulp_created__range: Filter results where pulp_created is between two comma separated values
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -256,14 +258,15 @@
             'ordering',
             'pulp_created',
             'pulp_created__gt',
             'pulp_created__gte',
             'pulp_created__lt',
             'pulp_created__lte',
             'pulp_created__range',
+            'pulp_href__in',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -325,14 +328,17 @@
         if 'pulp_created__lt' in local_var_params and local_var_params['pulp_created__lt'] is not None:  # noqa: E501
             query_params.append(('pulp_created__lt', local_var_params['pulp_created__lt']))  # noqa: E501
         if 'pulp_created__lte' in local_var_params and local_var_params['pulp_created__lte'] is not None:  # noqa: E501
             query_params.append(('pulp_created__lte', local_var_params['pulp_created__lte']))  # noqa: E501
         if 'pulp_created__range' in local_var_params and local_var_params['pulp_created__range'] is not None:  # noqa: E501
             query_params.append(('pulp_created__range', local_var_params['pulp_created__range']))  # noqa: E501
             collection_formats['pulp_created__range'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
             collection_formats['exclude_fields'] = 'multi'  # noqa: E501
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/api_client.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.6.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/configuration.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.6.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/exceptions.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/__init__.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/async_operation_response.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/content_summary_response.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_artifact.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_artifact.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_artifact_response.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_artifact_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_distribution.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_distribution_response.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_remote.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,26 +493,26 @@
 
         self._max_retries = max_retries
 
     @property
     def policy(self):
         """Gets the policy of this MavenMavenRemote.  # noqa: E501
 
-        The policy to use when downloading content.  # noqa: E501
+        The policy to use when downloading content.  * `immediate` - immediate * `When syncing, download all metadata and content now.` - When syncing, download all metadata and content now.  # noqa: E501
 
         :return: The policy of this MavenMavenRemote.  # noqa: E501
         :rtype: PolicyEnum
         """
         return self._policy
 
     @policy.setter
     def policy(self, policy):
         """Sets the policy of this MavenMavenRemote.
 
-        The policy to use when downloading content.  # noqa: E501
+        The policy to use when downloading content.  * `immediate` - immediate * `When syncing, download all metadata and content now.` - When syncing, download all metadata and content now.  # noqa: E501
 
         :param policy: The policy of this MavenMavenRemote.  # noqa: E501
         :type: PolicyEnum
         """
 
         self._policy = policy
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_remote_response.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_remote_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,26 +415,26 @@
 
         self._max_retries = max_retries
 
     @property
     def policy(self):
         """Gets the policy of this MavenMavenRemoteResponse.  # noqa: E501
 
-        The policy to use when downloading content.  # noqa: E501
+        The policy to use when downloading content.  * `immediate` - immediate * `When syncing, download all metadata and content now.` - When syncing, download all metadata and content now.  # noqa: E501
 
         :return: The policy of this MavenMavenRemoteResponse.  # noqa: E501
         :rtype: PolicyEnum
         """
         return self._policy
 
     @policy.setter
     def policy(self, policy):
         """Sets the policy of this MavenMavenRemoteResponse.
 
-        The policy to use when downloading content.  # noqa: E501
+        The policy to use when downloading content.  * `immediate` - immediate * `When syncing, download all metadata and content now.` - When syncing, download all metadata and content now.  # noqa: E501
 
         :param policy: The policy of this MavenMavenRemoteResponse.  # noqa: E501
         :type: PolicyEnum
         """
 
         self._policy = policy
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_remote_response_hidden_fields.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_repository.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/maven_maven_repository_response.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/maven_maven_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/paginated_repository_version_response_list.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_artifact_response_list.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_artifact_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_distribution_response_list.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_remote_response_list.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_repository_response_list.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/paginatedmaven_maven_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_distribution.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_remote.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -491,26 +491,26 @@
 
         self._max_retries = max_retries
 
     @property
     def policy(self):
         """Gets the policy of this PatchedmavenMavenRemote.  # noqa: E501
 
-        The policy to use when downloading content.  # noqa: E501
+        The policy to use when downloading content.  * `immediate` - immediate * `When syncing, download all metadata and content now.` - When syncing, download all metadata and content now.  # noqa: E501
 
         :return: The policy of this PatchedmavenMavenRemote.  # noqa: E501
         :rtype: PolicyEnum
         """
         return self._policy
 
     @policy.setter
     def policy(self, policy):
         """Sets the policy of this PatchedmavenMavenRemote.
 
-        The policy to use when downloading content.  # noqa: E501
+        The policy to use when downloading content.  * `immediate` - immediate * `When syncing, download all metadata and content now.` - When syncing, download all metadata and content now.  # noqa: E501
 
         :param policy: The policy of this PatchedmavenMavenRemote.  # noqa: E501
         :type: PolicyEnum
         """
 
         self._policy = policy
```

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_repository.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/patchedmaven_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/policy_enum.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/repair.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/repair.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/repository_add_cached_content.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/repository_add_cached_content.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/models/repository_version_response.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/pulpcore/client/pulp_maven/rest.py` & `pulp_maven-client-0.6.0/pulpcore/client/pulp_maven/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/setup.py` & `pulp_maven-client-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_maven-client"
-VERSION = "0.5.0"
+VERSION = "0.6.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_maven-client-0.5.0/test/test_async_operation_response.py` & `pulp_maven-client-0.6.0/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_content_artifact_api.py` & `pulp_maven-client-0.6.0/test/test_content_artifact_api.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_content_summary_response.py` & `pulp_maven-client-0.6.0/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_distributions_maven_api.py` & `pulp_maven-client-0.6.0/test/test_distributions_maven_api.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_maven_maven_artifact.py` & `pulp_maven-client-0.6.0/test/test_maven_maven_artifact.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_maven_maven_artifact_response.py` & `pulp_maven-client-0.6.0/test/test_maven_maven_artifact_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_maven_maven_distribution.py` & `pulp_maven-client-0.6.0/test/test_maven_maven_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_maven_maven_distribution_response.py` & `pulp_maven-client-0.6.0/test/test_maven_maven_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_maven_maven_remote.py` & `pulp_maven-client-0.6.0/test/test_maven_maven_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_maven_maven_remote_response.py` & `pulp_maven-client-0.6.0/test/test_maven_maven_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_maven_maven_remote_response_hidden_fields.py` & `pulp_maven-client-0.6.0/test/test_maven_maven_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_maven_maven_repository.py` & `pulp_maven-client-0.6.0/test/test_maven_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_maven_maven_repository_response.py` & `pulp_maven-client-0.6.0/test/test_maven_maven_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_paginated_repository_version_response_list.py` & `pulp_maven-client-0.6.0/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_paginatedmaven_maven_artifact_response_list.py` & `pulp_maven-client-0.6.0/test/test_paginatedmaven_maven_artifact_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_paginatedmaven_maven_distribution_response_list.py` & `pulp_maven-client-0.6.0/test/test_paginatedmaven_maven_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_paginatedmaven_maven_remote_response_list.py` & `pulp_maven-client-0.6.0/test/test_paginatedmaven_maven_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_paginatedmaven_maven_repository_response_list.py` & `pulp_maven-client-0.6.0/test/test_paginatedmaven_maven_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_patchedmaven_maven_distribution.py` & `pulp_maven-client-0.6.0/test/test_patchedmaven_maven_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_patchedmaven_maven_remote.py` & `pulp_maven-client-0.6.0/test/test_patchedmaven_maven_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_patchedmaven_maven_repository.py` & `pulp_maven-client-0.6.0/test/test_patchedmaven_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_policy_enum.py` & `pulp_maven-client-0.6.0/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_pulp_maven_api.py` & `pulp_maven-client-0.6.0/test/test_pulp_maven_api.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_remotes_maven_api.py` & `pulp_maven-client-0.6.0/test/test_remotes_maven_api.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_repair.py` & `pulp_maven-client-0.6.0/test/test_repair.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_repositories_maven_api.py` & `pulp_maven-client-0.6.0/test/test_repositories_maven_api.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_repositories_maven_versions_api.py` & `pulp_maven-client-0.6.0/test/test_repositories_maven_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_repository_add_cached_content.py` & `pulp_maven-client-0.6.0/test/test_repository_add_cached_content.py`

 * *Files identical despite different names*

### Comparing `pulp_maven-client-0.5.0/test/test_repository_version_response.py` & `pulp_maven-client-0.6.0/test/test_repository_version_response.py`

 * *Files identical despite different names*

