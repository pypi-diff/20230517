# Comparing `tmp/tad_dftd4-0.0.3.tar.gz` & `tmp/tad_dftd4-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_dftd4-0.0.3.tar", last modified: Mon Mar 13 14:09:05 2023, max compression
+gzip compressed data, was "tad_dftd4-0.0.4.tar", last modified: Wed May 17 06:56:31 2023, max compression
```

## Comparing `tad_dftd4-0.0.3.tar` & `tad_dftd4-0.0.4.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.388463 tad_dftd4-0.0.3/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.372463 tad_dftd4-0.0.3/.github/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.376463 tad_dftd4-0.0.3/.github/workflows/
--rw-rw-r--   0 friede    (1000) friede    (1000)     1941 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/.github/workflows/python.yml
--rw-rw-r--   0 friede    (1000) friede    (1000)     1489 2023-03-13 14:06:56.000000 tad_dftd4-0.0.3/.github/workflows/release.yml
--rw-rw-r--   0 friede    (1000) friede    (1000)     3826 2023-03-13 12:39:50.000000 tad_dftd4-0.0.3/.gitignore
--rw-rw-r--   0 friede    (1000) friede    (1000)     1678 2023-03-13 12:39:51.000000 tad_dftd4-0.0.3/.pre-commit-config.yaml
--rw-rw-r--   0 friede    (1000) friede    (1000)    14449 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/.pylintrc
--rw-rw-r--   0 friede    (1000) friede    (1000)       23 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/.readthedocs.yaml
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.376463 tad_dftd4-0.0.3/.vscode/
--rw-rw-r--   0 friede    (1000) friede    (1000)      687 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/.vscode/settings.json
--rw-rw-r--   0 friede    (1000) friede    (1000)     4919 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/CONTRIBUTING.md
--rw-rw-r--   0 friede    (1000) friede    (1000)    35149 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/COPYING
--rw-rw-r--   0 friede    (1000) friede    (1000)     7652 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/COPYING.LESSER
--rw-rw-r--   0 friede    (1000) friede    (1000)     9818 2023-03-13 14:09:05.388463 tad_dftd4-0.0.3/PKG-INFO
--rw-rw-r--   0 friede    (1000) friede    (1000)     8938 2023-03-13 12:13:06.000000 tad_dftd4-0.0.3/README.rst
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.376463 tad_dftd4-0.0.3/doc/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.376463 tad_dftd4-0.0.3/doc/_static/
--rw-rw-r--   0 friede    (1000) friede    (1000)     3273 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/_static/tad-dftd4-favicon.svg
--rw-rw-r--   0 friede    (1000) friede    (1000)     4282 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/_static/tad-dftd4.svg
--rw-rw-r--   0 friede    (1000) friede    (1000)     1966 2023-03-13 12:40:20.000000 tad_dftd4-0.0.3/doc/conf.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     6408 2023-03-13 12:13:06.000000 tad_dftd4-0.0.3/doc/index.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)     1434 2023-03-13 12:13:06.000000 tad_dftd4-0.0.3/doc/installation.rst
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.376463 tad_dftd4-0.0.3/doc/modules/
--rw-rw-r--   0 friede    (1000) friede    (1000)       47 2023-03-13 12:13:06.000000 tad_dftd4-0.0.3/doc/modules/_typing.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       47 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/charges.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/constants.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       46 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/cutoff.rst
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.376463 tad_dftd4-0.0.3/doc/modules/damping/
--rw-rw-r--   0 friede    (1000) friede    (1000)       51 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/damping/atm.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       82 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/damping/index.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       56 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/damping/rational.rst
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.376463 tad_dftd4-0.0.3/doc/modules/data/
--rw-rw-r--   0 friede    (1000) friede    (1000)       47 2023-03-13 12:13:06.000000 tad_dftd4-0.0.3/doc/modules/data/en.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       53 2023-03-13 12:13:06.000000 tad_dftd4-0.0.3/doc/modules/data/hardness.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)      100 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/data/index.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 12:13:06.000000 tad_dftd4-0.0.3/doc/modules/data/r4r2.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       50 2023-03-13 12:13:06.000000 tad_dftd4-0.0.3/doc/modules/data/radii.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 12:13:06.000000 tad_dftd4-0.0.3/doc/modules/data/zeff.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       48 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/defaults.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       44 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/disp.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)      257 2023-03-13 12:13:06.000000 tad_dftd4-0.0.3/doc/modules/index.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       45 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/model.rst
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.380463 tad_dftd4-0.0.3/doc/modules/ncoord/
--rw-rw-r--   0 friede    (1000) friede    (1000)       52 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/ncoord/count.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/ncoord/d4.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       50 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/ncoord/eeq.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       83 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/ncoord/index.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       46 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/params.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       45 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/modules/utils.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       80 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/doc/requirements.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)      846 2023-03-13 12:39:51.000000 tad_dftd4-0.0.3/environment.yaml
--rw-rw-r--   0 friede    (1000) friede    (1000)     1439 2023-03-13 12:39:50.000000 tad_dftd4-0.0.3/pyproject.toml
--rw-rw-r--   0 friede    (1000) friede    (1000)     1108 2023-03-13 14:09:05.388463 tad_dftd4-0.0.3/setup.cfg
--rw-rw-r--   0 friede    (1000) friede    (1000)      816 2023-03-13 12:39:58.000000 tad_dftd4-0.0.3/setup.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.372463 tad_dftd4-0.0.3/src/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.380463 tad_dftd4-0.0.3/src/tad_dftd4/
--rw-rw-r--   0 friede    (1000) friede    (1000)     3721 2023-03-13 14:07:11.000000 tad_dftd4-0.0.3/src/tad_dftd4/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      816 2023-03-13 14:07:11.000000 tad_dftd4-0.0.3/src/tad_dftd4/__version__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     7716 2023-03-13 12:40:23.000000 tad_dftd4-0.0.3/src/tad_dftd4/_typing.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    14275 2023-03-13 12:40:18.000000 tad_dftd4-0.0.3/src/tad_dftd4/charges.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2960 2023-03-13 12:40:22.000000 tad_dftd4-0.0.3/src/tad_dftd4/constants.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2393 2023-03-13 12:40:12.000000 tad_dftd4-0.0.3/src/tad_dftd4/cutoff.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.380463 tad_dftd4-0.0.3/src/tad_dftd4/damping/
--rw-rw-r--   0 friede    (1000) friede    (1000)      932 2023-03-13 12:40:22.000000 tad_dftd4-0.0.3/src/tad_dftd4/damping/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4323 2023-03-13 12:40:20.000000 tad_dftd4-0.0.3/src/tad_dftd4/damping/atm.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2039 2023-03-13 12:40:24.000000 tad_dftd4-0.0.3/src/tad_dftd4/damping/rational.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.384463 tad_dftd4-0.0.3/src/tad_dftd4/data/
--rw-rw-r--   0 friede    (1000) friede    (1000)     1045 2023-03-13 12:40:22.000000 tad_dftd4-0.0.3/src/tad_dftd4/data/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2002 2023-03-13 12:40:18.000000 tad_dftd4-0.0.3/src/tad_dftd4/data/en.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3442 2023-03-13 12:40:20.000000 tad_dftd4-0.0.3/src/tad_dftd4/data/hardness.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2611 2023-03-13 12:40:22.000000 tad_dftd4-0.0.3/src/tad_dftd4/data/r4r2.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2132 2023-03-13 12:40:23.000000 tad_dftd4-0.0.3/src/tad_dftd4/data/radii.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1702 2023-03-13 12:40:27.000000 tad_dftd4-0.0.3/src/tad_dftd4/data/zeff.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1594 2023-03-13 11:31:45.000000 tad_dftd4-0.0.3/src/tad_dftd4/defaults.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     9395 2023-03-13 12:40:13.000000 tad_dftd4-0.0.3/src/tad_dftd4/disp.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    11711 2023-03-13 12:40:22.000000 tad_dftd4-0.0.3/src/tad_dftd4/model.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.384463 tad_dftd4-0.0.3/src/tad_dftd4/ncoord/
--rw-rw-r--   0 friede    (1000) friede    (1000)     3060 2023-03-13 12:40:25.000000 tad_dftd4-0.0.3/src/tad_dftd4/ncoord/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3697 2023-03-13 12:40:22.000000 tad_dftd4-0.0.3/src/tad_dftd4/ncoord/count.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3736 2023-03-13 12:40:20.000000 tad_dftd4-0.0.3/src/tad_dftd4/ncoord/d4.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3928 2023-03-13 12:40:22.000000 tad_dftd4-0.0.3/src/tad_dftd4/ncoord/eeq.py
--rw-rw-r--   0 friede    (1000) friede    (1000)   661085 2023-03-13 12:40:59.000000 tad_dftd4-0.0.3/src/tad_dftd4/params.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4713 2023-03-13 12:40:18.000000 tad_dftd4-0.0.3/src/tad_dftd4/utils.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.380463 tad_dftd4-0.0.3/src/tad_dftd4.egg-info/
--rw-rw-r--   0 friede    (1000) friede    (1000)     9818 2023-03-13 14:09:05.000000 tad_dftd4-0.0.3/src/tad_dftd4.egg-info/PKG-INFO
--rw-rw-r--   0 friede    (1000) friede    (1000)     2771 2023-03-13 14:09:05.000000 tad_dftd4-0.0.3/src/tad_dftd4.egg-info/SOURCES.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)        1 2023-03-13 14:09:05.000000 tad_dftd4-0.0.3/src/tad_dftd4.egg-info/dependency_links.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)       75 2023-03-13 14:09:05.000000 tad_dftd4-0.0.3/src/tad_dftd4.egg-info/requires.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)       10 2023-03-13 14:09:05.000000 tad_dftd4-0.0.3/src/tad_dftd4.egg-info/top_level.txt
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.384463 tad_dftd4-0.0.3/test/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:23.000000 tad_dftd4-0.0.3/test/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1812 2023-03-13 12:40:15.000000 tad_dftd4-0.0.3/test/conftest.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    58424 2023-03-13 12:40:37.000000 tad_dftd4-0.0.3/test/molecules.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.384463 tad_dftd4-0.0.3/test/test_charge/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:26.000000 tad_dftd4-0.0.3/test/test_charge/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4372 2023-03-13 12:40:23.000000 tad_dftd4-0.0.3/test/test_charge/samples.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5882 2023-03-13 12:40:20.000000 tad_dftd4-0.0.3/test/test_charge/test_charges.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3169 2023-03-13 12:40:24.000000 tad_dftd4-0.0.3/test/test_charge/test_general.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2097 2023-03-13 12:40:25.000000 tad_dftd4-0.0.3/test/test_charge/test_grad.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.384463 tad_dftd4-0.0.3/test/test_cutoff/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:23.000000 tad_dftd4-0.0.3/test/test_cutoff/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2135 2023-03-13 14:07:11.000000 tad_dftd4-0.0.3/test/test_cutoff/test_general.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2171 2023-03-13 12:40:26.000000 tad_dftd4-0.0.3/test/test_cutoff/test_types.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.384463 tad_dftd4-0.0.3/test/test_disp/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:29.000000 tad_dftd4-0.0.3/test/test_disp/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    29533 2023-03-13 12:40:31.000000 tad_dftd4-0.0.3/test/test_disp/samples.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4347 2023-03-13 12:40:26.000000 tad_dftd4-0.0.3/test/test_disp/test_atm.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4353 2023-03-13 12:40:29.000000 tad_dftd4-0.0.3/test/test_disp/test_full.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1802 2023-03-13 12:40:22.000000 tad_dftd4-0.0.3/test/test_disp/test_general.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2775 2023-03-13 12:40:24.000000 tad_dftd4-0.0.3/test/test_disp/test_grad.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     6524 2023-03-13 12:40:18.000000 tad_dftd4-0.0.3/test/test_disp/test_twobody.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.388463 tad_dftd4-0.0.3/test/test_model/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:26.000000 tad_dftd4-0.0.3/test/test_model/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    47409 2023-03-13 12:40:32.000000 tad_dftd4-0.0.3/test/test_model/samples.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2716 2023-03-13 12:40:29.000000 tad_dftd4-0.0.3/test/test_model/test_c6.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2023 2023-03-13 12:40:29.000000 tad_dftd4-0.0.3/test/test_model/test_general.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2666 2023-03-13 12:40:24.000000 tad_dftd4-0.0.3/test/test_model/test_model.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4163 2023-03-13 12:40:24.000000 tad_dftd4-0.0.3/test/test_model/test_weights.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.388463 tad_dftd4-0.0.3/test/test_ncoord/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:23.000000 tad_dftd4-0.0.3/test/test_ncoord/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5232 2023-03-13 12:40:27.000000 tad_dftd4-0.0.3/test/test_ncoord/samples.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2365 2023-03-13 12:40:26.000000 tad_dftd4-0.0.3/test/test_ncoord/test_cn_d4.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2891 2023-03-13 12:40:25.000000 tad_dftd4-0.0.3/test/test_ncoord/test_cn_eeq.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2153 2023-03-13 12:40:26.000000 tad_dftd4-0.0.3/test/test_ncoord/test_general.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1770 2023-03-13 12:40:27.000000 tad_dftd4-0.0.3/test/test_ncoord/test_grad.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-03-13 14:09:05.388463 tad_dftd4-0.0.3/test/test_utils/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:30.000000 tad_dftd4-0.0.3/test/test_utils/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1750 2023-03-13 12:40:30.000000 tad_dftd4-0.0.3/test/test_utils/test_pack.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5446 2023-03-13 12:40:24.000000 tad_dftd4-0.0.3/test/test_utils/test_real.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1748 2023-03-13 12:40:21.000000 tad_dftd4-0.0.3/test/utils.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1626 2023-03-13 12:39:50.000000 tad_dftd4-0.0.3/tox.ini
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.142567 tad_dftd4-0.0.4/.github/
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/.github/workflows/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1941 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/.github/workflows/python.yml
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1489 2023-05-17 06:54:22.000000 tad_dftd4-0.0.4/.github/workflows/release.yml
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3826 2023-03-13 12:39:50.000000 tad_dftd4-0.0.4/.gitignore
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1677 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/.pre-commit-config.yaml
+-rw-rw-r--   0 friede    (1000) friede    (1000)    14449 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/.pylintrc
+-rw-rw-r--   0 friede    (1000) friede    (1000)       23 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/.readthedocs.yaml
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/.vscode/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      688 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/.vscode/settings.json
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4919 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/CONTRIBUTING.md
+-rw-rw-r--   0 friede    (1000) friede    (1000)    35149 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/COPYING
+-rw-rw-r--   0 friede    (1000) friede    (1000)     7652 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/COPYING.LESSER
+-rw-rw-r--   0 friede    (1000) friede    (1000)    10083 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/PKG-INFO
+-rw-rw-r--   0 friede    (1000) friede    (1000)     9203 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/README.rst
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/_static/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3273 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/doc/_static/tad-dftd4-favicon.svg
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4282 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/doc/_static/tad-dftd4.svg
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1966 2023-03-13 12:40:20.000000 tad_dftd4-0.0.4/doc/conf.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     6408 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/doc/index.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1434 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/installation.rst
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/modules/
+-rw-rw-r--   0 friede    (1000) friede    (1000)       47 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/_typing.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       47 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/charges.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/constants.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       46 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/cutoff.rst
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/modules/damping/
+-rw-rw-r--   0 friede    (1000) friede    (1000)       51 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/damping/atm.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       82 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/damping/index.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       56 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/damping/rational.rst
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/modules/data/
+-rw-rw-r--   0 friede    (1000) friede    (1000)       47 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/data/en.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       53 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/data/hardness.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)      100 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/data/index.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/data/r4r2.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       50 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/data/radii.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/data/zeff.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       48 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/defaults.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       44 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/disp.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)      257 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/index.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       45 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/model.rst
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/modules/ncoord/
+-rw-rw-r--   0 friede    (1000) friede    (1000)       52 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/ncoord/count.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/ncoord/d4.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       50 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/ncoord/eeq.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       83 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/ncoord/index.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       46 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/params.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       45 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/utils.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)       80 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/requirements.txt
+-rw-rw-r--   0 friede    (1000) friede    (1000)      846 2023-03-13 12:39:51.000000 tad_dftd4-0.0.4/environment.yaml
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1439 2023-03-13 12:39:50.000000 tad_dftd4-0.0.4/pyproject.toml
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1108 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/setup.cfg
+-rw-rw-r--   0 friede    (1000) friede    (1000)      816 2023-03-13 12:39:58.000000 tad_dftd4-0.0.4/setup.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.142567 tad_dftd4-0.0.4/src/
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/src/tad_dftd4/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3721 2023-03-13 14:07:11.000000 tad_dftd4-0.0.4/src/tad_dftd4/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)      816 2023-05-17 06:54:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/__version__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     7716 2023-03-13 12:40:23.000000 tad_dftd4-0.0.4/src/tad_dftd4/_typing.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)    14333 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/charges.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2960 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/constants.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2393 2023-03-13 12:40:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/cutoff.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/src/tad_dftd4/damping/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      932 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/damping/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4384 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/damping/atm.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2099 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/damping/rational.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/src/tad_dftd4/data/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1045 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2002 2023-03-13 12:40:18.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/en.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3442 2023-03-13 12:40:20.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/hardness.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2611 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/r4r2.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2132 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/radii.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1702 2023-03-13 12:40:27.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/zeff.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1594 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/src/tad_dftd4/defaults.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     9479 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/disp.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)    11893 2023-05-17 06:54:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/model.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/src/tad_dftd4/ncoord/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3060 2023-03-13 12:40:25.000000 tad_dftd4-0.0.4/src/tad_dftd4/ncoord/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3697 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/ncoord/count.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3794 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/ncoord/d4.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4019 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/ncoord/eeq.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)   661085 2023-03-13 12:40:59.000000 tad_dftd4-0.0.4/src/tad_dftd4/params.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4713 2023-03-13 12:40:18.000000 tad_dftd4-0.0.4/src/tad_dftd4/utils.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/
+-rw-rw-r--   0 friede    (1000) friede    (1000)    10083 2023-05-17 06:56:31.000000 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/PKG-INFO
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2771 2023-05-17 06:56:31.000000 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/SOURCES.txt
+-rw-rw-r--   0 friede    (1000) friede    (1000)        1 2023-05-17 06:56:31.000000 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/dependency_links.txt
+-rw-rw-r--   0 friede    (1000) friede    (1000)       75 2023-05-17 06:56:31.000000 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/requires.txt
+-rw-rw-r--   0 friede    (1000) friede    (1000)       10 2023-05-17 06:56:31.000000 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/top_level.txt
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/test/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:23.000000 tad_dftd4-0.0.4/test/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1812 2023-03-13 12:40:15.000000 tad_dftd4-0.0.4/test/conftest.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)    58424 2023-03-13 12:40:37.000000 tad_dftd4-0.0.4/test/molecules.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/test/test_charge/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_charge/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4372 2023-03-13 12:40:23.000000 tad_dftd4-0.0.4/test/test_charge/samples.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     5882 2023-03-13 12:40:20.000000 tad_dftd4-0.0.4/test/test_charge/test_charges.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3169 2023-03-13 12:40:24.000000 tad_dftd4-0.0.4/test/test_charge/test_general.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2097 2023-03-13 12:40:25.000000 tad_dftd4-0.0.4/test/test_charge/test_grad.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/test/test_cutoff/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:23.000000 tad_dftd4-0.0.4/test/test_cutoff/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2135 2023-03-13 14:07:11.000000 tad_dftd4-0.0.4/test/test_cutoff/test_general.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2171 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_cutoff/test_types.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/test/test_disp/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:29.000000 tad_dftd4-0.0.4/test/test_disp/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)    29533 2023-03-13 12:40:31.000000 tad_dftd4-0.0.4/test/test_disp/samples.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4347 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_disp/test_atm.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4353 2023-03-13 12:40:29.000000 tad_dftd4-0.0.4/test/test_disp/test_full.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1802 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/test/test_disp/test_general.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2775 2023-03-13 12:40:24.000000 tad_dftd4-0.0.4/test/test_disp/test_grad.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     6524 2023-03-13 12:40:18.000000 tad_dftd4-0.0.4/test/test_disp/test_twobody.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/test/test_model/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_model/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)    47409 2023-03-13 12:40:32.000000 tad_dftd4-0.0.4/test/test_model/samples.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2716 2023-03-13 12:40:29.000000 tad_dftd4-0.0.4/test/test_model/test_c6.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2023 2023-03-13 12:40:29.000000 tad_dftd4-0.0.4/test/test_model/test_general.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2666 2023-03-13 12:40:24.000000 tad_dftd4-0.0.4/test/test_model/test_model.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4163 2023-03-13 12:40:24.000000 tad_dftd4-0.0.4/test/test_model/test_weights.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/test/test_ncoord/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:23.000000 tad_dftd4-0.0.4/test/test_ncoord/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     5232 2023-03-13 12:40:27.000000 tad_dftd4-0.0.4/test/test_ncoord/samples.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2365 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_ncoord/test_cn_d4.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2891 2023-03-13 12:40:25.000000 tad_dftd4-0.0.4/test/test_ncoord/test_cn_eeq.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2153 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_ncoord/test_general.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1770 2023-03-13 12:40:27.000000 tad_dftd4-0.0.4/test/test_ncoord/test_grad.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/test/test_utils/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:30.000000 tad_dftd4-0.0.4/test/test_utils/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1750 2023-03-13 12:40:30.000000 tad_dftd4-0.0.4/test/test_utils/test_pack.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     5446 2023-03-13 12:40:24.000000 tad_dftd4-0.0.4/test/test_utils/test_real.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1748 2023-03-13 12:40:21.000000 tad_dftd4-0.0.4/test/utils.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1626 2023-03-13 12:39:50.000000 tad_dftd4-0.0.4/tox.ini
```

### Comparing `tad_dftd4-0.0.3/.github/workflows/python.yml` & `tad_dftd4-0.0.4/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/.github/workflows/release.yml` & `tad_dftd4-0.0.4/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,14 @@
           path: dist
 
       - name: Publish to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.TEST_PYPI_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
+          repository-url: https://test.pypi.org/legacy/
 
       - name: Publish to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `tad_dftd4-0.0.3/.gitignore` & `tad_dftd4-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/.pre-commit-config.yaml` & `tad_dftd4-0.0.4/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -31,23 +31,23 @@
   - repo: https://github.com/asottile/setup-cfg-fmt
     rev: v2.2.0
     hooks:
       - id: setup-cfg-fmt
         args: [--include-version-classifiers, --max-py-version, "3.11"]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.1.0
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
         args: [--py37-plus, --keep-runtime-typing]
 
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
         args: ["--profile", "black", "--filter-files"]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
```

### Comparing `tad_dftd4-0.0.3/.pylintrc` & `tad_dftd4-0.0.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/.vscode/settings.json` & `tad_dftd4-0.0.4/.vscode/settings.json`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "editor.formatOnPaste": false, // not supported by black
     "editor.insertSpaces": true,
     "editor.tabSize": 4
   },
   "python.analysis.diagnosticSeverityOverrides": {
     "reportPrivateImportUsage": "information"
   },
-  "python.defaultInterpreterPath": "${env:CONDA_PREFIX}/envs/dxtb/bin/python",
+  "python.defaultInterpreterPath": "${env:CONDA_PREFIX}/envs/torch/bin/python",
   "python.formatting.provider": "black",
   "python.linting.enabled": true,
   "python.linting.pylintEnabled": true,
   "python.linting.pylintArgs": ["--indent-string='    '"],
   "python.testing.pytestArgs": [],
   "python.testing.unittestEnabled": false,
   "python.testing.pytestEnabled": true
```

### Comparing `tad_dftd4-0.0.3/CONTRIBUTING.md` & `tad_dftd4-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/COPYING` & `tad_dftd4-0.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/COPYING.LESSER` & `tad_dftd4-0.0.4/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/PKG-INFO` & `tad_dftd4-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_dftd4
-Version: 0.0.3
+Version: 0.0.4
 Summary: Torch autodiff DFT-D4 implementation
 Author: "Marvin Friede"
 License: LGPL-3.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -105,24 +105,36 @@
 Install the required dependencies from the conda-forge channel.
 
 .. code::
 
     mamba env create -n torch -f environment.yaml
     mamba activate torch
 
+Install this project with ``pip`` in the environment
+
+.. code::
+
+    pip install .
+
+The following dependencies are required
+
+- `numpy <https://numpy.org/>`__
+- `torch <https://pytorch.org/>`__
+- `pytest <https://docs.pytest.org/>`__ (tests only)
+
 Development
 -----------
 
 For development, additionally install the following tools in your environment.
 
 .. code::
 
     mamba install black covdefaults coverage mypy pre-commit pylint tox
 
-With pip, add the option ``-e`` and the development dependencies for installing in development mode.
+With pip, add the option ``-e`` for installing in development mode, and add ``[dev]`` for the development dependencies
 
 .. code::
 
     pip install -e .[dev]
 
 The pre-commit hooks are initialized by running the following command in the root of the repository.
 
@@ -132,24 +144,24 @@
 
 For testing all Python environments, simply run `tox`.
 
 .. code::
 
     tox
 
-Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional _posargs_.
+Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional *posargs*.
 
 .. code::
 
     tox -- test
 
 Examples
 --------
 
-The following example shows how to calculate the DFT-D3 dispersion energy for a single structure.
+The following example shows how to calculate the DFT-D4 dispersion energy for a single structure.
 
 .. code:: python
 
     import torch
     import tad_dftd4 as d4
 
     numbers = d4.utils.to_number(symbols="C C C C N C S H H H H H".split())
```

### Comparing `tad_dftd4-0.0.3/README.rst` & `tad_dftd4-0.0.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -81,24 +81,36 @@
 Install the required dependencies from the conda-forge channel.
 
 .. code::
 
     mamba env create -n torch -f environment.yaml
     mamba activate torch
 
+Install this project with ``pip`` in the environment
+
+.. code::
+
+    pip install .
+
+The following dependencies are required
+
+- `numpy <https://numpy.org/>`__
+- `torch <https://pytorch.org/>`__
+- `pytest <https://docs.pytest.org/>`__ (tests only)
+
 Development
 -----------
 
 For development, additionally install the following tools in your environment.
 
 .. code::
 
     mamba install black covdefaults coverage mypy pre-commit pylint tox
 
-With pip, add the option ``-e`` and the development dependencies for installing in development mode.
+With pip, add the option ``-e`` for installing in development mode, and add ``[dev]`` for the development dependencies
 
 .. code::
 
     pip install -e .[dev]
 
 The pre-commit hooks are initialized by running the following command in the root of the repository.
 
@@ -108,24 +120,24 @@
 
 For testing all Python environments, simply run `tox`.
 
 .. code::
 
     tox
 
-Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional _posargs_.
+Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional *posargs*.
 
 .. code::
 
     tox -- test
 
 Examples
 --------
 
-The following example shows how to calculate the DFT-D3 dispersion energy for a single structure.
+The following example shows how to calculate the DFT-D4 dispersion energy for a single structure.
 
 .. code:: python
 
     import torch
     import tad_dftd4 as d4
 
     numbers = d4.utils.to_number(symbols="C C C C N C S H H H H H".split())
```

### Comparing `tad_dftd4-0.0.3/doc/_static/tad-dftd4-favicon.svg` & `tad_dftd4-0.0.4/doc/_static/tad-dftd4-favicon.svg`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 000000d0: 7273 696f 6e3d 2231 2e31 220a 2020 2069  rsion="1.1".   i
 000000e0: 643d 2273 7667 3522 0a20 2020 696e 6b73  d="svg5".   inks
 000000f0: 6361 7065 3a76 6572 7369 6f6e 3d22 312e  cape:version="1.
 00000100: 322e 3220 2831 3a31 2e32 2e32 2b32 3032  2.2 (1:1.2.2+202
 00000110: 3231 3230 3531 3535 302b 6230 6138 3438  212051550+b0a848
 00000120: 3635 3431 2922 0a20 2020 736f 6469 706f  6541)".   sodipo
 00000130: 6469 3a64 6f63 6e61 6d65 3d22 7461 642d  di:docname="tad-
-00000140: 6466 7464 332d 6661 7669 636f 6e2e 7376  dftd3-favicon.sv
+00000140: 6466 7464 342d 6661 7669 636f 6e2e 7376  dftd4-favicon.sv
 00000150: 6722 0a20 2020 786d 6c6e 733a 696e 6b73  g".   xmlns:inks
 00000160: 6361 7065 3d22 6874 7470 3a2f 2f77 7777  cape="http://www
 00000170: 2e69 6e6b 7363 6170 652e 6f72 672f 6e61  .inkscape.org/na
 00000180: 6d65 7370 6163 6573 2f69 6e6b 7363 6170  mespaces/inkscap
 00000190: 6522 0a20 2020 786d 6c6e 733a 736f 6469  e".   xmlns:sodi
 000001a0: 706f 6469 3d22 6874 7470 3a2f 2f73 6f64  podi="http://sod
 000001b0: 6970 6f64 692e 736f 7572 6365 666f 7267  ipodi.sourceforg
@@ -79,15 +79,15 @@
 000004e0: 2020 2069 6e6b 7363 6170 653a 6772 6f75     inkscape:grou
 000004f0: 706d 6f64 653d 226c 6179 6572 220a 2020  pmode="layer".  
 00000500: 2020 2069 643d 226c 6179 6572 3122 0a20     id="layer1". 
 00000510: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
 00000520: 7261 6e73 6c61 7465 282d 3631 2e31 3936  ranslate(-61.196
 00000530: 3039 342c 2d39 302e 3238 3332 3637 2922  094,-90.283267)"
 00000540: 3e0a 2020 2020 3c67 0a20 2020 2020 2020  >.    <g.       
-00000550: 6172 6961 2d6c 6162 656c 3d22 4433 220a  aria-label="D3".
+00000550: 6172 6961 2d6c 6162 656c 3d22 4434 220a  aria-label="D4".
 00000560: 2020 2020 2020 2069 643d 2274 6578 7431         id="text1
 00000570: 3137 3822 0a20 2020 2020 2020 7374 796c  178".       styl
 00000580: 653d 2266 6f6e 742d 7765 6967 6874 3a36  e="font-weight:6
 00000590: 3030 3b66 6f6e 742d 7369 7a65 3a32 352e  00;font-size:25.
 000005a0: 3470 783b 6c69 6e65 2d68 6569 6768 743a  4px;line-height:
 000005b0: 312e 3235 3b66 6f6e 742d 6661 6d69 6c79  1.25;font-family
 000005c0: 3a27 536f 7572 6365 2053 616e 7320 5072  :'Source Sans Pr
```

### Comparing `tad_dftd4-0.0.3/doc/_static/tad-dftd4.svg` & `tad_dftd4-0.0.4/doc/_static/tad-dftd4.svg`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 000000d0: 696f 6e3d 2231 2e31 220a 2020 2069 643d  ion="1.1".   id=
 000000e0: 2273 7667 3522 0a20 2020 696e 6b73 6361  "svg5".   inksca
 000000f0: 7065 3a76 6572 7369 6f6e 3d22 312e 322e  pe:version="1.2.
 00000100: 3220 2831 3a31 2e32 2e32 2b32 3032 3231  2 (1:1.2.2+20221
 00000110: 3230 3531 3535 302b 6230 6138 3438 3635  2051550+b0a84865
 00000120: 3431 2922 0a20 2020 736f 6469 706f 6469  41)".   sodipodi
 00000130: 3a64 6f63 6e61 6d65 3d22 7461 642d 6466  :docname="tad-df
-00000140: 7464 332e 7376 6722 0a20 2020 786d 6c6e  td3.svg".   xmln
+00000140: 7464 342e 7376 6722 0a20 2020 786d 6c6e  td4.svg".   xmln
 00000150: 733a 696e 6b73 6361 7065 3d22 6874 7470  s:inkscape="http
 00000160: 3a2f 2f77 7777 2e69 6e6b 7363 6170 652e  ://www.inkscape.
 00000170: 6f72 672f 6e61 6d65 7370 6163 6573 2f69  org/namespaces/i
 00000180: 6e6b 7363 6170 6522 0a20 2020 786d 6c6e  nkscape".   xmln
 00000190: 733a 736f 6469 706f 6469 3d22 6874 7470  s:sodipodi="http
 000001a0: 3a2f 2f73 6f64 6970 6f64 692e 736f 7572  ://sodipodi.sour
 000001b0: 6365 666f 7267 652e 6e65 742f 4454 442f  ceforge.net/DTD/
@@ -83,15 +83,15 @@
 00000520: 726f 7570 6d6f 6465 3d22 6c61 7965 7222  roupmode="layer"
 00000530: 0a20 2020 2020 6964 3d22 6c61 7965 7231  .     id="layer1
 00000540: 220a 2020 2020 2074 7261 6e73 666f 726d  ".     transform
 00000550: 3d22 7472 616e 736c 6174 6528 2d34 372e  ="translate(-47.
 00000560: 3634 3038 3132 2c2d 3838 2e34 3138 3033  640812,-88.41803
 00000570: 3429 223e 0a20 2020 203c 670a 2020 2020  4)">.    <g.    
 00000580: 2020 2061 7269 612d 6c61 6265 6c3d 2244     aria-label="D
-00000590: 3322 0a20 2020 2020 2020 6964 3d22 7465  3".       id="te
+00000590: 3422 0a20 2020 2020 2020 6964 3d22 7465  4".       id="te
 000005a0: 7874 3131 3738 220a 2020 2020 2020 2073  xt1178".       s
 000005b0: 7479 6c65 3d22 666f 6e74 2d77 6569 6768  tyle="font-weigh
 000005c0: 743a 3630 303b 666f 6e74 2d73 697a 653a  t:600;font-size:
 000005d0: 3235 2e34 7078 3b6c 696e 652d 6865 6967  25.4px;line-heig
 000005e0: 6874 3a31 2e32 353b 666f 6e74 2d66 616d  ht:1.25;font-fam
 000005f0: 696c 793a 2753 6f75 7263 6520 5361 6e73  ily:'Source Sans
 00000600: 2050 726f 273b 2d69 6e6b 7363 6170 652d   Pro';-inkscape-
```

### Comparing `tad_dftd4-0.0.3/doc/conf.py` & `tad_dftd4-0.0.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/doc/index.rst` & `tad_dftd4-0.0.4/doc/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 - \E. Caldeweyher, J.-M. Mewes, S. Ehlert and S. Grimme, *Phys. Chem. Chem. Phys.*, **2020**, *22*, 8499-8512. DOI: `10.1039/D0CP00502A <https://doi.org/10.1039/D0CP00502A>`__
 
 
 Examples
 --------
 
-The following example shows how to calculate the DFT-D3 dispersion energy for a single structure.
+The following example shows how to calculate the DFT-D4 dispersion energy for a single structure.
 
 .. code:: python
 
     import torch
     import tad_dftd4 as d4
 
     numbers = d4.utils.to_number(symbols="C C C C N C S H H H H H".split())
```

### Comparing `tad_dftd4-0.0.3/doc/installation.rst` & `tad_dftd4-0.0.4/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/environment.yaml` & `tad_dftd4-0.0.4/environment.yaml`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/pyproject.toml` & `tad_dftd4-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/setup.cfg` & `tad_dftd4-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/setup.py` & `tad_dftd4-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/__init__.py` & `tad_dftd4-0.0.4/src/tad_dftd4/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/__version__.py` & `tad_dftd4-0.0.4/src/tad_dftd4/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with tad-dftd4. If not, see <https://www.gnu.org/licenses/>.
 """
 Module containing the version string.
 """
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/_typing.py` & `tad_dftd4-0.0.4/src/tad_dftd4/_typing.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/charges.py` & `tad_dftd4-0.0.4/src/tad_dftd4/charges.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,15 @@
     tensor([[-9.3132e-09,  7.4506e-09, -4.8064e-02],
             [-1.2595e-02,  2.1816e-02,  1.6021e-02],
             [-1.2595e-02, -2.1816e-02,  1.6021e-02],
             [ 2.5191e-02, -6.9849e-10,  1.6021e-02]])
     >>> print(total_charge.grad)
     tensor(0.6312)
     """
+    dd = {"device": positions.device, "dtype": positions.dtype}
 
     if model.device != positions.device:
         raise RuntimeError(
             f"All tensors of '{model.__class__.__name__}' must be on the same "
             f"device!\nUse `{model.__class__.__name__}.param2019().to(device)` "
             "to correctly set the device."
         )
@@ -284,15 +285,15 @@
     if model.dtype != positions.dtype:
         raise RuntimeError(
             f"All tensors of '{model.__class__.__name__}' must have the same "
             f"dtype!\nUse `{model.__class__.__name__}.param2019().type(dtype)` "
             "to correctly set the dtype."
         )
 
-    eps = positions.new_tensor(torch.finfo(positions.dtype).eps)
+    eps = torch.tensor(torch.finfo(positions.dtype).eps, **dd)
 
     real = real_atoms(numbers)
     mask = real_pairs(numbers, diagonal=True)
 
     distances = torch.where(
         mask,
         torch.cdist(positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"),
@@ -310,23 +311,23 @@
     )
 
     rad = model.rad[numbers]
     gamma = 1.0 / torch.sqrt(rad.unsqueeze(-1) ** 2 + rad.unsqueeze(-2) ** 2)
     eta = torch.where(
         real,
         model.eta[numbers] + torch.sqrt(torch.tensor(2.0 / math.pi)) / rad,
-        distances.new_tensor(1.0),
+        torch.tensor(1.0, **dd),
     )
     coulomb = torch.where(
         diagonal,
         eta.unsqueeze(-1),
         torch.where(
             mask,
             torch.erf(distances * gamma) / distances,
-            distances.new_tensor(0.0),
+            torch.tensor(0.0, **dd),
         ),
     )
     constraint = torch.where(
         real,
         distances.new_ones(numbers.shape),
         distances.new_zeros(numbers.shape),
     )
```

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/constants.py` & `tad_dftd4-0.0.4/src/tad_dftd4/constants.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/cutoff.py` & `tad_dftd4-0.0.4/src/tad_dftd4/cutoff.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/damping/__init__.py` & `tad_dftd4-0.0.4/src/tad_dftd4/damping/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/damping/atm.py` & `tad_dftd4-0.0.4/src/tad_dftd4/damping/atm.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,16 @@
         Exponent of zero damping function. Defaults to `14.0`.
 
     Returns
     -------
     Tensor
         Atom-resolved ATM dispersion energy.
     """
+    dd = {"device": positions.device, "dtype": positions.dtype}
+
     s9 = s9.type(positions.dtype).to(positions.device)
     alp = alp.type(positions.dtype).to(positions.device)
 
     cutoff2 = cutoff * cutoff
 
     # C9_ABC = s9 * sqrt(|C6_AB * C6_AC * C6_BC|)
     c9 = s9 * torch.sqrt(
@@ -105,15 +107,15 @@
     # very slow: (pos.unsqueeze(-2) - pos.unsqueeze(-3)).pow(2).sum(-1)
     distances = torch.pow(
         torch.where(
             real_pairs(numbers, diagonal=False),
             torch.cdist(
                 positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"
             ),
-            positions.new_tensor(torch.finfo(positions.dtype).eps),
+            torch.tensor(torch.finfo(positions.dtype).eps, **dd),
         ),
         2.0,
     )
 
     r2ij = distances.unsqueeze(-1)
     r2ik = distances.unsqueeze(-2)
     r2jk = distances.unsqueeze(-3)
@@ -127,12 +129,12 @@
     s = (r2ij + r2jk - r2ik) * (r2ij - r2jk + r2ik) * (-r2ij + r2jk + r2ik)
     ang = torch.where(
         real_triples(numbers, diagonal=False)
         * (r2ij <= cutoff2)
         * (r2jk <= cutoff2)
         * (r2jk <= cutoff2),
         0.375 * s / r5 + 1.0 / r3,
-        positions.new_tensor(0.0),
+        torch.tensor(0.0, **dd),
     )
 
     energy = ang * fdamp * c9
     return torch.sum(energy, dim=(-2, -1)) / 6.0
```

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/damping/rational.py` & `tad_dftd4-0.0.4/src/tad_dftd4/damping/rational.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,11 +58,12 @@
         DFT-D4 damping parameters.
 
     Returns
     -------
     Tensor
         Values of the damping function.
     """
+    dd = {"device": distances.device, "dtype": distances.dtype}
 
-    a1 = param.get("a1", distances.new_tensor(defaults.A1))
-    a2 = param.get("a2", distances.new_tensor(defaults.A2))
+    a1 = param.get("a1", torch.tensor(defaults.A1, **dd))
+    a2 = param.get("a2", torch.tensor(defaults.A2, **dd))
     return 1.0 / (distances.pow(order) + (a1 * torch.sqrt(qq) + a2).pow(order))
```

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/data/__init__.py` & `tad_dftd4-0.0.4/src/tad_dftd4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/data/en.py` & `tad_dftd4-0.0.4/src/tad_dftd4/data/en.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/data/hardness.py` & `tad_dftd4-0.0.4/src/tad_dftd4/data/hardness.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/data/r4r2.py` & `tad_dftd4-0.0.4/src/tad_dftd4/data/r4r2.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/data/radii.py` & `tad_dftd4-0.0.4/src/tad_dftd4/data/radii.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with tad-dftd4. If not, see <https://www.gnu.org/licenses/>.
 """
 Atomic data: Radii
 ==================
 
-Covalent radii for DFT-D3 coordination number.
+Covalent radii for DFT-D4 coordination number.
 """
 
 import torch
 
 from .. import constants
 
 __all__ = ["cov_rad_d3"]
```

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/data/zeff.py` & `tad_dftd4-0.0.4/src/tad_dftd4/data/zeff.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/defaults.py` & `tad_dftd4-0.0.4/src/tad_dftd4/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/disp.py` & `tad_dftd4-0.0.4/src/tad_dftd4/disp.py`

 * *Files 10% similar despite different names*

```diff
@@ -191,52 +191,55 @@
         will be evaluated to `defaults.D4_DISP2_CUTOFF`.
 
     Returns
     -------
     Tensor
         Atom-resolved two-body dispersion energy.
     """
+    dd = {"device": positions.device, "dtype": positions.dtype}
+    zero = torch.tensor(0.0, **dd)
+
     if cutoff is None:
-        cutoff = positions.new_tensor(defaults.D4_DISP2_CUTOFF)
+        cutoff = torch.tensor(defaults.D4_DISP2_CUTOFF, **dd)
 
     mask = real_pairs(numbers, diagonal=False)
     distances = torch.where(
         mask,
         torch.cdist(positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"),
-        positions.new_tensor(torch.finfo(positions.dtype).eps),
+        torch.tensor(torch.finfo(positions.dtype).eps, **dd),
     )
 
     qq = 3 * r4r2.unsqueeze(-1) * r4r2.unsqueeze(-2)
     c8 = c6 * qq
 
     t6 = torch.where(
         mask * (distances <= cutoff),
         damping_function(6, distances, qq, param, **kwargs),
-        positions.new_tensor(0.0),
+        zero,
     )
     t8 = torch.where(
         mask * (distances <= cutoff),
         damping_function(8, distances, qq, param, **kwargs),
-        positions.new_tensor(0.0),
+        zero,
     )
 
     e6 = torch.sum(c6 * t6, dim=-1)
     e8 = torch.sum(c8 * t8, dim=-1)
 
-    s6 = param.get("s6", positions.new_tensor(defaults.S6))
-    s8 = param.get("s8", positions.new_tensor(defaults.S8))
+    s6 = param.get("s6", torch.tensor(defaults.S6, **dd))
+    s8 = param.get("s8", torch.tensor(defaults.S8, **dd))
 
     edisp = s6 * e6 + s8 * e8
 
     if "s10" in param and param["s10"] != 0.0:
         c10 = c6 * torch.pow(qq, 2) * 49.0 / 40.0
         t10 = torch.where(
             mask * (distances <= cutoff),
             damping_function(10, distances, qq, param, **kwargs),
-            positions.new_tensor(0.0),
+            zero,
         )
         e10 = torch.sum(c10 * t10, dim=-1)
         edisp += param["s10"] * e10
 
     return -0.5 * edisp
 
 
@@ -266,16 +269,18 @@
         Real-space cutoff. Defaults to `None`, i.e, `defaults.D4_DISP3_CUTOFF`.
 
     Returns
     -------
     Tensor
         Atom-resolved three-body dispersion energy.
     """
+    dd = {"device": positions.device, "dtype": positions.dtype}
+
     if cutoff is None:
-        cutoff = positions.new_tensor(defaults.D4_DISP3_CUTOFF)
+        cutoff = torch.tensor(defaults.D4_DISP3_CUTOFF, **dd)
 
-    s9 = param.get("s9", positions.new_tensor(defaults.S9))
-    a1 = param.get("a1", positions.new_tensor(defaults.A1))
-    a2 = param.get("a2", positions.new_tensor(defaults.A2))
-    alp = param.get("alp", positions.new_tensor(defaults.ALP))
+    s9 = param.get("s9", torch.tensor(defaults.S9, **dd))
+    a1 = param.get("a1", torch.tensor(defaults.A1, **dd))
+    a2 = param.get("a2", torch.tensor(defaults.A2, **dd))
+    alp = param.get("alp", torch.tensor(defaults.ALP, **dd))
 
     return get_atm_dispersion(numbers, positions, cutoff, c6, s9, a1, a2, alp)
```

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/model.py` & `tad_dftd4-0.0.4/src/tad_dftd4/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,14 +155,16 @@
             Partial charge of every atom. Defaults to `None` (0).
 
         Returns
         -------
         Tensor
             Weights for the atomic reference systems.
         """
+        dd = {"device": self.device, "dtype": self.dtype}
+
         if cn is None:
             cn = torch.zeros_like(self.numbers, dtype=self.dtype)
         if q is None:
             q = torch.zeros_like(self.numbers, dtype=self.dtype)
 
         refc = params.refc[self.numbers].to(self.device)
         refq = params.refq[self.numbers].type(self.dtype).to(self.device)
@@ -198,15 +200,15 @@
                 + torch.pow(tmp, 3 * self.wf),
                 torch.where(
                     refc == 1,
                     torch.pow(tmp, self.wf),
                     tmp,
                 ),
             ),
-            dcn.new_tensor(0.0),
+            torch.tensor(0.0, device=self.device, dtype=refcn.dtype),  # double!
         )
 
         # normalize weights
         norm = torch.sum(expw, dim=-1, keepdim=True)
         gw_temp = (expw / norm).type(self.dtype)
 
         # maximum reference CN for each atom
@@ -215,30 +217,30 @@
         # prevent division by 0 and small values
         exceptional = (torch.isnan(gw_temp)) | (gw_temp > torch.finfo(self.dtype).max)
 
         gw = torch.where(
             exceptional,
             torch.where(
                 refcn == maxcn,
-                gw_temp.new_tensor(1.0),
-                gw_temp.new_tensor(0.0),
+                torch.tensor(1.0, **dd),
+                torch.tensor(0.0, **dd),
             ),
             gw_temp,
         )
 
         # unsqueeze for reference dimension
         zeff = data.zeff[self.numbers].unsqueeze(-1)
         gam = data.gam[self.numbers].unsqueeze(-1) * self.gc
         q = q.unsqueeze(-1)
 
         # charge scaling
         zeta = torch.where(
             mask,
             self._zeta(gam, refq + zeff, q + zeff),
-            gw_temp.new_tensor(0.0),
+            torch.tensor(0.0, **dd),
         )
 
         return zeta * gw
 
     def get_atomic_c6(self, gw: Tensor) -> Tensor:
         """
         Calculate atomic C6 dispersion coefficients.
@@ -285,26 +287,28 @@
         -------
         Tensor
             Scaled charges.
         """
         return torch.where(
             qmod > 0.0,
             torch.exp(self.ga * (1.0 - torch.exp(gam * (1.0 - qref / qmod)))),
-            torch.exp(qmod.new_tensor(self.ga)),
+            torch.exp(torch.tensor(self.ga, device=self.device, dtype=self.dtype)),
         )
 
     def _set_refalpha_eeq(self) -> Tensor:
         """
         Set the reference polarizibilities for unique species.
 
         Returns
         -------
         Tensor
             Reference polarizibilities for unique species (not all atoms).
         """
+        zero = torch.tensor(0.0, device=self.device, dtype=self.dtype)
+
         numbers = self.unique
         refsys = params.refsys[numbers].to(self.device)
         refsq = params.refsq[numbers].type(self.dtype).to(self.device)
         refascale = params.refascale[numbers].type(self.dtype).to(self.device)
         refalpha = params.refalpha[numbers].type(self.dtype).to(self.device)
         refscount = params.refscount[numbers].type(self.dtype).to(self.device)
         secscale = params.secscale.type(self.dtype).to(self.device)
@@ -317,22 +321,22 @@
 
         aiw = secscale[refsys] * secalpha[refsys]
 
         # charge scaling
         zeta = torch.where(
             mask,
             self._zeta(gam, zeff, refsq + zeff),
-            gam.new_tensor(0.0),
+            zero,
         )
 
         aiw = secscale[refsys] * secalpha[refsys] * zeta.unsqueeze(-1)
         h = refalpha - refscount.unsqueeze(-1) * aiw
         alpha = refascale.unsqueeze(-1) * h
 
-        return torch.where(alpha > 0.0, alpha, alpha.new_tensor(0.0))
+        return torch.where(alpha > 0.0, alpha, zero)
 
 
 def trapzd(polarizability: Tensor) -> Tensor:
     """
     Numerical Casimir--Polder integration.
 
     Parameters
```

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/ncoord/__init__.py` & `tad_dftd4-0.0.4/src/tad_dftd4/ncoord/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/ncoord/count.py` & `tad_dftd4-0.0.4/src/tad_dftd4/ncoord/count.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/ncoord/d4.py` & `tad_dftd4-0.0.4/src/tad_dftd4/ncoord/d4.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,18 @@
         Coordination numbers for all atoms.
 
     Raises
     ------
     ValueError
         If shape mismatch between `numbers`, `positions` and `rcov` is detected.
     """
+    dd = {"device": positions.device, "dtype": positions.dtype}
 
     if cutoff is None:
-        cutoff = positions.new_tensor(defaults.D4_CN_CUTOFF)
+        cutoff = torch.tensor(defaults.D4_CN_CUTOFF, **dd)
 
     if rcov is None:
         rcov = cov_rad_d3[numbers]
     rcov = rcov.type(positions.dtype).to(positions.device)
 
     if en is None:
         en = pauling_en[numbers]
@@ -98,23 +99,23 @@
         )
 
     mask = real_pairs(numbers)
 
     distances = torch.where(
         mask,
         torch.cdist(positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"),
-        positions.new_tensor(torch.finfo(positions.dtype).eps),
+        torch.tensor(torch.finfo(positions.dtype).eps, **dd),
     )
 
     # Eq. 6
     endiff = torch.abs(en.unsqueeze(-2) - en.unsqueeze(-1))
     den = defaults.D4_K4 * torch.exp(
         -((endiff + defaults.D4_K5) ** 2.0) / defaults.D4_K6
     )
 
     rc = rcov.unsqueeze(-2) + rcov.unsqueeze(-1)
     cf = torch.where(
         mask * (distances <= cutoff),
         den * counting_function(distances, rc, **kwargs),
-        positions.new_tensor(0.0),
+        torch.tensor(0.0, **dd),
     )
     return torch.sum(cf, dim=-1)
```

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/ncoord/eeq.py` & `tad_dftd4-0.0.4/src/tad_dftd4/ncoord/eeq.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,17 +70,18 @@
         Coordination numbers for all atoms.
 
     Raises
     ------
     ValueError
         If shape mismatch between `numbers`, `positions` and `rcov` is detected.
     """
+    dd = {"device": positions.device, "dtype": positions.dtype}
 
     if cutoff is None:
-        cutoff = positions.new_tensor(defaults.D4_CN_EEQ_CUTOFF)
+        cutoff = torch.tensor(defaults.D4_CN_EEQ_CUTOFF, **dd)
 
     if rcov is None:
         rcov = cov_rad_d3[numbers]
     rcov = rcov.type(positions.dtype).to(positions.device)
 
     if numbers.shape != rcov.shape:
         raise ValueError(
@@ -98,34 +99,34 @@
         mask,
         torch.cdist(
             positions,
             positions,
             p=2,
             compute_mode="use_mm_for_euclid_dist",
         ),
-        positions.new_tensor(torch.finfo(positions.dtype).eps),
+        torch.tensor(torch.finfo(positions.dtype).eps, **dd),
     )
 
     rc = rcov.unsqueeze(-2) + rcov.unsqueeze(-1)
     cf = torch.where(
         mask * (distances <= cutoff),
         counting_function(distances, rc, **kwargs),
-        positions.new_tensor(0.0),
+        torch.tensor(0.0, **dd),
     )
     cn = torch.sum(cf, dim=-1)
 
     if cn_max is None:
         return cn
 
     return cut_coordination_number(cn, cn_max)
 
 
 def cut_coordination_number(
     cn: Tensor, cn_max: Tensor | float | int = defaults.D4_CN_EEQ_MAX
 ):
     if isinstance(cn_max, (float, int)):
-        cn_max = cn.new_tensor(cn_max)
+        cn_max = torch.tensor(cn_max, device=cn.device, dtype=cn.dtype)
 
     if cn_max > 50:
         return cn
 
     return torch.log(1.0 + torch.exp(cn_max)) - torch.log(1.0 + torch.exp(cn_max - cn))
```

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/params.py` & `tad_dftd4-0.0.4/src/tad_dftd4/params.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4/utils.py` & `tad_dftd4-0.0.4/src/tad_dftd4/utils.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4.egg-info/PKG-INFO` & `tad_dftd4-0.0.4/src/tad_dftd4.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad-dftd4
-Version: 0.0.3
+Version: 0.0.4
 Summary: Torch autodiff DFT-D4 implementation
 Author: "Marvin Friede"
 License: LGPL-3.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -105,24 +105,36 @@
 Install the required dependencies from the conda-forge channel.
 
 .. code::
 
     mamba env create -n torch -f environment.yaml
     mamba activate torch
 
+Install this project with ``pip`` in the environment
+
+.. code::
+
+    pip install .
+
+The following dependencies are required
+
+- `numpy <https://numpy.org/>`__
+- `torch <https://pytorch.org/>`__
+- `pytest <https://docs.pytest.org/>`__ (tests only)
+
 Development
 -----------
 
 For development, additionally install the following tools in your environment.
 
 .. code::
 
     mamba install black covdefaults coverage mypy pre-commit pylint tox
 
-With pip, add the option ``-e`` and the development dependencies for installing in development mode.
+With pip, add the option ``-e`` for installing in development mode, and add ``[dev]`` for the development dependencies
 
 .. code::
 
     pip install -e .[dev]
 
 The pre-commit hooks are initialized by running the following command in the root of the repository.
 
@@ -132,24 +144,24 @@
 
 For testing all Python environments, simply run `tox`.
 
 .. code::
 
     tox
 
-Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional _posargs_.
+Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional *posargs*.
 
 .. code::
 
     tox -- test
 
 Examples
 --------
 
-The following example shows how to calculate the DFT-D3 dispersion energy for a single structure.
+The following example shows how to calculate the DFT-D4 dispersion energy for a single structure.
 
 .. code:: python
 
     import torch
     import tad_dftd4 as d4
 
     numbers = d4.utils.to_number(symbols="C C C C N C S H H H H H".split())
```

### Comparing `tad_dftd4-0.0.3/src/tad_dftd4.egg-info/SOURCES.txt` & `tad_dftd4-0.0.4/src/tad_dftd4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/__init__.py` & `tad_dftd4-0.0.4/test/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/conftest.py` & `tad_dftd4-0.0.4/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/molecules.py` & `tad_dftd4-0.0.4/test/molecules.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_charge/__init__.py` & `tad_dftd4-0.0.4/test/test_charge/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_charge/samples.py` & `tad_dftd4-0.0.4/test/test_charge/samples.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_charge/test_charges.py` & `tad_dftd4-0.0.4/test/test_charge/test_charges.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_charge/test_general.py` & `tad_dftd4-0.0.4/test/test_charge/test_general.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_charge/test_grad.py` & `tad_dftd4-0.0.4/test/test_charge/test_grad.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_cutoff/__init__.py` & `tad_dftd4-0.0.4/test/test_cutoff/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_cutoff/test_general.py` & `tad_dftd4-0.0.4/test/test_cutoff/test_general.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_cutoff/test_types.py` & `tad_dftd4-0.0.4/test/test_cutoff/test_types.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_disp/__init__.py` & `tad_dftd4-0.0.4/test/test_disp/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_disp/samples.py` & `tad_dftd4-0.0.4/test/test_disp/samples.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_disp/test_atm.py` & `tad_dftd4-0.0.4/test/test_disp/test_atm.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_disp/test_full.py` & `tad_dftd4-0.0.4/test/test_disp/test_full.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_disp/test_general.py` & `tad_dftd4-0.0.4/test/test_disp/test_general.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_disp/test_grad.py` & `tad_dftd4-0.0.4/test/test_disp/test_grad.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_disp/test_twobody.py` & `tad_dftd4-0.0.4/test/test_disp/test_twobody.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_model/__init__.py` & `tad_dftd4-0.0.4/test/test_model/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_model/samples.py` & `tad_dftd4-0.0.4/test/test_model/samples.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_model/test_c6.py` & `tad_dftd4-0.0.4/test/test_model/test_c6.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_model/test_general.py` & `tad_dftd4-0.0.4/test/test_model/test_general.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_model/test_model.py` & `tad_dftd4-0.0.4/test/test_model/test_model.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_model/test_weights.py` & `tad_dftd4-0.0.4/test/test_model/test_weights.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_ncoord/__init__.py` & `tad_dftd4-0.0.4/test/test_ncoord/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_ncoord/samples.py` & `tad_dftd4-0.0.4/test/test_ncoord/samples.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_ncoord/test_cn_d4.py` & `tad_dftd4-0.0.4/test/test_ncoord/test_cn_d4.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_ncoord/test_cn_eeq.py` & `tad_dftd4-0.0.4/test/test_ncoord/test_cn_eeq.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_ncoord/test_general.py` & `tad_dftd4-0.0.4/test/test_ncoord/test_general.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_ncoord/test_grad.py` & `tad_dftd4-0.0.4/test/test_ncoord/test_grad.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_utils/__init__.py` & `tad_dftd4-0.0.4/test/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_utils/test_pack.py` & `tad_dftd4-0.0.4/test/test_utils/test_pack.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/test_utils/test_real.py` & `tad_dftd4-0.0.4/test/test_utils/test_real.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/test/utils.py` & `tad_dftd4-0.0.4/test/utils.py`

 * *Files identical despite different names*

### Comparing `tad_dftd4-0.0.3/tox.ini` & `tad_dftd4-0.0.4/tox.ini`

 * *Files identical despite different names*

