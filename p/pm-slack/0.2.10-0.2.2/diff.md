# Comparing `tmp/pm_slack-0.2.10.tar.gz` & `tmp/pm_slack-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm_slack-0.2.10.tar", max compression
+gzip compressed data, was "pm_slack-0.2.2.tar", max compression
```

## Comparing `pm_slack-0.2.10.tar` & `pm_slack-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2023-05-17 14:35:26.265610 pm_slack-0.2.10/LICENSE
--rw-r--r--   0        0        0       45 2023-05-17 14:35:26.265610 pm_slack-0.2.10/README.md
--rw-r--r--   0        0        0       76 2023-05-17 14:35:26.265610 pm_slack-0.2.10/pm_slack/__init__.py
--rw-r--r--   0        0        0     1064 2023-05-17 14:35:26.265610 pm_slack-0.2.10/pm_slack/main.py
--rw-r--r--   0        0        0        0 2023-05-17 14:35:26.265610 pm_slack-0.2.10/pm_slack/py.typed
--rw-r--r--   0        0        0      391 2023-05-17 14:35:26.265610 pm_slack-0.2.10/pm_slack/templates/__init__.py
--rw-r--r--   0        0        0     6131 2023-05-17 14:35:26.265610 pm_slack-0.2.10/pm_slack/templates/_templates.py
--rw-r--r--   0        0        0     1099 2023-05-17 14:35:48.073884 pm_slack-0.2.10/pyproject.toml
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 pm_slack-0.2.10/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-17 13:00:09.942545 pm_slack-0.2.2/LICENSE
+-rw-r--r--   0        0        0       45 2023-05-17 13:00:09.942545 pm_slack-0.2.2/README.md
+-rw-r--r--   0        0        0       76 2023-05-17 13:00:09.942545 pm_slack-0.2.2/pm_slack/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-17 13:00:09.942545 pm_slack-0.2.2/pm_slack/main.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:00:09.942545 pm_slack-0.2.2/pm_slack/py.typed
+-rw-r--r--   0        0        0      391 2023-05-17 13:00:09.942545 pm_slack-0.2.2/pm_slack/templates/__init__.py
+-rw-r--r--   0        0        0     6131 2023-05-17 13:00:09.942545 pm_slack-0.2.2/pm_slack/templates/_templates.py
+-rw-r--r--   0        0        0     1098 2023-05-17 13:00:32.242980 pm_slack-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pm_slack-0.2.2/PKG-INFO
```

### Comparing `pm_slack-0.2.10/LICENSE` & `pm_slack-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pm_slack-0.2.10/pm_slack/main.py` & `pm_slack-0.2.2/pm_slack/main.py`

 * *Files identical despite different names*

### Comparing `pm_slack-0.2.10/pm_slack/templates/_templates.py` & `pm_slack-0.2.2/pm_slack/templates/_templates.py`

 * *Files identical despite different names*

### Comparing `pm_slack-0.2.10/pyproject.toml` & `pm_slack-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pm_slack"
-version = "v0.2.10"
+version = "v0.2.2"
 description = "A Slack Library for Paket Mutfak"
 authors = ["Paket Mutfak Dev Team <dev@paketmutfak.com.tr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pm_slack-0.2.10/PKG-INFO` & `pm_slack-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm-slack
-Version: 0.2.10
+Version: 0.2.2
 Summary: A Slack Library for Paket Mutfak
 License: MIT
 Author: Paket Mutfak Dev Team
 Author-email: dev@paketmutfak.com.tr
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

