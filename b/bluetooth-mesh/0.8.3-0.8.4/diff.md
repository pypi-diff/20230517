# Comparing `tmp/bluetooth-mesh-0.8.3.tar.gz` & `tmp/bluetooth-mesh-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bluetooth-mesh-0.8.3.tar", last modified: Tue Apr 25 11:58:56 2023, max compression
+gzip compressed data, was "dist/bluetooth-mesh-0.8.4.tar", last modified: Wed May 17 08:30:16 2023, max compression
```

## Comparing `bluetooth-mesh-0.8.3.tar` & `bluetooth-mesh-0.8.4.tar`

### file list

```diff
@@ -1,129 +1,133 @@
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1234 2020-03-20 10:52:47.000000 bluetooth-mesh-0.8.3/.gitignore
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    13702 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/.pylintrc
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      252 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/.readthedocs.yml
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1238 2022-04-12 11:29:02.000000 bluetooth-mesh-0.8.3/.travis.yml
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      285 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/AUTHORS
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    18006 2018-11-22 08:06:11.000000 bluetooth-mesh-0.8.3/LICENSE
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3423 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/PKG-INFO
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1931 2022-04-12 10:11:41.000000 bluetooth-mesh-0.8.3/README.rst
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       74 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    36147 2022-02-02 12:42:42.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/application.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/apps/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      332 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/apps/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      113 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/apps/hookspecs.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    54089 2022-04-12 07:30:22.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/apps/meshcli.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      390 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/apps/mixins.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3348 2021-11-02 08:35:19.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/crypto.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    21860 2021-03-11 08:56:00.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/interfaces.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    18575 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/mesh.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4028 2022-04-12 11:29:09.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      589 2022-04-12 11:01:40.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/capnproto.py
--rwxrwxr-x   0 khorne    (1000) khorne    (1000)     8853 2021-11-02 08:35:19.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/capnproto_generator.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    37836 2023-04-25 11:58:34.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/config.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      432 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3144 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/battery.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3605 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/level.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      281 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     5615 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/ctl.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4944 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/lightness.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2588 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/onoff.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2237 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generics.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3676 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/health.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    23969 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/properties.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3727 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/scene.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    11769 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/sensor.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      672 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     6838 2022-12-06 09:54:57.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/debug.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4219 2022-11-04 10:39:27.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/debugV2.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     7081 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/gateway_config_server.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3695 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/light_extended_controller.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     5145 2021-06-17 10:39:22.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/network_diagnostic_server.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     7449 2022-04-12 11:29:09.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/rrule_scheduler.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     8703 2022-12-06 09:54:57.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_debug.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    10468 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_gateway_config_server.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     6482 2021-06-17 10:39:22.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_network_diagnostic_server.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2285 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_access.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2925 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_battery.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    41195 2023-04-25 11:58:34.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_config.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4162 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_generics.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     5255 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_health.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     6199 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_level.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    13545 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_light.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     5300 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_scene.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    31797 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_sensor.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1332 2021-04-26 14:31:14.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_strings.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4669 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_time.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     9414 2022-07-04 12:59:36.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/time.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    13716 2022-11-04 10:39:27.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/messages/util.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/models/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       67 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/models/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    17537 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/models/base.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    82908 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/models/models.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     9695 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/provisioning.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)        0 2020-03-19 13:27:43.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/__init__.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1478 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/fixtures.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     8072 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_application.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1979 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_construct_match.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3934 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_element.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1764 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_gatherer.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1965 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_key_derivation.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     4772 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_light_lightness_client.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    12070 2022-04-12 10:11:41.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_mesh.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    12410 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_model.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)    14459 2023-04-25 11:25:17.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_provisioning.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3227 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_scene_client.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1925 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_security.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1984 2021-04-15 08:26:46.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_signal.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2743 2021-06-15 07:23:33.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_tasklet.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2660 2021-01-29 08:55:12.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/tokenring.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     6875 2022-04-12 10:15:30.000000 bluetooth-mesh-0.8.3/bluetooth_mesh/utils.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3423 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/PKG-INFO
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3620 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/SOURCES.txt
--rw-rw-r--   0 khorne    (1000) khorne    (1000)        1 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/dependency_links.txt
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      132 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/entry_points.txt
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      257 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/requires.txt
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       15 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/top_level.txt
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)        7 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/.gitignore
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      634 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/Makefile
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/_ext/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     6620 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.3/docs/_ext/autoconstruct.py
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/_static/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)        0 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/_static/.keep
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/api/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      901 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/api/application.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2576 2022-06-06 08:21:17.000000 bluetooth-mesh-0.8.3/docs/api/messages.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      843 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/api/models.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      114 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/api.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2394 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.3/docs/conf.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1045 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/index.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      454 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/installation.rst
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/mod/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       69 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/application.rst
-drwxrwxr-x   0 khorne    (1000) khorne    (1000)        0 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/docs/mod/examples/
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      895 2020-12-02 08:20:28.000000 bluetooth-mesh-0.8.3/docs/mod/examples/bulk_query.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      957 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.3/docs/mod/examples/callbacks.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      979 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/examples/delay.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      779 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/examples/expect.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      577 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/examples/model.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     1110 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/examples/query.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      575 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/examples/repeat.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       59 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/messages.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     3653 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod/models.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       80 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/mod.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      119 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/docs/quickstart.rst
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2666 2020-08-04 09:22:08.000000 bluetooth-mesh-0.8.3/docs/skeleton.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      513 2020-07-10 07:18:10.000000 bluetooth-mesh-0.8.3/pyproject.toml
--rw-rw-r--   0 khorne    (1000) khorne    (1000)       63 2023-04-25 11:58:56.000000 bluetooth-mesh-0.8.3/setup.cfg
--rw-rw-r--   0 khorne    (1000) khorne    (1000)     2945 2023-04-25 11:58:43.000000 bluetooth-mesh-0.8.3/setup.py
--rw-rw-r--   0 khorne    (1000) khorne    (1000)      652 2022-06-06 08:22:51.000000 bluetooth-mesh-0.8.3/tox.ini
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1234 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/.gitignore
+-rw-r--r--   0 khorne    (1000) sudo        (27)    13702 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/.pylintrc
+-rw-r--r--   0 khorne    (1000) sudo        (27)      252 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/.readthedocs.yml
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1238 2022-05-05 10:57:27.000000 bluetooth-mesh-0.8.4/.travis.yml
+-rw-r--r--   0 khorne    (1000) sudo        (27)      285 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/AUTHORS
+-rw-r--r--   0 khorne    (1000) sudo        (27)    18006 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/LICENSE
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2936 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/PKG-INFO
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1931 2022-05-05 10:57:27.000000 bluetooth-mesh-0.8.4/README.rst
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/
+-rw-r--r--   0 khorne    (1000) sudo        (27)       74 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/__init__.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    36147 2022-12-22 08:53:08.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/application.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/apps/
+-rw-r--r--   0 khorne    (1000) sudo        (27)      332 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/apps/__init__.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)      113 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/apps/hookspecs.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    54089 2023-02-08 08:17:02.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/apps/meshcli.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)      390 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/apps/mixins.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3348 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/crypto.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    21860 2022-12-22 08:53:08.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/interfaces.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    18575 2022-12-22 08:53:14.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/mesh.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/
+-rw-r--r--   0 khorne    (1000) sudo        (27)     4028 2022-05-05 10:57:27.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/__init__.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)      589 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/capnproto.py
+-rwxr-xr-x   0 khorne    (1000) sudo        (27)     9057 2023-05-12 11:11:50.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/capnproto_generator.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    37881 2023-05-12 11:09:24.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/config.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/
+-rw-r--r--   0 khorne    (1000) sudo        (27)      432 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/__init__.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3144 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/battery.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3605 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/level.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/light/
+-rw-r--r--   0 khorne    (1000) sudo        (27)      281 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/light/__init__.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     5615 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/light/ctl.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     4944 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/light/lightness.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2588 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/onoff.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2237 2022-03-07 12:47:55.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generics.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3676 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/health.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    23969 2022-12-22 08:53:14.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/properties.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3727 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/scene.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    11769 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/sensor.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/
+-rw-r--r--   0 khorne    (1000) sudo        (27)      672 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/__init__.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     6838 2023-05-12 11:09:22.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/debug.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     4219 2023-05-12 11:09:22.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/debugV2.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     7081 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/gateway_config_server.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3695 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/light_extended_controller.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     5145 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/network_diagnostic_server.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     7449 2022-05-05 10:57:27.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/rrule_scheduler.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/test/
+-rw-r--r--   0 khorne    (1000) sudo        (27)     8703 2023-05-12 11:09:22.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/test/test_debug.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3903 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/test/test_debugV2.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    10468 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/test/test_gateway_config_server.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     6482 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/test/test_network_diagnostic_server.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     9971 2022-05-05 10:57:27.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/test/test_rrule_scheduler.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2285 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_access.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2925 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_battery.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    12309 2023-05-12 11:09:24.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_capnproto.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    41980 2023-05-12 11:09:24.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_config.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     4162 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_generics.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     5255 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_health.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     6199 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_level.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    13545 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_light.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     5300 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_scene.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    31797 2022-12-22 08:53:14.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_sensor.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1332 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_strings.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     4669 2022-06-07 11:08:22.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_time.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1300 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_util.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     9414 2022-12-22 08:53:14.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/time.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    15151 2023-05-12 11:09:24.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/messages/util.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/models/
+-rw-r--r--   0 khorne    (1000) sudo        (27)       67 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/models/__init__.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    17537 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/models/base.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    82908 2023-05-12 11:09:22.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/models/models.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     9695 2023-05-12 11:09:22.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/provisioning.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/
+-rw-r--r--   0 khorne    (1000) sudo        (27)        0 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/__init__.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1478 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/fixtures.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     8072 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_application.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1979 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_construct_match.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3934 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_element.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1764 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_gatherer.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1965 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_key_derivation.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     4772 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_light_lightness_client.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    12070 2022-05-05 10:57:27.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_mesh.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    12410 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_model.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)    14459 2023-05-12 11:09:22.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_provisioning.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3227 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_scene_client.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1925 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_security.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1984 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_signal.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2743 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_tasklet.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2660 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/tokenring.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     6875 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/bluetooth_mesh/utils.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh.egg-info/
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2936 2023-05-17 08:30:15.000000 bluetooth-mesh-0.8.4/bluetooth_mesh.egg-info/PKG-INFO
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3823 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh.egg-info/SOURCES.txt
+-rw-r--r--   0 khorne    (1000) sudo        (27)        1 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh.egg-info/dependency_links.txt
+-rw-r--r--   0 khorne    (1000) sudo        (27)      131 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh.egg-info/entry_points.txt
+-rw-r--r--   0 khorne    (1000) sudo        (27)      257 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh.egg-info/requires.txt
+-rw-r--r--   0 khorne    (1000) sudo        (27)       15 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/bluetooth_mesh.egg-info/top_level.txt
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/docs/
+-rw-r--r--   0 khorne    (1000) sudo        (27)        7 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/.gitignore
+-rw-r--r--   0 khorne    (1000) sudo        (27)      634 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/Makefile
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/docs/_ext/
+-rw-r--r--   0 khorne    (1000) sudo        (27)     6620 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/_ext/autoconstruct.py
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/docs/_static/
+-rw-r--r--   0 khorne    (1000) sudo        (27)        0 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/_static/.keep
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/docs/api/
+-rw-r--r--   0 khorne    (1000) sudo        (27)      901 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/api/application.rst
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2576 2022-05-05 12:01:55.000000 bluetooth-mesh-0.8.4/docs/api/messages.rst
+-rw-r--r--   0 khorne    (1000) sudo        (27)      843 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/api/models.rst
+-rw-r--r--   0 khorne    (1000) sudo        (27)      114 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/api.rst
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2394 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/conf.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1045 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/index.rst
+-rw-r--r--   0 khorne    (1000) sudo        (27)      454 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/installation.rst
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/docs/mod/
+-rw-r--r--   0 khorne    (1000) sudo        (27)       69 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod/application.rst
+drwxr-xr-x   0 khorne    (1000) sudo        (27)        0 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/docs/mod/examples/
+-rw-r--r--   0 khorne    (1000) sudo        (27)      895 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod/examples/bulk_query.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)      957 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod/examples/callbacks.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)      979 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod/examples/delay.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)      779 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod/examples/expect.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)      577 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod/examples/model.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)     1110 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod/examples/query.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)      575 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod/examples/repeat.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)       59 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod/messages.rst
+-rw-r--r--   0 khorne    (1000) sudo        (27)     3653 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod/models.rst
+-rw-r--r--   0 khorne    (1000) sudo        (27)       80 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/mod.rst
+-rw-r--r--   0 khorne    (1000) sudo        (27)      119 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/quickstart.rst
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2666 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/docs/skeleton.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)      513 2022-03-02 09:22:17.000000 bluetooth-mesh-0.8.4/pyproject.toml
+-rw-r--r--   0 khorne    (1000) sudo        (27)       63 2023-05-17 08:30:16.000000 bluetooth-mesh-0.8.4/setup.cfg
+-rw-r--r--   0 khorne    (1000) sudo        (27)     2945 2023-05-12 11:09:24.000000 bluetooth-mesh-0.8.4/setup.py
+-rw-r--r--   0 khorne    (1000) sudo        (27)      652 2022-06-07 08:12:33.000000 bluetooth-mesh-0.8.4/tox.ini
```

### Comparing `bluetooth-mesh-0.8.3/.gitignore` & `bluetooth-mesh-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/.pylintrc` & `bluetooth-mesh-0.8.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/.travis.yml` & `bluetooth-mesh-0.8.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/LICENSE` & `bluetooth-mesh-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/PKG-INFO` & `bluetooth-mesh-0.8.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,94 @@
 Metadata-Version: 2.1
 Name: bluetooth-mesh
-Version: 0.8.3
+Version: 0.8.4
 Summary: Bluetooth mesh for Python
 Home-page: http://github.com/silvairgit/python-bluetooth-mesh
 Author-email: michal.lowas-rzechonek@silvair.com
 License: UNKNOWN
-Description: =====================
-        python-bluetooth-mesh
-        =====================
-        
-        .. image:: https://img.shields.io/pypi/v/bluetooth-mesh.svg
-            :target: https://pypi.org/project/bluetooth-mesh
-            :alt: PyPI version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/bluetooth-mesh.svg
-            :target: https://pypi.org/project/bluetooth-mesh
-            :alt: Python versions
-        
-        .. image:: https://app.travis-ci.com/SilvairGit/python-bluetooth-mesh.svg?branch=master
-            :target: https://travis-ci.com/github/SilvairGit/python-bluetooth-mesh
-            :alt: See Build Status on Travis CI
-        
-        .. image:: https://readthedocs.org/projects/python-bluetooth-mesh/badge/?version=latest
-            :target: https://python-bluetooth-mesh.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        Bluetooth mesh SDK for Python allows developing applications communicating with
-        Bluetooth mesh network using BlueZ's bluetooth-meshd.
-        
-        ----
-        
-        What is this thing?
-        -------------------
-        
-        https://www.bluetooth.com/specifications/mesh-specifications
-        
-        https://git.kernel.org/pub/scm/bluetooth/bluez.git/tree/doc/mesh-api.txt
-        
-        
-        Installation
-        ------------
-        
-        You can install "python-bluetooth-mesh" via `pip`_ from `PyPI`_::
-        
-            $ pip install bluetooth-mesh
-        
-        
-        Contributing
-        ------------
-        Contributions are very welcome. Tests can be run with `tox`_, please ensure
-        the coverage at least stays the same before you submit a pull request.
-        
-        
-        License
-        -------
-        
-        Distributed under the terms of the `GPL-2.0`_ license, "python-bluetooth-mesh" is
-        free and open source software
-        
-        
-        Issues
-        ------
-        
-        If you encounter any problems, please `file an issue`_ along with a detailed description.
-        
-        .. _`GPL-2.0`: http://opensource.org/licenses/GPL-2.0
-        .. _`file an issue`: https://github.com/SilvairGit/python-bluetooth-mesh/issues
-        .. _`pytest`: https://github.com/pytest-dev/pytest
-        .. _`tox`: https://tox.readthedocs.io/en/latest/
-        .. _`pip`: https://pypi.org/project/pip/
-        .. _`PyPI`: https://pypi.org/project
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.6.0,<3.11.0
 Description-Content-Type: text/x-rst
-Provides-Extra: capnp
 Provides-Extra: docs
 Provides-Extra: tools
+Provides-Extra: capnp
+License-File: LICENSE
+License-File: AUTHORS
+
+=====================
+python-bluetooth-mesh
+=====================
+
+.. image:: https://img.shields.io/pypi/v/bluetooth-mesh.svg
+    :target: https://pypi.org/project/bluetooth-mesh
+    :alt: PyPI version
+
+.. image:: https://img.shields.io/pypi/pyversions/bluetooth-mesh.svg
+    :target: https://pypi.org/project/bluetooth-mesh
+    :alt: Python versions
+
+.. image:: https://app.travis-ci.com/SilvairGit/python-bluetooth-mesh.svg?branch=master
+    :target: https://travis-ci.com/github/SilvairGit/python-bluetooth-mesh
+    :alt: See Build Status on Travis CI
+
+.. image:: https://readthedocs.org/projects/python-bluetooth-mesh/badge/?version=latest
+    :target: https://python-bluetooth-mesh.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+Bluetooth mesh SDK for Python allows developing applications communicating with
+Bluetooth mesh network using BlueZ's bluetooth-meshd.
+
+----
+
+What is this thing?
+-------------------
+
+https://www.bluetooth.com/specifications/mesh-specifications
+
+https://git.kernel.org/pub/scm/bluetooth/bluez.git/tree/doc/mesh-api.txt
+
+
+Installation
+------------
+
+You can install "python-bluetooth-mesh" via `pip`_ from `PyPI`_::
+
+    $ pip install bluetooth-mesh
+
+
+Contributing
+------------
+Contributions are very welcome. Tests can be run with `tox`_, please ensure
+the coverage at least stays the same before you submit a pull request.
+
+
+License
+-------
+
+Distributed under the terms of the `GPL-2.0`_ license, "python-bluetooth-mesh" is
+free and open source software
+
+
+Issues
+------
+
+If you encounter any problems, please `file an issue`_ along with a detailed description.
+
+.. _`GPL-2.0`: http://opensource.org/licenses/GPL-2.0
+.. _`file an issue`: https://github.com/SilvairGit/python-bluetooth-mesh/issues
+.. _`pytest`: https://github.com/pytest-dev/pytest
+.. _`tox`: https://tox.readthedocs.io/en/latest/
+.. _`pip`: https://pypi.org/project/pip/
+.. _`PyPI`: https://pypi.org/project
+
+
```

### Comparing `bluetooth-mesh-0.8.3/README.rst` & `bluetooth-mesh-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/application.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/application.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/apps/meshcli.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/apps/meshcli.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/crypto.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/crypto.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/interfaces.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/interfaces.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/mesh.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/__init__.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/capnproto.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/capnproto.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/capnproto_generator.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/capnproto_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 from construct import (
     Adapter,
     Array,
     BitsInteger,
     Bytes,
     BytesInteger,
     Const,
+    Computed,
     Construct,
     Default,
     FixedSized,
     Flag,
     FocusedSeq,
     FormatField,
     GreedyBytes,
     GreedyRange,
     NullStripped,
+    IfThenElse,
     Padded,
     Pass,
     Rebuild,
     Renamed,
     Restreamed,
     Select,
     StopIf,
@@ -75,14 +77,17 @@
     message_name=None,
 ):
     struct_name = struct_name or names[con] or f"{message_name}Params"
 
     if field_name and field_name.startswith("_"):
         return
 
+    elif isinstance(con, Computed):
+        return
+
     if isinstance(con, Struct):
         visitor.enter_struct(field_name, struct_name, many=many)
 
         for subcon in con.subcons:
             convert(subcon, visitor, message_name=message_name)
 
         visitor.exit()
@@ -129,14 +134,17 @@
             con.subcon,
             visitor,
             field_name=con.name,
             message_name=message_name,
             many=many,
         )
 
+    elif isinstance(con, IfThenElse) and con.elsesubcon is Pass:
+        visitor.field(con.thensubcon, field_name, None)
+
     elif isinstance(con, StringEncoded):
         visitor.field(con, field_name, struct_name)
 
     elif isinstance(con, (GreedyRange, Array)):
         convert(
             con.subcon,
             visitor,
```

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/config.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,40 +31,40 @@
     Bytes,
     Bytewise,
     Embedded,
     ExprValidator,
     Flag,
     GreedyBytes,
     GreedyRange,
-    If,
-    IfThenElse,
     Int8ul,
     Int16ul,
     Int24ul,
     Int8sl,
-    Mapping,
     Padding,
     Rebuild,
     Select,
     Struct,
     len_,
     obj_,
-    this, Byte
+    this,
 )
 
 from bluetooth_mesh.messages.util import (
     BitList,
     EmbeddedBitStruct,
     EnumAdapter,
+    EnumSwitchStruct,
     LogAdapter,
     NamedSelect,
     Opcode,
     RangeValidator,
     Reversed,
     SwitchStruct,
+    IfThenElseDefault,
+    enum_switch_struct_len_,
 )
 from bluetooth_mesh.messages.util import EnumSwitch as Switch
 
 
 class SecureNetworkBeacon(enum.IntEnum):
     OFF = 0x00
     ON = 0x01
@@ -568,44 +568,37 @@
 )
 
 ExtendedModelLongFormat = Struct(
     "model_item_index" / Int8ul,
     "element_offset" / Int8sl
 )
 
-ElementOffsetRepresentedValue = {
-    0: 0,
-    1: 1,
-    2: 2,
-    - 4: 4,
-    - 3: 5,
-    - 2: 6,
-    - 1: 7
-}
-
 ExtendedModelShortFormat = BitStruct(
     "model_item_index" / BitsInteger(5),
-    "element_offset" / Mapping(BitsInteger(3), ElementOffsetRepresentedValue),
+    "element_offset" / BitsInteger(3, signed=True),
 )
 
 
 class ExtendedModelsItemFormat(enum.IntEnum):
-    SHORT = False
-    LONG = True
+    SHORT = 0
+    LONG = 1
 
 
 ModelRelationItem = BitStruct(
-    "extended_items_count" / Rebuild(BitsInteger(6), len_(this["extended_models_items"])),
-    "format" / EnumAdapter(Flag, ExtendedModelsItemFormat),
-    "corresponding_present" / Flag,
-    "corresponding_id" / If(this.corresponding_present, BitsInteger(8)),
-    "extended_models_items" / IfThenElse(
-        this.format == 0,
-        Bytewise(ExtendedModelShortFormat[this["extended_items_count"]]),
-        Bytewise(ExtendedModelLongFormat[this["extended_items_count"]])),
+    "extended_items_count" / Rebuild(BitsInteger(6), enum_switch_struct_len_(this["extended_models_items"])),
+    "format" / EnumAdapter(BitsInteger(1), ExtendedModelsItemFormat),
+    "corresponding_present" / BitsInteger(1),
+    "corresponding_id" / IfThenElseDefault(this.corresponding_present, BitsInteger(8), default=0),
+    "extended_models_items" / Bytewise(EnumSwitchStruct(Switch(
+        this.format,
+        {
+            ExtendedModelsItemFormat.SHORT: ExtendedModelShortFormat[this["extended_items_count"]],
+            ExtendedModelsItemFormat.LONG: ExtendedModelLongFormat[this["extended_items_count"]],
+        }
+    ))),
 )
 
 CompositionDataPage1Element = Struct(
     "number_s" / Rebuild(Int8ul, len_(this["sig_models"])),
     "number_v" / Rebuild(Int8ul, len_(this["vendor_models"])),
     "sig_models" / ModelRelationItem[this["number_s"]],
     "vendor_models" / ModelRelationItem[this["number_v"]],
```

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/battery.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/battery.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/level.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/level.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/ctl.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/light/ctl.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/light/lightness.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/light/lightness.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generic/onoff.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generic/onoff.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/generics.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/generics.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/health.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/health.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/properties.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/properties.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/scene.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/scene.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/sensor.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/sensor.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/__init__.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/__init__.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/debug.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/debug.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/debugV2.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/debugV2.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/gateway_config_server.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/gateway_config_server.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/light_extended_controller.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/light_extended_controller.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/network_diagnostic_server.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/network_diagnostic_server.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/rrule_scheduler.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/rrule_scheduler.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_debug.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_gateway_config_server.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/test/test_gateway_config_server.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/silvair/test/test_network_diagnostic_server.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/silvair/test/test_network_diagnostic_server.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_access.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_access.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_battery.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_battery.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_config.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -403,15 +403,15 @@
                         "number_v": 0,
                         "sig_models": [
                             {
                                 "extended_items_count": 0,
                                 "format": ExtendedModelsItemFormat.SHORT,
                                 "corresponding_present": True,
                                 "corresponding_id": 0x0A,
-                                "extended_models_items": []
+                                "extended_models_items": {"short": []}
                             },
                         ],
                         "vendor_models": []
                     },
                 ],
                 },
 
@@ -422,15 +422,15 @@
                         "number_v": 0,
                         "sig_models": [
                             {
                                 "extended_items_count": 0,
                                 "format": ExtendedModelsItemFormat.SHORT,
                                 "corresponding_present": True,
                                 "corresponding_id": 0x0A,
-                                "extended_models_items": []
+                                "extended_models_items": {"short": []}
                             }
                         ],
                         "vendor_models": []
                     }
                 ]
                 }
         },
@@ -559,71 +559,75 @@
                 "number_s": 2,
                 "number_v": 1,
                 "sig_models": [
                     {
                         "extended_items_count": 0,
                         "format": ExtendedModelsItemFormat.SHORT,
                         "corresponding_present": False,
-                        "corresponding_id": None,
-                        "extended_models_items": []
+                        "corresponding_id": 0,
+                        "extended_models_items": {"short": []}
                     },
                     {
                         "extended_items_count": 1,
                         "format": ExtendedModelsItemFormat.SHORT,
                         "corresponding_present": True,
                         "corresponding_id": 0,
-                        "extended_models_items": [
-                            {
-                                "model_item_index": 0,
-                                "element_offset": 0
-                            }
-                        ]
+                        "extended_models_items": {
+                            "short": [
+                                {
+                                    "model_item_index": 0,
+                                    "element_offset": 0
+                                }
+                            ]
+                        }
                     },
                 ],
                 "vendor_models": [
                     {
                         "extended_items_count": 0,
                         "format": ExtendedModelsItemFormat.SHORT,
                         "corresponding_present": False,
-                        "corresponding_id": None,
-                        "extended_models_items": []
+                        "corresponding_id": 0,
+                        "extended_models_items": {"short": []}
                     },
                 ]
             },
             {
                 "number_s": 1,
                 "number_v": 2,
                 "sig_models": [
                     {
                         "extended_items_count": 0,
                         "format": ExtendedModelsItemFormat.SHORT,
                         "corresponding_present": True,
                         "corresponding_id": 0,
-                        "extended_models_items": []
+                        "extended_models_items": {"short": []}
                     },
                 ],
                 "vendor_models": [
                     {
                         "extended_items_count": 1,
                         "format": ExtendedModelsItemFormat.SHORT,
                         "corresponding_present": True,
                         "corresponding_id": 1,
-                        "extended_models_items": [
-                            {
-                                "model_item_index": 2,
-                                "element_offset": -1
-                            }
-                        ]
+                        "extended_models_items": {
+                            "short": [
+                                {
+                                    "model_item_index": 2,
+                                    "element_offset": -1
+                                }
+                            ]
+                        }
                     },
                     {
                         "extended_items_count": 0,
                         "format": ExtendedModelsItemFormat.SHORT,
                         "corresponding_present": True,
                         "corresponding_id": 1,
-                        "extended_models_items": []
+                        "extended_models_items": {"short": []}
                     }
 
                 ]
             }
         ]
         },
         id="CompositionData Page 1"
@@ -636,95 +640,105 @@
             "number_v": 3,
             "sig_models": [
                 {
                     "extended_items_count": 1,
                     "format": ExtendedModelsItemFormat.LONG,
                     "corresponding_present": True,
                     "corresponding_id": 0x01,
-                    "extended_models_items": [
-                        {
-                            "model_item_index": 26,
-                            "element_offset": -3
-                        }
-                    ]
+                    "extended_models_items": {
+                        "long": [
+                            {
+                                "model_item_index": 26,
+                                "element_offset": -3
+                            }
+                        ]
+                    }
                 },
                 {
                     "extended_items_count": 2,
                     "format": ExtendedModelsItemFormat.SHORT,
                     "corresponding_present": True,
                     "corresponding_id": 0x01,
-                    "extended_models_items": [
-                        {
-                            "model_item_index": 0x07,
-                            "element_offset": 0x00
-                        },
-                        {
-                            "model_item_index": 0x06,
-                            "element_offset": 0x00
-                        }
-                    ]
+                    "extended_models_items": {
+                        "short": [
+                            {
+                                "model_item_index": 0x07,
+                                "element_offset": 0x00
+                            },
+                            {
+                                "model_item_index": 0x06,
+                                "element_offset": 0x00
+                            }
+                        ]
+                    }
                 },
                 {
                     "extended_items_count": 0,
                     "format": ExtendedModelsItemFormat.SHORT,
                     "corresponding_present": True,
                     "corresponding_id": 0x08,
-                    "extended_models_items": []
+                    "extended_models_items": {"short": []}
                 },
                 {
                     "extended_items_count": 1,
                     "format": ExtendedModelsItemFormat.SHORT,
                     "corresponding_present": True,
                     "corresponding_id": 0x08,
-                    "extended_models_items": [
-                        {
-                            "model_item_index": 0x09,
-                            "element_offset": 0x00
-                        }
-                    ]
+                    "extended_models_items": {
+                        "short": [
+                            {
+                                "model_item_index": 0x09,
+                                "element_offset": 0x00
+                            }
+                        ]
+                    }
                 },
                 {
                     "extended_items_count": 0,
                     "format": ExtendedModelsItemFormat.SHORT,
                     "corresponding_present": False,
-                    "corresponding_id": None,
-                    "extended_models_items": []
+                    "corresponding_id": 0,
+                    "extended_models_items": {"short": []}
                 },
             ],
             "vendor_models": [
                         {
                             "extended_items_count": 0,
                             "format": ExtendedModelsItemFormat.SHORT,
                             "corresponding_present": False,
-                            "corresponding_id": None,
-                            "extended_models_items": []
+                            "corresponding_id": 0,
+                            "extended_models_items": {"short": []}
                         },
                         {
                             "extended_items_count": 1,
                             "format": ExtendedModelsItemFormat.SHORT,
                             "corresponding_present": True,
                             "corresponding_id": 0x0A,
-                            "extended_models_items": [
-                                {
-                                    "model_item_index": 0x00,
-                                    "element_offset": 0x00
-                                }
-                            ]
+                            "extended_models_items": {
+                                "short": [
+                                    {
+                                        "model_item_index": 0x00,
+                                        "element_offset": 0x00
+                                    }
+                                ]
+                            }
                         },
                         {
                             "extended_items_count": 1,
                             "format": ExtendedModelsItemFormat.SHORT,
                             "corresponding_present": True,
                             "corresponding_id": 0x0A,
-                            "extended_models_items": [
-                                {
-                                    "model_item_index": 0x1A,
-                                    "element_offset": 0x00
-                                }
-                            ]
+                            "extended_models_items": {
+                                "short": [
+                                    {
+                                        "model_item_index": 0x1A,
+                                        "element_offset": 0x00
+                                    }
+                                ]
+                            }
                         },
                     ]
         },
         id="Config Composition Data Page 1 - single element"
     ),
     pytest.param(
         CompositionDataPage2,
@@ -750,61 +764,65 @@
         ModelRelationItem,
         bytes.fromhex('010A'),
         {
             "extended_items_count": 0,
             "format": ExtendedModelsItemFormat.SHORT,
             "corresponding_present": True,
             "corresponding_id": 10,
-            "extended_models_items": []
+            "extended_models_items": {"short": []}
         },
         id="Config Composition Data Page 1 - Single model item in short format with corresponding"
     ),
     pytest.param(
         ModelRelationItem,
         bytes.fromhex('030B'),
         {
             "extended_items_count": 0,
             "format": ExtendedModelsItemFormat.LONG,
             "corresponding_present": True,
             "corresponding_id": 11,
-            "extended_models_items": []
+            "extended_models_items": {"long": []}
         },
         id="Config Composition Data Page 1 - Single model item in long format with corresponding"
     ),
     pytest.param(
         ModelRelationItem,
         bytes.fromhex('0458'),
         {
             "extended_items_count": 1,
             "format": ExtendedModelsItemFormat.SHORT,
             "corresponding_present": False,
-            "corresponding_id": None,
-            "extended_models_items": [
-                        {
-                            "model_item_index": 0x0B,
-                            "element_offset": 0x00
-                        }
-                    ]
+            "corresponding_id": 0,
+            "extended_models_items": {
+                "short": [
+                    {
+                        "model_item_index": 0x0B,
+                        "element_offset": 0x00
+                    }
+                ]
+            }
         },
         id="Config Composition Data Page 1 - Single model item in short format with extending"
     ),
     pytest.param(
         ModelRelationItem,
         bytes.fromhex('060A0B'),
         {
             "extended_items_count": 1,
             "format": ExtendedModelsItemFormat.LONG,
             "corresponding_present": False,
-            "corresponding_id": None,
-            "extended_models_items": [
-                {
-                    "model_item_index": 10,
-                    "element_offset": 11
-                }
-            ]
+            "corresponding_id": 0,
+            "extended_models_items": {
+                "long": [
+                    {
+                        "model_item_index": 10,
+                        "element_offset": 11
+                    }
+                ]
+            }
         },
         id="Config Composition Data Page 1 - Single model item in long format with extending"
     ),
     pytest.param(
         ConfigDefaultTTLGet,
         bytes(),
         {},
```

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_generics.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_generics.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_health.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_health.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_level.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_level.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_light.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_light.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_scene.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_sensor.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_sensor.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_strings.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_strings.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/test/test_time.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/test/test_time.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/time.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/time.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/messages/util.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/messages/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,20 +35,23 @@
     Bitwise,
     Computed,
     Construct,
     Container,
     Embedded,
     Enum,
     ExprValidator,
+    FuncPath,
     Float32b,
     Float64b,
+    IfThenElse,
     Int8ub,
     Int16ub,
     Int24ub,
     Int32ub,
+    Pass,
     Rebuild,
     Restreamed,
     Select,
     SizeofError,
     Struct,
     Switch,
     ValidationError,
@@ -360,14 +363,44 @@
                 defaultfname,
                 self.default._compileparse(code),
             )
         )
         return "%s.get(%s, %s)(io, this)" % (fname, self.keyfunc, defaultfname)
 
 
+class EnumSwitchStruct(Adapter):
+    def __init__(self, subcon):
+        assert isinstance(subcon, EnumSwitch), "subcon must be an EnumSwitch"
+        assert subcon.default is Pass, "subcon must have a default Pass"
+
+        super().__init__(subcon)
+
+    def _decode(self, obj, context, path):
+        keyfunc = self.subcon.keyfunc
+        if callable(keyfunc):
+            keyfunc = keyfunc(context)
+
+        assert isinstance(keyfunc, enum.Enum), "keyfunc must be an enum"
+
+        return {keyfunc.name.lower(): obj}
+
+    def _encode(self, obj, context, path):
+        keyfunc = self.subcon.keyfunc
+        if callable(keyfunc):
+            keyfunc = keyfunc(context)
+
+        mapping = {_enum.value: _enum.name.lower() for _enum in self.subcon.cases.keys()}
+        key = mapping[keyfunc]
+
+        return obj[key]
+
+
+enum_switch_struct_len_ = FuncPath(lambda arg: len(next(iter(arg.values()))))
+
+
 class SwitchStruct(Adapter):
     def __init__(self, key, switch):
         super().__init__(Struct(key, switch))
         self.key = key
         self.switch = switch
         self._subcon = Struct(key, switch.subcon)
 
@@ -440,14 +473,28 @@
     def _decode(self, obj, context, path):
         return obj
 
     def _encode(self, obj, context, path):
         return obj
 
 
+class IfThenElseDefault(IfThenElse):
+    def __init__(self, condfunc, thensubcon, default):
+        super().__init__(condfunc, thensubcon, Pass)
+        self.condfunc = condfunc
+        self.thensubcon = thensubcon
+        self.default = default
+
+    def _parse(self, stream, context, path):
+        condfunc = self.condfunc
+        if callable(condfunc):
+            condfunc = condfunc(context)
+        return self.thensubcon._parsereport(stream, context, path) if condfunc else self.default
+
+
 def camelcase(field_name):
     if field_name is None:
         return None
 
     head, *tail = str(field_name).lower().replace(" ", "_").split("_")
     return "".join([head, *(i.title() for i in tail)])
```

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/models/base.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/models/base.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/models/models.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/models/models.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/provisioning.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/provisioning.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/fixtures.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_application.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_application.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_construct_match.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_construct_match.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_element.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_element.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_gatherer.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_gatherer.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_key_derivation.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_key_derivation.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_light_lightness_client.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_light_lightness_client.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_mesh.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_model.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_model.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_provisioning.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_provisioning.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_scene_client.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_scene_client.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_security.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_security.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_signal.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_signal.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/test/test_tasklet.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/test/test_tasklet.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/tokenring.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/tokenring.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh/utils.py` & `bluetooth-mesh-0.8.4/bluetooth_mesh/utils.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/PKG-INFO` & `bluetooth-mesh-0.8.4/bluetooth_mesh.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,94 @@
 Metadata-Version: 2.1
 Name: bluetooth-mesh
-Version: 0.8.3
+Version: 0.8.4
 Summary: Bluetooth mesh for Python
 Home-page: http://github.com/silvairgit/python-bluetooth-mesh
 Author-email: michal.lowas-rzechonek@silvair.com
 License: UNKNOWN
-Description: =====================
-        python-bluetooth-mesh
-        =====================
-        
-        .. image:: https://img.shields.io/pypi/v/bluetooth-mesh.svg
-            :target: https://pypi.org/project/bluetooth-mesh
-            :alt: PyPI version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/bluetooth-mesh.svg
-            :target: https://pypi.org/project/bluetooth-mesh
-            :alt: Python versions
-        
-        .. image:: https://app.travis-ci.com/SilvairGit/python-bluetooth-mesh.svg?branch=master
-            :target: https://travis-ci.com/github/SilvairGit/python-bluetooth-mesh
-            :alt: See Build Status on Travis CI
-        
-        .. image:: https://readthedocs.org/projects/python-bluetooth-mesh/badge/?version=latest
-            :target: https://python-bluetooth-mesh.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        Bluetooth mesh SDK for Python allows developing applications communicating with
-        Bluetooth mesh network using BlueZ's bluetooth-meshd.
-        
-        ----
-        
-        What is this thing?
-        -------------------
-        
-        https://www.bluetooth.com/specifications/mesh-specifications
-        
-        https://git.kernel.org/pub/scm/bluetooth/bluez.git/tree/doc/mesh-api.txt
-        
-        
-        Installation
-        ------------
-        
-        You can install "python-bluetooth-mesh" via `pip`_ from `PyPI`_::
-        
-            $ pip install bluetooth-mesh
-        
-        
-        Contributing
-        ------------
-        Contributions are very welcome. Tests can be run with `tox`_, please ensure
-        the coverage at least stays the same before you submit a pull request.
-        
-        
-        License
-        -------
-        
-        Distributed under the terms of the `GPL-2.0`_ license, "python-bluetooth-mesh" is
-        free and open source software
-        
-        
-        Issues
-        ------
-        
-        If you encounter any problems, please `file an issue`_ along with a detailed description.
-        
-        .. _`GPL-2.0`: http://opensource.org/licenses/GPL-2.0
-        .. _`file an issue`: https://github.com/SilvairGit/python-bluetooth-mesh/issues
-        .. _`pytest`: https://github.com/pytest-dev/pytest
-        .. _`tox`: https://tox.readthedocs.io/en/latest/
-        .. _`pip`: https://pypi.org/project/pip/
-        .. _`PyPI`: https://pypi.org/project
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.6.0,<3.11.0
 Description-Content-Type: text/x-rst
-Provides-Extra: capnp
 Provides-Extra: docs
 Provides-Extra: tools
+Provides-Extra: capnp
+License-File: LICENSE
+License-File: AUTHORS
+
+=====================
+python-bluetooth-mesh
+=====================
+
+.. image:: https://img.shields.io/pypi/v/bluetooth-mesh.svg
+    :target: https://pypi.org/project/bluetooth-mesh
+    :alt: PyPI version
+
+.. image:: https://img.shields.io/pypi/pyversions/bluetooth-mesh.svg
+    :target: https://pypi.org/project/bluetooth-mesh
+    :alt: Python versions
+
+.. image:: https://app.travis-ci.com/SilvairGit/python-bluetooth-mesh.svg?branch=master
+    :target: https://travis-ci.com/github/SilvairGit/python-bluetooth-mesh
+    :alt: See Build Status on Travis CI
+
+.. image:: https://readthedocs.org/projects/python-bluetooth-mesh/badge/?version=latest
+    :target: https://python-bluetooth-mesh.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+Bluetooth mesh SDK for Python allows developing applications communicating with
+Bluetooth mesh network using BlueZ's bluetooth-meshd.
+
+----
+
+What is this thing?
+-------------------
+
+https://www.bluetooth.com/specifications/mesh-specifications
+
+https://git.kernel.org/pub/scm/bluetooth/bluez.git/tree/doc/mesh-api.txt
+
+
+Installation
+------------
+
+You can install "python-bluetooth-mesh" via `pip`_ from `PyPI`_::
+
+    $ pip install bluetooth-mesh
+
+
+Contributing
+------------
+Contributions are very welcome. Tests can be run with `tox`_, please ensure
+the coverage at least stays the same before you submit a pull request.
+
+
+License
+-------
+
+Distributed under the terms of the `GPL-2.0`_ license, "python-bluetooth-mesh" is
+free and open source software
+
+
+Issues
+------
+
+If you encounter any problems, please `file an issue`_ along with a detailed description.
+
+.. _`GPL-2.0`: http://opensource.org/licenses/GPL-2.0
+.. _`file an issue`: https://github.com/SilvairGit/python-bluetooth-mesh/issues
+.. _`pytest`: https://github.com/pytest-dev/pytest
+.. _`tox`: https://tox.readthedocs.io/en/latest/
+.. _`pip`: https://pypi.org/project/pip/
+.. _`PyPI`: https://pypi.org/project
+
+
```

### Comparing `bluetooth-mesh-0.8.3/bluetooth_mesh.egg-info/SOURCES.txt` & `bluetooth-mesh-0.8.4/bluetooth_mesh.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -49,27 +49,31 @@
 bluetooth_mesh/messages/silvair/debug.py
 bluetooth_mesh/messages/silvair/debugV2.py
 bluetooth_mesh/messages/silvair/gateway_config_server.py
 bluetooth_mesh/messages/silvair/light_extended_controller.py
 bluetooth_mesh/messages/silvair/network_diagnostic_server.py
 bluetooth_mesh/messages/silvair/rrule_scheduler.py
 bluetooth_mesh/messages/silvair/test/test_debug.py
+bluetooth_mesh/messages/silvair/test/test_debugV2.py
 bluetooth_mesh/messages/silvair/test/test_gateway_config_server.py
 bluetooth_mesh/messages/silvair/test/test_network_diagnostic_server.py
+bluetooth_mesh/messages/silvair/test/test_rrule_scheduler.py
 bluetooth_mesh/messages/test/test_access.py
 bluetooth_mesh/messages/test/test_battery.py
+bluetooth_mesh/messages/test/test_capnproto.py
 bluetooth_mesh/messages/test/test_config.py
 bluetooth_mesh/messages/test/test_generics.py
 bluetooth_mesh/messages/test/test_health.py
 bluetooth_mesh/messages/test/test_level.py
 bluetooth_mesh/messages/test/test_light.py
 bluetooth_mesh/messages/test/test_scene.py
 bluetooth_mesh/messages/test/test_sensor.py
 bluetooth_mesh/messages/test/test_strings.py
 bluetooth_mesh/messages/test/test_time.py
+bluetooth_mesh/messages/test/test_util.py
 bluetooth_mesh/models/__init__.py
 bluetooth_mesh/models/base.py
 bluetooth_mesh/models/models.py
 bluetooth_mesh/test/__init__.py
 bluetooth_mesh/test/fixtures.py
 bluetooth_mesh/test/test_application.py
 bluetooth_mesh/test/test_construct_match.py
```

### Comparing `bluetooth-mesh-0.8.3/docs/Makefile` & `bluetooth-mesh-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/_ext/autoconstruct.py` & `bluetooth-mesh-0.8.4/docs/_ext/autoconstruct.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/api/application.rst` & `bluetooth-mesh-0.8.4/docs/api/application.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/api/messages.rst` & `bluetooth-mesh-0.8.4/docs/api/messages.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/api/models.rst` & `bluetooth-mesh-0.8.4/docs/api/models.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/conf.py` & `bluetooth-mesh-0.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/index.rst` & `bluetooth-mesh-0.8.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/mod/examples/bulk_query.py` & `bluetooth-mesh-0.8.4/docs/mod/examples/bulk_query.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/mod/examples/callbacks.py` & `bluetooth-mesh-0.8.4/docs/mod/examples/callbacks.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/mod/examples/delay.py` & `bluetooth-mesh-0.8.4/docs/mod/examples/delay.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/mod/examples/expect.py` & `bluetooth-mesh-0.8.4/docs/mod/examples/expect.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/mod/examples/model.py` & `bluetooth-mesh-0.8.4/docs/mod/examples/model.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/mod/examples/query.py` & `bluetooth-mesh-0.8.4/docs/mod/examples/query.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/mod/examples/repeat.py` & `bluetooth-mesh-0.8.4/docs/mod/examples/repeat.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/mod/models.rst` & `bluetooth-mesh-0.8.4/docs/mod/models.rst`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/docs/skeleton.py` & `bluetooth-mesh-0.8.4/docs/skeleton.py`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/pyproject.toml` & `bluetooth-mesh-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bluetooth-mesh-0.8.3/setup.py` & `bluetooth-mesh-0.8.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 # fmt: off
 setup(
     name='bluetooth-mesh',
-    version='0.8.3',
+    version='0.8.4',
     author_email='michal.lowas-rzechonek@silvair.com',
     description=(
         'Bluetooth mesh for Python'
     ),
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url='http://github.com/silvairgit/python-bluetooth-mesh',
```

### Comparing `bluetooth-mesh-0.8.3/tox.ini` & `bluetooth-mesh-0.8.4/tox.ini`

 * *Files identical despite different names*

