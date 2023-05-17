# Comparing `tmp/FedArtML-0.1.7.tar.gz` & `tmp/FedArtML-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FedArtML-0.1.7.tar", last modified: Wed Apr 12 14:36:13 2023, max compression
+gzip compressed data, was "dist\FedArtML-0.1.8.tar", last modified: Wed May 17 15:21:38 2023, max compression
```

## Comparing `FedArtML-0.1.7.tar` & `FedArtML-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:36:13.000000 FedArtML-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/
--rw-rw-rw-   0        0        0     3725 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3725 2023-04-12 14:36:13.000000 FedArtML-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2850 2023-04-12 14:34:59.000000 FedArtML-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 14:36:13.000000 FedArtML-0.1.7/fedartml/
--rw-rw-rw-   0        0        0      178 2022-11-24 21:44:10.000000 FedArtML-0.1.7/fedartml/__init__.py
--rw-rw-rw-   0        0        0    38522 2023-04-12 14:32:47.000000 FedArtML-0.1.7/fedartml/fl_interactive_plots.py
--rw-rw-rw-   0        0        0    19440 2023-04-12 14:30:37.000000 FedArtML-0.1.7/fedartml/fl_split_as_federated_data.py
--rw-rw-rw-   0        0        0     5701 2023-03-30 06:01:03.000000 FedArtML-0.1.7/fedartml/function_base.py
--rw-rw-rw-   0        0        0       42 2023-04-12 14:36:13.000000 FedArtML-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-04-12 14:35:41.000000 FedArtML-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:21:38.000000 FedArtML-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-05-17 15:21:38.000000 FedArtML-0.1.8/FedArtML.egg-info/
+-rw-rw-rw-   0        0        0     3725 2023-05-17 15:21:38.000000 FedArtML-0.1.8/FedArtML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-05-17 15:21:38.000000 FedArtML-0.1.8/FedArtML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 15:21:38.000000 FedArtML-0.1.8/FedArtML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-17 15:21:38.000000 FedArtML-0.1.8/FedArtML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 15:21:38.000000 FedArtML-0.1.8/FedArtML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3725 2023-05-17 15:21:38.000000 FedArtML-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2850 2023-04-12 14:34:59.000000 FedArtML-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 15:21:38.000000 FedArtML-0.1.8/fedartml/
+-rw-rw-rw-   0        0        0      178 2022-11-24 21:44:10.000000 FedArtML-0.1.8/fedartml/__init__.py
+-rw-rw-rw-   0        0        0    38522 2023-04-12 14:32:47.000000 FedArtML-0.1.8/fedartml/fl_interactive_plots.py
+-rw-rw-rw-   0        0        0    19441 2023-05-17 15:17:00.000000 FedArtML-0.1.8/fedartml/fl_split_as_federated_data.py
+-rw-rw-rw-   0        0        0     5701 2023-03-30 06:01:03.000000 FedArtML-0.1.8/fedartml/function_base.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 15:21:38.000000 FedArtML-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-05-17 15:20:55.000000 FedArtML-0.1.8/setup.py
```

### Comparing `FedArtML-0.1.7/FedArtML.egg-info/PKG-INFO` & `FedArtML-0.1.8/FedArtML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedArtML
-Version: 0.1.7
+Version: 0.1.8
 Summary: Federated learning for Artificial Intelligence and Machine Learning library 
 Home-page: 
 Author: Daniel Mauricio Jimenez Gutierrez, Aris Anagnostopoulos, Ioannis Chatzigiannakis, Andrea Vitaletti
 Author-email: jimenezgutierrez@diag.uniroma1.it
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FedArtML-0.1.7/PKG-INFO` & `FedArtML-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedArtML
-Version: 0.1.7
+Version: 0.1.8
 Summary: Federated learning for Artificial Intelligence and Machine Learning library 
 Home-page: 
 Author: Daniel Mauricio Jimenez Gutierrez, Aris Anagnostopoulos, Ioannis Chatzigiannakis, Andrea Vitaletti
 Author-email: jimenezgutierrez@diag.uniroma1.it
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FedArtML-0.1.7/README.md` & `FedArtML-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `FedArtML-0.1.7/fedartml/fl_interactive_plots.py` & `FedArtML-0.1.8/fedartml/fl_interactive_plots.py`

 * *Files identical despite different names*

### Comparing `FedArtML-0.1.7/fedartml/fl_split_as_federated_data.py` & `FedArtML-0.1.8/fedartml/fl_split_as_federated_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             if i == (local_nodes - 2):
                 n_fin = len(uniq_class_noniid) + 1
             else:
                 n_fin += n_class_per_node_noniid
 
         return pctg_distr, num_distr, idx_distr, num_per_node
 
-    def dirichlet_method(self, labels, local_nodes, alpha=0, random_state=None):
+    def dirichlet_method(self, labels, local_nodes, alpha=1000, random_state=None):
         """
         Create a federated dataset divided per each local node (client) using the Dirichlet (dirichlet) method.
 
         Parameters
         ----------
         labels : array-like
             The target values (class labels in classification).
@@ -162,16 +162,17 @@
         """
         labels = np.array(labels)
 
         min_size = 0
         num_classes = len(np.unique(labels))
         N = labels.shape[0]
         random_state_loop = random_state
+        idx_batch = [[] for _ in range(local_nodes)]
         while min_size < num_classes:
-            idx_batch = [[] for _ in range(local_nodes)]
+
             for k in range(num_classes):
                 idx_k = np.where(labels == k)[0]
                 np.random.seed(random_state_loop)
                 np.random.shuffle(idx_k)
                 proportions = np.random.dirichlet(np.repeat(alpha, local_nodes))
                 # Balance
                 proportions = np.array([p * (len(idx_j) < N / local_nodes) for p, idx_j in zip(proportions, idx_batch)])
@@ -205,15 +206,15 @@
             num_distr.append(aux_examples_node)
             idx_distr.append(idx_batch[j])
             if random_state is not None:
                 random_state_loop += 100
 
         return pctg_distr, num_distr, idx_distr, num_per_node
 
-    def create_clients(self, image_list, label_list, num_clients=5, prefix_cli='client', method="percent_noniid",
+    def create_clients(self, image_list, label_list, num_clients=4, prefix_cli='client', method="percent_noniid",
                        alpha=1000, percent_noniid=0):
         """
         Create a federated dataset divided per each local node (client) using the desired method (percent_noniid or
         dirichlet). It works only for classification problems (labels as classes).
 
         Parameters
         ----------
```

### Comparing `FedArtML-0.1.7/fedartml/function_base.py` & `FedArtML-0.1.8/fedartml/function_base.py`

 * *Files identical despite different names*

### Comparing `FedArtML-0.1.7/setup.py` & `FedArtML-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="FedArtML",
-    version="0.1.7",
+    version="0.1.8",
     description="Federated learning for Artificial Intelligence and Machine Learning library ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Daniel Mauricio Jimenez Gutierrez, Aris Anagnostopoulos, Ioannis Chatzigiannakis, Andrea Vitaletti",
     author_email="jimenezgutierrez@diag.uniroma1.it",
     license="MIT",
```

