# Comparing `tmp/Flask-PluginKit-3.7.1.tar.gz` & `tmp/Flask-PluginKit-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-PluginKit-3.7.1.tar", last modified: Tue Sep  7 13:36:32 2021, max compression
+gzip compressed data, was "Flask-PluginKit-3.7.2.tar", last modified: Wed May 17 03:26:26 2023, max compression
```

## Comparing `Flask-PluginKit-3.7.1.tar` & `Flask-PluginKit-3.7.2.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 13:36:32.376284 Flask-PluginKit-3.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 13:36:32.376284 Flask-PluginKit-3.7.1/Flask_PluginKit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-09-07 13:36:32.000000 Flask-PluginKit-3.7.1/Flask_PluginKit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      553 2021-09-07 13:36:32.000000 Flask-PluginKit-3.7.1/Flask_PluginKit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-07 13:36:32.000000 Flask-PluginKit-3.7.1/Flask_PluginKit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-07 13:36:21.000000 Flask-PluginKit-3.7.1/Flask_PluginKit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-09-07 13:36:32.000000 Flask-PluginKit-3.7.1/Flask_PluginKit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-09-07 13:36:32.000000 Flask-PluginKit-3.7.1/Flask_PluginKit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-09-07 13:36:32.376284 Flask-PluginKit-3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 13:36:32.376284 Flask-PluginKit-3.7.1/flask_pluginkit/
--rw-r--r--   0 runner    (1001) docker     (121)      653 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/flask_pluginkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/flask_pluginkit/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    10767 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/flask_pluginkit/_installer.py
--rw-r--r--   0 runner    (1001) docker     (121)    10148 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/flask_pluginkit/_web.py
--rw-r--r--   0 runner    (1001) docker     (121)      558 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/flask_pluginkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    48985 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/flask_pluginkit/pluginkit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 13:36:32.376284 Flask-PluginKit-3.7.1/flask_pluginkit/static/
--rw-r--r--   0 runner    (1001) docker     (121)      820 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/flask_pluginkit/static/translations.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 13:36:32.376284 Flask-PluginKit-3.7.1/flask_pluginkit/templates/
--rw-r--r--   0 runner    (1001) docker     (121)    14880 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/flask_pluginkit/templates/manager.html
--rw-r--r--   0 runner    (1001) docker     (121)    12095 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/flask_pluginkit/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-09-07 13:36:32.380284 Flask-PluginKit-3.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4139 2021-09-07 13:36:05.000000 Flask-PluginKit-3.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.394666 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3470 2023-05-17 03:26:26.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      614 2023-05-17 03:26:26.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:26:26.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 02:59:12.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 03:26:26.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-17 03:26:26.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1507 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       88 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3470 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-05-15 03:29:18.000000 Flask-PluginKit-3.7.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.394666 Flask-PluginKit-3.7.2/flask_pluginkit/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-05-17 02:45:19.000000 Flask-PluginKit-3.7.2/flask_pluginkit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/flask_pluginkit/_compat.py
+-rw-r--r--   0 root         (0) root         (0)    10767 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/flask_pluginkit/_installer.py
+-rw-r--r--   0 root         (0) root         (0)    10148 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/flask_pluginkit/_web.py
+-rw-r--r--   0 root         (0) root         (0)      558 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/flask_pluginkit/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    48626 2023-05-17 02:46:28.000000 Flask-PluginKit-3.7.2/flask_pluginkit/pluginkit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/flask_pluginkit/static/
+-rw-r--r--   0 root         (0) root         (0)      820 2023-05-15 03:29:18.000000 Flask-PluginKit-3.7.2/flask_pluginkit/static/translations.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/flask_pluginkit/templates/
+-rw-r--r--   0 root         (0) root         (0)    14880 2023-05-15 03:29:18.000000 Flask-PluginKit-3.7.2/flask_pluginkit/templates/manager.html
+-rw-r--r--   0 root         (0) root         (0)    12095 2023-05-15 03:29:18.000000 Flask-PluginKit-3.7.2/flask_pluginkit/utils.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4196 2023-05-17 02:57:23.000000 Flask-PluginKit-3.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     2490 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/tests/test_installer.py
+-rw-r--r--   0 root         (0) root         (0)     8485 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/tests/test_pm.py
+-rw-r--r--   0 root         (0) root         (0)     5584 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/tests/test_utils.py
```

### Comparing `Flask-PluginKit-3.7.1/Flask_PluginKit.egg-info/PKG-INFO` & `Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: Flask-PluginKit
-Version: 3.7.1
+Version: 3.7.2
 Summary: Load and run plugins for your Flask application
 Home-page: https://github.com/staugur/Flask-PluginKit
+Download-URL: https://github.com/staugur/Flask-PluginKit/releases/tag/v3.7.2
 Author: Hiroshi.tao
 Author-email: me@tcw.im
 License: BSD 3-Clause
-Download-URL: https://github.com/staugur/Flask-PluginKit/releases/tag/v3.7.1
 Project-URL: Code, https://github.com/staugur/Flask-PluginKit
 Project-URL: Issue tracker, https://github.com/staugur/Flask-PluginKit/issues
 Project-URL: Documentation, https://flask-pluginkit.rtfd.vip
 Keywords: flask plugin
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Flask
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.3.*,!=3.5.*
 License-File: LICENSE
 
@@ -111,9 +111,7 @@
     :target: https://github.com/staugur/Flask-PluginKit/actions/workflows/ci.yml
 .. |Documentation Status| image:: https://open.saintic.com/rtfd/badge/flask-pluginkit
     :target: https://flask-pluginkit.rtfd.vip
 .. |codecov| image:: https://codecov.io/gh/staugur/Flask-PluginKit/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/staugur/Flask-PluginKit
 .. |PyPI| image:: https://img.shields.io/pypi/v/Flask-PluginKit.svg?style=popout
     :target: https://pypi.org/project/Flask-PluginKit/
-
-
```

### Comparing `Flask-PluginKit-3.7.1/Flask_PluginKit.egg-info/SOURCES.txt` & `Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,8 +13,11 @@
 flask_pluginkit/_compat.py
 flask_pluginkit/_installer.py
 flask_pluginkit/_web.py
 flask_pluginkit/exceptions.py
 flask_pluginkit/pluginkit.py
 flask_pluginkit/utils.py
 flask_pluginkit/static/translations.ini
-flask_pluginkit/templates/manager.html
+flask_pluginkit/templates/manager.html
+tests/test_installer.py
+tests/test_pm.py
+tests/test_utils.py
```

### Comparing `Flask-PluginKit-3.7.1/LICENSE` & `Flask-PluginKit-3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.1/PKG-INFO` & `Flask-PluginKit-3.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: Flask-PluginKit
-Version: 3.7.1
+Version: 3.7.2
 Summary: Load and run plugins for your Flask application
 Home-page: https://github.com/staugur/Flask-PluginKit
+Download-URL: https://github.com/staugur/Flask-PluginKit/releases/tag/v3.7.2
 Author: Hiroshi.tao
 Author-email: me@tcw.im
 License: BSD 3-Clause
-Download-URL: https://github.com/staugur/Flask-PluginKit/releases/tag/v3.7.1
 Project-URL: Code, https://github.com/staugur/Flask-PluginKit
 Project-URL: Issue tracker, https://github.com/staugur/Flask-PluginKit/issues
 Project-URL: Documentation, https://flask-pluginkit.rtfd.vip
 Keywords: flask plugin
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Flask
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.3.*,!=3.5.*
 License-File: LICENSE
 
@@ -111,9 +111,7 @@
     :target: https://github.com/staugur/Flask-PluginKit/actions/workflows/ci.yml
 .. |Documentation Status| image:: https://open.saintic.com/rtfd/badge/flask-pluginkit
     :target: https://flask-pluginkit.rtfd.vip
 .. |codecov| image:: https://codecov.io/gh/staugur/Flask-PluginKit/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/staugur/Flask-PluginKit
 .. |PyPI| image:: https://img.shields.io/pypi/v/Flask-PluginKit.svg?style=popout
     :target: https://pypi.org/project/Flask-PluginKit/
-
-
```

### Comparing `Flask-PluginKit-3.7.1/README.rst` & `Flask-PluginKit-3.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.1/flask_pluginkit/_compat.py` & `Flask-PluginKit-3.7.2/flask_pluginkit/_compat.py`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.1/flask_pluginkit/_installer.py` & `Flask-PluginKit-3.7.2/flask_pluginkit/_installer.py`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.1/flask_pluginkit/_web.py` & `Flask-PluginKit-3.7.2/flask_pluginkit/_web.py`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.1/flask_pluginkit/exceptions.py` & `Flask-PluginKit-3.7.2/flask_pluginkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.1/flask_pluginkit/pluginkit.py` & `Flask-PluginKit-3.7.2/flask_pluginkit/pluginkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,17 @@
     .. deprecated:: 3.7.0
         Ready to remove ``stpl_reverse`` and ``try_compatible``
         in the next minor version, if it is still used,
         a warning will be issued.
 
     .. versionchanged:: 3.7.0
         Add ``p3`` feature for beta.
+
+    .. deprecated:: 3.7.2
+        Remove `before_first_request` hep
     """
 
     def __init__(
         self, app=None, plugins_base=None, plugins_folder="plugins", **options
     ):
         """Receive initialization parameters and
         pass options to :meth:`init_app` method.
@@ -184,15 +187,14 @@
         }
 
         #: Hook extension type handlers
         self.__het_allow_hooks = {
             "before_request": self.__before_request_hook_handler,
             "after_request": self.__after_request_hook_handler,
             "teardown_request": self.__teardown_request_hook_handler,
-            "before_first_request": self.__before_fist_request_hook_handler,
         }
 
         #: Dynamic Connection Point
         #:
         #: .. versionadded:: 3.2.0
         self._dcp_manager = DcpManager()
 
@@ -621,18 +623,14 @@
 
                         2. after_request, After request
                         (no exception before return)
 
                         3. teardown_request, After request
                         (before return, with or without exception)
 
-                        4. before_first_request, Before first request
-                        (Registers a function to be run before the first
-                        request to this instance of the application.)
-
         :raises PEPError: if hep rule or content is invalid.
         """
         if isinstance(hep_rule, dict):
             plugin_hep = {}
             for event, func in iteritems(hep_rule):
                 if event in self.__het_allow_hooks.keys():
                     if callable(func):
@@ -923,18 +921,14 @@
             plugin_info["plugin_p3"] = p3_rule
         else:
             raise PEPError(
                 "The p3 handler rule is invalid for %s, "
                 "it should be a dict." % plugin_info.plugin_name
             )
 
-    def __before_fist_request_hook_handler(self):
-        for func in self.get_enabled_heps["before_first_request"]:
-            func()
-
     def __before_request_hook_handler(self):
         for func in self.get_enabled_heps["before_request"]:
             resp = func()
             if resp is not None:
                 return resp
 
     def __after_request_hook_handler(self, response):
```

### Comparing `Flask-PluginKit-3.7.1/flask_pluginkit/static/translations.ini` & `Flask-PluginKit-3.7.2/flask_pluginkit/static/translations.ini`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.1/flask_pluginkit/templates/manager.html` & `Flask-PluginKit-3.7.2/flask_pluginkit/templates/manager.html`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.1/flask_pluginkit/utils.py` & `Flask-PluginKit-3.7.2/flask_pluginkit/utils.py`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.1/setup.py` & `Flask-PluginKit-3.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     long_description=_get_readme(),
     test_suite="setup.test_suite",
     tests_require=["Flask>=0.11", "Flask-Classful>=0.14.0"],
     packages=["flask_pluginkit"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.3.*,!=3.5.*",
-    install_requires=["Flask>=0.12", "semver>=2.10.0"],
+    install_requires=["Flask>=0.12", "semver>=2.10.0,<3.0.0"],
     cmdclass={
         "publish": PublishCommand,
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: Flask",
         "Environment :: Web Environment",
@@ -118,13 +118,14 @@
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

