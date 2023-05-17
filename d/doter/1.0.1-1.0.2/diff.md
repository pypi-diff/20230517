# Comparing `tmp/doter-1.0.1.tar.gz` & `tmp/doter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doter-1.0.1.tar", max compression
+gzip compressed data, was "doter-1.0.2.tar", max compression
```

## Comparing `doter-1.0.1.tar` & `doter-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,12 @@
--rw-r--r--   0        0        0    11358 2022-07-10 13:29:02.378083 doter-1.0.1/LICENSE
--rw-r--r--   0        0        0        0 2022-07-10 13:29:02.378083 doter-1.0.1/doter/__init__.py
--rw-r--r--   0        0        0      134 2022-07-10 13:29:02.378083 doter-1.0.1/doter/__main__.py
--rw-r--r--   0        0        0     3649 2022-07-10 13:29:02.378083 doter-1.0.1/doter/app.py
--rw-r--r--   0        0        0        0 2022-07-10 13:29:02.378083 doter-1.0.1/doter/commands/__init__.py
--rw-r--r--   0        0        0     2128 2022-07-10 13:29:02.378083 doter-1.0.1/doter/commands/backup.py
--rw-r--r--   0        0        0     1536 2022-07-10 13:29:02.378083 doter-1.0.1/doter/commands/clean.py
--rw-r--r--   0        0        0      592 2022-07-10 13:29:02.378083 doter-1.0.1/doter/commands/command.py
--rw-r--r--   0        0        0     3004 2022-07-10 13:29:02.378083 doter-1.0.1/doter/commands/install.py
--rw-r--r--   0        0        0     1572 2022-07-10 13:29:02.378083 doter-1.0.1/doter/commands/link.py
--rw-r--r--   0        0        0     1015 2022-07-10 13:29:02.378083 doter-1.0.1/doter/dotfile.py
--rw-r--r--   0        0        0     1298 2022-07-10 13:29:02.378083 doter-1.0.1/doter/eventbus.py
--rw-r--r--   0        0        0      179 2022-07-10 13:29:02.378083 doter-1.0.1/doter/events.py
--rw-r--r--   0        0        0      388 2022-07-10 13:29:02.378083 doter-1.0.1/doter/tpyings.py
--rw-r--r--   0        0        0     4426 2022-07-10 13:29:02.378083 doter-1.0.1/doter/ui.py
--rw-r--r--   0        0        0     3558 2022-07-10 13:29:02.378083 doter-1.0.1/doter/utils.py
--rw-r--r--   0        0        0      495 2022-07-10 13:29:02.378083 doter-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      762 2022-07-10 13:29:41.179570 doter-1.0.1/setup.py
--rw-r--r--   0        0        0      534 2022-07-10 13:29:41.179958 doter-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-17 13:07:57.424778 doter-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3540 2023-05-17 13:07:57.424778 doter-1.0.2/doter/commands/__init__.py
+-rw-r--r--   0        0        0     1682 2023-05-17 13:07:57.424778 doter-1.0.2/doter/commands/clean.py
+-rw-r--r--   0        0        0     3181 2023-05-17 13:07:57.424778 doter-1.0.2/doter/commands/install.py
+-rw-r--r--   0        0        0      600 2023-05-17 13:07:57.424778 doter-1.0.2/doter/config/__init__.py
+-rw-r--r--   0        0        0      667 2023-05-17 13:07:57.424778 doter-1.0.2/doter/exceptions.py
+-rw-r--r--   0        0        0      875 2023-05-17 13:07:57.424778 doter-1.0.2/doter/ui/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-17 13:07:57.424778 doter-1.0.2/doter/ui/cleanup_ui.py
+-rw-r--r--   0        0        0     2719 2023-05-17 13:07:57.424778 doter-1.0.2/doter/ui/install_ui.py
+-rw-r--r--   0        0        0     8132 2023-05-17 13:07:57.424778 doter-1.0.2/doter/utils.py
+-rw-r--r--   0        0        0      557 2023-05-17 13:07:57.424778 doter-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 doter-1.0.2/PKG-INFO
```

### Comparing `doter-1.0.1/LICENSE` & `doter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doter-1.0.1/PKG-INFO` & `doter-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: doter
-Version: 1.0.1
+Version: 1.0.2
 Summary: A dotfile manager
 License: MIT
 Author: Alex Zhang
 Author-email: zhangchi0104@live.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: fire (>=0.4.0,<0.5.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: joblib (>=1.2.0,<2.0.0)
+Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=10.15.2,<11.0.0)
```

