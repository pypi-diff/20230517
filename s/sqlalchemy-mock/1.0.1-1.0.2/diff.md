# Comparing `tmp/sqlalchemy_mock-1.0.1.tar.gz` & `tmp/sqlalchemy_mock-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mock-1.0.1.tar", max compression
+gzip compressed data, was "sqlalchemy_mock-1.0.2.tar", max compression
```

## Comparing `sqlalchemy_mock-1.0.1.tar` & `sqlalchemy_mock-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.1/README.md
--rw-r--r--   0        0        0      447 2023-05-13 15:03:07.504789 sqlalchemy_mock-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       43 2023-05-13 14:38:38.650764 sqlalchemy_mock-1.0.1/sqlalchemy_mock/__init__.py
--rw-r--r--   0        0        0     2077 2023-05-13 14:38:38.650922 sqlalchemy_mock-1.0.1/sqlalchemy_mock/query.py
--rw-r--r--   0        0        0     1314 2023-05-13 14:38:38.651032 sqlalchemy_mock-1.0.1/sqlalchemy_mock/session.py
--rw-r--r--   0        0        0     2177 2023-05-13 14:38:38.651239 sqlalchemy_mock-1.0.1/sqlalchemy_mock/utils.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.2/README.md
+-rw-r--r--   0        0        0      448 2023-05-17 19:53:35.084165 sqlalchemy_mock-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-05-13 14:38:38.650764 sqlalchemy_mock-1.0.2/sqlalchemy_mock/__init__.py
+-rw-r--r--   0        0        0     2077 2023-05-13 14:38:38.650922 sqlalchemy_mock-1.0.2/sqlalchemy_mock/query.py
+-rw-r--r--   0        0        0     1314 2023-05-13 14:38:38.651032 sqlalchemy_mock-1.0.2/sqlalchemy_mock/session.py
+-rw-r--r--   0        0        0     2182 2023-05-17 19:53:10.850350 sqlalchemy_mock-1.0.2/sqlalchemy_mock/utils.py
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.2/PKG-INFO
```

### Comparing `sqlalchemy_mock-1.0.1/README.md` & `sqlalchemy_mock-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.1/sqlalchemy_mock/query.py` & `sqlalchemy_mock-1.0.2/sqlalchemy_mock/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.1/sqlalchemy_mock/session.py` & `sqlalchemy_mock-1.0.2/sqlalchemy_mock/session.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.1/sqlalchemy_mock/utils.py` & `sqlalchemy_mock-1.0.2/sqlalchemy_mock/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import unittest
+import unittest.mock
 import sqlalchemy
 
 
 def set_choice_fields_to_record(record: object):
     for column in record.__table__.columns:
         if getattr(column.type, "choices", None):
             if isinstance(getattr(record, column.name), str):
```

### Comparing `sqlalchemy_mock-1.0.1/PKG-INFO` & `sqlalchemy_mock-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-mock
-Version: 1.0.1
+Version: 1.0.2
 Summary: The package for working with SQLAlchemy in unit tests
 Author: ivanostapiuk
 Author-email: ost.ivan13@gmail.com
 Requires-Python: >=3.0,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

