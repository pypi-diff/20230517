# Comparing `tmp/create-a-cli-tool-0.5.2.tar.gz` & `tmp/create-a-cli-tool-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-a-cli-tool-0.5.2.tar", last modified: Sun Oct 24 18:18:58 2021, max compression
+gzip compressed data, was "create-a-cli-tool-0.5.3.tar", last modified: Wed May 17 08:23:03 2023, max compression
```

## Comparing `create-a-cli-tool-0.5.2.tar` & `create-a-cli-tool-0.5.3.tar`

### file list

```diff
@@ -1,19 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 18:18:58.896690 create-a-cli-tool-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2021-10-24 18:18:48.000000 create-a-cli-tool-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2021-10-24 18:18:58.896690 create-a-cli-tool-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-10-24 18:18:48.000000 create-a-cli-tool-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 18:18:58.896690 create-a-cli-tool-0.5.2/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-10-24 18:18:48.000000 create-a-cli-tool-0.5.2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8290 2021-10-24 18:18:48.000000 create-a-cli-tool-0.5.2/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2021-10-24 18:18:48.000000 create-a-cli-tool-0.5.2/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-10-24 18:18:48.000000 create-a-cli-tool-0.5.2/cli/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 18:18:58.896690 create-a-cli-tool-0.5.2/cli/ext/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-10-24 18:18:48.000000 create-a-cli-tool-0.5.2/cli/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2021-10-24 18:18:48.000000 create-a-cli-tool-0.5.2/cli/ext/shard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 18:18:58.896690 create-a-cli-tool-0.5.2/create_a_cli_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2021-10-24 18:18:58.000000 create-a-cli-tool-0.5.2/create_a_cli_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-10-24 18:18:58.000000 create-a-cli-tool-0.5.2/create_a_cli_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-24 18:18:58.000000 create-a-cli-tool-0.5.2/create_a_cli_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-10-24 18:18:58.000000 create-a-cli-tool-0.5.2/create_a_cli_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-24 18:18:58.896690 create-a-cli-tool-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2021-10-24 18:18:48.000000 create-a-cli-tool-0.5.2/setup.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.718075 create-a-cli-tool-0.5.3/
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.702075 create-a-cli-tool-0.5.3/.github/
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.706075 create-a-cli-tool-0.5.3/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1283 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/.github/ISSUE_TEMPLATE/bug_report.yml
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.710075 create-a-cli-tool-0.5.3/.github/workflows/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1140 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/.github/workflows/ci.yml
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      628 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/.github/workflows/publish.yml
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       70 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/.gitignore
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      197 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/.readthedocs.yml
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1076 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/LICENSE
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       55 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/MANIFEST.in
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1993 2023-05-17 08:23:03.718075 create-a-cli-tool-0.5.3/PKG-INFO
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1241 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/README.rst
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.710075 create-a-cli-tool-0.5.3/cli/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      156 2023-05-17 08:18:21.000000 create-a-cli-tool-0.5.3/cli/__init__.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     8253 2023-05-17 08:15:30.000000 create-a-cli-tool-0.5.3/cli/cli.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2581 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/cli/commands.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      277 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/cli/errors.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.710075 create-a-cli-tool-0.5.3/cli/ext/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       21 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/cli/ext/__init__.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      918 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/cli/ext/shard.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        1 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/cli/py.typed
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.710075 create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1993 2023-05-17 08:23:03.000000 create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      741 2023-05-17 08:23:03.000000 create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        1 2023-05-17 08:23:03.000000 create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        4 2023-05-17 08:23:03.000000 create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/top_level.txt
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.714075 create-a-cli-tool-0.5.3/docs/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      634 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/Makefile
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      295 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/cli.ext.rst
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      390 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/cli.rst
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2538 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/conf.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1449 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/index.rst
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      795 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/make.bat
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       46 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/modules.rst
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        4 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/requirements.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1165 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/whats_new.rst
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.718075 create-a-cli-tool-0.5.3/examples/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      170 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/examples/arguments.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      165 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/examples/basic_cli.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      248 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/examples/group.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      189 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/examples/no_welcome_messages.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      325 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/examples/shard.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.718075 create-a-cli-tool-0.5.3/notes/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      387 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/notes/basic_cli.md
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      537 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/notes/group_cli.md
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      658 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/notes/shards.md
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       38 2023-05-17 08:23:03.718075 create-a-cli-tool-0.5.3/setup.cfg
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1394 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/setup.py
```

### Comparing `create-a-cli-tool-0.5.2/LICENSE` & `create-a-cli-tool-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.2/PKG-INFO` & `create-a-cli-tool-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: create-a-cli-tool
-Version: 0.5.2
+Version: 0.5.3
 Summary: A way to make simple python CLIs.
 Home-page: https://github.com/Sengolda/create-a-cli-tool
 Author: Sengolda
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -77,9 +76,7 @@
 
 Show your support
 ======================
 
 Give a ⭐️ if this project helped you!
 
 .. |CI_STATUS| image:: https://github.com/Sengolda/create-a-cli-tool/workflows/CI/badge.svg
-
-
```

### Comparing `create-a-cli-tool-0.5.2/README.rst` & `create-a-cli-tool-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.2/cli/cli.py` & `create-a-cli-tool-0.5.3/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,14 @@
             ):
                 cmd = self.get_command(args[0])
                 if not cmd:
                     print(self.command_not_found_message)
                     args = input(">>> ").split()
 
                 elif type(cmd) == Command:
-                    print(type(cmd))
                     try:
                         cmd._func(*args[1:])
                     except TypeError as e:
                         cmd._func()
                     args: List[str] = input(">>> ").split()  # type: ignore
 
                 elif type(cmd) == Group:
```

### Comparing `create-a-cli-tool-0.5.2/cli/commands.py` & `create-a-cli-tool-0.5.3/cli/commands.py`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.2/cli/ext/shard.py` & `create-a-cli-tool-0.5.3/cli/ext/shard.py`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.2/create_a_cli_tool.egg-info/PKG-INFO` & `create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: create-a-cli-tool
-Version: 0.5.2
+Version: 0.5.3
 Summary: A way to make simple python CLIs.
 Home-page: https://github.com/Sengolda/create-a-cli-tool
 Author: Sengolda
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -77,9 +76,7 @@
 
 Show your support
 ======================
 
 Give a ⭐️ if this project helped you!
 
 .. |CI_STATUS| image:: https://github.com/Sengolda/create-a-cli-tool/workflows/CI/badge.svg
-
-
```

### Comparing `create-a-cli-tool-0.5.2/setup.py` & `create-a-cli-tool-0.5.3/setup.py`

 * *Files identical despite different names*

