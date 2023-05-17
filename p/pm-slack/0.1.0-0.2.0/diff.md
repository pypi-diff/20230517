# Comparing `tmp/pm_slack-0.1.0.tar.gz` & `tmp/pm_slack-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm_slack-0.1.0.tar", max compression
+gzip compressed data, was "pm_slack-0.2.0.tar", max compression
```

## Comparing `pm_slack-0.1.0.tar` & `pm_slack-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2023-05-17 11:20:49.040098 pm_slack-0.1.0/LICENSE
--rw-r--r--   0        0        0       45 2023-05-17 11:20:49.040098 pm_slack-0.1.0/README.md
--rw-r--r--   0        0        0       76 2023-05-17 11:20:49.040098 pm_slack-0.1.0/pm_slack/__init__.py
--rw-r--r--   0        0        0     1026 2023-05-17 11:20:49.040098 pm_slack-0.1.0/pm_slack/main.py
--rw-r--r--   0        0        0        0 2023-05-17 11:20:49.040098 pm_slack-0.1.0/pm_slack/py.typed
--rw-r--r--   0        0        0      390 2023-05-17 11:20:49.040098 pm_slack-0.1.0/pm_slack/templates/__init__.py
--rw-r--r--   0        0        0     6131 2023-05-17 11:20:49.040098 pm_slack-0.1.0/pm_slack/templates/templates.py
--rw-r--r--   0        0        0     1097 2023-05-17 11:20:49.040098 pm_slack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pm_slack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-17 12:17:41.672465 pm_slack-0.2.0/LICENSE
+-rw-r--r--   0        0        0       45 2023-05-17 12:17:41.672465 pm_slack-0.2.0/README.md
+-rw-r--r--   0        0        0       76 2023-05-17 12:17:41.672465 pm_slack-0.2.0/pm_slack/__init__.py
+-rw-r--r--   0        0        0     1062 2023-05-17 12:17:41.672465 pm_slack-0.2.0/pm_slack/main.py
+-rw-r--r--   0        0        0        0 2023-05-17 12:17:41.672465 pm_slack-0.2.0/pm_slack/py.typed
+-rw-r--r--   0        0        0      390 2023-05-17 12:17:41.672465 pm_slack-0.2.0/pm_slack/templates/__init__.py
+-rw-r--r--   0        0        0     6131 2023-05-17 12:17:41.672465 pm_slack-0.2.0/pm_slack/templates/templates.py
+-rw-r--r--   0        0        0     1097 2023-05-17 12:17:41.672465 pm_slack-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pm_slack-0.2.0/PKG-INFO
```

### Comparing `pm_slack-0.1.0/LICENSE` & `pm_slack-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pm_slack-0.1.0/pm_slack/main.py` & `pm_slack-0.2.0/pm_slack/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from logging import Logger
 
 from slack_sdk import WebClient  # type: ignore
 from templates import Template
```

### Comparing `pm_slack-0.1.0/pm_slack/templates/templates.py` & `pm_slack-0.2.0/pm_slack/templates/templates.py`

 * *Files identical despite different names*

### Comparing `pm_slack-0.1.0/pyproject.toml` & `pm_slack-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pm_slack"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Slack Library for Paket Mutfak"
 authors = ["Paket Mutfak Dev Team <dev@paketmutfak.com.tr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pm_slack-0.1.0/PKG-INFO` & `pm_slack-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm-slack
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Slack Library for Paket Mutfak
 License: MIT
 Author: Paket Mutfak Dev Team
 Author-email: dev@paketmutfak.com.tr
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

