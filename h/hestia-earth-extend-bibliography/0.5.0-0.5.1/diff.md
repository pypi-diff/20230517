# Comparing `tmp/hestia-earth-extend-bibliography-0.5.0.tar.gz` & `tmp/hestia-earth-extend-bibliography-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-extend-bibliography-0.5.0.tar", last modified: Thu May  4 09:15:48 2023, max compression
+gzip compressed data, was "hestia-earth-extend-bibliography-0.5.1.tar", last modified: Wed May 17 14:29:58 2023, max compression
```

## Comparing `hestia-earth-extend-bibliography-0.5.0.tar` & `hestia-earth-extend-bibliography-0.5.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.479329 hestia-earth-extend-bibliography-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-04 09:15:48.480318 hestia-earth-extend-bibliography-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      754 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.468456 hestia-earth-extend-bibliography-0.5.0/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.469445 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/
--rw-rw-rw-   0 root         (0) root         (0)    10025 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.471422 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4225 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/crossref.py
--rw-rw-rw-   0 root         (0) root         (0)     2050 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.472410 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2266 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.472410 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3111 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/client.py
--rw-rw-rw-   0 root         (0) root         (0)     4376 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/unpaywall.py
--rw-rw-rw-   0 root         (0) root         (0)     4352 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.473399 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.473399 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/log.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.475376 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-04 09:15:48.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2088 2023-05-04 09:15:48.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-04 09:15:48.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-04 09:15:48.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-04 09:15:48.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-04 09:15:48.480318 hestia-earth-extend-bibliography-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1005 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.465491 hestia-earth-extend-bibliography-0.5.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.477352 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.477352 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1208 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_api/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.478341 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_sdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_sdk/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_crossref.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_mendeley.py
--rw-rw-rw-   0 root         (0) root         (0)     2101 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_unpaywall.py
--rw-rw-rw-   0 root         (0) root         (0)     2159 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_wos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.479329 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_rest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_rest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_rest/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.479329 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_soap/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_soap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_soap/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.905905 hestia-earth-extend-bibliography-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-17 14:29:58.905905 hestia-earth-extend-bibliography-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      754 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.893904 hestia-earth-extend-bibliography-0.5.1/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.894904 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/
+-rw-rw-rw-   0 root         (0) root         (0)    10025 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.896904 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4225 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/crossref.py
+-rw-rw-rw-   0 root         (0) root         (0)     2050 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.897904 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.898904 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3014 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4376 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/unpaywall.py
+-rw-rw-rw-   0 root         (0) root         (0)     4352 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/wos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.898904 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.899904 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/log.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.901904 hestia-earth-extend-bibliography-0.5.1/hestia_earth_extend_bibliography.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-17 14:29:58.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth_extend_bibliography.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-05-17 14:29:58.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth_extend_bibliography.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-17 14:29:58.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth_extend_bibliography.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-17 14:29:58.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth_extend_bibliography.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-17 14:29:58.000000 hestia-earth-extend-bibliography-0.5.1/hestia_earth_extend_bibliography.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-17 14:29:58.906905 hestia-earth-extend-bibliography-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.890903 hestia-earth-extend-bibliography-0.5.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.903905 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.903905 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/mendeley_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/mendeley_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/mendeley_api/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.904905 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/mendeley_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/mendeley_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/mendeley_sdk/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/test_crossref.py
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/test_mendeley.py
+-rw-rw-rw-   0 root         (0) root         (0)     2101 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/test_unpaywall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2159 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/test_wos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.905905 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/wos_rest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/wos_rest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/wos_rest/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:29:58.905905 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/wos_soap/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/wos_soap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2023-05-17 14:29:38.000000 hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/wos_soap/test_client.py
```

### Comparing `hestia-earth-extend-bibliography-0.5.0/LICENSE` & `hestia-earth-extend-bibliography-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/PKG-INFO` & `hestia-earth-extend-bibliography-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-extend-bibliography
-Version: 0.5.0
+Version: 0.5.1
 Summary: Hestia library to extend Bibliography Nodes with different APIs
 Home-page: https://gitlab.com/hestia-earth/hestia-data-validation
 Author: Guillaume Royer
 Author-email: guillaumeroyer.mail@gmail.com
 License: MIT
 Keywords: hestia,mendeley
 Platform: UNKNOWN
```

### Comparing `hestia-earth-extend-bibliography-0.5.0/README.md` & `hestia-earth-extend-bibliography-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/__init__.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/crossref.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/crossref.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/client.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/client.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from mendeley import Mendeley
 from hestia_earth.schema import Bibliography
 
-from hestia_earth.extend_bibliography.bibliography_apis.utils import ORINGAL_FIELD, extend_bibliography, capitalize, \
-    update_actor_names
+from hestia_earth.extend_bibliography.bibliography_apis.utils import (
+    ORINGAL_FIELD, extend_bibliography, capitalize, update_actor_names
+)
+from .session import get_session
 
 
 def _author_to_actor(author):
     return update_actor_names({
         'firstName': capitalize(author.first_name),
         'lastName': capitalize(author.last_name),
         'scopusID': author.scopus_author_id
@@ -72,11 +73,8 @@
 }
 
 
 def exec_search(session, key: str): return lambda value: SEARCH_BY_KEY[key](session, value.rstrip())
 
 
 def get_client(**kwargs):
-    mendel = Mendeley(client_id=int(kwargs.get('mendeley_username')), client_secret=kwargs.get('mendeley_password'))
-    auth = mendel.start_client_credentials_flow()
-    session = auth.authenticate()
-    return session
+    return get_session(client_id=int(kwargs.get('mendeley_username')), client_secret=kwargs.get('mendeley_password'))
```

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/unpaywall.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/unpaywall.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/utils.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/wos.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/client.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/client.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/log.py` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth/extend_bibliography/log.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/PKG-INFO` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth_extend_bibliography.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-extend-bibliography
-Version: 0.5.0
+Version: 0.5.1
 Summary: Hestia library to extend Bibliography Nodes with different APIs
 Home-page: https://gitlab.com/hestia-earth/hestia-data-validation
 Author: Guillaume Royer
 Author-email: guillaumeroyer.mail@gmail.com
 License: MIT
 Keywords: hestia,mendeley
 Platform: UNKNOWN
```

### Comparing `hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/SOURCES.txt` & `hestia-earth-extend-bibliography-0.5.1/hestia_earth_extend_bibliography.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 hestia_earth/extend_bibliography/bibliography_apis/unpaywall.py
 hestia_earth/extend_bibliography/bibliography_apis/utils.py
 hestia_earth/extend_bibliography/bibliography_apis/wos.py
 hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/__init__.py
 hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/client.py
 hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/__init__.py
 hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/client.py
+hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/session.py
 hestia_earth/extend_bibliography/bibliography_apis/wos_rest/__init__.py
 hestia_earth/extend_bibliography/bibliography_apis/wos_rest/client.py
 hestia_earth/extend_bibliography/bibliography_apis/wos_soap/__init__.py
 hestia_earth/extend_bibliography/bibliography_apis/wos_soap/client.py
 hestia_earth_extend_bibliography.egg-info/PKG-INFO
 hestia_earth_extend_bibliography.egg-info/SOURCES.txt
 hestia_earth_extend_bibliography.egg-info/dependency_links.txt
```

### Comparing `hestia-earth-extend-bibliography-0.5.0/setup.py` & `hestia-earth-extend-bibliography-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_api/test_client.py` & `hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/mendeley_api/test_client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_sdk/test_client.py` & `hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/mendeley_sdk/test_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from unittest.mock import patch
 import json
 import pickle
 
 from tests.utils import fixtures_path, get_citations, clean_bibliography
-from hestia_earth.extend_bibliography.bibliography_apis.mendeley_sdk.client import get_client, exec_search, \
+from hestia_earth.extend_bibliography.bibliography_apis.mendeley_sdk.client import (
+    get_client, exec_search,
     create_biblio
+)
 
 file_content = b"{}"
 
 
 class FakeMendeleySearch():
     def list(self, *args):
         with open(f"{fixtures_path}/mendeley-sdk/result.pickle", 'rb') as f:
```

### Comparing `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_crossref.py` & `hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/test_crossref.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_mendeley.py` & `hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/test_mendeley.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_unpaywall.py` & `hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/test_unpaywall.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_utils.py` & `hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/test_utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_wos.py` & `hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/test_wos.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_rest/test_client.py` & `hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/wos_rest/test_client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_soap/test_client.py` & `hestia-earth-extend-bibliography-0.5.1/tests/bibliography_apis/wos_soap/test_client.py`

 * *Files identical despite different names*

