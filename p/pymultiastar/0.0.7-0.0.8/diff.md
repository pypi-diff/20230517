# Comparing `tmp/pymultiastar-0.0.7.tar.gz` & `tmp/pymultiastar-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultiastar-0.0.7.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pymultiastar-0.0.8.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pymultiastar-0.0.7.tar` & `pymultiastar-0.0.8.tar`

### file list

```diff
@@ -1,63 +1,70 @@
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/.github/dependabot.yml
--rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/.github/workflows/pip.yml
--rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/.gitignore
--rw-r--r--   0        0        0     1417 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/CMakeLists.txt
--rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/LICENSE
--rw-r--r--   0        0        0     5378 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/README.md
--rw-r--r--   0        0        0   585757 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/assets/imgs/newyork_map.png
--rw-r--r--   0        0        0   578063 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/assets/imgs/newyork_solved_1.png
--rw-r--r--   0        0        0   543823 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/assets/imgs/newyork_solved_2.png
--rw-r--r--   0        0        0   839076 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/assets/imgs/simple_world_3d.png
--rw-r--r--   0        0        0    22832 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/assets/imgs/simple_world_3d_tradeoff.png
--rw-r--r--   0        0        0    99021 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/assets/imgs/tradeoff.png
--rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/contributing.md
--rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/contributing.md
--rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/css/material.css
--rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0     1033 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/css/style.css
--rw-r--r--   0        0        0     1613 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/gen_ref_nav.py
--rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/index.md
--rw-r--r--   0        0        0      394 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/js/mathjaxhelper.js
--rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/license.md
--rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/reference/index.md
--rw-r--r--   0        0        0       28 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/tutorials/geoplanner.md
--rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/docs/tutorials/simple.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/examples/__init__.py
--rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/examples/log.py
--rw-r--r--   0        0        0     1831 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/examples/run_maze_2d.py
--rw-r--r--   0        0        0     3698 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/examples/run_scenarios.py
--rw-r--r--   0        0        0     1202 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/examples/run_simple_demo.py
--rw-r--r--   0        0        0     2521 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/examples/run_simple_world_3d.py
--rw-r--r--   0        0        0     2012 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/mkdocs.yml
--rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/noxfile.py
--rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/output/.gitignore
--rw-r--r--   0        0        0     1537 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/scripts/upload.sh
--rw-r--r--   0        0        0     8764 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/include/pymultiastar.hpp
--rw-r--r--   0        0        0     3063 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/main.cpp
--rw-r--r--   0        0        0     1392 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/__init__.py
--rw-r--r--   0        0        0     2984 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/_core.pyi
--rw-r--r--   0        0        0      395 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/geoplanner/__init__.py
--rw-r--r--   0        0        0     8648 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/geoplanner/geoplanner.py
--rw-r--r--   0        0        0     4970 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/geoplanner/helper.py
--rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/geoplanner/log.py
--rw-r--r--   0        0        0     2807 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/geoplanner/types.py
--rw-r--r--   0        0        0      653 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/types.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/visualization/__init__.py
--rw-r--r--   0        0        0     1914 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/visualization/img2d_helpers.py
--rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/visualization/log.py
--rw-r--r--   0        0        0     9641 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar/visualization/vis3d_helpers.py
--rw-r--r--   0        0        0    18133 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/src/pymultiastar.cpp
--rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/tests/fixtures/.gitignore
--rw-r--r--   0        0        0  1869483 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/tests/fixtures/maze_large.png
--rw-r--r--   0        0        0    38313 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/tests/fixtures/maze_small.png
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/tests/fixtures/world/.gitignore
--rw-r--r--   0        0        0     2582 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/tests/fixtures/world/annarbor/plan.json
--rw-r--r--   0        0        0 38263232 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/tests/fixtures/world/annarbor/voxel_map.npy
--rw-r--r--   0        0        0     4540 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/tests/fixtures/world/newyork/plan.json
--rw-r--r--   0        0        0 68625128 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/tests/fixtures/world/newyork/voxel_map.npy
--rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/tests/test_basic.py
--rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/tests/test_geo_helper.py
--rw-r--r--   0        0        0     7283 2022-11-09 12:37:21.000000 pymultiastar-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     1748 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1417 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/CMakeLists.txt
+-rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/LICENSE
+-rw-r--r--   0        0        0     5378 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/README.md
+-rw-r--r--   0        0        0   585757 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/assets/imgs/newyork_map.png
+-rw-r--r--   0        0        0   578063 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/assets/imgs/newyork_solved_1.png
+-rw-r--r--   0        0        0   543823 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/assets/imgs/newyork_solved_2.png
+-rw-r--r--   0        0        0   839076 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/assets/imgs/simple_world_3d.png
+-rw-r--r--   0        0        0    22832 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/assets/imgs/simple_world_3d_tradeoff.png
+-rw-r--r--   0        0        0    99021 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/assets/imgs/tradeoff.png
+-rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/contributing.md
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/contributing.md
+-rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/css/material.css
+-rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0     1033 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/css/style.css
+-rw-r--r--   0        0        0     1613 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/index.md
+-rw-r--r--   0        0        0      394 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/js/mathjaxhelper.js
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/license.md
+-rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/reference/index.md
+-rw-r--r--   0        0        0       28 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/tutorials/geoplanner.md
+-rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/docs/tutorials/simple.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/examples/__init__.py
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/examples/log.py
+-rw-r--r--   0        0        0     1831 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/examples/run_maze_2d.py
+-rw-r--r--   0        0        0     3634 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/examples/run_scenarios.py
+-rw-r--r--   0        0        0     1202 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/examples/run_simple_demo.py
+-rw-r--r--   0        0        0     2521 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/examples/run_simple_world_3d.py
+-rw-r--r--   0        0        0     2012 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/mkdocs.yml
+-rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/noxfile.py
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/output/.gitignore
+-rw-r--r--   0        0        0     1605 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/scripts/upload.sh
+-rw-r--r--   0        0        0     8764 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/include/pymultiastar.hpp
+-rw-r--r--   0        0        0     3063 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/main.cpp
+-rw-r--r--   0        0        0     1392 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/__init__.py
+-rw-r--r--   0        0        0     3110 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/_core.pyi
+-rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/geoplanner/__init__.py
+-rw-r--r--   0        0        0     8193 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/geoplanner/geoplanner.py
+-rw-r--r--   0        0        0     4970 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/geoplanner/helper.py
+-rw-r--r--   0        0        0     3160 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/geoplanner/landing_selection.py
+-rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/geoplanner/log.py
+-rw-r--r--   0        0        0     3662 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/geoplanner/types.py
+-rw-r--r--   0        0        0      832 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/geoplanner/util.py
+-rw-r--r--   0        0        0      891 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/scripts/aclm.py
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/scripts/log.py
+-rw-r--r--   0        0        0      653 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/types.py
+-rw-r--r--   0        0        0     2655 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/util.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/visualization/__init__.py
+-rw-r--r--   0        0        0     1914 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/visualization/img2d_helpers.py
+-rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/visualization/log.py
+-rw-r--r--   0        0        0    10556 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar/visualization/vis3d_helpers.py
+-rw-r--r--   0        0        0    18133 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/src/pymultiastar.cpp
+-rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/fixtures/.gitignore
+-rw-r--r--   0        0        0  1869483 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/fixtures/maze_large.png
+-rw-r--r--   0        0        0    38313 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/fixtures/maze_small.png
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/fixtures/world/.gitignore
+-rw-r--r--   0        0        0    20739 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/fixtures/world/annarbor/landing_sites.csv
+-rw-r--r--   0        0        0     2637 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/fixtures/world/annarbor/plan.json
+-rw-r--r--   0        0        0 38263232 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/fixtures/world/annarbor/voxel_map.npy
+-rw-r--r--   0        0        0   107901 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/fixtures/world/newyork/landing_sites.csv
+-rw-r--r--   0        0        0     1680 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/fixtures/world/newyork/plan.json
+-rw-r--r--   0        0        0 68625128 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/fixtures/world/newyork/voxel_map.npy
+-rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/test_basic.py
+-rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/tests/test_geo_helper.py
+-rw-r--r--   0        0        0     7320 2022-11-09 12:37:21.000000 pymultiastar-0.0.8/PKG-INFO
```

### Comparing `pymultiastar-0.0.7/.github/workflows/pip.yml` & `pymultiastar-0.0.8/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/.github/workflows/wheels.yml` & `pymultiastar-0.0.8/.github/workflows/wheels.yml`

 * *Files 8% similar despite different names*

```diff
@@ -42,17 +42,17 @@
     steps:
     - uses: actions/checkout@v3
       with:
         submodules: true
 
     - uses: pypa/cibuildwheel@v2.12.3
       env:
-        CIBW_TEST_REQUIRES: pytest pyproj>=3.0
+        CIBW_TEST_REQUIRES: pytest pyproj>=3.0 scipy>=1.10.0
         CIBW_ARCHS_MACOS: universal2
-        CIBW_ARCHS_WINDOWS: auto ARM64
+        CIBW_ARCHS_WINDOWS: auto64 ARM64
         CIBW_ARCHS_LINUX: auto64
         CIBW_SKIP: "cp27-* cp35-* cp36-* cp37-* cp38-* pp* *musllinux*"
 
     - name: Verify clean directory
       run: git diff --exit-code
       shell: bash
```

### Comparing `pymultiastar-0.0.7/.gitignore` & `pymultiastar-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/.pre-commit-config.yaml` & `pymultiastar-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/LICENSE` & `pymultiastar-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/README.md` & `pymultiastar-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/assets/imgs/newyork_map.png` & `pymultiastar-0.0.8/assets/imgs/newyork_map.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/assets/imgs/newyork_solved_1.png` & `pymultiastar-0.0.8/assets/imgs/newyork_solved_1.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/assets/imgs/newyork_solved_2.png` & `pymultiastar-0.0.8/assets/imgs/newyork_solved_2.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/assets/imgs/simple_world_3d.png` & `pymultiastar-0.0.8/assets/imgs/simple_world_3d.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/assets/imgs/simple_world_3d_tradeoff.png` & `pymultiastar-0.0.8/assets/imgs/simple_world_3d_tradeoff.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/assets/imgs/tradeoff.png` & `pymultiastar-0.0.8/assets/imgs/tradeoff.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/docs/css/style.css` & `pymultiastar-0.0.8/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/docs/gen_ref_nav.py` & `pymultiastar-0.0.8/docs/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/docs/tutorials/simple.md` & `pymultiastar-0.0.8/docs/tutorials/simple.md`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/examples/run_maze_2d.py` & `pymultiastar-0.0.8/examples/run_maze_2d.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/examples/run_scenarios.py` & `pymultiastar-0.0.8/examples/run_scenarios.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,51 +3,38 @@
 import json
 import uuid
 import logging
 from pymultiastar.visualization.vis3d_helpers import visualize_plan, plot_pareto
 from pymultiastar.geoplanner.helper import EnhancedJSONEncoder
 from rich.prompt import Prompt
 
-from pymultiastar.geoplanner import (
-    GeoPlanner,
-    Scenario,
-    GPS,
-    LandingSite,
-    create_planner_from_configuration,
-)
+from pymultiastar.geoplanner import GeoPlanner, Scenario, GPS, LandingSite
+from pymultiastar.geoplanner.landing_selection import LSSPlanner
+from pymultiastar.geoplanner.util import create_planner_from_configuration
 from pymultiastar.types import LogLevel
 from log import logger
 
 
 app = typer.Typer()
 THIS_DIR = Path(__file__).parent
 WORLD_DIR = Path(__file__).parent.parent / "tests" / "fixtures" / "world"
 ANNARBOR_PLAN = WORLD_DIR / "annarbor/plan.json"
 OUTPUT_DIR = THIS_DIR.parent / "output"
 
 
-def plan_scenario(scenario: Scenario, geo_planner: GeoPlanner):
+def plan_scenario(scenario: Scenario, geo_planner: GeoPlanner, lss_planner: LSSPlanner):
     start_pos = GPS(*scenario["position"])
-    if scenario.get("landing_sites") is None:
-        raise NotImplementedError(
-            "This module relies upon the user providing landing sites"
-        )
-    assert scenario["landing_sites"] is not None
+    ls_list = lss_planner.query(start_pos, **scenario["lss_query_kwargs"])
 
-    ls_list = [
-        LandingSite(
-            GPS(*ls["position"]),
-            landing_site_risk=ls["landing_site_risk"],
-        )
-        for ls in scenario["landing_sites"]
-    ]
-    if scenario.get("planner_kwargs") is not None:
-        logger.warning(
-            "Not implemented! Updating planner arguments in each scenario is not yet supported!"
+    if scenario.get("planner_kwargs", None) is not None:
+        assert scenario["planner_kwargs"] is not None
+        npc = scenario["planner_kwargs"].get(
+            "normalizing_path_cost", geo_planner.planner_kwargs.normalizing_path_cost
         )
+        geo_planner.planner.normalizing_path_cost = npc
 
     logger.debug("Start Pos: %s", start_pos)
     logger.debug("Landing Sites: %s", ls_list)
 
     result = geo_planner.plan_multi_goal(start_pos, ls_list)
     logger.debug("Plan Result: %s", result)
 
@@ -83,15 +70,15 @@
     output_dir: Path = OUTPUT_DIR,
 ):
     # set log level
     logger.setLevel(getattr(logging, log_level.value))
     logging.getLogger().setLevel(getattr(logging, log_level.value))
 
     # read planner data
-    geo_planner, planner_data = create_planner_from_configuration(plan)
+    geo_planner, lss_planner, planner_data = create_planner_from_configuration(plan)
     voxel_meta = planner_data["voxel_meta"]
     scenarios = planner_data["scenarios"]
 
     scenario_results = []
     chosen_scenarios = []
     if not run_all_scenarios:
         # choose a scenario in the planner data
@@ -102,15 +89,15 @@
         )
         scenario = next(item for item in scenarios if item["name"] == scenario_str)
         chosen_scenarios.append(scenario)
     else:
         chosen_scenarios = scenarios
 
     for scenario in chosen_scenarios:
-        scenario_result, actions = plan_scenario(scenario, geo_planner)
+        scenario_result, actions = plan_scenario(scenario, geo_planner, lss_planner)
         scenario_results.append(scenario_result["plan_results"])
         if visualize:
             visualize_plan(
                 planner_data, scenario_result, xres=voxel_meta["xres"], actions=actions
             )
 
     file_name = planner_data.get("name", str(uuid.uuid4())) + ".json"
```

### Comparing `pymultiastar-0.0.7/examples/run_simple_demo.py` & `pymultiastar-0.0.8/examples/run_simple_demo.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/examples/run_simple_world_3d.py` & `pymultiastar-0.0.8/examples/run_simple_world_3d.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/mkdocs.yml` & `pymultiastar-0.0.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/pyproject.toml` & `pymultiastar-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymultiastar"
-version = "0.0.7"
+version = "0.0.8"
 description="Multi-goal A* with cpp bindings to python"
 readme = "README.md"
 authors = [
   { name = "Jeremy Castagno", email = "jeremybyu@gmail.com" },
 ]
 requires-python = ">=3.9"
 classifiers = [
@@ -19,15 +19,15 @@
 ]
 
 [build-system]
 requires = ["scikit-build-core>=0.3.3", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [project.optional-dependencies]
-geo = ["pyproj>=3.0"]
+geo = ["pyproj>=3.0", "scipy"]
 test = ["pytest", "Pillow", "pyproj>=3.0"]
 docs = ["mkdocstrings[python]", "mkdocs-autorefs>=0.3.1",
       "pymdown-extensions>=6.3", "mkdocs>=1.3", "griffe>=0.27.5", "python-markdown-math",
       "mkdocs-coverage>=0.2", "mkdocs-gen-files>=0.3",
       "mkdocs-literate-nav>=0.4","mkdocs-material>=7.3",
       "mkdocs-section-index>=0.3", "mkdocstrings-python>=0.5.1",
       "markdown-callouts>=0.2","markdown-exec>=0.5"]
@@ -47,8 +47,11 @@
 build-verbosity = 1
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.ruff]
 line-length = 100
-target-version = "py310"
+target-version = "py310"
+
+[project.scripts]
+aclm = "pymultiastar.scripts.aclm:main"
```

### Comparing `pymultiastar-0.0.7/src/include/pymultiastar.hpp` & `pymultiastar-0.0.8/src/include/pymultiastar.hpp`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/src/main.cpp` & `pymultiastar-0.0.8/src/main.cpp`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/src/pymultiastar/__init__.py` & `pymultiastar-0.0.8/src/pymultiastar/__init__.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/src/pymultiastar/_core.pyi` & `pymultiastar-0.0.8/src/pymultiastar/_core.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 __version__: str
 
 class PyMultiAStar(object):
     """
     A planner that will search for **multiple** goals with **heterogenous** values
     using a 3D A-star **discrete** planner.
     """
+    normalizing_path_cost: float
+    "normalizing path cost property. This property can be updated after object construction"
 
     def __init__(
         self,
         map: ArrayFloatMxNxK,
         allow_diag: bool = False,
         map_res: float = 2.0,
         obstacle_value: float = 1.0,
```

### Comparing `pymultiastar-0.0.7/src/pymultiastar/geoplanner/geoplanner.py` & `pymultiastar-0.0.8/src/pymultiastar/geoplanner/geoplanner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import time
 import pymultiastar as pmstar
 from typing import List, Tuple, Optional
 from pathlib import Path
-import json
 
 import numpy as np
 from pyproj import Transformer
 
 from ..types import ArrayFloatMxNxK, CellPath
 from .types import (PlannerKwargs, VoxelMeta, GPS, LandingSite, GeoMultiPlannerResult, Coord)
 from .helper import (
@@ -200,16 +199,7 @@
         if result is None:
             return None
         path_cost = result["goal_path_cost"]
         path = result["path_cells"]
         return (path, path_cost)
 
 
-def create_planner_from_configuration(plan: Path):
-    with open(plan, "r") as fh:
-        planner_data = json.load(fh)
-    planner_data["cost_map_fp"] = plan.parent / planner_data["cost_map_fp"]
-    voxel_meta: VoxelMeta = planner_data["voxel_meta"]
-
-    planner_kwargs = PlannerKwargs(**planner_data["planner_kwargs"])
-    geo_planner = GeoPlanner(planner_data["cost_map_fp"], voxel_meta, planner_kwargs)
-    return geo_planner, planner_data
```

### Comparing `pymultiastar-0.0.7/src/pymultiastar/geoplanner/helper.py` & `pymultiastar-0.0.8/src/pymultiastar/geoplanner/helper.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/src/pymultiastar/geoplanner/types.py` & `pymultiastar-0.0.8/src/pymultiastar/geoplanner/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,21 +25,50 @@
     normalizing_path_cost: float = 1.0
     goal_weight: float = 0.5
     path_weight: float = 0.5
     keep_nodes: bool = False
     path_w0: float = 1.0
 
 
+
+class PlannerKwargsDict(TypedDict):
+    allow_diag: bool
+    map_res: float
+    obstacle_value: float
+    normalizing_path_cost: float
+    goal_weight: float
+    path_weight: float
+    keep_nodes: bool
+    path_w0: float
+
+
+class LSSKwargs(TypedDict):
+    csv_fp: str
+    "CSV file path that holds all landing sites"
+    srid: str
+    "SRID to transform data to"
+    shift_alt: float
+    "How much to shift the altitude"
+
+class LSSQueryKwargs(TypedDict):
+    "Keyword arguments for landing site selection"
+    radius: float
+    "The radial search footprint"
+    max_altitude: float
+    "Maximum altitude allowed"
+    max_ls_risk: float
+    "Maximum landing site risk allowed"
+
 class Scenario(TypedDict):
     name: str
-    details: Optional[str]
     position: Coord  # assumed to be in GPS!
-    active: Optional[bool]
-    landing_sites: Optional[List[Dict]]
+    lss_query_kwargs: LSSQueryKwargs
     planner_kwargs: Optional[Dict]
+    details: Optional[str]
+    active: Optional[bool]
 
 
 class VoxelMeta(TypedDict):
     srid: str
     nrows: int
     ncols: int
     nslices: int
@@ -52,15 +81,16 @@
 
 
 class Plan(TypedDict):
     name: str
     cost_map_fp: str
     voxel_meta: VoxelMeta
     map_bbox: Optional[Dict]
-    planner_kwargs: PlannerKwargs
+    planner_kwargs: PlannerKwargsDict
+    lss_kwargs: LSSKwargs
     scenarios: List[Scenario]
 
 
 @dataclass
 class GPS:
     lat: float
     lon: float
@@ -85,14 +115,18 @@
 
 @dataclass
 class LandingSite(SuperDataClass):
     centroid: GPS
     "The centroid of the landing site in GPS coordinates"
     landing_site_risk: float
     "The normalized risk of this landing site [0-1]"
+    radius: Optional[float] = None
+    "The radius of this landing site"
+    uid: Optional[int] = None
+    "A unique identifier for this landing site"
 
     def __str__(self):
         result = f"GPS: {self.centroid.lat:.4f}, {self.centroid.lon:.4f}, \
 {self.centroid.alt:.1f}; Risk: {self.landing_site_risk:.1f}"
         return result
```

### Comparing `pymultiastar-0.0.7/src/pymultiastar/types.py` & `pymultiastar-0.0.8/src/pymultiastar/types.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/src/pymultiastar/visualization/img2d_helpers.py` & `pymultiastar-0.0.8/src/pymultiastar/visualization/img2d_helpers.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/src/pymultiastar/visualization/vis3d_helpers.py` & `pymultiastar-0.0.8/src/pymultiastar/visualization/vis3d_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from typing import Tuple
 import open3d as o3d
 import matplotlib as mpl
 import numpy as np
-from ..geoplanner.types import GPS, LandingSite, Coord, GeoMultiPlannerResult, CoordPath, CoordRisk
+from ..geoplanner.types import (
+    GPS,
+    LandingSite,
+    Coord,
+    GeoMultiPlannerResult,
+    CoordPath,
+    CoordRisk,
+)
 from ..geoplanner import GeoPlanner
 from ..geoplanner.helper import convert_cost_map_to_float
 from ..types import Cell
 from .. import calculate_pareto_points
 from typing import List
 from .log import logger
 
 default_buildings = [
-    [(7, 12), (7, 12), (0, 12 ), 255],
+    [(7, 12), (7, 12), (0, 12), 255],
 ]
 
+
 def create_map(
     shape=(20, 30, 15), buildings=default_buildings, dtype=np.float32, normalize=True
 ):
     data = np.zeros(shape, dtype=dtype)
     for x, y, z, value in buildings:
         data[x[0] : x[1], y[0] : y[1], z[0] : z[1]] = value
     if normalize:
@@ -62,23 +70,25 @@
     pcd_obstacle = convert_to_point_cloud(
         map, mask=obstacle_mask, color_by_height=True, **kwargs
     )
     # only way to make work better....
     pcd_obstacle = pcd_obstacle.voxel_down_sample(voxel_size=ds_voxel_size)
     obstacle = dict(name="Obstacles", geometry=pcd_obstacle)
 
-    xres = kwargs.get('xres', 1.0)
+    xres = kwargs.get("xres", 1.0)
     i, j, k = map.shape
-    map_bounds = np.array([
-        [0, 0, 0],
-        [0, i * xres, 0],
-        [j*xres, i*xres, 0],
-        [j*xres, 0, 0],
-        [0, 0, 0],
-    ])
+    map_bounds = np.array(
+        [
+            [0, 0, 0],
+            [0, i * xres, 0],
+            [j * xres, i * xres, 0],
+            [j * xres, 0, 0],
+            [0, 0, 0],
+        ]
+    )
     line_set = dict(name="Map Bounds", geometry=create_line(map_bounds))
     # when the point cloud is bigger than 7_000_000 points it will reappear if deselected
     # this was just a test to prove it
     # print(pcd_obstacle)
     # pcd = o3d.geometry.PointCloud()
     # colors = mpl.colormaps.get_cmap('viridis')(np.random.rand(10_000_000))[:, :3]
     # pcd.points = o3d.utility.Vector3dVector(np.random.randn(10_000_000, 3) * 10)
@@ -88,41 +98,44 @@
 
     # pf = dict(name="Potential Field", geometry=pcd_pf)
     # geoms = [obstacle, pf] if np.any(pf_mask) else [obstacle]
     geoms = [line_set, obstacle]
 
     return geoms
 
+
 def swap_xy_list(coord):
-    result:List[Coord] = []
+    result: List[Coord] = []
     for i in coord:
-        result.append((i[1], i[0], i[2])) 
+        result.append((i[1], i[0], i[2]))
     return result
 
 
 def swap_xy(coord: Coord | CoordPath):
     return (coord[1], coord[0], coord[2])
 
 
 def create_planning_objects(
     start: Coord,
     goals: List[CoordRisk],
     path: CoordPath,
-    radius:float=0.5,
-    flip_xy=True
+    radius: float = 0.5,
+    flip_xy=True,
 ):
     start = swap_xy(start) if flip_xy else start
     goals = [(swap_xy(goal[0]), goal[1]) if flip_xy else goal for goal in goals]
     path = swap_xy_list(path) if flip_xy else path
     start_object = dict(
         name="Start Position",
         geometry=create_object(start, color=[0.0, 0.0, 1.0], radius=radius),
     )
 
-    goal_objects = list(map(lambda x: create_object(x[0], radius=radius, color=x[1]), goals))
+    goal_objects = list(
+        map(lambda x: create_object(x[0], radius=radius, color=x[1]), goals)
+    )
     # logger.debug(f"Projected LS Coords {ls_coords}")
     goal_group = o3d.geometry.TriangleMesh()
     for ob in goal_objects:
         goal_group += ob
     goal_group = dict(name="Landing Sites", geometry=goal_group)
 
     path_line_set = create_line(path)
@@ -155,23 +168,28 @@
     ls_objects = list(map(lambda x: create_object(x), ls_coords))
     # logger.debug(f"Projected LS Coords {ls_coords}")
     ls_group = o3d.geometry.TriangleMesh()
     for ob in ls_objects:
         ls_group += ob
     ls_group = dict(name="Landing Sites", geometry=ls_group)
 
-    path_line_set = create_line(plan_results["path_projected_zero_origin"])
-    path_line_set = dict(name="Optimal Path", geometry=path_line_set)
+    if plan_results["path_projected_zero_origin"]:
+        path_line_set = create_line(plan_results["path_projected_zero_origin"])
+        path_line_set = dict(name="Optimal Path", geometry=path_line_set)
+    else:
+        path_line_set = dict(name="Optimal Path", geometry=o3d.geometry.TriangleMesh())
 
     all_labels = [(goal[0], str(goal[1])) for goal in zip(ls_coords, ls_list)]
 
     return [start_object, ls_group, path_line_set], all_labels
 
 
-def create_object(object: Coord, object_type="ico", color=[1.0, 0.0, 0.0], radius=3.0, cmap='viridis'):
+def create_object(
+    object: Coord, object_type="ico", color=[1.0, 0.0, 0.0], radius=3.0, cmap="viridis"
+):
     object_3d = None
     if object_type == "ico":
         object_3d = o3d.geometry.TriangleMesh.create_icosahedron(radius=radius)
 
     if not isinstance(color, list):
         color = mpl.colormaps.get_cmap(cmap)(color)[:3]
 
@@ -189,92 +207,134 @@
     line_set = o3d.geometry.LineSet(
         points=o3d.utility.Vector3dVector(points),
         lines=o3d.utility.Vector2iVector(lines),
     )
     line_set.paint_uniform_color(color)
     return line_set
 
-def visualize_world(all_geoms, all_labels:List[Tuple[Coord, str]]=[], look_at=None, 
-                    eye=None, point_size=7, actions=[]):
+
+def visualize_world(
+    all_geoms,
+    all_labels: List[Tuple[Coord, str]] = [],
+    look_at=None,
+    eye=None,
+    point_size=7,
+    actions=[],
+):
+    # using dictionary for easier mutable access
+    # used in toggle_labels function
+    label_dict = dict(labels_on=True)
 
     def init(vis):
         vis.show_ground = True
         vis.ground_plane = o3d.visualization.rendering.Scene.GroundPlane.XY  # type: ignore
         vis.point_size = point_size
         vis.show_axes = True
-
         for label in all_labels:
             vis.add_3d_label(label[0], label[1])
 
+    def toggle_labels(vis, label_dict):
+        if vis is not None:
+            if label_dict["labels_on"]:
+                vis.clear_3d_labels()
+            else:
+                for label in all_labels:
+                    vis.add_3d_label(label[0], label[1])
+
+        label_dict["labels_on"] = not label_dict["labels_on"]
+
     if eye is None or look_at is None:
-        boundary = all_geoms[0]['geometry'].get_axis_aligned_bounding_box()
+        boundary = all_geoms[0]["geometry"].get_axis_aligned_bounding_box()
         look_at = boundary.get_center()
         extent = boundary.get_extent()
-        eye = [extent[0]/2, -extent[1]/1.5, extent[1]]
+        eye = [extent[0] / 2, -extent[1] / 1.5, extent[1]]
 
+    actions.append(("Toggle Labels", lambda vis: toggle_labels(vis, label_dict)))
     logger.info("Please exit by closing the 3D Visualization Window!")
     o3d.visualization.draw(  # type: ignore
         all_geoms,
         lookat=look_at,
         eye=eye,
         up=[0, 0, 1],
         title="World Viewer",
         on_init=init,
         show_ui=True,
-        actions=actions
+        actions=actions,
     )
 
+
 def visualize_plan(planner_data, plan_result, xres=2.0, actions=[]):
     logger.info("Loading Map for Visualization ...")
 
     landing_objects, all_labels = create_landing_objects(**plan_result)  # type: ignore
     map_3d = np.load(planner_data["cost_map_fp"])
     map_3d = convert_cost_map_to_float(
         map_3d, reverse_yaxis=True, set_max_value_to_inf=False
     )
     world_geoms = create_pcd_map(map_3d, obstacle_value=1.0, xres=xres)
     logger.info("Finished Loaded Map!")
 
-    all_geoms = [*world_geoms, *landing_objects,]
+    all_geoms = [
+        *world_geoms,
+        *landing_objects,
+    ]
     visualize_world(all_geoms, all_labels=all_labels, actions=actions)
 
+
 def is_pareto_efficient(costs):
     """
     :param costs: An (n_points, n_costs) array
     :return: A (n_points, ) boolean array, indicating whether each point is Pareto efficient
     """
     is_efficient = np.ones(costs.shape[0], dtype=bool)
     for i, c in enumerate(costs):
         if is_efficient[i]:
             is_efficient[is_efficient] = np.any(
-                costs[is_efficient] <= c, axis=1)  # Remove dominated points
+                costs[is_efficient] <= c, axis=1
+            )  # Remove dominated points
     return is_efficient
 
 
 def plot_pareto(planner, start_cell, goal_cells, planning_parameters, **kwargs):
     import pandas as pd
     import matplotlib.pyplot as plt
-    pareto_points = calculate_pareto_points(planner, start_cell, goal_cells, **planning_parameters)
+
+    pareto_points = calculate_pareto_points(
+        planner, start_cell, goal_cells, **planning_parameters
+    )
     df = pd.DataFrame.from_records(pareto_points)
     plot_pareto_(df, **kwargs)
     plt.show()
 
-def plot_pareto_(df, x='goal_risk', y='path_risk', goal_name="Goal", total_risk='total_risk', fname=None):
+
+def plot_pareto_(
+    df,
+    x="goal_risk",
+    y="path_risk",
+    goal_name="Goal",
+    total_risk="total_risk",
+    fname=None,
+):
     import seaborn as sns
     import matplotlib.pyplot as plt
     import pandas as pd
-#     df_p = df_p[df_p['path_risk'] < 1.0]
-    costs = df[[x,y]].values
-    pareto_df = pd.DataFrame(costs[is_pareto_efficient(costs)], columns=[x, y]).sort_values(by=[x])
+
+    #     df_p = df_p[df_p['path_risk'] < 1.0]
+    costs = df[[x, y]].values
+    pareto_df = pd.DataFrame(
+        costs[is_pareto_efficient(costs)], columns=[x, y]
+    ).sort_values(by=[x])
     # ax.scatter(df_[0:4]['total_cost'], df_[0:4]['path_cost'], color='r', label='Chosen Landing Sites')
     ax = sns.scatterplot(data=df, x=x, y=y, color="m", label="All Goals", zorder=5)
-    ax.plot(pareto_df[x], pareto_df[y], color='g', label='Pareto Frontier', zorder=1)
+    ax.plot(pareto_df[x], pareto_df[y], color="g", label="Pareto Frontier", zorder=1)
     top_item = df.iloc[df[total_risk].idxmin()]
-    ax.scatter(top_item[x], top_item[y], color='r', label=f'Best {goal_name}', zorder=10)
+    ax.scatter(
+        top_item[x], top_item[y], color="r", label=f"Best {goal_name}", zorder=10
+    )
     sns.set(font_scale=1.3)  # crazy big
     ax.set_xlabel(f"{goal_name} Risk ($r_{goal_name[0].lower()}$)")
     ax.set_ylabel("Path Risk ($r_p$)")
-    ax.axis('equal')
-    plt.legend(loc='upper right')
+    ax.axis("equal")
+    plt.legend(loc="upper right")
     if fname:
-        plt.savefig(fname, bbox_inches='tight')
+        plt.savefig(fname, bbox_inches="tight")
     return ax
```

### Comparing `pymultiastar-0.0.7/src/pymultiastar.cpp` & `pymultiastar-0.0.8/src/pymultiastar.cpp`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/tests/fixtures/maze_large.png` & `pymultiastar-0.0.8/tests/fixtures/maze_large.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/tests/fixtures/maze_small.png` & `pymultiastar-0.0.8/tests/fixtures/maze_small.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/tests/fixtures/world/annarbor/plan.json` & `pymultiastar-0.0.8/tests/fixtures/world/annarbor/plan.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6479591836734694%*

 * *Differences: {"'lss_kwargs'": "OrderedDict([('csv_fp', './landing_sites.csv'), ('srid', 'epsg:26918'), "*

 * *                 "('shift_alt', 4.0)])",*

 * * "'planner_kwargs'": "{'normalizing_path_cost': 250.0}",*

 * * "'scenarios'": "{0: {'planner_kwargs': {'normalizing_path_cost': 250.0}, 'lss_query_kwargs': "*

 * *                "OrderedDict([('radius', 250.0), ('max_altitude', 400.0), ('max_ls_risk', 0.6)]), "*

 * *                "delete: ['active', 'landing_sites']}, insert: [(1, OrderedDict([('name', "*

 * *                "'Scenario 2'), (' […]*

```diff
@@ -1,82 +1,93 @@
 {
     "cost_map_fp": "./voxel_map.npy",
-    "map_bbox": {
-        "maxlat": 4684573.753,
-        "maxlon": 274696.77,
-        "minlat": 4682986.22,
-        "minlon": 273110.5474,
-        "projection": "EPSG:26917"
+    "lss_kwargs": {
+        "csv_fp": "./landing_sites.csv",
+        "shift_alt": 4.0,
+        "srid": "epsg:26918"
     },
     "name": "Ann Arbor",
     "planner_kwargs": {
         "allow_diag": true,
         "goal_weight": 0.5,
         "keep_nodes": false,
         "map_res": 2.0,
-        "normalizing_path_cost": 200.0,
+        "normalizing_path_cost": 250.0,
         "obstacle_value": 1.0,
         "path_w0": 1.0,
         "path_weight": 0.5
     },
     "scenarios": [
         {
-            "active": false,
             "details": "South East - Few Building Many Trees",
-            "landing_sites": [
-                {
-                    "landing_site_risk": 0.2970436067094503,
-                    "osm_id": 459948086,
-                    "position": [
-                        42.27052,
-                        -83.73692,
-                        273.65
-                    ],
-                    "radius": 8.71678689290668
-                },
-                {
-                    "landing_site_risk": 0.5251571215205322,
-                    "osm_id": 468944455,
-                    "position": [
-                        42.27106,
-                        -83.73654,
-                        273.71
-                    ],
-                    "radius": 4.01958993211309
-                },
-                {
-                    "landing_site_risk": 0.535970290151188,
-                    "osm_id": 473414093,
-                    "position": [
-                        42.27094,
-                        -83.73819,
-                        272.03
-                    ],
-                    "radius": 3.7825532318500055
-                },
-                {
-                    "landing_site_risk": 0.6990376743808593,
-                    "osm_id": 572952539,
-                    "position": [
-                        42.27161,
-                        -83.73729,
-                        266.74
-                    ],
-                    "radius": 4.5689250966093615
-                }
-            ],
+            "lss_query_kwargs": {
+                "max_altitude": 400.0,
+                "max_ls_risk": 0.6,
+                "radius": 250.0
+            },
             "name": "Scenario 1",
             "planner_kwargs": {
-                "normalizing_path_cost": 175.0
+                "normalizing_path_cost": 250.0
             },
             "position": [
                 42.27174,
                 -83.735778,
                 270.0
             ]
+        },
+        {
+            "details": "North West - Many Buildings",
+            "lss_query_kwargs": {
+                "max_altitude": 400.0,
+                "max_ls_risk": 0.6,
+                "radius": 250.0
+            },
+            "name": "Scenario 2",
+            "planner_kwargs": {
+                "normalizing_path_cost": 250.0
+            },
+            "position": [
+                42.27836,
+                -83.74738,
+                260.0
+            ]
+        },
+        {
+            "details": "South West - Parks and Buildings",
+            "lss_query_kwargs": {
+                "max_altitude": 400.0,
+                "max_ls_risk": 0.6,
+                "radius": 250.0
+            },
+            "name": "Scenario 3",
+            "planner_kwargs": {
+                "normalizing_path_cost": 250.0
+            },
+            "position": [
+                42.272593,
+                -83.747044,
+                255.0
+            ]
+        },
+        {
+            "details": "UK",
+            "lss_query_kwargs": {
+                "max_altitude": 400.0,
+                "max_ls_risk": 0.6,
+                "radius": 250.0
+            },
+            "name": "Scenario 4",
+            "planner_kwargs": {
+                "normalizing_path_cost": 250.0
+            },
+            "position": [
+                42.274866,
+                -83.735783,
+                270.0
+            ]
         }
     ],
     "voxel_meta": {
         "ncols": 792,
         "nrows": 792,
         "nslices": 61,
         "srid": "epsg:26917",
```

### Comparing `pymultiastar-0.0.7/tests/fixtures/world/annarbor/voxel_map.npy` & `pymultiastar-0.0.8/tests/fixtures/world/annarbor/voxel_map.npy`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/tests/fixtures/world/newyork/voxel_map.npy` & `pymultiastar-0.0.8/tests/fixtures/world/newyork/voxel_map.npy`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/tests/test_basic.py` & `pymultiastar-0.0.8/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/tests/test_geo_helper.py` & `pymultiastar-0.0.8/tests/test_geo_helper.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.7/PKG-INFO` & `pymultiastar-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pymultiastar
-Version: 0.0.7
+Version: 0.0.8
 Summary: Multi-goal A* with cpp bindings to python
 Author-Email: Jeremy Castagno <jeremybyu@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: numpy>=1.15
 Requires-Dist: pyproj>=3.0; extra == "geo"
+Requires-Dist: scipy; extra == "geo"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: Pillow; extra == "test"
 Requires-Dist: pyproj>=3.0; extra == "test"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Requires-Dist: mkdocs-autorefs>=0.3.1; extra == "docs"
 Requires-Dist: pymdown-extensions>=6.3; extra == "docs"
 Requires-Dist: mkdocs>=1.3; extra == "docs"
```

