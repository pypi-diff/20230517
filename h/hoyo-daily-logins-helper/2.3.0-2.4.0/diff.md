# Comparing `tmp/hoyo-daily-logins-helper-2.3.0.tar.gz` & `tmp/hoyo-daily-logins-helper-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.3.0.tar", last modified: Mon May 15 03:55:52 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.4.0.tar", last modified: Wed May 17 03:01:32 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-2.3.0.tar` & `hoyo-daily-logins-helper-2.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:52.301960 hoyo-daily-logins-helper-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:52.297960 hoyo-daily-logins-helper-2.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:52.301960 hoyo-daily-logins-helper-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-15 03:55:52.301960 hoyo-daily-logins-helper-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:52.301960 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 03:55:52.305960 hoyo-daily-logins-helper-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:52.301960 hoyo-daily-logins-helper-2.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:32.784653 hoyo-daily-logins-helper-2.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/setup.py
```

### Comparing `hoyo-daily-logins-helper-2.3.0/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.4.0/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,14 @@
           python-version: "3.11"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install .
           pip install ruff
       - name: Lint
-        run: ruff check src
+        run: ruff check hoyo_daily_logins_helper
       - name: Build
         run: |
           pip install build
           make build
           make install
           which hoyo-daily-logins-helper
```

### Comparing `hoyo-daily-logins-helper-2.3.0/.gitignore` & `hoyo-daily-logins-helper-2.4.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /.vscode
 /hoyo-daily-logins-helper.toml
 /_hoyo-daily-logins-helper.toml
-src/_version.py
+hoyo_daily_logins_helper/_version.py
 
 # Created by https://www.toptal.com/developers/gitignore/api/windows,macos,linux,python,intellij+all,visualstudiocode
 # Edit at https://www.toptal.com/developers/gitignore?templates=windows,macos,linux,python,intellij+all,visualstudiocode
 
 ### Intellij+all ###
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
 # Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
```

### Comparing `hoyo-daily-logins-helper-2.3.0/LICENSE` & `hoyo-daily-logins-helper-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.3.0/PKG-INFO` & `hoyo-daily-logins-helper-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.3.0
+Version: 2.4.0
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -44,17 +44,20 @@
 ```bash
 $ docker run --rm --env HOYO_GAME=starrail --env HOYO_COOKIE="your cookie string" ghcr.io/atomicptr/hoyo-daily-logins-helper
 ```
 
 ### pip
 
 ```bash
-$ pip install hoyo-daily-logins-helper
+$ pipx install hoyo-daily-logins-helper
 ```
 
+**Note**: While regular pip should work, it's highly recommended installing this
+tool via [pipx](https://pypa.github.io/pipx/) instead!
+
 PyPi: https://pypi.org/project/hoyo-daily-logins-helper/
 
 
 ## Configuration
 
 ### Cookie
```

### Comparing `hoyo-daily-logins-helper-2.3.0/README.md` & `hoyo-daily-logins-helper-2.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,20 @@
 ```bash
 $ docker run --rm --env HOYO_GAME=starrail --env HOYO_COOKIE="your cookie string" ghcr.io/atomicptr/hoyo-daily-logins-helper
 ```
 
 ### pip
 
 ```bash
-$ pip install hoyo-daily-logins-helper
+$ pipx install hoyo-daily-logins-helper
 ```
 
+**Note**: While regular pip should work, it's highly recommended installing this
+tool via [pipx](https://pypa.github.io/pipx/) instead!
+
 PyPi: https://pypi.org/project/hoyo-daily-logins-helper/
 
 
 ## Configuration
 
 ### Cookie
```

### Comparing `hoyo-daily-logins-helper-2.3.0/hoyo-daily-logins-helper.toml.template` & `hoyo-daily-logins-helper-2.4.0/hoyo-daily-logins-helper.toml.template`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.3.0
+Version: 2.4.0
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -44,17 +44,20 @@
 ```bash
 $ docker run --rm --env HOYO_GAME=starrail --env HOYO_COOKIE="your cookie string" ghcr.io/atomicptr/hoyo-daily-logins-helper
 ```
 
 ### pip
 
 ```bash
-$ pip install hoyo-daily-logins-helper
+$ pipx install hoyo-daily-logins-helper
 ```
 
+**Note**: While regular pip should work, it's highly recommended installing this
+tool via [pipx](https://pypa.github.io/pipx/) instead!
+
 PyPi: https://pypi.org/project/hoyo-daily-logins-helper/
 
 
 ## Configuration
 
 ### Cookie
```

### Comparing `hoyo-daily-logins-helper-2.3.0/pyproject.toml` & `hoyo-daily-logins-helper-2.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,14 @@
     "comboparse",
     "scheduler",
     "pytz",
 ]
 dynamic = ["version"]
 
 [project.scripts]
-hoyo-daily-logins-helper = "src.main:main"
+hoyo-daily-logins-helper = "hoyo_daily_logins_helper.main:main"
 
 [tool.setuptools]
 packages = {find = {exclude=["tests*"]}}
 
 [tool.setuptools_scm]
-write_to = "src/_version.py"
+write_to = "hoyo_daily_logins_helper/_version.py"
```

### Comparing `hoyo-daily-logins-helper-2.3.0/requirements.txt` & `hoyo-daily-logins-helper-2.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.3.0/src/games.py` & `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/games.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import logging
 import random
 import time
 from typing import Optional
 
-from src.http import http_get_json, http_post_json
-from src.notifications import NotificationManager, Notification
+from hoyo_daily_logins_helper.http import http_get_json, http_post_json
+from hoyo_daily_logins_helper.notifications import NotificationManager, \
+    Notification
 
 RET_CODE_ALREADY_SIGNED_IN = -5003
 
 GAMES = {
     "genshin": {
         "name": "Genshin Impact",
         "event_base_url": "https://hk4e-api-os.mihoyo.com/event/sol",
```

### Comparing `hoyo-daily-logins-helper-2.3.0/src/http.py` & `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import logging
 from typing import Dict
 
 import requests
 from requests import HTTPError, Response
 
-from src.utils import dict_prettify
+from hoyo_daily_logins_helper.utils import dict_prettify
 
 USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) " \
-              "AppleWebKit/537.36 (KHTML, like Gecko) " \
-              "Chrome/74.0.3729.169 Safari/537.36"
+             "AppleWebKit/537.36 (KHTML, like Gecko) " \
+             "Chrome/74.0.3729.169 Safari/537.36"
 _http_req_settings = {"user_agent": USER_AGENT}
 
 
 def http_set_user_agent(user_agent: str):
     _http_req_settings["user_agent"] = user_agent
 
 
@@ -34,32 +34,32 @@
 def http_post_json(url: str, max_retries: int = 2, **kwargs) -> Dict[str, any]:
     resp = http_post(url, max_retries, **kwargs)
     data = resp.text
     return json.loads(data)
 
 
 def http_request(
-    method: str,
-    url: str,
-    max_retries: int = 2,
-    **kwargs
+        method: str,
+        url: str,
+        max_retries: int = 2,
+        **kwargs
 ) -> Response:
     for i in range(max_retries + 1):
         try:
-            logging.debug(f"{method.upper()} {url}, REQ: {i+1}/{max_retries}")
+            logging.debug(f"{method.upper()} {url}, REQ: {i + 1}/{max_retries}")
             session = requests.Session()
             session.headers["User-Agent"] = _http_req_settings["user_agent"]
             resp = session.request(method, url, **kwargs)
 
             text = resp.text
             if resp.headers.get("Content-Type", "") == "application/json":
                 text = dict_prettify(json.loads(text))
             logging.debug(f"Response: {resp.status_code}\n\n{text}\n")
         except HTTPError as e:
-            logging.error(f"HTTP error: {e}, REQ: {i+1}/{max_retries}")
+            logging.error(f"HTTP error: {e}, REQ: {i + 1}/{max_retries}")
         except KeyError as e:
-            logging.error(f"Wrong response: {e}, REQ: {i+1}/{max_retries}")
+            logging.error(f"Wrong response: {e}, REQ: {i + 1}/{max_retries}")
         except Exception as e:
-            logging.error(f"Unknown error: {e}, REQ: {i+1}/{max_retries}")
+            logging.error(f"Unknown error: {e}, REQ: {i + 1}/{max_retries}")
         else:
             return resp
     raise Exception(f"All {max_retries} HTTP requests have failed")
```

### Comparing `hoyo-daily-logins-helper-2.3.0/src/main.py` & `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,33 +3,42 @@
 import sys
 import tomllib
 from pathlib import Path
 from typing import Optional
 
 import comboparse
 
-from src._version import __version__
-from src.consts import DEFAULT_LANGUAGE
-from src.games import GAMES, game_perform_checkin
-from src.http import http_set_user_agent
-from src.notifications import NotificationManager
-from src.scheduler import run_scheduler
-from src.utils import dict_prettify
+from hoyo_daily_logins_helper._version import __version__
+from hoyo_daily_logins_helper.consts import DEFAULT_LANGUAGE
+from hoyo_daily_logins_helper.games import GAMES, game_perform_checkin
+from hoyo_daily_logins_helper.http import http_set_user_agent
+from hoyo_daily_logins_helper.notifications import NotificationManager
+from hoyo_daily_logins_helper.scheduler import run_scheduler
+from hoyo_daily_logins_helper.utils import dict_prettify
 
 
 def main():
     """ Main function for CLI """
     cli_args = list(sys.argv[1:])
     default_file = Path("hoyo-daily-logins-helper.toml")
 
+    parser = comboparse.ComboParser(
+        prog="hoyo-daily-logins-helper",
+        description="Get hoyo daily login rewards automatically!",
+        env_prefix="HOYO",
+    )
+
     has_config_file = False
     has_single_game_flag = False
     has_legacy_cookie = False
 
-    if "--config-file" in cli_args:
+    if (
+            "--config-file" in cli_args or
+            parser.create_env_var_name("CONFIG_FILE") in os.environ
+    ):
         has_config_file = True
 
     if default_file.exists():
         has_config_file = True
         cli_args.append("--config-file")
         cli_args.append(default_file.absolute().__str__())
 
@@ -39,20 +48,14 @@
 
     # legacy GAME env var
     if "GAME" in os.environ:
         has_single_game_flag = True
     if "COOKIE" in os.environ:
         has_legacy_cookie = True
 
-    parser = comboparse.ComboParser(
-        prog="hoyo-daily-logins-helper",
-        description="Get hoyo daily login rewards automatically!",
-        env_prefix="HOYO",
-    )
-
     parser.add_argument(
         "-c", "--cookie",
         type=str,
         help="the cookie(s) for your accounts",
         action="append",
         required=not has_config_file and not has_legacy_cookie,
         default=[],
@@ -150,18 +153,19 @@
                 args.language = language
 
             user_agent = config_data.get("config", {}).get("user-agent", None)
 
             if user_agent:
                 args.user_agent = user_agent
 
-            enable_scheduler = config_data.get("config", {})\
+            enable_scheduler = config_data.get("config", {}) \
                 .get("enable_scheduler", False)
 
-            notifications = config_data.get("config", {}).get("notifications", [])
+            notifications = config_data.get("config", {}).get("notifications",
+                                                              [])
 
             notification_manager = NotificationManager(notifications)
 
             # parse accounts
             for index, account in enumerate(config_data.get("accounts", [])):
                 game = account.get("game", None)
                 cookie = account.get("cookie", None)
```

### Comparing `hoyo-daily-logins-helper-2.3.0/src/notifications.py` & `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/notifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 from dataclasses import dataclass
 from datetime import datetime
 from typing import List
 
-from src.http import http_post
+from hoyo_daily_logins_helper.http import http_post
 
 
 @dataclass
 class Notification:
     success: bool
     game_name: str
     account_identifier: str
@@ -85,15 +85,14 @@
         })
 
 
 class NotificationManager:
     _handler: List[_NotificationHandler] = []
 
     def __init__(self, notifications: List[dict]):
-        print("yolo", notifications)
         for notification in notifications:
             if "type" not in notification:
                 logging.error(
                     "Notification entry without type found",
                     notification
                 )
                 continue
```

### Comparing `hoyo-daily-logins-helper-2.3.0/src/scheduler.py` & `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/scheduler.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from datetime import datetime, timezone, time
 from time import sleep
 from typing import Optional
 
 import pytz
 from scheduler import Scheduler
 
-from src.games import game_perform_checkin
-from src.notifications import NotificationManager
+from hoyo_daily_logins_helper.games import game_perform_checkin
+from hoyo_daily_logins_helper.notifications import NotificationManager
 
 _RESET_TIME = {
     # running this one hour after reset to prevent potential fuckery with
     # timezones
     "hour": 5,
     "minute": 1,
 }
```

