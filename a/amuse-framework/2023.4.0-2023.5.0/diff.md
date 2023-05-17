# Comparing `tmp/amuse-framework-2023.4.0.tar.gz` & `tmp/amuse-framework-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-framework-2023.4.0.tar", last modified: Tue Apr  4 14:21:05 2023, max compression
+gzip compressed data, was "amuse-framework-2023.5.0.tar", last modified: Wed May 17 10:18:42 2023, max compression
```

## Comparing `amuse-framework-2023.4.0.tar` & `amuse-framework-2023.5.0.tar`

### file list

```diff
@@ -1,289 +1,289 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.518945 amuse-framework-2023.4.0/
--rw-r--r--   0 rieder     (501) staff       (20)      639 2021-12-07 10:22:56.000000 amuse-framework-2023.4.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     2471 2022-11-30 13:58:14.000000 amuse-framework-2023.4.0/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)     1242 2023-04-04 14:21:05.518624 amuse-framework-2023.4.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)      101 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.429623 amuse-framework-2023.4.0/bin/
--rwxr-xr-x   0 rieder     (501) staff       (20)      328 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/bin/amuse-tutorial
--rw-r--r--   0 rieder     (501) staff       (20)      728 2020-03-24 14:36:20.000000 amuse-framework-2023.4.0/bin/amusifier.in
--rw-r--r--   0 rieder     (501) staff       (20)    49446 2021-12-07 10:22:56.000000 amuse-framework-2023.4.0/config.guess
--rw-r--r--   0 rieder     (501) staff       (20)     2814 2021-12-07 10:22:56.000000 amuse-framework-2023.4.0/config.mk.in
--rw-r--r--   0 rieder     (501) staff       (20)    34424 2021-12-07 10:22:56.000000 amuse-framework-2023.4.0/config.sub
--rwxr-xr-x   0 rieder     (501) staff       (20)   412359 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/configure
--rwxr-xr-x   0 rieder     (501) staff       (20)    15358 2021-12-07 10:22:56.000000 amuse-framework-2023.4.0/install-sh
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.416648 amuse-framework-2023.4.0/lib/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.430719 amuse-framework-2023.4.0/lib/amuse_mpi/
--rw-r--r--   0 rieder     (501) staff       (20)      499 2022-11-30 13:58:14.000000 amuse-framework-2023.4.0/lib/amuse_mpi/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)      335 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/amuse_mpi/amuse_mpi.c
--rw-r--r--   0 rieder     (501) staff       (20)      212 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/amuse_mpi/amuse_mpi.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.431588 amuse-framework-2023.4.0/lib/forsockets/
--rw-r--r--   0 rieder     (501) staff       (20)      494 2022-11-30 13:58:14.000000 amuse-framework-2023.4.0/lib/forsockets/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     5068 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/forsockets/forsockets.c
--rw-r--r--   0 rieder     (501) staff       (20)      853 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/forsockets/forsockets.h
--rw-r--r--   0 rieder     (501) staff       (20)     4782 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/forsockets/forsocketsf.f90
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.432838 amuse-framework-2023.4.0/lib/g6/
--rw-r--r--   0 rieder     (501) staff       (20)      242 2022-11-30 13:58:14.000000 amuse-framework-2023.4.0/lib/g6/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)    12542 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/g6/g6lib.c
--rw-r--r--   0 rieder     (501) staff       (20)     3957 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/g6/g6lib.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.433525 amuse-framework-2023.4.0/lib/sapporo_2/
--rw-r--r--   0 rieder     (501) staff       (20)     1469 2022-11-30 13:58:14.000000 amuse-framework-2023.4.0/lib/sapporo_2/Makefile
--rwxr-xr-x   0 rieder     (501) staff       (20)     2548 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/lib/sapporo_2/download.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.436910 amuse-framework-2023.4.0/lib/sapporo_light/
--rw-r--r--   0 rieder     (501) staff       (20)     1339 2022-11-30 13:58:14.000000 amuse-framework-2023.4.0/lib/sapporo_light/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)      641 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/README
--rw-r--r--   0 rieder     (501) staff       (20)    11568 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/dev_evaluate_gravity.cu
--rw-r--r--   0 rieder     (501) staff       (20)    12542 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/g6lib.c
--rw-r--r--   0 rieder     (501) staff       (20)     1461 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/g6lib.h
--rw-r--r--   0 rieder     (501) staff       (20)     5486 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/host_evaluate_gravity.cu
--rw-r--r--   0 rieder     (501) staff       (20)     7585 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/sapporo.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     4632 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/sapporo.h
--rw-r--r--   0 rieder     (501) staff       (20)     2434 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/sapporoG6lib.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2964 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/sapporo_defs.h
--rw-r--r--   0 rieder     (501) staff       (20)      530 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/sapporo_multi.h
--rw-r--r--   0 rieder     (501) staff       (20)     5983 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/sapporo_light/send_fetch_data.cpp
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.437991 amuse-framework-2023.4.0/lib/simple_hash/
--rw-r--r--   0 rieder     (501) staff       (20)      619 2022-11-30 13:58:14.000000 amuse-framework-2023.4.0/lib/simple_hash/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     8876 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/simple_hash/simple_hash.c
--rw-r--r--   0 rieder     (501) staff       (20)     1112 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/simple_hash/simple_hash.h
--rw-r--r--   0 rieder     (501) staff       (20)     1906 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/simple_hash/test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3620 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/lib/simple_hash/test.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.439437 amuse-framework-2023.4.0/lib/stopcond/
--rw-r--r--   0 rieder     (501) staff       (20)      688 2022-11-30 13:58:14.000000 amuse-framework-2023.4.0/lib/stopcond/Makefile
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.439696 amuse-framework-2023.4.0/lib/stopcond/mpi/
--rw-r--r--   0 rieder     (501) staff       (20)      243 2022-11-30 13:58:14.000000 amuse-framework-2023.4.0/lib/stopcond/mpi/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)    18126 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/stopcond/stopcond.c
--rw-r--r--   0 rieder     (501) staff       (20)     3591 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/stopcond/stopcond.h
--rw-r--r--   0 rieder     (501) staff       (20)     1642 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/stopcond/stopcond.inc
--rw-r--r--   0 rieder     (501) staff       (20)    21963 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/stopcond/stopcondf.F90
--rw-r--r--   0 rieder     (501) staff       (20)     9654 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/lib/stopcond/stopcondf_isoc.F90
--rw-r--r--   0 rieder     (501) staff       (20)      140 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-04-04 14:21:05.519048 amuse-framework-2023.4.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     2060 2022-11-30 13:58:14.000000 amuse-framework-2023.4.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.422469 amuse-framework-2023.4.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.440851 amuse-framework-2023.4.0/src/amuse/
--rw-r--r--   0 rieder     (501) staff       (20)     1903 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/src/amuse/amuserc
--rw-r--r--   0 rieder     (501) staff       (20)      915 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/codes.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.440988 amuse-framework-2023.4.0/src/amuse/community/
--rw-r--r--   0 rieder     (501) staff       (20)     1277 2020-03-24 14:36:23.000000 amuse-framework-2023.4.0/src/amuse/community/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.444691 amuse-framework-2023.4.0/src/amuse/community/interface/
--rw-r--r--   0 rieder     (501) staff       (20)        1 2020-03-24 14:36:25.000000 amuse-framework-2023.4.0/src/amuse/community/interface/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     3894 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/community/interface/common.py
--rw-r--r--   0 rieder     (501) staff       (20)     3439 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/community/interface/example.py
--rw-r--r--   0 rieder     (501) staff       (20)    52603 2022-10-10 09:16:43.000000 amuse-framework-2023.4.0/src/amuse/community/interface/gd.py
--rw-r--r--   0 rieder     (501) staff       (20)    12910 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/community/interface/hydro.py
--rw-r--r--   0 rieder     (501) staff       (20)     1756 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/community/interface/mhd.py
--rw-r--r--   0 rieder     (501) staff       (20)    54169 2022-03-09 15:01:56.000000 amuse-framework-2023.4.0/src/amuse/community/interface/se.py
--rw-r--r--   0 rieder     (501) staff       (20)    28066 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/community/interface/stopping_conditions.py
--rw-r--r--   0 rieder     (501) staff       (20)     2968 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/config.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.448284 amuse-framework-2023.4.0/src/amuse/couple/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/couple/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    24220 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/couple/bridge.py
--rw-r--r--   0 rieder     (501) staff       (20)     5584 2023-02-13 15:26:10.000000 amuse-framework-2023.4.0/src/amuse/couple/collision_handler.py
--rw-r--r--   0 rieder     (501) staff       (20)    95615 2021-07-05 11:19:28.000000 amuse-framework-2023.4.0/src/amuse/couple/encounters.py
--rw-r--r--   0 rieder     (501) staff       (20)    11720 2021-04-22 16:00:02.000000 amuse-framework-2023.4.0/src/amuse/couple/fallback_stellar_evolution.py
--rw-r--r--   0 rieder     (501) staff       (20)   122275 2021-07-05 11:19:28.000000 amuse-framework-2023.4.0/src/amuse/couple/multiples.py
--rw-r--r--   0 rieder     (501) staff       (20)     6255 2021-04-22 16:00:02.000000 amuse-framework-2023.4.0/src/amuse/couple/parallel_stellar_evolution.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.450037 amuse-framework-2023.4.0/src/amuse/data/
--rw-r--r--   0 rieder     (501) staff       (20)    60725 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/data/AMUSE.bib
--rw-r--r--   0 rieder     (501) staff       (20)       27 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/data/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.459201 amuse-framework-2023.4.0/src/amuse/datamodel/
--rw-r--r--   0 rieder     (501) staff       (20)      388 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     3473 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/attributes.py
--rw-r--r--   0 rieder     (501) staff       (20)    64925 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/datamodel/base.py
--rw-r--r--   0 rieder     (501) staff       (20)        1 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/binding.py
--rw-r--r--   0 rieder     (501) staff       (20)       42 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/code_particles.py
--rw-r--r--   0 rieder     (501) staff       (20)      150 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/console.py
--rw-r--r--   0 rieder     (501) staff       (20)     7549 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/datamodel/grid_attributes.py
--rw-r--r--   0 rieder     (501) staff       (20)    42559 2022-10-10 09:16:43.000000 amuse-framework-2023.4.0/src/amuse/datamodel/grids.py
--rw-r--r--   0 rieder     (501) staff       (20)    50773 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/incode_storage.py
--rw-r--r--   0 rieder     (501) staff       (20)    13000 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/datamodel/indexing.py
--rw-r--r--   0 rieder     (501) staff       (20)    26559 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/datamodel/memory_storage.py
--rw-r--r--   0 rieder     (501) staff       (20)    26325 2023-02-28 13:02:04.000000 amuse-framework-2023.4.0/src/amuse/datamodel/parameters.py
--rw-r--r--   0 rieder     (501) staff       (20)    47337 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/datamodel/particle_attributes.py
--rw-r--r--   0 rieder     (501) staff       (20)   155010 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/datamodel/particles.py
--rw-r--r--   0 rieder     (501) staff       (20)     1551 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/rotation.py
--rw-r--r--   0 rieder     (501) staff       (20)       74 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/set.py
--rw-r--r--   0 rieder     (501) staff       (20)     3904 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/simple_hash.py
--rw-r--r--   0 rieder     (501) staff       (20)    10234 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/datamodel/staggeredgrid.py
--rw-r--r--   0 rieder     (501) staff       (20)    14471 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/trees.py
--rw-r--r--   0 rieder     (501) staff       (20)      188 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/datamodel/values.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.474144 amuse-framework-2023.4.0/src/amuse/ext/
--rw-r--r--   0 rieder     (501) staff       (20)     1290 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/ClusterCore.py
--rw-r--r--   0 rieder     (501) staff       (20)     2524 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/LagrangianRadii.py
--rw-r--r--   0 rieder     (501) staff       (20)     1689 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/SConstruct
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     6021 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/basicgraph.py
--rw-r--r--   0 rieder     (501) staff       (20)    69458 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/bbr_color.txt
--rw-r--r--   0 rieder     (501) staff       (20)     4018 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/bhtc_interface.pyx
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.474466 amuse-framework-2023.4.0/src/amuse/ext/blender/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/blender/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      771 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/blender/blender.py
--rw-r--r--   0 rieder     (501) staff       (20)     3386 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/boss_bodenheimer.py
--rw-r--r--   0 rieder     (501) staff       (20)    11167 2021-07-10 08:50:20.000000 amuse-framework-2023.4.0/src/amuse/ext/bridge.py
--rw-r--r--   0 rieder     (501) staff       (20)     5473 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)     7430 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/composition_methods.py
--rw-r--r--   0 rieder     (501) staff       (20)     1932 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/comsystem.py
--rw-r--r--   0 rieder     (501) staff       (20)     6851 2021-07-05 11:19:28.000000 amuse-framework-2023.4.0/src/amuse/ext/concurrent.py
--rw-r--r--   0 rieder     (501) staff       (20)     5397 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/cosmo.py
--rw-r--r--   0 rieder     (501) staff       (20)     2340 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/derived_grav_systems.py
--rw-r--r--   0 rieder     (501) staff       (20)     9939 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/evrard_test.py
--rw-r--r--   0 rieder     (501) staff       (20)     9832 2021-07-05 11:19:28.000000 amuse-framework-2023.4.0/src/amuse/ext/galactic_potentials.py
--rw-r--r--   0 rieder     (501) staff       (20)     3541 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/galactics_model.py
--rw-r--r--   0 rieder     (501) staff       (20)     2446 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/gasplummer.py
--rw-r--r--   0 rieder     (501) staff       (20)    12018 2022-10-10 09:16:43.000000 amuse-framework-2023.4.0/src/amuse/ext/grid_remappers.py
--rw-r--r--   0 rieder     (501) staff       (20)     5851 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ext/grid_to_sph.py
--rw-r--r--   0 rieder     (501) staff       (20)     2247 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/halogen_model.py
--rw-r--r--   0 rieder     (501) staff       (20)    22588 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/hydro_collision.py
--rw-r--r--   0 rieder     (501) staff       (20)    12419 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/job_server.py
--rw-r--r--   0 rieder     (501) staff       (20)       33 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/kingmodel.py
--rw-r--r--   0 rieder     (501) staff       (20)    10428 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/molecular_cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)    23761 2021-12-07 10:22:56.000000 amuse-framework-2023.4.0/src/amuse/ext/orbital_elements.py
--rw-r--r--   0 rieder     (501) staff       (20)     6567 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/particles_with_color.py
--rw-r--r--   0 rieder     (501) staff       (20)     2982 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/plotting_hydro.py
--rw-r--r--   0 rieder     (501) staff       (20)      134 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/plummer.py
--rw-r--r--   0 rieder     (501) staff       (20)     1271 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/plummer_helper.pyx
--rw-r--r--   0 rieder     (501) staff       (20)     1917 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/polarsupport.py
--rw-r--r--   0 rieder     (501) staff       (20)     5030 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/protodisk.py
--rw-r--r--   0 rieder     (501) staff       (20)     1981 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/radial_profile.py
--rw-r--r--   0 rieder     (501) staff       (20)     4067 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/relax_sph.py
--rw-r--r--   0 rieder     (501) staff       (20)    10547 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/roche_radius.py
--rw-r--r--   0 rieder     (501) staff       (20)     6928 2021-07-10 08:50:20.000000 amuse-framework-2023.4.0/src/amuse/ext/rotating_bridge.py
--rw-r--r--   0 rieder     (501) staff       (20)      137 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/salpeter.py
--rw-r--r--   0 rieder     (501) staff       (20)    12155 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ext/sink.py
--rw-r--r--   0 rieder     (501) staff       (20)    11837 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/sobol.py
--rw-r--r--   0 rieder     (501) staff       (20)    12891 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ext/solarsystem.py
--rw-r--r--   0 rieder     (501) staff       (20)     2200 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/speed.py
--rw-r--r--   0 rieder     (501) staff       (20)     3482 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/sph_to_grid.py
--rw-r--r--   0 rieder     (501) staff       (20)     3314 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/sph_to_star.py
--rw-r--r--   0 rieder     (501) staff       (20)    20811 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/spherical_model.py
--rw-r--r--   0 rieder     (501) staff       (20)    19994 2022-10-10 09:16:43.000000 amuse-framework-2023.4.0/src/amuse/ext/star_to_sph.py
--rw-r--r--   0 rieder     (501) staff       (20)     8764 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/static_potentials.py
--rw-r--r--   0 rieder     (501) staff       (20)     2688 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/stellar_gyration_radius.py
--rw-r--r--   0 rieder     (501) staff       (20)    18470 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/stellar_tidal_evolution.py
--rw-r--r--   0 rieder     (501) staff       (20)    41820 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/ext/stellar_wind.py
--rw-r--r--   0 rieder     (501) staff       (20)     1386 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ext/sticky_spheres.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.480372 amuse-framework-2023.4.0/src/amuse/ic/
--rw-r--r--   0 rieder     (501) staff       (20)     1229 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ic/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.481032 amuse-framework-2023.4.0/src/amuse/ic/_limepy/
--rwxr-xr-x   0 rieder     (501) staff       (20)      204 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ic/_limepy/__init__.py
--rwxr-xr-x   0 rieder     (501) staff       (20)    43751 2021-07-05 11:19:28.000000 amuse-framework-2023.4.0/src/amuse/ic/_limepy/limepy.py
--rwxr-xr-x   0 rieder     (501) staff       (20)    10121 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ic/_limepy/sample.py
--rw-r--r--   0 rieder     (501) staff       (20)     9096 2021-07-22 13:07:56.000000 amuse-framework-2023.4.0/src/amuse/ic/brokenimf.py
--rw-r--r--   0 rieder     (501) staff       (20)     2352 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ic/flatimf.py
--rw-r--r--   0 rieder     (501) staff       (20)      151 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ic/fractalcluster.py
--rw-r--r--   0 rieder     (501) staff       (20)     3678 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ic/gasplummer.py
--rw-r--r--   0 rieder     (501) staff       (20)     7649 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ic/isotropic_cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)    20594 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ic/kingmodel.py
--rw-r--r--   0 rieder     (501) staff       (20)      267 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ic/kroupa.py
--rw-r--r--   0 rieder     (501) staff       (20)     1724 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ic/limepy.py
--rw-r--r--   0 rieder     (501) staff       (20)    13570 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ic/make_planets_oligarch.py
--rw-r--r--   0 rieder     (501) staff       (20)       56 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ic/mameclot.py
--rw-r--r--   0 rieder     (501) staff       (20)      295 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ic/millerscalo.py
--rw-r--r--   0 rieder     (501) staff       (20)      468 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ic/molecular_cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)     6918 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ic/plummer.py
--rw-r--r--   0 rieder     (501) staff       (20)     2981 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ic/salpeter.py
--rw-r--r--   0 rieder     (501) staff       (20)      263 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/ic/scalo.py
--rw-r--r--   0 rieder     (501) staff       (20)    21531 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ic/solar_system_moons.py
--rw-r--r--   0 rieder     (501) staff       (20)      165 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/ic/solarsystem.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.486832 amuse-framework-2023.4.0/src/amuse/io/
--rw-r--r--   0 rieder     (501) staff       (20)     1001 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/io/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    17890 2021-04-21 10:40:53.000000 amuse-framework-2023.4.0/src/amuse/io/base.py
--rw-r--r--   0 rieder     (501) staff       (20)     6347 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/io/fi_io.py
--rw-r--r--   0 rieder     (501) staff       (20)    16756 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/io/gadget.py
--rw-r--r--   0 rieder     (501) staff       (20)     2608 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/io/horizons.py
--rw-r--r--   0 rieder     (501) staff       (20)    12272 2021-07-05 11:19:28.000000 amuse-framework-2023.4.0/src/amuse/io/nemobin.py
--rw-r--r--   0 rieder     (501) staff       (20)     5389 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/io/nemotsf.py
--rw-r--r--   0 rieder     (501) staff       (20)     1027 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/io/p10.txt
--rw-r--r--   0 rieder     (501) staff       (20)     4241 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/io/phigrape.py
--rw-r--r--   0 rieder     (501) staff       (20)    17938 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/io/starlab.py
--rw-r--r--   0 rieder     (501) staff       (20)     6419 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/io/store.py
--rw-r--r--   0 rieder     (501) staff       (20)    32086 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/io/store_v1.py
--rw-r--r--   0 rieder     (501) staff       (20)    45888 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/io/store_v2.py
--rw-r--r--   0 rieder     (501) staff       (20)    22593 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/io/text.py
--rw-r--r--   0 rieder     (501) staff       (20)    14998 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/io/vtk.py
--rw-r--r--   0 rieder     (501) staff       (20)     4808 2021-07-05 12:48:23.000000 amuse-framework-2023.4.0/src/amuse/lab.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.488165 amuse-framework-2023.4.0/src/amuse/plot/
--rw-r--r--   0 rieder     (501) staff       (20)       21 2021-07-10 08:50:20.000000 amuse-framework-2023.4.0/src/amuse/plot/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    22278 2021-07-10 08:50:20.000000 amuse-framework-2023.4.0/src/amuse/plot/_plot.py
--rwxr-xr-x   0 rieder     (501) staff       (20)    13863 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/plot/hydro.py
--rw-r--r--   0 rieder     (501) staff       (20)    12634 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/plot/mapper.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.492694 amuse-framework-2023.4.0/src/amuse/rfi/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/rfi/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    23061 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/rfi/async_request.py
--rw-r--r--   0 rieder     (501) staff       (20)    88683 2022-10-10 09:16:43.000000 amuse-framework-2023.4.0/src/amuse/rfi/channel.py
--rw-r--r--   0 rieder     (501) staff       (20)    52496 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/rfi/core.py
--rwxr-xr-x   0 rieder     (501) staff       (20)    15246 2021-07-05 11:19:28.000000 amuse-framework-2023.4.0/src/amuse/rfi/gencode.py
--rw-r--r--   0 rieder     (501) staff       (20)     4329 2021-04-22 16:00:02.000000 amuse-framework-2023.4.0/src/amuse/rfi/import_module.py
--rw-r--r--   0 rieder     (501) staff       (20)     5500 2021-04-22 16:00:02.000000 amuse-framework-2023.4.0/src/amuse/rfi/nospawn.py
--rw-r--r--   0 rieder     (501) staff       (20)    23380 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/rfi/python_code.py
--rw-r--r--   0 rieder     (501) staff       (20)     1197 2021-04-22 16:00:02.000000 amuse-framework-2023.4.0/src/amuse/rfi/run_command_redirected.py
--rw-r--r--   0 rieder     (501) staff       (20)     2138 2021-04-22 16:00:02.000000 amuse-framework-2023.4.0/src/amuse/rfi/slurm.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.498783 amuse-framework-2023.4.0/src/amuse/rfi/tools/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    45482 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/create_c.py
--rw-r--r--   0 rieder     (501) staff       (20)     4264 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/create_code.py
--rw-r--r--   0 rieder     (501) staff       (20)    10659 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/create_definition.py
--rw-r--r--   0 rieder     (501) staff       (20)    15062 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/create_dir.py
--rw-r--r--   0 rieder     (501) staff       (20)    64699 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/create_fortran.py
--rw-r--r--   0 rieder     (501) staff       (20)    53344 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/create_java.py
--rw-r--r--   0 rieder     (501) staff       (20)     2216 2021-04-22 16:00:02.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/create_python_worker.py
--rw-r--r--   0 rieder     (501) staff       (20)      991 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/cython_code_script.template
--rw-r--r--   0 rieder     (501) staff       (20)    11322 2021-07-05 11:19:28.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/fortran_tools.py
--rw-r--r--   0 rieder     (501) staff       (20)      980 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/java_code_script.template
--rw-r--r--   0 rieder     (501) staff       (20)     1102 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/rfi/tools/python_code_script.template
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.505046 amuse-framework-2023.4.0/src/amuse/support/
--rw-r--r--   0 rieder     (501) staff       (20)      569 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     5372 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/support/code.py
--rw-r--r--   0 rieder     (501) staff       (20)    11337 2023-02-22 12:53:22.000000 amuse-framework-2023.4.0/src/amuse/support/console.py
--rw-r--r--   0 rieder     (501) staff       (20)    15197 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/support/core.py
--rw-r--r--   0 rieder     (501) staff       (20)     2073 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/support/exceptions.py
--rw-r--r--   0 rieder     (501) staff       (20)    61635 2022-10-03 08:52:42.000000 amuse-framework-2023.4.0/src/amuse/support/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)    11438 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/support/literature.py
--rw-r--r--   0 rieder     (501) staff       (20)     8981 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/support/methods.py
--rw-r--r--   0 rieder     (501) staff       (20)    10236 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/support/options.py
--rw-r--r--   0 rieder     (501) staff       (20)    11751 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/support/parameter_tools.py
--rw-r--r--   0 rieder     (501) staff       (20)     1183 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/support/project.py
--rw-r--r--   0 rieder     (501) staff       (20)    19392 2021-04-12 16:14:01.000000 amuse-framework-2023.4.0/src/amuse/support/state.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.505664 amuse-framework-2023.4.0/src/amuse/support/thirdparty/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/support/thirdparty/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    18956 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/support/thirdparty/texttable.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.506942 amuse-framework-2023.4.0/src/amuse/test/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/test/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    12935 2021-04-22 16:00:02.000000 amuse-framework-2023.4.0/src/amuse/test/amusetest.py
--rw-r--r--   0 rieder     (501) staff       (20)    14500 2021-04-22 16:00:02.000000 amuse-framework-2023.4.0/src/amuse/test/compile_tools.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.515331 amuse-framework-2023.4.0/src/amuse/units/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/units/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    18324 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/units/constants.py
--rw-r--r--   0 rieder     (501) staff       (20)    33642 2021-12-07 10:22:56.000000 amuse-framework-2023.4.0/src/amuse/units/core.py
--rw-r--r--   0 rieder     (501) staff       (20)      731 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/units/derivedsi.py
--rw-r--r--   0 rieder     (501) staff       (20)    11358 2023-02-13 15:26:23.000000 amuse-framework-2023.4.0/src/amuse/units/generic_unit_converter.py
--rw-r--r--   0 rieder     (501) staff       (20)     2792 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/src/amuse/units/generic_unit_system.py
--rw-r--r--   0 rieder     (501) staff       (20)     4912 2021-12-07 10:22:56.000000 amuse-framework-2023.4.0/src/amuse/units/nbody_system.py
--rw-r--r--   0 rieder     (501) staff       (20)     7342 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/units/nist.py
--rw-r--r--   0 rieder     (501) staff       (20)    33920 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/units/nist.txt
--rw-r--r--   0 rieder     (501) staff       (20)    38873 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/units/nist2010.txt
--rw-r--r--   0 rieder     (501) staff       (20)     4718 2021-07-05 11:19:28.000000 amuse-framework-2023.4.0/src/amuse/units/optparse.py
--rw-r--r--   0 rieder     (501) staff       (20)    44745 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/units/quantities.py
--rw-r--r--   0 rieder     (501) staff       (20)     1853 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/units/scaling_converter.py
--rw-r--r--   0 rieder     (501) staff       (20)     2349 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/units/si.py
--rw-r--r--   0 rieder     (501) staff       (20)      190 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/units/translator.txt
--rw-r--r--   0 rieder     (501) staff       (20)      780 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/src/amuse/units/trigo.py
--rw-r--r--   0 rieder     (501) staff       (20)     4019 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/src/amuse/units/units.py
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-04-04 14:21:02.000000 amuse-framework-2023.4.0/src/amuse/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.516238 amuse-framework-2023.4.0/src/amuse_framework.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1242 2023-04-04 14:21:02.000000 amuse-framework-2023.4.0/src/amuse_framework.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     7390 2023-04-04 14:21:05.000000 amuse-framework-2023.4.0/src/amuse_framework.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-04-04 14:21:02.000000 amuse-framework-2023.4.0/src/amuse_framework.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)      130 2023-04-04 14:21:02.000000 amuse-framework-2023.4.0/src/amuse_framework.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-04-04 14:21:02.000000 amuse-framework-2023.4.0/src/amuse_framework.egg-info/top_level.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:21:05.518295 amuse-framework-2023.4.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2021-07-05 11:19:28.000000 amuse-framework-2023.4.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2022-11-30 13:58:15.000000 amuse-framework-2023.4.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2020-03-24 14:36:26.000000 amuse-framework-2023.4.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    50379 2023-04-04 13:47:06.000000 amuse-framework-2023.4.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2021-04-14 10:14:49.000000 amuse-framework-2023.4.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.386463 amuse-framework-2023.5.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      639 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     2471 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1242 2023-05-17 10:18:42.386313 amuse-framework-2023.5.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)      101 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.350414 amuse-framework-2023.5.0/bin/
+-rwxr-xr-x   0 rieder     (501) staff       (20)      328 2022-11-22 11:55:13.000000 amuse-framework-2023.5.0/bin/amuse-tutorial
+-rw-r--r--   0 rieder     (501) staff       (20)      728 2022-11-22 11:55:13.000000 amuse-framework-2023.5.0/bin/amusifier.in
+-rw-r--r--   0 rieder     (501) staff       (20)    49446 2023-02-28 13:39:09.000000 amuse-framework-2023.5.0/config.guess
+-rw-r--r--   0 rieder     (501) staff       (20)     2814 2022-11-22 11:55:13.000000 amuse-framework-2023.5.0/config.mk.in
+-rw-r--r--   0 rieder     (501) staff       (20)    34424 2023-02-28 13:39:09.000000 amuse-framework-2023.5.0/config.sub
+-rwxr-xr-x   0 rieder     (501) staff       (20)   412359 2023-03-22 19:10:26.000000 amuse-framework-2023.5.0/configure
+-rwxr-xr-x   0 rieder     (501) staff       (20)    15358 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/install-sh
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.346798 amuse-framework-2023.5.0/lib/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.350821 amuse-framework-2023.5.0/lib/amuse_mpi/
+-rw-r--r--   0 rieder     (501) staff       (20)      499 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/amuse_mpi/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)      335 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/amuse_mpi/amuse_mpi.c
+-rw-r--r--   0 rieder     (501) staff       (20)      212 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/amuse_mpi/amuse_mpi.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.351340 amuse-framework-2023.5.0/lib/forsockets/
+-rw-r--r--   0 rieder     (501) staff       (20)      494 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/forsockets/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     5068 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/forsockets/forsockets.c
+-rw-r--r--   0 rieder     (501) staff       (20)      853 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/forsockets/forsockets.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4782 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/forsockets/forsocketsf.f90
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.351741 amuse-framework-2023.5.0/lib/g6/
+-rw-r--r--   0 rieder     (501) staff       (20)      242 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/g6/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)    12542 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/g6/g6lib.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3957 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/g6/g6lib.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.351991 amuse-framework-2023.5.0/lib/sapporo_2/
+-rw-r--r--   0 rieder     (501) staff       (20)     1469 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/sapporo_2/Makefile
+-rwxr-xr-x   0 rieder     (501) staff       (20)     2548 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_2/download.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.353711 amuse-framework-2023.5.0/lib/sapporo_light/
+-rw-r--r--   0 rieder     (501) staff       (20)     1339 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/sapporo_light/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)      641 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/README
+-rw-r--r--   0 rieder     (501) staff       (20)    11568 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/dev_evaluate_gravity.cu
+-rw-r--r--   0 rieder     (501) staff       (20)    12542 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/g6lib.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1461 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/g6lib.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5486 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/host_evaluate_gravity.cu
+-rw-r--r--   0 rieder     (501) staff       (20)     7585 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/sapporo.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     4632 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/sapporo.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2434 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/sapporoG6lib.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2964 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/sapporo_defs.h
+-rw-r--r--   0 rieder     (501) staff       (20)      530 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/sapporo_multi.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5983 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/send_fetch_data.cpp
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.354526 amuse-framework-2023.5.0/lib/simple_hash/
+-rw-r--r--   0 rieder     (501) staff       (20)      619 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/simple_hash/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     8876 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/simple_hash/simple_hash.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1112 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/simple_hash/simple_hash.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1906 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/simple_hash/test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3620 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/simple_hash/test.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.355391 amuse-framework-2023.5.0/lib/stopcond/
+-rw-r--r--   0 rieder     (501) staff       (20)      688 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/stopcond/Makefile
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.355524 amuse-framework-2023.5.0/lib/stopcond/mpi/
+-rw-r--r--   0 rieder     (501) staff       (20)      243 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/stopcond/mpi/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)    18126 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/stopcond/stopcond.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3591 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/stopcond/stopcond.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1642 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/stopcond/stopcond.inc
+-rw-r--r--   0 rieder     (501) staff       (20)    21963 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/stopcond/stopcondf.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     9654 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/stopcond/stopcondf_isoc.F90
+-rw-r--r--   0 rieder     (501) staff       (20)      143 2023-05-17 09:30:35.000000 amuse-framework-2023.5.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:18:42.386507 amuse-framework-2023.5.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     2059 2023-05-17 09:47:47.000000 amuse-framework-2023.5.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.348353 amuse-framework-2023.5.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.356267 amuse-framework-2023.5.0/src/amuse/
+-rw-r--r--   0 rieder     (501) staff       (20)     1903 2023-04-15 06:02:12.000000 amuse-framework-2023.5.0/src/amuse/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/src/amuse/amuserc
+-rw-r--r--   0 rieder     (501) staff       (20)      915 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/src/amuse/codes.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.356414 amuse-framework-2023.5.0/src/amuse/community/
+-rw-r--r--   0 rieder     (501) staff       (20)     1277 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/src/amuse/community/__init__.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.357572 amuse-framework-2023.5.0/src/amuse/community/interface/
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3894 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/common.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3439 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/example.py
+-rw-r--r--   0 rieder     (501) staff       (20)    52603 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/gd.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12910 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/hydro.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1756 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/mhd.py
+-rw-r--r--   0 rieder     (501) staff       (20)    54169 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/se.py
+-rw-r--r--   0 rieder     (501) staff       (20)    28066 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/stopping_conditions.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2968 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/config.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.358679 amuse-framework-2023.5.0/src/amuse/couple/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    24220 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/couple/bridge.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5584 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/collision_handler.py
+-rw-r--r--   0 rieder     (501) staff       (20)    95615 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/encounters.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11720 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/fallback_stellar_evolution.py
+-rw-r--r--   0 rieder     (501) staff       (20)   122275 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/multiples.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6255 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/parallel_stellar_evolution.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.358985 amuse-framework-2023.5.0/src/amuse/data/
+-rw-r--r--   0 rieder     (501) staff       (20)    60725 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/data/AMUSE.bib
+-rw-r--r--   0 rieder     (501) staff       (20)       27 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/data/__init__.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.361921 amuse-framework-2023.5.0/src/amuse/datamodel/
+-rw-r--r--   0 rieder     (501) staff       (20)      388 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3473 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/attributes.py
+-rw-r--r--   0 rieder     (501) staff       (20)    64925 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/base.py
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/binding.py
+-rw-r--r--   0 rieder     (501) staff       (20)       42 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/code_particles.py
+-rw-r--r--   0 rieder     (501) staff       (20)      150 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/console.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7549 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/grid_attributes.py
+-rw-r--r--   0 rieder     (501) staff       (20)    42650 2023-04-17 12:49:34.000000 amuse-framework-2023.5.0/src/amuse/datamodel/grids.py
+-rw-r--r--   0 rieder     (501) staff       (20)    50773 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/incode_storage.py
+-rw-r--r--   0 rieder     (501) staff       (20)    13000 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/indexing.py
+-rw-r--r--   0 rieder     (501) staff       (20)    26559 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/memory_storage.py
+-rw-r--r--   0 rieder     (501) staff       (20)    26325 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/datamodel/parameters.py
+-rw-r--r--   0 rieder     (501) staff       (20)    47337 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/datamodel/particle_attributes.py
+-rw-r--r--   0 rieder     (501) staff       (20)   155220 2023-05-11 09:04:53.000000 amuse-framework-2023.5.0/src/amuse/datamodel/particles.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1551 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/rotation.py
+-rw-r--r--   0 rieder     (501) staff       (20)       74 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/set.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3904 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/simple_hash.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10234 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/staggeredgrid.py
+-rw-r--r--   0 rieder     (501) staff       (20)    14471 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/trees.py
+-rw-r--r--   0 rieder     (501) staff       (20)      188 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/values.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.369478 amuse-framework-2023.5.0/src/amuse/ext/
+-rw-r--r--   0 rieder     (501) staff       (20)     1290 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/ClusterCore.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2524 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/LagrangianRadii.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1689 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/SConstruct
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6021 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/basicgraph.py
+-rw-r--r--   0 rieder     (501) staff       (20)    69458 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/bbr_color.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     4018 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/bhtc_interface.pyx
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.369740 amuse-framework-2023.5.0/src/amuse/ext/blender/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/blender/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      771 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/blender/blender.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3386 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/boss_bodenheimer.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11167 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/bridge.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5473 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7430 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/composition_methods.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1932 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/comsystem.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6851 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/concurrent.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5397 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/cosmo.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2340 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/derived_grav_systems.py
+-rw-r--r--   0 rieder     (501) staff       (20)     9939 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/evrard_test.py
+-rw-r--r--   0 rieder     (501) staff       (20)     9832 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/galactic_potentials.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3541 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/galactics_model.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2446 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/gasplummer.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12018 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/ext/grid_remappers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5851 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/grid_to_sph.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2247 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/halogen_model.py
+-rw-r--r--   0 rieder     (501) staff       (20)    22588 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/hydro_collision.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12419 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/job_server.py
+-rw-r--r--   0 rieder     (501) staff       (20)       33 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/kingmodel.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10428 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/molecular_cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)    23761 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/orbital_elements.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6567 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/particles_with_color.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2982 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/plotting_hydro.py
+-rw-r--r--   0 rieder     (501) staff       (20)      134 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/plummer.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1271 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/plummer_helper.pyx
+-rw-r--r--   0 rieder     (501) staff       (20)     1917 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/polarsupport.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5030 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/protodisk.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1981 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/radial_profile.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4067 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/relax_sph.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10547 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/roche_radius.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6928 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/rotating_bridge.py
+-rw-r--r--   0 rieder     (501) staff       (20)      137 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/salpeter.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12155 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/sink.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11837 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/sobol.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12891 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/solarsystem.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2200 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/speed.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3482 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/sph_to_grid.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3314 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/sph_to_star.py
+-rw-r--r--   0 rieder     (501) staff       (20)    20811 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/spherical_model.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19994 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/star_to_sph.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8764 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/static_potentials.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2688 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/stellar_gyration_radius.py
+-rw-r--r--   0 rieder     (501) staff       (20)    18470 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/stellar_tidal_evolution.py
+-rw-r--r--   0 rieder     (501) staff       (20)    41820 2023-04-04 13:43:32.000000 amuse-framework-2023.5.0/src/amuse/ext/stellar_wind.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1386 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/sticky_spheres.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.372191 amuse-framework-2023.5.0/src/amuse/ic/
+-rw-r--r--   0 rieder     (501) staff       (20)     1229 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/__init__.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.372608 amuse-framework-2023.5.0/src/amuse/ic/_limepy/
+-rwxr-xr-x   0 rieder     (501) staff       (20)      204 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/_limepy/__init__.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)    43751 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/_limepy/limepy.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)    10121 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/_limepy/sample.py
+-rw-r--r--   0 rieder     (501) staff       (20)     9096 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/brokenimf.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2352 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/flatimf.py
+-rw-r--r--   0 rieder     (501) staff       (20)      151 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/fractalcluster.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3678 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/gasplummer.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7649 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/isotropic_cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)    20594 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/kingmodel.py
+-rw-r--r--   0 rieder     (501) staff       (20)      267 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/kroupa.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1724 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/limepy.py
+-rw-r--r--   0 rieder     (501) staff       (20)    13570 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/make_planets_oligarch.py
+-rw-r--r--   0 rieder     (501) staff       (20)       56 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/mameclot.py
+-rw-r--r--   0 rieder     (501) staff       (20)      295 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/millerscalo.py
+-rw-r--r--   0 rieder     (501) staff       (20)      468 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/molecular_cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6918 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/plummer.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2981 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/salpeter.py
+-rw-r--r--   0 rieder     (501) staff       (20)      263 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/scalo.py
+-rw-r--r--   0 rieder     (501) staff       (20)    21531 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/solar_system_moons.py
+-rw-r--r--   0 rieder     (501) staff       (20)      165 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/solarsystem.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.374654 amuse-framework-2023.5.0/src/amuse/io/
+-rw-r--r--   0 rieder     (501) staff       (20)     1001 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    17890 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/base.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6347 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/fi_io.py
+-rw-r--r--   0 rieder     (501) staff       (20)    16756 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/gadget.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/horizons.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12272 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/nemobin.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5389 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/nemotsf.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1027 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/p10.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     4241 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/phigrape.py
+-rw-r--r--   0 rieder     (501) staff       (20)    17938 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/starlab.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6419 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/store.py
+-rw-r--r--   0 rieder     (501) staff       (20)    32086 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/store_v1.py
+-rw-r--r--   0 rieder     (501) staff       (20)    46982 2023-05-11 09:04:53.000000 amuse-framework-2023.5.0/src/amuse/io/store_v2.py
+-rw-r--r--   0 rieder     (501) staff       (20)    22593 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/text.py
+-rw-r--r--   0 rieder     (501) staff       (20)    14998 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/vtk.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4808 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/lab.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.375177 amuse-framework-2023.5.0/src/amuse/plot/
+-rw-r--r--   0 rieder     (501) staff       (20)       21 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/plot/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    22278 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/plot/_plot.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)    13863 2023-04-04 13:20:13.000000 amuse-framework-2023.5.0/src/amuse/plot/hydro.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12634 2023-03-16 12:23:56.000000 amuse-framework-2023.5.0/src/amuse/plot/mapper.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.376543 amuse-framework-2023.5.0/src/amuse/rfi/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    23061 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/async_request.py
+-rw-r--r--   0 rieder     (501) staff       (20)    88683 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/channel.py
+-rw-r--r--   0 rieder     (501) staff       (20)    52496 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/core.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)    15246 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/gencode.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4329 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/import_module.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5500 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/nospawn.py
+-rw-r--r--   0 rieder     (501) staff       (20)    23380 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/python_code.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1197 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/run_command_redirected.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2138 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/slurm.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.378203 amuse-framework-2023.5.0/src/amuse/rfi/tools/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    45482 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_c.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4264 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_code.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10659 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_definition.py
+-rw-r--r--   0 rieder     (501) staff       (20)    15062 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_dir.py
+-rw-r--r--   0 rieder     (501) staff       (20)    64699 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_fortran.py
+-rw-r--r--   0 rieder     (501) staff       (20)    53344 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_java.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2216 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_python_worker.py
+-rw-r--r--   0 rieder     (501) staff       (20)      991 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/cython_code_script.template
+-rw-r--r--   0 rieder     (501) staff       (20)    11322 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/fortran_tools.py
+-rw-r--r--   0 rieder     (501) staff       (20)      980 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/java_code_script.template
+-rw-r--r--   0 rieder     (501) staff       (20)     1102 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/python_code_script.template
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.380099 amuse-framework-2023.5.0/src/amuse/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      569 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5372 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/code.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11337 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/support/console.py
+-rw-r--r--   0 rieder     (501) staff       (20)    15197 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/core.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2073 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/exceptions.py
+-rw-r--r--   0 rieder     (501) staff       (20)    61635 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11438 2023-04-15 06:02:12.000000 amuse-framework-2023.5.0/src/amuse/support/literature.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8981 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/methods.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10236 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/support/options.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11751 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/parameter_tools.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1183 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/project.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19392 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/state.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.380698 amuse-framework-2023.5.0/src/amuse/support/thirdparty/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/thirdparty/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    18956 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/thirdparty/texttable.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.381382 amuse-framework-2023.5.0/src/amuse/test/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/test/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12935 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/test/amusetest.py
+-rw-r--r--   0 rieder     (501) staff       (20)    14500 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/test/compile_tools.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.384403 amuse-framework-2023.5.0/src/amuse/units/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    18324 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/constants.py
+-rw-r--r--   0 rieder     (501) staff       (20)    33642 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/core.py
+-rw-r--r--   0 rieder     (501) staff       (20)      731 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/units/derivedsi.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11358 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/generic_unit_converter.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2792 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/units/generic_unit_system.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4912 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/nbody_system.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7342 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/nist.py
+-rw-r--r--   0 rieder     (501) staff       (20)    33920 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/nist.txt
+-rw-r--r--   0 rieder     (501) staff       (20)    38873 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/nist2010.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     4718 2023-03-14 12:52:28.000000 amuse-framework-2023.5.0/src/amuse/units/optparse.py
+-rw-r--r--   0 rieder     (501) staff       (20)    44745 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/units/quantities.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1853 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/scaling_converter.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2349 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/units/si.py
+-rw-r--r--   0 rieder     (501) staff       (20)      190 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/translator.txt
+-rw-r--r--   0 rieder     (501) staff       (20)      780 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/trigo.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4019 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/units/units.py
+-rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:18:40.000000 amuse-framework-2023.5.0/src/amuse/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.384974 amuse-framework-2023.5.0/src/amuse_framework.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1242 2023-05-17 10:18:40.000000 amuse-framework-2023.5.0/src/amuse_framework.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     7390 2023-05-17 10:18:42.000000 amuse-framework-2023.5.0/src/amuse_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:18:40.000000 amuse-framework-2023.5.0/src/amuse_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)      130 2023-05-17 10:18:40.000000 amuse-framework-2023.5.0/src/amuse_framework.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:18:40.000000 amuse-framework-2023.5.0/src/amuse_framework.egg-info/top_level.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.386097 amuse-framework-2023.5.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-framework-2023.5.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/version.py
```

### Comparing `amuse-framework-2023.4.0/MANIFEST.in` & `amuse-framework-2023.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/Makefile.in` & `amuse-framework-2023.5.0/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/PKG-INFO` & `amuse-framework-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-framework
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: The Astrophysical Multipurpose Software Environment
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `amuse-framework-2023.4.0/bin/amusifier.in` & `amuse-framework-2023.5.0/bin/amusifier.in`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/config.guess` & `amuse-framework-2023.5.0/config.guess`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/config.mk.in` & `amuse-framework-2023.5.0/config.mk.in`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/config.sub` & `amuse-framework-2023.5.0/config.sub`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/configure` & `amuse-framework-2023.5.0/configure`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/install-sh` & `amuse-framework-2023.5.0/install-sh`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/forsockets/forsockets.c` & `amuse-framework-2023.5.0/lib/forsockets/forsockets.c`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/forsockets/forsockets.h` & `amuse-framework-2023.5.0/lib/forsockets/forsockets.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/forsockets/forsocketsf.f90` & `amuse-framework-2023.5.0/lib/forsockets/forsocketsf.f90`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/g6/g6lib.c` & `amuse-framework-2023.5.0/lib/g6/g6lib.c`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/g6/g6lib.h` & `amuse-framework-2023.5.0/lib/g6/g6lib.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_2/Makefile` & `amuse-framework-2023.5.0/lib/sapporo_2/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_2/download.py` & `amuse-framework-2023.5.0/lib/sapporo_2/download.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/Makefile` & `amuse-framework-2023.5.0/lib/sapporo_light/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/README` & `amuse-framework-2023.5.0/lib/sapporo_light/README`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/dev_evaluate_gravity.cu` & `amuse-framework-2023.5.0/lib/sapporo_light/dev_evaluate_gravity.cu`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/g6lib.c` & `amuse-framework-2023.5.0/lib/sapporo_light/g6lib.c`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/g6lib.h` & `amuse-framework-2023.5.0/lib/sapporo_light/g6lib.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/host_evaluate_gravity.cu` & `amuse-framework-2023.5.0/lib/sapporo_light/host_evaluate_gravity.cu`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/sapporo.cpp` & `amuse-framework-2023.5.0/lib/sapporo_light/sapporo.cpp`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/sapporo.h` & `amuse-framework-2023.5.0/lib/sapporo_light/sapporo.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/sapporoG6lib.cpp` & `amuse-framework-2023.5.0/lib/sapporo_light/sapporoG6lib.cpp`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/sapporo_defs.h` & `amuse-framework-2023.5.0/lib/sapporo_light/sapporo_defs.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/sapporo_multi.h` & `amuse-framework-2023.5.0/lib/sapporo_light/sapporo_multi.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/sapporo_light/send_fetch_data.cpp` & `amuse-framework-2023.5.0/lib/sapporo_light/send_fetch_data.cpp`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/simple_hash/Makefile` & `amuse-framework-2023.5.0/lib/simple_hash/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/simple_hash/simple_hash.c` & `amuse-framework-2023.5.0/lib/simple_hash/simple_hash.c`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/simple_hash/simple_hash.h` & `amuse-framework-2023.5.0/lib/simple_hash/simple_hash.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/simple_hash/test.cpp` & `amuse-framework-2023.5.0/lib/simple_hash/test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/simple_hash/test.py` & `amuse-framework-2023.5.0/lib/simple_hash/test.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/stopcond/Makefile` & `amuse-framework-2023.5.0/lib/stopcond/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/stopcond/stopcond.c` & `amuse-framework-2023.5.0/lib/stopcond/stopcond.c`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/stopcond/stopcond.h` & `amuse-framework-2023.5.0/lib/stopcond/stopcond.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/stopcond/stopcond.inc` & `amuse-framework-2023.5.0/lib/stopcond/stopcond.inc`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/stopcond/stopcondf.F90` & `amuse-framework-2023.5.0/lib/stopcond/stopcondf.F90`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/lib/stopcond/stopcondf_isoc.F90` & `amuse-framework-2023.5.0/lib/stopcond/stopcondf_isoc.F90`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/setup.py` & `amuse-framework-2023.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 package_data = {
     'amuse.rfi.tools': ['*.template'],
     'amuse': [
         '*rc'
     ]
 }
 
-mapping_from_command_name_to_command_class=setup_commands()
+mapping_from_command_name_to_command_class = setup_commands()
 
 try:
     from src.amuse.version import version
     use_scm_version = False
     setup_requires = []
 except ImportError:
     version = False
@@ -63,18 +63,18 @@
     author=author,
     license=license_,
     description=description,
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     install_requires=install_requires,
     python_requires=">=3.7",
-    extras_require = {
-        "MPI" : ["mpi4py>=1.1.0"]
+    extras_require={
+        "MPI": ["mpi4py>=1.1.0"]
     },
     cmdclass=mapping_from_command_name_to_command_class,
     ext_modules=extensions,
     package_dir={'': 'src'},
     packages=packages,
     package_data=package_data,
     data_files=all_data_files,
-    scripts=[ "bin/amusifier" ],
+    scripts=["bin/amusifier", ],
 )
```

### Comparing `amuse-framework-2023.4.0/src/amuse/__init__.py` & `amuse-framework-2023.5.0/src/amuse/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/codes.py` & `amuse-framework-2023.5.0/src/amuse/codes.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/community/__init__.py` & `amuse-framework-2023.5.0/src/amuse/community/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/community/interface/common.py` & `amuse-framework-2023.5.0/src/amuse/community/interface/common.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/community/interface/example.py` & `amuse-framework-2023.5.0/src/amuse/community/interface/example.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/community/interface/gd.py` & `amuse-framework-2023.5.0/src/amuse/community/interface/gd.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/community/interface/hydro.py` & `amuse-framework-2023.5.0/src/amuse/community/interface/hydro.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/community/interface/mhd.py` & `amuse-framework-2023.5.0/src/amuse/community/interface/mhd.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/community/interface/se.py` & `amuse-framework-2023.5.0/src/amuse/community/interface/se.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/community/interface/stopping_conditions.py` & `amuse-framework-2023.5.0/src/amuse/community/interface/stopping_conditions.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/config.py` & `amuse-framework-2023.5.0/src/amuse/config.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/couple/bridge.py` & `amuse-framework-2023.5.0/src/amuse/couple/bridge.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/couple/collision_handler.py` & `amuse-framework-2023.5.0/src/amuse/couple/collision_handler.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/couple/encounters.py` & `amuse-framework-2023.5.0/src/amuse/couple/encounters.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/couple/fallback_stellar_evolution.py` & `amuse-framework-2023.5.0/src/amuse/couple/fallback_stellar_evolution.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/couple/multiples.py` & `amuse-framework-2023.5.0/src/amuse/couple/multiples.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/couple/parallel_stellar_evolution.py` & `amuse-framework-2023.5.0/src/amuse/couple/parallel_stellar_evolution.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/data/AMUSE.bib` & `amuse-framework-2023.5.0/src/amuse/data/AMUSE.bib`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/attributes.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/attributes.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/base.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/base.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/grid_attributes.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/grid_attributes.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/grids.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/grids.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,14 +264,17 @@
         if "position" in self._derived_attributes:
             return self._derived_attributes["position"].attribute_names
         if "position" in self.GLOBAL_DERIVED_ATTRIBUTES:
             return self.GLOBAL_DERIVED_ATTRIBUTES["position"].attribute_names
 
         raise Exception("do not know how to find axes_names")
 
+    def set_axes_names(self, value):
+        self.add_vector_attribute('position', value)
+
 class UnstructuredGrid(BaseGrid):
     GLOBAL_DERIVED_ATTRIBUTES=CompositeDictionary(BaseGrid.GLOBAL_DERIVED_ATTRIBUTES)
 class StructuredBaseGrid(BaseGrid):
     GLOBAL_DERIVED_ATTRIBUTES=CompositeDictionary(BaseGrid.GLOBAL_DERIVED_ATTRIBUTES)
 class StructuredGrid(StructuredBaseGrid):
     GLOBAL_DERIVED_ATTRIBUTES=CompositeDictionary(StructuredBaseGrid.GLOBAL_DERIVED_ATTRIBUTES)
 class RectilinearBaseGrid(StructuredBaseGrid):
```

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/incode_storage.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/incode_storage.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/indexing.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/indexing.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/memory_storage.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/memory_storage.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/parameters.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/parameters.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/particle_attributes.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/particle_attributes.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/particles.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/particles.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,14 +382,15 @@
         for x in values:
             if isinstance(x, (LinkedArray, ParticlesSubset)):
                 converted.append(x.copy(memento, keep_structure, filter_attributes))
             else:
                 converted.append(x)
         result.add_particles_to_store(keys, attributes, converted)
 
+        object.__setattr__(result, "_derived_attributes", CompositeDictionary(self._derived_attributes))
         result._private.collection_attributes = self._private.collection_attributes._copy_for_collection(result)
 
         return result
 
 
 
     def copy_to_new_particles(self, keys = None, keys_generator = None, memento = None, keep_structure = False, filter_attributes = lambda particle_set, x : True):
@@ -421,14 +422,15 @@
             else:
                 converted.append(x)
 
         memento[id(self._original_set())] = result
 
         result.add_particles_to_store(particle_keys, attributes, converted)
 
+        object.__setattr__(result, "_derived_attributes", CompositeDictionary(self._derived_attributes))
         result._private.collection_attributes = self._private.collection_attributes._copy_for_collection(result)
 
         return result
 
     def _factory_for_new_collection(self):
         return Particles
```

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/rotation.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/rotation.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/simple_hash.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/simple_hash.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/staggeredgrid.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/staggeredgrid.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/datamodel/trees.py` & `amuse-framework-2023.5.0/src/amuse/datamodel/trees.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/ClusterCore.py` & `amuse-framework-2023.5.0/src/amuse/ext/ClusterCore.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/LagrangianRadii.py` & `amuse-framework-2023.5.0/src/amuse/ext/LagrangianRadii.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/SConstruct` & `amuse-framework-2023.5.0/src/amuse/ext/SConstruct`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/basicgraph.py` & `amuse-framework-2023.5.0/src/amuse/ext/basicgraph.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/bbr_color.txt` & `amuse-framework-2023.5.0/src/amuse/ext/bbr_color.txt`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/bhtc_interface.pyx` & `amuse-framework-2023.5.0/src/amuse/ext/bhtc_interface.pyx`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/blender/blender.py` & `amuse-framework-2023.5.0/src/amuse/ext/blender/blender.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/boss_bodenheimer.py` & `amuse-framework-2023.5.0/src/amuse/ext/boss_bodenheimer.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/bridge.py` & `amuse-framework-2023.5.0/src/amuse/ext/bridge.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/cloud.py` & `amuse-framework-2023.5.0/src/amuse/ext/cloud.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/composition_methods.py` & `amuse-framework-2023.5.0/src/amuse/ext/composition_methods.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/comsystem.py` & `amuse-framework-2023.5.0/src/amuse/ext/comsystem.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/concurrent.py` & `amuse-framework-2023.5.0/src/amuse/ext/concurrent.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/cosmo.py` & `amuse-framework-2023.5.0/src/amuse/ext/cosmo.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/derived_grav_systems.py` & `amuse-framework-2023.5.0/src/amuse/ext/derived_grav_systems.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/evrard_test.py` & `amuse-framework-2023.5.0/src/amuse/ext/evrard_test.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/galactic_potentials.py` & `amuse-framework-2023.5.0/src/amuse/ext/galactic_potentials.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/galactics_model.py` & `amuse-framework-2023.5.0/src/amuse/ext/galactics_model.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/gasplummer.py` & `amuse-framework-2023.5.0/src/amuse/ext/gasplummer.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/grid_remappers.py` & `amuse-framework-2023.5.0/src/amuse/ext/grid_remappers.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/grid_to_sph.py` & `amuse-framework-2023.5.0/src/amuse/ext/grid_to_sph.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/halogen_model.py` & `amuse-framework-2023.5.0/src/amuse/ext/halogen_model.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/hydro_collision.py` & `amuse-framework-2023.5.0/src/amuse/ext/hydro_collision.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/job_server.py` & `amuse-framework-2023.5.0/src/amuse/ext/job_server.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/molecular_cloud.py` & `amuse-framework-2023.5.0/src/amuse/ext/molecular_cloud.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/orbital_elements.py` & `amuse-framework-2023.5.0/src/amuse/ext/orbital_elements.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/particles_with_color.py` & `amuse-framework-2023.5.0/src/amuse/ext/particles_with_color.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/plotting_hydro.py` & `amuse-framework-2023.5.0/src/amuse/ext/plotting_hydro.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/plummer_helper.pyx` & `amuse-framework-2023.5.0/src/amuse/ext/plummer_helper.pyx`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/polarsupport.py` & `amuse-framework-2023.5.0/src/amuse/ext/polarsupport.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/protodisk.py` & `amuse-framework-2023.5.0/src/amuse/ext/protodisk.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/radial_profile.py` & `amuse-framework-2023.5.0/src/amuse/ext/radial_profile.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/relax_sph.py` & `amuse-framework-2023.5.0/src/amuse/ext/relax_sph.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/roche_radius.py` & `amuse-framework-2023.5.0/src/amuse/ext/roche_radius.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/rotating_bridge.py` & `amuse-framework-2023.5.0/src/amuse/ext/rotating_bridge.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/sink.py` & `amuse-framework-2023.5.0/src/amuse/ext/sink.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/sobol.py` & `amuse-framework-2023.5.0/src/amuse/ext/sobol.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/solarsystem.py` & `amuse-framework-2023.5.0/src/amuse/ext/solarsystem.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/speed.py` & `amuse-framework-2023.5.0/src/amuse/ext/speed.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/sph_to_grid.py` & `amuse-framework-2023.5.0/src/amuse/ext/sph_to_grid.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/sph_to_star.py` & `amuse-framework-2023.5.0/src/amuse/ext/sph_to_star.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/spherical_model.py` & `amuse-framework-2023.5.0/src/amuse/ext/spherical_model.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/star_to_sph.py` & `amuse-framework-2023.5.0/src/amuse/ext/star_to_sph.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/static_potentials.py` & `amuse-framework-2023.5.0/src/amuse/ext/static_potentials.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/stellar_gyration_radius.py` & `amuse-framework-2023.5.0/src/amuse/ext/stellar_gyration_radius.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/stellar_tidal_evolution.py` & `amuse-framework-2023.5.0/src/amuse/ext/stellar_tidal_evolution.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/stellar_wind.py` & `amuse-framework-2023.5.0/src/amuse/ext/stellar_wind.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ext/sticky_spheres.py` & `amuse-framework-2023.5.0/src/amuse/ext/sticky_spheres.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/__init__.py` & `amuse-framework-2023.5.0/src/amuse/ic/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/_limepy/limepy.py` & `amuse-framework-2023.5.0/src/amuse/ic/_limepy/limepy.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/_limepy/sample.py` & `amuse-framework-2023.5.0/src/amuse/ic/_limepy/sample.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/brokenimf.py` & `amuse-framework-2023.5.0/src/amuse/ic/brokenimf.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/flatimf.py` & `amuse-framework-2023.5.0/src/amuse/ic/flatimf.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/gasplummer.py` & `amuse-framework-2023.5.0/src/amuse/ic/gasplummer.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/isotropic_cloud.py` & `amuse-framework-2023.5.0/src/amuse/ic/isotropic_cloud.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/kingmodel.py` & `amuse-framework-2023.5.0/src/amuse/ic/kingmodel.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/limepy.py` & `amuse-framework-2023.5.0/src/amuse/ic/limepy.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/make_planets_oligarch.py` & `amuse-framework-2023.5.0/src/amuse/ic/make_planets_oligarch.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/plummer.py` & `amuse-framework-2023.5.0/src/amuse/ic/plummer.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/salpeter.py` & `amuse-framework-2023.5.0/src/amuse/ic/salpeter.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/ic/solar_system_moons.py` & `amuse-framework-2023.5.0/src/amuse/ic/solar_system_moons.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/__init__.py` & `amuse-framework-2023.5.0/src/amuse/io/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/base.py` & `amuse-framework-2023.5.0/src/amuse/io/base.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/fi_io.py` & `amuse-framework-2023.5.0/src/amuse/io/fi_io.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/gadget.py` & `amuse-framework-2023.5.0/src/amuse/io/gadget.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/horizons.py` & `amuse-framework-2023.5.0/src/amuse/io/horizons.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/nemobin.py` & `amuse-framework-2023.5.0/src/amuse/io/nemobin.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/nemotsf.py` & `amuse-framework-2023.5.0/src/amuse/io/nemotsf.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/p10.txt` & `amuse-framework-2023.5.0/src/amuse/io/p10.txt`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/phigrape.py` & `amuse-framework-2023.5.0/src/amuse/io/phigrape.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/starlab.py` & `amuse-framework-2023.5.0/src/amuse/io/starlab.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/store.py` & `amuse-framework-2023.5.0/src/amuse/io/store.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/store_v1.py` & `amuse-framework-2023.5.0/src/amuse/io/store_v1.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/store_v2.py` & `amuse-framework-2023.5.0/src/amuse/io/store_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from amuse.datamodel import Particles
 from amuse.datamodel import Particle
 from amuse.datamodel import AttributeStorage
 from amuse.datamodel import LinkedArray
 from amuse.datamodel import Grid
 from amuse.datamodel import GridPoint
 from amuse.datamodel import AbstractSet
+from amuse.datamodel.base import VectorAttribute
+
 
 from amuse.io import store_v1
 
 import warnings
 
 import logging
 logger = logging.getLogger(__name__)
@@ -843,14 +845,15 @@
             data=keys,
             compression=self.compression,
             compression_opts=self.compression_opts,
         )
         self.hdf5file.flush()
         self.store_collection_attributes(particles, group, extra_attributes, links)
         self.store_values(particles, group, links)
+        self.store_selected_derived_attributes(particles,group)    
             
         mapping_from_setid_to_group[id(particles)] = group
         
         self.hdf5file.flush()
         
     
     def store_grid(self, grid, extra_attributes = {}, parent=None, mapping_from_setid_to_group = {}, links = []):
@@ -864,14 +867,15 @@
         group.create_dataset(
             "shape",
             data=numpy.asarray(grid.shape),
             compression=self.compression,
             compression_opts=self.compression_opts,
         )
     
+        self.store_selected_derived_attributes(grid, group)
         self.store_collection_attributes(grid, group, extra_attributes, links)
         self.store_values(grid, group, links)
         
         mapping_from_setid_to_group[id(grid)] = group
         
         self.hdf5file.flush()
         
@@ -920,16 +924,23 @@
                         attribute,
                         data=quantity,
                         compression=self.compression,
                         compression_opts=self.compression_opts,
                     )
                     dataset.attrs["units"] = "none".encode('ascii')
                 
+    def store_selected_derived_attributes(self, container, group):
+        saving=dict()
+        for key in container._derived_attributes.keys():
+            attr=container._derived_attributes[key]
+            if key not in container.GLOBAL_DERIVED_ATTRIBUTES and isinstance(attr, VectorAttribute):
+                saving[key]=attr
+        if len(saving): 
+            group.attrs["extra_vector_attributes"]=pickle_to_string(saving)
     
-
     def store_linked_array(self, attribute, attributes_group, quantity, group, links):
         subgroup = attributes_group.create_group(attribute)
         shape = quantity.shape
         kind_array = numpy.zeros(shape, dtype = numpy.int16)
         ref_dtype = h5py.special_dtype(ref=h5py.Reference)
         ref_array = numpy.empty(shape, dtype = ref_dtype)
         ref_dataset = subgroup.create_dataset(
@@ -1123,33 +1134,41 @@
             dataset.read_direct(keys)
         
             particles = class_of_the_container(is_working_copy = False)
             particles._private.attribute_storage = HDF5AttributeStorage(keys, group, self)
        
             self.mapping_from_groupid_to_set[group.id] = particles
             self.load_collection_attributes(particles, group)
-        
-        
+        if "extra_vector_attributes" in group.attrs.keys():
+            self.load_extra_derived_attributes(particles, group)
+                
         return particles
         
     def load_grid_from_group(self, group):
         try:
             class_of_the_container = unpickle_from_string(group.attrs["class_of_the_container"])
         except:
             class_of_the_container = Grid 
             
         shape = tuple(group["shape"])
         
         container = class_of_the_container()
         container._private.attribute_storage = HDF5GridAttributeStorage(shape, group, self)
         self.mapping_from_groupid_to_set[group.id] = container
         self.load_collection_attributes(container, group)
+        if "extra_vector_attributes" in group.attrs.keys():
+            self.load_extra_derived_attributes(container, group)
         
         return container
     
+    def load_extra_derived_attributes(self, container, group):
+        attrs=unpickle_from_string(group.attrs["extra_vector_attributes"])
+        for key, attr in attrs.items():
+            container._derived_attributes[key]=attr
+    
     def load_from_group(self, group):
         container_type = group.attrs['type'] if isinstance(group.attrs['type'], str) else group.attrs['type'].decode('ascii') 
         
         if container_type == 'particles':
             return self.load_particles_from_group(group)
         elif container_type == 'grid':
             return self.load_grid_from_group(group)
```

### Comparing `amuse-framework-2023.4.0/src/amuse/io/text.py` & `amuse-framework-2023.5.0/src/amuse/io/text.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/io/vtk.py` & `amuse-framework-2023.5.0/src/amuse/io/vtk.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/lab.py` & `amuse-framework-2023.5.0/src/amuse/lab.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/plot/_plot.py` & `amuse-framework-2023.5.0/src/amuse/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/plot/hydro.py` & `amuse-framework-2023.5.0/src/amuse/plot/hydro.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/plot/mapper.py` & `amuse-framework-2023.5.0/src/amuse/plot/mapper.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/async_request.py` & `amuse-framework-2023.5.0/src/amuse/rfi/async_request.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/channel.py` & `amuse-framework-2023.5.0/src/amuse/rfi/channel.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/core.py` & `amuse-framework-2023.5.0/src/amuse/rfi/core.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/gencode.py` & `amuse-framework-2023.5.0/src/amuse/rfi/gencode.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/import_module.py` & `amuse-framework-2023.5.0/src/amuse/rfi/import_module.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/nospawn.py` & `amuse-framework-2023.5.0/src/amuse/rfi/nospawn.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/python_code.py` & `amuse-framework-2023.5.0/src/amuse/rfi/python_code.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/run_command_redirected.py` & `amuse-framework-2023.5.0/src/amuse/rfi/run_command_redirected.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/slurm.py` & `amuse-framework-2023.5.0/src/amuse/rfi/slurm.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/create_c.py` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_c.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/create_code.py` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_code.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/create_definition.py` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_definition.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/create_dir.py` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_dir.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/create_fortran.py` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_fortran.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/create_java.py` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_java.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/create_python_worker.py` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_python_worker.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/cython_code_script.template` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/cython_code_script.template`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/fortran_tools.py` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/fortran_tools.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/java_code_script.template` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/java_code_script.template`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/rfi/tools/python_code_script.template` & `amuse-framework-2023.5.0/src/amuse/rfi/tools/python_code_script.template`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/__init__.py` & `amuse-framework-2023.5.0/src/amuse/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/code.py` & `amuse-framework-2023.5.0/src/amuse/support/code.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/console.py` & `amuse-framework-2023.5.0/src/amuse/support/console.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/core.py` & `amuse-framework-2023.5.0/src/amuse/support/core.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/exceptions.py` & `amuse-framework-2023.5.0/src/amuse/support/exceptions.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/interface.py` & `amuse-framework-2023.5.0/src/amuse/support/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/literature.py` & `amuse-framework-2023.5.0/src/amuse/support/literature.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/methods.py` & `amuse-framework-2023.5.0/src/amuse/support/methods.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/options.py` & `amuse-framework-2023.5.0/src/amuse/support/options.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/parameter_tools.py` & `amuse-framework-2023.5.0/src/amuse/support/parameter_tools.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/project.py` & `amuse-framework-2023.5.0/src/amuse/support/project.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/state.py` & `amuse-framework-2023.5.0/src/amuse/support/state.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/support/thirdparty/texttable.py` & `amuse-framework-2023.5.0/src/amuse/support/thirdparty/texttable.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/test/amusetest.py` & `amuse-framework-2023.5.0/src/amuse/test/amusetest.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/test/compile_tools.py` & `amuse-framework-2023.5.0/src/amuse/test/compile_tools.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/constants.py` & `amuse-framework-2023.5.0/src/amuse/units/constants.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/core.py` & `amuse-framework-2023.5.0/src/amuse/units/core.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/derivedsi.py` & `amuse-framework-2023.5.0/src/amuse/units/derivedsi.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/generic_unit_converter.py` & `amuse-framework-2023.5.0/src/amuse/units/generic_unit_converter.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/generic_unit_system.py` & `amuse-framework-2023.5.0/src/amuse/units/generic_unit_system.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/nbody_system.py` & `amuse-framework-2023.5.0/src/amuse/units/nbody_system.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/nist.py` & `amuse-framework-2023.5.0/src/amuse/units/nist.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/nist.txt` & `amuse-framework-2023.5.0/src/amuse/units/nist.txt`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/nist2010.txt` & `amuse-framework-2023.5.0/src/amuse/units/nist2010.txt`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/optparse.py` & `amuse-framework-2023.5.0/src/amuse/units/optparse.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/quantities.py` & `amuse-framework-2023.5.0/src/amuse/units/quantities.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/scaling_converter.py` & `amuse-framework-2023.5.0/src/amuse/units/scaling_converter.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/si.py` & `amuse-framework-2023.5.0/src/amuse/units/si.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/trigo.py` & `amuse-framework-2023.5.0/src/amuse/units/trigo.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse/units/units.py` & `amuse-framework-2023.5.0/src/amuse/units/units.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/src/amuse_framework.egg-info/PKG-INFO` & `amuse-framework-2023.5.0/src/amuse_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-framework
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: The Astrophysical Multipurpose Software Environment
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `amuse-framework-2023.4.0/src/amuse_framework.egg-info/SOURCES.txt` & `amuse-framework-2023.5.0/src/amuse_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/support/__init__.py` & `amuse-framework-2023.5.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/support/classifiers.py` & `amuse-framework-2023.5.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/support/config.py` & `amuse-framework-2023.5.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/support/generate_main.py` & `amuse-framework-2023.5.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/support/getsp.class` & `amuse-framework-2023.5.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/support/getsp.java` & `amuse-framework-2023.5.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/support/misc.py` & `amuse-framework-2023.5.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.4.0/support/setup_codes.py` & `amuse-framework-2023.5.0/support/setup_codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,52 @@
-
-
-__revision__ = "$Id:$"
-
 import warnings
-import sys, os, re, subprocess
+import sys
+import os
 import os.path
+import re
 import datetime
-import stat
 from copy import deepcopy
 from os.path import abspath
 
-from . import supportrc
-
 try:
     import numpy
 except ImportError:
-    warnings.warn( "numpy etc needed during build; operation may fail" )
+    warnings.warn("numpy needed during build; operation may fail")
 
 import configparser
-from io import StringIO
 
-from stat import ST_MODE
-from distutils import sysconfig
-from distutils.core import Command
-from distutils.dep_util import newer
+from subprocess import Popen, PIPE, STDOUT
+
+from glob import glob
+
 from distutils.dir_util import create_tree
-from distutils.util import convert_path
-from distutils import log
+# from distutils import log
+import logging
 from distutils import spawn
 from distutils import file_util
 from distutils.errors import DistutilsError
 from distutils.command.clean import clean
-from distutils.command.install import install
+from setuptools.command.install import install
+from setuptools import Command
 from setuptools.command.build import build
 from setuptools.command.develop import develop
 from setuptools.command.editable_wheel import editable_wheel
 
-from subprocess import call, Popen, PIPE, STDOUT
+from . import supportrc
 
 if supportrc["framework_install"]:
     from .generate_main import generate_main
-  
+
 try:
     from numpy.distutils import fcompiler
 except ImportError:
     fcompiler = None
 
 # check if Python is called on the first line with this expression
 first_line_re = re.compile('^#!.*python[0-9.]*([ \t].*)?$')
-    
-from glob import glob
 
 def pyfiles_in_build_dir(builddir):
     module_files = glob(os.path.join(builddir, "*.py"))
     result = []
     for x in module_files:
         result.append(os.path.abspath(x))
     return result
@@ -68,125 +61,122 @@
         ('no-inplace', 'k',
          "put compiled extensions into the  build temp "),
         ('lib-dir=', 'l', "directory containing libraries to build"),
         ('install-data=', None, "installation directory for data files"),
         ('root=', None, "install everything relative to this alternate root directory"),
     ]
 
-    negative_opt = {'no-inplace':'inplace'}
-    
+    negative_opt = {'no-inplace': 'inplace'}
+
     boolean_options = ['inplace']
 
-    def initialize_options (self):
+    def initialize_options(self):
         self.codes_dir = None
         self.lib_dir = None
         self.inplace = False
         self.build_lib = None
         self.build_temp = None
         self.install_data = None
-        self.root=None
-                
-    def finalize_options (self):
+        self.root = None
+
+    def finalize_options(self):
         self.set_undefined_options(
             'install',
-           ('build_lib', 'build_lib'),
-           ('root', 'root'),
-           ('install_data', 'install_data'),           
+            ('build_lib', 'build_lib'),
+            ('root', 'root'),
+            ('install_data', 'install_data'),
         )
 
         self.set_undefined_options(
             'build',
-           ('build_temp', 'build_temp'),
+            ('build_temp', 'build_temp'),
         )
 
         if self.lib_dir is None:
             if self.inplace:
                 self.lib_dir = os.path.join('lib')
             else:
                 self.lib_dir = os.path.join(self.build_temp, 'lib')
         else:
             if self.inplace:
                 pass
             else:
-                self.lib_dir=os.path.join(self.build_temp, 'lib')
+                self.lib_dir = os.path.join(self.build_temp, 'lib')
 
     def run(self):
-        data_dir = os.path.join(self.install_data,'share','amuse') # for the moment add to amuse..
+        data_dir = os.path.join(self.install_data, 'share', 'amuse')  # for the moment add to amuse..
         data_dir = os.path.abspath(data_dir)
 
         # copy only:
         # '*.h', '*.a', '*.mod', '*.inc', '*.so', '*.dylib'
-        files=[os.path.join(dp, f) for dp, dn, fn in os.walk(self.lib_dir) for f in fn]
-        ext=['.h', '.a', '.mod', '.inc', '.so', '.dylib']
-        files=[f  for f in files if (os.path.splitext(f)[1] in ext)]
-        files=[os.path.relpath(f,self.lib_dir) for f in files]
-        create_tree(os.path.join(data_dir,'lib'), files)
+        files = [os.path.join(dp, f) for dp, dn, fn in os.walk(self.lib_dir) for f in fn]
+        ext = ['.h', '.a', '.mod', '.inc', '.so', '.dylib']
+        files = [f for f in files if (os.path.splitext(f)[1] in ext)]
+        files = [os.path.relpath(f, self.lib_dir) for f in files]
+        create_tree(os.path.join(data_dir, 'lib'), files)
 
         for f in files:
-            src=os.path.join(self.lib_dir,f)
-            target=os.path.join(data_dir,'lib', f)
-            self.copy_file(src,target)
+            src = os.path.join(self.lib_dir, f)
+            target = os.path.join(data_dir, 'lib', f)
+            self.copy_file(src, target)
 
 class GenerateInstallIni(Command):
-    user_options =   (
+    user_options = (
         ('build-dir=', 'd', "directory to install to"),
         ('install-data=', None, "installation directory for data files"),
         ('force', 'f', "force installation (overwrite existing files)"),
         ('root=', None, "install everything relative to this alternate root directory"),
     )
-    
+
     boolean_options = ['force']
-    
+
     def initialize_options(self):
         self.build_dir = None
         self.install_data = None
         self.force = False
         self.root = None
-        
+
     def finalize_options(self):
         self.set_undefined_options(
             'install',
             ('build_lib', 'build_dir'),
             ('install_data', 'install_data'),
             ('root', 'root'),
             ('force', 'force'),
         )
-        
+
     def run(self):
         outfilename = os.path.join(self.build_dir, supportrc["package_name"], 'amuserc')
-        
-        
+
         # this does not work for pip installs
-        #~ data_dir = os.path.join(self.install_data,'share','amuse')
-        #~ if not self.root is None:
-            #~ data_dir = os.path.relpath(data_dir,self.root)
-            #~ data_dir =  os.path.join('/',data_dir)
-        #~ else:
-            #~ data_dir = os.path.abspath(data_dir)
+        # data_dir = os.path.join(self.install_data,'share','amuse')
+        # if not self.root is None:
+        #     data_dir = os.path.relpath(data_dir,self.root)
+        #     data_dir =  os.path.join('/',data_dir)
+        # else:
+        #     data_dir = os.path.abspath(data_dir)
 
         installinilines = []
         installinilines.append('[channel]')
         installinilines.append('must_check_if_worker_is_up_to_date=0')
         installinilines.append('use_python_interpreter=1')
-        #installinilines.append('worker_code_directory={0}'.format(os.path.join(data_dir, 'bin')))
+        # installinilines.append('worker_code_directory={0}'.format(os.path.join(data_dir, 'bin')))
         if sys.platform == 'win32':
             installinilines.append('worker_code_suffix=".exe"')
         installinilines.append('[data]')
-        #~ installinilines.append('input_data_root_directory={0}'.format(os.path.join(data_dir, 'data')))
+        # installinilines.append('input_data_root_directory={0}'.format(os.path.join(data_dir, 'data')))
         installinilines.append('output_data_root_directory=_amuse_output_data')
-        #~ installinilines.append('amuse_root_dir={0}'.format(data_dir))
-        
+        # installinilines.append('amuse_root_dir={0}'.format(data_dir))
+
         if 'BUILD_BINARY' in os.environ:
             installinilines.append('[test]')
             installinilines.append('can_run_tests_to_compile_modules=0')
 
         self.mkpath(os.path.join(self.build_dir, supportrc["package_name"]))
         file_util.write_file(outfilename, installinilines)
-        
-        
 
 
 class CodeCommand(Command):
     user_options = [
         ('build-lib=', 'b',
          "directory for compiled extension modules"),
         ('build-temp=', 't',
@@ -206,75 +196,73 @@
          "forcibly build everything (ignore file timestamps)"),
         ('variant', 'V',
          "build variants of the codes (gpu versions etc)"),
         ('codes-dir=', 'd', "directory containing codes"),
         ('lib-dir=', 'l', "directory containing libraries to build"),
     ]
 
-    negative_opt = {'no-inplace':'inplace'}
-    
+    negative_opt = {'no-inplace': 'inplace'}
+
     boolean_options = ['force', 'inplace', 'debug', 'variant']
 
-    def initialize_options (self):
+    def initialize_options(self):
         self.codes_dir = None
         self.lib_dir = None
         self.lib_src_dir = None
-        self.amuse_src_dir =  os.path.join('src',supportrc["package_name"])
+        self.amuse_src_dir = os.path.join('src', supportrc["package_name"])
         self.environment = {}
         self.environment_notset = {}
         self.found_cuda = False
         self.found_sapporo = False
         self.variant = True
         self.inplace = False
-        
+
         self.build_lib = None
         self.build_temp = None
         self.debug = None
         self.force = None
 
-
-        
-    def finalize_options (self):
+    def finalize_options(self):
         self.set_undefined_options(
             'build',
-           ('build_lib', 'build_lib'),
-           ('build_temp', 'build_temp'),
-           ('debug', 'debug'),
-           ('force', 'force'),
+            ('build_lib', 'build_lib'),
+            ('build_temp', 'build_temp'),
+            ('debug', 'debug'),
+            ('force', 'force'),
         )
 
-        self.config=None
+        self.config = None
 
         if supportrc["framework_install"]:
             try:
                 from . import config
-                self.config=config
+                self.config = config
             except ImportError:
                 # continue
                 pass
         else:
             from amuse import config
-            self.config=config
+            self.config = config
 
         if self.codes_dir is None:
             if self.inplace:
                 self.codes_dir = os.path.join(self.amuse_src_dir,'community')
                 self.codes_src_dir = self.codes_dir
             else:
-                #~ self.codes_dir = os.path.join(self.build_temp, 'src', 'amuse', 'community')
+                # self.codes_dir = os.path.join(self.build_temp, 'src', 'amuse', 'community')
                 self.codes_dir = os.path.join(self.build_temp, 'codes')
-                self.codes_src_dir = os.path.join(self.amuse_src_dir,'community')
+                self.codes_src_dir = os.path.join(self.amuse_src_dir, 'community')
         else:
             if self.inplace:
                 self.codes_src_dir = self.codes_dir
             else:
                 self.codes_src_dir = self.codes_dir
-                #~ self.codes_dir=os.path.join(self.build_temp, 'src', 'amuse', 'community')
-                self.codes_dir=os.path.join(self.build_temp, 'codes')
-            
+                # self.codes_dir = os.path.join(self.build_temp, 'src', 'amuse', 'community')
+                self.codes_dir = os.path.join(self.build_temp, 'codes')
+
         if self.lib_dir is None:
             if self.inplace:
                 self.lib_dir = os.path.join('lib')
                 self.lib_src_dir = self.lib_dir
             else:
                 self.lib_dir = os.path.join(self.build_temp, 'lib')
                 self.lib_src_dir = os.path.join('lib')
@@ -285,151 +273,147 @@
                 self.lib_src_dir = self.codes_dir
                 self.lib_dir=os.path.join(self.build_temp, 'lib')
 
         if self.config:
             self.environment['PYTHON'] = self.config.interpreters.python
         else:
             self.environment['PYTHON'] = sys.executable
-            
+
         self.set_cuda_variables()
         self.set_mpi_variables()
         self.set_compiler_variables()
-        
-        
+
         self.set_fortran_variables()
-        
+
         if 'FORTRAN' in self.environment:
             self.environment['F90'] = self.environment['FORTRAN']
             self.environment['FC'] = self.environment['FORTRAN']
         self.set_java_variables()
         self.set_openmp_flags()
         self.set_libdir_variables()
         self.set_libs_variables()
         self.save_cfgfile_if_not_exists()
-        
+
         if 'MSYSCON' in os.environ:
             pass
         else:
             if not supportrc["framework_install"]:
                 try:
                     from amuse.support import get_amuse_root_dir
                 except ImportError:
                     raise Exception("AMUSE framework needs to be installed and environment set up.")
                 self.environment['AMUSE_DIR'] = get_amuse_root_dir()
             else:
                 if self.inplace:
-                   self.environment['AMUSE_DIR'] = os.path.abspath(os.getcwd())
+                    self.environment['AMUSE_DIR'] = os.path.abspath(os.getcwd())
                 else:
-                   self.environment['AMUSE_DIR'] = os.path.abspath(self.build_temp)
+                    self.environment['AMUSE_DIR'] = os.path.abspath(self.build_temp)
 
             if self.inplace:
-               self.environment['MUSE_PACKAGE_DIR'] = os.path.abspath(os.getcwd())
+                self.environment['MUSE_PACKAGE_DIR'] = os.path.abspath(os.getcwd())
             else:
-               self.environment['MUSE_PACKAGE_DIR'] = os.path.abspath(self.build_temp)
+                self.environment['MUSE_PACKAGE_DIR'] = os.path.abspath(self.build_temp)
 
     
     def set_fortran_variables(self):
         if 'FORTRAN' in self.environment:
             return
-            
+
         if 'FORTRAN' in os.environ:
             self.environment['FORTRAN'] = os.environ['FORTRAN']
             return
-            
+
         if self.config:
             self.environment['FORTRAN'] = self.config.compilers.fc
             return
-        
+
         if 'FC' in os.environ:
             self.environment['FORTRAN'] = os.environ['FC']
             return
-            
+
         if 'FORT' in os.environ:
             self.environment['FORTRAN'] = os.environ['FORT']
             return
-            
+
         if 'F90' in os.environ:
             self.environment['FORTRAN'] = os.environ['F90']
             return
-            
+
         mpif90 = os.environ['MPIF90'] if 'MPIF90' in os.environ else 'mpif90'
-        
+
         try:
-            process = Popen([mpif90,'-show'], stdout = PIPE, stderr = PIPE)
+            process = Popen([mpif90, '-show'], stdout=PIPE, stderr=PIPE)
             stdoutstring, stderrstring = process.communicate()
             if process.returncode == 0:
                 parts = stdoutstring.split()
-                self.environment['FORTRAN']  = parts[0]
+                self.environment['FORTRAN'] = parts[0]
                 return
-            
-            process = Popen([mpif90,'--showme '], stdout = PIPE, stderr = PIPE)
+
+            process = Popen([mpif90, '--showme '], stdout=PIPE, stderr=PIPE)
             stdoutstring, stderrstring = process.communicate()
             if process.returncode == 0:
                 parts = stdoutstring.split()
-                self.environment['FORTRAN']  = parts[0]
-                return  
+                self.environment['FORTRAN'] = parts[0]
+                return
         except:
             pass
-            
-        
-        if fcompiler:    
+
+        if fcompiler:
             compiler = fcompiler.new_fcompiler(requiref90=True)
             if compiler is not None:
                 fortran_executable = compiler.executables['compiler_f90'][0]
                 self.environment['FORTRAN'] = fortran_executable
-    
-    
-    
+
     def is_mpi_enabled(self):
         if self.config and hasattr(self.config.mpi, 'is_enabled'):
             return self.config.mpi.is_enabled
         else:
             return True
-    
+
     def set_cuda_variables(self):
         all_found = True
         if self.config and self.config.cuda.is_enabled:
             self.found_cuda = True
             self.environment['CUDA_LIBDIRS'] = '-L'+self.config.cuda.toolkit_path+'/lib' + ' -L'+self.config.cuda.toolkit_path+'/lib64'
             self.environment['CUDA_TK'] = self.config.cuda.toolkit_path
             self.environment['CUDA_SDK'] = self.config.cuda.sdk_path
             if hasattr(self.config.cuda, 'cuda_libs'):
                 self.environment['CUDA_LIBS'] = self.config.cuda.cuda_libs
             else:
                 raise DistutilsError("configuration is not up to date for cuda, please reconfigure amuse by running 'configure --enable-cuda'")
-               
+
             return
-            
+
         if self.config and not self.config.cuda.is_enabled:
             self.found_cuda = True
             self.environment['CUDA_LIBDIRS'] = '-L/NOCUDACONFIGURED/lib' + ' -LNOCUDACONFIGURED/lib64'
             self.environment['CUDA_LIBS'] = '-lnocuda'
             self.environment['CUDART_LIBS'] = '-lnocudart'
             self.environment['CUDA_TK'] = '/NOCUDACONFIGURED'
             self.environment['CUDA_SDK'] = '/NOCUDACONFIGURED'
             return 
 
         for x in ['CUDA_TK', 'CUDA_SDK']:
             if not x in self.environment:
                 all_found = False
                 break
-        
+
         if all_found:
             cuda_dir = self.environment['CUDA_TK']
-            self.environment['CUDA_LIBDIRS'] = '-L'+cuda_dir+'/lib' +  ' -L'+cuda_dir+'/lib64'
+            self.environment['CUDA_LIBDIRS'] = '-L'+cuda_dir+'/lib' + ' -L'+cuda_dir+'/lib64'
             self.environment['CUDA_LIBS'] = '-lcudart'
             return
-            
-        dir = spawn.find_executable('nvcc')
-        if dir is None:
+
+        directory = spawn.find_executable('nvcc')
+        if directory is None:
             self.found_cuda = False
             self.environment_notset['CUDA_SDK'] = '<directory>'
             self.environment_notset['CUDA_TK'] = '<directory>'
             return
-        cuda_dir = os.path.dirname(os.path.dirname(dir))
+        cuda_dir = os.path.dirname(os.path.dirname(directory))
         self.environment['CUDA_LIBDIRS'] = '-L'+cuda_dir+'/lib' + ' -L'+cuda_dir+'/lib64'
         self.environment['CUDA_LIBS'] = '-lcudart'
         self.environment['CUDA_TK'] = cuda_dir
         if not 'CUDA_SDK' in self.environment:
             self.environment_notset['CUDA_SDK'] = '<directory>'
         
         self.found_cuda = True
@@ -437,36 +421,34 @@
     def set_mpi_variables(self):
         if self.config:
             self.environment['MPICXX'] = self.config.mpi.mpicxx
             self.environment['MPICC'] = self.config.mpi.mpicc
             self.environment['MPIF90'] = self.config.mpi.mpif95
             return
 
-    
     def set_compiler_variables(self):
         if self.config and not hasattr(self.config.compilers, 'found_fftw'):
             raise DistutilsError("configuration is not up to date, please reconfigure amuse by running 'configure'")
-            
+
         if self.config:
             self.environment['CXX'] = self.config.compilers.cxx
             self.environment['CC'] = self.config.compilers.cc
             self.environment['FC'] = self.config.compilers.fc
             self.environment['CFLAGS'] = self.config.compilers.cc_flags
             self.environment['CXXFLAGS'] = self.config.compilers.cxx_flags
             self.environment['FFLAGS'] = self.config.compilers.fc_flags
-            
+
             if self.config.compilers.found_fftw == 'yes':
                 self.environment['FFTW_FLAGS'] = self.config.compilers.fftw_flags
                 self.environment['FFTW_LIBS'] = self.config.compilers.fftw_libs
-            
-            
+
             if self.config.compilers.found_gsl == 'yes':
                 self.environment['GSL_FLAGS'] = self.config.compilers.gsl_flags
                 self.environment['GSL_LIBS'] = self.config.compilers.gsl_libs
-                
+
             return
 
     def set_java_variables(self):
         if self.config and hasattr(self.config, 'java') and hasattr(self.config.java, 'is_enabled') and self.config.java.is_enabled:
             self.environment['JAVA'] = self.config.java.java
             self.environment['JAVAC'] = self.config.java.javac
             self.environment['JAR'] = self.config.java.jar
@@ -479,25 +461,25 @@
     def set_openmp_flags(self):
         if self.config and hasattr(self.config, 'openmp'):
             self.environment['OPENMP_FCFLAGS'] = self.config.openmp.fcflags
             self.environment['OPENMP_CFLAGS'] = self.config.openmp.cflags
         else:
             self.environment['OPENMP_FCFLAGS'] = ''
             self.environment['OPENMP_CFLAGS'] = ''
-            
+
     def set_libdir_variables(self):
         for varname in ('SAPPORO_LIBDIRS', 'GRAPE6_LIBDIRS'):
             if varname in self.environment:
                 continue
-                
+
             if varname in os.environ:
                 self.environment[varname] = os.environ[varname]
             else:
-                self.environment_notset[varname] ='-L<directory>'
-        
+                self.environment_notset[varname] = '-L<directory>'
+
         if 'SAPPORO_LIBDIRS' in self.environment:
             self.environment['SAPPORO_LIBS'] = '-L{0} -lsapporo'.format(
                 self.environment['SAPPORO_LIBDIRS']
             )
         else:
             if self.config and hasattr(self.config.cuda, 'sapporo_version'):
                 if self.config.cuda.sapporo_version == '2':
@@ -510,170 +492,166 @@
                         os.path.abspath(os.getcwd())
                     )
             else:
                 self.environment['SAPPORO_LIBS'] = '-L{0}/lib/sapporo_light -lsapporo'.format(
                     os.path.abspath(os.getcwd())
                 )
             self.environment['BOOSTLIBS'] = ''
-     
+
     def set_libs_variables(self):
         for varname, libname in []:
             if varname in self.environment:
                 continue
-                
+
             if varname in os.environ:
                 self.environment[varname] = os.environ[varname]
             else:
                 self.environment_notset[varname] ='-L<directory> -l{0}'.format(libname)
 
     def copy_config_to_build_dir(self):
-        configpath=os.path.abspath(os.getcwd())
+        configpath = os.path.abspath(os.getcwd())
         if self.inplace:
-            topath=self.amuse_src_dir
+            topath = self.amuse_src_dir
         else:
-            topath=os.path.join(self.build_lib, "amuse")
-        self.copy_file(os.path.join(configpath,"config.mk"), topath) 
-     
+            topath = os.path.join(self.build_lib, "amuse")
+        self.copy_file(os.path.join(configpath, "config.mk"), topath)
+
     def copy_build_prereq_to_build_dir(self):
         if not os.path.exists(self.build_temp):
             self.mkpath(self.build_temp)
 
         if supportrc["framework_install"]:
-            configpath=os.path.abspath(os.getcwd())
-            self.copy_file(os.path.join(configpath,"config.mk"), self.build_temp) 
-        #~ self.copy_tree(os.path.join(configpath,"support"), os.path.join(self.build_temp,"support") )
-        #~ self.copy_tree(os.path.join(configpath,"src"), os.path.join(self.build_temp,"src") )
-        path=os.path.join(self.build_temp,"src")
+            configpath = os.path.abspath(os.getcwd())
+            self.copy_file(os.path.join(configpath, "config.mk"), self.build_temp)
+        # self.copy_tree(os.path.join(configpath,"support"), os.path.join(self.build_temp,"support") )
+        # self.copy_tree(os.path.join(configpath,"src"), os.path.join(self.build_temp,"src") )
+        path = os.path.join(self.build_temp, "src")
         if not os.path.exists(path) and not os.path.islink(path):
-            os.symlink(os.path.relpath(self.build_lib,self.build_temp), path)
-        
+            os.symlink(os.path.relpath(self.build_lib, self.build_temp), path)
+
     def copy_codes_to_build_dir(self):
 
-        for dir in self.makefile_paths(self.codes_src_dir):
-            reldir = os.path.relpath(dir, self.codes_src_dir)
+        for directory in self.makefile_paths(self.codes_src_dir):
+            reldir = os.path.relpath(directory, self.codes_src_dir)
             self.copy_tree(
-                dir, 
+                directory,
                 os.path.join(self.codes_dir, reldir)
             )
-        
+
     def copy_lib_to_build_dir(self):
-        for dir in self.makefile_paths(self.lib_src_dir):
-            reldir = os.path.relpath(dir, self.lib_src_dir)
+        for directory in self.makefile_paths(self.lib_src_dir):
+            reldir = os.path.relpath(directory, self.lib_src_dir)
             self.copy_tree(
-                dir, 
+                directory,
                 os.path.join(self.lib_dir, reldir)
             )
 
-
     def copy_worker_codes_to_build_dir(self):
         if sys.platform == 'win32':
             worker_code_re = re.compile(r'(([a-zA-Z0-9]+_)*)?worker(_[a-zA-Z0-9]+)?(.exe)?')
         else:
             worker_code_re = re.compile(r'(([a-zA-Z0-9]+_)*)?worker(_[a-zA-Z0-9]+)?')
         worker_so_re = re.compile(r'(([a-zA-Z0-9]+_)*)?cython(_[a-zA-Z0-9]+)?.so')
-            
-        
+
         lib_binbuilddir = os.path.join(self.build_lib, supportrc["package_name"], '_workers')
         if not os.path.exists(lib_binbuilddir):
             self.mkpath(lib_binbuilddir)
-            
+
         for srcdir in self.makefile_paths(self.codes_src_dir):
             reldir = os.path.relpath(srcdir, self.codes_src_dir)
             temp_builddir = os.path.join(self.codes_dir, reldir)
-            
-            self.announce("will copy worker: {0}".format(srcdir), level = log.INFO)
+
+            self.announce("will copy worker: {0}".format(srcdir), level=logging.INFO)
             lib_builddir = os.path.join(self.build_lib, os.path.relpath(srcdir, os.path.join(self.amuse_src_dir, '..')))
-            
-            
+
             shortname = reldir.lower()
-            self.announce(shortname, level = log.INFO)
-            
+            self.announce(shortname, level=logging.INFO)
+
             for name in os.listdir(temp_builddir):
                 path = os.path.join(temp_builddir, name)
                 stat = os.stat(path)
-                
+
                 if os.path.isfile(path):
                     if worker_so_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                         continue
 
-
-                #self.announce("will copy worker: {0}".format(name), level = log.INFO)
+                # self.announce("will copy worker: {0}".format(name), level = logging.INFO)
                 if os.path.isfile(path) and os.access(path, os.X_OK):
                     if worker_code_re.match(name):
                         topath = os.path.join(lib_binbuilddir, name)
                         self.copy_file(path, topath)
                     elif not name.endswith('.py'):
-                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level = log.WARN)
+                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=logging.WARN)
             
             # also copy file or dir named data
-            path=os.path.join(temp_builddir,'data')
+            path = os.path.join(temp_builddir, 'data')
             topath = os.path.join(lib_builddir, 'data')
             if os.path.isfile(path):
-                self.copy_file(path, topath)                
+                self.copy_file(path, topath)
             if os.path.isdir(path):
-                self.copy_tree(path, topath)                
+                self.copy_tree(path, topath)
 
     def copy_worker_codes(self):
         if sys.platform == 'win32':
             worker_code_re = re.compile(r'(([a-zA-Z0-9]+_)*)?worker(_[a-zA-Z0-9]+)?(.exe)?')
         else:
             worker_code_re = re.compile(r'(([a-zA-Z0-9]+_)*)?worker(_[a-zA-Z0-9]+)?')
         worker_so_re = re.compile(r'(([a-zA-Z0-9]+_)*)?cython(_[a-zA-Z0-9]+)?.so')
-            
+
         for srcdir in self.makefile_paths(self.codes_src_dir):
             reldir = os.path.relpath(srcdir, self.codes_src_dir)
             temp_builddir = os.path.join(self.codes_dir, reldir)
-            
-            self.announce("will copy worker: {0}".format(srcdir), level = log.INFO)
+
+            self.announce("will copy worker: {0}".format(srcdir), level=logging.INFO)
             lib_builddir = os.path.join(self.build_lib, os.path.relpath(srcdir, os.path.join(self.amuse_src_dir, '..')))
 
             shortname = reldir.lower()
-            self.announce(shortname, level = log.INFO)
+            self.announce(shortname, level=logging.INFO)
 
             for name in os.listdir(temp_builddir):
                 path = os.path.join(temp_builddir, name)
                 stat = os.stat(path)
-                
+
                 if os.path.isfile(path):
                     if worker_so_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                         continue
 
                 if os.path.isfile(path) and os.access(path, os.X_OK):
                     if worker_code_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                     elif not name.endswith('.py'):
-                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level = log.WARN)
+                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=logging.WARN)
             
             # also copy file or dir named data
-            path=os.path.join(temp_builddir,'data')
+            path = os.path.join(temp_builddir, 'data')
             topath = os.path.join(lib_builddir, 'data')
             if os.path.isfile(path):
-                self.copy_file(path, topath)                
+                self.copy_file(path, topath)
             if os.path.isdir(path):
                 self.copy_tree(path, topath)
-                                    
-    def subdirs_in_path(self,path):
+
+    def subdirs_in_path(self, path):
         if not os.path.exists(path):
             return
 
         names = sorted(os.listdir(path))
         for name in names:
             if name.startswith('.'):
                 continue
-                
+
             path_ = os.path.join(path, name)
             if os.path.isdir(path_):
                 yield path_
 
-    def makefile_paths(self,path):
+    def makefile_paths(self, path):
         for x in self.subdirs_in_path(path):
             for name in ('makefile', 'Makefile'):
                 makefile_path = os.path.join(x, name)
                 if os.path.exists(makefile_path):
                     yield x
                     break
 
@@ -683,419 +661,441 @@
             config.read(['amuse.cfg'])
             for name, value in config.items('environment'):
                 if isinstance(value, str) and value:
                     varname = name.upper()
                     self.environment[varname] = value
                     if varname in self.environment_notset:
                         del self.environment_notset[varname]
-                        
+
     def save_cfgfile_if_not_exists(self):
         if not os.path.exists('amuse.cfg'):
             config = configparser.RawConfigParser()
             config.add_section('environment')
             for name, value in self.environment.items():
                 config.set('environment', name, value)
-                
+
             for name, value in self.environment_notset.items():
                 config.set('environment', name, '')
-            
+
             with open('amuse.cfg', 'w') as f:
                 config.write(f)
 
-    
-    
-        
     def get_special_targets(self, name, directory, environment):
-        process = Popen(['make','-qp', '-C', directory], env = environment, stdout = PIPE, stderr = PIPE)
+        process = Popen(['make', '-qp', '-C', directory], env=environment, stdout=PIPE, stderr=PIPE)
         stdoutstring, stderrstring = process.communicate()
         stdoutstring = str(stdoutstring, 'utf-8')
         lines = stdoutstring.splitlines()
         result = []
         for line in lines:
             if line.startswith('muse_worker_gpu:'):
                 result.append(('muse_worker_gpu', 'GPU',))
             elif line.startswith('muse_worker_grape:'):
                 result.append(('muse_worker_grape', 'GRAPE6',))
             elif line.startswith('muse_worker_'):
                 index_of_the_colon = line.index(':')
                 if(index_of_the_colon > 0):
                     targetname = line[len('muse_worker_'):index_of_the_colon]
-                    if '%' not in targetname: result.append((line[:index_of_the_colon], targetname,))
+                    if '%' not in targetname:
+                        result.append((line[:index_of_the_colon], targetname,))
             elif line.startswith('worker_code_'):
                 index_of_the_colon = line.index(':')
                 if(index_of_the_colon > 0):
                     targetname = line[len('worker_code_'):index_of_the_colon]
-                    if '%' not in targetname: result.append((line[:index_of_the_colon], targetname,))
+                    if '%' not in targetname:
+                        result.append((line[:index_of_the_colon], targetname,))
             elif line.startswith(name + '_worker_'):
                 index_of_the_colon = line.index(':')
                 if(index_of_the_colon > 0):
                     targetname = line[len(name + '_worker_'):index_of_the_colon]
-                    if '%' not in targetname: result.append((line[:index_of_the_colon], targetname,))
-        
-        result=list(set(result))
-                    
+                    if '%' not in targetname:
+                        result.append((line[:index_of_the_colon], targetname,))
+
+        result = list(set(result))
+
         return result
-    
-    def call(self, arguments, buildlogfile = None, **keyword_arguments):
+
+    def call(self, arguments, buildlogfile=None, **keyword_arguments):
         stringio = []
-         
-        self.announce(' '.join(arguments), log.DEBUG)
-        
+
+        self.announce(' '.join(arguments), logging.DEBUG)
+
         process = Popen(
-            arguments, 
-            stdout = PIPE,
-            stderr = STDOUT,
+            arguments,
+            stdout=PIPE,
+            stderr=STDOUT,
             **keyword_arguments
         )
-        
+
         while True:
             line = process.stdout.readline()
             if len(line) == 0:
                 break
-            
-            if not buildlogfile is None:
+
+            if buildlogfile is not None:
                 buildlogfile.write(line)
-            self.announce(line[:-1].decode("utf-8"), log.DEBUG)
+            self.announce(line[:-1].decode("utf-8"), logging.DEBUG)
             stringio.append(str(line, 'utf-8'))
-            
+
         result = process.wait()
         content = ''.join(stringio)
-        
-        if result!=0:
-            self.announce("error in call, tail output:\n", log.INFO)
-            self.announce(''.join(stringio[-100:]), log.INFO)
-            self.announce("-"*80, log.INFO)
+
+        if result != 0:
+            self.announce("error in call, tail output:\n", logging.INFO)
+            self.announce(''.join(stringio[-100:]), logging.INFO)
+            self.announce("-"*80, logging.INFO)
 
         return result, content
-        
+
     def build_environment(self):
-        environment=self.environment.copy()
+        environment = self.environment.copy()
         environment.update(os.environ)
-        path=os.path.join(environment["MUSE_PACKAGE_DIR"],"src")
-        if environment["MUSE_PACKAGE_DIR"]!=environment["AMUSE_DIR"]:
-            path=path+":"+os.path.join(environment["AMUSE_DIR"],"src")
-        path=path+':'+environment.get("PYTHONPATH", "")
-        environment["PYTHONPATH"]=path
+        path = os.path.join(environment["MUSE_PACKAGE_DIR"], "src")
+        if environment["MUSE_PACKAGE_DIR"] != environment["AMUSE_DIR"]:
+            path = path+":"+os.path.join(environment["AMUSE_DIR"], "src")
+        path = path+':'+environment.get("PYTHONPATH", "")
+        environment["PYTHONPATH"] = path
         return environment
 
-
     def do_clean(self):
-        environment = self.build_environment()        
+        environment = self.build_environment()
 
         for x in self.makefile_paths(self.lib_dir):
             self.announce("cleaning libary " + x)
-            self.call(['make','-C', x, 'clean'], env=environment)
-           
+            self.call(['make', '-C', x, 'clean'], env=environment)
+
         for x in self.makefile_paths(self.codes_dir):
             if os.path.exists(x):
                 self.announce("cleaning " + x)
-                self.call(['make','-C', x, 'clean'], env=environment)
+                self.call(['make', '-C', x, 'clean'], env=environment)
 
     def do_distclean(self):
-        environment = self.build_environment()        
+        environment = self.build_environment()
 
         for x in self.makefile_paths(self.lib_dir):
             self.announce("cleaning libary:" + x)
-            self.call(['make','-C', x, 'distclean'], env=environment)
-            
+            self.call(['make', '-C', x, 'distclean'], env=environment)
+
         for x in self.makefile_paths(self.codes_dir):
             self.announce("cleaning community code:" + x)
-            self.call(['make','-C', x, 'distclean'], env=environment)
+            self.call(['make', '-C', x, 'distclean'], env=environment)
 
 
-    
-class SplitOutput(object) :
-    def __init__(self, file1, file2) :
+class SplitOutput(object):
+    def __init__(self, file1, file2):
         self.file1 = file1
         self.file2 = file2
 
-    def __del__(self) :
+    def __del__(self):
         self.close()
 
     def close(self):
         self.file1.close()
         self.file2.close()
 
-    def write(self, text) :
+    def write(self, text):
         self.file1.write(text)
         self.file2.write(text)
 
-    def flush(self) :
+    def flush(self):
         self.file1.flush()
         self.file2.flush()
-    
-        
+
+
 class BuildCodes(CodeCommand):
 
     description = "build interfaces to codes"
 
     user_options = list(CodeCommand.user_options)
-    user_options.append( ('clean=', 'c', "clean code",), )
+    user_options.append(('clean=', 'c', "clean code",), )
 
     def initialize_options(self):
         CodeCommand.initialize_options(self)
         self.clean = 'no'
-        
-    def finalize_options (self):
+
+    def finalize_options(self):
         CodeCommand.finalize_options(self)
         self.must_clean = self.clean == 'yes'
         self.must_dist_clean = self.clean == 'dist'
-    
+
     def run_make_on_directory(self, codename, directory, target, environment):
         buildlog = os.path.abspath("build.log")
-        
+
         with open(buildlog, "a") as output:
             output.write('*'*100)
             output.write('\n')
             output.write('Building code: {0}, target: {1}, in directory: {2}\n'.format(codename, target, directory))
             output.write('*'*100)
             output.write('\n')
             output.flush()
-        
+
         if environment.get('AMUSE_USE_CCACHE', 0) != "1" or "CCACHE_BASEDIR" in environment:
             build_environment = environment
         else:
             build_environment = deepcopy(environment)
             build_environment["CCACHE_BASEDIR"] = abspath(directory)
 
         with open(buildlog, "ab") as output:
             result, resultcontent = self.call(
-                ['make','-C', directory, target], 
+                ['make', '-C', directory, target], 
                 output,
-                env = build_environment
+                env=build_environment
             )
-        
+
         with open(buildlog, "a") as output:
             output.write('*'*100)
             output.write('\n')
-            
+
         return result, resultcontent
-    
+
     def is_download_needed(self, string):
         for line in string.splitlines():
             if 'DOWNLOAD_CODES' in line:
                 return True
         return False
-        
+
     def is_cuda_needed(self, string):
         for line in string.splitlines():
             if 'CUDA_TK variable is not set' in line:
                 return True
             if 'CUDA_SDK variable is not set' in line:
                 return True
         return False
-        
+
     def are_python_imports_needed(self, string):
         for line in string.splitlines():
             if 'Python imports not available' in line:
                 return True
         return False
-    
-    def run (self):      
+
+    def run(self):
         if self.must_clean:
             self.do_clean()
         if self.must_dist_clean:
             self.do_distclean()
 
         not_build = list()
         is_download_needed = list()
         is_cuda_needed = list()
         not_build_special = {}
         are_python_imports_needed = list()
         build = list()
         lib_build = list()
         lib_not_build = list()
         environment = self.build_environment()
-        
+
         buildlog = 'build.log'
-        
-        self.announce("building libraries and community codes", level = log.INFO)
-        self.announce("build, for logging, see '{0}'".format(buildlog), level = log.INFO)
-                
+
+        self.announce("building libraries and community codes", level=logging.INFO)
+        self.announce("build, for logging, see '{0}'".format(buildlog), level=logging.INFO)
+
         with open(buildlog, "w") as output:
             output.write('*'*100)
             output.write('\n')
             output.write('Building libraries and codes\n')
             output.write('*'*100)
             output.write('\n')
-        
+
         if not self.lib_dir == self.lib_src_dir:
             self.copy_build_prereq_to_build_dir()
             self.copy_lib_to_build_dir()
-                          
+
         for x in self.makefile_paths(self.lib_dir):
-            
+
             shortname = x[len(self.lib_dir) + 1:] + '-library'
             starttime = datetime.datetime.now()
-            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level =  log.INFO)
+            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=logging.INFO)
             returncode, outputlog = self.run_make_on_directory(shortname, x, 'all', environment)
-            
+
             endtime = datetime.datetime.now()
             if returncode == 2:
-                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level =  log.DEBUG)
+                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level=logging.DEBUG)
                 if self.is_download_needed(outputlog):
                     is_download_needed.append(x[len(self.lib_dir) + 1:])
                 elif self.is_cuda_needed(outputlog):
                     is_cuda_needed.append(x[len(self.lib_dir) + 1:])
                 else:
                     lib_not_build.append(shortname)
             else:
-                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level =  log.DEBUG)
+                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level=logging.DEBUG)
                 lib_build.append(shortname)
-            
+
         if not self.codes_dir == self.codes_src_dir:
             self.copy_codes_to_build_dir()
-        
-        #environment.update(self.environment)
+
+        # environment.update(self.environment)
         makefile_paths = list(self.makefile_paths(self.codes_dir))
 
         build_to_special_targets = {}
-        
+
         for x in makefile_paths:
             shortname = x[len(self.codes_dir) + 1:].lower()
             starttime = datetime.datetime.now()
             # For binary builds we do not want
             # to distribute mesa, it will make the
-            # download size from about 100mb size 
+            # download size from about 100mb size
             # to > 1Gb size.
             #
             # Could we remove some of the data files from mesa?
             #
             if not self.inplace and shortname == 'mesa':
-                self.announce("[{1:%H:%M:%S}] skipping {0}".format(shortname, starttime), level =  log.INFO)
-                continue 
-                
-            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level =  log.INFO)
+                self.announce("[{1:%H:%M:%S}] skipping {0}".format(shortname, starttime), level=logging.INFO)
+                continue
+
+            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=logging.INFO)
             returncode, outputlog = self.run_make_on_directory(shortname, x, 'all', environment)
             endtime = datetime.datetime.now()
             if returncode > 0:
-                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level =  log.DEBUG)
+                self.announce(
+                    "[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime),
+                    level=logging.DEBUG
+                )
                 if self.is_download_needed(outputlog):
                     is_download_needed.append(shortname)
                 elif self.is_cuda_needed(outputlog):
                     is_cuda_needed.append(shortname)
                 elif self.are_python_imports_needed(outputlog):
                     are_python_imports_needed.append(shortname)
                 else:
                     not_build.append(shortname)
-                    
+
                 if self.is_mpi_enabled():
                     continue
             else:
                 build.append(shortname)
                 is_built = True
-                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level =  log.DEBUG)
-            
+                self.announce(
+                    "[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime),
+                    level=logging.DEBUG
+                )
+
             if not self.variant:
                 continue
-                
+
             special_targets = self.get_special_targets(shortname, x, environment)
-            for target,target_name in special_targets:
+            for target, target_name in special_targets:
                 starttime = datetime.datetime.now()
-                self.announce("[{2:%H:%M:%S}] building {0} - {1}".format(shortname, target_name, starttime), level =  log.DEBUG)
+                self.announce(
+                    "[{2:%H:%M:%S}] building {0} - {1}".format(shortname, target_name, starttime),
+                    level=logging.DEBUG
+                )
                 returncode, outputlog = self.run_make_on_directory(shortname, x, target, environment)
                 endtime = datetime.datetime.now()
                 if returncode > 0:
                     specials_list = not_build_special.setdefault(shortname,[])
                     specials_list.append(target_name)
-                    self.announce("[{3:%H:%M:%S}] building {0} - {1}, failed, see {2!r} for error log".format(shortname, target_name, buildlog,endtime), level =  log.DEBUG)
+                    self.announce(
+                        "[{3:%H:%M:%S}] building {0} - {1}, failed, see {2!r} for error log".format(shortname, target_name, buildlog, endtime),
+                        level=logging.DEBUG
+                    )
                 else:
                     build_to_special_targets.setdefault(shortname, list()).append(target_name)
-                    self.announce("[{2:%H:%M:%S}] building {0} - {1}, succeeded".format(shortname, target_name, endtime), level =  log.DEBUG)
-                
-        #~ if supportrc["framework_install"]:
-            #~ self.copy_config_to_build_dir()
-        
+                    self.announce(
+                        "[{2:%H:%M:%S}] building {0} - {1}, succeeded".format(shortname, target_name, endtime), level=logging.DEBUG
+                    )
+
+        # if supportrc["framework_install"]:
+        #     self.copy_config_to_build_dir()
+
         if not self.codes_dir == self.codes_src_dir:
-            #~ self.copy_worker_codes_to_build_dir()
+            # self.copy_worker_codes_to_build_dir()
             self.copy_worker_codes()
-            
+
         with open(buildlog, "a") as output:
             output.write('*'*80)
             output.write('\n')
             output.write('Building finished\n')
             output.write('*'*80)
             output.write('\n')
-            
+
         self.announce("Environment variables")
         self.announce("="*80)
         sorted_keys = sorted(self.environment.keys())
         for x in sorted_keys:
-            self.announce("%s\t%s" % (x , self.environment[x] ))
-        
+            self.announce("%s\t%s" % (x, self.environment[x]))
+
         if not self.is_mpi_enabled():
             all_build = set(build)
             not_build_copy = []
             for x in not_build:
                 if x in build_to_special_targets:
-                    if not x in all_build:
+                    if x not in all_build:
                         build.append(x)
                         all_build.add(x)
                 else:
                     not_build_copy.append(x)
             not_build = not_build_copy
-                
-        
-        if not_build or not_build_special or is_download_needed or is_cuda_needed or are_python_imports_needed:
+
+        if (
+            not_build
+            or not_build_special
+            or is_download_needed
+            or is_cuda_needed
+            or are_python_imports_needed
+        ):
             if not_build:
-                level = log.WARN
+                level = logging.WARN
             else:
-                level = log.INFO
+                level = logging.INFO
             if not_build:
-                self.announce("Community codes not built (because of errors/ missing libraries):",  level = level)
-                self.announce("="*80,  level = level)
+                self.announce(
+                    "Community codes not built (because of errors/ missing libraries):",
+                    level=level
+                )
+                self.announce("="*80,  level=level)
                 for x in not_build:
-                    self.announce(' * {0}'.format(x), level =  level)
+                    self.announce(' * {0}'.format(x), level=level)
             if not_build_special:
-                self.announce("Optional builds skipped, need special libraries:",  level = level)
+                self.announce("Optional builds skipped, need special libraries:", level=level)
                 for x in sorted(not_build_special.keys()):
-                    self.announce(' * {0} - {1}'.format(x, ', '.join(not_build_special[x])), level = level)
+                    self.announce(' * {0} - {1}'.format(x, ', '.join(not_build_special[x])), level=level)
             if is_cuda_needed:
-                self.announce("Optional builds skipped, need CUDA/GPU libraries:",  level = level)
+                self.announce("Optional builds skipped, need CUDA/GPU libraries:", level=level)
                 for x in is_cuda_needed:
-                    self.announce(' * {0}'.format(x), level = level)
+                    self.announce(' * {0}'.format(x), level=level)
             if are_python_imports_needed:
-                self.announce("Optional builds skipped, need additional python packages:",  level = level)
+                self.announce("Optional builds skipped, need additional python packages:", level=level)
                 for x in are_python_imports_needed:
-                    self.announce(' * {0}'.format(x), level = level)
+                    self.announce(' * {0}'.format(x), level=level)
             if is_download_needed:
-                self.announce("Optional builds skipped, need separate download",  level = level)
+                self.announce("Optional builds skipped, need separate download", level=level)
                 for x in is_download_needed:
-                    self.announce(' * {0} , make {0}.code DOWNLOAD_CODES=1'.format(x), level = level)
+                    self.announce(
+                        f' * {x} , make {x}.code DOWNLOAD_CODES=1', level=level
+                    )
+
+            self.announce("="*80,  level=level)
 
-            self.announce("="*80,  level = level)
-        
         if build:
-            level = log.INFO
-            self.announce("Community codes built",  level = level)
-            self.announce("="*80,  level = level)
+            level = logging.INFO
+            self.announce("Community codes built",  level=level)
+            self.announce("="*80,  level=level)
             for x in build:
                 if x in build_to_special_targets:
                     y = build_to_special_targets[x]
-                    self.announce('* {0} ({1})'.format(x,','.join(y)),  level = level)
+                    self.announce('* {0} ({1})'.format(x, ','.join(y)), level=level)
                 else:
-                    self.announce('* {0}'.format(x),  level = level)
-            self.announce("="*80,  level = level)
-        
-        level = log.INFO
+                    self.announce('* {0}'.format(x),  level=level)
+            self.announce("="*80,  level=level)
+
+        level = logging.INFO
         self.announce(
             "{0} out of {1} codes built, {2} out of {3} libraries built".format(
                 len(build), 
                 len(build) + len(not_build), 
                 len(lib_build), 
                 len(lib_build) + len(lib_not_build)
             ),  
-            level = level
+            level=level
         )
         self.announce("(not all codes and libraries need to be built)")
         
         if self.config and (not hasattr(self.config, 'java') or not hasattr(self.config.java, 'is_enabled')):
             self.announce(
                 "Your configuration is out of date, please rerun configure",
-                level = level
+                level=level
             )
 
         allow_build_failures=environment.get("AMUSE_ALLOW_BUILD_FAILURES", supportrc["allow_build_failures"])
 
         if allow_build_failures=="none" and len(not_build)>0:
             raise Exception("Unexpected build failure(s) detected. Aborting.")
         if allow_build_failures=="some" and len(not_build)>0 and len(build)==0:
@@ -1137,132 +1137,130 @@
 
 class BuildCodes_inplace(BuildCodes):
 
     description = "build interfaces to codes, in place"
 
     def initialize_options(self):
         BuildCodes.initialize_options(self)
-        self.inplace=True
+        self.inplace = True
 
 
 class ConfigureCodes(CodeCommand):
 
     description = "run configure for amuse"
 
-    def run (self):
-
+    def run(self):
         if os.path.exists('config.mk') or self.config:
-            self.announce("Already configured, not running configure", level = 2)
+            self.announce("Already configured, not running configure", level=2)
             return
         environment = self.build_environment()
-        self.announce("Running configure for AMUSE", level = 2)
+        self.announce("Running configure for AMUSE", level=2)
         result,content=self.call(['./configure'], env=environment, shell=True)
         if not os.path.exists('config.mk'):
             self.announce("config.mk not generated; output of configure:", level=2)
             self.announce(content, level=2)
             raise Exception("configure failed")
         with open("config.mk") as infile:
             self.announce("configure generated config.mk", level=2)
             self.announce("="*80, level=2)
             for line in infile:
                 self.announce(line[:-1], level=2)
             self.announce("="*80, level=2)
 
-        
+
 class CleanCodes(CodeCommand):
 
     description = "clean build products in codes"
 
-    def run (self):
-                  
-        self.announce("Cleaning libraries and community codes", level = 2)
+    def run(self):
+        self.announce("Cleaning libraries and community codes", level=2)
         self.do_clean()
-        
- 
+
+
 class DistCleanCodes(CodeCommand):
 
     description = "clean for distribution"
 
-    def run (self):      
-      
-        self.announce("Cleaning for distribution, libraries and community codes", level = 2)
+    def run(self):
+        self.announce("Cleaning for distribution, libraries and community codes", level=2)
         self.do_distclean()
-        
-class BuildOneCode(BuildCodes):  
+
+
+class BuildOneCode(BuildCodes):
     description = "build one code"
 
     user_options = list(BuildCodes.user_options)
-    user_options.append( ('code-name=', 'n', "name of the code",), )
+    user_options.append(('code-name=', 'n', "name of the code",), )
 
     def initialize_options(self):
         BuildCodes.initialize_options(self)
         self.code_name = None
-        
-    def finalize_options (self):
+
+    def finalize_options(self):
         BuildCodes.finalize_options(self)
         if self.code_name is None:
             raise Exception("no code was specified")
 
     def subdirs_in_path(self,path):
         if not os.path.exists(path):
             return
-            
+
         names = os.listdir(path)
         for name in names:
             if name.startswith('.'):
                 continue
             if not name.lower().startswith(self.code_name.lower()):
                 continue
             path_ = os.path.join(path, name)
             if os.path.isdir(path_):
                 yield path_
 
     def run(self):
         if not self.inplace:
             self.run_command("build_py")
-        
+
         BuildCodes.run(self)
 
 class Clean(clean):
     # make sure sub_commands are independent
-    sub_commands=list(clean.sub_commands)
+    sub_commands = list(clean.sub_commands)
 
     def run(self):
         for cmd_name in self.get_sub_commands():
             self.run_command(cmd_name)
 
 class Install(install):
-    sub_commands=list(install.sub_commands)
-    
+    sub_commands = list(install.sub_commands)
+
     def run(self):
         # this ensures sub commands are run first (only run once)
         for cmd_name in self.get_sub_commands():
             self.run_command(cmd_name)
 
         install.run(self)
 
 class Develop(develop):
 
-    sub_commands=list(develop.sub_commands)
+    sub_commands = list(develop.sub_commands)
 
     def run(self):
         # this ensures sub commands are run first (only run once)
         for cmd_name in self.get_sub_commands():
             self.run_command(cmd_name)
 
         develop.run(self)
 
 class Editable_wheel(editable_wheel):
 
-    sub_commands=list(develop.sub_commands)
+    sub_commands = list(develop.sub_commands)
 
     def run(self):
-        build.sub_commands.remove( ('build_codes', None) )
-        build.sub_commands.append( ('build_libraries_in_place', None) )
-        
+        build.sub_commands.remove(('build_codes', None))
+        build.sub_commands.append(('build_libraries_in_place', None))
+
         # this ensures sub commands are run first (only run once)
         for cmd_name in self.get_sub_commands():
             self.run_command(cmd_name)
 
         editable_wheel.run(self)
 
 def setup_commands():
@@ -1273,33 +1271,31 @@
         'dist_clean': DistCleanCodes,
         'clean_python': clean,
         'clean': Clean,
         'install': Install,
         'build_libraries': BuildLibraries,
         'build_libraries_in_place': BuildLibraries_inplace,
         'install_libraries': InstallLibraries,
-        'develop' : Develop,
-        'develop_build' : BuildCodes_inplace,
-        'editable_wheel' : Editable_wheel
+        'develop': Develop,
+        'develop_build': BuildCodes_inplace,
+        'editable_wheel': Editable_wheel
     }
-    
+
     build.sub_commands.append(('build_codes', None))
     Clean.sub_commands.append(('clean_codes', None))
     Clean.sub_commands.append(('clean_python', None))
     Install.sub_commands.append(('install_libraries', None))
     Develop.sub_commands.append(('build_libraries_in_place', None))
-    
+
     if supportrc["framework_install"]:
         mapping_from_command_name_to_command_class.update(
             {
                 'configure_codes': ConfigureCodes,
                 'generate_install_ini': GenerateInstallIni,
                 'generate_main': generate_main,
             }
         )
         build.sub_commands.insert(0, ('configure_codes', None))
         Install.sub_commands.insert(0, ('generate_install_ini', None))
         Develop.sub_commands.insert(0, ('configure_codes', None))
 
-
-    
     return mapping_from_command_name_to_command_class
```

