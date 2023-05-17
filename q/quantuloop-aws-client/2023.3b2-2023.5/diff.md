# Comparing `tmp/quantuloop_aws_client-2023.3b2.tar.gz` & `tmp/quantuloop_aws_client-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantuloop_aws_client-2023.3b2.tar", max compression
+gzip compressed data, was "quantuloop_aws_client-2023.5.tar", max compression
```

## Comparing `quantuloop_aws_client-2023.3b2.tar` & `quantuloop_aws_client-2023.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11545 2023-03-27 19:21:26.238411 quantuloop_aws_client-2023.3b2/LICENSE
--rw-r--r--   0        0        0      144 2023-03-27 19:40:10.266443 quantuloop_aws_client-2023.3b2/README.md
--rw-r--r--   0        0        0      539 2023-03-30 16:28:04.197260 quantuloop_aws_client-2023.3b2/pyproject.toml
--rw-r--r--   0        0        0     6948 2023-03-30 16:27:36.776943 quantuloop_aws_client-2023.3b2/src/quantuloop_aws_client/__init__.py
--rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 quantuloop_aws_client-2023.3b2/setup.py
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 quantuloop_aws_client-2023.3b2/PKG-INFO
+-rw-r--r--   0        0        0    11545 2023-05-10 11:38:29.173331 quantuloop_aws_client-2023.5/LICENSE
+-rw-r--r--   0        0        0      144 2023-05-10 11:38:29.173331 quantuloop_aws_client-2023.5/README.md
+-rw-r--r--   0        0        0      536 2023-05-17 15:54:11.382058 quantuloop_aws_client-2023.5/pyproject.toml
+-rw-r--r--   0        0        0     7904 2023-05-17 17:31:39.966244 quantuloop_aws_client-2023.5/src/quantuloop_aws_client/__init__.py
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 quantuloop_aws_client-2023.5/setup.py
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 quantuloop_aws_client-2023.5/PKG-INFO
```

### Comparing `quantuloop_aws_client-2023.3b2/LICENSE` & `quantuloop_aws_client-2023.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quantuloop_aws_client-2023.3b2/pyproject.toml` & `quantuloop_aws_client-2023.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "quantuloop-aws-client"
-version = "2023.03b2"
+version = "2023.05"
 description = ""
 authors = ["Quantuloop <dev@quantuloop.com>"]
 readme = "README.md"
 packages = [{include = "quantuloop_aws_client", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-ket-lang = "^0.5.1"
+ket-lang = "0.6.1"
 requests = "^2.28.2"
 pyjwt = "^2.6.0"
 cryptography = "^40.0.1"
 bcrypt = "^4.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `quantuloop_aws_client-2023.3b2/src/quantuloop_aws_client/__init__.py` & `quantuloop_aws_client-2023.5/src/quantuloop_aws_client/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from time import time
 from typing import Literal
 from random import Random
 import getpass
 import json
 import zipfile
 from ket import quantum_exec_timeout
-from ket.base import set_quantum_execution_target
+from ket.base import set_quantum_execution_target, set_process_features
 from ket.clib.libket import JSON
 import requests
 import jwt
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.backends import default_backend
 
 PRIVATE_KEY = ""
 URL = ""
 VERIFY = True
 TIMEOUT = 0
 
-AVAILABLE_SIMULATORS = []
+AVAILABLE_SIMULATORS = {}
 SIMULATOR = ''
 RNG = Random()
 DUMP_TYPE = 'shots'
 SHOTS = '1024'
 GPU_COUNT = '1'
 PRECISION = '1'
 
@@ -38,15 +38,15 @@
 def available_simulators() -> list[str]:
     """Get a list of the available quantum simulators."""
 
     global AVAILABLE_SIMULATORS
     AVAILABLE_SIMULATORS = requests.get(
         URL+'/simulators', timeout=30, verify=VERIFY).json()
 
-    return AVAILABLE_SIMULATORS
+    return list(AVAILABLE_SIMULATORS)
 
 
 def set_server(*,
                url: str,
                private_key: PathLike,
                passphrase: bool | bytes | None = None,
                verify: bool = True,
@@ -84,17 +84,29 @@
         global TIMEOUT
         TIMEOUT = timeout
         quantum_exec_timeout(timeout)
 
     available_simulators()
 
 
-def set_simulator(simulator: str | None = None, *,
+def set_simulator(simulator: Literal['Quantuloop Sparse',
+                                     'Quantuloop Dense',
+                                     'Quantuloop QuEST',
+                                     'KBW Sparse',
+                                     'KBW Dense',
+                                     'arn:aws:braket:::device/quantum-simulator/amazon/sv1',
+                                     'arn:aws:braket:::device/quantum-simulator/amazon/tn1',
+                                     'arn:aws:braket:::device/quantum-simulator/amazon/dm1',
+                                     'arn:aws:braket:us-west-1::device/qpu/rigetti/Aspen-M-3',
+                                     'arn:aws:braket:eu-west-2::device/qpu/oqc/Lucy',
+                                     'arn:aws:braket:::device/qpu/ionq/ionQdevice'] | None = None, *,
                   seed: any | None = None,
-                  dump_type: str | None = None,
+                  dump_type: Literal["vector",
+                                     "probability",
+                                     "shots"] | None = None,
                   shots: int | None = None,
                   gpu_count: int | None = None,
                   precision: Literal[1, 2] | None = None):
     """Set the simulation server as the quantum execution target.
 
     You must run :func:`quantuloop_aws_client.set_server` before calling this function.
 
@@ -112,21 +124,21 @@
         dump_type: must be "vector", "probability", or "shots", default "vector".
         shots: select the number of shots if ``dump_type`` is "shots".
         gpu_count: maximum number of GPUs; if set to 0, simulation will use all available GPUs.
         precision: floating point precision used in the simulation; positive values are: 1 for single precision (float) and 2 for double precision
     """
 
     if simulator is not None:
-        simulator = simulator.lower()
         if simulator not in AVAILABLE_SIMULATORS:
             raise ValueError(
-                f"parameter 'simulator' must be in {AVAILABLE_SIMULATORS}"
+                f"parameter 'simulator' must be in {list(AVAILABLE_SIMULATORS)}"
             )
         global SIMULATOR
         SIMULATOR = simulator
+        set_process_features(**AVAILABLE_SIMULATORS[simulator])
 
     if seed is not None:
         global RNG
         RNG = Random(seed)
 
     if dump_type:
         if dump_type not in ["vector", "probability", "shots"]:
```

### Comparing `quantuloop_aws_client-2023.3b2/setup.py` & `quantuloop_aws_client-2023.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['bcrypt>=4.0.1,<5.0.0',
  'cryptography>=40.0.1,<41.0.0',
- 'ket-lang>=0.5.1,<0.6.0',
+ 'ket-lang==0.6.1',
  'pyjwt>=2.6.0,<3.0.0',
  'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'quantuloop-aws-client',
-    'version': '2023.3b2',
+    'version': '2023.5',
     'description': '',
     'long_description': '# Quantuloop AWS Client\n\nClient to access your quantum simulator server on AWS. For more information, visit <https://simulator.quantuloop.com>.\n',
     'author': 'Quantuloop',
     'author_email': 'dev@quantuloop.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `quantuloop_aws_client-2023.3b2/PKG-INFO` & `quantuloop_aws_client-2023.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: quantuloop-aws-client
-Version: 2023.3b2
+Version: 2023.5
 Summary: 
 Author: Quantuloop
 Author-email: dev@quantuloop.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
 Requires-Dist: cryptography (>=40.0.1,<41.0.0)
-Requires-Dist: ket-lang (>=0.5.1,<0.6.0)
+Requires-Dist: ket-lang (==0.6.1)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Quantuloop AWS Client
 
 Client to access your quantum simulator server on AWS. For more information, visit <https://simulator.quantuloop.com>.
```

