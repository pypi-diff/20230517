# Comparing `tmp/pybgpkit-0.4.3.tar.gz` & `tmp/pybgpkit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybgpkit-0.4.3.tar", last modified: Mon Apr 17 21:35:39 2023, max compression
+gzip compressed data, was "pybgpkit-0.4.4.tar", last modified: Wed May 17 18:10:11 2023, max compression
```

## Comparing `pybgpkit-0.4.3.tar` & `pybgpkit-0.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-17 21:35:39.971783 pybgpkit-0.4.3/
--rw-r--r--   0 mingwei    (501) staff       (20)     1063 2022-01-31 02:29:25.000000 pybgpkit-0.4.3/LICENSE
--rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-04-17 21:35:39.971657 pybgpkit-0.4.3/PKG-INFO
--rw-r--r--   0 mingwei    (501) staff       (20)     7389 2023-03-30 05:13:34.000000 pybgpkit-0.4.3/README.md
-drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-17 21:35:39.970776 pybgpkit-0.4.3/bgpkit/
--rw-r--r--   0 mingwei    (501) staff       (20)       98 2022-04-05 23:11:20.000000 pybgpkit-0.4.3/bgpkit/__init__.py
--rw-r--r--   0 mingwei    (501) staff       (20)     2322 2023-04-17 21:35:29.000000 pybgpkit-0.4.3/bgpkit/bgpkit_broker.py
--rw-r--r--   0 mingwei    (501) staff       (20)       34 2022-04-27 15:54:49.000000 pybgpkit-0.4.3/bgpkit/bgpkit_parser.py
--rw-r--r--   0 mingwei    (501) staff       (20)     2012 2022-04-05 22:19:49.000000 pybgpkit-0.4.3/bgpkit/bgpkit_roas.py
--rw-r--r--   0 mingwei    (501) staff       (20)     1589 2023-04-17 21:35:29.000000 pybgpkit-0.4.3/bgpkit/test_integration.py
-drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-17 21:35:39.971498 pybgpkit-0.4.3/pybgpkit.egg-info/
--rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-04-17 21:35:39.000000 pybgpkit-0.4.3/pybgpkit.egg-info/PKG-INFO
--rw-r--r--   0 mingwei    (501) staff       (20)      316 2023-04-17 21:35:39.000000 pybgpkit-0.4.3/pybgpkit.egg-info/SOURCES.txt
--rw-r--r--   0 mingwei    (501) staff       (20)        1 2023-04-17 21:35:39.000000 pybgpkit-0.4.3/pybgpkit.egg-info/dependency_links.txt
--rw-r--r--   0 mingwei    (501) staff       (20)       49 2023-04-17 21:35:39.000000 pybgpkit-0.4.3/pybgpkit.egg-info/requires.txt
--rw-r--r--   0 mingwei    (501) staff       (20)        7 2023-04-17 21:35:39.000000 pybgpkit-0.4.3/pybgpkit.egg-info/top_level.txt
--rw-r--r--   0 mingwei    (501) staff       (20)      103 2022-02-01 17:35:12.000000 pybgpkit-0.4.3/pyproject.toml
--rw-r--r--   0 mingwei    (501) staff       (20)       38 2023-04-17 21:35:39.971817 pybgpkit-0.4.3/setup.cfg
--rw-r--r--   0 mingwei    (501) staff       (20)      709 2023-04-17 21:35:29.000000 pybgpkit-0.4.3/setup.py
+drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-05-17 18:10:11.475025 pybgpkit-0.4.4/
+-rw-r--r--   0 mingwei    (501) staff       (20)     1063 2022-01-31 02:29:25.000000 pybgpkit-0.4.4/LICENSE
+-rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-05-17 18:10:11.474866 pybgpkit-0.4.4/PKG-INFO
+-rw-r--r--   0 mingwei    (501) staff       (20)     7389 2023-03-30 05:13:34.000000 pybgpkit-0.4.4/README.md
+drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-05-17 18:10:11.473635 pybgpkit-0.4.4/bgpkit/
+-rw-r--r--   0 mingwei    (501) staff       (20)       98 2022-04-05 23:11:20.000000 pybgpkit-0.4.4/bgpkit/__init__.py
+-rw-r--r--   0 mingwei    (501) staff       (20)     2319 2023-04-20 18:33:35.000000 pybgpkit-0.4.4/bgpkit/bgpkit_broker.py
+-rw-r--r--   0 mingwei    (501) staff       (20)       34 2022-04-27 15:54:49.000000 pybgpkit-0.4.4/bgpkit/bgpkit_parser.py
+-rw-r--r--   0 mingwei    (501) staff       (20)     2012 2022-04-05 22:19:49.000000 pybgpkit-0.4.4/bgpkit/bgpkit_roas.py
+-rw-r--r--   0 mingwei    (501) staff       (20)     1588 2023-04-20 18:51:22.000000 pybgpkit-0.4.4/bgpkit/test_integration.py
+drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-05-17 18:10:11.474627 pybgpkit-0.4.4/pybgpkit.egg-info/
+-rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-05-17 18:10:11.000000 pybgpkit-0.4.4/pybgpkit.egg-info/PKG-INFO
+-rw-r--r--   0 mingwei    (501) staff       (20)      316 2023-05-17 18:10:11.000000 pybgpkit-0.4.4/pybgpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)        1 2023-05-17 18:10:11.000000 pybgpkit-0.4.4/pybgpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)       49 2023-05-17 18:10:11.000000 pybgpkit-0.4.4/pybgpkit.egg-info/requires.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)        7 2023-05-17 18:10:11.000000 pybgpkit-0.4.4/pybgpkit.egg-info/top_level.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)      103 2022-02-01 17:35:12.000000 pybgpkit-0.4.4/pyproject.toml
+-rw-r--r--   0 mingwei    (501) staff       (20)       38 2023-05-17 18:10:11.475073 pybgpkit-0.4.4/setup.cfg
+-rw-r--r--   0 mingwei    (501) staff       (20)      709 2023-05-17 18:04:56.000000 pybgpkit-0.4.4/setup.py
```

### Comparing `pybgpkit-0.4.3/LICENSE` & `pybgpkit-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.3/PKG-INFO` & `pybgpkit-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybgpkit
-Version: 0.4.3
+Version: 0.4.4
 Summary: BGPKIT tools Python bindings
 Home-page: https://github.com/bgpkit/pybgpkit
 Author: Mingwei Zhang
 Author-email: mingwei@bgpkit.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pybgpkit-0.4.3/README.md` & `pybgpkit-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.3/bgpkit/bgpkit_broker.py` & `pybgpkit-0.4.4/bgpkit/bgpkit_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     url: str
     rough_size: int
     exact_size: int
 
 
 class Broker:
 
-    def __init__(self, api_url: str = "https://api.broker.bgpkit.com/v2", page_size: int = 100, verify=True):
+    def __init__(self, api_url: str = "https://api.bgpkit.com/broker", page_size: int = 100, verify=True):
         self.base_url = api_url.strip()
         self.page_size = int(page_size)
         self.verify = verify
         if not verify:
             # if a user disable SSL verification on-purpose, do not warn the user
             urllib3.disable_warnings()
```

### Comparing `pybgpkit-0.4.3/bgpkit/bgpkit_roas.py` & `pybgpkit-0.4.4/bgpkit/bgpkit_roas.py`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.3/pybgpkit.egg-info/PKG-INFO` & `pybgpkit-0.4.4/pybgpkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybgpkit
-Version: 0.4.3
+Version: 0.4.4
 Summary: BGPKIT tools Python bindings
 Home-page: https://github.com/bgpkit/pybgpkit
 Author: Mingwei Zhang
 Author-email: mingwei@bgpkit.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pybgpkit-0.4.3/setup.py` & `pybgpkit-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='pybgpkit',
-    version='0.4.3',
+    version='0.4.4',
     description='BGPKIT tools Python bindings',
     url='https://github.com/bgpkit/pybgpkit',
     author='Mingwei Zhang',
     author_email='mingwei@bgpkit.com',
     packages=setuptools.find_packages(),
     include_package_data=True,
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # available on pip
         'dataclasses_json',
-        'pybgpkit-parser==0.4.2',
+        'pybgpkit-parser==0.4.3',
         'requests',
     ]
 )
```

