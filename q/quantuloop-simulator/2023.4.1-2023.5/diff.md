# Comparing `tmp/quantuloop_simulator-2023.4.1.tar.gz` & `tmp/quantuloop_simulator-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantuloop_simulator-2023.4.1.tar", max compression
+gzip compressed data, was "quantuloop_simulator-2023.5.tar", max compression
```

## Comparing `quantuloop_simulator-2023.4.1.tar` & `quantuloop_simulator-2023.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11546 2023-04-27 20:18:00.209120 quantuloop_simulator-2023.4.1/LICENSE
--rw-r--r--   0        0        0     3480 2023-04-27 20:18:00.209120 quantuloop_simulator-2023.4.1/README.md
--rw-r--r--   0        0        0      674 2023-04-27 20:19:37.082320 quantuloop_simulator-2023.4.1/pyproject.toml
--rw-r--r--   0        0        0     3848 2023-04-27 20:24:23.873873 quantuloop_simulator-2023.4.1/src/quantuloop_simulator/__init__.py
--rw-r--r--   0        0        0     4340 1970-01-01 00:00:00.000000 quantuloop_simulator-2023.4.1/setup.py
--rw-r--r--   0        0        0     4161 1970-01-01 00:00:00.000000 quantuloop_simulator-2023.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11546 2023-04-27 20:18:00.209120 quantuloop_simulator-2023.5/LICENSE
+-rw-r--r--   0        0        0     3489 2023-05-17 16:54:38.301452 quantuloop_simulator-2023.5/README.md
+-rw-r--r--   0        0        0      676 2023-05-17 16:54:14.378176 quantuloop_simulator-2023.5/pyproject.toml
+-rw-r--r--   0        0        0     3848 2023-04-27 20:24:23.873873 quantuloop_simulator-2023.5/src/quantuloop_simulator/__init__.py
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 quantuloop_simulator-2023.5/setup.py
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 quantuloop_simulator-2023.5/PKG-INFO
```

### Comparing `quantuloop_simulator-2023.4.1/LICENSE` & `quantuloop_simulator-2023.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quantuloop_simulator-2023.4.1/README.md` & `quantuloop_simulator-2023.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
 The following system requirements are necessary to run the Quantuloop Dense simulator:
 
 * CUDA 11.2 or newer with compatible NVIDIA driver
 * Linux x86_64 with glibc 2.17 or newer
   * Ubuntu 18.04 or newer.
   * Red Hat Enterprise Linux 7 or newer.
-* Python 3.7 or newer
-* Ket 0.5.x
+* Python 3.8 or newer
+* Ket 0.6.1 or newer
 
 Quantuloop Dense is compatible only with CUDA architecture 70, 75, 80, and 86.
 
 ----
 
 By installing or using this package, you agree to the Quantuloop Quantum Simulator Suite EULA.
```

### Comparing `quantuloop_simulator-2023.4.1/pyproject.toml` & `quantuloop_simulator-2023.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "quantuloop-simulator"
-version = "2023.04.1"
+version = "2023.05"
 description = "Quantuloop Quantum Simulator Suite for HPC"
 authors = ["Quantuloop <dev@quantuloop.com>"]
 readme = "README.md"
 packages = [{include = "quantuloop_simulator", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-quantuloop-quest = "^0.2.1"
-quantuloop-dense = "^0.2"
-quantuloop-sparse = "^0.2"
+python = "^3.8"
+quantuloop-quest = "^0.2.2"
+quantuloop-dense = "^0.2.1"
+quantuloop-sparse = "^0.2.1"
 
 
 [[tool.poetry.source]]
 name = "quantuloop"
 url = "https://gitlab.com/api/v4/projects/43029789/packages/pypi/simple"
 default = false
 secondary = true
```

### Comparing `quantuloop_simulator-2023.4.1/src/quantuloop_simulator/__init__.py` & `quantuloop_simulator-2023.5/src/quantuloop_simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `quantuloop_simulator-2023.4.1/setup.py` & `quantuloop_simulator-2023.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 packages = \
 ['quantuloop_simulator']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['quantuloop-dense>=0.2,<0.3',
- 'quantuloop-quest>=0.2.1,<0.3.0',
- 'quantuloop-sparse>=0.2,<0.3']
+['quantuloop-dense>=0.2.1,<0.3.0',
+ 'quantuloop-quest>=0.2.2,<0.3.0',
+ 'quantuloop-sparse>=0.2.1,<0.3.0']
 
 setup_kwargs = {
     'name': 'quantuloop-simulator',
-    'version': '2023.4.1',
+    'version': '2023.5',
     'description': 'Quantuloop Quantum Simulator Suite for HPC',
-    'long_description': '# Quantuloop Quantum Simulator Suite for HPC\n\nThe **Quantuloop Quantum Simulator Suite for HPC** is a collection of high-performance quantum computer simulators for the **Ket language**. Since quantum algorithms explore distinct aspects of quantum computation to extract advantages, there is no silver bullet for the simulation of a quantum computer. The Quantuloop Quantum Simulator Suite for HPC offers three quantum simulators today, with new ones coming in the future. The simulators available today are:\n\n* **Quantuloop Sparse**, which brings the Bitwise Representation (implemented in the KBW Sparse) for HPC. This is the only simulator that implements this simulation algorithm and it provides many benefits:\n  * Ready for multi-GPU systems, allowing you to scale up simulations as needed.\n  * Efficient execution time with the amount of superposition, providing faster simulations.\n  * Exact simulation of more than 100 qubits [depending on the algorithm](https://repositorio.ufsc.br/handle/123456789/231060), making it ideal for larger simulations.\n* **Quantuloop Dense** is a state vector simulator built with the NVIDIA cuQuantum SDK cuStateVec. It provides several advantages:\n  * Great scalability in multi-GPU systems, enabling large simulations to be run with ease.\n  * The perfect fit for most quantum algorithms, allowing you to simulate many different types of quantum circuits.\n* **Quantuloop QuEST**, which is an interface for the open-source simulator QuEST. It provides many benefits, including:\n  * Excellent performance for single GPU systems, allowing you to run simulations even if you don\'t have access to multiple GPUs.\n\nBy using the Quantuloop Quantum Simulator Suite for HPC, you can enjoy the following benefits:\n\n* Faster simulation times, as the simulators are optimized for GPU-based computing.\n* Higher scalability, as multi-GPU systems, can be used to run large simulations.\n* Access to unique simulation algorithms, such as the Parallel Bitwise implemented in the Quantuloop Sparse simulator.\n* Ability to simulate a wide range of quantum algorithms and circuits, allowing you to explore the potential of quantum computing.\n\nThe use of this simulator is exclusively for Quantuloop\'s customers and partners. Contact your institution to get your access token or visit <https://quantuloop.com>.\n\n## Installation  \n\nInstalling using pip:\n\n```shell\npip install --index-url https://gitlab.com/api/v4/projects/43029789/packages/pypi/simple quantuloop-simulator\n```\n\nAdd in poetry:\n\n```shell\npoetry source add quantuloop https://gitlab.com/api/v4/projects/43029789/packages/pypi/simple --secondary\npoetry add quantuloop-simulator\n```\n\n## Usage\n\n```py\nimport quantuloop_simulator as ql\n\nql.set_simulator(\n    "Sparse", # or "Dense" or "QuEST"\n    token="YOR.ACCESS.TOKEN", # Quantuloop Access Token is required to use the simulators \n    precision=2, # optional, default 1\n    gpu_count=4, # optional, default use all GPUs\n)\n```\n\n## Compatibility\n\nThe following system requirements are necessary to run the Quantuloop Dense simulator:\n\n* CUDA 11.2 or newer with compatible NVIDIA driver\n* Linux x86_64 with glibc 2.17 or newer\n  * Ubuntu 18.04 or newer.\n  * Red Hat Enterprise Linux 7 or newer.\n* Python 3.7 or newer\n* Ket 0.5.x\n\nQuantuloop Dense is compatible only with CUDA architecture 70, 75, 80, and 86.\n\n----\n\nBy installing or using this package, you agree to the Quantuloop Quantum Simulator Suite EULA.\n\nAll rights reserved (C) 2023 Quantuloop\n',
+    'long_description': '# Quantuloop Quantum Simulator Suite for HPC\n\nThe **Quantuloop Quantum Simulator Suite for HPC** is a collection of high-performance quantum computer simulators for the **Ket language**. Since quantum algorithms explore distinct aspects of quantum computation to extract advantages, there is no silver bullet for the simulation of a quantum computer. The Quantuloop Quantum Simulator Suite for HPC offers three quantum simulators today, with new ones coming in the future. The simulators available today are:\n\n* **Quantuloop Sparse**, which brings the Bitwise Representation (implemented in the KBW Sparse) for HPC. This is the only simulator that implements this simulation algorithm and it provides many benefits:\n  * Ready for multi-GPU systems, allowing you to scale up simulations as needed.\n  * Efficient execution time with the amount of superposition, providing faster simulations.\n  * Exact simulation of more than 100 qubits [depending on the algorithm](https://repositorio.ufsc.br/handle/123456789/231060), making it ideal for larger simulations.\n* **Quantuloop Dense** is a state vector simulator built with the NVIDIA cuQuantum SDK cuStateVec. It provides several advantages:\n  * Great scalability in multi-GPU systems, enabling large simulations to be run with ease.\n  * The perfect fit for most quantum algorithms, allowing you to simulate many different types of quantum circuits.\n* **Quantuloop QuEST**, which is an interface for the open-source simulator QuEST. It provides many benefits, including:\n  * Excellent performance for single GPU systems, allowing you to run simulations even if you don\'t have access to multiple GPUs.\n\nBy using the Quantuloop Quantum Simulator Suite for HPC, you can enjoy the following benefits:\n\n* Faster simulation times, as the simulators are optimized for GPU-based computing.\n* Higher scalability, as multi-GPU systems, can be used to run large simulations.\n* Access to unique simulation algorithms, such as the Parallel Bitwise implemented in the Quantuloop Sparse simulator.\n* Ability to simulate a wide range of quantum algorithms and circuits, allowing you to explore the potential of quantum computing.\n\nThe use of this simulator is exclusively for Quantuloop\'s customers and partners. Contact your institution to get your access token or visit <https://quantuloop.com>.\n\n## Installation  \n\nInstalling using pip:\n\n```shell\npip install --index-url https://gitlab.com/api/v4/projects/43029789/packages/pypi/simple quantuloop-simulator\n```\n\nAdd in poetry:\n\n```shell\npoetry source add quantuloop https://gitlab.com/api/v4/projects/43029789/packages/pypi/simple --secondary\npoetry add quantuloop-simulator\n```\n\n## Usage\n\n```py\nimport quantuloop_simulator as ql\n\nql.set_simulator(\n    "Sparse", # or "Dense" or "QuEST"\n    token="YOR.ACCESS.TOKEN", # Quantuloop Access Token is required to use the simulators \n    precision=2, # optional, default 1\n    gpu_count=4, # optional, default use all GPUs\n)\n```\n\n## Compatibility\n\nThe following system requirements are necessary to run the Quantuloop Dense simulator:\n\n* CUDA 11.2 or newer with compatible NVIDIA driver\n* Linux x86_64 with glibc 2.17 or newer\n  * Ubuntu 18.04 or newer.\n  * Red Hat Enterprise Linux 7 or newer.\n* Python 3.8 or newer\n* Ket 0.6.1 or newer\n\nQuantuloop Dense is compatible only with CUDA architecture 70, 75, 80, and 86.\n\n----\n\nBy installing or using this package, you agree to the Quantuloop Quantum Simulator Suite EULA.\n\nAll rights reserved (C) 2023 Quantuloop\n',
     'author': 'Quantuloop',
     'author_email': 'dev@quantuloop.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `quantuloop_simulator-2023.4.1/PKG-INFO` & `quantuloop_simulator-2023.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: quantuloop-simulator
-Version: 2023.4.1
+Version: 2023.5
 Summary: Quantuloop Quantum Simulator Suite for HPC
 Author: Quantuloop
 Author-email: dev@quantuloop.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: quantuloop-dense (>=0.2,<0.3)
-Requires-Dist: quantuloop-quest (>=0.2.1,<0.3.0)
-Requires-Dist: quantuloop-sparse (>=0.2,<0.3)
+Requires-Dist: quantuloop-dense (>=0.2.1,<0.3.0)
+Requires-Dist: quantuloop-quest (>=0.2.2,<0.3.0)
+Requires-Dist: quantuloop-sparse (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # Quantuloop Quantum Simulator Suite for HPC
 
 The **Quantuloop Quantum Simulator Suite for HPC** is a collection of high-performance quantum computer simulators for the **Ket language**. Since quantum algorithms explore distinct aspects of quantum computation to extract advantages, there is no silver bullet for the simulation of a quantum computer. The Quantuloop Quantum Simulator Suite for HPC offers three quantum simulators today, with new ones coming in the future. The simulators available today are:
 
 * **Quantuloop Sparse**, which brings the Bitwise Representation (implemented in the KBW Sparse) for HPC. This is the only simulator that implements this simulation algorithm and it provides many benefits:
@@ -71,16 +70,16 @@
 
 The following system requirements are necessary to run the Quantuloop Dense simulator:
 
 * CUDA 11.2 or newer with compatible NVIDIA driver
 * Linux x86_64 with glibc 2.17 or newer
   * Ubuntu 18.04 or newer.
   * Red Hat Enterprise Linux 7 or newer.
-* Python 3.7 or newer
-* Ket 0.5.x
+* Python 3.8 or newer
+* Ket 0.6.1 or newer
 
 Quantuloop Dense is compatible only with CUDA architecture 70, 75, 80, and 86.
 
 ----
 
 By installing or using this package, you agree to the Quantuloop Quantum Simulator Suite EULA.
```

