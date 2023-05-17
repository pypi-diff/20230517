# Comparing `tmp/flask_management-0.1.3.tar.gz` & `tmp/flask_management-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_management-0.1.3.tar", max compression
+gzip compressed data, was "flask_management-0.1.4.tar", max compression
```

## Comparing `flask_management-0.1.3.tar` & `flask_management-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-05-15 07:20:16.429166 flask_management-0.1.3/LICENSE
--rw-r--r--   0        0        0      186 2023-05-15 07:52:15.971213 flask_management-0.1.3/README.md
--rw-r--r--   0        0        0       45 2023-05-15 07:20:44.714318 flask_management-0.1.3/flask_management/__main__.py
--rw-r--r--   0        0        0      659 2023-05-15 07:20:44.699986 flask_management-0.1.3/flask_management/constants.py
--rw-r--r--   0        0        0     1102 2023-05-15 07:20:44.703599 flask_management-0.1.3/flask_management/context.py
--rw-r--r--   0        0        0      862 2023-05-15 07:20:44.703127 flask_management-0.1.3/flask_management/generator.py
--rw-r--r--   0        0        0      559 2023-05-15 07:20:44.713851 flask_management-0.1.3/flask_management/main.py
--rw-r--r--   0        0        0        0 2023-05-15 07:20:44.704460 flask_management-0.1.3/flask_management/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 07:20:44.705010 flask_management-0.1.3/flask_management/templates/project/__init__.py
--rw-r--r--   0        0        0      344 2023-05-15 07:20:44.705440 flask_management-0.1.3/flask_management/templates/project/cookiecutter.json
--rw-r--r--   0        0        0     2058 2023-05-15 07:20:44.712954 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore
--rw-r--r--   0        0        0       25 2023-05-15 07:20:44.712191 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/README.md
--rw-r--r--   0        0        0      686 2023-05-15 07:20:44.711148 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml
--rw-r--r--   0        0        0      283 2023-05-15 07:20:44.713408 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-15 07:20:44.711861 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/tests/__init__.py
--rw-r--r--   0        0        0      418 2023-05-15 07:20:44.708330 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/__init__.py
--rw-r--r--   0        0        0      206 2023-05-15 07:20:44.706995 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/app_settings.py
--rw-r--r--   0        0        0      162 2023-05-15 07:20:44.709400 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/book/__init__.py
--rw-r--r--   0        0        0      120 2023-05-15 07:20:44.709994 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/book/api.py
--rw-r--r--   0        0        0      278 2023-05-15 07:20:44.710804 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/ext.py
--rw-r--r--   0        0        0      414 2023-05-15 07:20:44.707497 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/models.py
--rw-r--r--   0        0        0      216 2023-05-15 07:20:44.706410 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/signals.py
--rw-r--r--   0        0        0       78 2023-05-15 07:20:44.712473 flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.env }}
--rw-r--r--   0        0        0      673 2023-05-15 08:03:14.800709 flask_management-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 flask_management-0.1.3/setup.py
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 flask_management-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 07:20:16.429166 flask_management-0.1.4/LICENSE
+-rw-r--r--   0        0        0      186 2023-05-15 08:04:24.922081 flask_management-0.1.4/README.md
+-rw-r--r--   0        0        0       45 2023-05-15 07:20:44.714318 flask_management-0.1.4/flask_management/__main__.py
+-rw-r--r--   0        0        0      659 2023-05-15 07:20:44.699986 flask_management-0.1.4/flask_management/constants.py
+-rw-r--r--   0        0        0     1102 2023-05-15 07:20:44.703599 flask_management-0.1.4/flask_management/context.py
+-rw-r--r--   0        0        0     1318 2023-05-15 08:09:53.291424 flask_management-0.1.4/flask_management/main.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:20:44.704460 flask_management-0.1.4/flask_management/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:20:44.705010 flask_management-0.1.4/flask_management/templates/project/__init__.py
+-rw-r--r--   0        0        0      344 2023-05-15 07:20:44.705440 flask_management-0.1.4/flask_management/templates/project/cookiecutter.json
+-rw-r--r--   0        0        0     2058 2023-05-15 07:20:44.712954 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore
+-rw-r--r--   0        0        0       25 2023-05-15 07:20:44.712191 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/README.md
+-rw-r--r--   0        0        0      702 2023-05-17 07:36:14.503897 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-05-15 07:20:44.713408 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-15 07:20:44.711861 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/tests/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-15 07:20:44.708330 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-15 07:20:44.706995 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/app_settings.py
+-rw-r--r--   0        0        0      163 2023-05-15 08:09:53.286874 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/book/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-15 07:20:44.709994 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/book/api.py
+-rw-r--r--   0        0        0      278 2023-05-15 07:20:44.710804 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/ext.py
+-rw-r--r--   0        0        0      414 2023-05-15 07:20:44.707497 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/models.py
+-rw-r--r--   0        0        0      216 2023-05-15 07:20:44.706410 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/signals.py
+-rw-r--r--   0        0        0       78 2023-05-15 07:20:44.712473 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.env }}
+-rw-r--r--   0        0        0      673 2023-05-17 07:36:53.851084 flask_management-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 flask_management-0.1.4/setup.py
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 flask_management-0.1.4/PKG-INFO
```

### Comparing `flask_management-0.1.3/LICENSE` & `flask_management-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.3/flask_management/constants.py` & `flask_management-0.1.4/flask_management/constants.py`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.3/flask_management/context.py` & `flask_management-0.1.4/flask_management/context.py`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore` & `flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.3/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml` & `flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 [[tool.poetry.source]]
 name = "tuna"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple"
 default = true
 
 [tool.poetry.dependencies]
 python = "^{{ cookiecutter.python }}"
+
 flask = "*"
 blinker = "*"
 flask_migrate = "*"
 flask_sqlalchemy = "*"
+pydantic = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 pytest-cov = "^2.10.1"
 autoflake = "^1.4"
 flake8 = "^3.8.4"
 mypy = "^0.790"
```

### Comparing `flask_management-0.1.3/pyproject.toml` & `flask_management-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-management"
-version = "0.1.3"
+version = "0.1.4"
 description = "create the flask project quickly."
 authors = ["huangsong <huangsong@leyantech.com>"]
 readme = "README.md"
 packages = [{ include = "flask_management" }]
 homepage = "https://github.com/ponytailer/flask-management"
 
 [[tool.poetry.source]]
```

### Comparing `flask_management-0.1.3/setup.py` & `flask_management-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ['cookiecutter>=1.7.2', 'pydantic[email]>=1.7.2', 'typer']
 
 entry_points = \
 {'console_scripts': ['flaskapi = flask_management.main:app']}
 
 setup_kwargs = {
     'name': 'flask-management',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'create the flask project quickly.',
     'long_description': '# flask-management\n\n## How to use :\n\n- simple command: `flaskapi your-project-name`\n\n- choose your python version: `flaskapi your-project-name --python 3.7`\n\nInspired by `manage-fastapi`',
     'author': 'huangsong',
     'author_email': 'huangsong@leyantech.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ponytailer/flask-management',
```

### Comparing `flask_management-0.1.3/PKG-INFO` & `flask_management-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-management
-Version: 0.1.3
+Version: 0.1.4
 Summary: create the flask project quickly.
 Home-page: https://github.com/ponytailer/flask-management
 Author: huangsong
 Author-email: huangsong@leyantech.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

