# Comparing `tmp/psytricks-2.1.0.tar.gz` & `tmp/psytricks-2.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psytricks-2.1.0.tar", max compression
+gzip compressed data, was "psytricks-2.1.1a0.tar", max compression
```

## Comparing `psytricks-2.1.0.tar` & `psytricks-2.1.1a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.0/LICENSE
--rw-r--r--   0        0        0     6526 2023-05-10 20:14:28.925038 psytricks-2.1.0/README.md
--rw-r--r--   0        0        0     1045 2023-05-12 19:33:05.240400 psytricks-2.1.0/pyproject.toml
--rw-r--r--   0        0        0       93 2023-05-12 19:33:05.240400 psytricks-2.1.0/src/psytricks/__init__.py
--rw-r--r--   0        0        0     6146 2023-05-12 19:33:05.244397 psytricks-2.1.0/src/psytricks/__ps1__/psytricks-lib.ps1
--rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/__ps1__/psytricks-wrapper.ps1
--rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/__ps1__/restricks-server.example.xml
--rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.0/src/psytricks/__ps1__/restricks-server.ps1
--rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
--rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
--rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetSessions.json
--rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.0/src/psytricks/cli.py
--rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.0/src/psytricks/decoder.py
--rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/literals.py
--rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.0/src/psytricks/mappings.py
--rw-r--r--   0        0        0    23720 2023-05-12 19:24:30.404582 psytricks-2.1.0/src/psytricks/wrapper.py
--rw-r--r--   0        0        0     7336 1970-01-01 00:00:00.000000 psytricks-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.1a0/LICENSE
+-rw-r--r--   0        0        0     6526 2023-05-10 20:14:28.925038 psytricks-2.1.1a0/README.md
+-rw-r--r--   0        0        0     1116 2023-05-17 09:41:35.868353 psytricks-2.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-05-17 09:41:35.868353 psytricks-2.1.1a0/src/psytricks/__init__.py
+-rw-r--r--   0        0        0     6150 2023-05-17 09:41:35.868353 psytricks-2.1.1a0/src/psytricks/__ps1__/psytricks-lib.ps1
+-rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/__ps1__/psytricks-wrapper.ps1
+-rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/__ps1__/restricks-server.example.xml
+-rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.1a0/src/psytricks/__ps1__/restricks-server.ps1
+-rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
+-rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
+-rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetSessions.json
+-rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.1a0/src/psytricks/cli.py
+-rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.1a0/src/psytricks/decoder.py
+-rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/literals.py
+-rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.1a0/src/psytricks/mappings.py
+-rw-r--r--   0        0        0    23720 2023-05-12 19:24:30.404582 psytricks-2.1.1a0/src/psytricks/wrapper.py
+-rw-r--r--   0        0        0     7465 1970-01-01 00:00:00.000000 psytricks-2.1.1a0/PKG-INFO
```

### Comparing `psytricks-2.1.0/LICENSE` & `psytricks-2.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/README.md` & `psytricks-2.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/pyproject.toml` & `psytricks-2.1.1a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>"]
 description = "PowerShell Python Citrix Tricks."
+documentation = "https://imcf.one/apidocs/psytricks/psytricks.html"
 license = "GPL-3.0-or-later"
 name = "psytricks"
 readme = "README.md"
-version = "2.1.0"
+version = "2.1.1-a.0"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/imcf/psytricks/blob/main/CHANGELOG.md"
 "Organisation Homepage" = "https://imcf.one/"
 "Twitter" = "https://twitter.com/imcf_basel"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 loguru = "^0.6.0"
-python = "^3.10"
+python = "^3.9"
 requests = "^2.30.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 ipython = "^8.13.2"
 pylint = "^2.16.2"
```

### Comparing `psytricks-2.1.0/src/psytricks/__ps1__/psytricks-lib.ps1` & `psytricks-2.1.1a0/src/psytricks/__ps1__/psytricks-lib.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <#
 
 Collection of functions and other definitions to be sourced by other scripts.
 
 #>
 
 # the version variable will be filled by poetry at build time:
-$Version = "2.1.0"
+$Version = "2.1.1-a.0"
 
 
 #region properties-selectors
 
 $MachineProperties = @(
     "AgentVersion",
     "AssociatedUserUPNs",
```

### Comparing `psytricks-2.1.0/src/psytricks/__ps1__/psytricks-wrapper.ps1` & `psytricks-2.1.1a0/src/psytricks/__ps1__/psytricks-wrapper.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/src/psytricks/__ps1__/restricks-server.example.xml` & `psytricks-2.1.1a0/src/psytricks/__ps1__/restricks-server.example.xml`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/src/psytricks/__ps1__/restricks-server.ps1` & `psytricks-2.1.1a0/src/psytricks/__ps1__/restricks-server.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json` & `psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json` & `psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetSessions.json` & `psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetSessions.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/src/psytricks/cli.py` & `psytricks-2.1.1a0/src/psytricks/cli.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/src/psytricks/decoder.py` & `psytricks-2.1.1a0/src/psytricks/decoder.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/src/psytricks/literals.py` & `psytricks-2.1.1a0/src/psytricks/literals.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/src/psytricks/mappings.py` & `psytricks-2.1.1a0/src/psytricks/mappings.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/src/psytricks/wrapper.py` & `psytricks-2.1.1a0/src/psytricks/wrapper.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.0/PKG-INFO` & `psytricks-2.1.1a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: psytricks
-Version: 2.1.0
+Version: 2.1.1a0
 Summary: PowerShell Python Citrix Tricks.
 License: GPL-3.0-or-later
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Project-URL: Changelog, https://github.com/imcf/psytricks/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://imcf.one/apidocs/psytricks/psytricks.html
 Project-URL: Organisation Homepage, https://imcf.one/
 Project-URL: Twitter, https://twitter.com/imcf_basel
 Description-Content-Type: text/markdown
 
 # PSytricks
 
 ![PyPI](https://img.shields.io/pypi/v/psytricks)
```

