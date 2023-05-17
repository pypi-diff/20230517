# Comparing `tmp/psfam-0.0.13.tar.gz` & `tmp/psfam-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psfam-0.0.13.tar", last modified: Mon May 15 16:58:01 2023, max compression
+gzip compressed data, was "psfam-0.0.14.tar", last modified: Wed May 17 16:51:45 2023, max compression
```

## Comparing `psfam-0.0.13.tar` & `psfam-0.0.14.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 16:58:01.611863 psfam-0.0.13/
--rw-rw-rw-   0        0        0     6296 2023-05-15 16:58:01.610863 psfam-0.0.13/PKG-INFO
--rw-rw-rw-   0        0        0     5705 2023-05-05 16:06:42.000000 psfam-0.0.13/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 16:58:01.593861 psfam-0.0.13/psfam/
--rw-rw-rw-   0        0        0        0 2023-04-24 20:25:09.000000 psfam-0.0.13/psfam/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-29 21:06:06.000000 psfam-0.0.13/psfam/family.py
--rw-rw-rw-   0        0        0     5818 2023-04-25 15:45:54.000000 psfam-0.0.13/psfam/matrix_generator.py
--rw-rw-rw-   0        0        0     9947 2023-04-28 19:02:32.000000 psfam-0.0.13/psfam/pauli_organizer.py
--rw-rw-rw-   0        0        0     7605 2023-04-25 15:41:08.000000 psfam-0.0.13/psfam/pauli_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:58:01.608917 psfam-0.0.13/psfam.egg-info/
--rw-rw-rw-   0        0        0     6296 2023-05-15 16:58:01.000000 psfam-0.0.13/psfam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-15 16:58:01.000000 psfam-0.0.13/psfam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 16:58:01.000000 psfam-0.0.13/psfam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-15 16:58:01.000000 psfam-0.0.13/psfam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 16:58:01.000000 psfam-0.0.13/psfam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 16:58:01.612863 psfam-0.0.13/setup.cfg
--rw-rw-rw-   0        0        0      939 2023-05-15 16:56:48.000000 psfam-0.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:51:45.572756 psfam-0.0.14/
+-rw-rw-rw-   0        0        0     6349 2023-05-17 16:51:45.569747 psfam-0.0.14/PKG-INFO
+-rw-rw-rw-   0        0        0     5758 2023-05-15 20:34:34.000000 psfam-0.0.14/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 16:51:45.500611 psfam-0.0.14/psfam/
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:25:09.000000 psfam-0.0.14/psfam/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-29 21:06:06.000000 psfam-0.0.14/psfam/family.py
+-rw-rw-rw-   0        0        0     5818 2023-04-25 15:45:54.000000 psfam-0.0.14/psfam/matrix_generator.py
+-rw-rw-rw-   0        0        0     9947 2023-04-28 19:02:32.000000 psfam-0.0.14/psfam/pauli_organizer.py
+-rw-rw-rw-   0        0        0     7605 2023-04-25 15:41:08.000000 psfam-0.0.14/psfam/pauli_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:51:45.565670 psfam-0.0.14/psfam.egg-info/
+-rw-rw-rw-   0        0        0     6349 2023-05-17 16:51:45.000000 psfam-0.0.14/psfam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-17 16:51:45.000000 psfam-0.0.14/psfam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 16:51:45.000000 psfam-0.0.14/psfam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-17 16:51:45.000000 psfam-0.0.14/psfam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-17 16:51:45.000000 psfam-0.0.14/psfam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 16:51:45.573759 psfam-0.0.14/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-05-17 16:45:28.000000 psfam-0.0.14/setup.py
```

### Comparing `psfam-0.0.13/PKG-INFO` & `psfam-0.0.14/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: psfam
-Version: 0.0.13
-Summary: First attempt at putting psfam in a build.
+Version: 0.0.14
+Summary: Pauli string organizer for dense operators.
 Home-page: UNKNOWN
 Author: Ben Reggio
 Author-email: benjreggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
@@ -16,21 +16,20 @@
 
 The Psfam package is a python package which organizes the complete set of pauli strings of any size into commuting families for VQE, finding a unitary matrix from clifford operators which diagonalizes all of the strings, and implementing this unitary matrix on a qiskit circuit.
 
 Below are instructions on how to use the Psfam package. It will show the process of using a PauliOrganizer object to partition strings, then calculating an expectation value on a qiskit simulator.
 
 You'll need numpy and qiskit, so lets import those:
 
-<!---
 ```python
 from psfam.pauli_organizer import *
 import numpy as np
 from qiskit import *
 from qiskit.circuit.library import EfficientSU2
-```-->
+```
 
 Pick the number of qubits, and assign this to $m$. Pauli_organizer takes only the number of qubits as an argument. In its constructor, it partitions all the families. We can look at the properties of the object using properties(). This will tell us what $A$ matrix was used to generate all of the families. 
 
 
 ```python
 m=2
 PO = PauliOrganizer(m)
@@ -152,15 +151,15 @@
 qc.draw('mpl')
 ```
 
 
 
 
     
-![png](output_15_0.png)
+![](https://raw.githubusercontent.com/Benjreggio/psfamtest/blob/main/output_15_0.png)
     
 
 
 
 This code is straight from here: https://qiskit.org/documentation/tutorials/circuits/1_getting_started_with_qiskit.html. qiskit has methods to visualize the results.
```

### Comparing `psfam-0.0.13/README.md` & `psfam-0.0.14/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 The Psfam package is a python package which organizes the complete set of pauli strings of any size into commuting families for VQE, finding a unitary matrix from clifford operators which diagonalizes all of the strings, and implementing this unitary matrix on a qiskit circuit.
 
 Below are instructions on how to use the Psfam package. It will show the process of using a PauliOrganizer object to partition strings, then calculating an expectation value on a qiskit simulator.
 
 You'll need numpy and qiskit, so lets import those:
 
-<!---
 ```python
 from psfam.pauli_organizer import *
 import numpy as np
 from qiskit import *
 from qiskit.circuit.library import EfficientSU2
-```-->
+```
 
 Pick the number of qubits, and assign this to $m$. Pauli_organizer takes only the number of qubits as an argument. In its constructor, it partitions all the families. We can look at the properties of the object using properties(). This will tell us what $A$ matrix was used to generate all of the families. 
 
 
 ```python
 m=2
 PO = PauliOrganizer(m)
@@ -138,15 +137,15 @@
 qc.draw('mpl')
 ```
 
 
 
 
     
-![png](output_15_0.png)
+![](https://raw.githubusercontent.com/Benjreggio/psfamtest/blob/main/output_15_0.png)
     
 
 
 
 This code is straight from here: https://qiskit.org/documentation/tutorials/circuits/1_getting_started_with_qiskit.html. qiskit has methods to visualize the results.
```

### Comparing `psfam-0.0.13/psfam/family.py` & `psfam-0.0.14/psfam/family.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.13/psfam/matrix_generator.py` & `psfam-0.0.14/psfam/matrix_generator.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.13/psfam/pauli_organizer.py` & `psfam-0.0.14/psfam/pauli_organizer.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.13/psfam/pauli_utils.py` & `psfam-0.0.14/psfam/pauli_utils.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.13/psfam.egg-info/PKG-INFO` & `psfam-0.0.14/psfam.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: psfam
-Version: 0.0.13
-Summary: First attempt at putting psfam in a build.
+Version: 0.0.14
+Summary: Pauli string organizer for dense operators.
 Home-page: UNKNOWN
 Author: Ben Reggio
 Author-email: benjreggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
@@ -16,21 +16,20 @@
 
 The Psfam package is a python package which organizes the complete set of pauli strings of any size into commuting families for VQE, finding a unitary matrix from clifford operators which diagonalizes all of the strings, and implementing this unitary matrix on a qiskit circuit.
 
 Below are instructions on how to use the Psfam package. It will show the process of using a PauliOrganizer object to partition strings, then calculating an expectation value on a qiskit simulator.
 
 You'll need numpy and qiskit, so lets import those:
 
-<!---
 ```python
 from psfam.pauli_organizer import *
 import numpy as np
 from qiskit import *
 from qiskit.circuit.library import EfficientSU2
-```-->
+```
 
 Pick the number of qubits, and assign this to $m$. Pauli_organizer takes only the number of qubits as an argument. In its constructor, it partitions all the families. We can look at the properties of the object using properties(). This will tell us what $A$ matrix was used to generate all of the families. 
 
 
 ```python
 m=2
 PO = PauliOrganizer(m)
@@ -152,15 +151,15 @@
 qc.draw('mpl')
 ```
 
 
 
 
     
-![png](output_15_0.png)
+![](https://raw.githubusercontent.com/Benjreggio/psfamtest/blob/main/output_15_0.png)
     
 
 
 
 This code is straight from here: https://qiskit.org/documentation/tutorials/circuits/1_getting_started_with_qiskit.html. qiskit has methods to visualize the results.
```

### Comparing `psfam-0.0.13/setup.py` & `psfam-0.0.14/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "psfam",
-    version = "0.0.13",
+    version = "0.0.14",
     author = "Ben Reggio",
     author_email = "benjreggio@gmail.com",
-    description = ("First attempt at putting psfam in a build."),
+    description = ("Pauli string organizer for dense operators."),
     license = "MIT",
     packages=['psfam'],
     long_description=read('README.md'),
     long_description_content_type = "text/markdown",
-    install_requires = ['scikit-build','markdown','numpy','qiskit','galois','scipy'],
+    install_requires = ['scikit-build>= 0.1','markdown','numpy>=1.22','qiskit>=0.43','galois>=0.1','scipy>=1.8'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
     ],
 )
```

