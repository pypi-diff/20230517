# Comparing `tmp/openedx-events-7.3.0.tar.gz` & `tmp/openedx-events-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-7.3.0.tar", last modified: Mon May 15 15:26:52 2023, max compression
+gzip compressed data, was "openedx-events-8.0.0.tar", last modified: Wed May 17 12:15:18 2023, max compression
```

## Comparing `openedx-events-7.3.0.tar` & `openedx-events-8.0.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.046973 openedx-events-7.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     8734 2023-05-15 15:26:45.000000 openedx-events-7.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-15 15:26:45.000000 openedx-events-7.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-15 15:26:45.000000 openedx-events-7.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14760 2023-05-15 15:26:52.046973 openedx-events-7.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-05-15 15:26:45.000000 openedx-events-7.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.042973 openedx-events-7.3.0/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.042973 openedx-events-7.3.0/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.042973 openedx-events-7.3.0/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (122)     7436 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.046973 openedx-events-7.3.0/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.046973 openedx-events-7.3.0/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4973 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (122)    11058 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     8803 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.046973 openedx-events-7.3.0/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.046973 openedx-events-7.3.0/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8297 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5664 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.046973 openedx-events-7.3.0/openedx_events/management/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.046973 openedx-events-7.3.0/openedx_events/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/management/commands/consume_events.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.046973 openedx-events-7.3.0/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/tests/test_consume_events_command.py
--rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-05-15 15:26:45.000000 openedx-events-7.3.0/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.042973 openedx-events-7.3.0/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14760 2023-05-15 15:26:52.000000 openedx-events-7.3.0/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-15 15:26:52.000000 openedx-events-7.3.0/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 15:26:52.000000 openedx-events-7.3.0/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 15:26:52.000000 openedx-events-7.3.0/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-15 15:26:52.000000 openedx-events-7.3.0/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-15 15:26:52.000000 openedx-events-7.3.0/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.046973 openedx-events-7.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-15 15:26:45.000000 openedx-events-7.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-15 15:26:52.046973 openedx-events-7.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-05-15 15:26:45.000000 openedx-events-7.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:26:52.046973 openedx-events-7.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-15 15:26:45.000000 openedx-events-7.3.0/tests/test_openedx_events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.339470 openedx-events-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     8888 2023-05-17 12:15:13.000000 openedx-events-8.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-17 12:15:13.000000 openedx-events-8.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-17 12:15:13.000000 openedx-events-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14914 2023-05-17 12:15:18.339470 openedx-events-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-05-17 12:15:13.000000 openedx-events-8.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.327469 openedx-events-8.0.0/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.331470 openedx-events-8.0.0/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.331470 openedx-events-8.0.0/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (122)     7236 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.331470 openedx-events-8.0.0/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.335470 openedx-events-8.0.0/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4973 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11058 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8803 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.335470 openedx-events-8.0.0/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.335470 openedx-events-8.0.0/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8297 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5664 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.335470 openedx-events-8.0.0/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.335470 openedx-events-8.0.0/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/management/commands/consume_events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.339470 openedx-events-8.0.0/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-05-17 12:15:13.000000 openedx-events-8.0.0/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.327469 openedx-events-8.0.0/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14914 2023-05-17 12:15:18.000000 openedx-events-8.0.0/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-17 12:15:18.000000 openedx-events-8.0.0/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:15:18.000000 openedx-events-8.0.0/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:15:18.000000 openedx-events-8.0.0/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-17 12:15:18.000000 openedx-events-8.0.0/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-17 12:15:18.000000 openedx-events-8.0.0/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.339470 openedx-events-8.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-17 12:15:13.000000 openedx-events-8.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-17 12:15:18.339470 openedx-events-8.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-05-17 12:15:13.000000 openedx-events-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:15:18.339470 openedx-events-8.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-17 12:15:13.000000 openedx-events-8.0.0/tests/test_openedx_events.py
```

### Comparing `openedx-events-7.3.0/CHANGELOG.rst` & `openedx-events-8.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.0.0] - 2023-05-16
+--------------------
+Changed
+~~~~~~~
+* **Breaking change**: Remove ``signal`` argument from consume_events and make_single_consumer
+
 [7.3.0] - 2023-05-15
 --------------------
 Changed
 ~~~~~~~
 * Made `signal` argument optional in consume_events in preparation for removal
 
 [7.2.0] - 2023-05-03
```

### Comparing `openedx-events-7.3.0/LICENSE.txt` & `openedx-events-8.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/PKG-INFO` & `openedx-events-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 7.3.0
+Version: 8.0.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.0.0] - 2023-05-16
+--------------------
+Changed
+~~~~~~~
+* **Breaking change**: Remove ``signal`` argument from consume_events and make_single_consumer
+
 [7.3.0] - 2023-05-15
 --------------------
 Changed
 ~~~~~~~
 * Made `signal` argument optional in consume_events in preparation for removal
 
 [7.2.0] - 2023-05-03
```

### Comparing `openedx-events-7.3.0/README.rst` & `openedx-events-8.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/content_authoring/data.py` & `openedx-events-8.0.0/openedx_events/content_authoring/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/content_authoring/signals.py` & `openedx-events-8.0.0/openedx_events/content_authoring/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/data.py` & `openedx-events-8.0.0/openedx_events/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/__init__.py` & `openedx-events-8.0.0/openedx_events/event_bus/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,25 +154,23 @@
 #   called. The format of the string is a dotted path to an attribute in a module, e.g.
 #   ``some.module.path.EventBusImplementation``. See docstring of ``make_single_consumer`` for
 #   parameters. If setting is not supplied or the callable raises an exception or does not return
 #   an instance of EventBusConsumer, calls to the consumer will be ignored with a warning at startup.
 
 
 def make_single_consumer(*, topic: str, group_id: str,
-                         signal: OpenEdxPublicSignal = None,  # pylint: disable=unused-argument
                          **kwargs) -> EventBusConsumer:
     """
     Construct a consumer for a given topic, group, and signal.
 
     If misconfigured, returns a fake implementation that does nothing.
 
     Arguments:
         topic: The event bus topic to consume from (without any environmental prefix)
         group_id: The consumer group to participate in
-        signal: DEPRECATED This argument will be ignored. Signals will be determined by message headers
     """
     options = {
         'topic': topic,
         'group_id': group_id,
         **kwargs,
     }
     return _try_load(
```

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/avro/custom_serializers.py` & `openedx-events-8.0.0/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/avro/deserializer.py` & `openedx-events-8.0.0/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/avro/schema.py` & `openedx-events-8.0.0/openedx_events/event_bus/avro/schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/avro/serializer.py` & `openedx-events-8.0.0/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/avro/tests/test_avro.py` & `openedx-events-8.0.0/openedx_events/event_bus/avro/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx-events-8.0.0/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx-events-8.0.0/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx-events-8.0.0/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx-events-8.0.0/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/event_bus/tests/test_loader.py` & `openedx-events-8.0.0/openedx_events/event_bus/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/exceptions.py` & `openedx-events-8.0.0/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/learning/data.py` & `openedx-events-8.0.0/openedx_events/learning/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/learning/signals.py` & `openedx-events-8.0.0/openedx_events/learning/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/management/commands/consume_events.py` & `openedx-events-8.0.0/openedx_events/management/commands/consume_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class Command(BaseCommand):
     """
     Management command for consumer workers in the event bus.
     """
 
     help = """
-    Consume messages of specified signal type from a topic and send their data to that signal.
+    Consume messages from a topic and emit their data with the correct signal.
 
     Example::
 
         python manage.py consume_events -t user-login -g user-activity-service
 
         # send extra args, for example pass check_backlog flag to redis consumer
         python manage.py cms consume_events -t user-login -g user-activity-service  --extra '{"check_backlog": true}'
@@ -30,35 +30,29 @@
         # send extra args, for example replay events from specific redis msg id.
         python manage.py cms consume_events -t user-login -g user-activity-service \
             --extra '{"last_read_msg_id": "1679676448892-0"}'
     """
 
     def add_arguments(self, parser):
         """
-        Add arguments for parsing topic, group, signal and extra args.
+        Add arguments for parsing topic, group, and extra args.
         """
         parser.add_argument(
             '-t', '--topic',
             nargs=1,
             required=True,
             help='Topic to consume (without environment prefix)'
         )
         parser.add_argument(
             '-g', '--group_id',
             nargs=1,
             required=True,
             help='Consumer group id'
         )
         parser.add_argument(
-            '-s', '--signal',
-            nargs=1,
-            required=False,
-            help='DEPRECATED This argument will be ignored. Signals will be determined by message headers'
-        )
-        parser.add_argument(
             '--extra',
             nargs='?',
             type=str,
             required=False,
             help='JSON object to pass additional arguments to the consumer.'
         )
```

### Comparing `openedx-events-7.3.0/openedx_events/tests/test_consume_events_command.py` & `openedx-events-8.0.0/openedx_events/tests/test_consume_events_command.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/tests/test_tooling.py` & `openedx-events-8.0.0/openedx_events/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/tests/utils.py` & `openedx-events-8.0.0/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/tooling.py` & `openedx-events-8.0.0/openedx_events/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events/utils.py` & `openedx-events-8.0.0/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/openedx_events.egg-info/PKG-INFO` & `openedx-events-8.0.0/openedx_events.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 7.3.0
+Version: 8.0.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.0.0] - 2023-05-16
+--------------------
+Changed
+~~~~~~~
+* **Breaking change**: Remove ``signal`` argument from consume_events and make_single_consumer
+
 [7.3.0] - 2023-05-15
 --------------------
 Changed
 ~~~~~~~
 * Made `signal` argument optional in consume_events in preparation for removal
 
 [7.2.0] - 2023-05-03
```

### Comparing `openedx-events-7.3.0/openedx_events.egg-info/SOURCES.txt` & `openedx-events-8.0.0/openedx_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-7.3.0/setup.py` & `openedx-events-8.0.0/setup.py`

 * *Files identical despite different names*

