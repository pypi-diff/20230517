# Comparing `tmp/dynoscale-1.2.1.tar.gz` & `tmp/dynoscale-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynoscale-1.2.1.tar", last modified: Tue Mar 21 12:40:16 2023, max compression
+gzip compressed data, was "dynoscale-1.2.2.tar", last modified: Wed May 17 18:39:01 2023, max compression
```

## Comparing `dynoscale-1.2.1.tar` & `dynoscale-1.2.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-03-21 12:40:16.607243 dynoscale-1.2.1/
--rw-r--r--   0 fuho       (501) staff       (20)      666 2023-03-09 15:08:05.000000 dynoscale-1.2.1/CHANGELOG.md
--rw-r--r--   0 fuho       (501) staff       (20)     1059 2023-02-03 15:51:49.000000 dynoscale-1.2.1/LICENSE
--rw-r--r--   0 fuho       (501) staff       (20)    11504 2023-03-21 12:40:16.607443 dynoscale-1.2.1/PKG-INFO
--rw-r--r--   0 fuho       (501) staff       (20)     8761 2023-03-09 15:08:05.000000 dynoscale-1.2.1/README.md
--rw-r--r--   0 fuho       (501) staff       (20)      103 2023-02-03 15:51:49.000000 dynoscale-1.2.1/pyproject.toml
--rw-r--r--   0 fuho       (501) staff       (20)     2278 2023-03-21 12:40:16.608417 dynoscale-1.2.1/setup.cfg
--rw-r--r--   0 fuho       (501) staff       (20)       69 2023-02-03 15:51:49.000000 dynoscale-1.2.1/setup.py
-drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-03-21 12:40:16.587651 dynoscale-1.2.1/src/
-drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-03-21 12:40:16.596786 dynoscale-1.2.1/src/dynoscale/
--rw-r--r--   0 fuho       (501) staff       (20)       33 2023-02-06 17:47:45.000000 dynoscale-1.2.1/src/dynoscale/__init__.py
--rw-r--r--   0 fuho       (501) staff       (20)     2309 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/agent.py
--rw-r--r--   0 fuho       (501) staff       (20)     2873 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/asgi.py
--rw-r--r--   0 fuho       (501) staff       (20)     2273 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/config.py
--rw-r--r--   0 fuho       (501) staff       (20)      510 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/constants.py
-drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-03-21 12:40:16.600028 dynoscale-1.2.1/src/dynoscale/hooks/
--rw-r--r--   0 fuho       (501) staff       (20)        0 2023-02-03 15:51:49.000000 dynoscale-1.2.1/src/dynoscale/hooks/__init__.py
--rw-r--r--   0 fuho       (501) staff       (20)     2196 2023-02-03 15:51:49.000000 dynoscale-1.2.1/src/dynoscale/hooks/gunicorn.py
--rw-r--r--   0 fuho       (501) staff       (20)     4383 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/permadict.py
--rw-r--r--   0 fuho       (501) staff       (20)     7465 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/publisher.py
--rw-r--r--   0 fuho       (501) staff       (20)     3679 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/repository.py
--rw-r--r--   0 fuho       (501) staff       (20)     4543 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/utils.py
--rw-r--r--   0 fuho       (501) staff       (20)      883 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/uvicorn.py
--rw-r--r--   0 fuho       (501) staff       (20)     1545 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/version.py
-drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-03-21 12:40:16.601076 dynoscale-1.2.1/src/dynoscale/workers/
--rw-r--r--   0 fuho       (501) staff       (20)        0 2023-02-08 10:25:27.000000 dynoscale-1.2.1/src/dynoscale/workers/__init__.py
--rw-r--r--   0 fuho       (501) staff       (20)     3020 2023-03-21 12:36:25.000000 dynoscale-1.2.1/src/dynoscale/workers/rq_logger.py
--rw-r--r--   0 fuho       (501) staff       (20)     2439 2023-03-09 15:08:05.000000 dynoscale-1.2.1/src/dynoscale/wsgi.py
-drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-03-21 12:40:16.599068 dynoscale-1.2.1/src/dynoscale.egg-info/
--rw-r--r--   0 fuho       (501) staff       (20)    11504 2023-03-21 12:40:16.000000 dynoscale-1.2.1/src/dynoscale.egg-info/PKG-INFO
--rw-r--r--   0 fuho       (501) staff       (20)      901 2023-03-21 12:40:16.000000 dynoscale-1.2.1/src/dynoscale.egg-info/SOURCES.txt
--rw-r--r--   0 fuho       (501) staff       (20)        1 2023-03-21 12:40:16.000000 dynoscale-1.2.1/src/dynoscale.egg-info/dependency_links.txt
--rw-r--r--   0 fuho       (501) staff       (20)      286 2023-03-21 12:40:16.000000 dynoscale-1.2.1/src/dynoscale.egg-info/requires.txt
--rw-r--r--   0 fuho       (501) staff       (20)       10 2023-03-21 12:40:16.000000 dynoscale-1.2.1/src/dynoscale.egg-info/top_level.txt
-drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-03-21 12:40:16.606894 dynoscale-1.2.1/tests/
--rw-r--r--   0 fuho       (501) staff       (20)     7970 2023-03-09 15:08:05.000000 dynoscale-1.2.1/tests/test_agent.py
--rw-r--r--   0 fuho       (501) staff       (20)     6732 2023-03-21 12:15:45.000000 dynoscale-1.2.1/tests/test_asgi.py
--rw-r--r--   0 fuho       (501) staff       (20)     3800 2023-03-09 15:08:05.000000 dynoscale-1.2.1/tests/test_config.py
--rw-r--r--   0 fuho       (501) staff       (20)      447 2023-02-03 15:51:49.000000 dynoscale-1.2.1/tests/test_gunicorn_hooks.py
--rw-r--r--   0 fuho       (501) staff       (20)     1226 2023-03-09 15:08:05.000000 dynoscale-1.2.1/tests/test_hooks.py
--rw-r--r--   0 fuho       (501) staff       (20)     3636 2023-03-09 15:08:05.000000 dynoscale-1.2.1/tests/test_permadict.py
--rw-r--r--   0 fuho       (501) staff       (20)     6944 2023-03-09 15:08:05.000000 dynoscale-1.2.1/tests/test_publisher.py
--rw-r--r--   0 fuho       (501) staff       (20)     2007 2023-02-03 15:51:49.000000 dynoscale-1.2.1/tests/test_repository.py
--rw-r--r--   0 fuho       (501) staff       (20)     9075 2023-03-09 15:08:05.000000 dynoscale-1.2.1/tests/test_utils.py
--rw-r--r--   0 fuho       (501) staff       (20)     2386 2023-03-09 15:08:05.000000 dynoscale-1.2.1/tests/test_wsgi.py
+drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-05-17 18:39:01.378215 dynoscale-1.2.2/
+-rw-r--r--   0 fuho       (501) staff       (20)      870 2023-05-17 16:05:09.000000 dynoscale-1.2.2/CHANGELOG.md
+-rw-r--r--   0 fuho       (501) staff       (20)     1059 2023-05-07 01:47:44.000000 dynoscale-1.2.2/LICENSE
+-rw-r--r--   0 fuho       (501) staff       (20)    11708 2023-05-17 18:39:01.378332 dynoscale-1.2.2/PKG-INFO
+-rw-r--r--   0 fuho       (501) staff       (20)     8761 2023-05-07 01:47:44.000000 dynoscale-1.2.2/README.md
+-rw-r--r--   0 fuho       (501) staff       (20)      103 2023-05-07 01:47:44.000000 dynoscale-1.2.2/pyproject.toml
+-rw-r--r--   0 fuho       (501) staff       (20)     2278 2023-05-17 18:39:01.378634 dynoscale-1.2.2/setup.cfg
+-rw-r--r--   0 fuho       (501) staff       (20)       69 2023-05-07 01:47:44.000000 dynoscale-1.2.2/setup.py
+drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-05-17 18:39:01.372430 dynoscale-1.2.2/src/
+drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-05-17 18:39:01.375838 dynoscale-1.2.2/src/dynoscale/
+-rw-r--r--   0 fuho       (501) staff       (20)       33 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/__init__.py
+-rw-r--r--   0 fuho       (501) staff       (20)     2309 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/agent.py
+-rw-r--r--   0 fuho       (501) staff       (20)     2873 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/asgi.py
+-rw-r--r--   0 fuho       (501) staff       (20)     2432 2023-05-17 16:05:09.000000 dynoscale-1.2.2/src/dynoscale/config.py
+-rw-r--r--   0 fuho       (501) staff       (20)      728 2023-05-17 16:05:09.000000 dynoscale-1.2.2/src/dynoscale/constants.py
+drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-05-17 18:39:01.376629 dynoscale-1.2.2/src/dynoscale/hooks/
+-rw-r--r--   0 fuho       (501) staff       (20)        0 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/hooks/__init__.py
+-rw-r--r--   0 fuho       (501) staff       (20)     2196 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/hooks/gunicorn.py
+-rw-r--r--   0 fuho       (501) staff       (20)     4383 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/permadict.py
+-rw-r--r--   0 fuho       (501) staff       (20)     7465 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/publisher.py
+-rw-r--r--   0 fuho       (501) staff       (20)     3679 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/repository.py
+-rw-r--r--   0 fuho       (501) staff       (20)     4543 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/utils.py
+-rw-r--r--   0 fuho       (501) staff       (20)      883 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/uvicorn.py
+-rw-r--r--   0 fuho       (501) staff       (20)     1545 2023-05-17 09:41:37.000000 dynoscale-1.2.2/src/dynoscale/version.py
+drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-05-17 18:39:01.376839 dynoscale-1.2.2/src/dynoscale/workers/
+-rw-r--r--   0 fuho       (501) staff       (20)        0 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/workers/__init__.py
+-rw-r--r--   0 fuho       (501) staff       (20)     3415 2023-05-17 16:05:09.000000 dynoscale-1.2.2/src/dynoscale/workers/rq_logger.py
+-rw-r--r--   0 fuho       (501) staff       (20)     2439 2023-05-07 01:47:44.000000 dynoscale-1.2.2/src/dynoscale/wsgi.py
+drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-05-17 18:39:01.376434 dynoscale-1.2.2/src/dynoscale.egg-info/
+-rw-r--r--   0 fuho       (501) staff       (20)    11708 2023-05-17 18:39:01.000000 dynoscale-1.2.2/src/dynoscale.egg-info/PKG-INFO
+-rw-r--r--   0 fuho       (501) staff       (20)      901 2023-05-17 18:39:01.000000 dynoscale-1.2.2/src/dynoscale.egg-info/SOURCES.txt
+-rw-r--r--   0 fuho       (501) staff       (20)        1 2023-05-17 18:39:01.000000 dynoscale-1.2.2/src/dynoscale.egg-info/dependency_links.txt
+-rw-r--r--   0 fuho       (501) staff       (20)      286 2023-05-17 18:39:01.000000 dynoscale-1.2.2/src/dynoscale.egg-info/requires.txt
+-rw-r--r--   0 fuho       (501) staff       (20)       10 2023-05-17 18:39:01.000000 dynoscale-1.2.2/src/dynoscale.egg-info/top_level.txt
+drwxr-xr-x   0 fuho       (501) staff       (20)        0 2023-05-17 18:39:01.378088 dynoscale-1.2.2/tests/
+-rw-r--r--   0 fuho       (501) staff       (20)     7970 2023-05-07 01:47:44.000000 dynoscale-1.2.2/tests/test_agent.py
+-rw-r--r--   0 fuho       (501) staff       (20)     6732 2023-05-07 01:47:44.000000 dynoscale-1.2.2/tests/test_asgi.py
+-rw-r--r--   0 fuho       (501) staff       (20)     3800 2023-05-07 01:47:44.000000 dynoscale-1.2.2/tests/test_config.py
+-rw-r--r--   0 fuho       (501) staff       (20)      447 2023-05-07 01:47:44.000000 dynoscale-1.2.2/tests/test_gunicorn_hooks.py
+-rw-r--r--   0 fuho       (501) staff       (20)     1226 2023-05-07 01:47:44.000000 dynoscale-1.2.2/tests/test_hooks.py
+-rw-r--r--   0 fuho       (501) staff       (20)     3636 2023-05-07 01:47:44.000000 dynoscale-1.2.2/tests/test_permadict.py
+-rw-r--r--   0 fuho       (501) staff       (20)     6944 2023-05-07 01:47:44.000000 dynoscale-1.2.2/tests/test_publisher.py
+-rw-r--r--   0 fuho       (501) staff       (20)     2007 2023-05-07 01:47:44.000000 dynoscale-1.2.2/tests/test_repository.py
+-rw-r--r--   0 fuho       (501) staff       (20)     9075 2023-05-07 01:47:44.000000 dynoscale-1.2.2/tests/test_utils.py
+-rw-r--r--   0 fuho       (501) staff       (20)     2386 2023-05-07 01:47:44.000000 dynoscale-1.2.2/tests/test_wsgi.py
```

### Comparing `dynoscale-1.2.1/LICENSE` & `dynoscale-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/PKG-INFO` & `dynoscale-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynoscale
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple yet efficient scaling agent for Python apps on Heroku
 Home-page: https://dynoscale.net
 Author: Ondrej Dolejsi
 Author-email: ondrej.dolejsi@gmail.com
 License: MIT
 Project-URL: Documentation, http://dynoscale.net/documentation/category/general
 Project-URL: Source, https://github.com/Mjolnir-Software/dynoscale-python
@@ -290,18 +290,22 @@
 
 - `pip install -e ".[test]"`
 
 You can run _pytest_ from terminal: `pytest`
 
 You can run _flake8_ from terminal: `flake8 ./src`  
 
-# Change Log of `dynoscale` for Python
+# Changelog of `dynoscale` for Python
 
-### 1.2.1 [TBD]
- - ...
+### 1.2.2 [TBD]
+ - updated test/dev dependencies
+ - adding support for TLS redis urls with self-signed certificates
+
+### 1.2.1 [2023-03-01]
+ - Fix: Limit resource consumption while reporting on extreme numbers of pending tasks.
 
 ### 1.2.0 [2023-01-08]
  - dropping support for Python 3.7, 3.8, 3.9
  - adding support for Gunicorn with Uvicorn workers, use dynoscale.uvicorn.DynoscaleUnicornWorker
 
 ### 1.1.3 [2023-01-13]
```

### Comparing `dynoscale-1.2.1/README.md` & `dynoscale-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/setup.cfg` & `dynoscale-1.2.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -54,26 +54,26 @@
 	asgiref>=3.6.0
 	requests>=2.28.2
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
-test = pytest>=7.2.1
-	pytest-asyncio>=0.20.3
+test = pytest>=7.3.1
+	pytest-asyncio>=0.21.0
 	pytest-cov>=4.0.0
-	pylint>=2.16.1
-	flake8>=5.0.4
+	pylint>=2.17.4
+	flake8>=6.0.0
 	pytest-flake8>=1.1.1
-	responses>=0.22.0
-	redislite>=6.2.805324
-	rq>=1.12.0
-	Flask>=2.2.2
+	responses>=0.23.1
+	redislite>=6.2.859089
+	rq>=1.14.1
+	Flask>=2.3.2
 	colorlog>=6.7.0
-	starlette>=0.23.1
-	uvicorn[standard]>=0.20.0
+	starlette>=0.27.0
+	uvicorn[standard]>=0.22.0
 	gunicorn>=20.1.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dynoscale-1.2.1/src/dynoscale/agent.py` & `dynoscale-1.2.2/src/dynoscale/agent.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/src/dynoscale/asgi.py` & `dynoscale-1.2.2/src/dynoscale/asgi.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/src/dynoscale/config.py` & `dynoscale-1.2.2/src/dynoscale/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 from dynoscale.constants import *
 from dynoscale.repository import DEFAULT_DYNOSCALE_REPOSITORY_FILENAME
 from dynoscale.utils import is_valid_url, ensure_module
 
 
 def get_redis_urls_from_environ() -> Dict[str, str]:
     """Returns a dictionary of possible redis urls from all known redis_url environment variables"""
-    redis_env_vars = (ENV_REDIS_URL, ENV_REDISTOGO_URL, ENV_OPENREDIS_URL, ENV_REDISGREEN_URL, ENV_REDISCLOUD_URL)
+    redis_env_vars = (
+        ENV_REDIS_TLS_URL, ENV_REDIS_URL,
+        ENV_REDISTOGO_TLS_URL, ENV_REDISTOGO_URL,
+        ENV_OPENREDIS_TLS_URL, ENV_OPENREDIS_URL,
+        ENV_REDISGREEN_TLS_URL, ENV_REDISGREEN_URL,
+        ENV_REDISCLOUD_TLS_URL, ENV_REDISCLOUD_URL
+    )
     return {name: os.environ[name] for name in redis_env_vars if name in os.environ}
 
 
 class RunMode(Enum):
     PRODUCTION = 1
     DEVELOPMENT = 2
```

### Comparing `dynoscale-1.2.1/src/dynoscale/hooks/gunicorn.py` & `dynoscale-1.2.2/src/dynoscale/hooks/gunicorn.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/src/dynoscale/permadict.py` & `dynoscale-1.2.2/src/dynoscale/permadict.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/src/dynoscale/publisher.py` & `dynoscale-1.2.2/src/dynoscale/publisher.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/src/dynoscale/repository.py` & `dynoscale-1.2.2/src/dynoscale/repository.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/src/dynoscale/utils.py` & `dynoscale-1.2.2/src/dynoscale/utils.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/src/dynoscale/uvicorn.py` & `dynoscale-1.2.2/src/dynoscale/uvicorn.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/src/dynoscale/version.py` & `dynoscale-1.2.2/src/dynoscale/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  ██████╗ ██╗   ██╗███╗   ██╗ ██████╗ ███████╗ ██████╗ █████╗ ██╗     ███████╗ 
  ██╔══██╗╚██╗ ██╔╝████╗  ██║██╔═══██╗██╔════╝██╔════╝██╔══██╗██║     ██╔════╝ 
  ██║  ██║ ╚████╔╝ ██╔██╗ ██║██║   ██║███████╗██║     ███████║██║     █████╗   
  ██║  ██║  ╚██╔╝  ██║╚██╗██║██║   ██║╚════██║██║     ██╔══██║██║     ██╔══╝   
  ██████╔╝   ██║   ██║ ╚████║╚██████╔╝███████║╚██████╗██║  ██║███████╗███████╗ 
  ╚═════╝    ╚═╝   ╚═╝  ╚═══╝ ╚═════╝ ╚══════╝ ╚═════╝╚═╝  ╚═╝╚══════╝╚══════╝ 
 """
-__version__ = '1.2.1'
+__version__ = '1.2.2'
 
 __title__ = "dynoscale"
 __description__ = "Simple yet efficient scaling agent for Python apps on Heroku."
 __url__ = "https://pypi.org/project/dynoscale/"
 __author__ = "Ondrej Dolejsi"
 __author_email__ = "ondrej.dolejsi@gmail.com"
 __license__ = "MIT"
```

### Comparing `dynoscale-1.2.1/src/dynoscale/workers/rq_logger.py` & `dynoscale-1.2.2/src/dynoscale/workers/rq_logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import logging
 from contextlib import contextmanager
 from datetime import datetime
 from typing import Optional, Iterable, Generator
+from urllib.parse import urlparse, parse_qs, urlencode
 
 import redis
 from rq import Queue
 
 from dynoscale.config import Config, get_redis_urls_from_environ
 from dynoscale.repository import DynoscaleRepository, Record
 from dynoscale.utils import epoch_s
 
 logger = logging.getLogger(__name__)
 
 
+def allow_self_signed_certificates(url_str: str) -> str:
+    url = urlparse(url_str)
+    if not url.scheme == 'rediss':
+        return url_str
+
+    query_dict = parse_qs(url.query)
+    query_dict['ssl_cert_reqs'] = ['none']
+    return url._replace(query=urlencode(query_dict, doseq=True)).geturl()
+
+
 def get_enqueued_at_of_oldest_job(queue: Queue) -> Optional[datetime]:
     jobs = queue.get_jobs(offset=0, length=1)
     return jobs[0].enqueued_at if jobs else None
 
 
 def queue_time_records_for_connection(connection) -> Iterable[Record]:
     utc_now = datetime.utcnow()
@@ -25,18 +36,18 @@
         oldest_job_enqueued_at = get_enqueued_at_of_oldest_job(queue)
         if oldest_job_enqueued_at is not None:
             queue_time_ms = int((utc_now - oldest_job_enqueued_at).total_seconds() * 1_000)
             yield Record(timestamp=epoch_s(), metric=queue_time_ms, source=f"rq:{queue.name}", metadata="")
 
 
 @contextmanager
-def redis_connection(url: str) -> Generator[redis.Redis, None, None]:
+def redis_connection(url_str: str) -> Generator[redis.Redis, None, None]:
     conn = None
     try:
-        conn = redis.from_url(url)
+        conn = redis.from_url(allow_self_signed_certificates(url_str))
         yield conn
     finally:
         if conn:
             conn.close()
 
 
 def get_queue_time_records() -> Iterable[Record]:
```

### Comparing `dynoscale-1.2.1/src/dynoscale/wsgi.py` & `dynoscale-1.2.2/src/dynoscale/wsgi.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/src/dynoscale.egg-info/PKG-INFO` & `dynoscale-1.2.2/src/dynoscale.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynoscale
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple yet efficient scaling agent for Python apps on Heroku
 Home-page: https://dynoscale.net
 Author: Ondrej Dolejsi
 Author-email: ondrej.dolejsi@gmail.com
 License: MIT
 Project-URL: Documentation, http://dynoscale.net/documentation/category/general
 Project-URL: Source, https://github.com/Mjolnir-Software/dynoscale-python
@@ -290,18 +290,22 @@
 
 - `pip install -e ".[test]"`
 
 You can run _pytest_ from terminal: `pytest`
 
 You can run _flake8_ from terminal: `flake8 ./src`  
 
-# Change Log of `dynoscale` for Python
+# Changelog of `dynoscale` for Python
 
-### 1.2.1 [TBD]
- - ...
+### 1.2.2 [TBD]
+ - updated test/dev dependencies
+ - adding support for TLS redis urls with self-signed certificates
+
+### 1.2.1 [2023-03-01]
+ - Fix: Limit resource consumption while reporting on extreme numbers of pending tasks.
 
 ### 1.2.0 [2023-01-08]
  - dropping support for Python 3.7, 3.8, 3.9
  - adding support for Gunicorn with Uvicorn workers, use dynoscale.uvicorn.DynoscaleUnicornWorker
 
 ### 1.1.3 [2023-01-13]
```

### Comparing `dynoscale-1.2.1/src/dynoscale.egg-info/SOURCES.txt` & `dynoscale-1.2.2/src/dynoscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/tests/test_agent.py` & `dynoscale-1.2.2/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/tests/test_asgi.py` & `dynoscale-1.2.2/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/tests/test_config.py` & `dynoscale-1.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/tests/test_hooks.py` & `dynoscale-1.2.2/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/tests/test_permadict.py` & `dynoscale-1.2.2/tests/test_permadict.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/tests/test_publisher.py` & `dynoscale-1.2.2/tests/test_publisher.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/tests/test_repository.py` & `dynoscale-1.2.2/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/tests/test_utils.py` & `dynoscale-1.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dynoscale-1.2.1/tests/test_wsgi.py` & `dynoscale-1.2.2/tests/test_wsgi.py`

 * *Files identical despite different names*

