# Comparing `tmp/questdb-connect-0.0.58.tar.gz` & `tmp/questdb-connect-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.58.tar", last modified: Wed May 17 20:05:56 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.59.tar", last modified: Wed May 17 20:56:05 2023, max compression
```

## Comparing `questdb-connect-0.0.58.tar` & `questdb-connect-0.0.59.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:05:56.182206 questdb-connect-0.0.58/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.58/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-17 20:05:56.182053 questdb-connect-0.0.58/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.58/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-17 20:05:21.000000 questdb-connect-0.0.58/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-17 20:05:56.182243 questdb-connect-0.0.58/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:05:56.173318 questdb-connect-0.0.58/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:05:56.175850 questdb-connect-0.0.58/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.58/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.58/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.58/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.58/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.58/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.58/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:05:56.179817 questdb-connect-0.0.58/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.58/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11427 2023-05-16 13:44:28.000000 questdb-connect-0.0.58/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.58/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)     7253 2023-05-17 20:02:56.000000 questdb-connect-0.0.58/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.58/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:05:56.180813 questdb-connect-0.0.58/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-17 20:05:56.000000 questdb-connect-0.0.58/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-17 20:05:56.000000 questdb-connect-0.0.58/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-17 20:05:56.000000 questdb-connect-0.0.58/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-17 20:05:56.000000 questdb-connect-0.0.58/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-17 20:05:56.000000 questdb-connect-0.0.58/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-17 20:05:56.000000 questdb-connect-0.0.58/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:05:56.181595 questdb-connect-0.0.58/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.58/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.58/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.58/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:56:05.570367 questdb-connect-0.0.59/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.59/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-17 20:56:05.569859 questdb-connect-0.0.59/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.59/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-17 20:55:43.000000 questdb-connect-0.0.59/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-17 20:56:05.570480 questdb-connect-0.0.59/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:56:05.558962 questdb-connect-0.0.59/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:56:05.563482 questdb-connect-0.0.59/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.59/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.59/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.59/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.59/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.59/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.59/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:56:05.566072 questdb-connect-0.0.59/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.59/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11427 2023-05-16 13:44:28.000000 questdb-connect-0.0.59/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.59/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     7199 2023-05-17 20:55:43.000000 questdb-connect-0.0.59/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.59/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:56:05.567884 questdb-connect-0.0.59/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-17 20:56:05.000000 questdb-connect-0.0.59/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-17 20:56:05.000000 questdb-connect-0.0.59/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-17 20:56:05.000000 questdb-connect-0.0.59/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-17 20:56:05.000000 questdb-connect-0.0.59/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-17 20:56:05.000000 questdb-connect-0.0.59/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-17 20:56:05.000000 questdb-connect-0.0.59/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 20:56:05.568983 questdb-connect-0.0.59/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.59/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.59/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.59/tests/test_types.py
```

### Comparing `questdb-connect-0.0.58/LICENSE` & `questdb-connect-0.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/PKG-INFO` & `questdb-connect-0.0.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.58
+Version: 0.0.59
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.58/README.md` & `questdb-connect-0.0.59/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/pyproject.toml` & `questdb-connect-0.0.59/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.58'
+version = '0.0.59'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.58/src/examples/__init__.py` & `questdb-connect-0.0.59/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/src/examples/hello_world.py` & `questdb-connect-0.0.59/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.59/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/src/examples/server_utilisation.py` & `questdb-connect-0.0.59/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.59/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.59/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/src/questdb_connect/__init__.py` & `questdb-connect-0.0.59/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/src/questdb_connect/dialect.py` & `questdb-connect-0.0.59/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/src/questdb_connect/function_names.py` & `questdb-connect-0.0.59/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.59/src/questdb_connect/superset_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,36 +59,34 @@
     encryption_parameters = {"sslmode": "prefer"}
     sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname"
     parameters_schema = QDBParametersSchema()
     time_groupby_inline = True
     allows_hidden_cc_in_orderby = True
     time_secondary_columns = True
     try_remove_schema_from_table_name = True
-    supports_dynamic_schema = False
-    allow_dml = True
     max_column_name_length = 120
     top_keywords = {}
 
     _time_grain_expressions = {
-        None: '{col}',
         "PT1S": "date_trunc('second', {col})",
         "PT5S": "date_trunc('second', {col}) + 5000000L",
         "PT30S": "date_trunc('second', {col}) + 30000000L",
         "PT1M": "date_trunc('minute', {col})",
         "PT5M": "date_trunc('minute', {col}) + 300000000L",
         "PT10M": "date_trunc('minute', {col}) + 600000000L",
         "PT15M": "date_trunc('minute', {col}) + 900000000L",
         "PT30M": "date_trunc('minute', {col}) + 1800000000L",
         "PT1H": "date_trunc('hour', {col})",
         "PT6H": "date_trunc('hour', {col}) + 21600000000L",
         "PT1D": "date_trunc('day', {col})",
         "P1W": "date_trunc('week', {col})",
         "P1M": "date_trunc('month', {col})",
         "P1Y": "date_trunc('year', {col})",
-        "P3M": "date_trunc('quarter', {col})"
+        "P3M": "date_trunc('quarter', {col})",
+        "None": '{col}',
     }
 
     column_type_mappings = (
         (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
         (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
         (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
         (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
```

### Comparing `questdb-connect-0.0.58/src/questdb_connect/types.py` & `questdb-connect-0.0.59/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.59/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.58
+Version: 0.0.59
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.58/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.59/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/tests/test_dialect.py` & `questdb-connect-0.0.59/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/tests/test_superset.py` & `questdb-connect-0.0.59/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.58/tests/test_types.py` & `questdb-connect-0.0.59/tests/test_types.py`

 * *Files identical despite different names*

