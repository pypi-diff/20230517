# Comparing `tmp/xeauth-0.2.1.tar.gz` & `tmp/xeauth-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeauth-0.2.1.tar", max compression
+gzip compressed data, was "xeauth-0.2.2.tar", max compression
```

## Comparing `xeauth-0.2.1.tar` & `xeauth-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1073 2020-12-17 17:27:26.780407 xeauth-0.2.1/LICENSE
--rw-r--r--   0        0        0      877 2020-12-17 17:27:26.757073 xeauth-0.2.1/README.rst
--rw-r--r--   0        0        0     1432 2023-05-15 18:19:36.575580 xeauth-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       36 2020-12-17 17:27:26.787073 xeauth-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1002 2023-01-19 13:38:16.595387 xeauth-0.2.1/tests/test_xeauth.py
--rw-r--r--   0        0        0      262 2023-05-15 18:19:36.578913 xeauth-0.2.1/xeauth/__init__.py
--rw-r--r--   0        0        0     2266 2023-01-19 15:33:09.669806 xeauth-0.2.1/xeauth/admin.py
--rw-r--r--   0        0        0     3925 2023-01-19 15:32:52.905554 xeauth-0.2.1/xeauth/cli.py
--rw-r--r--   0        0        0     8207 2023-05-15 18:19:16.008607 xeauth-0.2.1/xeauth/github.py
--rw-r--r--   0        0        0     2123 2023-05-13 20:33:32.315405 xeauth-0.2.1/xeauth/settings.py
--rw-r--r--   0        0        0     2045 2023-05-15 18:19:16.008607 xeauth-0.2.1/xeauth/user.py
--rw-r--r--   0        0        0     1162 2023-01-19 13:38:16.922057 xeauth-0.2.1/xeauth/utils.py
--rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 xeauth-0.2.1/setup.py
--rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 xeauth-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2020-12-17 17:27:26.780407 xeauth-0.2.2/LICENSE
+-rw-r--r--   0        0        0      877 2020-12-17 17:27:26.757073 xeauth-0.2.2/README.rst
+-rw-r--r--   0        0        0     1330 2023-05-17 09:46:39.403455 xeauth-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       36 2020-12-17 17:27:26.787073 xeauth-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     1002 2023-01-19 13:38:16.595387 xeauth-0.2.2/tests/test_xeauth.py
+-rw-r--r--   0        0        0      262 2023-05-17 09:46:39.403455 xeauth-0.2.2/xeauth/__init__.py
+-rw-r--r--   0        0        0     2266 2023-01-19 15:33:09.669806 xeauth-0.2.2/xeauth/admin.py
+-rw-r--r--   0        0        0     3925 2023-01-19 15:32:52.905554 xeauth-0.2.2/xeauth/cli.py
+-rw-r--r--   0        0        0     8207 2023-05-15 18:19:16.008607 xeauth-0.2.2/xeauth/github.py
+-rw-r--r--   0        0        0      725 2023-05-17 09:46:20.653176 xeauth-0.2.2/xeauth/integrations/panel.py
+-rw-r--r--   0        0        0     2123 2023-05-13 20:33:32.315405 xeauth-0.2.2/xeauth/settings.py
+-rw-r--r--   0        0        0     2045 2023-05-15 18:19:16.008607 xeauth-0.2.2/xeauth/user.py
+-rw-r--r--   0        0        0     1162 2023-01-19 13:38:16.922057 xeauth-0.2.2/xeauth/utils.py
+-rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 xeauth-0.2.2/setup.py
+-rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 xeauth-0.2.2/PKG-INFO
```

### Comparing `xeauth-0.2.1/LICENSE` & `xeauth-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.1/README.rst` & `xeauth-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.1/pyproject.toml` & `xeauth-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "xeauth"
-version = "0.2.1"
+version = "0.2.2"
 homepage = "https://github.com/jmosbacher/xeauth"
 description = "Top-level package for xeauth."
 authors = ["Yossi Mosbacher <joe.mosbacher@gmail.com>"]
 readme = "README.rst"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -41,18 +41,16 @@
 sphinx = "*"
 tox = "*"
 yapf = "*"
 sphinx-material = "*"
 nbsphinx = "*"
 
 [tool.poetry.plugins] 
-[tool.poetry.plugins."eve_panel.auth"]
-"XenonAuth" = "xeauth.integrations.eve_panel:XenonEveAuth"
 [tool.poetry.plugins."panel.auth"]
-"xeauth" = "xeauth.integrations.panel_server:XenonPanelAuth"
+"xeauth" = "xeauth.integrations.panel:XenonLoginHandler"
 
 [tool.poetry.scripts]
 xeauth = 'xeauth.cli:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.8", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xeauth-0.2.1/tests/test_xeauth.py` & `xeauth-0.2.2/tests/test_xeauth.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.1/xeauth/admin.py` & `xeauth-0.2.2/xeauth/admin.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.1/xeauth/cli.py` & `xeauth-0.2.2/xeauth/cli.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.1/xeauth/github.py` & `xeauth-0.2.2/xeauth/github.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.1/xeauth/settings.py` & `xeauth-0.2.2/xeauth/settings.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.1/xeauth/user.py` & `xeauth-0.2.2/xeauth/user.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.1/xeauth/utils.py` & `xeauth-0.2.2/xeauth/utils.py`

 * *Files identical despite different names*

### Comparing `xeauth-0.2.1/setup.py` & `xeauth-0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['tests', 'xeauth']
+['tests', 'xeauth', 'xeauth.integrations']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['appdirs>=1.4.4,<2.0.0',
  'click',
  'gnupg>=2.3.1,<3.0.0',
  'httpx>=0.19,<0.25',
  'param>=1.12.0,<2.0.0',
  'rich>=13.1.0,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['xeauth = xeauth.cli:main'],
- 'eve_panel.auth': ['XenonAuth = xeauth.integrations.eve_panel:XenonEveAuth'],
- 'panel.auth': ['xeauth = xeauth.integrations.panel_server:XenonPanelAuth']}
+ 'panel.auth': ['xeauth = xeauth.integrations.panel:XenonLoginHandler']}
 
 setup_kwargs = {
     'name': 'xeauth',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Top-level package for xeauth.',
     'long_description': '======\nxeauth\n======\n\n\n.. image:: https://img.shields.io/pypi/v/xeauth.svg\n        :target: https://pypi.python.org/pypi/xeauth\n\n.. image:: https://img.shields.io/travis/jmosbacher/xeauth.svg\n        :target: https://travis-ci.com/jmosbacher/xeauth\n\n.. image:: https://readthedocs.org/projects/xeauth/badge/?version=latest\n        :target: https://xeauth.readthedocs.io/en/latest/?badge=latest\n        :alt: Documentation Status\n\n\n\n\nAuthentication client for the Xenon edark matter experiment.\n\n\n* Free software: MIT\n* Documentation: https://xeauth.readthedocs.io.\n\n\nFeatures\n--------\n\n* TODO\n\nCredits\n-------\n\nThis package was created with Cookiecutter_ and the `briggySmalls/cookiecutter-pypackage`_ project template.\n\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _`briggySmalls/cookiecutter-pypackage`: https://github.com/briggySmalls/cookiecutter-pypackage\n',
     'author': 'Yossi Mosbacher',
     'author_email': 'joe.mosbacher@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jmosbacher/xeauth',
```

### Comparing `xeauth-0.2.1/PKG-INFO` & `xeauth-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeauth
-Version: 0.2.1
+Version: 0.2.2
 Summary: Top-level package for xeauth.
 Home-page: https://github.com/jmosbacher/xeauth
 License: MIT
 Author: Yossi Mosbacher
 Author-email: joe.mosbacher@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 2 - Pre-Alpha
```

