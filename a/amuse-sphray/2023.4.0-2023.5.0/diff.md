# Comparing `tmp/amuse-sphray-2023.4.0.tar.gz` & `tmp/amuse-sphray-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-sphray-2023.4.0.tar", last modified: Tue Apr  4 14:22:36 2023, max compression
+gzip compressed data, was "amuse-sphray-2023.5.0.tar", last modified: Wed May 17 10:19:47 2023, max compression
```

## Comparing `amuse-sphray-2023.4.0.tar` & `amuse-sphray-2023.5.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:36.049568 amuse-sphray-2023.4.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2020-03-24 14:36:23.000000 amuse-sphray-2023.4.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-04-04 14:22:36.049374 amuse-sphray-2023.4.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       59 2020-03-24 14:36:23.000000 amuse-sphray-2023.4.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:35.996978 amuse-sphray-2023.4.0/amuse_sphray.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-04-04 14:22:33.000000 amuse-sphray-2023.4.0/amuse_sphray.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     6112 2023-04-04 14:22:35.000000 amuse-sphray-2023.4.0/amuse_sphray.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-04-04 14:22:33.000000 amuse-sphray-2023.4.0/amuse_sphray.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-04-04 14:22:33.000000 amuse-sphray-2023.4.0/amuse_sphray.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-04-04 14:22:33.000000 amuse-sphray-2023.4.0/amuse_sphray.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       71 2020-03-24 14:36:23.000000 amuse-sphray-2023.4.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-04-04 14:22:36.049629 amuse-sphray-2023.4.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1777 2021-04-23 11:09:14.000000 amuse-sphray-2023.4.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:35.993705 amuse-sphray-2023.4.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:35.993764 amuse-sphray-2023.4.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:35.993818 amuse-sphray-2023.4.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:35.998199 amuse-sphray-2023.4.0/src/amuse/community/sphray/
--rw-r--r--   0 rieder     (501) staff       (20)     1393 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       30 2022-10-03 08:52:42.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:35.993953 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:35.999778 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:36.007612 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/
--rw-r--r--   0 rieder     (501) staff       (20)   786348 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates.txt
--rw-r--r--   0 rieder     (501) staff       (20)   786348 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Cen.txt
--rw-r--r--   0 rieder     (501) staff       (20)   786348 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hui.txt
--rw-r--r--   0 rieder     (501) staff       (20)   785996 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hum.txt
--rw-r--r--   0 rieder     (501) staff       (20)   786348 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Vor.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:36.009466 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/column_depth/
--rw-r--r--   0 rieder     (501) staff       (20)     1288 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/column_depth/latmon_b2cd_table.txt
--rw-r--r--   0 rieder     (501) staff       (20)     1288 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/column_depth/tophat_b2cd_table.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:36.010479 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/spectra/
--rw-r--r--   0 rieder     (501) staff       (20)    49123 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/spectra/power2.0.cdf
--rw-r--r--   0 rieder     (501) staff       (20)    49123 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/spectra/power4.0.cdf
--rw-r--r--   0 rieder     (501) staff       (20)    49123 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/spectra/thermal1e5.cdf
--rw-r--r--   0 rieder     (501) staff       (20)    49123 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/spectra/thermal6e4.cdf
--rw-r--r--   0 rieder     (501) staff       (20)   370256 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/sphray_4K
--rw-r--r--   0 rieder     (501) staff       (20)       70 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/test1_sources_001.1
--rw-r--r--   0 rieder     (501) staff       (20)       69 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/test2_sources_001.1
--rw-r--r--   0 rieder     (501) staff       (20)     9907 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/interface.f90
--rw-r--r--   0 rieder     (501) staff       (20)    35232 2023-04-04 13:47:06.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/interface.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:36.033381 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/
--rw-r--r--   0 rieder     (501) staff       (20)     9708 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     8945 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/MakefileTemplate
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:36.042358 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/
--rw-r--r--   0 rieder     (501) staff       (20)    71467 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/GL.h
--rw-r--r--   0 rieder     (501) staff       (20)    16543 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/GLU.h
--rw-r--r--   0 rieder     (501) staff       (20)    19786 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/GLUT.h
--rw-r--r--   0 rieder     (501) staff       (20)      536 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/GLUT_fonts.c
--rw-r--r--   0 rieder     (501) staff       (20)    68448 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_freeglut.F90
--rw-r--r--   0 rieder     (501) staff       (20)   194062 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_gl.F90
--rw-r--r--   0 rieder     (501) staff       (20)    41410 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glu.F90
--rw-r--r--   0 rieder     (501) staff       (20)    56657 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glut.F90
--rw-r--r--   0 rieder     (501) staff       (20)    67729 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_openglut.F90
--rw-r--r--   0 rieder     (501) staff       (20)     1091 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/fthread.f
--rw-r--r--   0 rieder     (501) staff       (20)     6077 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/pt.c
--rw-r--r--   0 rieder     (501) staff       (20)     6831 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/pt.h
--rw-r--r--   0 rieder     (501) staff       (20)     1018 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/ptf77.c
--rw-r--r--   0 rieder     (501) staff       (20)    33052 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/amuse_helpers.F90
--rw-r--r--   0 rieder     (501) staff       (20)     5354 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/amuse_mainloop.F90
--rw-r--r--   0 rieder     (501) staff       (20)    25577 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/atomic_rates.F90
--rw-r--r--   0 rieder     (501) staff       (20)     3995 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/b2cd.F90
--rw-r--r--   0 rieder     (501) staff       (20)     8804 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/bdf.F90
--rw-r--r--   0 rieder     (501) staff       (20)    14046 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/cen_atomic_rates.F90
--rw-r--r--   0 rieder     (501) staff       (20)    23703 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/config.F90
--rw-r--r--   0 rieder     (501) staff       (20)     2264 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/cosmology.F90
--rw-r--r--   0 rieder     (501) staff       (20)     7761 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/density_test.F90
--rw-r--r--   0 rieder     (501) staff       (20)    12191 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/euler.F90
--rw-r--r--   0 rieder     (501) staff       (20)    13277 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_cosmoBH_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)    23569 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_general_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)     7836 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_owls_header_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)    16188 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_owls_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)     8724 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_public_header_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)     4112 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_public_header_hdf5_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)    13904 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_public_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)    13217 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_public_input_hdf5.F90
--rw-r--r--   0 rieder     (501) staff       (20)     7917 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_sphray_header_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)    14316 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_vbromm_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)    13702 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/global.F90
--rw-r--r--   0 rieder     (501) staff       (20)     2692 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/glsphray.F90
--rw-r--r--   0 rieder     (501) staff       (20)     1563 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/hash.f90
--rw-r--r--   0 rieder     (501) staff       (20)     5118 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/hdf5_io.F90
--rw-r--r--   0 rieder     (501) staff       (20)     4987 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/healpix_types.F90
--rw-r--r--   0 rieder     (501) staff       (20)    11601 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/hui_gnedin_atomic_rates.F90
--rw-r--r--   0 rieder     (501) staff       (20)     7028 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/hummer_atomic_rates.F90
--rw-r--r--   0 rieder     (501) staff       (20)    10043 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/iliev_comparison_project.F90
--rw-r--r--   0 rieder     (501) staff       (20)    14251 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/initialize.F90
--rw-r--r--   0 rieder     (501) staff       (20)    24603 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/ion_table_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)    10089 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/ion_temperature_update.F90
--rw-r--r--   0 rieder     (501) staff       (20)    34740 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/ionpar.F90
--rw-r--r--   0 rieder     (501) staff       (20)    12266 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/kerneldensity.F90
--rw-r--r--   0 rieder     (501) staff       (20)    17376 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/m_mrgrnk.F90
--rw-r--r--   0 rieder     (501) staff       (20)    13147 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/main_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)     6644 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/mainloop.F90
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:36.047459 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/
--rw-r--r--   0 rieder     (501) staff       (20)      167 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.gfortran.debug
--rw-r--r--   0 rieder     (501) staff       (20)      137 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.gfortran.opt
--rw-r--r--   0 rieder     (501) staff       (20)      201 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.intel.debug
--rw-r--r--   0 rieder     (501) staff       (20)      435 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.intel.opt
--rw-r--r--   0 rieder     (501) staff       (20)      136 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      206 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.cosma.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      195 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.cosma.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      369 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.ferrari.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      102 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.icc-graphics.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      145 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.icc-graphics.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      176 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.santabuntu.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      372 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.santabuntu.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      128 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.titania.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      177 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.titania.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      175 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.warp.opt
--rw-r--r--   0 rieder     (501) staff       (20)      180 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.warp.opt.bck
--rw-r--r--   0 rieder     (501) staff       (20)      221 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.warp.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      194 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.xgpc.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      447 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/makes/make.xgpc.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)    11160 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/mt19937.F90
--rw-r--r--   0 rieder     (501) staff       (20)    16660 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/myf03.f90
--rw-r--r--   0 rieder     (501) staff       (20)     6520 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/nblist.F90
--rw-r--r--   0 rieder     (501) staff       (20)    18132 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/octtree3.F90
--rw-r--r--   0 rieder     (501) staff       (20)    17069 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/octtree3p.F90
--rw-r--r--   0 rieder     (501) staff       (20)    23138 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/output.F90
--rw-r--r--   0 rieder     (501) staff       (20)    25364 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/particle_system.F90
--rw-r--r--   0 rieder     (501) staff       (20)     5612 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/physical_constants.F90
--rw-r--r--   0 rieder     (501) staff       (20)     9944 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/pix_tools.F90
--rw-r--r--   0 rieder     (501) staff       (20)    15588 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/ray.F90
--rw-r--r--   0 rieder     (501) staff       (20)    12331 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/raylist.F90
--rw-r--r--   0 rieder     (501) staff       (20)    68389 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/sobol.F90
--rw-r--r--   0 rieder     (501) staff       (20)    11314 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/source_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)     3072 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/spectra.F90
--rw-r--r--   0 rieder     (501) staff       (20)     2903 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/sphpar.F90
--rw-r--r--   0 rieder     (501) staff       (20)     3125 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/sphray.F90
--rw-r--r--   0 rieder     (501) staff       (20)     5124 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/update_particles.F90
--rw-r--r--   0 rieder     (501) staff       (20)    27441 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/viewer.F90
--rw-r--r--   0 rieder     (501) staff       (20)    23330 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/src/voronov_atomic_rates.F90
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-04-04 14:22:33.000000 amuse-sphray-2023.4.0/src/amuse/community/sphray/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-04-04 14:22:36.049086 amuse-sphray-2023.4.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2021-07-05 11:19:28.000000 amuse-sphray-2023.4.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2022-11-30 13:58:15.000000 amuse-sphray-2023.4.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2020-03-24 14:36:26.000000 amuse-sphray-2023.4.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    50379 2023-04-04 13:47:06.000000 amuse-sphray-2023.4.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2021-04-14 10:14:49.000000 amuse-sphray-2023.4.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.837463 amuse-sphray-2023.5.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-sphray-2023.5.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-05-17 10:19:47.837281 amuse-sphray-2023.5.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       59 2022-11-22 11:55:14.000000 amuse-sphray-2023.5.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.803613 amuse-sphray-2023.5.0/amuse_sphray.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-05-17 10:19:45.000000 amuse-sphray-2023.5.0/amuse_sphray.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     6112 2023-05-17 10:19:47.000000 amuse-sphray-2023.5.0/amuse_sphray.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:45.000000 amuse-sphray-2023.5.0/amuse_sphray.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:19:45.000000 amuse-sphray-2023.5.0/amuse_sphray.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:19:45.000000 amuse-sphray-2023.5.0/amuse_sphray.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-sphray-2023.5.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:47.837504 amuse-sphray-2023.5.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1777 2022-11-22 11:55:14.000000 amuse-sphray-2023.5.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.801528 amuse-sphray-2023.5.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.801584 amuse-sphray-2023.5.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.801639 amuse-sphray-2023.5.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.805018 amuse-sphray-2023.5.0/src/amuse/community/sphray/
+-rw-r--r--   0 rieder     (501) staff       (20)     1393 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       30 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/__init__.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.801780 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.806650 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.813588 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/
+-rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates.txt
+-rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Cen.txt
+-rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hui.txt
+-rw-r--r--   0 rieder     (501) staff       (20)   785996 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hum.txt
+-rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Vor.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.815310 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/column_depth/
+-rw-r--r--   0 rieder     (501) staff       (20)     1288 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/column_depth/latmon_b2cd_table.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     1288 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/column_depth/tophat_b2cd_table.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.816807 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/
+-rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/power2.0.cdf
+-rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/power4.0.cdf
+-rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/thermal1e5.cdf
+-rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/thermal6e4.cdf
+-rw-r--r--   0 rieder     (501) staff       (20)   370256 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/sphray_4K
+-rw-r--r--   0 rieder     (501) staff       (20)       70 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/test1_sources_001.1
+-rw-r--r--   0 rieder     (501) staff       (20)       69 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/test2_sources_001.1
+-rw-r--r--   0 rieder     (501) staff       (20)     9907 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/interface.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    35232 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/interface.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.829368 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     9708 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     8945 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/MakefileTemplate
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.832409 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/
+-rw-r--r--   0 rieder     (501) staff       (20)    71467 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GL.h
+-rw-r--r--   0 rieder     (501) staff       (20)    16543 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLU.h
+-rw-r--r--   0 rieder     (501) staff       (20)    19786 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLUT.h
+-rw-r--r--   0 rieder     (501) staff       (20)      536 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLUT_fonts.c
+-rw-r--r--   0 rieder     (501) staff       (20)    68448 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_freeglut.F90
+-rw-r--r--   0 rieder     (501) staff       (20)   194062 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_gl.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    41410 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glu.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    56657 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glut.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    67729 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_openglut.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     1091 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/fthread.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6077 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/pt.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6831 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/pt.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1018 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/ptf77.c
+-rw-r--r--   0 rieder     (501) staff       (20)    33052 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/amuse_helpers.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     5354 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/amuse_mainloop.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    25577 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/atomic_rates.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     3995 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/b2cd.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     8804 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/bdf.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    14046 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/cen_atomic_rates.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    23703 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/config.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     2264 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/cosmology.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     7761 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/density_test.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    12191 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/euler.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    13277 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_cosmoBH_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    23569 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_general_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     7836 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_owls_header_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    16188 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_owls_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     8724 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_header_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     4112 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_header_hdf5_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    13904 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    13217 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_input_hdf5.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     7917 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_sphray_header_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    14316 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_vbromm_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    13702 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/global.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     2692 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/glsphray.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     1563 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hash.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     5118 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hdf5_io.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     4987 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/healpix_types.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    11601 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hui_gnedin_atomic_rates.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     7028 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hummer_atomic_rates.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    10043 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/iliev_comparison_project.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    14251 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/initialize.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    24603 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ion_table_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    10089 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ion_temperature_update.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    34740 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ionpar.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    12266 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/kerneldensity.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    17376 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/m_mrgrnk.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    13147 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/main_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     6644 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/mainloop.F90
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.835771 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/
+-rw-r--r--   0 rieder     (501) staff       (20)      167 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.gfortran.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      137 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.gfortran.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      201 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.intel.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      435 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.intel.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      136 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      206 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.cosma.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      195 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.cosma.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      369 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.ferrari.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      102 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.icc-graphics.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.icc-graphics.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      176 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.santabuntu.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      372 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.santabuntu.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      128 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.titania.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      177 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.titania.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      175 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.warp.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      180 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.warp.opt.bck
+-rw-r--r--   0 rieder     (501) staff       (20)      221 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.warp.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      194 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.xgpc.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      447 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.xgpc.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)    11160 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/mt19937.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    16660 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/myf03.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     6520 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/nblist.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    18132 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/octtree3.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    17069 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/octtree3p.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    23138 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/output.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    25364 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/particle_system.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     5612 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/physical_constants.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     9944 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/pix_tools.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    15588 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ray.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    12331 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/raylist.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    68389 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sobol.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    11314 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/source_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     3072 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/spectra.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     2903 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sphpar.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     3125 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sphray.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     5124 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/update_particles.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    27441 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/viewer.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    23330 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/voronov_atomic_rates.F90
+-rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:45.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.837057 amuse-sphray-2023.5.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-sphray-2023.5.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/version.py
```

### Comparing `amuse-sphray-2023.4.0/PKG-INFO` & `amuse-sphray-2023.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-sphray
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: The Astrophysical Multipurpose Software Environment - SPHRay
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `amuse-sphray-2023.4.0/amuse_sphray.egg-info/PKG-INFO` & `amuse-sphray-2023.5.0/amuse_sphray.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-sphray
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: The Astrophysical Multipurpose Software Environment - SPHRay
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `amuse-sphray-2023.4.0/amuse_sphray.egg-info/SOURCES.txt` & `amuse-sphray-2023.5.0/amuse_sphray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/setup.py` & `amuse-sphray-2023.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/Makefile` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates.txt` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Cen.txt` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Cen.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hui.txt` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hui.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hum.txt` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hum.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Vor.txt` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Vor.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/column_depth/latmon_b2cd_table.txt` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/column_depth/latmon_b2cd_table.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/column_depth/tophat_b2cd_table.txt` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/column_depth/tophat_b2cd_table.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/spectra/power2.0.cdf` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/power2.0.cdf`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/spectra/power4.0.cdf` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/power4.0.cdf`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/spectra/thermal1e5.cdf` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/thermal1e5.cdf`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/spectra/thermal6e4.cdf` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/thermal6e4.cdf`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/data/input/sphray_4K` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/sphray_4K`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/interface.f90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/interface.f90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/interface.py` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/Makefile` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/MakefileTemplate` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/MakefileTemplate`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/GL.h` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GL.h`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/GLU.h` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLU.h`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/GLUT.h` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLUT.h`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/GLUT_fonts.c` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLUT_fonts.c`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_freeglut.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_freeglut.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_gl.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_gl.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glu.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glu.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glut.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glut.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_openglut.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_openglut.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/fthread.f` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/fthread.f`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/pt.c` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/pt.c`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/pt.h` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/pt.h`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/OpenGL/ptf77.c` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/ptf77.c`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/amuse_helpers.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/amuse_helpers.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/amuse_mainloop.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/amuse_mainloop.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/atomic_rates.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/atomic_rates.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/b2cd.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/b2cd.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/bdf.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/bdf.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/cen_atomic_rates.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/cen_atomic_rates.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/config.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/config.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/cosmology.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/cosmology.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/density_test.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/density_test.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/euler.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/euler.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_cosmoBH_input.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_cosmoBH_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_general_class.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_general_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_owls_header_class.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_owls_header_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_owls_input.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_owls_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_public_header_class.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_header_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_public_header_hdf5_class.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_header_hdf5_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_public_input.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_public_input_hdf5.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_input_hdf5.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_sphray_header_class.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_sphray_header_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/gadget_vbromm_input.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_vbromm_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/global.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/global.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/glsphray.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/glsphray.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/hash.f90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hash.f90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/hdf5_io.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hdf5_io.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/healpix_types.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/healpix_types.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/hui_gnedin_atomic_rates.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hui_gnedin_atomic_rates.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/hummer_atomic_rates.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hummer_atomic_rates.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/iliev_comparison_project.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/iliev_comparison_project.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/initialize.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/initialize.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/ion_table_class.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ion_table_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/ion_temperature_update.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ion_temperature_update.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/ionpar.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ionpar.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/kerneldensity.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/kerneldensity.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/m_mrgrnk.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/m_mrgrnk.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/main_input.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/main_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/mainloop.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/mainloop.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/mt19937.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/mt19937.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/myf03.f90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/myf03.f90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/nblist.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/nblist.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/octtree3.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/octtree3.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/octtree3p.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/octtree3p.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/output.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/output.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/particle_system.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/particle_system.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/physical_constants.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/physical_constants.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/pix_tools.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/pix_tools.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/ray.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ray.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/raylist.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/raylist.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/sobol.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sobol.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/source_input.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/source_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/spectra.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/spectra.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/sphpar.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sphpar.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/sphray.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sphray.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/update_particles.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/update_particles.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/viewer.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/viewer.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/src/amuse/community/sphray/src/voronov_atomic_rates.F90` & `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/voronov_atomic_rates.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/support/__init__.py` & `amuse-sphray-2023.5.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/support/classifiers.py` & `amuse-sphray-2023.5.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/support/config.py` & `amuse-sphray-2023.5.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/support/generate_main.py` & `amuse-sphray-2023.5.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/support/getsp.class` & `amuse-sphray-2023.5.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/support/getsp.java` & `amuse-sphray-2023.5.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/support/misc.py` & `amuse-sphray-2023.5.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.4.0/support/setup_codes.py` & `amuse-sphray-2023.5.0/support/setup_codes.py`

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

