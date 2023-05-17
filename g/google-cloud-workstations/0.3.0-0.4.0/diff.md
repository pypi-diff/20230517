# Comparing `tmp/google-cloud-workstations-0.3.0.tar.gz` & `tmp/google-cloud-workstations-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-workstations-0.3.0.tar", last modified: Thu May 11 18:37:01 2023, max compression
+gzip compressed data, was "google-cloud-workstations-0.4.0.tar", last modified: Wed May 17 17:31:22 2023, max compression
```

## Comparing `google-cloud-workstations-0.3.0.tar` & `google-cloud-workstations-0.4.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4600 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3682 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.395266 google-cloud-workstations-0.3.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.395266 google-cloud-workstations-0.3.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations/
--rw-rw-r--   0 root         (0)     1003     3048 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/
--rw-rw-r--   0 root         (0)     1003     2904 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8908 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/
--rw-rw-r--   0 root         (0)     1003      761 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003   129566 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/async_client.py
--rw-rw-r--   0 root         (0)     1003   140785 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/client.py
--rw-rw-r--   0 root         (0)     1003    27340 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20457 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    43040 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43871 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   142624 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/types/
--rw-rw-r--   0 root         (0)     1003     2643 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    55514 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/types/workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.403266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/
--rw-rw-r--   0 root         (0)     1003     2908 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     8916 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.403266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.403266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/
--rw-rw-r--   0 root         (0)     1003      761 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003   129831 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/async_client.py
--rw-rw-r--   0 root         (0)     1003   141050 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/client.py
--rw-rw-r--   0 root         (0)     1003    27504 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.403266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20465 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    43078 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43909 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   142768 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.403266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     2643 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    54080 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/types/workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/
--rw-r--r--   0 root         (0)     1003     4600 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2717 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2994 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   568245 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1/test_workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   567385 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1beta/test_workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.340876 google-cloud-workstations-0.4.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4600 2023-05-17 17:31:22.340876 google-cloud-workstations-0.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3682 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.328870 google-cloud-workstations-0.4.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.328870 google-cloud-workstations-0.4.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.328870 google-cloud-workstations-0.4.0/google/cloud/workstations/
+-rw-rw-r--   0 root         (0)     1003     3048 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003      653 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/
+-rw-rw-r--   0 root         (0)     1003     2904 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8908 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/
+-rw-rw-r--   0 root         (0)     1003      761 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003   129566 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/async_client.py
+-rw-rw-r--   0 root         (0)     1003   140785 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/client.py
+-rw-rw-r--   0 root         (0)     1003    27340 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20457 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43040 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43871 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   142624 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2643 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    55514 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/types/workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/
+-rw-rw-r--   0 root         (0)     1003     2908 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8916 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/
+-rw-rw-r--   0 root         (0)     1003      761 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003   130002 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/async_client.py
+-rw-rw-r--   0 root         (0)     1003   141221 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/client.py
+-rw-rw-r--   0 root         (0)     1003    27504 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20465 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43124 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43955 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   142768 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     2643 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    58373 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/types/workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/
+-rw-r--r--   0 root         (0)     1003     4600 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2717 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-05-17 17:31:22.340876 google-cloud-workstations-0.4.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2994 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   568245 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1/test_workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.340876 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   569173 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1beta/test_workstations.py
```

### Comparing `google-cloud-workstations-0.3.0/LICENSE` & `google-cloud-workstations-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/MANIFEST.in` & `google-cloud-workstations-0.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/PKG-INFO` & `google-cloud-workstations-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-workstations
-Version: 0.3.0
+Version: 0.4.0
 Summary: Google Cloud Workstations API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-workstations-0.3.0/README.rst` & `google-cloud-workstations-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations/gapic_version.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.3.0"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/gapic_metadata.json` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/gapic_version.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.3.0"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/async_client.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/client.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/pagers.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/base.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/grpc.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/rest.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/types/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/types/workstations.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/types/workstations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/gapic_metadata.json` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/gapic_version.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.3.0"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/async_client.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1277,15 +1277,17 @@
                 should not be set.
             workstation_config (:class:`google.cloud.workstations_v1beta.types.WorkstationConfig`):
                 Required. Config to create.
                 This corresponds to the ``workstation_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             workstation_config_id (:class:`str`):
-                Required. ID to use for the config.
+                Required. ID to use for the
+                workstation configuration.
+
                 This corresponds to the ``workstation_config_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
@@ -1404,15 +1406,16 @@
             workstation_config (:class:`google.cloud.workstations_v1beta.types.WorkstationConfig`):
                 Required. Config to update.
                 This corresponds to the ``workstation_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Mask specifying which
-                fields in the config should be updated.
+                fields in the workstation configuration
+                should be updated.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1526,16 +1529,16 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.workstations_v1beta.types.DeleteWorkstationConfigRequest, dict]]):
                 The request object. Message for deleting a workstation
                 configuration.
             name (:class:`str`):
-                Required. Name of the config to
-                delete.
+                Required. Name of the workstation
+                configuration to delete.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1717,15 +1720,16 @@
         request: Optional[Union[workstations.ListWorkstationsRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListWorkstationsAsyncPager:
-        r"""Returns all Workstations using the specified config.
+        r"""Returns all Workstations using the specified
+        workstation configuration.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1840,16 +1844,16 @@
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListUsableWorkstationsAsyncPager:
-        r"""Returns all Workstations using the specified config
-        on which the caller has the
+        r"""Returns all workstations using the specified
+        workstation configuration on which the caller has the
         "workstations.workstations.use" permission.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
@@ -2142,15 +2146,16 @@
             workstation (:class:`google.cloud.workstations_v1beta.types.Workstation`):
                 Required. Workstation to update.
                 This corresponds to the ``workstation`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Mask specifying which
-                fields in the config should be updated.
+                fields in the workstation configuration
+                should be updated.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/client.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1515,15 +1515,17 @@
                 should not be set.
             workstation_config (google.cloud.workstations_v1beta.types.WorkstationConfig):
                 Required. Config to create.
                 This corresponds to the ``workstation_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             workstation_config_id (str):
-                Required. ID to use for the config.
+                Required. ID to use for the
+                workstation configuration.
+
                 This corresponds to the ``workstation_config_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
@@ -1644,15 +1646,16 @@
             workstation_config (google.cloud.workstations_v1beta.types.WorkstationConfig):
                 Required. Config to update.
                 This corresponds to the ``workstation_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Mask specifying which
-                fields in the config should be updated.
+                fields in the workstation configuration
+                should be updated.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1768,16 +1771,16 @@
                 print(response)
 
         Args:
             request (Union[google.cloud.workstations_v1beta.types.DeleteWorkstationConfigRequest, dict]):
                 The request object. Message for deleting a workstation
                 configuration.
             name (str):
-                Required. Name of the config to
-                delete.
+                Required. Name of the workstation
+                configuration to delete.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1952,15 +1955,16 @@
         request: Optional[Union[workstations.ListWorkstationsRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListWorkstationsPager:
-        r"""Returns all Workstations using the specified config.
+        r"""Returns all Workstations using the specified
+        workstation configuration.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2066,16 +2070,16 @@
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListUsableWorkstationsPager:
-        r"""Returns all Workstations using the specified config
-        on which the caller has the
+        r"""Returns all workstations using the specified
+        workstation configuration on which the caller has the
         "workstations.workstations.use" permission.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
@@ -2359,15 +2363,16 @@
             workstation (google.cloud.workstations_v1beta.types.Workstation):
                 Required. Workstation to update.
                 This corresponds to the ``workstation`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Mask specifying which
-                fields in the config should be updated.
+                fields in the workstation configuration
+                should be updated.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/pagers.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/base.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,16 @@
     def list_workstations(
         self,
     ) -> Callable[
         [workstations.ListWorkstationsRequest], workstations.ListWorkstationsResponse
     ]:
         r"""Return a callable for the list workstations method over gRPC.
 
-        Returns all Workstations using the specified config.
+        Returns all Workstations using the specified
+        workstation configuration.
 
         Returns:
             Callable[[~.ListWorkstationsRequest],
                     ~.ListWorkstationsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -624,16 +625,16 @@
         self,
     ) -> Callable[
         [workstations.ListUsableWorkstationsRequest],
         workstations.ListUsableWorkstationsResponse,
     ]:
         r"""Return a callable for the list usable workstations method over gRPC.
 
-        Returns all Workstations using the specified config
-        on which the caller has the
+        Returns all workstations using the specified
+        workstation configuration on which the caller has the
         "workstations.workstations.use" permission.
 
         Returns:
             Callable[[~.ListUsableWorkstationsRequest],
                     ~.ListUsableWorkstationsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
```

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,15 +611,16 @@
         self,
     ) -> Callable[
         [workstations.ListWorkstationsRequest],
         Awaitable[workstations.ListWorkstationsResponse],
     ]:
         r"""Return a callable for the list workstations method over gRPC.
 
-        Returns all Workstations using the specified config.
+        Returns all Workstations using the specified
+        workstation configuration.
 
         Returns:
             Callable[[~.ListWorkstationsRequest],
                     Awaitable[~.ListWorkstationsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -640,16 +641,16 @@
         self,
     ) -> Callable[
         [workstations.ListUsableWorkstationsRequest],
         Awaitable[workstations.ListUsableWorkstationsResponse],
     ]:
         r"""Return a callable for the list usable workstations method over gRPC.
 
-        Returns all Workstations using the specified config
-        on which the caller has the
+        Returns all workstations using the specified
+        workstation configuration on which the caller has the
         "workstations.workstations.use" permission.
 
         Returns:
             Callable[[~.ListUsableWorkstationsRequest],
                     Awaitable[~.ListUsableWorkstationsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
```

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/rest.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/types/__init__.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/types/workstations.py` & `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/types/workstations.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,26 +89,33 @@
             Output only. Time when this resource was most
             recently updated.
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when this resource was
             soft-deleted.
         etag (str):
             Checksum computed by the server. May be sent
-            on update and delete requests to ensure that the
-            client has an up-to-date value before
+            on update and delete requests to make sure that
+            the client has an up-to-date value before
             proceeding.
         network (str):
             Immutable. Name of the Compute Engine network
             in which instances associated with this cluster
             will be created.
         subnetwork (str):
             Immutable. Name of the Compute Engine
             subnetwork in which instances associated with
             this cluster will be created. Must be part of
             the subnetwork specified for this cluster.
+        control_plane_ip (str):
+            Output only. The private IP address of the
+            control plane for this cluster. Workstation VMs
+            need access to this IP address to work with the
+            service, so make sure that your firewall rules
+            allow egress from the workstation VMs to this
+            address.
         private_cluster_config (google.cloud.workstations_v1beta.types.WorkstationCluster.PrivateClusterConfig):
             Configuration for private cluster.
         degraded (bool):
             Output only. Whether this resource is in degraded mode, in
             which case it may require user action to restore full
             functionality. Details can be found in the ``conditions``
             field.
@@ -213,14 +220,18 @@
         proto.STRING,
         number=10,
     )
     subnetwork: str = proto.Field(
         proto.STRING,
         number=11,
     )
+    control_plane_ip: str = proto.Field(
+        proto.STRING,
+        number=16,
+    )
     private_cluster_config: PrivateClusterConfig = proto.Field(
         proto.MESSAGE,
         number=12,
         message=PrivateClusterConfig,
     )
     degraded: bool = proto.Field(
         proto.BOOL,
@@ -263,16 +274,16 @@
             Output only. Time when this resource was most
             recently updated.
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when this resource was
             soft-deleted.
         etag (str):
             Checksum computed by the server. May be sent
-            on update and delete requests to ensure that the
-            client has an up-to-date value before
+            on update and delete requests to make sure that
+            the client has an up-to-date value before
             proceeding.
         idle_timeout (google.protobuf.duration_pb2.Duration):
             How long to wait before automatically
             stopping an instance that hasn't received any
             user traffic. A value of 0 indicates that this
             instance should never time out due to idleness.
             Defaults to 20 minutes.
@@ -288,17 +299,17 @@
             Directories to persist across workstation
             sessions.
         container (google.cloud.workstations_v1beta.types.WorkstationConfig.Container):
             Container that will be run for each
             workstation using this configuration when that
             workstation is started.
         encryption_key (google.cloud.workstations_v1beta.types.WorkstationConfig.CustomerEncryptionKey):
-            Encrypts resources of this workstation
-            configuration using a customer-managed
-            encryption key.
+            Immutable. Encrypts resources of this
+            workstation configuration using a
+            customer-managed encryption key.
             If specified, the boot disk of the Compute
             Engine instance and the persistent disk are
             encrypted using this encryption key. If this
             field is not set, the disks are encrypted using
             a generated key. Customer-managed encryption
             keys do not protect disk metadata.
             If the customer-managed encryption key is
@@ -307,22 +318,37 @@
             persistent disk with the new version of the key.
             Be sure to keep older versions of the key until
             the persistent disk is recreated. Otherwise,
             data on the persistent disk will be lost.
             If the encryption key is revoked, the
             workstation session will automatically be
             stopped within 7 hours.
+
+            Immutable after the workstation configuration is
+            created.
+        readiness_checks (MutableSequence[google.cloud.workstations_v1beta.types.WorkstationConfig.ReadinessCheck]):
+            Readiness checks to perform when starting a
+            workstation using this workstation
+            configuration. Mark a workstation as running
+            only after all specified readiness checks return
+            200 status codes.
         degraded (bool):
             Output only. Whether this resource is in degraded mode, in
             which case it may require user action to restore full
             functionality. Details can be found in the ``conditions``
             field.
         conditions (MutableSequence[google.rpc.status_pb2.Status]):
             Output only. Status conditions describing the
             current resource state.
+        enable_audit_agent (bool):
+            Whether to enable linux auditd logging on the workstation.
+            When enabled, a service account must also be specified that
+            has logging.buckets.write permission on the project.
+            Operating system audit logging is distinct from `Cloud Audit
+            Logs <https://cloud.google.com/workstations/docs/audit-logging>`__.
     """
 
     class Host(proto.Message):
         r"""Runtime host for a workstation.
 
         .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
@@ -349,25 +375,32 @@
                     image; otherwise, the image must be publicly
                     accessible.
                 tags (MutableSequence[str]):
                     Network tags to add to the Compute Engine
                     machines backing the Workstations.
                 pool_size (int):
                     Number of instances to pool for faster
-                    workstation starup.
+                    workstation startup.
+                pooled_instances (int):
+                    Output only. Number of instances currently
+                    available in the pool for faster workstation
+                    startup.
                 disable_public_ip_addresses (bool):
                     Whether instances have no public IP address.
                 shielded_instance_config (google.cloud.workstations_v1beta.types.WorkstationConfig.Host.GceInstance.GceShieldedInstanceConfig):
                     A set of Compute Engine Shielded instance
                     options.
                 confidential_instance_config (google.cloud.workstations_v1beta.types.WorkstationConfig.Host.GceInstance.GceConfidentialInstanceConfig):
                     A set of Compute Engine Confidential VM
                     instance options.
                 boot_disk_size_gb (int):
-                    Size of the boot disk in GB.
+                    Size of the boot disk in GB. Defaults to 50.
+                accelerators (MutableSequence[google.cloud.workstations_v1beta.types.WorkstationConfig.Host.GceInstance.Accelerator]):
+                    A list of the type and count of accelerator
+                    cards attached to the instance.
             """
 
             class GceShieldedInstanceConfig(proto.Message):
                 r"""A set of Compute Engine Shielded instance options.
 
                 Attributes:
                     enable_secure_boot (bool):
@@ -402,14 +435,35 @@
                 """
 
                 enable_confidential_compute: bool = proto.Field(
                     proto.BOOL,
                     number=1,
                 )
 
+            class Accelerator(proto.Message):
+                r"""An accelerator card attached to the instance.
+
+                Attributes:
+                    type_ (str):
+                        Type of accelerator resource to attach to the
+                        instance, for example, "nvidia-tesla-p100".
+                    count (int):
+                        Number of accelerator cards exposed to the
+                        instance.
+                """
+
+                type_: str = proto.Field(
+                    proto.STRING,
+                    number=1,
+                )
+                count: int = proto.Field(
+                    proto.INT32,
+                    number=2,
+                )
+
             machine_type: str = proto.Field(
                 proto.STRING,
                 number=1,
             )
             service_account: str = proto.Field(
                 proto.STRING,
                 number=2,
@@ -418,14 +472,18 @@
                 proto.STRING,
                 number=4,
             )
             pool_size: int = proto.Field(
                 proto.INT32,
                 number=5,
             )
+            pooled_instances: int = proto.Field(
+                proto.INT32,
+                number=12,
+            )
             disable_public_ip_addresses: bool = proto.Field(
                 proto.BOOL,
                 number=6,
             )
             shielded_instance_config: "WorkstationConfig.Host.GceInstance.GceShieldedInstanceConfig" = proto.Field(
                 proto.MESSAGE,
                 number=8,
@@ -436,14 +494,21 @@
                 number=10,
                 message="WorkstationConfig.Host.GceInstance.GceConfidentialInstanceConfig",
             )
             boot_disk_size_gb: int = proto.Field(
                 proto.INT32,
                 number=9,
             )
+            accelerators: MutableSequence[
+                "WorkstationConfig.Host.GceInstance.Accelerator"
+            ] = proto.RepeatedField(
+                proto.MESSAGE,
+                number=11,
+                message="WorkstationConfig.Host.GceInstance.Accelerator",
+            )
 
         gce_instance: "WorkstationConfig.Host.GceInstance" = proto.Field(
             proto.MESSAGE,
             number=1,
             oneof="config",
             message="WorkstationConfig.Host.GceInstance",
         )
@@ -467,21 +532,22 @@
         class GceRegionalPersistentDisk(proto.Message):
             r"""A PersistentDirectory backed by a Compute Engine regional
             persistent disk.
 
             Attributes:
                 size_gb (int):
                     Size of the disk in GB. Must be empty if source_snapshot is
-                    set.
+                    set. Defaults to 200.
                 fs_type (str):
                     Type of file system that the disk should be formatted with.
                     The workstation image must support this file system type.
-                    Must be empty if source_snapshot is set.
+                    Must be empty if source_snapshot is set. Defaults to ext4.
                 disk_type (str):
-                    Type of the disk to use.
+                    Type of the disk to use. Defaults to
+                    pd-standard.
                 source_snapshot (str):
                     Name of the snapshot to use as the source for the disk. If
                     set, size_gb and fs_type must be empty.
                 reclaim_policy (google.cloud.workstations_v1beta.types.WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk.ReclaimPolicy):
                     What should happen to the disk after the
                     workstation is deleted. Defaults to DELETE.
             """
@@ -540,24 +606,24 @@
 
     class Container(proto.Message):
         r"""A Docker container.
 
         Attributes:
             image (str):
                 Docker image defining the container. This
-                image must be accessible by the config's service
-                account.
+                image must be accessible by the service account
+                specified in the workstation configuration.
             command (MutableSequence[str]):
                 If set, overrides the default ENTRYPOINT
                 specified by the image.
             args (MutableSequence[str]):
                 Arguments passed to the entrypoint.
             env (MutableMapping[str, str]):
                 Environment variables passed to the
-                container.
+                container's entrypoint.
             working_dir (str):
                 If set, overrides the default DIR specified
                 by the image.
             run_as_user (int):
                 If set, overrides the USER specified in the
                 image with the given uid.
         """
@@ -590,35 +656,55 @@
 
     class CustomerEncryptionKey(proto.Message):
         r"""A customer-managed encryption key for the Compute Engine
         resources of this workstation configuration.
 
         Attributes:
             kms_key (str):
-                The name of the Google Cloud KMS encryption key. For
-                example,
+                Immutable. The name of the Google Cloud KMS encryption key.
+                For example,
                 ``projects/PROJECT_ID/locations/REGION/keyRings/KEY_RING/cryptoKeys/KEY_NAME``.
             kms_key_service_account (str):
-                The service account to use with the specified KMS key. We
-                recommend that you use a separate service account and follow
-                KMS best practices. For more information, see `Separation of
+                Immutable. The service account to use with the specified KMS
+                key. We recommend that you use a separate service account
+                and follow KMS best practices. For more information, see
+                `Separation of
                 duties <https://cloud.google.com/kms/docs/separation-of-duties>`__
                 and ``gcloud kms keys add-iam-policy-binding``
                 ```--member`` <https://cloud.google.com/sdk/gcloud/reference/kms/keys/add-iam-policy-binding#--member>`__.
         """
 
         kms_key: str = proto.Field(
             proto.STRING,
             number=1,
         )
         kms_key_service_account: str = proto.Field(
             proto.STRING,
             number=2,
         )
 
+    class ReadinessCheck(proto.Message):
+        r"""A readiness check to be performed on a workstation.
+
+        Attributes:
+            path (str):
+                Path to which the request should be sent.
+            port (int):
+                Port to which the request should be sent.
+        """
+
+        path: str = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        port: int = proto.Field(
+            proto.INT32,
+            number=2,
+        )
+
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     display_name: str = proto.Field(
         proto.STRING,
         number=2,
@@ -686,23 +772,32 @@
         message=Container,
     )
     encryption_key: CustomerEncryptionKey = proto.Field(
         proto.MESSAGE,
         number=17,
         message=CustomerEncryptionKey,
     )
+    readiness_checks: MutableSequence[ReadinessCheck] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=19,
+        message=ReadinessCheck,
+    )
     degraded: bool = proto.Field(
         proto.BOOL,
         number=15,
     )
     conditions: MutableSequence[status_pb2.Status] = proto.RepeatedField(
         proto.MESSAGE,
         number=16,
         message=status_pb2.Status,
     )
+    enable_audit_agent: bool = proto.Field(
+        proto.BOOL,
+        number=20,
+    )
 
 
 class Workstation(proto.Message):
     r"""A single instance of a developer workstation with its own
     persistent storage.
 
     Attributes:
@@ -730,27 +825,30 @@
             Output only. Time when this resource was most
             recently updated.
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when this resource was
             soft-deleted.
         etag (str):
             Checksum computed by the server. May be sent
-            on update and delete requests to ensure that the
-            client has an up-to-date value before
+            on update and delete requests to make sure that
+            the client has an up-to-date value before
             proceeding.
         state (google.cloud.workstations_v1beta.types.Workstation.State):
             Output only. Current state of the
             workstation.
         host (str):
             Output only. Host to which clients can send HTTPS traffic
             that will be received by the workstation. Authorized traffic
             will be received to the workstation as HTTP on port 80. To
             send traffic to a different port, clients may prefix the
             host with the destination port in the format
             ``{port}-{host}``.
+        env (MutableMapping[str, str]):
+            Environment variables passed to the
+            workstation container's entrypoint.
     """
 
     class State(proto.Enum):
         r"""Whether a workstation is running and ready to receive user
         requests.
 
         Values:
@@ -824,14 +922,19 @@
         number=10,
         enum=State,
     )
     host: str = proto.Field(
         proto.STRING,
         number=11,
     )
+    env: MutableMapping[str, str] = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=12,
+    )
 
 
 class GetWorkstationClusterRequest(proto.Message):
     r"""Request message for GetWorkstationCluster.
 
     Attributes:
         name (str):
@@ -986,15 +1089,15 @@
             delete.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not apply it.
         etag (str):
             If set, the request will be rejected if the
             latest version of the workstation cluster on the
-            server does not have this etag.
+            server does not have this ETag.
         force (bool):
             If set, any workstation configurations and
             workstations in the workstation cluster are also
             deleted. Otherwise, the request only works if
             the workstation cluster has no configurations or
             workstations.
     """
@@ -1154,15 +1257,16 @@
 class CreateWorkstationConfigRequest(proto.Message):
     r"""Message for creating a CreateWorkstationConfig.
 
     Attributes:
         parent (str):
             Required. Parent resource name.
         workstation_config_id (str):
-            Required. ID to use for the config.
+            Required. ID to use for the workstation
+            configuration.
         workstation_config (google.cloud.workstations_v1beta.types.WorkstationConfig):
             Required. Config to create.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
     """
 
@@ -1189,21 +1293,22 @@
     r"""Request message for UpdateWorkstationConfig.
 
     Attributes:
         workstation_config (google.cloud.workstations_v1beta.types.WorkstationConfig):
             Required. Config to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask specifying which fields in the
-            config should be updated.
+            workstation configuration should be updated.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         allow_missing (bool):
-            If set, and the config is not found, a new config will be
-            created. In this situation, update_mask is ignored.
+            If set and the workstation configuration is not found, a new
+            workstation configuration will be created. In this
+            situation, update_mask is ignored.
     """
 
     workstation_config: "WorkstationConfig" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="WorkstationConfig",
     )
@@ -1223,26 +1328,28 @@
 
 
 class DeleteWorkstationConfigRequest(proto.Message):
     r"""Message for deleting a workstation configuration.
 
     Attributes:
         name (str):
-            Required. Name of the config to delete.
+            Required. Name of the workstation
+            configuration to delete.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         etag (str):
-            If set, the request will be rejected if the
-            latest version of the config on the server does
-            not have this etag.
+            If set, the request is rejected if the latest
+            version of the workstation configuration on the
+            server does not have this ETag.
         force (bool):
-            If set, any Workstations in the config will
-            also be deleted. Otherwise, the request will
-            work only if the config has no workstations.
+            If set, any workstations in the workstation
+            configuration are also deleted. Otherwise, the
+            request works only if the workstation
+            configuration has no workstations.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     validate_only: bool = proto.Field(
@@ -1431,21 +1538,22 @@
     r"""Request message for UpdateWorkstation.
 
     Attributes:
         workstation (google.cloud.workstations_v1beta.types.Workstation):
             Required. Workstation to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask specifying which fields in the
-            config should be updated.
+            workstation configuration should be updated.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         allow_missing (bool):
-            If set, and the config is not found, a new config will be
-            created. In this situation, update_mask is ignored.
+            If set and the workstation configuration is not found, a new
+            workstation configuration is created. In this situation,
+            update_mask is ignored.
     """
 
     workstation: "Workstation" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Workstation",
     )
@@ -1472,15 +1580,15 @@
             Required. Name of the workstation to delete.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         etag (str):
             If set, the request will be rejected if the
             latest version of the workstation on the server
-            does not have this etag.
+            does not have this ETag.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     validate_only: bool = proto.Field(
@@ -1501,15 +1609,15 @@
             Required. Name of the workstation to start.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         etag (str):
             If set, the request will be rejected if the
             latest version of the workstation on the server
-            does not have this etag.
+            does not have this ETag.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     validate_only: bool = proto.Field(
@@ -1530,15 +1638,15 @@
             Required. Name of the workstation to stop.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         etag (str):
             If set, the request will be rejected if the
             latest version of the workstation on the server
-            does not have this etag.
+            does not have this ETag.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     validate_only: bool = proto.Field(
@@ -1603,15 +1711,15 @@
 class GenerateAccessTokenResponse(proto.Message):
     r"""Response message for GenerateAccessToken.
 
     Attributes:
         access_token (str):
             The generated bearer access token. To use this token,
             include it in an Authorization header of an HTTP request
-            sent to the associated workstation's hostname, for example,
+            sent to the associated workstation's hostname—for example,
             ``Authorization: Bearer <access_token>``.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Time at which the generated token will
             expire.
     """
 
     access_token: str = proto.Field(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/PKG-INFO` & `google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-workstations
-Version: 0.3.0
+Version: 0.4.0
 Summary: Google Cloud Workstations API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/SOURCES.txt` & `google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/setup.py` & `google-cloud-workstations-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/tests/__init__.py` & `google-cloud-workstations-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/tests/unit/__init__.py` & `google-cloud-workstations-0.4.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/tests/unit/gapic/__init__.py` & `google-cloud-workstations-0.4.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1/__init__.py` & `google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1/test_workstations.py` & `google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1/test_workstations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1beta/__init__.py` & `google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1beta/test_workstations.py` & `google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1beta/test_workstations.py`

 * *Files 0% similar despite different names*

```diff
@@ -734,14 +734,15 @@
             name="name_value",
             display_name="display_name_value",
             uid="uid_value",
             reconciling=True,
             etag="etag_value",
             network="network_value",
             subnetwork="subnetwork_value",
+            control_plane_ip="control_plane_ip_value",
             degraded=True,
         )
         response = client.get_workstation_cluster(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
@@ -752,14 +753,15 @@
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.uid == "uid_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.network == "network_value"
     assert response.subnetwork == "subnetwork_value"
+    assert response.control_plane_ip == "control_plane_ip_value"
     assert response.degraded is True
 
 
 def test_get_workstation_cluster_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = WorkstationsClient(
@@ -801,14 +803,15 @@
                 name="name_value",
                 display_name="display_name_value",
                 uid="uid_value",
                 reconciling=True,
                 etag="etag_value",
                 network="network_value",
                 subnetwork="subnetwork_value",
+                control_plane_ip="control_plane_ip_value",
                 degraded=True,
             )
         )
         response = await client.get_workstation_cluster(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
@@ -820,14 +823,15 @@
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.uid == "uid_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.network == "network_value"
     assert response.subnetwork == "subnetwork_value"
+    assert response.control_plane_ip == "control_plane_ip_value"
     assert response.degraded is True
 
 
 @pytest.mark.asyncio
 async def test_get_workstation_cluster_async_from_dict():
     await test_get_workstation_cluster_async(request_type=dict)
 
@@ -2208,14 +2212,15 @@
         call.return_value = workstations.WorkstationConfig(
             name="name_value",
             display_name="display_name_value",
             uid="uid_value",
             reconciling=True,
             etag="etag_value",
             degraded=True,
+            enable_audit_agent=True,
         )
         response = client.get_workstation_config(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == workstations.GetWorkstationConfigRequest()
@@ -2224,14 +2229,15 @@
     assert isinstance(response, workstations.WorkstationConfig)
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.uid == "uid_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.degraded is True
+    assert response.enable_audit_agent is True
 
 
 def test_get_workstation_config_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = WorkstationsClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2271,14 +2277,15 @@
             workstations.WorkstationConfig(
                 name="name_value",
                 display_name="display_name_value",
                 uid="uid_value",
                 reconciling=True,
                 etag="etag_value",
                 degraded=True,
+                enable_audit_agent=True,
             )
         )
         response = await client.get_workstation_config(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -2288,14 +2295,15 @@
     assert isinstance(response, workstations.WorkstationConfig)
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.uid == "uid_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.degraded is True
+    assert response.enable_audit_agent is True
 
 
 @pytest.mark.asyncio
 async def test_get_workstation_config_async_from_dict():
     await test_get_workstation_config_async(request_type=dict)
 
 
@@ -6735,14 +6743,15 @@
             name="name_value",
             display_name="display_name_value",
             uid="uid_value",
             reconciling=True,
             etag="etag_value",
             network="network_value",
             subnetwork="subnetwork_value",
+            control_plane_ip="control_plane_ip_value",
             degraded=True,
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = workstations.WorkstationCluster.pb(return_value)
@@ -6757,14 +6766,15 @@
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.uid == "uid_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.network == "network_value"
     assert response.subnetwork == "subnetwork_value"
+    assert response.control_plane_ip == "control_plane_ip_value"
     assert response.degraded is True
 
 
 def test_get_workstation_cluster_rest_required_fields(
     request_type=workstations.GetWorkstationClusterRequest,
 ):
     transport_class = transports.WorkstationsRestTransport
@@ -7367,14 +7377,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "network": "network_value",
         "subnetwork": "subnetwork_value",
+        "control_plane_ip": "control_plane_ip_value",
         "private_cluster_config": {
             "enable_private_endpoint": True,
             "cluster_hostname": "cluster_hostname_value",
             "service_attachment_uri": "service_attachment_uri_value",
             "allowed_projects": ["allowed_projects_value1", "allowed_projects_value2"],
         },
         "degraded": True,
@@ -7611,14 +7622,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "network": "network_value",
         "subnetwork": "subnetwork_value",
+        "control_plane_ip": "control_plane_ip_value",
         "private_cluster_config": {
             "enable_private_endpoint": True,
             "cluster_hostname": "cluster_hostname_value",
             "service_attachment_uri": "service_attachment_uri_value",
             "allowed_projects": ["allowed_projects_value1", "allowed_projects_value2"],
         },
         "degraded": True,
@@ -7742,14 +7754,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "network": "network_value",
         "subnetwork": "subnetwork_value",
+        "control_plane_ip": "control_plane_ip_value",
         "private_cluster_config": {
             "enable_private_endpoint": True,
             "cluster_hostname": "cluster_hostname_value",
             "service_attachment_uri": "service_attachment_uri_value",
             "allowed_projects": ["allowed_projects_value1", "allowed_projects_value2"],
         },
         "degraded": True,
@@ -7970,14 +7983,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "network": "network_value",
         "subnetwork": "subnetwork_value",
+        "control_plane_ip": "control_plane_ip_value",
         "private_cluster_config": {
             "enable_private_endpoint": True,
             "cluster_hostname": "cluster_hostname_value",
             "service_attachment_uri": "service_attachment_uri_value",
             "allowed_projects": ["allowed_projects_value1", "allowed_projects_value2"],
         },
         "degraded": True,
@@ -8386,14 +8400,15 @@
         return_value = workstations.WorkstationConfig(
             name="name_value",
             display_name="display_name_value",
             uid="uid_value",
             reconciling=True,
             etag="etag_value",
             degraded=True,
+            enable_audit_agent=True,
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = workstations.WorkstationConfig.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8406,14 +8421,15 @@
     assert isinstance(response, workstations.WorkstationConfig)
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.uid == "uid_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.degraded is True
+    assert response.enable_audit_agent is True
 
 
 def test_get_workstation_config_rest_required_fields(
     request_type=workstations.GetWorkstationConfigRequest,
 ):
     transport_class = transports.WorkstationsRestTransport
 
@@ -9393,22 +9409,24 @@
         "running_timeout": {},
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
+                "pooled_instances": 1706,
                 "disable_public_ip_addresses": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
+                "accelerators": [{"type_": "type__value", "count": 553}],
             }
         },
         "persistent_directories": [
             {
                 "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
@@ -9427,27 +9445,29 @@
             "working_dir": "working_dir_value",
             "run_as_user": 1190,
         },
         "encryption_key": {
             "kms_key": "kms_key_value",
             "kms_key_service_account": "kms_key_service_account_value",
         },
+        "readiness_checks": [{"path": "path_value", "port": 453}],
         "degraded": True,
         "conditions": [
             {
                 "code": 411,
                 "message": "message_value",
                 "details": [
                     {
                         "type_url": "type.googleapis.com/google.protobuf.Duration",
                         "value": b"\x08\x0c\x10\xdb\x07",
                     }
                 ],
             }
         ],
+        "enable_audit_agent": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -9673,22 +9693,24 @@
         "running_timeout": {},
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
+                "pooled_instances": 1706,
                 "disable_public_ip_addresses": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
+                "accelerators": [{"type_": "type__value", "count": 553}],
             }
         },
         "persistent_directories": [
             {
                 "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
@@ -9707,27 +9729,29 @@
             "working_dir": "working_dir_value",
             "run_as_user": 1190,
         },
         "encryption_key": {
             "kms_key": "kms_key_value",
             "kms_key_service_account": "kms_key_service_account_value",
         },
+        "readiness_checks": [{"path": "path_value", "port": 453}],
         "degraded": True,
         "conditions": [
             {
                 "code": 411,
                 "message": "message_value",
                 "details": [
                     {
                         "type_url": "type.googleapis.com/google.protobuf.Duration",
                         "value": b"\x08\x0c\x10\xdb\x07",
                     }
                 ],
             }
         ],
+        "enable_audit_agent": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -9840,22 +9864,24 @@
         "running_timeout": {},
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
+                "pooled_instances": 1706,
                 "disable_public_ip_addresses": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
+                "accelerators": [{"type_": "type__value", "count": 553}],
             }
         },
         "persistent_directories": [
             {
                 "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
@@ -9874,27 +9900,29 @@
             "working_dir": "working_dir_value",
             "run_as_user": 1190,
         },
         "encryption_key": {
             "kms_key": "kms_key_value",
             "kms_key_service_account": "kms_key_service_account_value",
         },
+        "readiness_checks": [{"path": "path_value", "port": 453}],
         "degraded": True,
         "conditions": [
             {
                 "code": 411,
                 "message": "message_value",
                 "details": [
                     {
                         "type_url": "type.googleapis.com/google.protobuf.Duration",
                         "value": b"\x08\x0c\x10\xdb\x07",
                     }
                 ],
             }
         ],
+        "enable_audit_agent": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -10102,22 +10130,24 @@
         "running_timeout": {},
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
+                "pooled_instances": 1706,
                 "disable_public_ip_addresses": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
+                "accelerators": [{"type_": "type__value", "count": 553}],
             }
         },
         "persistent_directories": [
             {
                 "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
@@ -10136,27 +10166,29 @@
             "working_dir": "working_dir_value",
             "run_as_user": 1190,
         },
         "encryption_key": {
             "kms_key": "kms_key_value",
             "kms_key_service_account": "kms_key_service_account_value",
         },
+        "readiness_checks": [{"path": "path_value", "port": 453}],
         "degraded": True,
         "conditions": [
             {
                 "code": 411,
                 "message": "message_value",
                 "details": [
                     {
                         "type_url": "type.googleapis.com/google.protobuf.Duration",
                         "value": b"\x08\x0c\x10\xdb\x07",
                     }
                 ],
             }
         ],
+        "enable_audit_agent": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -11535,14 +11567,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "state": 1,
         "host": "host_value",
+        "env": {},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -11759,14 +11792,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "state": 1,
         "host": "host_value",
+        "env": {},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -11873,14 +11907,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "state": 1,
         "host": "host_value",
+        "env": {},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -12082,14 +12117,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "state": 1,
         "host": "host_value",
+        "env": {},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
```

