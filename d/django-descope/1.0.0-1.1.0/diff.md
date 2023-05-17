# Comparing `tmp/django_descope-1.0.0.tar.gz` & `tmp/django_descope-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_descope-1.0.0.tar", max compression
+gzip compressed data, was "django_descope-1.1.0.tar", max compression
```

## Comparing `django_descope-1.0.0.tar` & `django_descope-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-04-21 17:51:35.225006 django_descope-1.0.0/LICENSE
--rw-r--r--   0        0        0     1715 2023-04-21 17:51:35.225006 django_descope-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/__init__.py
--rw-r--r--   0        0        0       96 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/apps.py
--rw-r--r--   0        0        0     1910 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/authentication.py
--rw-r--r--   0        0        0      638 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/middleware.py
--rw-r--r--   0        0        0      666 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/migrations/__init__.py
--rw-r--r--   0        0        0     1367 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/models.py
--rw-r--r--   0        0        0      576 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/settings.py
--rw-r--r--   0        0        0        0 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/templatetags/__init__.py
--rw-r--r--   0        0        0     1619 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/templatetags/descope.py
--rw-r--r--   0        0        0      165 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/urls.py
--rw-r--r--   0        0        0     1045 2023-04-21 17:51:35.225006 django_descope-1.0.0/django_descope/views.py
--rw-r--r--   0        0        0     2503 2023-04-21 17:52:04.729319 django_descope-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 django_descope-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-17 07:33:56.354577 django_descope-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1715 2023-05-17 07:33:56.354577 django_descope-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/__init__.py
+-rw-r--r--   0        0        0       96 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/apps.py
+-rw-r--r--   0        0        0     1910 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/authentication.py
+-rw-r--r--   0        0        0      544 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/middleware.py
+-rw-r--r--   0        0        0      666 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/migrations/__init__.py
+-rw-r--r--   0        0        0     1367 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/models.py
+-rw-r--r--   0        0        0      576 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/settings.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/templatetags/__init__.py
+-rw-r--r--   0        0        0     1619 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/templatetags/descope.py
+-rw-r--r--   0        0        0      165 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/urls.py
+-rw-r--r--   0        0        0     1045 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/views.py
+-rw-r--r--   0        0        0     2512 2023-05-17 07:34:30.222324 django_descope-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 django_descope-1.1.0/PKG-INFO
```

### Comparing `django_descope-1.0.0/LICENSE` & `django_descope-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_descope-1.0.0/README.md` & `django_descope-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 - Create two roles in Descope, that will be mapped to Django permissions
   - is_staff
   - is_superuser
 
 Map these roles to any user you would like to make a staff or superuser in your Django app.
 _The names of these roles can be customized in the settings below._
 
-2. Install "django_descope" and add to your INSTALLED_APPS setting like this:
+2. Install "django-descope" and add to your INSTALLED_APPS setting like this:
 
 ```bash
-poetry add django_descope
+poetry add django-descope
 OR
-pip install django_descope
+pip install django-descope
 ```
 
 ```
    INSTALLED_APPS = [
    ...
    'django_descope',
    ]
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # Descope Django App Descope is a user management and authentication platform.
 This plugin integrates Descope with your Django app. ## Quick start 1. Sign up
 for Descope and set admin roles - Get your project id - Create two roles in
 Descope, that will be mapped to Django permissions - is_staff - is_superuser
 Map these roles to any user you would like to make a staff or superuser in your
 Django app. _The names of these roles can be customized in the settings below._
-2. Install "django_descope" and add to your INSTALLED_APPS setting like this:
-```bash poetry add django_descope OR pip install django_descope ``` ```
+2. Install "django-descope" and add to your INSTALLED_APPS setting like this:
+```bash poetry add django-descope OR pip install django-descope ``` ```
 INSTALLED_APPS = [ ... 'django_descope', ] ``` 3. Add Descope Middleware
 **after** the SessionMiddleware ``` MIDDLEWARE = [ ...
 'django.contrib.sessions.middleware.SessionMiddleware', ...
 'django_descope.middleware.DescopeMiddleware', ] ``` 4. Include descope URLconf
 in your project urls.py like this: ``` path('auth/', include
 ('django_descope.urls')), ``` 5. In your site templates, insert the
 `descope_flow` tag where you want to place your flow ```html {% load descope %}
```

### Comparing `django_descope-1.0.0/django_descope/authentication.py` & `django_descope-1.1.0/django_descope/authentication.py`

 * *Files identical despite different names*

### Comparing `django_descope-1.0.0/django_descope/middleware.py` & `django_descope-1.1.0/django_descope/middleware.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,11 @@
 class DescopeMiddleware:
     _auth = DescopeAuthentication()
 
     def __init__(self, get_response: HttpResponse = None):
         self.get_response = get_response
 
     def __call__(self, request: HttpRequest):
-        response: HttpResponse = self.get_response(request)
-
         user = self._auth.authenticate(request)
         if user:
             login(request, user)
-            response = self.get_response(request)
-
-        return response
+        return self.get_response(request)
```

### Comparing `django_descope-1.0.0/django_descope/migrations/0001_initial.py` & `django_descope-1.1.0/django_descope/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_descope-1.0.0/django_descope/models.py` & `django_descope-1.1.0/django_descope/models.py`

 * *Files identical despite different names*

### Comparing `django_descope-1.0.0/django_descope/settings.py` & `django_descope-1.1.0/django_descope/settings.py`

 * *Files identical despite different names*

### Comparing `django_descope-1.0.0/django_descope/templatetags/descope.py` & `django_descope-1.1.0/django_descope/templatetags/descope.py`

 * *Files identical despite different names*

### Comparing `django_descope-1.0.0/django_descope/views.py` & `django_descope-1.1.0/django_descope/views.py`

 * *Files identical despite different names*

### Comparing `django_descope-1.0.0/pyproject.toml` & `django_descope-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1,<2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django_descope"
-version = "v1.0.0"
+version = "v1.1.0"
 description = "Descope plugin for Django"
 readme = "README.md"
 authors = ["Descope <info@descope.com>"]
 repository = "https://github.com/descope/django-descope"
 documentation = "https://docs.descope.com"
 keywords = ["descope", "jwt", "authentication", "django"]
 license = "MIT"
@@ -36,22 +36,22 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-Django = "==4.2"
-descope = "1.1.1"
+Django = ">=3.2.19,<4.3"
+descope = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "6.0.0"
 black = "23.3.0"
-pre-commit = "3.2.1"
-liccheck = "0.8.3"
+pre-commit = "3.3.1"
+liccheck = "0.9.0"
 isort = "5.12.0"
 python-dotenv = "1.0.0"
 tox = "4.4.8"
 django-debug-toolbar = "3.8.1"
 
 # Authorized and unauthorized licenses in LOWER CASE
 [tool.liccheck]
```

### Comparing `django_descope-1.0.0/PKG-INFO` & `django_descope-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-descope
-Version: 1.0.0
+Version: 1.1.0
 Summary: Descope plugin for Django
 Home-page: https://github.com/descope/django-descope
 License: MIT
 Keywords: descope,jwt,authentication,django
 Author: Descope
 Author-email: info@descope.com
 Requires-Python: >=3.8.1,<4.0
@@ -25,16 +25,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Dist: Django (==4.2)
-Requires-Dist: descope (==1.1.1)
+Requires-Dist: Django (>=3.2.19,<4.3)
+Requires-Dist: descope (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://docs.descope.com
 Project-URL: Repository, https://github.com/descope/django-descope
 Description-Content-Type: text/markdown
 
 # Descope Django App
 
 Descope is a user management and authentication platform.
@@ -48,20 +48,20 @@
 - Create two roles in Descope, that will be mapped to Django permissions
   - is_staff
   - is_superuser
 
 Map these roles to any user you would like to make a staff or superuser in your Django app.
 _The names of these roles can be customized in the settings below._
 
-2. Install "django_descope" and add to your INSTALLED_APPS setting like this:
+2. Install "django-descope" and add to your INSTALLED_APPS setting like this:
 
 ```bash
-poetry add django_descope
+poetry add django-descope
 OR
-pip install django_descope
+pip install django-descope
 ```
 
 ```
    INSTALLED_APPS = [
    ...
    'django_descope',
    ]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-descope Version: 1.0.0 Summary: Descope
+Metadata-Version: 2.1 Name: django-descope Version: 1.1.0 Summary: Descope
 plugin for Django Home-page: https://github.com/descope/django-descope License:
 MIT Keywords: descope,jwt,authentication,django Author: Descope Author-email:
 info@descope.com Requires-Python: >=3.8.1,<4.0 Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework :: Django ::
 4.1 Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
@@ -10,28 +10,28 @@
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
-Internet :: WWW/HTTP :: Dynamic Content Requires-Dist: Django (==4.2) Requires-
-Dist: descope (==1.1.1) Project-URL: Documentation, https://docs.descope.com
-Project-URL: Repository, https://github.com/descope/django-descope Description-
-Content-Type: text/markdown # Descope Django App Descope is a user management
-and authentication platform. This plugin integrates Descope with your Django
-app. ## Quick start 1. Sign up for Descope and set admin roles - Get your
-project id - Create two roles in Descope, that will be mapped to Django
-permissions - is_staff - is_superuser Map these roles to any user you would
-like to make a staff or superuser in your Django app. _The names of these roles
-can be customized in the settings below._ 2. Install "django_descope" and add
-to your INSTALLED_APPS setting like this: ```bash poetry add django_descope OR
-pip install django_descope ``` ``` INSTALLED_APPS = [ ... 'django_descope', ]
-``` 3. Add Descope Middleware **after** the SessionMiddleware ``` MIDDLEWARE =
-[ ... 'django.contrib.sessions.middleware.SessionMiddleware', ...
+Internet :: WWW/HTTP :: Dynamic Content Requires-Dist: Django (>=3.2.19,<4.3)
+Requires-Dist: descope (>=1.0.0,<2.0.0) Project-URL: Documentation, https://
+docs.descope.com Project-URL: Repository, https://github.com/descope/django-
+descope Description-Content-Type: text/markdown # Descope Django App Descope is
+a user management and authentication platform. This plugin integrates Descope
+with your Django app. ## Quick start 1. Sign up for Descope and set admin roles
+- Get your project id - Create two roles in Descope, that will be mapped to
+Django permissions - is_staff - is_superuser Map these roles to any user you
+would like to make a staff or superuser in your Django app. _The names of these
+roles can be customized in the settings below._ 2. Install "django-descope" and
+add to your INSTALLED_APPS setting like this: ```bash poetry add django-descope
+OR pip install django-descope ``` ``` INSTALLED_APPS = [ ... 'django_descope',
+] ``` 3. Add Descope Middleware **after** the SessionMiddleware ``` MIDDLEWARE
+= [ ... 'django.contrib.sessions.middleware.SessionMiddleware', ...
 'django_descope.middleware.DescopeMiddleware', ] ``` 4. Include descope URLconf
 in your project urls.py like this: ``` path('auth/', include
 ('django_descope.urls')), ``` 5. In your site templates, insert the
 `descope_flow` tag where you want to place your flow ```html {% load descope %}
 {% if user.is_authenticated %}
 ****** Welcome {{ user.email }} you are logged in! ******
 Log_Out
```

