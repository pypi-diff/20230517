# Comparing `tmp/oganesson-0.1.3.tar.gz` & `tmp/oganesson-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oganesson-0.1.3.tar", last modified: Wed May 17 00:47:12 2023, max compression
+gzip compressed data, was "oganesson-0.1.4.tar", last modified: Wed May 17 14:14:02 2023, max compression
```

## Comparing `oganesson-0.1.3.tar` & `oganesson-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.143987 oganesson-0.1.3/
--rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.3/.gitattributes
--rw-rw-rw-   0        0        0      344 2023-05-17 00:45:53.000000 oganesson-0.1.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2678 2023-05-17 00:47:12.143987 oganesson-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2239 2023-05-17 00:22:04.000000 oganesson-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.116986 oganesson-0.1.3/oganesson/
--rw-rw-rw-   0        0        0        5 2023-05-17 00:46:43.000000 oganesson-0.1.3/oganesson/VERSION
--rw-rw-rw-   0        0        0      428 2023-05-17 00:46:24.000000 oganesson-0.1.3/oganesson/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.3/oganesson/__main__.py
--rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.3/oganesson/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.136986 oganesson-0.1.3/oganesson/descriptors/
--rw-rw-rw-   0        0        0     1226 2023-05-17 00:39:53.000000 oganesson-0.1.3/oganesson/descriptors/__init__.py
--rw-rw-rw-   0        0        0     7896 2023-05-11 01:10:06.000000 oganesson-0.1.3/oganesson/descriptors/bacd.py
--rw-rw-rw-   0        0        0     3646 2023-05-16 23:54:40.000000 oganesson-0.1.3/oganesson/descriptors/rosa.py
--rw-rw-rw-   0        0        0     2801 2023-05-16 03:55:40.000000 oganesson-0.1.3/oganesson/descriptors/symmetry_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.137987 oganesson-0.1.3/oganesson/genetic_algorithms/
--rw-rw-rw-   0        0        0     7853 2023-05-17 00:02:20.000000 oganesson-0.1.3/oganesson/genetic_algorithms/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.3/oganesson/ogai.py
--rw-rw-rw-   0        0        0     6700 2023-05-16 04:38:44.000000 oganesson-0.1.3/oganesson/ogstructure.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.141985 oganesson-0.1.3/oganesson/utilities/
--rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.3/oganesson/utilities/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.3/oganesson/utilities/atomic_data.py
--rw-rw-rw-   0        0        0   405452 2023-05-16 02:56:53.000000 oganesson-0.1.3/oganesson/utilities/bonds_dictionary.py
--rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.3/oganesson/version.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.132989 oganesson-0.1.3/oganesson.egg-info/
--rw-rw-rw-   0        0        0     2678 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 00:47:12.143987 oganesson-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-05-17 00:46:24.000000 oganesson-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.086581 oganesson-0.1.4/
+-rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.4/.gitattributes
+-rw-rw-rw-   0        0        0     3018 2023-05-17 14:10:37.000000 oganesson-0.1.4/.gitignore
+-rw-rw-rw-   0        0        0      471 2023-05-17 14:13:40.000000 oganesson-0.1.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.4/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3314 2023-05-17 14:14:02.085579 oganesson-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2930 2023-05-17 14:10:37.000000 oganesson-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.056537 oganesson-0.1.4/assets/
+-rw-rw-rw-   0        0        0     2080 2023-05-16 02:19:45.000000 oganesson-0.1.4/assets/logo.svg
+drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.062079 oganesson-0.1.4/oganesson/
+-rw-rw-rw-   0        0        0        5 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/VERSION
+-rw-rw-rw-   0        0        0      901 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.4/oganesson/__main__.py
+-rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.4/oganesson/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.074069 oganesson-0.1.4/oganesson/dataset/
+-rw-rw-rw-   0        0        0     2315 2023-05-14 23:40:10.000000 oganesson-0.1.4/oganesson/dataset/vasp.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.079594 oganesson-0.1.4/oganesson/descriptors/
+-rw-rw-rw-   0        0        0     1454 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/__init__.py
+-rw-rw-rw-   0        0        0     7939 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/bacd.py
+-rw-rw-rw-   0        0        0      901 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/descriptors.py
+-rw-rw-rw-   0        0        0     5267 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/dscribe.py
+-rw-rw-rw-   0        0        0     3606 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/rosa.py
+-rw-rw-rw-   0        0        0     2805 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/symmetry_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.080593 oganesson-0.1.4/oganesson/genetic_algorithms/
+-rw-rw-rw-   0        0        0     7853 2023-05-17 13:42:10.000000 oganesson-0.1.4/oganesson/genetic_algorithms/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.4/oganesson/ogai.py
+-rw-rw-rw-   0        0        0    10992 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/ogstructure.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.081593 oganesson-0.1.4/oganesson/reinforcement_learning/
+-rw-rw-rw-   0        0        0        0 2023-05-16 14:41:36.000000 oganesson-0.1.4/oganesson/reinforcement_learning/m3gnet.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.084580 oganesson-0.1.4/oganesson/utilities/
+-rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.4/oganesson/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.4/oganesson/utilities/atomic_data.py
+-rw-rw-rw-   0        0        0   405452 2023-05-17 13:20:45.000000 oganesson-0.1.4/oganesson/utilities/bonds_dictionary.py
+-rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.4/oganesson/version.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.074069 oganesson-0.1.4/oganesson.egg-info/
+-rw-rw-rw-   0        0        0     3314 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      878 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 14:14:02.086581 oganesson-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-05-17 00:46:24.000000 oganesson-0.1.4/setup.py
```

### Comparing `oganesson-0.1.3/CONTRIBUTING.rst` & `oganesson-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.3/LICENSE` & `oganesson-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.3/PKG-INFO` & `oganesson-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.3
+Version: 0.1.4
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
 Keywords: ai,machine learning
 Description-Content-Type: text/markdown
@@ -26,27 +26,29 @@
 # Features
 
 `og` is currently under active development. The following features are currently available.
 
 
 ## Machine learning descriptors
 
-`og` will bring together machine learning descriptors for materials and molecules. At the moment, the three descriptors available are those introduced in this [publication](https://doi.org/10.1186/s13321-022-00658-9). 
+`og` will bring together machine learning descriptors for materials and molecules within a unified framework. `og` currently provides the following descriptors:
+
+- The BACD, ROSA and SymmetryFunctions introduced in this [publication](https://doi.org/10.1186/s13321-022-00658-9)
+- Most of the descriptors from [DScribe](https://github.com/SINGROUP/dscribe)
 
 Each descriptor has its own class, which extends the `Descriptors` class in the `oganesson.descriptors` module. Here is an example of how to describe a structure using the `BACD` and `SymmetryFunctions` descriptor classes.
 
 ```python
-from oganesson.descriptors.bacd import BACD
-from oganesson.descriptors.symmetry_functions import SymmetryFunctions
+from oganesson.descriptors import BACD, SymmetryFunctions
 from oganesson.ogstructure import OgStructure
 
-bacd = BACD(OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif'))
+bacd = BACD(OgStructure(file_name='examples/structures/Li3PO4_mp-13725.cif'))
 print(bacd.describe())
 
-sf = SymmetryFunctions(OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif'))
+sf = SymmetryFunctions(OgStructure(file_name='examples/structures/Li3PO4_mp-13725.cif'))
 print(sf.describe())
 ```
 
 ## Genetic algorithms
 
 The main purpose of `og` is to make complex artificial intelligence workflows easy to compose. Here is an example: running a genetic search for structures, where the structure optimization is performed using the M3GNET neural network model.
 
@@ -57,12 +59,23 @@
     ga.evolve()
 ```
 
 ## Generation of the diffusion path for NEB calculations
 
 The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and then write the POSCAR image files in each of these folders.
 
+In the following example, we explore the possible Li diffusion paths in Li3PO4, given there are 6 Li atoms in the cell.
+
 ```python
 from oganesson.ogstructure import OgStructure
-og = OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif')
+og = OgStructure(file_name='examples/structures/Li3PO4_mp-13725.cif')
 og.generate_neb('Li')
 ```
+Note that the default value of `r`, which is 3, is sufficient for lithium systems. However, for the case of larger atoms such as Na, a larger value of `r` would be required.
+
+## Finding a reasonable adsorption site of an atom on a surface
+
+```python
+from oganesson.ogstructure import OgStructure
+og=OgStructure(file_name='examples/structures/MoS2.vasp')
+og.add_atom_to_surface('Li').structure.to('MoS2_Li.vasp','poscar')
+```
```

### Comparing `oganesson-0.1.3/README.md` & `oganesson-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,69 @@
-<img src="./assets/logo.svg" width="200px">
-
-# Oganesson
-
-`oganesson` (`og` for short) is a python package that enables you to apply artificial intelligence workflows to your material discovery projects.
-
-
-## Installation
-
-You can install `og` using the `pip` command as follows:
-
-`pip install oganesson`
-
-# Features
-
-`og` is currently under active development. The following features are currently available.
-
-
-## Machine learning descriptors
-
-`og` will bring together machine learning descriptors for materials and molecules. At the moment, the three descriptors available are those introduced in this [publication](https://doi.org/10.1186/s13321-022-00658-9). 
-
-Each descriptor has its own class, which extends the `Descriptors` class in the `oganesson.descriptors` module. Here is an example of how to describe a structure using the `BACD` and `SymmetryFunctions` descriptor classes.
-
-```python
-from oganesson.descriptors.bacd import BACD
-from oganesson.descriptors.symmetry_functions import SymmetryFunctions
-from oganesson.ogstructure import OgStructure
-
-bacd = BACD(OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif'))
-print(bacd.describe())
-
-sf = SymmetryFunctions(OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif'))
-print(sf.describe())
-```
-
-## Genetic algorithms
-
-The main purpose of `og` is to make complex artificial intelligence workflows easy to compose. Here is an example: running a genetic search for structures, where the structure optimization is performed using the M3GNET neural network model.
-
-```python
-from oganesson.genetic_algorithms import GA
-ga = GA(['Na']*4 + ['H']*4)
-for i in range(10):
-    ga.evolve()
-```
-
-## Generation of the diffusion path for NEB calculations
-
-The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and then write the POSCAR image files in each of these folders.
-
-```python
-from oganesson.ogstructure import OgStructure
-og = OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif')
-og.generate_neb('Li')
+<img src="./assets/logo.svg" width="200px">
+
+# Oganesson
+
+`oganesson` (`og` for short) is a python package that enables you to apply artificial intelligence workflows to your material discovery projects.
+
+
+## Installation
+
+You can install `og` using the `pip` command as follows:
+
+`pip install oganesson`
+
+# Features
+
+`og` is currently under active development. The following features are currently available.
+
+
+## Machine learning descriptors
+
+`og` will bring together machine learning descriptors for materials and molecules within a unified framework. `og` currently provides the following descriptors:
+
+- The BACD, ROSA and SymmetryFunctions introduced in this [publication](https://doi.org/10.1186/s13321-022-00658-9)
+- Most of the descriptors from [DScribe](https://github.com/SINGROUP/dscribe)
+
+Each descriptor has its own class, which extends the `Descriptors` class in the `oganesson.descriptors` module. Here is an example of how to describe a structure using the `BACD` and `SymmetryFunctions` descriptor classes.
+
+```python
+from oganesson.descriptors import BACD, SymmetryFunctions
+from oganesson.ogstructure import OgStructure
+
+bacd = BACD(OgStructure(file_name='examples/structures/Li3PO4_mp-13725.cif'))
+print(bacd.describe())
+
+sf = SymmetryFunctions(OgStructure(file_name='examples/structures/Li3PO4_mp-13725.cif'))
+print(sf.describe())
+```
+
+## Genetic algorithms
+
+The main purpose of `og` is to make complex artificial intelligence workflows easy to compose. Here is an example: running a genetic search for structures, where the structure optimization is performed using the M3GNET neural network model.
+
+```python
+from oganesson.genetic_algorithms import GA
+ga = GA(['Na']*4 + ['H']*4)
+for i in range(10):
+    ga.evolve()
+```
+
+## Generation of the diffusion path for NEB calculations
+
+The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and then write the POSCAR image files in each of these folders.
+
+In the following example, we explore the possible Li diffusion paths in Li3PO4, given there are 6 Li atoms in the cell.
+
+```python
+from oganesson.ogstructure import OgStructure
+og = OgStructure(file_name='examples/structures/Li3PO4_mp-13725.cif')
+og.generate_neb('Li')
+```
+Note that the default value of `r`, which is 3, is sufficient for lithium systems. However, for the case of larger atoms such as Na, a larger value of `r` would be required.
+
+## Finding a reasonable adsorption site of an atom on a surface
+
+```python
+from oganesson.ogstructure import OgStructure
+og=OgStructure(file_name='examples/structures/MoS2.vasp')
+og.add_atom_to_surface('Li').structure.to('MoS2_Li.vasp','poscar')
 ```
```

### Comparing `oganesson-0.1.3/oganesson/cli.py` & `oganesson-0.1.4/oganesson/cli.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.3/oganesson/descriptors/__init__.py` & `oganesson-0.1.4/oganesson/descriptors/descriptors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from enum import Enum
 from ase import Atoms
 from pymatgen.core import Structure
 from abc import ABC, abstractmethod
 from oganesson.ogstructure import OgStructure
+from typing import Union
 
 class Descriptors(ABC):
-    def __init__(self, structure: Atoms | Structure | str | OgStructure) -> None:
+    def __init__(self, structure: Union[Atoms, Structure, str, OgStructure]) -> None:
         if isinstance(structure, OgStructure):
             self.structure = structure
         else:
             self.structure = OgStructure(structure)
 
     @abstractmethod
     def describe(self):
@@ -22,20 +22,7 @@
         '''
     
     def sensitivity_analysis(self):
         '''
         Perform standardized tests on the values of descriptors by perturbing the original structure
         and reporting the resulting perturbation in descriptors.
         '''
-
-class DescriptorsName(Enum):
-    BACD = 0
-    ROSA = 1
-    SymmetryFunctions = 2
-
-
-class Describe:
-    def __init__(self, 
-                 structure: Atoms | Structure | str | OgStructure, 
-                 descriptor: DescriptorsName | Descriptors, 
-                 string_format: str = None) -> None:
-        pass
```

### Comparing `oganesson-0.1.3/oganesson/descriptors/bacd.py` & `oganesson-0.1.4/oganesson/descriptors/bacd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Union
 from ase import Atoms
 from pymatgen.core import Structure
 from pymatgen.io.cif import CifParser
 from urllib.request import urlopen
 import pandas as pd
 import numpy as np
-from oganesson.descriptors import Descriptors
+from oganesson.descriptors.descriptors import Descriptors
 from oganesson.ogstructure import OgStructure
+from typing import Union
 
-class BACD(Descriptors):
-    def __init__(self, structure: Atoms | Structure | str | OgStructure) -> None:
+class _BACD(Descriptors):
+    def __init__(self, structure: Union[Atoms, Structure, str, OgStructure]) -> None:
         super().__init__(structure)
 
     def describe(self):
         
         atomic_numbers = []
 
         distance_matrix = []
```

### Comparing `oganesson-0.1.3/oganesson/descriptors/rosa.py` & `oganesson-0.1.4/oganesson/descriptors/rosa.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,111 +1,101 @@
-from ase import Atoms
-import os
-import string
-import random
-from pymatgen.core import Structure
-from pymatgen.io.cif import CifParser
-from urllib.request import urlopen
-import pandas as pd
-import matplotlib.pyplot as plt
-import pandas as pd
-import numpy as np
-from ase.build import bulk, niggli_reduce
-from gpaw import GPAW
-from ase.io import read
-import pandas as pd
-
-import glob
-
-from oganesson.descriptors import Descriptors
-from oganesson.ogstructure import OgStructure
-
-
-class ROSA(Descriptors):
-    def __init__(self, structure: Atoms | Structure | str | OgStructure, psfolder: str, descriptor_size=100, calculation_type='bulk') -> None:
-        super().__init__(structure)
-        self.psfolder = psfolder
-        self.descriptor_size = descriptor_size
-        self.calculation_type = calculation_type
-        g = glob.glob(
-            self.psfolder + '/*.PBE.gz')
-
-        self.available_atoms = []
-        for i in g:
-            self.available_atoms += [i.replace(
-                psfolder + '/', '').split('.')[0]]
-
-    def fix_psuedo(self, a):
-        for i in range(len(a)):
-            if not a[i].symbol in self.available_atoms:
-                print(a[i].symbol, 'is not available in GPAW, replacing it with Y')
-                a[i].symbol = 'Y'
-
-    def get_descriptors_for_structure(self, a):
-        half_descriptor_size = int(self.descriptor_size/2)
-        calc = GPAW(mode='lcao',
-                    xc='PBE',
-                    maxiter=1,
-                    convergence={'density': 1},
-                    kpts=[1, 1, 1])
-
-        # a.set_calculator(calc)
-        calc.calculate(a)
-        H = calc.hamiltonian
-        descriptors_below = []
-        descriptors_above = []
-
-        num_atoms = a.get_global_number_of_atoms()
-
-        ev = pd.DataFrame(calc.get_eigenvalues())
-        ef = calc.get_fermi_level()
-        ev_below = ev.loc[ev.values <= ef]
-        ev_above = ev.loc[ev.values > ef]
-
-        for e in ev_below.values.tolist()[::-1]:
-            descriptors_below += e
-        if len(ev_below) > half_descriptor_size:
-            descriptors_below = descriptors_below[0:half_descriptor_size]
-        elif len(ev_below) < half_descriptor_size:
-            for e in range(half_descriptor_size-len(ev_below)):
-                descriptors_below += [0]
-        descriptors_below = descriptors_below[::-1]
-
-        for e in ev_above.values.tolist():
-            descriptors_above += e
-        if len(ev_above) > half_descriptor_size:
-            descriptors_above = descriptors_above[0:half_descriptor_size]
-        elif len(ev_above) < half_descriptor_size:
-            for e in range(half_descriptor_size-len(ev_above)):
-                descriptors_above += [0]
-
-        return descriptors_below + descriptors_above + \
-            [ef,
-             H.e_band/num_atoms,
-             H.e_coulomb/num_atoms,
-             H.e_entropy/num_atoms,
-             H.e_external/num_atoms,
-             H.e_kinetic/num_atoms,
-             H.e_kinetic0/num_atoms,
-             H.e_xc/num_atoms,
-             H.e_total_free/num_atoms]
-
-    def describe(self):
-
-        structure = self.structure()
-
-        a = Atoms(pbc=True, cell=structure.lattice.matrix,
-                  positions=structure.cart_coords, numbers=structure.atomic_numbers)
-
-        d_pristine = []
-        try:
-            if self.calculation_type == 'bulk':
-                niggli_reduce(a)
-            self.fix_psuedo(a)
-            d_pristine = self.get_descriptors_for_structure(a)
-
-        except Exception as e:
-            print('Problem in GPAW')
-        if len(d_pristine) > 0:
-            return d_pristine
-        else:
-            return []
+from ase import Atoms
+from pymatgen.core import Structure
+import pandas as pd
+import matplotlib.pyplot as plt
+import pandas as pd
+from ase.build import niggli_reduce
+from gpaw import GPAW
+import glob
+from oganesson.descriptors.descriptors import Descriptors
+from oganesson.ogstructure import OgStructure
+from typing import Union
+
+class _ROSA(Descriptors):
+    def __init__(self, structure: Union[Atoms, Structure, str, OgStructure], psfolder: str, descriptor_size=100, calculation_type='bulk') -> None:
+        super().__init__(structure)
+        self.psfolder = psfolder
+        self.descriptor_size = descriptor_size
+        self.calculation_type = calculation_type
+        g = glob.glob(
+            self.psfolder + '/*.PBE.gz')
+
+        self.available_atoms = []
+        for i in g:
+            self.available_atoms += [i.replace(
+                psfolder + '/', '').split('.')[0]]
+
+    def fix_psuedo(self, a):
+        for i in range(len(a)):
+            if not a[i].symbol in self.available_atoms:
+                print(a[i].symbol, 'is not available in GPAW, replacing it with Y')
+                a[i].symbol = 'Y'
+
+    def get_descriptors_for_structure(self, a):
+        half_descriptor_size = int(self.descriptor_size/2)
+        calc = GPAW(mode='lcao',
+                    xc='PBE',
+                    maxiter=1,
+                    convergence={'density': 1},
+                    kpts=[1, 1, 1])
+
+        # a.set_calculator(calc)
+        calc.calculate(a)
+        H = calc.hamiltonian
+        descriptors_below = []
+        descriptors_above = []
+
+        num_atoms = a.get_global_number_of_atoms()
+
+        ev = pd.DataFrame(calc.get_eigenvalues())
+        ef = calc.get_fermi_level()
+        ev_below = ev.loc[ev.values <= ef]
+        ev_above = ev.loc[ev.values > ef]
+
+        for e in ev_below.values.tolist()[::-1]:
+            descriptors_below += e
+        if len(ev_below) > half_descriptor_size:
+            descriptors_below = descriptors_below[0:half_descriptor_size]
+        elif len(ev_below) < half_descriptor_size:
+            for e in range(half_descriptor_size-len(ev_below)):
+                descriptors_below += [0]
+        descriptors_below = descriptors_below[::-1]
+
+        for e in ev_above.values.tolist():
+            descriptors_above += e
+        if len(ev_above) > half_descriptor_size:
+            descriptors_above = descriptors_above[0:half_descriptor_size]
+        elif len(ev_above) < half_descriptor_size:
+            for e in range(half_descriptor_size-len(ev_above)):
+                descriptors_above += [0]
+
+        return descriptors_below + descriptors_above + \
+            [ef,
+             H.e_band/num_atoms,
+             H.e_coulomb/num_atoms,
+             H.e_entropy/num_atoms,
+             H.e_external/num_atoms,
+             H.e_kinetic/num_atoms,
+             H.e_kinetic0/num_atoms,
+             H.e_xc/num_atoms,
+             H.e_total_free/num_atoms]
+
+    def describe(self):
+
+        structure = self.structure()
+
+        a = Atoms(pbc=True, cell=structure.lattice.matrix,
+                  positions=structure.cart_coords, numbers=structure.atomic_numbers)
+
+        d_pristine = []
+        try:
+            if self.calculation_type == 'bulk':
+                niggli_reduce(a)
+            self.fix_psuedo(a)
+            d_pristine = self.get_descriptors_for_structure(a)
+
+        except Exception as e:
+            print('Problem in GPAW')
+        if len(d_pristine) > 0:
+            return d_pristine
+        else:
+            return []
```

### Comparing `oganesson-0.1.3/oganesson/descriptors/symmetry_functions.py` & `oganesson-0.1.4/oganesson/descriptors/symmetry_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from ase import Atoms
 from pymatgen.core import Structure
-from pymatgen.io.cif import CifParser
 import numpy as np
-from oganesson.descriptors import Descriptors
+from oganesson.descriptors.descriptors import Descriptors
 from oganesson.ogstructure import OgStructure
+from typing import Union
 
-class SymmetryFunctions(Descriptors):
-    def __init__(self, structure: Atoms | Structure | str | OgStructure) -> None:
+class _SymmetryFunctions(Descriptors):
+    def __init__(self, structure: Union[Atoms, Structure, str, OgStructure]) -> None:
         super().__init__(structure)
 
     @staticmethod
     def fc(Rij, iRc, fRc):
         if Rij <= fRc and Rij > iRc:
             return 1
         else:
```

### Comparing `oganesson-0.1.3/oganesson/genetic_algorithms/__init__.py` & `oganesson-0.1.4/oganesson/genetic_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.3/oganesson/utilities/__init__.py` & `oganesson-0.1.4/oganesson/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.3/oganesson/utilities/atomic_data.py` & `oganesson-0.1.4/oganesson/utilities/atomic_data.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.3/oganesson/utilities/bonds_dictionary.py` & `oganesson-0.1.4/oganesson/utilities/bonds_dictionary.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.3/oganesson.egg-info/PKG-INFO` & `oganesson-0.1.4/oganesson.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.3
+Version: 0.1.4
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
 Keywords: ai,machine learning
 Description-Content-Type: text/markdown
@@ -26,27 +26,29 @@
 # Features
 
 `og` is currently under active development. The following features are currently available.
 
 
 ## Machine learning descriptors
 
-`og` will bring together machine learning descriptors for materials and molecules. At the moment, the three descriptors available are those introduced in this [publication](https://doi.org/10.1186/s13321-022-00658-9). 
+`og` will bring together machine learning descriptors for materials and molecules within a unified framework. `og` currently provides the following descriptors:
+
+- The BACD, ROSA and SymmetryFunctions introduced in this [publication](https://doi.org/10.1186/s13321-022-00658-9)
+- Most of the descriptors from [DScribe](https://github.com/SINGROUP/dscribe)
 
 Each descriptor has its own class, which extends the `Descriptors` class in the `oganesson.descriptors` module. Here is an example of how to describe a structure using the `BACD` and `SymmetryFunctions` descriptor classes.
 
 ```python
-from oganesson.descriptors.bacd import BACD
-from oganesson.descriptors.symmetry_functions import SymmetryFunctions
+from oganesson.descriptors import BACD, SymmetryFunctions
 from oganesson.ogstructure import OgStructure
 
-bacd = BACD(OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif'))
+bacd = BACD(OgStructure(file_name='examples/structures/Li3PO4_mp-13725.cif'))
 print(bacd.describe())
 
-sf = SymmetryFunctions(OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif'))
+sf = SymmetryFunctions(OgStructure(file_name='examples/structures/Li3PO4_mp-13725.cif'))
 print(sf.describe())
 ```
 
 ## Genetic algorithms
 
 The main purpose of `og` is to make complex artificial intelligence workflows easy to compose. Here is an example: running a genetic search for structures, where the structure optimization is performed using the M3GNET neural network model.
 
@@ -57,12 +59,23 @@
     ga.evolve()
 ```
 
 ## Generation of the diffusion path for NEB calculations
 
 The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and then write the POSCAR image files in each of these folders.
 
+In the following example, we explore the possible Li diffusion paths in Li3PO4, given there are 6 Li atoms in the cell.
+
 ```python
 from oganesson.ogstructure import OgStructure
-og = OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif')
+og = OgStructure(file_name='examples/structures/Li3PO4_mp-13725.cif')
 og.generate_neb('Li')
 ```
+Note that the default value of `r`, which is 3, is sufficient for lithium systems. However, for the case of larger atoms such as Na, a larger value of `r` would be required.
+
+## Finding a reasonable adsorption site of an atom on a surface
+
+```python
+from oganesson.ogstructure import OgStructure
+og=OgStructure(file_name='examples/structures/MoS2.vasp')
+og.add_atom_to_surface('Li').structure.to('MoS2_Li.vasp','poscar')
+```
```

### Comparing `oganesson-0.1.3/oganesson.egg-info/SOURCES.txt` & `oganesson-0.1.4/oganesson.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 .gitattributes
+.gitignore
 CHANGELOG.md
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+assets/logo.svg
 oganesson/VERSION
 oganesson/__init__.py
 oganesson/__main__.py
 oganesson/cli.py
 oganesson/ogai.py
 oganesson/ogstructure.py
 oganesson/version.py
 oganesson.egg-info/PKG-INFO
 oganesson.egg-info/SOURCES.txt
 oganesson.egg-info/dependency_links.txt
 oganesson.egg-info/entry_points.txt
 oganesson.egg-info/requires.txt
 oganesson.egg-info/top_level.txt
+oganesson/dataset/vasp.py
 oganesson/descriptors/__init__.py
 oganesson/descriptors/bacd.py
+oganesson/descriptors/descriptors.py
+oganesson/descriptors/dscribe.py
 oganesson/descriptors/rosa.py
 oganesson/descriptors/symmetry_functions.py
 oganesson/genetic_algorithms/__init__.py
+oganesson/reinforcement_learning/m3gnet.py
 oganesson/utilities/__init__.py
 oganesson/utilities/atomic_data.py
 oganesson/utilities/bonds_dictionary.py
```

### Comparing `oganesson-0.1.3/setup.py` & `oganesson-0.1.4/setup.py`

 * *Files identical despite different names*

