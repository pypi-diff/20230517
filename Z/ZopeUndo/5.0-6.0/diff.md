# Comparing `tmp/ZopeUndo-5.0.tar.gz` & `tmp/ZopeUndo-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZopeUndo-5.0.tar", last modified: Thu Dec  8 07:27:34 2022, max compression
+gzip compressed data, was "ZopeUndo-6.0.tar", last modified: Wed May 17 06:49:33 2023, max compression
```

## Comparing `ZopeUndo-5.0.tar` & `ZopeUndo-6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-08 07:27:34.335744 ZopeUndo-5.0/
--rw-r--r--   0 mac        (513) staff       (20)      786 2022-12-08 07:27:32.000000 ZopeUndo-5.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-12-08 07:27:32.000000 ZopeUndo-5.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-12-08 07:27:32.000000 ZopeUndo-5.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-12-08 07:27:32.000000 ZopeUndo-5.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      196 2022-12-08 07:27:32.000000 ZopeUndo-5.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     2443 2022-12-08 07:27:34.335866 ZopeUndo-5.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      312 2022-12-08 07:27:32.000000 ZopeUndo-5.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      189 2022-12-08 07:27:32.000000 ZopeUndo-5.0/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      417 2022-12-08 07:27:34.336470 ZopeUndo-5.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2521 2022-12-08 07:27:32.000000 ZopeUndo-5.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-08 07:27:34.327409 ZopeUndo-5.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-08 07:27:34.332428 ZopeUndo-5.0/src/ZopeUndo/
--rw-r--r--   0 mac        (513) staff       (20)     1606 2022-12-08 07:27:32.000000 ZopeUndo-5.0/src/ZopeUndo/Prefix.py
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-12-08 07:27:32.000000 ZopeUndo-5.0/src/ZopeUndo/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-08 07:27:34.335508 ZopeUndo-5.0/src/ZopeUndo/tests/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-12-08 07:27:32.000000 ZopeUndo-5.0/src/ZopeUndo/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2037 2022-12-08 07:27:32.000000 ZopeUndo-5.0/src/ZopeUndo/tests/test_prefix.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-08 07:27:34.334779 ZopeUndo-5.0/src/ZopeUndo.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     2443 2022-12-08 07:27:33.000000 ZopeUndo-5.0/src/ZopeUndo.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      443 2022-12-08 07:27:34.000000 ZopeUndo-5.0/src/ZopeUndo.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-12-08 07:27:33.000000 ZopeUndo-5.0/src/ZopeUndo.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-12-08 07:27:33.000000 ZopeUndo-5.0/src/ZopeUndo.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       11 2022-12-08 07:27:34.000000 ZopeUndo-5.0/src/ZopeUndo.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        9 2022-12-08 07:27:34.000000 ZopeUndo-5.0/src/ZopeUndo.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1526 2022-12-08 07:27:32.000000 ZopeUndo-5.0/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-17 06:49:32.999647 ZopeUndo-6.0/
+-rw-r--r--   0 mac        (513) staff       (20)      921 2023-05-17 06:49:32.000000 ZopeUndo-6.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-05-17 06:49:32.000000 ZopeUndo-6.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-05-17 06:49:32.000000 ZopeUndo-6.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-05-17 06:49:32.000000 ZopeUndo-6.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      196 2023-05-17 06:49:32.000000 ZopeUndo-6.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     2249 2023-05-17 06:49:32.999813 ZopeUndo-6.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      312 2023-05-17 06:49:32.000000 ZopeUndo-6.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      189 2023-05-17 06:49:32.000000 ZopeUndo-6.0/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      418 2023-05-17 06:49:33.000418 ZopeUndo-6.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2185 2023-05-17 06:49:32.000000 ZopeUndo-6.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-17 06:49:32.990066 ZopeUndo-6.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-17 06:49:32.994608 ZopeUndo-6.0/src/ZopeUndo/
+-rw-r--r--   0 mac        (513) staff       (20)     1598 2023-05-17 06:49:32.000000 ZopeUndo-6.0/src/ZopeUndo/Prefix.py
+-rw-r--r--   0 mac        (513) staff       (20)        0 2023-05-17 06:49:32.000000 ZopeUndo-6.0/src/ZopeUndo/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-17 06:49:32.999172 ZopeUndo-6.0/src/ZopeUndo/tests/
+-rw-r--r--   0 mac        (513) staff       (20)        0 2023-05-17 06:49:32.000000 ZopeUndo-6.0/src/ZopeUndo/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     2037 2023-05-17 06:49:32.000000 ZopeUndo-6.0/src/ZopeUndo/tests/test_prefix.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-17 06:49:32.998224 ZopeUndo-6.0/src/ZopeUndo.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     2249 2023-05-17 06:49:32.000000 ZopeUndo-6.0/src/ZopeUndo.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      443 2023-05-17 06:49:32.000000 ZopeUndo-6.0/src/ZopeUndo.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-17 06:49:32.000000 ZopeUndo-6.0/src/ZopeUndo.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-17 06:49:32.000000 ZopeUndo-6.0/src/ZopeUndo.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       11 2023-05-17 06:49:32.000000 ZopeUndo-6.0/src/ZopeUndo.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        9 2023-05-17 06:49:32.000000 ZopeUndo-6.0/src/ZopeUndo.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1428 2023-05-17 06:49:32.000000 ZopeUndo-6.0/tox.ini
```

### Comparing `ZopeUndo-5.0/CHANGES.rst` & `ZopeUndo-6.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+6.0 (2023-05-17)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+
 5.0 (2022-12-08)
 ----------------
 
 - Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
 
 - Update PyPy version for Travis.
```

### Comparing `ZopeUndo-5.0/CONTRIBUTING.md` & `ZopeUndo-6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ZopeUndo-5.0/LICENSE.txt` & `ZopeUndo-6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ZopeUndo-5.0/setup.py` & `ZopeUndo-6.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,58 +14,51 @@
 
 import os
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '5.0'
+version = '6.0'
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'README.rst')) as f:
     README = f.read()
 with open(os.path.join(here, 'CHANGES.rst')) as f:
     CHANGES = f.read()
 
 
 setup(
     name='ZopeUndo',
     version=version,
     url='http://pypi.python.org/pypi/ZopeUndo',
     license='ZPL 2.1',
-    description="ZODB undo support for Zope2.",
+    description="ZODB undo support for Zope.",
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     long_description=README + '\n\n' + CHANGES,
     packages=find_packages('src'),
     package_dir={'': 'src'},
     classifiers=[
         "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
-        "Framework :: Zope :: 2",
-        "Framework :: Zope :: 4",
         "Framework :: Zope :: 5",
         "License :: OSI Approved :: Zope Public License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
+    python_requires='>=3.7',
     keywords="zope zope4 undo",
     install_requires=[
         'setuptools',
     ],
-    test_suite='ZopeUndo.tests',
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `ZopeUndo-5.0/src/ZopeUndo/Prefix.py` & `ZopeUndo-6.0/src/ZopeUndo/Prefix.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 
 
-class Prefix(object):
+class Prefix:
     """A Prefix() is equal to any path it is a prefix of.
 
     This class can be compared to a string.
     The comparison will return True if all path elements of the
     Prefix are found at the beginning of the string being compared.
 
     Two Prefixes can not be compared.
```

### Comparing `ZopeUndo-5.0/src/ZopeUndo/tests/test_prefix.py` & `ZopeUndo-6.0/src/ZopeUndo/tests/test_prefix.py`

 * *Files identical despite different names*

