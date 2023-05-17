# Comparing `tmp/minari-0.2.1.tar.gz` & `tmp/minari-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minari-0.2.1.tar", last modified: Tue Jan  3 12:48:22 2023, max compression
+gzip compressed data, was "minari-0.3.0b0.tar", last modified: Wed May 17 14:20:16 2023, max compression
```

## Comparing `minari-0.2.1.tar` & `minari-0.3.0b0.tar`

### file list

```diff
@@ -1,27 +1,37 @@
-drwxrwxr-x   0 will      (1000) will      (1000)        0 2023-01-03 12:48:22.023045 minari-0.2.1/
--rw-rw-r--   0 will      (1000) will      (1000)    12203 2022-12-04 00:47:19.000000 minari-0.2.1/LICENSE
--rw-rw-r--   0 will      (1000) will      (1000)     2504 2023-01-03 12:48:22.023045 minari-0.2.1/PKG-INFO
--rw-rw-r--   0 will      (1000) will      (1000)     1908 2023-01-02 16:45:45.000000 minari-0.2.1/README.md
-drwxrwxr-x   0 will      (1000) will      (1000)        0 2023-01-03 12:48:22.023045 minari-0.2.1/minari/
--rw-rw-r--   0 will      (1000) will      (1000)      236 2022-12-04 00:47:19.000000 minari-0.2.1/minari/__init__.py
--rw-rw-r--   0 will      (1000) will      (1000)  1313410 2023-01-03 11:47:04.000000 minari-0.2.1/minari/dataset.cpp
--rw-rw-r--   0 will      (1000) will      (1000)      632 2022-12-04 00:47:19.000000 minari-0.2.1/minari/dataset.pxd
--rw-rw-r--   0 will      (1000) will      (1000)     5667 2022-12-24 00:58:13.000000 minari-0.2.1/minari/dataset.pyi
--rw-rw-r--   0 will      (1000) will      (1000)    48256 2023-01-02 17:07:05.000000 minari-0.2.1/minari/dataset.pyx
--rw-rw-r--   0 will      (1000) will      (1000)     5326 2023-01-02 16:52:13.000000 minari-0.2.1/minari/logger.py
-drwxrwxr-x   0 will      (1000) will      (1000)        0 2023-01-03 12:48:22.023045 minari-0.2.1/minari/storage/
--rw-rw-r--   0 will      (1000) will      (1000)        0 2023-01-03 12:31:26.000000 minari-0.2.1/minari/storage/__init__.py
--rw-rw-r--   0 will      (1000) will      (1000)      584 2023-01-02 17:05:55.000000 minari-0.2.1/minari/storage/datasets_root_dir.py
--rw-rw-r--   0 will      (1000) will      (1000)     2122 2023-01-03 11:20:43.000000 minari-0.2.1/minari/storage/hosting.py
--rw-rw-r--   0 will      (1000) will      (1000)      694 2022-12-04 00:47:19.000000 minari-0.2.1/minari/storage/local.py
-drwxrwxr-x   0 will      (1000) will      (1000)        0 2023-01-03 12:48:22.023045 minari-0.2.1/minari/utils/
--rw-rw-r--   0 will      (1000) will      (1000)        0 2023-01-03 12:34:52.000000 minari-0.2.1/minari/utils/__init__.py
--rw-rw-r--   0 will      (1000) will      (1000)      839 2022-12-04 22:27:51.000000 minari-0.2.1/minari/utils/assert_name_spec.py
-drwxrwxr-x   0 will      (1000) will      (1000)        0 2023-01-03 12:48:22.023045 minari-0.2.1/minari.egg-info/
--rw-rw-r--   0 will      (1000) will      (1000)     2504 2023-01-03 12:48:21.000000 minari-0.2.1/minari.egg-info/PKG-INFO
--rw-rw-r--   0 will      (1000) will      (1000)      458 2023-01-03 12:48:22.000000 minari-0.2.1/minari.egg-info/SOURCES.txt
--rw-rw-r--   0 will      (1000) will      (1000)        1 2023-01-03 12:48:21.000000 minari-0.2.1/minari.egg-info/dependency_links.txt
--rw-rw-r--   0 will      (1000) will      (1000)      148 2023-01-03 12:48:21.000000 minari-0.2.1/minari.egg-info/requires.txt
--rw-rw-r--   0 will      (1000) will      (1000)        7 2023-01-03 12:48:21.000000 minari-0.2.1/minari.egg-info/top_level.txt
--rw-rw-r--   0 will      (1000) will      (1000)       38 2023-01-03 12:48:22.023045 minari-0.2.1/setup.cfg
--rw-rw-r--   0 will      (1000) will      (1000)     1870 2023-01-03 12:45:57.000000 minari-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.510837 minari-0.3.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-05-17 14:20:00.000000 minari-0.3.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-17 14:20:16.510837 minari-0.3.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-17 14:20:00.000000 minari-0.3.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.502837 minari-0.3.0b0/minari/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/minari/data_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/data_collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/minari/data_collector/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/data_collector/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/data_collector/callbacks/episode_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/data_collector/callbacks/step_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/data_collector/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/minari/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/dataset/minari_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/dataset/minari_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/minari/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/storage/datasets_root_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/storage/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/storage/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/minari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-17 14:20:00.000000 minari-0.3.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:20:16.510837 minari-0.3.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-17 14:20:00.000000 minari-0.3.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-05-17 14:20:00.000000 minari-0.3.0b0/tests/test_dataset_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 14:20:00.000000 minari-0.3.0b0/tests/test_dataset_download.py
```

### Comparing `minari-0.2.1/LICENSE` & `minari-0.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `minari-0.2.1/PKG-INFO` & `minari-0.3.0b0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,85 @@
 Metadata-Version: 2.1
 Name: minari
-Version: 0.2.1
-Summary: Datasets for offline deep reinforcement learning
-Home-page: https://github.com/Farama-Foundation/Minari
-Author: Will Dudley
-Author-email: will2346@live.co.uk
+Version: 0.3.0b0
+Summary: A standard format for offline reinforcement learning datasets, with popular reference datasets and related utilities.
+Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.6
+Project-URL: Homepage, https://farama.org
+Project-URL: Repository, https://github.com/Farama-Foundation/Minari
+Project-URL: Documentation, https://minari.farama.org/
+Project-URL: Bug Report, https://github.com/Farama-Foundation/Minari/issues
+Keywords: Reinforcement Learning,Offline RL,RL,AI,gymnasium,Farama
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7.0
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 
 <p align="center">
     <img src="minari-text.png" width="500px"/>
 </p>
 
-Minari is the new name of this library. Minari used to be called Kabuki.
+Minari is a Python library for conducting research in offline reinforcement learning, akin to an offline version of Gymnasium or an offline RL version of HuggingFace's datasets library. This library is currently in beta.
 
-Minari is intended to be a Python library for conducting research in offline reinforcement learning, akin to an offline version of Gymnasium or an offline RL version of HuggingFace's datasets library. The goal is to release a fully working beta in late November or early December.
+The documentation website is at [minari.farama.org](https://minari.farama.org/main/). We also have a public discord server (which we use for Q&A and to coordinate development work) that you can join here: https://discord.gg/bnJ6kubTg6.
 
-We have a public discord server (which we also use to coordinate development work) that you can join here: https://discord.gg/jfERDCSw.
+Note: Minari was previously developed under the name Kabuki.
 
 
 ## Installation
-`pip install numpy cython`
 
-`pip install git+https://github.com/Farama-Foundation/Minari.git`
+Currently the beta release is under development. If you'd like to start testing or contribute to Minari please install this project from source with: 
 
-## Downloading datasets
-
-```python
-import minari
-
-dataset = minari.download_dataset("LunarLander_v2_test-dataset")
+```bash
+git clone https://github.com/Farama-Foundation/Minari.git
+cd Minari
+pip install -e .
 ```
 
-## Recreating Gymnasium environments (Coming very soon!)
+## Getting Started
 
-```python
-import gymnasium as gym
+For an introduction to Minari, see [Basic Usage](https://minari.farama.org/main/content/basic_usage/). To create new datasets using Minari, see our [Pointmaze D4RL Dataset](https://minari.farama.org/main/tutorials/dataset_creation/point_maze_dataset/) tutorial, which re-creates the Maze2D datasets from [D4RL](https://github.com/Farama-Foundation/D4RL).
 
-env = gym.make(gym.SpecStack(json.loads(dataset.environment_stack)))
-```
+## API 
 
-## Uploading datasets
+To check available remote datasets:
 
 ```python
-dataset.save(
-    ".datasets/LunarLander-v2-test_dataset.hdf5"
-)  # todo: abstract away parent directory and hdf5 extension
-dataset = minari.upload_dataset("LunarLander_v2_test-dataset")
-```
-
-
-## Saving to dataset format
-It is not the aim of Minari to insist that you use a certain buffer implementation. However, in order to maintain standardisation across the library, we have a standardised format, the `MinariDataset` class, for saving replay buffers to file. 
+import minari
 
-This converter will have tests to ensure formatting standards
+minari.list_remote_datasets()
+```
 
-## Checking available remote datasets
+To check available local datasets:
 
 ```python
 import minari
 
-minari.list_remote_datasets()
+minari.list_local_datasets()
 ```
 
-## Checking available local datasets
+To download a dataset:
+
 ```python
 import minari
-minari.list_local_datasets()  # todo: implement
+
+dataset = minari.download_dataset("LunarLander_v2_remote-test-dataset")
 ```
-Datasets are stored in the `.datasets` directory in your project directory.
 
+## Project Maintainers
+Main Contributors: [Rodrigo Perez-Vicente](https://github.com/rodrigodelazcano), [Omar Younis](https://github.com/younik)
 
+Maintenance for this project is also contributed by the broader Farama team: [farama.org/team](https://farama.org/team).
 
 ___
 
 _Minari is a shortening of Minarai, the Japanese word for "learning by observation"._
```

### Comparing `minari-0.2.1/minari.egg-info/PKG-INFO` & `minari-0.3.0b0/minari.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,85 @@
 Metadata-Version: 2.1
 Name: minari
-Version: 0.2.1
-Summary: Datasets for offline deep reinforcement learning
-Home-page: https://github.com/Farama-Foundation/Minari
-Author: Will Dudley
-Author-email: will2346@live.co.uk
+Version: 0.3.0b0
+Summary: A standard format for offline reinforcement learning datasets, with popular reference datasets and related utilities.
+Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.6
+Project-URL: Homepage, https://farama.org
+Project-URL: Repository, https://github.com/Farama-Foundation/Minari
+Project-URL: Documentation, https://minari.farama.org/
+Project-URL: Bug Report, https://github.com/Farama-Foundation/Minari/issues
+Keywords: Reinforcement Learning,Offline RL,RL,AI,gymnasium,Farama
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7.0
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 
 <p align="center">
     <img src="minari-text.png" width="500px"/>
 </p>
 
-Minari is the new name of this library. Minari used to be called Kabuki.
+Minari is a Python library for conducting research in offline reinforcement learning, akin to an offline version of Gymnasium or an offline RL version of HuggingFace's datasets library. This library is currently in beta.
 
-Minari is intended to be a Python library for conducting research in offline reinforcement learning, akin to an offline version of Gymnasium or an offline RL version of HuggingFace's datasets library. The goal is to release a fully working beta in late November or early December.
+The documentation website is at [minari.farama.org](https://minari.farama.org/main/). We also have a public discord server (which we use for Q&A and to coordinate development work) that you can join here: https://discord.gg/bnJ6kubTg6.
 
-We have a public discord server (which we also use to coordinate development work) that you can join here: https://discord.gg/jfERDCSw.
+Note: Minari was previously developed under the name Kabuki.
 
 
 ## Installation
-`pip install numpy cython`
 
-`pip install git+https://github.com/Farama-Foundation/Minari.git`
+Currently the beta release is under development. If you'd like to start testing or contribute to Minari please install this project from source with: 
 
-## Downloading datasets
-
-```python
-import minari
-
-dataset = minari.download_dataset("LunarLander_v2_test-dataset")
+```bash
+git clone https://github.com/Farama-Foundation/Minari.git
+cd Minari
+pip install -e .
 ```
 
-## Recreating Gymnasium environments (Coming very soon!)
+## Getting Started
 
-```python
-import gymnasium as gym
+For an introduction to Minari, see [Basic Usage](https://minari.farama.org/main/content/basic_usage/). To create new datasets using Minari, see our [Pointmaze D4RL Dataset](https://minari.farama.org/main/tutorials/dataset_creation/point_maze_dataset/) tutorial, which re-creates the Maze2D datasets from [D4RL](https://github.com/Farama-Foundation/D4RL).
 
-env = gym.make(gym.SpecStack(json.loads(dataset.environment_stack)))
-```
+## API 
 
-## Uploading datasets
+To check available remote datasets:
 
 ```python
-dataset.save(
-    ".datasets/LunarLander-v2-test_dataset.hdf5"
-)  # todo: abstract away parent directory and hdf5 extension
-dataset = minari.upload_dataset("LunarLander_v2_test-dataset")
-```
-
-
-## Saving to dataset format
-It is not the aim of Minari to insist that you use a certain buffer implementation. However, in order to maintain standardisation across the library, we have a standardised format, the `MinariDataset` class, for saving replay buffers to file. 
+import minari
 
-This converter will have tests to ensure formatting standards
+minari.list_remote_datasets()
+```
 
-## Checking available remote datasets
+To check available local datasets:
 
 ```python
 import minari
 
-minari.list_remote_datasets()
+minari.list_local_datasets()
 ```
 
-## Checking available local datasets
+To download a dataset:
+
 ```python
 import minari
-minari.list_local_datasets()  # todo: implement
+
+dataset = minari.download_dataset("LunarLander_v2_remote-test-dataset")
 ```
-Datasets are stored in the `.datasets` directory in your project directory.
 
+## Project Maintainers
+Main Contributors: [Rodrigo Perez-Vicente](https://github.com/rodrigodelazcano), [Omar Younis](https://github.com/younik)
 
+Maintenance for this project is also contributed by the broader Farama team: [farama.org/team](https://farama.org/team).
 
 ___
 
 _Minari is a shortening of Minarai, the Japanese word for "learning by observation"._
```

