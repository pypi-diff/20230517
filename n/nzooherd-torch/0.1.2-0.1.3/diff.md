# Comparing `tmp/nzooherd_torch-0.1.2.tar.gz` & `tmp/nzooherd_torch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzooherd_torch-0.1.2.tar", max compression
+gzip compressed data, was "nzooherd_torch-0.1.3.tar", max compression
```

## Comparing `nzooherd_torch-0.1.2.tar` & `nzooherd_torch-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-05-17 04:43:54.755953 nzooherd_torch-0.1.2/nzooherd_torch/__init__.py
--rw-r--r--   0        0        0      326 2023-05-17 04:44:17.726077 nzooherd_torch-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 04:01:59.853602 nzooherd_torch-0.1.2/README.md
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 nzooherd_torch-0.1.2/setup.py
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 nzooherd_torch-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-05-17 07:57:57.276164 nzooherd_torch-0.1.3/nzooherd_torch/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-17 12:25:34.675156 nzooherd_torch-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 04:01:59.853602 nzooherd_torch-0.1.3/README.md
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 nzooherd_torch-0.1.3/setup.py
+-rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 nzooherd_torch-0.1.3/PKG-INFO
```

