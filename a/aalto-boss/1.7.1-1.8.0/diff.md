# Comparing `tmp/aalto-boss-1.7.1.tar.gz` & `tmp/aalto-boss-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aalto-boss-1.7.1.tar", last modified: Mon Feb 27 02:10:25 2023, max compression
+gzip compressed data, was "aalto-boss-1.8.0.tar", last modified: Wed May 17 11:36:34 2023, max compression
```

## Comparing `aalto-boss-1.7.1.tar` & `aalto-boss-1.8.0.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 02:10:25.383688 aalto-boss-1.7.1/
--rw-rw-rw-   0 root         (0) root         (0)    11334 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6039 2023-02-27 02:10:25.383688 aalto-boss-1.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4836 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 02:10:25.367686 aalto-boss-1.7.1/aalto_boss.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6039 2023-02-27 02:10:25.000000 aalto-boss-1.7.1/aalto_boss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1145 2023-02-27 02:10:25.000000 aalto-boss-1.7.1/aalto_boss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 02:10:25.000000 aalto-boss-1.7.1/aalto_boss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-02-27 02:10:25.000000 aalto-boss-1.7.1/aalto_boss.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-02-27 02:10:25.000000 aalto-boss-1.7.1/aalto_boss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-02-27 02:10:25.000000 aalto-boss-1.7.1/aalto_boss.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 02:10:25.368686 aalto-boss-1.7.1/boss/
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4799 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 02:10:25.371686 aalto-boss-1.7.1/boss/bo/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 02:10:25.374687 aalto-boss-1.7.1/boss/bo/acq/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/acq/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3825 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/acq/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4984 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/acq/cost.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/acq/ei.py
--rw-rw-rw-   0 root         (0) root         (0)     3005 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/acq/elcb.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/acq/exploit.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/acq/explore.py
--rw-rw-rw-   0 root         (0) root         (0)     2063 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/acq/lcb.py
--rw-rw-rw-   0 root         (0) root         (0)    13618 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/bo_main.py
--rw-rw-rw-   0 root         (0) root         (0)     1624 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/hmc.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/initmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     4685 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/kernel_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    16513 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/model.py
--rw-rw-rw-   0 root         (0) root         (0)    18742 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/results.py
--rw-rw-rw-   0 root         (0) root         (0)     5077 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/rstmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     1048 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/bo/userfunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 02:10:25.376687 aalto-boss-1.7.1/boss/io/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5953 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/io/dump.py
--rw-rw-rw-   0 root         (0) root         (0)     2971 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/io/ioutils.py
--rw-rw-rw-   0 root         (0) root         (0)    13932 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/io/main_output.py
--rw-rw-rw-   0 root         (0) root         (0)     9058 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/io/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     6543 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/keywords.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 02:10:25.379687 aalto-boss-1.7.1/boss/mep/
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/mep/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/mep/forest.py
--rw-rw-rw-   0 root         (0) root         (0)     5746 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/mep/mep.py
--rw-rw-rw-   0 root         (0) root         (0)     3721 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/mep/mepmain.py
--rw-rw-rw-   0 root         (0) root         (0)     2724 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/mep/neb.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/mep/node.py
--rw-rw-rw-   0 root         (0) root         (0)     3311 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/mep/path.py
--rw-rw-rw-   0 root         (0) root         (0)     2057 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/mep/space.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 02:10:25.380687 aalto-boss-1.7.1/boss/pp/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/pp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21153 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/pp/plot.py
--rw-rw-rw-   0 root         (0) root         (0)    19460 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/pp/pp_main.py
--rw-rw-rw-   0 root         (0) root         (0)    11442 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 02:10:25.383688 aalto-boss-1.7.1/boss/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/utils/arrays.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/utils/distributions.py
--rw-rw-rw-   0 root         (0) root         (0)    10560 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/utils/minimization.py
--rw-rw-rw-   0 root         (0) root         (0)    20566 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/utils/sobol_seq.py
--rw-rw-rw-   0 root         (0) root         (0)     6812 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/utils/sparselist.py
--rw-rw-rw-   0 root         (0) root         (0)    17913 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/utils/testing.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-02-27 02:10:23.000000 aalto-boss-1.7.1/boss/utils/timer.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-27 02:10:25.383688 aalto-boss-1.7.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3162 2023-02-27 02:10:24.000000 aalto-boss-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:36:34.135944 aalto-boss-1.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11334 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6039 2023-05-17 11:36:34.134944 aalto-boss-1.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4836 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:36:34.117943 aalto-boss-1.8.0/aalto_boss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6039 2023-05-17 11:36:34.000000 aalto-boss-1.8.0/aalto_boss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-17 11:36:34.000000 aalto-boss-1.8.0/aalto_boss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 11:36:34.000000 aalto-boss-1.8.0/aalto_boss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-17 11:36:34.000000 aalto-boss-1.8.0/aalto_boss.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 11:36:34.000000 aalto-boss-1.8.0/aalto_boss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-17 11:36:34.000000 aalto-boss-1.8.0/aalto_boss.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:36:34.119943 aalto-boss-1.8.0/boss/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4799 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:36:34.122943 aalto-boss-1.8.0/boss/bo/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:36:34.125943 aalto-boss-1.8.0/boss/bo/acq/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/acq/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4521 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/acq/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5647 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/acq/cost.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/acq/ei.py
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/acq/elcb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/acq/exploit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/acq/explore.py
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/acq/lcb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3831 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/acq/mes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/acq/multi.py
+-rw-rw-rw-   0 root         (0) root         (0)    14638 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/bo_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/hmc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4004 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/initmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6871 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/kernel_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    26921 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/model.py
+-rw-rw-rw-   0 root         (0) root         (0)    19805 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/results.py
+-rw-rw-rw-   0 root         (0) root         (0)     5064 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/rstmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/bo/userfunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:36:34.127943 aalto-boss-1.8.0/boss/io/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5973 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/io/dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     2971 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/io/ioutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14130 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/io/main_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     9058 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/io/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7026 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/keywords.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:36:34.130943 aalto-boss-1.8.0/boss/mep/
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/mep/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2047 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/mep/forest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5746 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/mep/mep.py
+-rw-rw-rw-   0 root         (0) root         (0)     3764 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/mep/mepmain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2724 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/mep/neb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/mep/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/mep/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/mep/space.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:36:34.131944 aalto-boss-1.8.0/boss/pp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/pp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21357 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/pp/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19502 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/pp/pp_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    17811 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:36:34.134944 aalto-boss-1.8.0/boss/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/utils/arrays.py
+-rw-rw-rw-   0 root         (0) root         (0)     3815 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/utils/distributions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11223 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/utils/minimization.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/utils/os.py
+-rw-rw-rw-   0 root         (0) root         (0)    20566 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/utils/sobol_seq.py
+-rw-rw-rw-   0 root         (0) root         (0)     6812 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/utils/sparselist.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/boss/utils/timer.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 11:36:34.135944 aalto-boss-1.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3162 2023-05-17 11:36:32.000000 aalto-boss-1.8.0/setup.py
```

### Comparing `aalto-boss-1.7.1/LICENSE` & `aalto-boss-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/PKG-INFO` & `aalto-boss-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aalto-boss
-Version: 1.7.1
+Version: 1.8.0
 Summary: Bayesian optimization structure search
 Home-page: https://gitlab.com/cest-group/boss
 Author: Ville Parkkinen, Henri Paulamaki, Arttu Tolvanen, Ulpu Remes, Nuutti Sten, Emma Lehto, Manuel Kuchelmeister, Tuomas Rossi, Mikael Granit"
     "Joakim Loefgren, Milica Todorovic, 
 Maintainer: The BOSS developers team
 Maintainer-email: milica.todorovic@utu.fi
 License: Apache License 2.0
```

### Comparing `aalto-boss-1.7.1/README.rst` & `aalto-boss-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/aalto_boss.egg-info/PKG-INFO` & `aalto-boss-1.8.0/aalto_boss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aalto-boss
-Version: 1.7.1
+Version: 1.8.0
 Summary: Bayesian optimization structure search
 Home-page: https://gitlab.com/cest-group/boss
 Author: Ville Parkkinen, Henri Paulamaki, Arttu Tolvanen, Ulpu Remes, Nuutti Sten, Emma Lehto, Manuel Kuchelmeister, Tuomas Rossi, Mikael Granit"
     "Joakim Loefgren, Milica Todorovic, 
 Maintainer: The BOSS developers team
 Maintainer-email: milica.todorovic@utu.fi
 License: Apache License 2.0
```

### Comparing `aalto-boss-1.7.1/aalto_boss.egg-info/SOURCES.txt` & `aalto-boss-1.8.0/aalto_boss.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 boss/bo/acq/base.py
 boss/bo/acq/cost.py
 boss/bo/acq/ei.py
 boss/bo/acq/elcb.py
 boss/bo/acq/exploit.py
 boss/bo/acq/explore.py
 boss/bo/acq/lcb.py
+boss/bo/acq/mes.py
+boss/bo/acq/multi.py
 boss/io/__init__.py
 boss/io/dump.py
 boss/io/ioutils.py
 boss/io/main_output.py
 boss/io/parse.py
 boss/mep/__init__.py
 boss/mep/forest.py
@@ -45,11 +47,11 @@
 boss/pp/__init__.py
 boss/pp/plot.py
 boss/pp/pp_main.py
 boss/utils/__init__.py
 boss/utils/arrays.py
 boss/utils/distributions.py
 boss/utils/minimization.py
+boss/utils/os.py
 boss/utils/sobol_seq.py
 boss/utils/sparselist.py
-boss/utils/testing.py
 boss/utils/timer.py
```

### Comparing `aalto-boss-1.7.1/boss/__init__.py` & `aalto-boss-1.8.0/boss/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.7.1"
+__version__ = "1.8.0"
 __url__ = "https://gitlab.com/cest-group/boss"
 __description__ = "Bayesian optimization structure search"
 __authors__ = [
     "Ville Parkkinen",
     "Henri Paulamaki",
     "Arttu Tolvanen",
     "Ulpu Remes",
```

### Comparing `aalto-boss-1.7.1/boss/__main__.py` & `aalto-boss-1.8.0/boss/__main__.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/bo/acq/base.py` & `aalto-boss-1.8.0/boss/bo/acq/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -96,29 +96,61 @@
           2D array containing data with 'float' type.
 
         Returns
         -------
         ndarray
           Array containing found minimum with 'float' type.
         """
+        if not self.has_gradient:
+            optimfunc = self.evaluate
+            self.get_minima_samples()
+        else:
+            optimfunc = self.evaluate_with_gradient
+
         if optimtype == 'score':
             gmin = Minimization.minimize_using_score(
-                self.evaluate_with_gradient, bounds)
+                optimfunc,
+                bounds,
+                has_gradient=self.has_gradient
+                )
         else:
             # Calculate number of local minimizers to start.
             # 1. Estimate number of local minima in the surrogate model.
             estimated_numpts = self.model.estimate_num_local_minima(bounds)
             # 2. Increase estimate to approximate number of local minima in
             # acquisition function. Here we assume that increase is
             # proportional to estimated number of local minima per dimension.
             dim = len(bounds)
             minima_multiplier = 1.7
             estimated_numpts = (minima_multiplier ** dim) * \
                 estimated_numpts
             num_pts = min(len(self.model.X), int(estimated_numpts))
             # Minimize acqfn to obtain sampling location
             gmin = Minimization.minimize_from_random(
-                self.evaluate_with_gradient,
+                optimfunc,
                 bounds,
                 num_pts=num_pts,
+                has_gradient=self.has_gradient
                 )
         return np.atleast_1d(np.array(gmin[0]))
+
+
+class CostAwareAcquisition(BaseAcquisition):
+    """
+    Base class for cost-aware acquisition functions.
+
+    """
+    @abstractmethod
+    def evaluate_cost(self, x):
+        """
+        Evaluates the acquisition cost at x and returns its value.
+
+        Parameters
+        ----------
+        x : ndarray
+            Location to evaluate acquisition cost at
+
+        Returns
+        -------
+        cost : float
+
+        """
```

### Comparing `aalto-boss-1.7.1/boss/bo/acq/cost.py` & `aalto-boss-1.8.0/boss/bo/acq/cost.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from boss.bo.acq.base import BaseAcquisition
+from boss.bo.acq.base import CostAwareAcquisition
 import numpy as np
 from boss.utils.arrays import shape_consistent_XY
 
 
 class CostFunc:
     """Wrapper class for the user-supplied cost.
 
@@ -18,26 +18,42 @@
         dY, Y = shape_consistent_XY(dY, Y, self.dim)
         return Y, dY
 
     def __call__(self, X):
         return self.eval(X)
 
 
-class DivisiveCost(BaseAcquisition):
+class DivisiveCost(CostAwareAcquisition):
     """
     Wraps the acquisition function with a user-defined cost function.
 
     DivisiveCost considers the cost by dividing the evaluations by a
     cost factor.
     """
     def __init__(self, acqfn, costfn):
         super().__init__()
         self.acqfn = acqfn
         self.costfn = costfn
 
+    def evaluate_cost(self, x):
+        """
+        Evaluates the acquisition cost at x and returns its value.
+
+        Parameters
+        ----------
+        x : ndarray
+            Location to evaluate acquisition cost at
+
+        Returns
+        -------
+        cost : float
+
+        """
+        return self.costfn(x)[0]
+
     def evaluate(self, x):
         """Compute the acquisition function divided by cost at location x.
 
         Parameters
         ----------
         x : ndarray
             Input to the acquisition function. 2D array containing data with
@@ -94,26 +110,42 @@
         ----------
         new_model : Model
             BaseModel used for the optimization.
         """
         self.acqfn.model = new_model
 
 
-class AdditiveCost(BaseAcquisition):
+class AdditiveCost(CostAwareAcquisition):
     """
     Wraps the acquisition function with a user-defined cost function.
     With that, the user can add 'weak' constrains on the search space.
 
     AdditiveCost considers the cost by adding a cost factor to the evaluations.
     """
     def __init__(self, acqfn, costfn):
         super().__init__()
         self.acqfn = acqfn
         self.costfn = costfn
 
+    def evaluate_cost(self, x):
+        """
+        Evaluates the acquisition cost at x and returns its value.
+
+        Parameters
+        ----------
+        x : ndarray
+            Location to evaluate acquisition cost at
+
+        Returns
+        -------
+        cost : float
+
+        """
+        return self.costfn(x)[0]
+
     def evaluate(self, x):
         """Compute the acquisition function with added cost at location x.
 
         Parameters
         ----------
         x : ndarray
             Input to the acquisition function. 2D array containing data with
```

### Comparing `aalto-boss-1.7.1/boss/bo/acq/ei.py` & `aalto-boss-1.8.0/boss/bo/acq/ei.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/bo/acq/elcb.py` & `aalto-boss-1.8.0/boss/bo/acq/elcb.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/bo/acq/exploit.py` & `aalto-boss-1.8.0/boss/bo/acq/exploit.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/bo/acq/explore.py` & `aalto-boss-1.8.0/boss/bo/acq/explore.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/bo/acq/lcb.py` & `aalto-boss-1.8.0/boss/bo/acq/lcb.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/bo/bo_main.py` & `aalto-boss-1.8.0/boss/bo/bo_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 from scipy.spatial.distance import euclidean
 
 import boss.io.ioutils as ioutils
 import boss.io.parse as parse
 from boss.bo.initmanager import InitManager
 from boss.bo.kernel_factory import KernelFactory
-from boss.bo.model import Model, GradientModel
 from boss.bo.results import BOResults, minimize_model
 from boss.bo.rstmanager import RstManager
 from boss.io.main_output import MainOutput
 from boss.settings import Settings
 from boss.utils.arrays import shape_consistent_XY
 from boss.utils.minimization import Minimization
 from boss.utils.timer import Timer
@@ -62,37 +61,48 @@
     def _setup(self):
         """Common setup for all factory methods."""
         settings = self.settings
         self.main_output = MainOutput(settings)
         if not self.rst_manager:
             self.rst_manager = RstManager(settings)
 
-        self.init_manager = InitManager(
-            settings["inittype"], settings["bounds"], settings["initpts"]
-        )
+        # Resolve optimisation domain
+        if settings.is_multi:
+            self.dim = settings.dim + 1
+            self.bounds = np.vstack((settings["bounds"], [[0, 0]]))
+        else:
+            self.dim = settings.dim
+            self.bounds = settings["bounds"]
+
+        if settings.is_multi:
+            self.init_manager = InitManager(
+                settings["inittype"], settings["bounds"], settings["task_initpts"]
+            )
+        else:
+            self.init_manager = InitManager(
+                settings["inittype"], settings["bounds"], settings["initpts"]
+            )
         self.acqfn = settings.acqfn
         self.expfn = settings.expfn
         self.user_func = settings.f
         self.ygrad = settings['ygrad']
 
         self.kernel = KernelFactory.construct_kernel(settings)
         self.model = None
         Minimization.set_parallel(self.settings["parallel_optims"])
 
         self.results = BOResults(settings=settings)
         self.results.add_defaults()
         self.itr_curr = 0
+        self.cum_cost = 0
 
     def init_model(self, X, Y, params=None):
         """Initializes the GP model."""
-        X, Y = shape_consistent_XY(
-            X, Y, self.settings.dim, nan_pad=False, ygrad=self.ygrad
-        )
-        model = Model if not self.ygrad else GradientModel
-        self.model = model(
+        X, Y = shape_consistent_XY(X, Y, self.dim, nan_pad=False, ygrad=self.ygrad)
+        self.model = self.settings.model_class(
             X,
             Y,
             self.kernel,
             self.settings["noise"],
             self.settings["ynorm"],
         )
         # Look for optimized model params from:
@@ -131,22 +141,22 @@
             The very first acquisition that will be used in the BO-run.
         """
         self.main_output.new_file()
         self.rst_manager.new_file()
         self.results.clear()
 
         # Ensure X,Y initial values are 2D arrays of the same size.
-        dim = self.settings.dim
+        dim = self.dim
         X_init, Y_init = shape_consistent_XY(
             X_init, Y_init, dim, nan_pad=True, ygrad=self.ygrad
         )
         self.settings["initpts"] = X_init.shape[0]
 
         X = np.empty((0, dim), float)
-        Y = np.empty((0, 1 + self.ygrad * self.settings.dim), float)
+        Y = np.empty((0, 1 + self.ygrad * dim), float)
         for i in range(self.settings["initpts"]):
             with self.main_output.summarize_results(self.results):
 
                 # Evaluate the userfn if initial y-data is not available
                 if np.isnan(Y_init[i]).all():
                     XY_out = self._eval_user_func(X_init[i, :])
                     X = np.vstack((X, XY_out[0]))
@@ -177,54 +187,61 @@
         """If initial data is not provided, get it from the rst/init manager."""
         if self.rst_manager.data.shape[0] > 0:
             X_init = self.rst_manager.X
             Y_init = self.rst_manager.Y
         else:
             X_init = self.init_manager.get_all()
             Y_init = np.empty(
-                (len(X_init), 1 + self.ygrad * self.settings.dim)) * np.nan
+                (len(X_init), 1 + self.ygrad * self.dim)) * np.nan
         return X_init, Y_init
 
-    def run(self, X_init=None, Y_init=None, iterpts=None):
+    def run(self, X_init=None, Y_init=None, iterpts=None, maxcost=None):
         """
         The Bayesian optimization main loop. Evaluates first the initialization
         points, then creates a GP model and uses it and an acquisition function
         to locate the next points where to evaluate. Stops when a pre-specified
         number of initialization points and BO points have been acquired or a
-        convergence criterion is met.
+        convergence criterion or cost limit is met.
 
         Returns
         -------
         BOResults
             An object that provides convenient access to the most
             important results from the optimization.
         """
         if iterpts:
             self.settings["iterpts"] = iterpts
+        if maxcost:
+            self.settings["maxcost"] = maxcost
         # Initialize model & files if we're starting fresh or restarting from file.
         if self.model is None:
             # Handle initial points
             if X_init is not None:
                 X_init, Y_init = shape_consistent_XY(
                     X_init,
                     Y_init,
-                    self.settings.dim,
+                    self.dim,
                     nan_pad=True,
                     ygrad=self.ygrad,
                 )
             else:
                 X_init, Y_init = self.get_initpts()
 
             X_next = self.init_run(X_init, Y_init)
         # The model already exists and we just need the next acquisition.
         else:
             X_next = self.acquire()
 
         # BO main loop
         for _ in range(self.itr_curr, self.settings["iterpts"] + 1):
+
+            if self.exceeds_cost_limit(X_next):
+                self.main_output.maxcost_stop()
+                break
+
             with self.main_output.summarize_results(self.results):
 
                 # 1. User func evaluation
                 X_new, Y_new = self._eval_user_func(X_next)
 
                 # 2. Model update: refit model to new data & optimize params.
                 self._update_model(X_new, Y_new)
@@ -256,14 +273,19 @@
             self.main_output.progress_msg(
                 "Evaluating objective function at x ="
                 + ioutils.oneDarray_line(x, len(x), float),
             )
         self.main_output.progress_msg(
             "Objective function evaluated," + f" time [s] {local_timer.lap_time}",
         )
+
+        # Update accumulated cost if needed
+        if self.settings["maxcost"] is not None:
+            self.cum_cost += self.acqfn.evaluate_cost(X_out)
+
         return X_out, Y
 
     def _update_model(self, X_next, Y_next):
         """Optimizes and refits model with new data."""
 
         # Store new data
         self.model.add_data(X_next, Y_next)
@@ -298,29 +320,39 @@
         should_optimize = self.itr_curr == self.settings["iterpts"] or (
             minfreq > 0 and (self.itr_curr % minfreq == 0)
         )
 
         if should_optimize:
             x_glmin, mu_glmin, nu_glmin = minimize_model(
                 self.model,
-                self.settings["bounds"],
+                self.bounds,
                 self.settings["optimtype"],
                 self.settings["kernel"],
                 self.settings["min_dist_acqs"],
                 accuracy=self.settings["minzacc"],
             )
             self.results.update(
                 {
                     "x_glmin": x_glmin,
                     "mu_glmin": mu_glmin,
                     "nu_glmin": nu_glmin,
                 }
             )
         self.itr_curr += 1
 
+    def exceeds_cost_limit(self, X_next):
+        """
+        Checks whether the next acquisition would exceed cost limit.
+        """
+        if self.settings["maxcost"] is None:
+            return False
+        else:
+            cost_next = self.acqfn.evaluate_cost(X_next)
+            return self.cum_cost + cost_next > self.settings["maxcost"]
+
     def has_converged(self):
         """
         Checks whether dxhat has been within tolerance for long enough
         TODO: should use dxmuhat instead?
         """
         glmin_tol = self.settings["glmin_tol"]
         if glmin_tol is None:
@@ -344,22 +376,21 @@
         """
         Get a new point to evaluate by either reading it from the rst-file or,
         in case it doesn't contain the next point to evaluate, by obtaining
         a new initial point (when run is in initialization stage) or
         minimizing the acquisition function (when the run is in BO stage).
         """
         minimizer_params = {
-            "bounds": self.settings["bounds"],
+            "bounds": self.bounds,
             "optimtype": self.settings["optimtype"],
         }
         x_next = self.acqfn.minimize(**minimizer_params)
         if self._loc_overconfident(x_next):
             x_next = self.expfn.minimize(**minimizer_params)
-            return x_next
-        return x_next
+        return x_next  # 1d array
 
     def _loc_overconfident(self, x_next):
         """
         Checks is model variance is lower than tolerance at suggested X_next.
         """
         acqtol = self.settings["acqtol"] if self.acqfn is not self.expfn else None
         if acqtol is None:
```

### Comparing `aalto-boss-1.7.1/boss/bo/hmc.py` & `aalto-boss-1.8.0/boss/bo/hmc.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/bo/model.py` & `aalto-boss-1.8.0/boss/bo/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             numpts *= max(1, bound_distance/float(kern.lengthscale))
         return int(numpts)
 
     # model parameters:
 
     def get_all_params(self):
         """
-        Returns model parameters as a dictionary with entries::
+        Returns model parameters as a dictionary with entries:
         noise, variance, lengthscales, periods
         where the last two are 1D lists. There exists a period only for those
         dimensions which are using a periodic kernel.
         """
         noise = float(self.model.likelihood.variance)
         sigma = float(self.model.kern.param_array[0])
         lss = []
@@ -306,29 +306,29 @@
         Y_norm = (Y - self.normmean) / self.normsd
         self.model.set_XY(np.atleast_2d(X), np.atleast_2d(Y_norm))
 
     def get_best_xy(self):
         """
         Returns the lowest energy acquisition (x, y).
         """
-        xbest = np.array(self.X[np.argmin(self.Y)])
-        ybest = np.min(self.Y)
-        return xbest, ybest
+        x_best = np.array(self.X[np.argmin(self.Y)])
+        y_best = np.min(self.Y)
+        return x_best, y_best
 
     @property
     def kernel(self):
         return self.model.kern
 
     @property
     def X(self):
         return self.model.X
 
     @property
     def Y(self):
-        return self.model.Y*self.normsd+self.normmean
+        return self.model.Y * self.normsd + self.normmean
 
 
 class GradientModel(Model):
     """
     Functionality for creating, refitting and optimizing a GP model with
     gradient observations.
 
@@ -514,7 +514,305 @@
         Y = Y_norm * self.normsd + self.normmean
 
         dY = np.empty((len(Y), self.dim), dtype=float)
         for d in range(self.dim):
             dY[:, d, None] = Y_multioutput[np.where(output_index == d + 1)[0]]
 
         return np.concatenate((Y, dY), axis=1)
+
+
+class MTModel(Model):
+    """
+    Functionality for creating, refitting and optimizing a MTGP model
+    """
+
+    def __init__(self, X, Y, kernel, noise, ynorm):
+        """
+        Initializes the multi-task model class.
+        """
+        # input properties
+        self.dim = kernel.input_dim
+        # output properties
+        self.num_tasks = kernel.parameters[-1].output_dim
+        # task indices
+        inds = np.squeeze(X[:, -1]).astype(int)
+        self.check_task_indices(inds)
+        # observations list
+        XX = [X[inds == index, :-1] for index in range(self.num_tasks)]
+        YY = [Y[inds == index] for index in range(self.num_tasks)]
+        # normalise observation mean and scale:
+        self.normmean = [np.mean(Y) for Y in YY]
+        self.normsd = [1] * self.num_tasks
+        # scale normalisation is not used unless ynorm is true:
+        self.use_norm = ynorm
+        self.normsd = [np.ptp(Y) for Y in YY] if self.use_norm else 1
+        # normalised observation list:
+        YY_norm = [(Y-m)/s for Y, m, s in zip(YY, self.normmean, self.normsd)]
+        # initialise model
+        self.model = GPy.models.GPCoregionalizedRegression(
+            XX,
+            YY_norm,
+            kernel=kernel
+        )
+        self.model.mixed_noise.constrain_fixed(noise)
+
+    # utils:
+
+    def check_task_indices(self, inds):
+        """
+        Raises an error if all tasks are not included in the index list or if
+        the list includes more tasks than expected.
+        """
+        counts = np.bincount(inds, minlength=self.num_tasks)
+        if not np.all(counts > 0):
+            raise ValueError("All tasks must be represented in the dataset.")
+
+        num_tasks = max(inds) + 1
+        if num_tasks > self.num_tasks:
+            raise ValueError(f"Received a dataset with {num_tasks} tasks. "\
+                             f"Expected {self.num_tasks} tasks.")
+
+    def extend_input(self, x, index):
+        """
+        Returns x extended with task index.
+        """
+        x = np.atleast_2d(x)
+        inds = np.full((len(x), 1), index)
+        x = np.hstack((x, inds))
+        return x
+
+    # predictions:
+
+    def predict(self, x, index=None, noise=True):
+        """
+        Returns model prediction mean and variance at point x with or without
+        model variance (noise).
+        """
+        # extend x with task index if needed
+        x = np.atleast_2d(x)
+        if index is not None:
+            x = self.extend_input(x, index)
+        # build metadata
+        inds = x[:, -1].astype(int)
+        meta = {'output_index': inds}
+        # predict output
+        m, v = self.model.predict(x, Y_metadata=meta, include_likelihood=noise)
+        v = np.clip(v, 1e-12, np.inf)
+        # remove normalisation
+        for i in np.unique(inds):
+            m[inds == i] = m[inds == i] * self.normsd[i] + self.normmean[i]
+            v[inds == i] = v[inds == i] * self.normsd[i] ** 2
+        return m, v
+
+    def predict_grads(self, x, index=None):
+        """
+        Returns model prediction mean and variance gradients with respect to
+        input at point x.
+        """
+        # extend x with task index if needed
+        x = np.atleast_2d(x)
+        if index is not None:
+            x = self.extend_input(x, index)
+        # predictive gradients
+        dmdx, dvdx = self.model.predictive_gradients(np.atleast_2d(x))
+        # remove normalisation
+        inds = x[:, -1].astype(int)
+        for i in np.unique(inds):
+            dmdx[inds == i] *= self.normsd[i]
+            dvdx[inds == i] *= self.normsd[i] ** 2
+        return dmdx, dvdx
+
+    def predict_mean_sd_grads(self, x, index=None, noise=True):
+        """
+        Returns the model prediction mean, standard deviation and their
+        gradients at point x and task index, with or without model variance
+        (noise).
+        """
+        m, v = self.predict(x, index=index, noise=noise)
+        dmdx, dvdx = self.predict_grads(np.atleast_2d(x), index=index)
+        dmdx = dmdx[:, :, 0]
+        dsdx = dvdx / (2 * np.sqrt(v))
+        return m, np.sqrt(v), dmdx, dsdx
+
+    def predict_mean_grad(self, x, index=None):
+        """
+        Returns model mean and its gradient at point x and task index.
+        """
+        m, _ = self.predict(x, index=index)
+        dmdx, _ = self.predict_grads(x, index=index)
+        return m, dmdx
+
+    def estimate_num_local_minima(self, search_bounds):
+        """
+        Returns estimated number of local minima calculated based on model
+        properties.
+        """
+        # For the ith dimension, the number of local minima along a slice
+        # is approximately n(i) = boundlength(i)/(2*lengthscale(i)). Note
+        # that periodic kernels operate on normalised distances: distance
+        # between inputs that are period(i)/2 apart is 1. To get the total
+        # number of minima for all of the search space, multiply together
+        # n(i) over all i.
+        numpts = 1
+
+        # get baseline kernel parameters (exclude coregionalisation kernel)
+        ks = self.model.kern.parameters[:-1]
+        for bounds, kern in zip(search_bounds, ks):
+            if hasattr(kern, 'period'):
+                bound_distance = (bounds[1]-bounds[0])/float(kern.period)
+            else:
+                bound_distance = (bounds[1]-bounds[0])/2
+            numpts *= max(1, bound_distance/float(kern.lengthscale))
+        return int(numpts)
+
+    def predict_task_covariance(self, x):
+        """
+        Return predictive covariance between tasks at point x.
+        """
+        inds = np.arange(self.num_tasks)
+        x = np.squeeze(x)[:-1]
+        x_list = np.vstack([self.extend_input(x, i) for i in inds])
+        meta = {'output_index': inds.astype(int)}
+        m, cov = self.model.predict(x_list, Y_metadata=meta, full_cov=True)
+        return np.outer(self.normsd, self.normsd) * cov
+
+    # model parameters:
+
+    def get_all_params(self):
+        """
+        Returns model parameters as a dictionary with entries:
+        noise, lengthscales, periods, kappa, W
+        There exists a period only for those dimensions which are using a
+        periodic kernel.
+        """
+        # likelihood params
+        ll = self.model.likelihood.likelihoods_list
+        noise = [float(likelihood.variance) for likelihood in ll]
+        # kernel params
+        lss = []
+        pers = []
+        # get baseline kernel parameters (exclude coregionalisation kernel)
+        ks = self.model.kern.parameters[:-1]
+        for kern in ks:
+            lss.append(float(kern.lengthscale))
+            if hasattr(kern, 'period'):
+                pers.append(float(kern.period))
+        # coregionalisation params
+        kappa = np.array(self.model.kern.parameters[-1].kappa).reshape(1, -1)
+        W = np.array(self.model.kern.parameters[-1].W).reshape(1, -1)
+
+        # the variables are returned in a dict:
+        params = {}
+        params['noise'] = noise
+        params['lengthscales'] = lss
+        params['periods'] = pers
+        params['kappa'] = kappa
+        params['W'] = W
+
+        return params
+
+    def get_task_covariance(self):
+        """
+        Returns estimated task covariance matrix.
+        """
+        kappa = np.array(self.model.kern.parameters[-1].kappa)
+        W = np.array(self.model.kern.parameters[-1].W)
+        cov = np.outer(W, W) + np.diag(kappa)
+        return np.outer(self.normsd, self.normsd) * cov
+
+    # observations:
+
+    def add_data(self, X_new, Y_new):
+        """
+        Updates the model evidence (observations) dataset appending.
+        """
+        X_new = X_new.reshape(-1, self.dim)
+        Y_new = Y_new.reshape(-1, 1)
+        inds_new = X_new[:, -1].astype(int)
+
+        # construct new datasets
+        X = np.vstack([self.X, X_new])
+        Y = np.vstack([self.Y, Y_new])
+        inds = X[:, -1].astype(int)
+
+        # update normalisation
+        Y_norm = np.vstack([self.model.Y, np.zeros_like(Y_new)])
+        for i in np.unique(inds_new):
+            self.normmean[i] = np.mean(Y[inds == i])
+            if self.use_norm:
+                self.normsd[i] = np.ptp(Y[inds == i])
+            Y_norm[inds == i] = (Y[inds == i] - self.normmean[i]) / self.normsd[i]
+
+        # update model
+        self.model.Y_metadata = {'output_index': inds}
+        self.model.set_XY(X, Y_norm)
+
+    def redefine_data(self, X, Y):
+        """
+        Updates the model evidence (observations) dataset overwriting.
+        """
+        inds = X[:, -1].astype(int)
+        self.check_task_indices(inds)
+
+        # update normalisation
+        Y_norm = np.zeros_like(Y)
+        for i in range(self.num_tasks):
+            self.normmean[i] = np.mean(Y[inds == i])
+            if self.use_norm:
+                self.normsd[i] = np.ptp(Y[inds == i])
+            Y_norm[inds == i] = (Y[inds == i] - self.normmean[i]) / self.normsd[i]
+
+        # update model
+        self.model.Y_metadata = {'output_index': inds}
+        self.model.set_XY(X, Y_norm)
+
+    def get_best_xy(self, index=None):
+        """
+        Returns the lowest energy acquisitions (x, y).
+        """
+        if index is None:
+            x_best = []
+            y_best = []
+            for index in range(self.num_tasks):
+                Y_i = self.get_Y(index)
+                x_best.append(np.array(self.get_X(index)[np.argmin(Y_i)]))
+                y_best.append(np.min(Y_i))
+        else:
+            Y_i = self.get_Y(index)
+            x_best = np.array(self.get_X(index)[np.argmin(Y_i)])
+            y_best = np.min(Y_i)
+        return x_best, y_best
+
+    def get_X(self, index=None):
+        """
+        Returns observed X.
+        """
+        if index is None:
+            return self.model.X
+        else:
+            return self.model.X[self.inds == index, :-1]
+
+    def get_Y(self, index=None):
+        """
+        Returns observed Y.
+        """
+        if index is None:
+            Y = self.model.Y.copy()
+            for index in range(self.num_tasks):
+                Y[self.inds == index] *= self.normsd[index]
+                Y[self.inds == index] += self.normmean[index]
+            return Y
+        else:
+            Y_norm = self.model.Y[self.inds == index]
+            return Y_norm * self.normsd[index] + self.normmean[index]
+
+    @property
+    def X(self):
+        return self.get_X()
+
+    @property
+    def Y(self):
+        return self.get_Y()
+
+    @property
+    def inds(self):
+        return self.model.X[:, -1].astype(int)
```

### Comparing `aalto-boss-1.7.1/boss/bo/results.py` & `aalto-boss-1.8.0/boss/bo/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,16 +196,29 @@
     e.g., the collection of global minima (which is both extendable and sparse).
     In their raw form, these results are stored using the SparseList class.
     """
     def __init__(self, settings: Settings) -> None:
         self.data = {}
         self.extendable_names = []
         self.settings = settings
+        self.resolve_optim_domain(self.settings)
         self.batch_tracker = BatchTracker(num_init_batches=1)
 
+    def resolve_optim_domain(self, settings: Settings) -> None:
+        """Resolves data dimension and bounds based on settings."""
+        self.task_index = None
+        self.bounds = []
+        if settings is not None:
+            if settings.is_multi:
+                self.task_index = 0
+                task_bounds = [[self.task_index] * 2]
+                self.bounds = np.vstack((self.settings["bounds"], task_bounds))
+            else:
+                self.bounds = settings["bounds"]
+
     def add_defaults(self):
         """Adds predefined data structures for the most common results. """
         for name in ["X", "Y", "X_next"]:
             self.add_new(name, extendable=False)
         for name in ["mu_glmin", "nu_glmin"]:
             self.add_new(name, extendable=True, sparse=True, default=np.nan)
         for name in ['x_glmin', 'model_params']:
@@ -394,35 +407,36 @@
         """
         itr = wrap_index(itr, self.num_iters)
         X = self.select("X", np.arange(itr + 1))
         Y = self.select("Y", np.arange(itr + 1))
         kernel = KernelFactory.construct_kernel(self.settings)
         noise = self.settings["noise"]
         ynorm = self.settings["ynorm"]
-        model = Model(X, Y, kernel, noise, ynorm)
+        model = self.settings.model_class(X, Y, kernel, noise, ynorm)
         params = self.select("model_params", itr)
         if params is not None:
             model.set_unfixed_params(params)
         else:
             model.optimize()
             self['model_params'][itr] = model.get_unfixed_params()
         return model
 
     def calc_missing_minima(self) -> None:
         """Calculates global minima for the given iteration(s).
 
         If a minima if found to be missing from the results, it 
         will be stored (in addition to being returned from the function).
         """
+        bounds = self.bounds if hasattr(self, "bounds") else self.settings["bounds"]
         for itr in range(self.num_iters):
             if self['mu_glmin'].is_default(itr):
                 model = self.reconstruct_model(itr)
                 x_glmin, mu_glmin, nu_glmin = minimize_model(
                     model,
-                    self.settings["bounds"],
+                    bounds,
                     self.settings['optimtype'],
                     self.settings["kernel"],
                     self.settings["min_dist_acqs"],
                     accuracy=self.settings["minzacc"],
                 )
                 self['x_glmin'][itr] = x_glmin
                 self['mu_glmin'][itr] = mu_glmin
@@ -442,15 +456,19 @@
         Tuple[np.ndarray, np.ndarray]
             The best acquisition as a tuple (x, y).
             
         """
         itr_max = wrap_index(itr_max, self.num_iters)
         X = self.select("X", np.arange(itr_max + 1))
         Y = self.select("Y", np.arange(itr_max + 1))
-        i_best = np.argmin(Y[:,0])
+        if self.task_index is not None:
+            inds = X[:, -1].astype(int)
+            X = X[inds == self.task_index]
+            Y = Y[inds == self.task_index]
+        i_best = np.argmin(Y[:, 0])
         x_best = X[i_best]
         y_best = Y[i_best]
         return x_best, y_best
 
     def get_est_yrange(self, itr_max: int = -1) -> np.ndarray:
         """Finds the estimated range of y.
 
@@ -463,15 +481,19 @@
         Returns
         -------
         tuple
             The estimated y-range as a tuple (y_low, y_high).
         """
         itr_max = wrap_index(itr_max, self.num_iters)
         Y = self.select("Y", np.arange(itr_max + 1))
-        return np.min(Y), np.max(Y)
+        if self.task_index is not None:
+            X = self.select("X", np.arange(itr_max + 1))
+            inds = X[:, -1].astype(int)
+            Y = Y[inds == self.task_index]
+        return np.min(Y[:, 0]), np.max(Y[:, 0])
 
     def get_next_acq(self, itr: int = -1) -> np.ndarray:
         itr = wrap_index(itr, self.num_iters)
         if itr == self.batch_tracker.num_iters - 1:
             return self['X_next']
         else:
             return self.select('X', itr + 1)
@@ -493,17 +515,18 @@
             A BOResults object pre-filled with data from the output files.
         """
         self = cls.__new__(cls)
         self.data = {}
         self.extendable_names = ['mu_glmin', 'nu_glmin', 'x_glmin', 'model_params']
         settings = Settings.from_file(rstfile)
         self.settings = settings
+        self.resolve_optim_domain(self.settings)
 
         # Assign batch data.
-        dim = settings.dim
+        dim = settings.dim + int(settings.is_multi)
         acqs, batch_ind_lims = parse.parse_acqs(
             settings,
             outfile,
             self.settings['ygrad'],
         )
         self.data['X'] = acqs[:, :dim]
         self.data['Y'] = acqs[:, dim:]
```

### Comparing `aalto-boss-1.7.1/boss/bo/rstmanager.py` & `aalto-boss-1.8.0/boss/bo/rstmanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         Initializes the class with an array (settings.rstvals) containing the data
         read from an rst-file.
         """
         if rst_data is None:
             rst_data = np.array([])
         self.data = rst_data
         self.settings = settings
-        self.x_dim = settings.dim
+        self.x_dim = settings.dim + int(settings.is_multi)
         self.ygrad = settings["ygrad"]
         self.rstfile = settings["rstfile"]
 
     @property
     def X(self):
         if self.data.shape[0] > 0:
              return self.data[:, :self.x_dim]
@@ -99,15 +99,15 @@
             return None
 
     def get_y(self, i):
         """
         Returns the i:th acquisition evaluation (energy and gradient) from the
         rst-data or None if it can't be found.
         """
-        len_x = self.x_dim  # for convenience
+        len_x = self.x_dim
         len_y = 1
         if self.ygrad:
             len_y += len_x
         y_new = None
         yd_new = None
         # Actual functionality:
         if (
@@ -124,15 +124,15 @@
             return (y_new, yd_new)
 
     def get_theta(self, i, n):
         """
         Returns the model paramters at iteration i from the rst-data or None
         if they can't be found.
         """
-        len_x = self.x_dim  # for convenience
+        len_x = self.x_dim
         len_y = 1
         if self.ygrad:
             len_y += len_x
         a = len_x + len_y
 
         # Actual functionality:
         if (
```

### Comparing `aalto-boss-1.7.1/boss/io/dump.py` & `aalto-boss-1.8.0/boss/io/dump.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         npts = npts_per_dim**2
     else:
         # 1D slice
         npts = npts_per_dim
     assert len(x1) == npts
 
     # Full ND array of query points
-    X = np.empty((npts, settings.dim))
+    X = np.empty((npts, np.atleast_2d(defaults).shape[1]))
 
     # Fill ND query point array with default values
     if settings["pp_var_defaults"] is None:
         X[:] = defaults
     else:
         X[:] = settings["pp_var_defaults"]
```

### Comparing `aalto-boss-1.7.1/boss/io/ioutils.py` & `aalto-boss-1.8.0/boss/io/ioutils.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/io/main_output.py` & `aalto-boss-1.8.0/boss/io/main_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,21 @@
     def convergence_stop(self):
         """
         Announces BO stop due to global minimum convergence
         """
         msg = "Stopped BO due to global minimum prediction convergence"
         self.progress_msg(msg, 0, True)
 
+    def maxcost_stop(self):
+        """
+        Announces BO stop due to cost limit reached
+        """
+        msg = "Stopped BO due to cost limit reached"
+        self.progress_msg(msg, 0, True)
+
     def initpt_summary(self, X_new, Y_new, timer):
         s = "| Data point added to dataset (x y): \n"
         for i in range(len(Y_new)):
             s += io.data_line(X_new[i], [Y_new[i]], fstr="%18.10E")
         self.ensemble_size += len(X_new)
         s += f"\n| Total ensemble size: {self.ensemble_size}\n"
         s += f"\nIteration time [s]: {timer.getLapTime():8.3f}"
```

### Comparing `aalto-boss-1.7.1/boss/io/parse.py` & `aalto-boss-1.8.0/boss/io/parse.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/keywords.py` & `aalto-boss-1.8.0/boss/keywords.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 categories = {}
 categories[(bool, 0)] = {
     "ygrad": False,
     "pp_models": False,
     "pp_acq_funcs": False,
     "pp_truef_at_glmins": False,
     "initupdate": True,
-    "ynorm": False,
+    "ynorm": None,
 }
 categories[(int, 0)] = {
     "initpts": 5,
     "iterpts": None,
     "updatefreq": 1,
     "cores": 1,
     "updaterestarts": 2,
@@ -51,51 +51,70 @@
     "mep_nebsteps": 20,
     "pp_truef_npts": None,
     "hmciters": 0,
     "minzacc": 15,
     "minfreq": 1,
     "seed": None,
     "parallel_optims": 0,
+    "num_tasks": None,
+    "W_rank": 1,
 }
 categories[(int, 1)] = {
+    "task_initpts": None,
     "pp_iters": None,
     "pp_model_slice": None,
 }
 categories[(float, 0)] = {
     "noise": 1e-12,
     "acqtol": 0.001,
     "min_dist_acqs": None,
+    "maxcost": None,
     "mep_maxe": None,
     "pp_local_minima": None,
 }
 categories[(float, 1)] = {
     "yrange": [-10.0, 10.0],
     "glmin_tol": None,
     "periods": None,
     "acqfnpars": np.array([]),
+    "task_cost": None,
     "pp_var_defaults": None,
     "thetainit": None,
+    "W_init": None,
+    "kappa_init": None,
+    "W_priorpar": None,
+    "kappa_priorpar": None,
+}
+categories[(float, 2)] = {
+    "bounds": None, 
+    "thetapriorpar": None, 
+    "thetabounds": None,
 }
-categories[(float, 2)] = {"bounds": None, "thetapriorpar": None, "thetabounds": None}
 categories[(str, 0)] = {
     "outfile": "boss.out",
     "ipfile": "boss.in",
     "rstfile": "boss.rst",
+    "model_name": None,
     "acqfn_name": "elcb",
     "inittype": "sobol",
     "optimtype": "score",
     "thetaprior": "gamma",
-    "userfn": None,
+    "W_prior": None,
+    "kappa_prior": None,
     "costfn": None,
     "costtype": 'divide',
 }
 categories[(str, 1)] = {
+    "userfn": None,
     "kernel": ["rbf"],
     "var_types": None,
 }
+categories[(str, 2)] = {
+    "userfn_list": None,
+}
 
 
 def get_copied_categories():
     """Returns deep copies of all categories.
 
     Useful when setting default values using the category
     dicts and we want to avoid changing the default value
@@ -160,15 +179,18 @@
             val = np.asarray([_eval_bool(x) for x in val_split])
         else:
             val = [cat_type(x) for x in val_split]
             if cat_type in [int, float]:
                 val = np.asarray(val)
     elif cat_dim == 2:
         rows = val_str.split(";")
-        val = np.asarray([np.fromstring(row, sep=" ") for row in rows])
+        if cat_type == str:
+            val = [row.split() for row in rows]
+        else:
+            val = np.asarray([np.fromstring(row, sep=" ") for row in rows])
     else:
         raise ValueError(f"Cannot convert '{val_str}' to {category}")
     return val
 
 
 def stringify(val):
     """Convert a Python type to a BOSS-style string.
@@ -191,35 +213,36 @@
             val_str = " ".join([str(x) for x in val])
     elif val_ndim >= 2:
         val = np.array(val)
         val_str = str(val)
         val_str = val_str.replace("\n", ";")
         val_str = val_str.replace("[", "")
         val_str = val_str.replace("]", "")
+        val_str = val_str.replace("\'", "")
     return val_str
 
 
-def func_from_keyword(func_str):
+def func_from_keyword(func_arr):
     """"""
-    fsplit = func_str.split()
-    if len(fsplit) == 2:
-        func_name = fsplit[1]
+    if len(func_arr) == 2:
+        func_name = func_arr[1]
     else:
         func_name = "f"
-    func_path = Path(fsplit[0])
+    func_path = Path(func_arr[0])
     sys.path.append(str(func_path.parent))
     func = getattr(importlib.import_module(func_path.stem), func_name)
     return func
 
 
 def func_to_keyword(func):
     """
     The user function is either an ordinary function or a user defined,
     callable object. In the second case we must pass the type and not the
     object instance to inspect.getfile.
     """
     if type(func).__name__ == "function":
         func_path = getfile(func)
         func_name = func.__name__
-        return f"{func_path} {func_name}"
+        path_arr = [func_path,  func_name]
+        return path_arr
     else:
         return None
```

### Comparing `aalto-boss-1.7.1/boss/mep/forest.py` & `aalto-boss-1.8.0/boss/mep/forest.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,18 @@
         all_children = []
         for tree in self.trees:
             all_children.extend(tree.get_all_children())
         return all_children
 
     def grow(self, model, eps, max_e, space):
         boundlength = space.bounds[1, :] - space.bounds[0, :]
-        dim = model.dim
+        dim = space.bounds.shape[1]
         new_point = np.random.random(dim) * boundlength + space.bounds[0, :]
+        if dim < model.dim:
+            new_point = np.hstack((new_point, 0))  # add task index
         new_e = model.predict(np.vstack(np.atleast_2d(new_point)))[0][0, 0]
         if new_e < max_e:
             closest, dist = self.get_closest_point(new_point, space)
             new_point = space.trace(closest.coords, new_point, model, eps, max_e)
             if not np.prod(new_point == closest.coords):
                 closest.children.append(Node(new_point, closest))
```

### Comparing `aalto-boss-1.7.1/boss/mep/mep.py` & `aalto-boss-1.8.0/boss/mep/mep.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/mep/mepmain.py` & `aalto-boss-1.8.0/boss/mep/mepmain.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
         # plot
         if self.minima.shape[1] == 2:
             self.plot2D(settings, mep)
 
     def get_model(self, settings, rstfile, main_output):
         input_data = parse.parse_input_file(rstfile)
         rst_data = input_data['rst_data']
-        acqs, mod_par = split_rst_data(rst_data, settings.dim)
+        dim = settings.dim + int(settings.is_multi)
+        acqs, mod_par = split_rst_data(rst_data, dim)
         self.model = recreate_model(
             settings,
             acqs[:, 1:],
             mod_par[-1, 1:],
         )
 
     def get_minima(self, minimafile, main_output):
```

### Comparing `aalto-boss-1.7.1/boss/mep/neb.py` & `aalto-boss-1.8.0/boss/mep/neb.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/mep/node.py` & `aalto-boss-1.8.0/boss/mep/node.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/mep/path.py` & `aalto-boss-1.8.0/boss/mep/path.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/mep/space.py` & `aalto-boss-1.8.0/boss/mep/space.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/pp/plot.py` & `aalto-boss-1.8.0/boss/pp/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 
 
 def plot_data_acquisitions(settings, dest_file, acqs, min_preds):
     """
     Plots minimum predictions and uncertainty, acquisition energies
     and locations as a function of iteration.
     """
+    dim = settings.dim + int(settings.is_multi)
     itNo_acqs = np.clip(acqs[:, 0], int(min_preds[0, 0]), np.inf)
-    x = acqs[:, 2 : settings.dim + 2]
-    y = acqs[:, settings.dim + 2]
+    x = acqs[:, 2 : dim + 2]
+    y = acqs[:, dim + 2]
     itNo_mp = min_preds[:, 0]
-    xhat = min_preds[:, 2 : settings.dim + 2]
+    xhat = min_preds[:, 2 : dim + 2]
     muhat = min_preds[:, -2]
     nuhat = min_preds[:, -1]
 
     plt.subplot(211)
     plt.fill_between(itNo_mp, muhat + nuhat, muhat, color="lightgrey")
     plt.fill_between(itNo_mp, muhat - nuhat, muhat, color="lightgrey")
     plt.plot(itNo_mp, muhat + nuhat, "grey", linewidth=2)
@@ -129,16 +130,16 @@
 
 def plot_hyperparameters(settings, dest_file, hypers, legends=True):
     """
     Plots GP model unfixed hyperparameters (variances and lengthscales)
     as a function of iteration.
     """
     itNo = hypers[:, 0]
-    var = hypers[:, 2]
-    ls = hypers[:, 3:]
+    var = hypers[:, 2] if not settings.is_multi else np.ones_like(itNo)
+    ls = hypers[:, 3:] if not settings.is_multi else hypers[:, 2:]
 
     colors = [
         "blue",
         "red",
         "green",
         "brown",
         "yellow",
@@ -247,33 +248,34 @@
     axis_labels=None,
     legends=True,
     paths=None,
 ):
     """
     Plots a (max 2D) slice of the model.
     """
+    dim = settings.dim + int(settings.is_multi)
     if xnext is not None:
-        xnext = shape_consistent_X(xnext, settings.dim)
+        xnext = shape_consistent_X(xnext, dim)
 
-    coords = model_data[:, : settings.dim]
+    coords = model_data[:, : dim]
     mu, nu = model_data[:, -2], model_data[:, -1]
     slice_dim = (
         1 if settings["pp_model_slice"][0] == settings["pp_model_slice"][1] else 2
     )
     if axis_labels is None:
         axis_labels = [
             r"$x_%i$" % (settings["pp_model_slice"][0] + 1),
             r"$x_%i$" % (settings["pp_model_slice"][1] + 1),
         ]
 
     if slice_dim == 1:
         x1 = coords[:, settings["pp_model_slice"][0]]
 
         if truef is not None:
-            crds = truef[:, : settings.dim]
+            crds = truef[:, : dim]
             tf = truef[:, -1]
             tfx1 = crds[:, settings["pp_model_slice"][0]]
             plt.plot(tfx1, tf, "k", linewidth=5, label="f(x)")
 
         if incl_uncert:
             plt.fill_between(x1, mu + nu, mu, color="lightgrey")
             plt.fill_between(x1, mu - nu, mu, color="lightgrey")
@@ -410,17 +412,18 @@
     axis_labels=None,
     legends=True,
 ):
     """
     Plots a (max 2D) slice of the acquisition function. Can include also
     acquisitions, xhat and xnext if those are given.
     """
+    dim = settings.dim + int(settings.is_multi)
     if xnext is not None:
-        xnext = shape_consistent_X(xnext, settings.dim)
-    coords = acqf_data[:, : settings.dim]
+        xnext = shape_consistent_X(xnext, dim)
+    coords = acqf_data[:, : dim]
     af = acqf_data[:, -1]
     slice_dim = (
         1 if settings["pp_model_slice"][0] == settings["pp_model_slice"][1] else 2
     )
     if axis_labels is None:
         axis_labels = [
             r"$x_%i$" % (settings["pp_model_slice"][0] + 1),
@@ -518,15 +521,16 @@
         )
 
 
 def plot_truef(settings, dest_file, truef_data, axis_labels=None):
     """
     Plots a (max 2D) slice of the true function.
     """
-    coords = truef_data[:, : settings.dim]
+    dim = settings.dim + int(settings.is_multi)
+    coords = truef_data[:, : dim]
     tf = truef_data[:, -1]
     slice_dim = (
         1 if settings["pp_model_slice"][0] == settings["pp_model_slice"][1] else 2
     )
     if axis_labels is None:
         axis_labels = [
             r"$x_%i$" % (settings["pp_model_slice"][0] + 1),
```

### Comparing `aalto-boss-1.7.1/boss/pp/pp_main.py` & `aalto-boss-1.8.0/boss/pp/pp_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     def _setup(self):
         """Common setup for all factory methods."""
 
         self.batch_tracker = self.results.batch_tracker
 
         if self.settings["pp_iters"] is None:
-            self.pp_iters = np.arange(0, self.settings["iterpts"] + 1)
+            self.pp_iters = np.arange(0, self.results.num_iters)
         else:
             self.pp_iters = self.settings['pp_iters']
 
         # User-specified model slices are interpreted as being indexed
         # from 1, so we convert to 0-based indexing here.
         self.settings["pp_model_slice"][:2] -= 1
 
@@ -362,28 +362,29 @@
             curr_xhat = self.results.select("x_glmin", it)
 
             # Local minima
             if sts["pp_local_minima"] is not None:
                 self.main_output.progress_msg("Finding model local minima")
                 mins = Minimization.minimize(
                     model.predict_mean_grad,
-                    sts["bounds"],
+                    self.results.bounds,
                     sts["kernel"],
                     np.hstack([model.X, model.Y]),
                     sts["min_dist_acqs"],
                     accuracy=sts["pp_local_minima"],
                     args=(),
                     lowest_min_only=False,
                 )
 
+                dim = sts.dim + int(sts.is_multi)
                 mins = sorted(mins, key=lambda x: (x[1]))
-                minima_data = [[]] * (sts.dim + 2)
+                minima_data = [[]] * (dim + 2)
                 for m in mins:
                     p = []
-                    for i in range(sts.dim):
+                    for i in range(dim):
                         p.append(m[0][i])
                     mu, var = model.predict(m[0])
                     nu = np.sqrt(var)
                     p.append(mu)
                     p.append(nu)
                     minima_data = np.insert(minima_data, len(minima_data[0]), p, axis=1)
```

### Comparing `aalto-boss-1.7.1/boss/utils/arrays.py` & `aalto-boss-1.8.0/boss/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/utils/minimization.py` & `aalto-boss-1.8.0/boss/utils/minimization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import warnings
-import os
-
-warnings.filterwarnings("ignore")  # ignore warnings
 import numpy as np
 import copy
-from operator import itemgetter
 import scipy.optimize
+import multiprocessing
+
+from operator import itemgetter
 from scipy.spatial.distance import euclidean
 
 import boss.utils.sobol_seq as sobol_seq
-import multiprocessing
+warnings.filterwarnings("ignore")  # ignore warnings
 
 # Module-global name for the multiprocessing pool. We only create it once in
 # Minimization.set_parallel()
 process_pool = None
 
 
 class Minimization:
@@ -45,24 +44,25 @@
             maxiter=1e4,
             maxls=15,
         )
         rc = d["warnflag"] == 0
         return x, f, rc
 
     @staticmethod
-    def _run_minimizer_with_finite_gradients(func, x0, bounds, args):
+    def _run_minimizer_with_finite_gradients(arguments):
         """
         Runs a single L-BFGS-B minimization starting from x0
         Approximate gradients using finite difference
 
-        func: The function to minimize. Must return value and gradients
+        func: The function to minimize. Must return value
         x0: Starting value
         bounds: Bounds passed to the minimizer
         args: arguments passed to the function func
         """
+        func, x0, bounds, args = arguments
         x, f, d = scipy.optimize.fmin_l_bfgs_b(
             func,
             x0,
             bounds=bounds,
             args=args,
             factr=1e8,
             pgtol=1e-4,
@@ -85,76 +85,83 @@
         # os.environ['OMP_NUM_THREADS'] = '1'
 
         # Create a multiprocessing pool
         if num_procs > 0:
             process_pool = multiprocessing.Pool(num_procs)
 
     @staticmethod
-    def _minimize(arguments):
+    def _minimize(arguments, has_gradient):
         """Wrapper on top of _run_minimizer for running either in parallel or
         in serial depending on whether a process pool has been created by
         Minimization.set_parallel().
         """
+        if not has_gradient:
+            minimizer = Minimization._run_minimizer_with_finite_gradients
+        else:
+            minimizer = Minimization._run_minimizer
         if process_pool is not None:
-            return_values = process_pool.map(Minimization._run_minimizer, arguments)
+            return_values = process_pool.map(minimizer, arguments)
             minima = []
             for returned_tuple in return_values:
                 x, f, s = returned_tuple
                 if s:
                     minima.append([list(x), float(f)])
         else:
             minima = []
             for arg in arguments:
-                x, f, s = Minimization._run_minimizer(arg)
+                x, f, s = minimizer(arg)
                 if s:
                     minima.append([list(x), float(f)])
         return minima
 
     @staticmethod
     def minimize(
         func,
         bounds,
         kerntype,
         acqs,
         min_dist_acqs,
         accuracy=0.3,
         args=(),
         lowest_min_only=True,
+        has_gradient=True
     ):
         """
         Tries to find global minimum of func by starting minimizers from
         accuracy*100 percentage of lowest acquisitions. func has to return both
         value and gradient given an x of same length as bounds.
         """
         acqsx = np.array(copy.deepcopy(acqs[:, : len(bounds)]))
         acqsy = np.array(copy.deepcopy(acqs[:, -1:]))
 
         points = []
         for i in range(len(acqsy)):
-            points.append([list(acqsx[i]), float(acqsy[i])])
+            if Minimization._within_bounds(acqsx[i], bounds):
+                points.append([list(acqsx[i]), float(acqsy[i])])
 
         points = Minimization._remove_duplicates(points, min_dist_acqs)
         points = sorted(points, key=itemgetter(1))
         X, Y = zip(*points)
         ind_last = min(len(Y) - 1, max(0, round(accuracy * (len(Y) - 1))))
         X = X[: ind_last + 1]
         X = np.array([X[i] for i in range(len(X))])
 
         widebounds = bounds.copy()
-        p = np.array(kerntype) == "stdp"
+        p = np.full((len(bounds),), False)
+        p[np.where(np.array(kerntype) == "stdp")] = True
         l = bounds[:, 1] - bounds[:, 0]
         widebounds[p, 0] -= 0.1 * l[p]
         widebounds[p, 1] += 0.1 * l[p]
 
         # Run bounded minimization on bounds which have been stretched for
         # periodic dimensions, then return the minima which have been found
         # inside the bounds. This prevents minima from being falsely
         # identified at the periodic boundaries.
         arguments = [(func, acq, widebounds, args) for acq in X]
-        minima = Minimization._minimize(arguments)
+        minima = Minimization._minimize(arguments, has_gradient)
 
         if len(minima) == 0:
             lo_acq = [list(acqsx[np.argmin(acqsy)]), float(np.min(acqsy))]
             minima.append(lo_acq)
 
         if lowest_min_only:
             globalmin = minima[0]
@@ -164,16 +171,16 @@
             return globalmin
         else:
             minima = Minimization._remove_duplicates(minima, min_dist_acqs)
             return minima
 
     @staticmethod
     def minimize_from_sobol(
-        func, bounds, num_pts, shift, args=(), lowest_min_only=True
-    ):
+        func, bounds, num_pts, shift, args=(), lowest_min_only=True,
+            has_gradient=True):
         """
         Tries to find global minimum of func by starting minimizers from
         num_pts shifted sobol points. func has to return both
         value and gradient given an x of same length as bounds.
         """
         sobs = np.transpose(sobol_seq.i4_sobol_generate(len(bounds), num_pts, 1))
 
@@ -182,15 +189,15 @@
             p = []
             for n in range(len(bounds)):
                 bl = bounds[n][1] - bounds[n][0]
                 p.append(bounds[n][0] + (sobs[i, n] * bl + shift[n]) % bl)
             points.append(p)
 
         arguments = [(func, pnt, bounds, args) for pnt in points]
-        minima = Minimization._minimize(arguments)
+        minima = Minimization._minimize(arguments, has_gradient)
 
         if len(minima) == 0:
             err_min = [list(points[-1]), float(func(points[-1], args[0], args[1])[0])]
             minima.append(err_min)  # later a better solution here?
 
         if lowest_min_only:
             globalmin = minima[0]
@@ -199,15 +206,15 @@
                     globalmin = minimum
             return globalmin
         else:
             return minima
 
     @staticmethod
     def minimize_from_random(
-        func, bounds, num_pts, args=(), lowest_min_only=True
+        func, bounds, num_pts, args=(), lowest_min_only=True, has_gradient=True
     ):
         """
         Tries to find global minimum of func by starting minimizers from
         num_pts random points (min 10 max 100). func has to return both
         value and gradient given an x of same length as bounds.
         """
         if num_pts < 10:
@@ -222,16 +229,16 @@
             p = []
             for n in range(len(bounds)):
                 bl = bounds[n][1] - bounds[n][0]
                 p.append(bounds[n][0] + rands[i, n] * bl)
             points.append(p)
 
         arguments = [(func, pnt, bounds, args) for pnt in points]
-        minima = Minimization._minimize(arguments)
-
+        minima = Minimization._minimize(arguments, has_gradient)
+        # TODO : Test here minima = []
         if len(minima) == 0:
             err_min = [list(points[-1]), float(func(points[-1])[0])]
             minima.append(err_min)  # later a better solution here?
 
         if lowest_min_only:
             globalmin = minima[0]
             for minimum in minima:
@@ -240,15 +247,15 @@
             return globalmin
         else:
             return minima
 
     @staticmethod
     def minimize_using_score(
         func, bounds, num_rnd_samples=10000, num_anchor=1, acqs=None, args=(),
-            lowest_min_only=True):
+            lowest_min_only=True, has_gradient=True):
         """Searches the global minimum of func by starting minimizers from
         num_anchor points. The points are chosen according to a score
         criteria, here the function itself is used to obtain the scores.
         """
         uniform_samples = np.random.uniform(
             low=bounds[:, 0], high=bounds[:, 1],
             size=(num_rnd_samples, len(bounds)))
@@ -257,15 +264,15 @@
             scores = scores[0]   # Ignore gradient
         sorted_idxs = np.argsort(scores.squeeze())
         starting_points = uniform_samples[sorted_idxs[:num_anchor]]
         if acqs is not None:
             # Add point with lowest func value to starting_points
             starting_points = np.vstack((starting_points, acqs))
         min_args = [(func, point, bounds, args) for point in starting_points]
-        minima = Minimization._minimize(min_args)
+        minima = Minimization._minimize(min_args, has_gradient)
 
         if len(minima) == 0:
             lowest_value = func(uniform_samples[sorted_idxs[0]])
             if isinstance(lowest_value, tuple):
                 lowest_value = lowest_value[0].squeeze()
             minima.append([uniform_samples[sorted_idxs[0]].tolist(),
                            lowest_value])
@@ -276,14 +283,22 @@
                     lowest_min = minimum
             return lowest_min
         else:
             return minima
 
 
     @staticmethod
+    def _within_bounds(x, bounds):
+        """
+        Check whether location x is within bounds.
+        """
+        return np.all(x >= bounds[:, 0]) and np.all(x <= bounds[:, 1])
+
+
+    @staticmethod
     def _remove_duplicates(original, min_distance):
         """
         Removes duplicates from a list of found local minima given a minimum
         distance between distinct minima.
         """
         if len(original) == 0:
             return original
```

### Comparing `aalto-boss-1.7.1/boss/utils/sobol_seq.py` & `aalto-boss-1.8.0/boss/utils/sobol_seq.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/utils/sparselist.py` & `aalto-boss-1.8.0/boss/utils/sparselist.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/boss/utils/timer.py` & `aalto-boss-1.8.0/boss/utils/timer.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.7.1/setup.py` & `aalto-boss-1.8.0/setup.py`

 * *Files identical despite different names*

