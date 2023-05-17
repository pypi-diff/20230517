# Comparing `tmp/nzooherd_torch-0.1.0.tar.gz` & `tmp/nzooherd_torch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzooherd_torch-0.1.0.tar", max compression
+gzip compressed data, was "nzooherd_torch-0.1.1.tar", max compression
```

## Comparing `nzooherd_torch-0.1.0.tar` & `nzooherd_torch-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-05-17 04:01:59.853602 nzooherd_torch-0.1.0/nzooherd_torch/__init__.py
--rw-r--r--   0        0        0      326 2023-05-17 04:03:29.962998 nzooherd_torch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 04:01:59.853602 nzooherd_torch-0.1.0/README.md
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 nzooherd_torch-0.1.0/setup.py
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 nzooherd_torch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-05-17 04:30:02.715724 nzooherd_torch-0.1.1/nzooherd_torch/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-17 04:30:12.836457 nzooherd_torch-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 04:01:59.853602 nzooherd_torch-0.1.1/README.md
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 nzooherd_torch-0.1.1/setup.py
+-rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 nzooherd_torch-0.1.1/PKG-INFO
```

