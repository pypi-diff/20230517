# Comparing `tmp/n26-3.3.0.tar.gz` & `tmp/n26-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n26-3.3.0.tar", last modified: Mon Apr 26 22:52:53 2021, max compression
+gzip compressed data, was "n26-3.3.1.tar", last modified: Wed May 17 17:42:22 2023, max compression
```

## Comparing `n26-3.3.0.tar` & `n26-3.3.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 22:52:53.291867 n26-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-04-26 22:52:45.000000 n26-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-04-26 22:52:53.291867 n26-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7342 2021-04-26 22:52:45.000000 n26-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 22:52:53.291867 n26-3.3.0/n26/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-04-26 22:52:45.000000 n26-3.3.0/n26/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-04-26 22:52:45.000000 n26-3.3.0/n26/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21697 2021-04-26 22:52:45.000000 n26-3.3.0/n26/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    22210 2021-04-26 22:52:45.000000 n26-3.3.0/n26/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2021-04-26 22:52:45.000000 n26-3.3.0/n26/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      531 2021-04-26 22:52:45.000000 n26-3.3.0/n26/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2021-04-26 22:52:45.000000 n26-3.3.0/n26/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 22:52:53.291867 n26-3.3.0/n26.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-04-26 22:52:53.000000 n26-3.3.0/n26.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      314 2021-04-26 22:52:53.000000 n26-3.3.0/n26.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-26 22:52:53.000000 n26-3.3.0/n26.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-04-26 22:52:53.000000 n26-3.3.0/n26.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-04-26 22:52:53.000000 n26-3.3.0/n26.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-04-26 22:52:53.000000 n26-3.3.0/n26.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      392 2021-04-26 22:52:45.000000 n26-3.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-04-26 22:52:53.291867 n26-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2021-04-26 22:52:45.000000 n26-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:42:22.668242 n26-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 17:42:13.000000 n26-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 17:42:13.000000 n26-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-17 17:42:22.668242 n26-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-17 17:42:13.000000 n26-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:42:22.668242 n26-3.3.1/n26/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 17:42:13.000000 n26-3.3.1/n26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 17:42:13.000000 n26-3.3.1/n26/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-05-17 17:42:13.000000 n26-3.3.1/n26/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22210 2023-05-17 17:42:13.000000 n26-3.3.1/n26/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 17:42:13.000000 n26-3.3.1/n26/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-17 17:42:13.000000 n26-3.3.1/n26/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-17 17:42:13.000000 n26-3.3.1/n26/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:42:22.668242 n26-3.3.1/n26.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-17 17:42:22.000000 n26-3.3.1/n26.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-17 17:42:22.000000 n26-3.3.1/n26.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:42:22.000000 n26-3.3.1/n26.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-17 17:42:22.000000 n26-3.3.1/n26.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 17:42:22.000000 n26-3.3.1/n26.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 17:42:22.000000 n26-3.3.1/n26.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-17 17:42:13.000000 n26-3.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 17:42:22.668242 n26-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-17 17:42:13.000000 n26-3.3.1/setup.py
```

### Comparing `n26-3.3.0/README.md` & `n26-3.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,19 @@
 # N26 Python CLI/API
+
 [![Build Status](https://github.com/femueller/python-n26/actions/workflows/python-app.yml/badge.svg)](https://github.com/femueller/python-n26/actions/workflows/python-app.yml)
 [![PyPI version](https://img.shields.io/github/pipenv/locked/python-version/femueller/python-n26)](https://img.shields.io/github/pipenv/locked/python-version/femueller/python-n26)
 [![PyPI version](https://badge.fury.io/py/n26.svg)](https://badge.fury.io/py/n26)
 [![Downloads](https://img.shields.io/pypi/dm/n26.svg)](https://img.shields.io/pypi/dm/n26.svg)
 
-- [N26 Python CLI/API](#N26-Python-CLIAPI)
-  - [About](#About)
-  - [Install](#Install)
-  - [Configuration](#Configuration)
-  - [Usage](#Usage)
-    - [CLI example](#CLI-example)
-    - [API example](#API-example)
-  - [Projects using python-n26](#Projects-using-python-n26)
-  - [Contribute](#Contribute)
-    - [Run locally](#Run-locally)
-  - [Maintainers](#Maintainers)
-  - [Credits](#Credits)
-  - [Disclaimer](#Disclaimer)
-  
 [![asciicast](https://asciinema.org/a/260083.svg)](https://asciinema.org/a/260083)
 
 ## About
-[python-n26](https://github.com/femueller/python-n26) is a Python 3.6+ library and Command Line Interface to request information from n26 bank accounts. You can use it to check your balance from the terminal or include it in your own Python projects.
+
+[python-n26](https://github.com/femueller/python-n26) is a Python library and Command Line Interface to request information from N26 bank accounts. You can use it to check your balance from the terminal or include it in your own Python projects.
 
 **Disclaimer:** This is an unofficial community project which is not affiliated with N26 GmbH/N26 Inc.
 
 ## Install
 
 ```shell
 pip3 install n26
@@ -36,45 +24,47 @@
 
 ## Configuration
 
 python-n26 uses [container-app-conf](https://github.com/markusressel/container-app-conf) to provide different options for configuration.
 You can place a YAML (`n26.yaml` or `n26.yml`) or TOML (`n26.toml` or `n26.tml`) configuration file in `./`, `~/` or `~/.config/`. Have a look at the [YAML example](n26.yml.example) and [TOML example](n26.tml.example).
 If you want to use environment variables:
 
-- `N26_USER`: username
-- `N26_PASSWORD`: password
-- `N26_DEVICE_TOKEN`: random [uuid](https://de.wikipedia.org/wiki/Universally_Unique_Identifier) to identify the device
-- `N26_LOGIN_DATA_STORE_PATH`: optional **file** path to store login data (recommended for cli usage)
-- `N26_MFA_TYPE`: `app` will use the paired app as 2 factor authentication, `sms` will use SMS to the registered number.
+-   `N26_USERNAME`: username
+-   `N26_PASSWORD`: password
+-   `N26_DEVICE_TOKEN`: random [uuid](https://de.wikipedia.org/wiki/Universally_Unique_Identifier) to identify the device
+-   `N26_LOGIN_DATA_STORE_PATH`: optional **file** path to store login data (recommended for cli usage)
+-   `N26_MFA_TYPE`: `app` will use the paired app as 2 factor authentication, `sms` will use SMS to the registered number.
 
 Note that **when specifying both** environment variables as well as a config file and a key is present in both locations the **enviroment variable values will be preferred**.
 
 ## Authentication
 
 ### Device Token
 
 Since 17th of June 2020 N26 requires a device_token to differentiate clients. This requires you to specify the `DEVICE_TOKEN`
 config option with a UUID of your choice. To generate a UUID you can use f.ex. one of the following options:
 
 Using python:
+
 ```python
 python -c 'import uuid; print(uuid.uuid4())'
 ```
 
 Using linux built-in tools:
+
 ```shell
 > uuidgen
 ```
 
 Using a website:
 [https://www.uuidgenerator.net/](https://www.uuidgenerator.net/)
 
 ### 2FA
 
-Since 14th of September 2019 N26 requires a login confirmation (2 factor authentication). 
+Since 14th of September 2019 N26 requires a login confirmation (2 factor authentication).
 
 There are two options here:
 
 1. Using the paired phone N26 app to approve login on devices that are not paired. This can be configured by setting `app` as the `mfa_type`. You will receive a notification on your phone when you start using this library to request data. python-n26 checks for your login confirmation every 5 seconds. If you fail to approve the login request within 60 seconds an exception is raised.
 2. Using a code delivered via SMS to your registered phone number as 2 factor authentication. This can be configured by setting `sms` as the `mfa_type`.
 
 If you do not specify a `login_data_store_path` this login information is only stored in memory. In order to avoid that every CLI command requires a new confirmation, the login data retrieved in the above process can be stored on the file system. Please note that **this information must be protected** from the eyes of third parties **at all costs**. You can specify the location to store this data in the [Configuration](#Configuration).
@@ -92,18 +82,19 @@
 
 ```bash
 > N26_USER=user N26_PASSWORD=passwd N26_DEVICE_TOKEN=00000000-0000-0000-0000-000000000000 N26_MFA_TYPE=app n26 balance
 123.45 EUR
 ```
 
 ### JSON output
-If you would like to work with the raw `JSON` rather than the pretty table 
+
+If you would like to work with the raw `JSON` rather than the pretty table
 layout you can use the global `-json` parameter:
 
-```bash 
+```bash
 > n26 -json balance
 {
   "id": "12345678-1234-1234-1234-123456789012",
   "physicalBalance": null,
   "availableBalance": 123.45,
   "usableBalance": 123.45,
   "bankBalance": 123.45,
@@ -121,16 +112,29 @@
   ],
   "externalId": {
     "iban": "DE12345678901234567890"
   }
 }
 ```
 
+### Docker
+
+```shell
+# ensure the n26 folder exists
+mkdir ~/.config/n26
+# mount the config and launch the command
+sudo docker run -it --rm \
+  -v "/home/markus/.config/n26.yaml:/app/n26.yaml" \
+  -v "/home/markus/.config/n26:/.config/n26" \
+  -u 1000:1000 \
+  femueller/python-n26
+```
 
 ### API example
+
 ```python
 from n26.api import Api
 api_client = Api()
 print(api_client.get_balance())
 ```
 
 This is going to use the same mechanism to load configuration as the CLI tool, to specify your own configuration you can use it as:
@@ -146,21 +150,16 @@
 conf.MFA_TYPE.value = "app"
 conf.validate()
 
 api_client = Api(conf)
 print(api_client.get_balance())
 ```
 
-## Projects using python-n26
-
-The following projects are using [python-n26](https://github.com/femueller/python-n26):
-
-* [home-assistant](https://github.com/home-assistant/home-assistant/tree/dev/homeassistant/components/n26): https://www.home-assistant.io/components/n26
-
 ## Contribute
+
 If there are any issues, bugs or missing API endpoints, feel free to contribute by forking the project and creating a Pull-Request.
 
 ### Run locally
 
 Prerequirements: [Pipenv](https://pipenv.readthedocs.io/)
 
 ```shell
@@ -169,29 +168,34 @@
 pipenv shell
 pipenv install
 python3 -m n26 balance
 ```
 
 ### Creating a new release (only for maintainers)
 
-```shell
-# Increment version number in n26/__init__.py
-
-# Create a new release using the Makefile
-make git-release
-```
+1. Increment version number in `n26/__init__.py` according to desired [SemVer](https://semver.org/#summary) release version
+2. Create a new release using the `Makefile`. This creates a new git tag, which triggers the "Upload Python Package" GitHub Action.
+    1. Run `make git-release`, this triggers: [https://github.com/femueller/python-n26/actions/workflows/python-publish.yml]()
+    2. New releases end up at: [https://pypi.org/project/n26/]()
 
 ## Maintainers
-* [Markus Ressel](https://github.com/markusressel)
-* [Felix Mueller](https://github.com/femueller)
+
+-   [Markus Ressel](https://github.com/markusressel)
+-   [Felix Mueller](https://github.com/femueller)
 
 ## Credits
-* [Nick Jüttner](https://github.com/njuettner) for providing [the API authentication flow](https://github.com/njuettner/alexa/blob/master/n26/app.py)
-* [Pierrick Paul](https://github.com/PierrickP/) for providing [the API endpoints](https://github.com/PierrickP/n26/blob/develop/lib/api.js)
+
+-   [Nick Jüttner](https://github.com/njuettner) for providing [the API authentication flow](https://github.com/njuettner/alexa/blob/master/n26/app.py)
+-   [Pierrick Paul](https://github.com/PierrickP/) for providing [the API endpoints](https://github.com/PierrickP/n26/blob/develop/lib/api.js)
 
 ## Similar projects
-* Go: https://github.com/guitmz/n26 by [Guilherme Thomazi Bonicontro](https://github.com/guitmz)
-* Go: https://github.com/njuettner/n26 by [Nick Jüttner](https://github.com/njuettner) (unmaintained)
-* Node https://github.com/PierrickP/n26 by [Pierrick Paul](https://github.com/PierrickP/) (unmaintained)
+
+-   Go: https://github.com/guitmz/n26 by [Guilherme Thomazi Bonicontro](https://github.com/guitmz)
+-   Go: https://github.com/njuettner/n26 by [Nick Jüttner](https://github.com/njuettner) (unmaintained)
+-   Node https://github.com/PierrickP/n26 by [Pierrick Paul](https://github.com/PierrickP/) (unmaintained)
 
 ## Disclaimer
+
 This project is not affiliated with N26 GmbH/N26 Inc. if you want to learn more about it, visit https://n26.com/.
+
+We've been trying [hard to collaborate with N26](https://github.com/femueller/python-n26/issues/107#issuecomment-1008825746) however, it's been always really challenging.  
+There is no guarantee that this project continues to work at any point, since none of the API endpoints are really documented.
```

### Comparing `n26-3.3.0/n26/api.py` & `n26-3.3.1/n26/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from n26.config import Config, MFA_TYPE_SMS
 from n26.const import DAILY_WITHDRAWAL_LIMIT, DAILY_PAYMENT_LIMIT
 from n26.util import create_request_url
 
 LOGGER = logging.getLogger(__name__)
 
 BASE_URL_DE = 'https://api.tech26.de'
-BASE_URL_GLOBAL = 'https://api.tech26.global'
 BASIC_AUTH_HEADERS = {"Authorization": "Basic bmF0aXZld2ViOg=="}
 USER_AGENT = ("Mozilla/5.0 (X11; Linux x86_64) "
               "AppleWebKit/537.36 (KHTML, like Gecko) "
               "Chrome/59.0.3071.86 Safari/537.36")
 
 GET = "get"
 POST = "post"
@@ -476,47 +475,47 @@
         Request an authentication token from the server
         :return: the token or None if the response did not contain a token
         """
         mfa_token = self._initiate_authentication_flow(username, password)
         self._request_mfa_approval(mfa_token)
         return self._complete_authentication_flow(mfa_token)
 
-    @staticmethod
-    def _initiate_authentication_flow(username: str, password: str) -> str:
+    def _initiate_authentication_flow(self, username: str, password: str) -> str:
         LOGGER.debug("Requesting authentication flow for user {}".format(username))
         values_token = {
             "grant_type": GRANT_TYPE_PASSWORD,
             "username": username,
             "password": password
         }
         # TODO: Seems like the user-agent is not necessary but might be a good idea anyway
-        response = requests.post(BASE_URL_GLOBAL + "/oauth2/token", data=values_token, headers=BASIC_AUTH_HEADERS)
+        response = requests.post(f"{self.config.AUTH_BASE_URL.value}/oauth2/token", data=values_token,
+                                 headers=BASIC_AUTH_HEADERS)
         if response.status_code != 403:
             raise ValueError("Unexpected response for initial auth request: {}".format(response.text))
 
         response_data = response.json()
         if response_data.get("error", "") == "mfa_required":
             return response_data["mfaToken"]
         else:
             raise ValueError("Unexpected response data")
 
-    @staticmethod
-    def _refresh_token(refresh_token: str):
+    def _refresh_token(self, refresh_token: str):
         """
         Refreshes an authentication token
         :param refresh_token: the refresh token issued by the server when requesting a token
         :return: the refreshed token data
         """
         LOGGER.debug("Requesting token refresh using refresh_token {}".format(refresh_token))
         values_token = {
             'grant_type': GRANT_TYPE_REFRESH_TOKEN,
             'refresh_token': refresh_token,
         }
 
-        response = requests.post(BASE_URL_GLOBAL + '/oauth2/token', data=values_token, headers=BASIC_AUTH_HEADERS)
+        response = requests.post(f"{self.config.AUTH_BASE_URL.value}/oauth2/token", data=values_token,
+                                 headers=BASIC_AUTH_HEADERS)
         response.raise_for_status()
         return response.json()
 
     def _request_mfa_approval(self, mfa_token: str):
         LOGGER.debug("Requesting MFA approval using mfa_token {}".format(mfa_token))
         mfa_data = {
             "mfaToken": mfa_token
```

### Comparing `n26-3.3.0/n26/cli.py` & `n26-3.3.1/n26/cli.py`

 * *Files identical despite different names*

### Comparing `n26-3.3.0/n26/config.py` & `n26-3.3.1/n26/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,25 @@
                 yaml_source,
                 toml_source
             ]
             kwargs["data_sources"] = data_sources
 
         return super(Config, cls).__new__(cls, *args, **kwargs)
 
+    AUTH_BASE_URL = StringConfigEntry(
+        description="Base URL for N26 Authentication",
+        example="",
+        default="https://api.tech26.de",
+        key_path=[
+            NODE_ROOT,
+            "auth_base_url"
+        ],
+        required=True
+    )
+
     USERNAME = StringConfigEntry(
         description="N26 account username",
         example="john.doe@example.com",
         key_path=[
             NODE_ROOT,
             "username"
         ],
```

### Comparing `n26-3.3.0/n26/const.py` & `n26-3.3.1/n26/const.py`

 * *Files identical despite different names*

### Comparing `n26-3.3.0/n26/util.py` & `n26-3.3.1/n26/util.py`

 * *Files identical despite different names*

### Comparing `n26-3.3.0/setup.py` & `n26-3.3.1/setup.py`

 * *Files identical despite different names*

