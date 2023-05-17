# Comparing `tmp/qmlearn-0.0.1rc0.tar.gz` & `tmp/qmlearn-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qmlearn-0.0.1rc0.tar", last modified: Mon Feb 20 19:26:39 2023, max compression
+gzip compressed data, was "qmlearn-0.0.1rc1.tar", last modified: Wed May 17 18:38:41 2023, max compression
```

## Comparing `qmlearn-0.0.1rc0.tar` & `qmlearn-0.0.1rc1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      190 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/.gitignore
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.964802 qmlearn-0.0.1rc0/Docs/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/.gitkeep
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      869 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/Makefile
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2006 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/conf.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      433 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/index.rst
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.968802 qmlearn-0.0.1rc0/Docs/source/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     6655 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/1_create_training.ipynb
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     9886 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/2_test_qml.ipynb
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    97970 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/3_predict_model.ipynb
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      942 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/contact.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      921 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/install.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      419 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/qmlearn.api.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      803 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/qmlearn.drivers.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      594 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/qmlearn.io.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      487 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/qmlearn.model.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      189 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/qmlearn.preprocessing.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      182 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/qmlearn.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      338 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/qmlearn.utils.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1236 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/source/tutorials.rst
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.972802 qmlearn-0.0.1rc0/Docs/static/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      436 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/static/custom.css
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   366742 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/static/figure3.png
--rw-rw-r--   0 sxc       (1000) sxc       (1000)  7514329 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/static/figures.key
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    52223 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/static/qmlearn.ico
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   110709 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/static/qmlearn.png
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.972802 qmlearn-0.0.1rc0/Docs/templates/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      603 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/templates/breadcrumbs.html
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      593 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/Docs/templates/footer.html
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1081 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/LICENSE
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      121 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/MANIFEST.in
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1465 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/PKG-INFO
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      704 2023-02-20 19:23:52.000000 qmlearn-0.0.1rc0/README.md
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.964802 qmlearn-0.0.1rc0/examples/
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.964802 qmlearn-0.0.1rc0/examples/examples/
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.976802 qmlearn-0.0.1rc0/examples/examples/h2o/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     5063 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/examples/h2o/0_create_images.ipynb
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     6814 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/examples/h2o/1_create_training.ipynb
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    10165 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/examples/h2o/2_test_qml.ipynb
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   101225 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/examples/h2o/3_predict_model.ipynb
--rw-rw-r--   0 sxc       (1000) sxc       (1000)  1709488 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/examples/h2o/h2o_md_300_QML_set.hdf5
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    32636 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/examples/h2o/h2o_vib.traj
--rw-rw-r--   0 sxc       (1000) sxc       (1000)  2034488 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/examples/h2o/h2o_vib_QML_set.hdf5
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.976802 qmlearn-0.0.1rc0/examples/hack_2022/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    73780 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/hack_2022/Creating_a_Data_Set_CI.ipynb
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   173921 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/hack_2022/Fitting_vext_2rdm_H2.ipynb
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.976802 qmlearn-0.0.1rc0/examples/test/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2293 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/test/test_reorder.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2176 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/examples/test/test_rotate.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.976802 qmlearn-0.0.1rc0/qmlearn/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      395 2023-02-20 19:26:24.000000 qmlearn-0.0.1rc0/qmlearn/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       36 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/__main__.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.976802 qmlearn-0.0.1rc0/qmlearn/api/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/api/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     6500 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/api/api4ase.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     6426 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/api/constraints.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/qmlearn/cui/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      875 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/cui/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3679 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/cui/traj2db.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/qmlearn/data/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1281 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/data/__init__.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/qmlearn/drivers/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/drivers/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    16275 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/drivers/core.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    10453 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/drivers/mol.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     9477 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/drivers/psi4.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    18485 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/drivers/pyscf.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2216 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/drivers/rotate.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/qmlearn/io/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3241 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/io/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1305 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/io/core.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    10030 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/io/hdf5.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2930 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/io/model.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/qmlearn/model/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       27 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/model/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      171 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/model/build.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    11996 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/model/model.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/qmlearn/preprocessing/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     8389 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/preprocessing/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1711 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/preprocessing/vibrations.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/qmlearn/utils/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       21 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/utils/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      487 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/utils/math.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1325 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/utils/utils.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/qmlearn/vibrations/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2314 2023-02-20 19:01:28.000000 qmlearn-0.0.1rc0/qmlearn/vibrations/__init__.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-02-20 19:26:39.976802 qmlearn-0.0.1rc0/qmlearn.egg-info/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1465 2023-02-20 19:26:39.000000 qmlearn-0.0.1rc0/qmlearn.egg-info/PKG-INFO
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1947 2023-02-20 19:26:39.000000 qmlearn-0.0.1rc0/qmlearn.egg-info/SOURCES.txt
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        1 2023-02-20 19:26:39.000000 qmlearn-0.0.1rc0/qmlearn.egg-info/dependency_links.txt
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      171 2023-02-20 19:26:39.000000 qmlearn-0.0.1rc0/qmlearn.egg-info/requires.txt
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        8 2023-02-20 19:26:39.000000 qmlearn-0.0.1rc0/qmlearn.egg-info/top_level.txt
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      147 2023-02-20 19:08:55.000000 qmlearn-0.0.1rc0/requirements.txt
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       38 2023-02-20 19:26:39.980802 qmlearn-0.0.1rc0/setup.cfg
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1914 2023-02-20 19:15:49.000000 qmlearn-0.0.1rc0/setup.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.622471 qmlearn-0.0.1rc1/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      190 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/.gitignore
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.562473 qmlearn-0.0.1rc1/Docs/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2022-04-15 19:40:21.000000 qmlearn-0.0.1rc1/Docs/.gitkeep
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      869 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/Makefile
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2006 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/conf.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      433 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/index.rst
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.566473 qmlearn-0.0.1rc1/Docs/source/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6655 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/1_create_training.ipynb
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     9886 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/2_test_qml.ipynb
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    97970 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/3_predict_model.ipynb
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      942 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/contact.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      921 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/install.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      419 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/qmlearn.api.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      803 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/qmlearn.drivers.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      594 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/qmlearn.io.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      487 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/qmlearn.model.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      189 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/qmlearn.preprocessing.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      182 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/qmlearn.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      338 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/qmlearn.utils.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1236 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/source/tutorials.rst
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.590472 qmlearn-0.0.1rc1/Docs/static/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      436 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/static/custom.css
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   366742 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/static/figure3.png
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)  7514329 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/static/figures.key
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    52223 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/static/qmlearn.ico
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   110709 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/static/qmlearn.png
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.590472 qmlearn-0.0.1rc1/Docs/templates/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      603 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/templates/breadcrumbs.html
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      593 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/Docs/templates/footer.html
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1081 2022-02-16 00:42:21.000000 qmlearn-0.0.1rc1/LICENSE
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      121 2022-02-16 00:44:09.000000 qmlearn-0.0.1rc1/MANIFEST.in
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1523 2023-05-17 18:38:41.622471 qmlearn-0.0.1rc1/PKG-INFO
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      762 2023-02-21 20:08:44.000000 qmlearn-0.0.1rc1/README.md
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.554473 qmlearn-0.0.1rc1/examples/
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.554473 qmlearn-0.0.1rc1/examples/examples/
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.598472 qmlearn-0.0.1rc1/examples/examples/h2o/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     5063 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/examples/examples/h2o/0_create_images.ipynb
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6814 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/examples/examples/h2o/1_create_training.ipynb
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    10165 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/examples/examples/h2o/2_test_qml.ipynb
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   101225 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/examples/examples/h2o/3_predict_model.ipynb
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)  1709488 2022-07-14 00:19:28.000000 qmlearn-0.0.1rc1/examples/examples/h2o/h2o_md_300_QML_set.hdf5
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    32636 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/examples/examples/h2o/h2o_vib.traj
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)  2034488 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/examples/examples/h2o/h2o_vib_QML_set.hdf5
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.610472 qmlearn-0.0.1rc1/examples/hack_2022/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    73780 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/examples/hack_2022/Creating_a_Data_Set_CI.ipynb
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   173921 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/examples/hack_2022/Fitting_vext_2rdm_H2.ipynb
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.610472 qmlearn-0.0.1rc1/examples/test/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2293 2022-04-26 02:43:23.000000 qmlearn-0.0.1rc1/examples/test/test_reorder.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2176 2022-04-26 02:21:22.000000 qmlearn-0.0.1rc1/examples/test/test_rotate.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.610472 qmlearn-0.0.1rc1/qmlearn/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      395 2023-05-17 18:22:57.000000 qmlearn-0.0.1rc1/qmlearn/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       36 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/__main__.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.614472 qmlearn-0.0.1rc1/qmlearn/api/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/api/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6500 2023-04-16 21:35:09.000000 qmlearn-0.0.1rc1/qmlearn/api/api4ase.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6426 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/api/constraints.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.614472 qmlearn-0.0.1rc1/qmlearn/cui/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      875 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/cui/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3679 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/cui/traj2db.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.614472 qmlearn-0.0.1rc1/qmlearn/data/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1281 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/data/__init__.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.614472 qmlearn-0.0.1rc1/qmlearn/drivers/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2022-02-16 22:31:36.000000 qmlearn-0.0.1rc1/qmlearn/drivers/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    16980 2023-04-04 21:41:34.000000 qmlearn-0.0.1rc1/qmlearn/drivers/core.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     9917 2023-04-04 21:22:43.000000 qmlearn-0.0.1rc1/qmlearn/drivers/mol.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     9477 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/drivers/psi4.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    18770 2023-05-11 19:03:19.000000 qmlearn-0.0.1rc1/qmlearn/drivers/pyscf.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2216 2022-12-14 15:42:48.000000 qmlearn-0.0.1rc1/qmlearn/drivers/rotate.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.622471 qmlearn-0.0.1rc1/qmlearn/io/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3251 2023-04-19 15:16:29.000000 qmlearn-0.0.1rc1/qmlearn/io/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1305 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/io/core.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    10030 2022-11-14 19:50:38.000000 qmlearn-0.0.1rc1/qmlearn/io/hdf5.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2974 2023-04-04 21:31:43.000000 qmlearn-0.0.1rc1/qmlearn/io/model.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.622471 qmlearn-0.0.1rc1/qmlearn/model/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       27 2022-09-26 18:46:49.000000 qmlearn-0.0.1rc1/qmlearn/model/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      171 2022-09-26 18:46:51.000000 qmlearn-0.0.1rc1/qmlearn/model/build.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    11996 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/model/model.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.622471 qmlearn-0.0.1rc1/qmlearn/preprocessing/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     8420 2023-04-21 19:20:36.000000 qmlearn-0.0.1rc1/qmlearn/preprocessing/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1711 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/preprocessing/vibrations.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.622471 qmlearn-0.0.1rc1/qmlearn/utils/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       21 2022-09-26 18:47:42.000000 qmlearn-0.0.1rc1/qmlearn/utils/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      487 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/utils/math.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1325 2022-10-11 14:03:20.000000 qmlearn-0.0.1rc1/qmlearn/utils/utils.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.622471 qmlearn-0.0.1rc1/qmlearn/vibrations/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2314 2022-12-14 16:39:50.000000 qmlearn-0.0.1rc1/qmlearn/vibrations/__init__.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-17 18:38:41.614472 qmlearn-0.0.1rc1/qmlearn.egg-info/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1523 2023-05-17 18:38:41.000000 qmlearn-0.0.1rc1/qmlearn.egg-info/PKG-INFO
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1947 2023-05-17 18:38:41.000000 qmlearn-0.0.1rc1/qmlearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        1 2023-05-17 18:38:41.000000 qmlearn-0.0.1rc1/qmlearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      171 2023-05-17 18:38:41.000000 qmlearn-0.0.1rc1/qmlearn.egg-info/requires.txt
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        8 2023-05-17 18:38:41.000000 qmlearn-0.0.1rc1/qmlearn.egg-info/top_level.txt
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      147 2023-02-21 20:08:44.000000 qmlearn-0.0.1rc1/requirements.txt
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       38 2023-05-17 18:38:41.622471 qmlearn-0.0.1rc1/setup.cfg
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1914 2023-02-21 20:08:44.000000 qmlearn-0.0.1rc1/setup.py
```

### Comparing `qmlearn-0.0.1rc0/Docs/Makefile` & `qmlearn-0.0.1rc1/Docs/Makefile`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/conf.py` & `qmlearn-0.0.1rc1/Docs/conf.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/source/1_create_training.ipynb` & `qmlearn-0.0.1rc1/Docs/source/1_create_training.ipynb`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/source/2_test_qml.ipynb` & `qmlearn-0.0.1rc1/Docs/source/2_test_qml.ipynb`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/source/3_predict_model.ipynb` & `qmlearn-0.0.1rc1/Docs/source/3_predict_model.ipynb`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/source/contact.rst` & `qmlearn-0.0.1rc1/Docs/source/contact.rst`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/source/install.rst` & `qmlearn-0.0.1rc1/Docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/source/qmlearn.drivers.rst` & `qmlearn-0.0.1rc1/Docs/source/qmlearn.drivers.rst`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/source/qmlearn.io.rst` & `qmlearn-0.0.1rc1/Docs/source/qmlearn.io.rst`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/source/tutorials.rst` & `qmlearn-0.0.1rc1/Docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/static/figure3.png` & `qmlearn-0.0.1rc1/Docs/static/figure3.png`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/static/figures.key` & `qmlearn-0.0.1rc1/Docs/static/figures.key`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/static/qmlearn.ico` & `qmlearn-0.0.1rc1/Docs/static/qmlearn.ico`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/static/qmlearn.png` & `qmlearn-0.0.1rc1/Docs/static/qmlearn.png`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/templates/breadcrumbs.html` & `qmlearn-0.0.1rc1/Docs/templates/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/Docs/templates/footer.html` & `qmlearn-0.0.1rc1/Docs/templates/footer.html`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/LICENSE` & `qmlearn-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/PKG-INFO` & `qmlearn-0.0.1rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qmlearn
-Version: 0.0.1rc0
+Version: 0.0.1rc1
 Summary: QMLearn
 Home-page: http://qmlearn.rutgers.edu
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -20,14 +20,16 @@
 Provides-Extra: all
 License-File: LICENSE
 
 # QMLearn
 
 *Quantum Machine Learning* by learning one-body reduced density matrices in the AO basis.
 
+![QM-Learn code and workflow](./Docs/static/figure3.png)
+
 # Contributors
  - Xuecheng Shao, Lukas Paetow, Md Rajib Khan Musa, Jessica A. Martinez B. and Michele Pavanello @ [PRG](https://sites.rutgers.edu/prg/) at [Rutgers University-Newark](http://sasn.rutgers.edu).
  - Mark E Tuckerman @ [Tuckerman Research Group](https://wp.nyu.edu/tuckerman_group/) at [NYU](https://cas.nyu.edu/)
 
 # Some info
 
  Code entirely in Python leveraging [PySCF](https://pyscf.org/) and [Psi4Numpy](https://github.com/psi4/psi4numpy) for generating GTO integrals and DFT targets. Regressions are carried out with [scikit-learn](https://scikit-learn.org/stable/) or other ML tools.
```

### Comparing `qmlearn-0.0.1rc0/README.md` & `qmlearn-0.0.1rc1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # QMLearn
 
 *Quantum Machine Learning* by learning one-body reduced density matrices in the AO basis.
 
+![QM-Learn code and workflow](./Docs/static/figure3.png)
+
 # Contributors
  - Xuecheng Shao, Lukas Paetow, Md Rajib Khan Musa, Jessica A. Martinez B. and Michele Pavanello @ [PRG](https://sites.rutgers.edu/prg/) at [Rutgers University-Newark](http://sasn.rutgers.edu).
  - Mark E Tuckerman @ [Tuckerman Research Group](https://wp.nyu.edu/tuckerman_group/) at [NYU](https://cas.nyu.edu/)
 
 # Some info
 
  Code entirely in Python leveraging [PySCF](https://pyscf.org/) and [Psi4Numpy](https://github.com/psi4/psi4numpy) for generating GTO integrals and DFT targets. Regressions are carried out with [scikit-learn](https://scikit-learn.org/stable/) or other ML tools.
```

### Comparing `qmlearn-0.0.1rc0/examples/examples/h2o/0_create_images.ipynb` & `qmlearn-0.0.1rc1/examples/examples/h2o/0_create_images.ipynb`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/examples/examples/h2o/1_create_training.ipynb` & `qmlearn-0.0.1rc1/examples/examples/h2o/1_create_training.ipynb`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/examples/examples/h2o/2_test_qml.ipynb` & `qmlearn-0.0.1rc1/examples/examples/h2o/2_test_qml.ipynb`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/examples/examples/h2o/3_predict_model.ipynb` & `qmlearn-0.0.1rc1/examples/examples/h2o/3_predict_model.ipynb`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/examples/examples/h2o/h2o_md_300_QML_set.hdf5` & `qmlearn-0.0.1rc1/examples/examples/h2o/h2o_md_300_QML_set.hdf5`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/examples/examples/h2o/h2o_vib.traj` & `qmlearn-0.0.1rc1/examples/examples/h2o/h2o_vib.traj`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/examples/examples/h2o/h2o_vib_QML_set.hdf5` & `qmlearn-0.0.1rc1/examples/examples/h2o/h2o_vib_QML_set.hdf5`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/examples/hack_2022/Creating_a_Data_Set_CI.ipynb` & `qmlearn-0.0.1rc1/examples/hack_2022/Creating_a_Data_Set_CI.ipynb`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/examples/hack_2022/Fitting_vext_2rdm_H2.ipynb` & `qmlearn-0.0.1rc1/examples/hack_2022/Fitting_vext_2rdm_H2.ipynb`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/examples/test/test_reorder.py` & `qmlearn-0.0.1rc1/examples/test/test_reorder.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/examples/test/test_rotate.py` & `qmlearn-0.0.1rc1/examples/test/test_rotate.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/api/api4ase.py` & `qmlearn-0.0.1rc1/qmlearn/api/api4ase.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/api/constraints.py` & `qmlearn-0.0.1rc1/qmlearn/api/constraints.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/cui/__init__.py` & `qmlearn-0.0.1rc1/qmlearn/cui/__init__.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/cui/traj2db.py` & `qmlearn-0.0.1rc1/qmlearn/cui/traj2db.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/data/__init__.py` & `qmlearn-0.0.1rc1/qmlearn/data/__init__.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/drivers/core.py` & `qmlearn-0.0.1rc1/qmlearn/drivers/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -207,20 +207,38 @@
             g = gamma@ovlp@gamma/2
         if kind==2:
             g = (3*gamma@ovlp@gamma@ovlp@gamma - 2*gamma@ovlp@gamma)/8
         if kind==3:
             g = (4*gamma@ovlp@gamma@ovlp@gamma -gamma@ovlp@gamma@ovlp@gamma@ovlp@gamma)/8
         return matrix_deviation(gamma, g)
 
+    def calc_occupations(self, gamma):
+        ovlp_x = self.ovlp_x
+        occs, orbs = np.linalg.eigh(ovlp_x@gamma@ovlp_x)
+        return occs[::-1], orbs[:,::-1]
+
     def init_ovlp_x(self, ovlp = None):
         ovlp = ovlp or self.ovlp
         svel, svec = np.linalg.eigh(ovlp)
         self._ovlp_x = np.einsum('ik,jk->ij', svec, svec*np.sqrt(svel))
         self._ovlp_x_inv = np.einsum('ik,jk->ij', svec, svec/np.sqrt(svel))
 
+    def purify_gamma(self, gamma, tol = 0.5):
+        ovlp_x_inv = self.ovlp_x_inv
+        occs, orbs = self.calc_occupations(gamma)
+        occs = np.abs(occs)
+        occs_i = np.rint(occs)
+        if np.all(np.abs(occs_i-occs) > tol):
+            if tol < 0.49 :
+                raise ValueError(f'The tol = {tol} is too small, try a bigger one.')
+            else :
+                raise ValueError('The density matrix is too bad.')
+        gamma = ovlp_x_inv@np.einsum('ik,jk->ij', orbs, orbs*occs_i)@ovlp_x_inv
+        return gamma
+
 def atoms_rmsd(target, atoms, transform = True, **kwargs) :
     r""" Function to return RMSD : Root mean square deviation between atoms and target:transform atom object. And the target atom coordinates.
 
     Parameters
     ----------
     target : :obj: ASE atoms object
         Reference atoms.
```

### Comparing `qmlearn-0.0.1rc0/qmlearn/drivers/mol.py` & `qmlearn-0.0.1rc1/qmlearn/drivers/mol.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,14 +69,16 @@
             'calc_etotal',
             'calc_etotal2',
             'calc_ke',
             'calc_dipole',
             'calc_quadrupole',
             'calc_forces',
             'calc_idempotency',
+            'calc_occupations',
+            'purify_gamma',
             'rotation2rotmat',
             'get_atom_naos',
             'vext',
             'ovlp',
             'ovlp_x',
             'ovlp_x_inv',
             'nao',
@@ -280,21 +282,7 @@
         elif 'quadrupole' == prop :
             if rotate :
                 raise AttributeError(f"{prop} not support rotation.")
         else :
             # others just return it self
             pass
         return y
-
-    def purify_gamma(self, gamma = None, tol = 0.5):
-        ovlp_x = self.engine.ovlp_x
-        ovlp_x_inv = self.engine.ovlp_x_inv
-        occs, orbs = np.linalg.eigh(ovlp_x@gamma@ovlp_x)
-        occs = np.abs(occs)
-        occs_i = np.rint(occs)
-        if np.all(np.abs(occs_i-occs) > tol):
-            if tol < 0.49 :
-                raise ValueError(f'The tol = {tol} is too small, try a bigger one.')
-            else :
-                raise ValueError('The density matrix is too bad.')
-        gamma = ovlp_x_inv@np.einsum('ik,jk->ij', orbs, orbs*occs_i)@ovlp_x_inv
-        return gamma
```

### Comparing `qmlearn-0.0.1rc0/qmlearn/drivers/psi4.py` & `qmlearn-0.0.1rc1/qmlearn/drivers/psi4.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/drivers/pyscf.py` & `qmlearn-0.0.1rc1/qmlearn/drivers/pyscf.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from scipy.linalg import eig
 from scipy.spatial.transform import Rotation
 from ase import Atoms, io
 from pyscf.pbc.tools.pyscf_ase import atoms_from_ase
 from pyscf import gto, ao2mo
 from pyscf import dft, scf, mp, fci, ci, cc, mcscf
 from pyscf.symm import Dmatrix
+from pyscf.scf import addons
 from functools import reduce
 
 from qmlearn.drivers.core import Engine
 
 methods_pyscf = {
         'dft' : dft.RKS,
         'hf' : scf.RHF,
@@ -470,14 +471,21 @@
         mol = mol or self.mol
         return rotation2rotmat(rotation, mol)
 
     def get_atom_naos(self, mol = None):
         mol = mol or self.mol
         return get_atom_naos(mol)
 
+    def project_dm_nr2nr(self, gamma, mol2, mol = None):
+        mol = mol or self.mol
+        if hasattr(mol, 'mol'): mol = mol.mol
+        if hasattr(mol2, 'mol'): mol2 = mol2.mol
+        dm = addons.project_dm_nr2nr(mol, gamma, mol2)
+        return dm
+
 def gamma2gamma(*args, **kwargs):
     r""" Function two assure 1-RDM to be the predicted one.
 
     Returns
     -------
     gamma : ndarray
         1-RDM """
```

### Comparing `qmlearn-0.0.1rc0/qmlearn/drivers/rotate.py` & `qmlearn-0.0.1rc1/qmlearn/drivers/rotate.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/io/__init__.py` & `qmlearn-0.0.1rc1/qmlearn/io/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         elif format in ['xyz', 'exyz', 'extxyz'] :
             images = io.read(traj, index = inds)[inds]
         else :
             raise AttributeError(f"Sorry, not support '{format}' format.")
     return images
 
 def read_db(filename, names = '*'):
-    db = DBHDF5(filename)
+    db = DBHDF5(filename, 'r')
     if names is None : names = '*'
     if isinstance(names, str):
         method = names
         names = dict.fromkeys(['qmmol', 'atoms', 'properties'])
         names['qmmol'] = db.get_names(method + '/qmmol*')[0]
         names['atoms'] = db.get_names(method + '/train_atoms*')[0]
         names['properties'] = db.get_names(method + '/train_prop*')[0]
@@ -48,15 +48,15 @@
             raise ValueError(f'The key {key} can not read from the db')
     data['_names'] = names.copy()
     db.close()
     return data
 
 def write_db(output, qmmol, images, properties, prefix = 'train', names = None, **kwargs):
     if names is None or len(names) < 2 : names = [None, ]*3
-    db = DBHDF5(output, qmmol=qmmol, **kwargs)
+    db = DBHDF5(output, 'w', qmmol=qmmol, **kwargs)
     db.write_qmmol(qmmol, name = names[0], **kwargs)
     db.write_images(images, prefix=prefix, name = names[1], **kwargs)
     db.write_properties(properties, prefix=prefix, name = names[1], **kwargs)
     print(db.names, flush = True)
     db.close()
 
 def merge_db(filenames, names = '*', output = None):
```

### Comparing `qmlearn-0.0.1rc0/qmlearn/io/core.py` & `qmlearn-0.0.1rc1/qmlearn/io/core.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/io/hdf5.py` & `qmlearn-0.0.1rc1/qmlearn/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/io/model.py` & `qmlearn-0.0.1rc1/qmlearn/io/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sklearn.linear_model import LinearRegression
 from sklearn.kernel_ridge import KernelRidge
 from qmlearn.model.model import QMModel
 from qmlearn.io import read_db
 from qmlearn.utils import tenumerate
 
-def db2qmmodel(filename, names = '*', mmodels = None, qmmol_options = None, purify_gamma = True):
+def db2qmmodel(filename, names = '*', mmodels = None, qmmol_options = None, purify_gamma = True, predicted_gamma = True):
     r"""Train QMModel to learn :math:`{\gamma}` in terms of :math:`V_{ext}` from training data
     then an additional layer of training learn :math:`{\delta}E` and :math:`{\delta}{\gamma}`
     based on previously learned :math:`{\gamma}`.
 
     Parameters
     ----------
     filename : str
@@ -57,15 +57,15 @@
             break
     else :
         delta_learn = False
     #
     if delta_learn :
         print('Start predicting...', flush = True)
         shape = y[0].shape
-        if 'gamma_pp' in properties:
+        if 'gamma_pp' in properties and predicted_gamma:
             gammas = properties['gamma_pp']
         else :
             gammas = []
             for i, a in tenumerate(train_atoms):
                 gamma = model.predict(a, refatoms=a).reshape(shape)
                 if model.purify_gamma :
                     gamma = model.qmmol.purify_gamma(gamma)
```

### Comparing `qmlearn-0.0.1rc0/qmlearn/model/model.py` & `qmlearn-0.0.1rc1/qmlearn/model/model.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/preprocessing/__init__.py` & `qmlearn-0.0.1rc1/qmlearn/preprocessing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,20 +176,20 @@
     if data is None :
         if properties is None : properties = ['vext', 'gamma', 'energy', 'forces', 'dipole']
         data= {k: [] for k in properties}
     properties = list(data.keys())
     #
     if isinstance(atoms, QMMol):
         qmmol = atoms
-    elif refqmmol is not None :
-        qmmol = refqmmol.duplicate(atoms, refatoms=atoms)
     else :
-        qmmol = QMMol(atoms = atoms, **qmmol_options)
-    #
-    qmmol.run()
+        if refqmmol is not None :
+            qmmol = refqmmol.duplicate(atoms, refatoms=atoms)
+        else :
+            qmmol = QMMol(atoms = atoms, **qmmol_options)
+        qmmol.run(**kwargs)
     #
     for key in properties :
         if key == 'vext' :
             data[key].append(qmmol.engine.vext)
         elif key == 'gamma' :
             data[key].append(qmmol.engine.gamma)
         elif key == 'energy' :
```

### Comparing `qmlearn-0.0.1rc0/qmlearn/preprocessing/vibrations.py` & `qmlearn-0.0.1rc1/qmlearn/preprocessing/vibrations.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/utils/utils.py` & `qmlearn-0.0.1rc1/qmlearn/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn/vibrations/__init__.py` & `qmlearn-0.0.1rc1/qmlearn/vibrations/__init__.py`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/qmlearn.egg-info/PKG-INFO` & `qmlearn-0.0.1rc1/qmlearn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qmlearn
-Version: 0.0.1rc0
+Version: 0.0.1rc1
 Summary: QMLearn
 Home-page: http://qmlearn.rutgers.edu
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -20,14 +20,16 @@
 Provides-Extra: all
 License-File: LICENSE
 
 # QMLearn
 
 *Quantum Machine Learning* by learning one-body reduced density matrices in the AO basis.
 
+![QM-Learn code and workflow](./Docs/static/figure3.png)
+
 # Contributors
  - Xuecheng Shao, Lukas Paetow, Md Rajib Khan Musa, Jessica A. Martinez B. and Michele Pavanello @ [PRG](https://sites.rutgers.edu/prg/) at [Rutgers University-Newark](http://sasn.rutgers.edu).
  - Mark E Tuckerman @ [Tuckerman Research Group](https://wp.nyu.edu/tuckerman_group/) at [NYU](https://cas.nyu.edu/)
 
 # Some info
 
  Code entirely in Python leveraging [PySCF](https://pyscf.org/) and [Psi4Numpy](https://github.com/psi4/psi4numpy) for generating GTO integrals and DFT targets. Regressions are carried out with [scikit-learn](https://scikit-learn.org/stable/) or other ML tools.
```

### Comparing `qmlearn-0.0.1rc0/qmlearn.egg-info/SOURCES.txt` & `qmlearn-0.0.1rc1/qmlearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qmlearn-0.0.1rc0/setup.py` & `qmlearn-0.0.1rc1/setup.py`

 * *Files identical despite different names*

