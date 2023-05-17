# Comparing `tmp/malbench-0.4.0.tar.gz` & `tmp/malbench-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malbench-0.4.0.tar", max compression
+gzip compressed data, was "malbench-0.4.1.tar", max compression
```

## Comparing `malbench-0.4.0.tar` & `malbench-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.4.0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.4.0/malbench/__init__.py
--rw-r--r--   0        0        0     3000 2023-05-02 19:13:53.949742 malbench-0.4.0/malbench/__main__.py
--rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.4.0/malbench/args.py
--rw-r--r--   0        0        0     6780 2023-05-15 02:55:05.437319 malbench-0.4.0/malbench/celebrations.py
--rw-r--r--   0        0        0      545 2023-05-03 20:58:37.976822 malbench-0.4.0/malbench/data/banner.txt
--rw-r--r--   0        0        0      567 2023-05-03 20:58:37.977821 malbench-0.4.0/malbench/data/disclaimer.txt
--rw-r--r--   0        0        0        5 2023-05-16 03:00:05.762021 malbench-0.4.0/malbench/data/version.txt
--rw-r--r--   0        0        0     5085 2023-05-16 02:57:51.049649 malbench-0.4.0/malbench/malware.py
--rw-r--r--   0        0        0    12072 2023-05-16 02:57:51.050649 malbench-0.4.0/malbench/message.py
--rw-r--r--   0        0        0      327 2023-05-08 02:07:22.949742 malbench-0.4.0/malbench/platform.py
--rw-r--r--   0        0        0      432 2023-05-03 20:58:37.979815 malbench-0.4.0/malbench/version.py
--rw-r--r--   0        0        0     1183 2023-05-16 02:59:58.088322 malbench-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6232 2023-05-08 02:07:22.941260 malbench-0.4.0/README.md
--rw-r--r--   0        0        0     6917 1970-01-01 00:00:00.000000 malbench-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.4.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.4.1/malbench/__init__.py
+-rw-r--r--   0        0        0     3000 2023-05-02 19:13:53.949742 malbench-0.4.1/malbench/__main__.py
+-rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.4.1/malbench/args.py
+-rw-r--r--   0        0        0     6780 2023-05-15 02:55:05.437319 malbench-0.4.1/malbench/celebrations.py
+-rw-r--r--   0        0        0      545 2023-05-03 20:58:37.976822 malbench-0.4.1/malbench/data/banner.txt
+-rw-r--r--   0        0        0      567 2023-05-03 20:58:37.977821 malbench-0.4.1/malbench/data/disclaimer.txt
+-rw-r--r--   0        0        0        5 2023-05-17 03:21:57.295031 malbench-0.4.1/malbench/data/version.txt
+-rw-r--r--   0        0        0     5085 2023-05-16 02:57:51.049649 malbench-0.4.1/malbench/malware.py
+-rw-r--r--   0        0        0    12072 2023-05-16 02:57:51.050649 malbench-0.4.1/malbench/message.py
+-rw-r--r--   0        0        0      327 2023-05-08 02:07:22.949742 malbench-0.4.1/malbench/platform.py
+-rw-r--r--   0        0        0      432 2023-05-03 20:58:37.979815 malbench-0.4.1/malbench/version.py
+-rw-r--r--   0        0        0     1183 2023-05-17 03:22:11.384081 malbench-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6232 2023-05-08 02:07:22.941260 malbench-0.4.1/README.md
+-rw-r--r--   0        0        0     6963 1970-01-01 00:00:00.000000 malbench-0.4.1/PKG-INFO
```

### Comparing `malbench-0.4.0/LICENSE` & `malbench-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `malbench-0.4.0/malbench/__main__.py` & `malbench-0.4.1/malbench/__main__.py`

 * *Files identical despite different names*

### Comparing `malbench-0.4.0/malbench/args.py` & `malbench-0.4.1/malbench/args.py`

 * *Files identical despite different names*

### Comparing `malbench-0.4.0/malbench/celebrations.py` & `malbench-0.4.1/malbench/celebrations.py`

 * *Files identical despite different names*

### Comparing `malbench-0.4.0/malbench/data/banner.txt` & `malbench-0.4.1/malbench/data/banner.txt`

 * *Files identical despite different names*

### Comparing `malbench-0.4.0/malbench/data/disclaimer.txt` & `malbench-0.4.1/malbench/data/disclaimer.txt`

 * *Files identical despite different names*

### Comparing `malbench-0.4.0/malbench/malware.py` & `malbench-0.4.1/malbench/malware.py`

 * *Files identical despite different names*

### Comparing `malbench-0.4.0/malbench/message.py` & `malbench-0.4.1/malbench/message.py`

 * *Files identical despite different names*

### Comparing `malbench-0.4.0/pyproject.toml` & `malbench-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "malbench"
-version = "0.4.0"
+version = "0.4.1"
 description = "A tool used to benchmark antivirus solutions against real-world malware samples."
 repository = "https://github.com/youkergav/Malbench"
 authors = ["Gavin Youker <youkergav@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 colorama = "^0.4.6"
 toml = "^0.10.2"
+python-dotenv = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.7.0"
 autopep8 = "^2.0.2"
 pdoc = "^13.1.0"
 coverage = "^7.2.3"
 mypy = "^1.2.0"
 types-toml = "^0.10.8.6"
 types-setuptools = "^67.7.0.0"
 types-colorama = "^0.4.15.11"
-python-dotenv = "^1.0.0"
 poethepoet = "^0.20.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `malbench-0.4.0/README.md` & `malbench-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `malbench-0.4.0/PKG-INFO` & `malbench-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: malbench
-Version: 0.4.0
+Version: 0.4.1
 Summary: A tool used to benchmark antivirus solutions against real-world malware samples.
 Home-page: https://github.com/youkergav/Malbench
 License: GPL-3.0-only
 Author: Gavin Youker
 Author-email: youkergav@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/youkergav/Malbench
 Description-Content-Type: text/markdown
 
 # Malbench
 Malbench is a command-line tool for testing and evaluating the effectiveness of malware detection tools (such as antivirus solutions). It does this by running a set of malware samples, and checking if the malware is flagged by the detection tool we are evaluating. Malbench is built to be modular and configurable, so it can be customized to meet the specific needs of different users and environments.
 ![Malbench Terminal Demo](https://i.imgur.com/oGQNU8i.gif)
```

