# Comparing `tmp/mpcontribs-client-5.3.3.tar.gz` & `tmp/mpcontribs-client-5.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.3.3.tar", last modified: Sat May 13 01:56:42 2023, max compression
+gzip compressed data, was "mpcontribs-client-5.3.4.tar", last modified: Wed May 17 18:12:42 2023, max compression
```

## Comparing `mpcontribs-client-5.3.3.tar` & `mpcontribs-client-5.3.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:56:42.050608 mpcontribs-client-5.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-13 01:56:42.050608 mpcontribs-client-5.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:56:42.042608 mpcontribs-client-5.3.3/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:56:42.042608 mpcontribs-client-5.3.3/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (123)    85643 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:56:42.046608 mpcontribs-client-5.3.3/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-13 01:56:41.000000 mpcontribs-client-5.3.3/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-13 01:56:42.000000 mpcontribs-client-5.3.3/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 01:56:41.000000 mpcontribs-client-5.3.3/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 01:56:41.000000 mpcontribs-client-5.3.3/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-13 01:56:41.000000 mpcontribs-client-5.3.3/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-13 01:56:41.000000 mpcontribs-client-5.3.3/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:56:42.050608 mpcontribs-client-5.3.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 01:56:42.050608 mpcontribs-client-5.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:56:42.050608 mpcontribs-client-5.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-13 01:56:26.000000 mpcontribs-client-5.3.3/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.809394 mpcontribs-client-5.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-17 18:12:42.809394 mpcontribs-client-5.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.797393 mpcontribs-client-5.3.4/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.797393 mpcontribs-client-5.3.4/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    85863 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.801393 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.805394 mpcontribs-client-5.3.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:12:42.809394 mpcontribs-client-5.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.805394 mpcontribs-client-5.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/tests/test_client.py
```

### Comparing `mpcontribs-client-5.3.3/LICENSE` & `mpcontribs-client-5.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.3/PKG-INFO` & `mpcontribs-client-5.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.3.3
+Version: 5.3.4
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.3.3/README.md` & `mpcontribs-client-5.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.3/mpcontribs/client/__init__.py` & `mpcontribs-client-5.3.4/mpcontribs/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from pint import UnitRegistry
 from pint.unit import UnitDefinition
 from pint.converters import ScaleConverter
 from pint.errors import DimensionalityError
 from tempfile import gettempdir
 
 RETRIES = 3
-MAX_WORKERS = 8
+MAX_WORKERS = 3
 MAX_ELEMS = 10
 MAX_NESTING = 5
 MEGABYTES = 1024 * 1024
 MAX_BYTES = 2.4 * MEGABYTES
 MAX_PAYLOAD = 15 * MEGABYTES
 MAX_COLUMNS = 160
 DEFAULT_HOST = "contribs-api.materialsproject.org"
@@ -210,21 +210,22 @@
         chunk = tuple(itertools.islice(it, n))
         if not chunk:
             return
         yield chunk
 
 
 def get_session(session=None):
-    # TODO add Bad Gateway 502?
     adapter_kwargs = dict(max_retries=Retry(
         total=RETRIES,
         read=RETRIES,
         connect=RETRIES,
         respect_retry_after_header=True,
-        status_forcelist=[429],  # rate limit
+        status_forcelist=[429, 502],  # rate limit
+        allowed_methods={'DELETE', 'GET', 'PUT', 'POST'},
+        backoff_factor=2
     ))
     return FuturesSession(
         session=session if session else _session,
         max_workers=MAX_WORKERS, adapter_kwargs=adapter_kwargs
     )
 
 
@@ -481,15 +482,15 @@
                         responses[tid]["result"] = response.result
                     if hasattr(response, "count"):
                         responses[tid]["count"] = response.count
 
                 elapsed = time.perf_counter() - start
                 timed_out = timeout > 0 and elapsed > timeout
 
-                if timed_out or not response.ok:
+                if timed_out:
                     for fut in futures:
                         fut.cancel()
 
     return responses
 
 
 @functools.lru_cache(maxsize=1000)
@@ -1776,17 +1777,20 @@
                     id2project[cid] = project_name
 
         existing = defaultdict(dict)
         unique_identifiers = defaultdict(dict)
         project_names = list(project_names)
 
         if not skip_dupe_check and len(collect_ids) != len(contributions):
-            unique_identifiers = self.get_unique_identifiers_flags({"name__in": project_names})
+            nproj = len(project_names)
+            query = {"name__in": project_names} if nproj > 1 else {"name": project_names[0]}
+            unique_identifiers = self.get_unique_identifiers_flags(query)
+            query = {"project__in": project_names} if nproj > 1 else {"project": project_names[0]}
             existing = defaultdict(dict, self.get_all_ids(
-                dict(project__in=project_names), include=COMPONENTS, timeout=timeout
+                query, include=COMPONENTS, timeout=timeout
             ))
 
         # prepare contributions
         contribs = defaultdict(list)
         digests = {project_name: defaultdict(set) for project_name in project_names}
         fields = [
             comp
```

### Comparing `mpcontribs-client-5.3.3/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.3.4/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.3.3
+Version: 5.3.4
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.3.3/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.3.4/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.3/requirements/deployment.txt` & `mpcontribs-client-5.3.4/requirements/deployment.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
@@ -79,15 +79,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/macos-latest_py3.10.txt` & `mpcontribs-client-5.3.4/requirements/macos-latest_py3.10.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
@@ -79,15 +79,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/macos-latest_py3.10_extras.txt` & `mpcontribs-client-5.3.4/requirements/macos-latest_py3.10_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
@@ -91,15 +91,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/macos-latest_py3.8.txt` & `mpcontribs-client-5.3.4/requirements/macos-latest_py3.8.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
@@ -83,15 +83,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/macos-latest_py3.8_extras.txt` & `mpcontribs-client-5.3.4/requirements/macos-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
@@ -95,15 +95,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/macos-latest_py3.9.txt` & `mpcontribs-client-5.3.4/requirements/macos-latest_py3.9.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
@@ -81,15 +81,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/macos-latest_py3.9_extras.txt` & `mpcontribs-client-5.3.4/requirements/macos-latest_py3.9_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
@@ -93,15 +93,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.10.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
@@ -77,15 +77,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
@@ -89,15 +89,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.8.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
@@ -81,15 +81,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
@@ -93,15 +93,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.9.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
@@ -79,15 +79,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.0
+emmet-core==0.55.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
@@ -91,15 +91,15 @@
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
```

### Comparing `mpcontribs-client-5.3.3/setup.py` & `mpcontribs-client-5.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.3/tests/test_client.py` & `mpcontribs-client-5.3.4/tests/test_client.py`

 * *Files identical despite different names*

