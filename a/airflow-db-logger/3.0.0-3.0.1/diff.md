# Comparing `tmp/airflow_db_logger-3.0.0.tar.gz` & `tmp/airflow_db_logger-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_db_logger-3.0.0.tar", last modified: Fri Apr 21 19:23:41 2023, max compression
+gzip compressed data, was "airflow_db_logger-3.0.1.tar", last modified: Wed May 17 14:42:56 2023, max compression
```

## Comparing `airflow_db_logger-3.0.0.tar` & `airflow_db_logger-3.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:41.413793 airflow_db_logger-3.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)       18 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-21 19:23:41.413793 airflow_db_logger-3.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3308 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:41.413793 airflow_db_logger-3.0.0/airflow_db_logger/
--rwxr-xr-x   0 runner    (1001) docker     (123)      700 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/airlfow_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4865 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2537 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/db.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4174 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/operators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2562 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/shell_logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2310 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:41.413793 airflow_db_logger-3.0.0/airflow_db_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-21 19:23:41.000000 airflow_db_logger-3.0.0/airflow_db_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-21 19:23:41.000000 airflow_db_logger-3.0.0/airflow_db_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:23:41.000000 airflow_db_logger-3.0.0/airflow_db_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 19:23:41.000000 airflow_db_logger-3.0.0/airflow_db_logger.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-04-21 19:23:41.413793 airflow_db_logger-3.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:42:56.870936 airflow_db_logger-3.0.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       18 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-17 14:42:56.870936 airflow_db_logger-3.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3317 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:42:56.870936 airflow_db_logger-3.0.1/airflow_db_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      700 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/airlfow_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4868 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2537 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/db.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4174 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2562 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/shell_logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2310 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/airflow_db_logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:42:56.870936 airflow_db_logger-3.0.1/airflow_db_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-17 14:42:56.000000 airflow_db_logger-3.0.1/airflow_db_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-17 14:42:56.000000 airflow_db_logger-3.0.1/airflow_db_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:42:56.000000 airflow_db_logger-3.0.1/airflow_db_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 14:42:56.000000 airflow_db_logger-3.0.1/airflow_db_logger.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-05-17 14:42:56.874937 airflow_db_logger-3.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-05-17 14:42:44.000000 airflow_db_logger-3.0.1/setup.py
```

### Comparing `airflow_db_logger-3.0.0/README.md` & `airflow_db_logger-3.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # AirflowDBLogger (python package)
 
 ##### Remember: If you like it \* it, so other people would also use it.
 
 An airflow logger that stores its results in a database given an SQLAlchemy connection.
 
 Supports:
-1. Airflow 1.10.x (for AirflowDBLogger <= 2.0.3)
-2. Airflow 2.5.3 (for AirflowDBLogger >= 2.0.5)
+1. Airflow <= 1.x.x (for AirflowDBLogger <= 2.0.3)
+2. Airflow >= 2.x.x (for AirflowDBLogger >= 3.0.0)
 3. Write and read logs to db.
 4. Logs cleanup operator
 
 
 ### Deprecation WARNING
 
 Versions before 2.0.5 do not support the current logger config and classes. Class structure has changed
@@ -43,15 +43,15 @@
 ```ini
 [core or logging(airflow 2)]
 logging_config_class = airflow_db_logger.LOGGING_CONFIG
 
 [db_logger]
 # Defaults loaded from airflow config
 
-log_level = INFO
+logging_level = INFO
 processor_log_level = 
 
 # Log flags
 show_reverse_order = false 
 show_log_splash = true
 
 # Write control
```

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/__init__.py` & `airflow_db_logger-3.0.1/airflow_db_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/airflow_utils.py` & `airflow_db_logger-3.0.1/airflow_db_logger/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/airlfow_config.py` & `airflow_db_logger-3.0.1/airflow_db_logger/airlfow_config.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/config.py` & `airflow_db_logger-3.0.1/airflow_db_logger/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 IS_RUNNING_DEBUG_EXECUTOR = AIRFLOW_EXECUTOR == "DebugExecutor"
 IS_USING_COLORED_CONSOLE = get(collection=__add_core("logging"), key="colored_console_log", default=False)
 
 # Loading sql parameters
 SQL_ALCHEMY_CONN = get(collection=__add_core("database"), key="sql_alchemy_conn", allow_empty=False)
 SQL_ALCHEMY_SCHEMA = get(collection=__add_core("database"), key="sql_alchemy_schema", allow_empty=True)
 
-DB_LOGGER_LOG_LEVEL = get(key="logging_level", default="INFO").upper()
+DB_LOGGER_LOG_LEVEL = get(key="logging_level", default=LOG_LEVEL).upper()
 DB_LOGGER_PROCESSOR_LOG_LEVEL = get("processor_log_level", default=LOG_LEVEL, allow_empty=True, otype=str)
 DB_LOGGER_SHOW_REVERSE_ORDER = get("show_reverse", False)
 DB_LOGGER_SHOW_LOG_SPLASH = get("show_log_splash", True)
 DB_LOGGER_LOG_SPLASH = get("log_splash", DB_LOGGER_DEFAULT_LOG_SPLASH)
 
 DB_LOGGER_SQL_ALCHEMY_SCHEMA = get("sql_alchemy_schema", SQL_ALCHEMY_SCHEMA)
 DB_LOGGER_SQL_ALCHEMY_CONNECTION = get("sql_alchemy_conn", SQL_ALCHEMY_CONN)
```

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/data.py` & `airflow_db_logger-3.0.1/airflow_db_logger/data.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/db.py` & `airflow_db_logger-3.0.1/airflow_db_logger/db.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/handlers.py` & `airflow_db_logger-3.0.1/airflow_db_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/log.py` & `airflow_db_logger-3.0.1/airflow_db_logger/log.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/logging_config.py` & `airflow_db_logger-3.0.1/airflow_db_logger/logging_config.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/operators.py` & `airflow_db_logger-3.0.1/airflow_db_logger/operators.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/shell_logging_config.py` & `airflow_db_logger-3.0.1/airflow_db_logger/shell_logging_config.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/storage.py` & `airflow_db_logger-3.0.1/airflow_db_logger/storage.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger/utils.py` & `airflow_db_logger-3.0.1/airflow_db_logger/utils.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/airflow_db_logger.egg-info/SOURCES.txt` & `airflow_db_logger-3.0.1/airflow_db_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-3.0.0/setup.py` & `airflow_db_logger-3.0.1/setup.py`

 * *Files identical despite different names*

