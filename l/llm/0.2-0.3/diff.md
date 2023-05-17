# Comparing `tmp/llm-0.2.tar.gz` & `tmp/llm-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-0.2.tar", last modified: Sat Apr  1 22:31:36 2023, max compression
+gzip compressed data, was "llm-0.3.tar", last modified: Wed May 17 21:15:02 2023, max compression
```

## Comparing `llm-0.2.tar` & `llm-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 22:31:36.611754 llm-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-01 22:31:19.000000 llm-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-01 22:31:36.611754 llm-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-01 22:31:19.000000 llm-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 22:31:36.611754 llm-0.2/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 22:31:19.000000 llm-0.2/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-01 22:31:19.000000 llm-0.2/llm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-01 22:31:19.000000 llm-0.2/llm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 22:31:36.611754 llm-0.2/llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-01 22:31:36.000000 llm-0.2/llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-01 22:31:36.000000 llm-0.2/llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 22:31:36.000000 llm-0.2/llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-01 22:31:36.000000 llm-0.2/llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-01 22:31:36.000000 llm-0.2/llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-01 22:31:36.000000 llm-0.2/llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 22:31:36.611754 llm-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-01 22:31:19.000000 llm-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 22:31:36.611754 llm-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-01 22:31:19.000000 llm-0.2/tests/test_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:15:02.527603 llm-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 21:14:47.000000 llm-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-17 21:15:02.527603 llm-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-17 21:14:47.000000 llm-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:15:02.527603 llm-0.3/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 21:14:47.000000 llm-0.3/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 21:14:47.000000 llm-0.3/llm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-17 21:14:47.000000 llm-0.3/llm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:15:02.527603 llm-0.3/llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:15:02.527603 llm-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-17 21:14:47.000000 llm-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:15:02.527603 llm-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-17 21:14:47.000000 llm-0.3/tests/test_llm.py
```

### Comparing `llm-0.2/LICENSE` & `llm-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-0.2/PKG-INFO` & `llm-0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm
-Version: 0.2
+Version: 0.3
 Summary: Access large language models from the command-line
 Home-page: https://github.com/simonw/llm
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/llm/issues
 Project-URL: CI, https://github.com/simonw/llm/actions
 Project-URL: Changelog, https://github.com/simonw/llm/releases
@@ -44,28 +44,78 @@
 
 To switch from ChatGPT 3.5 (the default) to GPT-4 if you have access:
 
     llm 'Ten names for cheesecakes' -4
 
 Pass `--model <model name>` to use a different model.
 
+You can also send a prompt to standard input, for example:
+
+    echo 'Ten names for cheesecakes' | llm
+
+### Using with a shell
+
+To generate a description of changes made to a Git repository since the last commit:
+
+    llm "Describe these changes: $(git diff)"
+
+This pattern of using `$(command)` inside a double quoted string is a useful way to quickly assemble prompts.
+
+## System prompts
+
+You can use `--system '...'` to set a system prompt.
+
+    llm 'SQL to calculate total sales by month' -s \
+      --system 'You are an exaggerated sentient cheesecake that knows SQL and talks about cheesecake a lot'
+
+This is useful for piping content to standard input, for example:
+
+    curl -s 'https://simonwillison.net/2023/May/15/per-interpreter-gils/' | \
+      llm --system 'Suggest topics for this post as a JSON array' --stream
+
+The `--code` option will set a system prompt for you that attempts to output just code without explanation, and will strip off any leading or trailing markdown code block syntax. You can use this to generate code and write it straight to a file:
+
+    llm 'Python CLI tool: reverse string passed to stdin' --code > fetch.py
+
+Be _very careful_ executing code generated by a LLM - always read it first!
+
 ## Logging to SQLite
 
 If a SQLite database file exists in `~/.llm/log.db` then the tool will log all prompts and responses to it.
 
 You can create that file by running the `init-db` command:
 
     llm init-db
 
 Now any prompts you run will be logged to that database.
 
 To avoid logging a prompt, pass `--no-log` or `-n` to the command:
 
     llm 'Ten names for cheesecakes' -n
 
+### Viewing the logs
+
+You can view the logs using the `llm logs` command:
+
+    llm logs
+
+This will output the three most recent logged items as a JSON array of objects.
+
+Add `-n 10` to see the ten most recent items:
+
+    llm logs -n 10
+
+Or `-n 0` to see everything that has ever been logged:
+
+    llm logs -n 0
+
+You can also use [Datasette](https://datasette.io/) to browse your logs like this:
+
+    datasette ~/.llm/log.db
+
 ## Help
 
 For help, run:
 
     llm --help
 
 You can also use:
```

### Comparing `llm-0.2/README.md` & `llm-0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -29,28 +29,78 @@
 
 To switch from ChatGPT 3.5 (the default) to GPT-4 if you have access:
 
     llm 'Ten names for cheesecakes' -4
 
 Pass `--model <model name>` to use a different model.
 
+You can also send a prompt to standard input, for example:
+
+    echo 'Ten names for cheesecakes' | llm
+
+### Using with a shell
+
+To generate a description of changes made to a Git repository since the last commit:
+
+    llm "Describe these changes: $(git diff)"
+
+This pattern of using `$(command)` inside a double quoted string is a useful way to quickly assemble prompts.
+
+## System prompts
+
+You can use `--system '...'` to set a system prompt.
+
+    llm 'SQL to calculate total sales by month' -s \
+      --system 'You are an exaggerated sentient cheesecake that knows SQL and talks about cheesecake a lot'
+
+This is useful for piping content to standard input, for example:
+
+    curl -s 'https://simonwillison.net/2023/May/15/per-interpreter-gils/' | \
+      llm --system 'Suggest topics for this post as a JSON array' --stream
+
+The `--code` option will set a system prompt for you that attempts to output just code without explanation, and will strip off any leading or trailing markdown code block syntax. You can use this to generate code and write it straight to a file:
+
+    llm 'Python CLI tool: reverse string passed to stdin' --code > fetch.py
+
+Be _very careful_ executing code generated by a LLM - always read it first!
+
 ## Logging to SQLite
 
 If a SQLite database file exists in `~/.llm/log.db` then the tool will log all prompts and responses to it.
 
 You can create that file by running the `init-db` command:
 
     llm init-db
 
 Now any prompts you run will be logged to that database.
 
 To avoid logging a prompt, pass `--no-log` or `-n` to the command:
 
     llm 'Ten names for cheesecakes' -n
 
+### Viewing the logs
+
+You can view the logs using the `llm logs` command:
+
+    llm logs
+
+This will output the three most recent logged items as a JSON array of objects.
+
+Add `-n 10` to see the ten most recent items:
+
+    llm logs -n 10
+
+Or `-n 0` to see everything that has ever been logged:
+
+    llm logs -n 0
+
+You can also use [Datasette](https://datasette.io/) to browse your logs like this:
+
+    datasette ~/.llm/log.db
+
 ## Help
 
 For help, run:
 
     llm --help
 
 You can also use:
```

### Comparing `llm-0.2/llm.egg-info/PKG-INFO` & `llm-0.3/llm.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm
-Version: 0.2
+Version: 0.3
 Summary: Access large language models from the command-line
 Home-page: https://github.com/simonw/llm
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/llm/issues
 Project-URL: CI, https://github.com/simonw/llm/actions
 Project-URL: Changelog, https://github.com/simonw/llm/releases
@@ -44,28 +44,78 @@
 
 To switch from ChatGPT 3.5 (the default) to GPT-4 if you have access:
 
     llm 'Ten names for cheesecakes' -4
 
 Pass `--model <model name>` to use a different model.
 
+You can also send a prompt to standard input, for example:
+
+    echo 'Ten names for cheesecakes' | llm
+
+### Using with a shell
+
+To generate a description of changes made to a Git repository since the last commit:
+
+    llm "Describe these changes: $(git diff)"
+
+This pattern of using `$(command)` inside a double quoted string is a useful way to quickly assemble prompts.
+
+## System prompts
+
+You can use `--system '...'` to set a system prompt.
+
+    llm 'SQL to calculate total sales by month' -s \
+      --system 'You are an exaggerated sentient cheesecake that knows SQL and talks about cheesecake a lot'
+
+This is useful for piping content to standard input, for example:
+
+    curl -s 'https://simonwillison.net/2023/May/15/per-interpreter-gils/' | \
+      llm --system 'Suggest topics for this post as a JSON array' --stream
+
+The `--code` option will set a system prompt for you that attempts to output just code without explanation, and will strip off any leading or trailing markdown code block syntax. You can use this to generate code and write it straight to a file:
+
+    llm 'Python CLI tool: reverse string passed to stdin' --code > fetch.py
+
+Be _very careful_ executing code generated by a LLM - always read it first!
+
 ## Logging to SQLite
 
 If a SQLite database file exists in `~/.llm/log.db` then the tool will log all prompts and responses to it.
 
 You can create that file by running the `init-db` command:
 
     llm init-db
 
 Now any prompts you run will be logged to that database.
 
 To avoid logging a prompt, pass `--no-log` or `-n` to the command:
 
     llm 'Ten names for cheesecakes' -n
 
+### Viewing the logs
+
+You can view the logs using the `llm logs` command:
+
+    llm logs
+
+This will output the three most recent logged items as a JSON array of objects.
+
+Add `-n 10` to see the ten most recent items:
+
+    llm logs -n 10
+
+Or `-n 0` to see everything that has ever been logged:
+
+    llm logs -n 0
+
+You can also use [Datasette](https://datasette.io/) to browse your logs like this:
+
+    datasette ~/.llm/log.db
+
 ## Help
 
 For help, run:
 
     llm --help
 
 You can also use:
```

### Comparing `llm-0.2/setup.py` & `llm-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.2"
+VERSION = "0.3"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

