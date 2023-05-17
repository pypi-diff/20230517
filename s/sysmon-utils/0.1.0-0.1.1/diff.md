# Comparing `tmp/sysmon_utils-0.1.0.tar.gz` & `tmp/sysmon_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysmon_utils-0.1.0.tar", max compression
+gzip compressed data, was "sysmon_utils-0.1.1.tar", max compression
```

## Comparing `sysmon_utils-0.1.0.tar` & `sysmon_utils-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/LICENSE
--rw-r--r--   0        0        0     1753 2023-05-16 17:54:32.278162 sysmon_utils-0.1.0/README.md
--rw-r--r--   0        0        0      528 2023-05-17 12:56:05.825263 sysmon_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/sysmon_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/sysmon_utils/commands/__init__.py
--rw-r--r--   0        0        0    23945 2023-05-16 17:54:33.594184 sysmon_utils-0.1.0/sysmon_utils/commands/main_app.py
--rw-r--r--   0        0        0      177 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/sysmon_utils/config.py
--rw-r--r--   0        0        0      677 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/sysmon_utils/main.py
--rw-r--r--   0        0        0        0 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/sysmon_utils/utils/__init__.py
--rw-r--r--   0        0        0      471 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/sysmon_utils/utils/arg_definitions.py
--rw-r--r--   0        0        0     4008 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/sysmon_utils/utils/dataset.py
--rw-r--r--   0        0        0      774 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/sysmon_utils/utils/events.py
--rw-r--r--   0        0        0     3390 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/sysmon_utils/utils/filters.py
--rw-r--r--   0        0        0     5053 2023-05-16 16:04:24.608680 sysmon_utils-0.1.0/sysmon_utils/utils/merge.py
--rw-r--r--   0        0        0     5554 2023-05-16 16:07:10.559366 sysmon_utils-0.1.0/sysmon_utils/utils/rules.py
--rw-r--r--   0        0        0     2363 1970-01-01 00:00:00.000000 sysmon_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-16 16:04:24.608680 sysmon_utils-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2069 2023-05-17 13:40:59.194040 sysmon_utils-0.1.1/README.md
+-rw-r--r--   0        0        0      591 2023-05-17 13:41:06.758176 sysmon_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 16:04:24.608680 sysmon_utils-0.1.1/sysmon_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:04:24.608680 sysmon_utils-0.1.1/sysmon_utils/commands/__init__.py
+-rw-r--r--   0        0        0    24021 2023-05-17 13:27:42.283662 sysmon_utils-0.1.1/sysmon_utils/commands/main_app.py
+-rw-r--r--   0        0        0      177 2023-05-16 16:04:24.608680 sysmon_utils-0.1.1/sysmon_utils/config.py
+-rw-r--r--   0        0        0      703 2023-05-17 13:27:58.935960 sysmon_utils-0.1.1/sysmon_utils/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:04:24.608680 sysmon_utils-0.1.1/sysmon_utils/utils/__init__.py
+-rw-r--r--   0        0        0      471 2023-05-16 16:04:24.608680 sysmon_utils-0.1.1/sysmon_utils/utils/arg_definitions.py
+-rw-r--r--   0        0        0     4008 2023-05-16 16:04:24.608680 sysmon_utils-0.1.1/sysmon_utils/utils/dataset.py
+-rw-r--r--   0        0        0      774 2023-05-16 16:04:24.608680 sysmon_utils-0.1.1/sysmon_utils/utils/events.py
+-rw-r--r--   0        0        0     3390 2023-05-16 16:04:24.608680 sysmon_utils-0.1.1/sysmon_utils/utils/filters.py
+-rw-r--r--   0        0        0     5053 2023-05-16 16:04:24.608680 sysmon_utils-0.1.1/sysmon_utils/utils/merge.py
+-rw-r--r--   0        0        0     5554 2023-05-16 16:07:10.559366 sysmon_utils-0.1.1/sysmon_utils/utils/rules.py
+-rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 sysmon_utils-0.1.1/PKG-INFO
```

### Comparing `sysmon_utils-0.1.0/LICENSE` & `sysmon_utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sysmon_utils-0.1.0/README.md` & `sysmon_utils-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # sysmon_utils
 
-Utilities for working with and testing Sysmon configs against Windows Event Logs. Works in combination with my [atomic-datasets-utils](https://github.com/cnnrshd/atomic-datasets-utils) to support my [sysmon-modular](https://github.com/cnnrshd/sysmon-modular) work. My goal is to make it easier to modify, verify, and test Sysmon configs.
+## NOTICE - In Development
+
+This library is still in development and subject to change. Some commands are a WIP, file and folder structure will be modified. Be sure to use `sysmon_utils --help` to get a list of all commands.
+
+Utilities for working with and testing Sysmon configs against Windows Event Logs. Works in combination with my [atomic-datasets-utils](https://github.com/cnnrshd/atomic-datasets-utils) to support my [sysmon-modular](https://github.com/cnnrshd/sysmon-modular) work. My goal is to make it easier to modify, verify, and test Sysmon configs. Development is sponsored by my (Connor Shade) employer [QOMPLX](https://www.qomplx.com/).
 
 ## Commands
 
 ### atomictests
 
 Checks for techniques found or overruled. Designed to run against the output of [atomic-datasets-utils](https://github.com/cnnrshd/atomic-datasets-utils) to test Sysmon Config functionality.
```

### Comparing `sysmon_utils-0.1.0/sysmon_utils/commands/main_app.py` & `sysmon_utils-0.1.1/sysmon_utils/commands/main_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import json
 import os
 import pathlib
 import re
 from dataclasses import asdict, dataclass
 from enum import Enum
 
-from config import config
+from sysmon_utils.config import config
 from lxml import etree
 from rich.progress import Progress
 from typer import Argument, BadParameter, FileText, FileTextWrite, Option, Typer
-from utils.arg_definitions import OUTFILE, SYSMON_CONFIG, WEL_LOGFILE
-from utils.dataset import (
+from sysmon_utils.utils.arg_definitions import OUTFILE, SYSMON_CONFIG, WEL_LOGFILE
+from sysmon_utils.utils.dataset import (
     extract_json_file,
     filter_files_by_pattern,
     get_working_datasets,
 )
-from utils.events import EVENT_LOOKUP
-from utils.merge import (
+from sysmon_utils.utils.events import EVENT_LOOKUP
+from sysmon_utils.utils.merge import (
     detect_file_format,
     merge_sysmon_configs,
     merge_with_base_config,
     read_file_list,
 )
-from utils.rules import Rule, extract_rules, get_techniques, rule_generator
+from sysmon_utils.utils.rules import Rule, extract_rules, get_techniques, rule_generator
 
 console = config.console
 DEBUG = config.debug
 
 app = Typer(
     rich_markup_mode="markdown",
 )
@@ -386,15 +386,15 @@
 
 
 ######
 # Test
 ######
 
 
-HELP_TEST_SECDATASETS = ":construction: WIP :construction: Tests CONFIG against data from [Security-Datasets](https://securitydatasets.com/introduction.html) Datasets"
+HELP_TEST_SECDATASETS = ":construction: WIP :construction: Tts CONFIG against data from [Security-Datasets](https://securitydatasets.com/introduction.html) Datasets"
 
 
 @app.command(
     name="secdatasets",
     short_help=HELP_TEST_SECDATASETS,
     help=""":construction: WIP :construction: Tests CONFIG against data from [Security-Datasets](https://securitydatasets.com/introduction.html).
     Be sure to specify outfile
```

### Comparing `sysmon_utils-0.1.0/sysmon_utils/main.py` & `sysmon_utils-0.1.1/sysmon_utils/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 __author__ = "Connor Shade"
 
 from rich.traceback import install as rich_log_install
 
 rich_log_install(show_locals=False)
 import logging
 
-from commands.main_app import app as main_app
-from config import config
+from sysmon_utils.commands.main_app import app as main_app
+from sysmon_utils.config import config
 from typer import Option
 
 console = config.console
 
 
 @main_app.callback()
 def main_config(debug: bool = Option(False, help="Enable debugging")):
```

### Comparing `sysmon_utils-0.1.0/sysmon_utils/utils/dataset.py` & `sysmon_utils-0.1.1/sysmon_utils/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `sysmon_utils-0.1.0/sysmon_utils/utils/events.py` & `sysmon_utils-0.1.1/sysmon_utils/utils/events.py`

 * *Files identical despite different names*

### Comparing `sysmon_utils-0.1.0/sysmon_utils/utils/filters.py` & `sysmon_utils-0.1.1/sysmon_utils/utils/filters.py`

 * *Files identical despite different names*

### Comparing `sysmon_utils-0.1.0/sysmon_utils/utils/merge.py` & `sysmon_utils-0.1.1/sysmon_utils/utils/merge.py`

 * *Files identical despite different names*

### Comparing `sysmon_utils-0.1.0/sysmon_utils/utils/rules.py` & `sysmon_utils-0.1.1/sysmon_utils/utils/rules.py`

 * *Files identical despite different names*

### Comparing `sysmon_utils-0.1.0/PKG-INFO` & `sysmon_utils-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysmon-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for working with and testing Sysmon configs.
 License: MIT
 Author: Connor Shade
 Author-email: cnnrshd@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,19 @@
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # sysmon_utils
 
-Utilities for working with and testing Sysmon configs against Windows Event Logs. Works in combination with my [atomic-datasets-utils](https://github.com/cnnrshd/atomic-datasets-utils) to support my [sysmon-modular](https://github.com/cnnrshd/sysmon-modular) work. My goal is to make it easier to modify, verify, and test Sysmon configs.
+## NOTICE - In Development
+
+This library is still in development and subject to change. Some commands are a WIP, file and folder structure will be modified. Be sure to use `sysmon_utils --help` to get a list of all commands.
+
+Utilities for working with and testing Sysmon configs against Windows Event Logs. Works in combination with my [atomic-datasets-utils](https://github.com/cnnrshd/atomic-datasets-utils) to support my [sysmon-modular](https://github.com/cnnrshd/sysmon-modular) work. My goal is to make it easier to modify, verify, and test Sysmon configs. Development is sponsored by my (Connor Shade) employer [QOMPLX](https://www.qomplx.com/).
 
 ## Commands
 
 ### atomictests
 
 Checks for techniques found or overruled. Designed to run against the output of [atomic-datasets-utils](https://github.com/cnnrshd/atomic-datasets-utils) to test Sysmon Config functionality.
```

