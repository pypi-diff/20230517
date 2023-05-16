# Comparing `tmp/himon-0.3.2.tar.gz` & `tmp/himon-0.4.0.tar.gz`

## Comparing `himon-0.3.2.tar` & `himon-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 himon-0.3.2/.editorconfig
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 himon-0.3.2/.flake8
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 himon-0.3.2/.gitattributes
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 himon-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 himon-0.3.2/.readthedocs.yaml
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 himon-0.3.2/mkdocs.yaml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 himon-0.3.2/.github/dependabot.yaml
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 himon-0.3.2/.github/workflows/publishing.yaml
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 himon-0.3.2/.github/workflows/testing.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 himon-0.3.2/docs/index.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 himon-0.3.2/docs/himon/__init__.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 himon-0.3.2/docs/himon/exceptions.md
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 himon-0.3.2/docs/himon/league_of_comic_geeks.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 himon-0.3.2/docs/himon/sqlite_cache.md
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 himon-0.3.2/docs/himon/schemas/__init__.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 himon-0.3.2/docs/himon/schemas/comic.md
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 himon-0.3.2/docs/himon/schemas/search_result.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 himon-0.3.2/docs/himon/schemas/series.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 himon-0.3.2/docs/img/favicon.ico
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 himon-0.3.2/himon/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 himon-0.3.2/himon/exceptions.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 himon-0.3.2/himon/league_of_comic_geeks.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 himon-0.3.2/himon/sqlite_cache.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 himon-0.3.2/himon/schemas/__init__.py
--rw-r--r--   0        0        0     8360 2020-02-02 00:00:00.000000 himon-0.3.2/himon/schemas/comic.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 himon-0.3.2/himon/schemas/search_result.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 himon-0.3.2/himon/schemas/series.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 himon-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0   184320 2020-02-02 00:00:00.000000 himon-0.3.2/tests/cache.sqlite
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 himon-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 himon-0.3.2/tests/test_comic.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 himon-0.3.2/tests/test_exceptions.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 himon-0.3.2/tests/test_init.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 himon-0.3.2/tests/test_search_result.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 himon-0.3.2/tests/test_series.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 himon-0.3.2/.gitignore
--rw-r--r--   0        0        0    32473 2020-02-02 00:00:00.000000 himon-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 himon-0.3.2/README.md
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 himon-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 himon-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 himon-0.4.0/.editorconfig
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 himon-0.4.0/.gitattributes
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 himon-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 himon-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 himon-0.4.0/mkdocs.yaml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 himon-0.4.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 himon-0.4.0/.github/workflows/publishing.yaml
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 himon-0.4.0/.github/workflows/testing.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 himon-0.4.0/docs/index.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 himon-0.4.0/docs/himon/__init__.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 himon-0.4.0/docs/himon/exceptions.md
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 himon-0.4.0/docs/himon/league_of_comic_geeks.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 himon-0.4.0/docs/himon/sqlite_cache.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 himon-0.4.0/docs/himon/schemas/__init__.md
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 himon-0.4.0/docs/himon/schemas/comic.md
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 himon-0.4.0/docs/himon/schemas/search_result.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 himon-0.4.0/docs/himon/schemas/series.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 himon-0.4.0/docs/img/favicon.ico
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 himon-0.4.0/himon/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 himon-0.4.0/himon/exceptions.py
+-rw-r--r--   0        0        0     9916 2020-02-02 00:00:00.000000 himon-0.4.0/himon/league_of_comic_geeks.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 himon-0.4.0/himon/sqlite_cache.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 himon-0.4.0/himon/schemas/__init__.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 himon-0.4.0/himon/schemas/_validators.py
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 himon-0.4.0/himon/schemas/comic.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 himon-0.4.0/himon/schemas/search_result.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 himon-0.4.0/himon/schemas/series.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 himon-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0   184320 2020-02-02 00:00:00.000000 himon-0.4.0/tests/cache.sqlite
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 himon-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 himon-0.4.0/tests/test_comic.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 himon-0.4.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 himon-0.4.0/tests/test_search_result.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 himon-0.4.0/tests/test_series.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 himon-0.4.0/.gitignore
+-rw-r--r--   0        0        0    32473 2020-02-02 00:00:00.000000 himon-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 himon-0.4.0/README.md
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 himon-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 himon-0.4.0/PKG-INFO
```

### Comparing `himon-0.3.2/.editorconfig` & `himon-0.4.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `himon-0.3.2/.gitattributes` & `himon-0.4.0/.gitattributes`

 * *Files identical despite different names*

### Comparing `himon-0.3.2/.github/workflows/publishing.yaml` & `himon-0.4.0/.github/workflows/publishing.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -13,24 +13,21 @@
       matrix:
         python-version:
           - '3.11'
         os:
           - ubuntu-latest
     runs-on: ${{ matrix.os }}
     steps:
-      #----------------------------------------------
       - name: Checkout repository
         uses: actions/checkout@v3
-      #----------------------------------------------
       - name: Setup python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Setup environment
         run: pip install twine build packaging
-      #----------------------------------------------
       - name: Build project
         run: python -m build
       - name: Check dist
         run: twine check dist/*
       - name: Publish project
         run: twine upload --username __token__ --password ${{ secrets.PYPI_TOKEN }} dist/*
```

### Comparing `himon-0.3.2/docs/img/favicon.ico` & `himon-0.4.0/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `himon-0.3.2/himon/__init__.py` & `himon-0.4.0/himon/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """himon package entry file."""
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 __all__ = ["__version__", "get_cache_root"]
 
 import os
 from pathlib import Path
 
 
 def get_cache_root() -> Path:
     """
     Create and return the path to the cache for Himon, supports XDG_CACHE_HOME env.
 
     Returns:
         The path to the Himon cache folder.
     """
     cache_home = os.getenv("XDG_CACHE_HOME", default=str(Path.home() / ".cache"))
-    folder = Path(cache_home).resolve() / "simyan"
+    folder = Path(cache_home).resolve() / "himon"
     folder.mkdir(parents=True, exist_ok=True)
     return folder
```

### Comparing `himon-0.3.2/himon/league_of_comic_geeks.py` & `himon-0.4.0/himon/league_of_comic_geeks.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,204 +62,235 @@
         self.cache = cache
 
         self.client_secret = client_secret
         self.access_token = access_token
 
     @sleep_and_retry
     @limits(calls=20, period=MINUTE)
-    def _perform_json_get_request(self, url: str, params: Dict[str, str] = None) -> Dict[str, Any]:
+    def _perform_get_request(self, url: str, params: Dict[str, str] = None) -> Dict[str, Any]:
         """
         Make GET request to League of Comic Geeks.
 
         Args:
             url: The url to request information from.
             params: Parameters to add to the request.
+
         Returns:
             Json response from League of Comic Geeks.
+
         Raises:
             ServiceError: If there is an issue with the request or response.
             AuthenticationError:
                 If League of Comic Geeks returns with an invalid API Key or Client Id response.
         """
         if params is None:
             params = {}
 
         try:
             response = get(url, params=params, headers=self.headers, timeout=self.timeout)
             response.raise_for_status()
             return response.json()
-        except ConnectionError:
-            raise ServiceError(f"Unable to connect to `{url}`")
+        except ConnectionError as err:
+            raise ServiceError(f"Unable to connect to `{url}`") from err
         except HTTPError as err:
             if err.response.status_code == 403:
-                raise AuthenticationError("Invalid API Key")
+                raise AuthenticationError("Invalid API Key") from err
             if err.response.status_code == 404:
-                raise ServiceError("Unknown endpoint")
-            raise ServiceError(f"{err.response.status_code}: {err.response.text}")
-        except JSONDecodeError:
-            raise ServiceError(f"Unable to parse response from `{url}` as Json")
-        except ReadTimeout:
-            raise ServiceError("Service took too long to respond")
-
-    def _json_get_request(
-        self, endpoint: str, params: Dict[str, str] = None, skip_cache: bool = False
+                raise ServiceError("Unknown endpoint") from err
+            raise ServiceError(f"{err.response.status_code}: {err.response.text}") from err
+        except JSONDecodeError as err:
+            raise ServiceError(f"Unable to parse response from `{url}` as Json") from err
+        except ReadTimeout as err:
+            raise ServiceError("Service took too long to respond") from err
+
+    def _get_request(
+        self,
+        endpoint: str,
+        params: Dict[str, str] = None,
+        skip_cache: bool = False,
     ) -> Dict[str, Any]:
         """
         Check cache or make GET request to League of Comic Geeks.
 
         Args:
             endpoint: The endpoint to request information from.
             params: Parameters to add to the request.
             skip_cache: Don't save or read from the cache.
+
         Returns:
             Json response from League of Comic Geeks.
+
         Raises:
             ServiceError: If there is an issue with the request or response.
             AuthenticationError:
                 If League of Comic Geeks returns with an invalid API Key or Client Id response.
         """
         if params is None:
             params = {}
 
         url = self.API_URL + endpoint
         cache_params = f"?{urlencode(params)}" if params else ""
         cache_key = f"{url}{cache_params}"
 
-        if self.cache and not skip_cache:
-            cached_response = self.cache.select(cache_key)
-            if cached_response:
-                return cached_response
+        if self.cache and not skip_cache and (cached_response := self.cache.select(cache_key)):
+            return cached_response
 
-        response = self._perform_json_get_request(url=url, params=params)
+        response = self._perform_get_request(url=url, params=params)
 
         if self.cache and not skip_cache:
             self.cache.insert(cache_key, response)
 
         return response
 
     @sleep_and_retry
     @limits(calls=20, period=MINUTE)
-    def _perform_str_get_request(self, url: str, params: Dict[str, str] = None) -> str:
+    def _str_get_request(self, endpoint: str, params: Dict[str, str] = None) -> str:
         """
         Make GET request to League of Comic Geeks, expecting a str response.
 
         Args:
-            url: The url to request information from.
+            endpoint: The endpoint to request information from.
             params: Parameters to add to the request.
+
         Returns:
             String response from League of Comic Geeks.
+
         Raises:
             ServiceError: If there is an issue with the request or response.
             AuthenticationError:
                 If League of Comic Geeks returns with an invalid API Key or Client Id response.
         """
         if params is None:
             params = {}
 
+        url = self.API_URL + endpoint
+
         try:
             response = get(url, params=params, headers=self.headers, timeout=self.timeout)
             response.raise_for_status()
             return response.json()
-        except ConnectionError:
-            raise ServiceError(f"Unable to connect to `{url}`")
+        except ConnectionError as err:
+            raise ServiceError(f"Unable to connect to `{url}`") from err
         except HTTPError as err:
             if err.response.status_code == 403:
-                raise AuthenticationError("Invalid API Key")
+                raise AuthenticationError("Invalid API Key") from err
             if err.response.status_code == 404:
-                raise ServiceError("Unknown endpoint")
-            raise ServiceError(f"{err.response.status_code}: {err.response.text}")
-        except JSONDecodeError:
-            raise ServiceError(f"Unable to parse response from `{url}` as Json")
-        except ReadTimeout:
-            raise ServiceError("Service took too long to respond")
-
-    def _str_get_request(self, endpoint: str, params: Dict[str, str] = None) -> str:
-        """
-        Check cache or make GET request to League of Comic Geeks.
-
-        Args:
-            endpoint: The endpoint to request information from.
-            params: Parameters to add to the request.
-        Returns:
-            String response from League of Comic Geeks.
-        Raises:
-            ServiceError: If there is an issue with the request or response.
-            AuthenticationError:
-                If League of Comic Geeks returns with an invalid API Key or Client Id response.
-        """
-        if params is None:
-            params = {}
-
-        url = self.API_URL + endpoint
-        return self._perform_str_get_request(url=url, params=params)
+                raise ServiceError("Unknown endpoint") from err
+            raise ServiceError(f"{err.response.status_code}: {err.response.text}") from err
+        except JSONDecodeError as err:
+            raise ServiceError(f"Unable to parse response from `{url}` as Json") from err
+        except ReadTimeout as err:
+            raise ServiceError("Service took too long to respond") from err
 
     def generate_access_token(self) -> str:
         """
         Request an access token.
 
         Returns:
             An access token.
+
         Raises:
             ServiceError: If there is an issue with the client id or secret.
         """
         self.headers["X-API-KEY"] = self.client_secret
         return self._str_get_request("/authorize/format/json")
 
     def search(self, search_term: str) -> List[SearchResult]:
         """
         Request a list of search results.
 
         Args:
             search_term: Search query string
         Returns:
             A list of results.
+
         Raises:
             ServiceError: If there is an issue with validating the response.
         """
         try:
             self.headers["X-API-KEY"] = self.access_token
-            results = self._json_get_request("/search/format/json", params={"query": search_term})
+            results = self._get_request("/search/format/json", params={"query": search_term})
             return parse_obj_as(List[SearchResult], results)
         except ValidationError as err:
-            raise ServiceError(err)
+            raise ServiceError(err) from err
 
-    def series(self, series_id: int) -> Series:
+    def get_series(self, series_id: int) -> Series:
         """
         Request data for a Series based on its id.
 
         Args:
             series_id: The Series id.
+
         Returns:
             A Series object.
+
         Raises:
             ServiceError: If there is an issue with validating the response.
         """
         try:
             self.headers["X-API-KEY"] = self.access_token
-            result = self._json_get_request(
-                "/series/format/json", params={"series_id": str(series_id)}
+            result = self._get_request(
+                "/series/format/json",
+                params={"series_id": str(series_id)},
             )
             if "details" in result:
                 result = result["details"]
             return parse_obj_as(Series, result)
         except ValidationError as err:
-            raise ServiceError(err)
+            raise ServiceError(err) from err
 
-    def comic(self, comic_id: int) -> Comic:
+    def series(self, series_id: int) -> Series:
+        """
+        Request data for a Series based on its id.
+
+        **DEPRECATED**: Use get_series()
+
+        Args:
+            series_id: The Series id.
+
+        Returns:
+            A Series object.
+
+        Raises:
+            ServiceError: If there is an issue with validating the response.
+        """
+        return self.get_series(series_id=series_id)
+
+    def get_comic(self, comic_id: int) -> Comic:
         """
         Request data for a Comic based on its id.
 
         Args:
             comic_id: The Comic id.
+
         Returns:
             A Comic object.
+
         Raises:
             ServiceError: If there is an issue with validating the response.
         """
         try:
             self.headers["X-API-KEY"] = self.access_token
-            result = self._json_get_request(
-                "/comic/format/json", params={"comic_id": str(comic_id)}
+            result = self._get_request(
+                "/comic/format/json",
+                params={"comic_id": str(comic_id)},
             )
             return parse_obj_as(Comic, result)
         except ValidationError as err:
-            raise ServiceError(err)
+            raise ServiceError(err) from err
+
+    def comic(self, comic_id: int) -> Comic:
+        """
+        Request data for a Comic based on its id.
+
+        **DEPRECATED**: Use get_comic()
+
+        Args:
+            comic_id: The Comic id.
+
+        Returns:
+            A Comic object.
+
+        Raises:
+            ServiceError: If there is an issue with validating the response.
+        """
+        return self.get_comic(comic_id=comic_id)
```

### Comparing `himon-0.3.2/himon/sqlite_cache.py` & `himon-0.4.0/himon/sqlite_cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,84 @@
 """
 The SQLiteCache module.
 
 This module provides the following classes:
 
 - SQLiteCache
 """
+__all__ = ["SQLiteCache"]
 import json
 import sqlite3
 from datetime import date, timedelta
+from pathlib import Path
 from typing import Any, Dict, Optional
 
 from himon import get_cache_root
 
 
 class SQLiteCache:
     """
     The SQLiteCache object to cache search results from League of Comic Geeks.
 
     Args:
         path: Path to database.
-        expiry: How long to keep cache results, in days.
+        expiry: How long to keep cache results.
 
     Attributes:
-        expiry (Optional[timedelta]): How long to keep cache results, in days.
+        expiry (Optional[int]): How long to keep cache results.
         con (sqlite3.Connection): Database connection
-        cur (sqlite3.Cursor): Database cursor
     """
 
     def __init__(
         self,
-        path: str = get_cache_root() / "cache.sqlite",
+        path: Path = None,
         expiry: Optional[int] = 14,
     ):
-        self.expiry = timedelta(days=expiry) if expiry else None
-        self.con = sqlite3.connect(path)
-        self.cur = self.con.cursor()
-        self.cur.execute("CREATE TABLE IF NOT EXISTS queries (query, response, date_added);")
+        self.expiry = expiry
+        self.con = sqlite3.connect(path or get_cache_root() / "cache.sqlite")
+        self.con.row_factory = sqlite3.Row
+
+        self.con.execute("CREATE TABLE IF NOT EXISTS queries (query, response, query_date);")
         self.delete()
 
     def select(self, query: str) -> Dict[str, Any]:
         """
         Retrieve data from the cache database.
 
         Args:
             query: Search string
         Returns:
             Empty dict or select results.
         """
         if self.expiry:
-            self.cur.execute(
-                "SELECT response FROM queries WHERE query = ? and date_added > ?;",
-                (query, (date.today() - self.expiry).isoformat()),
+            expiry = date.today() - timedelta(days=self.expiry)
+            cursor = self.con.execute(
+                "SELECT * FROM queries WHERE query = ? and query_date > ?;",
+                (query, expiry.isoformat()),
             )
         else:
-            self.cur.execute("SELECT response FROM queries WHERE query = ?;", (query,))
-        results = self.cur.fetchone()
-        if results:
-            return json.loads(results[0])
+            cursor = self.con.execute("SELECT * FROM queries WHERE query = ?;", (query,))
+        if results := cursor.fetchone():
+            return json.loads(results["response"])
         return {}
 
-    def insert(self, query: str, response: str):
+    def insert(self, query: str, response: Dict[str, Any]) -> None:
         """
         Insert data into the cache database.
 
         Args:
             query: Search string
             response: Data to save
         """
-        self.cur.execute(
-            "INSERT INTO queries (query, response, date_added) VALUES (?, ?, ?);",
+        self.con.execute(
+            "INSERT INTO queries (query, response, query_date) VALUES (?, ?, ?);",
             (query, json.dumps(response), date.today().isoformat()),
         )
         self.con.commit()
 
-    def delete(self):
+    def delete(self) -> None:
         """Remove all expired data from the cache database."""
         if not self.expiry:
             return
-        self.cur.execute(
-            "DELETE FROM queries WHERE date_added <= ?;",
-            ((date.today() - self.expiry).isoformat(),),
-        )
+        expiry = date.today() - timedelta(days=self.expiry)
+        self.con.execute("DELETE FROM queries WHERE query_date < ?;", (expiry.isoformat(),))
         self.con.commit()
```

### Comparing `himon-0.3.2/himon/schemas/__init__.py` & `himon-0.4.0/himon/schemas/_validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-"""himon.schemas package entry file."""
 __all__ = ["to_optional_str", "to_optional_int", "to_optional_float", "to_bool"]
 
 import html
 import re
 from typing import Optional
 
 
-def to_optional_int(v) -> Optional[int]:
+def to_optional_int(v: str) -> Optional[int]:
     """
     Convert a Str or 0 to None or return value.
 
     Args:
         v: Value to convert
     Return:
         Value mapped as None or value
@@ -19,15 +18,15 @@
         if not v or int(v) == 0:
             return None
         return int(v)
     except ValueError:
         return None
 
 
-def to_optional_float(v) -> Optional[float]:
+def to_optional_float(v: str) -> Optional[float]:
     """
     Convert a Str or 0 to None or return value.
 
     Args:
         v: Value to convert
     Return:
         Value mapped as None or value
@@ -38,15 +37,15 @@
         if not v or float(v) == 0:
             return None
         return float(v)
     except ValueError:
         return None
 
 
-def to_bool(v) -> bool:
+def to_bool(v: str) -> bool:
     """
     Convert a Str 0/1 to a bool.
 
     Args:
         v: Value to convert
     Return:
         Value mapped as Bool
@@ -56,15 +55,15 @@
     if str(v) == "0":
         return False
     if str(v) == "1":
         return True
     raise ValueError(f"Unknown bool value `{v}`.")
 
 
-def to_optional_str(v) -> Optional[str]:
+def to_optional_str(v: str) -> Optional[str]:
     """
     Convert a Str to None or return html stripped value.
 
     Args:
         v: Value to convert
     Return:
         Value mapped as None or html stripped value
```

### Comparing `himon-0.3.2/himon/schemas/comic.py` & `himon-0.4.0/himon/schemas/comic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,27 @@
 """
 The Comic module.
 
 This module provides the following classes:
 
-- Variant
-- KeyEvent
-- Creator
-- Character
 - Comic
 """
-__all__ = ["Comic", "Character", "Creator", "KeyEvent", "Variant"]
+__all__ = ["Comic"]
 from datetime import date, datetime
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
-from pydantic import BaseModel, Extra, Field, validator
+from pydantic import Field, validator
 
-from himon.schemas import to_bool, to_optional_float, to_optional_int, to_optional_str
+from himon.schemas import BaseModel
+from himon.schemas._validators import to_bool, to_optional_float, to_optional_int, to_optional_str
 from himon.schemas.search_result import SearchResult
 from himon.schemas.series import Series
 
 
-class ComicModel(BaseModel):
-    """Base model for Comic and subclasses."""
-
-    class Config:
-        """Any extra fields will be ignored, strings will have start/end whitespace stripped."""
-
-        anystr_strip_whitespace = True
-        allow_population_by_field_name = True
-        extra = Extra.ignore
-
-
-class Variant(ComicModel):
+class Variant(BaseModel):
     """
     The Variant object contains information for a variant comic.
 
     Attributes:
         date_modified: Date and time when the Variant was last updated.
         price: Price of the Variant.
         release_date: The date the Variant was released.
@@ -46,50 +32,50 @@
     date_modified: datetime
     price: Optional[float] = None
     release_date: date = Field(alias="date_release")
     title: str
     variant_id: int = Field(alias="id")
 
     @validator("price", pre=True)
-    def validate_optional_float(cls, v) -> Optional[float]:
+    def _to_optional_float(cls, v: str) -> Optional[float]:
         """Pydantic validator to convert a Str or 0 to None or return value."""
         return to_optional_float(v)
 
 
-class KeyEvent(ComicModel):
+class KeyEvent(BaseModel):
     """
     The KeyEvent object contains information for a key event.
 
     Attributes:
         character_id: Identifier used by League of Comic Geeks.
         event_id: Identifier used by League of Comic Geeks.
         name: Name/Title of the Event.
-        note:
-        parent_name:
-        type:
+        note: Unknown field
+        parent_name: Unknown field
+        type: Unknown field
         type_id: Identifier used by League of Comic Geeks.
         universe_name: Universe this Event took place in.
     """
 
     character_id: int
     event_id: int = Field(alias="id")
     name: str
     note: Optional[str] = None
-    parent_name: Optional[str] = None  # Unknown field
+    parent_name: Optional[str] = None
     type: int  # How is it different to type_id?
     type_id: int
     universe_name: Optional[str] = None
 
     @validator("note", "parent_name", pre=True)
-    def validate_optional_str(cls, v) -> Optional[str]:
+    def _to_optional_str(cls, v: str) -> Optional[str]:
         """Pydantic validator to convert a Str to None or return html stripped value."""
         return to_optional_str(v)
 
 
-class Creator(ComicModel):
+class Creator(BaseModel):
     """
     The Creator object contains information for a creator.
 
     Attributes:
         creator_id: Identifier used by League of Comic Geeks.
         name: Name/Title of the Creator.
         role: List of roles the Creator has in the comic. Separated by `,`.
@@ -108,76 +94,76 @@
         id_list = self.role_id.split(",")
         role_list = self.role.split(",")
         for index, role_id in enumerate(id_list):
             role_dict[int(role_id)] = role_list[index].strip().title()
         return role_dict
 
 
-class Character(ComicModel):
+class Character(BaseModel):
     """
     The Character object contains information for a character.
 
     Attributes:
         character_id: Identifier used by League of Comic Geeks.
         date_added: Date and time when the Character was added.
         date_modified: Date and time when the Character was last updated.
         full_name: Full name of Character
-        is_enabled:
+        is_enabled: Unknown field
         name: Name/Alias of Character.
-        parent_id:
-        parent_name:
+        parent_id: Unknown field
+        parent_name: Unknown field
         publisher_name: The publisher name of Character.
-        type_id:
+        type_id: Unknown field
         universe_id: Universe id this Character is from.
         universe_name: Universe name this Character is from.
     """
 
     character_id: int = Field(alias="id")
     date_added: datetime
     date_modified: datetime
     full_name: str
     is_enabled: bool = Field(alias="enabled")
     name: str
-    parent_id: Optional[int] = None  # Unknown field
-    parent_name: Optional[str] = None  # Unknown field
+    parent_id: Optional[int] = None
+    parent_name: Optional[str] = None
     publisher_name: Optional[str] = None
     type_id: int
     universe_id: Optional[int] = None
     universe_name: Optional[str] = None
 
     @validator("parent_name", "universe_name", pre=True)
-    def validate_optional_str(cls, v) -> Optional[str]:
+    def _to_optional_str(cls, v: str) -> Optional[str]:
         """Pydantic validator to convert a Str to None or return html stripped value."""
         return to_optional_str(v)
 
     @validator("parent_id", "universe_id", pre=True)
-    def validate_optional_int(cls, v) -> Optional[int]:
+    def _to_optional_int(cls, v: str) -> Optional[int]:
         """Pydantic validator to convert a Str or 0 to None or return value."""
         return to_optional_int(v)
 
     @validator("is_enabled", pre=True)
-    def validate_bool(cls, v) -> bool:
+    def _to_bool(cls, v: str) -> bool:
         """Pydantic validator to convert a Str 0/1 to a bool."""
         return to_bool(v)
 
 
-class Comic(ComicModel):
+class Comic(BaseModel):
     """
     The Comic object contains information for a comic.
 
     Attributes:
         characters: List of Characters in the Comic.
         collected_in: List of Comics this has been collected in.
         comic_id: Identifier used by League of Comic Geeks.
         creators: List of Creators associated with the Comic
         date_added: Date and time when the Comic was added.
         date_modified: Date and time when the Comic was last updated.
         description: Description of the Comic.
         format: Type of Comic.
-        is_enabled:
+        is_enabled: Unknown field
         is_nsfw: Comic has been marked as NSFW
         is_variant: Comic has been marked as Variant
         isbn: ISBN identifier
         key_events: List of Key Events taken place in the Comic.
         page_count: Count of pages in the Comic.
         parent_id: If it is a variant comic, id of the original comic.
         parent_title: If it is a variant comic, title of the origin comic.
@@ -210,33 +196,33 @@
     release_date: date = Field(alias="date_release")
     series: Series
     sku: str
     title: str
     upc: Optional[int] = None
     variants: List[Variant] = Field(default_factory=list)
 
-    def __init__(self, **data):
+    def __init__(self, **data: Any):
         if data["keys"]:
             data["key_events"] = list(data["keys"].values())
         for key, value in data["details"].items():
             data[key] = value
         super().__init__(**data)
 
     @validator("isbn", "parent_id", "upc", pre=True)
-    def validate_optional_int(cls, v) -> Optional[int]:
+    def _to_optional_int(cls, v: str) -> Optional[int]:
         """Pydantic validator to convert a Str or 0 to None or return value."""
         return to_optional_int(v)
 
     @validator("is_enabled", "is_nsfw", "is_variant", pre=True)
-    def validate_bool(cls, v) -> bool:
+    def _to_bool(cls, v: str) -> bool:
         """Pydantic validator to convert a Str 0/1 to a bool."""
         return to_bool(v)
 
     @validator("description", "parent_title", pre=True)
-    def validate_optional_str(cls, v) -> Optional[str]:
+    def _to_optional_str(cls, v: str) -> Optional[str]:
         """Pydantic validator to convert a Str to None or return html stripped value."""
         return to_optional_str(v)
 
     @validator("price", pre=True)
-    def validate_optional_float(cls, v) -> Optional[float]:
+    def _to_optional_float(cls, v: str) -> Optional[float]:
         """Pydantic validator to convert a Str or 0 to None or return value."""
         return to_optional_float(v)
```

### Comparing `himon-0.3.2/himon/schemas/search_result.py` & `himon-0.4.0/himon/schemas/search_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 
 - SearchResult
 """
 __all__ = ["SearchResult"]
 from datetime import date, datetime
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field, validator
+from pydantic import Field, validator
 
-from himon.schemas import to_bool, to_optional_float, to_optional_int, to_optional_str
+from himon.schemas import BaseModel
+from himon.schemas._validators import to_bool, to_optional_float, to_optional_int, to_optional_str
 
 
 class SearchResult(BaseModel):
     """
     The SearchResult object contains information for a search result.
 
     Attributes:
         comic_id: Identifier used by League of Comic Geeks.
         date_modified: Date and time when the Comic was last updated.
         description: Description of the Comic.
         format: Type of Comic.
-        is_enabled:
+        is_enabled: Unknown field
         is_variant: Comic has been marked as Variant.
         parent_id: If it is a variant comic, id of the original comic.
         parent_title: If it is a variant comic, title of the original comic.
         price: Price of Comic.
         publisher_id: The publisher id of the Comic.
         publisher_name: The publisher name of the Comic.
         release_date: The date the Comic was released.
@@ -54,33 +55,26 @@
     series_id: int
     series_name: str
     series_volume: Optional[int] = None
     title: str
     year_begin: int = Field(alias="series_begin")
     year_end: Optional[int] = Field(alias="series_end", default=None)
 
-    class Config:
-        """Any extra fields will be ignored, strings will have start/end whitespace stripped."""
-
-        anystr_strip_whitespace = True
-        allow_population_by_field_name = True
-        extra = Extra.ignore
-
     @validator("parent_id", "series_volume", "year_end", pre=True)
-    def validate_optional_int(cls, v) -> Optional[int]:
+    def _to_optional_int(cls, v: str) -> Optional[int]:
         """Pydantic validator to convert a Str or 0 to None or return value."""
         return to_optional_int(v)
 
     @validator("is_variant", "is_enabled", pre=True)
-    def validate_bool(cls, v) -> bool:
+    def _to_bool(cls, v: str) -> bool:
         """Pydantic validator to convert a Str 0/1 to a bool."""
         return to_bool(v)
 
     @validator("price", pre=True)
-    def validate_optional_float(cls, v) -> Optional[float]:
+    def _to_optional_float(cls, v: str) -> Optional[float]:
         """Pydantic validator to convert a Str or 0 to None or return value."""
         return to_optional_float(v)
 
     @validator("description", "parent_title", pre=True)
-    def validate_optional_str(cls, v) -> Optional[str]:
+    def _to_optional_str(cls, v: str) -> Optional[str]:
         """Pydantic validator to convert a Str to None or return html stripped value."""
         return to_optional_str(v)
```

### Comparing `himon-0.3.2/himon/schemas/series.py` & `himon-0.4.0/himon/schemas/series.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 
 - Series
 """
 __all__ = ["Series"]
 from datetime import datetime
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field, validator
+from pydantic import Field, validator
 
-from himon.schemas import to_bool, to_optional_int, to_optional_str
+from himon.schemas import BaseModel
+from himon.schemas._validators import to_bool, to_optional_int, to_optional_str
 
 
 class Series(BaseModel):
     """
     The Series object contains information for a series.
 
     Attributes:
         date_added: Date and time when the Series was added.
         date_modified: Date and time when the Series was last updated.
         description: Description of the Series.
-        is_enabled:
+        is_enabled: Unknown field
         publisher_id: The publisher id of the Series.
         publisher_name: The publisher name of the Series.
         series_id: Identifier used by League of Comic Geeks.
         title: Name/Title of the Series.
         volume: Volume number.
         year_begin: The year the Series started.
         year_end: The year the Series ended.
@@ -40,28 +41,21 @@
     publisher_name: str
     series_id: int = Field(alias="id")
     title: str
     volume: Optional[int] = None
     year_begin: int
     year_end: Optional[int] = None
 
-    class Config:
-        """Any extra fields will be ignored, strings will have start/end whitespace stripped."""
-
-        anystr_strip_whitespace = True
-        allow_population_by_field_name = True
-        extra = Extra.ignore
-
     @validator("description", pre=True)
-    def validate_optional_str(cls, v) -> Optional[str]:
+    def _to_optional_str(cls, v: str) -> Optional[str]:
         """Pydantic validator to convert a Str to None or return html stripped value."""
         return to_optional_str(v)
 
     @validator("is_enabled", pre=True)
-    def validate_bool(cls, v) -> bool:
+    def _to_bool(cls, v: str) -> bool:
         """Pydantic validator to convert a Str 0/1 to a bool."""
         return to_bool(v)
 
     @validator("volume", "year_end", pre=True)
-    def validate_optional_int(cls, v) -> Optional[int]:
+    def _to_optional_int(cls, v: str) -> Optional[int]:
         """Pydantic validator to convert a Str or 0 to None or return value."""
         return to_optional_int(v)
```

### Comparing `himon-0.3.2/tests/cache.sqlite` & `himon-0.4.0/tests/cache.sqlite`

 * *Files identical despite different names*

### Comparing `himon-0.3.2/tests/conftest.py` & `himon-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `himon-0.3.2/tests/test_comic.py` & `himon-0.4.0/tests/test_comic.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This module contains tests for Comic objects.
 """
 from datetime import date, datetime
 
 from himon.league_of_comic_geeks import LeagueofComicGeeks
 
 
-def test_comic(session: LeagueofComicGeeks):
+def test_comic(session: LeagueofComicGeeks) -> None:
     """Test using the comic endpoint with a valid comic_id."""
     result = session.comic(comic_id=2710631)
     assert result is not None
     assert result.comic_id == 2710631
 
     assert len(result.characters) == 106
     assert len(result.collected_in) == 13
@@ -31,29 +31,29 @@
     assert result.release_date == date(2009, 7, 15)
     assert result.sku == "MAY090106"
     assert result.title == "Blackest Night #1"
     assert result.upc == 76194128446000111
     assert len(result.variants) == 6
 
 
-def test_character_null_publisher(session: LeagueofComicGeeks):
+def test_character_null_publisher(session: LeagueofComicGeeks) -> None:
     """Test the comic endpoint with a comic that has a null character publisher name."""
     result = session.comic(comic_id=4174173)
     assert result is not None
 
     assert result.characters[0].publisher_name is None
 
 
-def test_key_event_null_universe(session: LeagueofComicGeeks):
+def test_key_event_null_universe(session: LeagueofComicGeeks) -> None:
     """Test the comic endpoint with a comic that has a null key event universe name."""
     result = session.comic(comic_id=4174173)
     assert result is not None
 
     assert result.key_events[0].universe_name is None
 
 
-def test_upc_alpha_only(session: LeagueofComicGeeks):
+def test_upc_alpha_only(session: LeagueofComicGeeks) -> None:
     """Test the comic endpoint with a comic that has an invalid character in the upc."""
     result = session.comic(comic_id=6257084)
     assert result is not None
 
     assert result.upc is None
```

### Comparing `himon-0.3.2/tests/test_exceptions.py` & `himon-0.4.0/tests/test_exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,30 +7,33 @@
 
 import pytest
 
 from himon.exceptions import AuthenticationError, ServiceError
 from himon.league_of_comic_geeks import LeagueofComicGeeks
 
 
-def test_unauthorized():
+def test_unauthorized() -> None:
     """Test generating an AuthenticationError."""
     session = LeagueofComicGeeks(
-        client_id="Invalid", client_secret="Invalid", access_token=None, cache=None
+        client_id="Invalid",
+        client_secret="Invalid",  # noqa: S106
+        access_token=None,
+        cache=None,
     )
     with pytest.raises(AuthenticationError):
         session.comic(comic_id=1)
 
 
-def test_not_found(session: LeagueofComicGeeks):
+def test_not_found(session: LeagueofComicGeeks) -> None:
     """Test a 404 Not Found raises a ServiceError."""
     with pytest.raises(ServiceError):
-        session._json_get_request(endpoint="/invalid")
+        session._get_request(endpoint="/invalid")
 
 
-def test_timeout(client_id: str, client_secret: str, access_token: Optional[str]):
+def test_timeout(client_id: str, client_secret: str, access_token: Optional[str]) -> None:
     """Test a TimeoutError for slow responses."""
     session = LeagueofComicGeeks(
         client_id=client_id,
         client_secret=client_secret,
         access_token=access_token,
         timeout=0.1,
         cache=None,
```

### Comparing `himon-0.3.2/tests/test_search_result.py` & `himon-0.4.0/tests/test_search_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This module contains tests for SearchResult objects.
 """
 from datetime import date
 
 from himon.league_of_comic_geeks import LeagueofComicGeeks
 
 
-def test_search_result(session: LeagueofComicGeeks):
+def test_search_result(session: LeagueofComicGeeks) -> None:
     """Test using the search endpoint with a valid comic title."""
     results = session.search(search_term="Blackest Night #1")
     assert len(results) != 0
     result = [x for x in results if x.comic_id == 2710631][0]
     assert result is not None
     assert result.comic_id == 2710631
```

### Comparing `himon-0.3.2/tests/test_series.py` & `himon-0.4.0/tests/test_series.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This module contains tests for Series objects.
 """
 from datetime import datetime
 
 from himon.league_of_comic_geeks import LeagueofComicGeeks
 
 
-def test_series(session: LeagueofComicGeeks):
+def test_series(session: LeagueofComicGeeks) -> None:
     """Test using the series endpoint with a valid series_id."""
     result = session.series(series_id=100096)
     assert result is not None
     assert result.series_id == 100096
 
     assert result.date_added == datetime(2012, 8, 5, 22, 20, 15)
     assert result.is_enabled is True
```

### Comparing `himon-0.3.2/LICENSE.txt` & `himon-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `himon-0.3.2/README.md` & `himon-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 # Himon
 
-[![PyPI - Python](https://img.shields.io/pypi/pyversions/Himon.svg?logo=PyPI&label=Python&style=flat-square)](https://pypi.python.org/pypi/Himon/)
-[![PyPI - Status](https://img.shields.io/pypi/status/Himon.svg?logo=PyPI&label=Status&style=flat-square)](https://pypi.python.org/pypi/Himon/)
-[![PyPI - Version](https://img.shields.io/pypi/v/Himon.svg?logo=PyPI&label=Version&style=flat-square)](https://pypi.python.org/pypi/Himon/)
-[![PyPI - License](https://img.shields.io/pypi/l/Himon.svg?logo=PyPI&label=License&style=flat-square)](https://opensource.org/licenses/GPL-3.0)
+[![PyPI - Python](https://img.shields.io/pypi/pyversions/Himon.svg?logo=Python&label=Python&style=flat-square)](https://pypi.python.org/pypi/Himon/)
+[![PyPI - Status](https://img.shields.io/pypi/status/Himon.svg?logo=Python&label=Status&style=flat-square)](https://pypi.python.org/pypi/Himon/)
+[![PyPI - Version](https://img.shields.io/pypi/v/Himon.svg?logo=Python&label=Version&style=flat-square)](https://pypi.python.org/pypi/Himon/)
+[![PyPI - License](https://img.shields.io/pypi/l/Himon.svg?logo=Python&label=License&style=flat-square)](https://opensource.org/licenses/GPL-3.0)
 
-[![Hatch](https://img.shields.io/badge/Packaging-Hatch-4051b5?logo=hatch&style=flat-square)](https://github.com/pypa/hatch)
-[![Pre-Commit](https://img.shields.io/badge/Pre--Commit-Enabled-informational?logo=pre-commit&style=flat-square)](https://github.com/pre-commit/pre-commit)
+[![Hatch](https://img.shields.io/badge/Packaging-Hatch-4051b5?style=flat-square)](https://github.com/pypa/hatch)
+[![Pre-Commit](https://img.shields.io/badge/Pre--Commit-Enabled-informational?style=flat-square&logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Black](https://img.shields.io/badge/Code--Style-Black-000000?style=flat-square)](https://github.com/psf/black)
-[![isort](https://img.shields.io/badge/Imports-isort-informational?style=flat-square)](https://pycqa.github.io/isort/)
-[![Flake8](https://img.shields.io/badge/Linter-Flake8-informational?style=flat-square)](https://github.com/PyCQA/flake8)
+[![Ruff](https://img.shields.io/badge/Linter-Ruff-informational?style=flat-square)](https://github.com/charliermarsh/ruff)
 
 [![Github - Contributors](https://img.shields.io/github/contributors/Buried-In-Code/Himon.svg?logo=Github&label=Contributors&style=flat-square)](https://github.com/Buried-In-Code/Himon/graphs/contributors)
-[![Github Action - Code Analysis](https://img.shields.io/github/workflow/status/Buried-In-Code/Himon/Code%20Analysis?logo=Github-Actions&label=Code-Analysis&style=flat-square)](https://github.com/Buried-In-Code/Himon/actions/workflows/code-analysis.yaml)
-[![Github Action - Testing](https://img.shields.io/github/workflow/status/Buried-In-Code/Himon/Testing?logo=Github-Actions&label=Tests&style=flat-square)](https://github.com/Buried-In-Code/Himon/actions/workflows/testing.yaml)
+[![Github Action - Testing](https://img.shields.io/github/actions/workflow/status/Buried-In-Code/Himon/testing.yaml?branch=main&logo=Github&label=Testing&style=flat-square)](https://github.com/Buried-In-Code/Himon/actions/workflows/testing.yaml)
 
 [![Read the Docs](https://img.shields.io/readthedocs/himon?label=Read-the-Docs&logo=Read-the-Docs&style=flat-square)](https://himon.readthedocs.io/en/latest/?badge=latest)
 
 A [Python](https://www.python.org/) wrapper for [League of Comic Geeks](https://leagueofcomicgeeks.com).
 
 ## Installation
 
-### PyPI
-
-1. Make sure you have [Python](https://www.python.org/) installed: `python --version`
-2. Install the library from [PyPI](https://pypi.org/project/himon): `pip install himon`
+```bash
+pip install Himon
+```
 
-### Github
+## Documentation
 
-1. Make sure you have [Python](https://www.python.org/) installed: `python --version`
-2. Clone the repo: `git clone https://github.com/Buried-In-Code/Himon`
-3. Install the library: `pip install .`
+[Read the project documentation](https://himon.readthedocs.io/en/latest/?badge=latest)
 
-## Example Usage
+### Example Usage
 
 ```python
 from himon.league_of_comic_geeks import LeagueofComicGeeks
 from himon.sqlite_cache import SQLiteCache
 
 access_token = None
 session = LeagueofComicGeeks(client_id="Client Id", client_secret="Client Secret", access_token=access_token, cache=SQLiteCache())
@@ -54,18 +49,22 @@
 print(f"Series: {series.series_id} - {series.title}")
 
 # Get Comic by id
 comic = session.comic(comic_id=2710631)
 print(f"Comic: {comic.comic_id} - {comic.title}")
 ```
 
+## Bugs/Requests
+
+Please use the [GitHub issue tracker](https://github.com/Buried-In-Code/Himon/issues) to submit bugs or request features.
+
 ## Notes
 
 Who or what is Himon?
 
 > Himon is a citizen of New Genesis who secretly lives on the planet Apokolips, which is ruled by Darkseid.
 >
 > More details at [Himon (New Earth)](<https://dc.fandom.com/wiki/Himon_(New_Earth)>)
 
 ## Socials
 
-[![Social - Discord](https://img.shields.io/discord/618581423070117932?color=7289DA&label=The-DEV-Environment&logo=discord&style=for-the-badge)](https://discord.gg/nqGMeGg)
+[![Social - Matrix](https://img.shields.io/matrix/The-Dev-Environment:matrix.org?label=The%20Dev%20Environment&logo=matrix&style=for-the-badge)](https://matrix.to/#/#The-Dev-Environment:matrix.org)
```

### Comparing `himon-0.3.2/pyproject.toml` & `himon-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,162 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 authors = [
-  { name = "BuriedInCode", email = "BuriedInCode@tuta.io" }
+  {email = "BuriedInCode@tuta.io", name = "BuriedInCode"}
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Natural Language :: English",
   "Operating System :: MacOS",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX :: Linux",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
   "Topic :: Internet",
   "Typing :: Typed"
 ]
 dependencies = [
-  "pydantic >= 1.10.4",
-  "requests >= 2.28.1",
-  "ratelimit >= 2.2.1"
+  "pydantic >= 1.10.7",
+  "ratelimit >= 2.2.1",
+  "requests >= 2.30.0"
 ]
 description = "A Python wrapper for League of Comic Geeks."
 dynamic = ["version"]
-keywords = ["comics", "comic", "metadata"]
+keywords = ["comic", "comics", "metadata"]
 license = "GPL-3.0-or-later"
 name = "Himon"
 readme = "README.md"
-requires-python = ">= 3.7"
+requires-python = ">= 3.8"
 
 [project.optional-dependencies]
 dev = [
-  "pre-commit >= 2.21.0",
+  "pre-commit >= 3.3.1"
 ]
 docs = [
-  "mkdocs >= 1.4.2",
-  "mkdocstrings[python] >= 0.19.1",
-  "mkdocs-include-markdown-plugin >= 4.0.3"
+  "mkdocs >= 1.4.3",
+  "mkdocs-include-markdown-plugin >= 4.0.4",
+  "mkdocs-material >= 9.1.11",
+  "mkdocstrings[python] >= 0.21.2"
 ]
 test = [
-  "pytest >= 7.2.0",
+  "pytest >= 7.3.1",
   "pytest-cov >= 4.0.0",
+  "pytest-pretty >= 1.2.0"
 ]
 
 [project.urls]
 Documentation = "https://himon.readthedocs.io/en/latest/"
 Homepage = "https://pypi.org/project/Himon"
 Issues = "https://github.com/Buried-In-Code/Himon/issues"
 Source = "https://github.com/Buried-In-Code/Himon"
 
-[tool.bandit]
-recursive = true
-skips = ["B101", "B106"]
-
 [tool.black]
 line-length = 100
-target-version = ["py37", "py38", "py39", "py310", "py311"]
+target-version = ["py310", "py311", "py38", "py39"]
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.coverage.run]
 source = ["himon"]
 
 [tool.hatch.version]
 path = "himon/__init__.py"
 
-[tool.isort]
-default_section = "THIRDPARTY"
-line_length = 100
-profile = "black"
-
 [tool.pytest.ini_options]
-addopts = ["--cov", "-x"]
+addopts = ["--cov"]
+
+[tool.ruff]
+fix = true
+format = "grouped"
+ignore = [
+  "A001",
+  "A003",
+  "ANN101",
+  "ANN102",
+  "ANN204",
+  "ANN206",
+  "ANN401",
+  "C901",
+  "D107",
+  "D212",
+  "RET504",
+  "SIM105"
+]
+line-length = 100
+select = [
+  "A",
+  "ANN",
+  "ARG",
+  "B",
+  "BLE",
+  "C40",
+  "C90",
+  "COM",
+  "D",
+  "DJ",
+  "E",
+  "ERA",
+  "F",
+  "G",
+  "I",
+  "ICN",
+  "INP",
+  "ISC",
+  "N",
+  "NPY",
+  "PD",
+  "PGH",
+  "PIE",
+  "PLC",
+  "PLE",
+  "PLW",
+  "PT",
+  "PTH",
+  "PYI",
+  "Q",
+  "RET",
+  "RSE",
+  "RUF",
+  "S",
+  "SIM",
+  "SLF",
+  "T10",
+  "T20",
+  "TCH",
+  "TID",
+  "UP",
+  "W",
+  "YTT"
+]
+show-fixes = true
+target-version = "py38"
+
+[tool.ruff.flake8-annotations]
+allow-star-arg-any = true
+mypy-init-return = true
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.ruff.isort]
+combine-as-imports = true
+
+[tool.ruff.mccabe]
+max-complexity = 18
+
+[tool.ruff.pep8-naming]
+classmethod-decorators = ["classmethod", "pydantic.validator"]
+
+[tool.ruff.per-file-ignores]
+"tests/test_*.py" = ["S101", "SLF001"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
```

### Comparing `himon-0.3.2/PKG-INFO` & `himon-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Himon
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Python wrapper for League of Comic Geeks.
 Project-URL: Documentation, https://himon.readthedocs.io/en/latest/
 Project-URL: Homepage, https://pypi.org/project/Himon
 Project-URL: Issues, https://github.com/Buried-In-Code/Himon/issues
 Project-URL: Source, https://github.com/Buried-In-Code/Himon
 Author-email: BuriedInCode <BuriedInCode@tuta.io>
 License-Expression: GPL-3.0-or-later
@@ -14,71 +14,67 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Requires-Dist: pydantic>=1.10.4
+Requires-Python: >=3.8
+Requires-Dist: pydantic>=1.10.7
 Requires-Dist: ratelimit>=2.2.1
-Requires-Dist: requests>=2.28.1
+Requires-Dist: requests>=2.30.0
 Provides-Extra: dev
-Requires-Dist: pre-commit>=2.21.0; extra == 'dev'
+Requires-Dist: pre-commit>=3.3.1; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: mkdocs-include-markdown-plugin>=4.0.3; extra == 'docs'
-Requires-Dist: mkdocs>=1.4.2; extra == 'docs'
-Requires-Dist: mkdocstrings[python]>=0.19.1; extra == 'docs'
+Requires-Dist: mkdocs-include-markdown-plugin>=4.0.4; extra == 'docs'
+Requires-Dist: mkdocs-material>=9.1.11; extra == 'docs'
+Requires-Dist: mkdocs>=1.4.3; extra == 'docs'
+Requires-Dist: mkdocstrings[python]>=0.21.2; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest-cov>=4.0.0; extra == 'test'
-Requires-Dist: pytest>=7.2.0; extra == 'test'
+Requires-Dist: pytest-pretty>=1.2.0; extra == 'test'
+Requires-Dist: pytest>=7.3.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Himon
 
-[![PyPI - Python](https://img.shields.io/pypi/pyversions/Himon.svg?logo=PyPI&label=Python&style=flat-square)](https://pypi.python.org/pypi/Himon/)
-[![PyPI - Status](https://img.shields.io/pypi/status/Himon.svg?logo=PyPI&label=Status&style=flat-square)](https://pypi.python.org/pypi/Himon/)
-[![PyPI - Version](https://img.shields.io/pypi/v/Himon.svg?logo=PyPI&label=Version&style=flat-square)](https://pypi.python.org/pypi/Himon/)
-[![PyPI - License](https://img.shields.io/pypi/l/Himon.svg?logo=PyPI&label=License&style=flat-square)](https://opensource.org/licenses/GPL-3.0)
+[![PyPI - Python](https://img.shields.io/pypi/pyversions/Himon.svg?logo=Python&label=Python&style=flat-square)](https://pypi.python.org/pypi/Himon/)
+[![PyPI - Status](https://img.shields.io/pypi/status/Himon.svg?logo=Python&label=Status&style=flat-square)](https://pypi.python.org/pypi/Himon/)
+[![PyPI - Version](https://img.shields.io/pypi/v/Himon.svg?logo=Python&label=Version&style=flat-square)](https://pypi.python.org/pypi/Himon/)
+[![PyPI - License](https://img.shields.io/pypi/l/Himon.svg?logo=Python&label=License&style=flat-square)](https://opensource.org/licenses/GPL-3.0)
 
-[![Hatch](https://img.shields.io/badge/Packaging-Hatch-4051b5?logo=hatch&style=flat-square)](https://github.com/pypa/hatch)
-[![Pre-Commit](https://img.shields.io/badge/Pre--Commit-Enabled-informational?logo=pre-commit&style=flat-square)](https://github.com/pre-commit/pre-commit)
+[![Hatch](https://img.shields.io/badge/Packaging-Hatch-4051b5?style=flat-square)](https://github.com/pypa/hatch)
+[![Pre-Commit](https://img.shields.io/badge/Pre--Commit-Enabled-informational?style=flat-square&logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Black](https://img.shields.io/badge/Code--Style-Black-000000?style=flat-square)](https://github.com/psf/black)
-[![isort](https://img.shields.io/badge/Imports-isort-informational?style=flat-square)](https://pycqa.github.io/isort/)
-[![Flake8](https://img.shields.io/badge/Linter-Flake8-informational?style=flat-square)](https://github.com/PyCQA/flake8)
+[![Ruff](https://img.shields.io/badge/Linter-Ruff-informational?style=flat-square)](https://github.com/charliermarsh/ruff)
 
 [![Github - Contributors](https://img.shields.io/github/contributors/Buried-In-Code/Himon.svg?logo=Github&label=Contributors&style=flat-square)](https://github.com/Buried-In-Code/Himon/graphs/contributors)
-[![Github Action - Code Analysis](https://img.shields.io/github/workflow/status/Buried-In-Code/Himon/Code%20Analysis?logo=Github-Actions&label=Code-Analysis&style=flat-square)](https://github.com/Buried-In-Code/Himon/actions/workflows/code-analysis.yaml)
-[![Github Action - Testing](https://img.shields.io/github/workflow/status/Buried-In-Code/Himon/Testing?logo=Github-Actions&label=Tests&style=flat-square)](https://github.com/Buried-In-Code/Himon/actions/workflows/testing.yaml)
+[![Github Action - Testing](https://img.shields.io/github/actions/workflow/status/Buried-In-Code/Himon/testing.yaml?branch=main&logo=Github&label=Testing&style=flat-square)](https://github.com/Buried-In-Code/Himon/actions/workflows/testing.yaml)
 
 [![Read the Docs](https://img.shields.io/readthedocs/himon?label=Read-the-Docs&logo=Read-the-Docs&style=flat-square)](https://himon.readthedocs.io/en/latest/?badge=latest)
 
 A [Python](https://www.python.org/) wrapper for [League of Comic Geeks](https://leagueofcomicgeeks.com).
 
 ## Installation
 
-### PyPI
-
-1. Make sure you have [Python](https://www.python.org/) installed: `python --version`
-2. Install the library from [PyPI](https://pypi.org/project/himon): `pip install himon`
+```bash
+pip install Himon
+```
 
-### Github
+## Documentation
 
-1. Make sure you have [Python](https://www.python.org/) installed: `python --version`
-2. Clone the repo: `git clone https://github.com/Buried-In-Code/Himon`
-3. Install the library: `pip install .`
+[Read the project documentation](https://himon.readthedocs.io/en/latest/?badge=latest)
 
-## Example Usage
+### Example Usage
 
 ```python
 from himon.league_of_comic_geeks import LeagueofComicGeeks
 from himon.sqlite_cache import SQLiteCache
 
 access_token = None
 session = LeagueofComicGeeks(client_id="Client Id", client_secret="Client Secret", access_token=access_token, cache=SQLiteCache())
@@ -96,18 +92,22 @@
 print(f"Series: {series.series_id} - {series.title}")
 
 # Get Comic by id
 comic = session.comic(comic_id=2710631)
 print(f"Comic: {comic.comic_id} - {comic.title}")
 ```
 
+## Bugs/Requests
+
+Please use the [GitHub issue tracker](https://github.com/Buried-In-Code/Himon/issues) to submit bugs or request features.
+
 ## Notes
 
 Who or what is Himon?
 
 > Himon is a citizen of New Genesis who secretly lives on the planet Apokolips, which is ruled by Darkseid.
 >
 > More details at [Himon (New Earth)](<https://dc.fandom.com/wiki/Himon_(New_Earth)>)
 
 ## Socials
 
-[![Social - Discord](https://img.shields.io/discord/618581423070117932?color=7289DA&label=The-DEV-Environment&logo=discord&style=for-the-badge)](https://discord.gg/nqGMeGg)
+[![Social - Matrix](https://img.shields.io/matrix/The-Dev-Environment:matrix.org?label=The%20Dev%20Environment&logo=matrix&style=for-the-badge)](https://matrix.to/#/#The-Dev-Environment:matrix.org)
```

