# Comparing `tmp/OncoAMBER-1.2.8.tar.gz` & `tmp/OncoAMBER-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.2.8.tar", last modified: Thu May 11 15:40:22 2023, max compression
+gzip compressed data, was "OncoAMBER-1.3.3.tar", last modified: Wed May 17 19:38:55 2023, max compression
```

## Comparing `OncoAMBER-1.2.8.tar` & `OncoAMBER-1.3.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:40:22.106850 OncoAMBER-1.2.8/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:40:22.014578 OncoAMBER-1.2.8/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-11 15:40:21.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-11 15:40:22.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-11 15:40:21.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-11 15:40:21.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-11 15:40:21.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-11 15:40:22.106468 OncoAMBER-1.2.8/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.8/README.md
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:40:22.104848 OncoAMBER-1.2.8/amber/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.8/amber/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.8/amber/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     2066 2023-05-09 16:56:51.000000 OncoAMBER-1.2.8/amber/Cell.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    22865 2023-05-11 15:06:44.000000 OncoAMBER-1.2.8/amber/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.8/amber/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.8/amber/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.8/amber/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    15144 2023-05-09 14:51:38.000000 OncoAMBER-1.2.8/amber/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5702 2023-05-10 21:23:03.000000 OncoAMBER-1.2.8/amber/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    26555 2023-05-10 22:10:54.000000 OncoAMBER-1.2.8/amber/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      332 2023-05-11 15:40:19.000000 OncoAMBER-1.2.8/amber/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.8/amber/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.8/amber/save_alpha_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.8/amber/save_beta_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-11 15:40:22.106951 OncoAMBER-1.2.8/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     3118 2023-05-11 15:40:19.000000 OncoAMBER-1.2.8/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-17 19:38:55.299062 OncoAMBER-1.3.3/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-17 19:38:55.075130 OncoAMBER-1.3.3/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5403 2023-05-17 19:38:55.000000 OncoAMBER-1.3.3/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      651 2023-05-17 19:38:55.000000 OncoAMBER-1.3.3/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-17 19:38:55.000000 OncoAMBER-1.3.3/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.3.3/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-17 19:38:55.000000 OncoAMBER-1.3.3/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-17 19:38:55.000000 OncoAMBER-1.3.3/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5403 2023-05-17 19:38:55.298679 OncoAMBER-1.3.3/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     4648 2023-05-11 18:02:47.000000 OncoAMBER-1.3.3/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-17 19:38:55.297012 OncoAMBER-1.3.3/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.3.3/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5936 2023-05-15 17:20:06.000000 OncoAMBER-1.3.3/amber/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2066 2023-05-09 16:56:51.000000 OncoAMBER-1.3.3/amber/Cell.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    23103 2023-05-17 19:24:06.000000 OncoAMBER-1.3.3/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.3.3/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.3.3/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.3.3/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    15144 2023-05-09 14:51:38.000000 OncoAMBER-1.3.3/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5695 2023-05-16 13:38:38.000000 OncoAMBER-1.3.3/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    28303 2023-05-17 19:21:59.000000 OncoAMBER-1.3.3/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      332 2023-05-17 19:38:35.000000 OncoAMBER-1.3.3/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.3.3/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17103 2023-05-12 22:54:55.000000 OncoAMBER-1.3.3/amber/save_alpha_dataframe2.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.3.3/amber/save_alpha_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17083 2023-05-12 22:54:55.000000 OncoAMBER-1.3.3/amber/save_beta_dataframe2.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.3.3/amber/save_beta_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-17 19:38:55.299155 OncoAMBER-1.3.3/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3118 2023-05-11 15:40:19.000000 OncoAMBER-1.3.3/setup.py
```

### Comparing `OncoAMBER-1.2.8/OncoAMBER.egg-info/SOURCES.txt` & `OncoAMBER-1.3.3/OncoAMBER.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -16,12 +16,14 @@
 amber/Vessel.py
 amber/Voxel.py
 amber/World.py
 amber/__init__.py
 amber/cell.py
 amber/config.py
 amber/process.py
+amber/save_alpha_dataframe2.csv
 amber/save_alpha_dataframe6.csv
+amber/save_beta_dataframe2.csv
 amber/save_beta_dataframe6.csv
 amber/vessel.py
 amber/voxel.py
 amber/world.py
```

### Comparing `OncoAMBER-1.2.8/amber/BasicGeometries.py` & `OncoAMBER-1.3.3/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.8/amber/BetaDistributionCalibration.py` & `OncoAMBER-1.3.3/amber/BetaDistributionCalibration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import numpy as np
-#from scipy.stats import qmc
 import matplotlib.pyplot as plt
 from scipy.stats import beta
-from scipy.optimize import curve_fit
-from mpl_toolkits.mplot3d import Axes3D
 import pandas as pd
 import seaborn as sns
 
 class Vessel:
-    def __init__(self, origin, radius):
+    def __init__(self, origin, radius, length):
         self.origin = (origin[0], origin[1], 0)
-        self.end = (origin[0], origin[1], side)
+        self.end = (origin[0], origin[1], length)
         self.radius = radius
 
     def closest_distance(self, point):
 
         # Compute the direction vector of the vessel segment
         vessel_dir = (self.end[0] - self.origin[0], self.end[1] - self.origin[1], self.end[2] - self.origin[2])
 
@@ -73,15 +70,15 @@
                 # points_y = sampler.random(n)[:,1] * side
                 points_x = np.random.uniform(0, side, n) #pseudo random
                 points_y = np.random.uniform(0, side, n)
 
 
                 vessels = []
                 for i in range(len(points_x)):
-                    vessels.append(Vessel([points_x[i], points_y[i]], radius))
+                    vessels.append(Vessel([points_x[i], points_y[i]], radius, side))
 
                 points = []
                 for i in range(5000):
                     point = [np.random.uniform(0, side), np.random.uniform(0, side), np.random.uniform(0, side)]
                     distances = []
                     for vessel in vessels:
                         distances.append(vessel.closest_distance(point))
@@ -138,9 +135,7 @@
 
     sns.heatmap(alpha_dataframe, cmap='viridis')
     plt.show()
 
     sns.heatmap(beta_dataframe, cmap='viridis')
     plt.show()
 
-
-
```

### Comparing `OncoAMBER-1.2.8/amber/Cell.py` & `OncoAMBER-1.3.3/amber/Cell.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.8/amber/Process.py` & `OncoAMBER-1.3.3/amber/Process.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     def __init__(self, config, list_of_process : list, finish_time, dt):
         self.list_of_process = list_of_process
         self.finish_time = finish_time
         self.dt = dt
         self.time = 0
         self.config = config
-    def show_cell_and_tumor_volume(self, number_tumor_cells, number_necrotic_cells, number_quiescent_cells, number_cycling_cells, tumor_size, times):
+    def show_cell_and_tumor_volume(self, number_tumor_cells, number_necrotic_cells, number_quiescent_cells, number_cycling_cells, tumor_size, tumor_size_free, times):
         # plot number of cells evolution
         plt.plot(times, number_tumor_cells, 'blue', label='All cells')
         plt.plot(times, number_cycling_cells, 'red', label='Cycling cells')
         plt.plot(times, number_quiescent_cells, 'green', label='Quiescent cells')
         plt.plot(times, number_necrotic_cells, 'black', label='Necrotic cells')
         plt.title('Number of cells evolution')
         plt.xlabel('Time')
@@ -29,14 +29,15 @@
         plt.legend()
         plt.savefig('Plots/Number_cells_evolution.png')
         plt.show()
 
         # plot tumor size evolution
         fig = plt.figure()
         plt.plot(times, tumor_size, 'red')
+        plt.plot(times, tumor_size_free, 'blue')
         plt.title('Tumor volume evolution')
         plt.xlabel('Time')
         plt.ylabel('Tumor volume [mm^3]')
         plt.grid(True)
         plt.savefig('Plots/Tumor_size_evolution.png')
         plt.show()
     def show(self, world: World, t = 0): #this function is used to show the world at a certain time
@@ -125,16 +126,16 @@
         process_local = [process for process in self.list_of_process if not process.is_global]
         process_global = [process for process in self.list_of_process if process.is_global]
 
         irradiations_times = [self.config.first_irradiation_time + i * self.config.time_between_fractions for i in
                               range(self.config.number_fractions)]
         applied_fractions = 0
 
-        number_cycling_cells = []; number_quiescent_cells = []; number_necrotic_cells = []; tumor_size = []; times = [];
-        number_tumor_cells = []
+        number_cycling_cells = []; number_quiescent_cells = []; number_necrotic_cells = [];
+        tumor_size = []; tumor_size_free = []; times = []; number_tumor_cells = []
 
         while self.time < self.finish_time:
             print(f'\033[1;31;47mTime: {self.time} hours / {self.finish_time} hours\033[0m')
             if video:
                 self.show(world, self.time)
 
             if applied_fractions < self.config.number_fractions and self.time >= irradiations_times[applied_fractions]:
@@ -162,30 +163,32 @@
                         else:
                             quiescent_cells += 1
 
             number_cycling_cells.append(cycling_cells)
             number_quiescent_cells.append(quiescent_cells)
             number_necrotic_cells.append(necrotic_cells)
             number_tumor_cells.append(cycling_cells + quiescent_cells + necrotic_cells)
-            tumor_size_ = world.measure_tumor_volume()
+            tumor_size_, tumor_size_free_ = world.measure_tumor_volume()
             tumor_size.append(tumor_size_)
+            tumor_size_free.append(tumor_size_free_)
             times.append(self.time)
 
             if not os.path.exists('DataOutput/'):
                 os.makedirs('DataOutput/')
 
             np.save('DataOutput/number_tumor_cells.npy', number_tumor_cells)
             np.save('DataOutput/number_necrotic_cells.npy', number_necrotic_cells)
             np.save('DataOutput/number_cycling_cells.npy', number_cycling_cells)
             np.save('DataOutput/number_quiescent_cells.npy', number_quiescent_cells)
             np.save('DataOutput/tumor_size.npy', tumor_size)
+            np.save('DataOutput/tumor_size_free.npy', tumor_size_free)
             np.save('DataOutput/times.npy', times)
 
             if self.config.show_cell_and_tumor_volume:
-                self.show_cell_and_tumor_volume(number_tumor_cells, number_necrotic_cells, number_quiescent_cells, number_cycling_cells, tumor_size, times)
+                self.show_cell_and_tumor_volume(number_tumor_cells, number_necrotic_cells, number_quiescent_cells, number_cycling_cells, tumor_size, tumor_size_free, times)
 
             self.time += self.dt
 
         print('Simulation finished')
 
         if self.config.show_final:
             self.show(world, self.time)
@@ -215,15 +218,15 @@
                 if cell.time_spent_cycling >= cell.doubling_time:
                     time_diff = cell.time_spent_cycling - cell.doubling_time
                     leftover_time = self.dt - time_diff
                     new_cell = cell.duplicate() #create a new cell (start cycling at 0)
                     new_cell.time_spent_cycling = leftover_time #reset the time spent cycling
                     cell.doubling_time = cell.random_doubling_time() #sample a new doubling time for the old cell
                     cell.time_spent_cycling = leftover_time #reset the time spent cycling
-                    voxel.add_cell(new_cell) #add the new cell to the voxel
+                    voxel.add_cell(new_cell, self.config.max_occupancy) #add the new cell to the voxel
         return
 
 class CellDeath(Process): #cell necrosis process, cells die in a voxel if they have too low vitality
     def __init__(self, config, name, dt, necrosis_threshold, necrosis_probability, apoptosis_threshold, apoptosis_probability):
         super().__init__(config, 'CellNecrosis', dt)
         self.necrosis_threshold = necrosis_threshold
         self.necrosis_probability = necrosis_probability
@@ -247,23 +250,26 @@
 
 
     def __call__(self, voxel):
         for cell in voxel.list_of_cells:
             vitality = cell.vitality()
             if vitality < self.apoptosis_threshold:
                 sample = np.random.uniform(0, 1)
+                print('apoptosis:', self.apoptosis_curve(vitality))
                 p_necro = (1 - ((1-self.necrosis_curve(vitality))**self.dt))
                 p_apopt = (1 - ((1-self.apoptosis_curve(vitality))**self.dt))
+                print(p_apopt)
                 if self.config.verbose: print('probability necro:', p_necro, 'probability apopto:', p_apopt)
                 n = p_necro
                 a = p_necro + p_apopt
                 if sample < n:
                     #necrosis
                     voxel.cell_becomes_necrotic(cell)
                 elif sample < a:
+                    print('apoptosis!!')
                     #apoptosis
                     voxel.remove_cell(cell)
 
 
 class CellAging(Process): #cell aging process, cells age in a voxel
     def __init__(self, config, name, dt):
         super().__init__(config,'CellAging', dt)
@@ -281,40 +287,37 @@
                 n_cell.time_before_death -= self.dt
                 if n_cell.time_before_death < 0:
                     voxel.remove_necrotic_cell(n_cell)
         pass
 
 
 class CellMigration(Process): #cell migration process, cells migrate in the world
-    def __init__(self, config, name, dt, pressure_threshold):
+    def __init__(self, config, name, dt):
         super().__init__(config, 'CellMigration', dt)
         self.is_global = True #run on the whole world, after the other processes
-        self.pressure_threshold = pressure_threshold
 
     def __call__(self, world: World):
-        exchange_matrix = world.compute_exchange_matrix(self.dt, pressure_threshold=self.pressure_threshold)
+        exchange_matrix = world.compute_exchange_matrix(self.dt)
         for voxel in world.voxel_list:
             voxel_num = voxel.voxel_number
             if voxel_num % 10000 == 0: print('voxel number = ', voxel_num)
-            list_of_neighbors = world.find_neighbors(voxel)
+            list_of_neighbors = world.find_moor_neighbors(voxel)
             np.random.shuffle(list_of_neighbors) #shuffle the list to avoid bias
             for neighbor in list_of_neighbors:
                 n_events = exchange_matrix[voxel_num, neighbor.voxel_number] #number of expected events in the time step
                 n_moving_cells = np.random.poisson(n_events)
-                n_moving_cells = min(n_moving_cells, int(round(len(voxel.list_of_cells)*0.5)))
+                n_moving_cells = min(n_moving_cells, int(round(len(voxel.list_of_cells))))
                 list_of_moving_cells = np.random.choice(voxel.list_of_cells, n_moving_cells, replace=False)
                 for cell in list_of_moving_cells:
-                    if neighbor.add_cell(cell):
+                    if neighbor.add_cell(cell, self.config.max_occupancy):
                         voxel.remove_cell(cell)
-
 class UpdateCellOxygen(Process):
-    def __init__(self, config, name, dt, voxel_half_length, effective_vessel_radius):
+    def __init__(self, config, name, dt, voxel_half_length):
         super().__init__(config, 'UpdateState', dt)
         self.voxel_side = int(voxel_half_length*20) #um/100
-        self.effective_vessel_radius = effective_vessel_radius
 
         amber_dir = os.path.abspath(os.path.dirname(__file__))
 
         alpha_file_name = 'save_alpha_dataframe' + str(self.voxel_side) + '.csv'
         beta_file_name = 'save_beta_dataframe' + str(self.voxel_side) + '.csv'
         alpha_file_name = os.path.join(amber_dir, alpha_file_name)
         beta_file_name = os.path.join(amber_dir, beta_file_name)
@@ -393,21 +396,21 @@
         for cell in voxel.list_of_cells:
             if cell.vitality() < self.threshold_for_VEGF_production and cell.type == 'TumorCell':
                 VEGF = VEGF + self.VEGF_production_per_cell*(1-cell.vitality())
         VEGF = min(VEGF, 1.0)
         voxel.molecular_factors['VEGF'] = VEGF
         return
 class UpdateVasculature(Process): #update the vasculature
-    def __init__(self, config, name, dt, killing_radius_threshold, killing_length_threshold, o2_per_volume, diffusion_number, splitting_rate, macro_steps, micro_steps, weight_direction, weight_vegf, weight_pressure, radius_pressure_sensitive):
+    def __init__(self, config, name, dt, killing_radius_threshold, killing_length_threshold, o2_per_volume, capillary_length, splitting_rate, macro_steps, micro_steps, weight_direction, weight_vegf, weight_pressure, radius_pressure_sensitive):
         super().__init__(config, 'UpdateVasculature', dt)
         self.is_global = True
         self.killing_radius_threshold = killing_radius_threshold
         self.killing_length_threshold = killing_length_threshold
         self.o2_per_volume = o2_per_volume
-        self.diffusion_number = diffusion_number
+        self.capillary_length = capillary_length
         self.dt = dt
         self.splitting_rate = splitting_rate
         self.macro_steps = macro_steps
         self.micro_steps = micro_steps
         self.weight_direction = weight_direction
         self.weight_vegf = weight_vegf
         self.weight_pressure = weight_pressure
@@ -443,15 +446,15 @@
         #         point = vessel.choose_random_point()
         #         #branch from this point
         #         world.vasculature.branching(vessel.id, point)
 
         world.vasculature_growth(self.dt, self.splitting_rate, self.macro_steps, self.micro_steps, self.weight_direction, self.weight_vegf, self.weight_pressure, self.radius_pressure_sensitive)
         world.update_volume_occupied_by_vessels()
         # world.vasculature.print_vessel_tree()
-        world.update_oxygen(o2_per_volume = self.o2_per_volume, diffusion_number=self.diffusion_number)
+        world.update_oxygen(o2_per_volume = self.o2_per_volume, capillary_length = self.capillary_length)
 
 class Irradiation(Process): #irradiation
     def __init__(self, config, name, dt, topas_file, irradiation_time, irradiation_intensity, world: World):
         super().__init__(config, 'Irradiation', dt)
         self.irradiation_time = irradiation_time
         self.irradiation_intensity = irradiation_intensity
```

### Comparing `OncoAMBER-1.2.8/amber/ReadAndWrite.py` & `OncoAMBER-1.3.3/amber/ReadAndWrite.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.8/amber/ScalarField.py` & `OncoAMBER-1.3.3/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.8/amber/Terminal.py` & `OncoAMBER-1.3.3/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.8/amber/Vessel.py` & `OncoAMBER-1.3.3/amber/Vessel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.8/amber/Voxel.py` & `OncoAMBER-1.3.3/amber/Voxel.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 # pressure = (NkT*ratio)/self.volume
                 return packing_density
 
         def random_points_in_voxel(self, n):
                 points = np.random.uniform(-self.half_length, self.half_length, (n,3))
                 points = points + self.position
                 return points
-        def add_cell(self, cell, max_occupancy = 0.68):
+        def add_cell(self, cell, max_occupancy):
                 if self.pressure() > max_occupancy:
                         #print('Voxel is full, pressure is', self.pressure(), ' number of cells is', self.number_of_alive_cells(), ' and number of necrotic cells is', self.number_of_necrotic_cells())
                         return False
                 else:
                         self.list_of_cells = np.append(cell, self.list_of_cells)
                         return True
```

### Comparing `OncoAMBER-1.2.8/amber/World.py` & `OncoAMBER-1.3.3/amber/World.py`

 * *Files 6% similar despite different names*

```diff
@@ -191,14 +191,35 @@
             return -1
         return n
 
     def find_voxel(self, position):
         voxel_number = self.find_voxel_number(position)
         return self.voxel_list[voxel_number]
 
+    def find_moor_neighbors(self, voxel):
+        # finds the Moore's neighbors of a voxel
+        voxel_number = voxel.voxel_number
+        num_voxels = self.number_of_voxels
+        i = voxel_number // (num_voxels ** 2)
+        j = (voxel_number // num_voxels) % num_voxels
+        k = voxel_number % num_voxels
+
+        neighbors = []
+        for di in [-1, 0, 1]:
+            for dj in [-1, 0, 1]:
+                for dk in [-1, 0, 1]:
+                    if di == 0 and dj == 0 and dk == 0:
+                        continue
+                    if (0 <= i + di < num_voxels) and (0 <= j + dj < num_voxels) and (0 <= k + dk < num_voxels):
+                        neighbors.append((i + di) * num_voxels ** 2 + (j + dj) * num_voxels + (k + dk))
+
+        neighbors_voxels = [self.voxel_list[n] for n in neighbors]
+        return neighbors_voxels
+
+
     def find_neighbors(self, voxel):
         #finds the neighbors of a voxel
         voxel_number = voxel.voxel_number
         num_voxels = self.number_of_voxels
         i = voxel_number // (num_voxels ** 2)
         j = (voxel_number // num_voxels) % num_voxels
         k = voxel_number % num_voxels
@@ -217,47 +238,55 @@
         if k < num_voxels - 1:
             neighbors.append(i * num_voxels ** 2 + j * num_voxels + (k + 1))
 
         neighbors = [n for n in neighbors if 0 <= n < num_voxels ** 3]
         neighbors_voxels = [self.voxel_list[n] for n in neighbors]
         return neighbors_voxels
 
-    def compute_exchange_matrix(self, dt, pressure_threshold):
+    def compute_exchange_matrix(self, dt):
         V = self.voxel_list[0].volume
+        side = self.voxel_list[0].half_length * 2
         total_voxels = self.total_number_of_voxels
         # Extract pressure and viscosity values for all voxels
         pressures = np.array([voxel.pressure() for voxel in self.voxel_list])
         viscosities = np.array([voxel.viscosity for voxel in self.voxel_list])
         # Initialize migration matrix with zeros
         migration_matrix = sparse.lil_matrix((total_voxels, total_voxels), dtype=np.float32)
 
         for i in range(total_voxels):
             voxel_i = self.voxel_list[i]
             voxel_pressure = pressures[i]
             viscosity = viscosities[i]
 
             # Find neighbors of the current voxel
-            neighbors = self.find_neighbors(voxel_i)
-
+            neighbors = self.find_moor_neighbors(voxel_i)
             for neighbor in neighbors:
                 j = neighbor.voxel_number
 
                 pressure_diff = voxel_pressure - pressures[j]
-                if pressure_diff > pressure_threshold:
+                distance = np.linalg.norm(voxel_i.position - neighbor.position)
+                coeff = (side/distance) * dt
+                if pressure_diff > 0:
 
                     t_res = (V / pressure_diff) * viscosity
                     if self.config.verbose:
                         print('V, pressure diff, viscosity ', V, pressure_diff, viscosity)
                         print('t_res = ', t_res)
-                    n_events = dt / t_res
+                    n_events = coeff / t_res
                     migration_matrix[i, j] = n_events
 
+            # pressure pushing cells to move towards the center of the tumor
+            voxel_distance = np.linalg.norm(voxel_i.position)
+            neighbor_towards_center = self.find_voxel_number(voxel_i.position * (1 - side/voxel_distance))
+            migration_matrix[i, neighbor_towards_center] += self.config.pressure_coefficient_central_migration * dt * voxel_distance
         # Convert the lil_matrix to a csr_matrix for faster arithmetic operations
         migration_matrix = migration_matrix.tocsr()
-
+        #show the matrix
+        # plt.spy(migration_matrix)
+        # plt.show()
         return migration_matrix
 
     def topas_param_file(self, name : str):
         print('-- Creating parameter file for topas simulation, file :', name)
         #returns a txt file that can be used as a parameter file for topas
         name = name + '.txt'
         #the file is saved in the TopasSimulation folder
@@ -284,27 +313,30 @@
         if len(doses) != self.total_number_of_voxels:
             print('Error: the number of doses is not equal to the number of voxels, Probably due to a unmatching Topas simulation')
             return
         for voxel in self.voxel_list:
             voxel.dose = doses[voxel.voxel_number]
         return
 
-    def update_oxygen(self, o2_per_volume=1, diffusion_number=5):
+    def update_oxygen(self, o2_per_volume=1, capillary_length=5):
         print('-- Computing oxygen map')
+        side = self.voxel_list[0].half_length * 2
         for voxel in self.voxel_list:
-            voxel.oxygen = int((voxel.vessel_volume * o2_per_volume) / (np.pi * self.config.effective_vessel_radius**2 * voxel.half_length * 2))
+            voxel.oxygen = int((voxel.vessel_volume * o2_per_volume) / side)
             voxel.bifurcation_density += voxel.oxygen
+        diffusion_number = int(capillary_length / side)
         for i in range(diffusion_number):
             new_oxygen_map = np.zeros(self.total_number_of_voxels)
             print('--- o2 map computing', i, 'out of', diffusion_number)
             for voxel in self.voxel_list:
                 sum = voxel.oxygen
-                for neighbor in self.find_neighbors(voxel):
+                list_neighbors = self.find_moor_neighbors(voxel)
+                for neighbor in list_neighbors:
                     sum += neighbor.oxygen
-                new_oxygen_map[voxel.voxel_number] = sum / (1 + len(self.find_neighbors(voxel)))
+                new_oxygen_map[voxel.voxel_number] = sum / (1 + len(list_neighbors))
             for voxel in self.voxel_list:
                 voxel.oxygen = int(new_oxygen_map[voxel.voxel_number])
         return
 
     def oxygen_map(self):
         values = []
         positions = []
@@ -472,19 +504,22 @@
         for vessel in self.vasculature.list_of_vessels:
             for point in vessel.path:
                 if self.is_inside(point):
                     volume += vessel.volume_per_point()
         return volume
 
     def measure_tumor_volume(self):
-        volume = 0
+        volume_necrotic_free = 0
+        volume_total = 0
         for voxel in self.voxel_list:
-            if voxel.number_of_tumor_cells() > 3:
-                volume += voxel.volume
-        return volume
+            if voxel.number_of_tumor_cells() > 0:
+                volume_necrotic_free += voxel.volume
+            if voxel.number_of_tumor_cells() > 0 or voxel.number_of_necrotic_cells() > 0:
+                volume_total += voxel.volume
+        return volume_total, volume_necrotic_free
 
     def show_angiogenesis_metrics(self, real=True, first=True):
         # Extract the voxel values for each parameter
         volume = self.voxel_list[0].volume
         side = self.voxel_list[0].half_length * 2
         if real:
             volume_values = [voxel.vessel_volume / volume for voxel in self.voxel_list]
```

### Comparing `OncoAMBER-1.2.8/amber/save_alpha_dataframe6.csv` & `OncoAMBER-1.3.3/amber/save_alpha_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.8/amber/save_beta_dataframe6.csv` & `OncoAMBER-1.3.3/amber/save_beta_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.8/setup.py` & `OncoAMBER-1.3.3/setup.py`

 * *Files identical despite different names*

