# Comparing `tmp/pydrawise-2023.5.0.tar.gz` & `tmp/pydrawise-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydrawise-2023.5.0.tar", last modified: Fri May 12 02:26:47 2023, max compression
+gzip compressed data, was "pydrawise-2023.5.1.tar", last modified: Wed May 17 12:58:45 2023, max compression
```

## Comparing `pydrawise-2023.5.0.tar` & `pydrawise-2023.5.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.937234 pydrawise-2023.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.933234 pydrawise-2023.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.933234 pydrawise-2023.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.933234 pydrawise-2023.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-12 02:26:47.937234 pydrawise-2023.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/hydrawise.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.933234 pydrawise-2023.5.0/pydrawise/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pydrawise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pydrawise/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pydrawise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pydrawise/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pydrawise/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.937234 pydrawise-2023.5.0/pydrawise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 02:26:47.937234 pydrawise-2023.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.937234 pydrawise-2023.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.938151 pydrawise-2023.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.938151 pydrawise-2023.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/hydrawise.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/pydrawise/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/pydrawise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/tests/test_schema.py
```

### Comparing `pydrawise-2023.5.0/.devcontainer.json` & `pydrawise-2023.5.1/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.0/.github/workflows/build-and-test.yml` & `pydrawise-2023.5.1/.github/workflows/build-and-test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.9", "3.10"]
+        python-version: ["3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `pydrawise-2023.5.0/.github/workflows/publish-python.yml` & `pydrawise-2023.5.1/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.0/.gitignore` & `pydrawise-2023.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.0/.pre-commit-config.yaml` & `pydrawise-2023.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.0/LICENSE` & `pydrawise-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.0/PKG-INFO` & `pydrawise-2023.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2023.5.0
+Version: 2023.5.1
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
 Platform: any
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pydrawise
 Python 3 library for interacting with Hydrawise sprinkler controllers.
 
 *Note that this project has no official relationship with Hydrawise or Hunter. Use at your own risk.*
@@ -33,16 +33,16 @@
     # Create a Hydrawise object and authenticate with your credentials.
     h = Hydrawise(Auth("username", "password"))
 
     # List the controllers attached to your account.
     controllers = await h.get_controllers()
 
     # List the zones controlled by the first controller.
-    zones = await controllers[0].get_zones()
+    zones = await h.get_zones(controllers[0])
     
     # Start the first zone.
-    await zones[0].start()
+    await h.start_zone(zones[0])
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `pydrawise-2023.5.0/README.md` & `pydrawise-2023.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     # Create a Hydrawise object and authenticate with your credentials.
     h = Hydrawise(Auth("username", "password"))
 
     # List the controllers attached to your account.
     controllers = await h.get_controllers()
 
     # List the zones controlled by the first controller.
-    zones = await controllers[0].get_zones()
+    zones = await h.get_zones(controllers[0])
     
     # Start the first zone.
-    await zones[0].start()
+    await h.start_zone(zones[0])
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `pydrawise-2023.5.0/hydrawise.graphql` & `pydrawise-2023.5.1/hydrawise.graphql`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.0/pydrawise/auth.py` & `pydrawise-2023.5.1/pydrawise/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 CLIENT_ID = "hydrawise_app"
 CLIENT_SECRET = "zn3CrjglwNV1"
 TOKEN_URL = "https://app.hydrawise.com/api/v2/oauth/access-token"
 DEFAULT_TIMEOUT = 60
 
 
 class Auth:
+    """Authentication support for the Hydrawise GraphQL API."""
+
     def __init__(self, username: str, password: str) -> None:
+        """Initializer."""
         self.__username = username
         self.__password = password
         self._lock = Lock()
         self._token: str | None = None
         self._token_type: str | None = None
         self._token_expires: datetime | None = None
         self._refresh_token: str | None = None
@@ -54,17 +57,22 @@
                 self._refresh_token = resp_json["refresh_token"]
                 self._token_type = resp_json["token_type"]
                 self._token_expires = datetime.now() + timedelta(
                     seconds=resp_json["expires_in"]
                 )
 
     async def check_token(self):
+        """Checks a token and refreshes if necessary."""
         with self._lock:
             if self._token is None:
                 await self._fetch_token_locked(refresh=False)
             elif self._token_expires - datetime.now() < timedelta(minutes=5):
                 await self._fetch_token_locked(refresh=True)
 
     async def token(self) -> str:
+        """Retrieves an authentication token for the current user.
+
+        :rtype: string
+        """
         await self.check_token()
         with self._lock:
             return f"{self._token_type} {self._token}"
```

### Comparing `pydrawise-2023.5.0/pydrawise.egg-info/PKG-INFO` & `pydrawise-2023.5.1/pydrawise.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2023.5.0
+Version: 2023.5.1
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
 Platform: any
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pydrawise
 Python 3 library for interacting with Hydrawise sprinkler controllers.
 
 *Note that this project has no official relationship with Hydrawise or Hunter. Use at your own risk.*
@@ -33,16 +33,16 @@
     # Create a Hydrawise object and authenticate with your credentials.
     h = Hydrawise(Auth("username", "password"))
 
     # List the controllers attached to your account.
     controllers = await h.get_controllers()
 
     # List the zones controlled by the first controller.
-    zones = await controllers[0].get_zones()
+    zones = await h.get_zones(controllers[0])
     
     # Start the first zone.
-    await zones[0].start()
+    await h.start_zone(zones[0])
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `pydrawise-2023.5.0/pydrawise.egg-info/SOURCES.txt` & `pydrawise-2023.5.1/pydrawise.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .vscode/settings.json
 pydrawise/__init__.py
 pydrawise/_version.py
 pydrawise/auth.py
 pydrawise/client.py
 pydrawise/exceptions.py
 pydrawise/schema.py
+pydrawise/schema_utils.py
 pydrawise.egg-info/PKG-INFO
 pydrawise.egg-info/SOURCES.txt
 pydrawise.egg-info/dependency_links.txt
 pydrawise.egg-info/requires.txt
 pydrawise.egg-info/top_level.txt
 pydrawise.egg-info/zip-safe
 tests/__init__.py
```

### Comparing `pydrawise-2023.5.0/pyproject.toml` & `pydrawise-2023.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 [project]
 name            = "pydrawise"
 description     = "Python API for interacting with Hydrawise sprinkler controllers."
 authors         = [
     {name = "David Knowles", email = "dknowles2@gmail.com"},
 ]
 dependencies    = ["aiohttp ", "apischema", "gql[aiohttp]", "graphql-core"]
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 dynamic         = ["readme", "version"]
 license         = {text = "Apache License 2.0"}
 keywords        = ["hydrawise", "api", "iot"]
 classifiers     = [
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [project.urls]
 "Homepage"      = "https://github.com/dknowles2/pydrawise"
 "Source Code"   = "https://github.com/dknowles2/pydrawise"
 "Bug Reports"   = "https://github.com/dknowles2/pydrawise/issues"
```

### Comparing `pydrawise-2023.5.0/tests/test_auth.py` & `pydrawise-2023.5.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.0/tests/test_client.py` & `pydrawise-2023.5.1/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from gql import Client
 from gql.client import AsyncClientSession
 from graphql import print_ast
 from pytest import fixture
 
 from pydrawise.auth import Auth
 from pydrawise.client import Hydrawise
-from pydrawise.schema import Controller, Zone, ZoneSuspension, deserialize
+from pydrawise.schema import Controller, Zone, ZoneSuspension
+from pydrawise.schema_utils import deserialize
 
 
 @fixture
 def mock_auth():
     mock_auth = create_autospec(Auth, spec_set=True, instance=True)
     mock_auth.token.return_value = "__token__"
     yield mock_auth
```

