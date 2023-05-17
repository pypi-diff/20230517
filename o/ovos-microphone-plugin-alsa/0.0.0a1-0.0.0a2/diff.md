# Comparing `tmp/ovos-microphone-plugin-alsa-0.0.0a1.tar.gz` & `tmp/ovos-microphone-plugin-alsa-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-microphone-plugin-alsa-0.0.0a1.tar", last modified: Wed May 17 19:44:54 2023, max compression
+gzip compressed data, was "ovos-microphone-plugin-alsa-0.0.0a2.tar", last modified: Wed May 17 19:45:06 2023, max compression
```

## Comparing `ovos-microphone-plugin-alsa-0.0.0a1.tar` & `ovos-microphone-plugin-alsa-0.0.0a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:44:54.618583 ovos-microphone-plugin-alsa-0.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-17 19:44:46.000000 ovos-microphone-plugin-alsa-0.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 19:44:46.000000 ovos-microphone-plugin-alsa-0.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-17 19:44:54.618583 ovos-microphone-plugin-alsa-0.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 19:44:46.000000 ovos-microphone-plugin-alsa-0.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:44:54.614583 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-17 19:44:46.000000 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-17 19:44:49.000000 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:44:54.614583 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-17 19:44:54.000000 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-17 19:44:54.000000 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:44:54.000000 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-17 19:44:54.000000 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 19:44:54.000000 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 19:44:54.000000 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:44:54.000000 ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:44:54.618583 ovos-microphone-plugin-alsa-0.0.0a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3121 2023-05-17 19:44:46.000000 ovos-microphone-plugin-alsa-0.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:45:06.813443 ovos-microphone-plugin-alsa-0.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-17 19:44:57.000000 ovos-microphone-plugin-alsa-0.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 19:44:57.000000 ovos-microphone-plugin-alsa-0.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-17 19:45:06.813443 ovos-microphone-plugin-alsa-0.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 19:44:57.000000 ovos-microphone-plugin-alsa-0.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:45:06.809443 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-17 19:44:57.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-17 19:45:00.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:45:06.809443 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:45:06.813443 ovos-microphone-plugin-alsa-0.0.0a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3121 2023-05-17 19:44:57.000000 ovos-microphone-plugin-alsa-0.0.0a2/setup.py
```

### Comparing `ovos-microphone-plugin-alsa-0.0.0a1/LICENSE` & `ovos-microphone-plugin-alsa-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-microphone-plugin-alsa-0.0.0a1/PKG-INFO` & `ovos-microphone-plugin-alsa-0.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-microphone-plugin-alsa
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A alsa microphone implementation for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-microphone-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin listener microphone alsa
```

### Comparing `ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa/__init__.py` & `ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-microphone-plugin-alsa-0.0.0a1/ovos_microphone_plugin_alsa.egg-info/PKG-INFO` & `ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-microphone-plugin-alsa
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A alsa microphone implementation for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-microphone-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin listener microphone alsa
```

### Comparing `ovos-microphone-plugin-alsa-0.0.0a1/setup.py` & `ovos-microphone-plugin-alsa-0.0.0a2/setup.py`

 * *Files identical despite different names*

