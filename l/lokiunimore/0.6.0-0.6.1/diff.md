# Comparing `tmp/lokiunimore-0.6.0.tar.gz` & `tmp/lokiunimore-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokiunimore-0.6.0.tar", max compression
+gzip compressed data, was "lokiunimore-0.6.1.tar", max compression
```

## Comparing `lokiunimore-0.6.0.tar` & `lokiunimore-0.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    34523 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     3434 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/README.md
--rw-r--r--   0        0        0       22 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/config/__init__.py
--rw-r--r--   0        0        0       41 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/config/__main__.py
--rw-r--r--   0        0        0     6187 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/config/config.py
--rw-r--r--   0        0        0       22 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/matrix/__init__.py
--rw-r--r--   0        0        0      735 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/matrix/__main__.py
--rw-r--r--   0        0        0    22084 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/matrix/client.py
--rw-r--r--   0        0        0     3066 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/matrix/templates/messages.py
--rw-r--r--   0        0        0       22 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/sql/__init__.py
--rw-r--r--   0        0        0      260 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/sql/__main__.py
--rw-r--r--   0        0        0     2431 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/sql/tables.py
--rw-r--r--   0        0        0      348 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/utils/device_names.py
--rw-r--r--   0        0        0      888 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/utils/logs.py
--rw-r--r--   0        0        0       19 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/web/__init__.py
--rw-r--r--   0        0        0      236 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/web/__main__.py
--rw-r--r--   0        0        0     5476 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/web/app.py
--rw-r--r--   0        0        0     1897 2023-03-08 19:53:12.132531 lokiunimore-0.6.0/lokiunimore/web/extensions/matrix_client.py
--rw-r--r--   0        0        0    67646 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/static/favicon.ico
--rw-r--r--   0        0        0     8288 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/static/icon.png
--rw-r--r--   0        0        0     9408 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/static/newcode.png
--rw-r--r--   0        0        0   151500 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/static/opengraph.png
--rw-r--r--   0        0        0    13849 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/static/rooms.png
--rw-r--r--   0        0        0    11414 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/static/s-192.png
--rw-r--r--   0        0        0    12609 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/static/spaces.png
--rw-r--r--   0        0        0     9703 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/static/thor.png
--rw-r--r--   0        0        0     2380 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/static/unimore.css
--rw-r--r--   0        0        0    15136 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/static/verify.png
--rw-r--r--   0        0        0     1941 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/_base.html
--rw-r--r--   0        0        0      593 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/errors/_base.html
--rw-r--r--   0        0        0      521 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/errors/failed-invite.html
--rw-r--r--   0        0        0      470 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/errors/no-link.html
--rw-r--r--   0        0        0      330 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/errors/not-found.html
--rw-r--r--   0        0        0      645 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/errors/not-student.html
--rw-r--r--   0        0        0      599 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/errors/not-verified.html
--rw-r--r--   0        0        0      300 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/errors/oidc.html
--rw-r--r--   0        0        0      418 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/errors/rate-invite.html
--rw-r--r--   0        0        0     2125 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/matrix/complete.html
--rw-r--r--   0        0        0     2481 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/matrix/join.html
--rw-r--r--   0        0        0     1764 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/matrix/verify.html
--rw-r--r--   0        0        0     5933 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/privacy.html
--rw-r--r--   0        0        0     5336 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/lokiunimore/web/templates/root.html
--rw-r--r--   0        0        0     4703 2023-03-08 19:53:12.136531 lokiunimore-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 lokiunimore-0.6.0/setup.py
--rw-r--r--   0        0        0     4695 1970-01-01 00:00:00.000000 lokiunimore-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     3434 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/config/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/config/__main__.py
+-rw-r--r--   0        0        0     6187 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/config/config.py
+-rw-r--r--   0        0        0       22 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/matrix/__init__.py
+-rw-r--r--   0        0        0      735 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/matrix/__main__.py
+-rw-r--r--   0        0        0    22084 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/matrix/client.py
+-rw-r--r--   0        0        0     3066 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/matrix/templates/messages.py
+-rw-r--r--   0        0        0       22 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/sql/__init__.py
+-rw-r--r--   0        0        0      260 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/sql/__main__.py
+-rw-r--r--   0        0        0     2431 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/sql/tables.py
+-rw-r--r--   0        0        0      348 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/utils/device_names.py
+-rw-r--r--   0        0        0      888 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/utils/logs.py
+-rw-r--r--   0        0        0       19 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/__main__.py
+-rw-r--r--   0        0        0     5476 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/app.py
+-rw-r--r--   0        0        0     1897 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/extensions/matrix_client.py
+-rw-r--r--   0        0        0    67646 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/favicon.ico
+-rw-r--r--   0        0        0     8288 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/icon.png
+-rw-r--r--   0        0        0     9408 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/newcode.png
+-rw-r--r--   0        0        0   151500 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/opengraph.png
+-rw-r--r--   0        0        0    13849 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/rooms.png
+-rw-r--r--   0        0        0    11414 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/s-192.png
+-rw-r--r--   0        0        0    12609 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/spaces.png
+-rw-r--r--   0        0        0     9703 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/thor.png
+-rw-r--r--   0        0        0     2380 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/unimore.css
+-rw-r--r--   0        0        0    15136 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/verify.png
+-rw-r--r--   0        0        0     1941 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/_base.html
+-rw-r--r--   0        0        0      593 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/_base.html
+-rw-r--r--   0        0        0      521 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/failed-invite.html
+-rw-r--r--   0        0        0      470 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/no-link.html
+-rw-r--r--   0        0        0      330 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/not-found.html
+-rw-r--r--   0        0        0      645 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/not-student.html
+-rw-r--r--   0        0        0      599 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/not-verified.html
+-rw-r--r--   0        0        0      300 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/oidc.html
+-rw-r--r--   0        0        0      418 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/rate-invite.html
+-rw-r--r--   0        0        0     2125 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/matrix/complete.html
+-rw-r--r--   0        0        0     2481 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/matrix/join.html
+-rw-r--r--   0        0        0     1764 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/matrix/verify.html
+-rw-r--r--   0        0        0     5933 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/privacy.html
+-rw-r--r--   0        0        0     5336 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/root.html
+-rw-r--r--   0        0        0     4703 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 lokiunimore-0.6.1/setup.py
+-rw-r--r--   0        0        0     4695 1970-01-01 00:00:00.000000 lokiunimore-0.6.1/PKG-INFO
```

### Comparing `lokiunimore-0.6.0/LICENSE.txt` & `lokiunimore-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/README.md` & `lokiunimore-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/config/config.py` & `lokiunimore-0.6.1/lokiunimore/config/config.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/matrix/__main__.py` & `lokiunimore-0.6.1/lokiunimore/matrix/__main__.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/matrix/client.py` & `lokiunimore-0.6.1/lokiunimore/matrix/client.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/matrix/templates/messages.py` & `lokiunimore-0.6.1/lokiunimore/matrix/templates/messages.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/sql/tables.py` & `lokiunimore-0.6.1/lokiunimore/sql/tables.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/utils/logs.py` & `lokiunimore-0.6.1/lokiunimore/utils/logs.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/app.py` & `lokiunimore-0.6.1/lokiunimore/web/app.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/extensions/matrix_client.py` & `lokiunimore-0.6.1/lokiunimore/web/extensions/matrix_client.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/static/favicon.ico` & `lokiunimore-0.6.1/lokiunimore/web/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/static/icon.png` & `lokiunimore-0.6.1/lokiunimore/web/static/icon.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/static/newcode.png` & `lokiunimore-0.6.1/lokiunimore/web/static/newcode.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/static/opengraph.png` & `lokiunimore-0.6.1/lokiunimore/web/static/opengraph.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/static/rooms.png` & `lokiunimore-0.6.1/lokiunimore/web/static/rooms.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/static/s-192.png` & `lokiunimore-0.6.1/lokiunimore/web/static/s-192.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/static/spaces.png` & `lokiunimore-0.6.1/lokiunimore/web/static/spaces.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/static/thor.png` & `lokiunimore-0.6.1/lokiunimore/web/static/thor.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/static/unimore.css` & `lokiunimore-0.6.1/lokiunimore/web/static/unimore.css`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/static/verify.png` & `lokiunimore-0.6.1/lokiunimore/web/static/verify.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/templates/_base.html` & `lokiunimore-0.6.1/lokiunimore/web/templates/_base.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/templates/errors/_base.html` & `lokiunimore-0.6.1/lokiunimore/web/templates/errors/_base.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/templates/errors/failed-invite.html` & `lokiunimore-0.6.1/lokiunimore/web/templates/errors/failed-invite.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/templates/errors/not-student.html` & `lokiunimore-0.6.1/lokiunimore/web/templates/errors/not-student.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/templates/errors/not-verified.html` & `lokiunimore-0.6.1/lokiunimore/web/templates/errors/not-verified.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/templates/matrix/complete.html` & `lokiunimore-0.6.1/lokiunimore/web/templates/matrix/complete.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/templates/matrix/join.html` & `lokiunimore-0.6.1/lokiunimore/web/templates/matrix/join.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/templates/matrix/verify.html` & `lokiunimore-0.6.1/lokiunimore/web/templates/matrix/verify.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/templates/privacy.html` & `lokiunimore-0.6.1/lokiunimore/web/templates/privacy.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/lokiunimore/web/templates/root.html` & `lokiunimore-0.6.1/lokiunimore/web/templates/root.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.0/pyproject.toml` & `lokiunimore-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # See https://python-poetry.org/docs/pyproject/ for more details!
 
 # The name of your project.
 # Ensure that it is available on PyPI: https://pypi.org/
 name = "lokiunimore"
 
 # The version of the package.
-version = "0.6.0"
+version = "0.6.1"
 
 # A brief, one-sentence description about your project.
 description = "Matrix room gatekeeper bot for the unofficial Unimore space"
 
 # A list of the authors of the project.
 authors = [
     "Stefano Pigozzi <me@steffo.eu>",
```

### Comparing `lokiunimore-0.6.0/setup.py` & `lokiunimore-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'requests>=2.28.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['lokiunimore = lokiunimore.__main__:main']}
 
 setup_kwargs = {
     'name': 'lokiunimore',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'Matrix room gatekeeper bot for the unofficial Unimore space',
     'long_description': "# Loki Bot\n\nGatekeeper bot for the Unimore Informatica unofficial Matrix space\n\n\\[ [**Website**](https://loki.steffo.eu) | [PyPI](https://pypi.org/project/lokiunimore/) \\]\n\n> TIP: You may be looking for its predecessor, [Thor Bot](https://github.com/Steffo99/thorunimore).\n\n![](lokiunimore/web/static/opengraph.png)\n\n## Functionality\n\nThis bot monitors a [pre-configured *public* Matrix space][config-public-space] for join events, sending a [welcome message][welcome-msg] to every new joiner.\n\nThe [welcome message][welcome-msg] contains a link, which when clicked starts the user verification process:\n\n1. a page describing the bot is opened, and it allows users to login with a [pre-configured OpenID Connect Identity Provider][config-oidc-idp];\n2. the claims of the OIDC IdP are verified, and the user's email address is checked to verify that its domain matches a [pre-configured RegEx][config-email-regex]\n with specific email requirements;\n3. if the email address fullfils all the requirements, an invitation to a different, [pre-configured *private* Matrix space][config-private-space] is sent to the user.\n\nAdditionally, the bot monitors for leave events from both spaces, deleting user data if no longer needed to protect the user's privacy.\n\n[welcome-msg]: https://github.com/Steffo99/lokiunimore/blob/99f7101abc3f68472844cd2f1bac5119e41c1682/lokiunimore/matrix/templates/messages.py#L3-L23\n[config-public-space]: https://github.com/Steffo99/lokiunimore/blob/main/lokiunimore/config/config.py#L50-L60\n[config-oidc-idp]: https://github.com/Steffo99/lokiunimore/blob/main/lokiunimore/config/config.py#L147-L202\n[config-email-regex]: https://github.com/Steffo99/lokiunimore/blob/main/lokiunimore/config/config.py#L194-L202\n[config-private-space]: https://github.com/Steffo99/lokiunimore/blob/99f7101abc3f68472844cd2f1bac5119e41c1682/lokiunimore/config/config.py#L76-L86\n\n## Setting up a development environment\n\n### Dependencies\n\nThis project uses [Poetry](https://python-poetry.org/) to manage the dependencies.\n\nTo install all dependencies in a venv, run:\n\n```console\n$ poetry install\n```\n\n> TIP: For easier venv management, you may want to set:\n> \n> ```console\n> $ poetry config virtualenvs.in-project true\n> ```\n\nTo activate the venv, run:\n\n```console\n$ poetry shell\n```\n\nTo run something in the venv without activating it, run:\n\n```console\n$ poetry run <COMMAND>\n```\n\n### Environment\n\nLoki requires a lot of environment variables to be set, therefore it makes use of [cfig](https://cfig.readthedocs.io/en/latest/) to simplify the setup.\n\nTo view the current configuration, followed by a description of each variable, run:\n\n```console\n$ poetry run python -m lokiunimore.config\n```\n\n## Deploying in production\n\nUse the [pre-built Docker image](https://github.com/Steffo99/lokiunimore/pkgs/container/lokiunimore), or build it from the [provided Dockerfile](Dockerfile).\n\nRun the image without any command to view and validate the current configuration.\n\nRun the image with the `gunicorn -b 0.0.0.0:80 lokiunimore.web.app:rp_app` command to launch the production web server on local port 80, expecting to be behind a  reverse proxy.\n\nRun the image with the `lokiunimore.matrix` command to launch the Matrix bot.\n\n### Using Docker Compose\n\nUse the [given Docker Compose file](docker-compose.yml).\n\nEither use [Portainer](https://www.portainer.io/), or start it manually using `docker compose up -d && docker compose logs -f`.\n",
     'author': 'Stefano Pigozzi',
     'author_email': 'me@steffo.eu',
     'maintainer': 'Stefano Pigozzi',
     'maintainer_email': 'me@steffo.eu',
     'url': 'https://loki.steffo.eu/',
```

### Comparing `lokiunimore-0.6.0/PKG-INFO` & `lokiunimore-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lokiunimore
-Version: 0.6.0
+Version: 0.6.1
 Summary: Matrix room gatekeeper bot for the unofficial Unimore space
 Home-page: https://loki.steffo.eu/
 License: AGPL-3.0-or-later
 Keywords: bot,matrix,authentication,unimore,oauth2
 Author: Stefano Pigozzi
 Author-email: me@steffo.eu
 Maintainer: Stefano Pigozzi
```

