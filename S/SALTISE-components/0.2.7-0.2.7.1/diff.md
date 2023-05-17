# Comparing `tmp/SALTISE_components-0.2.7.tar.gz` & `tmp/SALTISE_components-0.2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SALTISE_components-0.2.7.tar", last modified: Mon May  1 03:50:40 2023, max compression
+gzip compressed data, was "SALTISE_components-0.2.7.1.tar", last modified: Wed May 17 04:03:58 2023, max compression
```

## Comparing `SALTISE_components-0.2.7.tar` & `SALTISE_components-0.2.7.1.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-01 03:50:40.791466 SALTISE_components-0.2.7/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1530 2023-01-25 16:48:45.000000 SALTISE_components-0.2.7/LICENSE
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      229 2023-01-25 16:48:45.000000 SALTISE_components-0.2.7/MANIFEST.in
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3099 2023-05-01 03:50:40.791466 SALTISE_components-0.2.7/PKG-INFO
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2192 2023-01-29 03:20:32.000000 SALTISE_components-0.2.7/README.rst
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-01 03:50:40.739466 SALTISE_components-0.2.7/SALTISE_components.egg-info/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3099 2023-05-01 03:50:40.000000 SALTISE_components-0.2.7/SALTISE_components.egg-info/PKG-INFO
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1181 2023-05-01 03:50:40.000000 SALTISE_components-0.2.7/SALTISE_components.egg-info/SOURCES.txt
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        1 2023-05-01 03:50:40.000000 SALTISE_components-0.2.7/SALTISE_components.egg-info/dependency_links.txt
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       18 2023-05-01 03:50:40.000000 SALTISE_components-0.2.7/SALTISE_components.egg-info/requires.txt
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       11 2023-05-01 03:50:40.000000 SALTISE_components-0.2.7/SALTISE_components.egg-info/top_level.txt
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-01 03:50:40.739466 SALTISE_components-0.2.7/components/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7/components/__init__.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      181 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7/components/apps.py
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-01 03:50:40.735466 SALTISE_components-0.2.7/components/static/
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-01 03:50:40.735466 SALTISE_components-0.2.7/components/static/components/
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-01 03:50:40.743466 SALTISE_components-0.2.7/components/static/components/img/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    99647 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7/components/static/components/img/avatar.jpg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     6044 2023-02-27 03:59:13.000000 SALTISE_components-0.2.7/components/static/components/img/collection-placeholder.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    11080 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7/components/static/components/img/logo.gif
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2302 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7/components/static/components/img/logo.png
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     4446 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7/components/static/components/img/logo.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2223 2023-03-24 03:31:40.000000 SALTISE_components-0.2.7/components/static/components/img/vector-search.svg
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-01 03:50:40.735466 SALTISE_components-0.2.7/components/static/components/js/
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-01 03:50:40.791466 SALTISE_components-0.2.7/components/static/components/js/build/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   220507 2023-01-29 03:20:32.000000 SALTISE_components-0.2.7/components/static/components/js/build/createQuestions1.min.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   216093 2023-01-25 16:48:45.000000 SALTISE_components-0.2.7/components/static/components/js/build/createQuestions2.min.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   185729 2023-05-01 03:43:57.000000 SALTISE_components-0.2.7/components/static/components/js/build/dashboard.min.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)  2997345 2023-02-05 05:46:18.000000 SALTISE_components-0.2.7/components/static/components/js/build/dashboardInvitedUser.min.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)  2997219 2023-02-05 05:46:18.000000 SALTISE_components-0.2.7/components/static/components/js/build/dashboardNewUser.min.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)  2978104 2023-02-05 05:46:18.000000 SALTISE_components-0.2.7/components/static/components/js/build/dashboardStudent.min.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   192422 2023-05-01 03:43:57.000000 SALTISE_components-0.2.7/components/static/components/js/build/library.min.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   182102 2023-05-01 03:43:57.000000 SALTISE_components-0.2.7/components/static/components/js/build/navigation.min.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   210167 2023-01-25 16:48:46.000000 SALTISE_components-0.2.7/components/static/components/js/build/questions.min.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   275218 2023-05-01 03:43:57.000000 SALTISE_components-0.2.7/components/static/components/js/build/search.min.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      639 2023-02-22 04:47:56.000000 SALTISE_components-0.2.7/pyproject.toml
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      917 2023-05-01 03:50:40.791466 SALTISE_components-0.2.7/setup.cfg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       38 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7/setup.py
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-17 04:03:58.668828 SALTISE_components-0.2.7.1/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1530 2023-01-25 16:48:45.000000 SALTISE_components-0.2.7.1/LICENSE
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      229 2023-01-25 16:48:45.000000 SALTISE_components-0.2.7.1/MANIFEST.in
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3101 2023-05-17 04:03:58.668828 SALTISE_components-0.2.7.1/PKG-INFO
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2192 2023-01-29 03:20:32.000000 SALTISE_components-0.2.7.1/README.rst
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-17 04:03:58.624828 SALTISE_components-0.2.7.1/SALTISE_components.egg-info/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3101 2023-05-17 04:03:58.000000 SALTISE_components-0.2.7.1/SALTISE_components.egg-info/PKG-INFO
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1299 2023-05-17 04:03:58.000000 SALTISE_components-0.2.7.1/SALTISE_components.egg-info/SOURCES.txt
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        1 2023-05-17 04:03:58.000000 SALTISE_components-0.2.7.1/SALTISE_components.egg-info/dependency_links.txt
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       18 2023-05-17 04:03:58.000000 SALTISE_components-0.2.7.1/SALTISE_components.egg-info/requires.txt
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       11 2023-05-17 04:03:58.000000 SALTISE_components-0.2.7.1/SALTISE_components.egg-info/top_level.txt
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-17 04:03:58.624828 SALTISE_components-0.2.7.1/components/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7.1/components/__init__.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      181 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7.1/components/apps.py
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-17 04:03:58.620828 SALTISE_components-0.2.7.1/components/static/
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-17 04:03:58.620828 SALTISE_components-0.2.7.1/components/static/components/
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-17 04:03:58.624828 SALTISE_components-0.2.7.1/components/static/components/img/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    99647 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7.1/components/static/components/img/avatar.jpg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     6044 2023-02-27 03:59:13.000000 SALTISE_components-0.2.7.1/components/static/components/img/collection-placeholder.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    11080 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7.1/components/static/components/img/logo.gif
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2302 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7.1/components/static/components/img/logo.png
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     4446 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7.1/components/static/components/img/logo.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2223 2023-03-24 03:31:40.000000 SALTISE_components-0.2.7.1/components/static/components/img/vector-search.svg
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-17 04:03:58.620828 SALTISE_components-0.2.7.1/components/static/components/js/
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-05-17 04:03:58.668828 SALTISE_components-0.2.7.1/components/static/components/js/build/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   797340 2023-05-17 03:57:11.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/createAssignment.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   220507 2023-01-29 03:20:32.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/createQuestions1.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   216093 2023-01-25 16:48:45.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/createQuestions2.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   185729 2023-05-01 03:43:57.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/dashboard.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)  2997345 2023-02-05 05:46:18.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/dashboardInvitedUser.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)  2997219 2023-02-05 05:46:18.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/dashboardNewUser.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)  2979089 2023-05-15 03:02:55.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/dashboardStudent.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   192422 2023-05-01 03:43:57.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/library.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   182102 2023-05-01 03:43:57.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/navigation.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   210167 2023-01-25 16:48:46.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/questions.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)  2953775 2023-05-15 03:02:55.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/rationales.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)   275218 2023-05-01 03:43:57.000000 SALTISE_components-0.2.7.1/components/static/components/js/build/search.min.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      639 2023-02-22 04:47:56.000000 SALTISE_components-0.2.7.1/pyproject.toml
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      919 2023-05-17 04:03:58.668828 SALTISE_components-0.2.7.1/setup.cfg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       38 2023-01-24 19:01:52.000000 SALTISE_components-0.2.7.1/setup.py
```

### Comparing `SALTISE_components-0.2.7/LICENSE` & `SALTISE_components-0.2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/PKG-INFO` & `SALTISE_components-0.2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SALTISE_components
-Version: 0.2.7
+Version: 0.2.7.1
 Summary: A Django app to build and test a collection of front-end components for myDALITE
 Author: Jonathon Sumner
 Author-email: jsumner@dawsoncollege.qc.ca
 License: LICENSE.txt
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: SALTISE_components Version: 0.2.7 Summary: A Django
-app to build and test a collection of front-end components for myDALITE Author:
-Jonathon Sumner Author-email: jsumner@dawsoncollege.qc.ca License: LICENSE.txt
-Classifier: Environment :: Web Environment Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2 Classifier: Framework :: Django :: 3.2
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: BSD License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
-HTTP :: Dynamic Content License-File: LICENSE ========== components ==========
-SALTISE-components is a simple Django app to build and test a collection of
-front-end components for myDALITE built with preact and Material UI. Quick
-start ----------- 1. Add the Components app to your requirements, then pip
-install:: pip install SALTISE-components 2. Add "components" to your
-INSTALLED_APPS setting like this:: INSTALLED_APPS = [ ... 'components', ... ]
-3. Import minified script to access component library (you can override default
-styles using global css names)::
+Metadata-Version: 2.1 Name: SALTISE_components Version: 0.2.7.1 Summary: A
+Django app to build and test a collection of front-end components for myDALITE
+Author: Jonathon Sumner Author-email: jsumner@dawsoncollege.qc.ca License:
+LICENSE.txt Classifier: Environment :: Web Environment Classifier: Framework ::
+Django Classifier: Framework :: Django :: 2.2 Classifier: Framework :: Django
+:: 3.2 Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: BSD License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
+Internet :: WWW/HTTP :: Dynamic Content License-File: LICENSE ==========
+components ========== SALTISE-components is a simple Django app to build and
+test a collection of front-end components for myDALITE built with preact and
+Material UI. Quick start ----------- 1. Add the Components app to your
+requirements, then pip install:: pip install SALTISE-components 2. Add
+"components" to your INSTALLED_APPS setting like this:: INSTALLED_APPS = [ ...
+'components', ... ] 3. Import minified script to access component library (you
+can override default styles using global css names)::
  4. Inject components into the DOM, customizing props as needed. Assuming
 django-csp is installed, the Navigation components is injected via::
  Quick start dev --------------- 1. Install node modules:: npm install 2.
 Create python 3.8+ virtualenv and nstall pip-tools:: python -m pip install --
 upgrade pip pip install pip-tools 3. Install requirements:: pip-sync
 requirements/requirements.txt 4. Install pre-commit:: pre-commit install 5.
 Start the server:: python components.py runserver 6. Navigate to 'localhost:
```

### Comparing `SALTISE_components-0.2.7/README.rst` & `SALTISE_components-0.2.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/SALTISE_components.egg-info/PKG-INFO` & `SALTISE_components-0.2.7.1/SALTISE_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SALTISE-components
-Version: 0.2.7
+Version: 0.2.7.1
 Summary: A Django app to build and test a collection of front-end components for myDALITE
 Author: Jonathon Sumner
 Author-email: jsumner@dawsoncollege.qc.ca
 License: LICENSE.txt
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: SALTISE-components Version: 0.2.7 Summary: A Django
-app to build and test a collection of front-end components for myDALITE Author:
-Jonathon Sumner Author-email: jsumner@dawsoncollege.qc.ca License: LICENSE.txt
-Classifier: Environment :: Web Environment Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2 Classifier: Framework :: Django :: 3.2
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: BSD License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
-HTTP :: Dynamic Content License-File: LICENSE ========== components ==========
-SALTISE-components is a simple Django app to build and test a collection of
-front-end components for myDALITE built with preact and Material UI. Quick
-start ----------- 1. Add the Components app to your requirements, then pip
-install:: pip install SALTISE-components 2. Add "components" to your
-INSTALLED_APPS setting like this:: INSTALLED_APPS = [ ... 'components', ... ]
-3. Import minified script to access component library (you can override default
-styles using global css names)::
+Metadata-Version: 2.1 Name: SALTISE-components Version: 0.2.7.1 Summary: A
+Django app to build and test a collection of front-end components for myDALITE
+Author: Jonathon Sumner Author-email: jsumner@dawsoncollege.qc.ca License:
+LICENSE.txt Classifier: Environment :: Web Environment Classifier: Framework ::
+Django Classifier: Framework :: Django :: 2.2 Classifier: Framework :: Django
+:: 3.2 Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: BSD License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
+Internet :: WWW/HTTP :: Dynamic Content License-File: LICENSE ==========
+components ========== SALTISE-components is a simple Django app to build and
+test a collection of front-end components for myDALITE built with preact and
+Material UI. Quick start ----------- 1. Add the Components app to your
+requirements, then pip install:: pip install SALTISE-components 2. Add
+"components" to your INSTALLED_APPS setting like this:: INSTALLED_APPS = [ ...
+'components', ... ] 3. Import minified script to access component library (you
+can override default styles using global css names)::
  4. Inject components into the DOM, customizing props as needed. Assuming
 django-csp is installed, the Navigation components is injected via::
  Quick start dev --------------- 1. Install node modules:: npm install 2.
 Create python 3.8+ virtualenv and nstall pip-tools:: python -m pip install --
 upgrade pip pip install pip-tools 3. Install requirements:: pip-sync
 requirements/requirements.txt 4. Install pre-commit:: pre-commit install 5.
 Start the server:: python components.py runserver 6. Navigate to 'localhost:
```

### Comparing `SALTISE_components-0.2.7/SALTISE_components.egg-info/SOURCES.txt` & `SALTISE_components-0.2.7.1/SALTISE_components.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 components/apps.py
 components/static/components/img/avatar.jpg
 components/static/components/img/collection-placeholder.svg
 components/static/components/img/logo.gif
 components/static/components/img/logo.png
 components/static/components/img/logo.svg
 components/static/components/img/vector-search.svg
+components/static/components/js/build/createAssignment.min.js
 components/static/components/js/build/createQuestions1.min.js
 components/static/components/js/build/createQuestions2.min.js
 components/static/components/js/build/dashboard.min.js
 components/static/components/js/build/dashboardInvitedUser.min.js
 components/static/components/js/build/dashboardNewUser.min.js
 components/static/components/js/build/dashboardStudent.min.js
 components/static/components/js/build/library.min.js
 components/static/components/js/build/navigation.min.js
 components/static/components/js/build/questions.min.js
+components/static/components/js/build/rationales.min.js
 components/static/components/js/build/search.min.js
```

### Comparing `SALTISE_components-0.2.7/components/static/components/img/avatar.jpg` & `SALTISE_components-0.2.7.1/components/static/components/img/avatar.jpg`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/img/collection-placeholder.svg` & `SALTISE_components-0.2.7.1/components/static/components/img/collection-placeholder.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/img/logo.gif` & `SALTISE_components-0.2.7.1/components/static/components/img/logo.gif`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/img/logo.png` & `SALTISE_components-0.2.7.1/components/static/components/img/logo.png`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/img/logo.svg` & `SALTISE_components-0.2.7.1/components/static/components/img/logo.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/img/vector-search.svg` & `SALTISE_components-0.2.7.1/components/static/components/img/vector-search.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/js/build/createQuestions1.min.js` & `SALTISE_components-0.2.7.1/components/static/components/js/build/createQuestions1.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/js/build/createQuestions2.min.js` & `SALTISE_components-0.2.7.1/components/static/components/js/build/createQuestions2.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/js/build/dashboard.min.js` & `SALTISE_components-0.2.7.1/components/static/components/js/build/dashboard.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/js/build/dashboardInvitedUser.min.js` & `SALTISE_components-0.2.7.1/components/static/components/js/build/dashboardInvitedUser.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/js/build/dashboardNewUser.min.js` & `SALTISE_components-0.2.7.1/components/static/components/js/build/dashboardNewUser.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/js/build/dashboardStudent.min.js` & `SALTISE_components-0.2.7.1/components/static/components/js/build/dashboardStudent.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4822,77 +4822,73 @@
                 fontSize: "36px",
                 lineHeight: "49px",
                 marginTop: "30px",
                 marginBottom: "30px"
             },
             h2: {
                 fontSize: "20px",
-                fontWeight: 600,
+                fontWeight: 500,
                 lineHeight: "28px",
                 marginTop: "50px"
             },
             h3: {
                 fontSize: "16px",
-                fontWeight: 600,
+                fontWeight: 500,
                 lineHeight: "28px"
             },
             h4: {
                 fontSize: "14px",
                 lineHeight: "20px"
             },
             h5: {
                 fontSize: "14px",
-                fontWeight: 600,
+                fontWeight: 500,
                 lineHeight: "19px"
             },
             caption: {
                 fontSize: "10px",
                 lineHeight: "22px",
                 color: "#90929B"
             }
         },
         components: {
             MuiAppBar: {
                 styleOverrides: {
                     root: {
-                        backgroundColor: "#000B26",
-                        color: "#fff",
+                        backgroundColor: "#FFF",
+                        color: "#1743B3",
                         paddingLeft: 2,
-                        " img.logo": {
-                            height: 40,
-                            marginRight: 10
-                        },
                         " .MuiAvatar-root": {
                             height: 30,
-                            width: 30
+                            width: 30,
+                            "&:hover": {
+                                backgroundColor: "#1743B320"
+                            }
                         },
                         " .MuiIconButton-root": {
                             marginLeft: "15px",
                             marginRight: "15px",
-                            color: "#fff"
+                            color: "#1743B3",
+                            "&:hover": {
+                                backgroundColor: "#1743B320"
+                            }
                         },
                         " .MuiList-root": {
                             padding: "10px 0px"
                         },
                         " .MuiListItemButton-root": {
                             padding: "3px 17px",
                             color: "rgb(185 208 228)",
                             "&:hover": {
                                 backgroundColor: "#E9F5FF"
                             }
                         },
                         " .MuiListItemIcon-root": {
                             minWidth: "0px",
                             marginRight: "10px"
-                        },
-                        " span.cardo": {
-                            fontFamily: "Cardo"
-                        },
-                        " span.montserrat": {
-                            fontFamily: "Montserrat"
                         }
                     }
                 }
             },
             MuiButton: {
                 styleOverrides: {
                     sizeSmall: {
@@ -4923,49 +4919,50 @@
                         }
                     }
                 }
             },
             MuiCard: {
                 styleOverrides: {
                     root: {
-                        padding: "20px 20px",
                         borderRadius: "10px",
                         boxShadow: "none"
                     }
                 }
             },
             MuiCardContent: {
                 styleOverrides: {
                     root: {
-                        padding: "10px 0px 10px 0px"
+                        padding: "0px 20px"
                     }
                 }
             },
             MuiCardHeader: {
                 styleOverrides: {
                     root: {
-                        padding: "0px"
+                        padding: "20px"
                     },
                     title: {
                         fontSize: "16px",
-                        fontWeight: "600",
+                        fontWeight: 500,
                         lineHeight: "28px",
                         color: "#515159"
                     },
                     subheader: {
                         fontSize: "10px",
                         lineHeight: "20px",
                         color: "#90929B"
                     }
                 }
             },
             MuiCardActions: {
                 styleOverrides: {
                     root: {
-                        padding: "0px"
+                        height: "26px",
+                        justifyContent: "space-between",
+                        padding: "20px"
                     }
                 }
             },
             MuiDivider: {
                 styleOverrides: {
                     root: {
                         borderColor: "rgb(255, 255, 255, 0.1)"
@@ -4981,26 +4978,43 @@
                 styleOverrides: {
                     paper: {
                         padding: "20px 10px",
                         backgroundColor: "#0D2666",
                         color: "#fff"
                     },
                     root: {
+                        " img.logo": {
+                            height: 40,
+                            marginLeft: 8,
+                            marginRight: 10,
+                            width: 40
+                        },
+                        " span.cardo": {
+                            fontFamily: "Cardo"
+                        },
+                        " span.montserrat": {
+                            fontFamily: "Montserrat"
+                        },
                         " .MuiListItemButton-root": {
                             borderRadius: 10,
+                            marginBottom: 2,
                             padding: "4px 16px",
+                            "&.Mui-selected": {
+                                backgroundColor: "rgb(255, 255, 255, 0.1)"
+                            },
                             "&:hover": {
                                 backgroundColor: "rgb(255, 255, 255, 0.1)"
                             }
                         },
                         " .MuiListItemIcon-root": {
                             color: "#fff"
                         },
                         " .MuiTypography-root": {
-                            color: "#fff"
+                            color: "#fff",
+                            fontSize: "0.9rem"
                         }
                     }
                 }
             },
             MuiIconButton: {
                 styleOverrides: {
                     root: {
@@ -5072,15 +5086,15 @@
                     }
                 }
             },
             MuiCardHeader: {
                 styleOverrides: {
                     title: {
                         fontSize: "18px",
-                        fontWeight: "600",
+                        fontWeight: 500,
                         lineHeight: "28px"
                     },
                     subheader: {
                         fontSize: "10px",
                         lineHeight: "20px",
                         color: "#90929B"
                     }
@@ -6649,16 +6663,18 @@
             display: "flex",
             justifyContent: "space-between",
             alignItems: "flex-end",
             marginBottom: "20px"
         }),
         Cs = zt(Mt)({
             color: Bs.palette.secondary4.main,
+            cursor: "default",
             backgroundColor: Bs.palette.secondary1.main,
             borderRadius: "5px",
+            borderWidth: "1px",
             display: "flex",
             padding: "5px",
             alignItems: "center",
             " .MuiTypography-root": {
                 fontSize: "12px",
                 lineHeight: "16px"
             },
@@ -6805,17 +6821,19 @@
 
     function Ws(e) {
         let {
             gettext: gettext,
             assignment: a
         } = e;
         const i = (e => {
-            const a = new Date,
-                i = (e.getTime() - a.getTime()) / 864e5;
-            return Math.round(Math.abs(i))
+            if (e) {
+                const a = new Date,
+                    i = (e.getTime() - a.getTime()) / 864e5;
+                return Math.round(Math.abs(i))
+            }
         })(a.dueDate);
         return k($l, null, k(Mt, {
             display: "flex",
             justifyContent: "space-between"
         }, k(Mt, null, k(Vt, {
             variant: "h3"
         }, a.title)), k(Mt, {
@@ -25974,75 +25992,63 @@
         }), "Science");
     let HA, RA, DA, GA, _A, VA;
     TA.default = NA,
         function(e) {
             e[e.un = 1] = "un", e[e.deux = 2] = "deux", e[e.trois = 3] = "trois", e[e.quatre = 4] = "quatre"
         }(HA || (HA = {})),
         function(e) {
-            e.easy = "Easy", e.moderate = "Moderate", e.difficult = "Difficult", e.extreme = "Extreme"
+            e.easy = "Easy", e.moderate = "Avg", e.difficult = "Hard", e.unknown = "Not enough data"
         }(RA || (RA = {})),
         function(e) {
-            e[e.zero = 0] = "zero", e[e.un = 1] = "un", e[e.deux = 2] = "deux", e[e.trois = 3] = "trois"
+            e[e.un = 1] = "un", e[e.deux = 2] = "deux", e[e.trois = 3] = "trois", e[e.quatre = 4] = "quatre"
         }(DA || (DA = {})),
         function(e) {
             e.draft = "Draft", e.distributed = "Distributed"
         }(GA || (GA = {})),
         function(e) {
             e.question = "Question", e.group = "Group", e.collection = "Collection", e.assignment = "Assignment"
         }(_A || (_A = {})),
         function(e) {
             e.zero = "0", e.un = "1", e.deux = "2", e.trois = "3"
         }(VA || (VA = {}));
     const EA = [{
+            active: !0,
             author: hA.name.fullName(),
             creationDate: hA.date.recent(),
             difficulty: hA.helpers.arrayElement([RA.easy, RA.moderate, RA.difficult]),
             distributionState: hA.helpers.arrayElement([GA.draft, GA.distributed]),
             dueDate: hA.date.soon(),
-            groups: [],
+            group: {},
             questionCount: parseInt(hA.random.numeric(1)),
             title: hA.lorem.sentence(),
             issueCount: parseInt(hA.random.numeric(1)),
             progress: parseInt(hA.random.numeric(1)),
             answerCount: parseInt(hA.random.numeric(1))
         }, {
+            active: !0,
             author: hA.name.fullName(),
             creationDate: hA.date.recent(),
             difficulty: hA.helpers.arrayElement([RA.easy, RA.moderate, RA.difficult]),
             distributionState: hA.helpers.arrayElement([GA.draft, GA.distributed]),
             dueDate: hA.date.soon(),
-            groups: [{
+            group: {
                 title: hA.lorem.sentence(),
                 author: hA.name.fullName(),
                 session: hA.helpers.arrayElement(["Summer 2022", "Winter 2023"]),
                 studentCount: parseInt(hA.random.numeric(1)),
                 assignmentCount: parseInt(hA.random.numeric(1)),
                 active: hA.datatype.boolean(),
                 subject: hA.helpers.arrayElement([
                     ["Biology"],
                     ["Biology", "Cohesion"],
                     ["Mechanic", "Programming", "Thermodynamic"]
                 ]),
                 dueDate: hA.date.soon(),
                 progress: parseInt(hA.random.numeric(2))
-            }, {
-                title: hA.lorem.sentence(),
-                author: hA.name.fullName(),
-                session: hA.helpers.arrayElement(["Summer 2022", "Winter 2023"]),
-                studentCount: parseInt(hA.random.numeric(1)),
-                assignmentCount: parseInt(hA.random.numeric(1)),
-                active: hA.datatype.boolean(),
-                subject: hA.helpers.arrayElement([
-                    ["Biology"],
-                    ["Biology", "Cohesion"],
-                    ["Mechanic", "Programming", "Thermodynamic"]
-                ]),
-                dueDate: hA.date.soon(),
-                progress: parseInt(hA.random.numeric(2))
-            }],
+            },
             questionCount: parseInt(hA.random.numeric(1)),
             title: hA.lorem.sentence(),
             issueCount: parseInt(hA.random.numeric(1)),
             progress: parseInt(hA.random.numeric(1)),
             answerCount: parseInt(hA.random.numeric(1))
         }],
         JA = [{
@@ -26050,99 +26056,179 @@
             author: hA.name.fullName(),
             description: hA.lorem.sentence(),
             answerCount: parseInt(hA.random.numeric(1)),
             tags: hA.helpers.arrayElement([
                 ["Biology"],
                 ["Biology", "Cohesion"],
                 ["Mechanic", "Programming", "Thermodynamic"]
-            ])
+            ]),
+            url: "/"
         }, {
             title: hA.lorem.sentence(),
             author: hA.name.fullName(),
             description: hA.lorem.sentence(),
             answerCount: parseInt(hA.random.numeric(1)),
             tags: hA.helpers.arrayElement([
                 ["Biology"],
                 ["Biology", "Cohesion"],
                 ["Mechanic", "Programming", "Thermodynamic"]
-            ])
+            ]),
+            url: "/"
         }],
         FA = [{
-            answerCount: parseInt(hA.random.numeric(1)),
+            answer_count: parseInt(hA.random.numeric(1)),
             title: hA.lorem.sentence(),
             user: {
                 username: hA.name.fullName()
             },
-            description: hA.lorem.sentence(),
-            tags: hA.helpers.arrayElement([
-                ["Biology"],
-                ["Biology", "Cohesion"],
-                ["Mechanic", "Programming", "Thermodynamic"]
+            text: hA.lorem.sentence(),
+            discipline: {
+                pk: 1,
+                title: "Physics"
+            },
+            category: hA.helpers.arrayElement([
+                [{
+                    title: "Biology"
+                }],
+                [{
+                    title: "Biology"
+                }, {
+                    title: "Cohesion"
+                }],
+                [{
+                    title: "Mechanic"
+                }, {
+                    title: "Programming"
+                }, {
+                    title: "Thermodynamic"
+                }]
             ]),
             difficulty: {
                 score: .4,
                 value: HA.deux,
                 label: RA.moderate
             },
             peer_impact: hA.helpers.arrayElement([0, 1, 2, 3])
         }, {
-            answerCount: parseInt(hA.random.numeric(2)),
+            answer_count: parseInt(hA.random.numeric(2)),
             title: hA.lorem.sentence(),
             user: {
                 username: hA.name.fullName()
             },
-            description: hA.lorem.sentence(),
-            tags: hA.helpers.arrayElement([
-                ["Biology"],
-                ["Biology", "Cohesion"],
-                ["Mechanic", "Programming", "Thermodynamic"]
+            text: hA.lorem.sentence(),
+            discipline: {
+                pk: 1,
+                title: "Physics"
+            },
+            category: hA.helpers.arrayElement([
+                [{
+                    title: "Biology"
+                }],
+                [{
+                    title: "Biology"
+                }, {
+                    title: "Cohesion"
+                }],
+                [{
+                    title: "Mechanic"
+                }, {
+                    title: "Programming"
+                }, {
+                    title: "Thermodynamic"
+                }]
             ]),
             peer_impact: hA.helpers.arrayElement([0, 1, 2, 3]),
             difficulty: {
                 score: .7,
                 value: HA.trois,
                 label: RA.difficult
             }
         }, {
-            answerCount: parseInt(hA.random.numeric(1)),
+            answer_count: parseInt(hA.random.numeric(1)),
             title: hA.lorem.sentence(),
             user: {
                 username: hA.name.fullName()
             },
-            description: hA.lorem.sentence(),
-            tags: hA.helpers.arrayElement([
-                ["Biology"],
-                ["Biology", "Cohesion"],
-                ["Mechanic", "Programming", "Thermodynamic"]
+            text: hA.lorem.sentence(),
+            discipline: {
+                pk: 1,
+                title: "Physics"
+            },
+            category: hA.helpers.arrayElement([
+                [{
+                    title: "Biology"
+                }],
+                [{
+                    title: "Biology"
+                }, {
+                    title: "Cohesion"
+                }],
+                [{
+                    title: "Mechanic"
+                }, {
+                    title: "Programming"
+                }, {
+                    title: "Thermodynamic"
+                }]
             ]),
             peer_impact: hA.helpers.arrayElement([0, 1, 2, 3]),
             difficulty: {
                 score: .1,
                 value: HA.un,
                 label: RA.easy
             }
         }],
-        IA = {
+        IA = [{
+            title: hA.lorem.sentence(),
+            author: hA.name.fullName(),
+            session: hA.helpers.arrayElement(["Summer 2022", "Winter 2023", "Spring 2023"]),
+            studentCount: parseInt(hA.random.numeric(1)),
+            assignmentCount: parseInt(hA.random.numeric(1)),
+            active: hA.datatype.boolean(),
+            subject: hA.helpers.arrayElement([
+                ["Biology"],
+                ["Biology", "Cohesion"],
+                ["Mechanic", "Programming", "Thermodynamic"]
+            ]),
+            dueDate: hA.date.soon(),
+            progress: parseInt(hA.random.numeric(2))
+        }, {
+            title: hA.lorem.sentence(),
+            author: hA.name.fullName(),
+            session: hA.helpers.arrayElement(["Summer 2022", "Winter 2023", "Spring 2023"]),
+            studentCount: parseInt(hA.random.numeric(1)),
+            assignmentCount: parseInt(hA.random.numeric(1)),
+            active: hA.datatype.boolean(),
+            subject: hA.helpers.arrayElement([
+                ["Biology"],
+                ["Biology", "Cohesion"],
+                ["Mechanic", "Programming", "Thermodynamic"]
+            ]),
+            dueDate: hA.date.soon(),
+            progress: parseInt(hA.random.numeric(2))
+        }],
+        OA = {
             activeAssignmentCount: 4,
             activeGroupCount: 3,
             createdQuestionCount: 12
         };
-    parseInt(hA.random.numeric(1)), _A.assignment, _A.collection, _A.group, _A.question, parseInt(hA.random.numeric(1)), parseInt(hA.random.numeric(2)), parseInt(hA.random.numeric(1)), RA.easy, RA.moderate, RA.difficult, RA.extreme, parseInt(hA.random.numeric(2)), VA.zero, VA.un, VA.deux, VA.trois;
+    parseInt(hA.random.numeric(1)), _A.assignment, _A.collection, _A.group, _A.question, parseInt(hA.random.numeric(1)), parseInt(hA.random.numeric(2)), parseInt(hA.random.numeric(1)), RA.easy, RA.moderate, RA.difficult, RA.unknown, parseInt(hA.random.numeric(2)), VA.zero, VA.un, VA.deux, VA.trois;
     e.App = class extends v {
         constructor(e) {
             super(e), a(this, "cache", Qi({
                 key: "nonced",
                 nonce: this.props.nonce,
                 prepend: !0,
                 stylisPlugins: [Ii]
             })), this.state = {
                 assignments: EA,
                 collections: JA,
                 questions: FA,
-                teacher: IA
+                teacher: OA,
+                groups: IA
             }
         }
         componentDidMount() {}
         render() {
             return k(Ro, {
                 theme: Xt
             }, k(Vn, {
```

### Comparing `SALTISE_components-0.2.7/components/static/components/js/build/library.min.js` & `SALTISE_components-0.2.7.1/components/static/components/js/build/library.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/js/build/navigation.min.js` & `SALTISE_components-0.2.7.1/components/static/components/js/build/navigation.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/js/build/questions.min.js` & `SALTISE_components-0.2.7.1/components/static/components/js/build/questions.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/components/static/components/js/build/search.min.js` & `SALTISE_components-0.2.7.1/components/static/components/js/build/search.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/pyproject.toml` & `SALTISE_components-0.2.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SALTISE_components-0.2.7/setup.cfg` & `SALTISE_components-0.2.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SALTISE_components
-version = 0.2.7
+version = 0.2.7.1
 description = A Django app to build and test a collection of front-end components for myDALITE
 long_description = file: README.rst
 author = Jonathon Sumner
 author_email = jsumner@dawsoncollege.qc.ca
 license = LICENSE.txt
 classifiers = 
 	Environment :: Web Environment
```

