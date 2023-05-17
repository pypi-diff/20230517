# Comparing `tmp/asyncmy-0.2.7rc6.tar.gz` & `tmp/asyncmy-0.2.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncmy-0.2.7rc6.tar", max compression
+gzip compressed data, was "asyncmy-0.2.8rc1.tar", max compression
```

## Comparing `asyncmy-0.2.7rc6.tar` & `asyncmy-0.2.8rc1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1128 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/LICENSE
--rw-r--r--   0        0        0     5077 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/README.md
--rw-r--r--   0        0        0      106 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/__init__.py
--rw-r--r--   0        0        0     6855 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/auth.py
--rw-r--r--   0        0        0       50 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/charset.pxd
--rw-r--r--   0        0        0    10493 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/charset.pyx
--rw-r--r--   0        0        0    49722 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/connection.pyx
--rw-r--r--   0        0        0      878 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/constants/CLIENT.py
--rw-r--r--   0        0        0      129 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/constants/COLUMN.py
--rw-r--r--   0        0        0      679 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/constants/COMMAND.py
--rw-r--r--   0        0        0     1927 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/constants/CR.py
--rw-r--r--   0        0        0    12296 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/constants/ER.py
--rw-r--r--   0        0        0      370 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/constants/FIELD_TYPE.py
--rw-r--r--   0        0        0      214 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/constants/FLAG.py
--rw-r--r--   0        0        0      333 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/constants/SERVER_STATUS.py
--rw-r--r--   0        0        0        0 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/constants/__init__.py
--rw-r--r--   0        0        0     2131 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/contexts.py
--rw-r--r--   0        0        0     9656 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/converters.pyx
--rw-r--r--   0        0        0    17446 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/cursors.pyx
--rw-r--r--   0        0        0     4004 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/errors.pyx
--rw-r--r--   0        0        0      479 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/optionfile.py
--rw-r--r--   0        0        0     6348 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/pool.pyx
--rw-r--r--   0        0        0    11582 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/protocol.pyx
--rw-r--r--   0        0        0       52 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/__init__.py
--rw-r--r--   0        0        0    13427 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/binlogstream.py
--rw-r--r--   0        0        0     2189 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/bitmap.py
--rw-r--r--   0        0        0     3254 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/column.py
--rw-r--r--   0        0        0     1687 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/constants.py
--rw-r--r--   0        0        0      277 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/errors.py
--rw-r--r--   0        0        0     6697 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/events.py
--rw-r--r--   0        0        0     8721 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/gtid.py
--rw-r--r--   0        0        0    15555 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/packets.py
--rw-r--r--   0        0        0    22843 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/row_events.py
--rw-r--r--   0        0        0      944 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/table.py
--rw-r--r--   0        0        0      178 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/replication/utils.py
--rw-r--r--   0        0        0      455 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/structs.py
--rw-r--r--   0        0        0       26 2023-02-03 05:38:55.884856 asyncmy-0.2.7rc6/asyncmy/version.py
--rw-r--r--   0        0        0      400 2023-02-03 05:38:55.888856 asyncmy-0.2.7rc6/build.py
--rw-r--r--   0        0        0     1299 2023-02-03 05:38:55.888856 asyncmy-0.2.7rc6/pyproject.toml
--rw-r--r--   0        0        0     5886 1970-01-01 00:00:00.000000 asyncmy-0.2.7rc6/setup.py
--rw-r--r--   0        0        0     5878 1970-01-01 00:00:00.000000 asyncmy-0.2.7rc6/PKG-INFO
+-rw-r--r--   0        0        0     1241 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/LICENSE
+-rw-r--r--   0        0        0     5077 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/README.md
+-rw-r--r--   0        0        0      106 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/__init__.py
+-rw-r--r--   0        0        0     6855 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/auth.py
+-rw-r--r--   0        0        0       50 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/charset.pxd
+-rw-r--r--   0        0        0    10493 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/charset.pyx
+-rw-r--r--   0        0        0    49722 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/connection.pyx
+-rw-r--r--   0        0        0      878 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/constants/CLIENT.py
+-rw-r--r--   0        0        0      129 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/constants/COLUMN.py
+-rw-r--r--   0        0        0      679 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/constants/COMMAND.py
+-rw-r--r--   0        0        0     1927 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/constants/CR.py
+-rw-r--r--   0        0        0    12296 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/constants/ER.py
+-rw-r--r--   0        0        0      370 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/constants/FIELD_TYPE.py
+-rw-r--r--   0        0        0      214 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/constants/FLAG.py
+-rw-r--r--   0        0        0      333 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/constants/SERVER_STATUS.py
+-rw-r--r--   0        0        0        0 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/constants/__init__.py
+-rw-r--r--   0        0        0     2131 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/contexts.py
+-rw-r--r--   0        0        0     9657 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/converters.pyx
+-rw-r--r--   0        0        0    17446 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/cursors.pyx
+-rw-r--r--   0        0        0     4004 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/errors.pyx
+-rw-r--r--   0        0        0      479 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/optionfile.py
+-rw-r--r--   0        0        0     6348 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/pool.pyx
+-rw-r--r--   0        0        0    11582 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/protocol.pyx
+-rw-r--r--   0        0        0       52 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/__init__.py
+-rw-r--r--   0        0        0    13427 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/binlogstream.py
+-rw-r--r--   0        0        0     2189 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/bitmap.py
+-rw-r--r--   0        0        0     3254 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/column.py
+-rw-r--r--   0        0        0     1687 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/constants.py
+-rw-r--r--   0        0        0      277 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/errors.py
+-rw-r--r--   0        0        0     6697 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/events.py
+-rw-r--r--   0        0        0     8721 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/gtid.py
+-rw-r--r--   0        0        0    15555 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/packets.py
+-rw-r--r--   0        0        0    22843 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/row_events.py
+-rw-r--r--   0        0        0      944 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/table.py
+-rw-r--r--   0        0        0      178 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/replication/utils.py
+-rw-r--r--   0        0        0      455 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/structs.py
+-rw-r--r--   0        0        0       26 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/asyncmy/version.py
+-rw-r--r--   0        0        0      400 2023-04-11 09:41:23.394249 asyncmy-0.2.8rc1/build.py
+-rw-r--r--   0        0        0     1299 2023-04-11 09:41:23.398249 asyncmy-0.2.8rc1/pyproject.toml
+-rw-r--r--   0        0        0     5886 1970-01-01 00:00:00.000000 asyncmy-0.2.8rc1/setup.py
+-rw-r--r--   0        0        0     5878 1970-01-01 00:00:00.000000 asyncmy-0.2.8rc1/PKG-INFO
```

### Comparing `asyncmy-0.2.7rc6/CHANGELOG.md` & `asyncmy-0.2.8rc1/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # ChangeLog
 
 ## 0.2
 
+## 0.2.8
+
+- Fix sudden loss of float precision. (#56)
+
+### 0.2.7
+
+- Fix `No module named 'asyncmy.connection'`.
+
 ### 0.2.6
 
 - Fix raise_mysql_exception (#28)
 - Implement `read_timeout` and remove `write_timeout` parameters (#44)
 
 ### 0.2.5
```

### Comparing `asyncmy-0.2.7rc6/LICENSE` & `asyncmy-0.2.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/README.md` & `asyncmy-0.2.8rc1/README.md`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/auth.py` & `asyncmy-0.2.8rc1/asyncmy/auth.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/charset.pyx` & `asyncmy-0.2.8rc1/asyncmy/charset.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/connection.pyx` & `asyncmy-0.2.8rc1/asyncmy/connection.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/constants/CLIENT.py` & `asyncmy-0.2.8rc1/asyncmy/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/constants/COMMAND.py` & `asyncmy-0.2.8rc1/asyncmy/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/constants/CR.py` & `asyncmy-0.2.8rc1/asyncmy/constants/CR.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/constants/ER.py` & `asyncmy-0.2.8rc1/asyncmy/constants/ER.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/contexts.py` & `asyncmy-0.2.8rc1/asyncmy/contexts.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/converters.pyx` & `asyncmy-0.2.8rc1/asyncmy/converters.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 cpdef str escape_bool(int value, mapping: dict = None):
     return str(int(value))
 
 cpdef str escape_int(long long value, mapping: dict = None):
     return str(value)
 
-cpdef str escape_float(float value, mapping: dict = None):
+cpdef str escape_float(double value, mapping: dict = None):
     s = repr(value)
     if s in ("inf", "nan"):
         raise ProgrammingError("%s can not be used with MySQL" % s)
     if "e" not in s:
         s += "e0"
     return s
```

### Comparing `asyncmy-0.2.7rc6/asyncmy/cursors.pyx` & `asyncmy-0.2.8rc1/asyncmy/cursors.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/errors.pyx` & `asyncmy-0.2.8rc1/asyncmy/errors.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/pool.pyx` & `asyncmy-0.2.8rc1/asyncmy/pool.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/protocol.pyx` & `asyncmy-0.2.8rc1/asyncmy/protocol.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/replication/binlogstream.py` & `asyncmy-0.2.8rc1/asyncmy/replication/binlogstream.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/replication/bitmap.py` & `asyncmy-0.2.8rc1/asyncmy/replication/bitmap.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/replication/column.py` & `asyncmy-0.2.8rc1/asyncmy/replication/column.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/replication/constants.py` & `asyncmy-0.2.8rc1/asyncmy/replication/constants.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/replication/events.py` & `asyncmy-0.2.8rc1/asyncmy/replication/events.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/replication/gtid.py` & `asyncmy-0.2.8rc1/asyncmy/replication/gtid.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/replication/packets.py` & `asyncmy-0.2.8rc1/asyncmy/replication/packets.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/replication/row_events.py` & `asyncmy-0.2.8rc1/asyncmy/replication/row_events.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/asyncmy/replication/table.py` & `asyncmy-0.2.8rc1/asyncmy/replication/table.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.7rc6/pyproject.toml` & `asyncmy-0.2.8rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 license = "Apache-2.0"
 name = "asyncmy"
 packages = [
     { include = "asyncmy" },
 ]
 readme = "README.md"
 repository = "https://github.com/long2ice/asyncmy.git"
-version = "0.2.7-rc6"
+version = "0.2.8-rc1"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "*"
 black = "*"
```

### Comparing `asyncmy-0.2.7rc6/setup.py` & `asyncmy-0.2.8rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['asyncmy', 'asyncmy.constants', 'asyncmy.replication']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'asyncmy',
-    'version': '0.2.7rc6',
+    'version': '0.2.8rc1',
     'description': 'A fast asyncio MySQL driver',
     'long_description': '# asyncmy - A fast asyncio MySQL/MariaDB driver\n\n[![image](https://img.shields.io/pypi/v/asyncmy.svg?style=flat)](https://pypi.python.org/pypi/asyncmy)\n[![image](https://img.shields.io/github/license/long2ice/asyncmy)](https://github.com/long2ice/asyncmy)\n[![pypi](https://github.com/long2ice/asyncmy/actions/workflows/pypi.yml/badge.svg)](https://github.com/long2ice/asyncmy/actions/workflows/pypi.yml)\n[![ci](https://github.com/long2ice/asyncmy/actions/workflows/ci.yml/badge.svg)](https://github.com/long2ice/asyncmy/actions/workflows/ci.yml)\n\n## Introduction\n\n`asyncmy` is a fast asyncio MySQL/MariaDB driver, which reuse most of [pymysql](https://github.com/PyMySQL/PyMySQL)\nand [aiomysql](https://github.com/aio-libs/aiomysql) but rewrite core protocol with [cython](https://cython.org/) to\nspeedup.\n\n## Features\n\n- API compatible with [aiomysql](https://github.com/aio-libs/aiomysql).\n- Faster by [cython](https://cython.org/).\n- MySQL replication protocol support with `asyncio`.\n- Tested both MySQL and MariaDB in [CI](https://github.com/long2ice/asyncmy/blob/dev/.github/workflows/ci.yml).\n\n## Benchmark\n\nThe result comes from [benchmark](./benchmark).\n\n> The device is iMac Pro(2017) i9 3.6GHz 48G and MySQL version is 8.0.26.\n\n![benchmark](./images/benchmark.png)\n\n### Conclusion\n\n- There is no doubt that `mysqlclient` is the fastest MySQL driver.\n- All kinds of drivers have a small gap except `select`.\n- `asyncio` could enhance `insert`.\n- `asyncmy` performs remarkable when compared to other drivers.\n\n## Install\n\n```shell\npip install asyncmy\n```\n\n### Installing on Windows\n\nTo install asyncmy on Windows, you need to install the tools needed to build it.\n\n1. Download *Microsoft C++ Build Tools* from https://visualstudio.microsoft.com/visual-cpp-build-tools/\n2. Run CMD as Admin (not required but recommended) and navigate to the folder when your installer is downloaded\n3. Installer executable should look like this `vs_buildtools__XXXXXXXXX.XXXXXXXXXX.exe`, it will be easier if you rename\n   it to just `vs_buildtools.exe`\n4. Run this command (Make sure you have about 5-6GB of free storage)\n\n```shell\nvs_buildtools.exe --norestart --passive --downloadThenInstall --includeRecommended --add Microsoft.VisualStudio.Workload.NativeDesktop --add Microsoft.VisualStudio.Workload.VCTools --add Microsoft.VisualStudio.Workload.MSBuildTools\n```\n\n5. Wait until the installation is finished\n6. After installation will finish, restart your computer\n7. Install asyncmy via PIP\n\n```shell\npip install asyncmy\n```\n\nNow you can uninstall previously installed tools.\n\n## Usage\n\n### Use `connect`\n\n`asyncmy` provides a way to connect to MySQL database with simple factory function `asyncmy.connnect()`. Use this\nfunction if you want just one connection to the database, consider connection pool for multiple connections.\n\n```py\nfrom asyncmy import connect\nfrom asyncmy.cursors import DictCursor\nimport asyncio\n\n\nasync def run():\n    conn = await connect()\n    async with conn.cursor(cursor=DictCursor) as cursor:\n        await cursor.execute("create database if not exists test")\n        await cursor.execute(\n            """CREATE TABLE if not exists test.asyncmy\n    (\n        `id`       int primary key auto_increment,\n        `decimal`  decimal(10, 2),\n        `date`     date,\n        `datetime` datetime,\n        `float`    float,\n        `string`   varchar(200),\n        `tinyint`  tinyint\n    )"""\n        )\n\n\nif __name__ == \'__main__\':\n    asyncio.run(run())\n```\n\n### Use `pool`\n\n`asyncmy` provides connection pool as well as plain Connection objects.\n\n```py\nimport asyncmy\nimport asyncio\n\n\nasync def run():\n    pool = await asyncmy.create_pool()\n    async with pool.acquire() as conn:\n        async with conn.cursor() as cursor:\n            await cursor.execute("SELECT 1")\n            ret = await cursor.fetchone()\n            assert ret == (1,)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(run())\n```\n\n## Replication\n\n`asyncmy` supports MySQL replication protocol\nlike [python-mysql-replication](https://github.com/noplay/python-mysql-replication), but powered by `asyncio`.\n\n```py\nfrom asyncmy import connect\nfrom asyncmy.replication import BinLogStream\nimport asyncio\n\n\nasync def run():\n    conn = await connect()\n    ctl_conn = await connect()\n\n    stream = BinLogStream(\n        conn,\n        ctl_conn,\n        1,\n        master_log_file="binlog.000172",\n        master_log_position=2235312,\n        resume_stream=True,\n        blocking=True,\n    )\n    async for event in stream:\n        print(event)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(run())\n```\n\n## ThanksTo\n\n> asyncmy is build on top of these awesome projects.\n\n- [pymysql](https://github/pymysql/PyMySQL), a pure python MySQL client.\n- [aiomysql](https://github.com/aio-libs/aiomysql), a library for accessing a MySQL database from the asyncio.\n- [python-mysql-replication](https://github.com/noplay/python-mysql-replication), pure Python Implementation of MySQL\n  replication protocol build on top of PyMYSQL.\n\n## License\n\nThis project is licensed under the [Apache-2.0](./LICENSE) License.\n',
     'author': 'long2ice',
     'author_email': 'long2ice@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/long2ice/asyncmy',
```

### Comparing `asyncmy-0.2.7rc6/PKG-INFO` & `asyncmy-0.2.8rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncmy
-Version: 0.2.7rc6
+Version: 0.2.8rc1
 Summary: A fast asyncio MySQL driver
 Home-page: https://github.com/long2ice/asyncmy
 License: Apache-2.0
 Keywords: driver,asyncio,mysql
 Author: long2ice
 Author-email: long2ice@gmail.com
 Requires-Python: >=3.7,<4.0
```

