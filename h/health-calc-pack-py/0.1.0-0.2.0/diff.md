# Comparing `tmp/health_calc_pack_py-0.1.0.tar.gz` & `tmp/health_calc_pack_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "health_calc_pack_py-0.1.0.tar", max compression
+gzip compressed data, was "health_calc_pack_py-0.2.0.tar", max compression
```

## Comparing `health_calc_pack_py-0.1.0.tar` & `health_calc_pack_py-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,9 @@
--rw-r--r--   0        0        0        0 2023-05-17 00:37:39.882931 health_calc_pack_py-0.1.0/health_calc_pack_py/__init__.py
--rw-r--r--   0        0        0      348 2023-05-17 00:37:39.916353 health_calc_pack_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 00:37:39.882931 health_calc_pack_py-0.1.0/README.md
--rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 health_calc_pack_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-17 01:13:19.681769 health_calc_pack_py-0.2.0/health_calc_pack_py/__init__.py
+-rw-r--r--   0        0        0     2198 2023-05-17 02:07:50.108989 health_calc_pack_py-0.2.0/health_calc_pack_py/app.py
+-rw-r--r--   0        0        0      114 2023-05-17 01:13:20.285768 health_calc_pack_py-0.2.0/health_calc_pack_py/imc.py
+-rw-r--r--   0        0        0      869 2023-05-17 01:29:17.749957 health_calc_pack_py-0.2.0/health_calc_pack_py/macronutrientes.py
+-rw-r--r--   0        0        0     2988 2023-05-17 01:52:51.016461 health_calc_pack_py-0.2.0/health_calc_pack_py/static/swagger.json
+-rw-r--r--   0        0        0      234 2023-05-17 01:13:21.222773 health_calc_pack_py-0.2.0/health_calc_pack_py/test_imc.py
+-rw-r--r--   0        0        0      510 2023-05-17 01:48:05.517550 health_calc_pack_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1480 2023-05-17 01:46:36.647277 health_calc_pack_py-0.2.0/README.md
+-rw-r--r--   0        0        0     1970 1970-01-01 00:00:00.000000 health_calc_pack_py-0.2.0/PKG-INFO
```

