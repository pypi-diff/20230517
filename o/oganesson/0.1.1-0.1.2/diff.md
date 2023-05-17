# Comparing `tmp/oganesson-0.1.1.tar.gz` & `tmp/oganesson-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oganesson-0.1.1.tar", last modified: Tue May 16 06:40:57 2023, max compression
+gzip compressed data, was "oganesson-0.1.2.tar", last modified: Wed May 17 00:04:44 2023, max compression
```

## Comparing `oganesson-0.1.1.tar` & `oganesson-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.316781 oganesson-0.1.1/
--rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.1/.gitattributes
--rw-rw-rw-   0        0        0      191 2023-05-16 04:21:08.000000 oganesson-0.1.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2688 2023-05-16 06:40:57.315784 oganesson-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2235 2023-05-16 06:38:06.000000 oganesson-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.294468 oganesson-0.1.1/oganesson/
--rw-rw-rw-   0        0        0        5 2023-05-16 03:18:39.000000 oganesson-0.1.1/oganesson/VERSION
--rw-rw-rw-   0        0        0       74 2023-05-09 00:52:11.000000 oganesson-0.1.1/oganesson/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.1/oganesson/__main__.py
--rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.1/oganesson/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.310782 oganesson-0.1.1/oganesson/descriptors/
--rw-rw-rw-   0        0        0     1226 2023-05-16 04:44:12.000000 oganesson-0.1.1/oganesson/descriptors/__init__.py
--rw-rw-rw-   0        0        0     7896 2023-05-11 01:10:06.000000 oganesson-0.1.1/oganesson/descriptors/bacd.py
--rw-rw-rw-   0        0        0     3646 2023-05-16 03:55:37.000000 oganesson-0.1.1/oganesson/descriptors/rosa.py
--rw-rw-rw-   0        0        0     2801 2023-05-16 03:55:40.000000 oganesson-0.1.1/oganesson/descriptors/symmetry_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.311785 oganesson-0.1.1/oganesson/genetic_algorithms/
--rw-rw-rw-   0        0        0     7642 2023-05-16 06:10:22.000000 oganesson-0.1.1/oganesson/genetic_algorithms/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.1/oganesson/ogai.py
--rw-rw-rw-   0        0        0     6700 2023-05-16 04:38:44.000000 oganesson-0.1.1/oganesson/ogstructure.py
-drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.314799 oganesson-0.1.1/oganesson/utilities/
--rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.1/oganesson/utilities/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.1/oganesson/utilities/atomic_data.py
--rw-rw-rw-   0        0        0   405452 2023-05-16 02:56:53.000000 oganesson-0.1.1/oganesson/utilities/bonds_dictionary.py
--rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.1/oganesson/version.py
-drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.307351 oganesson-0.1.1/oganesson.egg-info/
--rw-rw-rw-   0        0        0     2688 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 06:40:57.316781 oganesson-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1046 2023-05-09 00:58:18.000000 oganesson-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.171761 oganesson-0.1.2/
+-rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.2/.gitattributes
+-rw-rw-rw-   0        0        0      297 2023-05-17 00:04:16.000000 oganesson-0.1.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2692 2023-05-17 00:04:44.170752 oganesson-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2239 2023-05-16 07:00:01.000000 oganesson-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.104276 oganesson-0.1.2/oganesson/
+-rw-rw-rw-   0        0        0        5 2023-05-17 00:04:16.000000 oganesson-0.1.2/oganesson/VERSION
+-rw-rw-rw-   0        0        0       74 2023-05-09 00:52:11.000000 oganesson-0.1.2/oganesson/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.2/oganesson/__main__.py
+-rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.2/oganesson/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.146719 oganesson-0.1.2/oganesson/descriptors/
+-rw-rw-rw-   0        0        0     1226 2023-05-16 04:44:12.000000 oganesson-0.1.2/oganesson/descriptors/__init__.py
+-rw-rw-rw-   0        0        0     7896 2023-05-11 01:10:06.000000 oganesson-0.1.2/oganesson/descriptors/bacd.py
+-rw-rw-rw-   0        0        0       29 2023-05-17 00:02:20.000000 oganesson-0.1.2/oganesson/descriptors/gpaw.py
+-rw-rw-rw-   0        0        0     3646 2023-05-16 23:54:40.000000 oganesson-0.1.2/oganesson/descriptors/rosa.py
+-rw-rw-rw-   0        0        0     2801 2023-05-16 03:55:40.000000 oganesson-0.1.2/oganesson/descriptors/symmetry_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.148227 oganesson-0.1.2/oganesson/genetic_algorithms/
+-rw-rw-rw-   0        0        0     7853 2023-05-17 00:02:20.000000 oganesson-0.1.2/oganesson/genetic_algorithms/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.2/oganesson/ogai.py
+-rw-rw-rw-   0        0        0     6700 2023-05-16 04:38:44.000000 oganesson-0.1.2/oganesson/ogstructure.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.168748 oganesson-0.1.2/oganesson/utilities/
+-rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.2/oganesson/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.2/oganesson/utilities/atomic_data.py
+-rw-rw-rw-   0        0        0   405452 2023-05-16 02:56:53.000000 oganesson-0.1.2/oganesson/utilities/bonds_dictionary.py
+-rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.2/oganesson/version.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.122273 oganesson-0.1.2/oganesson.egg-info/
+-rw-rw-rw-   0        0        0     2692 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       44 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 00:04:44.171761 oganesson-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-05-17 00:02:20.000000 oganesson-0.1.2/setup.py
```

### Comparing `oganesson-0.1.1/CONTRIBUTING.rst` & `oganesson-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/LICENSE` & `oganesson-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/PKG-INFO` & `oganesson-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.1
+Version: 0.1.2
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
 Keywords: ai,machine learning,model testing
 Description-Content-Type: text/markdown
@@ -55,14 +55,14 @@
 ga = GA(['Na']*4 + ['H']*4)
 for i in range(10):
     ga.evolve()
 ```
 
 ## Generation of the diffusion path for NEB calculations
 
-The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and writes the POSCAR image files in each of these folders.
+The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and then write the POSCAR image files in each of these folders.
 
 ```python
 from oganesson.ogstructure import OgStructure
 og = OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif')
 og.generate_neb('Li')
 ```
```

### Comparing `oganesson-0.1.1/README.md` & `oganesson-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,14 @@
 ga = GA(['Na']*4 + ['H']*4)
 for i in range(10):
     ga.evolve()
 ```
 
 ## Generation of the diffusion path for NEB calculations
 
-The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and writes the POSCAR image files in each of these folders.
+The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and then write the POSCAR image files in each of these folders.
 
 ```python
 from oganesson.ogstructure import OgStructure
 og = OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif')
 og.generate_neb('Li')
 ```
```

### Comparing `oganesson-0.1.1/oganesson/cli.py` & `oganesson-0.1.2/oganesson/cli.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/oganesson/descriptors/__init__.py` & `oganesson-0.1.2/oganesson/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/oganesson/descriptors/bacd.py` & `oganesson-0.1.2/oganesson/descriptors/bacd.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/oganesson/descriptors/rosa.py` & `oganesson-0.1.2/oganesson/descriptors/rosa.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/oganesson/descriptors/symmetry_functions.py` & `oganesson-0.1.2/oganesson/descriptors/symmetry_functions.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/oganesson/genetic_algorithms/__init__.py` & `oganesson-0.1.2/oganesson/genetic_algorithms/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,169 +4,170 @@
 from ase.ga.population import Population
 from ase.ga.utilities import closest_distances_generator, CellBounds
 from ase.ga.ofp_comparator import OFPComparator
 from ase.ga.offspring_creator import OperationSelector
 from ase.ga.standardmutations import StrainMutation
 from ase.ga.soft_mutation import SoftMutation
 from ase.ga.cutandsplicepairing import CutAndSplicePairing
-
 from ase import Atoms
 from ase.data import atomic_numbers
-from ase.ga.utilities import closest_distances_generator, CellBounds
 from ase.ga.startgenerator import StartGenerator
 from ase.ga.data import PrepareDB
-from ase.build import niggli_reduce
-from ase.calculators.singlepoint import SinglePointCalculator
-from ase.optimize import FIRE
-from ase.constraints import ExpCellFilter
 from ase.ga import set_raw_score
 from m3gnet.models import Relaxer
 from oganesson.ogstructure import OgStructure
 import os
-        
+
+
 class GA:
     def finalize(self, atoms, energy):
         raw_score = -energy
         set_raw_score(atoms, raw_score)
 
     def relax(self, atoms, cellbounds=None):
         relaxer = Relaxer()
         structure = OgStructure.ase_to_pymatgen(atoms)
         relax_results = relaxer.relax(structure, verbose=True)
 
         e = float(relax_results['trajectory'].energies[-1])
         self.finalize(atoms, energy=e)
         return OgStructure.pymatgen_to_ase(relax_results['final_structure'])
 
-    def __init__(self,blocks,population_size=20,box_volume=240) -> None:
-        pass
+    def __init__(self, blocks, population_size=20, box_volume=240,
+                 a: list = [3, 10], b: list = [3, 10], c: list = [3, 10],
+                 phi: list = [35, 145], chi: list = [35, 145], psi: list = [35, 145]) -> None:
         self.N = population_size
         self.volume = box_volume
         self.blocks = blocks
         self.Z = [atomic_numbers[x] for x in self.blocks]
 
         self.blmin = closest_distances_generator(atom_numbers=self.Z,
-                                            ratio_of_covalent_radii=0.6)
-        self.cellbounds = CellBounds(bounds={'phi': [35, 145], 'chi': [35, 145],
-                                        'psi': [35, 145], 'a': [3, 10],
-                                        'b': [3, 10], 'c': [3, 10]})
+                                                 ratio_of_covalent_radii=0.6)
+        self.cellbounds = CellBounds(bounds={'phi': phi, 'chi': chi,
+                                             'psi': psi, 'a': a,
+                                             'b': b, 'c': c})
 
         self.splits = {(2,): 1, (1,): 1}
         self.slab = Atoms('', pbc=True)
 
         self.sg = StartGenerator(self.slab, self.blocks, self.blmin, box_volume=self.volume,
-                            number_of_variable_cell_vectors=3,
-                            cellbounds=self.cellbounds, splits=self.splits)
+                                 number_of_variable_cell_vectors=3,
+                                 cellbounds=self.cellbounds, splits=self.splits)
 
         # Create the database
-
         self.database = PrepareDB(db_file_name='gadb.db',
-                    stoichiometry=self.Z)
+                                  stoichiometry=self.Z)
 
         # Generate N random structures
         # and add them to the database
         for i in range(self.N):
             a = self.sg.get_new_candidate()
             self.database.add_unrelaxed_candidate(a)
 
-        
         # Connect to the database and retrieve some information
         self.database_connection = DataConnection('gadb.db')
         self.slab = self.database_connection.get_slab()
         atom_numbers_to_optimize = self.database_connection.get_atom_numbers_to_optimize()
         self.n_top = len(atom_numbers_to_optimize)
 
         self.comp = OFPComparator(n_top=self.n_top, dE=1.0,
-                            cos_dist_max=1e-3, rcut=10., binwidth=0.05,
-                            pbc=[True, True, True], sigma=0.05, nsigma=4,
-                            recalculate=False)
+                                  cos_dist_max=1e-3, rcut=10., binwidth=0.05,
+                                  pbc=[True, True, True], sigma=0.05, nsigma=4,
+                                  recalculate=False)
 
         self.pairing = CutAndSplicePairing(self.slab, self.n_top, self.blmin, p1=1., p2=0., minfrac=0.15,
-                                    number_of_variable_cell_vectors=3,
-                                    cellbounds=self.cellbounds, use_tags=False)
+                                           number_of_variable_cell_vectors=3,
+                                           cellbounds=self.cellbounds, use_tags=False)
 
         self.strainmut = StrainMutation(self.blmin, stddev=0.7, cellbounds=self.cellbounds,
-                                number_of_variable_cell_vectors=3,
-                                use_tags=False)
-        self.blmin_soft = closest_distances_generator(atom_numbers_to_optimize, 0.1)
-        self.softmut = SoftMutation(self.blmin_soft, bounds=[2., 5.], use_tags=False)
+                                        number_of_variable_cell_vectors=3,
+                                        use_tags=False)
+        self.blmin_soft = closest_distances_generator(
+            atom_numbers_to_optimize, 0.1)
+        self.softmut = SoftMutation(self.blmin_soft, bounds=[
+                                    2., 5.], use_tags=False)
         self.operators = OperationSelector([4., 3., 3.],
-                                    [self.pairing, self.softmut, self.strainmut])
-
-        self.path = 'relaxed/'
+                                           [self.pairing, self.softmut, self.strainmut])
+        import uuid
+        self.path = 'run_'+uuid.uuid4().hex
         if not os.path.isdir(self.path):
             os.mkdir(self.path)
 
+        self.path_relaxed = self.path + '/relaxed/'
+        if not os.path.isdir(self.path_relaxed):
+            os.mkdir(self.path_relaxed)
+
         # Relax the initial candidates
         while self.database_connection.get_number_of_unrelaxed_candidates() > 0:
             a = self.database_connection.get_an_unrelaxed_candidate()
 
             relaxed_a = self.relax(a, cellbounds=self.cellbounds)
             a.positions = relaxed_a.positions
             a.cell = relaxed_a.cell
             a.pbc = True
             self.database_connection.add_relaxed_step(a)
-            
+
             cell = a.get_cell()
             if not self.cellbounds.is_within_bounds(cell):
                 self.database_connection.kill_candidate(a.info['confid'])
             else:
-                relaxed_a.write(self.path+str(a.info['confid'])+'.cif','cif')
+                relaxed_a.write(self.path_relaxed+str(a.info['confid'])+'.cif', 'cif')
 
     def evolve(self, num_offsprings=20):
-        # Initialize the population
         self.population = Population(data_connection=self.database_connection,
-                                population_size=self.N,
-                                comparator=self.comp,
-                                logfile='log.txt',
-                                use_extinct=True)
-
+                                     population_size=self.N,
+                                     comparator=self.comp,
+                                     logfile='log.txt',
+                                     use_extinct=True)
 
         current_pop = self.population.get_current_population()
-        self.strainmut.update_scaling_volume(current_pop, w_adapt=0.5, n_adapt=4)
+        self.strainmut.update_scaling_volume(
+            current_pop, w_adapt=0.5, n_adapt=4)
         self.pairing.update_scaling_volume(current_pop, w_adapt=0.5, n_adapt=4)
 
         for step in range(num_offsprings):
             print('Now starting configuration number {0}'.format(step))
 
             a3 = None
             while a3 is None:
                 a1, a2 = self.population.get_two_candidates()
                 a3, desc = self.operators.get_new_individual([a1, a2])
 
             # Save the unrelaxed candidate
-            self.database_connection.add_unrelaxed_candidate(a3, description=desc)
+            self.database_connection.add_unrelaxed_candidate(
+                a3, description=desc)
 
             # Relax the new candidate and save it
             relaxed_a = self.relax(a3, cellbounds=self.cellbounds)
             a3.positions = relaxed_a.positions
             a3.cell = relaxed_a.cell
             a3.pbc = True
             self.database_connection.add_relaxed_step(a3)
 
             # If the relaxation has changed the cell parameters
             # beyond the bounds we disregard it in the population
             cell = a3.get_cell()
             if not self.cellbounds.is_within_bounds(cell):
                 self.database_connection.kill_candidate(a3.info['confid'])
             else:
-                a3.write(self.path+str(a3.info['confid'])+'.cif','cif')
-            
+                a3.write(self.path_relaxed+str(a3.info['confid'])+'.cif', 'cif')
+
             # Update the population
             self.population.update()
 
             if step % 10 == 0:
                 current_pop = self.population.get_current_population()
                 self.strainmut.update_scaling_volume(current_pop, w_adapt=0.5,
-                                                n_adapt=4)
-                self.pairing.update_scaling_volume(current_pop, w_adapt=0.5, n_adapt=4)
+                                                     n_adapt=4)
+                self.pairing.update_scaling_volume(
+                    current_pop, w_adapt=0.5, n_adapt=4)
                 write('current_population.traj', current_pop)
 
         print('GA finished after step %d' % step)
         hiscore = get_raw_score(current_pop[0])
         print('Highest raw score = %8.4f eV' % hiscore)
 
         all_candidates = self.database_connection.get_all_relaxed_candidates()
         write('all_candidates.traj', all_candidates)
 
         current_pop = self.population.get_current_population()
-        write('current_population.traj', current_pop)
+        write('current_population.traj', current_pop)
```

### Comparing `oganesson-0.1.1/oganesson/ogstructure.py` & `oganesson-0.1.2/oganesson/ogstructure.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/oganesson/utilities/__init__.py` & `oganesson-0.1.2/oganesson/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/oganesson/utilities/atomic_data.py` & `oganesson-0.1.2/oganesson/utilities/atomic_data.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/oganesson/utilities/bonds_dictionary.py` & `oganesson-0.1.2/oganesson/utilities/bonds_dictionary.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.1/oganesson.egg-info/PKG-INFO` & `oganesson-0.1.2/oganesson.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.1
+Version: 0.1.2
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
 Keywords: ai,machine learning,model testing
 Description-Content-Type: text/markdown
@@ -55,14 +55,14 @@
 ga = GA(['Na']*4 + ['H']*4)
 for i in range(10):
     ga.evolve()
 ```
 
 ## Generation of the diffusion path for NEB calculations
 
-The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and writes the POSCAR image files in each of these folders.
+The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and then write the POSCAR image files in each of these folders.
 
 ```python
 from oganesson.ogstructure import OgStructure
 og = OgStructure(file_name='examples/structures/mp-541001_LiInI4.cif')
 og.generate_neb('Li')
 ```
```

### Comparing `oganesson-0.1.1/oganesson.egg-info/SOURCES.txt` & `oganesson-0.1.2/oganesson.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,13 +16,14 @@
 oganesson.egg-info/SOURCES.txt
 oganesson.egg-info/dependency_links.txt
 oganesson.egg-info/entry_points.txt
 oganesson.egg-info/requires.txt
 oganesson.egg-info/top_level.txt
 oganesson/descriptors/__init__.py
 oganesson/descriptors/bacd.py
+oganesson/descriptors/gpaw.py
 oganesson/descriptors/rosa.py
 oganesson/descriptors/symmetry_functions.py
 oganesson/genetic_algorithms/__init__.py
 oganesson/utilities/__init__.py
 oganesson/utilities/atomic_data.py
 oganesson/utilities/bonds_dictionary.py
```

### Comparing `oganesson-0.1.1/setup.py` & `oganesson-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,12 +19,16 @@
     long_description=README,
     long_description_content_type='text/markdown',
     author='Sherif Abdulkader Tawfik Abbas',
     author_email='sherif.tawfic@gmail.com',
     url='https://github.com/oganesson-ai/oganesson',
     keywords=['ai', 'machine learning',
               'model testing'],
-    install_requires=['xgboost',
+    install_requires=['ase',
                       'pandas',
-                      'numpy'],
+                      'numpy',
+                      'm3gnet',
+                      'pymatgen'
+                      'm3gnet',
+                      'gpaw'],
 
 )
```

