# Comparing `tmp/simplisafe-python-9.6.8.tar.gz` & `tmp/simplisafe-python-9.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplisafe-python-9.6.8.tar", last modified: Mon Mar  1 19:58:43 2021, max compression
+gzip compressed data, was "simplisafe-python-9.6.9.tar", max compression
```

## Comparing `simplisafe-python-9.6.8.tar` & `simplisafe-python-9.6.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1099 2020-08-12 19:37:17.370046 simplisafe-python-9.6.8/LICENSE
--rw-r--r--   0        0        0     2104 2020-08-12 19:44:14.638164 simplisafe-python-9.6.8/README.md
--rw-r--r--   0        0        0     1682 2021-03-01 19:47:38.436308 simplisafe-python-9.6.8/pyproject.toml
--rw-r--r--   0        0        0       64 2020-08-12 19:37:17.380171 simplisafe-python-9.6.8/simplipy/__init__.py
--rw-r--r--   0        0        0    13387 2021-03-01 19:47:38.436632 simplisafe-python-9.6.8/simplipy/api.py
--rw-r--r--   0        0        0     3421 2020-10-26 22:58:30.055210 simplisafe-python-9.6.8/simplipy/camera.py
--rw-r--r--   0        0        0       88 2020-10-21 17:38:23.743617 simplisafe-python-9.6.8/simplipy/const.py
--rw-r--r--   0        0        0     3784 2020-10-26 22:58:30.055423 simplisafe-python-9.6.8/simplipy/entity.py
--rw-r--r--   0        0        0      784 2021-02-28 21:18:06.091155 simplisafe-python-9.6.8/simplipy/errors.py
--rw-r--r--   0        0        0     2610 2020-10-22 03:02:03.495172 simplisafe-python-9.6.8/simplipy/lock.py
--rw-r--r--   0        0        0     1808 2020-10-21 20:13:03.900564 simplisafe-python-9.6.8/simplipy/sensor/v2.py
--rw-r--r--   0        0        0     1626 2020-10-21 20:13:03.900811 simplisafe-python-9.6.8/simplipy/sensor/v3.py
--rw-r--r--   0        0        0    13863 2020-11-04 23:58:59.726458 simplisafe-python-9.6.8/simplipy/system/__init__.py
--rw-r--r--   0        0        0     3462 2020-10-26 22:58:30.056534 simplisafe-python-9.6.8/simplipy/system/v2.py
--rw-r--r--   0        0        0    15797 2020-12-08 00:27:50.724060 simplisafe-python-9.6.8/simplipy/system/v3.py
--rw-r--r--   0        0        0       30 2020-08-12 19:37:17.384604 simplisafe-python-9.6.8/simplipy/util/__init__.py
--rw-r--r--   0        0        0      256 2020-08-12 19:44:14.643228 simplisafe-python-9.6.8/simplipy/util/dt.py
--rw-r--r--   0        0        0      274 2020-08-12 19:37:17.385486 simplisafe-python-9.6.8/simplipy/util/string.py
--rw-r--r--   0        0        0    11472 2021-01-29 19:18:37.072273 simplisafe-python-9.6.8/simplipy/websocket.py
--rw-r--r--   0        0        0     3023 2021-03-01 19:58:43.471224 simplisafe-python-9.6.8/setup.py
--rw-r--r--   0        0        0     3177 2021-03-01 19:58:43.471834 simplisafe-python-9.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1099 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/LICENSE
+-rw-r--r--   0        0        0     2104 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/README.md
+-rw-r--r--   0        0        0     1682 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/pyproject.toml
+-rw-r--r--   0        0        0       64 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/__init__.py
+-rw-r--r--   0        0        0    14139 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/api.py
+-rw-r--r--   0        0        0     3421 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/camera.py
+-rw-r--r--   0        0        0       88 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/const.py
+-rw-r--r--   0        0        0     3784 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/entity.py
+-rw-r--r--   0        0        0      784 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/errors.py
+-rw-r--r--   0        0        0     2610 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/lock.py
+-rw-r--r--   0        0        0     1808 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/sensor/v2.py
+-rw-r--r--   0        0        0     1626 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/sensor/v3.py
+-rw-r--r--   0        0        0    13863 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/system/__init__.py
+-rw-r--r--   0        0        0     3462 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/system/v2.py
+-rw-r--r--   0        0        0    15797 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/system/v3.py
+-rw-r--r--   0        0        0       30 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/util/__init__.py
+-rw-r--r--   0        0        0      256 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/util/dt.py
+-rw-r--r--   0        0        0      274 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/util/string.py
+-rw-r--r--   0        0        0    11472 2021-03-02 14:54:51.964511 simplisafe-python-9.6.9/simplipy/websocket.py
+-rw-r--r--   0        0        0     3023 2021-03-02 14:55:00.999652 simplisafe-python-9.6.9/setup.py
+-rw-r--r--   0        0        0     3177 2021-03-02 14:55:01.000064 simplisafe-python-9.6.9/PKG-INFO
```

### Comparing `simplisafe-python-9.6.8/LICENSE` & `simplisafe-python-9.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/README.md` & `simplisafe-python-9.6.9/README.md`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/pyproject.toml` & `simplisafe-python-9.6.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 multi_line_output = 3
 not_skip = "__init__.py"
 sections = "FUTURE,STDLIB,INBETWEENS,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 use_parentheses = true
 
 [tool.poetry]
 name = "simplisafe-python"
-version = "9.6.8"
+version = "9.6.9"
 description = "A Python3, async interface to the SimpliSafe API"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/simplisafe-python"
 packages = [
     { include = "simplipy" },
```

### Comparing `simplisafe-python-9.6.8/simplipy/api.py` & `simplisafe-python-9.6.9/simplipy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,14 +291,25 @@
                         data = await resp.json(content_type=None)
                     except JSONDecodeError:
                         message = await resp.text()
                         data = {"error": message}
 
                     LOGGER.debug("Data received from /%s: %s", endpoint, data)
 
+                    if isinstance(data, str):
+                        # In some cases, the SimpliSafe API will return a quoted string
+                        # in its response body (e.g., "\"node not found\""), which is
+                        # technically valid JSON. Additionally, SimpliSafe sets that
+                        # response's Content-Type header to application/json (#smh).
+                        # Together, these factors will allow a non-true-JSON  payload to
+                        # escape the try/except above. So, if we get here, we use the
+                        # string value (with quotes removed) to raise an error:
+                        message = data.replace('"', "")
+                        data = {"error": message}
+
                     resp.raise_for_status()
                     return data
             except ClientError as err:
                 # If we get an "error" related to MFA, the response body data is
                 # necessary for continuing on, so we swallow the error and return
                 # that data:
                 if data.get("error") == "mfa_required":
```

### Comparing `simplisafe-python-9.6.8/simplipy/camera.py` & `simplisafe-python-9.6.9/simplipy/camera.py`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/simplipy/entity.py` & `simplisafe-python-9.6.9/simplipy/entity.py`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/simplipy/errors.py` & `simplisafe-python-9.6.9/simplipy/errors.py`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/simplipy/lock.py` & `simplisafe-python-9.6.9/simplipy/lock.py`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/simplipy/sensor/v2.py` & `simplisafe-python-9.6.9/simplipy/sensor/v2.py`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/simplipy/sensor/v3.py` & `simplisafe-python-9.6.9/simplipy/sensor/v3.py`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/simplipy/system/__init__.py` & `simplisafe-python-9.6.9/simplipy/system/__init__.py`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/simplipy/system/v2.py` & `simplisafe-python-9.6.9/simplipy/system/v2.py`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/simplipy/system/v3.py` & `simplisafe-python-9.6.9/simplipy/system/v3.py`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/simplipy/websocket.py` & `simplisafe-python-9.6.9/simplipy/websocket.py`

 * *Files identical despite different names*

### Comparing `simplisafe-python-9.6.8/setup.py` & `simplisafe-python-9.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'python-socketio>=4.6,<6.0',
  'pytz>=2019.3,<2022.0',
  'voluptuous>=0.11.7,<0.13.0',
  'websockets>=8.1,<9.0']
 
 setup_kwargs = {
     'name': 'simplisafe-python',
-    'version': '9.6.8',
+    'version': '9.6.9',
     'description': 'A Python3, async interface to the SimpliSafe API',
     'long_description': '# 🚨 simplisafe-python: A Python3, async interface to the SimpliSafe™ API\n\n[![CI](https://github.com/bachya/simplisafe-python/workflows/CI/badge.svg)](https://github.com/bachya/simplisafe-python/actions)\n[![PyPi](https://img.shields.io/pypi/v/simplisafe-python.svg)](https://pypi.python.org/pypi/simplisafe-python)\n[![Version](https://img.shields.io/pypi/pyversions/simplisafe-python.svg)](https://pypi.python.org/pypi/simplisafe-python)\n[![License](https://img.shields.io/pypi/l/simplisafe-python.svg)](https://github.com/bachya/simplisafe-python/blob/master/LICENSE)\n[![Code Coverage](https://codecov.io/gh/bachya/simplisafe-python/branch/master/graph/badge.svg)](https://codecov.io/gh/bachya/simplisafe-python)\n[![Maintainability](https://api.codeclimate.com/v1/badges/f46d8b1dcfde6a2f683d/maintainability)](https://codeclimate.com/github/bachya/simplisafe-python/maintainability)\n[![Say Thanks](https://img.shields.io/badge/SayThanks-!-1EAEDB.svg)](https://saythanks.io/to/bachya)\n\n`simplisafe-python` (hereafter referred to as `simplipy`) is a Python3,\n`asyncio`-driven interface to the unofficial SimpliSafe™ API. With it, users can\nget data on their system (including available sensors), set the system state,\nand more.\n\n# Documentation\n\nYou can find complete documentation here: https://simplisafe-python.readthedocs.io\n\n# Contributing\n\n1. [Check for open features/bugs](https://github.com/bachya/simplisafe-python/issues)\n  or [initiate a discussion on one](https://github.com/bachya/simplisafe-python/issues/new).\n2. [Fork the repository](https://github.com/bachya/simplisafe-python/fork).\n3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`\n4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`\n5. Install the dev environment: `script/setup`\n6. Code your new feature or bug fix.\n7. Write tests that cover your new functionality.\n8. Run tests and ensure 100% code coverage: `script/test`\n9. Update `README.md` with any new documentation.\n10. Add yourself to `AUTHORS.md`.\n11. Submit a pull request!\n',
     'author': 'Aaron Bach',
     'author_email': 'bachya1208@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/bachya/simplisafe-python',
```

### Comparing `simplisafe-python-9.6.8/PKG-INFO` & `simplisafe-python-9.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplisafe-python
-Version: 9.6.8
+Version: 9.6.9
 Summary: A Python3, async interface to the SimpliSafe API
 Home-page: https://github.com/bachya/simplisafe-python
 License: MIT
 Author: Aaron Bach
 Author-email: bachya1208@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

