# Comparing `tmp/sans-1.0.0b2.tar.gz` & `tmp/sans-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sans-1.0.0b2.tar", last modified: Sat May 13 18:51:25 2023, max compression
+gzip compressed data, was "sans-1.1.0.tar", last modified: Wed May 17 19:10:31 2023, max compression
```

## Comparing `sans-1.0.0b2.tar` & `sans-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:25.288592 sans-1.0.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:25.276591 sans-1.0.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:25.280592 sans-1.0.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-13 18:51:11.000000 sans-1.0.0b2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-13 18:51:11.000000 sans-1.0.0b2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-13 18:51:11.000000 sans-1.0.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-13 18:51:11.000000 sans-1.0.0b2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-13 18:51:11.000000 sans-1.0.0b2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-13 18:51:11.000000 sans-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-13 18:51:25.288592 sans-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-13 18:51:11.000000 sans-1.0.0b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:25.280592 sans-1.0.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/limiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/lock.rst
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/response.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-13 18:51:11.000000 sans-1.0.0b2/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-13 18:51:11.000000 sans-1.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-13 18:51:11.000000 sans-1.0.0b2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:25.284592 sans-1.0.0b2/sans/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29256 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-13 18:51:11.000000 sans-1.0.0b2/sans/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:25.288592 sans-1.0.0b2/sans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-13 18:51:25.000000 sans-1.0.0b2/sans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-13 18:51:25.000000 sans-1.0.0b2/sans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 18:51:25.000000 sans-1.0.0b2/sans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-13 18:51:25.000000 sans-1.0.0b2/sans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-13 18:51:25.000000 sans-1.0.0b2/sans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-13 18:51:25.000000 sans-1.0.0b2/sans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 18:51:25.288592 sans-1.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-13 18:51:11.000000 sans-1.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:10:31.715571 sans-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:10:31.707571 sans-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:10:31.711571 sans-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-17 19:10:17.000000 sans-1.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-17 19:10:17.000000 sans-1.1.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-17 19:10:17.000000 sans-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-17 19:10:17.000000 sans-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 19:10:17.000000 sans-1.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 19:10:17.000000 sans-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 19:10:31.715571 sans-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-17 19:10:17.000000 sans-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:10:31.711571 sans-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 19:10:17.000000 sans-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-17 19:10:17.000000 sans-1.1.0/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-17 19:10:17.000000 sans-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 19:10:17.000000 sans-1.1.0/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 19:10:17.000000 sans-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-17 19:10:17.000000 sans-1.1.0/docs/limiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 19:10:17.000000 sans-1.1.0/docs/lock.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-17 19:10:17.000000 sans-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 19:10:17.000000 sans-1.1.0/docs/response.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-17 19:10:17.000000 sans-1.1.0/docs/url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 19:10:17.000000 sans-1.1.0/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-17 19:10:17.000000 sans-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-17 19:10:17.000000 sans-1.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:10:31.715571 sans-1.1.0/sans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-17 19:10:17.000000 sans-1.1.0/sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 19:10:17.000000 sans-1.1.0/sans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-17 19:10:17.000000 sans-1.1.0/sans/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-17 19:10:17.000000 sans-1.1.0/sans/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-17 19:10:17.000000 sans-1.1.0/sans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28956 2023-05-17 19:10:17.000000 sans-1.1.0/sans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-17 19:10:17.000000 sans-1.1.0/sans/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-17 19:10:17.000000 sans-1.1.0/sans/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-17 19:10:17.000000 sans-1.1.0/sans/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-17 19:10:17.000000 sans-1.1.0/sans/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:10:17.000000 sans-1.1.0/sans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-17 19:10:17.000000 sans-1.1.0/sans/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-17 19:10:17.000000 sans-1.1.0/sans/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-17 19:10:17.000000 sans-1.1.0/sans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:10:31.715571 sans-1.1.0/sans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 19:10:31.000000 sans-1.1.0/sans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-17 19:10:31.000000 sans-1.1.0/sans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:10:31.000000 sans-1.1.0/sans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 19:10:31.000000 sans-1.1.0/sans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 19:10:31.000000 sans-1.1.0/sans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 19:10:31.000000 sans-1.1.0/sans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:10:31.715571 sans-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 19:10:17.000000 sans-1.1.0/setup.py
```

### Comparing `sans-1.0.0b2/.github/workflows/codeql-analysis.yml` & `sans-1.1.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/.github/workflows/pythonpublish.yml` & `sans-1.1.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/.gitignore` & `sans-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/.pre-commit-config.yaml` & `sans-1.1.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.2.0
+    rev: v4.4.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-toml
     -   id: check-added-large-files
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.265
+    rev: v0.0.267
     hooks:
     -   id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
 -   repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.306
+    rev: v1.1.308
     hooks:
     -   id: pyright
         additional_dependencies:
             # required dependencies
         -   httpx ~= 0.23
         -   importlib_metadata >= 1.4.0; python_version < "3.8"
```

### Comparing `sans-1.0.0b2/LICENSE` & `sans-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/PKG-INFO` & `sans-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.0.0b2
+Version: 1.1.0
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/Zephyrkul/sans
 Project-URL: documentation, https://sans.readthedocs.io/en/stable/
 Project-URL: repository, https://github.com/Zephyrkul/sans.git
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sans-1.0.0b2/README.rst` & `sans-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/docs/Makefile` & `sans-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/docs/conf.py` & `sans-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/docs/make.bat` & `sans-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/pyproject.toml` & `sans-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [project]
     name = 'sans'
     description = 'Synchronous / Asynchronous HTTPX extension for NationStates'
     readme = 'README.rst'
     requires-python = '>=3.7.0,<4.0'
     classifiers = [
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Framework :: AsyncIO',
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
```

### Comparing `sans-1.0.0b2/sans/__init__.py` & `sans-1.1.0/sans/__init__.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/sans/__main__.py` & `sans-1.1.0/sans/__main__.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/sans/_state.py` & `sans-1.1.0/sans/_state.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/sans/auth.py` & `sans-1.1.0/sans/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,26 +16,37 @@
 
 class NSAuth(RateLimiter):
     def __init__(self, *, password: str | None = None, autologin: str | None = None):
         self._password = password
         self.autologin = autologin
 
     @property
+    def password(self) -> str | None:
+        return self._password
+
+    @password.setter
+    def password(self, value: str | None) -> None:
+        if value:
+            self._autologin = None  # likely out of date
+        self._password = value
+
+    @property
     def autologin(self) -> str | None:
         return self._autologin
 
     @autologin.setter
     def autologin(self, value: str | None) -> None:
         if value:
             self._password = None  # no longer needed
         self._autologin = value
 
     def _request_hook(self, request: Request) -> Request:
-        nation = request.url.params.get("nation")
-        if not nation:
+        params = request.url.params
+        nation = params.get("nation")
+        if not nation or not params.get("c"):
             return request
         auth = {}
         if self._password:
             auth["X-Password"] = self._password
         elif self._autologin:
             auth["X-Autologin"] = self._autologin
         pin = _PINS.get(nation)
```

### Comparing `sans-1.0.0b2/sans/client.pyi` & `sans-1.1.0/sans/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -66,73 +66,60 @@
     @overload
     def request(
         self,
         method: str,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
-    ) -> httpx.Response: ...
+    ) -> Response: ...
     @overload
     def request(
         self,
         method: str,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: RateLimiter = ...,
+        auth: AuthTypes,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
-    ) -> Response: ...
-    @overload
-    def send(
-        self,
-        request: httpx.Request,
-        *,
-        stream: bool = ...,
-        auth: AuthTypes,
-        follow_redirects: bool = ...,
     ) -> httpx.Response: ...
     @overload
     def send(
         self,
         request: httpx.Request,
         *,
         stream: bool = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
     ) -> Response: ...
     @overload
-    def get(
+    def send(
         self,
-        url: URLTypes,
+        request: httpx.Request,
         *,
-        params: QueryParamTypes = ...,
-        headers: HeaderTypes = ...,
-        cookies: CookieTypes = ...,
+        stream: bool = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
-        timeout: TimeoutTypes = ...,
-        extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def get(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
@@ -140,15 +127,15 @@
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    def options(
+    def get(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
@@ -166,15 +153,15 @@
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    def head(
+    def options(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
@@ -192,54 +179,50 @@
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    def post(
+    def head(
         self,
         url: URLTypes,
         *,
-        content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
-        files: RequestFiles = ...,
-        json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def post(
         self,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    def put(
+    def post(
         self,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
@@ -248,32 +231,32 @@
     ) -> httpx.Response: ...
     @overload
     def put(
         self,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    def patch(
+    def put(
         self,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
@@ -282,30 +265,34 @@
     ) -> httpx.Response: ...
     @overload
     def patch(
         self,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    def delete(
+    def patch(
         self,
         url: URLTypes,
         *,
+        content: RequestContent = ...,
+        data: RequestData = ...,
+        files: RequestFiles = ...,
+        json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
@@ -320,117 +307,117 @@
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    def stream(
+    def delete(
         self,
-        method: str,
         url: URLTypes,
         *,
-        content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
-        files: RequestFiles = ...,
-        json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
-    ) -> ContextManager[httpx.Response]: ...
+    ) -> httpx.Response: ...
     @overload
     def stream(
         self,
         method: str,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> ContextManager[Response]: ...
-
-class AsyncClientType(_ClientMixin, httpx.AsyncClient):
     @overload
-    async def request(
+    def stream(
         self,
         method: str,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
-    ) -> httpx.Response: ...
+    ) -> ContextManager[httpx.Response]: ...
+
+class AsyncClientType(_ClientMixin, httpx.AsyncClient):
     @overload
     async def request(
         self,
         method: str,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    async def send(
+    async def request(
         self,
-        request: httpx.Request,
+        method: str,
+        url: URLTypes,
         *,
-        stream: bool = ...,
+        content: RequestContent = ...,
+        data: RequestData = ...,
+        files: RequestFiles = ...,
+        json: Any = ...,
+        params: QueryParamTypes = ...,
+        headers: HeaderTypes = ...,
+        cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
+        timeout: TimeoutTypes = ...,
+        extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     async def send(
         self,
         request: httpx.Request,
         *,
         stream: bool = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
     ) -> Response: ...
     @overload
-    async def get(
+    async def send(
         self,
-        url: URLTypes,
+        request: httpx.Request,
         *,
-        params: QueryParamTypes = ...,
-        headers: HeaderTypes = ...,
-        cookies: CookieTypes = ...,
+        stream: bool = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
-        timeout: TimeoutTypes = ...,
-        extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     async def get(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
@@ -438,15 +425,15 @@
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    async def options(
+    async def get(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
@@ -464,15 +451,15 @@
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    async def head(
+    async def options(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
@@ -490,54 +477,50 @@
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    async def post(
+    async def head(
         self,
         url: URLTypes,
         *,
-        content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
-        files: RequestFiles = ...,
-        json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     async def post(
         self,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    async def put(
+    async def post(
         self,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
@@ -546,32 +529,32 @@
     ) -> httpx.Response: ...
     @overload
     async def put(
         self,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    async def patch(
+    async def put(
         self,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
@@ -580,30 +563,34 @@
     ) -> httpx.Response: ...
     @overload
     async def patch(
         self,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
-    async def delete(
+    async def patch(
         self,
         url: URLTypes,
         *,
+        content: RequestContent = ...,
+        data: RequestData = ...,
+        files: RequestFiles = ...,
+        json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
         auth: AuthTypes,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
@@ -618,237 +605,235 @@
         cookies: CookieTypes = ...,
         auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> Response: ...
     @overload
+    async def delete(
+        self,
+        url: URLTypes,
+        *,
+        params: QueryParamTypes = ...,
+        headers: HeaderTypes = ...,
+        cookies: CookieTypes = ...,
+        auth: AuthTypes,
+        follow_redirects: bool = ...,
+        timeout: TimeoutTypes = ...,
+        extensions: dict[Any, Any] = ...,
+    ) -> httpx.Response: ...
+    @overload
     def stream(
         self,
         method: str,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: RateLimiter = ...,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
-    ) -> AsyncContextManager[httpx.Response]: ...
+    ) -> AsyncContextManager[Response]: ...
     @overload
     def stream(
         self,
         method: str,
         url: URLTypes,
         *,
         content: RequestContent = ...,
-        data: RequestData[Any, Any] = ...,
+        data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: RateLimiter = ...,
+        auth: AuthTypes,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
-    ) -> AsyncContextManager[Response]: ...
+    ) -> AsyncContextManager[httpx.Response]: ...
 
 @overload
 def Client(
     *,
-    auth: AuthTypes,
+    auth: RateLimiter = ...,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     http1: bool = ...,
     http2: bool = ...,
     proxies: ProxiesTypes = ...,
     mounts: Mapping[str, httpx.BaseTransport] = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     limits: httpx.Limits = ...,
     max_redirects: int = ...,
-    event_hooks: Mapping[str, list[Callable[..., Any]]] = ...,
+    event_hooks: _EventHooksParam = ...,
     base_url: URLTypes = ...,
     transport: httpx.BaseTransport = ...,
     app: Callable[..., Any] = ...,
     trust_env: bool = ...,
-) -> httpx.Client: ...
+) -> ClientType: ...
 @overload
 def Client(
     *,
-    auth: RateLimiter = ...,
+    auth: AuthTypes,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     http1: bool = ...,
     http2: bool = ...,
     proxies: ProxiesTypes = ...,
     mounts: Mapping[str, httpx.BaseTransport] = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     limits: httpx.Limits = ...,
     max_redirects: int = ...,
-    event_hooks: _EventHooksParam = ...,
+    event_hooks: Mapping[str, list[Callable[..., Any]]] = ...,
     base_url: URLTypes = ...,
     transport: httpx.BaseTransport = ...,
     app: Callable[..., Any] = ...,
     trust_env: bool = ...,
-) -> ClientType: ...
+) -> httpx.Client: ...
 @overload
 def AsyncClient(
     *,
-    auth: AuthTypes,
+    auth: RateLimiter = ...,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     http1: bool = ...,
     http2: bool = ...,
     proxies: ProxiesTypes = ...,
     mounts: Mapping[str, httpx.BaseTransport] = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     limits: httpx.Limits = ...,
     max_redirects: int = ...,
-    event_hooks: _EventHooksParam = ...,
+    event_hooks: Mapping[str, Collection[Callable[..., Any]]] = ...,
     base_url: URLTypes = ...,
     transport: httpx.BaseTransport = ...,
     app: Callable[..., Any] = ...,
     trust_env: bool = ...,
-) -> httpx.AsyncClient: ...
+) -> AsyncClientType: ...
 @overload
 def AsyncClient(
     *,
-    auth: RateLimiter = ...,
+    auth: AuthTypes,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     http1: bool = ...,
     http2: bool = ...,
     proxies: ProxiesTypes = ...,
     mounts: Mapping[str, httpx.BaseTransport] = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     limits: httpx.Limits = ...,
     max_redirects: int = ...,
-    event_hooks: Mapping[str, Collection[Callable[..., Any]]] = ...,
+    event_hooks: _EventHooksParam = ...,
     base_url: URLTypes = ...,
     transport: httpx.BaseTransport = ...,
     app: Callable[..., Any] = ...,
     trust_env: bool = ...,
-) -> AsyncClientType: ...
+) -> httpx.AsyncClient: ...
 @overload
 def request(
     method: str,
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
-    data: RequestData[Any, Any] = ...,
+    data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: RateLimiter = ...,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
-) -> httpx.Response: ...
+) -> Response: ...
 @overload
 def request(
     method: str,
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
-    data: RequestData[Any, Any] = ...,
+    data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: RateLimiter = ...,
+    auth: AuthTypes,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
-) -> Response: ...
+) -> httpx.Response: ...
 @overload
 def stream(
     method: str,
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
-    data: RequestData[Any, Any] = ...,
+    data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: RateLimiter = ...,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
-) -> ContextManager[httpx.Response]: ...
+) -> ContextManager[Response]: ...
 @overload
 def stream(
     method: str,
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
-    data: RequestData[Any, Any] = ...,
+    data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: RateLimiter = ...,
+    auth: AuthTypes,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
-) -> ContextManager[Response]: ...
-@overload
-def get(
-    url: URLTypes,
-    *,
-    params: QueryParamTypes = ...,
-    headers: HeaderTypes = ...,
-    cookies: CookieTypes = ...,
-    auth: AuthTypes,
-    proxies: ProxiesTypes = ...,
-    follow_redirects: bool = ...,
-    cert: CertTypes = ...,
-    verify: VerifyTypes = ...,
-    timeout: TimeoutTypes = ...,
-    trust_env: bool = ...,
-) -> httpx.Response: ...
+) -> ContextManager[httpx.Response]: ...
 @overload
 def get(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
@@ -857,15 +842,15 @@
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
 @overload
-def options(
+def get(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     auth: AuthTypes,
     proxies: ProxiesTypes = ...,
@@ -887,15 +872,15 @@
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
 @overload
-def head(
+def options(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     auth: AuthTypes,
     proxies: ProxiesTypes = ...,
@@ -917,58 +902,54 @@
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
 @overload
-def post(
+def head(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
-    content: RequestContent = ...,
-    data: RequestData[Any, Any] = ...,
-    files: RequestFiles = ...,
-    json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     auth: AuthTypes,
     proxies: ProxiesTypes = ...,
-    timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
-    verify: VerifyTypes = ...,
     cert: CertTypes = ...,
+    verify: VerifyTypes = ...,
+    timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> httpx.Response: ...
 @overload
 def post(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
-    data: RequestData[Any, Any] = ...,
+    data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     auth: RateLimiter = ...,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
 @overload
-def put(
+def post(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
-    data: RequestData[Any, Any] = ...,
+    data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     auth: AuthTypes,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
@@ -979,34 +960,34 @@
 ) -> httpx.Response: ...
 @overload
 def put(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
-    data: RequestData[Any, Any] = ...,
+    data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     auth: RateLimiter = ...,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
 @overload
-def patch(
+def put(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
-    data: RequestData[Any, Any] = ...,
+    data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     auth: AuthTypes,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
@@ -1017,40 +998,44 @@
 ) -> httpx.Response: ...
 @overload
 def patch(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
-    data: RequestData[Any, Any] = ...,
+    data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     auth: RateLimiter = ...,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
 @overload
-def delete(
+def patch(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
+    content: RequestContent = ...,
+    data: RequestData = ...,
+    files: RequestFiles = ...,
+    json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     auth: AuthTypes,
     proxies: ProxiesTypes = ...,
+    timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
-    cert: CertTypes = ...,
     verify: VerifyTypes = ...,
-    timeout: TimeoutTypes = ...,
+    cert: CertTypes = ...,
     trust_env: bool = ...,
 ) -> httpx.Response: ...
 @overload
 def delete(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
@@ -1060,7 +1045,22 @@
     proxies: ProxiesTypes = ...,
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
+@overload
+def delete(
+    url: URLTypes,
+    *,
+    params: QueryParamTypes = ...,
+    headers: HeaderTypes = ...,
+    cookies: CookieTypes = ...,
+    auth: AuthTypes,
+    proxies: ProxiesTypes = ...,
+    follow_redirects: bool = ...,
+    cert: CertTypes = ...,
+    verify: VerifyTypes = ...,
+    timeout: TimeoutTypes = ...,
+    trust_env: bool = ...,
+) -> httpx.Response: ...
```

### Comparing `sans-1.0.0b2/sans/decoder.py` & `sans-1.1.0/sans/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                     yield event, element
                     path[0].clear()
 
 
 try:
     from lxml.etree import (
         XMLParser as LXMLParser,
-        _Element as LElement,  # type: ignore
+        _Element as LElement,
     )
 except ImportError:
     pass
 else:
 
     class LXMLDecoder:
         def __init__(self, encoding: str | None = None) -> None:
```

### Comparing `sans-1.0.0b2/sans/errors.py` & `sans-1.1.0/sans/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,28 +33,29 @@
     pass
 
 
 def narrow(original: HTTPStatusError) -> HTTPStatusError:
     code = original.response.status_code
     match = (sys.maxsize, HTTPStatusError)
     for exc in globals().values():
-        if not issubclass(exc, _HTTPStatusError):
-            continue
         if exc is HTTPStatusError:
             continue
-        codes = exc._codes  # type: ignore
+        if not isinstance(exc, type) or not issubclass(exc, _HTTPStatusError):
+            continue
+        codes = exc._codes
         if code in codes:
             match = min(match, (len(codes), exc))
     _, best = match
     if best is type(original):
         return original
     # bypass __init__
     _new = best.__new__(best)
     _new.__dict__.update(original.__dict__)
-    return _new
+    _new.args = original.args
+    return _new.with_traceback(original.__traceback__)
 
 
 class ClientError(_HTTPStatusError):
     """
     :exc:`httpx.HTTPStatusError` for 4XX: Client Error status codes.
     """
```

### Comparing `sans-1.0.0b2/sans/limiter.py` & `sans-1.1.0/sans/limiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from math import ldexp
 from random import random
 from typing import AsyncGenerator, Generator, Iterator
 
 import anyio
 import httpx
 
-from . import _state  # type: ignore
+from . import _state
 from .errors import AgentNotSetError
 from .response import Response
 from .url import API_URL
 
 __all__ = ["RateLimiter"]
 LOG = logging.getLogger(__name__)
```

### Comparing `sans-1.0.0b2/sans/lock.py` & `sans-1.1.0/sans/lock.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0b2/sans/response.py` & `sans-1.1.0/sans/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from .errors import narrow
 
 try:
     import xmltodict
 
     HAS_XMLTODICT = True
 except ImportError:
-    HAS_XMLTODICT = False  # type: ignore
+    HAS_XMLTODICT = False
 
 try:
-    from lxml.etree import _Element  # type: ignore
+    from lxml.etree import _Element
 
     HAS_LXML = True
 except ImportError:
-    HAS_LXML = False  # type: ignore
+    HAS_LXML = False
 else:
     from .decoder import LXMLDecoder
 
 __all__ = ["Response"]
 
 
 class Response(httpx.Response):
```

### Comparing `sans-1.0.0b2/sans/url.py` & `sans-1.1.0/sans/url.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 from __future__ import annotations
 
 from datetime import date as _date
-from typing import TYPE_CHECKING, Mapping
+from typing import TYPE_CHECKING, Dict, Mapping, NewType
 
 import httpx
 
 if TYPE_CHECKING:
     from typing_extensions import Literal
+
+    _Shard = NewType("_Shard", Dict[str, str])
+
 API_URL = httpx.URL("https://www.nationstates.net/cgi-bin/api.cgi")
 
 __all__ = [
     "API_URL",
     "Nation",
     "Region",
     "World",
     "WA",
+    "Command",
     "Shard",
     "NationsDump",
     "RegionsDump",
     "CardsDump",
 ]
 
 
-def Nation(nation: str, *shards: str, **parameters: str) -> httpx.URL:
+def Nation(nation: str, *shards: str | _Shard, **parameters: str) -> httpx.URL:
     return World(*shards, nation=nation, **parameters)
 
 
 def Region(region: str, *shards: str, **parameters: str) -> httpx.URL:
     return World(*shards, region=region, **parameters)
 
 
-def World(*shards: str | Mapping[str, str], **parameters: str) -> httpx.URL:
+def World(*shards: str | _Shard, **parameters: str) -> httpx.URL:
     q: list[str | None] = [parameters.pop("q", None)]
     query: dict[str, str] = {}
     for shard in shards:
-        try:
-            shard = dict(shard)  # type: ignore
-        except (TypeError, ValueError):
-            q.append(str(shard))
+        if isinstance(shard, Mapping):
+            shard = dict(shard)
+            q.append(shard.pop("q", None))
+            query.update(shard)
         else:
-            q.append(shard.pop("q", None))  # type: ignore
-            query.update(shard)  # type: ignore
+            q.append(str(shard))
     query.update(parameters, q=" ".join(map(str, filter(None, q))))
     if query.get("a", "").lower() == "sendtg":
         raise RuntimeError("sans does not currently support the telegram API.")
     return API_URL.copy_with(params=query)
 
 
-def WA(wa: Literal[1, "1", 2, "2"], *shards: str, **parameters: str) -> httpx.URL:
+def WA(
+    wa: Literal[1, "1", 2, "2"], *shards: str | _Shard, **parameters: str
+) -> httpx.URL:
     return World(*shards, wa=str(wa), **parameters)
 
 
-def Shard(q: str, **parameters: str) -> dict[str, str]:
+def Command(nation: str, c: str, **parameters: str) -> httpx.URL:
+    return World(nation=nation, c=c, **parameters)
+
+
+def Shard(q: str, **parameters: str) -> _Shard:
     parameters["q"] = q
-    return parameters
+    return parameters  # type: ignore
 
 
 # https://www.nationstates.net/archive/nations/2018-09-30-nations-xml.gz
 def NationsDump(date: _date | None = None) -> httpx.URL:
     if date:
         path = date.strftime("/archive/nations/%Y-%m-%d-nations-xml.gz")
     else:
```

### Comparing `sans-1.0.0b2/sans/utils.py` & `sans-1.1.0/sans/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 from __future__ import annotations
 
 import sys
-from typing import Any, Coroutine, Mapping, overload
+from typing import Any, Coroutine, overload
 from xml.etree import ElementTree as etree
 
+from .auth import NSAuth
 from .client import AsyncClientType, ClientType
 from .response import Response
-from .url import World
+from .url import Command
 
 __all__ = ["prepare_and_execute", "indent"]
 
 
 @overload
 def prepare_and_execute(
-    client: ClientType, *shards: str | Mapping[str, str], **parameters: str
+    client: ClientType, auth: NSAuth, nation: str, c: str, **parameters: str
 ) -> Response:
     ...
 
 
 @overload
 async def prepare_and_execute(
-    client: AsyncClientType, *shards: str | Mapping[str, str], **parameters: str
+    client: AsyncClientType, auth: NSAuth, nation: str, c: str, **parameters: str
 ) -> Response:
     ...
 
 
 def prepare_and_execute(
     client: ClientType | AsyncClientType,
-    *shards: str | Mapping[str, str],
+    auth: NSAuth,
+    nation: str,
+    c: str,
     **parameters: str,
 ) -> Response | Coroutine[Any, Any, Response]:
     if isinstance(client, AsyncClientType):
-        return _prepare_async(client, *shards, **parameters)
-    request = World(*shards, **parameters, mode="prepare")
-    response = client.get(request)
+        return _prepare_async(client, auth, nation, c, **parameters)
+    request = Command(nation, c, **parameters, mode="prepare")
+    response = client.get(request, auth=auth)
     response.raise_for_status()
     token: str = response.xml.find("SUCCESS").text  # type: ignore
-    request = World(*shards, **parameters, mode="execute", token=token)
-    return client.get(request)
+    request = Command(nation, c, **parameters, mode="execute", token=token)
+    return client.get(request, auth=auth)
 
 
 async def _prepare_async(
-    client: AsyncClientType, *shards: str | Mapping[str, str], **parameters: str
+    client: AsyncClientType, auth: NSAuth, nation: str, c: str, **parameters: str
 ) -> Response:
-    request = World(*shards, **parameters, mode="prepare")
-    response = await client.get(request)
+    request = Command(nation, c, **parameters, mode="prepare")
+    response = await client.get(request, auth=auth)
     response.raise_for_status()
     token: str = response.xml.find("SUCCESS").text  # type: ignore
-    request = World(*shards, **parameters, mode="execute", token=token)
-    return await client.get(request)
+    request = Command(nation, c, **parameters, mode="execute", token=token)
+    return await client.get(request, auth=auth)
 
 
 if sys.version_info < (3, 9):
     # from: https://github.com/python/cpython/blob/3.11/Lib/xml/etree/ElementTree.py#L1154
     def indent(
         tree: etree.Element | etree.ElementTree, space: str = "  ", level: int = 0
     ):
```

### Comparing `sans-1.0.0b2/sans.egg-info/PKG-INFO` & `sans-1.1.0/sans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.0.0b2
+Version: 1.1.0
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/Zephyrkul/sans
 Project-URL: documentation, https://sans.readthedocs.io/en/stable/
 Project-URL: repository, https://github.com/Zephyrkul/sans.git
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sans-1.0.0b2/sans.egg-info/SOURCES.txt` & `sans-1.1.0/sans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

