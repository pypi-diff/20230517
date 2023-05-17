# Comparing `tmp/hcai-nova-utils-0.2.0.tar.gz` & `tmp/hcai-nova-utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-utils-0.2.0.tar", last modified: Wed Apr  5 12:41:41 2023, max compression
+gzip compressed data, was "hcai-nova-utils-0.3.0.tar", last modified: Wed May 17 07:37:47 2023, max compression
```

## Comparing `hcai-nova-utils-0.2.0.tar` & `hcai-nova-utils-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 12:41:41.887085 hcai-nova-utils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-05 12:41:41.887085 hcai-nova-utils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 12:41:41.887085 hcai-nova-utils-0.2.0/hcai_nova_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-05 12:41:41.000000 hcai-nova-utils-0.2.0/hcai_nova_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-04-05 12:41:41.000000 hcai-nova-utils-0.2.0/hcai_nova_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-05 12:41:41.000000 hcai-nova-utils-0.2.0/hcai_nova_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-05 12:41:41.000000 hcai-nova-utils-0.2.0/hcai_nova_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-05 12:41:41.000000 hcai-nova-utils-0.2.0/hcai_nova_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 12:41:41.887085 hcai-nova-utils-0.2.0/nova_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 12:41:41.887085 hcai-nova-utils-0.2.0/nova_utils/db_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/db_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/db_utils/nova_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 12:41:41.887085 hcai-nova-utils-0.2.0/nova_utils/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      616 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/interfaces/dataset_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/interfaces/server_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 12:41:41.887085 hcai-nova-utils-0.2.0/nova_utils/ssi_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/ssi_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6664 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/ssi_utils/ssi_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/ssi_utils/ssi_data_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/ssi_utils/ssi_sample_list_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/ssi_utils/ssi_stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8240 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/nova_utils/ssi_utils/ssi_xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-05 12:41:41.887085 hcai-nova-utils-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-04-05 12:41:33.000000 hcai-nova-utils-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.086952 hcai-nova-utils-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-17 07:37:47.086952 hcai-nova-utils-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.082952 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-17 07:37:46.000000 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-05-17 07:37:47.000000 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 07:37:46.000000 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-17 07:37:46.000000 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-17 07:37:46.000000 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.082952 hcai-nova-utils-0.3.0/nova_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.082952 hcai-nova-utils-0.3.0/nova_utils/db_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/db_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/db_utils/nova_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.082952 hcai-nova-utils-0.3.0/nova_utils/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/interfaces/dataset_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6821 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/interfaces/server_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.082952 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6664 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_sample_list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8508 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 07:37:47.086952 hcai-nova-utils-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/setup.py
```

### Comparing `hcai-nova-utils-0.2.0/PKG-INFO` & `hcai-nova-utils-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcai-nova-utils-0.2.0/hcai_nova_utils.egg-info/PKG-INFO` & `hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcai-nova-utils-0.2.0/hcai_nova_utils.egg-info/SOURCES.txt` & `hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.2.0/nova_utils/interfaces/dataset_iterable.py` & `hcai-nova-utils-0.3.0/nova_utils/interfaces/dataset_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.2.0/nova_utils/interfaces/server_module.py` & `hcai-nova-utils-0.3.0/nova_utils/interfaces/server_module.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from nova_utils.interfaces.dataset_iterable import DatasetIterable
 from nova_utils.db_utils.nova_types import DataTypes
 import numpy as np
 
 REQUIREMENTS = []
 
-
+'''
 class Dataset(DatasetIterable):
     def __int__(self, *args, data: dict, **kwargs):
         super().__init__(*args, **kwargs)
         self.counter = 0
         self.data = data
 
     def __iter__(self):
@@ -18,40 +18,42 @@
     def __next__(self):
         data = self.data["counter"]
         self.counter += 1
         return data
 
     def get_output_info(self):
         return ""
-
+'''
 
 class Processor(ABC):
     """
     Base class of a data processor. This interface builds the foundation for all data processing classes.
     """
 
     # List of dependencies that need to be installed when the script is loaded
     DEPENDENCIES = []
 
     # Flag to indicate whether the processed input belongs to one role or to multiple roles
-    SINGLE_ROLE_INPUT = True
-
-
+    # SINGLE_ROLE_INPUT = True
 
     def __init__(self, logger, request_form=None):
         self.logger = logger
         self.request_form = request_form
         self.options = {"input_1": None}
         self.model = None
         self.data = None
         self.output = None
 
     @abstractmethod
-    def preprocess_sample(self, sample):
-        """Preprocess data to convert between nova-server dataset iterator item to the raw model input as required in forward_sample."""
+    def preprocess_sample(self, sample: dict ):
+        """Preprocess data to convert between nova-server dataset iterator item to the raw model input as required in process_sample.
+
+        Args:
+            sample (dict):
+        """
         return sample
 
     @abstractmethod
     def process_sample(self, sample):
         """Applying processing steps (e.g. feature extraction, data prediction etc... ) to the provided data."""
         return sample
 
@@ -107,15 +109,59 @@
     """
 
     def __init__(self, logger, request_form=None):
         super().__init__(logger, request_form)
 
     @abstractmethod
     def to_anno(self, data):
-        """Converts the output of process_data to the correct annotation format to upload them to the database"""
+        """Converts the output of process_data to the correct annotation format to upload them to the database.
+        !THE OUTPUT FORMAT OF THIS FUNCTION IS NOT YET FULLY DEFINED AND WILL CHANGE IN FUTURE RELEASES!
+
+        Args:
+            data (object): Data output of process_data function
+
+        Returns:
+            dict: A dictionary containing the predictions of the model in the correct annotation format.
+
+
+        Example:
+
+            Discrete annotation:
+                ::
+
+                    {
+                        '0.0_1.0' : {
+                            'speaker_1.audio' : {'id': '1', 'conf': 0.73}
+                            'speaker_2.audio' : {'id': '0', conf: 1.0}
+                        }
+                        ...
+                        'values': [],
+                        'confidences': []
+                    }
+
+            Continuous annotation:
+                ...
+            Free annotation:
+                ::
+
+                    {
+                        '0.0_1.0' : {
+                            'speaker_1.audio' : {'name': 'Hello', 'conf': 0.73}
+                            'speaker_2.audio' : {'name': '', conf: 1.0}
+                        }
+                        '1.0_2.0' : {
+                            'speaker_1.audio' : {'name': 'My Name', 'conf': 0.85}}
+                            'speaker_2.audio' : {'name': '', conf: 1.0}
+                        }
+                        ...
+                        'values': [],
+                        'confidences': []
+                    }
+
+        """
         raise NotImplemented
 
 
 class Extractor(Processor):
     """
     Base class of a feature extractor. Implement this interface in your own class to build a feature extractor.
     """
@@ -128,22 +174,26 @@
 
     def __init__(self, logger, request_form=None):
         super().__init__(logger, request_form)
 
     @abstractmethod
     def to_stream(self, data: object) -> dict:
         """Converts the return value from process_data() to data stream chunk that can be processed by nova-server.
-        The output should have the following format:
 
         Args:
-            data (object):
+            data (object): The data as returned by the process_data function of the Processor class
 
-        Returns: A dictionary mapping a stream identifier (usually composed using the role, signal, extracted feature name and sliding window parameters) to a tuple containing a chunk of the data as well as additional information.
-        Each tuple has the form ( type (nova_types.DataTypes), sample_rate (int), data_chunk (numpy.ndarray) ). The shape of the data chunk should in the form of (n_frames, n_features)
+
+        Returns:
+            dict: A dictionary mapping a stream identifier (usually composed using the role, signal, extracted feature name and sliding window parameters) to a tuple containing a chunk of the data as well as additional information.
+        Each tuple has the form ( type (nova_types.DataTypes), sample_rate (double), data_chunk (numpy.ndarray) ). The shape of the data chunk should in the form of (n_frames, n_features)
         An arbitrary number of streams maybe returned.
-        An example for a returned dictionary may look like this:
-        {
-        speaker_1.audio.mfcc[10ms,10ms,10ms] : ( DataTypes.AUDIO, 100, [[0.0, 0.0, ... 0.0], [0.0, 0.0, ... 0.0] ... [0.0, 0.0, ... 0.0]] )
-        speaker_2.audio.mfcc[10ms,10ms,10ms] : ( DataTypes.AUDIO, 100, [[0.0, 0.0, ... 0.0], [0.0, 0.0, ... 0.0] ... [0.0, 0.0, ... 0.0]] )
-        }
+
+        Example:
+            ::
+
+                {
+                    'speaker_1.audio.mfcc[10ms,10ms,10ms]' : ( DataTypes.AUDIO, 100, [[0.0, 0.0, ... 0.0], [0.0, 0.0, ... 0.0] ... [0.0, 0.0, ... 0.0]] ),
+                    'speaker_2.audio.mfcc[10ms,10ms,10ms]' : ( DataTypes.AUDIO, 100, [[0.0, 0.0, ... 0.0], [0.0, 0.0, ... 0.0] ... [0.0, 0.0, ... 0.0]] )
+                }
         """
-        raise NotImplemented
+        raise NotImplemented
```

### Comparing `hcai-nova-utils-0.2.0/nova_utils/ssi_utils/ssi_anno_utils.py` & `hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.2.0/nova_utils/ssi_utils/ssi_data_types.py` & `hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_data_types.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.2.0/nova_utils/ssi_utils/ssi_sample_list_utils.py` & `hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_sample_list_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.2.0/nova_utils/ssi_utils/ssi_stream_utils.py` & `hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_stream_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.2.0/nova_utils/ssi_utils/ssi_xml_utils.py` & `hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_xml_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import xml.etree.ElementTree as ET
 from pathlib import Path
 
 
 class Trainer:
     def __init__(
-        self,
-        model_script_path: str = "",
-        model_option_path: str = "",
-        model_option_string: str = "",
-        model_weights_path: str = "",
-        model_stream: int = 0,
-        model_create: str = "PythonModel",
-        users: list = None,
-        classes: list = None,
-        streams: list = None,
-        register: list = None,
-        info_trained: bool = False,
-        meta_right_ctx: int = 0,
-        meta_left_ctx: int = 0,
-        meta_balance: str = "none",
-        meta_backend: str = "nova-server",
-        ssi_v="5",
-        xml_version="1.0",
+            self,
+            model_script_path: str = "",
+            model_option_path: str = "",
+            model_option_string: str = "",
+            model_weights_path: str = "",
+            model_stream: int = 0,
+            model_create: str = "PythonModel",
+            model_multirole_input = False,
+            users: list = None,
+            classes: list = None,
+            streams: list = None,
+            register: list = None,
+            info_trained: bool = False,
+            meta_right_ctx: int = 0,
+            meta_left_ctx: int = 0,
+            meta_balance: str = "none",
+            meta_backend: str = "nova-server",
+            ssi_v="5",
+            xml_version="1.0",
     ):
 
         self.model_script_path = model_script_path
         self.model_option_path = model_option_path
         self.model_optstr = model_option_string
         self.model_weights_path = model_weights_path
         self.model_stream = model_stream
@@ -37,14 +38,15 @@
         self.info_trained = info_trained
         self.meta_right_ctx = meta_right_ctx
         self.meta_left_ctx = meta_left_ctx
         self.meta_balance = meta_balance
         self.meta_backend = meta_backend
         self.ssi_v = ssi_v
         self.xml_version = xml_version
+        self.model_multi_role_input = model_multirole_input
 
     def load_from_file(self, fp):
         root = ET.parse(Path(fp))
         info = root.find("info")
         meta = root.find("meta")
         register = root.find("register")
         streams = root.find("streams")
@@ -74,14 +76,15 @@
         if model is not None:
             self.model_stream = model.get("stream", default="0")
             self.model_create = model.get("create", default="PythonModel")
             self.model_option_path = model.get("option", default="")
             self.model_script_path = model.get("script", default="")
             self.model_weights_path = model.get("path", default="")
             self.model_optstr = model.get("optstr", default="")
+            self.model_multi_role_input = bool(model.get("multi_role_input", default=False))
 
     def write_to_file(self, fp):
         root = ET.Element("trainer")
         ET.SubElement(root, "info", trained=str(self.info_trained))
         ET.SubElement(
             root,
             "meta",
```

### Comparing `hcai-nova-utils-0.2.0/setup.py` & `hcai-nova-utils-0.3.0/setup.py`

 * *Files identical despite different names*

