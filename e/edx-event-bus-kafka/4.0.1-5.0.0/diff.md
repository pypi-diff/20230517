# Comparing `tmp/edx_event_bus_kafka-4.0.1.tar.gz` & `tmp/edx_event_bus_kafka-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_event_bus_kafka-4.0.1.tar", last modified: Thu May 11 16:10:29 2023, max compression
+gzip compressed data, was "edx_event_bus_kafka-5.0.0.tar", last modified: Wed May 17 16:02:11 2023, max compression
```

## Comparing `edx_event_bus_kafka-4.0.1.tar` & `edx_event_bus_kafka-5.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.581205 edx_event_bus_kafka-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)    12127 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19393 2023-05-11 16:10:29.581205 edx_event_bus_kafka-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6573 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.573205 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.577205 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5882 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30954 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    14863 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.581205 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    31454 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    18435 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/tests/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7678 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7386 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.581205 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.581205 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/management/commands/produce_event.py
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.569205 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.581205 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/templates/edx_event_bus_kafka/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.577205 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19393 2023-05-11 16:10:29.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-05-11 16:10:29.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 16:10:29.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 16:10:29.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-11 16:10:29.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-11 16:10:29.000000 edx_event_bus_kafka-4.0.1/edx_event_bus_kafka.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.581205 edx_event_bus_kafka-4.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-11 16:10:29.581205 edx_event_bus_kafka-4.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5009 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:10:29.581205 edx_event_bus_kafka-4.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-11 16:10:25.000000 edx_event_bus_kafka-4.0.1/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.012956 edx_event_bus_kafka-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    12277 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    19725 2023-05-17 16:02:11.012956 edx_event_bus_kafka-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6755 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.004956 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.008956 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5882 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30796 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14863 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.008956 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31454 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18435 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/tests/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7678 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7386 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.008956 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.008956 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/management/commands/produce_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.004956 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.008956 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.008956 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    19725 2023-05-17 16:02:10.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-05-17 16:02:11.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 16:02:10.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 16:02:10.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-17 16:02:10.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-17 16:02:10.000000 edx_event_bus_kafka-5.0.0/edx_event_bus_kafka.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.008956 edx_event_bus_kafka-5.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-17 16:02:11.012956 edx_event_bus_kafka-5.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5009 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:02:11.008956 edx_event_bus_kafka-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-17 16:02:06.000000 edx_event_bus_kafka-5.0.0/tests/test_models.py
```

### Comparing `edx_event_bus_kafka-4.0.1/CHANGELOG.rst` & `edx_event_bus_kafka-5.0.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[5.0.0] - 2023-05-17
+********************
+Changed
+=======
+* **BREAKING CHANGE**: Removed deprecated ``signal`` argument from consumer initialization
+
 [4.0.1] - 2023-05-10
 ********************
 Fixed
 =====
 * Added ``signal`` back as an argument when creating a consumer for compatibility with the openedx-events API
 
 [4.0.0] - 2023-05-10
```

### Comparing `edx_event_bus_kafka-4.0.1/LICENSE.txt` & `edx_event_bus_kafka-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/PKG-INFO` & `edx_event_bus_kafka-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx_event_bus_kafka
-Version: 4.0.1
+Version: 5.0.0
 Summary: Kafka implementation for Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-kafka
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -24,15 +24,15 @@
 Kafka implementation for Open edX event bus.
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
 
 Overview
 ********
-This package implements an event bus for Open EdX using Kafka.
+This package implements an event bus for Open edX using Kafka.
 
 The event bus acts as a broker between services publishing events and other services that consume these events.
 Implementing the event bus will allow for asynchronous messaging across services which greatly improves efficiency as we don't have to wait for scheduled batch synchronizations.
 Additionally, since the services all speak to the event bus, they are independent of one another and can still function if one service crashes.
 
 This package contains both the publishing code, which processes events into messages to send to the broker, and the consumer code,
 which polls the broker using a `while True` loop in order to turn messages back into event data to be emitted.
@@ -49,24 +49,31 @@
 
 To use this implementation of the Event Bus with openedx-events, you'll need to ensure that you include the dependency ``confluent_kafka[avro,schema-registry]`` (see `ADR 5 <https://github.com/openedx/event-bus-kafka/blob/main/docs/decisions/0005-optional-import-of-confluent-kafka.rst>`_ for an explanation) and set the following Django settings::
 
     EVENT_BUS_KAFKA_BOOTSTRAP_SERVERS: ...
     EVENT_BUS_KAFKA_SCHEMA_REGISTRY_URL: ...
     EVENT_BUS_TOPIC_PREFIX: ...
 
-    # Required, on the producing side only:
+    # On the producing side:
     EVENT_BUS_PRODUCER: edx_event_bus_kafka.create_producer
 
+    # On the consuming side:
+    EVENT_BUS_CONSUMER: edx_event_bus_kafka.KafkaEventConsumer
+
+
 Optional settings that are worth considering:
 
 - ``EVENT_BUS_KAFKA_CONSUMER_CONSECUTIVE_ERRORS_LIMIT``
 
 For manual testing, see `<docs/how_tos/manual_testing.rst>`__.
 
-Django management commands: ``edx_event_bus_kafka.management.commands.*`` expose ``Command`` classes
+Django management commands:
+
+- If you need to test event production, use the ``produce_event`` management command
+- To actually run the consumer, use openedx-events' ``consume_events`` management command
 
 OEP-52 documentation: https://open-edx-proposals.readthedocs.io/en/latest/architectural-decisions/oep-0052-arch-event-bus-architecture.html
 (TODO: `Set up documentation <https://openedx.atlassian.net/wiki/spaces/DOC/pages/21627535/Publish+Documentation+on+Read+the+Docs>`_)
 
 Development Workflow
 ********************
 
@@ -197,14 +204,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[5.0.0] - 2023-05-17
+********************
+Changed
+=======
+* **BREAKING CHANGE**: Removed deprecated ``signal`` argument from consumer initialization
+
 [4.0.1] - 2023-05-10
 ********************
 Fixed
 =====
 * Added ``signal`` back as an argument when creating a consumer for compatibility with the openedx-events API
 
 [4.0.0] - 2023-05-10
```

### Comparing `edx_event_bus_kafka-4.0.1/README.rst` & `edx_event_bus_kafka-5.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Kafka implementation for Open edX event bus.
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
 
 Overview
 ********
-This package implements an event bus for Open EdX using Kafka.
+This package implements an event bus for Open edX using Kafka.
 
 The event bus acts as a broker between services publishing events and other services that consume these events.
 Implementing the event bus will allow for asynchronous messaging across services which greatly improves efficiency as we don't have to wait for scheduled batch synchronizations.
 Additionally, since the services all speak to the event bus, they are independent of one another and can still function if one service crashes.
 
 This package contains both the publishing code, which processes events into messages to send to the broker, and the consumer code,
 which polls the broker using a `while True` loop in order to turn messages back into event data to be emitted.
@@ -29,24 +29,31 @@
 
 To use this implementation of the Event Bus with openedx-events, you'll need to ensure that you include the dependency ``confluent_kafka[avro,schema-registry]`` (see `ADR 5 <https://github.com/openedx/event-bus-kafka/blob/main/docs/decisions/0005-optional-import-of-confluent-kafka.rst>`_ for an explanation) and set the following Django settings::
 
     EVENT_BUS_KAFKA_BOOTSTRAP_SERVERS: ...
     EVENT_BUS_KAFKA_SCHEMA_REGISTRY_URL: ...
     EVENT_BUS_TOPIC_PREFIX: ...
 
-    # Required, on the producing side only:
+    # On the producing side:
     EVENT_BUS_PRODUCER: edx_event_bus_kafka.create_producer
 
+    # On the consuming side:
+    EVENT_BUS_CONSUMER: edx_event_bus_kafka.KafkaEventConsumer
+
+
 Optional settings that are worth considering:
 
 - ``EVENT_BUS_KAFKA_CONSUMER_CONSECUTIVE_ERRORS_LIMIT``
 
 For manual testing, see `<docs/how_tos/manual_testing.rst>`__.
 
-Django management commands: ``edx_event_bus_kafka.management.commands.*`` expose ``Command`` classes
+Django management commands:
+
+- If you need to test event production, use the ``produce_event`` management command
+- To actually run the consumer, use openedx-events' ``consume_events`` management command
 
 OEP-52 documentation: https://open-edx-proposals.readthedocs.io/en/latest/architectural-decisions/oep-0052-arch-event-bus-architecture.html
 (TODO: `Set up documentation <https://openedx.atlassian.net/wiki/spaces/DOC/pages/21627535/Publish+Documentation+on+Read+the+Docs>`_)
 
 Development Workflow
 ********************
```

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/config.py` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/consumer.py` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,21 +108,20 @@
     Note that the topic should be specified here *without* the optional environment prefix.
 
     Can also consume messages indefinitely off the queue.
 
     Attributes:
         topic: Topic to consume (without environment prefix).
         group_id: Consumer group id.
-        signal: DEPRECATED Type of signal to emit from consumed messages. Will be removed in a future version
         consumer: Actual kafka consumer instance.
         offset_time: The timestamp (in ISO format) that we would like to reset the consumers to. If this is used, the
             consumers will only reset the offsets of the topic but will not actually consume and process any messages.
     """
 
-    def __init__(self, topic, group_id, signal=None, offset_time=None):  # pylint: disable=unused-argument
+    def __init__(self, topic, group_id, offset_time=None):
         if confluent_kafka is None:  # pragma: no cover
             raise Exception('Library confluent-kafka not available. Cannot create event consumer.')
 
         self.topic = topic
         self.group_id = group_id
         self.consumer = self._create_consumer()
         self.offset_time = None
```

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/producer.py` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/tests/test_config.py` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/tests/test_consumer.py` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/tests/test_producer.py` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/tests/test_utils.py` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/internal/utils.py` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/management/commands/produce_event.py` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/management/commands/produce_event.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka.egg-info/PKG-INFO` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-bus-kafka
-Version: 4.0.1
+Version: 5.0.0
 Summary: Kafka implementation for Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-kafka
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -24,15 +24,15 @@
 Kafka implementation for Open edX event bus.
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
 
 Overview
 ********
-This package implements an event bus for Open EdX using Kafka.
+This package implements an event bus for Open edX using Kafka.
 
 The event bus acts as a broker between services publishing events and other services that consume these events.
 Implementing the event bus will allow for asynchronous messaging across services which greatly improves efficiency as we don't have to wait for scheduled batch synchronizations.
 Additionally, since the services all speak to the event bus, they are independent of one another and can still function if one service crashes.
 
 This package contains both the publishing code, which processes events into messages to send to the broker, and the consumer code,
 which polls the broker using a `while True` loop in order to turn messages back into event data to be emitted.
@@ -49,24 +49,31 @@
 
 To use this implementation of the Event Bus with openedx-events, you'll need to ensure that you include the dependency ``confluent_kafka[avro,schema-registry]`` (see `ADR 5 <https://github.com/openedx/event-bus-kafka/blob/main/docs/decisions/0005-optional-import-of-confluent-kafka.rst>`_ for an explanation) and set the following Django settings::
 
     EVENT_BUS_KAFKA_BOOTSTRAP_SERVERS: ...
     EVENT_BUS_KAFKA_SCHEMA_REGISTRY_URL: ...
     EVENT_BUS_TOPIC_PREFIX: ...
 
-    # Required, on the producing side only:
+    # On the producing side:
     EVENT_BUS_PRODUCER: edx_event_bus_kafka.create_producer
 
+    # On the consuming side:
+    EVENT_BUS_CONSUMER: edx_event_bus_kafka.KafkaEventConsumer
+
+
 Optional settings that are worth considering:
 
 - ``EVENT_BUS_KAFKA_CONSUMER_CONSECUTIVE_ERRORS_LIMIT``
 
 For manual testing, see `<docs/how_tos/manual_testing.rst>`__.
 
-Django management commands: ``edx_event_bus_kafka.management.commands.*`` expose ``Command`` classes
+Django management commands:
+
+- If you need to test event production, use the ``produce_event`` management command
+- To actually run the consumer, use openedx-events' ``consume_events`` management command
 
 OEP-52 documentation: https://open-edx-proposals.readthedocs.io/en/latest/architectural-decisions/oep-0052-arch-event-bus-architecture.html
 (TODO: `Set up documentation <https://openedx.atlassian.net/wiki/spaces/DOC/pages/21627535/Publish+Documentation+on+Read+the+Docs>`_)
 
 Development Workflow
 ********************
 
@@ -197,14 +204,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[5.0.0] - 2023-05-17
+********************
+Changed
+=======
+* **BREAKING CHANGE**: Removed deprecated ``signal`` argument from consumer initialization
+
 [4.0.1] - 2023-05-10
 ********************
 Fixed
 =====
 * Added ``signal`` back as an argument when creating a consumer for compatibility with the openedx-events API
 
 [4.0.0] - 2023-05-10
```

### Comparing `edx_event_bus_kafka-4.0.1/edx_event_bus_kafka.egg-info/SOURCES.txt` & `edx_event_bus_kafka-5.0.0/edx_event_bus_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/requirements/constraints.txt` & `edx_event_bus_kafka-5.0.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-4.0.1/setup.py` & `edx_event_bus_kafka-5.0.0/setup.py`

 * *Files identical despite different names*

