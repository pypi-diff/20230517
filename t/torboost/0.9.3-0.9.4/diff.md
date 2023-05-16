# Comparing `tmp/torboost-0.9.3.tar.gz` & `tmp/torboost-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torboost-0.9.3.tar", last modified: Tue May 31 12:09:00 2022, max compression
+gzip compressed data, was "torboost-0.9.4.tar", last modified: Tue May 16 22:05:21 2023, max compression
```

## Comparing `torboost-0.9.3.tar` & `torboost-0.9.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2022-05-31 12:09:00.933689 torboost-0.9.3/
--rw-r--r--   0 robert     (501) staff       (20)     1065 2022-05-27 00:38:30.000000 torboost-0.9.3/LICENSE
--rw-r--r--   0 robert     (501) staff       (20)     3326 2022-05-31 12:09:00.933332 torboost-0.9.3/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)     2786 2022-05-31 08:58:11.000000 torboost-0.9.3/README.md
--rw-r--r--   0 robert     (501) staff       (20)       38 2022-05-31 12:09:00.933784 torboost-0.9.3/setup.cfg
--rw-r--r--   0 robert     (501) staff       (20)     1366 2022-05-31 08:42:06.000000 torboost-0.9.3/setup.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2022-05-31 12:09:00.929542 torboost-0.9.3/torboost/
--rw-r--r--   0 robert     (501) staff       (20)        0 2022-05-27 11:12:38.000000 torboost-0.9.3/torboost/__init__.py
--rw-r--r--   0 robert     (501) staff       (20)     9072 2022-05-31 08:42:11.000000 torboost-0.9.3/torboost/torboost.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2022-05-31 12:09:00.932826 torboost-0.9.3/torboost.egg-info/
--rw-r--r--   0 robert     (501) staff       (20)     3326 2022-05-31 12:09:00.000000 torboost-0.9.3/torboost.egg-info/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)      262 2022-05-31 12:09:00.000000 torboost-0.9.3/torboost.egg-info/SOURCES.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2022-05-31 12:09:00.000000 torboost-0.9.3/torboost.egg-info/dependency_links.txt
--rw-r--r--   0 robert     (501) staff       (20)       60 2022-05-31 12:09:00.000000 torboost-0.9.3/torboost.egg-info/entry_points.txt
--rw-r--r--   0 robert     (501) staff       (20)       36 2022-05-31 12:09:00.000000 torboost-0.9.3/torboost.egg-info/requires.txt
--rw-r--r--   0 robert     (501) staff       (20)        9 2022-05-31 12:09:00.000000 torboost-0.9.3/torboost.egg-info/top_level.txt
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-05-16 22:05:21.762137 torboost-0.9.4/
+-rw-r--r--   0 robert     (501) staff       (20)     1065 2022-05-27 00:38:30.000000 torboost-0.9.4/LICENSE
+-rw-r--r--   0 robert     (501) staff       (20)     3325 2023-05-16 22:05:21.761757 torboost-0.9.4/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)     2805 2023-05-16 22:01:50.000000 torboost-0.9.4/README.md
+-rw-r--r--   0 robert     (501) staff       (20)       38 2023-05-16 22:05:21.762249 torboost-0.9.4/setup.cfg
+-rw-r--r--   0 robert     (501) staff       (20)     1366 2023-05-16 22:02:43.000000 torboost-0.9.4/setup.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-05-16 22:05:21.759062 torboost-0.9.4/torboost/
+-rw-r--r--   0 robert     (501) staff       (20)        0 2022-05-27 11:12:38.000000 torboost-0.9.4/torboost/__init__.py
+-rw-r--r--   0 robert     (501) staff       (20)     9310 2023-05-16 22:02:43.000000 torboost-0.9.4/torboost/torboost.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-05-16 22:05:21.761263 torboost-0.9.4/torboost.egg-info/
+-rw-r--r--   0 robert     (501) staff       (20)     3325 2023-05-16 22:05:21.000000 torboost-0.9.4/torboost.egg-info/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)      262 2023-05-16 22:05:21.000000 torboost-0.9.4/torboost.egg-info/SOURCES.txt
+-rw-r--r--   0 robert     (501) staff       (20)        1 2023-05-16 22:05:21.000000 torboost-0.9.4/torboost.egg-info/dependency_links.txt
+-rw-r--r--   0 robert     (501) staff       (20)       59 2023-05-16 22:05:21.000000 torboost-0.9.4/torboost.egg-info/entry_points.txt
+-rw-r--r--   0 robert     (501) staff       (20)       36 2023-05-16 22:05:21.000000 torboost-0.9.4/torboost.egg-info/requires.txt
+-rw-r--r--   0 robert     (501) staff       (20)        9 2023-05-16 22:05:21.000000 torboost-0.9.4/torboost.egg-info/top_level.txt
```

### Comparing `torboost-0.9.3/LICENSE` & `torboost-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torboost-0.9.3/PKG-INFO` & `torboost-0.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: torboost
-Version: 0.9.3
+Version: 0.9.4
 Summary: Download utility for Tor
 Home-page: https://github.com/tasooshi/torboost/
 Author: tasooshi
 Author-email: tasooshi@pm.me
 License: MIT License
 Keywords: Tor,onion,download
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,14 +26,15 @@
 ## Warning
 
 **This way of utilizing Tor network reduces your anonymity!**
 
 ## Requirements
 
 * `tor`
+* GNU/Linux only!
 
 ## Installation
 
 `$ pip install torboost`
 
 ## Usage
 
@@ -88,8 +88,7 @@
                         User-Agent header (default: python-requests/2.27.1)
   --config CONFIG       Custom Tor configuration file (JSON)
   --debug               Enable debugging mode (verbose output) (default: INFO)
   --combine             Combine all chunks downloaded so far
   --reset               Remove data directories and rebuild circuits
   -v, --version         show program's version number and exit
 ```
-
```

### Comparing `torboost-0.9.3/README.md` & `torboost-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ## Warning
 
 **This way of utilizing Tor network reduces your anonymity!**
 
 ## Requirements
 
 * `tor`
+* GNU/Linux only!
 
 ## Installation
 
 `$ pip install torboost`
 
 ## Usage
 
@@ -69,8 +70,8 @@
   --user-agent USER_AGENT
                         User-Agent header (default: python-requests/2.27.1)
   --config CONFIG       Custom Tor configuration file (JSON)
   --debug               Enable debugging mode (verbose output) (default: INFO)
   --combine             Combine all chunks downloaded so far
   --reset               Remove data directories and rebuild circuits
   -v, --version         show program's version number and exit
-```
+```
```

### Comparing `torboost-0.9.3/setup.py` & `torboost-0.9.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 #######################################################################
 # License: MIT License                                                #
 # Homepage: https://github.com/tasooshi/torboost/                     #
-# Version: 0.9.3                                                      #
+# Version: 0.9.4                                                      #
 #######################################################################
 
 import setuptools
 
 
 with open('README.md') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name='torboost',
-    version='0.9.3',
+    version='0.9.4',
     author='tasooshi',
     author_email='tasooshi@pm.me',
     description='Download utility for Tor',
     license='MIT License',
     keywords=[
         'Tor',
         'onion',
```

### Comparing `torboost-0.9.3/torboost/torboost.py` & `torboost-0.9.4/torboost/torboost.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from urllib import parse
 import argparse
 import hashlib
 import json
 import logging
 import pathlib
 import queue
-import requests
 import shutil
-import stem.process
 import threading
 import urllib3.exceptions
 
+import requests
+import stem.process
+from stem.util import system
+
 
-__version__ = '0.9.3'
+__version__ = '0.9.4'
 
 
 logging.basicConfig(format='%(name)s %(levelname)s [%(asctime)s] %(message)s', level=logging.INFO)
 logger = logging.getLogger('torboost')
 
 
 class TorBoost:
@@ -41,15 +43,15 @@
 
     def print_bootstrap(self, line):
         if 'Bootstrapped ' in line:
             logger.info(line)
 
     def request(self, headers, socks_port):
         headers.update({
-            'User-Agent': self.args.user_agent    
+            'User-Agent': self.args.user_agent
         })
         proxies = {
             'http': f'socks5h://localhost:{socks_port}',
             'https': f'socks5h://localhost:{socks_port}',
         }
         return requests.get(self.args.url, headers=headers, proxies=proxies, stream=True)
 
@@ -106,17 +108,17 @@
         }
         config.update(self.config)
         logger.info(f'Bootstrapping Tor process {proc_no}')
         logger.debug(f'with config: {config}')
         try:
             proc = stem.process.launch_tor_with_config(
                 take_ownership=True,
-                config = config,
+                config=config,
                 timeout=self.args.timeout,
-                init_msg_handler = self.print_bootstrap,
+                init_msg_handler=self.print_bootstrap,
             )
         except OSError:
             logger.error(f'Could not start Tor process, conflicting ports?')
             exit()
         self.procs[proc_no] = config
         self.procs[proc_no]['process'] = proc
 
@@ -187,14 +189,17 @@
     parser.add_argument('--config', help='Custom Tor configuration file (JSON)')
     parser.add_argument('--debug', action='store_const', dest='loglevel', const=logging.DEBUG, default=logging.INFO, help='Enable debugging mode (verbose output)')
     parser.add_argument('--combine', action='store_true', help='Combine all chunks downloaded so far')
     parser.add_argument('--reset', action='store_true', help='Remove data directories and rebuild circuits')
     parser.add_argument('-v', '--version', action='version', version=__version__)
     args = parser.parse_args()
     logger.setLevel(args.loglevel)
+    if system.is_windows():
+        logger.info(f'Custom `timeout` is not supported on Windows, restoring default value: {stem.process.DEFAULT_INIT_TIMEOUT}')
+        args.timeout = stem.process.DEFAULT_INIT_TIMEOUT
     boost = TorBoost(args)
     if args.combine:
         boost.combine()
         exit()
     if args.reset:
         boost.reset()
         exit()
```

### Comparing `torboost-0.9.3/torboost.egg-info/PKG-INFO` & `torboost-0.9.4/torboost.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: torboost
-Version: 0.9.3
+Version: 0.9.4
 Summary: Download utility for Tor
 Home-page: https://github.com/tasooshi/torboost/
 Author: tasooshi
 Author-email: tasooshi@pm.me
 License: MIT License
 Keywords: Tor,onion,download
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,14 +26,15 @@
 ## Warning
 
 **This way of utilizing Tor network reduces your anonymity!**
 
 ## Requirements
 
 * `tor`
+* GNU/Linux only!
 
 ## Installation
 
 `$ pip install torboost`
 
 ## Usage
 
@@ -88,8 +88,7 @@
                         User-Agent header (default: python-requests/2.27.1)
   --config CONFIG       Custom Tor configuration file (JSON)
   --debug               Enable debugging mode (verbose output) (default: INFO)
   --combine             Combine all chunks downloaded so far
   --reset               Remove data directories and rebuild circuits
   -v, --version         show program's version number and exit
 ```
-
```

