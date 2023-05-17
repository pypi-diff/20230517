# Comparing `tmp/pypipr-0.1.88.tar.gz` & `tmp/pypipr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-0.1.88.tar", max compression
+gzip compressed data, was "pypipr-0.1.9.tar", max compression
```

## Comparing `pypipr-0.1.88.tar` & `pypipr-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0        0 2022-10-24 06:22:00.291550 pypipr-0.1.88/pypipr/__init__.py
--rw-r--r--   0        0        0    34168 2023-05-17 11:08:04.140885 pypipr-0.1.88/pypipr/pypipr.py
--rw-r--r--   0        0        0      615 2023-05-17 11:10:17.838909 pypipr-0.1.88/pyproject.toml
--rw-r--r--   0        0        0    14092 2023-05-17 10:55:46.438615 pypipr-0.1.88/README.md
--rw-r--r--   0        0        0    15002 1970-01-01 00:00:00.000000 pypipr-0.1.88/setup.py
--rw-r--r--   0        0        0    14028 1970-01-01 00:00:00.000000 pypipr-0.1.88/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-11 16:47:36.486008 pypipr-0.1.9/pypipr/__init__.py
+-rw-r--r--   0        0        0     1816 2022-10-14 15:45:39.479083 pypipr-0.1.9/pypipr/iconsole.py
+-rw-r--r--   0        0        0      199 2022-10-14 15:23:12.870383 pypipr-0.1.9/pypipr/iconstant.py
+-rw-r--r--   0        0        0      315 2022-10-14 15:23:37.319991 pypipr-0.1.9/pypipr/idatetime.py
+-rw-r--r--   0        0        0      252 2022-10-14 15:24:05.627645 pypipr-0.1.9/pypipr/pypipr.py
+-rw-r--r--   0        0        0      358 2022-10-14 15:54:43.270169 pypipr-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1746 2022-10-14 15:42:50.506147 pypipr-0.1.9/README.md
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 pypipr-0.1.9/setup.py
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 pypipr-0.1.9/PKG-INFO
```

