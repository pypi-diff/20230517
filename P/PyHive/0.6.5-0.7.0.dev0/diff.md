# Comparing `tmp/PyHive-0.6.5.tar.gz` & `tmp/PyHive-0.7.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHive-0.6.5.tar", last modified: Mon Mar  7 23:09:33 2022, max compression
+gzip compressed data, was "PyHive-0.7.0.dev0.tar", last modified: Wed May 17 19:03:25 2023, max compression
```

## Comparing `PyHive-0.6.5.tar` & `PyHive-0.7.0.dev0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 bogdankyryliuk   (503) staff       (20)        0 2022-03-07 23:09:33.816537 PyHive-0.6.5/
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)      558 2021-03-17 18:29:08.000000 PyHive-0.6.5/LICENSE
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)       16 2021-03-17 18:29:08.000000 PyHive-0.6.5/MANIFEST.in
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)     7862 2022-03-07 23:09:33.816714 PyHive-0.6.5/PKG-INFO
-drwxr-xr-x   0 bogdankyryliuk   (503) staff       (20)        0 2022-03-07 23:09:33.807537 PyHive-0.6.5/PyHive.egg-info/
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)     7862 2022-03-07 23:09:33.000000 PyHive-0.6.5/PyHive.egg-info/PKG-INFO
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)      508 2022-03-07 23:09:33.000000 PyHive-0.6.5/PyHive.egg-info/SOURCES.txt
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)        1 2022-03-07 23:09:33.000000 PyHive-0.6.5/PyHive.egg-info/dependency_links.txt
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)      269 2022-03-07 23:09:33.000000 PyHive-0.6.5/PyHive.egg-info/entry_points.txt
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)      198 2022-03-07 23:09:33.000000 PyHive-0.6.5/PyHive.egg-info/requires.txt
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)       19 2022-03-07 23:09:33.000000 PyHive-0.6.5/PyHive.egg-info/top_level.txt
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)     5915 2022-03-07 23:02:32.000000 PyHive-0.6.5/README.rst
-drwxr-xr-x   0 bogdankyryliuk   (503) staff       (20)        0 2022-03-07 23:09:33.810389 PyHive-0.6.5/TCLIService/
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)   131364 2021-03-17 18:29:08.000000 PyHive-0.6.5/TCLIService/TCLIService.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)       49 2021-03-17 18:29:08.000000 PyHive-0.6.5/TCLIService/__init__.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)     1087 2021-03-17 18:29:08.000000 PyHive-0.6.5/TCLIService/constants.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)   263044 2021-03-17 18:29:08.000000 PyHive-0.6.5/TCLIService/ttypes.py
-drwxr-xr-x   0 bogdankyryliuk   (503) staff       (20)        0 2022-03-07 23:09:33.816063 PyHive-0.6.5/pyhive/
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)      101 2022-03-07 23:07:48.000000 PyHive-0.6.5/pyhive/__init__.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)     9248 2021-03-17 18:29:08.000000 PyHive-0.6.5/pyhive/common.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)     2196 2021-03-17 18:29:08.000000 PyHive-0.6.5/pyhive/exc.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)    22401 2022-03-07 23:02:32.000000 PyHive-0.6.5/pyhive/hive.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)    15379 2022-03-07 23:02:32.000000 PyHive-0.6.5/pyhive/presto.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)    13019 2021-04-23 18:12:46.000000 PyHive-0.6.5/pyhive/sqlalchemy_hive.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)     7388 2021-03-17 18:29:08.000000 PyHive-0.6.5/pyhive/sqlalchemy_presto.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)     1926 2021-04-23 18:12:46.000000 PyHive-0.6.5/pyhive/sqlalchemy_trino.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)     4833 2022-03-07 23:02:32.000000 PyHive-0.6.5/pyhive/trino.py
--rw-r--r--   0 bogdankyryliuk   (503) staff       (20)      883 2022-03-07 23:09:33.817316 PyHive-0.6.5/setup.cfg
--rwxr-xr-x   0 bogdankyryliuk   (503) staff       (20)     2149 2022-03-07 23:02:32.000000 PyHive-0.6.5/setup.py
+drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-05-17 19:03:25.969788 PyHive-0.7.0.dev0/
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      558 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/LICENSE
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)       16 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/MANIFEST.in
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     6474 2023-05-17 19:03:25.969849 PyHive-0.7.0.dev0/PKG-INFO
+drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-05-17 19:03:25.966211 PyHive-0.7.0.dev0/PyHive.egg-info/
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     6474 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/PKG-INFO
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      508 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/SOURCES.txt
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)        1 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/dependency_links.txt
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      268 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/entry_points.txt
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      198 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/requires.txt
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)       19 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/top_level.txt
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     5915 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/README.rst
+drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-05-17 19:03:25.967517 PyHive-0.7.0.dev0/TCLIService/
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)   131364 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/TCLIService/TCLIService.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)       49 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/TCLIService/__init__.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     1087 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/TCLIService/constants.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)   263044 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/TCLIService/ttypes.py
+drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-05-17 19:03:25.969609 PyHive-0.7.0.dev0/pyhive/
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      101 2023-05-17 17:02:25.000000 PyHive-0.7.0.dev0/pyhive/__init__.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     9340 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/common.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     2196 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/exc.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)    22401 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/hive.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)    15379 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/presto.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)    13017 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/sqlalchemy_hive.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     7388 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/sqlalchemy_presto.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     1926 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/sqlalchemy_trino.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     4833 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/trino.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      881 2023-05-17 19:03:25.970459 PyHive-0.7.0.dev0/setup.cfg
+-rwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)     2149 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/setup.py
```

### Comparing `PyHive-0.6.5/LICENSE` & `PyHive-0.7.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/PKG-INFO` & `PyHive-0.7.0.dev0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,192 +1,192 @@
 Metadata-Version: 2.1
 Name: PyHive
-Version: 0.6.5
+Version: 0.7.0.dev0
 Summary: Python interface to Hive
 Home-page: https://github.com/dropbox/PyHive
 Author: Jing Wang
 Author-email: jing@dropbox.com
 License: Apache License, Version 2.0
-Description: ================================
-        Project is currently unsupported
-        ================================
-        
-        
-        
-        
-        .. image:: https://travis-ci.org/dropbox/PyHive.svg?branch=master
-            :target: https://travis-ci.org/dropbox/PyHive
-        .. image:: https://img.shields.io/codecov/c/github/dropbox/PyHive.svg
-        
-        ======
-        PyHive
-        ======
-        
-        PyHive is a collection of Python `DB-API <http://www.python.org/dev/peps/pep-0249/>`_ and
-        `SQLAlchemy <http://www.sqlalchemy.org/>`_ interfaces for `Presto <http://prestodb.io/>`_ and
-        `Hive <http://hive.apache.org/>`_.
-        
-        Usage
-        =====
-        
-        DB-API
-        ------
-        .. code-block:: python
-        
-            from pyhive import presto  # or import hive or import trino
-            cursor = presto.connect('localhost').cursor()
-            cursor.execute('SELECT * FROM my_awesome_data LIMIT 10')
-            print cursor.fetchone()
-            print cursor.fetchall()
-        
-        DB-API (asynchronous)
-        ---------------------
-        .. code-block:: python
-        
-            from pyhive import hive
-            from TCLIService.ttypes import TOperationState
-            cursor = hive.connect('localhost').cursor()
-            cursor.execute('SELECT * FROM my_awesome_data LIMIT 10', async=True)
-        
-            status = cursor.poll().operationState
-            while status in (TOperationState.INITIALIZED_STATE, TOperationState.RUNNING_STATE):
-                logs = cursor.fetch_logs()
-                for message in logs:
-                    print message
-        
-                # If needed, an asynchronous query can be cancelled at any time with:
-                # cursor.cancel()
-        
-                status = cursor.poll().operationState
-        
-            print cursor.fetchall()
-        
-        In Python 3.7 `async` became a keyword; you can use `async_` instead:
-        
-        .. code-block:: python
-        
-            cursor.execute('SELECT * FROM my_awesome_data LIMIT 10', async_=True)
-        
-        
-        SQLAlchemy
-        ----------
-        First install this package to register it with SQLAlchemy (see ``setup.py``).
-        
-        .. code-block:: python
-        
-            from sqlalchemy import *
-            from sqlalchemy.engine import create_engine
-            from sqlalchemy.schema import *
-            # Presto
-            engine = create_engine('presto://localhost:8080/hive/default')
-            # Trino
-            engine = create_engine('trino://localhost:8080/hive/default')
-            # Hive
-            engine = create_engine('hive://localhost:10000/default')
-            logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
-            print select([func.count('*')], from_obj=logs).scalar()
-        
-            # Hive + HTTPS + LDAP or basic Auth
-            engine = create_engine('hive+https://username:password@localhost:10000/')
-            logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
-            print select([func.count('*')], from_obj=logs).scalar()
-        
-        Note: query generation functionality is not exhaustive or fully tested, but there should be no
-        problem with raw SQL.
-        
-        Passing session configuration
-        -----------------------------
-        
-        .. code-block:: python
-        
-            # DB-API
-            hive.connect('localhost', configuration={'hive.exec.reducers.max': '123'})
-            presto.connect('localhost', session_props={'query_max_run_time': '1234m'})
-            trino.connect('localhost',  session_props={'query_max_run_time': '1234m'})
-            # SQLAlchemy
-            create_engine(
-                'presto://user@host:443/hive',
-                connect_args={'protocol': 'https',
-                              'session_props': {'query_max_run_time': '1234m'}}
-            )
-            create_engine(
-                'trino://user@host:443/hive',
-                connect_args={'protocol': 'https',
-                              'session_props': {'query_max_run_time': '1234m'}}
-            )
-            create_engine(
-                'hive://user@host:10000/database',
-                connect_args={'configuration': {'hive.exec.reducers.max': '123'}},
-            )
-            # SQLAlchemy with LDAP
-            create_engine(
-                'hive://user:password@host:10000/database',
-                connect_args={'auth': 'LDAP'},
-            )
-        
-        Requirements
-        ============
-        
-        Install using
-        
-        - ``pip install 'pyhive[hive]'`` for the Hive interface and
-        - ``pip install 'pyhive[presto]'`` for the Presto interface.
-        - ``pip install 'pyhive[trino]'`` for the Trino interface
-        
-        PyHive works with
-        
-        - Python 2.7 / Python 3
-        - For Presto: Presto install
-        - For Trino: Trino install
-        - For Hive: `HiveServer2 <https://cwiki.apache.org/confluence/display/Hive/Setting+up+HiveServer2>`_ daemon
-        
-        Changelog
-        =========
-        See https://github.com/dropbox/PyHive/releases.
-        
-        Contributing
-        ============
-        - Please fill out the Dropbox Contributor License Agreement at https://opensource.dropbox.com/cla/ and note this in your pull request.
-        - Changes must come with tests, with the exception of trivial things like fixing comments. See .travis.yml for the test environment setup.
-        - Notes on project scope:
-        
-          - This project is intended to be a minimal Hive/Presto client that does that one thing and nothing else.
-            Features that can be implemented on top of PyHive, such integration with your favorite data analysis library, are likely out of scope.
-          - We prefer having a small number of generic features over a large number of specialized, inflexible features.
-            For example, the Presto code takes an arbitrary ``requests_session`` argument for customizing HTTP calls, as opposed to having a separate parameter/branch for each ``requests`` option.
-        
-        Testing
-        =======
-        .. image:: https://travis-ci.org/dropbox/PyHive.svg
-            :target: https://travis-ci.org/dropbox/PyHive
-        .. image:: http://codecov.io/github/dropbox/PyHive/coverage.svg?branch=master
-            :target: http://codecov.io/github/dropbox/PyHive?branch=master
-        
-        Run the following in an environment with Hive/Presto::
-        
-            ./scripts/make_test_tables.sh
-            virtualenv --no-site-packages env
-            source env/bin/activate
-            pip install -e .
-            pip install -r dev_requirements.txt
-            py.test
-        
-        WARNING: This drops/creates tables named ``one_row``, ``one_row_complex``, and ``many_rows``, plus a
-        database called ``pyhive_test_database``.
-        
-        Updating TCLIService
-        ====================
-        
-        The TCLIService module is autogenerated using a ``TCLIService.thrift`` file. To update it, the
-        ``generate.py`` file can be used: ``python generate.py <TCLIServiceURL>``. When left blank, the
-        version for Hive 2.3 will be downloaded.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database :: Front-Ends
 Provides-Extra: presto
 Provides-Extra: trino
 Provides-Extra: hive
 Provides-Extra: sqlalchemy
 Provides-Extra: kerberos
+License-File: LICENSE
+
+================================
+Project is currently unsupported
+================================
+
+
+
+
+.. image:: https://travis-ci.org/dropbox/PyHive.svg?branch=master
+    :target: https://travis-ci.org/dropbox/PyHive
+.. image:: https://img.shields.io/codecov/c/github/dropbox/PyHive.svg
+
+======
+PyHive
+======
+
+PyHive is a collection of Python `DB-API <http://www.python.org/dev/peps/pep-0249/>`_ and
+`SQLAlchemy <http://www.sqlalchemy.org/>`_ interfaces for `Presto <http://prestodb.io/>`_ and
+`Hive <http://hive.apache.org/>`_.
+
+Usage
+=====
+
+DB-API
+------
+.. code-block:: python
+
+    from pyhive import presto  # or import hive or import trino
+    cursor = presto.connect('localhost').cursor()
+    cursor.execute('SELECT * FROM my_awesome_data LIMIT 10')
+    print cursor.fetchone()
+    print cursor.fetchall()
+
+DB-API (asynchronous)
+---------------------
+.. code-block:: python
+
+    from pyhive import hive
+    from TCLIService.ttypes import TOperationState
+    cursor = hive.connect('localhost').cursor()
+    cursor.execute('SELECT * FROM my_awesome_data LIMIT 10', async=True)
+
+    status = cursor.poll().operationState
+    while status in (TOperationState.INITIALIZED_STATE, TOperationState.RUNNING_STATE):
+        logs = cursor.fetch_logs()
+        for message in logs:
+            print message
+
+        # If needed, an asynchronous query can be cancelled at any time with:
+        # cursor.cancel()
+
+        status = cursor.poll().operationState
+
+    print cursor.fetchall()
+
+In Python 3.7 `async` became a keyword; you can use `async_` instead:
+
+.. code-block:: python
+
+    cursor.execute('SELECT * FROM my_awesome_data LIMIT 10', async_=True)
+
+
+SQLAlchemy
+----------
+First install this package to register it with SQLAlchemy (see ``setup.py``).
+
+.. code-block:: python
+
+    from sqlalchemy import *
+    from sqlalchemy.engine import create_engine
+    from sqlalchemy.schema import *
+    # Presto
+    engine = create_engine('presto://localhost:8080/hive/default')
+    # Trino
+    engine = create_engine('trino://localhost:8080/hive/default')
+    # Hive
+    engine = create_engine('hive://localhost:10000/default')
+    logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
+    print select([func.count('*')], from_obj=logs).scalar()
+
+    # Hive + HTTPS + LDAP or basic Auth
+    engine = create_engine('hive+https://username:password@localhost:10000/')
+    logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
+    print select([func.count('*')], from_obj=logs).scalar()
+
+Note: query generation functionality is not exhaustive or fully tested, but there should be no
+problem with raw SQL.
+
+Passing session configuration
+-----------------------------
+
+.. code-block:: python
+
+    # DB-API
+    hive.connect('localhost', configuration={'hive.exec.reducers.max': '123'})
+    presto.connect('localhost', session_props={'query_max_run_time': '1234m'})
+    trino.connect('localhost',  session_props={'query_max_run_time': '1234m'})
+    # SQLAlchemy
+    create_engine(
+        'presto://user@host:443/hive',
+        connect_args={'protocol': 'https',
+                      'session_props': {'query_max_run_time': '1234m'}}
+    )
+    create_engine(
+        'trino://user@host:443/hive',
+        connect_args={'protocol': 'https',
+                      'session_props': {'query_max_run_time': '1234m'}}
+    )
+    create_engine(
+        'hive://user@host:10000/database',
+        connect_args={'configuration': {'hive.exec.reducers.max': '123'}},
+    )
+    # SQLAlchemy with LDAP
+    create_engine(
+        'hive://user:password@host:10000/database',
+        connect_args={'auth': 'LDAP'},
+    )
+
+Requirements
+============
+
+Install using
+
+- ``pip install 'pyhive[hive]'`` for the Hive interface and
+- ``pip install 'pyhive[presto]'`` for the Presto interface.
+- ``pip install 'pyhive[trino]'`` for the Trino interface
+
+PyHive works with
+
+- Python 2.7 / Python 3
+- For Presto: Presto install
+- For Trino: Trino install
+- For Hive: `HiveServer2 <https://cwiki.apache.org/confluence/display/Hive/Setting+up+HiveServer2>`_ daemon
+
+Changelog
+=========
+See https://github.com/dropbox/PyHive/releases.
+
+Contributing
+============
+- Please fill out the Dropbox Contributor License Agreement at https://opensource.dropbox.com/cla/ and note this in your pull request.
+- Changes must come with tests, with the exception of trivial things like fixing comments. See .travis.yml for the test environment setup.
+- Notes on project scope:
+
+  - This project is intended to be a minimal Hive/Presto client that does that one thing and nothing else.
+    Features that can be implemented on top of PyHive, such integration with your favorite data analysis library, are likely out of scope.
+  - We prefer having a small number of generic features over a large number of specialized, inflexible features.
+    For example, the Presto code takes an arbitrary ``requests_session`` argument for customizing HTTP calls, as opposed to having a separate parameter/branch for each ``requests`` option.
+
+Testing
+=======
+.. image:: https://travis-ci.org/dropbox/PyHive.svg
+    :target: https://travis-ci.org/dropbox/PyHive
+.. image:: http://codecov.io/github/dropbox/PyHive/coverage.svg?branch=master
+    :target: http://codecov.io/github/dropbox/PyHive?branch=master
+
+Run the following in an environment with Hive/Presto::
+
+    ./scripts/make_test_tables.sh
+    virtualenv --no-site-packages env
+    source env/bin/activate
+    pip install -e .
+    pip install -r dev_requirements.txt
+    py.test
+
+WARNING: This drops/creates tables named ``one_row``, ``one_row_complex``, and ``many_rows``, plus a
+database called ``pyhive_test_database``.
+
+Updating TCLIService
+====================
+
+The TCLIService module is autogenerated using a ``TCLIService.thrift`` file. To update it, the
+``generate.py`` file can be used: ``python generate.py <TCLIServiceURL>``. When left blank, the
+version for Hive 2.3 will be downloaded.
```

### Comparing `PyHive-0.6.5/PyHive.egg-info/PKG-INFO` & `PyHive-0.7.0.dev0/PyHive.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,192 +1,192 @@
 Metadata-Version: 2.1
 Name: PyHive
-Version: 0.6.5
+Version: 0.7.0.dev0
 Summary: Python interface to Hive
 Home-page: https://github.com/dropbox/PyHive
 Author: Jing Wang
 Author-email: jing@dropbox.com
 License: Apache License, Version 2.0
-Description: ================================
-        Project is currently unsupported
-        ================================
-        
-        
-        
-        
-        .. image:: https://travis-ci.org/dropbox/PyHive.svg?branch=master
-            :target: https://travis-ci.org/dropbox/PyHive
-        .. image:: https://img.shields.io/codecov/c/github/dropbox/PyHive.svg
-        
-        ======
-        PyHive
-        ======
-        
-        PyHive is a collection of Python `DB-API <http://www.python.org/dev/peps/pep-0249/>`_ and
-        `SQLAlchemy <http://www.sqlalchemy.org/>`_ interfaces for `Presto <http://prestodb.io/>`_ and
-        `Hive <http://hive.apache.org/>`_.
-        
-        Usage
-        =====
-        
-        DB-API
-        ------
-        .. code-block:: python
-        
-            from pyhive import presto  # or import hive or import trino
-            cursor = presto.connect('localhost').cursor()
-            cursor.execute('SELECT * FROM my_awesome_data LIMIT 10')
-            print cursor.fetchone()
-            print cursor.fetchall()
-        
-        DB-API (asynchronous)
-        ---------------------
-        .. code-block:: python
-        
-            from pyhive import hive
-            from TCLIService.ttypes import TOperationState
-            cursor = hive.connect('localhost').cursor()
-            cursor.execute('SELECT * FROM my_awesome_data LIMIT 10', async=True)
-        
-            status = cursor.poll().operationState
-            while status in (TOperationState.INITIALIZED_STATE, TOperationState.RUNNING_STATE):
-                logs = cursor.fetch_logs()
-                for message in logs:
-                    print message
-        
-                # If needed, an asynchronous query can be cancelled at any time with:
-                # cursor.cancel()
-        
-                status = cursor.poll().operationState
-        
-            print cursor.fetchall()
-        
-        In Python 3.7 `async` became a keyword; you can use `async_` instead:
-        
-        .. code-block:: python
-        
-            cursor.execute('SELECT * FROM my_awesome_data LIMIT 10', async_=True)
-        
-        
-        SQLAlchemy
-        ----------
-        First install this package to register it with SQLAlchemy (see ``setup.py``).
-        
-        .. code-block:: python
-        
-            from sqlalchemy import *
-            from sqlalchemy.engine import create_engine
-            from sqlalchemy.schema import *
-            # Presto
-            engine = create_engine('presto://localhost:8080/hive/default')
-            # Trino
-            engine = create_engine('trino://localhost:8080/hive/default')
-            # Hive
-            engine = create_engine('hive://localhost:10000/default')
-            logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
-            print select([func.count('*')], from_obj=logs).scalar()
-        
-            # Hive + HTTPS + LDAP or basic Auth
-            engine = create_engine('hive+https://username:password@localhost:10000/')
-            logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
-            print select([func.count('*')], from_obj=logs).scalar()
-        
-        Note: query generation functionality is not exhaustive or fully tested, but there should be no
-        problem with raw SQL.
-        
-        Passing session configuration
-        -----------------------------
-        
-        .. code-block:: python
-        
-            # DB-API
-            hive.connect('localhost', configuration={'hive.exec.reducers.max': '123'})
-            presto.connect('localhost', session_props={'query_max_run_time': '1234m'})
-            trino.connect('localhost',  session_props={'query_max_run_time': '1234m'})
-            # SQLAlchemy
-            create_engine(
-                'presto://user@host:443/hive',
-                connect_args={'protocol': 'https',
-                              'session_props': {'query_max_run_time': '1234m'}}
-            )
-            create_engine(
-                'trino://user@host:443/hive',
-                connect_args={'protocol': 'https',
-                              'session_props': {'query_max_run_time': '1234m'}}
-            )
-            create_engine(
-                'hive://user@host:10000/database',
-                connect_args={'configuration': {'hive.exec.reducers.max': '123'}},
-            )
-            # SQLAlchemy with LDAP
-            create_engine(
-                'hive://user:password@host:10000/database',
-                connect_args={'auth': 'LDAP'},
-            )
-        
-        Requirements
-        ============
-        
-        Install using
-        
-        - ``pip install 'pyhive[hive]'`` for the Hive interface and
-        - ``pip install 'pyhive[presto]'`` for the Presto interface.
-        - ``pip install 'pyhive[trino]'`` for the Trino interface
-        
-        PyHive works with
-        
-        - Python 2.7 / Python 3
-        - For Presto: Presto install
-        - For Trino: Trino install
-        - For Hive: `HiveServer2 <https://cwiki.apache.org/confluence/display/Hive/Setting+up+HiveServer2>`_ daemon
-        
-        Changelog
-        =========
-        See https://github.com/dropbox/PyHive/releases.
-        
-        Contributing
-        ============
-        - Please fill out the Dropbox Contributor License Agreement at https://opensource.dropbox.com/cla/ and note this in your pull request.
-        - Changes must come with tests, with the exception of trivial things like fixing comments. See .travis.yml for the test environment setup.
-        - Notes on project scope:
-        
-          - This project is intended to be a minimal Hive/Presto client that does that one thing and nothing else.
-            Features that can be implemented on top of PyHive, such integration with your favorite data analysis library, are likely out of scope.
-          - We prefer having a small number of generic features over a large number of specialized, inflexible features.
-            For example, the Presto code takes an arbitrary ``requests_session`` argument for customizing HTTP calls, as opposed to having a separate parameter/branch for each ``requests`` option.
-        
-        Testing
-        =======
-        .. image:: https://travis-ci.org/dropbox/PyHive.svg
-            :target: https://travis-ci.org/dropbox/PyHive
-        .. image:: http://codecov.io/github/dropbox/PyHive/coverage.svg?branch=master
-            :target: http://codecov.io/github/dropbox/PyHive?branch=master
-        
-        Run the following in an environment with Hive/Presto::
-        
-            ./scripts/make_test_tables.sh
-            virtualenv --no-site-packages env
-            source env/bin/activate
-            pip install -e .
-            pip install -r dev_requirements.txt
-            py.test
-        
-        WARNING: This drops/creates tables named ``one_row``, ``one_row_complex``, and ``many_rows``, plus a
-        database called ``pyhive_test_database``.
-        
-        Updating TCLIService
-        ====================
-        
-        The TCLIService module is autogenerated using a ``TCLIService.thrift`` file. To update it, the
-        ``generate.py`` file can be used: ``python generate.py <TCLIServiceURL>``. When left blank, the
-        version for Hive 2.3 will be downloaded.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database :: Front-Ends
 Provides-Extra: presto
 Provides-Extra: trino
 Provides-Extra: hive
 Provides-Extra: sqlalchemy
 Provides-Extra: kerberos
+License-File: LICENSE
+
+================================
+Project is currently unsupported
+================================
+
+
+
+
+.. image:: https://travis-ci.org/dropbox/PyHive.svg?branch=master
+    :target: https://travis-ci.org/dropbox/PyHive
+.. image:: https://img.shields.io/codecov/c/github/dropbox/PyHive.svg
+
+======
+PyHive
+======
+
+PyHive is a collection of Python `DB-API <http://www.python.org/dev/peps/pep-0249/>`_ and
+`SQLAlchemy <http://www.sqlalchemy.org/>`_ interfaces for `Presto <http://prestodb.io/>`_ and
+`Hive <http://hive.apache.org/>`_.
+
+Usage
+=====
+
+DB-API
+------
+.. code-block:: python
+
+    from pyhive import presto  # or import hive or import trino
+    cursor = presto.connect('localhost').cursor()
+    cursor.execute('SELECT * FROM my_awesome_data LIMIT 10')
+    print cursor.fetchone()
+    print cursor.fetchall()
+
+DB-API (asynchronous)
+---------------------
+.. code-block:: python
+
+    from pyhive import hive
+    from TCLIService.ttypes import TOperationState
+    cursor = hive.connect('localhost').cursor()
+    cursor.execute('SELECT * FROM my_awesome_data LIMIT 10', async=True)
+
+    status = cursor.poll().operationState
+    while status in (TOperationState.INITIALIZED_STATE, TOperationState.RUNNING_STATE):
+        logs = cursor.fetch_logs()
+        for message in logs:
+            print message
+
+        # If needed, an asynchronous query can be cancelled at any time with:
+        # cursor.cancel()
+
+        status = cursor.poll().operationState
+
+    print cursor.fetchall()
+
+In Python 3.7 `async` became a keyword; you can use `async_` instead:
+
+.. code-block:: python
+
+    cursor.execute('SELECT * FROM my_awesome_data LIMIT 10', async_=True)
+
+
+SQLAlchemy
+----------
+First install this package to register it with SQLAlchemy (see ``setup.py``).
+
+.. code-block:: python
+
+    from sqlalchemy import *
+    from sqlalchemy.engine import create_engine
+    from sqlalchemy.schema import *
+    # Presto
+    engine = create_engine('presto://localhost:8080/hive/default')
+    # Trino
+    engine = create_engine('trino://localhost:8080/hive/default')
+    # Hive
+    engine = create_engine('hive://localhost:10000/default')
+    logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
+    print select([func.count('*')], from_obj=logs).scalar()
+
+    # Hive + HTTPS + LDAP or basic Auth
+    engine = create_engine('hive+https://username:password@localhost:10000/')
+    logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
+    print select([func.count('*')], from_obj=logs).scalar()
+
+Note: query generation functionality is not exhaustive or fully tested, but there should be no
+problem with raw SQL.
+
+Passing session configuration
+-----------------------------
+
+.. code-block:: python
+
+    # DB-API
+    hive.connect('localhost', configuration={'hive.exec.reducers.max': '123'})
+    presto.connect('localhost', session_props={'query_max_run_time': '1234m'})
+    trino.connect('localhost',  session_props={'query_max_run_time': '1234m'})
+    # SQLAlchemy
+    create_engine(
+        'presto://user@host:443/hive',
+        connect_args={'protocol': 'https',
+                      'session_props': {'query_max_run_time': '1234m'}}
+    )
+    create_engine(
+        'trino://user@host:443/hive',
+        connect_args={'protocol': 'https',
+                      'session_props': {'query_max_run_time': '1234m'}}
+    )
+    create_engine(
+        'hive://user@host:10000/database',
+        connect_args={'configuration': {'hive.exec.reducers.max': '123'}},
+    )
+    # SQLAlchemy with LDAP
+    create_engine(
+        'hive://user:password@host:10000/database',
+        connect_args={'auth': 'LDAP'},
+    )
+
+Requirements
+============
+
+Install using
+
+- ``pip install 'pyhive[hive]'`` for the Hive interface and
+- ``pip install 'pyhive[presto]'`` for the Presto interface.
+- ``pip install 'pyhive[trino]'`` for the Trino interface
+
+PyHive works with
+
+- Python 2.7 / Python 3
+- For Presto: Presto install
+- For Trino: Trino install
+- For Hive: `HiveServer2 <https://cwiki.apache.org/confluence/display/Hive/Setting+up+HiveServer2>`_ daemon
+
+Changelog
+=========
+See https://github.com/dropbox/PyHive/releases.
+
+Contributing
+============
+- Please fill out the Dropbox Contributor License Agreement at https://opensource.dropbox.com/cla/ and note this in your pull request.
+- Changes must come with tests, with the exception of trivial things like fixing comments. See .travis.yml for the test environment setup.
+- Notes on project scope:
+
+  - This project is intended to be a minimal Hive/Presto client that does that one thing and nothing else.
+    Features that can be implemented on top of PyHive, such integration with your favorite data analysis library, are likely out of scope.
+  - We prefer having a small number of generic features over a large number of specialized, inflexible features.
+    For example, the Presto code takes an arbitrary ``requests_session`` argument for customizing HTTP calls, as opposed to having a separate parameter/branch for each ``requests`` option.
+
+Testing
+=======
+.. image:: https://travis-ci.org/dropbox/PyHive.svg
+    :target: https://travis-ci.org/dropbox/PyHive
+.. image:: http://codecov.io/github/dropbox/PyHive/coverage.svg?branch=master
+    :target: http://codecov.io/github/dropbox/PyHive?branch=master
+
+Run the following in an environment with Hive/Presto::
+
+    ./scripts/make_test_tables.sh
+    virtualenv --no-site-packages env
+    source env/bin/activate
+    pip install -e .
+    pip install -r dev_requirements.txt
+    py.test
+
+WARNING: This drops/creates tables named ``one_row``, ``one_row_complex``, and ``many_rows``, plus a
+database called ``pyhive_test_database``.
+
+Updating TCLIService
+====================
+
+The TCLIService module is autogenerated using a ``TCLIService.thrift`` file. To update it, the
+``generate.py`` file can be used: ``python generate.py <TCLIServiceURL>``. When left blank, the
+version for Hive 2.3 will be downloaded.
```

### Comparing `PyHive-0.6.5/README.rst` & `PyHive-0.7.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/TCLIService/TCLIService.py` & `PyHive-0.7.0.dev0/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/TCLIService/constants.py` & `PyHive-0.7.0.dev0/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/TCLIService/ttypes.py` & `PyHive-0.7.0.dev0/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/pyhive/common.py` & `PyHive-0.7.0.dev0/pyhive/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 import abc
 import collections
 import time
 import datetime
 from future.utils import with_metaclass
 from itertools import islice
 
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+
 
 class DBAPICursor(with_metaclass(abc.ABCMeta, object)):
     """Base class for some common DB-API logic"""
 
     _STATE_NONE = 0
     _STATE_RUNNING = 1
     _STATE_FINISHED = 2
@@ -241,15 +246,15 @@
     def escape_item(self, item):
         if item is None:
             return 'NULL'
         elif isinstance(item, (int, float)):
             return self.escape_number(item)
         elif isinstance(item, basestring):
             return self.escape_string(item)
-        elif isinstance(item, collections.Iterable):
+        elif isinstance(item, Iterable):
             return self.escape_sequence(item)
         elif isinstance(item, datetime.datetime):
             return self.escape_datetime(item, self._DATETIME_FORMAT)
         elif isinstance(item, datetime.date):
             return self.escape_datetime(item, self._DATE_FORMAT)
         else:
             raise exc.ProgrammingError("Unsupported object {}".format(item))
```

### Comparing `PyHive-0.6.5/pyhive/exc.py` & `PyHive-0.7.0.dev0/pyhive/exc.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/pyhive/hive.py` & `PyHive-0.7.0.dev0/pyhive/hive.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/pyhive/presto.py` & `PyHive-0.7.0.dev0/pyhive/presto.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/pyhive/sqlalchemy_hive.py` & `PyHive-0.7.0.dev0/pyhive/sqlalchemy_hive.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,16 +224,16 @@
         if not self._preserve_raw_colnames and '.' in colname:
             return colname.split('.')[-1], colname
         else:
             return colname, None
 
 
 class HiveDialect(default.DefaultDialect):
-    name = b'hive'
-    driver = b'thrift'
+    name = 'hive'
+    driver = 'thrift'
     execution_ctx_cls = HiveExecutionContext
     preparer = HiveIdentifierPreparer
     statement_compiler = HiveCompiler
     supports_views = True
     supports_alter = True
     supports_pk_autoincrement = False
     supports_default_values = False
```

### Comparing `PyHive-0.6.5/pyhive/sqlalchemy_presto.py` & `PyHive-0.7.0.dev0/pyhive/sqlalchemy_presto.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/pyhive/sqlalchemy_trino.py` & `PyHive-0.7.0.dev0/pyhive/sqlalchemy_trino.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/pyhive/trino.py` & `PyHive-0.7.0.dev0/pyhive/trino.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.6.5/setup.cfg` & `PyHive-0.7.0.dev0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [egg_info]
-tag_build = 0.6.5
+tag_build = dev
 tag_date = 0
 
 [tool:pytest]
 timeout = 100
 timeout_method = thread
 addopts = --random --tb=short --cov pyhive --cov-report html --cov-report term --flake8
 norecursedirs = env
```

### Comparing `PyHive-0.6.5/setup.py` & `PyHive-0.7.0.dev0/setup.py`

 * *Files identical despite different names*

