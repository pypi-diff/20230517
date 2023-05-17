# Comparing `tmp/yambs-1.1.0.tar.gz` & `tmp/yambs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.1.0.tar", last modified: Wed May 17 02:44:16 2023, max compression
+gzip compressed data, was "yambs-1.2.0.tar", last modified: Wed May 17 09:28:24 2023, max compression
```

## Comparing `yambs-1.1.0.tar` & `yambs-1.2.0.tar`

### file list

```diff
@@ -1,55 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 02:43:13.000000 yambs-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-17 02:44:16.654503 yambs-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-05-17 02:43:13.000000 yambs-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-17 02:43:13.000000 yambs-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 02:44:16.654503 yambs-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-17 02:43:13.000000 yambs-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.650503 yambs-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-17 02:43:13.000000 yambs-1.1.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-17 02:43:13.000000 yambs-1.1.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.650503 yambs-1.1.0/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.650503 yambs-1.1.0/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/schemas/Toolchain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.550675 yambs-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 09:27:00.000000 yambs-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-17 09:28:24.550675 yambs-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-17 09:27:00.000000 yambs-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-17 09:27:00.000000 yambs-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:28:24.550675 yambs-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-17 09:27:00.000000 yambs-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.542675 yambs-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-17 09:27:00.000000 yambs-1.2.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-17 09:27:00.000000 yambs-1.2.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.542675 yambs-1.2.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.546675 yambs-1.2.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.546675 yambs-1.2.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.546675 yambs-1.2.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.546675 yambs-1.2.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/schemas/Toolchain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.550675 yambs-1.2.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.550675 yambs-1.2.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/generate/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/generate/ninja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.550675 yambs-1.2.0/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-05-17 09:27:00.000000 yambs-1.2.0/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:28:24.546675 yambs-1.2.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-17 09:28:24.000000 yambs-1.2.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-17 09:28:24.000000 yambs-1.2.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:28:24.000000 yambs-1.2.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 09:28:24.000000 yambs-1.2.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 09:28:24.000000 yambs-1.2.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 09:28:24.000000 yambs-1.2.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.1.0/LICENSE` & `yambs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/PKG-INFO` & `yambs-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.1.0
+Version: 1.2.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=6f0dde62ff0b6f57cc4c8520ac87412c
+    hash=36af9eff7b3e51ae48c06f64cde33dcd
     =====================================
 -->
 
-# yambs ([1.1.0](https://pypi.org/project/yambs/))
+# yambs ([1.2.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -150,28 +150,29 @@
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mbs -h
 
-usage: mbs [-h] [--version] [-v] [-C DIR] {gen,noop} ...
+usage: mbs [-h] [--version] [-v] [-C DIR] {gen,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
-  -h, --help         show this help message and exit
-  --version          show program's version number and exit
-  -v, --verbose      set to increase logging verbosity
-  -C DIR, --dir DIR  execute from a specific directory
+  -h, --help          show this help message and exit
+  --version           show program's version number and exit
+  -v, --verbose       set to increase logging verbosity
+  -C DIR, --dir DIR   execute from a specific directory
 
 commands:
-  {gen,noop}         set of available commands
-    gen              poll the source tree and generate any new build files
-    noop             command stub (does nothing)
+  {gen,uf2conv,noop}  set of available commands
+    gen               poll the source tree and generate any new build files
+    uf2conv           Convert to UF2 or flash directly.
+    noop              command stub (does nothing)
 
 ```
 
 ## Sub-command Options
 
 ### `gen`
 
@@ -187,14 +188,46 @@
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
 
 ```
 
+### `uf2conv`
+
+```
+$ ./venv3.11/bin/mbs uf2conv -h
+
+usage: mbs uf2conv [-h] [-b BASE] [-f FAMILY] [-o FILE] [-d DEVICE_PATH] [-l]
+                   [-c] [-D] [-w] [-C] [-i]
+                   [INPUT]
+
+positional arguments:
+  INPUT                 input file (HEX, BIN or UF2)
+
+options:
+  -h, --help            show this help message and exit
+  -b BASE, --base BASE  set base address of application for BIN format
+                        (default: 0x2000)
+  -f FAMILY, --family FAMILY
+                        specify familyID - number or name (default: 0x0)
+  -o FILE, --output FILE
+                        write output to named file; defaults to "flash.uf2" or
+                        "flash.bin" where sensible
+  -d DEVICE_PATH, --device DEVICE_PATH
+                        select a device path to flash
+  -l, --list            list connected devices
+  -c, --convert         do not flash, just convert
+  -D, --deploy          just flash, do not convert
+  -w, --wait            wait for device to flash
+  -C, --carray          convert binary file to a C array, not UF2
+  -i, --info            display header information from UF2, do not convert
+
+```
+
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `yambs`'s source.
 Generated using [pydeps](https://github.com/thebjorn/pydeps) (via
 `mk python-deps`).
```

### Comparing `yambs-1.1.0/README.md` & `yambs-1.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=6f0dde62ff0b6f57cc4c8520ac87412c
+    hash=36af9eff7b3e51ae48c06f64cde33dcd
     =====================================
 -->
 
-# yambs ([1.1.0](https://pypi.org/project/yambs/))
+# yambs ([1.2.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -126,28 +126,29 @@
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mbs -h
 
-usage: mbs [-h] [--version] [-v] [-C DIR] {gen,noop} ...
+usage: mbs [-h] [--version] [-v] [-C DIR] {gen,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
-  -h, --help         show this help message and exit
-  --version          show program's version number and exit
-  -v, --verbose      set to increase logging verbosity
-  -C DIR, --dir DIR  execute from a specific directory
+  -h, --help          show this help message and exit
+  --version           show program's version number and exit
+  -v, --verbose       set to increase logging verbosity
+  -C DIR, --dir DIR   execute from a specific directory
 
 commands:
-  {gen,noop}         set of available commands
-    gen              poll the source tree and generate any new build files
-    noop             command stub (does nothing)
+  {gen,uf2conv,noop}  set of available commands
+    gen               poll the source tree and generate any new build files
+    uf2conv           Convert to UF2 or flash directly.
+    noop              command stub (does nothing)
 
 ```
 
 ## Sub-command Options
 
 ### `gen`
 
@@ -163,14 +164,46 @@
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
 
 ```
 
+### `uf2conv`
+
+```
+$ ./venv3.11/bin/mbs uf2conv -h
+
+usage: mbs uf2conv [-h] [-b BASE] [-f FAMILY] [-o FILE] [-d DEVICE_PATH] [-l]
+                   [-c] [-D] [-w] [-C] [-i]
+                   [INPUT]
+
+positional arguments:
+  INPUT                 input file (HEX, BIN or UF2)
+
+options:
+  -h, --help            show this help message and exit
+  -b BASE, --base BASE  set base address of application for BIN format
+                        (default: 0x2000)
+  -f FAMILY, --family FAMILY
+                        specify familyID - number or name (default: 0x0)
+  -o FILE, --output FILE
+                        write output to named file; defaults to "flash.uf2" or
+                        "flash.bin" where sensible
+  -d DEVICE_PATH, --device DEVICE_PATH
+                        select a device path to flash
+  -l, --list            list connected devices
+  -c, --convert         do not flash, just convert
+  -D, --deploy          just flash, do not convert
+  -w, --wait            wait for device to flash
+  -C, --carray          convert binary file to a C array, not UF2
+  -i, --info            display header information from UF2, do not convert
+
+```
+
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `yambs`'s source.
 Generated using [pydeps](https://github.com/thebjorn/pydeps) (via
 `mk python-deps`).
```

### Comparing `yambs-1.1.0/pyproject.toml` & `yambs-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.1.0"
+version = "1.2.0"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.1.0/setup.py` & `yambs-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/tests/test_entry.py` & `yambs-1.2.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/app.py` & `yambs-1.2.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/commands/gen.py` & `yambs-1.2.0/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/config/__init__.py` & `yambs-1.2.0/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/data/schemas/Chip.yaml` & `yambs-1.2.0/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/data/schemas/Config.yaml` & `yambs-1.2.0/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/data/templates/rules.ninja.j2` & `yambs-1.2.0/yambs/data/templates/rules.ninja.j2`

 * *Files 3% similar despite different names*

```diff
@@ -24,11 +24,14 @@
 
 rule link
   command = $tool $cflags $ldflags -Wl,-Map=$out.map $in -o $out
 
 rule bin
   command = ${toolchain_prefix}objcopy -O binary $in $out
 
+rule hex
+  command = ${toolchain_prefix}objcopy -O ihex $in $out
+
 rule dump
   command = ${toolchain_prefix}objdump -D $in > $out
 
 build_dir = {{build_root}}/$toolchain/$architecture/$cpu
```

### Comparing `yambs-1.1.0/yambs/entry.py` & `yambs-1.2.0/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/generate/__init__.py` & `yambs-1.2.0/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/generate/architectures.py` & `yambs-1.2.0/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/generate/chips.py` & `yambs-1.2.0/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/generate/common.py` & `yambs-1.2.0/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/generate/toolchains.py` & `yambs-1.2.0/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs/schemas.py` & `yambs-1.2.0/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.1.0/yambs.egg-info/PKG-INFO` & `yambs-1.2.0/yambs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.1.0
+Version: 1.2.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=6f0dde62ff0b6f57cc4c8520ac87412c
+    hash=36af9eff7b3e51ae48c06f64cde33dcd
     =====================================
 -->
 
-# yambs ([1.1.0](https://pypi.org/project/yambs/))
+# yambs ([1.2.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -150,28 +150,29 @@
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mbs -h
 
-usage: mbs [-h] [--version] [-v] [-C DIR] {gen,noop} ...
+usage: mbs [-h] [--version] [-v] [-C DIR] {gen,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
-  -h, --help         show this help message and exit
-  --version          show program's version number and exit
-  -v, --verbose      set to increase logging verbosity
-  -C DIR, --dir DIR  execute from a specific directory
+  -h, --help          show this help message and exit
+  --version           show program's version number and exit
+  -v, --verbose       set to increase logging verbosity
+  -C DIR, --dir DIR   execute from a specific directory
 
 commands:
-  {gen,noop}         set of available commands
-    gen              poll the source tree and generate any new build files
-    noop             command stub (does nothing)
+  {gen,uf2conv,noop}  set of available commands
+    gen               poll the source tree and generate any new build files
+    uf2conv           Convert to UF2 or flash directly.
+    noop              command stub (does nothing)
 
 ```
 
 ## Sub-command Options
 
 ### `gen`
 
@@ -187,14 +188,46 @@
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
 
 ```
 
+### `uf2conv`
+
+```
+$ ./venv3.11/bin/mbs uf2conv -h
+
+usage: mbs uf2conv [-h] [-b BASE] [-f FAMILY] [-o FILE] [-d DEVICE_PATH] [-l]
+                   [-c] [-D] [-w] [-C] [-i]
+                   [INPUT]
+
+positional arguments:
+  INPUT                 input file (HEX, BIN or UF2)
+
+options:
+  -h, --help            show this help message and exit
+  -b BASE, --base BASE  set base address of application for BIN format
+                        (default: 0x2000)
+  -f FAMILY, --family FAMILY
+                        specify familyID - number or name (default: 0x0)
+  -o FILE, --output FILE
+                        write output to named file; defaults to "flash.uf2" or
+                        "flash.bin" where sensible
+  -d DEVICE_PATH, --device DEVICE_PATH
+                        select a device path to flash
+  -l, --list            list connected devices
+  -c, --convert         do not flash, just convert
+  -D, --deploy          just flash, do not convert
+  -w, --wait            wait for device to flash
+  -C, --carray          convert binary file to a C array, not UF2
+  -i, --info            display header information from UF2, do not convert
+
+```
+
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `yambs`'s source.
 Generated using [pydeps](https://github.com/thebjorn/pydeps) (via
 `mk python-deps`).
```

### Comparing `yambs-1.1.0/yambs.egg-info/SOURCES.txt` & `yambs-1.2.0/yambs.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 yambs.egg-info/dependency_links.txt
 yambs.egg-info/entry_points.txt
 yambs.egg-info/requires.txt
 yambs.egg-info/top_level.txt
 yambs/commands/__init__.py
 yambs/commands/all.py
 yambs/commands/gen.py
+yambs/commands/uf2conv.py
 yambs/config/__init__.py
+yambs/data/uf2families.json
 yambs/data/schemas/Architecture.yaml
 yambs/data/schemas/Board.yaml
 yambs/data/schemas/Chip.yaml
 yambs/data/schemas/Config.yaml
 yambs/data/schemas/Toolchain.yaml
 yambs/data/templates/all.ninja.j2
 yambs/data/templates/architecture.ninja.j2
@@ -36,8 +38,10 @@
 yambs/data/templates/rules.ninja.j2
 yambs/data/templates/toolchain.ninja.j2
 yambs/generate/__init__.py
 yambs/generate/architectures.py
 yambs/generate/boards.py
 yambs/generate/chips.py
 yambs/generate/common.py
-yambs/generate/toolchains.py
+yambs/generate/ninja.py
+yambs/generate/toolchains.py
+yambs/uf2/__init__.py
```

