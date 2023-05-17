# Comparing `tmp/esmerald_sessions-0.2.0.tar.gz` & `tmp/esmerald_sessions-0.3.0.tar.gz`

## Comparing `esmerald_sessions-0.2.0.tar` & `esmerald_sessions-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/esmerald_sessions/__init__.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/esmerald_sessions/backends.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/esmerald_sessions/config.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/esmerald_sessions/datastructures.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/esmerald_sessions/enums.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/esmerald_sessions/exceptions.py
--rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/esmerald_sessions/middleware.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/esmerald_sessions/protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/esmerald_sessions/py.typed
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/esmerald_sessions/types.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/LICENSE
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/README.md
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 esmerald_sessions-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/esmerald_sessions/__init__.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/esmerald_sessions/backends.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/esmerald_sessions/config.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/esmerald_sessions/datastructures.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/esmerald_sessions/enums.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/esmerald_sessions/exceptions.py
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/esmerald_sessions/middleware.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/esmerald_sessions/protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/esmerald_sessions/py.typed
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/esmerald_sessions/types.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/README.md
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 esmerald_sessions-0.3.0/PKG-INFO
```

### Comparing `esmerald_sessions-0.2.0/esmerald_sessions/__init__.py` & `esmerald_sessions-0.3.0/esmerald_sessions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 from .backends import (
     AioMemCacheSessionBackend,
     AioRedisSessionBackend,
     MemCacheSessionBackend,
     RedisSessionBackend,
 )
```

### Comparing `esmerald_sessions-0.2.0/esmerald_sessions/backends.py` & `esmerald_sessions-0.3.0/esmerald_sessions/backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING, Any, Optional, Union
 
 import orjson
 from aiomcache import Client as AioMemcache
-from aioredis import Redis as AioRedis
 from pymemcache.client.base import Client as MemCache
 from redis import Redis
+from redis.asyncio import Redis as AioRedis
 
 from esmerald_sessions.datastructures import MemCacheJSONSerde
 from esmerald_sessions.protocols import SessionBackend
 
 if TYPE_CHECKING:
     from pydantic.typing import DictAny
```

### Comparing `esmerald_sessions-0.2.0/esmerald_sessions/config.py` & `esmerald_sessions-0.3.0/esmerald_sessions/config.py`

 * *Files identical despite different names*

### Comparing `esmerald_sessions-0.2.0/esmerald_sessions/datastructures.py` & `esmerald_sessions-0.3.0/esmerald_sessions/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald_sessions-0.2.0/esmerald_sessions/exceptions.py` & `esmerald_sessions-0.3.0/esmerald_sessions/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald_sessions-0.2.0/esmerald_sessions/middleware.py` & `esmerald_sessions-0.3.0/esmerald_sessions/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald_sessions-0.2.0/esmerald_sessions/protocols.py` & `esmerald_sessions-0.3.0/esmerald_sessions/protocols.py`

 * *Files identical despite different names*

### Comparing `esmerald_sessions-0.2.0/LICENSE` & `esmerald_sessions-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald_sessions-0.2.0/README.md` & `esmerald_sessions-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `esmerald_sessions-0.2.0/PKG-INFO` & `esmerald_sessions-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald_sessions
-Version: 0.2.0
+Version: 0.3.0
 Summary: An alternative SessionMiddleware for Esmerald with Pydantic.
 Project-URL: Homepage, https://github.com/dymmond/esmerald-sessions
 Project-URL: Documentation, https://esmerald-sessions.dymmond.com/
 Project-URL: Changelog, https://esmerald-sessions.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald-sessions
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -19,37 +19,36 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: aiomcache>=0.7.0
-Requires-Dist: aioredis<3.0.0,>=2.0.1
 Requires-Dist: asyncio<4.0.0,>=3.4.3
-Requires-Dist: esmerald>=0.2.10
+Requires-Dist: esmerald>=1.2.3
+Requires-Dist: orjson>=3.8.12
 Requires-Dist: pydantic<2.0.0,>=1.10.2
 Requires-Dist: pymemcache<5.0.0,>=4.0.0
 Requires-Dist: redis<5.0.0,>=4.3.4
 Provides-Extra: all
 Requires-Dist: aiomcache>=0.7.0; extra == 'all'
-Requires-Dist: aioredis<3.0.0,>=2.0.1; extra == 'all'
 Requires-Dist: asyncio<4.0.0,>=3.4.3; extra == 'all'
 Requires-Dist: esmerald>=0.5.1; extra == 'all'
 Requires-Dist: pydantic<2.0.0,>=1.10.2; extra == 'all'
 Requires-Dist: pymemcache<5.0.0,>=4.0.0; extra == 'all'
 Requires-Dist: pytz>=2022.6; extra == 'all'
 Requires-Dist: redis<5.0.0,>=4.3.4; extra == 'all'
 Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all'
@@ -59,29 +58,30 @@
 Requires-Dist: flake8<7.0.0,>=3.8.3; extra == 'dev'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'dev'
 Requires-Dist: loguru<0.7.0,>=0.6.0; extra == 'dev'
 Requires-Dist: mypy==0.991; extra == 'dev'
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev'
 Provides-Extra: doc
-Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
+Requires-Dist: mdx-include<2.0.0,>=1.4.2; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
-Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
-Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
+Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.2.5; extra == 'doc'
+Requires-Dist: mkdocs-material<10.0.0,>=9.0.13; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'doc'
-Requires-Dist: mkdocstrings<0.20.0,>=0.19.0; extra == 'doc'
-Requires-Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc'
+Requires-Dist: mkdocstrings<0.30.0,>=0.20.0; extra == 'doc'
+Requires-Dist: pyyaml<7.0.0,>=6.0; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: asyncz[test]==0.1.3; extra == 'test'
 Requires-Dist: fakeredis>=1.10.1; extra == 'test'
-Requires-Dist: pytest-asyncio<0.20.0,>=0.19.0; extra == 'test'
+Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest-mock>=3.10.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.27.0; extra == 'test'
+Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Esmerald
 
 <p align="center">
   <a href="https://esmerald.dymmond.com"><img src="https://res.cloudinary.com/dymmond/image/upload/v1671718628/esmerald/img/logo-gr_oyr4my.png" alt='Esmerald'></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: esmerald_sessions Version: 0.2.0 Summary: An
+Metadata-Version: 2.1 Name: esmerald_sessions Version: 0.3.0 Summary: An
 alternative SessionMiddleware for Esmerald with Pydantic. Project-URL:
 Homepage, https://github.com/dymmond/esmerald-sessions Project-URL:
 Documentation, https://esmerald-sessions.dymmond.com/ Project-URL: Changelog,
 https://esmerald-sessions.dymmond.com/release-notes/ Project-URL: Funding,
 https://github.com/sponsors/tarsil Project-URL: Source, https://github.com/
 dymmond/esmerald-sessions Author-email: Tiago Silva
 silva@dymmond.com> License-Expression: MIT License-File: LICENSE Keywords:
@@ -11,52 +11,51 @@
 Status :: 4 - Beta Classifier: Environment :: Web Environment Classifier:
 Framework :: AnyIO Classifier: Framework :: AsyncIO Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Internet
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
 HTTP :: HTTP Servers Classifier: Topic :: Software Development Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Application Frameworks Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
-Requires-Python: >=3.7 Requires-Dist: aiomcache>=0.7.0 Requires-Dist:
-aioredis<3.0.0,>=2.0.1 Requires-Dist: asyncio<4.0.0,>=3.4.3 Requires-Dist:
-esmerald>=0.2.10 Requires-Dist: pydantic<2.0.0,>=1.10.2 Requires-Dist:
+Requires-Python: >=3.8 Requires-Dist: aiomcache>=0.7.0 Requires-Dist:
+asyncio<4.0.0,>=3.4.3 Requires-Dist: esmerald>=1.2.3 Requires-Dist:
+orjson>=3.8.12 Requires-Dist: pydantic<2.0.0,>=1.10.2 Requires-Dist:
 pymemcache<5.0.0,>=4.0.0 Requires-Dist: redis<5.0.0,>=4.3.4 Provides-Extra: all
 Requires-Dist: aiomcache>=0.7.0; extra == 'all' Requires-Dist:
-aioredis<3.0.0,>=2.0.1; extra == 'all' Requires-Dist: asyncio<4.0.0,>=3.4.3;
-extra == 'all' Requires-Dist: esmerald>=0.5.1; extra == 'all' Requires-Dist:
-pydantic<2.0.0,>=1.10.2; extra == 'all' Requires-Dist:
+asyncio<4.0.0,>=3.4.3; extra == 'all' Requires-Dist: esmerald>=0.5.1; extra ==
+'all' Requires-Dist: pydantic<2.0.0,>=1.10.2; extra == 'all' Requires-Dist:
 pymemcache<5.0.0,>=4.0.0; extra == 'all' Requires-Dist: pytz>=2022.6; extra ==
 'all' Requires-Dist: redis<5.0.0,>=4.3.4; extra == 'all' Requires-Dist:
 tzlocal<5.0,>=4.2; extra == 'all' Provides-Extra: dev Requires-Dist:
 autoflake<3.0.0,>=1.4.0; extra == 'dev' Requires-Dist: black<23.0.0,>=22.10.0;
 extra == 'dev' Requires-Dist: flake8<7.0.0,>=3.8.3; extra == 'dev' Requires-
 Dist: isort<6.0.0,>=5.0.6; extra == 'dev' Requires-Dist: loguru<0.7.0,>=0.6.0;
 extra == 'dev' Requires-Dist: mypy==0.991; extra == 'dev' Requires-Dist: pre-
 commit<3.0.0,>=2.17.0; extra == 'dev' Requires-Dist:
 watchfiles<0.20.0,>=0.16.1; extra == 'dev' Provides-Extra: doc Requires-Dist:
-mdx-include<2.0.0,>=1.4.1; extra == 'doc' Requires-Dist:
+mdx-include<2.0.0,>=1.4.2; extra == 'doc' Requires-Dist:
 mkautodoc<0.3.0,>=0.2.0; extra == 'doc' Requires-Dist: mkdocs-
-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc' Requires-Dist: mkdocs-
-material<9.0.0,>=8.1.4; extra == 'doc' Requires-Dist: mkdocs<2.0.0,>=1.1.2;
-extra == 'doc' Requires-Dist: mkdocstrings<0.20.0,>=0.19.0; extra == 'doc'
-Requires-Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc' Provides-Extra: test
+markdownextradata-plugin<0.3.0,>=0.2.5; extra == 'doc' Requires-Dist: mkdocs-
+material<10.0.0,>=9.0.13; extra == 'doc' Requires-Dist: mkdocs<2.0.0,>=1.1.2;
+extra == 'doc' Requires-Dist: mkdocstrings<0.30.0,>=0.20.0; extra == 'doc'
+Requires-Dist: pyyaml<7.0.0,>=6.0; extra == 'doc' Provides-Extra: test
 Requires-Dist: asyncz[test]==0.1.3; extra == 'test' Requires-Dist:
-fakeredis>=1.10.1; extra == 'test' Requires-Dist: pytest-
-asyncio<0.20.0,>=0.19.0; extra == 'test' Requires-Dist: pytest-
-cov<5.0.0,>=2.12.0; extra == 'test' Requires-Dist: pytest-mock>=3.10.0; extra
-== 'test' Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test' Requires-Dist:
-requests<3.0.0,>=2.27.0; extra == 'test' Description-Content-Type: text/
-markdown # Esmerald
+fakeredis>=1.10.1; extra == 'test' Requires-Dist: pytest-asyncio>=0.19.0; extra
+== 'test' Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test' Requires-
+Dist: pytest-mock>=3.10.0; extra == 'test' Requires-Dist: pytest<8.0.0,>=7.1.3;
+extra == 'test' Requires-Dist: requests<3.0.0,>=2.27.0; extra == 'test'
+Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test' Description-Content-Type:
+text/markdown # Esmerald
                                   [Esmerald]
  ð An alternative SessionMiddleware for Esmerald with Pydantic at its core.
                                      ð
           [Test_Suite] [Package_version] [Supported_Python_versions]
 --- **Documentation**: [https://esmerald-sessions.dymmond.com](https://
 esmerald-sessions.dymmond.com) ð **Source Code**: [https://github.com/
 dymmond/esmerald-sessions](https://github.com/dymmond/esmerald-sessions) --- ##
```

