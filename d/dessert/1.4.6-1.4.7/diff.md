# Comparing `tmp/dessert-1.4.6.tar.gz` & `tmp/dessert-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dessert-1.4.6.tar", last modified: Fri Feb 17 19:41:50 2023, max compression
+gzip compressed data, was "dessert-1.4.7.tar", last modified: Wed May 17 10:19:51 2023, max compression
```

## Comparing `dessert-1.4.6.tar` & `dessert-1.4.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-02-17 19:41:50.285518 dessert-1.4.6/
--rw-r--r--   0 rotemy     (501) staff       (20)      227 2022-03-23 12:20:01.000000 dessert-1.4.6/.coveragerc
--rw-r--r--   0 rotemy     (501) staff       (20)       25 2022-03-23 12:20:01.000000 dessert-1.4.6/.gitattributes
-drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-02-17 19:41:50.280679 dessert-1.4.6/.github/
-drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-02-17 19:41:50.282758 dessert-1.4.6/.github/workflows/
--rw-r--r--   0 rotemy     (501) staff       (20)      824 2022-08-02 14:46:21.000000 dessert-1.4.6/.github/workflows/test.yml
--rw-r--r--   0 rotemy     (501) staff       (20)    11549 2023-02-17 19:41:50.000000 dessert-1.4.6/AUTHORS
--rw-r--r--   0 rotemy     (501) staff       (20)   354413 2023-02-17 19:41:50.000000 dessert-1.4.6/ChangeLog
--rw-r--r--   0 rotemy     (501) staff       (20)     1012 2022-03-23 12:20:01.000000 dessert-1.4.6/DEVELOPMENT.md
--rw-r--r--   0 rotemy     (501) staff       (20)     1061 2022-03-23 12:20:01.000000 dessert-1.4.6/LICENSE
--rw-r--r--   0 rotemy     (501) staff       (20)       51 2022-03-23 12:20:01.000000 dessert-1.4.6/MANIFEST.in
--rw-r--r--   0 rotemy     (501) staff       (20)      265 2023-02-14 19:46:06.000000 dessert-1.4.6/Makefile
--rw-r--r--   0 rotemy     (501) staff       (20)     2199 2023-02-17 19:41:50.285647 dessert-1.4.6/PKG-INFO
--rw-r--r--   0 rotemy     (501) staff       (20)     1206 2023-02-14 19:46:06.000000 dessert-1.4.6/README.md
-drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-02-17 19:41:50.283623 dessert-1.4.6/dessert/
--rw-r--r--   0 rotemy     (501) staff       (20)      467 2022-08-02 13:57:50.000000 dessert-1.4.6/dessert/__init__.py
--rw-r--r--   0 rotemy     (501) staff       (20)       86 2022-03-23 12:20:06.000000 dessert-1.4.6/dessert/__version__.py
--rw-r--r--   0 rotemy     (501) staff       (20)      345 2022-03-23 12:20:06.000000 dessert-1.4.6/dessert/conf.py
--rw-r--r--   0 rotemy     (501) staff       (20)     1624 2022-03-23 12:20:06.000000 dessert-1.4.6/dessert/pathlib.py
--rw-r--r--   0 rotemy     (501) staff       (20)    38821 2023-02-17 19:41:30.000000 dessert-1.4.6/dessert/rewrite.py
--rw-r--r--   0 rotemy     (501) staff       (20)     1945 2022-03-23 12:20:06.000000 dessert-1.4.6/dessert/saferepr.py
--rw-r--r--   0 rotemy     (501) staff       (20)    14757 2022-03-23 12:20:06.000000 dessert-1.4.6/dessert/util.py
--rw-r--r--   0 rotemy     (501) staff       (20)      160 2022-03-23 12:20:06.000000 dessert-1.4.6/dessert/warning_types.py
-drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-02-17 19:41:50.284334 dessert-1.4.6/dessert.egg-info/
--rw-r--r--   0 rotemy     (501) staff       (20)     2199 2023-02-17 19:41:50.000000 dessert-1.4.6/dessert.egg-info/PKG-INFO
--rw-r--r--   0 rotemy     (501) staff       (20)      756 2023-02-17 19:41:50.000000 dessert-1.4.6/dessert.egg-info/SOURCES.txt
--rw-r--r--   0 rotemy     (501) staff       (20)        1 2023-02-17 19:41:50.000000 dessert-1.4.6/dessert.egg-info/dependency_links.txt
--rw-r--r--   0 rotemy     (501) staff       (20)        1 2023-02-17 19:41:50.000000 dessert-1.4.6/dessert.egg-info/not-zip-safe
--rw-r--r--   0 rotemy     (501) staff       (20)       47 2023-02-17 19:41:50.000000 dessert-1.4.6/dessert.egg-info/pbr.json
--rw-r--r--   0 rotemy     (501) staff       (20)       65 2023-02-17 19:41:50.000000 dessert-1.4.6/dessert.egg-info/requires.txt
--rw-r--r--   0 rotemy     (501) staff       (20)        8 2023-02-17 19:41:50.000000 dessert-1.4.6/dessert.egg-info/top_level.txt
--rw-r--r--   0 rotemy     (501) staff       (20)       33 2022-03-23 12:20:01.000000 dessert-1.4.6/requirements.txt
-drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-02-17 19:41:50.284647 dessert-1.4.6/scripts/
--rw-r--r--   0 rotemy     (501) staff       (20)      246 2022-03-23 12:20:02.000000 dessert-1.4.6/scripts/call-tox.bat
--rw-r--r--   0 rotemy     (501) staff       (20)      546 2022-03-23 12:20:02.000000 dessert-1.4.6/scripts/check-manifest.py
--rw-r--r--   0 rotemy     (501) staff       (20)      322 2022-03-23 12:20:02.000000 dessert-1.4.6/scripts/install-pypy.bat
--rw-r--r--   0 rotemy     (501) staff       (20)      625 2023-02-17 19:41:50.286003 dessert-1.4.6/setup.cfg
--rw-r--r--   0 rotemy     (501) staff       (20)      224 2023-02-14 19:46:06.000000 dessert-1.4.6/setup.py
-drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-02-17 19:41:50.285412 dessert-1.4.6/tests/
--rw-r--r--   0 rotemy     (501) staff       (20)       94 2022-03-23 12:20:06.000000 dessert-1.4.6/tests/__init__.py
--rw-r--r--   0 rotemy     (501) staff       (20)       28 2022-03-23 12:20:06.000000 dessert-1.4.6/tests/conftest.py
--rw-r--r--   0 rotemy     (501) staff       (20)      377 2022-03-23 12:20:06.000000 dessert-1.4.6/tests/driver.py
--rw-r--r--   0 rotemy     (501) staff       (20)      181 2022-03-23 12:20:06.000000 dessert-1.4.6/tests/examples.py
--rw-r--r--   0 rotemy     (501) staff       (20)     3620 2023-02-14 19:46:06.000000 dessert-1.4.6/tests/test_dessert.py
--rw-r--r--   0 rotemy     (501) staff       (20)      889 2022-03-23 12:20:06.000000 dessert-1.4.6/tests/test_integration.py
--rw-r--r--   0 rotemy     (501) staff       (20)      579 2022-03-23 12:20:06.000000 dessert-1.4.6/tests/test_readme_doctest.py
--rw-r--r--   0 rotemy     (501) staff       (20)      121 2022-03-23 12:20:01.000000 dessert-1.4.6/tox.ini
+drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-05-17 10:19:51.971242 dessert-1.4.7/
+-rw-r--r--   0 rotemy     (501) staff       (20)      227 2022-03-23 12:20:01.000000 dessert-1.4.7/.coveragerc
+-rw-r--r--   0 rotemy     (501) staff       (20)       25 2022-03-23 12:20:01.000000 dessert-1.4.7/.gitattributes
+drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-05-17 10:19:51.964745 dessert-1.4.7/.github/
+drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-05-17 10:19:51.967200 dessert-1.4.7/.github/workflows/
+-rw-r--r--   0 rotemy     (501) staff       (20)      832 2023-05-17 10:19:09.000000 dessert-1.4.7/.github/workflows/test.yml
+-rw-r--r--   0 rotemy     (501) staff       (20)    11585 2023-05-17 10:19:51.000000 dessert-1.4.7/AUTHORS
+-rw-r--r--   0 rotemy     (501) staff       (20)   354522 2023-05-17 10:19:51.000000 dessert-1.4.7/ChangeLog
+-rw-r--r--   0 rotemy     (501) staff       (20)     1012 2022-03-23 12:20:01.000000 dessert-1.4.7/DEVELOPMENT.md
+-rw-r--r--   0 rotemy     (501) staff       (20)     1061 2022-03-23 12:20:01.000000 dessert-1.4.7/LICENSE
+-rw-r--r--   0 rotemy     (501) staff       (20)       51 2022-03-23 12:20:01.000000 dessert-1.4.7/MANIFEST.in
+-rw-r--r--   0 rotemy     (501) staff       (20)      265 2023-02-14 19:46:06.000000 dessert-1.4.7/Makefile
+-rw-r--r--   0 rotemy     (501) staff       (20)     1881 2023-05-17 10:19:51.971320 dessert-1.4.7/PKG-INFO
+-rw-r--r--   0 rotemy     (501) staff       (20)     1206 2023-02-14 19:46:06.000000 dessert-1.4.7/README.md
+drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-05-17 10:19:51.968487 dessert-1.4.7/dessert/
+-rw-r--r--   0 rotemy     (501) staff       (20)      467 2022-08-02 13:57:50.000000 dessert-1.4.7/dessert/__init__.py
+-rw-r--r--   0 rotemy     (501) staff       (20)       86 2022-03-23 12:20:06.000000 dessert-1.4.7/dessert/__version__.py
+-rw-r--r--   0 rotemy     (501) staff       (20)      345 2022-03-23 12:20:06.000000 dessert-1.4.7/dessert/conf.py
+-rw-r--r--   0 rotemy     (501) staff       (20)     1624 2022-03-23 12:20:06.000000 dessert-1.4.7/dessert/pathlib.py
+-rw-r--r--   0 rotemy     (501) staff       (20)    39063 2023-05-17 10:19:09.000000 dessert-1.4.7/dessert/rewrite.py
+-rw-r--r--   0 rotemy     (501) staff       (20)     1945 2022-03-23 12:20:06.000000 dessert-1.4.7/dessert/saferepr.py
+-rw-r--r--   0 rotemy     (501) staff       (20)    14757 2022-03-23 12:20:06.000000 dessert-1.4.7/dessert/util.py
+-rw-r--r--   0 rotemy     (501) staff       (20)      160 2022-03-23 12:20:06.000000 dessert-1.4.7/dessert/warning_types.py
+drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-05-17 10:19:51.969240 dessert-1.4.7/dessert.egg-info/
+-rw-r--r--   0 rotemy     (501) staff       (20)     1881 2023-05-17 10:19:51.000000 dessert-1.4.7/dessert.egg-info/PKG-INFO
+-rw-r--r--   0 rotemy     (501) staff       (20)      756 2023-05-17 10:19:51.000000 dessert-1.4.7/dessert.egg-info/SOURCES.txt
+-rw-r--r--   0 rotemy     (501) staff       (20)        1 2023-05-17 10:19:51.000000 dessert-1.4.7/dessert.egg-info/dependency_links.txt
+-rw-r--r--   0 rotemy     (501) staff       (20)        1 2023-05-17 10:19:51.000000 dessert-1.4.7/dessert.egg-info/not-zip-safe
+-rw-r--r--   0 rotemy     (501) staff       (20)       47 2023-05-17 10:19:51.000000 dessert-1.4.7/dessert.egg-info/pbr.json
+-rw-r--r--   0 rotemy     (501) staff       (20)       65 2023-05-17 10:19:51.000000 dessert-1.4.7/dessert.egg-info/requires.txt
+-rw-r--r--   0 rotemy     (501) staff       (20)        8 2023-05-17 10:19:51.000000 dessert-1.4.7/dessert.egg-info/top_level.txt
+-rw-r--r--   0 rotemy     (501) staff       (20)       33 2022-03-23 12:20:01.000000 dessert-1.4.7/requirements.txt
+drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-05-17 10:19:51.969776 dessert-1.4.7/scripts/
+-rw-r--r--   0 rotemy     (501) staff       (20)      246 2022-03-23 12:20:02.000000 dessert-1.4.7/scripts/call-tox.bat
+-rw-r--r--   0 rotemy     (501) staff       (20)      546 2022-03-23 12:20:02.000000 dessert-1.4.7/scripts/check-manifest.py
+-rw-r--r--   0 rotemy     (501) staff       (20)      322 2022-03-23 12:20:02.000000 dessert-1.4.7/scripts/install-pypy.bat
+-rw-r--r--   0 rotemy     (501) staff       (20)      665 2023-05-17 10:19:51.971582 dessert-1.4.7/setup.cfg
+-rw-r--r--   0 rotemy     (501) staff       (20)      224 2023-02-14 19:46:06.000000 dessert-1.4.7/setup.py
+drwxr-xr-x   0 rotemy     (501) staff       (20)        0 2023-05-17 10:19:51.971110 dessert-1.4.7/tests/
+-rw-r--r--   0 rotemy     (501) staff       (20)       94 2022-03-23 12:20:06.000000 dessert-1.4.7/tests/__init__.py
+-rw-r--r--   0 rotemy     (501) staff       (20)       28 2022-03-23 12:20:06.000000 dessert-1.4.7/tests/conftest.py
+-rw-r--r--   0 rotemy     (501) staff       (20)      377 2022-03-23 12:20:06.000000 dessert-1.4.7/tests/driver.py
+-rw-r--r--   0 rotemy     (501) staff       (20)      181 2022-03-23 12:20:06.000000 dessert-1.4.7/tests/examples.py
+-rw-r--r--   0 rotemy     (501) staff       (20)     3620 2023-02-14 19:46:06.000000 dessert-1.4.7/tests/test_dessert.py
+-rw-r--r--   0 rotemy     (501) staff       (20)      889 2022-03-23 12:20:06.000000 dessert-1.4.7/tests/test_integration.py
+-rw-r--r--   0 rotemy     (501) staff       (20)      579 2022-03-23 12:20:06.000000 dessert-1.4.7/tests/test_readme_doctest.py
+-rw-r--r--   0 rotemy     (501) staff       (20)      121 2022-03-23 12:20:01.000000 dessert-1.4.7/tox.ini
```

### Comparing `dessert-1.4.6/.github/workflows/test.yml` & `dessert-1.4.7/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 on: [push]
 
 jobs:
   Test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `dessert-1.4.6/AUTHORS` & `dessert-1.4.7/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
 Miro Hrončok <miro@hroncok.cz>
 NODA, Kai <nodakai@gmail.com>
 Ned Batchelder <ned@nedbatchelder.com>
 Nicholas Chammas <nicholas.chammas@gmail.com>
 Nick Loadholtes <nick@ironboundsoftware.com>
 Nicolas Delaby <nicolas.delaby@ezeep.com>
 Nikita Tsvetkov <nikitanovosibirsk@yandex.com>
+Nikita Tsvetkov <tsv1@fastmail.com>
 Nikolaus Rath <Nikolaus@rath.org>
 Oleg Alexandrov <oleg.alexandrov@gmail.com>
 Oleksii Markhovskyi <olexiy.markhovsky@gmail.com>
 Oliver Bestwalter <oliver.bestwalter@avira.com>
 Omar Kohl <omarkohl@gmail.com>
 Omer Hadari <hadari.omer@gmail.com>
 Oscar Hellström <oscar@hellstrom.st>
```

### Comparing `dessert-1.4.6/ChangeLog` & `dessert-1.4.7/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+1.4.7
+-----
+
+* update github action
+* add package classifier
+* fix error 'AST node line range is not valid'
+
 1.4.6
 -----
 
 * On Windows attempting to create pyc for builtins hangs
 
 1.4.5
 -----
```

### Comparing `dessert-1.4.6/DEVELOPMENT.md` & `dessert-1.4.7/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `dessert-1.4.6/LICENSE` & `dessert-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dessert-1.4.6/PKG-INFO` & `dessert-1.4.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 Metadata-Version: 2.1
 Name: dessert
-Version: 1.4.6
+Version: 1.4.7
 Summary: Assertion introspection via AST rewriting
 Home-page: https://github.com/vmalloc/dessert
 Author: Rotem Yaari
 Author-email: vmalloc@gmail.com
 License: MIT
-Description: ![Build Status](https://github.com/vmalloc/dessert/actions/workflows/test.yml/badge.svg?branch=develop)
-        ![Version](https://img.shields.io/pypi/v/dessert.svg)
-        
-        Overview
-        ========
-        
-        Dessert is a utility library enabling Python code to introspect assertions raised via the `assert` statement.
-        
-        It is a standalone version of the introspection code from [pytest](http://pytest.org ), and all credit is due to Holger Krekel and the pytest developers for this code.
-        
-        Usage
-        =====
-        
-        Using dessert is fairly simple:
-        
-        ```python
-        
-        >>> with open(tmp_filename, "w") as f:
-        ...     _ = f.write("""
-        ... def func():
-        ...     def x():
-        ...         return 1
-        ...     def y():
-        ...         return -1
-        ...     assert y() == x()
-        ... """)
-        
-        >>> import emport
-        >>> import dessert
-        >>> with dessert.rewrite_assertions_context():
-        ...     module = emport.import_file(tmp_filename)
-        >>> module.func() # doctest: +IGNORE_EXCEPTION_DETAIL +ELLIPSIS
-        Traceback (most recent call last):
-            ...
-            assert y() == x()
-        AssertionError: assert -1 == 1
-        +  where -1 = <function y at ...>()
-        +  and   1 = <function x at ...>()
-        ```
-        
-        Licence
-        =======
-        
-        Dessert is released under the MIT license. It is 99% based on pytest, which is released under the MIT license.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+
+![Build Status](https://github.com/vmalloc/dessert/actions/workflows/test.yml/badge.svg?branch=develop)
+![Version](https://img.shields.io/pypi/v/dessert.svg)
+
+Overview
+========
+
+Dessert is a utility library enabling Python code to introspect assertions raised via the `assert` statement.
+
+It is a standalone version of the introspection code from [pytest](http://pytest.org ), and all credit is due to Holger Krekel and the pytest developers for this code.
+
+Usage
+=====
+
+Using dessert is fairly simple:
+
+```python
+
+>>> with open(tmp_filename, "w") as f:
+...     _ = f.write("""
+... def func():
+...     def x():
+...         return 1
+...     def y():
+...         return -1
+...     assert y() == x()
+... """)
+
+>>> import emport
+>>> import dessert
+>>> with dessert.rewrite_assertions_context():
+...     module = emport.import_file(tmp_filename)
+>>> module.func() # doctest: +IGNORE_EXCEPTION_DETAIL +ELLIPSIS
+Traceback (most recent call last):
+    ...
+    assert y() == x()
+AssertionError: assert -1 == 1
++  where -1 = <function y at ...>()
++  and   1 = <function x at ...>()
+```
+
+Licence
+=======
+
+Dessert is released under the MIT license. It is 99% based on pytest, which is released under the MIT license.
+
```

### Comparing `dessert-1.4.6/README.md` & `dessert-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `dessert-1.4.6/dessert/pathlib.py` & `dessert-1.4.7/dessert/pathlib.py`

 * *Files identical despite different names*

### Comparing `dessert-1.4.6/dessert/rewrite.py` & `dessert-1.4.7/dessert/rewrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -827,29 +827,32 @@
         """
         Returns an AST issuing a warning if the value of node is `None`.
         This is used to warn the user when asserting a function that asserts
         internally already.
         See issue #3191 for more details.
         """
         val_is_none = ast.Compare(node, [ast.Is()], [ast.NameConstant(None)])
-        send_warning = ast.parse(
-            """\
-from dessert.warning_types import DessertAssertRewriteWarning
-from warnings import warn_explicit
-warn_explicit(
-    DessertAssertRewriteWarning('asserting the value None, please use "assert is None"'),
-    category=None,
-    filename={filename!r},
-    lineno={lineno},
-)
-            """.format(
-                filename=module_path, lineno=lineno
-            )
-        ).body
-        return ast.If(val_is_none, send_warning, [])
+
+        exc_call = ast.Call(
+            func=ast.Name("DessertAssertRewriteWarning", ast.Load()),
+            args=[ast.Str('asserting the value None, please use "assert is None"')],
+            keywords=[]
+        )
+        warn_call = ast.Call(
+            func=ast.Name("warn_explicit", ast.Load()),
+            args=[exc_call, ast.NameConstant(None), ast.Str(module_path), ast.Num(lineno)],
+            keywords=[]
+        )
+        body = [
+            ast.ImportFrom("dessert.warning_types", [ast.alias("DessertAssertRewriteWarning")], level=0),
+            ast.ImportFrom("warnings", [ast.alias("warn_explicit")], level=0),
+            ast.Expr(warn_call),
+        ]
+
+        return ast.If(val_is_none, body, [])
 
     def visit_Name(self, name):
         # Display the repr of the name if it's a local variable or
         # _should_repr_global_name() thinks it's acceptable.
         locs = ast.Call(self.builtin("locals"), [], [])
         inlocs = ast.Compare(ast.Str(name.id), [ast.In()], [locs])
         dorepr = self.helper("_should_repr_global_name", name)
```

### Comparing `dessert-1.4.6/dessert/saferepr.py` & `dessert-1.4.7/dessert/saferepr.py`

 * *Files identical despite different names*

### Comparing `dessert-1.4.6/dessert/util.py` & `dessert-1.4.7/dessert/util.py`

 * *Files identical despite different names*

### Comparing `dessert-1.4.6/dessert.egg-info/PKG-INFO` & `dessert-1.4.7/dessert.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 Metadata-Version: 2.1
 Name: dessert
-Version: 1.4.6
+Version: 1.4.7
 Summary: Assertion introspection via AST rewriting
 Home-page: https://github.com/vmalloc/dessert
 Author: Rotem Yaari
 Author-email: vmalloc@gmail.com
 License: MIT
-Description: ![Build Status](https://github.com/vmalloc/dessert/actions/workflows/test.yml/badge.svg?branch=develop)
-        ![Version](https://img.shields.io/pypi/v/dessert.svg)
-        
-        Overview
-        ========
-        
-        Dessert is a utility library enabling Python code to introspect assertions raised via the `assert` statement.
-        
-        It is a standalone version of the introspection code from [pytest](http://pytest.org ), and all credit is due to Holger Krekel and the pytest developers for this code.
-        
-        Usage
-        =====
-        
-        Using dessert is fairly simple:
-        
-        ```python
-        
-        >>> with open(tmp_filename, "w") as f:
-        ...     _ = f.write("""
-        ... def func():
-        ...     def x():
-        ...         return 1
-        ...     def y():
-        ...         return -1
-        ...     assert y() == x()
-        ... """)
-        
-        >>> import emport
-        >>> import dessert
-        >>> with dessert.rewrite_assertions_context():
-        ...     module = emport.import_file(tmp_filename)
-        >>> module.func() # doctest: +IGNORE_EXCEPTION_DETAIL +ELLIPSIS
-        Traceback (most recent call last):
-            ...
-            assert y() == x()
-        AssertionError: assert -1 == 1
-        +  where -1 = <function y at ...>()
-        +  and   1 = <function x at ...>()
-        ```
-        
-        Licence
-        =======
-        
-        Dessert is released under the MIT license. It is 99% based on pytest, which is released under the MIT license.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+
+![Build Status](https://github.com/vmalloc/dessert/actions/workflows/test.yml/badge.svg?branch=develop)
+![Version](https://img.shields.io/pypi/v/dessert.svg)
+
+Overview
+========
+
+Dessert is a utility library enabling Python code to introspect assertions raised via the `assert` statement.
+
+It is a standalone version of the introspection code from [pytest](http://pytest.org ), and all credit is due to Holger Krekel and the pytest developers for this code.
+
+Usage
+=====
+
+Using dessert is fairly simple:
+
+```python
+
+>>> with open(tmp_filename, "w") as f:
+...     _ = f.write("""
+... def func():
+...     def x():
+...         return 1
+...     def y():
+...         return -1
+...     assert y() == x()
+... """)
+
+>>> import emport
+>>> import dessert
+>>> with dessert.rewrite_assertions_context():
+...     module = emport.import_file(tmp_filename)
+>>> module.func() # doctest: +IGNORE_EXCEPTION_DETAIL +ELLIPSIS
+Traceback (most recent call last):
+    ...
+    assert y() == x()
+AssertionError: assert -1 == 1
++  where -1 = <function y at ...>()
++  and   1 = <function x at ...>()
+```
+
+Licence
+=======
+
+Dessert is released under the MIT license. It is 99% based on pytest, which is released under the MIT license.
+
```

### Comparing `dessert-1.4.6/dessert.egg-info/SOURCES.txt` & `dessert-1.4.7/dessert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dessert-1.4.6/scripts/check-manifest.py` & `dessert-1.4.7/scripts/check-manifest.py`

 * *Files identical despite different names*

### Comparing `dessert-1.4.6/setup.cfg` & `dessert-1.4.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 classifiers = 
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 summary = Assertion introspection via AST rewriting
 description-file = 
 	README.md
 description-content-type = text/markdown
 license = MIT
 author = Rotem Yaari
 author_email = vmalloc@gmail.com
```

### Comparing `dessert-1.4.6/tests/test_dessert.py` & `dessert-1.4.7/tests/test_dessert.py`

 * *Files identical despite different names*

### Comparing `dessert-1.4.6/tests/test_integration.py` & `dessert-1.4.7/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `dessert-1.4.6/tests/test_readme_doctest.py` & `dessert-1.4.7/tests/test_readme_doctest.py`

 * *Files identical despite different names*

