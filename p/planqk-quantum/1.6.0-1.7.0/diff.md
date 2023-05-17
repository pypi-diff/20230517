# Comparing `tmp/planqk-quantum-1.6.0.tar.gz` & `tmp/planqk-quantum-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-1.6.0.tar", last modified: Wed Mar 22 16:31:58 2023, max compression
+gzip compressed data, was "planqk-quantum-1.7.0.tar", last modified: Wed May 17 13:27:47 2023, max compression
```

## Comparing `planqk-quantum-1.6.0.tar` & `planqk-quantum-1.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 16:31:58.945018 planqk-quantum-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-03-22 16:31:58.945018 planqk-quantum-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 16:31:58.941018 planqk-quantum-1.6.0/planqk/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3069 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3545 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 16:31:58.945018 planqk-quantum-1.6.0/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5848 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 16:31:58.941018 planqk-quantum-1.6.0/planqk/qiskit/providers/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 16:31:58.945018 planqk-quantum-1.6.0/planqk/qiskit/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/qiskit/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6170 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/qiskit/providers/azure/planqk_azure_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     8698 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/qiskit/providers/azure/planqk_azure_job.py
--rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/qiskit/providers/azure/planqk_azure_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     4906 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/planqk/qiskit/providers/azure/planqk_target_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 16:31:58.945018 planqk-quantum-1.6.0/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-03-22 16:31:58.000000 planqk-quantum-1.6.0/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-03-22 16:31:58.000000 planqk-quantum-1.6.0/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-22 16:31:58.000000 planqk-quantum-1.6.0/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-03-22 16:31:58.000000 planqk-quantum-1.6.0/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-22 16:31:58.000000 planqk-quantum-1.6.0/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-22 16:31:58.945018 planqk-quantum-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-03-22 16:31:47.000000 planqk-quantum-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/planqk/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3069 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3679 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5848 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.820867 planqk-quantum-1.7.0/planqk/qiskit/providers/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6170 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8698 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4906 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_target_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-05-17 13:27:47.000000 planqk-quantum-1.7.0/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-05-17 13:27:47.000000 planqk-quantum-1.7.0/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:27:47.000000 planqk-quantum-1.7.0/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-17 13:27:47.000000 planqk-quantum-1.7.0/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-17 13:27:47.000000 planqk-quantum-1.7.0/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/setup.py
```

### Comparing `planqk-quantum-1.6.0/LICENSE` & `planqk-quantum-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.6.0/PKG-INFO` & `planqk-quantum-1.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python library for the PlanQK Quantum Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: StoneOne AG
 Author-email: info@stoneone.de
 License: apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,17 +12,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python library for the PlanQK Platform
 
 [![PyPI version](https://badge.fury.io/py/planqk-quantum.svg)](https://badge.fury.io/py/planqk-quantum)
 
-PlanQK Quantum Platform library is an SDK for developing quantum circuits with [Qiskit](https://pypi.org/project/qiskit) 
-that can be performed and metered as jobs on quantum devices provided by the [PlanQK Platform](https://docs.platform.planqk.de/).  
- 
+The `planqk-quantum` library is a SDK for developing quantum circuits using [Qiskit](https://pypi.org/project/qiskit) to be run on quantum devices provided by the [PlanQK Platform](https://docs.platform.planqk.de).
+
+## Getting Started
+
+Check out the following guides on how to get started with PlanQK:
+
+- [Tutorial on how to create a PlanQK Service using the `planqk-quantum` library](https://docs.platform.planqk.de/tutorials/tutorial-qiskit.html)
+- [General guide on how to create and deploy PlanQK Services](https://docs.platform.planqk.de/docs/service-platform/managed-services.html)
+
 ## Installation
 
 The package is released on PyPI and can be installed via `pip`:
 
 ```bash
 pip install planqk-quantum
 ```
```

### Comparing `planqk-quantum-1.6.0/README.md` & `planqk-quantum-1.7.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Python library for the PlanQK Platform
 
 [![PyPI version](https://badge.fury.io/py/planqk-quantum.svg)](https://badge.fury.io/py/planqk-quantum)
 
-PlanQK Quantum Platform library is an SDK for developing quantum circuits with [Qiskit](https://pypi.org/project/qiskit) 
-that can be performed and metered as jobs on quantum devices provided by the [PlanQK Platform](https://docs.platform.planqk.de/).  
- 
+The `planqk-quantum` library is a SDK for developing quantum circuits using [Qiskit](https://pypi.org/project/qiskit) to be run on quantum devices provided by the [PlanQK Platform](https://docs.platform.planqk.de).
+
+## Getting Started
+
+Check out the following guides on how to get started with PlanQK:
+
+- [Tutorial on how to create a PlanQK Service using the `planqk-quantum` library](https://docs.platform.planqk.de/tutorials/tutorial-qiskit.html)
+- [General guide on how to create and deploy PlanQK Services](https://docs.platform.planqk.de/docs/service-platform/managed-services.html)
+
 ## Installation
 
 The package is released on PyPI and can be installed via `pip`:
 
 ```bash
 pip install planqk-quantum
 ```
```

### Comparing `planqk-quantum-1.6.0/planqk/client.py` & `planqk-quantum-1.7.0/planqk/client.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.6.0/planqk/credentials.py` & `planqk-quantum-1.7.0/planqk/credentials.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import logging
 import os
+import platform
 from abc import ABC, abstractmethod
 from json import JSONDecodeError
 
 from planqk.exceptions import CredentialUnavailableError, PlanqkClientError
 
 _TOKEN_ENV_VARIABLE = 'PLANQK_QUANTUM_ACCESS_TOKEN'
-_TOKEN_FILE_ENV_VARIABLE = 'PLANQK_QUANTUM_ACCESS_TOKEN_FILE'
 
 logger = logging.getLogger(__name__)
 
 
 class CredentialProvider(ABC):
 
     @abstractmethod
@@ -27,57 +27,60 @@
             access_token = os.environ.get("SERVICE_EXECUTION_TOKEN")
             if not access_token:
                 message = f'Environment variable {_TOKEN_ENV_VARIABLE} or SERVICE_EXECUTION_TOKEN not set'
                 raise CredentialUnavailableError(message)
         return access_token
 
 
-class TokenFileCredential(CredentialProvider):
+class ConfigFileCredential(CredentialProvider):
+    def __init__(self):
+        if platform.system() == 'Windows':
+            config_dir = os.path.join(os.getenv('LOCALAPPDATA'), 'planqk')
+        else:
+            config_dir = os.path.join(os.path.expanduser('~'), '.config', 'planqk')
+        self.config_file = os.path.join(config_dir, 'config.json')
 
     def get_access_token(self) -> str:
-        access_token_file = os.environ.get(_TOKEN_FILE_ENV_VARIABLE)
-        if not access_token_file:
-            raise CredentialUnavailableError('Access Token file location not set')
-        if not os.path.isfile(access_token_file):
-            raise CredentialUnavailableError(f'Access Token file at {access_token_file} does not exist')
+        if not self.config_file:
+            raise CredentialUnavailableError('Config file location not set')
+        if not os.path.isfile(self.config_file):
+            raise CredentialUnavailableError(f'Config file at {self.config_file} does not exist')
         try:
-            access_token = TokenFileCredential.parse_access_token_file(access_token_file)
+            access_token = ConfigFileCredential.parse_file(self.config_file)
         except JSONDecodeError:
-            raise CredentialUnavailableError('Failed to parse Access Token file: Invalid JSON')
+            raise CredentialUnavailableError('Failed to parse config file: Invalid JSON')
         except KeyError as e:
-            raise CredentialUnavailableError(f'Failed to parse Access Token file: Missing expected value - {str(e)}')
+            raise CredentialUnavailableError(f'Failed to parse config file: Missing expected value - {str(e)}')
         except Exception as e:
-            raise CredentialUnavailableError(f'Failed to parse Access Token file: {str(e)}')
+            raise CredentialUnavailableError(f'Failed to parse config file: {str(e)}')
         return access_token
 
     @staticmethod
-    def parse_access_token_file(path) -> str:
+    def parse_file(path) -> str:
         with open(path, 'r') as file:
             data = json.load(file)
-            return data['access_token']
+            return data['auth']['value']
 
 
 class StaticCredential(CredentialProvider):
-
     def __init__(self, access_token=None):
         self.access_token = access_token
 
     def get_access_token(self) -> str:
         if not self.access_token:
             raise CredentialUnavailableError(f'Access Token not set')
         return self.access_token
 
 
 class DefaultCredentialsProvider(CredentialProvider):
-
     def __init__(self, access_token=None):
         self.credentials = [
-            EnvironmentCredential(),
             StaticCredential(access_token),
-            TokenFileCredential(),
+            EnvironmentCredential(),
+            ConfigFileCredential(),
         ]
 
     def get_access_token(self) -> str:
         for credential in self.credentials:
             try:
                 access_token = credential.get_access_token()
                 logger.debug('%s acquired an access token from %s',
```

### Comparing `planqk-quantum-1.6.0/planqk/qiskit/job.py` & `planqk-quantum-1.7.0/planqk/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.6.0/planqk/qiskit/provider.py` & `planqk-quantum-1.7.0/planqk/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.6.0/planqk/qiskit/providers/azure/planqk_azure_backend.py` & `planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.6.0/planqk/qiskit/providers/azure/planqk_azure_job.py` & `planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.6.0/planqk/qiskit/providers/azure/planqk_azure_provider.py` & `planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.6.0/planqk/qiskit/providers/azure/planqk_target_factory.py` & `planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_target_factory.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.6.0/planqk_quantum.egg-info/PKG-INFO` & `planqk-quantum-1.7.0/planqk_quantum.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python library for the PlanQK Quantum Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: StoneOne AG
 Author-email: info@stoneone.de
 License: apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,17 +12,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python library for the PlanQK Platform
 
 [![PyPI version](https://badge.fury.io/py/planqk-quantum.svg)](https://badge.fury.io/py/planqk-quantum)
 
-PlanQK Quantum Platform library is an SDK for developing quantum circuits with [Qiskit](https://pypi.org/project/qiskit) 
-that can be performed and metered as jobs on quantum devices provided by the [PlanQK Platform](https://docs.platform.planqk.de/).  
- 
+The `planqk-quantum` library is a SDK for developing quantum circuits using [Qiskit](https://pypi.org/project/qiskit) to be run on quantum devices provided by the [PlanQK Platform](https://docs.platform.planqk.de).
+
+## Getting Started
+
+Check out the following guides on how to get started with PlanQK:
+
+- [Tutorial on how to create a PlanQK Service using the `planqk-quantum` library](https://docs.platform.planqk.de/tutorials/tutorial-qiskit.html)
+- [General guide on how to create and deploy PlanQK Services](https://docs.platform.planqk.de/docs/service-platform/managed-services.html)
+
 ## Installation
 
 The package is released on PyPI and can be installed via `pip`:
 
 ```bash
 pip install planqk-quantum
 ```
```

### Comparing `planqk-quantum-1.6.0/planqk_quantum.egg-info/SOURCES.txt` & `planqk-quantum-1.7.0/planqk_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.6.0/setup.py` & `planqk-quantum-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="1.6.0",
+    version="1.7.0",
     author='StoneOne AG',
     author_email='info@stoneone.de',
     url='https://github.com/planqk/planqk-quantum',
     description='Python library for the PlanQK Quantum Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
```

