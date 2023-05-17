# Comparing `tmp/piicli-0.0.1.tar.gz` & `tmp/piicli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "piicli-0.0.2.tar", max compression
```

## Comparing `piicli-0.0.1.tar` & `piicli-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,7 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 piicli-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 piicli-0.0.1/.idea/P1.iml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 piicli-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 piicli-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 piicli-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 piicli-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 piicli-0.0.1/src/piicli/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 piicli-0.0.1/src/piicli/main.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 piicli-0.0.1/LICENSE
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 piicli-0.0.1/README.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 piicli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 piicli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 09:44:17.758376 piicli-0.0.2/LICENSE
+-rw-r--r--   0        0        0      170 2023-05-16 09:44:41.423465 piicli-0.0.2/README.md
+-rw-r--r--   0        0        0      719 2023-05-17 12:26:00.167399 piicli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 11:11:21.834362 piicli-0.0.2/src/piicli/__init__.py
+-rw-r--r--   0        0        0     4552 2023-05-17 12:22:45.339270 piicli-0.0.2/src/piicli/main.py
+-rw-r--r--   0        0        0      331 2023-05-17 10:39:02.171793 piicli-0.0.2/src/piicli/utils.py
+-rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 piicli-0.0.2/PKG-INFO
```

### Comparing `piicli-0.0.1/LICENSE` & `piicli-0.0.2/LICENSE`

 * *Files identical despite different names*

