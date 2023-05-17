# Comparing `tmp/lnmmeshio-5.2.2.tar.gz` & `tmp/lnmmeshio-5.2.3.tar.gz`

## Comparing `lnmmeshio-5.2.2.tar` & `lnmmeshio-5.2.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/.isort.cfg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/pytest.ini
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/requirements-dev.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/requirements.txt
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/.github/workflows/build_and_test.yml
--rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/__init__.py
--rw-r--r--   0        0        0    12053 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/discretization.py
--rw-r--r--   0        0        0    13496 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/ensightio.py
--rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/fiber.py
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/ioutils.py
--rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/meshio_to_discretization.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/mimics_stlio.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/node.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/nodeset.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/progress.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/__init__.py
--rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/element.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/element_container.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/hex20.py
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/hex27.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/hex8.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/line2.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/line3.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/parse_element.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/pyramid5.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/quad4.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/quad8.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/quad9.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/tet10.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/tet4.py
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/tri3.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/tri6.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/vertex.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/element/wedge6.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/functions/__init__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/functions/component.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/functions/function.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/functions/linear_interpolation_variable.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/functions/variable.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/src/lnmmeshio/functions/variablereader.py
--rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_disc.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_discretization.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_ele_container.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_element_factory.py
--rw-r--r--   0        0        0    20936 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_eles.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_ensight.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_fibers.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_integration.py
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_meshio2discretization.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_mimics_stlio.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_override.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/test_write_data.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/data/cube.mesh
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/data/cube.stl
--rw-r--r--   0        0        0    17448 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/data/dummy.dat
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/data/dummy.mesh
--rw-r--r--   0        0        0   928184 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/data/dummy.stl
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/data/dummy2.dat
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/test_lnmmeshio/data/full.dat
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/LICENSE
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/pyproject.toml
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lnmmeshio-5.2.2/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/.isort.cfg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/pytest.ini
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/requirements-dev.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/requirements.txt
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/.github/workflows/build_and_test.yml
+-rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/__init__.py
+-rw-r--r--   0        0        0    12053 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/discretization.py
+-rw-r--r--   0        0        0    13496 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/ensightio.py
+-rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/fiber.py
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/ioutils.py
+-rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/meshio_to_discretization.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/mimics_stlio.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/node.py
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/nodeset.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/progress.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/__init__.py
+-rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/element.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/element_container.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/hex20.py
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/hex27.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/hex8.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/line2.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/line3.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/parse_element.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/pyramid5.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/quad4.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/quad8.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/quad9.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/tet10.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/tet4.py
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/tri3.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/tri6.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/vertex.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/element/wedge6.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/functions/__init__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/functions/component.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/functions/function.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/functions/linear_interpolation_variable.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/functions/variable.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/src/lnmmeshio/functions/variablereader.py
+-rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_disc.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_discretization.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_ele_container.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_element_factory.py
+-rw-r--r--   0        0        0    20936 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_eles.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_ensight.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_fibers.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_integration.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_meshio2discretization.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_mimics_stlio.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_override.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/test_write_data.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/data/cube.mesh
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/data/cube.stl
+-rw-r--r--   0        0        0    17448 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/data/dummy.dat
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/data/dummy.mesh
+-rw-r--r--   0        0        0   928184 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/data/dummy.stl
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/data/dummy2.dat
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/test_lnmmeshio/data/full.dat
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/LICENSE
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lnmmeshio-5.2.3/PKG-INFO
```

### Comparing `lnmmeshio-5.2.2/.github/workflows/build_and_test.yml` & `lnmmeshio-5.2.3/.github/workflows/build_and_test.yml`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/__init__.py` & `lnmmeshio-5.2.3/src/lnmmeshio/__init__.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/discretization.py` & `lnmmeshio-5.2.3/src/lnmmeshio/discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/ensightio.py` & `lnmmeshio-5.2.3/src/lnmmeshio/ensightio.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/fiber.py` & `lnmmeshio-5.2.3/src/lnmmeshio/fiber.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/ioutils.py` & `lnmmeshio-5.2.3/src/lnmmeshio/ioutils.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/meshio_to_discretization.py` & `lnmmeshio-5.2.3/src/lnmmeshio/meshio_to_discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/mimics_stlio.py` & `lnmmeshio-5.2.3/src/lnmmeshio/mimics_stlio.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This file is mainly based on the stl-reader by meshio (https://github.com/nschloe/meshio).
 
 Copyright (c) 2015-2021 Nico Schlömer et al.
 
 I/O for the STL format, cf.
 <https://en.wikipedia.org/wiki/STL_(file_format)>.
 """
+import io
 import logging
 import struct
 
 import numpy
 from meshio import Mesh
 
 
@@ -110,19 +111,22 @@
 
     if attrs is None:
         attrs = numpy.zeros((len(pts)), dtype=numpy.uint16)
 
     normals = _compute_normals(pts)
 
     with open(filename, "wb") as fh:
-        # 80 character header data
-        msg = "This file was generated by meshio."
-        msg += (79 - len(msg)) * "X"
-        msg += "\n"
-        fh.write(msg.encode("utf-8"))
+        # 80 character header data containing default color for 3-matic
+        byte_io = io.BytesIO()
+        byte_io.write(
+            b"COLOR=\xc0\xc0\xc0\x00,MATERIAL=\x80\x80\x80\xff\x80\x80\x80\xff\x00\x00\x00\xff\x00\x00\xa0A;SOLID\x00"
+        )
+        byte_io.write(b" " * (80 - byte_io.getbuffer().nbytes))
+
+        fh.write(byte_io.getbuffer().tobytes())
         fh.write(numpy.uint32(len(cells[0].data)))
         for pt, normal, attr in zip(pts, normals, attrs):
             fh.write(normal.astype(numpy.float32))
             fh.write(pt.astype(numpy.float32))
             fh.write(attr)
 
     return
```

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/node.py` & `lnmmeshio-5.2.3/src/lnmmeshio/node.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/nodeset.py` & `lnmmeshio-5.2.3/src/lnmmeshio/nodeset.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/progress.py` & `lnmmeshio-5.2.3/src/lnmmeshio/progress.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/element.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/element.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/element_container.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/element_container.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/hex20.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/hex20.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/hex27.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/hex27.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/hex8.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/hex8.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/line2.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/line2.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/line3.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/line3.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/parse_element.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/parse_element.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/pyramid5.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/pyramid5.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/quad4.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/quad4.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/quad8.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/quad8.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/quad9.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/quad9.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/tet10.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/tet10.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/tet4.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/tet4.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/tri3.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/tri3.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/tri6.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/tri6.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/vertex.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/vertex.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/element/wedge6.py` & `lnmmeshio-5.2.3/src/lnmmeshio/element/wedge6.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/functions/component.py` & `lnmmeshio-5.2.3/src/lnmmeshio/functions/component.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/functions/function.py` & `lnmmeshio-5.2.3/src/lnmmeshio/functions/function.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/functions/linear_interpolation_variable.py` & `lnmmeshio-5.2.3/src/lnmmeshio/functions/linear_interpolation_variable.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/src/lnmmeshio/functions/variablereader.py` & `lnmmeshio-5.2.3/src/lnmmeshio/functions/variablereader.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_disc.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_disc.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_discretization.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_ele_container.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_ele_container.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_element_factory.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_element_factory.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_eles.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_eles.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_ensight.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_ensight.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_fibers.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_fibers.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_integration.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_integration.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_meshio2discretization.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_meshio2discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_mimics_stlio.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_mimics_stlio.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_override.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_override.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/test_write_data.py` & `lnmmeshio-5.2.3/test_lnmmeshio/test_write_data.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/data/cube.stl` & `lnmmeshio-5.2.3/test_lnmmeshio/data/cube.stl`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-00000000: 5468 6973 2066 696c 6520 7761 7320 6765  This file was ge
-00000010: 6e65 7261 7465 6420 6279 206d 6573 6869  nerated by meshi
-00000020: 6f2e 5858 5858 5858 5858 5858 5858 5858  o.XXXXXXXXXXXXXX
-00000030: 5858 5858 5858 5858 5858 5858 5858 5858  XXXXXXXXXXXXXXXX
-00000040: 5858 5858 5858 5858 5858 5858 5858 580a  XXXXXXXXXXXXXXX.
+00000000: 434f 4c4f 523d c0c0 c000 2c4d 4154 4552  COLOR=....,MATER
+00000010: 4941 4c3d 8080 80ff 8080 80ff 0000 00ff  IAL=............
+00000020: 0000 a041 3b53 4f4c 4944 0020 2020 2020  ...A;SOLID.     
+00000030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000040: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000050: 0c00 0000 0000 0000 0000 80bf 0000 0000  ................
 00000060: 0000 0000 0000 0000 0000 0000 0000 2041  .............. A
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 2041 0100 0000 0000 0000 80bf 0000  .. A............
 00000090: 0000 0000 2041 0000 0000 0000 0000 0000  .... A..........
 000000a0: 2041 0000 0000 0000 2041 0000 0000 0000   A...... A......
 000000b0: 0000 0000 2041 0100 0000 803f 0000 0000  .... A.....?....
```

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/data/dummy.dat` & `lnmmeshio-5.2.3/test_lnmmeshio/data/dummy.dat`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/data/dummy.stl` & `lnmmeshio-5.2.3/test_lnmmeshio/data/dummy.stl`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/data/dummy2.dat` & `lnmmeshio-5.2.3/test_lnmmeshio/data/dummy2.dat`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/test_lnmmeshio/data/full.dat` & `lnmmeshio-5.2.3/test_lnmmeshio/data/full.dat`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/LICENSE` & `lnmmeshio-5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/README.md` & `lnmmeshio-5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.2.2/pyproject.toml` & `lnmmeshio-5.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lnmmeshio"
-version = "5.2.2"
+version = "5.2.3"
 authors = [
   { name="Amadeus Gebauer", email="amadeus.gebauer@tum.de" },
 ]
 description = "Import and export from and to various mesh formats including dat files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lnmmeshio-5.2.2/PKG-INFO` & `lnmmeshio-5.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnmmeshio
-Version: 5.2.2
+Version: 5.2.3
 Summary: Import and export from and to various mesh formats including dat files
 Project-URL: Homepage, https://github.com/amgebauer/lnmmeshio
 Project-URL: Bug Tracker, https://github.com/amgebauer/lnmmeshio/issues
 Author-email: Amadeus Gebauer <amadeus.gebauer@tum.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

