# Comparing `tmp/bmsdna_lakeapi-0.1.0.tar.gz` & `tmp/bmsdna_lakeapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.1.0.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.1.1.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.1.0.tar` & `bmsdna_lakeapi-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1081 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/LICENSE
--rw-r--r--   0        0        0     3688 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/README.md
--rw-r--r--   0        0        0      166 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1135 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     3601 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     6908 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     5670 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    12151 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12625 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15576 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6566 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     8044 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     3601 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     1692 2023-05-17 09:25:11.181012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2361 2023-05-17 09:25:11.185012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-17 09:25:11.185012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-17 09:25:11.185012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-17 09:25:11.185012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0     1784 2023-05-17 09:25:11.185012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-17 09:25:11.185012 bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     1783 2023-05-17 09:25:11.185012 bmsdna_lakeapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5002 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4722 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/README.md
+-rw-r--r--   0        0        0      166 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1135 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     3601 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     6908 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     5670 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    12190 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12625 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15576 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6566 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     8044 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     3601 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     1692 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2361 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     1804 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6036 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.1.1/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.1.0/LICENSE` & `bmsdna_lakeapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/README.md` & `bmsdna_lakeapi-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # The BMS Lake API
 
 A FastAPI Plugin that allows you to expose your Data Lake as an API, allowing multiple output formats, such as Parquet, Csv, Json, Excel, ...
 
-It also contains a minimal security layer for convenience (Basic Auth), but you can also bring your own.
+The lake API also contains a minimal security layer for convenience (Basic Auth), but you can also bring your own.
 
 It constrast to [roapi](https://github.com/roapi/roapi), we intentionally do not want to expose most SQL by default, but we limit possible queries using a config. This makes it easy for you to control what happens on your data. If you want the sql endpoint, you can enable this.
 
 To run the app with default config, just do:
+
 ```python
 app = FastAPI()
 bmsdna.lakeapi.init_lakeapi(app)
 ```
 
 To adjust the config, you can do like this:
 
@@ -19,23 +20,46 @@
 import bmsdna.lakeapi
 
 def_cfg = bmsdna.lakeapi.get_default_config() # Get default startup config
 cfg = dataclasses.replace(def_cfg, enable_sql_endpoint=True, data_path="tests/data") # Use dataclasses.replace to set the properties you want
 sti = bmsdna.lakeapi.init_lakeapi(app, cfg, "config_test.yml") # Enable it. The first parameter is the FastAPI instance, the 2nd one is the basic config and the third one the config of the tables
 ```
 
+## Installation 
+[![PyPI version](https://badge.fury.io/py/bmsdna-lakeapi.svg)](https://pypi.org/project/bmsdna-lakeapi/)
+
+Pypi Package `bmsdna-lakeapi` can be installed like any python package : `pip install bmsdna-lakeapi`
+
 ## OpenApi
 
 Of course, everything works with Open API and FastAPI. Meaning you can add other FastAPI routes, you can use the /docs and /redoc endpoint.
 
 ## Default Security
 
 By Default, Basic Authentication is enabled. To add a user, simply run `add_lakeapi_user YOURUSERNAME --yaml-file config.yml`. This will add the user to your config yaml (argon2 encrypted).
 The generated Password is printed. If you do not want this logic, you can overwrite the username_retriver of the Default Config
 
+## Standalone Mode
+
+If you just want to run this thing, you can run it with a webserver:
+
+Uvicorn: `uvicorn bmsdna.lakeapi.standalone:app --host 0.0.0.0 --port 8080`
+
+Gunicorn: `gunicorn bmsdna.lakeapi.standalone:app --workers 4 --worker-class uvicorn.workers.UvicornWorker --bind 0.0.0.0:80`
+
+Of course you need to adjust your http options as needed. Also, you need to `pip install` uvicorn/gunicorn
+
+You can still use environment variables for configuration
+
+## Environment Variables
+
+ - CONFIG_PATH: The path of the config file, defaults to `config.yml`. If you want to split the config, you can specify a folder, too
+ - DATA_PATH: The path of the data files, defaults to `data`. Paths in `config.yml` are relative to DATA_PATH
+ - ENABLE_SQL_ENDPOINT: Set this to 1 to enable the SQL Endpoint
+
 ## Config File
 
 The application by default relies on a Config file beeing present at the root of your project that's call `config.yml`.
 
 The config file looks something like this, see also [our test yaml](config_test.yml):
 
 ```yaml
```

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 def get_default_config():
     from bmsdna.lakeapi.core.uservalidation import get_username
 
     return BasicConfig(
         username_retriever=get_username,
-        enable_sql_endpoint=False,
+        enable_sql_endpoint=os.getenv("ENABLE_SQL_ENDPOINT", "0") == "1",
         temp_folder_path=os.getenv("TEMP", "/tmp"),
         data_path=os.environ.get("DATA_PATH", "data"),
         token_jwt_secret=os.getenv("JWT_SECRET", None),
     )
 
 
 @dataclass
```

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.0/pyproject.toml` & `bmsdna_lakeapi-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
@@ -32,14 +32,15 @@
 xlsxwriter = "^3.1.0"
 pyjwt = {version = "^2.6.0", optional = true}
 "ruamel.yaml" = {version = "^0.17.26", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.308"
 black = "^23.3.0"
+uvicorn = "^0.22.0"
 
 
 
 
 
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `bmsdna_lakeapi-0.1.0/PKG-INFO` & `bmsdna_lakeapi-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,19 +32,20 @@
 Requires-Dist: xlsxwriter (>=3.1.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # The BMS Lake API
 
 A FastAPI Plugin that allows you to expose your Data Lake as an API, allowing multiple output formats, such as Parquet, Csv, Json, Excel, ...
 
-It also contains a minimal security layer for convenience (Basic Auth), but you can also bring your own.
+The lake API also contains a minimal security layer for convenience (Basic Auth), but you can also bring your own.
 
 It constrast to [roapi](https://github.com/roapi/roapi), we intentionally do not want to expose most SQL by default, but we limit possible queries using a config. This makes it easy for you to control what happens on your data. If you want the sql endpoint, you can enable this.
 
 To run the app with default config, just do:
+
 ```python
 app = FastAPI()
 bmsdna.lakeapi.init_lakeapi(app)
 ```
 
 To adjust the config, you can do like this:
 
@@ -53,23 +54,46 @@
 import bmsdna.lakeapi
 
 def_cfg = bmsdna.lakeapi.get_default_config() # Get default startup config
 cfg = dataclasses.replace(def_cfg, enable_sql_endpoint=True, data_path="tests/data") # Use dataclasses.replace to set the properties you want
 sti = bmsdna.lakeapi.init_lakeapi(app, cfg, "config_test.yml") # Enable it. The first parameter is the FastAPI instance, the 2nd one is the basic config and the third one the config of the tables
 ```
 
+## Installation 
+[![PyPI version](https://badge.fury.io/py/bmsdna-lakeapi.svg)](https://pypi.org/project/bmsdna-lakeapi/)
+
+Pypi Package `bmsdna-lakeapi` can be installed like any python package : `pip install bmsdna-lakeapi`
+
 ## OpenApi
 
 Of course, everything works with Open API and FastAPI. Meaning you can add other FastAPI routes, you can use the /docs and /redoc endpoint.
 
 ## Default Security
 
 By Default, Basic Authentication is enabled. To add a user, simply run `add_lakeapi_user YOURUSERNAME --yaml-file config.yml`. This will add the user to your config yaml (argon2 encrypted).
 The generated Password is printed. If you do not want this logic, you can overwrite the username_retriver of the Default Config
 
+## Standalone Mode
+
+If you just want to run this thing, you can run it with a webserver:
+
+Uvicorn: `uvicorn bmsdna.lakeapi.standalone:app --host 0.0.0.0 --port 8080`
+
+Gunicorn: `gunicorn bmsdna.lakeapi.standalone:app --workers 4 --worker-class uvicorn.workers.UvicornWorker --bind 0.0.0.0:80`
+
+Of course you need to adjust your http options as needed. Also, you need to `pip install` uvicorn/gunicorn
+
+You can still use environment variables for configuration
+
+## Environment Variables
+
+ - CONFIG_PATH: The path of the config file, defaults to `config.yml`. If you want to split the config, you can specify a folder, too
+ - DATA_PATH: The path of the data files, defaults to `data`. Paths in `config.yml` are relative to DATA_PATH
+ - ENABLE_SQL_ENDPOINT: Set this to 1 to enable the SQL Endpoint
+
 ## Config File
 
 The application by default relies on a Config file beeing present at the root of your project that's call `config.yml`.
 
 The config file looks something like this, see also [our test yaml](config_test.yml):
 
 ```yaml
```

