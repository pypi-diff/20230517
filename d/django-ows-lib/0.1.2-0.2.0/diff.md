# Comparing `tmp/django-ows-lib-0.1.2.tar.gz` & `tmp/django-ows-lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ows-lib-0.1.2.tar", last modified: Tue May 16 05:25:33 2023, max compression
+gzip compressed data, was "django-ows-lib-0.2.0.tar", last modified: Wed May 17 06:21:11 2023, max compression
```

## Comparing `django-ows-lib-0.1.2.tar` & `django-ows-lib-0.2.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.077010 django-ows-lib-0.1.2/django_ows_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-16 05:25:33.000000 django-ows-lib-0.1.2/django_ows_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-16 05:25:33.000000 django-ows-lib-0.1.2/django_ows_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:25:33.000000 django-ows-lib-0.1.2/django_ows_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 05:25:33.000000 django-ows-lib-0.1.2/django_ows_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 05:25:33.000000 django-ows-lib-0.1.2/django_ows_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.077010 django-ows-lib-0.1.2/ows_lib/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.077010 django-ows-lib-0.1.2/ows_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.077010 django-ows-lib-0.1.2/ows_lib/client/csw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/csw/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.077010 django-ows-lib-0.1.2/ows_lib/client/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.077010 django-ows-lib-0.1.2/ows_lib/client/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/client/wms/wms130.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.077010 django-ows-lib-0.1.2/ows_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/models/ogc_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/csw/
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wms/wms130.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/gml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/gml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/gml/gml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/iso_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/iso_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_requests/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/csw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/csw/get_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 05:25:33.081010 django-ows-lib-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-16 05:25:31.000000 django-ows-lib-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/django_ows_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/django_ows_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/django_ows_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/django_ows_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/django_ows_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/django_ows_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/client/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/csw/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/client/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/client/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/client/wms/wms130.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/models/ogc_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/xml_mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.450641 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/wms130.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/gml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/gml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/gml/gml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/iso_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/iso_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 06:21:11.454641 django-ows-lib-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-17 06:21:11.000000 django-ows-lib-0.2.0/setup.py
```

### Comparing `django-ows-lib-0.1.2/LICENSE` & `django-ows-lib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/PKG-INFO` & `django-ows-lib-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.1.2
+Version: 0.2.0
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-ows-lib-0.1.2/README.rst` & `django-ows-lib-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/django_ows_lib.egg-info/PKG-INFO` & `django-ows-lib-0.2.0/django_ows_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.1.2
+Version: 0.2.0
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-ows-lib-0.1.2/django_ows_lib.egg-info/SOURCES.txt` & `django-ows-lib-0.2.0/django_ows_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/client/csw/mixins.py` & `django-ows-lib-0.2.0/ows_lib/client/csw/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/client/enums.py` & `django-ows-lib-0.2.0/ows_lib/client/enums.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/client/exceptions.py` & `django-ows-lib-0.2.0/ows_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/client/mixins.py` & `django-ows-lib-0.2.0/ows_lib/client/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/client/utils.py` & `django-ows-lib-0.2.0/ows_lib/client/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/client/wfs/mixins.py` & `django-ows-lib-0.2.0/ows_lib/client/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/client/wms/mixins.py` & `django-ows-lib-0.2.0/ows_lib/client/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/models/ogc_request.py` & `django-ows-lib-0.2.0/ows_lib/models/ogc_request.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/csw/csw202.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/csw/csw202.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/mixins.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wfs/mixins.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wfs/wfs200.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wms/mixins.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wms/wms111.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/wms111.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/capabilities/wms/wms130.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/capabilities/wms/wms130.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/iso_metadata/iso_metadata.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,45 +43,59 @@
 
 class EXGeographicBoundingBox(xmlmap.XmlObject):
     ROOT_NS = GMD_NAMESPACE
     ROOT_NAME = "EX_GeographicBoundingBox"
     ROOT_NAMESPACES = dict([("gmd", GMD_NAMESPACE),
                             ("gco", GCO_NAMESPACE)])
 
-    min_x = xmlmap.FloatField(xpath="gmd:westBoundLongitude/gco:Decimal")
-    max_x = xmlmap.FloatField(xpath="gmd:eastBoundLongitude/gco:Decimal")
-    min_y = xmlmap.FloatField(xpath="gmd:southBoundLatitude/gco:Decimal")
-    max_y = xmlmap.FloatField(xpath="gmd:northBoundLatitude/gco:Decimal")
-
-    def to_polygon(self):
-        if self.min_x and self.max_x and self.min_y and self.max_y:
-            return GeosPolygon(((self.min_x, self.min_y),
-                               (self.min_x, self.max_y),
-                               (self.max_x, self.max_y),
-                               (self.max_x, self.min_y),
-                               (self.min_x, self.min_y)))
+    _min_x = xmlmap.FloatField(xpath="gmd:westBoundLongitude/gco:Decimal")
+    _max_x = xmlmap.FloatField(xpath="gmd:eastBoundLongitude/gco:Decimal")
+    _min_y = xmlmap.FloatField(xpath="gmd:southBoundLatitude/gco:Decimal")
+    _max_y = xmlmap.FloatField(xpath="gmd:northBoundLatitude/gco:Decimal")
+
+    @property
+    def geometry(self) -> GeosPolygon:
+        if self._min_x and self._max_x and self._min_y and self._max_y:
+            return GeosPolygon(((self._min_x, self._min_y),
+                               (self._min_x, self._max_y),
+                               (self._max_x, self._max_y),
+                               (self._max_x, self._min_y),
+                               (self._min_x, self._min_y)))
+
+    @geometry.setter
+    def geometry(self, value: GeosPolygon):
+        self._min_x = value.extent[0]
+        self._min_y = value.extent[1]
+        self._max_x = value.extent[2]
+        self._max_y = value.extent[3]
 
 
 class EXBoundingPolygon(xmlmap.XmlObject):
     ROOT_NS = GMD_NAMESPACE
     ROOT_NAME = "EX_BoundingPolygon"
     ROOT_NAMESPACES = dict([("gmd", GMD_NAMESPACE)])
 
-    geometry_list = xmlmap.NodeListField(xpath="gmd:polygon",
-                                         node_class=Gml)
+    _geometry_list = xmlmap.NodeListField(xpath="gmd:polygon",
+                                          node_class=Gml)
 
-    def get_geometries(self):
+    @property
+    def geometries(self) -> MultiPolygon:
         """Return all founded gml geometries as a list of geos geometries.
-        :return: a list of geos geometries
-        :rtype: list
+        :return: 
+        :rtype: MultiPolygon
         """
         geometries = []
-        for geometry in self.geometry_list:
-            geometries.append(geometry.to_gml())
-        return geometries
+        for geometry in self._geometry_list:
+            geometries.append(geometry.to_geometry())
+        return MultiPolygon(geometries)
+
+    @geometries.setter
+    def geometries(self, value):
+        # TODO
+        raise NotImplementedError()
 
 
 class ReferenceSystem(CustomXmlObject, xmlmap.XmlObject):
     ROOT_NAMESPACES = dict([("gmd", GMD_NAMESPACE),
                             ("gco", GCO_NAMESPACE)])
 
     ref_system = xmlmap.StringField(xpath="gmd:code/gco:CharacterString")
@@ -122,100 +136,80 @@
        This class is intended mostly for internal use, but could be
        useful when extending or adding additional ISO Metadata
        :class:`~eulxml.xmlmap.XmlObject` classes.  The
        :attr:`GMD_NAMESPACE` is mapped to the prefix **gmd**.
        :attr:`GCO_NAMESPACE` is mapped to the prefix **gco**.
     """
     ROOT_NS = GMD_NAMESPACE
-    ROOT_NAMESPACES = dict([("gmd", GMD_NAMESPACE),
-                            ("gco", GCO_NAMESPACE)])
+    ROOT_NAMESPACES = {
+        "gmd": GMD_NAMESPACE,
+        "gco": GCO_NAMESPACE,
+    }
 
 
 class BasicInformation(BaseIsoMetadata):
     title = xmlmap.StringField(
         xpath="gmd:citation/gmd:CI_Citation/gmd:title/gco:CharacterString")
     abstract = xmlmap.StringField(xpath="gmd:abstract/gco:CharacterString")
     access_constraints = xmlmap.StringField(
         xpath="gmd:resourceConstraints/gmd:MD_LegalConstraints[gmd:accessConstraints/gmd:MD_RestrictionCode/@codeListValue=\"otherRestrictions\"]/gmd:otherConstraints/gco:CharacterString")
     # dataset specific fields
-    code_md = xmlmap.StringField(
+    _code_md = xmlmap.StringField(
         xpath="gmd:citation/gmd:CI_Citation/gmd:identifier/gmd:MD_Identifier/gmd:code/gco:CharacterString")
-    code_rs = xmlmap.StringField(
+    _code_rs = xmlmap.StringField(
         xpath="gmd:citation/gmd:CI_Citation/gmd:identifier/gmd:RS_Identifier/gmd:code/gco:CharacterString")
-    code_space_rs = xmlmap.StringField(
+    _code_space_rs = xmlmap.StringField(
         xpath="gmd:citation/gmd:CI_Citation/gmd:identifier/gmd:RS_Identifier/gmd:codeSpace/gco:CharacterString")
 
     # character_set_code = xmlmap.StringField(xpath=f"{NS_WC}characterSet']/{NS_WC}MD_CharacterSetCode']/@codeListValue")
 
     dataset_contact = xmlmap.NodeField(xpath="gmd:pointOfContact/gmd:CI_ResponsibleParty",
                                        node_class=CiResponsibleParty)
     keywords = xmlmap.NodeListField(xpath="gmd:descriptiveKeywords/gmd:MD_Keywords/gmd:keyword",
                                     node_class=Keyword)
 
-    def get_bounding_geometry(self):
-        polygon_list = []
-        for bbox in self.bbox_lat_lon_list:  # noqa xmlmap.NodeListField provide iterator
-            polygon_list.append(bbox.to_polygon())
-        for polygon in self.bounding_polygon_list:  # noqa xmlmap.NodeListField provide iterator
-            polygon_list.extend(polygon.get_geometries())
-        return MultiPolygon(polygon_list)
-
-    def get_spatial_res(self, field_dict):
-        if self.equivalent_scale is not None and self.equivalent_scale > 0:
-            field_dict["spatial_res_value"] = self.equivalent_scale
-            field_dict["spatial_res_type"] = "scaleDenominator"
-        elif self.ground_res is not None and self.ground_res > 0:
-            field_dict["spatial_res_value"] = self.ground_res
-            field_dict["spatial_res_type"] = "groundDistance"
-        field_dict.pop("equivalent_scale", None)
-        field_dict.pop("ground_res", None)
-
-    def get_dataset_id(self, field_dict):
-        if field_dict.get("code_md", None):
-            code = field_dict["code_md"]
+    is_broken = False  # flag to signal that this metadata object has integrity error
+
+    def _parse_identifier(self):
+        _dataset_id = ""
+        _code_space = ""
+        if self._code_md:
             # new implementation:
             # http://inspire.ec.europa.eu/file/1705/download?token=iSTwpRWd&usg=AOvVaw18y1aTdkoMCBxpIz7tOOgu
             # from 2017-03-02 - the MD_Identifier - see C.2.5 Unique resource identifier - it is separated with a slash
             # - the codes pace should be everything after the last slash
             # now try to check if a single slash is available and if the md_identifier is a url
-            parsed_url = urllib.parse.urlsplit(code)
+            parsed_url = urllib.parse.urlsplit(self._code_md)
             if parsed_url.scheme == "http" or parsed_url.scheme == "https" and "/" in parsed_url.path:
-                tmp = code.split("/")
-                field_dict["dataset_id"] = tmp[len(tmp) - 1]
-                field_dict["dataset_id_code_space"] = code.replace(
-                    field_dict["dataset_id"], "")
-            elif parsed_url.scheme == "http" or parsed_url.scheme == "https" and "#" in code:
-                tmp = code.split("#")
-                field_dict["dataset_id"] = tmp[1]
-                field_dict["dataset_id_code_space"] = tmp[0]
+                tmp = self._code_md.split("/")
+                _dataset_id = tmp[len(tmp) - 1]
+                _code_space = self._code_md.replace(_dataset_id, "")
+            elif parsed_url.scheme == "http" or parsed_url.scheme == "https" and "#" in self._code_md:
+                tmp = self._code_md.split("#")
+                _dataset_id = tmp[1]
+                _code_space = tmp[0]
             else:
-                field_dict["dataset_id"] = code
-                field_dict["dataset_id_code_space"] = ""
-            del field_dict["code_md"]
-
-        elif field_dict.get("code_rs", None):
+                _dataset_id = self._code_md
+                _code_space = ""
+        elif self._code_rs:
             # try to read code from RS_Identifier
-            code = field_dict["code_rs"]
-            code_space = field_dict["code_space_rs"]
-            if code_space is not None and code is not None and len(code_space) > 0 and len(code) > 0:
-                field_dict["dataset_id"] = code
-                field_dict["dataset_id_code_space"] = code_space
+            if self._code_space_rs is not None and self._code_rs is not None and len(self._code_space_rs) > 0 and len(self._code_rs) > 0:
+                _dataset_id = self._code_rs
+                _code_space = self._code_space_rs
             else:
-                field_dict["is_broken"] = True
-            del field_dict["code_rs"]
-
-        field_dict.pop("code_space_rs", None)
+                self.is_broken = True
+        return _dataset_id.replace('\n', '').strip(), _code_space.replace('\n', '').strip()
 
-    def get_date_stamp(self, field_dict):
-        date = field_dict.pop("date_stamp_date", None)
-        date_time = field_dict.pop("date_stamp_date_time", None)
-        if date:
-            field_dict.update({"date_stamp": date})
-        elif date_time:
-            field_dict.update({"date_stamp": date_time})
+    @property
+    def dataset_id(self) -> str:
+        return self._parse_identifier()[0]
+
+    @property
+    def dataset_id_code_space(self) -> str:
+        return self._parse_identifier()[1]
 
 
 class MdDataIdentification(BasicInformation):
     ROOT_NAME = "MD_DataIdentification"
     equivalent_scale = xmlmap.FloatField(
         xpath="gmd:spatialResolution/gmd:MD_Resolution/gmd:equivalentScale/gmd:MD_RepresentativeFraction/gmd:denominator/gco:Integer")
     ground_res = xmlmap.FloatField(
@@ -227,32 +221,40 @@
     bounding_polygon_list = xmlmap.NodeListField(xpath="gmd:extent/gmd:EX_Extent/gmd:geographicElement/gmd:EX_BoundingPolygon",
                                                  node_class=EXBoundingPolygon)
     dimensions = xmlmap.NodeListField(xpath="gmd:extent/gmd:EX_Extent/gmd:temporalElement/gmd:EX_TemporalExtent/gmd:extent",
                                       node_class=Dimension)
 
 
 class SvOperationMetadata(BasicInformation):
+    ROOT_NS = SRV_NAMESPACE
     ROOT_NAME = "SV_OperationMetadata"
-    ROOT_NAMESPACES = dict([("gmd", GMD_NAMESPACE),
-                            ("gco", GCO_NAMESPACE),
-                            ("srv", SRV_NAMESPACE)])
+    ROOT_NAMESPACES = {
+        "gmd": GMD_NAMESPACE,
+        "gco": GCO_NAMESPACE,
+        "srv": SRV_NAMESPACE
+    }
+
     # mandatory fields
     operation = xmlmap.StringField(
         xpath="svr:operationName/gco:characterString")
     dcp = xmlmap.StringListField(
         xpath="srv:DCP/srv:DCPList[codeList='http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/ML_gmxCodelists.xml#DCPList']/@codeListValue")
     url = xmlmap.StringListField(
         xpath="srv:connectPoint/gmd:CI_OnlineResource/gmd:linkage/gmd:URL")
 
 
 class SvServiceIdentification(BaseIsoMetadata):
+    ROOT_NS = GMD_NAMESPACE
     ROOT_NAME = "SV_ServiceIdentification"
-    ROOT_NAMESPACES = dict([("gmd", GMD_NAMESPACE),
-                            ("gco", GCO_NAMESPACE),
-                            ("srv", SRV_NAMESPACE)])
+    ROOT_NAMESPACES = {
+        "gmd": GMD_NAMESPACE,
+        "gco": GCO_NAMESPACE,
+        "srv": SRV_NAMESPACE
+    }
+
     # mandatory fields
     service_type = xmlmap.StringField(xpath="srv:serviceType/gco:LocalName")
     coupling_type = xmlmap.StringField(
         xpath="srv:couplingType/srv:SV_CouplingType[@codeList='SV_CouplingType']/@codeListValue")
     contains_operations = xmlmap.NodeListField(xpath="srv:containsOperations/svr:SV_OperationMetadata",
                                                node_class=SvOperationMetadata)
     # optional fields
@@ -261,87 +263,125 @@
     bbox_lat_lon_list = xmlmap.NodeListField(xpath="srv:extent/gmd:EX_Extent/gmd:geographicElement/gmd:EX_GeographicBoundingBox",
                                              node_class=EXGeographicBoundingBox)
     bounding_polygon_list = xmlmap.NodeListField(xpath="srv:extent/gmd:EX_Extent/gmd:geographicElement/gmd:EX_BoundingPolygon",
                                                  node_class=EXBoundingPolygon)
     dimensions = xmlmap.NodeListField(xpath="srv:extent/gmd:EX_Extent/gmd:temporalElement/gmd:EX_TemporalExtent/gmd:extent",
                                       node_class=Dimension)
 
+    equivalent_scale = xmlmap.FloatField(
+        xpath="srv:spatialResolution/gmd:MD_Resolution/gmd:equivalentScale/gmd:MD_RepresentativeFraction/gmd:denominator/gco:Integer")
+    ground_res = xmlmap.FloatField(
+        xpath="srv:spatialResolution/gmd:MD_Resolution/gmd:distance/gco:Distance")
+
 
 class MdMetadata(BaseIsoMetadata):
     """XML mapper class to deserialize/serialize metadata information defined in the ISO 19115 specs.
 
-    :Example:
-
-    .. code-block:: python
-       from registry.parsers.iso import iso_metadata
-
-       # iso metadata from scratch
-       iso_md = iso_metadata.IsoMetadata()
-       iso_md = file_identifier = "4be3fcf9-9376-4813-9bfd-708912038635"
-       iso_md.hierarchy_level = "dataset"
-       ...
-       iso_md.serializeDocument()  # to get the serialized xml document
-
-       # iso metadata from other object. All field names which shall be initiated shall have the same name.
-       iso_md = IsoMetadata.from_dict({"file_identifier": "4be3fcf9-9376-4813-9bfd-708912038635",
-                                       "hierarchy_level": "dataset", ... })
-       iso_md.serializeDocument()  # to get the serialized xml document
-
     """
+    XSD_SCHEMA = "http://www.isotc211.org/2005/gmd"  # NOSONAR: the xml schema url will still be with insecure http protocol. To match all xml files, we need to let it as it is.
+
     ROOT_NAME = "MD_Metadata"
     ROOT_NS = GMD_NAMESPACE
+    ROOT_NAMESPACES = {
+        "gmd": GMD_NAMESPACE,
+    }
 
     file_identifier = xmlmap.StringField(
         xpath="gmd:fileIdentifier/gco:CharacterString")
     # language = xmlmap.StringField(xpath=f"{NS_WC}identificationInfo']//{NS_WC}language']/{NS_WC}LanguageCode']")
-    hierarchy_level = xmlmap.StringField(
+    _hierarchy_level = xmlmap.StringField(
         xpath="gmd:hierarchyLevel/gmd:MD_ScopeCode[@codeList='http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/ML_gmxCodelists.xml#MD_ScopeCode']/@codeListValue")
-    date_stamp_date = xmlmap.DateField(xpath="gmd:dateStamp/gco:Date")
-    date_stamp_date_time = xmlmap.DateTimeField(
+    _date_stamp_date = xmlmap.DateField(xpath="gmd:dateStamp/gco:Date")
+    _date_stamp_date_time = xmlmap.DateTimeField(
         xpath="gmd:dateStamp/gco:DateTime")
     metadata_contact = xmlmap.NodeField(
         xpath="gmd:contact/gmd:CI_ResponsibleParty", node_class=CiResponsibleParty)
     reference_systems = xmlmap.NodeListField(
         xpath="gmd:referenceSystemInfo/gmd:MD_ReferenceSystem/gmd:referenceSystemIdentifier/gmd:RS_Identifier", node_class=ReferenceSystem)
 
-    md_data_identification = xmlmap.NodeField(xpath="gmd:identificationInfo/gmd:MD_DataIdentification",
-                                              node_class=MdDataIdentification)
-    sv_service_identification = xmlmap.NodeField(xpath="gmd:identificationInfo/gmd:SV_ServiceIdentification",
-                                                 node_class=SvServiceIdentification)
-
-    def get_field_dict(self):
-        """Custom function to convert xml object to database model schema.
-
-        :return: all attributes in db model structure
-        :rtype: dict
-        """
-        field_dict = super().get_field_dict()
-        if self.md_data_identification:
-            field_dict["bounding_geometry"] = self.md_data_identification.get_bounding_geometry()
-            field_dict.update(self.md_data_identification.get_field_dict())
-            self.md_data_identification.get_spatial_res(field_dict=field_dict)
-            self.md_data_identification.get_dataset_id(field_dict=field_dict)
-            self.md_data_identification.get_date_stamp(field_dict=field_dict)
-        elif self.sv_service_identification:
-            field_dict["bounding_geometry"] = self.sv_service_identification.get_bounding_geometry()
-            field_dict.update(self.sv_service_identification.get_field_dict())
-            self.sv_service_identification.get_spatial_res(
-                field_dict=field_dict)
-            self.sv_service_identification.get_dataset_id(
-                field_dict=field_dict)
-            self.sv_service_identification.get_date_stamp(
-                field_dict=field_dict)
-        # no database field. So we drop it here.
-        field_dict.pop("hierarchy_level", None)
-        return field_dict
+    _md_data_identification = xmlmap.NodeField(xpath="gmd:identificationInfo/gmd:MD_DataIdentification",
+                                               node_class=MdDataIdentification)
+    _sv_service_identification = xmlmap.NodeField(xpath="gmd:identificationInfo/gmd:SV_ServiceIdentification",
+                                                  node_class=SvServiceIdentification)
+
+    def _get_child_identification(self):
+        if self._md_data_identification:
+            return self._md_data_identification
+        elif self._sv_service_identification:
+            return self._sv_service_identification
+
+    @property
+    def date_stamp(self):
+        return self._date_stamp_date if self._date_stamp_date else self._date_stamp_date_time
+
+    @date_stamp.setter
+    def date_stamp(self, value):
+        # TODO
+        raise NotImplementedError()
+
+    @property
+    def bounding_geometry(self):
+        child = self._get_child_identification()
+        if child:
+            polygon_list = []
+            for bbox in child.bbox_lat_lon_list:
+                polygon_list.append(bbox.geometry)
+            for polygon in child.bounding_polygon_list:
+                polygon_list.extend(polygon.geometries)
+            return MultiPolygon(polygon_list)
+
+    @bounding_geometry.setter
+    def bounding_geometry(self, value: MultiPolygon):
+        bbox = value.convex_hull
+        bounding_polygons = value
+        # TODO
+        raise NotImplementedError()
+
+    def get_spatial_res(self):
+        child = self._get_child_identification()
+        if child:
+            if child.equivalent_scale is not None and child.equivalent_scale > 0:
+                return child.equivalent_scale, "scaleDenominator"
+            elif self.ground_res is not None and self.ground_res > 0:
+                return child.ground_res, "groundDistance"
+
+    @property
+    def spatial_res_type(self):
+        return self.get_spatial_res()[0]
+
+    @spatial_res_type.setter
+    def spatial_res_type(self, value):
+        # TODO
+        raise NotImplementedError()
+
+    @property
+    def spatial_res_value(self):
+        return self.get_spatial_res()[1]
+
+    @spatial_res_value.setter
+    def spatial_res_value(self, value):
+        # TODO
+        raise NotImplementedError()
+
+    @property
+    def dataset_id(self) -> str:
+        child = self._get_child_identification()
+        if child:
+            return child.dataset_id
+
+    @property
+    def dataset_id_code_space(self) -> str:
+        child = self._get_child_identification()
+        if child:
+            return child.dataset_id_code_space
 
 
 class WrappedIsoMetadata(xmlmap.XmlObject):
     """Helper class to parse wrapped IsoMetadata objects.
 
-    This class is needed you want to parse GetRecordsResponse xml for example. There are 0..n ``gmd:MD_Metadata``
+    This class is needed if you want to parse GetRecordsResponse xml for example. There are 0..n ``gmd:MD_Metadata``
     nodes wrapped by a ``csw:GetRecordsResponse`` node.
     """
-    ROOT_NAMESPACES = dict([("gmd", GMD_NAMESPACE)])
+    ROOT_NAMESPACES = {"gmd": GMD_NAMESPACE}
 
     iso_metadata = xmlmap.NodeListField(
         xpath="//gmd:MD_Metadata", node_class=MdMetadata)
```

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/mixins.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/namespaces.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/namespaces.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/utils.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/csw/get_records.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py` & `django-ows-lib-0.2.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.2/setup.py` & `django-ows-lib-0.2.0/setup.py`

 * *Files identical despite different names*

