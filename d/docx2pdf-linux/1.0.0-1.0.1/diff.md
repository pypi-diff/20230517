# Comparing `tmp/docx2pdf-linux-1.0.0.tar.gz` & `tmp/docx2pdf-linux-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx2pdf-linux-1.0.0.tar", last modified: Wed May 17 03:19:28 2023, max compression
+gzip compressed data, was "docx2pdf-linux-1.0.1.tar", last modified: Wed May 17 03:30:26 2023, max compression
```

## Comparing `docx2pdf-linux-1.0.0.tar` & `docx2pdf-linux-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 03:19:28.363363 docx2pdf-linux-1.0.0/
--rw-rw-rw-   0        0        0      136 2023-05-17 03:19:28.360347 docx2pdf-linux-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 03:19:28.307426 docx2pdf-linux-1.0.0/docx2pdf_linux/
--rw-rw-rw-   0        0        0       39 2023-05-17 03:16:09.000000 docx2pdf-linux-1.0.0/docx2pdf_linux/__init__.py
--rw-rw-rw-   0        0        0      167 2023-05-17 03:09:22.000000 docx2pdf-linux-1.0.0/docx2pdf_linux/converter.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:19:28.355434 docx2pdf-linux-1.0.0/docx2pdf_linux.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-17 03:19:27.000000 docx2pdf-linux-1.0.0/docx2pdf_linux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-17 03:19:28.000000 docx2pdf-linux-1.0.0/docx2pdf_linux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 03:19:28.000000 docx2pdf-linux-1.0.0/docx2pdf_linux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 03:19:28.000000 docx2pdf-linux-1.0.0/docx2pdf_linux.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-17 03:19:28.000000 docx2pdf-linux-1.0.0/docx2pdf_linux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 03:19:28.365345 docx2pdf-linux-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      270 2023-05-17 03:09:49.000000 docx2pdf-linux-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:30:26.267351 docx2pdf-linux-1.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-05-17 03:26:45.000000 docx2pdf-linux-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2416 2023-05-17 03:30:26.264721 docx2pdf-linux-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1537 2023-05-17 03:27:08.000000 docx2pdf-linux-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 03:30:26.216658 docx2pdf-linux-1.0.1/docx2pdf_linux/
+-rw-rw-rw-   0        0        0       39 2023-05-17 03:16:09.000000 docx2pdf-linux-1.0.1/docx2pdf_linux/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-05-17 03:09:22.000000 docx2pdf-linux-1.0.1/docx2pdf_linux/converter.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:30:26.258725 docx2pdf-linux-1.0.1/docx2pdf_linux.egg-info/
+-rw-rw-rw-   0        0        0     2416 2023-05-17 03:30:25.000000 docx2pdf-linux-1.0.1/docx2pdf_linux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-17 03:30:26.000000 docx2pdf-linux-1.0.1/docx2pdf_linux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 03:30:25.000000 docx2pdf-linux-1.0.1/docx2pdf_linux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 03:30:25.000000 docx2pdf-linux-1.0.1/docx2pdf_linux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-17 03:30:25.000000 docx2pdf-linux-1.0.1/docx2pdf_linux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 03:30:26.267351 docx2pdf-linux-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1188 2023-05-17 03:30:16.000000 docx2pdf-linux-1.0.1/setup.py
```

