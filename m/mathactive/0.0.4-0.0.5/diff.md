# Comparing `tmp/mathactive-0.0.4.tar.gz` & `tmp/mathactive-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathactive-0.0.4.tar", max compression
+gzip compressed data, was "mathactive-0.0.5.tar", max compression
```

## Comparing `mathactive-0.0.4.tar` & `mathactive-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    34336 2023-03-24 02:28:44.521708 mathactive-0.0.4/LICENSE.md
--rw-r--r--   0        0        0      570 2023-05-17 03:51:26.723214 mathactive-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-07 16:23:10.191094 mathactive-0.0.4/src/mathactive/__init__.py
--rw-r--r--   0        0        0      820 2023-03-24 02:28:44.525707 mathactive-0.0.4/src/mathactive/data/difficulty_start_stop_step.csv
--rw-r--r--   0        0        0     1066 2023-03-24 02:28:44.525707 mathactive-0.0.4/src/mathactive/generators.py
--rw-r--r--   0        0        0      427 2023-03-24 02:28:44.525707 mathactive-0.0.4/src/mathactive/hints.py
--rw-r--r--   0        0        0     3470 2023-03-03 18:38:05.790120 mathactive-0.0.4/src/mathactive/machine.py
--rwxr-xr-x   0        0        0      663 2023-03-24 02:28:44.525707 mathactive-0.0.4/src/mathactive/manage.py
--rw-r--r--   0        0        0     2575 2023-03-24 02:28:44.525707 mathactive-0.0.4/src/mathactive/microlessons/num_one.py
--rw-r--r--   0        0        0      822 2023-03-24 02:28:44.525707 mathactive-0.0.4/src/mathactive/microlessons/utils.py
--rw-r--r--   0        0        0     2732 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/personalize.py
--rw-r--r--   0        0        0     1813 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/python_quiz.py
--rw-r--r--   0        0        0     1191 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/questions.py
--rw-r--r--   0        0        0     2594 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/utils.py
--rw-r--r--   0        0        0        0 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/webapp/__init__.py
--rw-r--r--   0        0        0       63 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/webapp/admin.py
--rw-r--r--   0        0        0      144 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/webapp/apps.py
--rw-r--r--   0        0        0        0 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/webapp/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/webapp/models.py
--rw-r--r--   0        0        0       60 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/webapp/tests.py
--rw-r--r--   0        0        0       63 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/webapp/views.py
--rw-r--r--   0        0        0        0 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/website/__init__.py
--rw-r--r--   0        0        0      402 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/website/asgi.py
--rw-r--r--   0        0        0     3224 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/website/settings.py
--rw-r--r--   0        0        0      749 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/website/urls.py
--rw-r--r--   0        0        0      391 2023-03-24 02:28:44.529707 mathactive-0.0.4/src/mathactive/website/wsgi.py
--rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 mathactive-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34336 2023-03-24 02:28:44.521708 mathactive-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0      507 2023-05-17 03:56:17.934040 mathactive-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-07 16:23:10.191094 mathactive-0.0.5/src/mathactive/__init__.py
+-rw-r--r--   0        0        0      820 2023-03-24 02:28:44.525707 mathactive-0.0.5/src/mathactive/data/difficulty_start_stop_step.csv
+-rw-r--r--   0        0        0     1066 2023-03-24 02:28:44.525707 mathactive-0.0.5/src/mathactive/generators.py
+-rw-r--r--   0        0        0      427 2023-03-24 02:28:44.525707 mathactive-0.0.5/src/mathactive/hints.py
+-rw-r--r--   0        0        0     3470 2023-03-03 18:38:05.790120 mathactive-0.0.5/src/mathactive/machine.py
+-rwxr-xr-x   0        0        0      663 2023-03-24 02:28:44.525707 mathactive-0.0.5/src/mathactive/manage.py
+-rw-r--r--   0        0        0     2575 2023-03-24 02:28:44.525707 mathactive-0.0.5/src/mathactive/microlessons/num_one.py
+-rw-r--r--   0        0        0      822 2023-03-24 02:28:44.525707 mathactive-0.0.5/src/mathactive/microlessons/utils.py
+-rw-r--r--   0        0        0     2732 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/personalize.py
+-rw-r--r--   0        0        0     1813 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/python_quiz.py
+-rw-r--r--   0        0        0     1191 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/questions.py
+-rw-r--r--   0        0        0     2594 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/utils.py
+-rw-r--r--   0        0        0        0 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/webapp/__init__.py
+-rw-r--r--   0        0        0       63 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/webapp/admin.py
+-rw-r--r--   0        0        0      144 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/webapp/apps.py
+-rw-r--r--   0        0        0        0 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/webapp/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/webapp/models.py
+-rw-r--r--   0        0        0       60 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/webapp/tests.py
+-rw-r--r--   0        0        0       63 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/webapp/views.py
+-rw-r--r--   0        0        0        0 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/website/__init__.py
+-rw-r--r--   0        0        0      402 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/website/asgi.py
+-rw-r--r--   0        0        0     3224 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/website/settings.py
+-rw-r--r--   0        0        0      749 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/website/urls.py
+-rw-r--r--   0        0        0      391 2023-03-24 02:28:44.529707 mathactive-0.0.5/src/mathactive/website/wsgi.py
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 mathactive-0.0.5/PKG-INFO
```

### Comparing `mathactive-0.0.4/LICENSE.md` & `mathactive-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/data/difficulty_start_stop_step.csv` & `mathactive-0.0.5/src/mathactive/data/difficulty_start_stop_step.csv`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/generators.py` & `mathactive-0.0.5/src/mathactive/generators.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/machine.py` & `mathactive-0.0.5/src/mathactive/machine.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/manage.py` & `mathactive-0.0.5/src/mathactive/manage.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/microlessons/num_one.py` & `mathactive-0.0.5/src/mathactive/microlessons/num_one.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/microlessons/utils.py` & `mathactive-0.0.5/src/mathactive/microlessons/utils.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/personalize.py` & `mathactive-0.0.5/src/mathactive/personalize.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/python_quiz.py` & `mathactive-0.0.5/src/mathactive/python_quiz.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/questions.py` & `mathactive-0.0.5/src/mathactive/questions.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/utils.py` & `mathactive-0.0.5/src/mathactive/utils.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/website/settings.py` & `mathactive-0.0.5/src/mathactive/website/settings.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/src/mathactive/website/urls.py` & `mathactive-0.0.5/src/mathactive/website/urls.py`

 * *Files identical despite different names*

### Comparing `mathactive-0.0.4/PKG-INFO` & `mathactive-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathactive
-Version: 0.0.4
+Version: 0.0.5
 Summary: Conversational math active learning.
 License: AGPLv3
 Author: hobs
 Author-email: hobson@totalgood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -13,10 +13,10 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django
-Requires-Dist: fastapi
+Requires-Dist: django (==4.2.1)
+Requires-Dist: fastapi (==0.95.2)
 Requires-Dist: mathtext (==0.0.6)
```

