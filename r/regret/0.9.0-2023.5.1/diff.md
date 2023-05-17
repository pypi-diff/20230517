# Comparing `tmp/regret-0.9.0.tar.gz` & `tmp/regret-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/regret-0.9.0.tar", last modified: Tue Oct 29 00:40:11 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `regret-0.9.0.tar` & `regret-2023.5.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-10-29 00:40:11.000000 regret-0.9.0/
--rw-r--r--   0 julian     (501) staff       (20)     3394 2019-10-29 00:40:11.000000 regret-0.9.0/PKG-INFO
--rw-r--r--   0 julian     (501) staff       (20)      150 2019-10-19 16:24:40.000000 regret-0.9.0/codecov.yml
--rw-r--r--   0 julian     (501) staff       (20)        8 2019-10-26 22:08:23.000000 regret-0.9.0/test-requirements.txt
--rw-r--r--   0 julian     (501) staff       (20)      248 2019-10-19 16:24:40.000000 regret-0.9.0/pyproject.toml
--rw-r--r--   0 julian     (501) staff       (20)       66 2019-10-19 16:24:40.000000 regret-0.9.0/MANIFEST.in
--rw-r--r--   0 julian     (501) staff       (20)       92 2019-10-19 16:24:40.000000 regret-0.9.0/.coveragerc
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-10-29 00:40:11.000000 regret-0.9.0/docs/
--rw-r--r--   0 julian     (501) staff       (20)       89 2019-10-19 16:24:41.000000 regret-0.9.0/docs/index.rst
--rw-r--r--   0 julian     (501) staff       (20)       53 2019-10-19 16:24:40.000000 regret-0.9.0/docs/requirements.txt
--rw-r--r--   0 julian     (501) staff       (20)      580 2019-10-19 16:24:41.000000 regret-0.9.0/docs/Makefile
--rw-r--r--   0 julian     (501) staff       (20)     5534 2019-10-21 22:48:33.000000 regret-0.9.0/docs/conf.py
--rw-r--r--   0 julian     (501) staff       (20)       24 2019-10-20 01:44:04.000000 regret-0.9.0/docs/spelling_wordlist.txt
--rw-r--r--   0 julian     (501) staff       (20)     1057 2019-10-19 16:24:40.000000 regret-0.9.0/COPYING
--rw-r--r--   0 julian     (501) staff       (20)       57 2019-10-19 16:24:40.000000 regret-0.9.0/setup.py
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-10-29 00:40:11.000000 regret-0.9.0/.github/
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-10-29 00:40:11.000000 regret-0.9.0/.github/workflows/
--rw-r--r--   0 julian     (501) staff       (20)      695 2019-10-20 13:21:54.000000 regret-0.9.0/.github/workflows/packaging.yml
--rw-r--r--   0 julian     (501) staff       (20)     3398 2019-10-26 22:09:39.000000 regret-0.9.0/tox.ini
--rw-r--r--   0 julian     (501) staff       (20)      140 2019-10-19 16:24:40.000000 regret-0.9.0/.testr.conf
--rw-r--r--   0 julian     (501) staff       (20)     1158 2019-10-29 00:40:11.000000 regret-0.9.0/setup.cfg
--rw-r--r--   0 julian     (501) staff       (20)     1858 2019-10-26 14:30:06.000000 regret-0.9.0/README.rst
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-10-29 00:40:11.000000 regret-0.9.0/regret.egg-info/
--rw-r--r--   0 julian     (501) staff       (20)     3394 2019-10-29 00:40:10.000000 regret-0.9.0/regret.egg-info/PKG-INFO
--rw-r--r--   0 julian     (501) staff       (20)      587 2019-10-29 00:40:10.000000 regret-0.9.0/regret.egg-info/SOURCES.txt
--rw-r--r--   0 julian     (501) staff       (20)       34 2019-10-29 00:40:10.000000 regret-0.9.0/regret.egg-info/requires.txt
--rw-r--r--   0 julian     (501) staff       (20)        7 2019-10-29 00:40:10.000000 regret-0.9.0/regret.egg-info/top_level.txt
--rw-r--r--   0 julian     (501) staff       (20)        1 2019-10-29 00:40:10.000000 regret-0.9.0/regret.egg-info/dependency_links.txt
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-10-29 00:40:11.000000 regret-0.9.0/regret/
--rw-r--r--   0 julian     (501) staff       (20)     3559 2019-10-29 00:37:10.000000 regret-0.9.0/regret/_api.py
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-10-29 00:40:11.000000 regret-0.9.0/regret/tests/
--rw-r--r--   0 julian     (501) staff       (20)        0 2019-10-19 16:24:40.000000 regret-0.9.0/regret/tests/__init__.py
--rw-r--r--   0 julian     (501) staff       (20)     3559 2019-10-29 00:39:33.000000 regret-0.9.0/regret/tests/test_integration.py
--rw-r--r--   0 julian     (501) staff       (20)     6393 2019-10-27 13:29:14.000000 regret-0.9.0/regret/tests/test_api.py
--rw-r--r--   0 julian     (501) staff       (20)      180 2019-10-20 19:28:00.000000 regret-0.9.0/regret/__init__.py
--rw-r--r--   0 julian     (501) staff       (20)      265 2019-10-25 12:50:47.000000 regret-0.9.0/regret/_warnings.py
--rw-r--r--   0 julian     (501) staff       (20)      200 2019-10-20 19:30:41.000000 regret-0.9.0/regret/testing.py
--rw-r--r--   0 julian     (501) staff       (20)      315 2019-10-29 00:37:27.000000 regret-0.9.0/regret/_sphinx.py
--rw-r--r--   0 julian     (501) staff       (20)      218 2019-10-20 00:58:05.000000 regret-0.9.0/.travis.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 regret-2023.5.1/.flake8
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 regret-2023.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 regret-2023.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 regret-2023.5.1/.testr.conf
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 regret-2023.5.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 regret-2023.5.1/MANIFEST.in
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 regret-2023.5.1/noxfile.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 regret-2023.5.1/test-requirements.in
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 regret-2023.5.1/test-requirements.txt
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 regret-2023.5.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 regret-2023.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 regret-2023.5.1/.github/release.yml
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 regret-2023.5.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/Makefile
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/before-you-deprecate.rst
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/compatibility.rst
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/conf.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/index.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/requirements.in
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/what-you-can-deprecate.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/api/modules.rst
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 regret-2023.5.1/docs/api/regret.rst
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/__init__.py
+-rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/_api.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/_inspect.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/_sphinx.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/_warnings.py
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/emitted.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/testing.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/tests/__init__.py
+-rw-r--r--   0        0        0    62906 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/tests/test_api.py
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/tests/test_integration.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 regret-2023.5.1/regret/tests/test_testing.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 regret-2023.5.1/COPYING
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 regret-2023.5.1/README.rst
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 regret-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 regret-2023.5.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `regret-0.9.0/PKG-INFO` & `regret-2023.5.1/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,102 @@
-Metadata-Version: 1.2
-Name: regret
-Version: 0.9.0
-Summary: "You made a thing, but now you wish it'd go away... Deprecations, a love story."
-Home-page: https://github.com/Julian/regret
-Author: Julian Berman
-Author-email: Julian+regret@GrayVines.com
-License: UNKNOWN
-Project-URL: Documentation, https://regret.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/Julian/regret
-Project-URL: Issues, https://github.com/Julian/regret/issues/
-Description: ======
-        regret
-        ======
-        
-        |PyPI| |Pythons| |CI| |Codecov| |ReadTheDocs|
-        
-        .. |PyPI| image:: https://img.shields.io/pypi/v/regret.svg
-          :alt: PyPI version
-          :target: https://pypi.org/project/regret/
-        
-        .. |Pythons| image:: https://img.shields.io/pypi/pyversions/regret.svg
-          :alt: Supported Python versions
-          :target: https://pypi.org/project/regret/
-        
-        .. |CI| image:: https://travis-ci.com/Julian/regret.svg?branch=master
-          :alt: Build status
-          :target: https://travis-ci.com/Julian/regret
-        
-        .. |Codecov| image:: https://codecov.io/gh/Julian/regret/branch/master/graph/badge.svg
-          :alt: Codecov Code coverage
-          :target: https://codecov.io/gh/Julian/regret
-        
-        .. |ReadTheDocs| image:: https://readthedocs.org/projects/regret/badge/?version=stable&style=flat
-          :alt: ReadTheDocs status
-          :target: https://regret.readthedocs.io/en/stable/
-        
-        ``Regret`` is a library for deprecating functionality in Python
-        libraries and applications.
-        
-        Its documentation lives on `Read the Docs
-        <https://regret.readthedocs.io/en/stable/>`_.
-        
-        
-        Design Goals
-        ------------
-        
-        ``Regret`` is meant to cover all of the deprecations an author may encounter.
-        
-        It is intended to:
-        
-            * be versioning system agnostic (i.e. `SemVer
-              <https://semver.org/>`_, `CalVer <https://calver.org/>`_, `HipsTer
-              <https://en.wikipedia.org/wiki/Hipster_(contemporary_subculture)>`_,
-              etc.)
-        
-            * be itself fully tested
-        
-            * minimize the amount of deprecation-related code required for authors
-        
-        In particular, as a lofty first milestone, it is intended to cover all
-        of the specific deprecations required for these `jsonschema issues
-        <https://github.com/Julian/jsonschema/issues?utf8=%E2%9C%93&q=label%3A%22Pending+Deprecation%22>`_,
-        and with luck, to subsume all the functionality present in
-        `twisted.python.deprecate <https://twistedmatrix.com/documents/current/api/twisted.python.deprecate.html>`_.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+======
+regret
+======
+
+|PyPI| |Pythons| |CI| |Codecov| |ReadTheDocs|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/regret.svg
+  :alt: PyPI version
+  :target: https://pypi.org/project/regret/
+
+.. |Pythons| image:: https://img.shields.io/pypi/pyversions/regret.svg
+  :alt: Supported Python versions
+  :target: https://pypi.org/project/regret/
+
+.. |CI| image:: https://github.com/Julian/regret/workflows/CI/badge.svg
+  :alt: Build status
+  :target: https://github.com/Julian/regret/actions?query=workflow%3ACI
+
+.. |Codecov| image:: https://codecov.io/gh/Julian/regret/branch/master/graph/badge.svg
+  :alt: Codecov Code coverage
+  :target: https://codecov.io/gh/Julian/regret
+
+.. |ReadTheDocs| image:: https://readthedocs.org/projects/regret/badge/?version=stable&style=flat
+  :alt: ReadTheDocs status
+  :target: https://regret.readthedocs.io/en/stable/
+
+``regret`` is a library for deprecating functionality in Python
+libraries and applications.
+
+Its documentation lives on `Read the Docs
+<https://regret.readthedocs.io/en/stable/>`_.
+
+
+Deprecations
+------------
+
+``regret`` can deprecate:
+
+    - [x] callables
+        - [x] functions
+        - [x] classes
+            - [ ] subclassable classes
+    - [ ] attributes
+        - [ ] of modules
+        - [ ] of classes (& methods)
+        - [ ] of instances
+    - [ ] descriptors
+        - [ ] classmethod
+    - [ ] modules
+        - [ ] current module
+        - [ ] other module
+    - [ ] parameters to callables
+        - [x] previously required parameters that will be removed
+        - [x] optional parameters that are now required
+        - [ ] deprecated values for parameters
+        - [ ] type changes for parameters
+        - [ ] mutual exclusion
+    - [ ] interfaces
+        - [ ] PEP 544 protocols
+        - [ ] ``zope.interface``\s
+    - [x] inheritability of a class
+
+
+Design Goals
+------------
+
+``regret`` is meant to cover all of the deprecations an author may encounter.
+
+It is intended to:
+
+    * be versioning system agnostic (i.e. `SemVer
+      <https://semver.org/>`_, `CalVer <https://calver.org/>`_, `HipsTer
+      <https://en.wikipedia.org/wiki/Hipster_(contemporary_subculture)>`_,
+      etc.), because deprecations originate from a version, a point in
+      time, or both.
+
+    * be documentation system aware (i.e. `Sphinx
+      <https://www.sphinx-doc.org>`_, `epydoc
+      <https://en.wikipedia.org/wiki/Epydoc>`_, `Plaintext
+      <https://www.google.com/search?q=use+sphinx>`_, etc.), because
+      deprecations need communication.
+
+    * be itself fully tested, because deprecations must not break the
+      code they deprecate
+
+    * support removal date indication, and likely "policies" which
+      automate choosing default removal dates, because deprecations
+      ultimately intend some ultimate change
+
+    * make "clean code" trivially easy to deprecate, and make complex
+      code *possible* to deprecate, because the deprecation process is
+      fraught with edge cases and unforeseen necessity.
+
+    * minimize the amount of deprecation-related code required for
+      authors, since deprecations are boring, and we all want to focus on
+      developing our libraries instead.
+
+In particular, as a lofty first milestone, it is intended to cover all
+of the specific deprecations required for these `jsonschema issues
+<https://github.com/Julian/jsonschema/issues?utf8=%E2%9C%93&q=label%3A%22Pending+Deprecation%22>`_,
+and with luck, to subsume all the functionality present in
+`twisted.python.deprecate <https://docs.twistedmatrix.com/en/stable/api/twisted.python.deprecate.html>`_.
```

### Comparing `regret-0.9.0/docs/Makefile` & `regret-2023.5.1/docs/Makefile`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `regret-0.9.0/COPYING` & `regret-2023.5.1/COPYING`

 * *Files identical despite different names*

