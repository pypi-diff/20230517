# Comparing `tmp/amuse-athena-2023.4.0.tar.gz` & `tmp/amuse-athena-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-athena-2023.4.0.tar", last modified: Tue Apr  4 14:19:35 2023, max compression
+gzip compressed data, was "amuse-athena-2023.5.0.tar", last modified: Wed May 17 10:17:29 2023, max compression
```

## Comparing `amuse-athena-2023.4.0.tar` & `amuse-athena-2023.5.0.tar`

### file list

```diff
@@ -1,461 +1,461 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.719426 amuse-athena-2023.4.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-04-04 14:19:35.719227 amuse-athena-2023.4.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       59 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.582535 amuse-athena-2023.4.0/amuse_athena.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-04-04 14:19:33.000000 amuse-athena-2023.4.0/amuse_athena.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)    26055 2023-04-04 14:19:35.000000 amuse-athena-2023.4.0/amuse_athena.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-04-04 14:19:33.000000 amuse-athena-2023.4.0/amuse_athena.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-04-04 14:19:33.000000 amuse-athena-2023.4.0/amuse_athena.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-04-04 14:19:33.000000 amuse-athena-2023.4.0/amuse_athena.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       71 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-04-04 14:19:35.719485 amuse-athena-2023.4.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1777 2021-04-23 11:09:14.000000 amuse-athena-2023.4.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.575487 amuse-athena-2023.4.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.575545 amuse-athena-2023.4.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.575606 amuse-athena-2023.4.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.588399 amuse-athena-2023.4.0/src/amuse/community/athena/
--rw-r--r--   0 rieder     (501) staff       (20)     6368 2022-11-30 13:58:14.000000 amuse-athena-2023.4.0/src/amuse/community/athena/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       30 2022-10-03 08:52:42.000000 amuse-athena-2023.4.0/src/amuse/community/athena/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     1456 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/amuse_problem_3.1.c
--rw-r--r--   0 rieder     (501) staff       (20)     1438 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/amuse_problem_4.0.c
--rw-r--r--   0 rieder     (501) staff       (20)     1438 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/amuse_problem_4.1.c
--rwxr-xr-x   0 rieder     (501) staff       (20)     2212 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/download.py
--rw-r--r--   0 rieder     (501) staff       (20)    53617 2023-04-04 13:47:06.000000 amuse-athena-2023.4.0/src/amuse/community/athena/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)    21626 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/interface_3.1.c
--rw-r--r--   0 rieder     (501) staff       (20)    43174 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/interface_4.0.c
--rw-r--r--   0 rieder     (501) staff       (20)    94883 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/interface_4.1.c
--rw-r--r--   0 rieder     (501) staff       (20)      908 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/makefile.patch
--rwxr-xr-x   0 rieder     (501) staff       (20)     2859 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/patch_files.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.575745 amuse-athena-2023.4.0/src/amuse/community/athena/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.589623 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/
--rw-r--r--   0 rieder     (501) staff       (20)     2428 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)     2720 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/Makeoptions.in
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.591061 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/autom4te.cache/
--rw-r--r--   0 rieder     (501) staff       (20)   146872 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/autom4te.cache/output.0
--rw-r--r--   0 rieder     (501) staff       (20)     5106 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/autom4te.cache/requests
--rw-r--r--   0 rieder     (501) staff       (20)     7765 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/autom4te.cache/traces.0
--rwxr-xr-x   0 rieder     (501) staff       (20)   146471 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/configure
--rw-r--r--   0 rieder     (501) staff       (20)    21424 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/configure.ac
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.591327 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/doc/
--rw-r--r--   0 rieder     (501) staff       (20)      552 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/doc/pbs-script
--rwxr-xr-x   0 rieder     (501) staff       (20)     5598 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/install-sh
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.603817 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/
--rw-r--r--   0 rieder     (501) staff       (20)     4367 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)     4632 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/ath_array.c
--rw-r--r--   0 rieder     (501) staff       (20)     4098 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/ath_files.c
--rw-r--r--   0 rieder     (501) staff       (20)     9753 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/ath_log.c
--rw-r--r--   0 rieder     (501) staff       (20)     2475 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/ath_signal.c
--rw-r--r--   0 rieder     (501) staff       (20)    22054 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/athena.h
--rw-r--r--   0 rieder     (501) staff       (20)     3459 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/baton.c
--rw-r--r--   0 rieder     (501) staff       (20)    96563 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/bvals_mhd.c
--rw-r--r--   0 rieder     (501) staff       (20)    84875 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/bvals_shear.c
--rw-r--r--   0 rieder     (501) staff       (20)     5317 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/cc_pos.c
--rw-r--r--   0 rieder     (501) staff       (20)      433 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/config.h.in
--rw-r--r--   0 rieder     (501) staff       (20)    35952 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/convert_var.c
--rw-r--r--   0 rieder     (501) staff       (20)      876 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/copyright.h
--rw-r--r--   0 rieder     (501) staff       (20)     5237 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/defs.h.in
--rw-r--r--   0 rieder     (501) staff       (20)     8144 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/dump_binary.c
--rw-r--r--   0 rieder     (501) staff       (20)    14784 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/dump_history.c
--rw-r--r--   0 rieder     (501) staff       (20)    15062 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/dump_tab.c
--rw-r--r--   0 rieder     (501) staff       (20)    10697 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/dump_vtk.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.608557 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/
--rw-r--r--   0 rieder     (501) staff       (20)    17771 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/LICENSE
--rw-r--r--   0 rieder     (501) staff       (20)     1545 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    11355 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/ath_fft.c
--rw-r--r--   0 rieder     (501) staff       (20)     1662 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/factor.c
--rw-r--r--   0 rieder     (501) staff       (20)    11433 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.c
--rw-r--r--   0 rieder     (501) staff       (20)     2348 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.h
--rw-r--r--   0 rieder     (501) staff       (20)    15253 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     2572 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.h
--rw-r--r--   0 rieder     (501) staff       (20)    10480 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.c
--rw-r--r--   0 rieder     (501) staff       (20)     1203 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.h
--rw-r--r--   0 rieder     (501) staff       (20)    20644 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     1552 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.h
--rw-r--r--   0 rieder     (501) staff       (20)     3814 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    13200 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.c
--rw-r--r--   0 rieder     (501) staff       (20)     2598 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.h
--rw-r--r--   0 rieder     (501) staff       (20)    15313 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     2640 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.h
--rw-r--r--   0 rieder     (501) staff       (20)     3524 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/globals.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.610540 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/
--rw-r--r--   0 rieder     (501) staff       (20)     1287 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    40334 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/bvals_grav.c
--rw-r--r--   0 rieder     (501) staff       (20)     1539 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    20655 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg.c
--rw-r--r--   0 rieder     (501) staff       (20)    10585 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft.c
--rw-r--r--   0 rieder     (501) staff       (20)    17807 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft_obc.c
--rw-r--r--   0 rieder     (501) staff       (20)    35053 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_multigrid.c
--rw-r--r--   0 rieder     (501) staff       (20)    48007 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/init_grid.c
--rw-r--r--   0 rieder     (501) staff       (20)    37805 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/init_mesh.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.615149 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/
--rw-r--r--   0 rieder     (501) staff       (20)     1466 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)     3239 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate.c
--rw-r--r--   0 rieder     (501) staff       (20)    22956 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_ctu.c
--rw-r--r--   0 rieder     (501) staff       (20)    15882 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl.c
--rw-r--r--   0 rieder     (501) staff       (20)    22889 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)    73042 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_ctu.c
--rw-r--r--   0 rieder     (501) staff       (20)    48617 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl.c
--rw-r--r--   0 rieder     (501) staff       (20)    54176 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)   138756 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_ctu.c
--rw-r--r--   0 rieder     (501) staff       (20)    79851 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl.c
--rw-r--r--   0 rieder     (501) staff       (20)    84225 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)     1151 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    28050 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/main.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.617366 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/
--rw-r--r--   0 rieder     (501) staff       (20)     1355 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    13039 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/conduction.c
--rw-r--r--   0 rieder     (501) staff       (20)     2773 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/cool.c
--rw-r--r--   0 rieder     (501) staff       (20)     3252 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/diff_dt.c
--rw-r--r--   0 rieder     (501) staff       (20)     4491 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/get_eta.c
--rw-r--r--   0 rieder     (501) staff       (20)     3299 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/integrate_diffusion.c
--rw-r--r--   0 rieder     (501) staff       (20)     1606 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    45134 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/resistivity.c
--rw-r--r--   0 rieder     (501) staff       (20)    26948 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/viscosity.c
--rw-r--r--   0 rieder     (501) staff       (20)     5855 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/new_dt.c
--rw-r--r--   0 rieder     (501) staff       (20)    45790 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output.c
--rw-r--r--   0 rieder     (501) staff       (20)    11218 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output_pdf.c
--rw-r--r--   0 rieder     (501) staff       (20)     4214 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output_pgm.c
--rw-r--r--   0 rieder     (501) staff       (20)     5464 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output_ppm.c
--rw-r--r--   0 rieder     (501) staff       (20)     8395 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output_tab.c
--rw-r--r--   0 rieder     (501) staff       (20)     8403 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output_vtk.c
--rw-r--r--   0 rieder     (501) staff       (20)    65505 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/palette.h
--rw-r--r--   0 rieder     (501) staff       (20)    31102 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/par.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.622639 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/
--rw-r--r--   0 rieder     (501) staff       (20)     1326 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    87780 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/bvals_particle.c
--rw-r--r--   0 rieder     (501) staff       (20)    13665 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/dump_particle_history.c
--rw-r--r--   0 rieder     (501) staff       (20)    41179 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/feedback.c
--rw-r--r--   0 rieder     (501) staff       (20)     9078 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/init_particle.c
--rw-r--r--   0 rieder     (501) staff       (20)    29582 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/integrators_particle.c
--rw-r--r--   0 rieder     (501) staff       (20)    11513 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/output_particle.c
--rw-r--r--   0 rieder     (501) staff       (20)     1491 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/particle.h
--rw-r--r--   0 rieder     (501) staff       (20)     3799 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    23052 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/utils_particle.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.646670 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/
--rw-r--r--   0 rieder     (501) staff       (20)     4565 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/README
--rw-r--r--   0 rieder     (501) staff       (20)     3503 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/blast.c
--rw-r--r--   0 rieder     (501) staff       (20)    15849 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/bubble.c
--rw-r--r--   0 rieder     (501) staff       (20)     6022 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/carbuncle.c
--rw-r--r--   0 rieder     (501) staff       (20)     7857 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/collapse3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     9095 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw1d.c
--rw-r--r--   0 rieder     (501) staff       (20)    12810 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    17446 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     8063 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cshock1d.c
--rw-r--r--   0 rieder     (501) staff       (20)     3295 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/current_sheet.c
--rw-r--r--   0 rieder     (501) staff       (20)     9456 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cyladvect.c
--rw-r--r--   0 rieder     (501) staff       (20)     6663 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylblast.c
--rw-r--r--   0 rieder     (501) staff       (20)     6283 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylbphi.c
--rw-r--r--   0 rieder     (501) staff       (20)     9325 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylbr.c
--rw-r--r--   0 rieder     (501) staff       (20)     7401 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylfieldloop.c
--rw-r--r--   0 rieder     (501) staff       (20)    25462 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylnewtmri.c
--rw-r--r--   0 rieder     (501) staff       (20)     5379 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylrayleigh.c
--rw-r--r--   0 rieder     (501) staff       (20)     6349 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylunif.c
--rw-r--r--   0 rieder     (501) staff       (20)     6362 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylwind.c
--rw-r--r--   0 rieder     (501) staff       (20)     6841 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylwindrot.c
--rw-r--r--   0 rieder     (501) staff       (20)     8182 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylwindrotb.c
--rw-r--r--   0 rieder     (501) staff       (20)     7564 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/dmr.c
--rw-r--r--   0 rieder     (501) staff       (20)    13562 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/field_loop.c
--rw-r--r--   0 rieder     (501) staff       (20)    12054 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/firehose.c
--rw-r--r--   0 rieder     (501) staff       (20)     4867 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/hall_drift.c
--rw-r--r--   0 rieder     (501) staff       (20)    16086 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/hb3.c
--rw-r--r--   0 rieder     (501) staff       (20)    25056 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/hgb.c
--rw-r--r--   0 rieder     (501) staff       (20)    12816 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/hkdisk.c
--rw-r--r--   0 rieder     (501) staff       (20)     6137 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/jeans.c
--rw-r--r--   0 rieder     (501) staff       (20)     7058 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/jet.c
--rw-r--r--   0 rieder     (501) staff       (20)     8274 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/kh.c
--rw-r--r--   0 rieder     (501) staff       (20)    17209 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave1d.c
--rw-r--r--   0 rieder     (501) staff       (20)    18726 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    21769 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     3693 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/lw_implode.c
--rw-r--r--   0 rieder     (501) staff       (20)     7336 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/noh.c
--rw-r--r--   0 rieder     (501) staff       (20)     4220 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/orszag-tang.c
--rw-r--r--   0 rieder     (501) staff       (20)    14369 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_circ.c
--rw-r--r--   0 rieder     (501) staff       (20)    10895 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_collision.c
--rw-r--r--   0 rieder     (501) staff       (20)     9861 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_epicycle.c
--rw-r--r--   0 rieder     (501) staff       (20)     8447 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_friction.c
--rw-r--r--   0 rieder     (501) staff       (20)    12838 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave1d.c
--rw-r--r--   0 rieder     (501) staff       (20)    11854 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    14766 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_shwave1d.c
--rw-r--r--   0 rieder     (501) staff       (20)    12434 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_shwave2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    27638 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_strat2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    27921 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_strat3d.c
--rw-r--r--   0 rieder     (501) staff       (20)    10544 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/pgflow.c
--rw-r--r--   0 rieder     (501) staff       (20)    12411 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/planet-disk.c
--rw-r--r--   0 rieder     (501) staff       (20)     4045 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/rotor.c
--rw-r--r--   0 rieder     (501) staff       (20)    20876 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/rt.c
--rw-r--r--   0 rieder     (501) staff       (20)     8808 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/shk_cloud.c
--rw-r--r--   0 rieder     (501) staff       (20)     7338 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/shkset1d.c
--rw-r--r--   0 rieder     (501) staff       (20)    14921 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/shkset2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    30745 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/shkset3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     3250 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/shu-osher.c
--rw-r--r--   0 rieder     (501) staff       (20)    41891 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/strat.c
--rw-r--r--   0 rieder     (501) staff       (20)    19916 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_multi.c
--rw-r--r--   0 rieder     (501) staff       (20)    25339 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_single.c
--rw-r--r--   0 rieder     (501) staff       (20)    20516 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_multi.c
--rw-r--r--   0 rieder     (501) staff       (20)    25902 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_single.c
--rw-r--r--   0 rieder     (501) staff       (20)    20966 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/ti.c
--rw-r--r--   0 rieder     (501) staff       (20)    24287 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/turb.c
--rw-r--r--   0 rieder     (501) staff       (20)     4145 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/twoibw.c
--rw-r--r--   0 rieder     (501) staff       (20)    10180 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prototypes.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.649461 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/
--rw-r--r--   0 rieder     (501) staff       (20)     1343 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    18745 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/esystem_prim.c
--rw-r--r--   0 rieder     (501) staff       (20)     2581 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_dc.c
--rw-r--r--   0 rieder     (501) staff       (20)    12889 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_plm.c
--rw-r--r--   0 rieder     (501) staff       (20)    22476 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_ppm.c
--rw-r--r--   0 rieder     (501) staff       (20)    11888 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim2.c
--rw-r--r--   0 rieder     (501) staff       (20)    14242 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim3.c
--rw-r--r--   0 rieder     (501) staff       (20)     1755 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    27483 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/restart.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.654026 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/
--rw-r--r--   0 rieder     (501) staff       (20)     1343 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    22384 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/esystem_roe.c
--rw-r--r--   0 rieder     (501) staff       (20)    20557 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/exact.c
--rw-r--r--   0 rieder     (501) staff       (20)    28427 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/exact_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)     8082 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/force.c
--rw-r--r--   0 rieder     (501) staff       (20)     6545 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc.c
--rw-r--r--   0 rieder     (501) staff       (20)    30910 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)    21397 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld.c
--rw-r--r--   0 rieder     (501) staff       (20)    33705 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)     7683 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle.c
--rw-r--r--   0 rieder     (501) staff       (20)    19191 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)     1706 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)     9544 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/roe.c
--rw-r--r--   0 rieder     (501) staff       (20)     3816 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/two_shock.c
--rw-r--r--   0 rieder     (501) staff       (20)    10463 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/show_config.c
--rw-r--r--   0 rieder     (501) staff       (20)    85682 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/smr.c
--rw-r--r--   0 rieder     (501) staff       (20)    32081 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/utils.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.580515 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.660830 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)     3986 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1125
--rw-r--r--   0 rieder     (501) staff       (20)     3985 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1203
--rw-r--r--   0 rieder     (501) staff       (20)     3994 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.leveque
--rw-r--r--   0 rieder     (501) staff       (20)     3587 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d
--rw-r--r--   0 rieder     (501) staff       (20)     3621 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     3919 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.noh
--rw-r--r--   0 rieder     (501) staff       (20)     2206 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.pgflow
--rw-r--r--   0 rieder     (501) staff       (20)     3263 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.shu-osher
--rw-r--r--   0 rieder     (501) staff       (20)     3947 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.slow-moving-shock
--rw-r--r--   0 rieder     (501) staff       (20)     4004 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod
--rw-r--r--   0 rieder     (501) staff       (20)     3927 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-lw
--rw-r--r--   0 rieder     (501) staff       (20)     3989 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-toro
--rw-r--r--   0 rieder     (501) staff       (20)     4333 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.twoibw
--rwxr-xr-x   0 rieder     (501) staff       (20)     1116 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/run.linear_wave1d
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.667806 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     4222 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.brio-wu
--rw-r--r--   0 rieder     (501) staff       (20)     3728 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cpaw1d
--rw-r--r--   0 rieder     (501) staff       (20)     2195 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cshock1d
--rw-r--r--   0 rieder     (501) staff       (20)     3801 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d
--rw-r--r--   0 rieder     (501) staff       (20)     3604 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     2627 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1a
--rw-r--r--   0 rieder     (501) staff       (20)     2636 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1b
--rw-r--r--   0 rieder     (501) staff       (20)     2650 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2a
--rw-r--r--   0 rieder     (501) staff       (20)     2636 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2b
--rw-r--r--   0 rieder     (501) staff       (20)     2640 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3a
--rw-r--r--   0 rieder     (501) staff       (20)     2608 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3b
--rw-r--r--   0 rieder     (501) staff       (20)     2608 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4a
--rw-r--r--   0 rieder     (501) staff       (20)     2606 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4b
--rw-r--r--   0 rieder     (501) staff       (20)     2608 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4c
--rw-r--r--   0 rieder     (501) staff       (20)     2604 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4d
--rw-r--r--   0 rieder     (501) staff       (20)     4106 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.torrilhon
--rwxr-xr-x   0 rieder     (501) staff       (20)      857 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.cpaw1d
--rwxr-xr-x   0 rieder     (501) staff       (20)     1177 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.linear_wave1d
--rwxr-xr-x   0 rieder     (501) staff       (20)      684 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.test
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.668655 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)     2737 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb1
--rw-r--r--   0 rieder     (501) staff       (20)     2684 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb2
--rw-r--r--   0 rieder     (501) staff       (20)     2684 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb3
--rw-r--r--   0 rieder     (501) staff       (20)     2684 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb4
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.673096 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     4215 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk1
--rw-r--r--   0 rieder     (501) staff       (20)     4215 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk2
--rw-r--r--   0 rieder     (501) staff       (20)     4215 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk3
--rw-r--r--   0 rieder     (501) staff       (20)     3005 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod1
--rw-r--r--   0 rieder     (501) staff       (20)     3006 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod2
--rw-r--r--   0 rieder     (501) staff       (20)     4231 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWoffFRF
--rw-r--r--   0 rieder     (501) staff       (20)     4229 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWonSRF
--rw-r--r--   0 rieder     (501) staff       (20)     4214 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SlowShock
--rw-r--r--   0 rieder     (501) staff       (20)     4230 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.brio-wu
--rw-r--r--   0 rieder     (501) staff       (20)     2986 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub1
--rw-r--r--   0 rieder     (501) staff       (20)     2986 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub2
--rw-r--r--   0 rieder     (501) staff       (20)     2986 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub3
--rw-r--r--   0 rieder     (501) staff       (20)     2986 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub4
--rw-r--r--   0 rieder     (501) staff       (20)     2996 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubcontact
--rw-r--r--   0 rieder     (501) staff       (20)     2999 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubrot
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.675696 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)     3200 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.blast
--rw-r--r--   0 rieder     (501) staff       (20)     2218 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.carbuncle
--rw-r--r--   0 rieder     (501) staff       (20)     3713 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.dmr
--rw-r--r--   0 rieder     (501) staff       (20)     2220 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.jeans
--rw-r--r--   0 rieder     (501) staff       (20)     3968 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.kh
--rw-r--r--   0 rieder     (501) staff       (20)     3894 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d
--rw-r--r--   0 rieder     (501) staff       (20)     3901 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     2824 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.lw_implode
--rw-r--r--   0 rieder     (501) staff       (20)     2582 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.noh
--rw-r--r--   0 rieder     (501) staff       (20)     2519 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.pgflow
--rw-r--r--   0 rieder     (501) staff       (20)     2446 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.rt
--rw-r--r--   0 rieder     (501) staff       (20)     3465 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.shk_cloud
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.679879 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     2742 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.Tconduct
--rw-r--r--   0 rieder     (501) staff       (20)     3498 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B1
--rw-r--r--   0 rieder     (501) staff       (20)     3403 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B10
--rw-r--r--   0 rieder     (501) staff       (20)     4435 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.cpaw2d
--rw-r--r--   0 rieder     (501) staff       (20)     4173 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.field_loop
--rw-r--r--   0 rieder     (501) staff       (20)     2003 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hall_drift
--rw-r--r--   0 rieder     (501) staff       (20)     3498 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hb3
--rw-r--r--   0 rieder     (501) staff       (20)     2848 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.kh
--rw-r--r--   0 rieder     (501) staff       (20)     5173 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d
--rw-r--r--   0 rieder     (501) staff       (20)     3931 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     2598 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.orszag-tang
--rw-r--r--   0 rieder     (501) staff       (20)     2842 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rj2a
--rw-r--r--   0 rieder     (501) staff       (20)     2686 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rotor
--rw-r--r--   0 rieder     (501) staff       (20)     2737 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rt
--rwxr-xr-x   0 rieder     (501) staff       (20)      907 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.cpaw2d
--rwxr-xr-x   0 rieder     (501) staff       (20)     1230 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.linear_wave2d
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.680277 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)     2052 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.blast
--rw-r--r--   0 rieder     (501) staff       (20)     2828 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.jet
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.681372 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     2183 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.blast
--rw-r--r--   0 rieder     (501) staff       (20)     3405 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.brio-wu
--rw-r--r--   0 rieder     (501) staff       (20)     2019 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.current-sheet
--rw-r--r--   0 rieder     (501) staff       (20)     2889 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.jet
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.684503 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)    16800 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-160-FPwave.dat
--rw-r--r--   0 rieder     (501) staff       (20)     4200 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-40-FPwave.dat
--rw-r--r--   0 rieder     (501) staff       (20)     3192 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.blast
--rw-r--r--   0 rieder     (501) staff       (20)     2217 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.carbuncle
--rw-r--r--   0 rieder     (501) staff       (20)     1904 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.fp-wave
--rw-r--r--   0 rieder     (501) staff       (20)     4064 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d
--rw-r--r--   0 rieder     (501) staff       (20)     4056 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     2216 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.nl-shwave
--rw-r--r--   0 rieder     (501) staff       (20)     3078 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.noh
--rw-r--r--   0 rieder     (501) staff       (20)     2364 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.pgflow
--rw-r--r--   0 rieder     (501) staff       (20)     3540 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shk_cloud
--rw-r--r--   0 rieder     (501) staff       (20)     2816 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shwave
--rw-r--r--   0 rieder     (501) staff       (20)     2437 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.turb
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.687481 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     3148 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.Tconduct
--rw-r--r--   0 rieder     (501) staff       (20)     3314 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B1
--rw-r--r--   0 rieder     (501) staff       (20)     3414 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B10
--rw-r--r--   0 rieder     (501) staff       (20)     4527 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.cpaw3d
--rw-r--r--   0 rieder     (501) staff       (20)     4160 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop
--rw-r--r--   0 rieder     (501) staff       (20)     3591 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop4
--rw-r--r--   0 rieder     (501) staff       (20)     2960 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.hgb
--rw-r--r--   0 rieder     (501) staff       (20)     5410 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d
--rw-r--r--   0 rieder     (501) staff       (20)     3999 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     2877 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rj2a_3d
--rw-r--r--   0 rieder     (501) staff       (20)     2200 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rt
--rw-r--r--   0 rieder     (501) staff       (20)     5397 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.strat
--rwxr-xr-x   0 rieder     (501) staff       (20)      964 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.cpaw3d
--rwxr-xr-x   0 rieder     (501) staff       (20)     1317 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.linear_wave3d
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.687660 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)     2913 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/athinput.jet
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.691440 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     2232 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.blast
--rw-r--r--   0 rieder     (501) staff       (20)     2944 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.jet
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.704939 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/
--rw-r--r--   0 rieder     (501) staff       (20)     2952 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2754 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2603 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B0-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2690 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2859 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2820 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2860 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2186 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-1D
--rw-r--r--   0 rieder     (501) staff       (20)     2304 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2422 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2386 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2504 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-3D
--rw-r--r--   0 rieder     (501) staff       (20)     3831 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2677 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-3D
--rw-r--r--   0 rieder     (501) staff       (20)     3249 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylnewtmri
--rw-r--r--   0 rieder     (501) staff       (20)     2390 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylrayleigh-2D
--rw-r--r--   0 rieder     (501) staff       (20)     1803 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylunif-1D
--rw-r--r--   0 rieder     (501) staff       (20)     2112 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-1D
--rw-r--r--   0 rieder     (501) staff       (20)     2245 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2395 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2235 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-1D
--rw-r--r--   0 rieder     (501) staff       (20)     2404 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2486 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2142 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-1D
--rw-r--r--   0 rieder     (501) staff       (20)     2302 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2396 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2499 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.hkdisk-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      838 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cyladvect-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      717 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      690 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      819 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast.mpi-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      792 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylfieldloop-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      682 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylunif-1D
--rwxr-xr-x   0 rieder     (501) staff       (20)      723 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-1D
--rwxr-xr-x   0 rieder     (501) staff       (20)      748 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      849 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-1D
--rwxr-xr-x   0 rieder     (501) staff       (20)      849 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      849 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      731 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-1D
--rwxr-xr-x   0 rieder     (501) staff       (20)      771 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      751 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      852 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-1D
--rwxr-xr-x   0 rieder     (501) staff       (20)      852 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      852 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-3D
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.709746 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/
--rw-r--r--   0 rieder     (501) staff       (20)     2762 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_circ
--rw-r--r--   0 rieder     (501) staff       (20)     3007 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_collision
--rw-r--r--   0 rieder     (501) staff       (20)     2663 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_epicycle
--rw-r--r--   0 rieder     (501) staff       (20)     2535 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_friction
--rw-r--r--   0 rieder     (501) staff       (20)     2894 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave1d
--rw-r--r--   0 rieder     (501) staff       (20)     3079 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave2d
--rw-r--r--   0 rieder     (501) staff       (20)     3184 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave1d
--rw-r--r--   0 rieder     (501) staff       (20)     3148 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave2d
--rw-r--r--   0 rieder     (501) staff       (20)     4321 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat2d
--rw-r--r--   0 rieder     (501) staff       (20)     4348 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat3d
--rw-r--r--   0 rieder     (501) staff       (20)     4057 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_multi
--rw-r--r--   0 rieder     (501) staff       (20)     5158 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_single
--rw-r--r--   0 rieder     (501) staff       (20)     4114 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_multi
--rw-r--r--   0 rieder     (501) staff       (20)     5373 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_single
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.581001 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.710448 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/idl/
--rw-r--r--   0 rieder     (501) staff       (20)      748 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/idl/noh.pro
--rw-r--r--   0 rieder     (501) staff       (20)     1874 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/idl/plotdecay.pro
--rw-r--r--   0 rieder     (501) staff       (20)    13414 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/idl/pltath.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.715885 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/
--rw-r--r--   0 rieder     (501) staff       (20)      334 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/animateppm.m
--rw-r--r--   0 rieder     (501) staff       (20)      508 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_construct_filename.m
--rw-r--r--   0 rieder     (501) staff       (20)     6756 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_getvar.m
--rw-r--r--   0 rieder     (501) staff       (20)      487 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_ijk_to_xyz.m
--rw-r--r--   0 rieder     (501) staff       (20)     5020 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_init_grid.m
--rw-r--r--   0 rieder     (501) staff       (20)     1851 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_ijk.m
--rw-r--r--   0 rieder     (501) staff       (20)     2081 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_xyz.m
--rw-r--r--   0 rieder     (501) staff       (20)     1354 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_palette.m
--rw-r--r--   0 rieder     (501) staff       (20)      723 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_parse_filename.m
--rw-r--r--   0 rieder     (501) staff       (20)      960 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_pcolor.m
--rw-r--r--   0 rieder     (501) staff       (20)      403 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_plotbdry.m
--rw-r--r--   0 rieder     (501) staff       (20)     4338 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_readbin.m
--rw-r--r--   0 rieder     (501) staff       (20)      326 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_sizeof.m
--rw-r--r--   0 rieder     (501) staff       (20)      642 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_ijk.m
--rw-r--r--   0 rieder     (501) staff       (20)     2011 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_xyz.m
--rw-r--r--   0 rieder     (501) staff       (20)     1169 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_text.m
--rw-r--r--   0 rieder     (501) staff       (20)     1196 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_xyz_to_ijk.m
--rw-r--r--   0 rieder     (501) staff       (20)       94 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/displayppm.m
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.716648 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/particle/
--rw-r--r--   0 rieder     (501) staff       (20)     1015 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/particle/Read_par_standard.m
--rw-r--r--   0 rieder     (501) staff       (20)     7217 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/particle/join_lis.c
--rw-r--r--   0 rieder     (501) staff       (20)     1361 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/particle/par_motion_movie.m
--rw-r--r--   0 rieder     (501) staff       (20)     7804 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/particle/sort_lis.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.716828 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/sm/
--rw-r--r--   0 rieder     (501) staff       (20)     7015 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/sm/plot-smr-tab.sm
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.717290 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/vtk/
--rw-r--r--   0 rieder     (501) staff       (20)    19489 2020-03-24 14:36:23.000000 amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/vtk/join_vtk.c
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-04-04 14:19:33.000000 amuse-athena-2023.4.0/src/amuse/community/athena/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:19:35.718901 amuse-athena-2023.4.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2020-03-24 14:36:26.000000 amuse-athena-2023.4.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2021-07-05 11:19:28.000000 amuse-athena-2023.4.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2022-11-30 13:58:15.000000 amuse-athena-2023.4.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2020-03-24 14:36:26.000000 amuse-athena-2023.4.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2020-03-24 14:36:26.000000 amuse-athena-2023.4.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2020-03-24 14:36:26.000000 amuse-athena-2023.4.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2020-03-24 14:36:26.000000 amuse-athena-2023.4.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    50379 2023-04-04 13:47:06.000000 amuse-athena-2023.4.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2021-04-14 10:14:49.000000 amuse-athena-2023.4.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.859997 amuse-athena-2023.5.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-05-17 10:17:29.859819 amuse-athena-2023.5.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       59 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.770409 amuse-athena-2023.5.0/amuse_athena.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-05-17 10:17:28.000000 amuse-athena-2023.5.0/amuse_athena.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)    26055 2023-05-17 10:17:29.000000 amuse-athena-2023.5.0/amuse_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:17:28.000000 amuse-athena-2023.5.0/amuse_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:17:28.000000 amuse-athena-2023.5.0/amuse_athena.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:17:28.000000 amuse-athena-2023.5.0/amuse_athena.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-athena-2023.5.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:17:29.860043 amuse-athena-2023.5.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1777 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.766105 amuse-athena-2023.5.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.766156 amuse-athena-2023.5.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.766209 amuse-athena-2023.5.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.772483 amuse-athena-2023.5.0/src/amuse/community/athena/
+-rw-r--r--   0 rieder     (501) staff       (20)     6368 2023-03-14 13:48:48.000000 amuse-athena-2023.5.0/src/amuse/community/athena/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       30 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1456 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_3.1.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1438 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_4.0.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1438 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_4.1.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)     2212 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/download.py
+-rw-r--r--   0 rieder     (501) staff       (20)    53617 2023-03-14 13:48:48.000000 amuse-athena-2023.5.0/src/amuse/community/athena/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)    21626 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/interface_3.1.c
+-rw-r--r--   0 rieder     (501) staff       (20)    43174 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/interface_4.0.c
+-rw-r--r--   0 rieder     (501) staff       (20)    94883 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/interface_4.1.c
+-rw-r--r--   0 rieder     (501) staff       (20)      908 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/makefile.patch
+-rwxr-xr-x   0 rieder     (501) staff       (20)     2859 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/patch_files.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.766335 amuse-athena-2023.5.0/src/amuse/community/athena/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.773715 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/
+-rw-r--r--   0 rieder     (501) staff       (20)     2428 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)     2720 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/Makeoptions.in
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.774531 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/
+-rw-r--r--   0 rieder     (501) staff       (20)   146872 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/output.0
+-rw-r--r--   0 rieder     (501) staff       (20)     5106 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/requests
+-rw-r--r--   0 rieder     (501) staff       (20)     7765 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/traces.0
+-rwxr-xr-x   0 rieder     (501) staff       (20)   146471 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/configure
+-rw-r--r--   0 rieder     (501) staff       (20)    21424 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/configure.ac
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.774714 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/doc/
+-rw-r--r--   0 rieder     (501) staff       (20)      552 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/doc/pbs-script
+-rwxr-xr-x   0 rieder     (501) staff       (20)     5598 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/install-sh
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.780698 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     4367 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)     4632 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_array.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4098 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_files.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9753 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_log.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2475 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_signal.c
+-rw-r--r--   0 rieder     (501) staff       (20)    22054 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/athena.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3459 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/baton.c
+-rw-r--r--   0 rieder     (501) staff       (20)    96563 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/bvals_mhd.c
+-rw-r--r--   0 rieder     (501) staff       (20)    84875 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/bvals_shear.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5317 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/cc_pos.c
+-rw-r--r--   0 rieder     (501) staff       (20)      433 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/config.h.in
+-rw-r--r--   0 rieder     (501) staff       (20)    35952 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/convert_var.c
+-rw-r--r--   0 rieder     (501) staff       (20)      876 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/copyright.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5237 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/defs.h.in
+-rw-r--r--   0 rieder     (501) staff       (20)     8144 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_binary.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14784 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_history.c
+-rw-r--r--   0 rieder     (501) staff       (20)    15062 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_tab.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10697 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_vtk.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.783120 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/
+-rw-r--r--   0 rieder     (501) staff       (20)    17771 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/LICENSE
+-rw-r--r--   0 rieder     (501) staff       (20)     1545 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    11355 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/ath_fft.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1662 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/factor.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11433 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2348 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.h
+-rw-r--r--   0 rieder     (501) staff       (20)    15253 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2572 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.h
+-rw-r--r--   0 rieder     (501) staff       (20)    10480 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1203 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.h
+-rw-r--r--   0 rieder     (501) staff       (20)    20644 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1552 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3814 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    13200 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2598 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.h
+-rw-r--r--   0 rieder     (501) staff       (20)    15313 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2640 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3524 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/globals.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.784176 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/
+-rw-r--r--   0 rieder     (501) staff       (20)     1287 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    40334 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/bvals_grav.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1539 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    20655 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10585 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft.c
+-rw-r--r--   0 rieder     (501) staff       (20)    17807 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft_obc.c
+-rw-r--r--   0 rieder     (501) staff       (20)    35053 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_multigrid.c
+-rw-r--r--   0 rieder     (501) staff       (20)    48007 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/init_grid.c
+-rw-r--r--   0 rieder     (501) staff       (20)    37805 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/init_mesh.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.786162 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/
+-rw-r--r--   0 rieder     (501) staff       (20)     1466 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)     3239 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate.c
+-rw-r--r--   0 rieder     (501) staff       (20)    22956 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_ctu.c
+-rw-r--r--   0 rieder     (501) staff       (20)    15882 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl.c
+-rw-r--r--   0 rieder     (501) staff       (20)    22889 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)    73042 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_ctu.c
+-rw-r--r--   0 rieder     (501) staff       (20)    48617 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl.c
+-rw-r--r--   0 rieder     (501) staff       (20)    54176 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)   138756 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_ctu.c
+-rw-r--r--   0 rieder     (501) staff       (20)    79851 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl.c
+-rw-r--r--   0 rieder     (501) staff       (20)    84225 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1151 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    28050 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/main.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.787490 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/
+-rw-r--r--   0 rieder     (501) staff       (20)     1355 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    13039 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/conduction.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2773 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/cool.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3252 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/diff_dt.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4491 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/get_eta.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3299 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/integrate_diffusion.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1606 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    45134 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/resistivity.c
+-rw-r--r--   0 rieder     (501) staff       (20)    26948 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/viscosity.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5855 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/new_dt.c
+-rw-r--r--   0 rieder     (501) staff       (20)    45790 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11218 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_pdf.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4214 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_pgm.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5464 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_ppm.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8395 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_tab.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8403 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_vtk.c
+-rw-r--r--   0 rieder     (501) staff       (20)    65505 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/palette.h
+-rw-r--r--   0 rieder     (501) staff       (20)    31102 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/par.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.789009 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/
+-rw-r--r--   0 rieder     (501) staff       (20)     1326 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    87780 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/bvals_particle.c
+-rw-r--r--   0 rieder     (501) staff       (20)    13665 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/dump_particle_history.c
+-rw-r--r--   0 rieder     (501) staff       (20)    41179 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/feedback.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9078 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/init_particle.c
+-rw-r--r--   0 rieder     (501) staff       (20)    29582 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/integrators_particle.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11513 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/output_particle.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1491 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/particle.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3799 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    23052 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/utils_particle.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.822698 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/
+-rw-r--r--   0 rieder     (501) staff       (20)     4565 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/README
+-rw-r--r--   0 rieder     (501) staff       (20)     3503 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/blast.c
+-rw-r--r--   0 rieder     (501) staff       (20)    15849 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/bubble.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6022 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/carbuncle.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7857 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/collapse3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9095 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12810 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    17446 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8063 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cshock1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3295 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/current_sheet.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9456 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cyladvect.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6663 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylblast.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6283 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylbphi.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9325 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylbr.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7401 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylfieldloop.c
+-rw-r--r--   0 rieder     (501) staff       (20)    25462 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylnewtmri.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5379 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylrayleigh.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6349 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylunif.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6362 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwind.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6841 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwindrot.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8182 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwindrotb.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7564 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/dmr.c
+-rw-r--r--   0 rieder     (501) staff       (20)    13562 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/field_loop.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12054 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/firehose.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4867 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hall_drift.c
+-rw-r--r--   0 rieder     (501) staff       (20)    16086 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hb3.c
+-rw-r--r--   0 rieder     (501) staff       (20)    25056 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hgb.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12816 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hkdisk.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6137 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/jeans.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7058 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/jet.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8274 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/kh.c
+-rw-r--r--   0 rieder     (501) staff       (20)    17209 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    18726 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    21769 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3693 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/lw_implode.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7336 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/noh.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4220 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/orszag-tang.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14369 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_circ.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10895 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_collision.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9861 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_epicycle.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8447 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_friction.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12838 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11854 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14766 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_shwave1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12434 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_shwave2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    27638 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_strat2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    27921 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_strat3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10544 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/pgflow.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12411 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/planet-disk.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4045 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/rotor.c
+-rw-r--r--   0 rieder     (501) staff       (20)    20876 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/rt.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8808 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shk_cloud.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7338 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14921 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    30745 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3250 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shu-osher.c
+-rw-r--r--   0 rieder     (501) staff       (20)    41891 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/strat.c
+-rw-r--r--   0 rieder     (501) staff       (20)    19916 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_multi.c
+-rw-r--r--   0 rieder     (501) staff       (20)    25339 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_single.c
+-rw-r--r--   0 rieder     (501) staff       (20)    20516 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_multi.c
+-rw-r--r--   0 rieder     (501) staff       (20)    25902 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_single.c
+-rw-r--r--   0 rieder     (501) staff       (20)    20966 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/ti.c
+-rw-r--r--   0 rieder     (501) staff       (20)    24287 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/turb.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4145 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/twoibw.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10180 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prototypes.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.823952 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/
+-rw-r--r--   0 rieder     (501) staff       (20)     1343 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    18745 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/esystem_prim.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2581 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_dc.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12889 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_plm.c
+-rw-r--r--   0 rieder     (501) staff       (20)    22476 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_ppm.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11888 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim2.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14242 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim3.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1755 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    27483 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/restart.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.826355 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/
+-rw-r--r--   0 rieder     (501) staff       (20)     1343 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    22384 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/esystem_roe.c
+-rw-r--r--   0 rieder     (501) staff       (20)    20557 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/exact.c
+-rw-r--r--   0 rieder     (501) staff       (20)    28427 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/exact_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8082 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/force.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6545 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc.c
+-rw-r--r--   0 rieder     (501) staff       (20)    30910 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)    21397 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld.c
+-rw-r--r--   0 rieder     (501) staff       (20)    33705 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7683 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle.c
+-rw-r--r--   0 rieder     (501) staff       (20)    19191 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1706 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)     9544 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/roe.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3816 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/two_shock.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10463 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/show_config.c
+-rw-r--r--   0 rieder     (501) staff       (20)    85682 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/smr.c
+-rw-r--r--   0 rieder     (501) staff       (20)    32081 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/utils.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.768186 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.829004 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)     3986 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1125
+-rw-r--r--   0 rieder     (501) staff       (20)     3985 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1203
+-rw-r--r--   0 rieder     (501) staff       (20)     3994 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.leveque
+-rw-r--r--   0 rieder     (501) staff       (20)     3587 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d
+-rw-r--r--   0 rieder     (501) staff       (20)     3621 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     3919 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.noh
+-rw-r--r--   0 rieder     (501) staff       (20)     2206 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.pgflow
+-rw-r--r--   0 rieder     (501) staff       (20)     3263 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.shu-osher
+-rw-r--r--   0 rieder     (501) staff       (20)     3947 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.slow-moving-shock
+-rw-r--r--   0 rieder     (501) staff       (20)     4004 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod
+-rw-r--r--   0 rieder     (501) staff       (20)     3927 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-lw
+-rw-r--r--   0 rieder     (501) staff       (20)     3989 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-toro
+-rw-r--r--   0 rieder     (501) staff       (20)     4333 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.twoibw
+-rwxr-xr-x   0 rieder     (501) staff       (20)     1116 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/run.linear_wave1d
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.831982 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     4222 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.brio-wu
+-rw-r--r--   0 rieder     (501) staff       (20)     3728 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cpaw1d
+-rw-r--r--   0 rieder     (501) staff       (20)     2195 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cshock1d
+-rw-r--r--   0 rieder     (501) staff       (20)     3801 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d
+-rw-r--r--   0 rieder     (501) staff       (20)     3604 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     2627 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1a
+-rw-r--r--   0 rieder     (501) staff       (20)     2636 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1b
+-rw-r--r--   0 rieder     (501) staff       (20)     2650 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2a
+-rw-r--r--   0 rieder     (501) staff       (20)     2636 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2b
+-rw-r--r--   0 rieder     (501) staff       (20)     2640 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3a
+-rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3b
+-rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4a
+-rw-r--r--   0 rieder     (501) staff       (20)     2606 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4b
+-rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4c
+-rw-r--r--   0 rieder     (501) staff       (20)     2604 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4d
+-rw-r--r--   0 rieder     (501) staff       (20)     4106 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.torrilhon
+-rwxr-xr-x   0 rieder     (501) staff       (20)      857 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.cpaw1d
+-rwxr-xr-x   0 rieder     (501) staff       (20)     1177 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.linear_wave1d
+-rwxr-xr-x   0 rieder     (501) staff       (20)      684 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.test
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.832581 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)     2737 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb1
+-rw-r--r--   0 rieder     (501) staff       (20)     2684 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb2
+-rw-r--r--   0 rieder     (501) staff       (20)     2684 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb3
+-rw-r--r--   0 rieder     (501) staff       (20)     2684 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb4
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.834906 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     4215 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk1
+-rw-r--r--   0 rieder     (501) staff       (20)     4215 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk2
+-rw-r--r--   0 rieder     (501) staff       (20)     4215 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk3
+-rw-r--r--   0 rieder     (501) staff       (20)     3005 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod1
+-rw-r--r--   0 rieder     (501) staff       (20)     3006 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod2
+-rw-r--r--   0 rieder     (501) staff       (20)     4231 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWoffFRF
+-rw-r--r--   0 rieder     (501) staff       (20)     4229 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWonSRF
+-rw-r--r--   0 rieder     (501) staff       (20)     4214 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SlowShock
+-rw-r--r--   0 rieder     (501) staff       (20)     4230 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.brio-wu
+-rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub1
+-rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub2
+-rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub3
+-rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub4
+-rw-r--r--   0 rieder     (501) staff       (20)     2996 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubcontact
+-rw-r--r--   0 rieder     (501) staff       (20)     2999 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubrot
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.836683 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)     3200 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.blast
+-rw-r--r--   0 rieder     (501) staff       (20)     2218 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.carbuncle
+-rw-r--r--   0 rieder     (501) staff       (20)     3713 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.dmr
+-rw-r--r--   0 rieder     (501) staff       (20)     2220 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.jeans
+-rw-r--r--   0 rieder     (501) staff       (20)     3968 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.kh
+-rw-r--r--   0 rieder     (501) staff       (20)     3894 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d
+-rw-r--r--   0 rieder     (501) staff       (20)     3901 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     2824 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.lw_implode
+-rw-r--r--   0 rieder     (501) staff       (20)     2582 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.noh
+-rw-r--r--   0 rieder     (501) staff       (20)     2519 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.pgflow
+-rw-r--r--   0 rieder     (501) staff       (20)     2446 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.rt
+-rw-r--r--   0 rieder     (501) staff       (20)     3465 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.shk_cloud
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.838905 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     2742 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.Tconduct
+-rw-r--r--   0 rieder     (501) staff       (20)     3498 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B1
+-rw-r--r--   0 rieder     (501) staff       (20)     3403 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B10
+-rw-r--r--   0 rieder     (501) staff       (20)     4435 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.cpaw2d
+-rw-r--r--   0 rieder     (501) staff       (20)     4173 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.field_loop
+-rw-r--r--   0 rieder     (501) staff       (20)     2003 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hall_drift
+-rw-r--r--   0 rieder     (501) staff       (20)     3498 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hb3
+-rw-r--r--   0 rieder     (501) staff       (20)     2848 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.kh
+-rw-r--r--   0 rieder     (501) staff       (20)     5173 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d
+-rw-r--r--   0 rieder     (501) staff       (20)     3931 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     2598 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.orszag-tang
+-rw-r--r--   0 rieder     (501) staff       (20)     2842 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rj2a
+-rw-r--r--   0 rieder     (501) staff       (20)     2686 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rotor
+-rw-r--r--   0 rieder     (501) staff       (20)     2737 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rt
+-rwxr-xr-x   0 rieder     (501) staff       (20)      907 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.cpaw2d
+-rwxr-xr-x   0 rieder     (501) staff       (20)     1230 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.linear_wave2d
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.839181 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)     2052 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.blast
+-rw-r--r--   0 rieder     (501) staff       (20)     2828 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.jet
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.839736 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     2183 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.blast
+-rw-r--r--   0 rieder     (501) staff       (20)     3405 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.brio-wu
+-rw-r--r--   0 rieder     (501) staff       (20)     2019 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.current-sheet
+-rw-r--r--   0 rieder     (501) staff       (20)     2889 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.jet
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.841681 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)    16800 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-160-FPwave.dat
+-rw-r--r--   0 rieder     (501) staff       (20)     4200 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-40-FPwave.dat
+-rw-r--r--   0 rieder     (501) staff       (20)     3192 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.blast
+-rw-r--r--   0 rieder     (501) staff       (20)     2217 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.carbuncle
+-rw-r--r--   0 rieder     (501) staff       (20)     1904 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.fp-wave
+-rw-r--r--   0 rieder     (501) staff       (20)     4064 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d
+-rw-r--r--   0 rieder     (501) staff       (20)     4056 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     2216 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.nl-shwave
+-rw-r--r--   0 rieder     (501) staff       (20)     3078 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.noh
+-rw-r--r--   0 rieder     (501) staff       (20)     2364 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.pgflow
+-rw-r--r--   0 rieder     (501) staff       (20)     3540 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shk_cloud
+-rw-r--r--   0 rieder     (501) staff       (20)     2816 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shwave
+-rw-r--r--   0 rieder     (501) staff       (20)     2437 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.turb
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.844266 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     3148 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.Tconduct
+-rw-r--r--   0 rieder     (501) staff       (20)     3314 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B1
+-rw-r--r--   0 rieder     (501) staff       (20)     3414 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B10
+-rw-r--r--   0 rieder     (501) staff       (20)     4527 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.cpaw3d
+-rw-r--r--   0 rieder     (501) staff       (20)     4160 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop
+-rw-r--r--   0 rieder     (501) staff       (20)     3591 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop4
+-rw-r--r--   0 rieder     (501) staff       (20)     2960 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.hgb
+-rw-r--r--   0 rieder     (501) staff       (20)     5410 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d
+-rw-r--r--   0 rieder     (501) staff       (20)     3999 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     2877 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rj2a_3d
+-rw-r--r--   0 rieder     (501) staff       (20)     2200 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rt
+-rw-r--r--   0 rieder     (501) staff       (20)     5397 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.strat
+-rwxr-xr-x   0 rieder     (501) staff       (20)      964 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.cpaw3d
+-rwxr-xr-x   0 rieder     (501) staff       (20)     1317 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.linear_wave3d
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.844407 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)     2913 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/athinput.jet
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.844690 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     2232 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.blast
+-rw-r--r--   0 rieder     (501) staff       (20)     2944 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.jet
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.851225 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/
+-rw-r--r--   0 rieder     (501) staff       (20)     2952 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2754 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2603 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B0-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2690 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2859 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2820 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2860 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2186 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-1D
+-rw-r--r--   0 rieder     (501) staff       (20)     2304 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2422 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2386 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2504 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     3831 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2677 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     3249 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylnewtmri
+-rw-r--r--   0 rieder     (501) staff       (20)     2390 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylrayleigh-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     1803 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylunif-1D
+-rw-r--r--   0 rieder     (501) staff       (20)     2112 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-1D
+-rw-r--r--   0 rieder     (501) staff       (20)     2245 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2395 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2235 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-1D
+-rw-r--r--   0 rieder     (501) staff       (20)     2404 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2486 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2142 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-1D
+-rw-r--r--   0 rieder     (501) staff       (20)     2302 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2396 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2499 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.hkdisk-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      838 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cyladvect-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      717 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      690 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      819 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast.mpi-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      792 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylfieldloop-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      682 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylunif-1D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      723 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-1D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      748 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      849 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-1D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      849 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      849 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      731 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-1D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      771 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      751 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      852 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-1D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      852 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      852 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-3D
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.853635 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/
+-rw-r--r--   0 rieder     (501) staff       (20)     2762 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_circ
+-rw-r--r--   0 rieder     (501) staff       (20)     3007 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_collision
+-rw-r--r--   0 rieder     (501) staff       (20)     2663 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_epicycle
+-rw-r--r--   0 rieder     (501) staff       (20)     2535 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_friction
+-rw-r--r--   0 rieder     (501) staff       (20)     2894 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave1d
+-rw-r--r--   0 rieder     (501) staff       (20)     3079 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave2d
+-rw-r--r--   0 rieder     (501) staff       (20)     3184 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave1d
+-rw-r--r--   0 rieder     (501) staff       (20)     3148 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave2d
+-rw-r--r--   0 rieder     (501) staff       (20)     4321 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat2d
+-rw-r--r--   0 rieder     (501) staff       (20)     4348 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat3d
+-rw-r--r--   0 rieder     (501) staff       (20)     4057 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_multi
+-rw-r--r--   0 rieder     (501) staff       (20)     5158 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_single
+-rw-r--r--   0 rieder     (501) staff       (20)     4114 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_multi
+-rw-r--r--   0 rieder     (501) staff       (20)     5373 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_single
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.768885 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.854202 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/
+-rw-r--r--   0 rieder     (501) staff       (20)      748 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/noh.pro
+-rw-r--r--   0 rieder     (501) staff       (20)     1874 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/plotdecay.pro
+-rw-r--r--   0 rieder     (501) staff       (20)    13414 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/pltath.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.857278 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/
+-rw-r--r--   0 rieder     (501) staff       (20)      334 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/animateppm.m
+-rw-r--r--   0 rieder     (501) staff       (20)      508 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_construct_filename.m
+-rw-r--r--   0 rieder     (501) staff       (20)     6756 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_getvar.m
+-rw-r--r--   0 rieder     (501) staff       (20)      487 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_ijk_to_xyz.m
+-rw-r--r--   0 rieder     (501) staff       (20)     5020 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_init_grid.m
+-rw-r--r--   0 rieder     (501) staff       (20)     1851 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_ijk.m
+-rw-r--r--   0 rieder     (501) staff       (20)     2081 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_xyz.m
+-rw-r--r--   0 rieder     (501) staff       (20)     1354 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_palette.m
+-rw-r--r--   0 rieder     (501) staff       (20)      723 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_parse_filename.m
+-rw-r--r--   0 rieder     (501) staff       (20)      960 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_pcolor.m
+-rw-r--r--   0 rieder     (501) staff       (20)      403 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_plotbdry.m
+-rw-r--r--   0 rieder     (501) staff       (20)     4338 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_readbin.m
+-rw-r--r--   0 rieder     (501) staff       (20)      326 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_sizeof.m
+-rw-r--r--   0 rieder     (501) staff       (20)      642 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_ijk.m
+-rw-r--r--   0 rieder     (501) staff       (20)     2011 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_xyz.m
+-rw-r--r--   0 rieder     (501) staff       (20)     1169 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_text.m
+-rw-r--r--   0 rieder     (501) staff       (20)     1196 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_xyz_to_ijk.m
+-rw-r--r--   0 rieder     (501) staff       (20)       94 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/displayppm.m
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.857955 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/
+-rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/Read_par_standard.m
+-rw-r--r--   0 rieder     (501) staff       (20)     7217 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/join_lis.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1361 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/par_motion_movie.m
+-rw-r--r--   0 rieder     (501) staff       (20)     7804 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/sort_lis.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.858121 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/sm/
+-rw-r--r--   0 rieder     (501) staff       (20)     7015 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/sm/plot-smr-tab.sm
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.858285 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/vtk/
+-rw-r--r--   0 rieder     (501) staff       (20)    19489 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/vtk/join_vtk.c
+-rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:17:28.000000 amuse-athena-2023.5.0/src/amuse/community/athena/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.859584 amuse-athena-2023.5.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-athena-2023.5.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-athena-2023.5.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/version.py
```

### Comparing `amuse-athena-2023.4.0/PKG-INFO` & `amuse-athena-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-athena
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: The Astrophysical Multipurpose Software Environment - Athena
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `amuse-athena-2023.4.0/amuse_athena.egg-info/PKG-INFO` & `amuse-athena-2023.5.0/amuse_athena.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-athena
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: The Astrophysical Multipurpose Software Environment - Athena
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `amuse-athena-2023.4.0/amuse_athena.egg-info/SOURCES.txt` & `amuse-athena-2023.5.0/amuse_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/setup.py` & `amuse-athena-2023.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/Makefile` & `amuse-athena-2023.5.0/src/amuse/community/athena/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/amuse_problem_3.1.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_3.1.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/amuse_problem_4.0.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_4.0.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/amuse_problem_4.1.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_4.1.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/download.py` & `amuse-athena-2023.5.0/src/amuse/community/athena/download.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/interface.py` & `amuse-athena-2023.5.0/src/amuse/community/athena/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/interface_3.1.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/interface_3.1.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/interface_4.0.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/interface_4.0.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/interface_4.1.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/interface_4.1.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/makefile.patch` & `amuse-athena-2023.5.0/src/amuse/community/athena/makefile.patch`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/patch_files.py` & `amuse-athena-2023.5.0/src/amuse/community/athena/patch_files.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/Makefile.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/Makeoptions.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/Makeoptions.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/autom4te.cache/output.0` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/output.0`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/autom4te.cache/requests` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/requests`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/autom4te.cache/traces.0` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/traces.0`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/configure` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/configure`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/configure.ac` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/configure.ac`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/doc/pbs-script` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/doc/pbs-script`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/install-sh` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/install-sh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/Makefile.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/ath_array.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_array.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/ath_files.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_files.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/ath_log.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_log.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/ath_signal.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_signal.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/athena.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/athena.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/baton.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/baton.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/bvals_mhd.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/bvals_mhd.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/bvals_shear.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/bvals_shear.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/cc_pos.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/cc_pos.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/convert_var.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/convert_var.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/copyright.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/copyright.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/defs.h.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/defs.h.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/dump_binary.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_binary.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/dump_history.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_history.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/dump_tab.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_tab.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/dump_vtk.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_vtk.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/LICENSE` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/LICENSE`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/Makefile.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/ath_fft.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/ath_fft.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/factor.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/factor.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/prototypes.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/globals.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/globals.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/Makefile.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/bvals_grav.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/bvals_grav.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/prototypes.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft_obc.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft_obc.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_multigrid.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_multigrid.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/init_grid.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/init_grid.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/init_mesh.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/init_mesh.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/Makefile.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_ctu.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_ctu.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl_sr.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_ctu.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_ctu.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl_sr.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_ctu.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_ctu.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl_sr.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/integrators/prototypes.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/main.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/main.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/Makefile.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/conduction.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/conduction.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/cool.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/cool.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/diff_dt.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/diff_dt.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/get_eta.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/get_eta.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/integrate_diffusion.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/integrate_diffusion.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/prototypes.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/resistivity.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/resistivity.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/microphysics/viscosity.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/viscosity.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/new_dt.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/new_dt.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output_pdf.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_pdf.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output_pgm.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_pgm.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output_ppm.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_ppm.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output_tab.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_tab.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/output_vtk.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_vtk.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/palette.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/palette.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/par.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/par.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/Makefile.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/bvals_particle.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/bvals_particle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/dump_particle_history.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/dump_particle_history.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/feedback.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/feedback.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/init_particle.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/init_particle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/integrators_particle.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/integrators_particle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/output_particle.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/output_particle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/particle.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/particle.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/prototypes.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/particles/utils_particle.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/utils_particle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/README` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/README`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/blast.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/blast.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/bubble.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/bubble.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/carbuncle.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/carbuncle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/collapse3d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/collapse3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw1d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw2d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw3d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cshock1d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cshock1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/current_sheet.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/current_sheet.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cyladvect.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cyladvect.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylblast.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylblast.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylbphi.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylbphi.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylbr.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylbr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylfieldloop.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylfieldloop.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylnewtmri.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylnewtmri.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylrayleigh.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylrayleigh.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylunif.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylunif.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylwind.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwind.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylwindrot.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwindrot.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/cylwindrotb.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwindrotb.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/dmr.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/dmr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/field_loop.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/field_loop.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/firehose.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/firehose.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/hall_drift.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hall_drift.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/hb3.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hb3.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/hgb.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hgb.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/hkdisk.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hkdisk.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/jeans.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/jeans.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/jet.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/jet.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/kh.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/kh.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave1d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave2d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave3d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/lw_implode.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/lw_implode.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/noh.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/noh.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/orszag-tang.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/orszag-tang.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_circ.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_circ.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_collision.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_collision.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_epicycle.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_epicycle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_friction.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_friction.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave1d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave2d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_shwave1d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_shwave1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_shwave2d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_shwave2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_strat2d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_strat2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/par_strat3d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_strat3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/pgflow.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/pgflow.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/planet-disk.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/planet-disk.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/rotor.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/rotor.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/rt.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/rt.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/shk_cloud.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shk_cloud.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/shkset1d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/shkset2d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/shkset3d.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/shu-osher.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shu-osher.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/strat.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/strat.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_multi.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_multi.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_single.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_single.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_multi.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_multi.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_single.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_single.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/ti.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/ti.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/turb.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/turb.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prob/twoibw.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/twoibw.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/prototypes.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/Makefile.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/esystem_prim.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/esystem_prim.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_dc.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_dc.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_plm.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_plm.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_ppm.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_ppm.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim2.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim2.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim3.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim3.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/reconstruction/prototypes.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/restart.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/restart.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/Makefile.in` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/esystem_roe.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/esystem_roe.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/exact.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/exact.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/exact_sr.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/exact_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/force.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/force.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc_sr.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld_sr.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle_sr.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/prototypes.h` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/roe.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/roe.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/rsolvers/two_shock.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/two_shock.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/show_config.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/show_config.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/smr.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/smr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/src/utils.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/utils.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1125` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1125`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1203` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1203`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.leveque` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.leveque`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d-3lev1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.noh` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.noh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.pgflow` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.pgflow`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.shu-osher` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.shu-osher`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.slow-moving-shock` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.slow-moving-shock`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-lw` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-lw`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-toro` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-toro`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.twoibw` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.twoibw`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/run.linear_wave1d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/run.linear_wave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.brio-wu` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.brio-wu`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cpaw1d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cpaw1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cshock1d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cshock1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d-3lev1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1a` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1a`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1b` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1b`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2a` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2a`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2b` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2b`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3a` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3a`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3b` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3b`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4a` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4a`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4b` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4b`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.torrilhon` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.torrilhon`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.cpaw1d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.cpaw1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.linear_wave1d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.linear_wave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.test` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.test`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb2` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb2`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb3` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb3`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb4` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb4`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk2` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk2`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk3` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk3`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod2` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod2`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWoffFRF` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWoffFRF`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWonSRF` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWonSRF`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SlowShock` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SlowShock`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.brio-wu` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.brio-wu`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub2` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub2`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub3` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub3`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub4` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub4`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubcontact` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubcontact`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubrot` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubrot`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.blast` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.blast`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.carbuncle` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.carbuncle`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.dmr` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.dmr`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.jeans` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.jeans`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.kh` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.kh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d-3lev1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.lw_implode` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.lw_implode`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.noh` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.noh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.pgflow` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.pgflow`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.rt` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.rt`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.shk_cloud` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.shk_cloud`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.Tconduct` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.Tconduct`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B10` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B10`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.cpaw2d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.cpaw2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.field_loop` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.field_loop`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hall_drift` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hall_drift`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hb3` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hb3`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.kh` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.kh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d-3lev1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.orszag-tang` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.orszag-tang`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rj2a` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rj2a`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rotor` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rotor`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rt` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rt`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.cpaw2d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.cpaw2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.linear_wave2d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.linear_wave2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.blast` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.blast`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.jet` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.jet`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.blast` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.blast`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.brio-wu` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.brio-wu`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.current-sheet` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.current-sheet`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.jet` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.jet`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-160-FPwave.dat` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-160-FPwave.dat`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-40-FPwave.dat` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-40-FPwave.dat`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.blast` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.blast`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.carbuncle` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.carbuncle`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.fp-wave` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.fp-wave`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d-3lev1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.nl-shwave` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.nl-shwave`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.noh` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.noh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.pgflow` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.pgflow`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shk_cloud` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shk_cloud`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shwave` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shwave`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.turb` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.turb`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.Tconduct` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.Tconduct`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B10` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B10`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.cpaw3d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.cpaw3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop4` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop4`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.hgb` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.hgb`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d-3lev1` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rj2a_3d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rj2a_3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rt` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rt`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.strat` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.strat`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.cpaw3d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.cpaw3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.linear_wave3d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.linear_wave3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/athinput.jet` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/athinput.jet`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.blast` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.blast`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.jet` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.jet`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B0-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B0-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-1D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylnewtmri` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylnewtmri`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylrayleigh-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylrayleigh-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylunif-1D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylunif-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-1D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-1D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-1D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.hkdisk-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.hkdisk-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cyladvect-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cyladvect-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast.mpi-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast.mpi-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylfieldloop-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylfieldloop-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylunif-1D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylunif-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-1D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-1D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-1D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-1D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-2D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-3D` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_circ` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_circ`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_collision` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_collision`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_epicycle` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_epicycle`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_friction` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_friction`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave1d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave2d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave1d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave2d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat2d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat3d` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_multi` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_multi`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_single` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_single`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_multi` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_multi`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_single` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_single`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/idl/noh.pro` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/noh.pro`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/idl/plotdecay.pro` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/plotdecay.pro`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/idl/pltath.pro` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/pltath.pro`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_getvar.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_getvar.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_init_grid.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_init_grid.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_ijk.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_ijk.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_xyz.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_xyz.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_palette.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_palette.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_parse_filename.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_parse_filename.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_pcolor.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_pcolor.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_readbin.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_readbin.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_ijk.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_ijk.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_xyz.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_xyz.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_text.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_text.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_xyz_to_ijk.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_xyz_to_ijk.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/particle/Read_par_standard.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/Read_par_standard.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/particle/join_lis.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/join_lis.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/particle/par_motion_movie.m` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/par_motion_movie.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/particle/sort_lis.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/sort_lis.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/sm/plot-smr-tab.sm` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/sm/plot-smr-tab.sm`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/src/amuse/community/athena/src/athena/vis/vtk/join_vtk.c` & `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/vtk/join_vtk.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/support/__init__.py` & `amuse-athena-2023.5.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/support/classifiers.py` & `amuse-athena-2023.5.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/support/config.py` & `amuse-athena-2023.5.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/support/generate_main.py` & `amuse-athena-2023.5.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/support/getsp.class` & `amuse-athena-2023.5.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/support/getsp.java` & `amuse-athena-2023.5.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/support/misc.py` & `amuse-athena-2023.5.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.4.0/support/setup_codes.py` & `amuse-athena-2023.5.0/support/setup_codes.py`

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

