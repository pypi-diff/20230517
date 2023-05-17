# Comparing `tmp/HuMobi-0.1.8.tar.gz` & `tmp/HuMobi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HuMobi-0.1.8.tar", last modified: Mon Jul  4 11:16:38 2022, max compression
+gzip compressed data, was "HuMobi-0.1.9.tar", last modified: Mon Jul  4 11:24:51 2022, max compression
```

## Comparing `HuMobi-0.1.8.tar` & `HuMobi-0.1.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.998345 HuMobi-0.1.8/
--rw-rw-rw-   0        0        0     1543 2022-04-13 10:31:39.000000 HuMobi-0.1.8/LICENSE
--rw-rw-rw-   0        0        0    40835 2022-07-04 11:16:37.999338 HuMobi-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    40301 2022-05-23 07:31:50.000000 HuMobi-0.1.8/README.md
--rw-rw-rw-   0        0        0       86 2022-04-13 10:31:39.000000 HuMobi-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      894 2022-07-04 11:16:38.000334 HuMobi-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-04-13 10:31:39.000000 HuMobi-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.945158 HuMobi-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.981013 HuMobi-0.1.8/src/HuMobi.egg-info/
--rw-rw-rw-   0        0        0    40835 2022-07-04 11:16:37.000000 HuMobi-0.1.8/src/HuMobi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1758 2022-07-04 11:16:37.000000 HuMobi-0.1.8/src/HuMobi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-04 11:16:37.000000 HuMobi-0.1.8/src/HuMobi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      177 2022-07-04 11:16:37.000000 HuMobi-0.1.8/src/HuMobi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-07-04 11:16:37.000000 HuMobi-0.1.8/src/HuMobi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.982015 HuMobi-0.1.8/src/humobi/
--rw-rw-rw-   0        0        0       41 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.983444 HuMobi-0.1.8/src/humobi/measures/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/measures/__init__.py
--rw-rw-rw-   0        0        0     2222 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/measures/collective.py
--rw-rw-rw-   0        0        0    24038 2022-07-04 10:32:28.000000 HuMobi-0.1.8/src/humobi/measures/individual.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.985444 HuMobi-0.1.8/src/humobi/misc/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/misc/__init__.py
--rw-rw-rw-   0        0        0     1117 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/misc/create_grid.py
--rw-rw-rw-   0        0        0     8955 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/misc/generators.py
--rw-rw-rw-   0        0        0    11754 2022-05-25 07:01:52.000000 HuMobi-0.1.8/src/humobi/misc/utils.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.985444 HuMobi-0.1.8/src/humobi/models/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.987438 HuMobi-0.1.8/src/humobi/models/agent_module/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/models/agent_module/__init__.py
--rw-rw-rw-   0        0        0     2382 2022-05-23 07:31:50.000000 HuMobi-0.1.8/src/humobi/models/agent_module/agent_class.py
--rw-rw-rw-   0        0        0      834 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/models/agent_module/generate_agents.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.988434 HuMobi-0.1.8/src/humobi/models/mobility_model/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/models/mobility_model/__init__.py
--rw-rw-rw-   0        0        0     1734 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/models/mobility_model/data_generating.py
--rw-rw-rw-   0        0        0     2932 2022-07-04 09:23:58.000000 HuMobi-0.1.8/src/humobi/models/mobility_model/data_sampling.py
--rw-rw-rw-   0        0        0     2716 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/models/mobility_model/who.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.989431 HuMobi-0.1.8/src/humobi/models/spatial_modules/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/models/spatial_modules/__init__.py
--rw-rw-rw-   0        0        0      445 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/models/spatial_modules/where.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.991424 HuMobi-0.1.8/src/humobi/models/spatial_tools/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/models/spatial_tools/__init__.py
--rw-rw-rw-   0        0        0     4749 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/models/spatial_tools/distributions.py
--rw-rw-rw-   0        0        0      407 2022-05-25 07:01:52.000000 HuMobi-0.1.8/src/humobi/models/spatial_tools/filtering.py
--rw-rw-rw-   0        0        0     4950 2022-05-30 14:46:45.000000 HuMobi-0.1.8/src/humobi/models/spatial_tools/generating.py
--rw-rw-rw-   0        0        0     1557 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/models/spatial_tools/misc.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.992421 HuMobi-0.1.8/src/humobi/models/temporal_tools/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/models/temporal_tools/__init__.py
--rw-rw-rw-   0        0        0     3726 2022-07-04 09:23:58.000000 HuMobi-0.1.8/src/humobi/models/temporal_tools/cluster_traj.py
--rw-rw-rw-   0        0        0      734 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/models/temporal_tools/when.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.993418 HuMobi-0.1.8/src/humobi/predictors/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/predictors/__init__.py
--rw-rw-rw-   0        0        0    10765 2022-06-28 11:10:31.000000 HuMobi-0.1.8/src/humobi/predictors/deep.py
--rw-rw-rw-   0        0        0     4371 2022-04-22 07:19:16.000000 HuMobi-0.1.8/src/humobi/predictors/markov.py
--rw-rw-rw-   0        0        0     2863 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/predictors/sparse.py
--rw-rw-rw-   0        0        0    16841 2022-07-04 11:11:07.000000 HuMobi-0.1.8/src/humobi/predictors/wrapper.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.996341 HuMobi-0.1.8/src/humobi/preprocessing/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     4671 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/preprocessing/filters.py
--rw-rw-rw-   0        0        0    11361 2022-07-04 10:14:49.000000 HuMobi-0.1.8/src/humobi/preprocessing/spatial_aggregation.py
--rw-rw-rw-   0        0        0     4203 2022-07-04 09:23:13.000000 HuMobi-0.1.8/src/humobi/preprocessing/temporal_aggregation.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.997345 HuMobi-0.1.8/src/humobi/structures/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/structures/__init__.py
--rw-rw-rw-   0        0        0     6833 2022-05-23 09:11:29.000000 HuMobi-0.1.8/src/humobi/structures/trajectory.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:16:37.998345 HuMobi-0.1.8/src/humobi/tools/
--rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/tools/__init__.py
--rw-rw-rw-   0        0        0     5026 2022-04-13 10:31:39.000000 HuMobi-0.1.8/src/humobi/tools/processing.py
--rw-rw-rw-   0        0        0     3905 2022-05-23 07:31:50.000000 HuMobi-0.1.8/src/humobi/tools/user_statistics.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.016799 HuMobi-0.1.9/
+-rw-rw-rw-   0        0        0     1543 2022-04-13 10:31:39.000000 HuMobi-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    40835 2022-07-04 11:24:51.017796 HuMobi-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    40301 2022-05-23 07:31:50.000000 HuMobi-0.1.9/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-13 10:31:39.000000 HuMobi-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      894 2022-07-04 11:24:51.018797 HuMobi-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0       71 2022-04-13 10:31:39.000000 HuMobi-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:50.972300 HuMobi-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.000296 HuMobi-0.1.9/src/HuMobi.egg-info/
+-rw-rw-rw-   0        0        0    40835 2022-07-04 11:24:50.000000 HuMobi-0.1.9/src/HuMobi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1758 2022-07-04 11:24:50.000000 HuMobi-0.1.9/src/HuMobi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-04 11:24:50.000000 HuMobi-0.1.9/src/HuMobi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      177 2022-07-04 11:24:50.000000 HuMobi-0.1.9/src/HuMobi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-07-04 11:24:50.000000 HuMobi-0.1.9/src/HuMobi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.001292 HuMobi-0.1.9/src/humobi/
+-rw-rw-rw-   0        0        0       41 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.002289 HuMobi-0.1.9/src/humobi/measures/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/measures/__init__.py
+-rw-rw-rw-   0        0        0     2222 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/measures/collective.py
+-rw-rw-rw-   0        0        0    24038 2022-07-04 10:32:28.000000 HuMobi-0.1.9/src/humobi/measures/individual.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.003286 HuMobi-0.1.9/src/humobi/misc/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/misc/__init__.py
+-rw-rw-rw-   0        0        0     1117 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/misc/create_grid.py
+-rw-rw-rw-   0        0        0     8955 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/misc/generators.py
+-rw-rw-rw-   0        0        0    11754 2022-05-25 07:01:52.000000 HuMobi-0.1.9/src/humobi/misc/utils.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.004282 HuMobi-0.1.9/src/humobi/models/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/models/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.005279 HuMobi-0.1.9/src/humobi/models/agent_module/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/models/agent_module/__init__.py
+-rw-rw-rw-   0        0        0     2382 2022-05-23 07:31:50.000000 HuMobi-0.1.9/src/humobi/models/agent_module/agent_class.py
+-rw-rw-rw-   0        0        0      834 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/models/agent_module/generate_agents.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.006276 HuMobi-0.1.9/src/humobi/models/mobility_model/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/models/mobility_model/__init__.py
+-rw-rw-rw-   0        0        0     1734 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/models/mobility_model/data_generating.py
+-rw-rw-rw-   0        0        0     2932 2022-07-04 09:23:58.000000 HuMobi-0.1.9/src/humobi/models/mobility_model/data_sampling.py
+-rw-rw-rw-   0        0        0     2716 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/models/mobility_model/who.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.008329 HuMobi-0.1.9/src/humobi/models/spatial_modules/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/models/spatial_modules/__init__.py
+-rw-rw-rw-   0        0        0      445 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/models/spatial_modules/where.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.009819 HuMobi-0.1.9/src/humobi/models/spatial_tools/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/models/spatial_tools/__init__.py
+-rw-rw-rw-   0        0        0     4749 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/models/spatial_tools/distributions.py
+-rw-rw-rw-   0        0        0      407 2022-05-25 07:01:52.000000 HuMobi-0.1.9/src/humobi/models/spatial_tools/filtering.py
+-rw-rw-rw-   0        0        0     4950 2022-05-30 14:46:45.000000 HuMobi-0.1.9/src/humobi/models/spatial_tools/generating.py
+-rw-rw-rw-   0        0        0     1557 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/models/spatial_tools/misc.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.010818 HuMobi-0.1.9/src/humobi/models/temporal_tools/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/models/temporal_tools/__init__.py
+-rw-rw-rw-   0        0        0     3726 2022-07-04 09:23:58.000000 HuMobi-0.1.9/src/humobi/models/temporal_tools/cluster_traj.py
+-rw-rw-rw-   0        0        0      734 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/models/temporal_tools/when.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.012812 HuMobi-0.1.9/src/humobi/predictors/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/predictors/__init__.py
+-rw-rw-rw-   0        0        0    10765 2022-06-28 11:10:31.000000 HuMobi-0.1.9/src/humobi/predictors/deep.py
+-rw-rw-rw-   0        0        0     4371 2022-04-22 07:19:16.000000 HuMobi-0.1.9/src/humobi/predictors/markov.py
+-rw-rw-rw-   0        0        0     2863 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/predictors/sparse.py
+-rw-rw-rw-   0        0        0    16841 2022-07-04 11:11:07.000000 HuMobi-0.1.9/src/humobi/predictors/wrapper.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.014805 HuMobi-0.1.9/src/humobi/preprocessing/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     4671 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/preprocessing/filters.py
+-rw-rw-rw-   0        0        0    11351 2022-07-04 11:24:13.000000 HuMobi-0.1.9/src/humobi/preprocessing/spatial_aggregation.py
+-rw-rw-rw-   0        0        0     4203 2022-07-04 09:23:13.000000 HuMobi-0.1.9/src/humobi/preprocessing/temporal_aggregation.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.015802 HuMobi-0.1.9/src/humobi/structures/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/structures/__init__.py
+-rw-rw-rw-   0        0        0     6833 2022-05-23 09:11:29.000000 HuMobi-0.1.9/src/humobi/structures/trajectory.py
+drwxrwxrwx   0        0        0        0 2022-07-04 11:24:51.016799 HuMobi-0.1.9/src/humobi/tools/
+-rw-rw-rw-   0        0        0        0 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/tools/__init__.py
+-rw-rw-rw-   0        0        0     5026 2022-04-13 10:31:39.000000 HuMobi-0.1.9/src/humobi/tools/processing.py
+-rw-rw-rw-   0        0        0     3905 2022-05-23 07:31:50.000000 HuMobi-0.1.9/src/humobi/tools/user_statistics.py
```

### Comparing `HuMobi-0.1.8/LICENSE` & `HuMobi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/PKG-INFO` & `HuMobi-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HuMobi
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library dedicated to human mobility data processing
 Home-page: https://github.com/SmolakK/HuMobi
 Author: Kamil Smolak
 Author-email: kamil.smolak@upwr.edu.pl
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/SmolakK/HuMobi/issues
 Platform: UNKNOWN
```

### Comparing `HuMobi-0.1.8/README.md` & `HuMobi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/setup.cfg` & `HuMobi-0.1.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2048 754d 6f62 690d 0a76 6572 7369   = HuMobi..versi
-00000020: 6f6e 203d 2030 2e31 2e38 0d0a 6175 7468  on = 0.1.8..auth
+00000020: 6f6e 203d 2030 2e31 2e39 0d0a 6175 7468  on = 0.1.9..auth
 00000030: 6f72 203d 204b 616d 696c 2053 6d6f 6c61  or = Kamil Smola
 00000040: 6b0d 0a61 7574 686f 725f 656d 6169 6c20  k..author_email 
 00000050: 3d20 6b61 6d69 6c2e 736d 6f6c 616b 4075  = kamil.smolak@u
 00000060: 7077 722e 6564 752e 706c 0d0a 6465 7363  pwr.edu.pl..desc
 00000070: 7269 7074 696f 6e20 3d20 4120 6c69 6272  ription = A libr
 00000080: 6172 7920 6465 6469 6361 7465 6420 746f  ary dedicated to
 00000090: 2068 756d 616e 206d 6f62 696c 6974 7920   human mobility
```

### Comparing `HuMobi-0.1.8/src/HuMobi.egg-info/PKG-INFO` & `HuMobi-0.1.9/src/HuMobi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HuMobi
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library dedicated to human mobility data processing
 Home-page: https://github.com/SmolakK/HuMobi
 Author: Kamil Smolak
 Author-email: kamil.smolak@upwr.edu.pl
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/SmolakK/HuMobi/issues
 Platform: UNKNOWN
```

### Comparing `HuMobi-0.1.8/src/HuMobi.egg-info/SOURCES.txt` & `HuMobi-0.1.9/src/HuMobi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/measures/collective.py` & `HuMobi-0.1.9/src/humobi/measures/collective.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/measures/individual.py` & `HuMobi-0.1.9/src/humobi/measures/individual.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/misc/create_grid.py` & `HuMobi-0.1.9/src/humobi/misc/create_grid.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/misc/generators.py` & `HuMobi-0.1.9/src/humobi/misc/generators.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/misc/utils.py` & `HuMobi-0.1.9/src/humobi/misc/utils.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/models/agent_module/agent_class.py` & `HuMobi-0.1.9/src/humobi/models/agent_module/agent_class.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/models/agent_module/generate_agents.py` & `HuMobi-0.1.9/src/humobi/models/agent_module/generate_agents.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/models/mobility_model/data_generating.py` & `HuMobi-0.1.9/src/humobi/models/mobility_model/data_generating.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/models/mobility_model/data_sampling.py` & `HuMobi-0.1.9/src/humobi/models/mobility_model/data_sampling.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/models/mobility_model/who.py` & `HuMobi-0.1.9/src/humobi/models/mobility_model/who.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/models/spatial_tools/distributions.py` & `HuMobi-0.1.9/src/humobi/models/spatial_tools/distributions.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/models/spatial_tools/generating.py` & `HuMobi-0.1.9/src/humobi/models/spatial_tools/generating.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/models/spatial_tools/misc.py` & `HuMobi-0.1.9/src/humobi/models/spatial_tools/misc.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/models/temporal_tools/cluster_traj.py` & `HuMobi-0.1.9/src/humobi/models/temporal_tools/cluster_traj.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/models/temporal_tools/when.py` & `HuMobi-0.1.9/src/humobi/models/temporal_tools/when.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/predictors/deep.py` & `HuMobi-0.1.9/src/humobi/predictors/deep.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/predictors/markov.py` & `HuMobi-0.1.9/src/humobi/predictors/markov.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/predictors/sparse.py` & `HuMobi-0.1.9/src/humobi/predictors/sparse.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/predictors/wrapper.py` & `HuMobi-0.1.9/src/humobi/predictors/wrapper.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/preprocessing/filters.py` & `HuMobi-0.1.9/src/humobi/preprocessing/filters.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/preprocessing/spatial_aggregation.py` & `HuMobi-0.1.9/src/humobi/preprocessing/spatial_aggregation.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,36 +129,36 @@
 		Returns:
 			A TrajectoriesFrame with aggregated geometry.
 		"""
 		trajectories_copy = trajectories_frame.copy()
 		if trajectories_copy.crs.is_geographic:
 			trajectories_copy.to_crs(dest_crs=3857)
 		if self._detect_range and self._detect_origin:
-			self._x_min = trajectories_frame['geometry'].x.min()
-			self._x_max = trajectories_frame['geometry'].x.max()
-			self._y_min = trajectories_frame['geometry'].y.min()
-			self._y_max = trajectories_frame['geometry'].y.max()
+			self._x_min = trajectories_copy['geometry'].x.min()
+			self._x_max = trajectories_copy['geometry'].x.max()
+			self._y_min = trajectories_copy['geometry'].y.min()
+			self._y_max = trajectories_copy['geometry'].y.max()
 		x_points = resolution_to_points(self.resolution, self.x_max, self.x_min)
 		y_points = resolution_to_points(self.resolution, self.y_max, self.y_min)
 		x = np.linspace(self.x_min, self.x_max, x_points)
 		y = np.linspace(self.y_min, self.y_max, y_points)
 		centroid_x = moving_average(x)
 		centroid_y = moving_average(y)
 		agg_dict = {}
 		if parallel:
 			with cf.ThreadPoolExecutor(max_workers=6) as executor:
-				indis = [indi for indi, val in trajectories_frame['geometry'].iteritems()]
-				vals = [val for indi, val in trajectories_frame['geometry'].iteritems()]
+				indis = [indi for indi, val in trajectories_copy['geometry'].iteritems()]
+				vals = [val for indi, val in trajectories_copy['geometry'].iteritems()]
 				results = list(tqdm(
 					executor.map(self._aggregate_multi, repeat(x), repeat(y), repeat(centroid_x), repeat(centroid_y),
-					             indis, vals), total=trajectories_frame.shape[0]))
+					             indis, vals), total=trajectories_copy.shape[0]))
 			for result in results:
 				agg_dict[result[0]] = result[1]
 		else:
-			for indi, val in tqdm(trajectories_frame['geometry'].iteritems(), total=trajectories_frame.shape[0]):
+			for indi, val in tqdm(trajectories_copy['geometry'].iteritems(), total=trajectories_copy.shape[0]):
 				if np.isnan(val.x):
 					agg_dict[indi] = Point(float('nan'), float('nan'))
 					continue
 				assigned_x, assigned_y = self._aggregate(x, y, centroid_x, centroid_y, val)
 				agg_dict[indi] = Point(assigned_x, assigned_y)
 		if inplace:
 			trajectories_copy['geometry'].update(pd.Series(agg_dict))
@@ -239,15 +239,15 @@
 			A spatially aggregated TrajectoriesFrame
 		"""
 		if not hasattr(trajectories_frame, '_geom_cols'):
 			trajectories_frame = TrajectoriesFrame(trajectories_frame)
 		trajectories_copy = trajectories_frame.copy()
 		if trajectories_copy.crs.is_geographic:
 			trajectories_copy.to_crs(dest_crs=3857)
-		coordinates_frame = trajectories_frame[[trajectories_copy._geom_cols[0], trajectories_copy._geom_cols[1]]]
+		coordinates_frame = trajectories_copy[[trajectories_copy._geom_cols[0], trajectories_copy._geom_cols[1]]]
 		clustered = coordinates_frame.groupby(level=0).progress_apply(lambda x: self._user_aggregate(x))
 		if drop_noise:
 			clustered[clustered['labels'] == -1] = None
 			if len(clustered) == 0:
 				return None
 		if centres_as_geometry:
 			clustered = clustered.groupby(level=0).progress_apply(lambda x: self._recalcuate_centres(x))
```

### Comparing `HuMobi-0.1.8/src/humobi/preprocessing/temporal_aggregation.py` & `HuMobi-0.1.9/src/humobi/preprocessing/temporal_aggregation.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/structures/trajectory.py` & `HuMobi-0.1.9/src/humobi/structures/trajectory.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/tools/processing.py` & `HuMobi-0.1.9/src/humobi/tools/processing.py`

 * *Files identical despite different names*

### Comparing `HuMobi-0.1.8/src/humobi/tools/user_statistics.py` & `HuMobi-0.1.9/src/humobi/tools/user_statistics.py`

 * *Files identical despite different names*

