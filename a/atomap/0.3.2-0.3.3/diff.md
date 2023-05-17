# Comparing `tmp/atomap-0.3.2.tar.gz` & `tmp/atomap-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomap-0.3.2.tar", last modified: Thu Apr 28 15:26:11 2022, max compression
+gzip compressed data, was "atomap-0.3.3.tar", last modified: Wed May 17 14:27:40 2023, max compression
```

## Comparing `atomap-0.3.2.tar` & `atomap-0.3.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 magnunor  (1000) magnunor  (1000)        0 2022-04-28 15:26:11.023671 atomap-0.3.2/
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    35055 2021-03-22 09:50:58.000000 atomap-0.3.2/LICENSE
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)       34 2021-03-22 09:50:58.000000 atomap-0.3.2/MANIFEST.in
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     1519 2022-04-28 15:26:11.023671 atomap-0.3.2/PKG-INFO
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)      891 2021-03-22 09:50:58.000000 atomap-0.3.2/README.md
-drwxr-xr-x   0 magnunor  (1000) magnunor  (1000)        0 2022-04-28 15:26:11.015670 atomap-0.3.2/atomap/
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)        0 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/__init__.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     7441 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/analysis_tools.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     3799 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/animation_plotting_tools.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)      647 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/api.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    39365 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/atom_finding_refining.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    19878 2021-06-11 13:01:24.000000 atomap-0.3.2/atomap/atom_lattice.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    15109 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/atom_plane.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    31164 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/atom_position.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)      592 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/conftest.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     4628 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/convert_ase.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    35868 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/dummy_data.py
-drwxr-xr-x   0 magnunor  (1000) magnunor  (1000)        0 2022-04-28 15:26:11.015670 atomap-0.3.2/atomap/example_data/
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)   296016 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/example_data/example_detector_image.hspy
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    79683 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/example_data/simulated_nanoparticle.hspy
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)      568 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/example_data.py
-drwxr-xr-x   0 magnunor  (1000) magnunor  (1000)        0 2022-04-28 15:26:11.015670 atomap-0.3.2/atomap/external/
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)        0 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/external/__init__.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     5213 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/external/add_marker.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     4308 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/external/gaussian2d.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2073 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/fitting_tools.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     5652 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/gui_classes.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    12002 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/initial_position_finding.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    10239 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/io.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     8174 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/main.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    28430 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/plotting.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    12647 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/process_parameters.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    22224 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/quantification.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     4081 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/stats.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)   111357 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/sublattice.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     6240 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/symmetry_finding.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    14518 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/testing_tools.py
-drwxr-xr-x   0 magnunor  (1000) magnunor  (1000)        0 2022-04-28 15:26:11.019670 atomap-0.3.2/atomap/tests/
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)        0 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/__init__.py
-drwxr-xr-x   0 magnunor  (1000) magnunor  (1000)        0 2022-04-28 15:26:11.019670 atomap-0.3.2/atomap/tests/datasets/
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)        0 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/datasets/__init__.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)      147 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/datasets/dataset_filenames.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)   201661 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/datasets/test_ABF_cropped.hdf5
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)   205738 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/datasets/test_ADF_cropped.hdf5
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    72457 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/datasets/test_atom_lattice.hdf5
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     3006 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_adf_abf_sto.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2420 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_analysis_tools.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2663 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_animation_plotting_tools.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)      340 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_ase_import.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    26892 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/tests/test_atom_finding_refining.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    13176 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_atom_lattice.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2451 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_atom_plane.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    17293 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/tests/test_atom_position.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     7058 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_dummy_data.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)      287 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_example_data.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2466 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_fitting_accuracy.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2171 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_fitting_tools.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     9329 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_gui_function_qt.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     3721 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_initial_position_finding.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     6890 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_io.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     1855 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_main.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)      645 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_peak_separation.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     3219 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_plotting.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)      594 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_process_parameters.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     5524 2022-04-28 15:20:21.000000 atomap-0.3.2/atomap/tests/test_quantification.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     1517 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_stats.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    54181 2021-06-11 13:01:24.000000 atomap-0.3.2/atomap/tests/test_sublattice.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     6106 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_symmetry_finding.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     8556 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_testing_tools.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    24742 2021-03-22 09:50:58.000000 atomap-0.3.2/atomap/tests/test_tools.py
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)    57790 2021-06-11 13:01:24.000000 atomap-0.3.2/atomap/tools.py
-drwxr-xr-x   0 magnunor  (1000) magnunor  (1000)        0 2022-04-28 15:26:11.015670 atomap-0.3.2/atomap.egg-info/
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     1519 2022-04-28 15:26:10.000000 atomap-0.3.2/atomap.egg-info/PKG-INFO
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2045 2022-04-28 15:26:10.000000 atomap-0.3.2/atomap.egg-info/SOURCES.txt
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)        1 2022-04-28 15:26:10.000000 atomap-0.3.2/atomap.egg-info/dependency_links.txt
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)      115 2022-04-28 15:26:10.000000 atomap-0.3.2/atomap.egg-info/requires.txt
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)        7 2022-04-28 15:26:10.000000 atomap-0.3.2/atomap.egg-info/top_level.txt
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)       79 2022-04-28 15:26:11.023671 atomap-0.3.2/setup.cfg
--rw-r--r--   0 magnunor  (1000) magnunor  (1000)     1770 2022-04-28 15:22:19.000000 atomap-0.3.2/setup.py
+drwxrwxr-x   0 magnunor  (1000) magnunor  (1000)        0 2023-05-17 14:27:40.499956 atomap-0.3.3/
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)    35055 2020-08-09 16:40:43.000000 atomap-0.3.3/LICENSE
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)       34 2020-08-09 16:40:43.000000 atomap-0.3.3/MANIFEST.in
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)     1519 2023-05-17 14:27:40.499956 atomap-0.3.3/PKG-INFO
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)      891 2021-01-30 19:49:15.000000 atomap-0.3.3/README.md
+drwxrwxr-x   0 magnunor  (1000) magnunor  (1000)        0 2023-05-17 14:27:40.491956 atomap-0.3.3/atomap/
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)        0 2020-08-09 16:40:43.000000 atomap-0.3.3/atomap/__init__.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     7441 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/analysis_tools.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     3799 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/animation_plotting_tools.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)      647 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/api.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    39364 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/atom_finding_refining.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    19878 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/atom_lattice.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    15109 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/atom_plane.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    31163 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/atom_position.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)      592 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/conftest.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)     4628 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/convert_ase.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    35868 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/dummy_data.py
+drwxrwxr-x   0 magnunor  (1000) magnunor  (1000)        0 2023-05-17 14:27:40.495956 atomap-0.3.3/atomap/example_data/
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)   296016 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/example_data/example_detector_image.hspy
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    79683 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/example_data/simulated_nanoparticle.hspy
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)      568 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/example_data.py
+drwxrwxr-x   0 magnunor  (1000) magnunor  (1000)        0 2023-05-17 14:27:40.495956 atomap-0.3.3/atomap/external/
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)        0 2020-08-09 16:40:43.000000 atomap-0.3.3/atomap/external/__init__.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)     5196 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/external/add_marker.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)     4308 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/external/gaussian2d.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)     2073 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/fitting_tools.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)     5652 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/gui_classes.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    12002 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/initial_position_finding.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)    10239 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/io.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)     8174 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/main.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    28429 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/plotting.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)    12647 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/process_parameters.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    22234 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/quantification.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     4081 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/stats.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)   111357 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/sublattice.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     6240 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/symmetry_finding.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    14518 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/testing_tools.py
+drwxrwxr-x   0 magnunor  (1000) magnunor  (1000)        0 2023-05-17 14:27:40.495956 atomap-0.3.3/atomap/tests/
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)        0 2020-08-09 16:40:43.000000 atomap-0.3.3/atomap/tests/__init__.py
+drwxrwxr-x   0 magnunor  (1000) magnunor  (1000)        0 2023-05-17 14:27:40.499956 atomap-0.3.3/atomap/tests/datasets/
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)        0 2020-08-09 16:40:43.000000 atomap-0.3.3/atomap/tests/datasets/__init__.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)      147 2020-08-09 16:40:43.000000 atomap-0.3.3/atomap/tests/datasets/dataset_filenames.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)   205229 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/tests/datasets/test_ABF_cropped.hdf5
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)   209306 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/tests/datasets/test_ADF_cropped.hdf5
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)    72457 2020-08-09 16:40:43.000000 atomap-0.3.3/atomap/tests/datasets/test_atom_lattice.hdf5
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     3006 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_adf_abf_sto.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2420 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_analysis_tools.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2663 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_animation_plotting_tools.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)      340 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_ase_import.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    26892 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/tests/test_atom_finding_refining.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)    13176 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_atom_lattice.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2451 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_atom_plane.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    17293 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/tests/test_atom_position.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     7058 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_dummy_data.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)      287 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_example_data.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2466 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_fitting_accuracy.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2171 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_fitting_tools.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    11741 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/tests/test_gui_function_qt.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     3721 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_initial_position_finding.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     6890 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_io.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     1855 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_main.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)      645 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_peak_separation.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     3219 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_plotting.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)      594 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_process_parameters.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)     5529 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/tests/test_quantification.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     1517 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_stats.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    54181 2023-05-17 14:22:38.000000 atomap-0.3.3/atomap/tests/test_sublattice.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     6106 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_symmetry_finding.py
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     8556 2021-01-30 19:49:15.000000 atomap-0.3.3/atomap/tests/test_testing_tools.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    24718 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/tests/test_tools.py
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)    57789 2023-05-17 14:22:49.000000 atomap-0.3.3/atomap/tools.py
+drwxrwxr-x   0 magnunor  (1000) magnunor  (1000)        0 2023-05-17 14:27:40.495956 atomap-0.3.3/atomap.egg-info/
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     1519 2023-05-17 14:27:40.000000 atomap-0.3.3/atomap.egg-info/PKG-INFO
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)     2045 2023-05-17 14:27:40.000000 atomap-0.3.3/atomap.egg-info/SOURCES.txt
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)        1 2023-05-17 14:27:40.000000 atomap-0.3.3/atomap.egg-info/dependency_links.txt
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)      116 2023-05-17 14:27:40.000000 atomap-0.3.3/atomap.egg-info/requires.txt
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)        7 2023-05-17 14:27:40.000000 atomap-0.3.3/atomap.egg-info/top_level.txt
+-rw-r--r--   0 magnunor  (1000) magnunor  (1000)       79 2023-05-17 14:27:40.499956 atomap-0.3.3/setup.cfg
+-rw-rw-r--   0 magnunor  (1000) magnunor  (1000)     1772 2023-05-17 14:23:55.000000 atomap-0.3.3/setup.py
```

### Comparing `atomap-0.3.2/LICENSE` & `atomap-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/PKG-INFO` & `atomap-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: atomap
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library for analysing atomic resolution images
 Home-page: https://atomap.org/
 Author: Magnus Nord
 Author-email: magnunor@gmail.com
 License: GPL v3
-Download-URL: https://gitlab.com/atomap/atomap/repository/archive.tar?ref=0.3.2
+Download-URL: https://gitlab.com/atomap/atomap/repository/archive.tar?ref=0.3.3
 Keywords: STEM,data analysis,microscopy
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `atomap-0.3.2/README.md` & `atomap-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/analysis_tools.py` & `atomap-0.3.3/atomap/analysis_tools.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/animation_plotting_tools.py` & `atomap-0.3.3/atomap/animation_plotting_tools.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/api.py` & `atomap-0.3.3/atomap/api.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/atom_finding_refining.py` & `atomap-0.3.3/atomap/atom_finding_refining.py`

 * *Files 0% similar despite different names*

```diff
@@ -1093,15 +1093,14 @@
                 atom.sigma_y = abs(g.sigma_y.value)
                 atom.amplitude_gaussian = g.A.value
                 atom._gaussian_fitted = True
             break
 
 
 def refine_sublattice(sublattice, refinement_config_list, percent_to_nn):
-
     total_number_of_refinements = 0
     for refinement_config in refinement_config_list:
         total_number_of_refinements += refinement_config[1]
 
     sublattice.find_nearest_neighbors()
 
     current_counts = 1
```

### Comparing `atomap-0.3.2/atomap/atom_lattice.py` & `atomap-0.3.3/atomap/atom_lattice.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/atom_plane.py` & `atomap-0.3.3/atomap/atom_plane.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/atom_position.py` & `atomap-0.3.3/atomap/atom_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,14 @@
             x1 = image_data.shape[1]
         if y1 > image_data.shape[0]:
             y1 = image_data.shape[0]
         image_slice = copy.deepcopy(image_data[y0:y1, x0:x1])
         return image_slice, x0, y0
 
     def _plot_gaussian2d_debug(self, slice_radius, gaussian, data_slice):
-
         X, Y = np.meshgrid(
             np.arange(-slice_radius, slice_radius, 1),
             np.arange(-slice_radius, slice_radius, 1),
         )
         s_m = gaussian.function(X, Y)
 
         fig, axarr = plt.subplots(2, 2)
```

### Comparing `atomap-0.3.2/atomap/conftest.py` & `atomap-0.3.3/atomap/conftest.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/convert_ase.py` & `atomap-0.3.3/atomap/convert_ase.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/dummy_data.py` & `atomap-0.3.3/atomap/dummy_data.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/example_data/example_detector_image.hspy` & `atomap-0.3.3/atomap/example_data/example_detector_image.hspy`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/example_data/simulated_nanoparticle.hspy` & `atomap-0.3.3/atomap/example_data/simulated_nanoparticle.hspy`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/example_data.py` & `atomap-0.3.3/atomap/example_data.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/external/add_marker.py` & `atomap-0.3.3/atomap/external/add_marker.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,16 @@
         plot. If True, the marker will be added to the
         metadata.Markers list, and be plotted with plot(plot_markers=True).
         If the signal is saved as a HyperSpy HDF5 file, the markers will be
         stored in the HDF5 signal and be restored when the file is loaded.
 
     Examples
     --------
-    >>> import scipy.misc
     >>> import hyperspy.api as hs
-    >>> im = hs.signals.Signal2D(scipy.misc.ascent())
+    >>> im = hs.signals.Signal2D(np.random.random((512, 512)))
     >>> m = hs.markers.rectangle(x1=150, y1=100, x2=400, y2=400, color='red')
     >>> im.add_marker(m)
 
     Adding to a 1D signal, where the point will change
     when the navigation index is changed
     >>> import numpy as np
     >>> s = hs.signals.Signal1D(np.random.random((3, 100)))
```

### Comparing `atomap-0.3.2/atomap/external/gaussian2d.py` & `atomap-0.3.3/atomap/external/gaussian2d.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/fitting_tools.py` & `atomap-0.3.3/atomap/fitting_tools.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/gui_classes.py` & `atomap-0.3.3/atomap/gui_classes.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/initial_position_finding.py` & `atomap-0.3.3/atomap/initial_position_finding.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/io.py` & `atomap-0.3.3/atomap/io.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/main.py` & `atomap-0.3.3/atomap/main.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/plotting.py` & `atomap-0.3.3/atomap/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         headwidth=0.0,
         headlength=0.0,
         headaxislength=0.0,
         scale=20.0,
         pivot="middle",
     )
     ax.set_xlim(min(x_pos_list), max(x_pos_list))
-    ax.set_ylim(min(y_pos_list), max(y_pos_list))
+    ax.set_ylim(max(y_pos_list), min(y_pos_list))
     ax.set_aspect("equal")
     if save:
         fig.savefig("vector_field.png", dpi=200)
 
 
 def plot_zone_vector_and_atom_distance_map(
     image_data,
@@ -632,15 +632,14 @@
         amplitude_data[1][0][-1] * distance_data_scale,
     )
 
 
 def _make_line_profile_subplot_from_three_parameter_data(
     ax, data_list, interface_plane, scale_x=1.0, scale_y=1.0, invert_line_profiles=False
 ):
-
     projected_positions = to.project_position_property(data_list, interface_plane)
     layer_list = to.sort_projected_positions_into_layers(projected_positions)
     line_profile_data = to.combine_projected_positions_layers(layer_list)
 
     line_profile_data = np.array(line_profile_data)
 
     position = line_profile_data[:, 0]
```

### Comparing `atomap-0.3.2/atomap/process_parameters.py` & `atomap-0.3.3/atomap/process_parameters.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/quantification.py` & `atomap-0.3.3/atomap/quantification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿import numpy as np
 from scipy import ndimage, optimize
 import matplotlib.pyplot as plt
-from matplotlib import cm
+from matplotlib import colormaps
 import sklearn.mixture as mixture
 
 from atomap.sublattice import Sublattice
 from atomap.atom_lattice import Atom_Lattice
 
 
 def centered_distance_matrix(centre, det_image):
@@ -568,15 +568,15 @@
         dic[int(sort_indices[i])] = i
 
     sorted_labels = np.copy(labels)
     for k, v in dic.items():
         sorted_labels[labels == k] = v
 
     x = np.linspace(0.0, 1.0, max_atom_nums)
-    truncated_cmap = cm.get_cmap(cmap)(x)[np.newaxis, :, :3].tolist()
+    truncated_cmap = colormaps["viridis"](x)[np.newaxis, :, :3].tolist()
     truncated_cmap[0] = truncated_cmap[0][-model.n_components :]
 
     if image is None:
         image = sublattice.signal
     sub_lattices = {}
     atom_positions = sublattice.atom_positions
     for num in sort_indices.ravel():
```

### Comparing `atomap-0.3.2/atomap/stats.py` & `atomap-0.3.3/atomap/stats.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/sublattice.py` & `atomap-0.3.3/atomap/sublattice.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/symmetry_finding.py` & `atomap-0.3.3/atomap/symmetry_finding.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/testing_tools.py` & `atomap-0.3.3/atomap/testing_tools.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/datasets/test_ABF_cropped.hdf5` & `atomap-0.3.3/atomap/tests/datasets/test_ABF_cropped.hdf5`

 * *Files 4% similar despite different names*

#### h5dump {}

```diff
@@ -1,8 +1,8 @@
-HDF5 "/tmp/diffoscope_nfxta4uy_/tmp0mt_k1ix_TarContainer/0/42.hdf5" {
+HDF5 "/tmp/diffoscope_nfxta4uy_/tmpub7ono0w_TarContainer/0/42.hdf5" {
 GROUP "/" {
    ATTRIBUTE "file_format" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
@@ -17,15 +17,15 @@
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
       }
       DATASPACE  SCALAR
       DATA {
-      (0): "3.0"
+      (0): "3.1"
       }
    }
    GROUP "Experiments" {
       GROUP "__unnamed__" {
          ATTRIBUTE "package" {
             DATATYPE  H5T_STRING {
                STRSIZE H5T_VARIABLE;
@@ -43,18 +43,41 @@
                STRSIZE H5T_VARIABLE;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_UTF8;
                CTYPE H5T_C_S1;
             }
             DATASPACE  SCALAR
             DATA {
-            (0): "1.6.1"
+            (0): "1.7.5"
             }
          }
          GROUP "axis-0" {
+            ATTRIBUTE "_type" {
+               DATATYPE  H5T_STRING {
+                  STRSIZE H5T_VARIABLE;
+                  STRPAD H5T_STR_NULLTERM;
+                  CSET H5T_CSET_UTF8;
+                  CTYPE H5T_C_S1;
+               }
+               DATASPACE  SCALAR
+               DATA {
+               (0): "UniformDataAxis"
+               }
+            }
+            ATTRIBUTE "is_binned" {
+               DATATYPE  H5T_ENUM {
+                  H5T_STD_I8LE;
+                  "FALSE"            0;
+                  "TRUE"             1;
+               }
+               DATASPACE  SCALAR
+               DATA {
+               (0): FALSE
+               }
+            }
             ATTRIBUTE "navigate" {
                DATATYPE  H5T_ENUM {
                   H5T_STD_I8LE;
                   "FALSE"            0;
                   "TRUE"             1;
                }
                DATASPACE  SCALAR
@@ -81,14 +104,37 @@
                DATASPACE  SCALAR
                DATA {
                (0): 400
                }
             }
          }
          GROUP "axis-1" {
+            ATTRIBUTE "_type" {
+               DATATYPE  H5T_STRING {
+                  STRSIZE H5T_VARIABLE;
+                  STRPAD H5T_STR_NULLTERM;
+                  CSET H5T_CSET_UTF8;
+                  CTYPE H5T_C_S1;
+               }
+               DATASPACE  SCALAR
+               DATA {
+               (0): "UniformDataAxis"
+               }
+            }
+            ATTRIBUTE "is_binned" {
+               DATATYPE  H5T_ENUM {
+                  H5T_STD_I8LE;
+                  "FALSE"            0;
+                  "TRUE"             1;
+               }
+               DATASPACE  SCALAR
+               DATA {
+               (0): FALSE
+               }
+            }
             ATTRIBUTE "navigate" {
                DATATYPE  H5T_ENUM {
                   H5T_STD_I8LE;
                   "FALSE"            0;
                   "TRUE"             1;
                }
                DATASPACE  SCALAR
@@ -116,15 +162,15 @@
                DATA {
                (0): 380
                }
             }
          }
          DATASET "data" {
             DATATYPE  16-bit little-endian floating-point 16-bit precision
-            DATASPACE  SIMPLE { ( 400, 380 ) / ( H5S_UNLIMITED, H5S_UNLIMITED ) }
+            DATASPACE  SIMPLE { ( 400, 380 ) / ( 400, 380 ) }
             DATA {
             (0,0): 2368, 2186, 2436, 2616, 2968, 3152, 3118, 3102, 3336,
             (0,9): 3634, 3382, 3260, 3304, 3274, 3318, 3060, 2690, 2298,
             (0,18): 1861, 1769, 1738, 1643, 1703, 1861, 1814, 1964, 2298,
             (0,27): 2536, 2928, 2888, 3036, 3126, 3240, 3336, 3318, 3196,
             (0,36): 3316, 3072, 2750, 2640, 2460, 2478, 2340, 2412, 2392,
             (0,45): 2504, 2754, 3008, 3104, 3254, 3480, 3502, 3530, 3444,
@@ -17336,27 +17382,118 @@
                      CTYPE H5T_C_S1;
                   }
                   DATASPACE  SCALAR
                   DATA {
                   (0): ""
                   }
                }
-            }
-            GROUP "Signal" {
-               ATTRIBUTE "binned" {
-                  DATATYPE  H5T_ENUM {
-                     H5T_STD_I8LE;
-                     "FALSE"            0;
-                     "TRUE"             1;
+               GROUP "FileIO" {
+                  GROUP "0" {
+                     ATTRIBUTE "hyperspy_version" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "1.7.5"
+                        }
+                     }
+                     ATTRIBUTE "io_plugin" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "hyperspy.io_plugins.hspy"
+                        }
+                     }
+                     ATTRIBUTE "operation" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "load"
+                        }
+                     }
+                     ATTRIBUTE "timestamp" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "2023-05-14T19:23:22.083086+02:00"
+                        }
+                     }
                   }
-                  DATASPACE  SCALAR
-                  DATA {
-                  (0): FALSE
+                  GROUP "1" {
+                     ATTRIBUTE "hyperspy_version" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "1.7.5"
+                        }
+                     }
+                     ATTRIBUTE "io_plugin" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "hyperspy.io_plugins.hspy"
+                        }
+                     }
+                     ATTRIBUTE "operation" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "save"
+                        }
+                     }
+                     ATTRIBUTE "timestamp" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "2023-05-14T19:23:32.219564+02:00"
+                        }
+                     }
                   }
                }
+            }
+            GROUP "Signal" {
                ATTRIBUTE "record_by" {
                   DATATYPE  H5T_STRING {
                      STRSIZE H5T_VARIABLE;
                      STRPAD H5T_STR_NULLTERM;
                      CSET H5T_CSET_UTF8;
                      CTYPE H5T_C_S1;
                   }
```

### Comparing `atomap-0.3.2/atomap/tests/datasets/test_ADF_cropped.hdf5` & `atomap-0.3.3/atomap/tests/datasets/test_ADF_cropped.hdf5`

 * *Files 4% similar despite different names*

#### h5dump {}

```diff
@@ -1,8 +1,8 @@
-HDF5 "/tmp/diffoscope_nfxta4uy_/tmp0mt_k1ix_TarContainer/0/43.hdf5" {
+HDF5 "/tmp/diffoscope_nfxta4uy_/tmpub7ono0w_TarContainer/0/43.hdf5" {
 GROUP "/" {
    ATTRIBUTE "file_format" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
@@ -17,15 +17,15 @@
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
       }
       DATASPACE  SCALAR
       DATA {
-      (0): "3.0"
+      (0): "3.1"
       }
    }
    GROUP "Experiments" {
       GROUP "__unnamed__" {
          ATTRIBUTE "package" {
             DATATYPE  H5T_STRING {
                STRSIZE H5T_VARIABLE;
@@ -43,18 +43,41 @@
                STRSIZE H5T_VARIABLE;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_UTF8;
                CTYPE H5T_C_S1;
             }
             DATASPACE  SCALAR
             DATA {
-            (0): "1.6.1"
+            (0): "1.7.5"
             }
          }
          GROUP "axis-0" {
+            ATTRIBUTE "_type" {
+               DATATYPE  H5T_STRING {
+                  STRSIZE H5T_VARIABLE;
+                  STRPAD H5T_STR_NULLTERM;
+                  CSET H5T_CSET_UTF8;
+                  CTYPE H5T_C_S1;
+               }
+               DATASPACE  SCALAR
+               DATA {
+               (0): "UniformDataAxis"
+               }
+            }
+            ATTRIBUTE "is_binned" {
+               DATATYPE  H5T_ENUM {
+                  H5T_STD_I8LE;
+                  "FALSE"            0;
+                  "TRUE"             1;
+               }
+               DATASPACE  SCALAR
+               DATA {
+               (0): FALSE
+               }
+            }
             ATTRIBUTE "navigate" {
                DATATYPE  H5T_ENUM {
                   H5T_STD_I8LE;
                   "FALSE"            0;
                   "TRUE"             1;
                }
                DATASPACE  SCALAR
@@ -81,14 +104,37 @@
                DATASPACE  SCALAR
                DATA {
                (0): 400
                }
             }
          }
          GROUP "axis-1" {
+            ATTRIBUTE "_type" {
+               DATATYPE  H5T_STRING {
+                  STRSIZE H5T_VARIABLE;
+                  STRPAD H5T_STR_NULLTERM;
+                  CSET H5T_CSET_UTF8;
+                  CTYPE H5T_C_S1;
+               }
+               DATASPACE  SCALAR
+               DATA {
+               (0): "UniformDataAxis"
+               }
+            }
+            ATTRIBUTE "is_binned" {
+               DATATYPE  H5T_ENUM {
+                  H5T_STD_I8LE;
+                  "FALSE"            0;
+                  "TRUE"             1;
+               }
+               DATASPACE  SCALAR
+               DATA {
+               (0): FALSE
+               }
+            }
             ATTRIBUTE "navigate" {
                DATATYPE  H5T_ENUM {
                   H5T_STD_I8LE;
                   "FALSE"            0;
                   "TRUE"             1;
                }
                DATASPACE  SCALAR
@@ -116,15 +162,15 @@
                DATA {
                (0): 380
                }
             }
          }
          DATASET "data" {
             DATATYPE  16-bit little-endian floating-point 16-bit precision
-            DATASPACE  SIMPLE { ( 400, 380 ) / ( H5S_UNLIMITED, H5S_UNLIMITED ) }
+            DATASPACE  SIMPLE { ( 400, 380 ) / ( 400, 380 ) }
             DATA {
             (0,0): 2538, 2618, 2596, 2356, 2016, 1953, 1981, 2054, 1870,
             (0,9): 1721, 1851, 2022, 2030, 1988, 2108, 2462, 2600, 2930,
             (0,18): 3414, 3644, 3612, 3792, 3756, 3596, 3344, 3100, 2684,
             (0,27): 2324, 1844, 1902, 1995, 1677, 1647, 1606, 1744, 1981,
             (0,36): 2118, 2110, 2094, 2292, 2394, 2360, 2302, 2416, 2294,
             (0,45): 2150, 2142, 2044, 1802, 1665, 1626, 1712, 1801, 1830,
@@ -17336,27 +17382,118 @@
                      CTYPE H5T_C_S1;
                   }
                   DATASPACE  SCALAR
                   DATA {
                   (0): ""
                   }
                }
-            }
-            GROUP "Signal" {
-               ATTRIBUTE "binned" {
-                  DATATYPE  H5T_ENUM {
-                     H5T_STD_I8LE;
-                     "FALSE"            0;
-                     "TRUE"             1;
+               GROUP "FileIO" {
+                  GROUP "0" {
+                     ATTRIBUTE "hyperspy_version" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "1.7.5"
+                        }
+                     }
+                     ATTRIBUTE "io_plugin" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "hyperspy.io_plugins.hspy"
+                        }
+                     }
+                     ATTRIBUTE "operation" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "load"
+                        }
+                     }
+                     ATTRIBUTE "timestamp" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "2023-05-14T19:22:43.534712+02:00"
+                        }
+                     }
                   }
-                  DATASPACE  SCALAR
-                  DATA {
-                  (0): FALSE
+                  GROUP "1" {
+                     ATTRIBUTE "hyperspy_version" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "1.7.5"
+                        }
+                     }
+                     ATTRIBUTE "io_plugin" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "hyperspy.io_plugins.hspy"
+                        }
+                     }
+                     ATTRIBUTE "operation" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "save"
+                        }
+                     }
+                     ATTRIBUTE "timestamp" {
+                        DATATYPE  H5T_STRING {
+                           STRSIZE H5T_VARIABLE;
+                           STRPAD H5T_STR_NULLTERM;
+                           CSET H5T_CSET_UTF8;
+                           CTYPE H5T_C_S1;
+                        }
+                        DATASPACE  SCALAR
+                        DATA {
+                        (0): "2023-05-14T19:22:59.590677+02:00"
+                        }
+                     }
                   }
                }
+            }
+            GROUP "Signal" {
                ATTRIBUTE "record_by" {
                   DATATYPE  H5T_STRING {
                      STRSIZE H5T_VARIABLE;
                      STRPAD H5T_STR_NULLTERM;
                      CSET H5T_CSET_UTF8;
                      CTYPE H5T_C_S1;
                   }
```

### Comparing `atomap-0.3.2/atomap/tests/datasets/test_atom_lattice.hdf5` & `atomap-0.3.3/atomap/tests/datasets/test_atom_lattice.hdf5`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_adf_abf_sto.py` & `atomap-0.3.3/atomap/tests/test_adf_abf_sto.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_analysis_tools.py` & `atomap-0.3.3/atomap/tests/test_analysis_tools.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_animation_plotting_tools.py` & `atomap-0.3.3/atomap/tests/test_animation_plotting_tools.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_atom_finding_refining.py` & `atomap-0.3.3/atomap/tests/test_atom_finding_refining.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_atom_lattice.py` & `atomap-0.3.3/atomap/tests/test_atom_lattice.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_atom_plane.py` & `atomap-0.3.3/atomap/tests/test_atom_plane.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_atom_position.py` & `atomap-0.3.3/atomap/tests/test_atom_position.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_dummy_data.py` & `atomap-0.3.3/atomap/tests/test_dummy_data.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_fitting_accuracy.py` & `atomap-0.3.3/atomap/tests/test_fitting_accuracy.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_fitting_tools.py` & `atomap-0.3.3/atomap/tests/test_fitting_tools.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_initial_position_finding.py` & `atomap-0.3.3/atomap/tests/test_initial_position_finding.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_io.py` & `atomap-0.3.3/atomap/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_main.py` & `atomap-0.3.3/atomap/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_peak_separation.py` & `atomap-0.3.3/atomap/tests/test_peak_separation.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_plotting.py` & `atomap-0.3.3/atomap/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_process_parameters.py` & `atomap-0.3.3/atomap/tests/test_process_parameters.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_quantification.py` & `atomap-0.3.3/atomap/tests/test_quantification.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,18 +90,18 @@
         for i in range(4):
             dic[int(sort_indices[i])] = i
 
         sorted_labels = np.copy(labels)
         for k, v in dic.items():
             sorted_labels[labels == k] = v
 
-        from matplotlib import cm
+        from matplotlib import colormaps
 
         x = np.linspace(0.0, 1.0, 4)
-        rgb = cm.get_cmap("viridis")(x)[np.newaxis, :, :3].tolist()
+        rgb = colormaps["viridis"](x)[np.newaxis, :, :3].tolist()
 
         quant._plot_fitted_hist(int_array, model, rgb, sort_indices)
 
     def test_statistical_method(self):
         models = quant.get_statistical_quant_criteria([self.sublattice], 10)
         atom_lattice = quant.statistical_quant(
             self.sublattice, models[3], 4, "C", 3.5, plot=False
```

### Comparing `atomap-0.3.2/atomap/tests/test_stats.py` & `atomap-0.3.3/atomap/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_sublattice.py` & `atomap-0.3.3/atomap/tests/test_sublattice.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_symmetry_finding.py` & `atomap-0.3.3/atomap/tests/test_symmetry_finding.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_testing_tools.py` & `atomap-0.3.3/atomap/tests/test_testing_tools.py`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/atomap/tests/test_tools.py` & `atomap-0.3.3/atomap/tests/test_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,17 +337,15 @@
         np.testing.assert_allclose(self.x, x_rot)
         np.testing.assert_allclose(self.y, y_rot)
 
 
 class TestRotatePointsAroundPosition:
     def test_degrees_centre_0(self):
         xc, yc = 0, 0
-        x, y = [5,], [
-            0,
-        ]
+        x, y = list([5]), list([0])
         x_rot, y_rot = to._rotate_points_around_position(xc, yc, x, y, 90)
         assert len(x_rot)
         assert len(y_rot)
         assert approx(x_rot[0]) == 0
         assert approx(y_rot[0]) == -5
         x_rot, y_rot = to._rotate_points_around_position(xc, yc, x, y, -90)
         assert approx(x_rot[0]) == 0
@@ -357,17 +355,15 @@
         assert approx(y_rot[0]) == 0
         x_rot, y_rot = to._rotate_points_around_position(xc, yc, x, y, -180)
         assert approx(x_rot[0]) == -5
         assert approx(y_rot[0]) == 0
 
     def test_degrees_centre_10(self):
         xc, yc = 10, 10
-        x, y = [5,], [
-            0,
-        ]
+        x, y = list([5]), list([0])
         x_rot, y_rot = to._rotate_points_around_position(xc, yc, x, y, 90)
         assert approx(x_rot[0]) == 0
         assert approx(y_rot[0]) == 15
         x_rot, y_rot = to._rotate_points_around_position(xc, yc, x, y, -90)
         assert approx(x_rot[0]) == 20
         assert approx(y_rot[0]) == 5
         x_rot, y_rot = to._rotate_points_around_position(xc, yc, x, y, 180)
```

### Comparing `atomap-0.3.2/atomap/tools.py` & `atomap-0.3.3/atomap/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1220,15 +1220,14 @@
 
     for i, j in progressbar(
         np.ndindex(image.shape[-2:]),
         desc="Building intensity map",
         total=np.prod(image.shape[-2:]),
         leave=False,
     ):
-
         point_index = point_record[i, j]
         if point_index == -1:
             intensity_record[..., i, j] = np.nan
         else:
             summed = integrated_intensity[point_index]
             intensity_record[..., i, j] = summed
```

### Comparing `atomap-0.3.2/atomap.egg-info/PKG-INFO` & `atomap-0.3.3/atomap.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: atomap
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library for analysing atomic resolution images
 Home-page: https://atomap.org/
 Author: Magnus Nord
 Author-email: magnunor@gmail.com
 License: GPL v3
-Download-URL: https://gitlab.com/atomap/atomap/repository/archive.tar?ref=0.3.2
+Download-URL: https://gitlab.com/atomap/atomap/repository/archive.tar?ref=0.3.3
 Keywords: STEM,data analysis,microscopy
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `atomap-0.3.2/atomap.egg-info/SOURCES.txt` & `atomap-0.3.3/atomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomap-0.3.2/setup.py` & `atomap-0.3.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,38 +8,38 @@
         packages = [
             'atomap',
             'atomap.tests',
             'atomap.tests.datasets',
             'atomap.external',
             'atomap.example_data',
             ],
-        version = '0.3.2',
+        version = '0.3.3',
         description = 'Library for analysing atomic resolution images',
         long_description=long_description,
         long_description_content_type='text/markdown',
         author = 'Magnus Nord',
         author_email = 'magnunor@gmail.com',
         license = 'GPL v3',
         url = 'https://atomap.org/',
-        download_url = 'https://gitlab.com/atomap/atomap/repository/archive.tar?ref=0.3.2',
+        download_url = 'https://gitlab.com/atomap/atomap/repository/archive.tar?ref=0.3.3',
         keywords = [
             'STEM',
             'data analysis',
             'microscopy',
             ],
         install_requires = [
             'scipy>=1.4.0',
             'numpy>=1.13',
             'h5py',
             'matplotlib>=3.1.0',
             'scikit-learn',
             'scikit-image>=0.17.1',
             'hyperspy>=1.5.2',
-            'ase>=3.17.0'
-            'numba'
+            'ase>=3.17.0',
+            'numba',
             ],
         classifiers = [
             'Development Status :: 3 - Alpha',
             'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
             'Intended Audience :: Science/Research',
             'Programming Language :: Python :: 3',
             ],
```

