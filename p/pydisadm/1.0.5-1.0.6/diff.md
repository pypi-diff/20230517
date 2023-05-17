# Comparing `tmp/pydisadm-1.0.5.tar.gz` & `tmp/pydisadm-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.0.5.tar", max compression
+gzip compressed data, was "pydisadm-1.0.6.tar", max compression
```

## Comparing `pydisadm-1.0.5.tar` & `pydisadm-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     2131 2023-05-16 14:57:57.488005 pydisadm-1.0.5/README.md
--rw-r--r--   0        0        0      111 2023-05-16 14:57:57.488005 pydisadm-1.0.5/pydisadm/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-16 14:57:57.488005 pydisadm-1.0.5/pydisadm/__main__.py
--rw-r--r--   0        0        0     1120 2023-05-16 14:57:57.488005 pydisadm-1.0.5/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     5874 2023-05-16 14:57:57.488005 pydisadm-1.0.5/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0      539 2023-05-16 14:57:57.488005 pydisadm-1.0.5/pydisadm/bot/utils.py
--rw-r--r--   0        0        0      649 2023-05-16 14:57:57.488005 pydisadm-1.0.5/pydisadm/configuration.py
--rw-r--r--   0        0        0     6012 2023-05-16 14:57:57.488005 pydisadm-1.0.5/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0   368313 2023-05-16 14:57:57.492005 pydisadm-1.0.5/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-16 14:57:57.492005 pydisadm-1.0.5/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-16 14:57:57.508005 pydisadm-1.0.5/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      441 2023-05-16 14:57:57.508005 pydisadm-1.0.5/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0      940 2023-05-16 14:57:57.508005 pydisadm-1.0.5/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0      947 2023-05-16 14:57:57.512005 pydisadm-1.0.5/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     2976 2023-05-16 14:57:57.512005 pydisadm-1.0.5/pydisadm/services/database.py
--rw-r--r--   0        0        0     1164 2023-05-16 14:57:57.512005 pydisadm-1.0.5/pydisadm/services/esi.py
--rw-r--r--   0        0        0      372 2023-05-16 14:57:57.512005 pydisadm-1.0.5/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      521 2023-05-16 14:57:57.512005 pydisadm-1.0.5/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      120 2023-05-16 14:57:57.512005 pydisadm-1.0.5/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      894 2023-05-16 14:58:27.595876 pydisadm-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 pydisadm-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2363 2023-05-17 03:38:22.468533 pydisadm-1.0.6/README.md
+-rw-r--r--   0        0        0      111 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1120 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     5874 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0      539 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0      850 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/configuration.py
+-rw-r--r--   0        0        0     6012 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0   368313 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      441 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0      940 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0      947 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     2976 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1164 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      372 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      521 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      120 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      934 2023-05-17 03:38:58.333031 pydisadm-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 pydisadm-1.0.6/PKG-INFO
```

### Comparing `pydisadm-1.0.5/README.md` & `pydisadm-1.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # EVE ADM Bot
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/agelito/adm-bot/ci-cd.yml)
 ![PyPI](https://img.shields.io/pypi/v/pydisadm)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pydisadm)
+[![codecov](https://codecov.io/gh/agelito/adm-bot/branch/main/graph/badge.svg?token=OHRY3OW18Y)](https://codecov.io/gh/agelito/adm-bot)
 
 This is a discord bot which will collect alliance system ADM's daily and provide commands to display them in a convenient tier list.
 
 ## ⚡ Quick Start
 
 ### From PyPI
 ```shell
@@ -56,9 +57,16 @@
 - `DISCORD_APP_ID` - the bot application ID
 - `ALLIANCE_ID` - the alliance ID for collecting ADM values, only systems owned by this alliance will be collected.
 
 ## 🔍 Caveats
 * The ADM data from ESI is only updated once a day, so refreshing more often than that is not necessary.
 * The database will continue to fill up with historic entries, manually inspect size and purge older entries if it's too big.
 
+## 🚧 Development
+
+### Run Unit Tests
+```shell
+pytest tests/ --cov=pydisadm --cov-branch
+```
+
 ## 💡 Credits
 Project is forked from and inspired by [@anjode](https://www.github.com/anjode)
```

### Comparing `pydisadm-1.0.5/pydisadm/__main__.py` & `pydisadm-1.0.6/pydisadm/__main__.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/bot/adm_bot.py` & `pydisadm-1.0.6/pydisadm/bot/adm_bot.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/bot/adm_cog.py` & `pydisadm-1.0.6/pydisadm/bot/adm_cog.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/bot/utils.py` & `pydisadm-1.0.6/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/controller/adm_controller.py` & `pydisadm-1.0.6/pydisadm/controller/adm_controller.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/data/mapConstellations.csv` & `pydisadm-1.0.6/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/data/mapRegions.csv` & `pydisadm-1.0.6/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.0.6/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/loader/static_data.py` & `pydisadm-1.0.6/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.0.6/pydisadm/runnable/runnable_refresh.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/services/database.py` & `pydisadm-1.0.6/pydisadm/services/database.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/services/esi.py` & `pydisadm-1.0.6/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pydisadm/utils/plot_utils.py` & `pydisadm-1.0.6/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.5/pyproject.toml` & `pydisadm-1.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.0.5"
+version = "1.0.6"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
 
@@ -18,14 +18,16 @@
 tabulate = "^0.9.0"
 matplotlib = "^3.7.1"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.4"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version"
```

### Comparing `pydisadm-1.0.5/PKG-INFO` & `pydisadm-1.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,15 @@
 Description-Content-Type: text/markdown
 
 # EVE ADM Bot
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/agelito/adm-bot/ci-cd.yml)
 ![PyPI](https://img.shields.io/pypi/v/pydisadm)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pydisadm)
+[![codecov](https://codecov.io/gh/agelito/adm-bot/branch/main/graph/badge.svg?token=OHRY3OW18Y)](https://codecov.io/gh/agelito/adm-bot)
 
 This is a discord bot which will collect alliance system ADM's daily and provide commands to display them in a convenient tier list.
 
 ## ⚡ Quick Start
 
 ### From PyPI
 ```shell
@@ -79,10 +80,17 @@
 - `DISCORD_APP_ID` - the bot application ID
 - `ALLIANCE_ID` - the alliance ID for collecting ADM values, only systems owned by this alliance will be collected.
 
 ## 🔍 Caveats
 * The ADM data from ESI is only updated once a day, so refreshing more often than that is not necessary.
 * The database will continue to fill up with historic entries, manually inspect size and purge older entries if it's too big.
 
+## 🚧 Development
+
+### Run Unit Tests
+```shell
+pytest tests/ --cov=pydisadm --cov-branch
+```
+
 ## 💡 Credits
 Project is forked from and inspired by [@anjode](https://www.github.com/anjode)
```

