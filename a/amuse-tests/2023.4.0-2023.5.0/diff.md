# Comparing `tmp/amuse-tests-2023.4.0.tar.gz` & `tmp/amuse-tests-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-tests-2023.4.0.tar", last modified: Tue Apr  4 14:22:43 2023, max compression
+gzip compressed data, was "amuse-tests-2023.5.0.tar", last modified: Wed May 17 10:19:52 2023, max compression
```

## Comparing `amuse-tests-2023.4.0.tar` & `amuse-tests-2023.5.0.tar`

### file list

```diff
@@ -1,225 +1,226 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:43.015311 amuse-tests-2023.4.0/
--rw-r--r--   0 rieder     (501) staff       (20)      215 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1208 2023-04-04 14:22:43.015112 amuse-tests-2023.4.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       83 2020-03-24 14:36:23.000000 amuse-tests-2023.4.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:42.940010 amuse-tests-2023.4.0/amuse_tests.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1208 2023-04-04 14:22:40.000000 amuse-tests-2023.4.0/amuse_tests.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)    10261 2023-04-04 14:22:42.000000 amuse-tests-2023.4.0/amuse_tests.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-04-04 14:22:40.000000 amuse-tests-2023.4.0/amuse_tests.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-04-04 14:22:40.000000 amuse-tests-2023.4.0/amuse_tests.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-04-04 14:22:40.000000 amuse-tests-2023.4.0/amuse_tests.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       76 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-04-04 14:22:43.015363 amuse-tests-2023.4.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1960 2021-04-23 11:09:14.000000 amuse-tests-2023.4.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:42.937833 amuse-tests-2023.4.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:42.937892 amuse-tests-2023.4.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:42.937952 amuse-tests-2023.4.0/src/amuse/test/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:42.940298 amuse-tests-2023.4.0/src/amuse/test/suite/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:26.000000 amuse-tests-2023.4.0/src/amuse/test/suite/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:42.973111 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    15226 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/gd_tests.py
--rw-r--r--   0 rieder     (501) staff       (20)        1 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/legacy_support.py
--rw-r--r--   0 rieder     (501) staff       (20)     6218 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_aarsethzare.py
--rw-r--r--   0 rieder     (501) staff       (20)    18691 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_adaptb.py
--rw-r--r--   0 rieder     (501) staff       (20)   128934 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_athena.py
--rw-r--r--   0 rieder     (501) staff       (20)    40330 2022-10-03 08:52:42.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_bhtree.py
--rw-r--r--   0 rieder     (501) staff       (20)    13290 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_bonsai.py
--rw-r--r--   0 rieder     (501) staff       (20)    13495 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_bonsai2.py
--rw-r--r--   0 rieder     (501) staff       (20)     2086 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_bridge.py
--rw-r--r--   0 rieder     (501) staff       (20)    18163 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_brutus.py
--rw-r--r--   0 rieder     (501) staff       (20)    30297 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_bse.py
--rw-r--r--   0 rieder     (501) staff       (20)    79426 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_capreole.py
--rw-r--r--   0 rieder     (501) staff       (20)     5328 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_create_dir.py
--rw-r--r--   0 rieder     (501) staff       (20)    58983 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_encounters.py
--rw-r--r--   0 rieder     (501) staff       (20)    47719 2022-11-30 13:58:15.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_evtwin.py
--rw-r--r--   0 rieder     (501) staff       (20)    20188 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_fastkick.py
--rw-r--r--   0 rieder     (501) staff       (20)    82682 2022-11-30 13:58:15.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_fi.py
--rw-r--r--   0 rieder     (501) staff       (20)    76139 2022-11-30 13:58:15.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_gadget2.py
--rw-r--r--   0 rieder     (501) staff       (20)    19758 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_galactics.py
--rw-r--r--   0 rieder     (501) staff       (20)      612 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_galaxia.py
--rw-r--r--   0 rieder     (501) staff       (20)    13393 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_gravity_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)    31652 2022-10-03 08:52:42.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_hacs64.py
--rw-r--r--   0 rieder     (501) staff       (20)    19462 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_halogen.py
--rw-r--r--   0 rieder     (501) staff       (20)    35886 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_hermite.py
--rw-r--r--   0 rieder     (501) staff       (20)    18675 2023-04-04 13:47:06.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_higpus.py
--rw-r--r--   0 rieder     (501) staff       (20)    17901 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_hop.py
--rw-r--r--   0 rieder     (501) staff       (20)    36829 2021-12-07 10:22:56.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_huayno.py
--rw-r--r--   0 rieder     (501) staff       (20)     4918 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_interface.py
--rw-r--r--   0 rieder     (501) staff       (20)     2551 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_kepler.py
--rw-r--r--   0 rieder     (501) staff       (20)    16208 2022-11-30 07:27:07.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_krome.py
--rw-r--r--   0 rieder     (501) staff       (20)      611 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_lab.py
--rw-r--r--   0 rieder     (501) staff       (20)    30062 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mercury.py
--rw-r--r--   0 rieder     (501) staff       (20)    57505 2022-11-30 13:58:15.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mesa_15140.py
--rw-r--r--   0 rieder     (501) staff       (20)    55849 2022-10-03 08:52:42.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mesa_2208.py
--rw-r--r--   0 rieder     (501) staff       (20)    31008 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mi6.py
--rw-r--r--   0 rieder     (501) staff       (20)    32453 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mikkola.py
--rw-r--r--   0 rieder     (501) staff       (20)    61702 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mmams.py
--rw-r--r--   0 rieder     (501) staff       (20)    30714 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mobse.py
--rw-r--r--   0 rieder     (501) staff       (20)    11804 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mocassin.py
--rw-r--r--   0 rieder     (501) staff       (20)    33325 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mosse.py
--rw-r--r--   0 rieder     (501) staff       (20)    46711 2022-10-03 08:52:42.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mpiamrvac.py
--rw-r--r--   0 rieder     (501) staff       (20)    44675 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_multiples.py
--rw-r--r--   0 rieder     (501) staff       (20)     3375 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_nbody6xx.py
--rw-r--r--   0 rieder     (501) staff       (20)     8533 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_octgrav.py
--rw-r--r--   0 rieder     (501) staff       (20)     4252 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_parallel.py
--rw-r--r--   0 rieder     (501) staff       (20)     2632 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_parameter_doc.py
--rw-r--r--   0 rieder     (501) staff       (20)     8679 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_particle_attributes.py
--rw-r--r--   0 rieder     (501) staff       (20)     4562 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_petar.py
--rw-r--r--   0 rieder     (501) staff       (20)    45951 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_ph4.py
--rw-r--r--   0 rieder     (501) staff       (20)     4584 2021-12-07 10:22:56.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_phantom.py
--rw-r--r--   0 rieder     (501) staff       (20)    35731 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_phigrape.py
--rw-r--r--   0 rieder     (501) staff       (20)    22135 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_pikachu.py
--rw-r--r--   0 rieder     (501) staff       (20)    22766 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_rebound.py
--rw-r--r--   0 rieder     (501) staff       (20)    27693 2022-10-03 08:52:42.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_sakura.py
--rw-r--r--   0 rieder     (501) staff       (20)    28326 2023-02-13 15:26:17.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_seba.py
--rw-r--r--   0 rieder     (501) staff       (20)    23885 2021-07-05 11:19:28.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_secularmultiple.py
--rw-r--r--   0 rieder     (501) staff       (20)    23796 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_simplex.py
--rw-r--r--   0 rieder     (501) staff       (20)    50786 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_simplex_data.txt
--rw-r--r--   0 rieder     (501) staff       (20)    23775 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_smalln.py
--rw-r--r--   0 rieder     (501) staff       (20)    25091 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_sphray.py
--rw-r--r--   0 rieder     (501) staff       (20)   370256 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_sphray_data_4K
--rw-r--r--   0 rieder     (501) staff       (20)       70 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_sphray_data_sources_001.1
--rw-r--r--   0 rieder     (501) staff       (20)    32379 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_sse.py
--rw-r--r--   0 rieder     (501) staff       (20)     5910 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_stellar_evolution.py
--rw-r--r--   0 rieder     (501) staff       (20)    26865 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_tupan.py
--rw-r--r--   0 rieder     (501) staff       (20)    12467 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_twobody.py
--rw-r--r--   0 rieder     (501) staff       (20)     6734 2022-10-03 08:52:42.000000 amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_vader.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:42.977692 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2020-03-24 14:36:26.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    30140 2023-04-04 13:47:06.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_async.py
--rw-r--r--   0 rieder     (501) staff       (20)     2210 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_c_distributed_implementation.py
--rw-r--r--   0 rieder     (501) staff       (20)    25904 2022-10-03 08:52:42.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_c_implementation.py
--rw-r--r--   0 rieder     (501) staff       (20)    19229 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_c_implementation_simplified.py
--rw-r--r--   0 rieder     (501) staff       (20)     1755 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_c_sockets_implementation.py
--rw-r--r--   0 rieder     (501) staff       (20)    21368 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_fortran_implementation.py
--rw-r--r--   0 rieder     (501) staff       (20)     9731 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_fortran_sockets_implementation.py
--rw-r--r--   0 rieder     (501) staff       (20)     3746 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_grid_implementation.py
--rw-r--r--   0 rieder     (501) staff       (20)    21112 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_java_implementation.py
--rw-r--r--   0 rieder     (501) staff       (20)    40168 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_python_implementation.py
--rw-r--r--   0 rieder     (501) staff       (20)     3948 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_python_implementation_mpi.py
--rw-r--r--   0 rieder     (501) staff       (20)     5776 2022-10-03 08:52:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_python_sockets_implementation.py
--rw-r--r--   0 rieder     (501) staff       (20)    37119 2022-11-30 13:58:15.000000 amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_stopping_conditions.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:42.998787 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    19563 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/evolved.dyn
--rw-r--r--   0 rieder     (501) staff       (20)   344304 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/gadget_snapshot
--rw-r--r--   0 rieder     (501) staff       (20)    53296 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/gassphere_bigendian.dat
--rw-r--r--   0 rieder     (501) staff       (20)    53296 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/gassphere_littleendian.dat
--rw-r--r--   0 rieder     (501) staff       (20)   148110 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/h2048.txt
--rw-r--r--   0 rieder     (501) staff       (20)     1027 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/p10.txt
--rw-r--r--   0 rieder     (501) staff       (20)     3086 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/plummer.dyn
--rw-r--r--   0 rieder     (501) staff       (20)     7451 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/plummer128.nemo
--rw-r--r--   0 rieder     (501) staff       (20)    12941 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/plummer_100.ini
--rw-r--r--   0 rieder     (501) staff       (20)      133 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_amuse_import.py
--rw-r--r--   0 rieder     (501) staff       (20)     4779 2023-02-13 15:24:31.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_amusetest.py
--rw-r--r--   0 rieder     (501) staff       (20)     8290 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_attribute_error.py
--rw-r--r--   0 rieder     (501) staff       (20)    14016 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_attribute_storage.py
--rw-r--r--   0 rieder     (501) staff       (20)    20414 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_binaryio.py
--rw-r--r--   0 rieder     (501) staff       (20)    18754 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_bridge.py
--rw-r--r--   0 rieder     (501) staff       (20)    12342 2023-02-13 15:24:31.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_console.py
--rw-r--r--   0 rieder     (501) staff       (20)     1202 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_constants.py
--rw-r--r--   0 rieder     (501) staff       (20)     3808 2022-11-30 13:58:15.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_generate_fortran.py
--rw-r--r--   0 rieder     (501) staff       (20)     4399 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_generic_units.py
--rw-r--r--   0 rieder     (501) staff       (20)     3361 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_grid_attributes.py
--rw-r--r--   0 rieder     (501) staff       (20)    47790 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_grids.py
--rw-r--r--   0 rieder     (501) staff       (20)     1622 2021-12-07 10:22:52.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_imf.py
--rw-r--r--   0 rieder     (501) staff       (20)    16726 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_incode_particle_sets.py
--rw-r--r--   0 rieder     (501) staff       (20)    25723 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_incode_storage.py
--rw-r--r--   0 rieder     (501) staff       (20)    19310 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_indexing.py
--rw-r--r--   0 rieder     (501) staff       (20)     5046 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_inmemorystorage.py
--rw-r--r--   0 rieder     (501) staff       (20)    73292 2022-10-03 08:52:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_interface.py
--rw-r--r--   0 rieder     (501) staff       (20)    20366 2022-10-03 08:52:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_io.py
--rw-r--r--   0 rieder     (501) staff       (20)    25325 2022-10-03 08:52:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_links.py
--rw-r--r--   0 rieder     (501) staff       (20)     2566 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_literature.py
--rw-r--r--   0 rieder     (501) staff       (20)     3260 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_nbody_units.py
--rw-r--r--   0 rieder     (501) staff       (20)     1733 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_nemo.py
--rw-r--r--   0 rieder     (501) staff       (20)     8973 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_options.py
--rw-r--r--   0 rieder     (501) staff       (20)     2523 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_optparse.py
--rw-r--r--   0 rieder     (501) staff       (20)    42579 2023-02-28 13:02:12.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_parameters.py
--rw-r--r--   0 rieder     (501) staff       (20)    23693 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_particle_attributes.py
--rw-r--r--   0 rieder     (501) staff       (20)   205198 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_particles.py
--rw-r--r--   0 rieder     (501) staff       (20)     2192 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_particles_properties.py
--rw-r--r--   0 rieder     (501) staff       (20)     1118 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_phigrape.py
--rw-r--r--   0 rieder     (501) staff       (20)     8328 2023-02-13 15:24:31.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_pickle.py
--rw-r--r--   0 rieder     (501) staff       (20)     6358 2021-04-14 13:39:41.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_plot.py
--rw-r--r--   0 rieder     (501) staff       (20)    20644 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_quantities.py
--rw-r--r--   0 rieder     (501) staff       (20)     8184 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_rotation.py
--rw-r--r--   0 rieder     (501) staff       (20)      782 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_scaling_converter.py
--rw-r--r--   0 rieder     (501) staff       (20)     7012 2022-10-03 08:52:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_staggeredgrid.py
--rw-r--r--   0 rieder     (501) staff       (20)    11071 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_starlab.py
--rw-r--r--   0 rieder     (501) staff       (20)     7057 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_stopping_conditions.py
--rw-r--r--   0 rieder     (501) staff       (20)    42160 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_store.py
--rw-r--r--   0 rieder     (501) staff       (20)     1239 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_subsub.dyn
--rw-r--r--   0 rieder     (501) staff       (20)    21044 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_textio.py
--rw-r--r--   0 rieder     (501) staff       (20)    10845 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_trees.py
--rw-r--r--   0 rieder     (501) staff       (20)     6468 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_unit_conversion.py
--rw-r--r--   0 rieder     (501) staff       (20)     5253 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_vtkio.py
--rw-r--r--   0 rieder     (501) staff       (20)    42656 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/ticket245.dat
--rw-r--r--   0 rieder     (501) staff       (20)     2480 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/tiny_lcdm_data_littleendian.dat
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:43.010917 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     1015 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_boss_bodenheimer.py
--rw-r--r--   0 rieder     (501) staff       (20)     6951 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_brokenimf.py
--rw-r--r--   0 rieder     (501) staff       (20)     2572 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)    12086 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_collision_handler.py
--rw-r--r--   0 rieder     (501) staff       (20)     3862 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_composition_methods.py
--rw-r--r--   0 rieder     (501) staff       (20)     5815 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_concurrent.py
--rw-r--r--   0 rieder     (501) staff       (20)    30402 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_distributed_particles.py
--rw-r--r--   0 rieder     (501) staff       (20)     1508 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_evrardmodel.py
--rw-r--r--   0 rieder     (501) staff       (20)    10659 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_fallback_stellar_evolution.py
--rw-r--r--   0 rieder     (501) staff       (20)     4072 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_flatimf.py
--rw-r--r--   0 rieder     (501) staff       (20)     4049 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_fractalcluster.py
--rw-r--r--   0 rieder     (501) staff       (20)     9518 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_galactic_potentials.py
--rw-r--r--   0 rieder     (501) staff       (20)     8124 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_galactics_model.py
--rw-r--r--   0 rieder     (501) staff       (20)     3575 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_gasplummer.py
--rw-r--r--   0 rieder     (501) staff       (20)    13426 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_grid_remappers.py
--rw-r--r--   0 rieder     (501) staff       (20)     7115 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_grid_to_sph.py
--rw-r--r--   0 rieder     (501) staff       (20)     2021 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_halogen_model.py
--rw-r--r--   0 rieder     (501) staff       (20)    10749 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_hydro_collision.py
--rw-r--r--   0 rieder     (501) staff       (20)     1454 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_isotropic_cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)     2841 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_jobserver.py
--rw-r--r--   0 rieder     (501) staff       (20)     2916 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_kingmodel.py
--rw-r--r--   0 rieder     (501) staff       (20)      957 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_limepy.py
--rw-r--r--   0 rieder     (501) staff       (20)      909 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_mameclot.py
--rw-r--r--   0 rieder     (501) staff       (20)     1404 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_molecular_cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)    27307 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_orbital_elements.py
--rw-r--r--   0 rieder     (501) staff       (20)     5466 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_parallel_stellar_evolution.py
--rw-r--r--   0 rieder     (501) staff       (20)     2462 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_particles_with_color.py
--rw-r--r--   0 rieder     (501) staff       (20)     1902 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_plummer.py
--rw-r--r--   0 rieder     (501) staff       (20)     2065 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_roche_radius.py
--rw-r--r--   0 rieder     (501) staff       (20)     3489 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_rotating_bridge.py
--rw-r--r--   0 rieder     (501) staff       (20)     2651 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_salpeter.py
--rw-r--r--   0 rieder     (501) staff       (20)    26125 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_sink.py
--rw-r--r--   0 rieder     (501) staff       (20)     2437 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_solarsystem.py
--rw-r--r--   0 rieder     (501) staff       (20)     7581 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_sph_to_grid.py
--rw-r--r--   0 rieder     (501) staff       (20)     9005 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_sph_to_star.py
--rw-r--r--   0 rieder     (501) staff       (20)    19786 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_spherical_model.py
--rw-r--r--   0 rieder     (501) staff       (20)    57279 2021-04-22 16:00:02.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_star_to_sph.py
--rw-r--r--   0 rieder     (501) staff       (20)     3709 2021-07-05 11:19:28.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_static_potentials.py
--rw-r--r--   0 rieder     (501) staff       (20)    32919 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_stellar_wind.py
--rw-r--r--   0 rieder     (501) staff       (20)     3505 2022-10-10 09:16:43.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_sticky_spheres.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:43.011830 amuse-tests-2023.4.0/src/amuse/test/suite/reports/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/reports/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     2951 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/reports/plot_speed_report.py
--rw-r--r--   0 rieder     (501) staff       (20)    19645 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/reports/speed_report.py
--rw-r--r--   0 rieder     (501) staff       (20)    10126 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/reports/test_speed.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:43.013267 amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/
--rw-r--r--   0 rieder     (501) staff       (20)    12721 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/FinalSnapshot.out
--rw-r--r--   0 rieder     (501) staff       (20)        0 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      591 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/test_issue123.py
--rw-r--r--   0 rieder     (501) staff       (20)     1308 2021-07-22 12:57:15.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/test_issue777.py
--rw-r--r--   0 rieder     (501) staff       (20)     6420 2023-02-13 15:24:31.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/test_issue850.py
--rw-r--r--   0 rieder     (501) staff       (20)     1132 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/test_ticket118.py
--rw-r--r--   0 rieder     (501) staff       (20)     3600 2021-04-12 16:14:01.000000 amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/test_ticket208.py
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-04-04 14:22:40.000000 amuse-tests-2023.4.0/src/amuse/test/suite/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:43.014803 amuse-tests-2023.4.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2020-03-24 14:36:26.000000 amuse-tests-2023.4.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2021-07-05 11:19:28.000000 amuse-tests-2023.4.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2022-11-30 13:58:15.000000 amuse-tests-2023.4.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2020-03-24 14:36:26.000000 amuse-tests-2023.4.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2020-03-24 14:36:26.000000 amuse-tests-2023.4.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2020-03-24 14:36:26.000000 amuse-tests-2023.4.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2020-03-24 14:36:26.000000 amuse-tests-2023.4.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    50379 2023-04-04 13:47:06.000000 amuse-tests-2023.4.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2021-04-14 10:14:49.000000 amuse-tests-2023.4.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.754807 amuse-tests-2023.5.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      215 2022-11-22 11:55:14.000000 amuse-tests-2023.5.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1208 2023-05-17 10:19:52.754644 amuse-tests-2023.5.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       83 2022-11-22 11:55:14.000000 amuse-tests-2023.5.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.705423 amuse-tests-2023.5.0/amuse_tests.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1208 2023-05-17 10:19:51.000000 amuse-tests-2023.5.0/amuse_tests.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)    10313 2023-05-17 10:19:52.000000 amuse-tests-2023.5.0/amuse_tests.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:51.000000 amuse-tests-2023.5.0/amuse_tests.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:19:51.000000 amuse-tests-2023.5.0/amuse_tests.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:19:51.000000 amuse-tests-2023.5.0/amuse_tests.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-tests-2023.5.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:52.754859 amuse-tests-2023.5.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1960 2022-11-22 11:55:14.000000 amuse-tests-2023.5.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.703571 amuse-tests-2023.5.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.703623 amuse-tests-2023.5.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.703675 amuse-tests-2023.5.0/src/amuse/test/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.705764 amuse-tests-2023.5.0/src/amuse/test/suite/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/__init__.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.726022 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    15226 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/gd_tests.py
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/legacy_support.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6218 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_aarsethzare.py
+-rw-r--r--   0 rieder     (501) staff       (20)    18691 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_adaptb.py
+-rw-r--r--   0 rieder     (501) staff       (20)   128934 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_athena.py
+-rw-r--r--   0 rieder     (501) staff       (20)    40330 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_bhtree.py
+-rw-r--r--   0 rieder     (501) staff       (20)    13290 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_bonsai.py
+-rw-r--r--   0 rieder     (501) staff       (20)    13495 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_bonsai2.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2086 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_bridge.py
+-rw-r--r--   0 rieder     (501) staff       (20)    18163 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_brutus.py
+-rw-r--r--   0 rieder     (501) staff       (20)    30297 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_bse.py
+-rw-r--r--   0 rieder     (501) staff       (20)    79426 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_capreole.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5328 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_create_dir.py
+-rw-r--r--   0 rieder     (501) staff       (20)    58983 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_encounters.py
+-rw-r--r--   0 rieder     (501) staff       (20)    47719 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_evtwin.py
+-rw-r--r--   0 rieder     (501) staff       (20)    20188 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_fastkick.py
+-rw-r--r--   0 rieder     (501) staff       (20)    82682 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_fi.py
+-rw-r--r--   0 rieder     (501) staff       (20)    76139 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_gadget2.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19758 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_galactics.py
+-rw-r--r--   0 rieder     (501) staff       (20)      612 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_galaxia.py
+-rw-r--r--   0 rieder     (501) staff       (20)    13393 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_gravity_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)    31652 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_hacs64.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19462 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_halogen.py
+-rw-r--r--   0 rieder     (501) staff       (20)    35886 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_hermite.py
+-rw-r--r--   0 rieder     (501) staff       (20)    18675 2023-04-04 13:20:13.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_higpus.py
+-rw-r--r--   0 rieder     (501) staff       (20)    17901 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_hop.py
+-rw-r--r--   0 rieder     (501) staff       (20)    36829 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_huayno.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4918 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2551 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_kepler.py
+-rw-r--r--   0 rieder     (501) staff       (20)    16208 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_krome.py
+-rw-r--r--   0 rieder     (501) staff       (20)      611 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_lab.py
+-rw-r--r--   0 rieder     (501) staff       (20)    30062 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mercury.py
+-rw-r--r--   0 rieder     (501) staff       (20)    57650 2023-05-16 12:26:22.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mesa_15140.py
+-rw-r--r--   0 rieder     (501) staff       (20)    55849 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mesa_2208.py
+-rw-r--r--   0 rieder     (501) staff       (20)    31008 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mi6.py
+-rw-r--r--   0 rieder     (501) staff       (20)    32453 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mikkola.py
+-rw-r--r--   0 rieder     (501) staff       (20)    61702 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mmams.py
+-rw-r--r--   0 rieder     (501) staff       (20)    30714 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mobse.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11804 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mocassin.py
+-rw-r--r--   0 rieder     (501) staff       (20)    33325 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mosse.py
+-rw-r--r--   0 rieder     (501) staff       (20)    46711 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mpiamrvac.py
+-rw-r--r--   0 rieder     (501) staff       (20)    44675 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_multiples.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3375 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_nbody6xx.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8533 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_octgrav.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4252 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_parallel.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2632 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_parameter_doc.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8679 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_particle_attributes.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4562 2023-05-16 07:05:57.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_petar.py
+-rw-r--r--   0 rieder     (501) staff       (20)    45951 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_ph4.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4584 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_phantom.py
+-rw-r--r--   0 rieder     (501) staff       (20)    35731 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_phigrape.py
+-rw-r--r--   0 rieder     (501) staff       (20)    22135 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_pikachu.py
+-rw-r--r--   0 rieder     (501) staff       (20)    22766 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_rebound.py
+-rw-r--r--   0 rieder     (501) staff       (20)    27693 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_sakura.py
+-rw-r--r--   0 rieder     (501) staff       (20)    28326 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_seba.py
+-rw-r--r--   0 rieder     (501) staff       (20)    23885 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_secularmultiple.py
+-rw-r--r--   0 rieder     (501) staff       (20)    23796 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_simplex.py
+-rw-r--r--   0 rieder     (501) staff       (20)    50786 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_simplex_data.txt
+-rw-r--r--   0 rieder     (501) staff       (20)    23775 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_smalln.py
+-rw-r--r--   0 rieder     (501) staff       (20)    25091 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_sphray.py
+-rw-r--r--   0 rieder     (501) staff       (20)   370256 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_sphray_data_4K
+-rw-r--r--   0 rieder     (501) staff       (20)       70 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_sphray_data_sources_001.1
+-rw-r--r--   0 rieder     (501) staff       (20)    32406 2023-05-15 07:11:06.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_sse.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5910 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_stellar_evolution.py
+-rw-r--r--   0 rieder     (501) staff       (20)    26865 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_tupan.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12467 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_twobody.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6734 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_vader.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.729361 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    30140 2023-04-04 13:20:13.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_async.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2210 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_c_distributed_implementation.py
+-rw-r--r--   0 rieder     (501) staff       (20)    25904 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_c_implementation.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19229 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_c_implementation_simplified.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1755 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_c_sockets_implementation.py
+-rw-r--r--   0 rieder     (501) staff       (20)    21368 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_fortran_implementation.py
+-rw-r--r--   0 rieder     (501) staff       (20)     9731 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_fortran_sockets_implementation.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3746 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_grid_implementation.py
+-rw-r--r--   0 rieder     (501) staff       (20)    21112 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_java_implementation.py
+-rw-r--r--   0 rieder     (501) staff       (20)    40168 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_python_implementation.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3948 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_python_implementation_mpi.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5776 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_python_sockets_implementation.py
+-rw-r--r--   0 rieder     (501) staff       (20)    37119 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_stopping_conditions.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.743738 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19563 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/evolved.dyn
+-rw-r--r--   0 rieder     (501) staff       (20)   344304 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/gadget_snapshot
+-rw-r--r--   0 rieder     (501) staff       (20)    53296 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/gassphere_bigendian.dat
+-rw-r--r--   0 rieder     (501) staff       (20)    53296 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/gassphere_littleendian.dat
+-rw-r--r--   0 rieder     (501) staff       (20)   148110 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/h2048.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     1027 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/p10.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     3086 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/plummer.dyn
+-rw-r--r--   0 rieder     (501) staff       (20)     7451 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/plummer128.nemo
+-rw-r--r--   0 rieder     (501) staff       (20)    12941 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/plummer_100.ini
+-rw-r--r--   0 rieder     (501) staff       (20)      133 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_amuse_import.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4779 2023-02-28 13:34:30.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_amusetest.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8290 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_attribute_error.py
+-rw-r--r--   0 rieder     (501) staff       (20)    14016 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_attribute_storage.py
+-rw-r--r--   0 rieder     (501) staff       (20)    20414 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_binaryio.py
+-rw-r--r--   0 rieder     (501) staff       (20)    18754 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_bridge.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12342 2023-02-28 13:34:30.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_console.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1202 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_constants.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3808 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_generate_fortran.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4399 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_generic_units.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3361 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_grid_attributes.py
+-rw-r--r--   0 rieder     (501) staff       (20)    47790 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_grids.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1622 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_imf.py
+-rw-r--r--   0 rieder     (501) staff       (20)    16726 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_incode_particle_sets.py
+-rw-r--r--   0 rieder     (501) staff       (20)    25723 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_incode_storage.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19310 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_indexing.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5046 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_inmemorystorage.py
+-rw-r--r--   0 rieder     (501) staff       (20)    73292 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)    20366 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_io.py
+-rw-r--r--   0 rieder     (501) staff       (20)    25325 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_links.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2566 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_literature.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3260 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_nbody_units.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1733 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_nemo.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8973 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_options.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2523 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_optparse.py
+-rw-r--r--   0 rieder     (501) staff       (20)    42579 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_parameters.py
+-rw-r--r--   0 rieder     (501) staff       (20)    23693 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_particle_attributes.py
+-rw-r--r--   0 rieder     (501) staff       (20)   205198 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_particles.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2192 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_particles_properties.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1118 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_phigrape.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8328 2023-02-28 13:34:30.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_pickle.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6358 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_plot.py
+-rw-r--r--   0 rieder     (501) staff       (20)    20644 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_quantities.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8184 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_rotation.py
+-rw-r--r--   0 rieder     (501) staff       (20)      782 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_scaling_converter.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7012 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_staggeredgrid.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11071 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_starlab.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7057 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_stopping_conditions.py
+-rw-r--r--   0 rieder     (501) staff       (20)    42160 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_store.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1239 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_subsub.dyn
+-rw-r--r--   0 rieder     (501) staff       (20)    21044 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_textio.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10845 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_trees.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6468 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_unit_conversion.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5253 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_vtkio.py
+-rw-r--r--   0 rieder     (501) staff       (20)    42656 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/ticket245.dat
+-rw-r--r--   0 rieder     (501) staff       (20)     2480 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/tiny_lcdm_data_littleendian.dat
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.751046 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_boss_bodenheimer.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6951 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_brokenimf.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2572 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12086 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_collision_handler.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3862 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_composition_methods.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5815 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_concurrent.py
+-rw-r--r--   0 rieder     (501) staff       (20)    30402 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_distributed_particles.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1508 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_evrardmodel.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10659 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_fallback_stellar_evolution.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4072 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_flatimf.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4049 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_fractalcluster.py
+-rw-r--r--   0 rieder     (501) staff       (20)     9518 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_galactic_potentials.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8124 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_galactics_model.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3575 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_gasplummer.py
+-rw-r--r--   0 rieder     (501) staff       (20)    13426 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_grid_remappers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7115 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_grid_to_sph.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2021 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_halogen_model.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10749 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_hydro_collision.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1454 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_isotropic_cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2841 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_jobserver.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2916 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_kingmodel.py
+-rw-r--r--   0 rieder     (501) staff       (20)      957 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_limepy.py
+-rw-r--r--   0 rieder     (501) staff       (20)      909 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_mameclot.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1404 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_molecular_cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)    27307 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_orbital_elements.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5466 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_parallel_stellar_evolution.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2462 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_particles_with_color.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1902 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_plummer.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2065 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_roche_radius.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3489 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_rotating_bridge.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2651 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_salpeter.py
+-rw-r--r--   0 rieder     (501) staff       (20)    26125 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_sink.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2437 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_solarsystem.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7581 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_sph_to_grid.py
+-rw-r--r--   0 rieder     (501) staff       (20)     9005 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_sph_to_star.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19786 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_spherical_model.py
+-rw-r--r--   0 rieder     (501) staff       (20)    57279 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_star_to_sph.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3709 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_static_potentials.py
+-rw-r--r--   0 rieder     (501) staff       (20)    32919 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_stellar_wind.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3505 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_sticky_spheres.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.751695 amuse-tests-2023.5.0/src/amuse/test/suite/reports/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/reports/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2951 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/reports/plot_speed_report.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19645 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/reports/speed_report.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10126 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/reports/test_speed.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.753163 amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/
+-rw-r--r--   0 rieder     (501) staff       (20)    12721 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/FinalSnapshot.out
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1077 2023-05-11 09:04:53.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_github856.py
+-rw-r--r--   0 rieder     (501) staff       (20)      591 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_issue123.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1308 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_issue777.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6420 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_issue850.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1132 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_ticket118.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3600 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_ticket208.py
+-rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:51.000000 amuse-tests-2023.5.0/src/amuse/test/suite/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:52.754425 amuse-tests-2023.5.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-tests-2023.5.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-tests-2023.5.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-tests-2023.5.0/support/version.py
```

### Comparing `amuse-tests-2023.4.0/PKG-INFO` & `amuse-tests-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-tests
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: The Astrophysical Multipurpose Software Environment - tests
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `amuse-tests-2023.4.0/amuse_tests.egg-info/PKG-INFO` & `amuse-tests-2023.5.0/amuse_tests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-tests
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: The Astrophysical Multipurpose Software Environment - tests
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `amuse-tests-2023.4.0/amuse_tests.egg-info/SOURCES.txt` & `amuse-tests-2023.5.0/amuse_tests.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -190,14 +190,15 @@
 src/amuse/test/suite/ext_tests/test_sticky_spheres.py
 src/amuse/test/suite/reports/__init__.py
 src/amuse/test/suite/reports/plot_speed_report.py
 src/amuse/test/suite/reports/speed_report.py
 src/amuse/test/suite/reports/test_speed.py
 src/amuse/test/suite/ticket_tests/FinalSnapshot.out
 src/amuse/test/suite/ticket_tests/__init__.py
+src/amuse/test/suite/ticket_tests/test_github856.py
 src/amuse/test/suite/ticket_tests/test_issue123.py
 src/amuse/test/suite/ticket_tests/test_issue777.py
 src/amuse/test/suite/ticket_tests/test_issue850.py
 src/amuse/test/suite/ticket_tests/test_ticket118.py
 src/amuse/test/suite/ticket_tests/test_ticket208.py
 support/__init__.py
 support/classifiers.py
```

### Comparing `amuse-tests-2023.4.0/setup.py` & `amuse-tests-2023.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/gd_tests.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/gd_tests.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_aarsethzare.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_aarsethzare.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_adaptb.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_adaptb.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_athena.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_athena.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_bhtree.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_bhtree.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_bonsai.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_bonsai.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_bonsai2.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_bonsai2.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_bridge.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_bridge.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_brutus.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_brutus.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_bse.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_bse.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_capreole.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_capreole.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_create_dir.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_create_dir.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_encounters.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_encounters.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_evtwin.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_evtwin.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_fastkick.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_fastkick.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_fi.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_fi.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_gadget2.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_gadget2.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_galactics.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_galactics.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_galaxia.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_galaxia.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_gravity_codes.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_gravity_codes.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_hacs64.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_hacs64.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_halogen.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_halogen.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_hermite.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_hermite.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_higpus.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_higpus.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_hop.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_hop.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_huayno.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_huayno.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_interface.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_kepler.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_kepler.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_krome.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_krome.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_lab.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_lab.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mercury.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mercury.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mesa_15140.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mesa_15140.py`

 * *Files 0% similar despite different names*

```diff
@@ -748,33 +748,37 @@
             (0.3) - instance.parameters.metallicity)
         self.assertAlmostEqual(
             composition[3:, k_surface].sum(),
             instance.parameters.metallicity)
 
         he4_start = composition[2,k_surface] 
         h1_start = composition[0,k_surface] 
+
+        h1_profile = composition[0] * 1
+        he4_profile = composition[2] * 1
+
+        instance.particles[0].set_control('okay_to_remesh',False) # Turn of remeshing
+
         # Gradually and consistently increase helium and decrease hydrogen
         # abundances until reversed
-        for alpha in [0.3, 1.0, -0.5, -0.125]:
-            h1_profile = composition[0] * 1
-            he4_profile = composition[2] * 1
+        for alpha in numpy.arange(0.1,1.1,0.1):
             composition[0] = alpha * he4_profile + (1-alpha) * h1_profile
             composition[2] = (1-alpha) * he4_profile + alpha * h1_profile
             instance.particles[0].set_chemical_abundance_profiles(composition)
-            instance.evolve_model(1 | units.julianyr)
+            instance.particles[0].evolve_for(1 | units.julianyr)
             composition = (
                 instance.particles[0].get_chemical_abundance_profiles()
             )
 
         self.assertAlmostEqual(
-            composition[2, k_surface],0.7051777340467488)
-        self.assertAlmostEqual(composition[0, k_surface],  2.74649042e-01 )
+            composition[2, k_surface],h1_start,3)
+        self.assertAlmostEqual(composition[0, k_surface], he4_start, 3)
         self.assertAlmostEqual(
             composition[3:, k_surface].sum(),
-            0.020144181852121544)
+            0.020,3)
         self.assertAlmostEqual(composition.sum(axis=0), 1.0)
 
         self.assertRaises(
             AmuseException,
             instance.particles[0].set_chemical_abundance_profiles,
             composition[:7],
             expected_message=(
@@ -883,15 +887,15 @@
             instance.imported_stars[0].get_radius_profile()[-1],
             1.0 | units.RSun)
         self.assertIsOfOrder(
             instance.imported_stars[0].get_temperature_profile()[0],
             1.0e7 | units.K)
         self.assertIsOfOrder(
             instance.imported_stars[0].get_pressure_profile()[0],
-            1.0e18 | units.barye)
+            1.0e17 | units.barye)
         self.assertAlmostEqual(
             instance.imported_stars[0].get_mass_profile()[-1],
             instance.native_stars[0].get_mass_profile()[-1])
 
         print(instance.particles)
         instance.evolve_model(keep_synchronous=False)
         print(instance.particles)
@@ -1063,15 +1067,15 @@
         self.assertAlmostRelativeEqual(
             star.mass_change, -1.0e-8 | units.MSun / units.julianyr)
         self.assertAlmostRelativeEqual(
             star.wind, -1.0e-8 | units.MSun / units.julianyr, 3)
 
         star.evolve_for(1.0e5 | units.julianyr)
         self.assertAlmostRelativeEqual(star.age, 2.e5 | units.julianyr, 3)
-        self.assertAlmostRelativeEqual(star.mass,  1.00 | units.MSun)
+        self.assertAlmostRelativeEqual(star.mass,  1.00 | units.MSun, 3)
         print(star.as_set())
         instance.stop()
 
     def slowtest19a(self):
         print("Testing MESA core mass")
         instance = self.new_instance_of_an_optional_code(MESA)
         set_mesa_paths_instance(instance)
@@ -1187,15 +1191,15 @@
         self.assertAlmostEqual(he3_core_mass, 0 | units.MSun)
 
     def test22(self):
         print("Testing MESA calculate_core_mass (short version of slowtest21)")
         instance = self.new_instance_of_an_optional_code(MESA)
         set_mesa_paths_instance(instance)
         star = instance.particles.add_particle(Particle(mass=1 | units.MSun))
-        instance.evolve_model(0.3 | units.Gyr)  # VERY short, for test speed up
+        instance.evolve_model(0.2 | units.Gyr)  # VERY short, for test speed up
         central_hydrogen_abundance = star.get_chemical_abundance_profiles(
         )[0][0]
         print(central_hydrogen_abundance)
         self.assertTrue(
             central_hydrogen_abundance < 0.69)  # some hydrogen is burned
         self.assertTrue(
             central_hydrogen_abundance > 0.68)  # ... but not that much yet
@@ -1210,15 +1214,15 @@
         #     3
         # )
 
         # For test speed up, we use a weird core_H_abundance_limit to define
         # the "hydrogen exhausted core"
         # FIXME updated values in the rest of the test
         limit = 0.69
-        expected_core_mass = 0.0847273423268 | units.MSun
+        expected_core_mass = 0.0288211177139 | units.MSun
         self.assertAlmostEqual(
             star.calculate_core_mass(core_H_abundance_limit=limit),
             expected_core_mass, 3)
 
         h1_core_mass = star.calculate_core_mass(
             species=["h1"], core_H_abundance_limit=limit)
         he3_core_mass = star.calculate_core_mass(
@@ -1238,15 +1242,15 @@
         metal_core_mass = star.calculate_core_mass(
             species=["c12", "n14", "o16", "ne20", "mg24"],
             core_H_abundance_limit=limit)
         instance.stop()
         self.assertAlmostRelativeEqual(
             h1_core_mass, expected_core_mass*0.685, 2)
         self.assertAlmostRelativeEqual(
-            he4_core_mass, expected_core_mass*0.295, 2)
+            he4_core_mass, expected_core_mass*0.29, 2)
         self.assertAlmostRelativeEqual(
             metal_core_mass, expected_core_mass*0.02, 1)
         self.assertAlmostRelativeEqual(
             expected_core_mass,
             he4_core_mass + he3_core_mass + metal_core_mass + h1_core_mass, 7)
         self.assertAlmostRelativeEqual(
             metal_core_mass,
@@ -1329,14 +1333,15 @@
                                                                 'be': 0.0,
                                                                 'b': 0.0,
                                                                 'c': 0.0,
                                                                 'n': 0.0,
                                                                 'o': 0.0,
                                                                 'f': 0.0,
                                                                 'ne': 0.0,
+                                                                'na': 0.0,
                                                                 'mg': 0.0,
                                                                 'al': 0.0,
                                                                 'si': 0.0,
                                                                 'p': 0.0,
                                                                 's': 0.0,
                                                                 'cl': 0.0,
                                                                 'ar': 0.0,
```

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mesa_2208.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mesa_2208.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mi6.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mi6.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mikkola.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mikkola.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mmams.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mmams.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mobse.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mobse.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mocassin.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mocassin.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mosse.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mosse.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_mpiamrvac.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_mpiamrvac.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_multiples.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_multiples.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_nbody6xx.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_nbody6xx.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_octgrav.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_octgrav.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_parallel.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_parameter_doc.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_parameter_doc.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_particle_attributes.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_particle_attributes.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_petar.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_petar.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_ph4.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_ph4.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_phantom.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_phantom.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_phigrape.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_phigrape.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_pikachu.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_pikachu.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_rebound.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_rebound.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_sakura.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_sakura.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_seba.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_seba.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_secularmultiple.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_secularmultiple.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_simplex.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_simplex.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_simplex_data.txt` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_simplex_data.txt`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_smalln.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_smalln.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_sphray.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_sphray.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_sphray_data_4K` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_sphray_data_4K`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_sse.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_sse.py`

 * *Files 0% similar despite different names*

```diff
@@ -699,15 +699,16 @@
         sse_src_path = os.path.join(os.path.dirname(sys.modules[SSE.__module__].__file__), 'src')
         if not os.path.exists(os.path.join(sse_src_path, "evolve.in")):
             self.skip("Not in a source release")
         instance = SSE()
         instance.particles.add_particle(Particle(mass = 1.416 | units.MSun))
         instance.particles[0].evolve_for(7000.0 | units.Myr)
         evolved_star = instance.particles.copy()[0]
-        evolved_star.temperature = instance.particles[0].temperature
+        # See issue #957
+        # evolved_star.temperature = instance.particles[0].temperature
         instance.stop()
        
         testpath = get_path_to_results()
         shutil.copy(os.path.join(sse_src_path, "evolve.in"), os.path.join(testpath, "evolve.in"))
         
         call([os.path.join(sse_src_path, "sse")], cwd=testpath)
```

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_stellar_evolution.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_stellar_evolution.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_tupan.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_tupan.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_twobody.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_twobody.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/codes_tests/test_vader.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/codes_tests/test_vader.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_async.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_async.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_c_distributed_implementation.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_c_distributed_implementation.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_c_implementation.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_c_implementation.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_c_implementation_simplified.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_c_implementation_simplified.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_c_sockets_implementation.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_c_sockets_implementation.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_fortran_implementation.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_fortran_implementation.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_fortran_sockets_implementation.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_fortran_sockets_implementation.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_grid_implementation.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_grid_implementation.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_java_implementation.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_java_implementation.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_python_implementation.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_python_implementation.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_python_implementation_mpi.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_python_implementation_mpi.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_python_sockets_implementation.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_python_sockets_implementation.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/compile_tests/test_stopping_conditions.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/compile_tests/test_stopping_conditions.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/evolved.dyn` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/evolved.dyn`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/gadget_snapshot` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/gadget_snapshot`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/gassphere_bigendian.dat` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/gassphere_bigendian.dat`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/gassphere_littleendian.dat` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/gassphere_littleendian.dat`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/h2048.txt` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/h2048.txt`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/p10.txt` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/p10.txt`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/plummer.dyn` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/plummer.dyn`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/plummer128.nemo` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/plummer128.nemo`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/plummer_100.ini` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/plummer_100.ini`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_amusetest.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_amusetest.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_attribute_error.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_attribute_error.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_attribute_storage.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_attribute_storage.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_binaryio.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_binaryio.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_bridge.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_bridge.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_console.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_console.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_constants.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_generate_fortran.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_generate_fortran.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_generic_units.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_generic_units.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_grid_attributes.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_grid_attributes.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_grids.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_grids.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_imf.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_imf.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_incode_particle_sets.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_incode_particle_sets.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_incode_storage.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_incode_storage.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_indexing.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_inmemorystorage.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_inmemorystorage.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_interface.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_io.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_io.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_links.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_links.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_literature.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_literature.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_nbody_units.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_nbody_units.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_nemo.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_nemo.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_options.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_options.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_optparse.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_optparse.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_parameters.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_particle_attributes.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_particle_attributes.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_particles.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_particles.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_particles_properties.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_particles_properties.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_phigrape.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_phigrape.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_pickle.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_plot.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_quantities.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_quantities.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_rotation.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_scaling_converter.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_scaling_converter.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_staggeredgrid.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_staggeredgrid.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_starlab.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_starlab.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_stopping_conditions.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_stopping_conditions.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_store.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_store.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_subsub.dyn` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_subsub.dyn`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_textio.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_textio.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_trees.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_trees.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_unit_conversion.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/test_vtkio.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/test_vtkio.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/ticket245.dat` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/ticket245.dat`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/core_tests/tiny_lcdm_data_littleendian.dat` & `amuse-tests-2023.5.0/src/amuse/test/suite/core_tests/tiny_lcdm_data_littleendian.dat`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_boss_bodenheimer.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_boss_bodenheimer.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_brokenimf.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_brokenimf.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_cloud.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_collision_handler.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_collision_handler.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_composition_methods.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_composition_methods.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_concurrent.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_distributed_particles.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_distributed_particles.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_evrardmodel.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_evrardmodel.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_fallback_stellar_evolution.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_fallback_stellar_evolution.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_flatimf.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_flatimf.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_fractalcluster.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_fractalcluster.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_galactic_potentials.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_galactic_potentials.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_galactics_model.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_galactics_model.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_gasplummer.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_gasplummer.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_grid_remappers.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_grid_remappers.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_grid_to_sph.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_grid_to_sph.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_halogen_model.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_halogen_model.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_hydro_collision.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_hydro_collision.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_isotropic_cloud.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_isotropic_cloud.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_jobserver.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_jobserver.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_kingmodel.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_kingmodel.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_limepy.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_limepy.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_mameclot.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_mameclot.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_molecular_cloud.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_molecular_cloud.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_orbital_elements.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_orbital_elements.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_parallel_stellar_evolution.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_parallel_stellar_evolution.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_particles_with_color.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_particles_with_color.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_plummer.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_plummer.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_roche_radius.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_roche_radius.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_rotating_bridge.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_rotating_bridge.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_salpeter.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_salpeter.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_sink.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_sink.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_solarsystem.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_solarsystem.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_sph_to_grid.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_sph_to_grid.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_sph_to_star.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_sph_to_star.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_spherical_model.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_spherical_model.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_star_to_sph.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_star_to_sph.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_static_potentials.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_static_potentials.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_stellar_wind.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_stellar_wind.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ext_tests/test_sticky_spheres.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ext_tests/test_sticky_spheres.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/reports/plot_speed_report.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/reports/plot_speed_report.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/reports/speed_report.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/reports/speed_report.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/reports/test_speed.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/reports/test_speed.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/FinalSnapshot.out` & `amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/FinalSnapshot.out`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/test_issue123.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_issue123.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/test_issue777.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_issue777.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/test_issue850.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_issue850.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/test_ticket118.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_ticket118.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/src/amuse/test/suite/ticket_tests/test_ticket208.py` & `amuse-tests-2023.5.0/src/amuse/test/suite/ticket_tests/test_ticket208.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/support/__init__.py` & `amuse-tests-2023.5.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/support/classifiers.py` & `amuse-tests-2023.5.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/support/config.py` & `amuse-tests-2023.5.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/support/generate_main.py` & `amuse-tests-2023.5.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/support/getsp.class` & `amuse-tests-2023.5.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/support/getsp.java` & `amuse-tests-2023.5.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/support/misc.py` & `amuse-tests-2023.5.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-tests-2023.4.0/support/setup_codes.py` & `amuse-tests-2023.5.0/support/setup_codes.py`

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

