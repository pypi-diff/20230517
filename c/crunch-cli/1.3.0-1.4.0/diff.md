# Comparing `tmp/crunch-cli-1.3.0.tar.gz` & `tmp/crunch-cli-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.3.0.tar", last modified: Mon May 15 11:21:11 2023, max compression
+gzip compressed data, was "crunch-cli-1.4.0.tar", last modified: Wed May 17 10:59:36 2023, max compression
```

## Comparing `crunch-cli-1.3.0.tar` & `crunch-cli-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:21:11.632765 crunch-cli-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 11:21:11.632765 crunch-cli-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:21:11.628765 crunch-cli-1.3.0/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:21:11.628765 crunch-cli-1.3.0/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:21:11.628765 crunch-cli-1.3.0/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:21:11.632765 crunch-cli-1.3.0/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:21:11.632765 crunch-cli-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:59:36.409298 crunch-cli-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-17 10:59:36.409298 crunch-cli-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:59:36.405298 crunch-cli-1.4.0/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:59:36.405298 crunch-cli-1.4.0/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:59:36.405298 crunch-cli-1.4.0/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:59:36.409298 crunch-cli-1.4.0/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-17 10:59:36.000000 crunch-cli-1.4.0/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-17 10:59:36.000000 crunch-cli-1.4.0/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:59:36.000000 crunch-cli-1.4.0/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 10:59:36.000000 crunch-cli-1.4.0/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:59:36.000000 crunch-cli-1.4.0/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 10:59:36.000000 crunch-cli-1.4.0/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 10:59:36.000000 crunch-cli-1.4.0/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:59:36.409298 crunch-cli-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-17 10:59:30.000000 crunch-cli-1.4.0/setup.py
```

### Comparing `crunch-cli-1.3.0/crunch/command/convert.py` & `crunch-cli-1.4.0/crunch/command/convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import re
 import typing
 
 import astor
 import click
 
-from .. import constants
+from .. import constants, utils
 
 
 def convert_cells(cells: typing.List[typing.Any]):
     module = ast.Module()
     module.body = []
 
     for index, cell in enumerate(cells):
@@ -21,19 +21,15 @@
             print(f"convert {cell_id} {message}")
 
         cell_type = cell["cell_type"]
         if cell_type != "code":
             log(f"skip since not code: {cell_type}")
             continue
 
-        source = "\n".join(
-            line
-            for line in cell["source"]
-            if not re.match(r"^\s*?(!|%|#)", line)
-        )
+        source = utils.strip_python_special_lines(cell["source"])
 
         if not len(source):
             log(f"skip since empty (without !bash, %magic and #comment)")
             continue
 
         valid = 0
         tree = ast.parse(source)
```

### Comparing `crunch-cli-1.3.0/crunch/command/download.py` & `crunch-cli-1.4.0/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.3.0/crunch/command/push.py` & `crunch-cli-1.4.0/crunch/command/push.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.3.0/crunch/command/setup.py` & `crunch-cli-1.4.0/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.3.0/crunch/command/test.py` & `crunch-cli-1.4.0/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.3.0/crunch/constants.py` & `crunch-cli-1.4.0/crunch/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 DOT_CRUNCHDAO_DIRECTORY = ".crunchdao"
 DOT_DATA_DIRECTORY = "data"
 TOKEN_FILE = "token"
 PROJECT_FILE = "project"
 DOT_GITIGNORE_FILE = ".gitignore"
+REQUIREMENTS_TXT = "requirements.txt"
 CONVERTED_MAIN_PY = "__converted_main.py"
 DEFAULT_MODEL_DIRECTORY = "resources"
 
 IGNORED_FILES = [
     ".git/",
     f"{DOT_CRUNCHDAO_DIRECTORY}/",
     f"{DOT_DATA_DIRECTORY}/",
```

### Comparing `crunch-cli-1.3.0/crunch/demo-project/.gitignore` & `crunch-cli-1.4.0/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.3.0/crunch/demo-project/main.py` & `crunch-cli-1.4.0/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.3.0/crunch/ensure.py` & `crunch-cli-1.4.0/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.3.0/crunch/inline.py` & `crunch-cli-1.4.0/crunch/inline.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 import typing
 
 import click
 import pandas
 
-from . import command, constants, tester, utils, api
+from . import command, constants, tester, utils, api, library
 
 
 class _Inline:
 
     def __init__(self, module: typing.Any, model_directory: str):
         self.module = module
         self.model_directory = model_directory
@@ -18,15 +18,15 @@
         self.session = utils.CustomSession(
             os.environ.get(constants.WEB_BASE_URL_ENV_VAR, constants.WEB_BASE_URL_DEFAULT),
             os.environ.get(constants.API_BASE_URL_ENV_VAR, constants.API_BASE_URL_DEFAULT),
             bool(os.environ.get(constants.DEBUG_ENV_VAR, "False")),
         )
 
         print(f"loaded inline runner with module: {module}")
-    
+
     def load_data(self) -> typing.Tuple[pandas.DataFrame, pandas.DataFrame, pandas.DataFrame]:
         try:
             (
                 _,
                 _,
                 x_train_path,
                 y_train_path,
@@ -39,15 +39,24 @@
         x_train = utils.read(x_train_path)
         y_train = utils.read(y_train_path)
         x_test = utils.read(x_test_path)
 
         return x_train, y_train, x_test
 
     def test(self, force_first_train=True, train_frequency=1, raise_abort=False):
+        tester.install_logger()
+
         try:
+            library.scan(
+                self.session,
+                module=self.module
+            )
+
+            logging.warn('')
+
             return tester.run(
                 self.module,
                 self.session,
                 self.model_directory,
                 force_first_train,
                 train_frequency,
             )
@@ -61,9 +70,9 @@
 
 
 def load(module_or_module_name: typing.Any, model_directory=constants.DEFAULT_MODEL_DIRECTORY):
     if isinstance(module_or_module_name, str):
         module = sys.modules[module_or_module_name]
     else:
         module = module_or_module_name
-    
+
     return _Inline(module, model_directory)
```

### Comparing `crunch-cli-1.3.0/crunch/main.py` & `crunch-cli-1.4.0/crunch/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
+import logging
 
 import click
 
-from . import command, constants, utils, api
+from . import command, constants, utils, api, library, tester
 
 session = None
 debug = False
 
 
 @click.group()
 @click.option("--debug", "enable_debug", envvar=constants.DEBUG_ENV_VAR, is_flag=True, help="Enable debug output.")
@@ -121,21 +122,28 @@
 
 
 @cli.command(help="Test your code locally.")
 @click.option("--main-file", "main_file_path", default="main.py", show_default=True, help="Entrypoint of your code.")
 @click.option("--model-directory", "model_directory_path", default="resources", show_default=True, help="Directory where your model is stored.")
 @click.option("--no-force-first-train", is_flag=True, help="Do not force the train at the first loop.")
 @click.option("--train-frequency", default=1, show_default=True, help="Train interval.")
+@click.option("--skip-library-check", is_flag=True, help="Skip forbidden library check.")
 def test(
     main_file_path: str,
     model_directory_path: str,
     no_force_first_train: bool,
     train_frequency: int,
+    skip_library_check: bool
 ):
     utils.change_root()
+    tester.install_logger()
+
+    if not skip_library_check and os.path.exists(constants.REQUIREMENTS_TXT):
+        library.scan(session, requirements_file=constants.REQUIREMENTS_TXT)
+        logging.warn('')
 
     command.test(
         session,
         main_file_path=main_file_path,
         model_directory_path=model_directory_path,
         force_first_train=not no_force_first_train,
         train_frequency=train_frequency,
```

### Comparing `crunch-cli-1.3.0/crunch/tester.py` & `crunch-cli-1.4.0/crunch/tester.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,26 +23,36 @@
 
     while bytes >= 1024 and suffix_index < 8:
         bytes /= 1024
         suffix_index += 1
 
     return f"{bytes:,.2f} {suffixes[suffix_index]}"
 
+_logged_installed = False
+def install_logger():
+    global _logged_installed
+    if _logged_installed:
+        return
+    
+    coloredlogs.install(
+        level=logging.INFO,
+        fmt='%(asctime)s %(message)s',
+        datefmt='%H:%M:%S',
+    )
+
+    _logged_installed = True
+
 def run(
     module: typing.Any,
     session: requests.Session,
     model_directory_path: str,
     force_first_train: bool,
     train_frequency: int,
 ):
-    coloredlogs.install(
-        level=logging.INFO,
-        fmt='%(asctime)s %(message)s',
-        datefmt='%H:%M:%S',
-    )
+    install_logger()
 
     logging.info('running local test')
     logging.warn("internet access isn't restricted, no check will be done")
     logging.info("")
 
     memory_before = _get_process_memory()
     start = time.time()
```

### Comparing `crunch-cli-1.3.0/crunch/utils.py` & `crunch-cli-1.4.0/crunch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 import traceback
 import typing
 import urllib
 import urllib.parse
+import re
 
 import click
 import joblib
 import pandas
 import requests
 
 from . import constants, api
@@ -94,15 +95,15 @@
 def _read_crunchdao_file(name: str, raise_if_missing: bool):
     path = os.path.join(constants.DOT_CRUNCHDAO_DIRECTORY, name)
 
     if not os.path.exists(path):
         if raise_if_missing:
             print(f"{path}: not found, are you in a project directory?")
             raise click.Abort()
-        
+
         return None
 
     with open(path) as fd:
         return fd.read()
 
 
 def read_project_name():
@@ -133,7 +134,15 @@
 
 
 def guess_extension(dataframe: typing.Union[pandas.DataFrame, typing.Any]):
     if isinstance(dataframe, pandas.DataFrame):
         return "parquet"
 
     return "joblib"
+
+
+def strip_python_special_lines(lines: typing.List[str]):
+    return "\n".join(
+        line
+        for line in lines
+        if not re.match(r"^\s*?(!|%|#)", line)
+    )
```

### Comparing `crunch-cli-1.3.0/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.4.0/crunch_cli.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 crunch/__init__.py
 crunch/__version__.py
 crunch/api.py
 crunch/constants.py
 crunch/ensure.py
 crunch/inline.py
+crunch/library.py
 crunch/main.py
 crunch/tester.py
 crunch/utils.py
 crunch/command/__init__.py
 crunch/command/convert.py
 crunch/command/download.py
 crunch/command/push.py
```

### Comparing `crunch-cli-1.3.0/setup.py` & `crunch-cli-1.4.0/setup.py`

 * *Files identical despite different names*

