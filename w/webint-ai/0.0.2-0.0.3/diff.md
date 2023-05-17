# Comparing `tmp/webint_ai-0.0.2.tar.gz` & `tmp/webint_ai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_ai-0.0.2.tar", max compression
+gzip compressed data, was "webint_ai-0.0.3.tar", max compression
```

## Comparing `webint_ai-0.0.2.tar` & `webint_ai-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      623 2023-03-21 21:33:00.853559 webint_ai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1517 2023-03-21 07:06:35.172968 webint_ai-0.0.2/webint_ai/__init__.py
--rw-r--r--   0        0        0      156 2023-03-21 01:32:45.174619 webint_ai-0.0.2/webint_ai/templates/__init__.py
--rw-r--r--   0        0        0       84 2023-03-20 23:10:50.085902 webint_ai-0.0.2/webint_ai/templates/chat.html
--rw-r--r--   0        0        0      433 2023-03-21 02:37:31.970964 webint_ai-0.0.2/webint_ai/templates/chat_response.html
--rw-r--r--   0        0        0      348 2023-03-21 00:46:08.183348 webint_ai-0.0.2/webint_ai/templates/index.html
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 webint_ai-0.0.2/setup.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 webint_ai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      623 2023-05-17 18:22:26.621543 webint_ai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3865 2023-05-17 01:45:45.623398 webint_ai-0.0.3/webint_ai/__init__.py
+-rw-r--r--   0        0        0      156 2023-03-21 01:32:45.174619 webint_ai-0.0.3/webint_ai/templates/__init__.py
+-rw-r--r--   0        0        0       84 2023-03-20 23:10:50.085902 webint_ai-0.0.3/webint_ai/templates/chat.html
+-rw-r--r--   0        0        0      433 2023-03-21 02:37:31.970964 webint_ai-0.0.3/webint_ai/templates/chat_response.html
+-rw-r--r--   0        0        0      367 2023-03-22 00:34:09.529026 webint_ai-0.0.3/webint_ai/templates/index.html
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 webint_ai-0.0.3/setup.py
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 webint_ai-0.0.3/PKG-INFO
```

### Comparing `webint_ai-0.0.2/pyproject.toml` & `webint_ai-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-ai"
-version = "0.0.2"
+version = "0.0.3"
 description = "interface artificial intelligence"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 packages = [{include = "webint_ai"}]
 
 [tool.poetry.plugins."webapps"]
 ai = "webint_ai:app"
```

### Comparing `webint_ai-0.0.2/setup.py` & `webint_ai-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['markdown>=3.4.1,<4.0.0', 'openai>=0.27.2,<0.28.0', 'webint>=0.0']
 
 entry_points = \
 {'webapps': ['ai = webint_ai:app']}
 
 setup_kwargs = {
     'name': 'webint-ai',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'interface artificial intelligence',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `webint_ai-0.0.2/PKG-INFO` & `webint_ai-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webint-ai
-Version: 0.0.2
+Version: 0.0.3
 Summary: interface artificial intelligence
 License: AGPL-3.0-or-later
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

