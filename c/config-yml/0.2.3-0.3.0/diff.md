# Comparing `tmp/config_yml-0.2.3.tar.gz` & `tmp/config_yml-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_yml-0.2.3.tar", last modified: Sat May  6 08:13:11 2023, max compression
+gzip compressed data, was "config_yml-0.3.0.tar", last modified: Wed May 17 12:35:03 2023, max compression
```

## Comparing `config_yml-0.2.3.tar` & `config_yml-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:11.512197 config_yml-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-06 08:13:11.512197 config_yml-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 08:13:01.000000 config_yml-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:11.512197 config_yml-0.2.3/config_yml/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-06 08:13:01.000000 config_yml-0.2.3/config_yml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-06 08:13:01.000000 config_yml-0.2.3/config_yml/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:11.512197 config_yml-0.2.3/config_yml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-06 08:13:11.000000 config_yml-0.2.3/config_yml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-06 08:13:11.000000 config_yml-0.2.3/config_yml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:13:11.000000 config_yml-0.2.3/config_yml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 08:13:11.000000 config_yml-0.2.3/config_yml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 08:13:11.000000 config_yml-0.2.3/config_yml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:13:11.512197 config_yml-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-06 08:13:01.000000 config_yml-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:11.512197 config_yml-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:01.000000 config_yml-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:11.512197 config_yml-0.2.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:01.000000 config_yml-0.2.3/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 08:13:01.000000 config_yml-0.2.3/tests/data/config_existing.yml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 08:13:01.000000 config_yml-0.2.3/tests/data/config_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-06 08:13:01.000000 config_yml-0.2.3/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:35:03.539859 config_yml-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-17 12:35:03.539859 config_yml-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-17 12:34:53.000000 config_yml-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:35:03.535859 config_yml-0.3.0/config_yml/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 12:34:53.000000 config_yml-0.3.0/config_yml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-17 12:34:53.000000 config_yml-0.3.0/config_yml/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:35:03.539859 config_yml-0.3.0/config_yml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-17 12:35:03.000000 config_yml-0.3.0/config_yml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-17 12:35:03.000000 config_yml-0.3.0/config_yml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:35:03.000000 config_yml-0.3.0/config_yml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 12:35:03.000000 config_yml-0.3.0/config_yml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 12:35:03.000000 config_yml-0.3.0/config_yml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:35:03.539859 config_yml-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-17 12:34:53.000000 config_yml-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:35:03.539859 config_yml-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:34:53.000000 config_yml-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:35:03.539859 config_yml-0.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:34:53.000000 config_yml-0.3.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 12:34:53.000000 config_yml-0.3.0/tests/data/config_existing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 12:34:53.000000 config_yml-0.3.0/tests/data/config_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-05-17 12:34:53.000000 config_yml-0.3.0/tests/test_config.py
```

### Comparing `config_yml-0.2.3/config_yml/config.py` & `config_yml-0.3.0/config_yml/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 """ Config class """
 import os
 import copy
 from pathlib import Path
 import logging
-import yaml
 import shutil
+import yaml
 
 log = logging.getLogger(__name__)
 
 
 class Config:
     """ Manages a config file that will be generated in the /var/ folder
     """
 
-    def __init__(self, package_name: str, template_path: str, config_file_name: str, dry_run_abs_path: str = None):
+    def __init__(self, package_name: str,
+                 template_path: str,
+                 config_file_name: str,
+                 dry_run: bool = False,
+                 dry_run_abs_path: str = None):
         """_summary_
 
         Args:
             package_name (str): Name of the package owner of the config file
             template_path (str): Path of the template file
             config_path (str): Name of config file (will be placed in home/var/{modulename} folder)
-            dry_run_abs_path (str): None if no dry run selected
-                                    "" if dry run selected, with empsty config file
-                                    "{absolute-path}" if dry run selected, starting with an initial file
+            dry_run (bool): If dry run of not
+            dry_run_abs_path (str): "{absolute-path}" if dry run selected, starting with an initial file copied
+                                    "None", if not initial config
         """
         self._template_path = template_path
         self._config_file_name = config_file_name
         self.homevar = os.path.join(str(Path.home()), 'var', package_name)
 
         if not os.path.exists(self.homevar):
             os.makedirs(self.homevar)
 
-        if dry_run_abs_path is not None:
-            self.dry_run = True
+        self.dry_run = dry_run
+
+        if dry_run:
             self.homevar = os.path.join(self.homevar, 'dryrun_config')
             if os.path.exists(self.homevar):
                 shutil.rmtree(self.homevar)
             os.makedirs(self.homevar)
-            if  dry_run_abs_path != "":
-                shutil.copy(dry_run_abs_path,  os.path.join(self.homevar, self._config_file_name))           
-        else:
-            self.dry_run = False
+            if  dry_run_abs_path:
+                shutil.copy(dry_run_abs_path,  os.path.join(self.homevar, self._config_file_name))
 
         self.config = {}
 
         self.read_config()
 
     def __del__(self):
         if self.dry_run:
-            shutil.rmtree(self.homevar)
+            if os.path.exists(self.homevar):
+                shutil.rmtree(self.homevar)
 
     def __getitem__(self, key):
         return self.config.get(key, None)
 
     def get_config_path(self) -> str:
         """Get the path for the config, inside the homevar path
         Args:
```

### Comparing `config_yml-0.2.3/setup.py` & `config_yml-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="config_yml",
-    version="0.2.3",
+    version="0.3.0",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Utility modules for Class management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/config_yml",
     packages=setuptools.find_packages(),
```

### Comparing `config_yml-0.2.3/tests/test_config.py` & `config_yml-0.3.0/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         # Instatiate a config file from scratch, based only on template
         # Will be automatically writen to file
         template_path = f'{Path(__file__).parent}/data/config_template.yml'
         config = Config(
                     package_name="config_yml",
                     template_path=template_path,
                     config_file_name="config_new.yml",
-                    dry_run_abs_path=""
+                    dry_run=True
                   )
 
         try:
             # Check that resulting config file equals the template file
             with open(config.get_config_path(), "r", encoding="utf-8") as config_file:
                 config_read = yaml.load(config_file, Loader=yaml.FullLoader)
                 with open(template_path, "r", encoding="utf-8") as template_config_file:
@@ -115,14 +115,15 @@
 
         # Instatiate a config file from scratch, with an updated template, with an existing config
         template_path = f'{Path(__file__).parent}/data/config_template.yml'
         config = Config(
                         package_name="config_yml",
                         template_path=template_path,
                         config_file_name="config_existing.yml",
+                        dry_run=True,
                         dry_run_abs_path=existing_path
                        )
 
         expected_merged = {
                             "key_template1": "template",
                             "key_template2": "changed",
                             "key_template3": "new in config",
```

