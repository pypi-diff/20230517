# Comparing `tmp/zodburi-2.5.0.tar.gz` & `tmp/zodburi-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodburi-2.5.0.tar", last modified: Wed May 12 11:24:33 2021, max compression
+gzip compressed data, was "zodburi-2.6.0.tar", last modified: Wed May 17 08:08:40 2023, max compression
```

## Comparing `zodburi-2.5.0.tar` & `zodburi-2.6.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 kirr      (1000) kirr      (1000)        0 2021-05-12 11:24:33.236387 zodburi-2.5.0/
--rw-r--r--   0 kirr      (1000) kirr      (1000)     2612 2021-05-12 11:23:23.000000 zodburi-2.5.0/CHANGES.rst
--rw-r--r--   0 kirr      (1000) kirr      (1000)     4751 2020-11-15 20:26:47.000000 zodburi-2.5.0/CONTRIBUTORS.txt
--rw-r--r--   0 kirr      (1000) kirr      (1000)      111 2020-11-15 20:26:47.000000 zodburi-2.5.0/COPYRIGHT.txt
--rw-r--r--   0 kirr      (1000) kirr      (1000)     1719 2017-04-02 14:32:32.000000 zodburi-2.5.0/LICENSE.txt
--rw-r--r--   0 kirr      (1000) kirr      (1000)      264 2021-05-12 11:19:54.000000 zodburi-2.5.0/MANIFEST.in
--rw-r--r--   0 kirr      (1000) kirr      (1000)     4802 2021-05-12 11:24:33.236387 zodburi-2.5.0/PKG-INFO
--rw-r--r--   0 kirr      (1000) kirr      (1000)      227 2020-11-15 20:26:47.000000 zodburi-2.5.0/README.rst
--rw-r--r--   0 kirr      (1000) kirr      (1000)      773 2021-05-12 11:19:54.000000 zodburi-2.5.0/RELEASING.txt
--rw-r--r--   0 kirr      (1000) kirr      (1000)     1591 2020-11-15 20:26:47.000000 zodburi-2.5.0/contributing.md
-drwxr-xr-x   0 kirr      (1000) kirr      (1000)        0 2021-05-12 11:24:33.228387 zodburi-2.5.0/docs/
--rw-r--r--   0 kirr      (1000) kirr      (1000)     2697 2017-04-02 14:32:32.000000 zodburi-2.5.0/docs/Makefile
--rw-r--r--   0 kirr      (1000) kirr      (1000)      114 2017-04-02 14:32:32.000000 zodburi-2.5.0/docs/api.rst
--rw-r--r--   0 kirr      (1000) kirr      (1000)     6286 2020-11-15 20:26:47.000000 zodburi-2.5.0/docs/conf.py
--rw-r--r--   0 kirr      (1000) kirr      (1000)     9400 2021-05-10 09:36:28.000000 zodburi-2.5.0/docs/index.rst
--rw-r--r--   0 kirr      (1000) kirr      (1000)       10 2017-04-19 07:58:48.000000 zodburi-2.5.0/rtd.txt
--rw-r--r--   0 kirr      (1000) kirr      (1000)      263 2021-05-12 11:24:33.236387 zodburi-2.5.0/setup.cfg
--rw-r--r--   0 kirr      (1000) kirr      (1000)     2270 2021-05-12 11:23:23.000000 zodburi-2.5.0/setup.py
--rw-r--r--   0 kirr      (1000) kirr      (1000)     1442 2021-05-12 11:19:54.000000 zodburi-2.5.0/tox.ini
-drwxr-xr-x   0 kirr      (1000) kirr      (1000)        0 2021-05-12 11:24:33.232387 zodburi-2.5.0/zodburi/
--rw-r--r--   0 kirr      (1000) kirr      (1000)     2139 2021-05-10 09:36:28.000000 zodburi-2.5.0/zodburi/__init__.py
--rw-r--r--   0 kirr      (1000) kirr      (1000)      338 2020-11-15 20:26:47.000000 zodburi-2.5.0/zodburi/_compat.py
--rw-r--r--   0 kirr      (1000) kirr      (1000)     1387 2017-04-02 14:32:32.000000 zodburi-2.5.0/zodburi/datatypes.py
--rw-r--r--   0 kirr      (1000) kirr      (1000)     8615 2021-05-10 09:36:28.000000 zodburi-2.5.0/zodburi/resolvers.py
-drwxr-xr-x   0 kirr      (1000) kirr      (1000)        0 2021-05-12 11:24:33.236387 zodburi-2.5.0/zodburi/tests/
--rw-r--r--   0 kirr      (1000) kirr      (1000)     1636 2017-04-19 07:58:48.000000 zodburi-2.5.0/zodburi/tests/__init__.py
--rw-r--r--   0 kirr      (1000) kirr      (1000)     3061 2017-04-02 14:32:32.000000 zodburi-2.5.0/zodburi/tests/test_datatypes.py
--rw-r--r--   0 kirr      (1000) kirr      (1000)    26186 2021-05-10 09:36:28.000000 zodburi-2.5.0/zodburi/tests/test_resolvers.py
-drwxr-xr-x   0 kirr      (1000) kirr      (1000)        0 2021-05-12 11:24:33.232387 zodburi-2.5.0/zodburi.egg-info/
--rw-r--r--   0 kirr      (1000) kirr      (1000)     4802 2021-05-12 11:24:33.000000 zodburi-2.5.0/zodburi.egg-info/PKG-INFO
--rw-r--r--   0 kirr      (1000) kirr      (1000)      586 2021-05-12 11:24:33.000000 zodburi-2.5.0/zodburi.egg-info/SOURCES.txt
--rw-r--r--   0 kirr      (1000) kirr      (1000)        1 2021-05-12 11:24:33.000000 zodburi-2.5.0/zodburi.egg-info/dependency_links.txt
--rw-r--r--   0 kirr      (1000) kirr      (1000)      301 2021-05-12 11:24:33.000000 zodburi-2.5.0/zodburi.egg-info/entry_points.txt
--rw-r--r--   0 kirr      (1000) kirr      (1000)        1 2021-05-12 11:24:33.000000 zodburi-2.5.0/zodburi.egg-info/not-zip-safe
--rw-r--r--   0 kirr      (1000) kirr      (1000)      165 2021-05-12 11:24:33.000000 zodburi-2.5.0/zodburi.egg-info/requires.txt
--rw-r--r--   0 kirr      (1000) kirr      (1000)        8 2021-05-12 11:24:33.000000 zodburi-2.5.0/zodburi.egg-info/top_level.txt
+drwxr-xr-x   0 azmeuk    (1000) azmeuk    (1000)        0 2023-05-17 08:08:40.386383 zodburi-2.6.0/
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     2709 2023-05-17 08:07:17.000000 zodburi-2.6.0/CHANGES.rst
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     4751 2023-02-15 08:43:35.000000 zodburi-2.6.0/CONTRIBUTORS.txt
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)      111 2023-02-15 08:43:35.000000 zodburi-2.6.0/COPYRIGHT.txt
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     1719 2023-02-15 08:43:35.000000 zodburi-2.6.0/LICENSE.txt
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)      264 2023-02-15 08:43:35.000000 zodburi-2.6.0/MANIFEST.in
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     3872 2023-05-17 08:08:40.386383 zodburi-2.6.0/PKG-INFO
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)      227 2023-02-15 08:43:35.000000 zodburi-2.6.0/README.rst
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     1591 2023-02-15 08:43:35.000000 zodburi-2.6.0/contributing.md
+drwxr-xr-x   0 azmeuk    (1000) azmeuk    (1000)        0 2023-05-17 08:08:40.386383 zodburi-2.6.0/docs/
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     2697 2023-02-15 08:43:35.000000 zodburi-2.6.0/docs/Makefile
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)      114 2023-02-15 08:43:35.000000 zodburi-2.6.0/docs/api.rst
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     6262 2023-02-15 09:09:08.000000 zodburi-2.6.0/docs/conf.py
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     9374 2023-02-15 09:09:08.000000 zodburi-2.6.0/docs/index.rst
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)       10 2023-02-15 08:43:35.000000 zodburi-2.6.0/rtd.txt
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)      263 2023-05-17 08:08:40.389717 zodburi-2.6.0/setup.cfg
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     2225 2023-05-17 08:07:32.000000 zodburi-2.6.0/setup.py
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     1350 2023-02-15 09:09:08.000000 zodburi-2.6.0/tox.ini
+drwxr-xr-x   0 azmeuk    (1000) azmeuk    (1000)        0 2023-05-17 08:08:40.386383 zodburi-2.6.0/zodburi/
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     2140 2023-02-15 09:09:08.000000 zodburi-2.6.0/zodburi/__init__.py
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)      338 2023-02-15 08:43:35.000000 zodburi-2.6.0/zodburi/_compat.py
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     1387 2023-02-15 08:43:35.000000 zodburi-2.6.0/zodburi/datatypes.py
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     8144 2023-02-15 09:09:08.000000 zodburi-2.6.0/zodburi/resolvers.py
+drwxr-xr-x   0 azmeuk    (1000) azmeuk    (1000)        0 2023-05-17 08:08:40.386383 zodburi-2.6.0/zodburi/tests/
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     1650 2023-02-15 09:09:08.000000 zodburi-2.6.0/zodburi/tests/__init__.py
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     3061 2023-02-15 08:43:35.000000 zodburi-2.6.0/zodburi/tests/test_datatypes.py
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)    24321 2023-02-15 09:09:08.000000 zodburi-2.6.0/zodburi/tests/test_resolvers.py
+drwxr-xr-x   0 azmeuk    (1000) azmeuk    (1000)        0 2023-05-17 08:08:40.386383 zodburi-2.6.0/zodburi.egg-info/
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)     3872 2023-05-17 08:08:40.000000 zodburi-2.6.0/zodburi.egg-info/PKG-INFO
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)      572 2023-05-17 08:08:40.000000 zodburi-2.6.0/zodburi.egg-info/SOURCES.txt
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)        1 2023-05-17 08:08:40.000000 zodburi-2.6.0/zodburi.egg-info/dependency_links.txt
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)      259 2023-05-17 08:08:40.000000 zodburi-2.6.0/zodburi.egg-info/entry_points.txt
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)        1 2023-02-15 08:47:02.000000 zodburi-2.6.0/zodburi.egg-info/not-zip-safe
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)      165 2023-05-17 08:08:40.000000 zodburi-2.6.0/zodburi.egg-info/requires.txt
+-rw-r--r--   0 azmeuk    (1000) azmeuk    (1000)        8 2023-05-17 08:08:40.000000 zodburi-2.6.0/zodburi.egg-info/top_level.txt
```

### Comparing `zodburi-2.5.0/CHANGES.rst` & `zodburi-2.6.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 .. _change-log:
 
 Change Log
 ----------
 
+2.6.0 (2023-05-17)
+~~~~~~~~~~~~~~~~~~
+
+- Stop support for ZODB4
+
+- Stop support for python<3.7
+
+
 2.5.0 (2021-05-12)
 ~~~~~~~~~~~~~~~~~~
 
 - Support both ZODB4 and ZODB5.
 
 - Add support for PyPy.
```

### Comparing `zodburi-2.5.0/CONTRIBUTORS.txt` & `zodburi-2.6.0/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `zodburi-2.5.0/LICENSE.txt` & `zodburi-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zodburi-2.5.0/contributing.md` & `zodburi-2.6.0/contributing.md`

 * *Files identical despite different names*

### Comparing `zodburi-2.5.0/docs/Makefile` & `zodburi-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zodburi-2.5.0/docs/conf.py` & `zodburi-2.6.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # zodburi documentation build configuration file
 #
 # This file is execfile()d with the current directory set to its containing
 # dir.
 #
 # The contents of this file are pickled, so don't put values in the
```

### Comparing `zodburi-2.5.0/docs/index.rst` & `zodburi-2.6.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 Overview
 --------
 
 A library which parses URIs and converts them to ZODB storage objects and
 database arguments.
 
-It will run under CPython 2.7, 3.5 to 3.8, pypy and pypy3.  It will not run under Jython.  It requires ZODB >= 3.10.0.
+It will run under CPython 3.7+ and pypy3.  It will not run under Jython.  It requires ZODB >= 5.0.0.
 
 Installation
 ------------
 
-Install using setuptools, e.g. (within a virtualenv)::
+Install using pip, e.g. (within a virtualenv)::
 
-  $ easy_install zodburi
+  $ pip install zodburi
 
 Using
 -----
 
 ``zodburi`` has exactly one api: :func:`zodburi.resolve_uri`.  This API
 obtains a ZODB storage factory and a set of keyword arguments suitable for
 passing to the ``ZODB.DB.DB`` constructor.  For example:
```

### Comparing `zodburi-2.5.0/setup.py` & `zodburi-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,46 +4,45 @@
 from setuptools import find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 try:
     with open(os.path.join(here, 'README.rst')) as f:
         README = f.read()
-except IOError:
+except OSError:
     README = ''
 
 try:
     with open(os.path.join(here, 'CHANGES.rst')) as f:
         CHANGES = f.read()
-except IOError:
+except OSError:
     CHANGES = ''
 
 requires = ['ZODB', 'ZConfig', 'ZEO']
 tests_require = requires + ['mock']
 testing_extras = tests_require + ['nose', 'coverage']
 docs_extras = tests_require + [
     'Sphinx >= 1.8.1',
     'repoze.sphinx.autointerface',
     'pylons-sphinx-themes >= 1.0.10',
 ]
 
 setup(name='zodburi',
-      version='2.5.0',
+      version='2.6.0',
       description=('Construct ZODB storage instances from URIs.'),
       long_description=README + '\n\n' +  CHANGES,
       classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "License :: Repoze Public License",
         ],
       keywords='zodb zodbconn',
       author="Chris Rossi",
       author_email="pylons-discuss@googlegroups.com",
```

### Comparing `zodburi-2.5.0/tox.ini` & `zodburi-2.6.0/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 [tox]
 envlist =
-    {py27,py35,py36,pypy,pypy3}-{zodb4,zodb5},
-    {py37,py38}-zodb5,
-    cover,docs,lint
+    py37,py38,py39,py310,py311,pypy3,cover,docs,lint
 
 [testenv]
 commands =
     python setup.py -q test -q
 deps =
     mock
-    zodb4: ZODB==4.*
-    zodb5: ZODB==5.*
-    zodb4: ZEO==4.*
-    zodb5: ZEO==5.*
+    ZODB==5.*
+    ZEO==5.*
 
 [testenv:cover]
 basepython =
-    python3.7
+    python3.9
 commands =
     python setup.py nosetests --with-xunit --with-xcoverage
 deps =
     {[testenv]deps}
     nose
     coverage
     nosexcover
@@ -29,22 +25,21 @@
 # cobertura jenkins reporting and b) pypy and jython can't handle any
 # combination of versions of coverage and nosexcover that i can find.
 # coverage==3.4 is required by nosexcover.
 
 
 [testenv:docs]
 basepython =
-    python3.7
+    python3.11
 commands =
     sphinx-build -b html -d docs/_build/doctrees docs docs/_build/html
 deps =
     Sphinx
     pylons-sphinx-themes
 
-
 [testenv:lint]
 skip_install = true
 commands =
     check-manifest
 deps =
     check-manifest
```

### Comparing `zodburi-2.5.0/zodburi/__init__.py` & `zodburi-2.6.0/zodburi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 bytes_parameters = (
     'cache_size_bytes', 'historical_cache_size_bytes', 'large_record_size')
 
 parameters = dict(database_name = 'database_name')
 for parameter in connection_parameters:
     parameters['connection_' + parameter] = parameter
 
-has_units = re.compile('\s*(\d+)\s*([kmg])b\s*$').match
+has_units = re.compile(r'\s*(\d+)\s*([kmg])b\s*$').match
 units = dict(k=1<<10, m=1<<20, g=1<<30)
 def _parse_bytes(s):
     m = has_units(s.lower())
     if m:
         v, uname = m.group(1, 2)
         return int(v) * units[uname]
     else:
```

### Comparing `zodburi-2.5.0/zodburi/datatypes.py` & `zodburi-2.6.0/zodburi/datatypes.py`

 * *Files identical despite different names*

### Comparing `zodburi-2.5.0/zodburi/resolvers.py` & `zodburi-2.6.0/zodburi/resolvers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from io import BytesIO
 import os
 import re
 
 from ZConfig import loadConfig
 from ZConfig import loadSchemaFile
 from ZEO.ClientStorage import ClientStorage
@@ -15,19 +14,16 @@
 from zodburi.datatypes import convert_bytesize
 from zodburi.datatypes import convert_int
 from zodburi.datatypes import convert_tuple
 from zodburi._compat import parse_qsl
 from zodburi._compat import urlsplit
 from zodburi import _resolve_uri
 
-# Capability test for older Pythons (2.x < 2.7.4, 3.x < 3.2.4)
-(scheme, netloc, path, query, frag) = urlsplit('scheme:///path/#frag')
-_BROKEN_URLSPLIT = frag != 'frag'
 
-class Resolver(object):
+class Resolver:
     _int_args = ()
     _string_args = ()
     _bytesize_args = ()
     _float_args = ()
     _tuple_args = ()
 
     def interpret_kwargs(self, kw):
@@ -157,31 +153,26 @@
                 return DemoStorage(base=ClientStorage(*args, **kw))
         else:
             def factory():
                 return ClientStorage(*args, **kw)
         return factory, unused
 
 
-class ZConfigURIResolver(object):
+class ZConfigURIResolver:
 
     schema_xml_template = b"""
     <schema>
         <import package="ZODB"/>
         <multisection type="ZODB.storage" attribute="storages" />
         <multisection type="ZODB.database" attribute="databases" />
     </schema>
     """
 
     def __call__(self, uri):
         (scheme, netloc, path, query, frag) = urlsplit(uri)
-        if _BROKEN_URLSPLIT: #pragma NO COVER
-            # urlsplit used not to allow fragments in non-standard schemes,
-            # stuffed everything into 'path'
-            (scheme, netloc, path, query, frag
-            ) = urlsplit('http:' + path)
         path = os.path.normpath(path)
         schema_xml = self.schema_xml_template
         schema = loadSchemaFile(BytesIO(schema_xml))
         config, handler = loadConfig(schema, path)
         for config_item in config.databases + config.storages:
             if not frag:
                 # use the first defined in the file
@@ -204,15 +195,15 @@
         else:
             factory = config_item
             dbkw = dict(parse_qsl(query))
 
         return factory.open, dbkw
 
 
-class DemoStorageURIResolver(object):
+class DemoStorageURIResolver:
 
     # demo:(base_uri)/(δ_uri)#dbkw...
     # URI format follows XRI Cross-references to refer to base and δ
     # (see https://en.wikipedia.org/wiki/Extensible_Resource_Identifier)
     _uri_re = re.compile(r'^demo:\((?P<base>.*)\)/\((?P<changes>.*)\)(?P<frag>#.*)?$')
 
     def __call__(self, uri):
```

### Comparing `zodburi-2.5.0/zodburi/tests/__init__.py` & `zodburi-2.6.0/zodburi/tests/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import mock
+from unittest import mock
 import unittest
 
 
 class TestResolveURI(unittest.TestCase):
 
     @mock.patch('zodburi.resolvers.MappingStorage')
     def test_it(self, MappingStorage):
```

### Comparing `zodburi-2.5.0/zodburi/tests/test_datatypes.py` & `zodburi-2.6.0/zodburi/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `zodburi-2.5.0/zodburi/tests/test_resolvers.py` & `zodburi-2.6.0/zodburi/tests/test_resolvers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import mock
+from unittest import mock
 import pkg_resources
 import unittest
 
 
-ZODB_VERSION = tuple(map(int, pkg_resources.get_distribution("ZODB").version.split('.')))
-
-
 class Base:
 
     def test_interpret_kwargs_noargs(self):
         resolver = self._makeOne()
         kwargs = resolver.interpret_kwargs({})
         self.assertEqual(kwargs, ({}, {}))
 
@@ -207,16 +204,16 @@
             self.assertTrue(os.path.exists(BLOB_DIR))
         finally:
             storage.close()
 
     def test_dbargs(self):
         resolver = self._makeOne()
         factory, dbkw = resolver(
-            ('file:///tmp/../foo/bar?connection_pool_size=1'
-             '&connection_cache_size=1&database_name=dbname'))
+            'file:///tmp/../foo/bar?connection_pool_size=1'
+             '&connection_cache_size=1&database_name=dbname')
         self.assertEqual(dbkw, {'connection_cache_size': '1',
                                 'connection_pool_size': '1',
                                 'database_name': 'dbname'})
 
 
 class TestClientStorageURIResolver(unittest.TestCase):
     def _getTargetClass(self):
@@ -438,33 +435,23 @@
         """)
         self.tmp.flush()
         resolver = self._makeOne()
         factory, dbkw = resolver('zconfig://%s' % self.tmp.name)
         storage = factory()
         from ZODB.MappingStorage import MappingStorage
         self.assertTrue(isinstance(storage, MappingStorage))
-        if ZODB_VERSION[0] < 5:
-            self.assertEqual(dbkw,
-                             {'connection_cache_size': 5000,
-                              'connection_cache_size_bytes': 0,
-                              'connection_historical_cache_size': 1000,
-                              'connection_historical_cache_size_bytes': 0,
-                              'connection_historical_pool_size': 3,
-                              'connection_historical_timeout': 300,
-                              'connection_pool_size': 7})
-        else:
-            self.assertEqual(dbkw,
-                             {'connection_cache_size': 5000,
-                              'connection_cache_size_bytes': 0,
-                              'connection_historical_cache_size': 1000,
-                              'connection_historical_cache_size_bytes': 0,
-                              'connection_historical_pool_size': 3,
-                              'connection_historical_timeout': 300,
-                              'connection_large_record_size': 16777216,
-                              'connection_pool_size': 7})
+        self.assertEqual(dbkw,
+                         {'connection_cache_size': 5000,
+                          'connection_cache_size_bytes': 0,
+                          'connection_historical_cache_size': 1000,
+                          'connection_historical_cache_size_bytes': 0,
+                          'connection_historical_pool_size': 3,
+                          'connection_historical_timeout': 300,
+                          'connection_large_record_size': 16777216,
+                          'connection_pool_size': 7})
 
 
     def test_named_database(self):
         self.tmp.write(b"""
         <zodb x>
           <mappingstorage>
           </mappingstorage>
@@ -475,47 +462,36 @@
         """)
         self.tmp.flush()
         resolver = self._makeOne()
         factory, dbkw = resolver('zconfig://%s#x' % self.tmp.name)
         storage = factory()
         from ZODB.MappingStorage import MappingStorage
         self.assertTrue(isinstance(storage, MappingStorage))
-        if ZODB_VERSION[0] < 5:
-            self.assertEqual(dbkw,
-                             {'connection_cache_size': 20000,
-                              'connection_cache_size_bytes': 0,
-                              'connection_historical_cache_size': 1000,
-                              'connection_historical_cache_size_bytes': 0,
-                              'connection_historical_pool_size': 3,
-                              'connection_historical_timeout': 300,
-                              'connection_pool_size': 5,
-                              'database_name': 'foo'})
-        else:
-            self.assertEqual(dbkw,
-                             {'connection_cache_size': 20000,
-                              'connection_cache_size_bytes': 0,
-                              'connection_historical_cache_size': 1000,
-                              'connection_historical_cache_size_bytes': 0,
-                              'connection_historical_pool_size': 3,
-                              'connection_historical_timeout': 300,
-                              'connection_large_record_size': 16777216,
-                              'connection_pool_size': 5,
-                              'database_name': 'foo'})
+        self.assertEqual(dbkw,
+                         {'connection_cache_size': 20000,
+                          'connection_cache_size_bytes': 0,
+                          'connection_historical_cache_size': 1000,
+                          'connection_historical_cache_size_bytes': 0,
+                          'connection_historical_pool_size': 3,
+                          'connection_historical_timeout': 300,
+                          'connection_large_record_size': 16777216,
+                          'connection_pool_size': 5,
+                          'database_name': 'foo'})
 
 
     def test_database_all_options(self):
         from zodburi import connection_parameters, bytes_parameters
         self.tmp.write(("""
         <zodb x>
           <mappingstorage>
           </mappingstorage>
           database-name foo
           %s
         </zodb>
-        """ % '\n'.join("%s %s" % (
+        """ % '\n'.join("{} {}".format(
                             name.replace('_', '-'),
                             '%sMB' % i if name in bytes_parameters else i,
                            )
                         for (i, name)
                         in enumerate(connection_parameters)
                         )).encode())
         self.tmp.flush()
@@ -542,35 +518,24 @@
         """)
         self.tmp.flush()
         from zodburi import resolve_uri
         factory, dbkw = resolve_uri('zconfig://%s' % self.tmp.name)
         storage = factory()
         from ZODB.MappingStorage import MappingStorage
         self.assertTrue(isinstance(storage, MappingStorage))
-        if ZODB_VERSION[0] < 5:
-            self.assertEqual(dbkw,
-                             {'cache_size': 5000,
-                              'cache_size_bytes': 0,
-                              'historical_cache_size': 1000,
-                              'historical_cache_size_bytes': 0,
-                              'historical_pool_size': 3,
-                              'historical_timeout': 300,
-                              'pool_size': 7,
-                              'database_name': 'unnamed'})
-        else:
-            self.assertEqual(dbkw,
-                             {'cache_size': 5000,
-                              'cache_size_bytes': 0,
-                              'historical_cache_size': 1000,
-                              'historical_cache_size_bytes': 0,
-                              'historical_pool_size': 3,
-                              'historical_timeout': 300,
-                              'large_record_size': 16777216,
-                              'pool_size': 7,
-                              'database_name': 'unnamed'})
+        self.assertEqual(dbkw,
+                         {'cache_size': 5000,
+                          'cache_size_bytes': 0,
+                          'historical_cache_size': 1000,
+                          'historical_cache_size_bytes': 0,
+                          'historical_pool_size': 3,
+                          'historical_timeout': 300,
+                          'large_record_size': 16777216,
+                          'pool_size': 7,
+                          'database_name': 'unnamed'})
 
 
 class TestMappingStorageURIResolver(Base, unittest.TestCase):
 
     def _getTargetClass(self):
         from zodburi.resolvers import MappingStorageURIResolver
         return MappingStorageURIResolver
@@ -618,15 +583,15 @@
         self.addCleanup(_)
 
         resolver = self._makeOne()
         basef   = os.path.join(tmpdir, 'base.fs')
         changef = os.path.join(tmpdir, 'changes.fs')
         self.assertFalse(os.path.exists(basef))
         self.assertFalse(os.path.exists(changef))
-        factory, dbkw = resolver('demo:(file://%s)/(file://%s?quota=200)' % (basef, changef))
+        factory, dbkw = resolver('demo:(file://{})/(file://{}?quota=200)'.format(basef, changef))
         self.assertEqual(dbkw, {})
         demo = factory()
         from ZODB.DemoStorage import DemoStorage
         from ZODB.FileStorage import FileStorage
         self.assertTrue(isinstance(demo, DemoStorage))
         self.assertTrue(isinstance(demo.base, FileStorage))
         self.assertTrue(isinstance(demo.changes, FileStorage))
```

### Comparing `zodburi-2.5.0/zodburi.egg-info/SOURCES.txt` & `zodburi-2.6.0/zodburi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 CHANGES.rst
 CONTRIBUTORS.txt
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-RELEASING.txt
 contributing.md
 rtd.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/api.rst
```

