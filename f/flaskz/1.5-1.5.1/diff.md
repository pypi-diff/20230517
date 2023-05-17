# Comparing `tmp/flaskz-1.5.tar.gz` & `tmp/flaskz-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.5.tar", last modified: Sun Apr 30 16:26:54 2023, max compression
+gzip compressed data, was "flaskz-1.5.1.tar", last modified: Wed May 17 02:10:09 2023, max compression
```

## Comparing `flaskz-1.5.tar` & `flaskz-1.5.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.371591 flaskz-1.5/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.5/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)     6014 2023-04-30 16:26:54.371934 flaskz-1.5/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     5573 2023-04-30 02:34:26.000000 flaskz-1.5/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.5/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      702 2023-04-30 16:26:54.373355 flaskz-1.5/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.317386 flaskz-1.5/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.322595 flaskz-1.5/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       21 2023-04-25 08:17:23.000000 flaskz-1.5/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.329130 flaskz-1.5/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.5/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.5/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.334334 flaskz-1.5/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.5/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.5/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)     9693 2023-04-26 10:31:33.000000 flaskz-1.5/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.335590 flaskz-1.5/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2148 2023-04-29 08:02:14.000000 flaskz-1.5/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.341339 flaskz-1.5/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     5452 2023-04-29 08:02:14.000000 flaskz-1.5/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    26141 2023-04-27 03:54:02.000000 flaskz-1.5/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     8353 2023-04-26 10:19:02.000000 flaskz-1.5/src/flaskz/models/_model.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     5969 2023-04-30 02:33:59.000000 flaskz-1.5/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.5/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.346233 flaskz-1.5/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    19354 2023-04-27 11:45:35.000000 flaskz-1.5/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.5/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     3816 2023-04-27 11:38:34.000000 flaskz-1.5/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.369687 flaskz-1.5/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      253 2022-11-07 02:04:34.000000 flaskz-1.5/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2099 2023-04-30 03:06:59.000000 flaskz-1.5/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2571 2023-04-26 10:28:36.000000 flaskz-1.5/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.5/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    10388 2023-04-26 10:28:36.000000 flaskz-1.5/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.5/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.5/src/flaskz/utils/_magic.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     5002 2023-04-26 10:29:46.000000 flaskz-1.5/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7682 2023-04-27 03:34:22.000000 flaskz-1.5/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2578 2023-04-26 10:29:46.000000 flaskz-1.5/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     2784 2023-04-24 11:30:26.000000 flaskz-1.5/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.326104 flaskz-1.5/src/flaskz.egg-info/
--rwxrwxrwx   0 taozh      (501) staff       (20)     6014 2023-04-30 16:26:54.000000 flaskz-1.5/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      919 2023-04-30 16:26:54.000000 flaskz-1.5/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-04-30 16:26:54.000000 flaskz-1.5/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-04-30 16:26:54.000000 flaskz-1.5/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-04-30 16:26:54.000000 flaskz-1.5/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 02:10:09.291438 flaskz-1.5.1/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.5.1/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)     6223 2023-05-17 02:10:09.291691 flaskz-1.5.1/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5783 2023-05-17 02:04:13.000000 flaskz-1.5.1/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.5.1/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      704 2023-05-17 02:10:09.292873 flaskz-1.5.1/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 02:10:09.257556 flaskz-1.5.1/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 02:10:09.262179 flaskz-1.5.1/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       23 2023-05-15 02:54:24.000000 flaskz-1.5.1/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 02:10:09.267078 flaskz-1.5.1/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.5.1/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.5.1/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 02:10:09.270043 flaskz-1.5.1/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.5.1/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.5.1/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)     9693 2023-04-26 10:31:33.000000 flaskz-1.5.1/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 02:10:09.271074 flaskz-1.5.1/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2256 2023-05-15 03:14:20.000000 flaskz-1.5.1/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 02:10:09.275052 flaskz-1.5.1/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5488 2023-05-17 02:06:29.000000 flaskz-1.5.1/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    26588 2023-05-17 01:59:00.000000 flaskz-1.5.1/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     8353 2023-04-26 10:19:02.000000 flaskz-1.5.1/src/flaskz/models/_model.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6450 2023-05-15 09:29:19.000000 flaskz-1.5.1/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.5.1/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 02:10:09.278302 flaskz-1.5.1/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    19354 2023-04-27 11:45:35.000000 flaskz-1.5.1/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.5.1/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     3931 2023-05-16 02:55:12.000000 flaskz-1.5.1/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 02:10:09.290263 flaskz-1.5.1/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-05-10 07:01:15.000000 flaskz-1.5.1/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.5.1/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.5.1/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.5.1/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.5.1/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.5.1/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.5.1/src/flaskz/utils/_magic.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6078 2023-05-10 09:11:49.000000 flaskz-1.5.1/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7742 2023-05-16 02:51:46.000000 flaskz-1.5.1/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.5.1/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     2784 2023-04-24 11:30:26.000000 flaskz-1.5.1/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 02:10:09.265450 flaskz-1.5.1/src/flaskz.egg-info/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6223 2023-05-17 02:10:09.000000 flaskz-1.5.1/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      919 2023-05-17 02:10:09.000000 flaskz-1.5.1/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-05-17 02:10:09.000000 flaskz-1.5.1/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-05-17 02:10:09.000000 flaskz-1.5.1/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-05-17 02:10:09.000000 flaskz-1.5.1/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.5/LICENSE` & `flaskz-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/PKG-INFO` & `flaskz-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.5
+Version: 1.5.1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,17 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.5.1** `2023/05/17`
+    - [C] `db_session`上下文管理器自动关闭非缓存session
+    - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
     - [A] 重构`flaskz.rest`路由生成模块*
         - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
         - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
         - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
         - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
         - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
```

### Comparing `flaskz-1.5/README.md` & `flaskz-1.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.5.1** `2023/05/17`
+    - [C] `db_session`上下文管理器自动关闭非缓存session
+    - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
     - [A] 重构`flaskz.rest`路由生成模块*
         - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
         - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
         - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
         - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
         - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
```

### Comparing `flaskz-1.5/setup.cfg` & `flaskz-1.5.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flaskz
-version = 1.5
+version = 1.5.1
 author = Zhang Tao
 author_email = taozh1982@gmail.com
 description = Flask and SQLAlchemy extensions for web applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taozh1982/flaskz
 project_urls =
```

### Comparing `flaskz-1.5/src/flaskz/auth/_jws.py` & `flaskz-1.5.1/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz/ext/cypher.py` & `flaskz-1.5.1/src/flaskz/ext/cypher.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz/ext/ssh.py` & `flaskz-1.5.1/src/flaskz/ext/ssh.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz/log/__init__.py` & `flaskz-1.5.1/src/flaskz/log/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import datetime
 import json
 import logging
 import os
 from logging.handlers import TimedRotatingFileHandler
+from typing import Union
 
-from flask import Flask
 from werkzeug.local import LocalProxy
 
 _flaskz_logger: logging.Logger = None  # @2022-04-27: fix _get_app_logger --> NameError: name '_flaskz_logger' is not defined
-flaskz_logger = LocalProxy(lambda: _get_app_logger())
+flaskz_logger: Union[LocalProxy, logging.Logger] = LocalProxy(lambda: _get_app_logger())  # @2023-05-15: add type Union
 
 
 def init_log(app):
     """
     Initialize system log configuration
+
+    Example:
+        init_log(app)
+
     :param app:
     :return:
     """
     app_config = get_app_config_items(app) or {}
     level = logging.getLevelName(app_config.get('FLASKZ_LOGGER_LEVEL'))
     formatter = logging.Formatter(app_config.get('FLASKZ_LOGGER_FORMAT'))
     global _flaskz_logger
```

### Comparing `flaskz-1.5/src/flaskz/models/__init__.py` & `flaskz-1.5.1/src/flaskz/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 from sqlalchemy import create_engine, event
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine import ExceptionContext
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
 from ..log import flaskz_logger
-from ..utils import Attribute, cls_to_dict
+from ..utils import Attribute
 
 DBSession = sessionmaker(autocommit=False)
 
 ModelBase = declarative_base()
 
 
 def init_model(app):
     """
     Initialize the database.
+
+    Example:
+        init_model(flask_app)
+
     """
     is_app = isinstance(app, Flask)
     app_config = get_app_config_items(app) or {}
     database_uri = app_config.get('FLASKZ_DATABASE_URI')
 
     # enable sqlite foreign key
     # if database_uri.startswith('sqlite'):
```

### Comparing `flaskz-1.5/src/flaskz/models/_base.py` & `flaskz-1.5.1/src/flaskz/models/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import text
+from sqlalchemy import text, Integer, Numeric
 
 from .. import res_status_codes
 from ..utils import find_list, filter_list, is_str, is_dict, is_list, ins_to_dict, get_dict_value_by_type
 
 __all__ = ['BaseModelMixin']
 
 
@@ -218,15 +218,15 @@
         if cascade > 0:
             for relationship in cls.get_relationships():
                 lazy = relationship.lazy
                 if lazy != 'dynamic' and lazy != 'noload':
                     fields.append(relationship.key)
         items = {}
         for field in fields:
-            items[field] = getattr(ins, field)
+            items[field] = getattr(ins, field, None)
         return items
 
     @classmethod
     def to_dict_field_filter(cls, field):
         """
         to_dict field filter callback.
         If return false, the field will not be returned.
@@ -251,20 +251,26 @@
                 auto_fields.append(col)
             else:
                 auto_fields.append(cls.get_column_field(col))
 
         for col in cls.get_columns():
             field = cls.get_column_field(col)  # col.key
             if (field in data) and (field not in auto_fields) and (not col.info.get('auto', False)):
+                col_type = col.type
                 value = data.get(field)
+                is_blank_str = is_str(value) and value.strip() == ""
                 if col.nullable is False:
-                    if not (value is None or (is_str(value) and value.strip() == "")):
+                    if not (value is None or is_blank_str):
                         attrs[field] = value
                 else:
-                    attrs[field] = value
+                    # @2023-05-16 add to fix DataError: (1366, "Incorrect integer value: '' for column")
+                    if is_blank_str and (isinstance(col_type, Integer) or isinstance(col_type, Numeric)):
+                        attrs[field] = None
+                    else:
+                        attrs[field] = value
 
         return attrs
 
     @classmethod
     def get_columns_json(cls, data):
         """
         Get the attributes(dict) corresponding to the column from the specified data(dict).
@@ -401,16 +407,16 @@
         else:
             with db_session() as session:
                 session.bulk_update_mappings(cls, items)
 
     @classmethod
     def _update_ins(cls, instance, data):
         if instance:
-            for field in cls.filter_attrs_by_columns(data):  # Only the fields in json will be updated
-                setattr(instance, field, data.get(field))
+            for field, value in cls.filter_attrs_by_columns(data).items():  # Only the fields in json will be updated
+                setattr(instance, field, value)  # @2023-05-11, data.get(field)-->ins_attrs.get(field)
             relationships = create_relationships(cls, data)
             for field in relationships:
                 setattr(instance, field, relationships[field])
         return instance
 
     # -------------------------------------------delete-------------------------------------------
     @classmethod
@@ -657,37 +663,38 @@
         """
         filter_likes = pss_option.get('filter_likes', [])
         filter_ands = pss_option.get('filter_ands', [])
         filter_ors = pss_option.get('filter_ors', [])
         offset = max(get_dict_value_by_type(pss_option, 'offset', int, 0), 0)  # @2023-01-09 update, add type check
         limit = max(get_dict_value_by_type(pss_option, 'limit', int, 0), 0)
 
-        # pss_json.get('order') or cls.get_query_default_order()
-        # bool(pss_json.get('order')) --> Boolean value of this clause is not defined
         orders = pss_option.get('order')
         if orders is None:
-            orders = [cls.get_query_default_order()]  # default order
+            orders = []
         elif not is_list(orders):  # asc/desc
             orders = [orders]
 
-        if not is_list(orders):
-            orders = []
+        if len(orders) == 0:  # @2023-05-04 fix
+            default_order = cls.get_query_default_order()
+            if default_order:
+                orders = [default_order]  # default order
 
         with db_session(do_commit=False) as session:
             query = session.query(cls)
             if len(filter_likes) > 0:
                 query = query.filter(text('(' + (' OR '.join(filter_likes)) + ')'))
             if len(filter_ands) > 0:
                 query = query.filter(text('(' + (' AND '.join(filter_ands)) + ')'))
             if len(filter_ors) > 0:
                 query = query.filter(text('(' + (' OR '.join(filter_ors)) + ')'))
             count = query.count()
             if count > 0 and offset < count:
                 for order in orders:
-                    query = query.order_by(order)
+                    if order is not None:
+                        query = query.order_by(order)
                 query = query.offset(offset)
                 if limit > 0:
                     query = query.limit(limit)
                 items = query.all()
             else:
                 items = []
         return {
@@ -740,15 +747,15 @@
         return res_status_codes.db_data_already_exist  # used to return to the client
 
     def __repr__(self):
         cls = self.__class__
         attrs = []
         for col in cls.get_columns():
             field = cls.get_column_field(col)
-            attrs.append(field + '=' + str(getattr(self, field)))
+            attrs.append(field + '=' + str(getattr(self, field, None)))
         return cls.get_class_name() + '(' + (', '.join(attrs)) + ')'
 
     # -------------------------------------------new-------------------------------------------
 
 
 # must
 from ._util import create_instance, create_relationships, db_session
```

### Comparing `flaskz-1.5/src/flaskz/models/_model.py` & `flaskz-1.5.1/src/flaskz/models/_model.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz/models/_util.py` & `flaskz-1.5.1/src/flaskz/models/_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             relationship_map[key] = relationship
 
     return relationship_map
 
 
 def query_all_models(*models):
     """
-    Query all the data of the specified model list.
+    Query all the data of the specified model(ModelMixin) list.
 
     .. versionadded:: 1.5
 
     Example:
         result = query_all_models(User, Role)
 
     :param models:
@@ -92,15 +92,15 @@
         else:
             result.append(r)
     return result
 
 
 def query_multiple_model(*cls_list):
     """
-    Query all the data of the multiple specified model class.
+    Query all the data of the multiple specified model(ModelMixin) class.
 
     Example:
         result = query_multiple_model(User, Role)
 
     :param cls_list:
     :return:If failed, returns the failed tuple, otherwise, returns the the data list.
     """
@@ -118,32 +118,31 @@
 
 def get_debug_queries():
     if _has_g_context():  # @2022-07-26 add,
         return getattr(g, 'z_debug_queries', [])
     return []
 
 
-def _has_g_context():
-    if not g:  # @2022-11-28: change, (not g) != (g is None)
-        return False
-    return True
-    # return has_request_context() or g is not None
-
-
 def get_db_session():
     """
-    Get the db session from g(flask)/ Create a db session.
+    Get the db session from g(flask)/ Create a db session(without request).
     If not exist, create a session and return.
 
+    Example:
+        session = get_db_session()
+        session.query(User).all()
+        session.close()             # close session
+
     :return:
     """
     if _has_g_context():  # @2022-07-26 add, make sure work without flask request
         session = get_g_cache('_flaskz_db_session')
         if session is None:
             session = DBSession()
+            setattr(session, '_flaskz_db_session', True)
             set_g_cache('_flaskz_db_session', session)
     else:
         session = DBSession()
     return session
 
 
 def close_db_session():
@@ -160,30 +159,32 @@
 
 @contextmanager
 def db_session(do_commit=True):
     """
     Database session context manager.
 
     Example:
-        instance = create_instance(cls, json_data)
         with db_session() as session:
+            instance = create_instance(cls, json_data)
             session.add(instance)
 
     :param do_commit: If false, session will not commit,generally used for query operations
     :return:
     """
     session = get_db_session()
     try:
         yield session
         if do_commit is not False:
             session.commit()
     except Exception as e:
         if do_commit is not False:
             session.rollback()
         raise e
+    if getattr(session, '_flaskz_db_session', None) is not True:  # @2023-05-06: add, close non-cached session
+        session.close()
 
 
 def model_to_dict(ins, option=None):
     """
     Convert model data to dict.
 
     Example:
@@ -212,7 +213,16 @@
     """
     Check if the object is an instance of the BaseModelMixin.
 
     :param obj:
     :return:
     """
     return isinstance(obj, BaseModelMixin)
+
+
+def _has_g_context():
+    # if has_request_context():  # If there is request context, g must exist
+    #     return True
+    if not g:  # @2022-11-28: change, (not g) != (g is None)
+        return False
+    return True
+    # return has_request_context() or g is not None
```

### Comparing `flaskz-1.5/src/flaskz/res_status_codes.py` & `flaskz-1.5.1/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz/rest/__init__.py` & `flaskz-1.5.1/src/flaskz/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz/rest/_mgmt.py` & `flaskz-1.5.1/src/flaskz/rest/_mgmt.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz/rest/_util.py` & `flaskz-1.5.1/src/flaskz/rest/_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,27 +8,29 @@
            'rest_login_required', 'rest_permission_required',
            'get_rest_log_msg',
            'log_operation',
            'gen_route_method']
 
 
 def get_current_model_rest_manager_callback(callback_name):
-    model_rest_manager = getattr(current_app, 'model_rest_manager', None)
-    if model_rest_manager:
-        return getattr(model_rest_manager, callback_name)
+    if current_app:
+        model_rest_manager = getattr(current_app, 'model_rest_manager', None)
+        if model_rest_manager:
+            return getattr(model_rest_manager, callback_name, None)
 
 
 def rest_login_required():
     """
     If you decorate a view with this, it will ensure that the current user is logged in and authenticated before calling the actual view.
 
-    @sys_mgmt_bp.route('/auth/account/', methods=['GET', 'POST'])
-    @rest_login_required()
-    def sys_auth_account_query():
-        pass
+    Example:
+        @sys_mgmt_bp.route('/auth/account/', methods=['GET', 'POST'])
+        @rest_login_required()
+        def sys_auth_account_query():
+            pass
 
     :return:
     """
 
     def decorate(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
@@ -46,23 +48,24 @@
 
 
 def rest_permission_required(module, op_permission=None):
     """
     If you decorate a view with this, it will ensure that the current user.
     has the module permission and operation permission before calling the actual view.
 
-    @sys_mgmt_bp.route('/role/', methods=['GET'])
-    @rest_permission_required('role')
-    def sys_role_query():
-        pass
-
-    @sys_mgmt_bp.route('/role/', methods=['POST'])
-    @rest_permission_required('role', 'add')
-    def sys_role_add():
-        pass
+    Example:
+        @sys_mgmt_bp.route('/role/', methods=['GET'])
+        @rest_permission_required('role')
+        def sys_role_query():
+            pass
+
+        @sys_mgmt_bp.route('/role/', methods=['POST'])
+        @rest_permission_required('role', 'add')
+        def sys_role_add():
+            pass
 
     :param module:
     :param op_permission:
     :return:
     """
 
     def decorate(func):
```

### Comparing `flaskz-1.5/src/flaskz/utils/_app.py` & `flaskz-1.5.1/src/flaskz/utils/_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 app_config = None
 
 
 def init_app_config(app):
     """
     Initialize application configuration.
+    Once initialized, the application configuration can be get through get_app_config function anywhere.
+
+    .. versionadded:: 1.5
 
     Example:
         init_app_config(app)    # Flask
         init_app_config(DevelopmentConfig)  # Class
         init_app_config({...})  # dict
 
-    .. versionadded:: 1.5
 
     :param app:Flask/Config/dict
     :return:
     """
     config = get_app_config_items(app)
     if type(config) is dict:
         global app_config
@@ -31,14 +33,18 @@
     """
     Get the specified config value of the application.
     If the config is initialized by init_app_config, return the initialized config, otherwise return the config of the current application.
     If key is None return all config values(dict), otherwise return the specified config value
 
     .. versionupdated:: 1.5
 
+    Example:
+        get_app_config()                        # all Config
+        get_app_config('FLASKZ_LOGGER_LEVEL')   # specified config value
+
     :param key:
     :return:
     """
     config = None
     if app_config:
         config = app_config
     elif current_app:
```

### Comparing `flaskz-1.5/src/flaskz/utils/_cache.py` & `flaskz-1.5.1/src/flaskz/utils/_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,89 +25,95 @@
         set_app_cache('sys_module_name_mapping', module_name_mapping)
 
     :param expire_minutes:
     :param key:
     :param data:
     :return:
     """
-    cache = getattr(current_app, 'z_data_cache', None)
-    if cache is None:
-        cache = current_app.z_data_cache = {}
-    cache[key] = _generate_cache_expire_data(data, expire_minutes)
+    if current_app:
+        cache = getattr(current_app, 'z_data_cache', None)
+        if cache is None:
+            cache = current_app.z_data_cache = {}
+        cache[key] = _generate_cache_expire_data(data, expire_minutes)
 
 
 def get_app_cache(key):
     """
     Get the current application data cache by the key.
 
     Example:
         module_name_mapping = get_app_cache('sys_module_name_mapping')
 
     :param key:
     :return:
     """
-    cache = getattr(current_app, 'z_data_cache', None)
-    if cache:
-        data = cache.get(key)
-        if is_dict(data) and '_zexpires_time' in data:
-            if data.get('_zexpires_time') < time.time():
-                return None
-            return data.get('data')
-        return data
+    if current_app:
+        cache = getattr(current_app, 'z_data_cache', None)
+        if cache:
+            data = cache.get(key)
+            if is_dict(data) and '_zexpires_time' in data:
+                if data.get('_zexpires_time') < time.time():
+                    return None
+                return data.get('data')
+            return data
 
     return None
 
 
 def clear_app_cache():
     """
     Clear all the current application data caches.
 
     :return:
     """
-    cache = getattr(current_app, 'z_data_cache', None)
-    if cache:
-        cache.clear()
+    if current_app:
+        cache = getattr(current_app, 'z_data_cache', None)
+        if cache:
+            cache.clear()
 
 
 def set_g_cache(key, data):
     """
     Set the data cache in g, such as db session.
 
     Example:
         set_g_cache('_flaskz_db_session', session)
 
     :param key:
     :param data:
     :return:
     """
-    cache = getattr(g, 'z_data_cache', None)
-    if cache is None:
-        cache = g.z_data_cache = {}
-    cache[key] = data
+    if g:
+        cache = getattr(g, 'z_data_cache', None)
+        if cache is None:
+            cache = g.z_data_cache = {}
+        cache[key] = data
 
 
 def get_g_cache(key):
     """
     Get the g data cache by the key.
 
     Example:
         session = get_g_cache('_flaskz_db_session')
 
     :param key:
     :return:
     """
-    cache = getattr(g, 'z_data_cache', None)
-    if cache:
-        return cache.get(key)
-    return None
+    if g:
+        cache = getattr(g, 'z_data_cache', None)
+        if cache:
+            return cache.get(key)
+        return None
 
 
 def remove_g_cache(key):
     """
     Remove the g data cache.
 
     :param key:
     :return:
     """
-    cache = getattr(g, 'z_data_cache', None)
-    if cache:
-        del cache[key]
+    if g:
+        cache = getattr(g, 'z_data_cache', None)
+        if cache:
+            del cache[key]
```

### Comparing `flaskz-1.5/src/flaskz/utils/_cls.py` & `flaskz-1.5.1/src/flaskz/utils/_cls.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz/utils/_common.py` & `flaskz-1.5.1/src/flaskz/utils/_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         for item in ins_list:
             k_value = item
             for k in keys:
                 k_value = getattr(k_value, k)
             map_dict[k_value] = item
     else:
         for item in ins_list:
-            map_dict[getattr(item, attr)] = item
+            map_dict[getattr(item, attr, None)] = item
 
     return map_dict
 
 
 def get_dict_mapping(dict_list, key='id', key_join="+"):
     """
     Create a dict map of the specified dict list withe the specified key
```

### Comparing `flaskz-1.5/src/flaskz/utils/_func.py` & `flaskz-1.5.1/src/flaskz/utils/_func.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz/utils/_magic.py` & `flaskz-1.5.1/src/flaskz/utils/_magic.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz/utils/_request_api.py` & `flaskz-1.5.1/src/flaskz/utils/_request_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Not included by default.
 If use it, please install the 'requests' package first
 """
 import inspect
 import textwrap
-import urllib
+from urllib import parse as urllib_parse
 
 import requests
 from flask import request
 from requests import Session
 
 from ._common import is_dict
 from .. import res_status_codes
@@ -54,18 +54,20 @@
         _url = url.get('url')
         if 'method' in url:
             _method = url.get("method")
     else:
         _url = url
 
     if base_url:
-        _url = base_url + _url
+        base_url = base_url.rstrip('/')
+        _url = _url.lstrip('/')
+        _url = base_url + '/' + _url
 
     if is_dict(url_params):
-        _url = _url.format(**url_params)
+        _url = append_url_search_params(_url, url_params)
 
     _method = _method.strip().upper()
 
     flaskz_logger.debug('Api request:\n   url={url}\n   method={method}\n   data={data}\n   json={json}'.format(**{
         'url': _url,
         'method': _method,
         'data': kwargs.get('data'),
@@ -113,15 +115,15 @@
     """
     req_kwargs = {'url': url}
     _payload = payload or ['method', 'data', 'json', 'headers', 'cookies']
     for item in _payload:
         if item == 'json':  # @2022-05-06: fix request.json -->BadRequest('Content-Type was not 'application/json')
             req_kwargs[item] = request.get_json(force=True, silent=True)
         else:
-            req_kwargs[item] = getattr(request, item)
+            req_kwargs[item] = getattr(request, item, None)
     req_kwargs.update(kwargs)  # kwargs high priority
 
     url_params = req_kwargs.get('url_params')
     if url_params is None:  # if url_params is none, append request.view_args
         req_kwargs['url_params'] = request.view_args or {}
 
     req_kwargs['raw_response'] = True
@@ -134,24 +136,53 @@
         return res[1], error_code
 
     return res.text, res.status_code, res.headers.items()
 
 
 def append_url_search_params(url, params):  # @2022-05-09: add
     """
-    Appends a specified key/value pair as a new search parameter.
+    Appends specified key/value pair as search parameter.
+    Only append the key if its value is None.
 
     Example:
-        append_url_search_params('https://example.com',{'foo':1,'bar':2}) --> 'https://example.com?foo=1&bar=2' # append
-        append_url_search_params('https://example.com?foo=1&bar=2',{'baz':3}) --> 'https://example.com?foo=1&bar=2&baz=3' # append
-        append_url_search_params('https://example.com?foo=1&bar=2',{'bar':3}) --> 'https://example.com?foo=1&bar=3' # replace
-        append_url_search_params('a/b',{'c':3}) --> 'a/b?c=3'
+        append_url_search_params('https://example.com',{'foo':1,'bar':2, 'xx': None}) # 'https://example.com?foo=1&bar=2&xx' # append
+        append_url_search_params('https://example.com?foo=1&bar=2',{'baz':3}) # 'https://example.com?foo=1&bar=2&baz=3' # append
+        append_url_search_params('https://example.com?foo=1&bar=2',{'bar':3}) # 'https://example.com?foo=1&bar=3' # replace
+        append_url_search_params('a/b',{'c':3,'d':None}) # 'a/b?c=3&d'
+
+        append_url_search_params('https://example.com', ['a', 'b', 'c=2']) # 'https://example.com?a&b&c=2'
+        append_url_search_params('https://example.com', 'a=1&b=2&c')  # 'https://example.com?a=1&b=2&c'
 
     :param url:
     :param params:
     :return:
 
     """
-    url_parts = urllib.parse.urlparse(url)
-    query = dict(urllib.parse.parse_qsl(url_parts.query))
-    query.update(params)
-    return url_parts._replace(query=urllib.parse.urlencode(query)).geturl()
+    url_parts = urllib_parse.urlparse(url)
+    query = dict(urllib_parse.parse_qsl(url_parts.query))
+
+    kv_params = {}
+    k_params = []
+    params_type = type(params)
+    if params_type is list:
+        k_params = params
+    elif params_type is str:
+        k_params = [params]
+    elif params_type is dict:
+        for k, v in params.items():
+            if v is not None:
+                kv_params[k] = v
+            else:
+                k_params.append(k)
+        query.update(kv_params)
+
+    query_string = urllib_parse.urlencode(query)
+    if len(k_params) > 0:
+        k_str = '&'.join(k_params)
+        if query_string:
+            if not k_str.startswith('&'):
+                k_str = '&' + k_str
+            query_string += k_str
+        else:
+            query_string += k_str
+
+    return url_parts._replace(query=query_string).geturl()
```

### Comparing `flaskz-1.5/src/flaskz/utils/_request_args.py` & `flaskz-1.5.1/src/flaskz/utils/_request_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 
 def get_remote_addr():
     """
     Get the remote ip address.
 
     :return:
     """
-    return request.environ.get('HTTP_X_REAL_IP', request.remote_addr)
+    if request:
+        return request.environ.get('HTTP_X_REAL_IP', request.remote_addr)
 
 
 def is_ajax():
     """
     Check if the request is an ajax request.
     :return:
     """
-    return request.headers.get('X-Requested-With') == 'XMLHttpRequest'
+    if request:
+        return request.headers.get('X-Requested-With') == 'XMLHttpRequest'
+    return False
 
 
 def get_request_json(*args):
     """
     Get the JSON data(parsed) in request.
     If json does not exist or parsing json error, return {}
```

### Comparing `flaskz-1.5/src/flaskz/utils/_response.py` & `flaskz-1.5.1/src/flaskz/utils/_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,18 @@
             return status_code[1] or status_code[0]
         elif len_ > 0:
             return status_code[0]
     return status_code
 
 
 def get_current_response_manager(callback_name):
-    response_manager = getattr(current_app, 'response_manager', None)
-    if response_manager:
-        return getattr(response_manager, callback_name)
+    if current_app:
+        response_manager = getattr(current_app, 'response_manager', None)
+        if response_manager:
+            return getattr(response_manager, callback_name, None)
 
 
 class ResponseManager:
     """
     Used to generate response.
     """
```

### Comparing `flaskz-1.5/src/flaskz/utils/_timer.py` & `flaskz-1.5.1/src/flaskz/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.5.1/src/flaskz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.5
+Version: 1.5.1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,17 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.5.1** `2023/05/17`
+    - [C] `db_session`上下文管理器自动关闭非缓存session
+    - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
     - [A] 重构`flaskz.rest`路由生成模块*
         - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
         - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
         - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
         - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
         - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
```

### Comparing `flaskz-1.5/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.5.1/src/flaskz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

