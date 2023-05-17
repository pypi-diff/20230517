# Comparing `tmp/honeybee-doe2-0.0.5.tar.gz` & `tmp/honeybee-doe2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.0.5.tar", last modified: Tue May 16 02:06:32 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.1.0.tar", last modified: Wed May 17 16:08:24 2023, max compression
```

## Comparing `honeybee-doe2-0.0.5.tar` & `honeybee-doe2-0.1.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-16 02:06:31.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:06:31.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 02:06:31.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 02:06:31.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 02:06:31.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-17 16:07:11.000000 honeybee-doe2-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-17 16:07:11.000000 honeybee-doe2-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-17 16:07:11.000000 honeybee-doe2-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 16:07:11.000000 honeybee-doe2-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-17 16:07:11.000000 honeybee-doe2-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-17 16:07:11.000000 honeybee-doe2-0.1.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/shades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 16:08:23.000000 honeybee-doe2-0.1.0/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:08:23.000000 honeybee-doe2-0.1.0/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-17 16:08:23.000000 honeybee-doe2-0.1.0/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 16:08:23.000000 honeybee-doe2-0.1.0/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 16:08:23.000000 honeybee-doe2-0.1.0/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 16:08:24.000000 honeybee-doe2-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-17 16:07:12.000000 honeybee-doe2-0.1.0/setup.py
```

### Comparing `honeybee-doe2-0.0.5/LICENSE` & `honeybee-doe2-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/PKG-INFO` & `honeybee-doe2-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.0.5
+Version: 0.1.0
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.0.5/README.md` & `honeybee-doe2-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.1.0/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.1.0/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.1.0/honeybee_doe2/geometry/polygon.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ..utils.doe_formatters import short_name
 from honeybee.face import Face
+from honeybee.shade import Shade
 from ladybug_geometry.geometry3d import Vector3D, Plane, Face3D
 from ladybug_geometry.geometry2d import Point2D
 import math
 
 
 class DoePolygon(object):
     "A Doe2 Polygon."
@@ -15,15 +16,15 @@
 
     @classmethod
     def from_face(cls, face: Face, flip=False):
         """
         Create a DoePolygon from a Honeybee Face.
 
         Args:
-            face: A Face3D object.
+            face: A Face object.
 
         """
         name = short_name(face.display_name)
 
         geometry: Face3D = face.geometry
 
         rel_plane = geometry.plane
```

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/aperture.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/groundcontact.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .inputils.run_period import RunPeriod
 from .inputils.title import Title
 
 from .story import Doe2Story
 from .constructions import Construction, ConstructionCollection
 
 from .hvac import HVACSystem, Zone
+from .shades import Doe2Shade, Doe2ShadeCollection
 
 
 class ModelDoe2Properties(object):
     """_summary_
 
     Args:
         object (_type_): _description_
@@ -91,14 +92,25 @@
         return self._get_hvac_sys_zones(self.stories)
 
     @staticmethod
     def _get_hvac_sys_zones(stories):
         hvac_sys_zones = [HVACSystem.from_story(story) for story in stories]
         return hvac_sys_zones
 
+    @property
+    def fixed_shades(self):
+        return self._get_fixed_shades(self.host)
+
+    @staticmethod
+    def _get_fixed_shades(obj):
+        if obj.shades is not None:
+            return Doe2ShadeCollection.from_hb_shades(obj.shades).to_inp()
+        else:
+            return None
+
     def __str__(self):
         return "Model Doe2 Properties: [host: {}]".format(self.host.display_name)
 
     def __repr__(self):
         return str(self)
 
     def ToString(self):
```

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/roof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/story.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.1.0/honeybee_doe2/properties/wall.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.1.0/honeybee_doe2/utils/doe_formatters.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/utils/geometry.py` & `honeybee-doe2-0.1.0/honeybee_doe2/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2/writer.py` & `honeybee-doe2-0.1.0/honeybee_doe2/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     sb_data = sbd()
 
     hb_model.convert_to_units(units='Feet')
 
     room_mapper = {
         r.identifier: r.display_name for r in hb_model.rooms
     }
-
+    for i, shade in enumerate(hb_model.shades):
+        shade.display_name = f'shade_{i}'
     for face in hb_model.faces:
         if isinstance(face.boundary_condition, Surface):
             adj_room_identifier = face.boundary_condition.boundary_condition_objects[1]
             face.user_data = {'adjacent_room': room_mapper[adj_room_identifier]}
 
     for i, room in enumerate(hb_model.rooms):
         room_name = room.display_name
@@ -73,15 +74,15 @@
         fb.mats_layers,
         hb_model.properties.doe2.mats_cons_layers,
         fb.glzCode,
         '\n'.join(gt.to_inp() for gt in window_constructions),
         fb.polygons,
         '\n'.join(s.story_poly for s in hb_model.properties.doe2.stories),
         fb.wallParams,
-        # '\n'.join(shd.to_inp() for shd in hb_model.context_shades),  # TODO shade support
+        hb_model.properties.doe2.fixed_shades,
         fb.miscCost,
         fb.perfCurve,
         fb.floorNspace,
         '\n'.join(str(story) for story in hb_model.properties.doe2.stories),
         fb.elecFuelMeter,
         fb.elec_meter,
         fb.fuel_meter,
```

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.1.0/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.0.5
+Version: 0.1.0
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.0.5/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.1.0/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 honeybee_doe2/properties/face.py
 honeybee_doe2/properties/groundcontact.py
 honeybee_doe2/properties/hvac.py
 honeybee_doe2/properties/materials.py
 honeybee_doe2/properties/model.py
 honeybee_doe2/properties/roof.py
 honeybee_doe2/properties/room.py
+honeybee_doe2/properties/shades.py
 honeybee_doe2/properties/story.py
 honeybee_doe2/properties/wall.py
 honeybee_doe2/properties/inputils/__init__.py
 honeybee_doe2/properties/inputils/blocks.py
 honeybee_doe2/properties/inputils/compliance.py
 honeybee_doe2/properties/inputils/glass_types.py
 honeybee_doe2/properties/inputils/run_period.py
```

### Comparing `honeybee-doe2-0.0.5/setup.py` & `honeybee-doe2-0.1.0/setup.py`

 * *Files identical despite different names*

