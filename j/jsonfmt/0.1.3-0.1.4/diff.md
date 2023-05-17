# Comparing `tmp/jsonfmt-0.1.3.tar.gz` & `tmp/jsonfmt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonfmt-0.1.3.tar", last modified: Thu May 11 16:15:58 2023, max compression
+gzip compressed data, was "jsonfmt-0.1.4.tar", last modified: Wed May 17 03:16:09 2023, max compression
```

## Comparing `jsonfmt-0.1.3.tar` & `jsonfmt-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:15:58.444173 jsonfmt-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 16:15:42.000000 jsonfmt-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-11 16:15:58.444173 jsonfmt-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-11 16:15:42.000000 jsonfmt-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:15:58.444173 jsonfmt-0.1.3/jsonfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     4964 2023-05-11 16:15:42.000000 jsonfmt-0.1.3/jsonfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-11 16:15:42.000000 jsonfmt-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:15:58.444173 jsonfmt-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:16:09.595387 jsonfmt-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 03:15:53.000000 jsonfmt-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-17 03:16:09.595387 jsonfmt-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-17 03:15:53.000000 jsonfmt-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:16:09.591387 jsonfmt-0.1.4/jsonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5020 2023-05-17 03:15:53.000000 jsonfmt-0.1.4/jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-17 03:15:53.000000 jsonfmt-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:16:09.595387 jsonfmt-0.1.4/setup.cfg
```

### Comparing `jsonfmt-0.1.3/LICENSE` & `jsonfmt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.1.3/PKG-INFO` & `jsonfmt-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-Metadata-Version: 2.1
-Name: jsonfmt
-Version: 0.1.3
-Summary: A simple tool for formatting JSON object.
-Author-email: Seamile <lanhuermao@gmail.com>
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JSON Formator
 
-![PyPI - Downloads](https://img.shields.io/pypi/dm/jsonfmt?label=Install&color=green)
-![PyPI](https://img.shields.io/pypi/v/jsonfmt?color=9cf)
-![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?branch=main&label=build&logo=python)
-
+![GitHub Build Status](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?label=Build&logo=python&logoColor=white)
+[![Downloads](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Installs)](https://pepy.tech/project/jsonfmt)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
-**jsonfmt** is a JSON object formatting tool.
+**jsonfmt** is a CLI tool for pretty printing or compressing JSON objects.
 
 It has the following features:
 
 1. Print the JSON object with **hightlight** and **pretty format** from files or stdin.
-2. Compress the JSON object into a single line without spaces.
+2. Minimize the JSON object to a single line.
 3. Output part of a large JSON object via jsonpath.
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
 ```
@@ -39,153 +23,158 @@
 
 ```shell
 $ jsonfmt [-h] [-c] [-O] [-p JSONPATH] [json_files ...]
 ```
 
 - positional arguments:
 
-     - `json_files`   the json files that will be processed
+    - `json_files`   the json files that will be processed
 
 - options:
 
-     - `-h, --help`: show this help message and exit.
-     - `-c`: compression the JSON object in the files or stdin.
-     - `-e`: escape non-ASCII characters.
-     - `-i INDENT`: number of spaces to use for indentation. (default: 4)
-     - `-O`: overwrite to the json file.
-     - `-p JSONPATH`: output part of JSON object via jsonpath.
-     - `-v`: show the version.
+    - `-h, --help`: show this help message and exit.
+    - `-c`: compression the JSON object in the files or stdin.
+    - `-e`: escape non-ASCII characters.
+    - `-i INDENT`: number of spaces to use for indentation. (default: 4)
+    - `-O`: overwrite to the json file.
+    - `-p JSONPATH`: output part of JSON object via jsonpath.
+    - `-v`: show the version.
 
 
 ## Example
 
 In the file example.json there is a compressed JSON object.
 
 1. Pretty print from json file.
 
-     ```shell
-     $ jsonfmt example.json
-     ```
-
-     Output:
-     ```json
-     {
-          "age": 23,
-          "gender": "纯爷们",
-          "history": [
-               {
-                    "action": "eat",
-                    "date": "2021-03-02",
-                    "items": [
-                         {
-                              "calorie": 294.9,
-                              "name": "hamburger"
-                         },
-                         {
-                              "calorie": 266,
-                              "name": "pizza"
-                         }
-                    ]
-               },
-               {
-                    "action": "drink",
-                    "date": "2022-11-01",
-                    "items": [
-                         {
-                              "calorie": 37.5,
-                              "name": "Coca Cola"
-                         },
-                         {
-                              "calorie": 54.5,
-                              "name": "juice"
-                         }
-                    ]
-               },
-               {
-                    "action": "sport",
-                    "date": "2023-04-27",
-                    "items": [
-                         {
-                              "calorie": -375,
-                              "name": "running"
-                         },
-                         {
-                              "calorie": -350,
-                              "name": "swimming"
-                         }
-                    ]
-               }
-          ],
-          "name": "Bob"
-     }
-    ```
-
-     Of course, you can use the `-O` parameter to overwrite the file with the result:
-
-     ```shell
-     $ jsonfmt -O example.json
-     ```
+    ```shell
+    $ jsonfmt example.json
+    ```
 
+    Output:
+    ```json
+    {
+        "age": 23,
+        "gender": "纯爷们",
+        "history": [
+            {
+                "action": "eat",
+                "date": "2021-03-02",
+                "items": [
+                    {
+                        "calorie": 294.9,
+                        "name": "hamburger"
+                    },
+                    {
+                        "calorie": 266,
+                        "name": "pizza"
+                    }
+                ]
+            },
+            {
+                "action": "drink",
+                "date": "2022-11-01",
+                "items": [
+                    {
+                        "calorie": 37.5,
+                        "name": "Coca Cola"
+                    },
+                    {
+                        "calorie": 54.5,
+                        "name": "juice"
+                    }
+                ]
+            },
+            {
+                "action": "sport",
+                "date": "2023-04-27",
+                "items": [
+                    {
+                        "calorie": -375,
+                        "name": "running"
+                    },
+                    {
+                        "calorie": -350,
+                        "name": "swimming"
+                    }
+                ]
+            }
+        ],
+        "name": "Bob"
+    }
+    ```
 
 2. Format a JSON object from stdin via pipeline.
 
-     ```shell
-     $ curl https://raw.githubusercontent.com/seamile/jsonfmt/main/example.json | jsonfmt
-     ```
-
-     Output: Ditto.
-
-
-3. Compress the JSON object.
-
-     ```shell
-     $ echo '{
-          "name": "alex",
-          "age": 21,
-          "items": ["pen", "ruler", "phone"]
-     }' | jsonfmt -c
-     ```
-
-     Output:
-     ```json
-     {"age":21,"items":["pen","ruler","phone"],"name":"alex"}
-     ```
+    ```shell
+    $ curl https://raw.githubusercontent.com/seamile/jsonfmt/main/example.json | jsonfmt
+    ```
+
+    Output: Ditto.
+
+
+3. Minimize the JSON object.
+
+    ```shell
+    $ echo '{
+        "name": "alex",
+        "age": 21,
+        "items": ["pen", "ruler", "phone"]
+    }' | jsonfmt -c
+    ```
+
+    Output:
+    ```json
+    {"age":21,"items":["pen","ruler","phone"],"name":"alex"}
+    ```
 
 4. Use jsonpath to match part of a JSON object.
 
-     **jsonfmt** uses a simplified jsonpath syntax.
+    **jsonfmt** uses a simplified jsonpath syntax.
+
+    - It matches JSON objects starting from the root node.
+    - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
+
+        ```shell
+        $ jsonfmt -p 'history/0/date' example.json
+        ```
+
+        Output:
+        ```json
+        "2021-03-02"
+        ```
+
+    - If you want to match all items in a list, just use `*` to match.
+
+        ```shell
+        $ jsonfmt -p 'history/*/items/*/name' example.json
+        ```
+
+        Output:
+        ```json
+        [
+            [
+                "hamburger",
+                "pizza"
+            ],
+            [
+                "Coca Cola",
+                "juice"
+            ],
+            [
+                "running",
+                "swimming"
+            ]
+        ]
+        ```
 
-     - It matches JSON objects starting from the root node.
-     - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
+4. You can use the `-O` parameter to overwrite the file with the result.
 
-          ```shell
-          $ jsonfmt -p 'history/0/date' example.json
-          ```
-
-          Output:
-          ```json
-          "2021-03-02"
-          ```
-
-     - If you want to match all items in a list, just use `*` to match.
-
-          ```shell
-          $ jsonfmt -p 'history/*/items/*/name' example.json
-          ```
-
-          Output:
-          ```json
-          [
-               [
-                    "hamburger",
-                    "pizza"
-               ],
-               [
-                    "Coca Cola",
-                    "juice"
-               ],
-               [
-                    "running",
-                    "swimming"
-               ]
-          ]
-          ```
+    ```shell
+    $ jsonfmt -O example.json
+    ```
+
+5. To output the result to a new file, you can use the redirect symbol `>`.
+
+    ```shell
+    $ jsonfmt example.json > formatted.json
+    ```
```

### Comparing `jsonfmt-0.1.3/jsonfmt.egg-info/PKG-INFO` & `jsonfmt-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple tool for formatting JSON object.
 Author-email: Seamile <lanhuermao@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSON Formator
 
-![PyPI - Downloads](https://img.shields.io/pypi/dm/jsonfmt?label=Install&color=green)
-![PyPI](https://img.shields.io/pypi/v/jsonfmt?color=9cf)
-![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?branch=main&label=build&logo=python)
+![GitHub Build Status](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?label=Build&logo=python&logoColor=white)
+[![Downloads](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Installs)](https://pepy.tech/project/jsonfmt)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
-
-**jsonfmt** is a JSON object formatting tool.
+**jsonfmt** is a CLI tool for pretty printing or compressing JSON objects.
 
 It has the following features:
 
 1. Print the JSON object with **hightlight** and **pretty format** from files or stdin.
-2. Compress the JSON object into a single line without spaces.
+2. Minimize the JSON object to a single line.
 3. Output part of a large JSON object via jsonpath.
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
 ```
@@ -39,153 +39,158 @@
 
 ```shell
 $ jsonfmt [-h] [-c] [-O] [-p JSONPATH] [json_files ...]
 ```
 
 - positional arguments:
 
-     - `json_files`   the json files that will be processed
+    - `json_files`   the json files that will be processed
 
 - options:
 
-     - `-h, --help`: show this help message and exit.
-     - `-c`: compression the JSON object in the files or stdin.
-     - `-e`: escape non-ASCII characters.
-     - `-i INDENT`: number of spaces to use for indentation. (default: 4)
-     - `-O`: overwrite to the json file.
-     - `-p JSONPATH`: output part of JSON object via jsonpath.
-     - `-v`: show the version.
+    - `-h, --help`: show this help message and exit.
+    - `-c`: compression the JSON object in the files or stdin.
+    - `-e`: escape non-ASCII characters.
+    - `-i INDENT`: number of spaces to use for indentation. (default: 4)
+    - `-O`: overwrite to the json file.
+    - `-p JSONPATH`: output part of JSON object via jsonpath.
+    - `-v`: show the version.
 
 
 ## Example
 
 In the file example.json there is a compressed JSON object.
 
 1. Pretty print from json file.
 
-     ```shell
-     $ jsonfmt example.json
-     ```
-
-     Output:
-     ```json
-     {
-          "age": 23,
-          "gender": "纯爷们",
-          "history": [
-               {
-                    "action": "eat",
-                    "date": "2021-03-02",
-                    "items": [
-                         {
-                              "calorie": 294.9,
-                              "name": "hamburger"
-                         },
-                         {
-                              "calorie": 266,
-                              "name": "pizza"
-                         }
-                    ]
-               },
-               {
-                    "action": "drink",
-                    "date": "2022-11-01",
-                    "items": [
-                         {
-                              "calorie": 37.5,
-                              "name": "Coca Cola"
-                         },
-                         {
-                              "calorie": 54.5,
-                              "name": "juice"
-                         }
-                    ]
-               },
-               {
-                    "action": "sport",
-                    "date": "2023-04-27",
-                    "items": [
-                         {
-                              "calorie": -375,
-                              "name": "running"
-                         },
-                         {
-                              "calorie": -350,
-                              "name": "swimming"
-                         }
-                    ]
-               }
-          ],
-          "name": "Bob"
-     }
-    ```
-
-     Of course, you can use the `-O` parameter to overwrite the file with the result:
-
-     ```shell
-     $ jsonfmt -O example.json
-     ```
+    ```shell
+    $ jsonfmt example.json
+    ```
 
+    Output:
+    ```json
+    {
+        "age": 23,
+        "gender": "纯爷们",
+        "history": [
+            {
+                "action": "eat",
+                "date": "2021-03-02",
+                "items": [
+                    {
+                        "calorie": 294.9,
+                        "name": "hamburger"
+                    },
+                    {
+                        "calorie": 266,
+                        "name": "pizza"
+                    }
+                ]
+            },
+            {
+                "action": "drink",
+                "date": "2022-11-01",
+                "items": [
+                    {
+                        "calorie": 37.5,
+                        "name": "Coca Cola"
+                    },
+                    {
+                        "calorie": 54.5,
+                        "name": "juice"
+                    }
+                ]
+            },
+            {
+                "action": "sport",
+                "date": "2023-04-27",
+                "items": [
+                    {
+                        "calorie": -375,
+                        "name": "running"
+                    },
+                    {
+                        "calorie": -350,
+                        "name": "swimming"
+                    }
+                ]
+            }
+        ],
+        "name": "Bob"
+    }
+    ```
 
 2. Format a JSON object from stdin via pipeline.
 
-     ```shell
-     $ curl https://raw.githubusercontent.com/seamile/jsonfmt/main/example.json | jsonfmt
-     ```
-
-     Output: Ditto.
-
-
-3. Compress the JSON object.
-
-     ```shell
-     $ echo '{
-          "name": "alex",
-          "age": 21,
-          "items": ["pen", "ruler", "phone"]
-     }' | jsonfmt -c
-     ```
-
-     Output:
-     ```json
-     {"age":21,"items":["pen","ruler","phone"],"name":"alex"}
-     ```
+    ```shell
+    $ curl https://raw.githubusercontent.com/seamile/jsonfmt/main/example.json | jsonfmt
+    ```
+
+    Output: Ditto.
+
+
+3. Minimize the JSON object.
+
+    ```shell
+    $ echo '{
+        "name": "alex",
+        "age": 21,
+        "items": ["pen", "ruler", "phone"]
+    }' | jsonfmt -c
+    ```
+
+    Output:
+    ```json
+    {"age":21,"items":["pen","ruler","phone"],"name":"alex"}
+    ```
 
 4. Use jsonpath to match part of a JSON object.
 
-     **jsonfmt** uses a simplified jsonpath syntax.
+    **jsonfmt** uses a simplified jsonpath syntax.
+
+    - It matches JSON objects starting from the root node.
+    - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
+
+        ```shell
+        $ jsonfmt -p 'history/0/date' example.json
+        ```
+
+        Output:
+        ```json
+        "2021-03-02"
+        ```
+
+    - If you want to match all items in a list, just use `*` to match.
+
+        ```shell
+        $ jsonfmt -p 'history/*/items/*/name' example.json
+        ```
+
+        Output:
+        ```json
+        [
+            [
+                "hamburger",
+                "pizza"
+            ],
+            [
+                "Coca Cola",
+                "juice"
+            ],
+            [
+                "running",
+                "swimming"
+            ]
+        ]
+        ```
 
-     - It matches JSON objects starting from the root node.
-     - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
+4. You can use the `-O` parameter to overwrite the file with the result.
 
-          ```shell
-          $ jsonfmt -p 'history/0/date' example.json
-          ```
-
-          Output:
-          ```json
-          "2021-03-02"
-          ```
-
-     - If you want to match all items in a list, just use `*` to match.
-
-          ```shell
-          $ jsonfmt -p 'history/*/items/*/name' example.json
-          ```
-
-          Output:
-          ```json
-          [
-               [
-                    "hamburger",
-                    "pizza"
-               ],
-               [
-                    "Coca Cola",
-                    "juice"
-               ],
-               [
-                    "running",
-                    "swimming"
-               ]
-          ]
-          ```
+    ```shell
+    $ jsonfmt -O example.json
+    ```
+
+5. To output the result to a new file, you can use the redirect symbol `>`.
+
+    ```shell
+    $ jsonfmt example.json > formatted.json
+    ```
```

### Comparing `jsonfmt-0.1.3/jsonfmt.py` & `jsonfmt-0.1.4/jsonfmt.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,32 @@
 #!/usr/bin/env python
 '''JSON Format Tool'''
 
 import json
 from sys import stdin, stdout, stderr
 from argparse import ArgumentParser
-from typing import Any, List, IO, Union
+from typing import Any, List, IO, Optional, Sequence, Union
 
 from pygments import highlight
 from pygments.lexers import JsonLexer
 from pygments.formatters import TerminalFormatter
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 
 def print_err(msg: str):
-    print(f'\033[0;31m{msg}\033[0m', file=stderr)
+    print(f'\033[1;91mjsonfmt:\033[0m \033[0;91m{msg}\033[0m', file=stderr)
 
 
 class JSONPathError(Exception):
     pass
 
 
-def output(json_obj: Any, compression: bool, escape: bool, indent: int,
-           output_fp: IO = stdout):
-    '''output formated json to file or stdout'''
-    if output_fp.fileno() > 2:
-        output_fp.seek(0)
-        output_fp.truncate()
-    if compression:
-        json.dump(json_obj, output_fp, ensure_ascii=escape,
-                  sort_keys=True, separators=(',', ':'))
-    else:
-        json_text = json.dumps(json_obj, ensure_ascii=escape,
-                               sort_keys=True, indent=indent)
-        # highlight the json code when outputint to TTY divice
-        if output_fp.isatty():
-            json_text = highlight(json_text, JsonLexer(), TerminalFormatter())
-        output_fp.write(json_text)
-
-    # append a blank line at the end of `fp``
-    output_fp.write('\n')
+class JSONParseError(Exception):
+    pass
 
 
 def parse_jsonpath(jsonpath: str) -> List[Union[str, int]]:
     '''parse the jsonpath into a list of pathname components'''
     jsonpath = jsonpath.strip().strip('/')
     if not jsonpath:
         return []
@@ -51,38 +34,72 @@
         components = jsonpath.split('/')
         for i, c in enumerate(components):
             if c.isdecimal():
                 components[i] = int(c)  # type: ignore
         return components  # type: ignore
 
 
-def get_element_by_components(json_obj: Any,
-                              jpath_components: List[Union[str, int]]) -> Any:
+def match_element(py_obj: Any, jpath_components: List[Union[str, int]]) -> Any:
     for i, c in enumerate(jpath_components):
-        if c == '*' and isinstance(json_obj, list):
-            return [get_element_by_components(sub_obj, jpath_components[i + 1:])
-                    for sub_obj in json_obj]
+        if c == '*' and isinstance(py_obj, list):
+            return [match_element(sub_obj, jpath_components[i + 1:])
+                    for sub_obj in py_obj]
         else:
             try:
-                json_obj = json_obj[c]
+                py_obj = py_obj[c]
             except (IndexError, KeyError, TypeError):
-                raise JSONPathError(f'Invalid path node `{c}`')
+                raise JSONPathError(f'invalid path node `{c}`')
 
-    return json_obj
+    return py_obj
 
 
-def jsonpath_match(json_obj: Any, jsonpath: str) -> Any:
+def read_json_to_py(json_fp: IO, jsonpath: str) -> Any:
+    '''read json obj from IO and match sub-element by jsonpath'''
+    # parse json object to python object
+    try:
+        py_obj = json.load(json_fp)
+    except (json.JSONDecodeError, UnicodeDecodeError) as e:
+        print_err(f"no json object in `{json_fp.name}`")
+        raise JSONParseError from e
+
+    # parse jsonpath and match the sub-element of py_obj
     jpath_components = parse_jsonpath(jsonpath)
-    if not jpath_components:
-        return json_obj
+    try:
+        return match_element(py_obj, jpath_components)
+    except JSONPathError as e:
+        print_err(f'{e}')
+        raise JSONParseError from e
+
+
+def output(py_obj: Any, compact: bool, escape: bool, indent: int,
+           output_fp: IO = stdout):
+    '''output formated json to file or stdout'''
+    if output_fp.fileno() > 2:
+        output_fp.seek(0)
+        output_fp.truncate()
+
+    if compact:
+        json_text = json.dumps(py_obj, ensure_ascii=escape, sort_keys=True,
+                               separators=(',', ':'))
     else:
-        return get_element_by_components(json_obj, jpath_components)
+        json_text = json.dumps(py_obj, ensure_ascii=escape, sort_keys=True,
+                               indent=indent)
 
+    # highlight the json code when output to TTY divice
+    if output_fp.isatty():
+        json_text = highlight(json_text, JsonLexer(), TerminalFormatter())
 
-def parse_cmdline_args():
+    # append a blank line at the end of `fp``
+    if json_text[-1] != '\n':
+        json_text += '\n'
+
+    output_fp.write(json_text)
+
+
+def parse_cmdline_args(args: Optional[Sequence[str]] = None):
     parser = ArgumentParser('jsonfmt')
     parser.add_argument('-c', dest='compression', action='store_true',
                         help='compression the json object in the files or stdin')
     parser.add_argument('-e', dest='escape', action='store_true',
                         help='escape non-ASCII characters')
     parser.add_argument('-i', dest='indent', type=int, default=4,
                         help='number of spaces to use for indentation (default: %(default)s)')
@@ -90,50 +107,40 @@
                         help='overwrite the formated json object into the json file')
     parser.add_argument('-p', dest='jsonpath', type=str, default='',
                         help='output part of json object via jsonpath')
     parser.add_argument(dest='json_files', nargs='*',
                         help='the json files that will be processed')
     parser.add_argument('-v', dest='version', action='version', version=__version__,
                         help="show the version")
-    return parser.parse_args()
+    return parser.parse_args(args)
 
 
 def main():
     args = parse_cmdline_args()
 
     if args.json_files:
-        # get json from files
         for j_file in args.json_files:
             try:
-                with open(j_file, 'r+') as fp:
+                # read json from file
+                with open(j_file, 'r+') as json_fp:
                     try:
-                        j_obj = json.load(fp)
-                        matched_obj = jsonpath_match(j_obj, args.jsonpath)
-                    except json.decoder.JSONDecodeError:
-                        print_err(f"no json object found from file `{j_file}`")
-                        continue
-                    except JSONPathError as e:
-                        print_err(f'{e}')
-                        continue
-                    output_fp = fp if args.overwrite else stdout
-                    output(matched_obj, args.compression, args.escape,
-                           args.indent, output_fp)
-
+                        py_obj = read_json_to_py(json_fp, args.jsonpath)
+                    except JSONParseError:
+                        exit(1)
+                    else:
+                        output_fp = json_fp if args.overwrite else stdout
+                        output(py_obj, args.compression, args.escape,
+                               args.indent, output_fp)
             except FileNotFoundError:
-                print_err(f'No such file `{j_file}`')
+                print_err(f'no such file `{j_file}`')
     else:
-        # get json from stdin
+        # read json from stdin
         try:
-            j_obj = json.load(stdin)
-            matched_obj = jsonpath_match(j_obj, args.jsonpath)
-        except json.decoder.JSONDecodeError:
-            print_err("no json object found from `stdin`")
+            py_obj = read_json_to_py(stdin, args.jsonpath)
+        except JSONParseError:
             exit(1)
-        except JSONPathError as e:
-            print_err(f'{e}')
-            exit(2)
         else:
-            output(matched_obj, args.compression, args.escape, args.indent)
+            output(py_obj, args.compression, args.escape, args.indent, stdout)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jsonfmt-0.1.3/pyproject.toml` & `jsonfmt-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsonfmt"
 dynamic = ["version"]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {text = "MIT"}
 description = "A simple tool for formatting JSON object."
 readme = "README.md"
 authors = [{name = "Seamile", email = "lanhuermao@gmail.com"}]
 dependencies = ["Pygments >=2.13.0"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

