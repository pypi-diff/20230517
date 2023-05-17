# Comparing `tmp/latch_config-0.1.5.tar.gz` & `tmp/latch_config-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_config-0.1.5.tar", max compression
+gzip compressed data, was "latch_config-0.1.6.tar", max compression
```

## Comparing `latch_config-0.1.5.tar` & `latch_config-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_config-0.1.5/LICENSE
--rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_config-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-10 15:25:16.083190 latch_config-0.1.5/latch_config/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-09 17:07:12.285092 latch_config-0.1.5/latch_config/config.py
--rw-r--r--   0        0        0        0 2023-05-09 16:28:54.229755 latch_config-0.1.5/latch_config/py.typed
--rw-r--r--   0        0        0     1086 2023-05-10 15:26:47.132443 latch_config-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 latch_config-0.1.5/setup.py
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 latch_config-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_config-0.1.6/LICENSE
+-rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_config-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 15:25:16.083190 latch_config-0.1.6/latch_config/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-17 00:12:15.069833 latch_config-0.1.6/latch_config/config.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:28:54.229755 latch_config-0.1.6/latch_config/py.typed
+-rw-r--r--   0        0        0     1086 2023-05-17 00:12:32.078809 latch_config-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 latch_config-0.1.6/setup.py
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 latch_config-0.1.6/PKG-INFO
```

### Comparing `latch_config-0.1.5/LICENSE` & `latch_config-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_config-0.1.5/latch_config/config.py` & `latch_config-0.1.6/latch_config/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 @dataclass(frozen=True)
 class DatabaseTxRetriesConfig:
     delay_quant: float = 0.05
     max_wait_time: float = 30
 
 
 @dataclass(frozen=True)
-class DatabaseConfig:
+class PostgresConnectionConfig:
     host: str
     password: str
 
     conn_retries: DatabaseConnRetriesConfig
     tx_retries: DatabaseTxRetriesConfig
 
     port: str = "5432"
@@ -32,32 +32,23 @@
     pool_size: int = 20
 
 
 @dataclass(frozen=True)
 class DatadogConfig:
     service_version: str = field(metadata=dict(env_name_override="DD_VERSION"))
     deployment_environment: str = field(metadata=dict(env_name_override="DD_ENV"))
-    service_name: str = field(
-        default="nucleus_data", metadata=dict(env_name_override="DD_SERVICE")
-    )
+    service_name: str = field(metadata=dict(env_name_override="DD_SERVICE"))
 
 
 class LoggingMode(str, Enum):
     console = "console"
     console_json = "console_json"
     file_json = "file_json"
 
 
-@dataclass(frozen=True)
-class Config:
-    database: DatabaseConfig
-    datadog: DatadogConfig
-    logging_mode: LoggingMode = LoggingMode.console_json
-
-
 T = TypeVar("T")
 
 
 def read_config(x: type[T], env_prefix: str = "") -> T:
     res = {}
     for f in fields(x):
         val = None
```

### Comparing `latch_config-0.1.5/pyproject.toml` & `latch_config-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-config"
-version = "0.1.5"
+version = "0.1.6"
 description = "Shared config for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_config"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_config-0.1.5/setup.py` & `latch_config-0.1.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['latch_config']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'latch-config',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Shared config for latch python backend services',
     'long_description': '# python-config\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

