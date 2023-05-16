# Comparing `tmp/sqapi-0.41.tar.gz` & `tmp/sqapi-0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqapi-0.41.tar", last modified: Tue May 16 04:25:47 2023, max compression
+gzip compressed data, was "sqapi-0.42.tar", last modified: Tue May 16 23:52:26 2023, max compression
```

## Comparing `sqapi-0.41.tar` & `sqapi-0.42.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-16 04:25:47.372913 sqapi-0.41/
--rw-r--r--   0 ariell     (501) staff       (20)     1061 2023-05-10 02:42:34.000000 sqapi-0.41/LICENSE.txt
--rw-r--r--   0 ariell     (501) staff       (20)    11898 2023-05-16 04:25:47.372972 sqapi-0.41/PKG-INFO
--rw-r--r--   0 ariell     (501) staff       (20)    10870 2023-05-16 04:05:23.000000 sqapi-0.41/README.md
--rw-r--r--   0 ariell     (501) staff       (20)       79 2023-05-16 04:25:47.373233 sqapi-0.41/setup.cfg
--rw-r--r--   0 ariell     (501) staff       (20)     1787 2023-05-16 04:22:00.000000 sqapi-0.41/setup.py
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-16 04:25:47.372210 sqapi-0.41/sqapi/
--rw-r--r--   0 ariell     (501) staff       (20)        0 2023-04-06 00:14:19.000000 sqapi-0.41/sqapi/__init__.py
--rw-r--r--   0 ariell     (501) staff       (20)    12728 2023-05-10 02:42:22.000000 sqapi-0.41/sqapi/annotate.py
--rw-r--r--   0 ariell     (501) staff       (20)     4202 2023-04-07 04:44:10.000000 sqapi-0.41/sqapi/api.py
--rw-r--r--   0 ariell     (501) staff       (20)     4930 2023-05-16 04:03:19.000000 sqapi-0.41/sqapi/helpers.py
--rw-r--r--   0 ariell     (501) staff       (20)     1632 2022-05-09 04:38:36.000000 sqapi-0.41/sqapi/media.py
--rw-r--r--   0 ariell     (501) staff       (20)     7454 2023-04-06 07:30:14.000000 sqapi-0.41/sqapi/request.py
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-16 04:25:47.372825 sqapi-0.41/sqapi.egg-info/
--rw-r--r--   0 ariell     (501) staff       (20)    11898 2023-05-16 04:25:47.000000 sqapi-0.41/sqapi.egg-info/PKG-INFO
--rw-r--r--   0 ariell     (501) staff       (20)      282 2023-05-16 04:25:47.000000 sqapi-0.41/sqapi.egg-info/SOURCES.txt
--rw-r--r--   0 ariell     (501) staff       (20)        1 2023-05-16 04:25:47.000000 sqapi-0.41/sqapi.egg-info/dependency_links.txt
--rw-r--r--   0 ariell     (501) staff       (20)       29 2023-05-16 04:25:47.000000 sqapi-0.41/sqapi.egg-info/requires.txt
--rw-r--r--   0 ariell     (501) staff       (20)        6 2023-05-16 04:25:47.000000 sqapi-0.41/sqapi.egg-info/top_level.txt
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-16 23:52:26.255943 sqapi-0.42/
+-rw-r--r--   0 ariell     (501) staff       (20)     1061 2023-05-10 02:42:34.000000 sqapi-0.42/LICENSE.txt
+-rw-r--r--   0 ariell     (501) staff       (20)    12022 2023-05-16 23:52:26.256019 sqapi-0.42/PKG-INFO
+-rw-r--r--   0 ariell     (501) staff       (20)    10994 2023-05-16 23:45:41.000000 sqapi-0.42/README.md
+-rw-r--r--   0 ariell     (501) staff       (20)       79 2023-05-16 23:52:26.256298 sqapi-0.42/setup.cfg
+-rw-r--r--   0 ariell     (501) staff       (20)     1787 2023-05-16 23:52:21.000000 sqapi-0.42/setup.py
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-16 23:52:26.255061 sqapi-0.42/sqapi/
+-rw-r--r--   0 ariell     (501) staff       (20)        0 2023-04-06 00:14:19.000000 sqapi-0.42/sqapi/__init__.py
+-rw-r--r--   0 ariell     (501) staff       (20)    12905 2023-05-16 23:50:48.000000 sqapi-0.42/sqapi/annotate.py
+-rw-r--r--   0 ariell     (501) staff       (20)     4202 2023-04-07 04:44:10.000000 sqapi-0.42/sqapi/api.py
+-rw-r--r--   0 ariell     (501) staff       (20)     4930 2023-05-16 04:03:19.000000 sqapi-0.42/sqapi/helpers.py
+-rw-r--r--   0 ariell     (501) staff       (20)     1632 2022-05-09 04:38:36.000000 sqapi-0.42/sqapi/media.py
+-rw-r--r--   0 ariell     (501) staff       (20)     7454 2023-04-06 07:30:14.000000 sqapi-0.42/sqapi/request.py
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-16 23:52:26.255843 sqapi-0.42/sqapi.egg-info/
+-rw-r--r--   0 ariell     (501) staff       (20)    12022 2023-05-16 23:52:26.000000 sqapi-0.42/sqapi.egg-info/PKG-INFO
+-rw-r--r--   0 ariell     (501) staff       (20)      282 2023-05-16 23:52:26.000000 sqapi-0.42/sqapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ariell     (501) staff       (20)        1 2023-05-16 23:52:26.000000 sqapi-0.42/sqapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ariell     (501) staff       (20)       29 2023-05-16 23:52:26.000000 sqapi-0.42/sqapi.egg-info/requires.txt
+-rw-r--r--   0 ariell     (501) staff       (20)        6 2023-05-16 23:52:26.000000 sqapi-0.42/sqapi.egg-info/top_level.txt
```

### Comparing `sqapi-0.41/LICENSE.txt` & `sqapi-0.42/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqapi-0.41/PKG-INFO` & `sqapi-0.42/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqapi
-Version: 0.41
+Version: 0.42
 Summary: A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 Home-page: https://bitbucket.org/ariell/pysq
 Download-URL: https://bitbucket.org/ariell/pysq/get/bede6badfc1ea09cd45b3ae3d4bc3551daa0b3e0.tar.gz
 Author: Greybits Engineering
 License: MIT
 Keywords: SQUIDLE+,API,SQ,Machine Learning
 Classifier: Development Status :: 3 - Alpha
@@ -221,15 +221,21 @@
 }
 ```
 That will attempt to map the classifier outputs `ECK`, `ASC` and `SUB` to a Label in SQ+.
 
 #### 3. Run your bot
 Now you're ready to run your classifier `RandoBot`, by simply executing this from the command line:
 ```shell
-python run_bot.py --label_map_file rando_bot_label_map.json --prob_thresh 0.5 --poll_delay -1 --email_results
+# bash
+# Install sqapi module using pip
+pip install sqapi
+# See help to show all arguments
+python run_bot.py --help
+# Run automated labeler algorithm with selected arguments
+python run_bot.py --label_map_file rando_bot_label_map.json
 ```
 
 This will prompt you for a annotation_set id and attempt to provide automated suggestions on the labels it contains 
 using random class allocations and probabilities. It will only submit suggestions with a probability > 0.5 and 
 it will run once (as defined by the `--poll_delay=-1` parameter) 
 and it will send an email to the owner the annotation_set once complete.
```

### Comparing `sqapi-0.41/README.md` & `sqapi-0.42/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,21 @@
 }
 ```
 That will attempt to map the classifier outputs `ECK`, `ASC` and `SUB` to a Label in SQ+.
 
 #### 3. Run your bot
 Now you're ready to run your classifier `RandoBot`, by simply executing this from the command line:
 ```shell
-python run_bot.py --label_map_file rando_bot_label_map.json --prob_thresh 0.5 --poll_delay -1 --email_results
+# bash
+# Install sqapi module using pip
+pip install sqapi
+# See help to show all arguments
+python run_bot.py --help
+# Run automated labeler algorithm with selected arguments
+python run_bot.py --label_map_file rando_bot_label_map.json
 ```
 
 This will prompt you for a annotation_set id and attempt to provide automated suggestions on the labels it contains 
 using random class allocations and probabilities. It will only submit suggestions with a probability > 0.5 and 
 it will run once (as defined by the `--poll_delay=-1` parameter) 
 and it will send an email to the owner the annotation_set once complete.
```

### Comparing `sqapi-0.41/setup.py` & `sqapi-0.42/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sqapi',
-    version='0.41',
+    version='0.42',
     packages=['sqapi'],
     install_requires=['requests', 'numpy', 'opencv-python'],
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.',   # Give a short description about your library
     author='Greybits Engineering',                   # Type in your name
```

### Comparing `sqapi-0.41/sqapi/annotate.py` & `sqapi-0.42/sqapi/annotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import inspect
 import json
+import os.path
 
 import time
 import traceback
 
 from sqapi.request import Get
 from sqapi.api import SQAPI, DEFAULT_HOST
 from sqapi.media import SQMediaObject
 
 DEFAULT_PROB_THRESH = 0.5
-DEFAULT_POLL_DELAY = 5
+DEFAULT_POLL_DELAY = -1
 DEFAULT_ANNOTATOR_NAME = '{user[first_name]}-{user[last_name]}'
 
 
 class Annotator:
     def __init__(self, host: str = DEFAULT_HOST, api_key: str = None, annotator_info: str = None,
                  prob_thresh: float = DEFAULT_PROB_THRESH, poll_delay: int = DEFAULT_POLL_DELAY,
                  label_map_file: str = None, verbosity: int = 2, email_results: bool = None, **kw):
         """
         Generic annotator abstract class
 
         :param annotator_info: used for the name of the annotation_set, include version info, defaults to ClassName
         :param label_map_file: path to a local file that contains the label mappings
         :param prob_thresh: probability threshold for submitted labels, only submitted if p > prob_thresh
-        :param poll_delay: the poll delay for running the loop. To run once, set poll_delay = -1
+        :param poll_delay: the poll delay for running the loop. To run once, set poll_delay = -1 (default)
         :param annotation_set_id: if supplied, will create suggested labels to the specific annotation_set with that ID
         :param affiliation_group_id: if supplied, will attempt to annotate all annotation_sets within an affiliation group
         :param user_group_id: if supplied, will attempt to annotate all annotation_sets within a user_group
         :param after_date: filter annotation_sets that were created after a specific date
         :param host: the Squidle+ instance hostname
-        :param api_key: the API key for the user on that `host`. If omitted, you'll be asked to log in.
+        :param api_key: the API key for the user on that `host`. If omitted, you'll be prompted to log in.
         :param verbosity: the verbosity of the output (0,1,2,3)
         :param email_results: flag to optionally send an email upon completion
         """
+        assert os.path.isfile(label_map_file), \
+            "label_map_file does not appear to be a valid file. A Label Mapping file is required"
+
         annotator_info = annotator_info or self.__class__.__name__
         self.sqapi = SQAPI(host=host, api_key=api_key, verbosity=verbosity)
         self.annotator_info = annotator_info.format(user=self.sqapi.current_user)  #(annotator_name or self.sqapi.cliargs.annotator_name).format(user=self.sqapi.current_user)
         self.prob_thresh = prob_thresh #or self.sqapi.cliargs.prob_thresh
         self.poll_delay = poll_delay #or self.sqapi.cliargs.poll_delay
         self.label_map_file = label_map_file #or self.sqapi.cliargs.label_map_file
         self.email_results = email_results
```

### Comparing `sqapi-0.41/sqapi/api.py` & `sqapi-0.42/sqapi/api.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.41/sqapi/helpers.py` & `sqapi-0.42/sqapi/helpers.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.41/sqapi/media.py` & `sqapi-0.42/sqapi/media.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.41/sqapi/request.py` & `sqapi-0.42/sqapi/request.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.41/sqapi.egg-info/PKG-INFO` & `sqapi-0.42/sqapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqapi
-Version: 0.41
+Version: 0.42
 Summary: A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 Home-page: https://bitbucket.org/ariell/pysq
 Download-URL: https://bitbucket.org/ariell/pysq/get/bede6badfc1ea09cd45b3ae3d4bc3551daa0b3e0.tar.gz
 Author: Greybits Engineering
 License: MIT
 Keywords: SQUIDLE+,API,SQ,Machine Learning
 Classifier: Development Status :: 3 - Alpha
@@ -221,15 +221,21 @@
 }
 ```
 That will attempt to map the classifier outputs `ECK`, `ASC` and `SUB` to a Label in SQ+.
 
 #### 3. Run your bot
 Now you're ready to run your classifier `RandoBot`, by simply executing this from the command line:
 ```shell
-python run_bot.py --label_map_file rando_bot_label_map.json --prob_thresh 0.5 --poll_delay -1 --email_results
+# bash
+# Install sqapi module using pip
+pip install sqapi
+# See help to show all arguments
+python run_bot.py --help
+# Run automated labeler algorithm with selected arguments
+python run_bot.py --label_map_file rando_bot_label_map.json
 ```
 
 This will prompt you for a annotation_set id and attempt to provide automated suggestions on the labels it contains 
 using random class allocations and probabilities. It will only submit suggestions with a probability > 0.5 and 
 it will run once (as defined by the `--poll_delay=-1` parameter) 
 and it will send an email to the owner the annotation_set once complete.
```

