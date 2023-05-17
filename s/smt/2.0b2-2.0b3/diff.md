# Comparing `tmp/smt-2.0b2.tar.gz` & `tmp/smt-2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\rlafage\workspace\smt\dist\.tmp-imctwyom\smt-2.0b2.tar", last modified: Thu Apr 13 14:42:19 2023, max compression
+gzip compressed data, was "D:\rlafage\workspace\smt\dist\.tmp-ul6sai3g\smt-2.0b3.tar", last modified: Wed May 17 09:23:58 2023, max compression
```

## Comparing `smt-2.0b2.tar` & `smt-2.0b3.tar`

### file list

```diff
@@ -1,118 +1,119 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.340367 smt-2.0b2/
--rw-rw-rw-   0        0        0     1543 2018-12-22 21:42:35.000000 smt-2.0b2/LICENSE.txt
--rw-rw-rw-   0        0        0       84 2019-06-10 15:38:34.000000 smt-2.0b2/MANIFEST.in
--rw-rw-rw-   0        0        0     1737 2023-04-13 14:42:19.340367 smt-2.0b2/PKG-INFO
--rw-rw-rw-   0        0        0     2990 2023-03-08 08:23:36.000000 smt-2.0b2/README.md
--rw-rw-rw-   0        0        0       69 2023-03-02 15:01:33.000000 smt-2.0b2/pyproject.toml
--rw-rw-rw-   0        0        0      114 2023-04-13 14:42:19.340367 smt-2.0b2/setup.cfg
--rw-rw-rw-   0        0        0     3767 2023-03-08 08:23:36.000000 smt-2.0b2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.125345 smt-2.0b2/smt/
--rw-rw-rw-   0        0        0       23 2023-04-13 14:40:53.000000 smt-2.0b2/smt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.182230 smt-2.0b2/smt/applications/
--rw-rw-rw-   0        0        0      187 2021-01-26 14:08:32.000000 smt-2.0b2/smt/applications/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-04-13 14:40:53.000000 smt-2.0b2/smt/applications/application.py
--rw-rw-rw-   0        0        0    16178 2023-04-13 14:40:53.000000 smt-2.0b2/smt/applications/ego.py
--rw-rw-rw-   0        0        0    28159 2023-04-13 14:40:53.000000 smt-2.0b2/smt/applications/mfk.py
--rw-rw-rw-   0        0        0     2382 2023-04-13 14:40:53.000000 smt-2.0b2/smt/applications/mfkpls.py
--rw-rw-rw-   0        0        0     2137 2023-04-13 14:40:53.000000 smt-2.0b2/smt/applications/mfkplsk.py
--rw-rw-rw-   0        0        0    17327 2023-04-13 14:40:53.000000 smt-2.0b2/smt/applications/mixed_integer.py
--rw-rw-rw-   0        0        0    26114 2023-04-13 14:40:53.000000 smt-2.0b2/smt/applications/moe.py
--rw-rw-rw-   0        0        0    10088 2023-04-13 14:40:53.000000 smt-2.0b2/smt/applications/vfm.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.229110 smt-2.0b2/smt/problems/
--rw-rw-rw-   0        0        0      801 2023-04-13 13:31:06.000000 smt-2.0b2/smt/problems/__init__.py
--rw-rw-rw-   0        0        0     1738 2022-08-23 09:30:16.000000 smt-2.0b2/smt/problems/branin.py
--rw-rw-rw-   0        0        0     4199 2022-08-23 09:30:16.000000 smt-2.0b2/smt/problems/cantilever_beam.py
--rw-rw-rw-   0        0        0     1358 2020-11-30 16:48:50.000000 smt-2.0b2/smt/problems/lp_norm.py
--rw-rw-rw-   0        0        0     1505 2023-04-13 13:31:06.000000 smt-2.0b2/smt/problems/mixed_cantilever_beam.py
--rw-rw-rw-   0        0        0      964 2020-11-30 16:48:50.000000 smt-2.0b2/smt/problems/ndim_cantilever_beam.py
--rw-rw-rw-   0        0        0      940 2020-11-30 16:48:50.000000 smt-2.0b2/smt/problems/ndim_robot_arm.py
--rw-rw-rw-   0        0        0      935 2020-11-30 16:48:50.000000 smt-2.0b2/smt/problems/ndim_rosenbrock.py
--rw-rw-rw-   0        0        0      853 2020-11-30 16:48:50.000000 smt-2.0b2/smt/problems/ndim_step_function.py
--rw-rw-rw-   0        0        0     1876 2023-04-13 13:31:06.000000 smt-2.0b2/smt/problems/neural_network.py
--rw-rw-rw-   0        0        0     3314 2022-01-12 15:11:14.000000 smt-2.0b2/smt/problems/problem.py
--rw-rw-rw-   0        0        0     2700 2020-11-30 16:48:50.000000 smt-2.0b2/smt/problems/reduced_problem.py
--rw-rw-rw-   0        0        0     3100 2022-08-23 09:30:16.000000 smt-2.0b2/smt/problems/robot_arm.py
--rw-rw-rw-   0        0        0     1467 2020-11-30 16:48:50.000000 smt-2.0b2/smt/problems/rosenbrock.py
--rw-rw-rw-   0        0        0     1146 2022-08-23 09:30:16.000000 smt-2.0b2/smt/problems/sphere.py
--rw-rw-rw-   0        0        0     2108 2022-08-23 09:30:16.000000 smt-2.0b2/smt/problems/tensor_product.py
--rw-rw-rw-   0        0        0     4703 2022-08-23 09:30:16.000000 smt-2.0b2/smt/problems/torsion_vibration.py
--rw-rw-rw-   0        0        0     3157 2022-08-23 09:30:16.000000 smt-2.0b2/smt/problems/water_flow.py
--rw-rw-rw-   0        0        0     2805 2022-08-23 09:30:16.000000 smt-2.0b2/smt/problems/water_flow_lfidelity.py
--rw-rw-rw-   0        0        0     3036 2022-08-23 09:30:16.000000 smt-2.0b2/smt/problems/welded_beam.py
--rw-rw-rw-   0        0        0     3372 2022-08-22 07:12:21.000000 smt-2.0b2/smt/problems/wing_weight.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.244733 smt-2.0b2/smt/sampling_methods/
--rw-rw-rw-   0        0        0       93 2018-12-22 21:42:35.000000 smt-2.0b2/smt/sampling_methods/__init__.py
--rw-rw-rw-   0        0        0     2016 2023-01-12 17:00:33.000000 smt-2.0b2/smt/sampling_methods/full_factorial.py
--rw-rw-rw-   0        0        0    13859 2023-04-13 14:40:53.000000 smt-2.0b2/smt/sampling_methods/lhs.py
--rw-rw-rw-   0        0        0      829 2021-01-28 14:52:03.000000 smt-2.0b2/smt/sampling_methods/random.py
--rw-rw-rw-   0        0        0     4675 2023-01-12 17:00:33.000000 smt-2.0b2/smt/sampling_methods/sampling_method.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.113219 smt-2.0b2/smt/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.244733 smt-2.0b2/smt/src/idw/
--rw-rw-rw-   0        0        0     2529 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/idw/idw.cpp
--rw-rw-rw-   0        0        0      335 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/idw/idw.hpp
--rw-rw-rw-   0        0        0   313797 2023-04-13 14:42:16.000000 smt-2.0b2/smt/src/idw/idwclib.cpp
--rw-rw-rw-   0        0        0      931 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/idw/idwclib.pyx
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.244733 smt-2.0b2/smt/src/rbf/
--rw-rw-rw-   0        0        0     2080 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rbf/rbf.cpp
--rw-rw-rw-   0        0        0      366 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rbf/rbf.hpp
--rw-rw-rw-   0        0        0   316817 2023-04-13 14:42:15.000000 smt-2.0b2/smt/src/rbf/rbfclib.cpp
--rw-rw-rw-   0        0        0     1058 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rbf/rbfclib.pyx
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.260356 smt-2.0b2/smt/src/rmts/
--rw-rw-rw-   0        0        0     7239 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rmts/rmtb.cpp
--rw-rw-rw-   0        0        0      394 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rmts/rmtb.hpp
--rw-rw-rw-   0        0        0     5968 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rmts/rmtc.cpp
--rw-rw-rw-   0        0        0      692 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rmts/rmtc.hpp
--rw-rw-rw-   0        0        0     2684 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rmts/rmts.cpp
--rw-rw-rw-   0        0        0      608 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rmts/rmts.hpp
--rw-rw-rw-   0        0        0   430206 2023-04-13 14:42:16.000000 smt-2.0b2/smt/src/rmts/rmtsclib.cpp
--rw-rw-rw-   0        0        0     3618 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rmts/rmtsclib.pyx
--rw-rw-rw-   0        0        0      532 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rmts/utils.cpp
--rw-rw-rw-   0        0        0      178 2018-12-22 21:42:35.000000 smt-2.0b2/smt/src/rmts/utils.hpp
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.282488 smt-2.0b2/smt/surrogate_models/
--rw-rw-rw-   0        0        0      532 2023-04-13 13:31:06.000000 smt-2.0b2/smt/surrogate_models/__init__.py
--rw-rw-rw-   0        0        0     1980 2023-03-01 09:44:14.000000 smt-2.0b2/smt/surrogate_models/gekpls.py
--rw-rw-rw-   0        0        0    10492 2021-01-12 13:42:11.000000 smt-2.0b2/smt/surrogate_models/genn.py
--rw-rw-rw-   0        0        0     3805 2021-01-26 14:08:32.000000 smt-2.0b2/smt/surrogate_models/idw.py
--rw-rw-rw-   0        0        0     4633 2023-04-13 14:40:53.000000 smt-2.0b2/smt/surrogate_models/kpls.py
--rw-rw-rw-   0        0        0     1436 2023-04-13 14:40:53.000000 smt-2.0b2/smt/surrogate_models/kplsk.py
--rw-rw-rw-   0        0        0      955 2023-04-13 14:40:53.000000 smt-2.0b2/smt/surrogate_models/krg.py
--rw-rw-rw-   0        0        0    70885 2023-04-13 14:40:53.000000 smt-2.0b2/smt/surrogate_models/krg_based.py
--rw-rw-rw-   0        0        0     2783 2023-01-12 15:06:16.000000 smt-2.0b2/smt/surrogate_models/ls.py
--rw-rw-rw-   0        0        0    17658 2023-03-01 09:44:14.000000 smt-2.0b2/smt/surrogate_models/mgp.py
--rw-rw-rw-   0        0        0     4937 2023-04-13 14:40:53.000000 smt-2.0b2/smt/surrogate_models/qp.py
--rw-rw-rw-   0        0        0     6530 2021-01-12 13:42:11.000000 smt-2.0b2/smt/surrogate_models/rbf.py
--rw-rw-rw-   0        0        0     4635 2021-01-12 13:42:11.000000 smt-2.0b2/smt/surrogate_models/rmtb.py
--rw-rw-rw-   0        0        0     5761 2021-01-12 13:42:11.000000 smt-2.0b2/smt/surrogate_models/rmtc.py
--rw-rw-rw-   0        0        0    20916 2023-04-13 14:40:53.000000 smt-2.0b2/smt/surrogate_models/rmts.py
--rw-rw-rw-   0        0        0    19216 2023-04-13 13:31:06.000000 smt-2.0b2/smt/surrogate_models/surrogate_model.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.324739 smt-2.0b2/smt/utils/
--rw-rw-rw-   0        0        0       37 2018-12-22 21:42:35.000000 smt-2.0b2/smt/utils/__init__.py
--rw-rw-rw-   0        0        0     1863 2020-04-22 07:33:16.000000 smt-2.0b2/smt/utils/caching.py
--rw-rw-rw-   0        0        0      949 2022-10-21 19:56:44.000000 smt-2.0b2/smt/utils/checks.py
--rw-rw-rw-   0        0        0    13183 2023-03-01 09:44:14.000000 smt-2.0b2/smt/utils/krg_sampling.py
--rw-rw-rw-   0        0        0    51472 2023-04-13 14:40:53.000000 smt-2.0b2/smt/utils/kriging.py
--rw-rw-rw-   0        0        0     8022 2022-08-23 09:30:16.000000 smt-2.0b2/smt/utils/line_search.py
--rw-rw-rw-   0        0        0    17986 2023-04-13 14:40:53.000000 smt-2.0b2/smt/utils/linear_solvers.py
--rw-rw-rw-   0        0        0     3750 2023-04-13 14:40:53.000000 smt-2.0b2/smt/utils/misc.py
--rw-rw-rw-   0        0        0     6936 2023-03-08 08:23:36.000000 smt-2.0b2/smt/utils/mixed_integer.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.340367 smt-2.0b2/smt/utils/neural_net/
--rw-rw-rw-   0        0        0      293 2019-04-14 10:57:11.000000 smt-2.0b2/smt/utils/neural_net/__init__.py
--rw-rw-rw-   0        0        0     2528 2020-04-22 07:33:16.000000 smt-2.0b2/smt/utils/neural_net/activation.py
--rw-rw-rw-   0        0        0    11665 2023-04-13 14:40:53.000000 smt-2.0b2/smt/utils/neural_net/bwd_prop.py
--rw-rw-rw-   0        0        0    10006 2023-04-13 14:40:53.000000 smt-2.0b2/smt/utils/neural_net/data.py
--rw-rw-rw-   0        0        0     9734 2023-04-13 14:40:53.000000 smt-2.0b2/smt/utils/neural_net/fwd_prop.py
--rw-rw-rw-   0        0        0     3604 2023-04-13 14:40:53.000000 smt-2.0b2/smt/utils/neural_net/loss.py
--rw-rw-rw-   0        0        0     1080 2019-04-14 10:57:11.000000 smt-2.0b2/smt/utils/neural_net/metrics.py
--rw-rw-rw-   0        0        0    21968 2023-04-13 14:40:53.000000 smt-2.0b2/smt/utils/neural_net/model.py
--rw-rw-rw-   0        0        0    13245 2023-04-13 14:40:53.000000 smt-2.0b2/smt/utils/neural_net/optimizer.py
--rw-rw-rw-   0        0        0     4630 2020-04-22 07:33:16.000000 smt-2.0b2/smt/utils/options_dictionary.py
--rw-rw-rw-   0        0        0     3608 2020-11-30 16:48:50.000000 smt-2.0b2/smt/utils/printer.py
--rw-rw-rw-   0        0        0     4087 2020-04-22 07:33:16.000000 smt-2.0b2/smt/utils/silence.py
--rw-rw-rw-   0        0        0     1413 2020-04-22 07:33:16.000000 smt-2.0b2/smt/utils/sm_test_case.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:19.140974 smt-2.0b2/smt.egg-info/
--rw-rw-rw-   0        0        0     1737 2023-04-13 14:42:18.000000 smt-2.0b2/smt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2969 2023-04-13 14:42:19.000000 smt-2.0b2/smt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:42:18.000000 smt-2.0b2/smt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-09-09 08:43:37.000000 smt-2.0b2/smt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-04-13 14:42:18.000000 smt-2.0b2/smt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-13 14:42:18.000000 smt-2.0b2/smt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.583097 smt-2.0b3/
+-rw-rw-rw-   0        0        0     1543 2018-12-22 21:42:35.000000 smt-2.0b3/LICENSE.txt
+-rw-rw-rw-   0        0        0       84 2019-06-10 15:38:34.000000 smt-2.0b3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1760 2023-05-17 09:23:58.583097 smt-2.0b3/PKG-INFO
+-rw-rw-rw-   0        0        0     2990 2023-03-08 08:23:36.000000 smt-2.0b3/README.md
+-rw-rw-rw-   0        0        0       69 2023-03-02 15:01:33.000000 smt-2.0b3/pyproject.toml
+-rw-rw-rw-   0        0        0      114 2023-05-17 09:23:58.583097 smt-2.0b3/setup.cfg
+-rw-rw-rw-   0        0        0     3885 2023-05-16 15:13:53.000000 smt-2.0b3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.420324 smt-2.0b3/smt/
+-rw-rw-rw-   0        0        0       23 2023-05-17 09:22:32.000000 smt-2.0b3/smt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.451581 smt-2.0b3/smt/applications/
+-rw-rw-rw-   0        0        0      187 2021-01-26 14:08:32.000000 smt-2.0b3/smt/applications/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-04-13 14:40:53.000000 smt-2.0b3/smt/applications/application.py
+-rw-rw-rw-   0        0        0    15322 2023-05-17 09:22:32.000000 smt-2.0b3/smt/applications/ego.py
+-rw-rw-rw-   0        0        0    28217 2023-05-16 15:13:53.000000 smt-2.0b3/smt/applications/mfk.py
+-rw-rw-rw-   0        0        0     2382 2023-04-13 14:40:53.000000 smt-2.0b3/smt/applications/mfkpls.py
+-rw-rw-rw-   0        0        0     2137 2023-04-13 14:40:53.000000 smt-2.0b3/smt/applications/mfkplsk.py
+-rw-rw-rw-   0        0        0    12570 2023-05-17 09:22:32.000000 smt-2.0b3/smt/applications/mixed_integer.py
+-rw-rw-rw-   0        0        0    26146 2023-05-16 15:13:53.000000 smt-2.0b3/smt/applications/moe.py
+-rw-rw-rw-   0        0        0    10088 2023-04-13 14:40:53.000000 smt-2.0b3/smt/applications/vfm.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.498456 smt-2.0b3/smt/problems/
+-rw-rw-rw-   0        0        0      860 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/__init__.py
+-rw-rw-rw-   0        0        0     1738 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/branin.py
+-rw-rw-rw-   0        0        0     4199 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/cantilever_beam.py
+-rw-rw-rw-   0        0        0     5334 2023-05-17 09:22:32.000000 smt-2.0b3/smt/problems/hierarchical_goldstein.py
+-rw-rw-rw-   0        0        0     1358 2020-11-30 16:48:50.000000 smt-2.0b3/smt/problems/lp_norm.py
+-rw-rw-rw-   0        0        0     1890 2023-05-17 09:22:32.000000 smt-2.0b3/smt/problems/mixed_cantilever_beam.py
+-rw-rw-rw-   0        0        0      992 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/ndim_cantilever_beam.py
+-rw-rw-rw-   0        0        0      968 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/ndim_robot_arm.py
+-rw-rw-rw-   0        0        0      963 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/ndim_rosenbrock.py
+-rw-rw-rw-   0        0        0      881 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/ndim_step_function.py
+-rw-rw-rw-   0        0        0     3276 2023-05-17 09:22:32.000000 smt-2.0b3/smt/problems/neural_network.py
+-rw-rw-rw-   0        0        0     4754 2023-05-17 09:22:32.000000 smt-2.0b3/smt/problems/problem.py
+-rw-rw-rw-   0        0        0     2728 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/reduced_problem.py
+-rw-rw-rw-   0        0        0     3100 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/robot_arm.py
+-rw-rw-rw-   0        0        0     1467 2020-11-30 16:48:50.000000 smt-2.0b3/smt/problems/rosenbrock.py
+-rw-rw-rw-   0        0        0     1146 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/sphere.py
+-rw-rw-rw-   0        0        0     2108 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/tensor_product.py
+-rw-rw-rw-   0        0        0     4703 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/torsion_vibration.py
+-rw-rw-rw-   0        0        0     3157 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/water_flow.py
+-rw-rw-rw-   0        0        0     2805 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/water_flow_lfidelity.py
+-rw-rw-rw-   0        0        0     3036 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/welded_beam.py
+-rw-rw-rw-   0        0        0     3372 2022-08-22 07:12:21.000000 smt-2.0b3/smt/problems/wing_weight.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.498456 smt-2.0b3/smt/sampling_methods/
+-rw-rw-rw-   0        0        0       93 2018-12-22 21:42:35.000000 smt-2.0b3/smt/sampling_methods/__init__.py
+-rw-rw-rw-   0        0        0     2016 2023-01-12 17:00:33.000000 smt-2.0b3/smt/sampling_methods/full_factorial.py
+-rw-rw-rw-   0        0        0    13859 2023-04-13 14:40:53.000000 smt-2.0b3/smt/sampling_methods/lhs.py
+-rw-rw-rw-   0        0        0      829 2021-01-28 14:52:03.000000 smt-2.0b3/smt/sampling_methods/random.py
+-rw-rw-rw-   0        0        0     4675 2023-01-12 17:00:33.000000 smt-2.0b3/smt/sampling_methods/sampling_method.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.400117 smt-2.0b3/smt/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.514080 smt-2.0b3/smt/src/idw/
+-rw-rw-rw-   0        0        0     2529 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/idw/idw.cpp
+-rw-rw-rw-   0        0        0      335 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/idw/idw.hpp
+-rw-rw-rw-   0        0        0   313797 2023-05-17 09:23:55.000000 smt-2.0b3/smt/src/idw/idwclib.cpp
+-rw-rw-rw-   0        0        0      931 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/idw/idwclib.pyx
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.520589 smt-2.0b3/smt/src/rbf/
+-rw-rw-rw-   0        0        0     2080 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rbf/rbf.cpp
+-rw-rw-rw-   0        0        0      366 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rbf/rbf.hpp
+-rw-rw-rw-   0        0        0   316817 2023-05-17 09:23:55.000000 smt-2.0b3/smt/src/rbf/rbfclib.cpp
+-rw-rw-rw-   0        0        0     1058 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rbf/rbfclib.pyx
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.520589 smt-2.0b3/smt/src/rmts/
+-rw-rw-rw-   0        0        0     7239 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmtb.cpp
+-rw-rw-rw-   0        0        0      394 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmtb.hpp
+-rw-rw-rw-   0        0        0     5968 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmtc.cpp
+-rw-rw-rw-   0        0        0      692 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmtc.hpp
+-rw-rw-rw-   0        0        0     2684 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmts.cpp
+-rw-rw-rw-   0        0        0      608 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmts.hpp
+-rw-rw-rw-   0        0        0   430206 2023-05-17 09:23:56.000000 smt-2.0b3/smt/src/rmts/rmtsclib.cpp
+-rw-rw-rw-   0        0        0     3618 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmtsclib.pyx
+-rw-rw-rw-   0        0        0      532 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/utils.cpp
+-rw-rw-rw-   0        0        0      178 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/utils.hpp
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.551848 smt-2.0b3/smt/surrogate_models/
+-rw-rw-rw-   0        0        0      561 2023-05-17 09:22:32.000000 smt-2.0b3/smt/surrogate_models/__init__.py
+-rw-rw-rw-   0        0        0     1985 2023-05-16 15:13:53.000000 smt-2.0b3/smt/surrogate_models/gekpls.py
+-rw-rw-rw-   0        0        0    10492 2021-01-12 13:42:11.000000 smt-2.0b3/smt/surrogate_models/genn.py
+-rw-rw-rw-   0        0        0     3805 2021-01-26 14:08:32.000000 smt-2.0b3/smt/surrogate_models/idw.py
+-rw-rw-rw-   0        0        0     4633 2023-05-15 09:02:07.000000 smt-2.0b3/smt/surrogate_models/kpls.py
+-rw-rw-rw-   0        0        0     1436 2023-04-13 14:40:53.000000 smt-2.0b3/smt/surrogate_models/kplsk.py
+-rw-rw-rw-   0        0        0      955 2023-04-13 14:40:53.000000 smt-2.0b3/smt/surrogate_models/krg.py
+-rw-rw-rw-   0        0        0    75098 2023-05-17 09:22:32.000000 smt-2.0b3/smt/surrogate_models/krg_based.py
+-rw-rw-rw-   0        0        0     2783 2023-01-12 15:06:16.000000 smt-2.0b3/smt/surrogate_models/ls.py
+-rw-rw-rw-   0        0        0    17716 2023-05-16 15:13:53.000000 smt-2.0b3/smt/surrogate_models/mgp.py
+-rw-rw-rw-   0        0        0     4937 2023-04-13 14:40:53.000000 smt-2.0b3/smt/surrogate_models/qp.py
+-rw-rw-rw-   0        0        0     6530 2021-01-12 13:42:11.000000 smt-2.0b3/smt/surrogate_models/rbf.py
+-rw-rw-rw-   0        0        0     4635 2021-01-12 13:42:11.000000 smt-2.0b3/smt/surrogate_models/rmtb.py
+-rw-rw-rw-   0        0        0     5761 2021-01-12 13:42:11.000000 smt-2.0b3/smt/surrogate_models/rmtc.py
+-rw-rw-rw-   0        0        0    20916 2023-04-13 14:40:53.000000 smt-2.0b3/smt/surrogate_models/rmts.py
+-rw-rw-rw-   0        0        0    19436 2023-05-16 15:13:53.000000 smt-2.0b3/smt/surrogate_models/surrogate_model.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.567473 smt-2.0b3/smt/utils/
+-rw-rw-rw-   0        0        0       37 2018-12-22 21:42:35.000000 smt-2.0b3/smt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1863 2020-04-22 07:33:16.000000 smt-2.0b3/smt/utils/caching.py
+-rw-rw-rw-   0        0        0      949 2022-10-21 19:56:44.000000 smt-2.0b3/smt/utils/checks.py
+-rw-rw-rw-   0        0        0    28396 2023-05-17 09:22:32.000000 smt-2.0b3/smt/utils/design_space.py
+-rw-rw-rw-   0        0        0    13183 2023-03-01 09:44:14.000000 smt-2.0b3/smt/utils/krg_sampling.py
+-rw-rw-rw-   0        0        0    50183 2023-05-17 09:22:32.000000 smt-2.0b3/smt/utils/kriging.py
+-rw-rw-rw-   0        0        0     8022 2022-08-23 09:30:16.000000 smt-2.0b3/smt/utils/line_search.py
+-rw-rw-rw-   0        0        0    17986 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/linear_solvers.py
+-rw-rw-rw-   0        0        0     3750 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.583097 smt-2.0b3/smt/utils/neural_net/
+-rw-rw-rw-   0        0        0      293 2019-04-14 10:57:11.000000 smt-2.0b3/smt/utils/neural_net/__init__.py
+-rw-rw-rw-   0        0        0     2528 2020-04-22 07:33:16.000000 smt-2.0b3/smt/utils/neural_net/activation.py
+-rw-rw-rw-   0        0        0    11665 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/bwd_prop.py
+-rw-rw-rw-   0        0        0    10006 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/data.py
+-rw-rw-rw-   0        0        0     9734 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/fwd_prop.py
+-rw-rw-rw-   0        0        0     3604 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/loss.py
+-rw-rw-rw-   0        0        0     1080 2019-04-14 10:57:11.000000 smt-2.0b3/smt/utils/neural_net/metrics.py
+-rw-rw-rw-   0        0        0    21968 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/model.py
+-rw-rw-rw-   0        0        0    13245 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/optimizer.py
+-rw-rw-rw-   0        0        0     4630 2020-04-22 07:33:16.000000 smt-2.0b3/smt/utils/options_dictionary.py
+-rw-rw-rw-   0        0        0     3608 2020-11-30 16:48:50.000000 smt-2.0b3/smt/utils/printer.py
+-rw-rw-rw-   0        0        0     4087 2020-04-22 07:33:16.000000 smt-2.0b3/smt/utils/silence.py
+-rw-rw-rw-   0        0        0     1413 2020-04-22 07:33:16.000000 smt-2.0b3/smt/utils/sm_test_case.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.420324 smt-2.0b3/smt.egg-info/
+-rw-rw-rw-   0        0        0     1760 2023-05-17 09:23:57.000000 smt-2.0b3/smt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-05-17 09:23:58.000000 smt-2.0b3/smt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 09:23:57.000000 smt-2.0b3/smt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-09-09 08:43:37.000000 smt-2.0b3/smt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       49 2023-05-17 09:23:57.000000 smt-2.0b3/smt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-17 09:23:57.000000 smt-2.0b3/smt.egg-info/top_level.txt
```

### Comparing `smt-2.0b2/LICENSE.txt` & `smt-2.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/PKG-INFO` & `smt-2.0b3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smt
-Version: 2.0b2
+Version: 2.0b3
 Summary: The Surrogate Modeling Toolbox (SMT)
 Home-page: https://github.com/SMTorg/smt
 Download-URL: https://github.com/SMTorg/smt/releases
 Author: Mohamed Amine Bouhlel et al.
 Author-email: mbouhlel@umich.edu
 License: BSD-3
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
+Provides-Extra: numba
 License-File: LICENSE.txt
 
 
 The surrogate modeling toolbox (SMT) is a Python package that contains 
 a collection of surrogate modeling methods, sampling techniques, and 
 benchmarking functions. This package provides a library of surrogate 
 models that is simple to use and facilitates the implementation of additional methods.
```

### Comparing `smt-2.0b2/README.md` & `smt-2.0b3/README.md`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/setup.py` & `smt-2.0b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,19 @@
         "smt.applications",
     ],
     install_requires=[
         "scikit-learn",
         "pyDOE2",
         "scipy",
     ],
+    extras_require={
+        'numba': [  # pip install smt[numba]
+            "numba~=0.56.4",
+        ],
+    },
     python_requires=">=3.7",
     zip_safe=False,
     ext_modules=ext,
     url="https://github.com/SMTorg/smt",  # use the URL to the github repo
     download_url="https://github.com/SMTorg/smt/releases",
 )
```

### Comparing `smt-2.0b2/smt/applications/application.py` & `smt-2.0b3/smt/applications/application.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/applications/ego.py` & `smt-2.0b3/smt/applications/ego.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 import numpy as np
 
 from types import FunctionType
 
 from scipy.stats import norm
 from scipy.optimize import minimize
 
-from smt.utils.mixed_integer import XType
-from smt.sampling_methods import LHS
-from smt.surrogate_models import KPLS, KRG, KPLSK, MGP, GEKPLS, MixIntKernelType
+from smt.surrogate_models import KPLS, KRG, KPLSK, MGP, GEKPLS
 from smt.applications.application import SurrogateBasedApplication
-from smt.applications.mixed_integer import (
-    MixedIntegerContext,
-    MixedIntegerSamplingMethod,
+from smt.applications.mixed_integer import MixedIntegerContext
+from smt.utils.design_space import (
+    BaseDesignSpace,
+    DesignSpace,
+    FloatVariable,
+    CategoricalVariable,
 )
-from smt.utils.kriging import XSpecs
 
 
 class Evaluator(object):
     """
     An interface for evaluation of a function at x points (nsamples of dimension nx).
     User can derive this interface and override the run() method to implement custom multiprocessing.
     """
@@ -156,39 +156,31 @@
                         "Internal optimization succeeded at EGO iter = {}.{}".format(
                             k, p
                         )
                     )
                 # Set temporaly the y-coord point based on the kriging prediction
                 x_et_k = np.atleast_2d(x_et_k)
                 if self.mixint:
-                    x_et_k = self.mixint.cast_to_discrete_values(
-                        x_et_k, self.categorical_kernel == None
-                    )
+                    x_et_k, _ = self.design_space.correct_get_acting(x_et_k)
                 y_et_k = self._get_virtual_point(x_et_k, y_data)
 
                 # Update y_data with predicted value
                 y_data = y_data.reshape(y_data.shape[0], self.gpr.ny)
                 y_data = np.vstack((y_data, y_et_k))
                 x_data = np.atleast_2d(np.append(x_data, x_et_k, axis=0))
 
             # Compute the real values of y_data
             x_to_compute = np.atleast_2d(x_data[-n_parallel:])
-            if self.mixint and not (self.work_in_folded_space):
-                x_to_compute = self.mixint.fold_with_enum_index(x_to_compute)
             y = self._evaluator.run(fun, x_to_compute)
             y_data[-n_parallel:] = y
 
         # Find the optimal point
         ind_best = np.argmin(y_data if y_data.ndim == 1 else y_data[:, 0])
         x_opt = x_data[ind_best]
         y_opt = y_data[ind_best]
-
-        if self.mixint and not (self.work_in_folded_space):
-            x_opt = self.mixint.fold_with_enum_index(x_opt)[0]
-
         return x_opt, y_opt, ind_best, x_data, y_data
 
     def log(self, msg):
         if self.options["verbose"]:
             print(msg)
 
     def EI(self, points, enable_tunneling=False, x_data=None):
@@ -247,58 +239,52 @@
 
         ndarray: initial coord-x doe
         ndarray: initial coord-y doe = fun(xdoe)
 
         """
         # Set the model
         self.gpr = self.options["surrogate"]
-        self.xspecs = self.gpr.options["xspecs"]
-        self.xlimits = self.xspecs.limits
+        self.design_space: BaseDesignSpace = self.gpr.design_space
+        if isinstance(self.design_space, DesignSpace):
+            self.design_space.seed = self.options["random_state"]
 
         # Handle mixed integer optimization
-        self.work_in_folded_space = self.gpr.options["categorical_kernel"] is not None
-
-        if self.gpr.options["xspecs"].types != [XType.FLOAT] * len(
-            self.gpr.options["xspecs"].limits
-        ):
-            self.xtypes = self.gpr.options["xspecs"].types
+        is_continuous = self.design_space.is_all_cont
+        if not is_continuous:
             self.categorical_kernel = self.gpr.options["categorical_kernel"]
             self.mixint = MixedIntegerContext(
-                self.gpr.options["xspecs"],
-                work_in_folded_space=self.work_in_folded_space,
+                self.design_space,
+                work_in_folded_space=True,
             )
 
+            underlying_gpr = self.gpr
             self.gpr = self.mixint.build_kriging_model(self.gpr)
-            self._sampling = self.mixint.build_sampling_method(
-                LHS,
-                criterion="ese",
-                random_state=self.options["random_state"],
-                output_in_folded_space=self.work_in_folded_space,
+
+            self.categorical_kernel = underlying_gpr.options["categorical_kernel"]
+            self.mixint = MixedIntegerContext(
+                self.design_space,
+                work_in_folded_space=True,
             )
+            self._sampling = self.mixint.build_sampling_method()
+
         else:
             self.mixint = None
-            self._sampling = MixedIntegerSamplingMethod(
-                LHS,
-                self.xspecs,
-                criterion="ese",
-                random_state=self.options["random_state"],
-            )
+            self._sampling = lambda n: self.design_space.sample_valid_x(n)[0]
             self.categorical_kernel = None
+
         # Build DOE
         self._evaluator = self.options["evaluator"]
         xdoe = self.options["xdoe"]
         if xdoe is None:
             self.log("Build initial DOE with LHS")
             n_doe = self.options["n_doe"]
             x_doe = self._sampling(n_doe)
         else:
             self.log("Initial DOE given")
             x_doe = np.atleast_2d(xdoe)
-            if self.mixint and not (self.work_in_folded_space):
-                x_doe = self.mixint.unfold_with_enum_mask(x_doe)
 
         ydoe = self.options["ydoe"]
         if ydoe is None:
             y_doe = self._evaluator.run(fun, x_doe)
         else:  # to save time if y_doe is already given to EGO
             y_doe = ydoe
 
@@ -333,30 +319,27 @@
         """
         self._train_gpr(x_data, y_data)
 
         criterion = self.options["criterion"]
         n_start = self.options["n_start"]
         n_max_optim = self.options["n_max_optim"]
         if self.mixint:
-            bounds = self.mixint.get_unfolded_xlimits()
+            bounds = self.design_space.get_num_bounds()
             method = "COBYLA"
             cons = []
             for j in range(len(bounds)):
                 lower, upper = bounds[j]
-                if self.work_in_folded_space:
-                    if isinstance(self.xtypes[j], tuple):
-                        upper = int(upper - 1)
                 l = {"type": "ineq", "fun": lambda x, lb=lower, i=j: x[i] - lb}
                 u = {"type": "ineq", "fun": lambda x, ub=upper, i=j: ub - x[i]}
                 cons.append(l)
                 cons.append(u)
             options = {"maxiter": 500, "catol": 1e-6, "tol": 1e-6, "rhobeg": 0.2}
             bounds = None
         else:
-            bounds = self.xlimits
+            bounds = self.design_space.get_num_bounds()
             method = "SLSQP"
             cons = ()
             options = {"maxiter": 200}
 
         if criterion == "EI":
             self.obj_k = lambda x: -self.EI(np.atleast_2d(x), enable_tunneling, x_data)
         elif criterion == "SBO":
```

### Comparing `smt-2.0b2/smt/applications/mfk.py` & `smt-2.0b3/smt/applications/mfk.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,15 +426,15 @@
 
         # scaled predictor
         if descale:
             mu = mu * self.y_std + self.y_mean
 
         return mu[:, -1].reshape((n_eval, 1))
 
-    def _predict_values(self, X):
+    def _predict_values(self, X, is_acting=None):
         """
         Evaluates the model at a set of points.
 
         Arguments
         ---------
         x : np.ndarray [n_evals, dim]
             Evaluation point input variable values
@@ -443,15 +443,15 @@
         -------
         y : np.ndarray
             Evaluation point output variable values
         """
 
         return self._predict_intermediate_values(X, self.nlvl)
 
-    def _predict_variances(self, X):
+    def _predict_variances(self, X: np.ndarray, is_acting=None) -> np.ndarray:
         """
         Evaluates the model at a set of points.
 
         Arguments
         ---------
         x : np.ndarray [n_evals, dim]
             Evaluation point input variable values
```

### Comparing `smt-2.0b2/smt/applications/mfkpls.py` & `smt-2.0b3/smt/applications/mfkpls.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/applications/mfkplsk.py` & `smt-2.0b3/smt/applications/mfkplsk.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/applications/mixed_integer.py` & `smt-2.0b3/smt/surrogate_models/mgp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,471 +1,530 @@
 """
-Author: Remi Lafage <remi.lafage@onera.fr>
+Author: Remy Priem (remy.priem@onera.fr)
 
 This package is distributed under New BSD license.
 """
 
-from smt.surrogate_models.surrogate_model import SurrogateModel
-from smt.sampling_methods.sampling_method import SamplingMethod
-from smt.utils.checks import ensure_2d_array
-from smt.utils.mixed_integer import (
-    cast_to_discrete_values,
-    cast_to_enum_value,
-    cast_to_mixed_integer,
-    encode_with_enum_index,
-    fold_with_enum_index,
-    unfold_with_enum_mask,
-    unfold_xlimits_with_continuous_limits,
-)
-from smt.surrogate_models.krg_based import KrgBased, MixIntKernelType
-from smt.utils.mixed_integer import XType
-from smt.utils.kriging import XRole
-import warnings
-
-
-class MixedIntegerSamplingMethod(SamplingMethod):
-    """
-    Sampling method decorator that takes an SMT continuous sampling method and
-    cast values according x types specification to implement a sampling method
-    handling integer (ORD) or categorical (ENUM) features
-    """
+from __future__ import division
+import numpy as np
+from scipy import linalg
+
+from smt.utils.kriging import differences, componentwise_distance
+from smt.surrogate_models.krg_based import KrgBased
+from smt.utils.checks import check_support, check_nx, ensure_2d_array
 
-    def __init__(self, sampling_method_class, xspecs, **kwargs):
-        """
-        Parameters
-        ----------
-        sampling_method_class: class name
-            SMT sampling method class
-        kwargs: options of the given sampling method
-            options used to instanciate the SMT sampling method
-            with the additional 'output_in_folded_space' boolean option
-            specifying if doe output should be in folded space (enum indexes)
-            or not (enum masks)
-        """
-        super()
-        self._xspecs = xspecs
-        self._unfolded_xlimits = unfold_xlimits_with_continuous_limits(self._xspecs)
-        self._output_in_folded_space = kwargs.get("output_in_folded_space", True)
-        kwargs.pop("output_in_folded_space", None)
-        self._sampling_method = sampling_method_class(
-            xlimits=self._unfolded_xlimits, **kwargs
-        )
+"""
+The Active kriging class.
+"""
 
-    def _compute(self, nt):
-        doe = self._sampling_method(nt)
-        unfold_xdoe = cast_to_discrete_values(self._xspecs, True, doe)
-        if self._output_in_folded_space:
-            return fold_with_enum_index(self._xspecs.types, unfold_xdoe)
-        else:
-            return unfold_xdoe
 
-    def __call__(self, nt):
-        return self._compute(nt)
+class MGP(KrgBased):
+    name = "MGP"
 
-    def expand_lhs(self, x, nt, method="basic"):
-        doe = self._sampling_method(nt)
-        unfold_xdoe = cast_to_discrete_values(self._xspecs, True, doe)
-        if self._output_in_folded_space:
-            return fold_with_enum_index(self._xspecs.types, unfold_xdoe)
-        else:
-            return unfold_xdoe
+    def _initialize(self):
+        """
+        Initialized MGP
 
+        """
+        super(MGP, self)._initialize()
+        declare = self.options.declare
+        declare("n_comp", 1, types=int, desc="Number of active dimensions")
+        declare(
+            "prior",
+            {"mean": [0.0], "var": 5.0 / 4.0},
+            types=dict,
+            desc="Parameters for Gaussian prior of the Hyperparameters",
+        )
+        self.options["hyper_opt"] = "TNC"
+        self.options["corr"] = "act_exp"
 
-class MixedIntegerSurrogateModel(SurrogateModel):
-    """
-    Surrogate model (not Kriging) decorator that takes an SMT continuous surrogate model and
-    cast values according x types specification to implement a surrogate model
-    handling integer (ORD) or categorical (ENUM) features
-    """
-
-    def __init__(
-        self,
-        xspecs,
-        surrogate,
-        input_in_folded_space=True,
-    ):
+    def _componentwise_distance(self, dx, small=False, opt=0):
         """
-        Parameters
-        ----------
-        xspecs : x specifications XSpecs
-            xtypes: x types list
-                x types specification: list of either FLOAT, ORD or (ENUM, n) spec.
-            xlimits: array-like
-                bounds of x features
-            xroles: x roles list
-                x roles specification
-        surrogate: SMT surrogate model (not Kriging)
-            instance of a SMT surrogate model
-        input_in_folded_space: bool
-            whether x data are in given in folded space (enum indexes) or not (enum masks)
-        categorical_kernel: string
-            the kernel to use for categorical inputs. Only for non continuous Kriging.
-        """
-        super().__init__()
-        self._surrogate = surrogate
-
-        if isinstance(self._surrogate, KrgBased):
-            raise ValueError(
-                "Using MixedIntegerSurrogateModel integer model with "
-                + str(self._surrogate.name)
-                + " is not supported. Please use MixedIntegerKrigingModel instead."
-            )
-        self._xspecs = xspecs
-        if XRole.META in xspecs.roles:
-            raise ValueError(
-                "Using MixedIntegerSurrogateModel integer model with hierarchical variables is not supported. Please use MixedIntegerKrigingModel instead."
-            )
+        Compute the componentwise distance with respect to the correlation kernel
 
-        self._input_in_folded_space = input_in_folded_space
-        self.supports = self._surrogate.supports
-        self.options["print_global"] = False
-
-        if "poly" in self._surrogate.options:
-            if self._surrogate.options["poly"] != "constant":
-                raise ValueError("constant regression must be used with mixed integer")
-
-    @property
-    def name(self):
-        return "MixedInteger" + self._surrogate.name
 
-    def _initialize(self):
-        self.supports["derivatives"] = False
+        Parameters
+        ----------
+        dx : numpy.ndarray
+            Distance matrix.
+        small : bool, optional
+            Compute the componentwise distance in small (n_components) dimension
+            or in initial dimension. The default is False.
+        opt : int, optional
+            useless for MGP
 
-    def set_training_values(self, xt, yt, name=None):
-        xt = ensure_2d_array(xt, "xt")
-        if self._input_in_folded_space:
-            xt2 = unfold_with_enum_mask(self._xspecs.types, xt)
-        else:
-            xt2 = xt
-        xt2 = cast_to_discrete_values(self._xspecs, True, xt2)
-        super().set_training_values(xt2, yt)
-        self._surrogate.set_training_values(xt2, yt, name)
-
-    def update_training_values(self, yt, name=None):
-        super().update_training_values(yt, name)
-        self._surrogate.update_training_values(yt, name)
-
-    def _train(self):
-        self._surrogate._train()
-
-    def predict_values(self, x):
-        xp = ensure_2d_array(x, "xp")
-        if self._input_in_folded_space:
-            x2 = unfold_with_enum_mask(self._xspecs.types, xp)
-        else:
-            x2 = xp
-        return self._surrogate.predict_values(
-            cast_to_discrete_values(self._xspecs, True, x2)
-        )
+        Returns
+        -------
+        d : numpy.ndarray
+            Component wise distance.
 
-    def predict_variances(self, x):
-        xp = ensure_2d_array(x, "xp")
-        if self._input_in_folded_space:
-            x2 = unfold_with_enum_mask(self._xspecs.types, xp)
+        """
+        if small:
+            d = componentwise_distance(dx, self.options["corr"], self.options["n_comp"])
         else:
-            x2 = xp
-        return self._surrogate.predict_variances(
-            cast_to_discrete_values(self._xspecs, True, x2)
-        )
-
-    def _predict_values(self, x):
-        pass
-
+            d = componentwise_distance(dx, self.options["corr"], self.nx)
+        return d
 
-class MixedIntegerKrigingModel(KrgBased):
-    """
-    Kriging model decorator that takes an SMT continuous surrogate model and
-    cast values according x types specification to implement a surrogate model
-    handling integer (ORD) or categorical (ENUM) features
-    """
-
-    def __init__(
-        self,
-        surrogate,
-        input_in_folded_space=True,
-    ):
+    def _predict_values(self, x, is_acting=None):
         """
+        Predict the value of the MGP for a given point
+
         Parameters
         ----------
-        xspecs : x specifications XSpecs
-            xtypes: x types list
-                x types specification: list of either FLOAT, ORD or (ENUM, n) spec.
-            xlimits: array-like
-                bounds of x features
-            xroles: x roles list
-                x roles specification
-        surrogate: SMT Kriging surrogate model
-            instance of a SMT Kriging surrogate model
-        """
-        super().__init__()
-        self._surrogate = surrogate
-        if not (isinstance(self._surrogate, KrgBased)):
-            raise ValueError(
-                "Using MixedIntegerKrigingModel integer model with "
-                + str(self._surrogate.name)
-                + " is not supported. Please use MixedIntegerSurrogateModel instead."
-            )
-        self._xspecs = self._surrogate.options["xspecs"]
+        x : numpy.ndarray
+            Point to compute.
 
-        self._input_in_folded_space = input_in_folded_space
-        self.supports = self._surrogate.supports
-        self.options["print_global"] = False
-
-        if "poly" in self._surrogate.options:
-            if self._surrogate.options["poly"] != "constant":
-                raise ValueError("constant regression must be used with mixed integer")
-
-        if (XRole.META in self._xspecs.roles) and self._surrogate.options[
-            "categorical_kernel"
-        ] is None:
-            self._surrogate.options[
-                "categorical_kernel"
-            ] = MixIntKernelType.HOMO_HSPHERE
-            warnings.warn(
-                "Using MixedIntegerSurrogateModel integer model with Continuous Relaxation is not supported. Switched to homoscedastic hypersphere kernel instead."
-            )
-        if self._surrogate.options["categorical_kernel"] is not None:
-            self._input_in_folded_space = False
+        Raises
+        ------
+        ValueError
+            The number fo dimension is not good.
 
-    @property
-    def name(self):
-        return "MixedInteger" + self._surrogate.name
-
-    def _initialize(self):
-        super()._initialize()
-        self.supports["derivatives"] = False
-
-    def set_training_values(self, xt, yt, name=None):
-        xt = ensure_2d_array(xt, "xt")
-        if self._input_in_folded_space:
-            xt2 = unfold_with_enum_mask(self._xspecs.types, xt)
+        Returns
+        -------
+        y : numpy.ndarray
+            Value of the MGP at the given point x.
+        """
+        n_eval, n_features = x.shape
+        if n_features < self.nx:
+            if n_features != self.options["n_comp"]:
+                raise ValueError(
+                    "dim(u) should be equal to %i" % self.options["n_comp"]
+                )
+            theta = np.eye(self.options["n_comp"]).reshape(
+                (self.options["n_comp"] ** 2,)
+            )
+            # Get pairwise componentwise L1-distances to the input training set
+            u = x
+            x = self.get_x_from_u(u)
+
+            u = u * self.embedding["norm"] - self.U_mean
+            du = differences(u, Y=self.U_norma.copy())
+            d = self._componentwise_distance(du, small=True)
+
+            # Get an approximation of x
+            x = (x - self.X_offset) / self.X_scale
+            dx = differences(x, Y=self.X_norma.copy())
+            d_x = self._componentwise_distance(dx)
         else:
-            xt2 = xt
-        xt2 = cast_to_discrete_values(
-            self._xspecs, (self._surrogate.options["categorical_kernel"] == None), xt2
+            if n_features != self.nx:
+                raise ValueError("dim(x) should be equal to %i" % self.X_scale.shape[0])
+            theta = self.optimal_theta
+
+            # Get pairwise componentwise L1-distances to the input training set
+            x = (x - self.X_offset) / self.X_scale
+            dx = differences(x, Y=self.X_norma.copy())
+            d = self._componentwise_distance(dx)
+            d_x = None
+
+        # Compute the correlation function
+        r = self._correlation_types[self.options["corr"]](theta, d, d_x=d_x).reshape(
+            n_eval, self.nt
         )
-        super().set_training_values(xt2, yt)
-        self._surrogate.set_training_values(xt2, yt, name)
 
-    def update_training_values(self, yt, name=None):
-        super().update_training_values(yt, name)
-        self._surrogate.update_training_values(yt, name)
-
-    def _train(self):
-        self._surrogate._train()
-
-    def predict_values(self, x):
-        xp = ensure_2d_array(x, "xp")
-        if self._input_in_folded_space:
-            x2 = unfold_with_enum_mask(self._xspecs.types, xp)
-        else:
-            x2 = xp
-        return self._surrogate.predict_values(
-            cast_to_discrete_values(
-                self._xspecs,
-                (self._surrogate.options["categorical_kernel"] == None),
-                x2,
-            )
-        )
+        f = self._regression_types[self.options["poly"]](x)
+        # Scaled predictor
+        y_ = np.dot(f, self.optimal_par["beta"]) + np.dot(r, self.optimal_par["gamma"])
+        # Predictor
+        y = (self.y_mean + self.y_std * y_).ravel()
+        return y
+
+    def _predict_mgp_variances_base(self, x):
+        """Base computation of MGP MSE used by predict_variances and predict_variances_no_uq"""
+        _, n_features = x.shape
+
+        if n_features < self.nx:
+            if n_features != self.options["n_comp"]:
+                raise ValueError(
+                    "dim(u) should be equal to %i" % self.options["n_comp"]
+                )
+            u = x
+            x = self.get_x_from_u(u)
 
-    def predict_variances(self, x):
-        xp = ensure_2d_array(x, "xp")
-        if self._input_in_folded_space:
-            x2 = unfold_with_enum_mask(self._xspecs.types, xp)
+            u = u * self.embedding["norm"] - self.U_mean
+            x = (x - self.X_offset) / self.X_scale
         else:
-            x2 = xp
-        return self._surrogate.predict_variances(
-            cast_to_discrete_values(
-                self._xspecs,
-                (self._surrogate.options["categorical_kernel"] == None),
-                x2,
-            )
-        )
+            if n_features != self.nx:
+                raise ValueError("dim(x) should be equal to %i" % self.X_scale.shape[0])
+            u = None
+            x = (x - self.X_offset) / self.X_scale
 
-    def _predict_values(self, x):
-        pass
+        dy = self._predict_value_derivatives_hyper(x, u)
+        dMSE, MSE = self._predict_variance_derivatives_hyper(x, u)
 
+        return MSE, dy, dMSE
 
-class MixedIntegerContext(object):
-    """
-    Class which acts as sampling method and surrogate model factory
-    to handle integer and categorical variables consistently.
-    """
-
-    def __init__(self, xspecs, work_in_folded_space=True):
+    def _predict_variances(self, x: np.ndarray, is_acting=None) -> np.ndarray:
         """
+        Predict the variance of a specific point
+
         Parameters
         ----------
-        xspecs : x specifications XSpecs
-            xtypes: x types list
-                x types specification: list of either FLOAT, ORD or (ENUM, n) spec.
-            xlimits: array-like
-                bounds of x features
-            xroles: x roles list
-                x roles specification
-        work_in_folded_space: bool
-            whether x data are in given in folded space (enum indexes) or not (enum masks)
-        categorical_kernel: string
-            the kernel to use for categorical inputs. Only for non continuous Kriging.
-        """
-
-        self._xspecs = xspecs
-        self._unfold_space = not work_in_folded_space
-        self._unfolded_xlimits = unfold_xlimits_with_continuous_limits(
-            self._xspecs, unfold_space=self._unfold_space
-        )
-        self._work_in_folded_space = work_in_folded_space
+        x : numpy.ndarray
+            Point to compute.
 
-    def build_sampling_method(self, sampling_method_class, **kwargs):
-        """
-        Build MixedIntegerSamplingMethod from given SMT sampling method.
-        """
-        kwargs["output_in_folded_space"] = self._work_in_folded_space
-        return MixedIntegerSamplingMethod(sampling_method_class, self._xspecs, **kwargs)
-
-    def build_kriging_model(self, surrogate):
-        """
-        Build MixedIntegerKrigingModel from given SMT surrogate model.
-        """
-        surrogate.options["xspecs"] = self._xspecs
-        return MixedIntegerKrigingModel(
-            surrogate=surrogate,
-            input_in_folded_space=self._work_in_folded_space,
-        )
+        Raises
+        ------
+        ValueError
+            The number fo dimension is not good.
 
-    def build_surrogate_model(self, surrogate):
-        """
-        Build MixedIntegerKrigingModel from given SMT surrogate model.
+        Returns
+        -------
+        numpy.nd array
+            MSE.
         """
-        return MixedIntegerSurrogateModel(
-            self._xspecs,
-            surrogate=surrogate,
-            input_in_folded_space=self._work_in_folded_space,
+        MSE, dy, dMSE = self._predict_mgp_variances_base(x)
+        arg_1 = np.einsum("ij,ij->i", dy.T, linalg.solve(self.inv_sigma_R, dy).T)
+        arg_2 = np.einsum("ij,ij->i", dMSE.T, linalg.solve(self.inv_sigma_R, dMSE).T)
+
+        MGPMSE = np.zeros(x.shape[0])
+        MGPMSE[MSE != 0] = (
+            (4.0 / 3.0) * MSE[MSE != 0]
+            + arg_1[MSE != 0]
+            + (1.0 / (3.0 * MSE[MSE != 0])) * arg_2[MSE != 0]
         )
+        MGPMSE[MGPMSE < 0.0] = 0.0
+        return MGPMSE
 
-    def get_unfolded_xlimits(self):
-        """
-        Returns relaxed xlimits
-        Each level of an enumerate gives a new continuous dimension in [0, 1].
-        Each integer dimensions are relaxed continuously.
-        """
-
-        return self._unfolded_xlimits
+    def predict_variances_no_uq(self, x):
+        """Like predict_variances but without taking account hyperparameters uncertainty"""
+        check_support(self, "variances")
+        x = ensure_2d_array(x, "x")
+        self._check_xdim(x)
+        n = x.shape[0]
+        x2 = np.copy(x)
+        s2, _, _ = self._predict_mgp_variances_base(x)
+        s2[s2 < 0.0] = 0.0
+        return s2.reshape((n, self.ny))
+
+    def _check_xdim(self, x):
+        _, n_features = x.shape
+        nx = self.nx
+        if n_features < self.nx:
+            nx = self.options["n_comp"]
+        check_nx(nx, x)
 
-    def get_unfolded_dimension(self):
+    def _reduced_log_prior(self, theta, grad=False, hessian=False):
         """
-        Returns x dimension (int) taking into account  unfolded categorical features
-        """
-
-        return len(self._unfolded_xlimits)
-
-    def cast_to_discrete_values(self, x, unfold_space):
-        """
-        Project continuously relaxed values to their closer assessable values.
-        Note: categorical (or enum) x dimensions are still expanded that is
-        there are still as many columns as categorical possible values for the given x dimension.
-        For instance, if an input dimension is typed ["blue", "red", "green"] in xlimits a sample/row of
-        the input x may contain the values (or mask) [..., 0, 0, 1, ...] to specify "green" for
-        this original dimension.
+        Compute the reduced log prior at given hyperparameters
 
         Parameters
         ----------
-        x : np.ndarray [n_evals, dim]
-            continuous evaluation point input variable values
-        unfold_space : boolean
-            whether or not working in the continuous relaxation folded space
+        theta : numpy.ndarray
+            Hyperparameters.
+        grad : bool, optional
+            True to compuyte gradient. The default is False.
+        hessian : bool, optional
+            True to compute hessian. The default is False.
+
         Returns
         -------
-        np.ndarray
-            feasible evaluation point value in categorical space.
+        res : numpy.ndarray
+            Value, gradient, hessian of the reduced log prior.
+
         """
-        return cast_to_discrete_values(self._xspecs, unfold_space, x)
+        nb_theta = len(theta)
+
+        if theta.ndim < 2:
+            theta = np.atleast_2d(theta).T
 
-    def fold_with_enum_index(self, x):
+        mean = np.ones((nb_theta, 1)) * self.options["prior"]["mean"]
+        sig_inv = np.eye(nb_theta) / self.options["prior"]["var"]
+
+        if grad:
+            sig_inv_m = np.atleast_2d(np.sum(sig_inv, axis=0)).T
+            res = -2.0 * (theta - mean) * sig_inv_m
+        elif hessian:
+            res = -2.0 * np.atleast_2d(np.sum(sig_inv, axis=0)).T
+        else:
+            res = -np.dot((theta - mean).T, sig_inv.dot(theta - mean))
+        return res
+
+    def _predict_value_derivatives_hyper(self, x, u=None):
         """
-        Reduce categorical inputs from discrete unfolded space to
-        initial x dimension space where categorical x dimensions are valued by the index
-        in the corresponding enumerate list.
-        For instance, if an input dimension is typed ["blue", "red", "green"] a sample/row of
-        the input x may contain the mask [..., 0, 0, 1, ...] which will be contracted in [..., 2, ...]
-        meaning the "green" value.
-        This function is the opposite of unfold_with_enum_mask().
+        Compute the derivatives of the mean of the GP with respect to the hyperparameters
 
         Parameters
         ----------
-        x: np.ndarray [n_evals, dim]
-            continuous evaluation point input variable values
+        x : numpy.ndarray
+            Point to compute in initial dimension.
+        u : numpy.ndarray, optional
+            Point to compute in small dimension. The default is None.
 
         Returns
         -------
-        np.ndarray [n_evals, dim]
-            evaluation point input variable values with enumerate index for categorical variables
+        dy : numpy.ndarray
+            Derivatives of the mean of the GP with respect to the hyperparameters.
+
         """
-        return fold_with_enum_index(self._xspecs.types, x)
+        # Initialization
+        n_eval, _ = x.shape
+
+        # Get pairwise componentwise L1-distances to the input training set
+        dx = differences(x, Y=self.X_norma.copy())
+        d_x = self._componentwise_distance(dx)
+        if u is not None:
+            theta = np.eye(self.options["n_comp"]).reshape(
+                (self.options["n_comp"] ** 2,)
+            )
+
+            # Get pairwise componentwise L1-distances to the input training set
+            du = differences(u, Y=self.U_norma.copy())
+            d = self._componentwise_distance(du, small=True)
+        else:
+            theta = self.optimal_theta
+
+            # Get pairwise componentwise L1-distances to the input training set
+            d = d_x
+            d_x = None
+
+        # Compute the correlation function
+        r = self._correlation_types[self.options["corr"]](theta, d, d_x=d_x).reshape(
+            n_eval, self.nt
+        )
+        # Compute the regression function
+        f = self._regression_types[self.options["poly"]](x)
+
+        dy = np.zeros((len(self.optimal_theta), n_eval))
 
-    def unfold_with_enum_mask(self, x):
+        gamma = self.optimal_par["gamma"]
+        Rinv_dR_gamma = self.optimal_par["Rinv_dR_gamma"]
+        Rinv_dmu = self.optimal_par["Rinv_dmu"]
+
+        for omega in range(len(self.optimal_theta)):
+            drdomega = self._correlation_types[self.options["corr"]](
+                theta, d, grad_ind=omega, d_x=d_x
+            ).reshape(n_eval, self.nt)
+
+            dbetadomega = self.optimal_par["dbeta_all"][omega]
+
+            dy_omega = (
+                f.dot(dbetadomega)
+                + drdomega.dot(gamma)
+                - r.dot(Rinv_dR_gamma[omega] + Rinv_dmu[omega])
+            )
+
+            dy[omega, :] = dy_omega[:, 0]
+
+        return dy
+
+    def _predict_variance_derivatives_hyper(self, x, u=None):
         """
-        Expand categorical inputs from initial x dimension space where categorical x dimensions
-        are valued by the index in the corresponding enumerate list to the discrete unfolded space.
-        For instance, if an input dimension is typed ["blue", "red", "green"] a sample/row of
-        the input x may contain [..., 2, ...] which will be expanded in [..., 0, 0, 1, ...].
-        This function is the opposite of fold_with_enum_index().
+        Compute the derivatives of the variance of the GP with respect to the hyperparameters
 
         Parameters
         ----------
-        x: np.ndarray [n_evals, nx]
-            continuous evaluation point input variable values
+        x : numpy.ndarray
+            Point to compute in initial dimension.
+        u : numpy.ndarray, optional
+            Point to compute in small dimension. The default is None.
 
         Returns
         -------
-        np.ndarray [n_evals, nx continuous]
-            evaluation point input variable values with enumerate index for categorical variables
+        dMSE : numpy.ndarrray
+            derivatives of the variance of the GP with respect to the hyperparameters.
+        MSE : TYPE
+            Variance of the GP.
+
         """
-        return unfold_with_enum_mask(self._xspecs.types, x)
+        # Initialization
+        n_eval, n_features_x = x.shape
+
+        # Get pairwise componentwise L1-distances to the input training set
+        dx = differences(x, Y=self.X_norma.copy())
+        d_x = self._componentwise_distance(dx)
+        if u is not None:
+            theta = np.eye(self.options["n_comp"]).reshape(
+                (self.options["n_comp"] ** 2,)
+            )
+            # Get pairwise componentwise L1-distances to the input training set
+            du = differences(u, Y=self.U_norma.copy())
+            d = self._componentwise_distance(du, small=True)
+        else:
+            theta = self.optimal_theta
+            # Get pairwise componentwise L1-distances to the input training set
+            d = d_x
+            d_x = None
+
+        # Compute the correlation function
+        r = (
+            self._correlation_types[self.options["corr"]](theta, d, d_x=d_x)
+            .reshape(n_eval, self.nt)
+            .T
+        )
+        f = self._regression_types[self.options["poly"]](x).T
+
+        C = self.optimal_par["C"]
+        G = self.optimal_par["G"]
+        Ft = self.optimal_par["Ft"]
+        sigma2 = self.optimal_par["sigma2"]
+
+        rt = linalg.solve_triangular(C, r, lower=True)
+
+        F_Rinv_r = np.dot(Ft.T, rt)
+
+        u_ = linalg.solve_triangular(G.T, f - F_Rinv_r)
+
+        MSE = self.optimal_par["sigma2"] * (
+            1.0 - (rt**2.0).sum(axis=0) + (u_**2.0).sum(axis=0)
+        )
+        # Mean Squared Error might be slightly negative depending on
+        # machine precision: force to zero!
+        MSE[MSE < 0.0] = 0.0
+
+        Ginv_u = linalg.solve_triangular(G, u_, lower=False)
+        Rinv_F = linalg.solve_triangular(C.T, Ft, lower=False)
+        Rinv_r = linalg.solve_triangular(C.T, rt, lower=False)
+        Rinv_F_Ginv_u = Rinv_F.dot(Ginv_u)
+
+        dMSE = np.zeros((len(self.optimal_theta), n_eval))
+
+        dr_all = self.optimal_par["dr"]
+        dsigma = self.optimal_par["dsigma"]
+
+        for omega in range(len(self.optimal_theta)):
+            drdomega = (
+                self._correlation_types[self.options["corr"]](
+                    theta, d, grad_ind=omega, d_x=d_x
+                )
+                .reshape(n_eval, self.nt)
+                .T
+            )
 
-    def cast_to_enum_value(self, x_col, enum_indexes):
+            dRdomega = np.zeros((self.nt, self.nt))
+            dRdomega[self.ij[:, 0], self.ij[:, 1]] = dr_all[omega][:, 0]
+            dRdomega[self.ij[:, 1], self.ij[:, 0]] = dr_all[omega][:, 0]
+
+            # Compute du2dtheta
+
+            dRdomega_Rinv_F_Ginv_u = dRdomega.dot(Rinv_F_Ginv_u)
+            r_Rinv_dRdomega_Rinv_F_Ginv_u = np.einsum(
+                "ij,ij->i", Rinv_r.T, dRdomega_Rinv_F_Ginv_u.T
+            )
+            drdomega_Rinv_F_Ginv_u = np.einsum("ij,ij->i", drdomega.T, Rinv_F_Ginv_u.T)
+            u_Ginv_F_Rinv_dRdomega_Rinv_F_Ginv_u = np.einsum(
+                "ij,ij->i", Rinv_F_Ginv_u.T, dRdomega_Rinv_F_Ginv_u.T
+            )
+
+            du2domega = (
+                2.0 * r_Rinv_dRdomega_Rinv_F_Ginv_u
+                - 2.0 * drdomega_Rinv_F_Ginv_u
+                + u_Ginv_F_Rinv_dRdomega_Rinv_F_Ginv_u
+            )
+            du2domega = np.atleast_2d(du2domega)
+
+            # Compute drt2dtheta
+            drdomega_Rinv_r = np.einsum("ij,ij->i", drdomega.T, Rinv_r.T)
+            r_Rinv_dRdomega_Rinv_r = np.einsum(
+                "ij,ij->i", Rinv_r.T, dRdomega.dot(Rinv_r).T
+            )
+
+            drt2domega = 2.0 * drdomega_Rinv_r - r_Rinv_dRdomega_Rinv_r
+            drt2domega = np.atleast_2d(drt2domega)
+
+            dMSE[omega] = dsigma[omega] * MSE / sigma2 + sigma2 * (
+                -drt2domega + du2domega
+            )
+
+        return dMSE, MSE
+
+    def get_x_from_u(self, u):
         """
-        Return enumerate levels from indexes for the given x feature specified by x_col.
+        Compute the point in initial dimension from a point in low dimension
 
         Parameters
         ----------
-        x_col: int
-            index of the feature typed as enum
-        enum_indexes: list
-            list of indexes in the possible values for the enum
+        u : numpy.ndarray
+            Point in low dimension.
 
         Returns
         -------
-            list of levels (labels) for the given enum feature
+        res : numpy.ndarray
+            point in initial dimension.
+
         """
-        return cast_to_enum_value(self._xspecs, x_col, enum_indexes)
+        u = np.atleast_2d(u)
+
+        self.embedding["Q_C"], self.embedding["R_C"]
+
+        x_temp = np.dot(
+            self.embedding["Q_C"],
+            linalg.solve_triangular(self.embedding["R_C"].T, u.T, lower=True),
+        ).T
+
+        res = np.atleast_2d(x_temp)
+        return res
 
-    def cast_to_mixed_integer(self, x):
+    def get_u_from_x(self, x):
         """
-        Convert an x point with enum indexes to x point with enum levels
+        Compute the point in low dimension from a point in initial dimension
 
         Parameters
         ----------
-        x: array-like
-            point to convert
+        x : numpy.ndarray
+            Point in initial dimension.
 
         Returns
         -------
-            x as a list with enum levels if any
+        u : numpy.ndarray
+             Point in low dimension.
+
         """
-        return cast_to_mixed_integer(self._xspecs, x)
+        u = x.dot(self.embedding["C"])
+        return u
 
-    def encode_with_enum_index(self, x):
+    def _specific_train(self):
+        """
+        Compute the specific training values necessary for MGP (Hessian)
         """
-        Convert an x point with enum levels to x point with enum indexes
+        # Compute covariance matrix of hyperparameters
+        var_R = np.zeros((len(self.optimal_theta), len(self.optimal_theta)))
+        r, r_ij, par = self._reduced_likelihood_hessian(self.optimal_theta)
+        var_R[r_ij[:, 0], r_ij[:, 1]] = r[:, 0]
+        var_R[r_ij[:, 1], r_ij[:, 0]] = r[:, 0]
 
-        Parameters
-        ----------
-        x as a list with enum levels if any
-            point to convert
-        Returns
-        -------
-        np.ndarray [n_evals, dim]
-            evaluation point input variable values with enumerate index for categorical variables
+        self.inv_sigma_R = -var_R
+
+        # Compute normalise embedding
+        self.optimal_par = par
+
+        A = np.reshape(self.optimal_theta, (self.options["n_comp"], self.nx)).T
+        B = (A.T / self.X_scale).T
+        norm_B = np.linalg.norm(B)
+        C = B / norm_B
+
+        self.embedding = {}
+        self.embedding["A"] = A
+        self.embedding["C"] = C
+        self.embedding["norm"] = norm_B
+        self.embedding["Q_C"], self.embedding["R_C"] = linalg.qr(C, mode="economic")
+
+        # Compute normalisation in embeding base
+        self.U_norma = self.X_norma.dot(A)
+        self.U_mean = self.X_offset.dot(C) * norm_B
+
+        # Compute best number of Components for Active Kriging
+        svd = linalg.svd(A)
+        svd_cumsum = np.cumsum(svd[1])
+        svd_sum = np.sum(svd[1])
+        self.best_ncomp = min(np.argwhere(svd_cumsum > 0.99 * svd_sum)) + 1
+
+    def _check_param(self):
         """
+        Overrides KrgBased implementation
+        This function checks some parameters of the model.
+        """
+
+        d = self.options["n_comp"] * self.nx
+
+        if self.options["corr"] != "act_exp":
+            raise ValueError("MGP must be used with act_exp correlation function")
+        if self.options["hyper_opt"] != "TNC":
+            raise ValueError("MGP must be used with TNC hyperparameters optimizer")
 
-        return encode_with_enum_index(self._specs, x)
+        if len(self.options["theta0"]) != d:
+            if len(self.options["theta0"]) == 1:
+                self.options["theta0"] *= np.ones(d)
+            else:
+                raise ValueError(
+                    "the number of dim %s should be equal to the length of theta0 %s."
+                    % (d, len(self.options["theta0"]))
+                )
```

### Comparing `smt-2.0b2/smt/applications/moe.py` & `smt-2.0b3/smt/applications/moe.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,18 +78,18 @@
         self._setup()
 
         for name in self.training_points:
             xt, yt = self.training_points[name][0]
             self.moe.set_training_values(xt, yt, name=name)
         self.moe.train()
 
-    def _predict_values(self, x: np.ndarray) -> np.ndarray:
+    def _predict_values(self, x: np.ndarray, is_acting=None) -> np.ndarray:
         return self.moe.predict_values(x)
 
-    def _predict_variances(self, x: np.ndarray) -> np.ndarray:
+    def _predict_variances(self, x: np.ndarray, is_acting=None) -> np.ndarray:
         return self.moe.predict_variances(x)
 
 
 class MOE(SurrogateBasedApplication):
     # Names of experts available to be part of the mixture
     AVAILABLE_EXPERTS = [
         name
```

### Comparing `smt-2.0b2/smt/applications/vfm.py` & `smt-2.0b3/smt/applications/vfm.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/__init__.py` & `smt-2.0b3/smt/problems/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,11 +9,12 @@
 from .water_flow import WaterFlow
 from .water_flow_lfidelity import WaterFlowLFidelity
 from .welded_beam import WeldedBeam
 from .wing_weight import WingWeight
 from .ndim_cantilever_beam import NdimCantileverBeam
 from .mixed_cantilever_beam import MixedCantileverBeam
 from .neural_network import HierarchicalNeuralNetwork
+from .hierarchical_goldstein import HierarchicalGoldstein
 from .ndim_robot_arm import NdimRobotArm
 from .ndim_rosenbrock import NdimRosenbrock
 from .ndim_step_function import NdimStepFunction
 from .lp_norm import LpNorm
```

### Comparing `smt-2.0b2/smt/problems/branin.py` & `smt-2.0b3/smt/problems/branin.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/cantilever_beam.py` & `smt-2.0b3/smt/problems/cantilever_beam.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/lp_norm.py` & `smt-2.0b3/smt/problems/lp_norm.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/mixed_cantilever_beam.py` & `smt-2.0b3/smt/problems/mixed_cantilever_beam.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Cantilever beam problem from:
 P. Saves, Y. Diouane, N. Bartoli, T. Lefebvre, and J. Morlier. A mixed-categorical correlation kernel for gaussian process, 2022
 """
 import numpy as np
 
 from smt.problems.problem import Problem
+from smt.utils.design_space import DesignSpace, FloatVariable, CategoricalVariable
 
 
 class MixedCantileverBeam(Problem):
     def _initialize(self):
         self.options.declare("name", "MixedCantileverBeam", types=str)
         self.options.declare("P", 50e3, types=(int, float), desc="Tip load (50 kN)")
         self.options.declare(
@@ -31,14 +32,24 @@
             0.136,
             0.360,
             0.0922,
             0.138,
             0.369,
         ]
 
+        self._set_design_space(
+            DesignSpace(
+                [
+                    CategoricalVariable(values=[str(i + 1) for i in range(12)]),
+                    FloatVariable(10.0, 20.0),
+                    FloatVariable(1.0, 2.0),
+                ]
+            )
+        )
+
     def _evaluate(self, x, kx=0):
         """
         Arguments
         ---------
         x : ndarray[ne, nx]
             Evaluation points.
```

### Comparing `smt-2.0b2/smt/problems/ndim_cantilever_beam.py` & `smt-2.0b3/smt/problems/ndim_cantilever_beam.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from smt.problems.problem import Problem
 from smt.problems.reduced_problem import ReducedProblem
 from smt.problems.cantilever_beam import CantileverBeam
 
 
 class NdimCantileverBeam(Problem):
     def __init__(self, ndim=1, w=0.2):
+        super().__init__()
         self.problem = ReducedProblem(
             CantileverBeam(ndim=3 * ndim), np.arange(1, 3 * ndim, 3), w=w
         )
 
         self.options = OptionsDictionary()
         self.options.declare("ndim", ndim, types=int)
         self.options.declare("return_complex", False, types=bool)
```

### Comparing `smt-2.0b2/smt/problems/ndim_robot_arm.py` & `smt-2.0b3/smt/problems/ndim_robot_arm.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from smt.problems.problem import Problem
 from smt.problems.reduced_problem import ReducedProblem
 from smt.problems.robot_arm import RobotArm
 
 
 class NdimRobotArm(Problem):
     def __init__(self, ndim=1, w=0.2):
+        super().__init__()
         self.problem = ReducedProblem(
             RobotArm(ndim=2 * (ndim + 1)), np.arange(3, 2 * (ndim + 1), 2), w=w
         )
 
         self.options = OptionsDictionary()
         self.options.declare("ndim", ndim, types=int)
         self.options.declare("return_complex", False, types=bool)
```

### Comparing `smt-2.0b2/smt/problems/ndim_rosenbrock.py` & `smt-2.0b3/smt/problems/ndim_rosenbrock.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from smt.problems.problem import Problem
 from smt.problems.reduced_problem import ReducedProblem
 from smt.problems.rosenbrock import Rosenbrock
 
 
 class NdimRosenbrock(Problem):
     def __init__(self, ndim=1, w=0.2):
+        super().__init__()
         self.problem = ReducedProblem(
             Rosenbrock(ndim=ndim + 1), np.arange(1, ndim + 1), w=w
         )
 
         self.options = OptionsDictionary()
         self.options.declare("ndim", ndim, types=int)
         self.options.declare("return_complex", False, types=bool)
```

### Comparing `smt-2.0b2/smt/problems/ndim_step_function.py` & `smt-2.0b3/smt/problems/ndim_step_function.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from smt.utils.options_dictionary import OptionsDictionary
 from smt.problems.problem import Problem
 from smt.problems.tensor_product import TensorProduct
 
 
 class NdimStepFunction(Problem):
     def __init__(self, ndim=1, width=10.0):
+        super().__init__()
         self.problem = TensorProduct(ndim=ndim, func="tanh", width=width)
 
         self.options = OptionsDictionary()
         self.options.declare("ndim", ndim, types=int)
         self.options.declare("return_complex", False, types=bool)
         self.options.declare("name", "NdimStepFunction", types=str)
```

### Comparing `smt-2.0b2/smt/problems/reduced_problem.py` & `smt-2.0b3/smt/problems/reduced_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             Pointer to the Problem object being wrapped.
         dims : int or list/tuple of ints
             Either the number of dimensions or a list of the dimension indices that this
             problem uses.
         w : float
             The value to use for all unaccounted for inputs where 0/1 is lower/upper bound.
         """
+        super().__init__()
         self.problem = problem
         self.w = w
 
         if isinstance(dims, int):
             self.dims = np.arange(dims)
             assert dims <= problem.options["ndim"]
         elif isinstance(dims, (list, tuple, np.ndarray)):
```

### Comparing `smt-2.0b2/smt/problems/robot_arm.py` & `smt-2.0b3/smt/problems/robot_arm.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/rosenbrock.py` & `smt-2.0b3/smt/problems/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/sphere.py` & `smt-2.0b3/smt/problems/sphere.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/tensor_product.py` & `smt-2.0b3/smt/problems/tensor_product.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/torsion_vibration.py` & `smt-2.0b3/smt/problems/torsion_vibration.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/water_flow.py` & `smt-2.0b3/smt/problems/water_flow.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/water_flow_lfidelity.py` & `smt-2.0b3/smt/problems/water_flow_lfidelity.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/welded_beam.py` & `smt-2.0b3/smt/problems/welded_beam.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/problems/wing_weight.py` & `smt-2.0b3/smt/problems/wing_weight.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/sampling_methods/full_factorial.py` & `smt-2.0b3/smt/sampling_methods/full_factorial.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/sampling_methods/lhs.py` & `smt-2.0b3/smt/sampling_methods/lhs.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/sampling_methods/random.py` & `smt-2.0b3/smt/sampling_methods/random.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/sampling_methods/sampling_method.py` & `smt-2.0b3/smt/sampling_methods/sampling_method.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/idw/idw.cpp` & `smt-2.0b3/smt/src/idw/idw.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/idw/idwclib.cpp` & `smt-2.0b3/smt/src/idw/idwclib.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
             "smt\\src\\idw\\idw.hpp"
         ],
         "include_dirs": [
             "smt/src/idw",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include"
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include"
         ],
         "language": "c++",
         "name": "smt.surrogate_models.idwclib",
         "sources": [
             "smt/src/idw/idwclib.pyx",
             "smt/src/idw/idw.cpp"
         ]
@@ -1070,195 +1070,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":689
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":690
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":691
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":692
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":696
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":697
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":698
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":699
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":703
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":704
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":713
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":714
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":715
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":717
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":718
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":719
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":721
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":722
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":724
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":725
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":726
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1290,42 +1290,42 @@
 /*--- Type declarations ---*/
 #ifndef _ARRAYARRAY_H
 struct arrayobject;
 typedef struct arrayobject arrayobject;
 #endif
 struct __pyx_obj_3smt_16surrogate_models_7idwclib_PyIDW;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":728
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":729
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":730
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":732
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3551,15 +3551,15 @@
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":734
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3568,29 +3568,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3601,15 +3601,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":737
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3618,29 +3618,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3651,15 +3651,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":740
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3668,29 +3668,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3701,15 +3701,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":743
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3718,29 +3718,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3751,15 +3751,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":746
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3768,29 +3768,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3801,212 +3801,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":749
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":928
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":932
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":934
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":936
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":940
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4022,15 +4022,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4038,53 +4038,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":941
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":943
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":944
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -4092,30 +4092,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":940
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4130,15 +4130,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":946
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4154,15 +4154,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4170,53 +4170,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":947
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":949
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":950
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -4224,30 +4224,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":946
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4262,15 +4262,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":952
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4286,15 +4286,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4302,53 +4302,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":953
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":955
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":956
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -4356,30 +4356,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":952
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4394,176 +4394,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":966
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":978
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":966
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":981
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":993
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":981
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":996
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":996
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1006
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1013
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4789,26 +4789,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(3, 950, __pyx_L1_error)
@@ -5211,15 +5211,15 @@
  * import numpy as np
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `smt-2.0b2/smt/src/idw/idwclib.pyx` & `smt-2.0b3/smt/src/idw/idwclib.pyx`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/rbf/rbf.cpp` & `smt-2.0b3/smt/src/rbf/rbf.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/rbf/rbfclib.cpp` & `smt-2.0b3/smt/src/rbf/rbfclib.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
             "smt\\src\\rbf\\rbf.hpp"
         ],
         "include_dirs": [
             "smt/src/rbf",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include"
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include"
         ],
         "language": "c++",
         "name": "smt.surrogate_models.rbfclib",
         "sources": [
             "smt/src/rbf/rbfclib.pyx",
             "smt/src/rbf/rbf.cpp"
         ]
@@ -1070,195 +1070,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":689
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":690
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":691
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":692
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":696
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":697
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":698
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":699
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":703
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":704
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":713
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":714
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":715
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":717
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":718
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":719
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":721
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":722
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":724
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":725
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":726
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1290,42 +1290,42 @@
 /*--- Type declarations ---*/
 #ifndef _ARRAYARRAY_H
 struct arrayobject;
 typedef struct arrayobject arrayobject;
 #endif
 struct __pyx_obj_3smt_16surrogate_models_7rbfclib_PyRBF;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":728
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":729
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":730
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":732
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3602,15 +3602,15 @@
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":734
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3619,29 +3619,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3652,15 +3652,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":737
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3669,29 +3669,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3702,15 +3702,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":740
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3719,29 +3719,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3752,15 +3752,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":743
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3769,29 +3769,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3802,15 +3802,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":746
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3819,29 +3819,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3852,212 +3852,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":749
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":928
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":932
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":934
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":936
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":940
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4073,15 +4073,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4089,53 +4089,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":941
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":943
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":944
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -4143,30 +4143,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":940
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4181,15 +4181,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":946
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4205,15 +4205,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4221,53 +4221,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":947
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":949
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":950
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -4275,30 +4275,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":946
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4313,15 +4313,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":952
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4337,15 +4337,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4353,53 +4353,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":953
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":955
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":956
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -4407,30 +4407,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":952
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4445,176 +4445,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":966
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":978
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":966
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":981
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":993
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":981
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":996
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":996
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1006
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1013
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4842,26 +4842,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(3, 950, __pyx_L1_error)
@@ -5264,15 +5264,15 @@
  * import numpy as np
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `smt-2.0b2/smt/src/rbf/rbfclib.pyx` & `smt-2.0b3/smt/src/rbf/rbfclib.pyx`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/rmts/rmtb.cpp` & `smt-2.0b3/smt/src/rmts/rmtb.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/rmts/rmtc.cpp` & `smt-2.0b3/smt/src/rmts/rmtc.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/rmts/rmtc.hpp` & `smt-2.0b3/smt/src/rmts/rmtc.hpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/rmts/rmts.cpp` & `smt-2.0b3/smt/src/rmts/rmts.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/rmts/rmts.hpp` & `smt-2.0b3/smt/src/rmts/rmts.hpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/rmts/rmtsclib.cpp` & `smt-2.0b3/smt/src/rmts/rmtsclib.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
             "smt\\src\\rmts\\rmtb.hpp",
             "smt\\src\\rmts\\rmtc.hpp"
         ],
         "include_dirs": [
             "smt/src/rmts",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-db2w92ph\\lib\\site-packages\\numpy\\core\\include"
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include"
         ],
         "language": "c++",
         "name": "smt.surrogate_models.rmtsclib",
         "sources": [
             "smt/src/rmts/rmtsclib.pyx",
             "smt/src/rmts/utils.cpp",
             "smt/src/rmts/rmts.cpp",
@@ -1075,195 +1075,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":689
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":690
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":691
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":692
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":696
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":697
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":698
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":699
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":703
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":704
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":713
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":714
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":715
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":717
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":718
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":719
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":721
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":722
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":724
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":725
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":726
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1296,42 +1296,42 @@
 #ifndef _ARRAYARRAY_H
 struct arrayobject;
 typedef struct arrayobject arrayobject;
 #endif
 struct __pyx_obj_3smt_16surrogate_models_8rmtsclib_PyRMTB;
 struct __pyx_obj_3smt_16surrogate_models_8rmtsclib_PyRMTC;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":728
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":729
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":730
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":732
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -5650,15 +5650,15 @@
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":734
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5667,29 +5667,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5700,15 +5700,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":737
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5717,29 +5717,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5750,15 +5750,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":740
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5767,29 +5767,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5800,15 +5800,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":743
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5817,29 +5817,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5850,15 +5850,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":746
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5867,29 +5867,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5900,212 +5900,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":749
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":928
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":932
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":934
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":936
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":940
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6121,15 +6121,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6137,53 +6137,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":941
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":943
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":944
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -6191,30 +6191,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":940
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6229,15 +6229,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":946
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6253,15 +6253,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6269,53 +6269,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":947
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":949
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":950
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -6323,30 +6323,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":946
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6361,15 +6361,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":952
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6385,15 +6385,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6401,53 +6401,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":953
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":955
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":956
+      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -6455,30 +6455,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":952
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6493,176 +6493,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":966
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":978
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":966
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":981
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":993
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":981
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":996
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":996
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1006
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1013
+/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -7036,26 +7036,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(3, 950, __pyx_L1_error)
@@ -7468,15 +7468,15 @@
  * import numpy as np
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../AppData/Local/Temp/build-env-db2w92ph/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `smt-2.0b2/smt/src/rmts/rmtsclib.pyx` & `smt-2.0b3/smt/src/rmts/rmtsclib.pyx`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/src/rmts/utils.cpp` & `smt-2.0b3/smt/src/rmts/utils.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/gekpls.py` & `smt-2.0b3/smt/surrogate_models/gekpls.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         if 0 in self.training_points[None]:
             self.coeff_pls, XX, yy = ge_compute_pls(
                 X.copy(),
                 y.copy(),
                 self.options["n_comp"],
                 self.training_points,
                 self.options["delta_x"],
-                self.options["xspecs"].limits,
+                self.design_space.get_num_bounds(),
                 self.options["extra_points"],
             )
             if self.options["extra_points"] != 0:
                 self.nt *= self.options["extra_points"] + 1
                 X = np.vstack((X, XX))
                 y = np.vstack((y, yy))
```

### Comparing `smt-2.0b2/smt/surrogate_models/genn.py` & `smt-2.0b3/smt/surrogate_models/genn.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/idw.py` & `smt-2.0b3/smt/surrogate_models/idw.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/kpls.py` & `smt-2.0b3/smt/surrogate_models/kpls.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/kplsk.py` & `smt-2.0b3/smt/surrogate_models/kplsk.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/krg.py` & `smt-2.0b3/smt/surrogate_models/krg.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/krg_based.py` & `smt-2.0b3/smt/surrogate_models/krg_based.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,27 +25,37 @@
     gower_componentwise_distances,
     componentwise_distance,
     componentwise_distance_PLS,
     compute_X_cont,
     cross_levels,
     compute_X_cross,
     cross_levels_homo_space,
-    XSpecs,
     MixHrcKernelType,
+    matrix_data_corr_levels_cat_matrix,
+    matrix_data_corr_levels_cat_mod,
+    matrix_data_corr_levels_cat_mod_comps,
 )
 from smt.utils.misc import standardization
+from smt.utils.checks import ensure_2d_array, check_support
 from scipy.stats import multivariate_normal as m_norm
 from smt.sampling_methods import LHS
-from smt.utils.mixed_integer import unfold_with_enum_mask
-
-MixIntKernelType = Enum(
-    "MixIntKernelType", ["EXP_HOMO_HSPHERE", "HOMO_HSPHERE", "CONT_RELAX", "GOWER"]
+from smt.utils.design_space import (
+    BaseDesignSpace,
+    ensure_design_space,
+    CategoricalVariable,
 )
 
 
+class MixIntKernelType(Enum):
+    EXP_HOMO_HSPHERE = "EXP_HOMO_HSPHERE"
+    HOMO_HSPHERE = "HOMO_HSPHERE"
+    CONT_RELAX = "CONT_RELAX"
+    GOWER = "GOWER"
+
+
 class KrgBased(SurrogateModel):
     _regression_types = {"constant": constant, "linear": linear, "quadratic": quadratic}
 
     _correlation_types = {
         "pow_exp": pow_exp,
         "abs_exp": abs_exp,
         "squar_exp": squar_exp,
@@ -84,15 +94,15 @@
             "pow_exp_power",
             1.9,
             types=(float),
             desc="Power for the pow_exp kernel function (valid values in (0.0, 2.0]), This option is set automatically when corr option is squar, abs, or matern.",
         )
         declare(
             "categorical_kernel",
-            None,
+            MixIntKernelType.CONT_RELAX,
             values=[
                 MixIntKernelType.CONT_RELAX,
                 MixIntKernelType.GOWER,
                 MixIntKernelType.EXP_HOMO_HSPHERE,
                 MixIntKernelType.HOMO_HSPHERE,
             ],
             desc="The kernel to use for categorical inputs. Only for non continuous Kriging",
@@ -161,28 +171,34 @@
         declare(
             "n_start",
             10,
             types=int,
             desc="number of optimizer runs (multistart method)",
         )
         declare(
-            "xspecs",
+            "xlimits",
             None,
-            types=XSpecs,
-            desc="""xspecs : x specifications including
-                xtypes: x types list
-                    x types specification: list of either FLOAT, ORD or (ENUM, n) spec.
-                xlimits: array-like
-                    bounds of x features""",
+            types=(list, np.ndarray),
+            desc="definition of a design space of float (continuous) variables: "
+            "array-like of size nx x 2 (lower, upper bounds)",
+        )
+        declare(
+            "design_space",
+            None,
+            types=(BaseDesignSpace, list, np.ndarray),
+            desc="definition of the (hierarchical) design space: "
+            "use `smt.utils.design_space.DesignSpace` as the main API. Also accepts list of float variable bounds",
         )
         self.best_iteration_fail = None
         self.nb_ill_matrix = 5
+        self.is_acting_points = {}
         supports["derivatives"] = True
         supports["variances"] = True
         supports["variance_derivatives"] = True
+        supports["x_hierarchy"] = True
 
     def _final_initialize(self):
         # initialize default power values
         if self.options["corr"] == "squar_exp":
             self.options["pow_exp_power"] = 2.0
         elif self.options["corr"] in ["abs_exp", "matern32", "matern52"]:
             self.options["pow_exp_power"] = 1.0
@@ -191,39 +207,88 @@
         assert (
             self.options["pow_exp_power"] > 0 and self.options["pow_exp_power"] <= 2
         ), (
             "The power value for exponential power function can only be >0 and <=2, but %s was given"
             % self.options["pow_exp_power"]
         )
 
+    @property
+    def design_space(self) -> BaseDesignSpace:
+        xt = self.training_points.get(None)
+        if xt is not None:
+            xt = xt[0][0]
+
+        if self.options["design_space"] is None:
+            self.options["design_space"] = ensure_design_space(xt=xt)
+
+        elif not isinstance(self.options["design_space"], BaseDesignSpace):
+            ds_input = self.options["design_space"]
+            self.options["design_space"] = ensure_design_space(
+                xt=xt, xlimits=ds_input, design_space=ds_input
+            )
+        return self.options["design_space"]
+
+    @property
+    def is_continuous(self) -> bool:
+        return self.design_space.is_all_cont
+
+    def set_training_values(
+        self, xt: np.ndarray, yt: np.ndarray, name=None, is_acting=None
+    ) -> None:
+        """
+        Set training data (values).
+
+        Parameters
+        ----------
+        xt : np.ndarray[nt, nx] or np.ndarray[nt]
+            The input values for the nt training points.
+        yt : np.ndarray[nt, ny] or np.ndarray[nt]
+            The output values for the nt training points.
+        name : str or None
+            An optional label for the group of training points being set.
+            This is only used in special situations (e.g., multi-fidelity applications).
+        is_acting : np.ndarray[nt, nx] or np.ndarray[nt]
+            Matrix specifying which of the design variables is acting in a hierarchical design space
+        """
+        super().set_training_values(xt, yt, name=name)
+        if is_acting is not None:
+            self.is_acting_points[name] = is_acting
+
     def _new_train(self):
         # Sampling points X and y
         X = self.training_points[None][0][0]
         y = self.training_points[None][0][1]
+        # Get is_acting status from design space model if needed (might correct training points)
+        is_acting = self.is_acting_points.get(None)
+        if is_acting is None:
+            X, is_acting = self.design_space.correct_get_acting(X)
+            self.training_points[None][0][0] = X
+            self.is_acting_points[None] = is_acting
 
         # Compute PLS-coefficients (attr of self) and modified X and y (if GEKPLS is used)
         if self.name not in ["Kriging", "MGP"]:
-            if self.options["categorical_kernel"] is None:
+            if self.is_continuous:
                 X, y = self._compute_pls(X.copy(), y.copy())
 
         self._check_param()
         self.X_train = X
+        self.is_acting_train = is_acting
+        self._corr_params = None
 
-        if self.options["categorical_kernel"] is not None:
+        if not (self.is_continuous):
             D, self.ij, X = gower_componentwise_distances(
                 X=X,
-                xspecs=self.options["xspecs"],
+                x_is_acting=is_acting,
+                design_space=self.design_space,
                 hierarchical_kernel=self.options["hierarchical_kernel"],
             )
             self.Lij, self.n_levels = cross_levels(
-                X=self.X_train, ij=self.ij, xtypes=self.options["xspecs"].types
-            )
-            _, self.cat_features = compute_X_cont(
-                self.X_train, self.options["xspecs"].types
+                X=self.X_train, ij=self.ij, design_space=self.design_space
             )
+            _, self.cat_features = compute_X_cont(self.X_train, self.design_space)
         # Center and scale X and y
         (
             self.X_norma,
             self.y_norma,
             self.X_offset,
             self.y_mean,
             self.X_scale,
@@ -249,15 +314,15 @@
             self.optimal_noise = self.options["noise0"] * np.ones(self.nt)
             for i in range(self.nt):
                 diff = self.y_norma[index_unique == i] - y_norma_unique[i]
                 if np.sum(diff**2) != 0.0:
                     self.optimal_noise[i] = np.std(diff, ddof=1) ** 2
             self.optimal_noise = self.optimal_noise / nt_reps
             self.y_norma = y_norma_unique
-        if self.options["categorical_kernel"] is None:
+        if self.is_continuous:
             # Calculate matrix of distances D between samples
             D, self.ij = cross_distances(self.X_norma)
 
         if np.min(np.sum(np.abs(D), axis=1)) == 0.0:
             warnings.warn(
                 "Warning: multiple x input features have the same value (at least same row twice)."
             )
@@ -291,18 +356,86 @@
         """
         Train the model
         """
         # outputs['sol'] = self.sol
 
         self._new_train()
 
+    def _initialize_theta(self, theta, n_levels, cat_features, cat_kernel):
+        if self._corr_params is not None:
+            return self._corr_params
+
+        nx = self.nx
+        try:
+            cat_kernel_comps = self.options["cat_kernel_comps"]
+            if cat_kernel_comps is not None:
+                n_levels = np.array(cat_kernel_comps)
+        except KeyError:
+            cat_kernel_comps = None
+        try:
+            ncomp = self.options["n_comp"]
+            try:
+                self.pls_coeff_cont
+            except AttributeError:
+                self.pls_coeff_cont = []
+        except KeyError:
+            cat_kernel_comps = None
+            ncomp = 1e5
+
+        theta_cont_features = np.zeros((len(theta), 1), dtype=bool)
+        theta_cat_features = np.zeros((len(theta), len(n_levels)), dtype=bool)
+        i = 0
+        j = 0
+        n_theta_cont = 0
+        for feat in cat_features:
+            if feat:
+                if cat_kernel in [
+                    MixIntKernelType.EXP_HOMO_HSPHERE,
+                    MixIntKernelType.HOMO_HSPHERE,
+                ]:
+                    # theta_cont_features[
+                    #     j : j + int(nlevels[i] * (nlevels[i] - 1) / 2)
+                    # ] = False  # Matrix is already False
+                    theta_cat_features[
+                        j : j + int(n_levels[i] * (n_levels[i] - 1) / 2), i
+                    ] = [True] * int(n_levels[i] * (n_levels[i] - 1) / 2)
+                    j += int(n_levels[i] * (n_levels[i] - 1) / 2)
+                i += 1
+            else:
+                if cat_kernel in [
+                    MixIntKernelType.EXP_HOMO_HSPHERE,
+                    MixIntKernelType.HOMO_HSPHERE,
+                ]:
+                    if n_theta_cont < ncomp:
+                        theta_cont_features[j] = True
+                        j += 1
+                        n_theta_cont += 1
+
+        theta_cat_features = (
+            [
+                np.where(theta_cat_features[:, i_lvl])[0]
+                for i_lvl in range(len(n_levels))
+            ],
+            np.any(theta_cat_features, axis=1) if len(n_levels) > 0 else None,
+        )
+
+        self._corr_params = params = (
+            cat_kernel_comps,
+            ncomp,
+            theta_cat_features,
+            theta_cont_features,
+            nx,
+            n_levels,
+        )
+        return params
+
     def _matrix_data_corr(
         self,
         corr,
-        xtypes,
+        design_space,
         power,
         theta,
         theta_bounds,
         dx,
         Lij,
         n_levels,
         cat_features,
@@ -312,16 +445,16 @@
         """
         matrix kernel correlation model.
 
         Parameters
         ----------
         corr: correlation_types
             - The autocorrelation model
-        xtypes: np.ndarray [dim]
-                -the types (FLOAT,ORD,ENUM) of the input variables
+        design_space: BaseDesignSpace
+            - The design space definition
         theta : list[small_d * n_comp]
             Hyperparameters of the correlation model
         dx: np.ndarray[n_obs * (n_obs - 1) / 2, n_comp]
             - The gower_componentwise_distances between the samples.
         Lij: np.ndarray [n_obs * (n_obs - 1) / 2, 2]
                 - The levels corresponding to the indices i and j of the vectors in X.
         n_levels: np.ndarray
@@ -333,83 +466,46 @@
         x : np.ndarray[n_obs , n_comp]
             - The input instead of dx for homo_hs prediction
         Returns
         -------
         r: np.ndarray[n_obs * (n_obs - 1) / 2,1]
             An array containing the values of the autocorrelation model.
         """
+
         _correlation_types = {
             "pow_exp": pow_exp,
             "abs_exp": abs_exp,
             "squar_exp": squar_exp,
             "act_exp": act_exp,
             "matern52": matern52,
             "matern32": matern32,
         }
 
-        r = np.zeros((dx.shape[0], 1))
-        nx = self.nx
-        nlevels = n_levels
-        try:
-            cat_kernel_comps = self.options["cat_kernel_comps"]
-            if cat_kernel_comps is not None:
-                nlevels = np.array(cat_kernel_comps)
-        except KeyError:
-            cat_kernel_comps = None
-        try:
-            ncomp = self.options["n_comp"]
-            try:
-                self.pls_coeff_cont
-            except AttributeError:
-                self.pls_coeff_cont = []
-        except KeyError:
-            cat_kernel_comps = None
-            ncomp = 1e5
-        theta_cont_features = np.zeros((len(theta), 1), dtype=bool)
-        theta_cat_features = np.zeros((len(theta), len(nlevels)), dtype=bool)
-        i = 0
-        j = 0
-        n_theta_cont = 0
-        for feat in cat_features:
-            if feat:
-                if cat_kernel in [
-                    MixIntKernelType.EXP_HOMO_HSPHERE,
-                    MixIntKernelType.HOMO_HSPHERE,
-                ]:
-                    theta_cont_features[
-                        j : j + int(nlevels[i] * (nlevels[i] - 1) / 2)
-                    ] = False
-                    theta_cat_features[
-                        j : j + int(nlevels[i] * (nlevels[i] - 1) / 2), i
-                    ] = [True] * int(nlevels[i] * (nlevels[i] - 1) / 2)
-                    j += int(nlevels[i] * (nlevels[i] - 1) / 2)
-                i += 1
-            else:
-                if cat_kernel in [
-                    MixIntKernelType.EXP_HOMO_HSPHERE,
-                    MixIntKernelType.HOMO_HSPHERE,
-                ]:
-                    if n_theta_cont < ncomp:
-                        theta_cont_features[j] = True
-                        j += 1
-                        n_theta_cont += 1
+        # Initialize static parameters
+        (
+            cat_kernel_comps,
+            ncomp,
+            theta_cat_features,
+            theta_cont_features,
+            nx,
+            n_levels,
+        ) = self._initialize_theta(theta, n_levels, cat_features, cat_kernel)
+
         # Sampling points X and y
         X = self.training_points[None][0][0]
         y = self.training_points[None][0][1]
 
         if cat_kernel == MixIntKernelType.CONT_RELAX:
-            from smt.applications.mixed_integer import unfold_with_enum_mask
-
-            X_pls_space = unfold_with_enum_mask(xtypes, X)
+            X_pls_space, _ = design_space.unfold_x(X)
             nx = len(theta)
 
         elif cat_kernel == MixIntKernelType.GOWER:
             X_pls_space = np.copy(X)
         else:
-            X_pls_space, _ = compute_X_cont(X, xtypes)
+            X_pls_space, _ = compute_X_cont(X, design_space)
             d_cont = dx[:, np.logical_not(cat_features)]
         if cat_kernel_comps is not None or ncomp < 1e5:
             ###Modifier la condition : if PLS cont
             if self.pls_coeff_cont == []:
                 X, y = self._compute_pls(X_pls_space.copy(), y.copy())
                 self.pls_coeff_cont = self.coeff_pls
             if (
@@ -461,69 +557,43 @@
         r_cat = np.copy(r_cont) * 0
         r = np.copy(r_cont)
         ##Theta_cat_i loop
         try:
             self.coeff_pls_cat
         except AttributeError:
             self.coeff_pls_cat = []
-        for i in range(len(nlevels)):
-            theta_cat = theta[theta_cat_features[:, i]]
+
+        theta_cat_kernel = theta
+        if len(n_levels) > 0:
+            theta_cat_kernel = theta.copy()
             if cat_kernel == MixIntKernelType.EXP_HOMO_HSPHERE:
-                theta_cat = theta_cat * (0.5 * np.pi / theta_bounds[1])
+                theta_cat_kernel[theta_cat_features[1]] *= 0.5 * np.pi / theta_bounds[1]
             elif cat_kernel == MixIntKernelType.HOMO_HSPHERE:
-                theta_cat = theta_cat * (2.0 * np.pi / theta_bounds[1])
-            Theta_mat = np.zeros((nlevels[i], nlevels[i]))
-            L = np.zeros((nlevels[i], nlevels[i]))
-            v = 0
-            for j in range(nlevels[i]):
-                for k in range(nlevels[i] - j):
-                    if j == k + j:
-                        Theta_mat[j, k + j] = 1
-                    else:
-                        Theta_mat[j, k + j] = theta_cat[v]
-                        Theta_mat[k + j, j] = theta_cat[v]
-                        v = v + 1
-
-            for j in range(nlevels[i]):
-                for k in range(nlevels[i] - j):
-                    if j == k + j:
-                        if j == 0:
-                            L[j, k + j] = 1
-
-                        else:
-                            L[j, k + j] = 1
-                            for l in range(j):
-                                L[j, k + j] = L[j, k + j] * np.sin(Theta_mat[j, l])
+                theta_cat_kernel[theta_cat_features[1]] *= 2.0 * np.pi / theta_bounds[1]
 
-                    else:
-                        if j == 0:
-                            L[k + j, j] = np.cos(Theta_mat[k, 0])
-                        else:
-                            L[k + j, j] = np.cos(Theta_mat[k + j, j])
-                            for l in range(j):
-                                L[k + j, j] = L[k + j, j] * np.sin(Theta_mat[k + j, l])
-
-            T = np.dot(L, L.T)
-
-            if cat_kernel == MixIntKernelType.EXP_HOMO_HSPHERE:
-                T = (T - 1) * theta_bounds[1] / 2
-                T = np.exp(2 * T)
-            k = (1 + np.exp(-theta_bounds[1])) / np.exp(-theta_bounds[0])
-            T = (T + np.exp(-theta_bounds[1])) / (k)
+        for i in range(len(n_levels)):
+            theta_cat = theta_cat_kernel[theta_cat_features[0][i]]
+            T = matrix_data_corr_levels_cat_matrix(
+                i,
+                n_levels,
+                theta_cat,
+                theta_bounds,
+                is_ehh=cat_kernel == MixIntKernelType.EXP_HOMO_HSPHERE,
+            )
 
             if cat_kernel_comps is not None:
                 # Sampling points X and y
                 X = self.training_points[None][0][0]
                 y = self.training_points[None][0][1]
                 X_icat = X[:, cat_features]
                 X_icat = X_icat[:, i]
                 old_n_comp = (
                     self.options["n_comp"] if "n_comp" in self.options else None
                 )
-                self.options["n_comp"] = int(nlevels[i] / 2 * (nlevels[i] - 1))
+                self.options["n_comp"] = int(n_levels[i] / 2 * (n_levels[i] - 1))
                 X_full_space = compute_X_cross(X_icat, n_levels[i])
                 try:
                     self.coeff_pls = self.coeff_pls_cat[i]
                 except IndexError:
                     _, _ = self._compute_pls(X_full_space.copy(), y.copy())
                     self.coeff_pls_cat.append(self.coeff_pls)
 
@@ -543,43 +613,39 @@
                     self.options["n_comp"],
                     self.coeff_pls,
                     power=self.options["pow_exp_power"],
                     theta=None,
                     return_derivative=False,
                 )
 
-            for k in range(np.shape(Lij[i])[0]):
-                indi = int(Lij[i][k][0])
-                indj = int(Lij[i][k][1])
-
-                if indi == indj:
-                    r_cat[k] = 1.0
-                else:
-                    if cat_kernel in [
+                matrix_data_corr_levels_cat_mod_comps(
+                    i,
+                    Lij,
+                    r_cat,
+                    n_levels,
+                    T,
+                    d_cat_i,
+                    has_cat_kernel=cat_kernel
+                    in [
                         MixIntKernelType.EXP_HOMO_HSPHERE,
                         MixIntKernelType.HOMO_HSPHERE,
-                    ]:
-                        if cat_kernel_comps is not None:
-                            Theta_i_red = np.zeros(
-                                int((nlevels[i] - 1) * nlevels[i] / 2)
-                            )
-                            indmatvec = 0
-                            for j in range(nlevels[i]):
-                                for l in range(nlevels[i]):
-                                    if l > j:
-                                        Theta_i_red[indmatvec] = T[j, l]
-                                        indmatvec += 1
-                            kval_cat = 0
-                            for indijk in range(len(Theta_i_red)):
-                                kval_cat += np.multiply(
-                                    Theta_i_red[indijk], d_cat_i[k : k + 1][0][indijk]
-                                )
-                            r_cat[k] = kval_cat
-                        else:
-                            r_cat[k] = T[indi, indj]
+                    ],
+                )
+            else:
+                matrix_data_corr_levels_cat_mod(
+                    i,
+                    Lij,
+                    r_cat,
+                    T,
+                    has_cat_kernel=cat_kernel
+                    in [
+                        MixIntKernelType.EXP_HOMO_HSPHERE,
+                        MixIntKernelType.HOMO_HSPHERE,
+                    ],
+                )
 
             r = np.multiply(r, r_cat)
             if cat_kernel_comps is not None:
                 if old_n_comp == None:
                     self.options._dict.pop("n_comp", None)
                 else:
                     self.options["n_comp"] = old_n_comp
@@ -634,35 +700,31 @@
         noise = self.noise0
         tmp_var = theta
         if self.options["use_het_noise"]:
             noise = self.optimal_noise
         if self.options["eval_noise"] and not self.options["use_het_noise"]:
             theta = tmp_var[0 : self.D.shape[1]]
             noise = tmp_var[self.D.shape[1] :]
-        if self.options["categorical_kernel"] is not None:
+        if not (self.is_continuous):
             dx = self.D
             if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
-                from smt.applications.mixed_integer import unfold_with_enum_mask
-
-                X2 = unfold_with_enum_mask(
-                    self.options["xspecs"].types, self.training_points[None][0][0]
-                )
+                X2, _ = self.design_space.unfold_x(self.training_points[None][0][0])
                 (
                     self.X2_norma,
                     _,
                     self.X2_offset,
                     _,
                     self.X2_scale,
                     _,
                 ) = standardization(X2, self.training_points[None][0][1])
                 dx, _ = cross_distances(self.X2_norma)
 
             r = self._matrix_data_corr(
                 corr=self.options["corr"],
-                xtypes=self.options["xspecs"].types,
+                design_space=self.design_space,
                 power=self.options["pow_exp_power"],
                 theta=theta,
                 theta_bounds=self.options["theta_bounds"],
                 dx=dx,
                 Lij=self.Lij,
                 n_levels=self.n_levels,
                 cat_features=self.cat_features,
@@ -1044,73 +1106,119 @@
 
                 if self.name in ["MGP"] and eta == omega:
                     hess[ind_0 + i, 0] += log_prior[eta]
             par["Rinv_dR_gamma"] = Rinv_dRdomega_gamma_all
             par["Rinv_dmu"] = Rinv_dmudomega_all
         return hess, hess_ij, par
 
-    def _predict_values(self, x):
+    def predict_values(self, x: np.ndarray, is_acting=None) -> np.ndarray:
+        """
+        Predict the output values at a set of points.
+
+        Parameters
+        ----------
+        x : np.ndarray[nt, nx] or np.ndarray[nt]
+            Input values for the prediction points.
+        is_acting : np.ndarray[nt, nx] or np.ndarray[nt]
+            Matrix specifying for each design variable whether it is acting or not (for hierarchical design spaces)
+
+        Returns
+        -------
+        y : np.ndarray[nt, ny]
+            Output values at the prediction points.
+        """
+        x = ensure_2d_array(x, "x")
+        self._check_xdim(x)
+
+        if is_acting is not None:
+            is_acting = ensure_2d_array(is_acting, "is_acting")
+            if is_acting.shape != x.shape:
+                raise ValueError(
+                    f"is_acting should have the same dimensions as x: {is_acting.shape} != {x.shape}"
+                )
+
+        n = x.shape[0]
+        x2 = np.copy(x)
+        self.printer.active = (
+            self.options["print_global"] and self.options["print_prediction"]
+        )
+
+        if self.name == "MixExp":
+            # Mixture of experts model
+            self.printer._title("Evaluation of the Mixture of experts")
+        else:
+            self.printer._title("Evaluation")
+        self.printer("   %-12s : %i" % ("# eval points.", n))
+        self.printer()
+
+        # Evaluate the unknown points using the specified model-method
+        with self.printer._timed_context("Predicting", key="prediction"):
+            y = self._predict_values(x2, is_acting=is_acting)
+        time_pt = self.printer._time("prediction")[-1] / n
+        self.printer()
+        self.printer("Prediction time/pt. (sec) : %10.7f" % time_pt)
+        self.printer()
+        return y.reshape((n, self.ny))
+
+    def _predict_values(self, x: np.ndarray, is_acting=None) -> np.ndarray:
         """
         Evaluates the model at a set of points.
 
         Parameters
         ----------
         x : np.ndarray [n_evals, dim]
             Evaluation point input variable values
+        is_acting : np.ndarray[nt, nx] or np.ndarray[nt]
+            Matrix specifying for each design variable whether it is acting or not (for hierarchical design spaces)
 
         Returns
         -------
         y : np.ndarray
             Evaluation point output variable values
         """
         # Initialization
+        if is_acting is None:
+            x, is_acting = self.design_space.correct_get_acting(x)
         n_eval, n_features_x = x.shape
 
-        if self.options["categorical_kernel"] is not None:
+        if not (self.is_continuous):
             dx = gower_componentwise_distances(
                 x,
-                xspecs=self.options["xspecs"],
+                x_is_acting=is_acting,
+                design_space=self.design_space,
                 hierarchical_kernel=self.options["hierarchical_kernel"],
                 y=np.copy(self.X_train),
+                y_is_acting=self.is_acting_train,
+            )
+            _, ij = cross_distances(x, self.X_train)
+            Lij, _ = cross_levels(
+                X=x, ij=ij, design_space=self.design_space, y=self.X_train
             )
+            self.ij = ij
+            if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
+                Xpred, _ = self.design_space.unfold_x(x)
+                Xpred_norma = (Xpred - self.X2_offset) / self.X2_scale
+                # Get pairwise componentwise L1-distances to the input training set
+                dx = differences(Xpred_norma, Y=self.X2_norma.copy())
 
-            d = componentwise_distance(
-                dx,
-                self.options["corr"],
-                self.nx,
+            r = self._matrix_data_corr(
+                corr=self.options["corr"],
+                design_space=self.design_space,
                 power=self.options["pow_exp_power"],
-                theta=None,
-                return_derivative=False,
-            )
-            if self.options["categorical_kernel"] is not None:
-                _, ij = cross_distances(x, self.X_train)
-                Lij, _ = cross_levels(
-                    X=x, ij=ij, xtypes=self.options["xspecs"].types, y=self.X_train
-                )
-                self.ij = ij
-                if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
-                    Xpred = unfold_with_enum_mask(self.options["xspecs"].types, x)
-                    Xpred_norma = (Xpred - self.X2_offset) / self.X2_scale
-                    # Get pairwise componentwise L1-distances to the input training set
-                    dx = differences(Xpred_norma, Y=self.X2_norma.copy())
-                r = self._matrix_data_corr(
-                    corr=self.options["corr"],
-                    xtypes=self.options["xspecs"].types,
-                    power=self.options["pow_exp_power"],
-                    theta=self.optimal_theta,
-                    theta_bounds=self.options["theta_bounds"],
-                    dx=dx,
-                    Lij=Lij,
-                    n_levels=self.n_levels,
-                    cat_features=self.cat_features,
-                    cat_kernel=self.options["categorical_kernel"],
-                    x=x,
-                ).reshape(n_eval, self.nt)
+                theta=self.optimal_theta,
+                theta_bounds=self.options["theta_bounds"],
+                dx=dx,
+                Lij=Lij,
+                n_levels=self.n_levels,
+                cat_features=self.cat_features,
+                cat_kernel=self.options["categorical_kernel"],
+                x=x,
+            ).reshape(n_eval, self.nt)
 
-            X_cont, _ = compute_X_cont(x, self.options["xspecs"].types)
+            X_cont, _ = compute_X_cont(x, self.design_space)
             X_cont = (X_cont - self.X_offset) / self.X_scale
 
         else:
             X_cont = (x - self.X_offset) / self.X_scale
             # Get pairwise componentwise L1-distances to the input training set
             dx = differences(X_cont, Y=self.X_norma.copy())
             d = self._componentwise_distance(dx)
@@ -1179,73 +1287,102 @@
         beta = self.optimal_par["beta"]
         gamma = self.optimal_par["gamma"]
         df_dx = np.dot(df.T, beta)
 
         y = (df_dx[kx] + np.dot(drx, gamma)) * self.y_std / self.X_scale[kx]
         return y
 
-    def _predict_variances(self, x):
+    def predict_variances(self, x: np.ndarray, is_acting=None) -> np.ndarray:
+        """
+        Predict the variances at a set of points.
+
+        Parameters
+        ----------
+        x : np.ndarray[nt, nx] or np.ndarray[nt]
+            Input values for the prediction points.
+        is_acting : np.ndarray[nt, nx] or np.ndarray[nt]
+            Matrix specifying for each design variable whether it is acting or not (for hierarchical design spaces)
+
+        Returns
+        -------
+        s2 : np.ndarray[nt, ny]
+            Variances.
+        """
+        check_support(self, "variances")
+        x = ensure_2d_array(x, "x")
+        self._check_xdim(x)
+
+        if is_acting is not None:
+            is_acting = ensure_2d_array(is_acting, "is_acting")
+            if is_acting.shape != x.shape:
+                raise ValueError(
+                    f"is_acting should have the same dimensions as x: {is_acting.shape} != {x.shape}"
+                )
+
+        n = x.shape[0]
+        x2 = np.copy(x)
+        s2 = self._predict_variances(x2, is_acting=is_acting)
+        return s2.reshape((n, self.ny))
+
+    def _predict_variances(self, x: np.ndarray, is_acting=None) -> np.ndarray:
         """
         Provide uncertainty of the model at a set of points
         Parameters
         ----------
         x : np.ndarray [n_evals, dim]
             Evaluation point input variable values
+        is_acting : np.ndarray[nt, nx] or np.ndarray[nt]
+            Matrix specifying for each design variable whether it is acting or not (for hierarchical design spaces)
         Returns
         -------
         MSE : np.ndarray
             Evaluation point output variable MSE
         """
         # Initialization
+        if is_acting is None:
+            x, is_acting = self.design_space.correct_get_acting(x)
         n_eval, n_features_x = x.shape
         X_cont = x
 
-        if self.options["categorical_kernel"] is not None:
+        if not (self.is_continuous):
             dx = gower_componentwise_distances(
                 x,
-                xspecs=self.options["xspecs"],
+                x_is_acting=is_acting,
+                design_space=self.design_space,
                 hierarchical_kernel=self.options["hierarchical_kernel"],
                 y=np.copy(self.X_train),
+                y_is_acting=self.is_acting_train,
             )
-            d = componentwise_distance(
-                dx,
-                self.options["corr"],
-                self.nx,
-                self.options["pow_exp_power"],
-                theta=None,
-                return_derivative=False,
+            _, ij = cross_distances(x, self.X_train)
+            Lij, _ = cross_levels(
+                X=x, ij=ij, design_space=self.design_space, y=self.X_train
             )
-            if self.options["categorical_kernel"] is not None:
-                _, ij = cross_distances(x, self.X_train)
-                Lij, _ = cross_levels(
-                    X=x, ij=ij, xtypes=self.options["xspecs"].types, y=self.X_train
-                )
-                self.ij = ij
-                if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
-                    from smt.applications.mixed_integer import unfold_with_enum_mask
-
-                    Xpred = unfold_with_enum_mask(self.options["xspecs"].types, x)
-                    Xpred_norma = (Xpred - self.X2_offset) / self.X2_scale
-
-                    # Get pairwise componentwise L1-distances to the input training set
-                    dx = differences(Xpred_norma, Y=self.X2_norma.copy())
-                r = self._matrix_data_corr(
-                    corr=self.options["corr"],
-                    xtypes=self.options["xspecs"].types,
-                    power=self.options["pow_exp_power"],
-                    theta=self.optimal_theta,
-                    theta_bounds=self.options["theta_bounds"],
-                    dx=dx,
-                    Lij=Lij,
-                    n_levels=self.n_levels,
-                    cat_features=self.cat_features,
-                    cat_kernel=self.options["categorical_kernel"],
-                    x=x,
-                ).reshape(n_eval, self.nt)
-            X_cont, _ = compute_X_cont(x, self.options["xspecs"].types)
+            self.ij = ij
+            if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
+                Xpred, _ = self.design_space.unfold_x(x)
+                Xpred_norma = (Xpred - self.X2_offset) / self.X2_scale
+
+                # Get pairwise componentwise L1-distances to the input training set
+                dx = differences(Xpred_norma, Y=self.X2_norma.copy())
+
+            r = self._matrix_data_corr(
+                corr=self.options["corr"],
+                design_space=self.design_space,
+                power=self.options["pow_exp_power"],
+                theta=self.optimal_theta,
+                theta_bounds=self.options["theta_bounds"],
+                dx=dx,
+                Lij=Lij,
+                n_levels=self.n_levels,
+                cat_features=self.cat_features,
+                cat_kernel=self.options["categorical_kernel"],
+                x=x,
+            ).reshape(n_eval, self.nt)
+
+            X_cont, _ = compute_X_cont(x, self.design_space)
             X_cont = (X_cont - self.X_offset) / self.X_scale
         else:
             x = (x - self.X_offset) / self.X_scale
             X_cont = np.copy(x)
             # Get pairwise componentwise L1-distances to the input training set
             dx = differences(x, Y=self.X_norma.copy())
             d = self._componentwise_distance(dx)
@@ -1452,22 +1589,24 @@
                 theta0_rand = m_norm.rvs(
                     self.options["prior"]["mean"] * len(self.theta0),
                     self.options["prior"]["var"],
                     1,
                 )
                 theta0 = self.theta0
             else:
+                theta_bounds = self.options["theta_bounds"]
+                log10t_bounds = np.log10(theta_bounds)
                 theta0_rand = np.random.rand(len(self.theta0))
                 theta0_rand = (
                     theta0_rand * (log10t_bounds[1] - log10t_bounds[0])
                     + log10t_bounds[0]
                 )
                 theta0 = np.log10(self.theta0)
 
-            if self.options["categorical_kernel"]:
+            if not (self.is_continuous):
                 self.D = D
             else:
                 ##from abs distance to kernel distance
                 self.D = self._componentwise_distance(D, opt=ii)
 
             # Initialization
             k, incr, stop, best_optimal_rlf_value, max_retry = 0, 0, 1, -1e20, 10
@@ -1517,14 +1656,15 @@
                     sampling = LHS(
                         xlimits=theta_limits, criterion="maximin", random_state=41
                     )
                     theta_lhs_loops = sampling(self.options["n_start"])
                     theta_all_loops = np.vstack((theta_all_loops, theta_lhs_loops))
 
                 optimal_theta_res = {"fun": float("inf")}
+                optimal_theta_res_loop = None
                 try:
                     if self.options["hyper_opt"] == "Cobyla":
                         for theta0_loop in theta_all_loops:
                             optimal_theta_res_loop = optimize.minimize(
                                 minus_reduced_likelihood_function,
                                 theta0_loop,
                                 constraints=[
@@ -1550,14 +1690,18 @@
                                 jac=grad_minus_reduced_likelihood_function,
                                 bounds=bounds_hyp,
                                 options={"maxiter": 100},
                             )
                             if optimal_theta_res_loop["fun"] < optimal_theta_res["fun"]:
                                 optimal_theta_res = optimal_theta_res_loop
 
+                    if "x" not in optimal_theta_res:
+                        raise ValueError(
+                            f"Optimizer encountered a problem: {optimal_theta_res_loop!s}"
+                        )
                     optimal_theta = optimal_theta_res["x"]
 
                     if self.name not in ["MGP"]:
                         optimal_theta = 10**optimal_theta
 
                     optimal_rlf_value, optimal_par = self._reduced_likelihood_function(
                         theta=optimal_theta
@@ -1648,20 +1792,14 @@
 
     def _check_param(self):
         """
         This function checks some parameters of the model
         and amend theta0 if possible (see _amend_theta0_option).
         """
         d = self.options["n_comp"] if "n_comp" in self.options else self.nx
-
-        if (self.options["xspecs"] is None) and (
-            self.options["categorical_kernel"] is not None
-        ):
-            raise ValueError("xspecs required for mixed integer Kriging")
-
         if self.name in ["KPLS"]:
             if self.options["corr"] not in ["pow_exp", "squar_exp", "abs_exp"]:
                 raise ValueError(
                     "KPLS only works with a squared exponential, or an absolute exponential kernel with variable power"
                 )
             if (
                 self.options["categorical_kernel"]
@@ -1677,38 +1815,30 @@
                     )
 
         mat_dim = (
             self.options["cat_kernel_comps"]
             if "cat_kernel_comps" in self.options
             else None
         )
-        if self.options["categorical_kernel"] in [
-            MixIntKernelType.EXP_HOMO_HSPHERE,
-            MixIntKernelType.HOMO_HSPHERE,
-            MixIntKernelType.CONT_RELAX,
-        ]:
-            n_comp = self.options["n_comp"] if "n_comp" in self.options else None
-            n_param = compute_n_param(
-                self.options["xspecs"].types,
-                self.options["categorical_kernel"],
-                self.nx,
-                d,
-                n_comp,
-                mat_dim,
-            )
 
-            self.options["theta0"] *= np.ones(n_param)
+        n_comp = self.options["n_comp"] if "n_comp" in self.options else None
+        n_param = compute_n_param(
+            self.design_space,
+            self.options["categorical_kernel"],
+            d,
+            n_comp,
+            mat_dim,
+        )
 
-        if len(self.options["theta0"]) != d and self.options[
-            "categorical_kernel"
-        ] not in [
-            MixIntKernelType.EXP_HOMO_HSPHERE,
-            MixIntKernelType.CONT_RELAX,
-            MixIntKernelType.HOMO_HSPHERE,
-        ]:
+        self.options["theta0"] *= np.ones(n_param)
+
+        if len(self.options["theta0"]) != d and (
+            self.options["categorical_kernel"] == MixIntKernelType.GOWER
+            or self.is_continuous
+        ):
             if len(self.options["theta0"]) == 1:
                 self.options["theta0"] *= np.ones(d)
             else:
                 raise ValueError(
                     "the length of theta0 (%s) should be equal to the number of dim (%s)."
                     % (len(self.options["theta0"]), d)
                 )
@@ -1751,49 +1881,49 @@
                     "n_samples=%d must be greater than the "
                     "regression model size p=%d."
                 )
                 % (self.nt, p)
             )
 
 
-def compute_n_param(xtypes, cat_kernel, nx, d, n_comp, mat_dim):
+def compute_n_param(design_space, cat_kernel, d, n_comp, mat_dim):
     """
     Returns the he number of parameters needed for an homoscedastic or full group kernel.
     Parameters
      ----------
-    xtypes: np.ndarray [dim]
-            -the types (FLOAT,ORD,ENUM) of the input variables,
+    design_space: BaseDesignSpace
+            - design space definition
     cat_kernel : string
             -The kernel to use for categorical inputs. Only for non continuous Kriging,
-    nx: int
-            -The number of variables,
     d: int
             - n_comp or nx
     n_comp : int
             - if PLS, then it is the number of components else None,
     mat_dim : int
             - if PLS, then it is the number of components for matrix kernel (mixed integer) else None,
     Returns
     -------
      n_param: int
             - The number of parameters.
     """
-    n_param = nx
+    n_param = design_space.n_dv
     if n_comp is not None:
         n_param = d
         if cat_kernel == MixIntKernelType.CONT_RELAX:
             return n_param
         if mat_dim is not None:
             return int(np.sum([l * (l - 1) / 2 for l in mat_dim]) + n_param)
-
-    for i, xtyp in enumerate(xtypes):
-        if isinstance(xtyp, tuple):
-            if nx == d:
+    if cat_kernel == MixIntKernelType.GOWER:
+        return n_param
+    for i, dv in enumerate(design_space.design_variables):
+        if isinstance(dv, CategoricalVariable):
+            n_values = dv.n_values
+            if design_space.n_dv == d:
                 n_param -= 1
             if cat_kernel in [
                 MixIntKernelType.EXP_HOMO_HSPHERE,
                 MixIntKernelType.HOMO_HSPHERE,
             ]:
-                n_param += int(xtyp[1] * (xtyp[1] - 1) / 2)
+                n_param += int(n_values * (n_values - 1) / 2)
             if cat_kernel == MixIntKernelType.CONT_RELAX:
-                n_param += int(xtyp[1])
+                n_param += int(n_values)
     return n_param
```

### Comparing `smt-2.0b2/smt/surrogate_models/ls.py` & `smt-2.0b3/smt/surrogate_models/ls.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/mgp.py` & `smt-2.0b3/smt/surrogate_models/rmts.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,530 +1,580 @@
 """
-Author: Remy Priem (remy.priem@onera.fr)
+Author: Dr. John T. Hwang <hwangjt@umich.edu>
 
 This package is distributed under New BSD license.
 """
-
-from __future__ import division
 import numpy as np
-from scipy import linalg
+import scipy.sparse
+from numbers import Integral
 
-from smt.utils.kriging import differences, componentwise_distance
-from smt.surrogate_models.krg_based import KrgBased
-from smt.utils.checks import check_support, check_nx, ensure_2d_array
+from smt.utils.linear_solvers import get_solver, LinearSolver, VALID_SOLVERS
+from smt.utils.line_search import get_line_search_class, LineSearch, VALID_LINE_SEARCHES
+from smt.utils.caching import cached_operation
+from smt.surrogate_models.surrogate_model import SurrogateModel
 
-"""
-The Active kriging class.
-"""
 
+class RMTS(SurrogateModel):
+    """
+    Regularized Minimal-energy Tensor-product Spline interpolant base class for RMTC and RMTB.
+    """
 
-class MGP(KrgBased):
-    name = "MGP"
+    name = "RMTS"
 
     def _initialize(self):
-        """
-        Initialized MGP
-
-        """
-        super(MGP, self)._initialize()
+        super(RMTS, self)._initialize()
         declare = self.options.declare
-        declare("n_comp", 1, types=int, desc="Number of active dimensions")
+        supports = self.supports
+
         declare(
-            "prior",
-            {"mean": [0.0], "var": 5.0 / 4.0},
-            types=dict,
-            desc="Parameters for Gaussian prior of the Hyperparameters",
+            "xlimits",
+            types=np.ndarray,
+            desc="Lower/upper bounds in each dimension - ndarray [nx, 2]",
+        )
+        declare(
+            "smoothness",
+            1.0,
+            types=(Integral, float, tuple, list, np.ndarray),
+            desc="Smoothness parameter in each dimension - length nx. None implies uniform",
+        )
+        declare(
+            "regularization_weight",
+            1e-14,
+            types=(Integral, float),
+            desc="Weight of the term penalizing the norm of the spline coefficients."
+            + " This is useful as an alternative to energy minimization "
+            + " when energy minimization makes the training time too long.",
+        )
+        declare(
+            "energy_weight",
+            1e-4,
+            types=(Integral, float),
+            desc="The weight of the energy minimization terms",
+        )
+        declare(
+            "extrapolate",
+            False,
+            types=bool,
+            desc="Whether to perform linear extrapolation for external evaluation points",
+        )
+        declare(
+            "min_energy",
+            True,
+            types=bool,
+            desc="Whether to perform energy minimization",
+        )
+        declare(
+            "approx_order", 4, types=Integral, desc="Exponent in the approximation term"
+        )
+        declare(
+            "solver",
+            "krylov",
+            values=VALID_SOLVERS,
+            types=LinearSolver,
+            desc="Linear solver",
+        )
+        declare(
+            "derivative_solver",
+            "krylov",
+            values=VALID_SOLVERS,
+            types=LinearSolver,
+            desc="Linear solver used for computing output derivatives (dy_dyt)",
+        )
+        declare(
+            "grad_weight",
+            0.5,
+            types=(Integral, float),
+            desc="Weight on gradient training data",
+        )
+        declare(
+            "solver_tolerance",
+            1e-12,
+            types=(Integral, float),
+            desc="Convergence tolerance for the nonlinear solver",
+        )
+        declare(
+            "nonlinear_maxiter",
+            10,
+            types=Integral,
+            desc="Maximum number of nonlinear solver iterations",
+        )
+        declare(
+            "line_search",
+            "backtracking",
+            values=VALID_LINE_SEARCHES,
+            types=LineSearch,
+            desc="Line search algorithm",
+        )
+        declare(
+            "save_energy_terms",
+            False,
+            types=bool,
+            desc="Whether to cache energy terms in the data_dir directory",
+        )
+        declare(
+            "data_dir",
+            None,
+            values=(None,),
+            types=str,
+            desc="Directory for loading / saving cached data; None means do not save or load",
+        )
+        declare(
+            "max_print_depth",
+            5,
+            types=Integral,
+            desc="Maximum depth (level of nesting) to print operation descriptions and times",
         )
-        self.options["hyper_opt"] = "TNC"
-        self.options["corr"] = "act_exp"
-
-    def _componentwise_distance(self, dx, small=False, opt=0):
-        """
-        Compute the componentwise distance with respect to the correlation kernel
 
+        supports["training_derivatives"] = True
+        supports["derivatives"] = True
+        supports["output_derivatives"] = True
+
+    def _setup_hessian(self):
+        diag = np.ones(self.num["dof"])
+        arange = np.arange(self.num["dof"])
+        full_hess = scipy.sparse.csc_matrix((diag, (arange, arange)))
+        return full_hess
 
-        Parameters
-        ----------
-        dx : numpy.ndarray
-            Distance matrix.
-        small : bool, optional
-            Compute the componentwise distance in small (n_components) dimension
-            or in initial dimension. The default is False.
-        opt : int, optional
-            useless for MGP
+    def _compute_jac(self, ix1, ix2, x):
+        data, rows, cols = self._compute_jac_raw(ix1, ix2, x)
+        n = x.shape[0]
+        full_jac = scipy.sparse.csc_matrix(
+            (data, (rows, cols)), shape=(n, self.num["coeff"])
+        )
+        if self.full_dof2coeff is not None:
+            full_jac = full_jac * self.full_dof2coeff
+        return full_jac
+
+    def _compute_approx_terms(self):
+        # This computes the approximation terms for the training points.
+        # We loop over kx: 0 is for values and kx>0 represents.
+        # the 1-based index of the derivative given by the training point data.
+        num = self.num
+        xlimits = self.options["xlimits"]
+
+        full_jac_dict = {}
+        for kx in self.training_points[None]:
+            xt, yt = self.training_points[None][kx]
+
+            xmin = np.min(xt, axis=0)
+            xmax = np.max(xt, axis=0)
+            assert np.all(xlimits[:, 0] <= xmin), (
+                "Training points below min for %s" % kx
+            )
+            assert np.all(xlimits[:, 1] >= xmax), (
+                "Training points above max for %s" % kx
+            )
 
-        Returns
-        -------
-        d : numpy.ndarray
-            Component wise distance.
+            if kx == 0:
+                c = 1.0
+            else:
+                self.options["grad_weight"] / xlimits.shape[0]
 
-        """
-        if small:
-            d = componentwise_distance(dx, self.options["corr"], self.options["n_comp"])
-        else:
-            d = componentwise_distance(dx, self.options["corr"], self.nx)
-        return d
+            full_jac = self._compute_jac(kx, 0, xt)
+            full_jac_dict[kx] = (full_jac, full_jac.T.tocsc(), c)
 
-    def _predict_values(self, x):
-        """
-        Predict the value of the MGP for a given point
+        return full_jac_dict
 
-        Parameters
-        ----------
-        x : numpy.ndarray
-            Point to compute.
-
-        Raises
-        ------
-        ValueError
-            The number fo dimension is not good.
+    def _compute_energy_terms(self):
+        # This computes the energy terms that are to be minimized.
+        # The quadrature points are the centroids of the multi-dimensional elements.
+        num = self.num
+        xlimits = self.options["xlimits"]
+
+        inputs = {}
+        inputs["nx"] = xlimits.shape[0]
+        inputs["elem_list"] = num["elem_list"]
+        if self.__class__.__name__ == "RMTB":
+            inputs["num_ctrl_list"] = num["ctrl_list"]
+            inputs["order_list"] = num["order_list"]
 
-        Returns
-        -------
-        y : numpy.ndarray
-            Value of the MGP at the given point x.
-        """
-        n_eval, n_features = x.shape
-        if n_features < self.nx:
-            if n_features != self.options["n_comp"]:
-                raise ValueError(
-                    "dim(u) should be equal to %i" % self.options["n_comp"]
-                )
-            theta = np.eye(self.options["n_comp"]).reshape(
-                (self.options["n_comp"] ** 2,)
-            )
-            # Get pairwise componentwise L1-distances to the input training set
-            u = x
-            x = self.get_x_from_u(u)
-
-            u = u * self.embedding["norm"] - self.U_mean
-            du = differences(u, Y=self.U_norma.copy())
-            d = self._componentwise_distance(du, small=True)
-
-            # Get an approximation of x
-            x = (x - self.X_offset) / self.X_scale
-            dx = differences(x, Y=self.X_norma.copy())
-            d_x = self._componentwise_distance(dx)
+        if self.options["save_energy_terms"]:
+            cache_dir = self.options["data_dir"]
         else:
-            if n_features != self.nx:
-                raise ValueError("dim(x) should be equal to %i" % self.X_scale.shape[0])
-            theta = self.optimal_theta
-
-            # Get pairwise componentwise L1-distances to the input training set
-            x = (x - self.X_offset) / self.X_scale
-            dx = differences(x, Y=self.X_norma.copy())
-            d = self._componentwise_distance(dx)
-            d_x = None
-
-        # Compute the correlation function
-        r = self._correlation_types[self.options["corr"]](theta, d, d_x=d_x).reshape(
-            n_eval, self.nt
-        )
-
-        f = self._regression_types[self.options["poly"]](x)
-        # Scaled predictor
-        y_ = np.dot(f, self.optimal_par["beta"]) + np.dot(r, self.optimal_par["gamma"])
-        # Predictor
-        y = (self.y_mean + self.y_std * y_).ravel()
-        return y
-
-    def _predict_mgp_variances_base(self, x):
-        """Base computation of MGP MSE used by predict_variances and predict_variances_no_uq"""
-        _, n_features = x.shape
-
-        if n_features < self.nx:
-            if n_features != self.options["n_comp"]:
-                raise ValueError(
-                    "dim(u) should be equal to %i" % self.options["n_comp"]
+            cache_dir = None
+        with cached_operation(inputs, cache_dir) as outputs:
+            if outputs:
+                sq_mtx = outputs["sq_mtx"]
+            else:
+                n = np.prod(2 * num["elem_list"])
+                x = np.empty(n * num["x"])
+                self.rmtsc.compute_quadrature_points(
+                    n, np.array(2 * num["elem_list"], dtype=np.int32), x
                 )
-            u = x
-            x = self.get_x_from_u(u)
+                x = x.reshape((n, num["x"]))
 
-            u = u * self.embedding["norm"] - self.U_mean
-            x = (x - self.X_offset) / self.X_scale
-        else:
-            if n_features != self.nx:
-                raise ValueError("dim(x) should be equal to %i" % self.X_scale.shape[0])
-            u = None
-            x = (x - self.X_offset) / self.X_scale
+                sq_mtx = [None] * num["x"]
+                for kx in range(num["x"]):
+                    mtx = self._compute_jac(kx + 1, kx + 1, x)
+                    sq_mtx[kx] = (
+                        mtx.T.tocsc() * mtx * (xlimits[kx, 1] - xlimits[kx, 0]) ** 4
+                    )
+
+                outputs["sq_mtx"] = sq_mtx
+
+        elem_vol = np.prod((xlimits[:, 1] - xlimits[:, 0]) / (2 * num["elem_list"]))
+        total_vol = np.prod(xlimits[:, 1] - xlimits[:, 0])
+
+        full_hess = scipy.sparse.csc_matrix((num["dof"], num["dof"]))
+        for kx in range(num["x"]):
+            full_hess += sq_mtx[kx] * (
+                elem_vol
+                / total_vol
+                * self.options["smoothness"][kx]
+                / (xlimits[kx, 1] - xlimits[kx, 0]) ** 4
+            )
 
-        dy = self._predict_value_derivatives_hyper(x, u)
-        dMSE, MSE = self._predict_variance_derivatives_hyper(x, u)
+        return full_hess
 
-        return MSE, dy, dMSE
+    def _opt_func(self, sol, p, yt_dict):
+        full_hess = self.full_hess
+        full_jac_dict = self.full_jac_dict
+
+        func = 0.5 * np.dot(sol, full_hess * sol)
+        for kx in self.training_points[None]:
+            full_jac, full_jac_T, c = full_jac_dict[kx]
+            yt = yt_dict[kx]
+            func += 0.5 * c * np.sum((full_jac * sol - yt) ** p)
+
+        return func
+
+    def _opt_grad(self, sol, p, yt_dict):
+        full_hess = self.full_hess
+        full_jac_dict = self.full_jac_dict
+
+        grad = full_hess * sol
+        for kx in self.training_points[None]:
+            full_jac, full_jac_T, c = full_jac_dict[kx]
+            yt = yt_dict[kx]
+            grad += 0.5 * c * full_jac_T * p * (full_jac * sol - yt) ** (p - 1)
+
+        return grad
+
+    def _opt_dgrad_dyt(self, sol, p, yt_dict, kx):
+        full_hess = self.full_hess
+        full_jac_dict = self.full_jac_dict
+
+        full_jac, full_jac_T, c = full_jac_dict[kx]
+        yt = yt_dict[kx]
+
+        diag_vec = p * (p - 1) * (full_jac * sol - yt) ** (p - 2)
+        diag_mtx = scipy.sparse.diags(diag_vec, format="csc")
+        mtx = 0.5 * c * full_jac_T.dot(diag_mtx)
+
+        return -mtx.todense()
+
+    def _opt_hess(self, sol, p, yt_dict):
+        full_hess = self.full_hess
+        full_jac_dict = self.full_jac_dict
+
+        hess = scipy.sparse.csc_matrix(full_hess)
+        for kx in self.training_points[None]:
+            full_jac, full_jac_T, c = full_jac_dict[kx]
+            yt = yt_dict[kx]
+
+            diag_vec = p * (p - 1) * (full_jac * sol - yt) ** (p - 2)
+            diag_mtx = scipy.sparse.diags(diag_vec, format="csc")
+            hess += 0.5 * c * full_jac_T * diag_mtx * full_jac
+
+        return hess
+
+    def _opt_norm(self, sol, p, yt_dict):
+        full_hess = self.full_hess
+        full_jac_dict = self.full_jac_dict
+
+        grad = self._opt_grad(sol, p, yt_dict)
+        return np.linalg.norm(grad)
+
+    def _get_yt_dict(self, ind_y):
+        yt_dict = {}
+        for kx in self.training_points[None]:
+            xt, yt = self.training_points[None][kx]
+            yt_dict[kx] = yt[:, ind_y]
+        return yt_dict
+
+    def _run_newton_solver(self, sol):
+        num = self.num
+        options = self.options
+
+        solver = get_solver(options["solver"])
+        ls_class = get_line_search_class(options["line_search"])
+
+        total_size = int(num["dof"])
+        rhs = np.zeros((total_size, num["y"]))
+        d_sol = np.zeros((total_size, num["y"]))
+
+        p = self.options["approx_order"]
+        for ind_y in range(rhs.shape[1]):
+            with self.printer._timed_context("Solving for output %i" % ind_y):
+                yt_dict = self._get_yt_dict(ind_y)
+
+                norm = self._opt_norm(sol[:, ind_y], p, yt_dict)
+                fval = self._opt_func(sol[:, ind_y], p, yt_dict)
+                self.printer(
+                    "Iteration (num., iy, grad. norm, func.) : %3i %3i %15.9e %15.9e"
+                    % (0, ind_y, norm, fval)
+                )
 
-    def _predict_variances(self, x):
-        """
-        Predict the variance of a specific point
+                iter_count = 0
+                while (
+                    iter_count < options["nonlinear_maxiter"]
+                    and norm > options["solver_tolerance"]
+                ):
+                    with self.printer._timed_context():
+                        with self.printer._timed_context("Assembling linear system"):
+                            mtx = self._opt_hess(sol[:, ind_y], p, yt_dict)
+                            rhs[:, ind_y] = -self._opt_grad(sol[:, ind_y], p, yt_dict)
 
-        Parameters
-        ----------
-        x : numpy.ndarray
-            Point to compute.
-
-        Raises
-        ------
-        ValueError
-            The number fo dimension is not good.
+                        with self.printer._timed_context("Initializing linear solver"):
+                            solver._setup(mtx, self.printer)
 
-        Returns
-        -------
-        numpy.nd array
-            MSE.
-        """
-        MSE, dy, dMSE = self._predict_mgp_variances_base(x)
-        arg_1 = np.einsum("ij,ij->i", dy.T, linalg.solve(self.inv_sigma_R, dy).T)
-        arg_2 = np.einsum("ij,ij->i", dMSE.T, linalg.solve(self.inv_sigma_R, dMSE).T)
-
-        MGPMSE = np.zeros(x.shape[0])
-        MGPMSE[MSE != 0] = (
-            (4.0 / 3.0) * MSE[MSE != 0]
-            + arg_1[MSE != 0]
-            + (1.0 / (3.0 * MSE[MSE != 0])) * arg_2[MSE != 0]
-        )
-        MGPMSE[MGPMSE < 0.0] = 0.0
-        return MGPMSE
-
-    def predict_variances_no_uq(self, x):
-        """Like predict_variances but without taking account hyperparameters uncertainty"""
-        check_support(self, "variances")
-        x = ensure_2d_array(x, "x")
-        self._check_xdim(x)
-        n = x.shape[0]
-        x2 = np.copy(x)
-        s2, _, _ = self._predict_mgp_variances_base(x)
-        s2[s2 < 0.0] = 0.0
-        return s2.reshape((n, self.ny))
-
-    def _check_xdim(self, x):
-        _, n_features = x.shape
-        nx = self.nx
-        if n_features < self.nx:
-            nx = self.options["n_comp"]
-        check_nx(nx, x)
+                        with self.printer._timed_context("Solving linear system"):
+                            solver._solve(rhs[:, ind_y], d_sol[:, ind_y], ind_y=ind_y)
 
-    def _reduced_log_prior(self, theta, grad=False, hessian=False):
-        """
-        Compute the reduced log prior at given hyperparameters
+                        func = lambda x: self._opt_func(x, p, yt_dict)
+                        grad = lambda x: self._opt_grad(x, p, yt_dict)
 
-        Parameters
-        ----------
-        theta : numpy.ndarray
-            Hyperparameters.
-        grad : bool, optional
-            True to compuyte gradient. The default is False.
-        hessian : bool, optional
-            True to compute hessian. The default is False.
+                        # sol[:, ind_y] += d_sol[:, ind_y]
 
-        Returns
-        -------
-        res : numpy.ndarray
-            Value, gradient, hessian of the reduced log prior.
+                        ls = ls_class(sol[:, ind_y], d_sol[:, ind_y], func, grad)
+                        with self.printer._timed_context("Performing line search"):
+                            sol[:, ind_y] = ls(1.0)
 
-        """
-        nb_theta = len(theta)
+                    norm = self._opt_norm(sol[:, ind_y], p, yt_dict)
+                    fval = self._opt_func(sol[:, ind_y], p, yt_dict)
+                    self.printer(
+                        "Iteration (num., iy, grad. norm, func.) : %3i %3i %15.9e %15.9e"
+                        % (iter_count, ind_y, norm, fval)
+                    )
 
-        if theta.ndim < 2:
-            theta = np.atleast_2d(theta).T
+                    self.mtx = mtx
 
-        mean = np.ones((nb_theta, 1)) * self.options["prior"]["mean"]
-        sig_inv = np.eye(nb_theta) / self.options["prior"]["var"]
+                    iter_count += 1
 
-        if grad:
-            sig_inv_m = np.atleast_2d(np.sum(sig_inv, axis=0)).T
-            res = -2.0 * (theta - mean) * sig_inv_m
-        elif hessian:
-            res = -2.0 * np.atleast_2d(np.sum(sig_inv, axis=0)).T
-        else:
-            res = -np.dot((theta - mean).T, sig_inv.dot(theta - mean))
-        return res
+    def _solve(self):
+        num = self.num
+        options = self.options
 
-    def _predict_value_derivatives_hyper(self, x, u=None):
-        """
-        Compute the derivatives of the mean of the GP with respect to the hyperparameters
+        solver = get_solver(options["solver"])
+        ls_class = get_line_search_class(options["line_search"])
 
-        Parameters
-        ----------
-        x : numpy.ndarray
-            Point to compute in initial dimension.
-        u : numpy.ndarray, optional
-            Point to compute in small dimension. The default is None.
+        total_size = int(num["dof"])
+        rhs = np.zeros((total_size, num["y"]))
+        sol = np.zeros((total_size, num["y"]))
+        d_sol = np.zeros((total_size, num["y"]))
 
-        Returns
-        -------
-        dy : numpy.ndarray
-            Derivatives of the mean of the GP with respect to the hyperparameters.
+        with self.printer._timed_context(
+            "Solving initial startup problem (n=%i)" % total_size
+        ):
+            approx_order = options["approx_order"]
+            nonlinear_maxiter = options["nonlinear_maxiter"]
+            options["approx_order"] = 2
+            options["nonlinear_maxiter"] = 1
 
-        """
-        # Initialization
-        n_eval, _ = x.shape
+            self._run_newton_solver(sol)
 
-        # Get pairwise componentwise L1-distances to the input training set
-        dx = differences(x, Y=self.X_norma.copy())
-        d_x = self._componentwise_distance(dx)
-        if u is not None:
-            theta = np.eye(self.options["n_comp"]).reshape(
-                (self.options["n_comp"] ** 2,)
-            )
+            options["approx_order"] = approx_order
+            options["nonlinear_maxiter"] = nonlinear_maxiter
 
-            # Get pairwise componentwise L1-distances to the input training set
-            du = differences(u, Y=self.U_norma.copy())
-            d = self._componentwise_distance(du, small=True)
-        else:
-            theta = self.optimal_theta
+        with self.printer._timed_context(
+            "Solving nonlinear problem (n=%i)" % total_size
+        ):
+            self._run_newton_solver(sol)
 
-            # Get pairwise componentwise L1-distances to the input training set
-            d = d_x
-            d_x = None
+        return sol
 
-        # Compute the correlation function
-        r = self._correlation_types[self.options["corr"]](theta, d, d_x=d_x).reshape(
-            n_eval, self.nt
-        )
-        # Compute the regression function
-        f = self._regression_types[self.options["poly"]](x)
+    def _new_train(self):
+        """
+        Train the model
+        """
+        with self.printer._timed_context("Pre-computing matrices", "assembly"):
+            with self.printer._timed_context("Computing dof2coeff", "dof2coeff"):
+                self.full_dof2coeff = self._compute_dof2coeff()
 
-        dy = np.zeros((len(self.optimal_theta), n_eval))
+            with self.printer._timed_context("Initializing Hessian", "init_hess"):
+                self.full_hess = (
+                    self._setup_hessian() * self.options["regularization_weight"]
+                )
 
-        gamma = self.optimal_par["gamma"]
-        Rinv_dR_gamma = self.optimal_par["Rinv_dR_gamma"]
-        Rinv_dmu = self.optimal_par["Rinv_dmu"]
+            if self.options["min_energy"]:
+                with self.printer._timed_context("Computing energy terms", "energy"):
+                    self.full_hess += (
+                        self._compute_energy_terms() * self.options["energy_weight"]
+                    )
+
+            with self.printer._timed_context("Computing approximation terms", "approx"):
+                self.full_jac_dict = self._compute_approx_terms()
+
+        with self.printer._timed_context(
+            "Solving for degrees of freedom", "total_solution"
+        ):
+            self.sol = self._solve()
 
-        for omega in range(len(self.optimal_theta)):
-            drdomega = self._correlation_types[self.options["corr"]](
-                theta, d, grad_ind=omega, d_x=d_x
-            ).reshape(n_eval, self.nt)
+        if self.full_dof2coeff is not None:
+            self.sol_coeff = self.full_dof2coeff * self.sol
+        else:
+            self.sol_coeff = self.sol
 
-            dbetadomega = self.optimal_par["dbeta_all"][omega]
+    def _train(self):
+        """
+        Train the model
+        """
+        self._setup()
 
-            dy_omega = (
-                f.dot(dbetadomega)
-                + drdomega.dot(gamma)
-                - r.dot(Rinv_dR_gamma[omega] + Rinv_dmu[omega])
-            )
+        tmp = self.rmtsc
+        self.rmtsc = None
 
-            dy[omega, :] = dy_omega[:, 0]
+        inputs = {"self": self}
+        with cached_operation(inputs, self.options["data_dir"]) as outputs:
+            self.rmtsc = tmp
 
-        return dy
+            if outputs:
+                self.sol_coeff = outputs["sol_coeff"]
+                self.sol = outputs["sol"]
+                self.mtx = outputs["mtx"]
+                self.full_dof2coeff = outputs["full_dof2coeff"]
+                self.full_hess = outputs["full_hess"]
+                self.full_jac_dict = outputs["full_jac_dict"]
+            else:
+                self._new_train()
+                outputs["sol_coeff"] = self.sol_coeff
+                outputs["sol"] = self.sol
+                outputs["mtx"] = self.mtx
+                outputs["full_dof2coeff"] = self.full_dof2coeff
+                outputs["full_hess"] = self.full_hess
+                outputs["full_jac_dict"] = self.full_jac_dict
 
-    def _predict_variance_derivatives_hyper(self, x, u=None):
+    def _predict_values(self, x):
         """
-        Compute the derivatives of the variance of the GP with respect to the hyperparameters
+        Evaluates the model at a set of points.
 
-        Parameters
-        ----------
-        x : numpy.ndarray
-            Point to compute in initial dimension.
-        u : numpy.ndarray, optional
-            Point to compute in small dimension. The default is None.
+        Arguments
+        ---------
+        x : np.ndarray [n_evals, dim]
+            Evaluation point input variable values
 
         Returns
         -------
-        dMSE : numpy.ndarrray
-            derivatives of the variance of the GP with respect to the hyperparameters.
-        MSE : TYPE
-            Variance of the GP.
-
+        y : np.ndarray
+            Evaluation point output variable values
         """
-        # Initialization
-        n_eval, n_features_x = x.shape
-
-        # Get pairwise componentwise L1-distances to the input training set
-        dx = differences(x, Y=self.X_norma.copy())
-        d_x = self._componentwise_distance(dx)
-        if u is not None:
-            theta = np.eye(self.options["n_comp"]).reshape(
-                (self.options["n_comp"] ** 2,)
-            )
-            # Get pairwise componentwise L1-distances to the input training set
-            du = differences(u, Y=self.U_norma.copy())
-            d = self._componentwise_distance(du, small=True)
-        else:
-            theta = self.optimal_theta
-            # Get pairwise componentwise L1-distances to the input training set
-            d = d_x
-            d_x = None
-
-        # Compute the correlation function
-        r = (
-            self._correlation_types[self.options["corr"]](theta, d, d_x=d_x)
-            .reshape(n_eval, self.nt)
-            .T
-        )
-        f = self._regression_types[self.options["poly"]](x).T
-
-        C = self.optimal_par["C"]
-        G = self.optimal_par["G"]
-        Ft = self.optimal_par["Ft"]
-        sigma2 = self.optimal_par["sigma2"]
-
-        rt = linalg.solve_triangular(C, r, lower=True)
-
-        F_Rinv_r = np.dot(Ft.T, rt)
-
-        u_ = linalg.solve_triangular(G.T, f - F_Rinv_r)
-
-        MSE = self.optimal_par["sigma2"] * (
-            1.0 - (rt**2.0).sum(axis=0) + (u_**2.0).sum(axis=0)
-        )
-        # Mean Squared Error might be slightly negative depending on
-        # machine precision: force to zero!
-        MSE[MSE < 0.0] = 0.0
+        mtx = self._compute_prediction_mtx(x, 0)
+        y = mtx.dot(self.sol_coeff)
 
-        Ginv_u = linalg.solve_triangular(G, u_, lower=False)
-        Rinv_F = linalg.solve_triangular(C.T, Ft, lower=False)
-        Rinv_r = linalg.solve_triangular(C.T, rt, lower=False)
-        Rinv_F_Ginv_u = Rinv_F.dot(Ginv_u)
-
-        dMSE = np.zeros((len(self.optimal_theta), n_eval))
-
-        dr_all = self.optimal_par["dr"]
-        dsigma = self.optimal_par["dsigma"]
-
-        for omega in range(len(self.optimal_theta)):
-            drdomega = (
-                self._correlation_types[self.options["corr"]](
-                    theta, d, grad_ind=omega, d_x=d_x
-                )
-                .reshape(n_eval, self.nt)
-                .T
-            )
-
-            dRdomega = np.zeros((self.nt, self.nt))
-            dRdomega[self.ij[:, 0], self.ij[:, 1]] = dr_all[omega][:, 0]
-            dRdomega[self.ij[:, 1], self.ij[:, 0]] = dr_all[omega][:, 0]
-
-            # Compute du2dtheta
-
-            dRdomega_Rinv_F_Ginv_u = dRdomega.dot(Rinv_F_Ginv_u)
-            r_Rinv_dRdomega_Rinv_F_Ginv_u = np.einsum(
-                "ij,ij->i", Rinv_r.T, dRdomega_Rinv_F_Ginv_u.T
-            )
-            drdomega_Rinv_F_Ginv_u = np.einsum("ij,ij->i", drdomega.T, Rinv_F_Ginv_u.T)
-            u_Ginv_F_Rinv_dRdomega_Rinv_F_Ginv_u = np.einsum(
-                "ij,ij->i", Rinv_F_Ginv_u.T, dRdomega_Rinv_F_Ginv_u.T
-            )
-
-            du2domega = (
-                2.0 * r_Rinv_dRdomega_Rinv_F_Ginv_u
-                - 2.0 * drdomega_Rinv_F_Ginv_u
-                + u_Ginv_F_Rinv_dRdomega_Rinv_F_Ginv_u
-            )
-            du2domega = np.atleast_2d(du2domega)
-
-            # Compute drt2dtheta
-            drdomega_Rinv_r = np.einsum("ij,ij->i", drdomega.T, Rinv_r.T)
-            r_Rinv_dRdomega_Rinv_r = np.einsum(
-                "ij,ij->i", Rinv_r.T, dRdomega.dot(Rinv_r).T
-            )
-
-            drt2domega = 2.0 * drdomega_Rinv_r - r_Rinv_dRdomega_Rinv_r
-            drt2domega = np.atleast_2d(drt2domega)
-
-            dMSE[omega] = dsigma[omega] * MSE / sigma2 + sigma2 * (
-                -drt2domega + du2domega
-            )
-
-        return dMSE, MSE
+        return y
 
-    def get_x_from_u(self, u):
+    def _predict_derivatives(self, x, kx):
         """
-        Compute the point in initial dimension from a point in low dimension
+        Evaluates the derivatives at a set of points.
 
-        Parameters
-        ----------
-        u : numpy.ndarray
-            Point in low dimension.
+        Arguments
+        ---------
+        x : np.ndarray [n_evals, dim]
+            Evaluation point input variable values
+        kx : int
+            The 0-based index of the input variable with respect to which derivatives are desired.
 
         Returns
         -------
-        res : numpy.ndarray
-            point in initial dimension.
-
+        y : np.ndarray
+            Derivative values.
         """
-        u = np.atleast_2d(u)
+        mtx = self._compute_prediction_mtx(x, kx + 1)
+        y = mtx.dot(self.sol_coeff)
 
-        self.embedding["Q_C"], self.embedding["R_C"]
+        return y
 
-        x_temp = np.dot(
-            self.embedding["Q_C"],
-            linalg.solve_triangular(self.embedding["R_C"].T, u.T, lower=True),
-        ).T
+    def _compute_prediction_mtx(self, x, kx):
+        n = x.shape[0]
 
-        res = np.atleast_2d(x_temp)
-        return res
+        num = self.num
+        options = self.options
 
-    def get_u_from_x(self, x):
-        """
-        Compute the point in low dimension from a point in initial dimension
+        data, rows, cols = self._compute_jac_raw(kx, 0, x)
 
-        Parameters
-        ----------
-        x : numpy.ndarray
-            Point in initial dimension.
+        # In the explanation below, n is the number of dimensions, and
+        # a_k and b_k are the lower and upper bounds for x_k.
+        #
+        # A C1 extrapolation can get very tricky, so we implement a simple C0
+        # extrapolation. We basically linarly extrapolate from the nearest
+        # domain point. For example, if n = 4 and x2 > b2 and x3 > b3:
+        #    f(x1,x2,x3,x4) = f(x1,b2,b3,x4) + dfdx2 (x2-b2) + dfdx3 (x3-b3)
+        #    where the derivatives are evaluated at x1,b2,b3,x4 (called b) and
+        #    dfdx1|x = dfdx1|b + d2fdx1dx2|b (x2-b2) + d2fdx1dx3|b (x3-b3)
+        #    dfdx2|x = dfdx2|b.
+        # The dfdx2|x derivative is what it is because f and all derivatives
+        # evaluated at x1,b2,b3,x4 are constant with respect to changes in x2.
+        # On the other hand, the dfdx1|x derivative is what it is because
+        # f and all derivatives evaluated at x1,b2,b3,x4 change with x1.
+        # The extrapolation function is non-differentiable at boundaries:
+        # i.e., where x_k = a_k or x_k = b_k for at least one k.
+        if options["extrapolate"]:
+            # First we evaluate the vector pointing to each evaluation points
+            # from the nearest point on the domain, in a matrix called dx.
+            # If the ith evaluation point is not external, dx[i, :] = 0.
+            dx = np.empty(n * num["support"] * num["x"])
+            self.rmtsc.compute_ext_dist(n, num["support"], x.flatten(), dx)
+            dx = dx.reshape((n * num["support"], num["x"]))
+
+            isexternal = np.array(np.array(dx, bool), float)
+
+            for ix in range(num["x"]):
+                # Now we compute the first order term where we have a
+                # derivative times (x_k - b_k) or (x_k - a_k).
+                data_tmp, rows, cols = self._compute_jac_raw(kx, ix + 1, x)
+                data_tmp *= dx[:, ix]
+
+                # If we are evaluating a derivative (with index kx),
+                # we zero the first order terms for which dx_k = 0.
+                if kx != 0:
+                    data_tmp *= 1 - isexternal[:, kx - 1]
 
-        Returns
-        -------
-        u : numpy.ndarray
-             Point in low dimension.
+                data += data_tmp
 
-        """
-        u = x.dot(self.embedding["C"])
-        return u
+        mtx = scipy.sparse.csc_matrix((data, (rows, cols)), shape=(n, num["coeff"]))
+        return mtx
 
-    def _specific_train(self):
-        """
-        Compute the specific training values necessary for MGP (Hessian)
-        """
-        # Compute covariance matrix of hyperparameters
-        var_R = np.zeros((len(self.optimal_theta), len(self.optimal_theta)))
-        r, r_ij, par = self._reduced_likelihood_hessian(self.optimal_theta)
-        var_R[r_ij[:, 0], r_ij[:, 1]] = r[:, 0]
-        var_R[r_ij[:, 1], r_ij[:, 0]] = r[:, 0]
-
-        self.inv_sigma_R = -var_R
-
-        # Compute normalise embedding
-        self.optimal_par = par
-
-        A = np.reshape(self.optimal_theta, (self.options["n_comp"], self.nx)).T
-        B = (A.T / self.X_scale).T
-        norm_B = np.linalg.norm(B)
-        C = B / norm_B
-
-        self.embedding = {}
-        self.embedding["A"] = A
-        self.embedding["C"] = C
-        self.embedding["norm"] = norm_B
-        self.embedding["Q_C"], self.embedding["R_C"] = linalg.qr(C, mode="economic")
-
-        # Compute normalisation in embeding base
-        self.U_norma = self.X_norma.dot(A)
-        self.U_mean = self.X_offset.dot(C) * norm_B
-
-        # Compute best number of Components for Active Kriging
-        svd = linalg.svd(A)
-        svd_cumsum = np.cumsum(svd[1])
-        svd_sum = np.sum(svd[1])
-        self.best_ncomp = min(np.argwhere(svd_cumsum > 0.99 * svd_sum)) + 1
+    def _predict_output_derivatives(self, x):
+        # dy_dyt = dy_dw * (dR_dw)^{-1} * dR_dyt
 
-    def _check_param(self):
-        """
-        Overrides KrgBased implementation
-        This function checks some parameters of the model.
-        """
+        n = x.shape[0]
+        nw = self.mtx.shape[0]
+        nx = x.shape[1]
+        ny = self.sol.shape[1]
+
+        p = self.options["approx_order"]
+
+        dy_dw = self._compute_prediction_mtx(x, 0)
+        if self.full_dof2coeff is not None:
+            dy_dw = dy_dw * self.full_dof2coeff
+        dy_dw = dy_dw.todense()
+
+        dR_dw = self.mtx
+
+        dy_dyt = {}
+        for kx in self.training_points[None]:
+            nt = self.training_points[None][kx][0].shape[0]
+
+            dR_dyt = np.zeros((nw, nt, ny))
+            for ind_y in range(ny):
+                yt_dict = self._get_yt_dict(ind_y)
+                dR_dyt[:, :, ind_y] = self._opt_dgrad_dyt(
+                    self.sol[:, ind_y], p, yt_dict, kx
+                )
+
+            solver = get_solver(self.options["derivative_solver"])
+            solver._setup(dR_dw, self.printer)
 
-        d = self.options["n_comp"] * self.nx
+            dw_dyt = np.zeros((nw, nt, ny))
+            for ind_t in range(nt):
+                for ind_y in range(ny):
+                    solver._solve(
+                        dR_dyt[:, ind_t, ind_y], dw_dyt[:, ind_t, ind_y], ind_y=ind_y
+                    )
+                    dw_dyt[:, ind_t, ind_y] *= -1.0
 
-        if self.options["corr"] != "act_exp":
-            raise ValueError("MGP must be used with act_exp correlation function")
-        if self.options["hyper_opt"] != "TNC":
-            raise ValueError("MGP must be used with TNC hyperparameters optimizer")
-
-        if len(self.options["theta0"]) != d:
-            if len(self.options["theta0"]) == 1:
-                self.options["theta0"] *= np.ones(d)
+            if kx == 0:
+                dy_dyt[None] = np.einsum("ij,jkl->ikl", dy_dw, dw_dyt)
             else:
-                raise ValueError(
-                    "the number of dim %s should be equal to the length of theta0 %s."
-                    % (d, len(self.options["theta0"]))
-                )
+                dy_dyt[kx - 1] = np.einsum("ij,jkl->ikl", dy_dw, dw_dyt)
+
+        return dy_dyt
```

### Comparing `smt-2.0b2/smt/surrogate_models/qp.py` & `smt-2.0b3/smt/surrogate_models/qp.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/rbf.py` & `smt-2.0b3/smt/surrogate_models/rbf.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/rmtb.py` & `smt-2.0b3/smt/surrogate_models/rmtb.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/rmtc.py` & `smt-2.0b3/smt/surrogate_models/rmtc.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/surrogate_models/surrogate_model.py` & `smt-2.0b3/smt/surrogate_models/surrogate_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         self.supports = supports = {}
         supports["training_derivatives"] = False
         supports["derivatives"] = False
         supports["output_derivatives"] = False
         supports["adjoint_api"] = False
         supports["variances"] = False
         supports["variance_derivatives"] = False
+        supports["x_hierarchy"] = False
 
         declare = self.options.declare
 
         declare(
             "print_global",
             True,
             types=bool,
@@ -283,14 +284,15 @@
         Returns
         -------
         y : np.ndarray[nt, ny]
             Output values at the prediction points.
         """
         x = ensure_2d_array(x, "x")
         self._check_xdim(x)
+
         n = x.shape[0]
         x2 = np.copy(x)
         self.printer.active = (
             self.options["print_global"] and self.options["print_prediction"]
         )
 
         if self.name == "MixExp":
@@ -388,14 +390,15 @@
         -------
         s2 : np.ndarray[nt, ny]
             Variances.
         """
         check_support(self, "variances")
         x = ensure_2d_array(x, "x")
         self._check_xdim(x)
+
         n = x.shape[0]
         x2 = np.copy(x)
         s2 = self._predict_variances(x2)
         return s2.reshape((n, self.ny))
 
     def predict_variance_derivatives(self, x, kx):
         """
@@ -539,14 +542,16 @@
 
         in the _initialize() implementation.
 
         Parameters
         ----------
         x : np.ndarray[nt, nx]
             Input values for the prediction points.
+        is_acting : np.ndarray[nt, nx] or np.ndarray[nt]
+            Matrix specifying for each design variable whether it is acting or not (for hierarchical design spaces)
 
         Returns
         -------
         s2 : np.ndarray[nt, ny]
             Variances.
         """
         check_support(self, "variances", fail=True)
```

### Comparing `smt-2.0b2/smt/utils/caching.py` & `smt-2.0b3/smt/utils/caching.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/checks.py` & `smt-2.0b3/smt/utils/checks.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/krg_sampling.py` & `smt-2.0b3/smt/utils/krg_sampling.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/kriging.py` & `smt-2.0b3/smt/utils/kriging.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,146 +1,58 @@
 """
 Author: Dr. Mohamed A. Bouhlel <mbouhlel@umich.edu>
 
 This package is distributed under New BSD license.
 """
-
+import warnings
 import numpy as np
 from enum import Enum
 from copy import deepcopy
 
 from sklearn.cross_decomposition import PLSRegression as pls
 
 from pyDOE2 import bbdesign
 from sklearn.metrics.pairwise import check_pairwise_arrays
-from smt.utils.mixed_integer import XType
-
-MixHrcKernelType = Enum("MixHrcKernelType", ["ARC_KERNEL", "ALG_KERNEL"])
-## This define the variables roles for hierarchical Kriging models
-XRole = Enum("XType", ["NEUTRAL", "META", "DECREED"])
-
-
-class XSpecs:
-    """
-    A class to specify input variables type and domain
-
-    Attributes
-    ----------
-    _xtypes : list
-        list of mixed integer variables types
+from smt.utils.design_space import BaseDesignSpace, CategoricalVariable
 
-    _xlimits : np.array
-        list of corresponding domain which depends on variables types
+try:
+    from numba import njit, prange
 
-    _xroles : np.array
-        list of mixed integer variables roles
-    """
+    USE_NUMBA_JIT = True  # Set False to temporarily disable
 
-    def __init__(self, xtypes=None, xlimits=None, xroles=None):
-        self._xlimits = xlimits
-        if (
-            xtypes is None and xlimits is not None
-        ):  # when xtypes is not specified default to float
-            self._xtypes = [XType.FLOAT] * len(xlimits)
-        else:
-            self._xtypes = xtypes
-        if (
-            xroles is None and xlimits is not None
-        ):  # when xroles is not specified default to neutral
-            self._xroles = [XRole.NEUTRAL] * len(xlimits)
-        else:
-            self._xroles = xroles
-        self._check_consistency()
+except ImportError:  # pip install smt[numba]
+    USE_NUMBA_JIT = False
+    prange = range
 
-    @property
-    def roles(self):
-        return self._xroles
-
-    @property
-    def types(self):
-        return self._xtypes
-
-    @property
-    def limits(self):
-        return self._xlimits
-
-    @roles.setter
-    def roles(self, xroles):
-        self._xroles = xroles
-        self._check_consistency()
-
-    @types.setter
-    def types(self, xtypes):
-        self._xtypes = xtypes
-        self._check_consistency()
-
-    @limits.setter
-    def limits(self, xlimits):
-        self._xlimits = xlimits
-        self._check_consistency()
-
-    def clone(self):
-        """
-        Return a clone of this object.
-        Returns
-        -------
-            Deep-copied clone.
-        """
-        return XSpecs(
-            deepcopy(self._xtypes), deepcopy(self._xlimits), deepcopy(self._xroles)
-        )
+"""
+Quick benchmarking with the mixed-integer hierarchical Goldstein function indicates the following:
 
-    def _check_consistency(self):
-        if self._xlimits is None:
-            raise ValueError("xlimits not specified in xspecs")
+| Scenario                 | No numba | Numba   | Numba with caching | Speedup | Overhead |
+|--------------------------|----------|---------|--------------------|---------|----------|
+| HGoldstein 15 pt DoE     | 1.3 sec  | ~25 sec | 1.1 sec            | 15%     | 24 sec   |
+| HGoldstein 150 pt DoE    | 38 sec   | ~29 sec | 7.4 sec            | 80%     | 23 sec   |
 
-        if self._xtypes is None:
-            raise ValueError("xtypes not specified in xspecs")
+Important to note: caching is only needed once after installation of smt, so users will only
+experience this overhead ONCE --> the rest of the time they use smt it will be faster than without numba!
+"""
 
-        if self._xroles is None:
-            raise ValueError("xroles not specified in xspecs")
 
-        if len(self._xlimits) != len(self._xtypes):
-            raise ValueError(
-                f"number of x limits ({len(self._xlimits)}) do not"
-                f" correspond to number of specified types ({len(self._xtypes)})"
-            )
+def njit_use(parallel=False):
+    if USE_NUMBA_JIT:
+        # njit:          https://numba.readthedocs.io/en/stable/user/jit.html#nopython
+        # cache=True:    https://numba.readthedocs.io/en/stable/user/jit.html#cache
+        # parallel=True: https://numba.readthedocs.io/en/stable/user/parallel.html
+        return njit(parallel=parallel, cache=True)
+
+    return lambda func: func
 
-        if len(self._xlimits) != len(self._xroles):
-            raise ValueError(
-                f"number of x limits ({len(self._xlimits)}) do not"
-                f" correspond to number of specified roles ({len(self._xroles)})"
-            )
 
-        for i, xtyp in enumerate(self._xtypes):
-            if (not isinstance(xtyp, tuple)) and len(self._xlimits[i]) != 2:
-                if xtyp == XType.ORD and isinstance(self._xlimits[i][0], str):
-                    listint = list(map(float, self._xlimits[i]))
-                    sortedlistint = sorted(listint)
-                    if not np.array_equal(sortedlistint, listint):
-                        raise ValueError(
-                            f"Unsorted x limits ({self._xlimits[i]}) for variable type {xtyp} (index={i})"
-                        )
-                else:
-                    raise ValueError(
-                        f"Bad x limits ({self._xlimits[i]}) for variable type {xtyp} (index={i})"
-                    )
-            if (
-                xtyp != XType.FLOAT
-                and xtyp != XType.ORD
-                and (not isinstance(xtyp, tuple) or xtyp[0] != XType.ENUM)
-            ):
-                raise ValueError(f"Bad type specification {xtyp}")
-
-            if isinstance(xtyp, tuple) and len(self._xlimits[i]) != xtyp[1]:
-                raise ValueError(
-                    f"Bad x limits and x types specs not consistent. "
-                    f"Got a categorical type with {xtyp[1]} levels "
-                    f"while x limits contains {len(self._xlimits[i])} values (index={i})"
-                )
+class MixHrcKernelType(Enum):
+    ARC_KERNEL = "ARC_KERNEL"
+    ALG_KERNEL = "ALG_KERNEL"
 
 
 def cross_distances(X, y=None):
     """
     Computes the nonzero componentwise cross-distances between the vectors
     in X or between the vectors in X and the vectors in y.
 
@@ -162,85 +74,112 @@
               distances in D.
     """
     n_samples, n_features = X.shape
     if y is None:
         n_nonzero_cross_dist = n_samples * (n_samples - 1) // 2
         ij = np.zeros((n_nonzero_cross_dist, 2), dtype=np.int32)
         D = np.zeros((n_nonzero_cross_dist, n_features))
-        ll_1 = 0
 
-        for k in range(n_samples - 1):
-            ll_0 = ll_1
-            ll_1 = ll_0 + n_samples - k - 1
-            ij[ll_0:ll_1, 0] = k
-            ij[ll_0:ll_1, 1] = np.arange(k + 1, n_samples)
-            D[ll_0:ll_1] = X[k] - X[(k + 1) : n_samples]
+        _cross_dist_mat(n_samples, ij, X, D)
     else:
         n_y, n_features = y.shape
         X, y = check_pairwise_arrays(X, y)
         n_nonzero_cross_dist = n_samples * n_y
         ij = np.zeros((n_nonzero_cross_dist, 2), dtype=np.int32)
         D = np.zeros((n_nonzero_cross_dist, n_features))
-        for k in range(n_nonzero_cross_dist):
-            xk = k // n_y
-            yk = k % n_y
-            D[k] = X[xk] - y[yk]
-            ij[k, 0] = xk
-            ij[k, 1] = yk
+
+        _cross_dist_mat_y(n_nonzero_cross_dist, n_y, X, y, D, ij)
 
     return D, ij.astype(np.int32)
 
 
-def cross_levels(X, ij, xtypes, y=None):
+@njit_use()
+def _cross_dist_mat(n_samples, ij, X, D):
+    ll_1 = 0
+    for k in range(n_samples - 1):
+        ll_0 = ll_1
+        ll_1 = ll_0 + n_samples - k - 1
+        ij[ll_0:ll_1, 0] = k
+        ij[ll_0:ll_1, 1] = np.arange(k + 1, n_samples)
+        D[ll_0:ll_1] = X[k] - X[(k + 1) : n_samples]
+
+
+@njit_use()
+def _cross_dist_mat_y(n_nonzero_cross_dist, n_y, X, y, D, ij):
+    for k in prange(n_nonzero_cross_dist):
+        xk = k // n_y
+        yk = k % n_y
+        D[k] = X[xk] - y[yk]
+        ij[k, 0] = xk
+        ij[k, 1] = yk
+
+
+def cross_levels(X, ij, design_space, y=None):
     """
     Returns the levels corresponding to the indices i and j of the vectors in X and the number of levels.
     Parameters
     ----------
 
     X: np.ndarray [n_obs, dim]
             - The input variables.
     y: np.ndarray [n_y, dim]
             - The training data.
     ij: np.ndarray [n_obs * (n_obs - 1) / 2, 2]
             - The indices i and j of the vectors in X associated to the cross-
               distances in D.
-    xtypes: np.ndarray [dim]
-            -the types (FLOAT,ORD,ENUM) of the input variables
+    design_space: BaseDesignSpace
+        - The design space definition
     Returns
     -------
 
      Lij: np.ndarray [n_obs * (n_obs - 1) / 2, 2]
             - The levels corresponding to the indices i and j of the vectors in X.
      n_levels: np.ndarray
             - The number of levels for every categorical variable.
     """
 
     n_levels = []
-    for i, xtyp in enumerate(xtypes):
-        if isinstance(xtyp, tuple):
-            n_levels.append(xtyp[1])
+    for dv in design_space.design_variables:
+        if isinstance(dv, CategoricalVariable):
+            n_levels.append(dv.n_values)
     n_levels = np.array(n_levels)
     n_var = n_levels.shape[0]
     n, _ = ij.shape
-    X_cont, cat_features = compute_X_cont(X, xtypes)
+    X_cont, cat_features = compute_X_cont(X, design_space)
     X_cat = X[:, cat_features]
 
+    if y is None:
+        Lij = _cross_levels_mat(n_var, n, X_cat, ij)
+    else:
+        Lij = _cross_levels_mat_y(n_var, n, X_cat, ij, y, cat_features)
+
+    return Lij, n_levels
+
+
+@njit_use(parallel=True)
+def _cross_levels_mat(n_var, n, X_cat, ij):
     Lij = np.zeros((n_var, n, 2))
-    for k in range(n_var):
-        for l in range(n):
+    for k in prange(n_var):
+        for l in prange(n):
             i, j = ij[l]
-            if y is None:
-                Lij[k][l][0] = X_cat[i, k]
-                Lij[k][l][1] = X_cat[j, k]
-            else:
-                y_cat = y[:, cat_features]
-                Lij[k][l][0] = X_cat[i, k]
-                Lij[k][l][1] = y_cat[j, k]
+            Lij[k][l][0] = X_cat[i, k]
+            Lij[k][l][1] = X_cat[j, k]
+    return Lij
 
-    return Lij, n_levels
+
+@njit_use(parallel=True)
+def _cross_levels_mat_y(n_var, n, X_cat, ij, y, cat_features):
+    Lij = np.zeros((n_var, n, 2))
+    y_cat = y[:, cat_features]
+    for k in prange(n_var):
+        for l in prange(n):
+            i, j = ij[l]
+            Lij[k][l][0] = X_cat[i, k]
+            Lij[k][l][1] = y_cat[j, k]
+    return Lij
 
 
 def cross_levels_homo_space(X, ij, y=None):
     """
     Computes the nonzero componentwise (or Hadamard) product between the vectors in X
     Parameters
     ----------
@@ -267,136 +206,148 @@
             dx[l] = X[i] * X[j]
         else:
             dx[l] = X[i] * y[j]
 
     return dx
 
 
-def compute_X_cont(x, xtypes):
+def compute_X_cont(x, design_space):
     """
-    Some parts were extracted from gower 0.0.5 library
-    Computes the X_cont part of a vector x for mixed integer
+    Gets the X_cont part of a vector x for mixed integer
     Parameters
     ----------
     x: np.ndarray [n_obs, dim]
             - The input variables.
-    xtypes: np.ndarray [dim]
-            -the types (FLOAT,ORD,ENUM) of the input variables
+    design_space : BaseDesignSpace
+        - The design space definition
     Returns
     -------
     X_cont: np.ndarray [n_obs, dim_cont]
          - The non categorical values of the input variables.
     cat_features: np.ndarray [dim]
         -  Indices of the categorical input dimensions.
 
     """
-    if xtypes is None:
-        return x, None
-    cat_features = [
-        not (xtype == XType.FLOAT or xtype == XType.ORD) for xtype in xtypes
-    ]
-    return x[:, np.logical_not(cat_features)], cat_features
+    is_cat_mask = design_space.is_cat_mask
+    return x[:, ~is_cat_mask], is_cat_mask
 
 
-def gower_componentwise_distances(X, xspecs, hierarchical_kernel, y=None):
+def gower_componentwise_distances(
+    X, x_is_acting, design_space, hierarchical_kernel, y=None, y_is_acting=None
+):
     """
     Computes the nonzero Gower-distances componentwise between the vectors
     in X.
     Parameters
     ----------
     X: np.ndarray [n_obs, dim]
-            - The input variables.
+        - The input variables.
+    x_is_acting: np.ndarray [n_obs, dim]
+        - is_acting matrix for the inputs
+    design_space : BaseDesignSpace
+        - The design space definition
     y: np.ndarray [n_y, dim]
-            - The training data.
-    xspecs : XSpecs object including
-        xlimits: np.ndarray[dim, 2]
-                - The upper and lower var bounds.
-        xtypes: np.ndarray [dim]
-                - The types (FLOAT,ORD,ENUM) of the input variables
-        xroles: np.ndarray [dim]
-                - The roles (NEUTRAL,META,DECREED) of the input variables
+        - The training data
+    y_is_acting: np.ndarray [n_y, dim]
+        - is_acting matrix for the training points
     Returns
     -------
     D: np.ndarray [n_obs * (n_obs - 1) / 2, dim]
             - The gower distances between the vectors in X.
     ij: np.ndarray [n_obs * (n_obs - 1) / 2, 2]
             - The indices i and j of the vectors in X associated to the cross-
               distances in D.
     X_cont: np.ndarray [n_obs, dim_cont]
          - The non categorical values of the input variables.
     """
     X = X.astype(np.float64)
     Xt = X
-    X_cont, cat_features = compute_X_cont(Xt, xspecs.types)
+    X_cont, cat_features = compute_X_cont(Xt, design_space)
+    is_decreed = design_space.is_conditionally_acting
 
     # function checks
     if y is None:
         Y = X
+        y_is_acting = x_is_acting
     else:
         Y = y
+        if y_is_acting is None:
+            raise ValueError(f"Expected y_is_acting because y is given")
+
     if not isinstance(X, np.ndarray):
         if not np.array_equal(X.columns, Y.columns):
             raise TypeError("X and Y must have same columns!")
     else:
         if not X.shape[1] == Y.shape[1]:
             raise TypeError("X and Y must have same y-dim!")
+
+    if x_is_acting.shape != X.shape or y_is_acting.shape != Y.shape:
+        raise ValueError(f"is_acting matrices must have same shape as X!")
+
     x_n_rows, x_n_cols = X.shape
     y_n_rows, y_n_cols = Y.shape
     if not isinstance(X, np.ndarray):
         X = np.asarray(X)
     if not isinstance(Y, np.ndarray):
         Y = np.asarray(Y)
+
     Z = np.concatenate((X, Y))
+    z_is_acting = np.concatenate((x_is_acting, y_is_acting))
+    Z_cat = Z[:, cat_features]
+    z_cat_is_acting = z_is_acting[:, cat_features]
+    cat_is_decreed = is_decreed[cat_features]
+
     x_index = range(0, x_n_rows)
     y_index = range(x_n_rows, x_n_rows + y_n_rows)
-    Z_cat = Z[:, cat_features]
     X_cat = Z_cat[x_index,]
     Y_cat = Z_cat[y_index,]
+    x_cat_is_acting = z_cat_is_acting[x_index,]
+    y_cat_is_acting = z_cat_is_acting[y_index,]
+
+    # To support categorical decreed variables, some extra math wizardry is needed
+    if np.any(cat_is_decreed) or np.any(~x_cat_is_acting) or np.any(~y_cat_is_acting):
+        raise ValueError(
+            "Decreed (conditionally-active) categorical variables are not supported yet!"
+        )
 
     # This is to normalize the numeric values between 0 and 1.
-    Z_num = Z[:, np.logical_not(cat_features)]
-    lim = np.array(xspecs.limits, dtype=object)[np.logical_not(cat_features)]
-    lb = np.zeros(np.shape(lim)[0])
-    ub = np.ones(np.shape(lim)[0])
-    max_meta_num = 1
-    if np.shape(lim)[0] > 0:
-        for k, i in enumerate(lim):
-            if xspecs.roles[k] != XRole.META:
-                lb[k] = i[0]
-                ub[k] = i[-1]
-            else:
-                max_meta_num = i[-1]
-        Z_offset = lb
-        Z_max = ub
+    Z_num = Z[:, ~cat_features]
+    z_num_is_acting = z_is_acting[:, ~cat_features]
+    num_is_decreed = is_decreed[~cat_features]
+    num_bounds = design_space.get_num_bounds()[~cat_features, :]
+    if num_bounds.shape[0] > 0:
+        Z_offset = num_bounds[:, 0]
+        Z_max = num_bounds[:, 1]
         Z_scale = Z_max - Z_offset
         Z_num = (Z_num - Z_offset) / Z_scale
     X_num = Z_num[x_index,]
     Y_num = Z_num[y_index,]
+    x_num_is_acting = z_num_is_acting[x_index,]
+    y_num_is_acting = z_num_is_acting[y_index,]
 
     D_cat = compute_D_cat(X_cat, Y_cat, y)
     D_num, ij = compute_D_num(
         X_num,
         Y_num,
+        x_num_is_acting,
+        y_num_is_acting,
+        num_is_decreed,
         y,
-        xspecs,
-        X_cat,
-        Y_cat,
-        cat_features,
-        max_meta_num,
         hierarchical_kernel,
     )
     D = np.concatenate((D_cat, D_num), axis=1) * 0
     D[:, np.logical_not(cat_features)] = D_num
     D[:, cat_features] = D_cat
     if y is not None:
         return D
     else:
         return D, ij.astype(np.int32), X_cont
 
 
+@njit_use(parallel=True)
 def compute_D_cat(X_cat, Y_cat, y):
     nx_samples, n_features = X_cat.shape
     ny_samples, n_features = Y_cat.shape
     n_nonzero_cross_dist = nx_samples * ny_samples
     if y is None:
         n_nonzero_cross_dist = nx_samples * (nx_samples - 1) // 2
     D_cat = np.zeros((n_nonzero_cross_dist, n_features))
@@ -404,35 +355,33 @@
     k1max = nx_samples
     if y is None:
         k1max = nx_samples - 1
     for k1 in range(k1max):
         k2max = ny_samples
         if y is None:
             k2max = ny_samples - k1 - 1
-        for k2 in range(k2max):
+        for k2 in prange(k2max):
             l2 = k2
             if y is None:
                 l2 = k2 + k1 + 1
-            D_cat[indD] = X_cat[k1] != Y_cat[l2]
-            indD += 1
+            D_cat[indD + k2] = X_cat[k1] != Y_cat[l2]
+        indD += k2max
     return D_cat
 
 
+@njit_use()  # setting parallel=True results in a stack overflow
 def compute_D_num(
     X_num,
     Y_num,
+    x_num_is_acting,
+    y_num_is_acting,
+    num_is_decreed,
     y,
-    xspecs,
-    X_cat,
-    Y_cat,
-    cat_features,
-    max_meta_num,
     hierarchical_kernel,
 ):
-    active_roles = len(xspecs.limits) * [XRole.NEUTRAL] != xspecs.roles
     nx_samples, n_features = X_num.shape
     ny_samples, n_features = Y_num.shape
     n_nonzero_cross_dist = nx_samples * ny_samples
     if y is None:
         n_nonzero_cross_dist = nx_samples * (nx_samples - 1) // 2
     D_num = np.zeros((n_nonzero_cross_dist, n_features))
     ij = np.zeros((n_nonzero_cross_dist, 2), dtype=np.int32)
@@ -451,140 +400,85 @@
             ij[ll_0:ll_1, 1] = np.arange(k1 + 1, nx_samples)
         for k2 in range(k2max):
             l2 = k2
             if y is None:
                 l2 = k2 + k1 + 1
             D_num[indD] = np.abs(X_num[k1] - Y_num[l2])
             indD += 1
-    if active_roles:
+
+    if np.any(num_is_decreed):
         D_num = apply_the_algebraic_distance_to_the_decreed_variable(
-            xspecs,
             X_num,
             Y_num,
+            x_num_is_acting,
+            y_num_is_acting,
+            num_is_decreed,
             y,
-            max_meta_num,
-            cat_features,
-            X_cat,
-            Y_cat,
             D_num,
             hierarchical_kernel,
         )
 
     return D_num, ij
 
 
+@njit_use()  # setting parallel=True results in a stack overflow
 def apply_the_algebraic_distance_to_the_decreed_variable(
-    xspecs,
     X_num,
     Y_num,
+    x_num_is_acting,
+    y_num_is_acting,
+    num_is_decreed,
     y,
-    max_meta_num,
-    cat_features,
-    X_cat,
-    Y_cat,
     D_num,
     hierarchical_kernel,
 ):
     nx_samples, n_features = X_num.shape
     ny_samples, n_features = Y_num.shape
-    decreed_features = np.array([(xrole == XRole.DECREED) for xrole in xspecs.roles])
-    meta_features = np.array([(xrole == XRole.META) for xrole in xspecs.roles])
-    decreed_num_features = decreed_features[np.logical_not(cat_features)]
-    meta_num_features = meta_features[np.logical_not(cat_features)]
-    meta_cat_features = meta_features[cat_features]
 
     indD = 0
     k1max = nx_samples
     if y is None:
         k1max = nx_samples - 1
     for k1 in range(k1max):
         k2max = ny_samples
         if y is None:
             k2max = ny_samples - k1 - 1
+        x_k1_acting = x_num_is_acting[k1]
         for k2 in range(k2max):
             l2 = k2
             if y is None:
                 l2 = k2 + k1 + 1
             abs_delta = np.abs(X_num[k1] - Y_num[l2])
+            y_l2_acting = y_num_is_acting[l2]
 
+            # Calculate the distances between the decreed (aka conditionally acting) variables
             if hierarchical_kernel == MixHrcKernelType.ALG_KERNEL:
-                abs_delta[decreed_num_features] = (
+                abs_delta[num_is_decreed] = (
                     2
-                    * np.abs(
-                        X_num[k1][decreed_num_features]
-                        - Y_num[l2][decreed_num_features]
-                    )
+                    * np.abs(X_num[k1][num_is_decreed] - Y_num[l2][num_is_decreed])
                     / (
-                        np.sqrt(1 + X_num[k1][decreed_num_features] ** 2)
-                        * np.sqrt(1 + Y_num[l2][decreed_num_features] ** 2)
+                        np.sqrt(1 + X_num[k1][num_is_decreed] ** 2)
+                        * np.sqrt(1 + Y_num[l2][num_is_decreed] ** 2)
                     )
                 )
             elif hierarchical_kernel == MixHrcKernelType.ARC_KERNEL:
-                abs_delta[decreed_num_features] = np.sqrt(2) * np.sqrt(
+                abs_delta[num_is_decreed] = np.sqrt(2) * np.sqrt(
                     1
                     - np.cos(
                         np.pi
-                        * np.abs(
-                            X_num[k1][decreed_num_features]
-                            - Y_num[l2][decreed_num_features]
-                        )
+                        * np.abs(X_num[k1][num_is_decreed] - Y_num[l2][num_is_decreed])
                     )
                 )
-            abs_delta[meta_num_features] = abs_delta[meta_num_features] / max_meta_num
 
-            if np.max(meta_num_features):
-                # This is the meta variable index
-                minmeta = int(
-                    np.min([X_num[k1][meta_num_features], Y_num[l2][meta_num_features]])
-                )
-                maxmeta = int(
-                    np.max([X_num[k1][meta_num_features], Y_num[l2][meta_num_features]])
-                )
-                ind_dec = min((decreed_num_features).nonzero()[0])
-                abs_delta[minmeta + ind_dec :] = abs_delta[minmeta + ind_dec :] * 0 + 1
-                abs_delta[maxmeta + ind_dec :] = abs_delta[maxmeta + ind_dec :] * 0
-            if np.max(meta_cat_features):
-                # This is the meta variable index
-                from smt.utils.mixed_integer import cast_to_enum_value
-
-                actives_x1 = np.array(
-                    list(
-                        map(
-                            int,
-                            cast_to_enum_value(
-                                xspecs.limits,
-                                np.where(meta_features * cat_features)[0][0],
-                                np.int32(X_cat[k1][meta_cat_features]),
-                            )[0].split(","),
-                        )
-                    )
-                )
-                actives_y2 = np.array(
-                    list(
-                        map(
-                            int,
-                            cast_to_enum_value(
-                                xspecs.limits,
-                                np.where(meta_features * cat_features)[0][0],
-                                np.int32(Y_cat[l2][meta_cat_features]),
-                            )[0].split(","),
-                        )
-                    )
-                )
-                actives_both = np.array(list(set(actives_x1).intersection(actives_y2)))
-                decreed_num_features_inactives = np.copy(decreed_num_features)
-                decreed_num_features_inactives[actives_x1] = False
-                decreed_num_features_inactives[actives_y2] = False
-                decreed_num_features_uniques = np.copy(
-                    decreed_num_features
-                    * np.logical_not(decreed_num_features_inactives)
-                )
-                decreed_num_features_uniques[list(actives_both)] = False
-                abs_delta[decreed_num_features_inactives] = 0
-                abs_delta[decreed_num_features_uniques] = 1
+            # Set distances for non-acting variables: 0 if both are non-acting, 1 if only one is non-acting
+            both_non_acting = num_is_decreed & ~(x_k1_acting | y_l2_acting)
+            abs_delta[both_non_acting] = 0.0
+
+            either_acting = num_is_decreed & (x_k1_acting != y_l2_acting)
+            abs_delta[either_acting] = 1.0
 
             D_num[indD] = abs_delta
             indD += 1
     return D_num
 
 
 def differences(X, Y):
@@ -1305,56 +1199,65 @@
     -------
 
     D_corr: np.ndarray [n_obs * (n_obs - 1) / 2, dim]
             - The componentwise cross-spatial-correlation-distance between the
               vectors in X.
 
     """
-    # Fit the matrix iteratively: avoid some memory troubles .
-    limit = int(1e4)
-
-    D_corr = np.zeros((D.shape[0], dim))
-    i, nb_limit = 0, int(limit)
-
-    if (power is None) and (not (corr == "act_exp")):
+    if power is None and corr != "act_exp":
         raise ValueError(
             "Missing power initialization to compute cross-spatial correlation distance"
         )
 
-    if return_derivative == False:
-        while True:
-            if i * nb_limit > D_corr.shape[0]:
-                return D_corr
-            else:
-                D_corr[i * nb_limit : (i + 1) * nb_limit, :] = D[
-                    i * nb_limit : (i + 1) * nb_limit, :
-                ]
-                if not (corr == "act_exp"):
-                    D_corr[i * nb_limit : (i + 1) * nb_limit, :] = (
-                        np.abs(D_corr[i * nb_limit : (i + 1) * nb_limit, :]) ** power
-                    )
-                i += 1
+    if not return_derivative:
+        if corr == "act_exp":
+            return _comp_dist_act_exp(D, dim)
+        return _comp_dist(D, dim, power)
     else:
         if theta is None:
             raise ValueError(
                 "Missing theta to compute spatial derivative of theta cross-spatial correlation distance"
             )
         if corr == "act_exp":
             raise ValueError("this option is not implemented for active learning")
-        else:
-            der = np.ones(D.shape)
-            for i, j in np.ndindex(D.shape):
-                der[i][j] = np.abs(D[i][j]) ** (power - 1)
-                if D[i][j] < 0:
-                    der[i][j] = -der[i][j]
+        der = _comp_dist_derivative(D, power)
+        D_corr = power * np.einsum("j,ij->ij", theta.T, der)
+        return D_corr
 
-            D_corr = power * np.einsum("j,ij->ij", theta.T, der)
-            return D_corr
 
-        i += 1
+@njit_use(parallel=True)
+def _comp_dist_act_exp(D, dim):
+    D_corr = np.zeros((D.shape[0], dim))
+    i, nb_limit = 0, 1000
+    for i in prange((D_corr.shape[0] // nb_limit) + 1):
+        D_corr[i * nb_limit : (i + 1) * nb_limit, :] = D[
+            i * nb_limit : (i + 1) * nb_limit, :
+        ]
+    return D_corr
+
+
+@njit_use()
+def _comp_dist(D, dim, power):
+    D_corr = np.zeros((D.shape[0], dim))
+    i, nb_limit = 0, 1000
+    for i in range((D_corr.shape[0] // nb_limit) + 1):
+        D_corr[i * nb_limit : (i + 1) * nb_limit, :] = (
+            np.abs(D[i * nb_limit : (i + 1) * nb_limit, :]) ** power
+        )
+    return D_corr
+
+
+@njit_use()
+def _comp_dist_derivative(D, power):
+    der = np.ones(D.shape)
+    for i, j in np.ndindex(D.shape):
+        der[i][j] = np.abs(D[i][j]) ** (power - 1)
+        if D[i][j] < 0:
+            der[i][j] = -der[i][j]
+    return der
 
 
 def componentwise_distance_PLS(
     D, corr, n_comp, coeff_pls, power=2.0, theta=None, return_derivative=False
 ):
     """
     Computes the nonzero componentwise cross-spatial-correlation-distance
@@ -1546,7 +1449,92 @@
     x = np.asarray(x, dtype=np.float64)
     n_eval, n_features = x.shape
     f = np.hstack([np.ones([n_eval, 1]), x])
     for k in range(n_features):
         f = np.hstack([f, x[:, k, np.newaxis] * x[:, k:]])
 
     return f
+
+
+@njit_use(parallel=True)
+def matrix_data_corr_levels_cat_matrix(
+    i, n_levels, theta_cat, theta_bounds, is_ehh: bool
+):
+    Theta_mat = np.zeros((n_levels[i], n_levels[i]))
+    L = np.zeros((n_levels[i], n_levels[i]))
+    v = 0
+    for j in range(n_levels[i]):
+        for k in range(n_levels[i] - j):
+            if j == k + j:
+                Theta_mat[j, k + j] = 1
+            else:
+                Theta_mat[j, k + j] = theta_cat[v]
+                Theta_mat[k + j, j] = theta_cat[v]
+                v = v + 1
+
+    for j in range(n_levels[i]):
+        for k in range(n_levels[i] - j):
+            if j == k + j:
+                if j == 0:
+                    L[j, k + j] = 1
+
+                else:
+                    L[j, k + j] = 1
+                    for l in range(j):
+                        L[j, k + j] = L[j, k + j] * np.sin(Theta_mat[j, l])
+
+            else:
+                if j == 0:
+                    L[k + j, j] = np.cos(Theta_mat[k, 0])
+                else:
+                    L[k + j, j] = np.cos(Theta_mat[k + j, j])
+                    for l in range(j):
+                        L[k + j, j] = L[k + j, j] * np.sin(Theta_mat[k + j, l])
+
+    T = np.dot(L, L.T)
+
+    if is_ehh:
+        T = (T - 1) * theta_bounds[1] / 2
+        T = np.exp(2 * T)
+    k = (1 + np.exp(-theta_bounds[1])) / np.exp(-theta_bounds[0])
+    T = (T + np.exp(-theta_bounds[1])) / (k)
+    return T
+
+
+@njit_use()
+def matrix_data_corr_levels_cat_mod(i, Lij, r_cat, T, has_cat_kernel):
+    for k in range(np.shape(Lij[i])[0]):
+        indi = int(Lij[i][k][0])
+        indj = int(Lij[i][k][1])
+
+        if indi == indj:
+            r_cat[k] = 1.0
+        else:
+            if has_cat_kernel:
+                r_cat[k] = T[indi, indj]
+
+
+@njit_use()
+def matrix_data_corr_levels_cat_mod_comps(
+    i, Lij, r_cat, n_levels, T, d_cat_i, has_cat_kernel
+):
+    for k in range(np.shape(Lij[i])[0]):
+        indi = int(Lij[i][k][0])
+        indj = int(Lij[i][k][1])
+
+        if indi == indj:
+            r_cat[k] = 1.0
+        else:
+            if has_cat_kernel:
+                Theta_i_red = np.zeros(int((n_levels[i] - 1) * n_levels[i] / 2))
+                indmatvec = 0
+                for j in range(n_levels[i]):
+                    for l in range(n_levels[i]):
+                        if l > j:
+                            Theta_i_red[indmatvec] = T[j, l]
+                            indmatvec += 1
+                kval_cat = 0
+                for indijk in range(len(Theta_i_red)):
+                    kval_cat += np.multiply(
+                        Theta_i_red[indijk], d_cat_i[k : k + 1][0][indijk]
+                    )
+                r_cat[k] = kval_cat
```

### Comparing `smt-2.0b2/smt/utils/line_search.py` & `smt-2.0b3/smt/utils/line_search.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/linear_solvers.py` & `smt-2.0b3/smt/utils/linear_solvers.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/misc.py` & `smt-2.0b3/smt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/neural_net/activation.py` & `smt-2.0b3/smt/utils/neural_net/activation.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/neural_net/bwd_prop.py` & `smt-2.0b3/smt/utils/neural_net/bwd_prop.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/neural_net/data.py` & `smt-2.0b3/smt/utils/neural_net/data.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/neural_net/fwd_prop.py` & `smt-2.0b3/smt/utils/neural_net/fwd_prop.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/neural_net/loss.py` & `smt-2.0b3/smt/utils/neural_net/loss.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/neural_net/metrics.py` & `smt-2.0b3/smt/utils/neural_net/metrics.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/neural_net/model.py` & `smt-2.0b3/smt/utils/neural_net/model.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/neural_net/optimizer.py` & `smt-2.0b3/smt/utils/neural_net/optimizer.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/options_dictionary.py` & `smt-2.0b3/smt/utils/options_dictionary.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/printer.py` & `smt-2.0b3/smt/utils/printer.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/silence.py` & `smt-2.0b3/smt/utils/silence.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt/utils/sm_test_case.py` & `smt-2.0b3/smt/utils/sm_test_case.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b2/smt.egg-info/PKG-INFO` & `smt-2.0b3/smt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smt
-Version: 2.0b2
+Version: 2.0b3
 Summary: The Surrogate Modeling Toolbox (SMT)
 Home-page: https://github.com/SMTorg/smt
 Download-URL: https://github.com/SMTorg/smt/releases
 Author: Mohamed Amine Bouhlel et al.
 Author-email: mbouhlel@umich.edu
 License: BSD-3
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
+Provides-Extra: numba
 License-File: LICENSE.txt
 
 
 The surrogate modeling toolbox (SMT) is a Python package that contains 
 a collection of surrogate modeling methods, sampling techniques, and 
 benchmarking functions. This package provides a library of surrogate 
 models that is simple to use and facilitates the implementation of additional methods.
```

### Comparing `smt-2.0b2/smt.egg-info/SOURCES.txt` & `smt-2.0b3/smt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 smt/applications/mfkplsk.py
 smt/applications/mixed_integer.py
 smt/applications/moe.py
 smt/applications/vfm.py
 smt/problems/__init__.py
 smt/problems/branin.py
 smt/problems/cantilever_beam.py
+smt/problems/hierarchical_goldstein.py
 smt/problems/lp_norm.py
 smt/problems/mixed_cantilever_beam.py
 smt/problems/ndim_cantilever_beam.py
 smt/problems/ndim_robot_arm.py
 smt/problems/ndim_rosenbrock.py
 smt/problems/ndim_step_function.py
 smt/problems/neural_network.py
@@ -88,20 +89,20 @@
 smt/surrogate_models/rmtb.py
 smt/surrogate_models/rmtc.py
 smt/surrogate_models/rmts.py
 smt/surrogate_models/surrogate_model.py
 smt/utils/__init__.py
 smt/utils/caching.py
 smt/utils/checks.py
+smt/utils/design_space.py
 smt/utils/krg_sampling.py
 smt/utils/kriging.py
 smt/utils/line_search.py
 smt/utils/linear_solvers.py
 smt/utils/misc.py
-smt/utils/mixed_integer.py
 smt/utils/options_dictionary.py
 smt/utils/printer.py
 smt/utils/silence.py
 smt/utils/sm_test_case.py
 smt/utils/neural_net/__init__.py
 smt/utils/neural_net/activation.py
 smt/utils/neural_net/bwd_prop.py
```

