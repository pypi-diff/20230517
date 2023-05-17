# Comparing `tmp/gpt-term-1.0.4.tar.gz` & `tmp/gpt-term-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-term-1.0.4.tar", last modified: Thu May 11 11:25:33 2023, max compression
+gzip compressed data, was "gpt-term-1.0.5.tar", last modified: Wed May 17 07:48:41 2023, max compression
```

## Comparing `gpt-term-1.0.4.tar` & `gpt-term-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:25:33.586511 gpt-term-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-11 11:25:22.000000 gpt-term-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 11:25:22.000000 gpt-term-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-11 11:25:33.586511 gpt-term-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-05-11 11:25:22.000000 gpt-term-1.0.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-05-11 11:25:22.000000 gpt-term-1.0.4/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:25:33.582511 gpt-term-1.0.4/gpt_term/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 11:25:22.000000 gpt-term-1.0.4/gpt_term/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-11 11:25:22.000000 gpt-term-1.0.4/gpt_term/config.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)    48444 2023-05-11 11:25:22.000000 gpt-term-1.0.4/gpt_term/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:25:33.586511 gpt-term-1.0.4/gpt_term.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-11 11:25:33.000000 gpt-term-1.0.4/gpt_term.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-11 11:25:33.000000 gpt-term-1.0.4/gpt_term.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:25:33.000000 gpt-term-1.0.4/gpt_term.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 11:25:33.000000 gpt-term-1.0.4/gpt_term.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 11:25:33.000000 gpt-term-1.0.4/gpt_term.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 11:25:33.000000 gpt-term-1.0.4/gpt_term.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:25:33.586511 gpt-term-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-11 11:25:22.000000 gpt-term-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.572279 gpt-term-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.560279 gpt-term-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.564279 gpt-term-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 07:48:26.000000 gpt-term-1.0.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-17 07:48:26.000000 gpt-term-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 07:48:26.000000 gpt-term-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-05-17 07:48:41.572279 gpt-term-1.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.564279 gpt-term-1.0.5/README.assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-05-17 07:48:26.000000 gpt-term-1.0.5/README.assets/image-20230303233352970.png
+-rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-05-17 07:48:26.000000 gpt-term-1.0.5/README.assets/small.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-05-17 07:48:26.000000 gpt-term-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-17 07:48:26.000000 gpt-term-1.0.5/README.zh-CN.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-05-17 07:48:26.000000 gpt-term-1.0.5/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.572279 gpt-term-1.0.5/gpt_term/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 07:48:26.000000 gpt-term-1.0.5/gpt_term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 07:48:26.000000 gpt-term-1.0.5/gpt_term/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 07:48:26.000000 gpt-term-1.0.5/gpt_term/config.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48444 2023-05-17 07:48:26.000000 gpt-term-1.0.5/gpt_term/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.572279 gpt-term-1.0.5/gpt_term.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-17 07:48:26.000000 gpt-term-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 07:48:26.000000 gpt-term-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:48:41.572279 gpt-term-1.0.5/setup.cfg
```

### Comparing `gpt-term-1.0.4/LICENSE` & `gpt-term-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.4/PKG-INFO` & `gpt-term-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: gpt-term
-Version: 1.0.4
-Summary: Use ChatGPT in terminal
-Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
-Author: xiaoxx970
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Chat with GPT in Terminal
 
 [![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.md)
 [![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.zh-CN.md)
 [![Platform badge](https://img.shields.io/badge/Platform-MacOS%7CWindows%7CLinux-green)]()
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
@@ -315,8 +301,8 @@
 │   └── main.py               # Main program
 ├── requirements.txt          # List of dependencies
 └── setup.py
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `gpt-term-1.0.4/README.md` & `gpt-term-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: gpt-term
+Version: 1.0.5
+Summary: Chat with GPT in Terminal
+Author: xiaoxx970, Ace-Radom
+License: MIT License
+        
+        Copyright (c) 2023 xiaoxx970
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/xiaoxx970/chatgpt-in-terminal/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Chat with GPT in Terminal
 
 [![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.md)
 [![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.zh-CN.md)
 [![Platform badge](https://img.shields.io/badge/Platform-MacOS%7CWindows%7CLinux-green)]()
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
@@ -301,8 +337,8 @@
 │   └── main.py               # Main program
 ├── requirements.txt          # List of dependencies
 └── setup.py
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `gpt-term-1.0.4/gpt_term/config.ini` & `gpt-term-1.0.5/gpt_term/config.ini`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.4/gpt_term/main.py` & `gpt-term-1.0.5/gpt_term/main.py`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.4/gpt_term.egg-info/PKG-INFO` & `gpt-term-1.0.5/gpt_term.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,39 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.0.4
-Summary: Use ChatGPT in terminal
-Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
-Author: xiaoxx970
-License: MIT
+Version: 1.0.5
+Summary: Chat with GPT in Terminal
+Author: xiaoxx970, Ace-Radom
+License: MIT License
+        
+        Copyright (c) 2023 xiaoxx970
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/xiaoxx970/chatgpt-in-terminal/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Chat with GPT in Terminal
 
 [![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.md)
```

