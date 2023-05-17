# Comparing `tmp/markata_gh-0.7.0.dev0.tar.gz` & `tmp/markata_gh-0.7.0.dev1.tar.gz`

## Comparing `markata_gh-0.7.0.dev0.tar` & `markata_gh-0.7.0.dev1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/.flake8
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/.github/workflows/release.yml
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/markata_gh/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/markata_gh/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/markata_gh/repo_list.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/tests/__init__.py
--rw-r--r--   0        0        0    17257 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/.gitignore
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/LICENSE.txt
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/README.md
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/.flake8
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/markata_gh/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/markata_gh/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/markata_gh/repo_list.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/tests/__init__.py
+-rw-r--r--   0        0        0    17257 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/.gitignore
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/LICENSE.txt
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/README.md
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 markata_gh-0.7.0.dev1/PKG-INFO
```

### Comparing `markata_gh-0.7.0.dev0/markata_gh/repo_list.py` & `markata_gh-0.7.0.dev1/markata_gh/repo_list.py`

 * *Files identical despite different names*

### Comparing `markata_gh-0.7.0.dev0/.gitignore` & `markata_gh-0.7.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `markata_gh-0.7.0.dev0/README.md` & `markata_gh-0.7.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `markata_gh-0.7.0.dev0/pyproject.toml` & `markata_gh-0.7.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `markata_gh-0.7.0.dev0/PKG-INFO` & `markata_gh-0.7.0.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: markata-gh
-Version: 0.7.0.dev0
+Version: 0.7.0.dev1
 Project-URL: Documentation, https://github.com/WaylonWalker/markata-gh#readme
 Project-URL: Issues, https://github.com/WaylonWalker/markata-gh/issues
 Project-URL: Source, https://github.com/WaylonWalker/markata-gh
 Author-email: "Waylon S. Walker" <waylon@waylonwalker.com>
+License-Expression: MIT
+License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

