# Comparing `tmp/message_ix-3.6.0.tar.gz` & `tmp/message_ix-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "message_ix-3.6.0.tar", last modified: Thu Aug 18 07:17:33 2022, max compression
+gzip compressed data, was "message_ix-3.7.0.tar", last modified: Wed May 17 10:01:04 2023, max compression
```

## Comparing `message_ix-3.6.0.tar` & `message_ix-3.7.0.tar`

### file list

```diff
@@ -1,235 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.613180 message_ix-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-08-18 07:17:26.000000 message_ix-3.6.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     4758 2022-08-18 07:17:26.000000 message_ix-3.6.0/CONTRIBUTOR_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-18 07:17:26.000000 message_ix-3.6.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)    12536 2022-08-18 07:17:26.000000 message_ix-3.6.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-18 07:17:26.000000 message_ix-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-18 07:17:26.000000 message_ix-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-08-18 07:17:26.000000 message_ix-3.6.0/NOTICE.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5474 2022-08-18 07:17:33.613180 message_ix-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4207 2022-08-18 07:17:26.000000 message_ix-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    19498 2022-08-18 07:17:26.000000 message_ix-3.6.0/RELEASE_NOTES.rst
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-08-18 07:17:26.000000 message_ix-3.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.589180 message_ix-3.6.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.589180 message_ix-3.6.0/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    56426 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/combined-logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)    46251 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/iiasa-logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (121)   287453 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/ix_components.png
--rw-r--r--   0 runner    (1001) docker     (121)    63183 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/ix_features.svg
--rw-r--r--   0 runner    (1001) docker     (121)    29607 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/messageix-community-logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (121)    29611 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/messageix-community-logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6603 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/messageix-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (121)    20070 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/messageix-logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (121)    20238 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/messageix-logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    35766 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/storage.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.589180 message_ix-3.6.0/doc/_static/usage_figures/
--rw-r--r--   0 runner    (1001) docker     (121)   212371 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/usage_figures/1-s2.0-S2210670721005333-gr19_lrg.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    28288 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/usage_figures/10.1016-j.scs.2021.103257.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     7406 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/usage_figures/10.1038-s41560-018-0172-6.webp
--rw-r--r--   0 runner    (1001) docker     (121)    10624 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/usage_figures/10.1038-s41560-018-0179-z.webp
--rw-r--r--   0 runner    (1001) docker     (121)   285235 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/usage_figures/10.3390-en12081483.png
--rw-r--r--   0 runner    (1001) docker     (121)    27712 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/_static/usage_figures/41560_2021_904.webp
--rw-r--r--   0 runner    (1001) docker     (121)     8214 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.593180 message_ix-3.6.0/doc/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/contrib/cla.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7147 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/contrib/release.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4070 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/contrib/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/contrib/version.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.593180 message_ix-3.6.0/doc/contrib/video/
--rw-r--r--   0 runner    (1001) docker     (121)    12950 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/contrib/video/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/contrib/video.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12617 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/debugging.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/efficiency.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4392 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/framework.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4724 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8938 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/macro.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/notice.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6907 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/prereqs.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13650 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/references.bib
--rw-r--r--   0 runner    (1001) docker     (121)    11652 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/reporting.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/rmessageix.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2725 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/sharing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7102 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/time.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.593180 message_ix-3.6.0/doc/tools/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/tools/add_year.rst
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5410 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-18 07:17:26.000000 message_ix-3.6.0/doc/whatsnew.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.593180 message_ix-3.6.0/message_ix/
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5174 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    27154 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    24087 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/macro.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.593180 message_ix-3.6.0/message_ix/model/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.593180 message_ix-3.6.0/message_ix/model/MACRO/
--rw-r--r--   0 runner    (1001) docker     (121)     6008 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MACRO/macro_calibration.gms
--rwxr-xr-x   0 runner    (1001) docker     (121)    20309 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MACRO/macro_core.gms
--rwxr-xr-x   0 runner    (1001) docker     (121)    13933 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MACRO/macro_data_load.gms
--rwxr-xr-x   0 runner    (1001) docker     (121)      285 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MACRO/macro_reporting.gms
--rwxr-xr-x   0 runner    (1001) docker     (121)     3896 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MACRO/macro_solve.gms
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MACRO_run.gms
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.593180 message_ix-3.6.0/message_ix/model/MESSAGE/
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/auxiliary_settings.gms
--rw-r--r--   0 runner    (1001) docker     (121)    13932 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/data_load.gms
--rw-r--r--   0 runner    (1001) docker     (121)   118055 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/model_core.gms
--rw-r--r--   0 runner    (1001) docker     (121)     5244 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/model_setup.gms
--rw-r--r--   0 runner    (1001) docker     (121)     9385 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/model_solve.gms
--rw-r--r--   0 runner    (1001) docker     (121)    42901 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/parameter_def.gms
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/reporting.gms
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/reporting_for_MACRO.gms
--rw-r--r--   0 runner    (1001) docker     (121)     9803 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/scaling_investment_costs.gms
--rw-r--r--   0 runner    (1001) docker     (121)    26255 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/sets_maps_def.gms
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE/version_check.gms
--rw-r--r--   0 runner    (1001) docker     (121)    16678 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE-MACRO_run.gms
--rw-r--r--   0 runner    (1001) docker     (121)     5656 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE_master.gms
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE_project.gpr
--rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/MESSAGE_run.gms
--rwxr-xr-x   0 runner    (1001) docker     (121)       19 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/conopt.opt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.593180 message_ix-3.6.0/message_ix/model/data/
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.597180 message_ix-3.6.0/message_ix/model/includes/
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/includes/aux_computation_time.gms
--rw-r--r--   0 runner    (1001) docker     (121)     7776 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/includes/period_parameter_assignment.gms
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.597180 message_ix-3.6.0/message_ix/model/output/
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/output/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/model/version.gms
--rw-r--r--   0 runner    (1001) docker     (121)    18866 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/models.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.597180 message_ix-3.6.0/message_ix/reporting/
--rw-r--r--   0 runner    (1001) docker     (121)     8963 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4859 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/reporting/computations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/reporting/pyam.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.597180 message_ix-3.6.0/message_ix/testing/
--rw-r--r--   0 runner    (1001) docker     (121)    24077 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5283 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/testing/nightly.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.597180 message_ix-3.6.0/message_ix/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.601179 message_ix-3.6.0/message_ix/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)  1474560 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/data/legacy.lobs
--rw-r--r--   0 runner    (1001) docker     (121)    97428 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/data/legacy.script
--rw-r--r--   0 runner    (1001) docker     (121)    22589 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/data/multiregion_macro_input.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/data/report-pyam-write.csv
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/data/scenarios.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/data/test_core.R
--rw-r--r--   0 runner    (1001) docker     (121)    23762 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/data/westeros_macro_input.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.601179 message_ix-3.6.0/message_ix/tests/reporting/
--rw-r--r--   0 runner    (1001) docker     (121)     3921 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/reporting/test_computations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    16949 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3743 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_feature_addon.py
--rw-r--r--   0 runner    (1001) docker     (121)    11093 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_feature_bound_activity_shares.py
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_feature_bound_emission.py
--rw-r--r--   0 runner    (1001) docker     (121)     5246 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_feature_capacity_factor.py
--rw-r--r--   0 runner    (1001) docker     (121)     9406 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_feature_duration_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_feature_price_commodity.py
--rw-r--r--   0 runner    (1001) docker     (121)     7981 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_feature_price_emission.py
--rw-r--r--   0 runner    (1001) docker     (121)    10261 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_feature_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)    10058 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_feature_temporal_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     8205 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_feature_vintage_and_active_years.py
--rw-r--r--   0 runner    (1001) docker     (121)     4960 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_legacy_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    10560 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_macro.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_nightly.py
--rw-r--r--   0 runner    (1001) docker     (121)     8471 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_reporting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_soft_constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.601179 message_ix-3.6.0/message_ix/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (121)     4404 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/tools/test_add_year.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.601179 message_ix-3.6.0/message_ix/tests/util/
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/util/test_sphinx_gams.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tests/util/test_tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.601179 message_ix-3.6.0/message_ix/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.601179 message_ix-3.6.0/message_ix/tools/add_year/
--rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tools/add_year/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    36637 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tools/add_year/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6809 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/tools/add_year/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.601179 message_ix-3.6.0/message_ix/util/
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/util/sphinx_gams.py
--rw-r--r--   0 runner    (1001) docker     (121)     3479 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/util/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-18 07:17:26.000000 message_ix-3.6.0/message_ix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.593180 message_ix-3.6.0/message_ix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5474 2022-08-18 07:17:33.000000 message_ix-3.6.0/message_ix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7672 2022-08-18 07:17:33.000000 message_ix-3.6.0/message_ix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 07:17:33.000000 message_ix-3.6.0/message_ix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-08-18 07:17:33.000000 message_ix-3.6.0/message_ix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-08-18 07:17:33.000000 message_ix-3.6.0/message_ix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-18 07:17:33.000000 message_ix-3.6.0/message_ix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 07:17:33.000000 message_ix-3.6.0/message_ix.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-08-18 07:17:26.000000 message_ix-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-08-18 07:17:33.613180 message_ix-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-08-18 07:17:26.000000 message_ix-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.601179 message_ix-3.6.0/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.601179 message_ix-3.6.0/tutorial/Austrian_energy_system/
--rw-r--r--   0 runner    (1001) docker     (121)    24737 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/Austrian_energy_system/R_austria.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3255 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/Austrian_energy_system/R_austria_load_scenario.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    27307 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/Austrian_energy_system/austria.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   262519 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/Austrian_energy_system/austria.png
--rw-r--r--   0 runner    (1001) docker     (121)     5584 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/Austrian_energy_system/austria_load_scenario.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  1083468 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/Austrian_energy_system/austria_multiple_policies-answers.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     8723 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/Austrian_energy_system/austria_multiple_policies.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     6481 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/Austrian_energy_system/austria_single_policy.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     7770 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.605180 message_ix-3.6.0/tutorial/westeros/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:17:33.613180 message_ix-3.6.0/tutorial/westeros/_static/
--rw-r--r--   0 runner    (1001) docker     (121)   366425 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/addon_technologies_res.png
--rw-r--r--   0 runner    (1001) docker     (121)   352728 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/baseline_res.png
--rw-r--r--   0 runner    (1001) docker     (121)    61042 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/cf_wind.png
--rw-r--r--   0 runner    (1001) docker     (121)   466546 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/doc_page.png
--rw-r--r--   0 runner    (1001) docker     (121)     9643 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/firm-capacity.png
--rw-r--r--   0 runner    (1001) docker     (121)    36988 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/firm-capacity.pptx
--rw-r--r--   0 runner    (1001) docker     (121)   355057 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/fossil_resource_res.png
--rw-r--r--   0 runner    (1001) docker     (121)    16072 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/historical_new_capacity_and_total_installed_capacity.png
--rw-r--r--   0 runner    (1001) docker     (121)    40818 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/historical_new_capacity_and_total_installed_capacity.pptx
--rw-r--r--   0 runner    (1001) docker     (121)   356843 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/historical_new_capacity_res.png
--rw-r--r--   0 runner    (1001) docker     (121)    28746 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/historical_new_capacity_use_in_scenarios.png
--rw-r--r--   0 runner    (1001) docker     (121)    23332 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/historical_new_capacity_use_in_scenarios.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    76122 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/load_seasons.png
--rw-r--r--   0 runner    (1001) docker     (121)   378859 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/message_ixmp.png
--rw-r--r--   0 runner    (1001) docker     (121)   355585 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/renewable_resource_res.png
--rw-r--r--   0 runner    (1001) docker     (121)   371927 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/renewable_resource_res_exercise.png
--rw-r--r--   0 runner    (1001) docker     (121)    15383 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/soft-constraint.PNG
--rw-r--r--   0 runner    (1001) docker     (121)   126599 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/westeroes_tax_emission_soft_constraint_figures.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (121)    88069 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/westeros.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   251945 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow.pptx
--rw-r--r--   0 runner    (1001) docker     (121)   127178 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow_part1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   158392 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow_part2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     8525 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/westeros_renewable_resource_potentials.png
--rw-r--r--   0 runner    (1001) docker     (121)    41058 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/westeros_renewable_resource_potentials.pptx
--rw-r--r--   0 runner    (1001) docker     (121)   174345 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/_static/westeros_res.pptx
--rw-r--r--   0 runner    (1001) docker     (121)    22811 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_addon_technologies.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    44167 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9550 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_baseline_demand.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    16519 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_baseline_technology_basic.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)     9559 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_baseline_technology_constraint.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    12119 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_baseline_technology_economic.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    10271 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_baseline_technology_historic.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)     8432 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_baseline_using_xlsx_import_part1.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    15985 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_baseline_using_xlsx_import_part2.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     7278 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_emissions_bounds.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9318 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_emissions_taxes.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    12584 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_firm_capacity.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    14686 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_flexible_generation.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    14581 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_fossil_resource.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    33556 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_historical_new_capacity.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    16709 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_renewable_resource.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    35533 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_report.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    20126 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_seasonality.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    13570 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_share_constraint.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9237 2022-08-18 07:17:26.000000 message_ix-3.6.0/tutorial/westeros/westeros_soft_constraints.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.406697 message_ix-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-17 10:00:42.000000 message_ix-3.7.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-17 10:00:42.000000 message_ix-3.7.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-17 10:00:42.000000 message_ix-3.7.0/CONTRIBUTOR_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-17 10:00:42.000000 message_ix-3.7.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-05-17 10:00:42.000000 message_ix-3.7.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 10:00:42.000000 message_ix-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-17 10:00:42.000000 message_ix-3.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-17 10:00:42.000000 message_ix-3.7.0/NOTICE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-17 10:01:04.406697 message_ix-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-17 10:00:42.000000 message_ix-3.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22877 2023-05-17 10:00:42.000000 message_ix-3.7.0/RELEASE_NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-17 10:00:42.000000 message_ix-3.7.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.370695 message_ix-3.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.374696 message_ix-3.7.0/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    56426 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/combined-logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    46251 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/iiasa-logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   287453 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/ix_components.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63183 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/ix_features.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29607 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/messageix-community-logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29611 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/messageix-community-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/messageix-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/messageix-logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/messageix-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35766 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/storage.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.374696 message_ix-3.7.0/doc/_static/usage_figures/
+-rw-r--r--   0 runner    (1001) docker     (123)   212371 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/usage_figures/1-s2.0-S2210670721005333-gr19_lrg.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    83467 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/usage_figures/10.1016-j.est.2022.104587.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/usage_figures/10.1016-j.scs.2021.103257.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/usage_figures/10.1038-s41560-018-0172-6.webp
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/usage_figures/10.1038-s41560-018-0179-z.webp
+-rw-r--r--   0 runner    (1001) docker     (123)   285235 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/usage_figures/10.3390-en12081483.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/_static/usage_figures/41560_2021_904.webp
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.374696 message_ix-3.7.0/doc/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/contrib/cla.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/contrib/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/contrib/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/contrib/version.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.374696 message_ix-3.7.0/doc/contrib/video/
+-rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/contrib/video/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/contrib/video.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/debugging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/efficiency.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/framework.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/macro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/notice.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/prereqs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    11652 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/reporting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/rmessageix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/sharing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/time.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.374696 message_ix-3.7.0/doc/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/tools/add_year.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 10:00:42.000000 message_ix-3.7.0/doc/whatsnew.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.374696 message_ix-3.7.0/message_ix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27221 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24209 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/macro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.378696 message_ix-3.7.0/message_ix/model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.378696 message_ix-3.7.0/message_ix/model/MACRO/
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MACRO/macro_calibration.gms
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20311 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MACRO/macro_core.gms
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13933 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MACRO/macro_data_load.gms
+-rwxr-xr-x   0 runner    (1001) docker     (123)      285 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MACRO/macro_reporting.gms
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3896 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MACRO/macro_solve.gms
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MACRO_run.gms
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.378696 message_ix-3.7.0/message_ix/model/MESSAGE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/auxiliary_settings.gms
+-rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/data_load.gms
+-rw-r--r--   0 runner    (1001) docker     (123)   121744 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/model_core.gms
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/model_setup.gms
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/model_solve.gms
+-rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/parameter_def.gms
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/reporting.gms
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/reporting_for_MACRO.gms
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/scaling_investment_costs.gms
+-rw-r--r--   0 runner    (1001) docker     (123)    26306 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/sets_maps_def.gms
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE/version_check.gms
+-rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE-MACRO_run.gms
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE_master.gms
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE_project.gpr
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/MESSAGE_run.gms
+-rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/conopt.opt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.382696 message_ix-3.7.0/message_ix/model/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.382696 message_ix-3.7.0/message_ix/model/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/includes/aux_computation_time.gms
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/includes/period_parameter_assignment.gms
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.382696 message_ix-3.7.0/message_ix/model/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/output/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/model/version.gms
+-rw-r--r--   0 runner    (1001) docker     (123)    21514 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.382696 message_ix-3.7.0/message_ix/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/reporting/computations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/reporting/pyam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.382696 message_ix-3.7.0/message_ix/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)    25653 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/testing/nightly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.386696 message_ix-3.7.0/message_ix/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.386696 message_ix-3.7.0/message_ix/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1474560 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/data/legacy.lobs
+-rw-r--r--   0 runner    (1001) docker     (123)    97428 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/data/legacy.script
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/data/multiregion_macro_input.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/data/report-pyam-write.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/data/scenarios.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/data/test_core.R
+-rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/data/westeros_macro_input.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.386696 message_ix-3.7.0/message_ix/tests/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/reporting/test_computations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_equation_NEW_CAPACITY_CONTRAINT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_feature_addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_feature_bound_activity_shares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_feature_bound_emission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_feature_capacity_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_feature_duration_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_feature_price_commodity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_feature_price_emission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_feature_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_feature_temporal_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_feature_vintage_and_active_years.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_legacy_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_nightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_soft_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.386696 message_ix-3.7.0/message_ix/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/tools/test_add_year.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.386696 message_ix-3.7.0/message_ix/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/util/test_sphinx_gams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tests/util/test_tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.386696 message_ix-3.7.0/message_ix/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.390697 message_ix-3.7.0/message_ix/tools/add_year/
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tools/add_year/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36703 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tools/add_year/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/tools/add_year/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.390697 message_ix-3.7.0/message_ix/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/util/sphinx_gams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/util/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-17 10:00:42.000000 message_ix-3.7.0/message_ix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.378696 message_ix-3.7.0/message_ix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-17 10:01:04.000000 message_ix-3.7.0/message_ix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-17 10:01:04.000000 message_ix-3.7.0/message_ix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:01:04.000000 message_ix-3.7.0/message_ix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 10:01:04.000000 message_ix-3.7.0/message_ix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-17 10:01:04.000000 message_ix-3.7.0/message_ix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 10:01:04.000000 message_ix-3.7.0/message_ix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-17 10:00:42.000000 message_ix-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:01:04.406697 message_ix-3.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.390697 message_ix-3.7.0/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.390697 message_ix-3.7.0/tutorial/Austrian_energy_system/
+-rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/Austrian_energy_system/R_austria.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/Austrian_energy_system/R_austria_load_scenario.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/Austrian_energy_system/austria.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   262519 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/Austrian_energy_system/austria.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/Austrian_energy_system/austria_load_scenario.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   814998 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/Austrian_energy_system/austria_multiple_policies-answers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/Austrian_energy_system/austria_multiple_policies.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/Austrian_energy_system/austria_single_policy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.394697 message_ix-3.7.0/tutorial/westeros/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:01:04.406697 message_ix-3.7.0/tutorial/westeros/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   366425 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/addon_technologies_res.png
+-rw-r--r--   0 runner    (1001) docker     (123)   352728 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/baseline_res.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/bilateral.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)    61042 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/cf_wind.png
+-rw-r--r--   0 runner    (1001) docker     (123)   466546 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/doc_page.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37675 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/external.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/firm-capacity.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36988 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/firm-capacity.pptx
+-rw-r--r--   0 runner    (1001) docker     (123)   355057 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/fossil_resource_res.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/historical_new_capacity_and_total_installed_capacity.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40818 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/historical_new_capacity_and_total_installed_capacity.pptx
+-rw-r--r--   0 runner    (1001) docker     (123)   356843 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/historical_new_capacity_res.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28746 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/historical_new_capacity_use_in_scenarios.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23332 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/historical_new_capacity_use_in_scenarios.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    26522 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/hub.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)    76122 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/load_seasons.png
+-rw-r--r--   0 runner    (1001) docker     (123)   378859 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/message_ixmp.png
+-rw-r--r--   0 runner    (1001) docker     (123)   355585 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/renewable_resource_res.png
+-rw-r--r--   0 runner    (1001) docker     (123)   371927 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/renewable_resource_res_exercise.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/soft-constraint.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   126599 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/westeroes_tax_emission_soft_constraint_figures.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (123)    88069 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/westeros.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   251945 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow.pptx
+-rw-r--r--   0 runner    (1001) docker     (123)   127178 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow_part1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   158392 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow_part2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/westeros_renewable_resource_potentials.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41058 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/westeros_renewable_resource_potentials.pptx
+-rw-r--r--   0 runner    (1001) docker     (123)   174345 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/_static/westeros_res.pptx
+-rw-r--r--   0 runner    (1001) docker     (123)    23200 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_addon_technologies.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    44973 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_baseline_demand.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_baseline_technology_basic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_baseline_technology_constraint.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_baseline_technology_economic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_baseline_technology_historic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_baseline_using_xlsx_import_part1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16363 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_baseline_using_xlsx_import_part2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_emissions_bounds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_emissions_taxes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_firm_capacity.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_flexible_generation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_fossil_resource.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33969 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_historical_new_capacity.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    54472 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_multinode.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_renewable_resource.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45858 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_report.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_seasonality.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_share_constraint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-17 10:00:42.000000 message_ix-3.7.0/tutorial/westeros/westeros_soft_constraints.ipynb
```

### Comparing `message_ix-3.6.0/AUTHORS.md` & `message_ix-3.7.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/CONTRIBUTOR_LICENSE.rst` & `message_ix-3.7.0/CONTRIBUTOR_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/INSTALL.rst` & `message_ix-3.7.0/INSTALL.rst`

 * *Files 2% similar despite different names*

```diff
@@ -74,43 +74,46 @@
    If you are a beginner, you may want to watch the video before attempting the installation yourself.
 
    .. raw:: html
 
       <iframe width="690" height="360" src="https://www.youtube.com/embed/QZw-7rIqUJ0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
 
 4. Install Python via either `Miniconda`_ or `Anaconda`_. [1]_
-   We recommend the latest version; currently Python 3.8.
+   We recommend the latest version; currently Python 3.10. [2]_
 
 5. Open a command prompt.
    Windows users should use the “Anaconda Prompt” to avoid issues with permissions and environment variables when installing and using |MESSAGEix|.
    This program is available in the Windows Start menu after installing Anaconda.
 
-6. Configure conda to install :mod:`message_ix` from the conda-forge channel [2]_::
+6. Configure conda to install :mod:`message_ix` from the conda-forge channel [3]_::
 
     $ conda config --prepend channels conda-forge
 
 7. Create a new conda environment and activate it.
    This step is **required** if using Anaconda, but *optional* if using Miniconda.
    This example uses the name ``message_env``, but you can use any name of your choice::
 
     $ conda create --name message_env
     $ conda activate message_env
 
-8. Install the ``message-ix`` package into the current environment (either e.g. ``message_env``, or another name from step 7) [3]_::
+8. Install the ``message-ix`` package into the current environment (either e.g. ``message_env``, or another name from step 7) [4]_::
 
     $ conda install message-ix
 
 Again: at this point, installation is complete.
 You do not need to complete the steps in “Using ``pip``” or “From source”.
 Go to the section `Check that installation was successful`_.
 
 .. [1] See the `conda glossary`_ for the differences between Anaconda and Miniconda, and the definitions of the terms ‘channel’ and ‘environment’ here.
-.. [2] The ‘$’ character at the start of these lines indicates that the command text should be entered in the terminal or prompt, depending on the operating system.
-       Do not retype the ‘$’ character itself.
-.. [3] Notice that conda uses the hyphen (‘-’) in package names, different from the underscore (‘_’) used in Python when importing the package.
+.. [2] On newer macOS systems with "Apple M1" processors: the Miniconda or Anaconda installers provided for M1 lead to errors in ixmp.
+   Instead, we recommend to use the macOS installers for "x86_64" processors on these systems.
+   See also `ixmp issue 473<https://github.com/iiasa/ixmp/issues/473>`_.
+.. [3] The ‘$’ character at the start of these lines indicates that the command text should be entered in the terminal or prompt, depending on the operating system.
+   Do not retype the ‘$’ character itself.
+.. [4] Notice that conda uses the hyphen (‘-’) in package names, different from the underscore (‘_’) used in Python when importing the package.
 .. note:: When using Anaconda (not Miniconda), steps (5) through (8) can also be performed using the graphical Anaconda Navigator.
    See the `Anaconda Navigator documentation`_ for how to perform the various steps.
 
 
 Using ``pip``
 -------------
```

### Comparing `message_ix-3.6.0/LICENSE` & `message_ix-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/NOTICE.rst` & `message_ix-3.7.0/NOTICE.rst`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 The aim of this request is to ensure good scientific practice and collaborative development of the platform.
 
 1. Understand the code license
 ==============================
 
 Use the most recent version of |MESSAGEix| from the Github repository.
 Specify clearly which version (e.g. release tag, such as ``v1.1.0``, or commit hash, such as ``26cc08f``) you have used, and whether you have made any modifications to the code.
+To retrieve this information from the command line, use ``git describe --tags``, which will show you the version, number of commits since then, and the hash of your current commit.
+Note that the commit hash does not include the preceeding ``-g``.
 
 Read and understand the file ``LICENSE``; in particular, clause 7 (“Disclaimer of Warranty”), which states:
 
     Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
 
 .. _notice-cite:
 
@@ -27,14 +29,17 @@
 
   | Daniel Huppmann, Matthew Gidden, Oliver Fricko, Peter Kolp, Clara Orthofer, Michael Pimmer, Nikolay Kushin, Adriano Vinca, Alessio Mastrucci, Keywan Riahi, and Volker Krey.
   | "The MESSAGEix Integrated Assessment Model and the ix modeling platform".
   | *Environmental Modelling & Software* 112:143-156, 2019.
   | doi: `10.1016/j.envsoft.2018.11.012`_
   | electronic pre-print available at `pure.iiasa.ac.at/15157/`_.
 
+You should also cite the software project itself. The data for citing both the manuscript and the software can be found in the citation file :file:`CITATION.cff`.
+You can use `the official cff tools <https://github.com/citation-file-format/citation-file-format#tools-to-work-with-citationcff-files-wrench>`__ to export the data to BibTeX and other formats.
+
 In addition, you may:
 
 - **Cite the code via Zenodo**.
   The DOI `10.5281/zenodo.4005684 <https://doi.org/10.5281/zenodo.4005684>`_ represents *all* versions of the :mod:`message_ix` code, and will always resolve to the latest version.
   At that page, you can also choose a different DOI in order to cite one specific version; for instance, `10.5281/zenodo.4005685 <https://doi.org/10.5281/zenodo.4005685>`_ to cite v3.1.0.
   Zenodo also provides citation export in BibTeX and other formats.
 - Include a link, e.g. in a footnote, to the online documentation at https://docs.messageix.org.
```

### Comparing `message_ix-3.6.0/PKG-INFO` & `message_ix-3.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: message_ix
-Version: 3.6.0
-Summary: the MESSAGEix integrated assessment model
-Home-page: http://github.com/iiasa/message_ix
+Version: 3.7.0
+Summary: The MESSAGEix integrated assessment model framework
 Author: IIASA Energy, Climate, and Environment (ECE) Program
-Author-email: message_ix@iiasa.ac.at
-License: Apache
-Project-URL: Documentation, https://docs.messageix.org/
+Maintainer-email: Paul Natsuo Kishimoto <mail@paul.kishimoto.name>, Fridolin Glatter <glatter@iiasa.ac.at>
+Project-URL: homepage, https://github.com/iiasa/message_ix
+Project-URL: repository, https://github.com/iiasa/message_ix
+Project-URL: documentation, https://docs.messageix.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -19,17 +19,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: R
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
-Provides-Extra: report
 Provides-Extra: docs
 Provides-Extra: tutorial
+Provides-Extra: report
 Provides-Extra: tests
 License-File: LICENSE
 License-File: NOTICE.rst
 License-File: AUTHORS.md
 
 # The MESSAGEix framework
 
@@ -75,13 +75,13 @@
 - Documentation for the ‘latest’ or ‘stable’ release is shown by default.
 - Use the chooser to access the [‘latest’ version](https://docs.messageix.org/en/latest/), corresponding to the ``main`` branch and including the latest development code; or to access docs for a specific release, e.g. `v3.2.0`.
 - For offline use, the documentation can be built from the source code.
   See the file [`doc/README.rst`](doc/README.rst)
 
 ## License
 
-Copyright © 2018–2022 IIASA Energy, Climate, and Environment (ECE) Program
+Copyright © 2018–2023 IIASA Energy, Climate, and Environment (ECE) Program
 
 The MESSAGEix framework is licensed under the Apache License, Version 2.0 (the "License"); you may not use the files in this repository except in compliance with the License. You may obtain a copy of the License in [`LICENSE`](LICENSE) or at <http://www.apache.org/licenses/LICENSE-2.0>.
 
 In addition and per good scientific practice, you **must** cite the appropriate publications when you use MESSAGEix in scientific work.
 Again, see [‘User guidelines and notice’](https://docs.messageix.org/en/stable/notice.html) or the file [`NOTICE.rst`](NOTICE.rst).
```

### Comparing `message_ix-3.6.0/README.md` & `message_ix-3.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,13 +42,13 @@
 - Documentation for the ‘latest’ or ‘stable’ release is shown by default.
 - Use the chooser to access the [‘latest’ version](https://docs.messageix.org/en/latest/), corresponding to the ``main`` branch and including the latest development code; or to access docs for a specific release, e.g. `v3.2.0`.
 - For offline use, the documentation can be built from the source code.
   See the file [`doc/README.rst`](doc/README.rst)
 
 ## License
 
-Copyright © 2018–2022 IIASA Energy, Climate, and Environment (ECE) Program
+Copyright © 2018–2023 IIASA Energy, Climate, and Environment (ECE) Program
 
 The MESSAGEix framework is licensed under the Apache License, Version 2.0 (the "License"); you may not use the files in this repository except in compliance with the License. You may obtain a copy of the License in [`LICENSE`](LICENSE) or at <http://www.apache.org/licenses/LICENSE-2.0>.
 
 In addition and per good scientific practice, you **must** cite the appropriate publications when you use MESSAGEix in scientific work.
 Again, see [‘User guidelines and notice’](https://docs.messageix.org/en/stable/notice.html) or the file [`NOTICE.rst`](NOTICE.rst).
```

### Comparing `message_ix-3.6.0/RELEASE_NOTES.rst` & `message_ix-3.7.0/RELEASE_NOTES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,70 @@
 .. Next release
 .. ============
 
 .. All changes
 .. -----------
 
+.. _v3.7.0:
+
+v3.7.0 (2023-05-16)
+===================
+
+Migration notes
+---------------
+
+- The default `lpmethod` has been changed from "Dual Simplex" (`lpmethod=2`) to "Barrier" (`lpmethod=4`).
+  NOTE: this may result in changes to the solution.
+  In order to use the previous default `lpmethod`, the user-specific default setting can be set through the user's ixmp configuration file.
+  Alternatively, the `lpmethod` can be specified directly as an argument when solving a scenario.
+  Both of these configuration methods are further explained :meth:`here <message_ix.models.GAMSModel>`.
+
+- The dimensionality of one set and two parameters (``map_tec_storage``, ``storage_initial``, and ``storage_self_discharge``) are extended to allow repesentation of the mode of operation of storage technologies and the temporal level of storage containers.
+  If these items are already populated with data in a Scenario, this data will be incompatible with the MESSAGE GAMS implementation in this release; a :class:`UserWarning` will be emitted when the :class:`.Scenario` is instantiated, and :meth:`~.message_ix.Scenario.solve` will raise a :class:`ValueError`.
+  (If these items are empty, their dimensions will be updated automatically.
+  New Scenarios are unaffected.)
+
+  Users must update data for these items, specifically:
+
+  ==========================  ============================================
+  Existing parameter or set   Dimension(s) to add
+  ==========================  ============================================
+  ``map_tec_storage``         ``mode``, ``storage_mode``, ``lvl_temporal``
+  ``storage_initial``         ``mode``
+  ``storage_self_discharge``  ``mode``
+  ==========================  ============================================
+
+  For the set ``map_tec_storage``, values for the new dimensions represent, respectively, the ``mode`` of operation for charge/discharge technologies, and the ``storage_mode`` and ``lvl_temporal`` for the corresponding storage device.
+  For the two parameters, :func:`.expand_dims` is provided to help:
+
+  .. code-block:: python
+
+      from message_ix import Scenario
+      from message_ix.util import expand_dims
+
+      scen, platform = Scenario.from_url("…")
+
+      # Re-use the existing data in `scen`, adding the `mode` dimension
+      expand_dims(scen, "storage_initial", mode="an existing mode")
+
+
+All changes
+-----------
+
+- Add a tutorial for Westeros multi-node and different trade possibilities (:pull:`683`).
+- Add additional oscillation detection mechanism for macro iterations (:pull:`645`, :pull:`676`)
+- Adjust default `lpmethod` from "Dual Simplex" (2) to "Barrier" (4); do NOT remove `cplex.opt` file(s) after solving workflow completes (:pull:`657`).
+- Adjust :meth:`.Scenario.add_macro` calculations for pandas 1.5.0 (:pull:`656`).
+- Ensure `levelized_cost` are also calculated for technologies with only variable costs (:pull:`653`).
+- Correct calculation of `COST_NODAL_NET` for standalone MESSAGE (:pull:`648`)
+- Account for difference in period-length in equations `NEW_CAPACITY_CONSTRAINT_LO` and `NEW_CAPACITY_CONSTRAINT_UP` (:pull:`654`)
+- Extend functionality of storage solutions to include "mode" and temporal level (:pull:`633`)
+- Introduce a citation file :file:`CITATION.cff` with citation information (:pull:`695`).
+- Correct GAMS for the assignment of "capacity_factor" at "year" (:pull:`705`).
+
 .. _v3.6.0:
 
 v3.6.0 (2022-08-17)
 ===================
 
 Migration notes
 ---------------
@@ -21,15 +78,14 @@
      df = scen.vintage_and_active_years().query(f"{scen.y0} <= year_vtg")
 
 - The :ref:`default reports <default-reports>` (tables in IAMC format) available in a :class:`~message_ix.reporting.Reporter` have changed keys to e.g. ``message::default`` with **two** colons.
   Code using e.g. ``message:default`` (one colon) should be updated to use the current keys.
 
   This matches fixed behaviour upstream in :mod:`genno` version 1.12 to avoid unintended confusion with keys like ``A:i``: ``i`` (after the first colon) is the name for the sole dimension of a 1-dimensional quantity, whereas ``default`` in ``message::default`` is a tag.
 
-
 All changes
 -----------
 
 - Adjust keys for IAMC-format reporting nodes (:pull:`628`, :pull:`641`)
 - New reporting computation :func:`.as_message_df` (:pull:`628`).
 - Extend functionality of :meth:`.vintage_and_active_years`; add aliases :meth:`.yv_ya`, :meth:`.ya`, and :attr:`.y0` (:pull:`572`, :pull:`623`).
 - Add scripts and HOWTO for documentation videos (:pull:`396`).
```

### Comparing `message_ix-3.6.0/conftest.py` & `message_ix-3.7.0/conftest.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/Makefile` & `message_ix-3.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/README.rst` & `message_ix-3.7.0/doc/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 
 There are a number of guides out there, e.g. on docutils_.
 
 
 Building the docs on your local machine
 ---------------------------------------
 
-From the command line, run::
+From the command line, run in `doc/`::
 
     make html
 
 You can then view the site by::
 
     cd build
-    python -m SimpleHTTPServer
+    python -m http.server
 
-and pointing your browser at http://localhost:8000/html/
+and pointing your browser at http://0.0.0.0:8000/_build/html/
 
 
 Read the Docs
 -------------
 
 On Read the Docs (RTD), the documentation is built using a command similar to:
```

### Comparing `message_ix-3.6.0/doc/_static/combined-logo-white.svg` & `message_ix-3.7.0/doc/_static/combined-logo-white.svg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/custom.css` & `message_ix-3.7.0/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/iiasa-logo-white.svg` & `message_ix-3.7.0/doc/_static/iiasa-logo-white.svg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/ix_components.png` & `message_ix-3.7.0/doc/_static/ix_components.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/ix_features.svg` & `message_ix-3.7.0/doc/_static/ix_features.svg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/messageix-community-logo-white.svg` & `message_ix-3.7.0/doc/_static/messageix-community-logo-white.svg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/messageix-community-logo.svg` & `message_ix-3.7.0/doc/_static/messageix-community-logo.svg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/messageix-favicon.svg` & `message_ix-3.7.0/doc/_static/messageix-favicon.svg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/messageix-logo-white.svg` & `message_ix-3.7.0/doc/_static/messageix-logo-white.svg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/messageix-logo.svg` & `message_ix-3.7.0/doc/_static/messageix-logo.svg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/storage.png` & `message_ix-3.7.0/doc/_static/storage.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/usage_figures/1-s2.0-S2210670721005333-gr19_lrg.jpg` & `message_ix-3.7.0/doc/_static/usage_figures/1-s2.0-S2210670721005333-gr19_lrg.jpg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/usage_figures/10.1016-j.scs.2021.103257.jpg` & `message_ix-3.7.0/doc/_static/usage_figures/10.1016-j.scs.2021.103257.jpg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/usage_figures/10.1038-s41560-018-0172-6.webp` & `message_ix-3.7.0/doc/_static/usage_figures/10.1038-s41560-018-0172-6.webp`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/usage_figures/10.1038-s41560-018-0179-z.webp` & `message_ix-3.7.0/doc/_static/usage_figures/10.1038-s41560-018-0179-z.webp`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/usage_figures/10.3390-en12081483.png` & `message_ix-3.7.0/doc/_static/usage_figures/10.3390-en12081483.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/_static/usage_figures/41560_2021_904.webp` & `message_ix-3.7.0/doc/_static/usage_figures/41560_2021_904.webp`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/api.rst` & `message_ix-3.7.0/doc/api.rst`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
    MESSAGE
    MACRO
    MESSAGE_MACRO
    GAMSModel
    DEFAULT_CPLEX_OPTIONS
    MESSAGE_ITEMS
+   MACRO_ITEMS
 
 .. autodata:: DEFAULT_CPLEX_OPTIONS
 
    These configure the GAMS CPLEX solver (or another solver, if selected); see `the solver documentation <https://www.gams.com/latest/docs/S_CPLEX.html>`_ for possible values.
 
 .. autoclass:: GAMSModel
    :members:
@@ -190,22 +191,18 @@
         - :obj:`None`
 
 .. autoclass:: MESSAGE
    :members: initialize
    :exclude-members: defaults
    :show-inheritance:
 
-   .. autoattribute:: name
-
 .. autoclass:: MACRO
    :members:
    :show-inheritance:
 
-   .. autoattribute:: name
-
 .. autoclass:: MESSAGE_MACRO
    :members:
    :show-inheritance:
 
    MESSAGE_MACRO solves the MESSAGE and MACRO models iteratively, connecting changes in technology activity and resource demands (from MESSAGE) to changes in final demands and prices (from MACRO).
    This iteration continues until the solution *converges*; i.e. the two models reach a stable point for the values of these parameters.
 
@@ -217,41 +214,37 @@
      This option applies to the same value as `max_adjustment`: the relative change in final demands between two iterations.
      If the absolute relative change is less than `convergence_criterion`, the linked model run is complete.
    - **max_iteration** (:class:`int`, default 50): the maximum number of iterations between the two models.
      If the solution does not converge after this many iterations, the linked model run fails and no valid result is produced.
 
    .. seealso:: :meth:`.Scenario.add_macro`
 
-   .. autoattribute:: name
-
 .. autodata:: MESSAGE_ITEMS
    :annotation: = dict(…)
 
    Keys are the names of items (sets, parameters, variables, and equations); values are :class:`dict` specifying their type and dimensionality, with keys 'ix_type', 'idx_sets', and in some cases 'idx_names'.
    These include all items listed in the MESSAGE mathematical specification, i.e. :ref:`sets_maps_def` and :ref:`parameter_def`.
 
    .. seealso:: :meth:`.MESSAGE.initialize`, :data:`.MACRO_ITEMS`
 
 .. currentmodule:: message_ix.macro
 
 .. autodata:: MACRO_ITEMS
    :annotation: = dict(…)
 
-   All of the items in the MACRO mathematical formulation.
-
    .. seealso:: :data:`.MESSAGE_ITEMS`
 
 
 .. _utils:
 
 Utility methods
 ---------------
 
 .. automodule:: message_ix.util
-   :members: make_df
+   :members: expand_dims, make_df
 
 
 Testing utilities
 -----------------
 
 .. automodule:: message_ix.testing
    :members: make_dantzig, make_westeros
```

### Comparing `message_ix-3.6.0/doc/conf.py` & `message_ix-3.7.0/doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
-from pathlib import Path
+try:
+    from importlib.metadata import version
+except ImportError:  # Python 3.7
+    from importlib_metadata import version
 
-from pkg_resources import get_distribution
+from pathlib import Path
 
 # -- Project information -----------------------------------------------------
 
 project = "MESSAGEix"
-copyright = "2021, IIASA Energy, Climate, and Environment (ECE) Program"
+copyright = "2018–2023, IIASA Energy, Climate, and Environment (ECE) Program"
 author = "MESSAGEix Developers"
 
 # The major project version, used as the replacement for |version|.
-version = get_distribution("message_ix").version
+version = version("message_ix")
 # The full project version, used as the replacement for |release| and e.g. in
 # the HTML templates.
 release = version
 
 
 # -- General configuration ----------------------------------------------------
 
@@ -102,17 +105,17 @@
 # -- Options for sphinx.ext.extlinks ---------------------------------------------------
 
 # Link to "main" blob if a non-release version of the docs is being built; otherwise
 # to the tag for the release
 gh_ref = "main" if ".dev" in version else f"v{version}"
 
 extlinks = {
-    "issue": ("https://github.com/iiasa/message_ix/issue/%s", "#"),
-    "pull": ("https://github.com/iiasa/message_ix/pull/%s", "PR #"),
-    "tut": (f"https://github.com/iiasa/message_ix/blob/{gh_ref}/tutorial/%s", ""),
+    "issue": ("https://github.com/iiasa/message_ix/issue/%s", "#%s"),
+    "pull": ("https://github.com/iiasa/message_ix/pull/%s", "PR #%s"),
+    "tut": (f"https://github.com/iiasa/message_ix/blob/{gh_ref}/tutorial/%s", None),
 }
 
 
 # -- Options for sphinx.ext.intersphinx ---------------------------------------
 
 intersphinx_mapping = {
     "dask": ("https://docs.dask.org/en/stable/", None),
@@ -121,14 +124,15 @@
     # For a local build, uncomment and use the following line with a path to
     # the directory containing built HTML documentation for ixmp:
     # 'ixmp': ('/home/user/path-to-ixmp/doc/build/html', None),
     "message-ix-models": (
         "https://docs.messageix.org/projects/models/en/latest/",
         None,
     ),
+    "message_doc": ("https://docs.messageix.org/projects/global/en/latest/", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable/", None),
     "pint": ("https://pint.readthedocs.io/en/stable/", None),
     "pyam": ("https://pyam-iamc.readthedocs.io/en/stable/", None),
     "python": ("https://docs.python.org/3/", None),
     "sphinx": ("https://www.sphinx-doc.org/en/master/", None),
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `message_ix-3.6.0/doc/contrib/release.rst` & `message_ix-3.7.0/doc/contrib/release.rst`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
   - Maintainer or Owner on both Github repositories.
   - Maintainer on the
     `conda-forge/ixmp-feedstock <https://github.com/conda-forge/ixmp-feedstock>`__
     and
     `message-ix-feedstock <https://github.com/conda-forge/message-ix-feedstock>`__
     repositories.
-    This means your Github account is listed in the :file:`recipe/meta.yaml`, under the key ``recipe-maintainers:``.
+    This means your Github account is listed in each of them in the :file:`recipe/meta.yaml`, under the key ``recipe-maintainers:``. For an easy way of achieving that, see `the conda-forge docs <https://conda-forge.org/docs/maintainer/updating_pkgs.html#updating-the-maintainer-list>`__.
 
 - In the below:
 
   - ``<version>`` stands for the full version number, e.g. ``1.2.0``.
     Always include all three parts: major, minor, and patch, i.e. ``1.2.0`` and never ``1.2``.
     Look very carefully to see when ``v<version>`` versus ``<version>`` should be used.
   - ``<upstream>`` stands for your local name for the Git remote that is the IIASA Github repository.
@@ -41,18 +41,18 @@
 1. Mark any new deprecations.
    Explicitly state the version when the removal is targeted, so that users can adjust their code.
 
 2. Remove any items targeted for removal in this release.
 
    .. note:: This can be done at any point, and should be done before the release prep begins.
       For instance, a feature marked as deprecated in v2.0 *should* be removed before 3.0 is released.
-      But *may* also be removed from the ``master`` branch *immediately after* 2.0.0 is released.
+      But *may* also be removed from the ``main`` branch *immediately after* 2.0.0 is released.
       This is preferred, because it forces tutorials, user code, etc. to stay ahead of deprecations.
 
-3. (message_ix only) Edit :file:`setup.cfg`, updating the ``install_requires`` line for ixmp as necessary.
+3. (message_ix only) Edit :file:`pyproject.toml`, updating the list ``dependencies`` in the ``project`` section for ixmp as necessary.
 
    Each version of message_ix depends on a minimum version of ixmp.
    message_ix **must not** depend on or use deprecated features of ixmp; it **should** remain compatible with earlier versions of ixmp, where possible.
 
 **Check continuous integration.**
 Any failures in (4) or (5) must be corrected before releasing.
 
@@ -68,20 +68,20 @@
 
     $ git checkout -v release/X.Y.Z
 
 2. Edit :file:`RELEASE_NOTES.rst`:
 
    - Comment the heading "Next release", and insert below it:
 
-     - A commented "All changes" sub-heading (``---``).
-     - A ReST anchor with the version number.
+     - A commented "All changes" sub-heading (``---``)
+     - A ReST anchor with the version number
      - Another heading (``===``) below it, with the version number and date
 
-   - Add a short text description summarizing the release.
-   - If necessary, add a subsection "Migration notes" explaining to users how to adjust to changes in the release.
+   - Add a short text description summarizing the release
+   - If necessary, add a subsection "Migration notes" explaining to users how to adjust to changes in the release
 
    For example, the top of the file should look like:
 
    .. code-block:: rest
       :caption: Before editing
 
       Next release
@@ -117,15 +117,15 @@
       -----------
 
       - Description of a change (:pull:`9999`).
 
    Build the docs locally to ensure any ReST markup in these additions renders correctly.
 
 3. Make a commit with a message like “Mark v<version> in release notes”.
-4. Tag the release candidate version, i.e. with a ``rcN`` suffix, and push::
+4. Tag the release candidate version, i.e. with a ``rcN`` suffix where ``N`` is a natural number, and push::
 
    $ git tag vX.Y.ZrcN
    $ git push --tags <upstream> release/X.Y.Z
 
 5. Open a PR with the title “Release vX.Y.Z” using this branch.
    Check:
 
@@ -158,14 +158,14 @@
 
 9. Check at https://github.com/iiasa/message_ix/actions/workflows/publish.yaml (or `ixmp <https://github.com/iiasa/ixmp/actions/workflows/publish.yaml>`__) and https://pypi.org/project/message-ix/ (or `ixmp <https://pypi.org/project/ixmp/>`__) that the distributions are published.
 
 10. Update on conda-forge.
     A PR should automatically be opened by a bot after the GitHub release (sometimes this takes from 30 minutes to several hours).
 
     1. Confirm that any new dependencies are added.
-       The minimum versions in :file:`meta.yaml` should match the versions in :file:`setup.cfg`.
+       The minimum versions in :file:`meta.yaml` should match the versions in :file:`pyproject.toml`.
     2. Ensure that tests pass and complete any other checklist items.
     3. Merge the PR.
     4. Check that the new package version appears on conda-forge. This may take up to several hours.
 
-11. Announce the release(s) on our mailing list/Google group and/or on Twitter.
+11. Announce the release(s) on the GitHub Discussions pages and/or on Twitter.
     Copy the text from the What's New page of the built documentation.
```

### Comparing `message_ix-3.6.0/doc/contrib/tutorial.rst` & `message_ix-3.7.0/doc/contrib/tutorial.rst`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 - Description of individual steps:
 
   - A brief explanation of the step.
   - A link to any relevant mathematical documentation.
 
 - Modeling results and visualizations:
 
-  - Model outputs and post-processing calculations in tutorials should demonstrate usage of the :doc:`message_ix.reporting module <reporting>`.
+  - Model outputs and post-processing calculations in tutorials should demonstrate usage of the :doc:`message_ix.reporting module </reporting>`.
   - Plots to depict results should use `pyam <https://github.com/IAMconsortium/pyam/>`_.
   - Include a brief discussion of insights from the results, in line with the learning objectives.
 
 - Exercises: include self-test questions, small activities, and exercises at the end of a tutorial so that users (and instructors, if any) can check their learning.
 
 
 Location
```

### Comparing `message_ix-3.6.0/doc/contrib/version.rst` & `message_ix-3.7.0/doc/contrib/version.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Versions and releases
 *********************
 
 - We use `semantic versioning <https://semver.org>`_.
 
   To paraphrase: a **major** version increment (e.g. from 3.5 to 4.0) means there are *backwards-incompatible* changes to the API or functionality (e.g. code written for version 3.5 may no longer work with 4.0).
-  Major releases always include migration notes in :doc:`whatsnew` to alert users to such changes and suggest how to adjust their code.
+  Major releases always include migration notes in :doc:`/whatsnew` to alert users to such changes and suggest how to adjust their code.
   A **minor** version increment may fix bugs or add new features, but does not change existing functionality.
   Code written for e.g. version 3.5 will continue to work with 3.6.
 
 - Releases of :mod:`ixmp` and :mod:`message_ix` are generally made at the same time, and the version numbers kept synchronized.
 
 - Each version of :mod:`message_ix` has a minimum required version of :mod:`ixmp`.
```

### Comparing `message_ix-3.6.0/doc/contrib/video/install.rst` & `message_ix-3.7.0/doc/contrib/video/install.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/contrib/video.rst` & `message_ix-3.7.0/doc/contrib/video.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/contributing.rst` & `message_ix-3.7.0/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/debugging.rst` & `message_ix-3.7.0/doc/debugging.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/efficiency.rst` & `message_ix-3.7.0/doc/efficiency.rst`

 * *Files 13% similar despite different names*

```diff
@@ -12,59 +12,59 @@
  
 For the implementation of |MESSAGEix|, we opted to formulate the model in an agnostic manner, 
 so that for each technology, the most "appropriate" parametrization can be applied.
 As an additional benefit, we do not need to define an explicit efficiency parameter
 or "main" input and output fuels.  
 
 The recommended approach is illustrated below for multiple examples. 
-The decision variables :math:`CAP\_NEW`, :math:`CAP` and :math:`ACT` as well as all bounds 
+The decision variables :math:`\text{CAP_NEW}`, :math:`\text{CAP}` and :math:`\text{ACT}` as well as all bounds 
 are always understood to be in the same units. All cost parameters also have to be provided 
 in monetary units per these units - there is no "automatic rescaling" done either within the ixmp API
 or in the GAMS implementation pre- or postprocessing.
 
 Example 1 - Power plants
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 Technical specifications of power plants are commonly stated in terms of electricity generated (output). 
-Therefore, the decision variables should be understood as outputs, with the parameter :math:`output = 1` 
-and parameter :math:`input = \frac{1}{efficiency}`. This may seem counter-intuitive at first, but the clear 
+Therefore, the decision variables should be understood as outputs, with the parameter :math:`\text{output} = 1` 
+and parameter :math:`\text{input} = \frac{1}{\text{efficiency}}`. This may seem counter-intuitive at first, but the clear 
 advantage is that all technical parameters can be immediately related to values found in the literature.
 
 Example 2 - Refineries
 ~~~~~~~~~~~~~~~~~~~~~~
 
 For crude oil refineries, it is more common to scale costs and emissions 
-in terms of crude oil input quantities. Hence, the parameter :math:`input = 1` 
+in terms of crude oil input quantities. Hence, the parameter :math:`\text{input} = 1` 
 and the output parameters (usually for multiple different oil products) 
 should be set accordingly.
 
 The decision variables and bounds are then implicitly understood as input-based.
 
 An alternative would be to parametrize a refinery based on outputs, but 
 considering that there are multiple outputs (in fixed proportions), 
 the sum of output parameters over all products should be set to 1,
-i.e., :math:`\sum_{c} output_{c} = 1`. The input of crude oil should then 
-include the losses during the refining process,  :math:`input > 1`.
+i.e., :math:`\sum_{c} \text{output}_{c} = 1`. The input of crude oil should then 
+include the losses during the refining process,  :math:`\text{input} > 1`.
  
 Example 3 - Combined power- and heat plants
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 As a third option, technical specifications of combined heat- and power plants
 are usually also given with regard to electricity generated under the 
 assumption that the electricity generated is maximized. Then, as in example 1,
 the capacity and activity variables should be understood as electricity generated.
 
 Assuming that such a plant usually has (at least) two modes of operation, these 
 modes could be parametrized as follows:
 
-:math:`input = \frac{1}{efficiency}`
+:math:`\text{input} = \frac{1}{\text{efficiency}}`
 
-:math:`output_{'M1','electricity'} = 1` and :math:`output_{'M1','heat'} = 0.2`
+:math:`\text{output}_{\text{M1},\text{electricity}} = 1` and :math:`\text{output}_{\text{M1},\text{heat}} = 0.2`
 
-:math:`output_{'M2','electricity'} = 0.5` and :math:`output_{'M2','heat'} = 3`.
+:math:`\text{output}_{\text{M2},\text{electricity}} = 0.5` and :math:`\text{output}_{\text{M2}, \text{heat}} = 3`.
 
 Note that the activity level in mode 'M2' has an odd interpretation - the amount 
 of electricity generated if electricity generation were maximized. The sum of outputs 
 is greater than 1 in either mode. However, we believe that this approach at least
 has the benefit of a parametrization that can be directly related to technical reports.
```

### Comparing `message_ix-3.6.0/doc/faq.rst` & `message_ix-3.7.0/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/framework.rst` & `message_ix-3.7.0/doc/framework.rst`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 The framework can be applied to analyse scenarios of the energy system transformation under technical-engineering constraints and political-societal considerations.
 
 Framework components
 ====================
 
 .. figure:: _static/ix_components.png
 
-   Components and their interlinkages in the |ixmp| (:cite:`huppmann_messageix_2018`): web-based user interface, scientific
+   Components and their interlinkages in the |ixmp| (:cite:`Huppmann-2018`): web-based user interface, scientific
    programming interface, modeling platform, database backend, implementation
    of the |MESSAGEix| mathematical model formulation.
 
 
 **MESSAGE** is a specific mathematical formulation of a model developed for strategic energy planning and integrated assessment of energy-engineering-economy-environment systems (E4).
-The formulation included in :mod:`message_ix` is a re-implementation and extension of “MESSAGE V” (Messner and Strubegger, 1995 :cite:`messner_users_1995`), the integrated assessment model developed at |IIASA| since the 1980s.
+The formulation included in :mod:`message_ix` is a re-implementation and extension of “MESSAGE V” (Messner and Strubegger, 1995 :cite:`Messner-Strubegger-1995`), the integrated assessment model developed at |IIASA| since the 1980s.
 The optimization model can be linked to the general-equilibrium **MACRO** model to incorporate feedback between prices and demand levels for energy and commodities.
 The :mod:`message_ix` package includes code for both MESSAGE, MACRO, and the MESSAGE-MACRO link.
 These are written in the `GAMS`_ mathematical programming language.
 :mod:`message_ix` uses GAMS to compute the numerical solution of a model instance.
 
 .. _`GAMS`: http://www.gams.com
 
@@ -44,18 +44,18 @@
   - conversion technologies from primary to secondary energy forms,
   - transmission and distribution (e.g. of electricity), and
   - final demand for energy services.
 
 - **Vintaging** of capacity, early retirement and decommissioning of
   technologies.
 - System integration of **variable renewable energy sources** (based on
-  Sullivan et al., 2013 :cite:`sullivan_VRE_2013` and Johnson et al., 2016
-  :cite:`johnson_VRE_2016`).
+  Sullivan et al., 2013 :cite:`Sullivan-2013` and Johnson et al., 2016
+  :cite:`Johnson-2016`).
 - Soft relaxation of **dynamic constraints** on new capacity and activity
-  (Keppo and Strubegger, 2010 :cite:`keppo_short_2010`).
+  (Keppo and Strubegger, 2010 :cite:`Keppo-2010`).
 - **Perfect-foresight** and **dynamic-recursive** (myopic) solution algorithms.
 
 .. _running:
 
 Running a model
 ===============
```

### Comparing `message_ix-3.6.0/doc/index.rst` & `message_ix-3.7.0/doc/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 *************************
 
 |MESSAGEix| is a versatile, dynamic systems-optimization modelling framework developed by the |IIASA| Energy, Climate, and Environment (ECE) Program [#rename]_ since the 1980s.
 
 This is the documentation for :mod:`message_ix`, a Python package that ties together all components of the framework.
 :mod:`message_ix` and :mod:`ixmp` are free and open source, licensed under the `APACHE 2.0 open-source license`_.
 
-- For the scientific reference of the framework, see Huppmann et al. (2019) :cite:`huppmann_messageix_2018`.
+- For the scientific reference of the framework, see Huppmann et al. (2019) :cite:`Huppmann-2018`.
 - For an overview and recent publications related to the specific |MESSAGEix|-GLOBIOM global model instance used at the IIASA ECE Program, see the `MESSAGEix-GLOBIOM documentation`_.
 
 
 .. _getting-started:
 
 Getting started
 ===============
@@ -43,15 +43,15 @@
    tutorials
    Publications, Projects, and Tools <usage>
 
 .. figure:: _static/ix_features.svg
    :width: 360px
    :align: center
 
-   Features of ``ixmp``, ``message_ix``, and related packages :cite:`huppmann_messageix_2018`
+   Features of ``ixmp``, ``message_ix``, and related packages :cite:`Huppmann-2018`
 
 
 .. _core:
 
 Mathematical specification
 ==========================
```

### Comparing `message_ix-3.6.0/doc/install.rst` & `message_ix-3.7.0/doc/install.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/make.bat` & `message_ix-3.7.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/prereqs.rst` & `message_ix-3.7.0/doc/prereqs.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/reporting.rst` & `message_ix-3.7.0/doc/reporting.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/rmessageix.rst` & `message_ix-3.7.0/doc/rmessageix.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/sharing.rst` & `message_ix-3.7.0/doc/sharing.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/doc/time.rst` & `message_ix-3.7.0/doc/time.rst`

 * *Files 6% similar despite different names*

```diff
@@ -38,53 +38,53 @@
 
 Time slices
 ===========
 
 The ``time`` set is used to index parameter dimensions with the names "time", "time_origin", "time_dest", etc.
 These are variously referred to as “(sub-annual) time slices”, “time steps”, or other names.
 Elements in this set are labels for **portions of a single year**.
-The special value ``'year'`` represents the entire year.
+The special value ``'Year'`` represents the entire year.
 
 Since a ``year`` element refers to the representative, final year within a period, using ``year`` and ``time`` together denotes *a portion of that specific year*.
 
 Example 4
    In a Scenario with ``year`` elements [2000, 2002, 2004] and ``time`` elements [summer, winter]:
 
    - The ``year`` element ``2002`` refers to the period from 2001-01-01 to 2002-12-31 inclusive, which has a ``duration_period`` of 2 years.
    - The ``time`` element 'summer', **used alone**, refers to a portion of any year.
    - In a |MESSAGEix| parameter indexed by (``year``, ``time``, …), values with the key (``2002``, 'summer', ...) refer to the 'summer' portion of the final year (2002-01-01 to 2002-12-31) within the entire period (2001-01-01 to 2002-12-31) denoted by ``2002``.
 
 Duration of sub-annual time slices
 ----------------------------------
-The duration of each sub-annual time slice should be defined relative to the whole year, with a value between 0 and 1, using parameter ``duration_time``.
+The duration of each sub-annual time slice should be defined relative to the whole year, with a value between 0 and 1, using the parameter ``duration_time``.
 For example, in a model with four seasons with the same length, ``duration_time`` of each season will be 0.25.
 Please note that the duration of time slices does not need to be equal to each other.
 This information is needed to calculate capacity of a technology that is active in different time slices.
-Time slices can be represented at different temporal levels, using sets ``lvl_temporal`` and ``map_temporal_hierarchy``.
-This helps introducing a flexible temporal resolution, e.g., by representing some technologies at finer time resolution while others at ``year``.
+Time slices can be represented at different temporal levels, using the sets ``lvl_temporal`` and ``map_temporal_hierarchy``.
+This helps introducing a flexible temporal resolution, e.g., by representing some technologies at finer time resolution while others at ``Year``.
 When there are more than one temporal levels, e.g., "year", "season", "month", "day", etc., ``duration_time`` is defined for time slices at each **temporal level** separately.
 The sum of ``duration_time`` of time slices at each temporal level must be equal to 1.
 For example, in a model with 4 time slices as "season" and 10 time slices as "day" under each "season", ``duration_time`` of each "season" and "day" can be specified as 0.25 and 0.025, respectively.
 
 By default, the unit of ``ACT`` is treated per year in the GAMS formulation for different time slices.
-This means values reported in time slice "year" and "month" both have the same unit (e.g., GWa).
+This means values reported in time slice "Year" and "month" both have the same unit (e.g., GWa).
 However, the user can report the values across parameters and variables with different units relative to the length of the full year.
-For example, the user can report ``ACT`` in units of "GWa" and "GWh" for time slices of "year" and "hour", respectively, in the same model.
+For example, the user can report ``ACT`` in units of "GWa" and "GWh" for time slices of "Year" and "hour", respectively, in the same model.
 To activate this feature, the parent time slice for which the relative units are desired should be specified by set ``time_relative``.
-This will ensure that parameter ``duration_time_rel``  is effective.
+This will ensure that parameter ``duration_time_rel`` is effective.
 Otherwise, this parameter is filled by value of 1, meaning that the units will be treated uniformly across different sub-annual time slices.
 
 Discounting
 ===========
 
 The ``interest_rate`` in |MESSAGEix| is defined for a period of one year, therefore, for periods of more than a year, the discounting is performed in a cumulative manner.
 
 Example 5
    Using the same setup as Example 2:
 
    - Discounting for the element ``1010`` involves discounting for years ``1001``, ``1002``, ... , ``1010``.
-   - Using the standard PV formula, we have that, for the year ``1001`` the discount factor would be :math:`(1 + interest_rate)^(1000 - 1001)`, for the year  ``1002`` the discount factor would be :math:`(1 + interest_rate)^(1000 - 1002)`, and so on.
-   - Therefore, the period discount factor for the element ``1010`` is :math:`df_1010 = (1 + interest_rate)^(1000 - 1001) + (1 + interest_rate)^(1000 - 1002) + ... + (1 + interest_rate)^(1000 - 1010)`
-   - Analogously, the period discount factor for the element ``1020`` is :math:`df_1020 = (1 + interest_rate)^(1000 - 1011) + (1 + interest_rate)^(1000 - 1012) + ... + (1 + interest_rate)^(1000 - 1020)`
+   - Using the standard PV formula, we have that, for the year ``1001`` the discount factor would be :math:`(1 + \text{interest_rate})^{1000 - 1001}`, for the year  ``1002`` the discount factor would be :math:`(1 + \text{interest_rate})^{1000 - 1002}`, and so on.
+   - Therefore, the period discount factor for the element ``1010`` is :math:`\text{df}_{1010} = (1 + \text{interest_rate})^{1000 - 1001} + ... + (1 + \text{interest_rate})^{1000 - 1010}`
+   - Analogously, the period discount factor for the element ``1020`` is :math:`\text{df}_{1020} = (1 + \text{interest_rate})^{1000 - 1011} + ... + (1 + \text{interest_rate})^{1000 - 1020}`
    - So, if we have a cost of ``K_1010`` for the element ``1010``, its discounted value would be ``df_1010 * K_1010``, which means, all the years in  element ``1010`` have a representative cost of ``K_1010`` that is discounted up to the initial ``year`` of the setup, namely, the year ``1000``.
 
 In practice, since the representative year of a period is always its final year, the actual calculation of the period discount factor within the model is performed backwards, i.e., starting from the final year of the period until the initial year.
```

### Comparing `message_ix-3.6.0/doc/usage.rst` & `message_ix-3.7.0/doc/usage.rst`

 * *Files 16% similar despite different names*

```diff
@@ -19,63 +19,78 @@
 
 Publications
 ============
 
 The following is a selection of academic publications in which |MESSAGEix| was used to carry out energy systems research.
 For each, the spatial scope/resolution, keywords and specific usage of |MESSAGEix| are described.
 
+Role of energy storage in energy and water security in Central Asia
+-----------------------------------------------------------------------------------
+.. figure:: _static/usage_figures/10.1016-j.est.2022.104587.JPG
+   :width: 250px
+   :align: right
+
+:cite:ct:`Zakeri-2022`
+
+- **Spatial**: Regional (Central Asia), multi-country including Kazakhstan, Kyrgyzstan, Tajikistan, Turkmenistan, and Uzbekistan
+- **Keywords**: Energy storage, seasonal pumped hydropower storage, water management, renewable energy systems, energy policy, electricity storage, energy model
+- **Usage**: Model the energy-water system of Central Asia with 12 sub-annual time slices and analyze the role of energy and water storage solutions.
+- **Data and code**: Data and scripts for building the model are openly available on `Github <https://github.com/iiasa/central-asia-storage>`__
+
+Central Asia has faced major energy and water security challenges. Technic… `Read more → <https://doi.org/10.1016/j.est.2022.104587>`__
+
 Climate mitigation scenarios with persistent COVID-19-related energy demand changes
 -----------------------------------------------------------------------------------
 .. figure:: _static/usage_figures/41560_2021_904.webp
    :width: 250px
    :align: right
 
-:cite:ct:`Kikstra2021`
+:cite:ct:`Kikstra-2021`
 
 - **Spatial**: Global, :ref:`11-region aggregation <message-ix-models:R11>`
 - **Keywords**: Climate-change mitigation, energy and behaviour, energy supply and demand
 - **Usage**: Capture global economy, energy and climate dynamics and feedbacks in the medium-to-long term, including regionally heterogeneous responses to the COVID-19 emergency.
 
 The COVID-19 pandemic caused radical temporary breaks with past energy use… `Read more → <https://www.nature.com/articles/s41560-021-00904-8>`__
 
 Deep seawater cooling and desalination: Combining seawater air conditioning and desalination
 --------------------------------------------------------------------------------------------
 .. figure:: _static/usage_figures/10.1016-j.scs.2021.103257.jpg
    :width: 250px
    :align: right
 
-:cite:ct:`HUNT2021103257`
+:cite:ct:`Hunt-2021`
 
 - **Spatial**: Malé, Maldives
 - **Keywords**: Building cooling, industrial cooling, energy efficiency, seawater air conditioning, low temperature thermal desalination, vertical farming
 - **Usage**: Simulate Malé´s cooling and water services demand and optimize the renewable energy supply.
 
 In tropical climates, the energy consumed by heating, ventilation and air… `Read more → <https://www.sciencedirect.com/science/article/pii/S2210670721005333>`__
 
 Energy investment needs for fulfilling the Paris Agreement and achieving the Sustainable Development Goals
 ----------------------------------------------------------------------------------------------------------
 .. figure:: _static/usage_figures/10.1038-s41560-018-0179-z.webp
    :width: 250px
    :align: right
 
-:cite:ct:`McCollum2018`
+:cite:ct:`McCollum-2018`
 
 - **Spatial**: Global
 - **Keywords**: Energy and society, finance, socioeconomic scenarios
 - **Usage**: Calculate SDG investment needs with a diverse set of approaches within a multi-model analysis.
 
 Low-carbon investments are necessary for driving the energy system… `Read more → <https://www.nature.com/articles/s41560-018-0179-z>`__
 
 A low energy demand scenario for meeting the 1.5 °C target and sustainable development goals without negative emission technologies
 -----------------------------------------------------------------------------------------------------------------------------------
 .. figure:: _static/usage_figures/10.1038-s41560-018-0172-6.webp
    :width: 250px
    :align: right
 
-:cite:ct:`Grubler2018`
+:cite:ct:`Grubler-2018`
 
 - **Spatial**: Global
 - **Keywords**: Energy modelling, socioeconomic scenarios
 - **Usage**: Calculate the energy supply impacts by imposing three types of constraints.
 
 Scenarios that limit global warming to 1.5 °C describe major… `Read more → <https://www.nature.com/articles/s41560-018-0172-6>`__
 
@@ -91,15 +106,15 @@
 
 d2ix: A Model Input-Data Management and Analysis Tool for MESSAGEix
 -------------------------------------------------------------------
 .. figure:: _static/usage_figures/10.3390-en12081483.png
    :width: 250px
    :align: right
 
-:cite:ct:`d2ix`
+:cite:ct:`Zipperle-Orthofer-2019`
 
 - **Goal**: Manageable, comprehensible, and traceable representation of input data.
 - **Features**: Spreadsheet interface that enables presentation and editing of model input data in a concise form.
 - **GitHub**: https://github.com/tum-ewk/d2ix
 
 Bottom-up integrated assessment models, like |MESSAGEix|, depend on the… `Read more → <https://www.mdpi.com/1996-1073/12/8/1483/htm>`__
```

### Comparing `message_ix-3.6.0/message_ix/__init__.py` & `message_ix-3.7.0/message_ix/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import logging
 from pathlib import Path
 
+try:
+    from importlib.metadata import PackageNotFoundError, version
+except ImportError:  # Python 3.7
+    from importlib_metadata import PackageNotFoundError, version  # type: ignore
+
 from ixmp import ModelError, config
 from ixmp.model import MODELS
-from pkg_resources import DistributionNotFound, get_distribution
 
 from .core import Scenario
 from .models import MACRO, MESSAGE, MESSAGE_MACRO
 from .reporting import Reporter
 from .util import make_df
 
 __all__ = [
@@ -19,16 +23,16 @@
     "Reporter",
     "Scenario",
     "config",
     "make_df",
 ]
 
 try:
-    __version__ = get_distribution(__name__).version
-except DistributionNotFound:
+    __version__ = version(__name__)
+except PackageNotFoundError:  # pragma: no cover
     # Package is not installed
     __version__ = "999"
 
 # Register configuration keys with ixmp core and set default
 config.register("message model dir", Path, Path(__file__).parent / "model")
 config.register("message solve options", dict)
```

### Comparing `message_ix-3.6.0/message_ix/cli.py` & `message_ix-3.7.0/message_ix/cli.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/core.py` & `message_ix-3.7.0/message_ix/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,15 +415,15 @@
             pd.DataFrame(
                 {"year": year, "value": [duration_first] + duration, "unit": "y"}
             ),
         )
 
     def vintage_and_active_years(
         self,
-        ya_args: Union[Tuple[str, str], Tuple[str, str, Union[int, str]]] = None,
+        ya_args: Union[Tuple[str, str], Tuple[str, str, Union[int, str]], None] = None,
         tl_only: bool = True,
         **kwargs,
     ) -> pd.DataFrame:
         r"""Return matched pairs of vintage and active periods for use in data input.
 
         Each returned pair of (vintage period :math:`y^V`, active period :math:`y`)
         satisfies all of the following conditions:
@@ -440,15 +440,15 @@
            b. :math:`y - y^V + \text{duration_period}_{n,t,y^V} <
               \text{technical_lifetime}_{n,t,y^V}`: the active period is partly or fully
               within the technical lifetime defined for that technology, node, and
               vintage. This is the same condition as :meth:`years_active`.
 
         4. If `ya_args` are given and `tl_only` is :obj:`True` (the default): :math:`y`
            is in the subset of :math:`Y` for which
-           :math:`\text{technical_lifetime}_{n,t,y}` is defined.[1]_
+           :math:`\text{technical_lifetime}_{n,t,y}` is defined. [1]_
         5. (Deprecated) If `in_horizon` is :obj:`True`: :math:`y \geq y_0`, the
            :attr:`.firstmodelyear`.
 
         .. [1] note this applies to :math:`y`, whereas condition 3(a) applies to
            :math:`y^V`.
 
         Parameters
@@ -709,15 +709,16 @@
         MACRO.initialize(clone)
 
         add_model_data(self, clone, data)
         clone.commit("finished adding macro")
         calibrate(clone, check_convergence=check_convergence, **kwargs)
         return clone
 
-    def rename(self, name, mapping, keep=False):
+    # FIXME reduce complexity from 18 to <=14
+    def rename(self, name, mapping, keep=False):  # noqa: C901
         """Rename an element in a set
 
         Parameters
         ----------
         name : str
             name of the set to change (e.g., 'technology')
         mapping : str
```

### Comparing `message_ix-3.6.0/message_ix/macro.py` & `message_ix-3.7.0/message_ix/macro.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 UNITS = dict(
     cost_MESSAGE="cost_ref",
     demand_MESSAGE="demand_ref",
     historical_gdp="gdp_calibrate",
     price_MESSAGE="price_ref",
 )
 
-# ixmp items (sets, parameters, variables, and equations) in MACRO.
+#: All of the ixmp items (sets, parameters, variables, and equations) in the MACRO
+#: mathematical formulation.
 MACRO_ITEMS = dict(
     sector=dict(ix_type="set"),
     mapping_macro_sector=dict(ix_type="set", idx_sets=["sector", "commodity", "level"]),
     MERtoPPP=dict(ix_type="par", idx_sets=["node", "year"]),
     aeei=dict(ix_type="par", idx_sets=["node", "sector", "year"]),
     cost_MESSAGE=dict(ix_type="par", idx_sets=["node", "year"]),
     demand_MESSAGE=dict(ix_type="par", idx_sets=["node", "sector", "year"]),
@@ -367,22 +368,20 @@
         """
         esub = self.data["esub"]
         self.data["rho"] = (esub - 1) / esub
         return self.data["rho"]
 
     @lru_cache()
     def _gdp0(self):
-        """
-        Derive GDP reference values from "gdp_calibrate" for MACRO calibration.
+        """Derive GDP reference values from "gdp_calibrate" for MACRO calibration.
 
         Returns
         -------
-        pandas Series
+        pandas.Series
             Calculated "gdp0" parameter.
-
         """
         gdp = self.data["gdp_calibrate"]
         gdp0 = gdp.iloc[gdp.index.isin([self.init_year], level="year")]
         self.data["gdp0"] = gdp0
         return self.data["gdp0"]
 
     @lru_cache()
@@ -522,31 +521,34 @@
         if demand.isnull().any():
             raise RuntimeError("NaN values found in demand calculation")
         self.data["demand"] = demand
         return demand
 
     @lru_cache()
     def _bconst(self):
-        """
-        Calculate production function coefficient of different energy sectors ("bcosnt")
-        for MACRO calibration (specified as "prfconst" in GAMS formulation).
+        """Calculate production function coefficient ("bconst").
+
+        This quantity is specified as "prfconst" in the GAMS formulation.
 
         Returns
         -------
-        pandas Series
+        pandas.Series
             Data as initial value for parameter "prfconst".
-
         """
         price_ref = self.data["price_ref"]
         demand_ref = self.data["demand_ref"]
         rho = self._rho()
         gdp0 = self._gdp0()
-        # TODO: automatically get the units here!!
-        bconst = price_ref / 1e3 * (gdp0 / demand_ref) ** (rho - 1)
-        self.data["bconst"] = bconst
+
+        # TODO automatically get the units here
+        # NB(PNK) pandas 1.4.4 automatically drops "year" in the division; pandas 1.5.0
+        # does not. Drop here pre-emptively.
+        tmp = ((gdp0 / demand_ref) ** (rho - 1)).droplevel("year")
+        self.data["bconst"] = price_ref / 1e3 * tmp
+
         return self.data["bconst"]
 
     @lru_cache()
     def _aconst(self):
         """
         Calculate production function coefficient of capital and labor ("aconst"),
         for MACRO calibration (specified as "lakl" in GAMS formulation).
@@ -563,15 +565,15 @@
         gdp0 = self._gdp0()
         k0 = self._k0()
         kpvs = self.data["kpvs"]
         partmp = (bconst * demand_ref**rho).groupby(level="node").sum()
         # TODO: automatically get the units here!!
         aconst = ((gdp0 / 1e3) ** rho - partmp) / (k0 / 1e3) ** (rho * kpvs)
         # want the series to only have index of node
-        self.data["aconst"] = aconst.reset_index(level="year", drop=True)
+        self.data["aconst"] = aconst.droplevel("year")
         return self.data["aconst"]
 
 
 def add_model_data(base, clone, data):
     """Calculate required parameters and add data to `clone`.
 
     Parameters
```

### Comparing `message_ix-3.6.0/message_ix/model/MACRO/macro_calibration.gms` & `message_ix-3.7.0/message_ix/model/MACRO/macro_calibration.gms`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
          MAX_ITER
 ;
 
 * ------------------------------------------------------------------------------
 * solving the model region by region
 * ------------------------------------------------------------------------------
 
+* no check is made to see if a certain convergence criteria is acheived.
+* MAX_ITER will determine the number of iterations after which the calibration is automatically halted.
 FOR (ctr = 1 TO max_it BY 1,
 
 * ------------------------------------------------------------------------------
 * solve MACRO model
 * ------------------------------------------------------------------------------
 
 $INCLUDE MACRO/macro_solve.gms
```

### Comparing `message_ix-3.6.0/message_ix/model/MACRO/macro_core.gms` & `message_ix-3.7.0/message_ix/model/MACRO/macro_core.gms`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 )
 ;
 
 ***
 * Equation CAPITAL_CONSTRAINT
 * ---------------------------------
 * The following equation specifies the allocation of total production among current consumption :math:`{C}_{n, y}`, investment into building up capital stock excluding
-* the sectors represented in MESSAGE :math:`{I}_{n, y}` and the MESSAGE system costs :math:`{EC}_{n, y}` which are derived from a previous MESSAGE model run. As described in :cite:`manne_buying_1992`, the first-order
+* the sectors represented in MESSAGE :math:`{I}_{n, y}` and the MESSAGE system costs :math:`{EC}_{n, y}` which are derived from a previous MESSAGE model run. As described in :cite:`Manne-Richels-1992`, the first-order
 * optimality conditions lead to the Ramsey rule for the optimal allocation of savings, investment and consumption over time.
 *
 * .. math:: Y_{n, y} = C_{n, y} + I_{r, y} + {EC}_{n, y} \qquad \forall{n, y}
 *
 ***
 
 CAPITAL_CONSTRAINT(node_active, year)..
@@ -289,15 +289,15 @@
 + SUM(sector, eneprice(node_active, sector, year) * 1E-3 / enestart(node_active, sector, year) * (PHYSENE(node_active, sector, year) - enestart(node_active, sector, year)) * (PHYSENE(node_active, sector, year) - enestart(node_active, sector, year))))
 ;
 
 ***
 * Equation TERMINAL_CONDITION
 * ---------------------------------
 * Given the finite time horizon of MACRO, a terminal constraint needs to be applied to ensure that investments are chosen at an appropriate level, i.e. to replace depriciated capital and
-* provide net growth of capital stock beyond MACRO's time horizon :cite:`manne_buying_1992`. The goal is to avoid to the extend possible model artifacts resulting from this finite time horizon
+* provide net growth of capital stock beyond MACRO's time horizon :cite:`Manne-Richels-1992`. The goal is to avoid to the extend possible model artifacts resulting from this finite time horizon
 * cutoff.
 *
 * .. math:: K_{n, y} \cdot  \left( grow_{n, y} + {depr}_n \right) \leq I_{n, y} \qquad \forall{ n, y = last year}
 ***
 
 TERMINAL_CONDITION(node_active, last_period)..
 I(node_active, last_period) =G= K(node_active, last_period) * (grow(node_active, last_period) + depr(node_active))
```

### Comparing `message_ix-3.6.0/message_ix/model/MACRO/macro_data_load.gms` & `message_ix-3.7.0/message_ix/model/MACRO/macro_data_load.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/MACRO/macro_solve.gms` & `message_ix-3.7.0/message_ix/model/MACRO/macro_solve.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/MACRO_run.gms` & `message_ix-3.7.0/message_ix/model/MACRO_run.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/auxiliary_settings.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/auxiliary_settings.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/data_load.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/data_load.gms`

 * *Files 2% similar despite different names*

```diff
@@ -137,22 +137,25 @@
 map_ren_grade(node,commodity,grade,year_all)$(
     SUM(level_renewable, renewable_potential(node,commodity,grade,level_renewable,year_all) ) ) = yes;
 
 * mapping of technologies to commodities and ratings
 map_rating(node,inv_tec,commodity,level,rating,year_all)$(
     SUM(time, reliability_factor(node,inv_tec,year_all,commodity,level,time,rating) ) ) = yes;
 
-* set the default capacity factor for technologies where no parameter value is provided in the input data
-capacity_factor(node,tec,year_all2,year_all,time)$( map_tec_time(node,tec,year_all,time)
-    AND map_tec_lifetime(node,tec,year_all2,year_all) AND NOT is_capacity_factor(node,tec,year_all2,year_all,time) ) = 1 ;
-
 * assign the yearly average capacity factor (used in equation OPERATION_CONSTRAINT)
 capacity_factor(node,tec,year_all2,year_all,'year') =
     sum(time$map_tec_time(node,tec,year_all,time), duration_time(time)
-        * capacity_factor(node,tec,year_all2,year_all,time) ) ;
+        * capacity_factor(node,tec,year_all2,year_all,time) );
+
+* update the masking set for capacity factor based on the average values added above
+is_capacity_factor(node,tec,year_all2,year_all,time)$(capacity_factor(node,tec,year_all2,year_all,'year') ) = yes;
+
+* set the default capacity factor for technologies where no parameter value is provided in the input data
+capacity_factor(node,tec,year_all2,year_all,time)$( map_tec_time(node,tec,year_all,time)
+    AND map_tec_lifetime(node,tec,year_all2,year_all) AND NOT is_capacity_factor(node,tec,year_all2,year_all,time) ) = 1 ;
 
 * set the default operation factor for technologies where no parameter value is provided in the input data
 operation_factor(node,tec,year_all2,year_all)$( map_tec(node,tec,year_all)
     AND map_tec_lifetime(node,tec,year_all2,year_all) AND NOT operation_factor(node,tec,year_all2,year_all) ) = 1 ;
 
 * set the upper bound on addon-technology activity to 1 by default
 addon_up(node,tec,year_all,mode,time,type_addon)$(
@@ -164,19 +167,19 @@
 emission_scaling(type_emission,emission)$( cat_emission(type_emission,emission)
         and not emission_scaling(type_emission,emission) ) = 1 ;
 
 * mapping of storage technologies to their level and commodity (can be different from level and commodity of storage media)
 map_time_commodity_storage(node,tec,level,commodity,mode,year_all,time)$( storage_tec(tec) AND
     SUM( (node2,year_all2,time_act), input(node2,tec,year_all,year_all2,mode,node,commodity,level,time_act,time) ) ) = yes;
 
-* mapping of sequence of sub-annual timesteps in a period and temporal level
+* mapping of sequence of sub-annual time slices in a period and temporal level
 map_time_period(year_all,lvl_temporal,time,time2)$( time_order(lvl_temporal,time) AND
      time_order(lvl_temporal,time) + 1 = time_order(lvl_temporal,time2) ) = yes;
 
-* mapping of sequence of the last sub-annual timestep to the first to create a close the order of timesteps
+* mapping of sequence of the last sub-annual time slice to the first to create a close the order of time slices
 map_time_period(year_all,lvl_temporal,time,time2)$( time_order(lvl_temporal,time) AND
      time_order(lvl_temporal,time) = SMAX(time3,time_order(lvl_temporal,time3) ) AND time_order(lvl_temporal,time2) = 1 ) = yes;
 *----------------------------------------------------------------------------------------------------------------------*
 * sanity checks on the data set                                                                                        *
 *----------------------------------------------------------------------------------------------------------------------*
 
 Parameter check ;
```

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/model_core.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/model_core.gms`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 * :math:`ACT\_UP_{n,t,y,h} \in \mathbb{R}_+`               Relaxation of upper dynamic constraint on activity [#ACT_BD]_
 * :math:`ACT\_LO_{n,t,y,h} \in \mathbb{R}_+`               Relaxation of lower dynamic constraint on activity [#ACT_BD]_
 * :math:`LAND_{n,s,y} \in [0,1]`                           Relative share of land-use scenario (for land-use model emulator)
 * :math:`EMISS_{n,e,\widehat{t},y} \in \mathbb{R}`         Auxiliary variable for aggregate emissions by technology type
 * :math:`REL_{r,n,y} \in \mathbb{R}`                       Auxiliary variable for left-hand side of relations (linear constraints)
 * :math:`COMMODITY\_USE_{n,c,l,y} \in \mathbb{R}`          Auxiliary variable for amount of commodity used at specific level
 * :math:`COMMODITY\_BALANCE_{n,c,l,y,h} \in \mathbb{R}`    Auxiliary variable for right-hand side of :ref:`commodity_balance`
-* :math:`STORAGE_{n,t,l,c,y,h} \in \mathbb{R}`             State of charge or content of storage at each sub-annual timestep
-* :math:`STORAGE\_CHARGE_{n,t,l,c,y,h} \in \mathbb{R}`     Charging of storage in each sub-annual timestep (negative for discharging)
+* :math:`STORAGE_{n,t,m,l,c,y,h} \in \mathbb{R}`             State of charge or content of storage at each sub-annual time slice
+* :math:`STORAGE\_CHARGE_{n,t,m,l,c,y,h} \in \mathbb{R}`     Charging of storage in each sub-annual time slice (negative for discharging)
 * ======================================================== ====================================================================================
 *
 * The index :math:`y^V` is the year of construction (vintage) wherever it is necessary to
 * clearly distinguish between year of construction and the year of operation.
 *
 * All decision variables are by year, not by (multi-year) period, except :math:`STOCK_{n,c,l,y}`.
 * In particular, the new capacity variable :math:`CAP\_NEW_{n,t,y}` has to be multiplied by the number of years
@@ -102,15 +102,15 @@
     CAP_NEW_UP(node,tec,year_all)    relaxation variable for dynamic constraints on new capacity (upwards)
     CAP_NEW_LO(node,tec,year_all)    relaxation variable for dynamic constraints on new capacity (downwards)
     ACT_UP(node,tec,year_all,time)   relaxation variable for dynamic constraints on activity (upwards)
     ACT_LO(node,tec,year_all,time)   relaxation variable for dynamic constraints on activity (downwards)
 * land-use model emulator
     LAND(node,land_scenario,year_all) relative share of land-use scenario
 * content of storage
-    STORAGE(node,tec,level,commodity,year_all,time)       state of charge (SoC) of storage at each sub-annual timestep (positive)
+    STORAGE(node,tec,mode,level,commodity,year_all,time)       state of charge (SoC) of storage at each sub-annual time slice (positive)
 ;
 
 Variables
 * intertemporal stock variables (input or output quantity into the stock)
     STOCK_CHG(node,commodity,level,year_all,time) annual input into and output from stocks of commodities
 * technology activity variables (can be negative for some technologies, upper and lower bounds stated explicitly)
     ACT(node,tec,vintage,year_all,mode,time)     activity of technology by mode-year-timeperiod
@@ -119,15 +119,15 @@
 * nodal system costs over time
     COST_NODAL(node, year_all)                   system costs at the node level over time
 * auxiliary variable for aggregate emissions by technology type and land-use model emulator
     EMISS(node,emission,type_tec,year_all)       aggregate emissions by technology type and land-use model emulator
 * auxiliary variable for left-hand side of relations (linear constraints)
     REL(relation,node,year_all)                  auxiliary variable for left-hand side of user-defined relations
 * change in the content of storage device
-    STORAGE_CHARGE(node,tec,level,commodity,year_all,time)    charging of storage in each timestep (negative for discharge)
+    STORAGE_CHARGE(node,tec,mode,level,commodity,year_all,time)    charging of storage in each time slice (negative for discharge)
 ;
 
 ***
 * .. _section_auxiliary_variable_def:
 *
 * Auxiliary variables
 * ^^^^^^^^^^^^^^^^^^^
@@ -284,16 +284,16 @@
     DYNAMIC_LAND_TYPE_CONSTRAINT_UP dynamic constraint on land-use change (upper bound)
     DYNAMIC_LAND_TYPE_CONSTRAINT_LO dynamic constraint on land-use change (lower bound)
     RELATION_EQUIVALENCE            auxiliary equation to simplify the implementation of relations
     RELATION_CONSTRAINT_UP          upper bound of relations (linear constraints)
     RELATION_CONSTRAINT_LO          lower bound of relations (linear constraints)
     STORAGE_CHANGE                  change in the state of charge of storage
     STORAGE_BALANCE                 balance of the state of charge of storage
-    STORAGE_BALANCE_INIT            balance of the state of charge of storage at sub-annual time steps with initial storage content
-    STORAGE_EQUIVALENCE             mapping state of storage as activity of storage technologies
+    STORAGE_BALANCE_INIT            balance of the state of charge of storage at sub-annual time slices with initial storage content
+    STORAGE_INPUT                   connecting an input commodity to maintain the activity of storage container (not stored commodity)
 ;
 *----------------------------------------------------------------------------------------------------------------------*
 * equation statements                                                                                                  *
 *----------------------------------------------------------------------------------------------------------------------*
 
 ***
 * .. _section_objective:
@@ -952,15 +952,15 @@
 *----------------------------------------------------------------------------------------------------------------------*
 ***
 * .. _section_system_reliability:
 *
 * System reliability and flexibility requirements
 * -----------------------------------------------
 * This section followi allows to include system-wide reliability and flexility considerations.
-* The current formulation is based on Sullivan et al., 2013 :cite:`sullivan_VRE_2013`.
+* The current formulation is based on Sullivan et al., 2013 :cite:`Sullivan-2013`.
 *
 * Aggregate use of a commodity
 * ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 * The system reliability and flexibility constraints are implemented using an auxiliary variable representing
 * the total use (i.e., input of each commodity per level).
 *
 * .. _equation_commodity_use_level:
@@ -1086,15 +1086,15 @@
 
 ***
 * .. _equation_system_reliability_constraint:
 *
 * Equation SYSTEM_RELIABILITY_CONSTRAINT
 * """"""""""""""""""""""""""""""""""""""
 * This constraint ensures that there is sufficient firm (dispatchable) capacity in each period.
-* The formulation is based on Sullivan et al., 2013 :cite:`sullivan_VRE_2013`.
+* The formulation is based on Sullivan et al., 2013 :cite:`Sullivan-2013`.
 *
 *   .. math::
 *      \sum_{t, q \substack{t \in T^{INV} \\ y^V \leq y} } &
 *          reliability\_factor_{n,t,y,c,l,h,'firm'}
 *          \cdot CAP\_FIRM_{n,t,c,l,y} \\
 *      + \sum_{t,q,y^V \leq y} &
 *          reliability\_factor_{n,t,y,c,l,h,q}
@@ -1519,148 +1519,164 @@
 * Dynamic constraints on new capacity and activity
 * ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 *
 * The constraints in this section specify dynamic upper and lower bounds on new capacity and activity.
 * These can be used to model limits on market penetration and/or rates of expansion or phase-out of a technology.
 *
 * The formulation directly includes the option for 'soft' relaxations of dynamic constraints
-* (cf. Keppo and Strubegger, 2010 :cite:`keppo_short_2010`).
+* (cf. Keppo and Strubegger, 2010 :cite:`Keppo-2010`).
 *
 * See also the :ref:`corresponding parameter definitions <section_parameter_dynamic_constraints>`.
 *
 * .. _equation_new_capacity_constraint_up:
 *
 * Equation NEW_CAPACITY_CONSTRAINT_UP
 * """""""""""""""""""""""""""""""""""
 * The level of new capacity additions cannot be greater than an initial value (compounded over the period duration),
 * annual growth of the existing 'capital stock', and a "soft" relaxation of the upper bound.
 *
 *  .. math::
 *     CAP\_NEW_{n,t,y}
-*         \leq & ~ initial\_new\_capacity\_up_{n,t,y}
+*         \leq & \Bigg(~ initial\_new\_capacity\_up_{n,t,y}
 *             \cdot \frac{ \Big( 1 + growth\_new\_capacity\_up_{n,t,y} \Big)^{|y|} - 1 }
 *                        { growth\_new\_capacity\_up_{n,t,y} } \\
 *              & + \Big( CAP\_NEW_{n,t,y-1} + historical\_new\_capacity_{n,t,y-1} \Big) \\
 *              & \hspace{2 cm} \cdot \Big( 1 + growth\_new\_capacity\_up_{n,t,y} \Big)^{|y|} \\
-*              & + CAP\_NEW\_UP_{n,t,y} \cdot \Bigg( \Big( 1 + soft\_new\_capacity\_up_{n,t,y}\Big)^{|y|} - 1 \Bigg) \\
+*              & + CAP\_NEW\_UP_{n,t,y} \cdot \Bigg( \Big( 1 + soft\_new\_capacity\_up_{n,t,y}\Big)^{|y|} - 1 \Bigg)\Bigg) \\
+*              & * \frac{|y-1|}{|y|} \\
 *         & \quad \forall \ t \ \in \ T^{INV}
 *
 * Here, :math:`|y|` is the number of years in period :math:`y`, i.e., :math:`duration\_period_{y}`.
 ***
 NEW_CAPACITY_CONSTRAINT_UP(node,inv_tec,year)$( map_tec(node,inv_tec,year)
         AND is_dynamic_new_capacity_up(node,inv_tec,year) )..
 * actual new capacity
     CAP_NEW(node,inv_tec,year) =L=
 * initial new capacity (compounded over the duration of the period)
-        initial_new_capacity_up(node,inv_tec,year) * (
+        (initial_new_capacity_up(node,inv_tec,year) * (
             ( ( POWER( 1 + growth_new_capacity_up(node,inv_tec,year) , duration_period(year) ) - 1 )
                 / growth_new_capacity_up(node,inv_tec,year) )$( growth_new_capacity_up(node,inv_tec,year) )
               + ( duration_period(year) )$( NOT growth_new_capacity_up(node,inv_tec,year) )
             )
 * growth of 'capital stock' from previous period
         + SUM(year_all2$( seq_period(year_all2,year) ),
             CAP_NEW(node,inv_tec,year_all2)$( map_tec(node,inv_tec,year_all2) AND model_horizon(year_all2) )
               + historical_new_capacity(node,inv_tec,year_all2) )
               # placeholder for spillover across nodes, technologies, periods (other than immediate predecessor)
             * POWER( 1 + growth_new_capacity_up(node,inv_tec,year) , duration_period(year) )
 * 'soft' relaxation of dynamic constraints
         + ( CAP_NEW_UP(node,inv_tec,year)
             * ( POWER( 1 + soft_new_capacity_up(node,inv_tec,year) , duration_period(year) ) - 1 )
-           )$( soft_new_capacity_up(node,inv_tec,year) )
+           )$( soft_new_capacity_up(node,inv_tec,year) ))
+       * SUM(year_all2$( seq_period(year_all2,year) ),
+            ( duration_period(year_all2) / duration_period(year) ))
 * optional relaxation for calibration and debugging
 %SLACK_CAP_NEW_DYNAMIC_UP% + SLACK_CAP_NEW_DYNAMIC_UP(node,inv_tec,year)
 ;
 
 * GAMS implementation comment:
 * The sums in the constraint have to be over `year_all2` (not `year2`) to also get the dynamic effect from historical
 * new capacity. If one would sum over `year2`, periods prior to the first model year would be ignored.
+* Furthermore, as `CAP_NEW` is derived from the value in a previous period, any change in the duration of two consecutive
+* model periods needs to be accounted for. This is done by using the ratio of two consecutive model periods as a
+* multiplication factor.
 
 ***
 * .. _equation_new_capacity_soft_constraint_up:
 *
 * Equation NEW_CAPACITY_SOFT_CONSTRAINT_UP
 * """"""""""""""""""""""""""""""""""""""""
 * This constraint ensures that the relaxation of the dynamic constraint on new capacity (investment) does not exceed
-* the level of the investment in the previous period (cf. Keppo and Strubegger, 2010 :cite:`keppo_short_2010`).
+* the level of the investment in the previous period (cf. Keppo and Strubegger, 2010 :cite:`Keppo-2010`).
 *
 *   .. math::
 *      CAP\_NEW\_UP_{n,t,y} \leq \sum_{y-1} CAP\_NEW_{n^L,t,y-1} & \text{if } y \neq 'first\_period' \\
 *                                + \sum_{y-1} historical\_new\_capacity_{n^L,t,y-1} & \text{if } y = 'first\_period' \\
-*                           \quad \forall \ t \ \in \ T^{INV}   
+*                           \quad \forall \ t \ \in \ T^{INV}
 *
 ***
 NEW_CAPACITY_SOFT_CONSTRAINT_UP(node,inv_tec,year)$( soft_new_capacity_up(node,inv_tec,year) )..
     CAP_NEW_UP(node,inv_tec,year) =L=
-        SUM(year2$( seq_period(year2,year) ), 
+        SUM(year2$( seq_period(year2,year) ),
             CAP_NEW(node,inv_tec,year2)) $ (NOT first_period(year))
       + SUM(year_all2$( seq_period(year_all2,year) ),
             historical_new_capacity(node,inv_tec,year_all2)) $ first_period(year)
 ;
 
 ***
 * .. _equation_new_capacity_constraint_lo:
 *
 * Equation NEW_CAPACITY_CONSTRAINT_LO
 * """""""""""""""""""""""""""""""""""
 * This constraint gives dynamic lower bounds on new capacity.
 *
 *  .. math::
 *     CAP\_NEW_{n,t,y}
-*         \geq & - initial\_new\_capacity\_lo_{n,t,y}
+*         \geq & \Bigg(- initial\_new\_capacity\_lo_{n,t,y}
 *             \cdot \frac{ \Big( 1 + growth\_new\_capacity\_lo_{n,t,y} \Big)^{|y|} }
 *                        { growth\_new\_capacity\_lo_{n,t,y} } \\
 *              & + \Big( CAP\_NEW_{n,t,y-1} + historical\_new\_capacity_{n,t,y-1} \Big) \\
 *              & \hspace{2 cm} \cdot \Big( 1 + growth\_new\_capacity\_lo_{n,t,y} \Big)^{|y|} \\
-*              & - CAP\_NEW\_LO_{n,t,y} \cdot \Bigg( \Big( 1 + soft\_new\_capacity\_lo_{n,t,y}\Big)^{|y|} - 1 \Bigg) \\
+*              & - CAP\_NEW\_LO_{n,t,y} \cdot \Bigg( \Big( 1 + soft\_new\_capacity\_lo_{n,t,y}\Big)^{|y|} - 1 \Bigg)\Bigg) \\
+*              & * \frac{|y-1|}{|y|} \\
 *         & \quad \forall \ t \ \in \ T^{INV}
 *
 ***
 NEW_CAPACITY_CONSTRAINT_LO(node,inv_tec,year)$( map_tec(node,inv_tec,year)
         AND is_dynamic_new_capacity_lo(node,inv_tec,year) )..
 * actual new capacity
     CAP_NEW(node,inv_tec,year) =G=
 * initial new capacity (compounded over the duration of the period)
-        - initial_new_capacity_lo(node,inv_tec,year) * (
+        (- initial_new_capacity_lo(node,inv_tec,year) * (
             ( ( POWER( 1 + growth_new_capacity_lo(node,inv_tec,year) , duration_period(year) ) - 1 )
                 / growth_new_capacity_lo(node,inv_tec,year) )$( growth_new_capacity_lo(node,inv_tec,year) )
               + ( duration_period(year) )$( NOT growth_new_capacity_lo(node,inv_tec,year) )
             )
 * growth of 'capital stock' from previous period
         + SUM(year_all2$( seq_period(year_all2,year) ),
                 CAP_NEW(node,inv_tec,year_all2)$( map_tec(node,inv_tec,year_all2) AND model_horizon(year_all2) )
                 + historical_new_capacity(node,inv_tec,year_all2)
                 # placeholder for spillover across nodes, technologies, periods (other than immediate predecessor)
             ) * POWER( 1 + growth_new_capacity_lo(node,inv_tec,year) , duration_period(year) )
 * 'soft' relaxation of dynamic constraints
         - ( CAP_NEW_LO(node,inv_tec,year)
             * ( POWER( 1 + soft_new_capacity_lo(node,inv_tec,year) , duration_period(year) ) - 1 )
-           )$( soft_new_capacity_lo(node,inv_tec,year) )
+           )$( soft_new_capacity_lo(node,inv_tec,year) ))
+       * SUM(year_all2$( seq_period(year_all2,year) ),
+            ( duration_period(year_all2) / duration_period(year) ))
 * optional relaxation for calibration and debugging
 %SLACK_CAP_NEW_DYNAMIC_LO% - SLACK_CAP_NEW_DYNAMIC_LO(node,inv_tec,year)
 ;
 
+* GAMS implementation comment:
+* The sums in the constraint have to be over `year_all2` (not `year2`) to also get the dynamic effect from historical
+* new capacity. If one would sum over `year2`, periods prior to the first model year would be ignored.
+* Furthermore, as `CAP_NEW` is derived from the value in a previous period, any change in the duration of two consecutive
+* model periods needs to be accounted for. This is done by using the ratio of two consecutive model periods as a
+* multiplication factor.
+
 ***
 * .. _equation_new_capacity_soft_constraint_lo:
 *
 * Equation NEW_CAPACITY_SOFT_CONSTRAINT_LO
 * """"""""""""""""""""""""""""""""""""""""
 * This constraint ensures that the relaxation of the dynamic constraint on new capacity does not exceed
 * level of the investment in the previous year.
 *
 *   .. math::
 *      CAP\_NEW\_LO_{n,t,y} \leq \sum_{y-1} CAP\_NEW_{n^L,t,y-1} & \text{if } y \neq 'first\_period' \\
 *                                + \sum_{y-1} historical\_new\_capacity_{n^L,t,y-1} & \text{if } y = 'first\_period' \\
-*                           \quad \forall \ t \ \in \ T^{INV}  
+*                           \quad \forall \ t \ \in \ T^{INV}
 *
 ***
 NEW_CAPACITY_SOFT_CONSTRAINT_LO(node,inv_tec,year)$( soft_new_capacity_lo(node,inv_tec,year) )..
     CAP_NEW_LO(node,inv_tec,year) =L=
         SUM(year2$( seq_period(year2,year) ),
             CAP_NEW(node,inv_tec,year2) ) $ (NOT first_period(year))
-      + SUM(year_all2$( seq_period(year_all2,year) ), 
+      + SUM(year_all2$( seq_period(year_all2,year) ),
             historical_new_capacity(node,inv_tec,year_all2) ) $ first_period(year)
 ;
 
 ***
 * .. _equation_activity_constraint_up:
 *
 * Equation ACTIVITY_CONSTRAINT_UP
@@ -1713,15 +1729,15 @@
 * """"""""""""""""""""""""""""""""""""
 * This constraint ensures that the relaxation of the dynamic activity constraint does not exceed the
 * level of the activity in the previous period.
 *
 *   .. math::
 *      ACT\_UP_{n,t,y,h} \leq \sum_{y^V \leq y,m,y-1} ACT_{n^L,t,y^V,y-1,m,h} & \text{if } y \neq 'first\_period' \\
 *                             + \sum_{m,y-1} historical\_activity_{n^L,t,y-1,m,h} & \text{if } y = 'first\_period'
-*      
+*
 *
 ***
 ACTIVITY_SOFT_CONSTRAINT_UP(node,tec,year,time)$( soft_activity_up(node,tec,year,time) )..
     ACT_UP(node,tec,year,time) =L=
         SUM((vintage,mode,year2)$( map_tec_lifetime(node,tec,vintage,year2) AND map_tec_act(node,tec,year2,mode,time)
                                    AND seq_period(year2,year) ),
             ACT(node,tec,vintage,year2,mode,time) ) $ (NOT first_period(year))
@@ -2131,144 +2147,159 @@
 *----------------------------------------------------------------------------------------------------------------------*
 ***
 * .. _gams-storage:
 *
 * Storage section
 * ---------------
 *
-* Storage technologies can be used to store a commodity (e.g., water, heat, electricity, etc.)
-* and shift it over sub-annual time slices. The storage solution presented here has three
-* distinctive parts: (i) Charger: a technology for charging a commodity to the storage container,
+* MESSAGEix offers a set of equations to represent a wide range of storage solutions flexibly.
+* Storage solutions are modeled as "technologies" that can be used to store a "commodity" (e.g., water, heat, electricity, etc.)
+* and shift it over sub-annual time slices within one model period. The storage solution presented here has three
+* distinct parts: (i) Charger: a technology for charging a commodity to the storage container,
 * for example, a pump in a pumped hydropower storage (PHS) plant. (ii) Discharger: a technology
 * to convert the stored commodity to the output commodity, e.g., a turbine in PHS.
 * (iii) Storage container: a device for storing a commodity over time, such as a water reservoir in PHS.
+* If desired, the user can combine charger and discharger parts into one technology, using two different "modes" of operation
+* for that technology like turbo-machinery in PHS. This way the capacity related information, like investment cost, lifetime, capacity factor, etc.,
+* will be defined only for one technology (i.e., charger-discharger), as opposed to modeling these two parts separately.
 *
 * .. figure:: ../../_static/storage.png
 *
 * Storage equations
 * ^^^^^^^^^^^^^^^^^
 * The content of storage device depends on three factors: charge or discharge in
-* one time step (represented by `Equation STORAGE_CHANGE`_), the state of charge in the previous
-* time step, and storage losses between two consecutive time steps.
+* one time slice (represented by `Equation STORAGE_CHANGE`_), linked to the state of charge in the previous
+* time slice and storage losses between these two consecutive time slices (represented by `Equation STORAGE_BALANCE`_).
+* Moreover, the storage device can be optionally filled with an initial value as percentage of its capacity (see more details under `Equation STORAGE_BALANCE_INIT`_).
+* Another option is to link a commodity for maintaining the operation of storage device over time (see `Equation STORAGE_INPUT`_).
 *
 * .. _equation_storage_change:
 *
 * Equation STORAGE_CHANGE
 * """""""""""""""""""""""
 * This equation shows the change in the content of the storage container in each
-* sub-annual timestep. This change is based on the activity of charger and discharger
+* sub-annual time slice. This change is based on the activity of charger and discharger
 * technologies connected to that storage container. The notation :math:`S^{storage}`
 * represents the mapping set `map_tec_storage` denoting charger-discharger
 * technologies connected to a specific storage container in a specific node and
 * storage level. Where:
 *
 * - :math:`t^{C}` is a charging technology and :math:`t^{D}` is the corresponding discharger.
-* - :math:`h-1` is the time step prior to :math:`h`.
-*
+* - :math:`h-1` is the time slice prior to :math:`h`.
+* - :math: `l^{T}` is `lvl_temporal`, i.e., the temporal level at which storage is operating
+* - :math: `m^{S}` is `mode` of operation for storage container technology
+
 *   .. math::
-*      STORAGE\_CHARGE_{n,t,l,c,y,h} =
+*      STORAGE\_CHARGE_{n,t,m^s,l,c,y,h} =
 *          \sum_{\substack{n^L,m,h-1 \\ y^V \leq y, (n,t^C,t,l,y) \sim S^{storage}}} output_{n^L,t^C,y^V,y,m,n,c,l,h-1,h}
 *             \cdot & ACT_{n^L,t^C,y^V,y,m,h-1} \\
 *          - \sum_{\substack{n^L,m,c,h-1 \\ y^V \leq y, (n,t^D,t,l,y) \sim S^{storage}}} input_{n^L,t^D,y^V,y,m,n,c,l,h-1,h}
 *              \cdot ACT_{n^L,t^D,y^V,y,m,h-1} \quad \forall \ t \in T^{STOR}, & \forall \ l \in L^{STOR}
 ***
-STORAGE_CHANGE(node,storage_tec,level_storage,commodity,year,time) ..
-* change in the content of storage in the examined timestep
-    STORAGE_CHARGE(node,storage_tec,level_storage,commodity,year,time) =E=
+STORAGE_CHANGE(node,storage_tec,mode,level_storage,commodity,year,time)$sum(
+               (tec,mode2,lvl_temporal), map_tec_storage(node,tec,mode2,storage_tec,mode,level_storage,commodity,lvl_temporal) ) ..
+* change in the content of storage in the examined time slice
+    STORAGE_CHARGE(node,storage_tec,mode,level_storage,commodity,year,time) =E=
 * increase in the content of storage due to the activity of charging technologies
-        SUM( (location,vintage,mode,tec,time2)$(
-        map_tec_lifetime(node,tec,vintage,year)
-        AND map_tec_storage(node,tec,storage_tec,level_storage,commodity) ),
-            output(location,tec,vintage,year,mode,node,commodity,level_storage,time2,time)
-            * duration_time_rel(time,time2) * ACT(location,tec,vintage,year,mode,time) )
+        SUM( (location,vintage,tec,mode2,time2,time3,lvl_temporal)$(
+        map_tec_lifetime(node,tec,vintage,year) AND map_temporal_hierarchy(lvl_temporal,time,time3
+                )$map_tec_storage(node,tec,mode2,storage_tec,mode,level_storage,commodity,lvl_temporal) ),
+            output(location,tec,vintage,year,mode2,node,commodity,level_storage,time2,time)
+            * duration_time_rel(time,time2) * ACT(location,tec,vintage,year,mode2,time2) )
 * decrease in the content of storage due to the activity of discharging technologies
-        - SUM( (location,vintage,mode,tec,time2)$(
-        map_tec_lifetime(node,tec,vintage,year)
-        AND map_tec_storage(node,tec,storage_tec,level_storage,commodity) ),
-            input(location,tec,vintage,year,mode,node,commodity,level_storage,time2,time)
-            * duration_time_rel(time,time2) * ACT(location,tec,vintage,year,mode,time) );
+        - SUM( (location,vintage,tec,mode2,time2,time3,lvl_temporal)$(
+        map_tec_lifetime(node,tec,vintage,year) AND map_temporal_hierarchy(lvl_temporal,time,time3
+                )$map_tec_storage(node,tec,mode2,storage_tec,mode,level_storage,commodity,lvl_temporal) ),
+            input(location,tec,vintage,year,mode2,node,commodity,level_storage,time2,time)
+            * duration_time_rel(time,time2) * ACT(location,tec,vintage,year,mode2,time2) );
 
 ***
 * .. _equation_storage_balance:
 *
 * Equation STORAGE_BALANCE
 * """"""""""""""""""""""""
 *
 * This equation ensures the commodity balance of storage technologies, where the commodity is shifted between sub-annual
-* timesteps within a model period. If the state of charge of storage is set exogenously in one timestep through
-* :math:`\storageinitial_{ntlcyh}`, the content from the previous timestep is not carried over to this timestep.
+* time slices within a model period. If the state of charge of storage is set exogenously in one time slice through
+* :math:`\storageinitial_{ntlcyh}`, the content from the previous time slice is not carried over to this time slice.
 *
 * .. math::
-*    \STORAGE_{ntlcyh} =\ & \STORAGECHARGE_{ntlcyh} + \\
-*    & \STORAGE_{ntlcy(h-1)} \cdot (1 - \storageselfdischarge_{ntly(h-1)}) \\
-*    \forall\ & t \in T^{STOR}, l \in L^{STOR}, \storageinitial_{ntlcyh} = 0
-***
-STORAGE_BALANCE(node,storage_tec,level,commodity,year,time2)$ (
-    SUM(tec, map_tec_storage(node,tec,storage_tec,level,commodity) )
-    AND NOT storage_initial(node,storage_tec,level,commodity,year,time2) )..
-* Showing the the state of charge of storage at each timestep
-    STORAGE(node,storage_tec,level,commodity,year,time2) =E=
-* change in the content of storage in the examined timestep
-    + STORAGE_CHARGE(node,storage_tec,level,commodity,year,time2)
-* storage content in the previous subannual timestep
-    + SUM((lvl_temporal,time)$map_time_period(year,lvl_temporal,time,time2),
-        STORAGE(node,storage_tec,level,commodity,year,time)
-* considering storage self-discharge losses due to keeping the storage media between two subannual timesteps
-        * (1 - storage_self_discharge(node,storage_tec,level,commodity,year,time) ) ) ;
+*    \STORAGE_{ntmlcyh} =\ & \STORAGECHARGE_{ntmlcyh} \\
+*    & + \STORAGE_{ntmlcy(h-1)} \cdot (1 - \storageselfdischarge_{ntmly(h-1)}) \\
+*    \forall\ & t \in T^{STOR}, l \in L^{STOR}, \storageinitial_{ntmlcyh} = 0
+***
+STORAGE_BALANCE(node,storage_tec,mode,level,commodity,year,time2,lvl_temporal)$ (
+    SUM((tec,mode2), map_tec_storage(node,tec,mode2,storage_tec,mode,level,commodity,lvl_temporal) )
+*    AND NOT storage_initial(node,storage_tec,mode,level,commodity,year,time2)
+)..
+* Showing the the state of charge of storage at each time slice
+    STORAGE(node,storage_tec,mode,level,commodity,year,time2) =E=
+* change in the content of storage in the examined time slice
+    + STORAGE_CHARGE(node,storage_tec,mode,level,commodity,year,time2)
+* storage content in the previous subannual time slice
+    + SUM(time$map_time_period(year,lvl_temporal,time,time2),
+        STORAGE(node,storage_tec,mode,level,commodity,year,time)
+* considering storage self-discharge losses due to keeping the storage media between two subannual time slices
+        * (1 - storage_self_discharge(node,storage_tec,mode,level,commodity,year,time) ) ) ;
 
 ***
 * .. _equation_storage_balance_init:
 *
 * Equation STORAGE_BALANCE_INIT
 * """""""""""""""""""""""""""""
 *
 * Where :math:`\storageinitial_{ntlyh}` has a non-zero value, this equation ensures that the amount of commodity stored
-* at the end of the period is equal to that value plus any change during the period.
+* at the end of a sub-annual time slice is equal or greater than the initialized content of storage in the following time slice.
+* The values in parameter :math:`\storageinitial_{ntlyh}` are percentages showing
+* a fraction of installed capacity of storage device (container) that can be filled initially.
 *
 * .. math::
-*    \STORAGE_{ntlcyh} =\ & \storageinitial_{ntlcyh} + \STORAGECHARGE_{ntlcyh} \\
-*    \forall\ & \storageinitial_{ntlcyh} \neq 0
+*    \STORAGE_{ntmlcy(h-1)} \geq &  \storageinitial_{ntmlcyh} \cdot duration\_time_{h} \cdot capacity\_factor_{n,t,y^V,y,h} \cdot CAP_{n,t,y^V,y}  \\
+*    \quad \forall \ t \ \in \ T^{INV}, \forall\ & \storageinitial_{ntmlcyh} \neq 0
 ***
 
-STORAGE_BALANCE_INIT(node,storage_tec,level,commodity,year,time)$ (
-    SUM(tec, map_tec_storage(node,tec,storage_tec,level,commodity) )
-    AND storage_initial(node,storage_tec,level,commodity,year,time) )..
-* Showing the state of charge of storage at a timestep with an initial storage content
-    STORAGE(node,storage_tec,level,commodity,year,time) =E=
-* initial content of storage and change in the content of storage in the examined timestep
-* (here the content from the previous time step is not carried over)
-    storage_initial(node,storage_tec,level,commodity,year,time)
-    + STORAGE_CHARGE(node,storage_tec,level,commodity,year,time) ;
-
+STORAGE_BALANCE_INIT(node,storage_tec,mode,level,commodity,year,time,time2)$ (
+    SUM((tec,mode2,lvl_temporal), map_tec_storage(node,tec,mode2,storage_tec,mode,level,commodity,lvl_temporal)
+        AND map_time_period(year,lvl_temporal,time,time2) )
+    AND storage_initial(node,storage_tec,mode,level,commodity,year,time2) )..
+* Showing the state of charge of storage at a time slice prior to a time slice that has initial storage content
+    STORAGE(node,storage_tec,mode,level,commodity,year,time) =G=
+* Initial content of storage in the examined time slice as a percentage multiplier in available capacity of storage
+        storage_initial(node,storage_tec,mode,level,commodity,year,time2)
+        * SUM(vintage$( map_tec_lifetime(node,storage_tec,vintage,year) ), capacity_factor(node,storage_tec,vintage,year,time2)
+             * CAP(node,storage_tec,vintage,year) / duration_time(time2)  )
+;
 ***
-* .. _equation_storage_equivalence:
+* .. _equation_storage_input:
 *
-* Equation STORAGE_EQUIVALENCE
+* Equation STORAGE_INPUT
 * """"""""""""""""""""""""""""
 *
-* This equation links :math:`\STORAGE` to activity (:math:`\ACT`) for each active storage *container* technology
-* :math:`t`; this is distinct from the *(dis)charge* technologies :math:`t^C,t^D` appearing in
+* This equation links :math:`\STORAGE` to an input commodity to maintain the activity (:math:`\ACT`) of each active storage *container* technology
+* :math:`t`. This input commodity is distinct from the stored commodity. For example, in a pumped hydro storage solution, a user can link heating
+* for keeping the stored water warm. In this case, the input commodity is not a function of charge or discharge, but the amount of stored media in the container over time.
+* Therefore, the input commodity specified here is distinct from the one stored and discharged by *(dis)charge* technologies :math:`t^C,t^D` appearing in
 * :ref:`equation_storage_change`.
 *
 * .. math::
-*    \STORAGE_{ntlcy^Ah} =\ & \sum_{\{n^Ly^Vh^O \vert K\}} \durationtimerel_{hh^O} \times \ACT_{n^Lty^Vy^Amh^O} \\
+*    \STORAGE_{ntmlcy^Ah} =\ & \sum_{\{n^Ly^Vh^O \vert K\}} \durationtimerel_{hh^O} \times \ACT_{n^Lty^Vy^Amh^O} \\
 *    \forall\ & n,t,l,c,m,y^A,h \vert t \in T^{STOR} \\
 *    K:\ & \input_{n^Lty^Vy^Amn^Oclhh^O} \neq 0
 *
 ***
 
-* Connecting an input commodity to maintain the operation of storage container over time (optional)
-STORAGE_EQUIVALENCE(node,storage_tec,level,commodity,level_storage,commodity2,mode,year,time)$
+STORAGE_INPUT(node,storage_tec,level,commodity,level_storage,commodity2,mode,year,time)$
     ( map_time_commodity_storage(node,storage_tec,level,commodity,mode,year,time) AND
-      SUM( tec, map_tec_storage(node,tec,storage_tec,level_storage,commodity2) ) )..
-
-         STORAGE(node,storage_tec,level_storage,commodity2,year,time) =E=
+      SUM( (tec,mode2,lvl_temporal), map_tec_storage(node,tec,mode2,storage_tec,mode,level_storage,commodity2,lvl_temporal) ) ) ..
+* Connecting an input commodity to maintain the operation of storage container over time (optional)
+  STORAGE(node,storage_tec,mode,level_storage,commodity2,year,time) =E=
         SUM( (location,vintage,time2)$(map_tec_lifetime(node,storage_tec,vintage,year)$(
-              input(location,storage_tec,vintage,year,mode,node,commodity,level,time2,time) ) ),
-              duration_time_rel(time,time2) * ACT(location,storage_tec,vintage,year,mode,time) );
+              input(location,storage_tec,vintage,year,mode,node,commodity,level,time,time2) ) ),
+              duration_time_rel(time,time2) * ACT(location,storage_tec,vintage,year,mode,time) )
+;
 
 *----------------------------------------------------------------------------------------------------------------------*
 * model statements                                                                                                     *
 *----------------------------------------------------------------------------------------------------------------------*
 
 Model MESSAGE_LP / all / ;
```

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/model_setup.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/model_setup.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/model_solve.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/model_solve.gms`

 * *Files 0% similar despite different names*

```diff
@@ -163,8 +163,8 @@
 COST_NODAL_NET.L(node, year)$(NOT macro_base_period(year)) = (
     COST_NODAL.L(node, year) + trade_cost(node, year)
 * subtract emission taxes applied at any higher nodal level (via map_node set)
     - sum((type_emission,emission,type_tec,type_year,node2)$( emission_scaling(type_emission,emission)
             AND map_node(node2,node) AND cat_year(type_year,year) ),
         emission_scaling(type_emission,emission) * tax_emission(node2,type_emission,type_tec,type_year)
         * EMISS.L(node,emission,type_tec,year) )
-) / 1000 ;
+) ;
```

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/parameter_def.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/parameter_def.gms`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 *
 * In |MESSAGEix|, all parameters are understood as yearly values, not as per (multi-year) period.
 * This provides flexibility when changing the resolution of the model horizon (i.e., the set ``year``).
 ***
 
 ***
 * .. _section_parameter_general:
+* .. _duration_time_rel:
 *
 * General parameters of the |MESSAGEix| implementation
 * ----------------------------------------------------
 *
 * .. caution::
 *
 *    Parameters written in **bold** are auxiliary parameters
@@ -48,15 +49,15 @@
 *    * - **df_period**
 *      - ``year``
 *      - Cumulative discount factor over period duration [#df_auto]_
 *    * - **df_year**
 *      - ``year``
 *      - Discount factor of the last year in the period [#df_auto]_
 *
-* .. [#duration_time_year] The element 'year' in the set of subannual time slices ``time`` has the value of 1.
+* .. [#duration_time_year] The element 'Year' in the set of subannual time slices ``time`` has the value of 1.
 *    This value is assigned by default when creating a new :class:`ixmp.Scenario` based on the ``MESSAGE`` scheme.
 *
 * .. [#short_dur] The short-hand notation :math:`|y|` is used for the parameters :math:`duration\_period_y`
 *    in the mathematical model documentation for exponents.
 *
 * .. [#year_auto] The values for this parameter are computed automatically when exporting a ``MESSAGE``-scheme
 *    :class:`ixmp.Scenario` to gdx.
@@ -145,15 +146,15 @@
 *
 * .. [#demand] The parameter ``demand`` in a ``MESSAGE``-scheme ``ixmp.Scenario`` is translated
 *    to the parameter ``demand_fixed`` in the |MESSAGEix| implementation in GAMS. The variable ``DEMAND`` is introduced
 *    as an auxiliary reporting variable; it equals ``demand_fixed`` in a `MESSAGE`-standalone run and reports
 *    the final demand including the price response in an iterative `MESSAGE-MACRO` solution.
 *
 * .. [#peakload] The parameters ``peak_load_factor`` (maximum peak load factor for reliability constraint of firm capacity) and
-*    ``reliability_factor`` (reliability of a technology (per rating)) are based on the formulation proposed by Sullivan et al., 2013 :cite:`sullivan_VRE_2013`.
+*    ``reliability_factor`` (reliability of a technology (per rating)) are based on the formulation proposed by Sullivan et al., 2013 :cite:`Sullivan-2013`.
 *    It is used in :ref:`reliability_constraint`.
 *
 ***
 
 Parameter
     demand_fixed(node,commodity,level,year_all,time)     exogenous demand levels
     peak_load_factor(node,commodity,level,year_all,time) maximum peak load factor for reliability constraint of firm capacity
@@ -213,14 +214,15 @@
 *
 * .. [#tecvintage] Fixed and variable cost parameters and technical specifications are indexed over both
 *    the year of construction (vintage) and the year of operation (actual).
 *    This allows to represent changing technology characteristics depending on the age of the plant.
 *
 * .. [#levelizedcost] The parameter ``levelized_cost`` is computed in the GAMS pre-processing under the assumption of
 *    full capacity utilization until the end of the technical lifetime.
+*    As these are calculated in the preprocessing, the reported ``levelized_cost`` in the output GDX-file exclude fuel costs.
 *
 * .. [#construction] The construction time only has an effect on the investment costs; in |MESSAGEix|,
 *    each unit of new-built capacity is available instantaneously at the beginning of the model period.
 *
 * .. [#rating] Maximum share of technology in commodity use per rating. The upper bound of a contribution by any technology to the constraints on system reliability
 *    (:ref:`reliability_constraint`) and flexibility (:ref:`flexibility_constraint`) can depend on the share of the technology output in the total commodity use at
 *    a specific level.
@@ -296,15 +298,15 @@
 ***
 * .. _section_parameter_dynamic_constraints:
 *
 * Dynamic constraints on new capacity and activity
 * ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 *
 * These parameters are used in the :ref:`dynamic constraint equations <dynamic_constraints>` to limit the growth (or decline) of activity or of new capacity in each period, relative to the preceding period.
-* The ``soft_`` parameters control ‘soft’ relaxation of these dynamic constraints, using the method of Keppo and Strubegger (2010) :cite:`keppo_short_2010`.
+* The ``soft_`` parameters control ‘soft’ relaxation of these dynamic constraints, using the method of Keppo and Strubegger (2010) :cite:`Keppo-2010`.
 *
 * The ``growth_`` and ``soft_`` parameters are expressed as *relative annual change* and are unitless.
 * Because these are annual values, are compounded in the :ref:`constraint equations <dynamic_constraints>` by ``duration_period`` (:math:`|y|`) to obtain the relative *inter-period* change.
 *
 * **Example:** a value of 0.05 for ``growth_activity_up`` sets an upper bound of :math:`1 + 0.05 = 105\%` activity in one year relative to activity in the preceding year.
 * In a period with duration :math:`|y| = 5 \text{ years}`, the activity in the :doc:`representative year </time>` is bounded at :math:`(1.05)^5 = 128\%` of the activity in the representative year of the preceding period.
 *
@@ -410,20 +412,20 @@
 *
 * Parameters for representing storage solutions
 * ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 *
 * The |MESSAGEix| formulation includes "storage" solutions to model sub-annual, inter-temporal storage of commodities in each period.
 * This feature can be used to model electricity storage (pumped hydro, batteries, compressed air energy storage, etc.), thermal energy storage,
 * demand side management, and in general any technology for storing commodities (gas, hydrogen, water, etc.) over sub-annual timesteps.
-* The user defines the chronological order of sub-annual time steps by assigning a number to them in parameter ``time_order``.
+* The user defines the chronological order of sub-annual time slices by assigning a number to them in parameter ``time_order``.
 * This order is used by storage equations to shift the stored commodity in a correct timeline, e.g., from Jan through to Dec, and not vice versa.
-* The last sub-annual timestep is linked to the first one to close the loop of the year. Parameter ``storage_initial`` is to set an initial amount
-* for the content of storage in any desirable timestep (optionally). This initial value is a cost-free stored media that storage can discharge
-* in the same or following timesteps. ``storage_self_discharge`` represents the self-discharge (loss) of storage as % of the level of stored media
-* in each timestep. This allows to model time-related losses in storage separately, in addition to charging and discharging losses.
+* The last sub-annual time slice is linked to the first one to close the loop of the year. Parameter ``storage_initial`` is to set an initial amount
+* for the content of storage in any desirable time slice (optionally). This initial value is a cost-free stored media that storage can discharge
+* in the same or following time slices. ``storage_self_discharge`` represents the self-discharge (loss) of storage as % of the level of stored media
+* in each time slice. This allows to model time-related losses in storage separately, in addition to charging and discharging losses.
 *
 * .. list-table::
 *    :widths: 20 80
 *    :header-rows: 1
 *
 *    * - Parameter name
 *      - Index names
@@ -433,31 +435,31 @@
 *      - ``node`` | ``tec`` | ``level`` | ``commodity`` | ``year_act`` | ``time``
 *    * - time_order
 *      - ``lvl_temporal`` | ``time``
 *
 ***
 
 Parameters
-    storage_initial(node,tec,level,commodity,year_all,time)                       initial content of storage
-    storage_self_discharge(node,tec,level,commodity,year_all,time)                self-discharge (loss) of storage as % of storage level in each timestep
-    time_order(lvl_temporal,time)                                                 sequence of subannual timesteps
+    storage_initial(node,tec,mode,level,commodity,year_all,time)                       initial content of storage
+    storage_self_discharge(node,tec,mode,level,commodity,year_all,time)                self-discharge (loss) of storage as % of storage level in each time slice
+    time_order(lvl_temporal,time)                                                 sequence of subannual time slices
 ;
 
 *----------------------------------------------------------------------------------------------------------------------*
 * Soft relaxations of dynamic constraints                                                                              *
 *----------------------------------------------------------------------------------------------------------------------*
 
 ***
 * .. _section_parameter_soft_constraints:
 *
 * Cost parameters for 'soft' relaxations of dynamic constraints
 * ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 *
 * The implementation of |MESSAGEix| includes the functionality for 'soft' relaxations of dynamic constraints on
-* new-built capacity and activity (see Keppo and Strubegger, 2010 :cite:`keppo_short_2010`).
+* new-built capacity and activity (see Keppo and Strubegger, 2010 :cite:`Keppo-2010`).
 * Refer to the section :ref:`dynamic_constraints`. Absolute cost and levelized cost multipliers are used
 * for the relaxation of upper and lower bounds.
 *
 * .. list-table::
 *    :widths: 20 80
 *    :header-rows: 1
 *
```

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/reporting.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/reporting.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/reporting_for_MACRO.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/reporting_for_MACRO.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/scaling_investment_costs.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/scaling_investment_costs.gms`

 * *Files 2% similar despite different names*

```diff
@@ -9,49 +9,51 @@
 
 * compute the technical lifetime remaining beyond the overall model horizon
 beyond_horizon_lifetime(node,inv_tec,vintage)$( map_tec(node,inv_tec,vintage) ) =
     technical_lifetime(node,inv_tec,vintage) - remaining_years(vintage) ;
 beyond_horizon_lifetime(node,inv_tec,vintage)$( beyond_horizon_lifetime(node,inv_tec,vintage) < 0 ) = 0 ;
 
 ***
-* Levelized capital costs
-* -----------------------
+* Levelized costs excluding fuel costs
+* ------------------------------------
 * For the 'soft' relaxations of the dynamic constraints and the associated penalty factor in the objective function,
 * we need to compute the parameter :math:`levelized\_cost_{n,t,y}`.
 *
 * .. math::
 *    levelized\_cost_{n,t,m,y,h} := \
 *        & inv\_cost_{n,t,y} \cdot \frac{ interestrate_{y} \cdot \left( 1 + interestrate_{y} \right)^{|y|} }
 *                                      { \left( 1 + interestrate_{y} \right)^{|y|} - 1 } \\
 *        & + fix\_cost_{n,t,y,y} \cdot \frac{ 1 }{ \sum_{h'} duration\_time_{h'} \cdot capacity\_factor_{n,t,y,y,h'} } \\
 *        & + var\_cost_{n,t,y,y,m,h}
 *
 * where :math:`|y| = technical\_lifetime_{n,t,y}`. This formulation implicitly assumes constant fixed
 * and variable costs over time.
 *
-* **Warning:** All soft relaxations of the dynamic activity constraint are
+* **Warning:** 
+* Levelized capital costs do not include fuel-related costs.
+* All soft relaxations of the dynamic activity constraint are
 * disabled if the levelized costs are negative!
 ***
 
-levelized_cost(node,tec,year,time)$( map_tec_time(node,tec,year,time) AND inv_tec(tec) ) =
-    inv_cost(node,tec,year)
+levelized_cost(node,tec,year,time)$( map_tec_time(node,tec,year,time)) =
+    (inv_cost(node,tec,year)
         * (
 * compute discounted annualized investment costs if interest rate > 0
             ( interestrate(year)
                 * ( 1 + interestrate(year) ) ** technical_lifetime(node,tec,year)
                 / ( ( 1 + interestrate(year) ) ** technical_lifetime(node,tec,year) - 1 )
               )$( interestrate(year) )
 * if interest rate = 0, annualized investment costs are total investment costs divided by technical lifetime
             + ( 1 / technical_lifetime(node,tec,year) )$( interestrate(year) eq 0 )
           )
 * add (proportional) fixed and variable costs, assuming that these remain constant over the technical lifetime
     + ( fix_cost(node,tec,year,year) /
           sum(time2$( map_tec_time(node,tec,year,time2) ),
              duration_time(time2) * capacity_factor(node,tec,year,year,time2) )
-        )$( fix_cost(node,tec,year,year) )
+        )$( fix_cost(node,tec,year,year) ))$(inv_tec(tec))
     + sum(mode$( map_tec_act(node,tec,year,mode,time) ), var_cost(node,tec,year,year,mode,time) )
 ;
 
 * the soft relaxations of the dynamic activity constraints are disabled if the levelized costs are negative
 loop((node,tec,year,time)$( levelized_cost(node,tec,year,time) < 0
         AND ( soft_activity_up(node,tec,year,time) + soft_activity_lo(node,tec,year,time) ) > 0 ),
     put_utility 'log' /'Remove relaxations for dynamic activity constraints for ',node.tl,'|',tec.tl,'|',year.tl,'!' ;
```

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/sets_maps_def.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/sets_maps_def.gms`

 * *Files 2% similar despite different names*

```diff
@@ -338,15 +338,15 @@
 *    * - Set name
 *      - Explanatory comments
 *    * - map_node(node,location)
 *      - Mapping of nodes across hierarchy levels (location is in node)
 *    * - map_time(time,time2)
 *      - Mapping of time periods across hierarchy levels (time2 is in time)
 *    * - map_time_period(year_all,lvl_temporal,time,time2)
-*      - Mapping of the sequence of sub-annual timesteps (used in :ref:`storage <gams-storage>`)
+*      - Mapping of the sequence of sub-annual timeslices (used in :ref:`storage <gams-storage>`)
 *    * - map_resource(node,commodity,grade,year_all)
 *      - Mapping of resources and grades to node over time
 *    * - map_ren_grade(node,commodity,grade,year_all)
 *      - Mapping of renewables and grades to node over time
 *    * - map_ren_com(node,tec,commodity,year_all)
 *      - Mapping of technologies to renewable energy source as input
 *    * - map_rating(node,tec,commodity,level,rating,year_all)
@@ -357,39 +357,39 @@
 *      - Mapping of commodity-level to node and time
 *    * - map_tec(node,tec,year_all)
 *      - Mapping of technology to node and years
 *    * - map_tec_time(node,tec,year_all,time)
 *      - Mapping of technology to temporal dissagregation (time)
 *    * - map_tec_mode(node,tec,year_all,mode)
 *      - Mapping of technology to modes
-*    * - map_tec_storage(node,tec,tec2,level,commodity)
+*    * - map_tec_storage(node,tec,mode,tec2,mode2,level,commodity,lvl_temporal)
 *      - Mapping of charge-discharge technologies ``tec`` to their storage container ``tec2``, stored ``commodity`` and ``level``.
 *    * - map_time_commodity_storage(node,tec,level,commodity,mode,year_all,time)
 *      - Mapping of storage containers to their input commodity-level (not commodity-level of stored media)
 ***
 
 Sets
     map_node(node,location)                            mapping of nodes across hierarchy levels (location is in node)
     map_time(time,time2)                               mapping of time periods across hierarchy levels (time2 is in time)
-    map_time_period(year_all,lvl_temporal,time,time2)  mapping of the sequence of sub-annual timesteps
+    map_time_period(year_all,lvl_temporal,time,time2)  mapping of the sequence of sub-annual time slices
 
     map_resource(node,commodity,grade,year_all)  mapping of resources and grades to node over time
     map_ren_grade(node,commodity,grade,year_all) mapping of renewables and grades to node over time
     map_ren_com(node,tec,commodity,year_all)     mapping of technologies to renewable energy source as input
     map_rating(node,tec,commodity,level,rating,year_all) mapping of technologies to ratings bin assignment
 
     map_commodity(node,commodity,level,year_all,time)    mapping of commodity-level to node and time
     map_stocks(node,commodity,level,year_all)    mapping of commodity-level to node and time
 
     map_tec(node,tec,year_all)                      mapping of technology to node and years
     map_tec_time(node,tec,year_all,time)            mapping of technology to temporal dissagregation (time)
     map_tec_mode(node,tec,year_all,mode)            mapping of technology to modes
     map_tec_act(node,tec,year_all,mode,time)        mapping of technology to modes AND temporal dissagregation
     map_tec_addon(tec,type_addon)                   mapping of types of add-on technologies to the underlying parent technology
-    map_tec_storage(node,tec,tec2,level,commodity)  mapping of charge-discharging technologies to their respective storage container tec and level-commodity
+    map_tec_storage(node,tec,mode,tec2,mode2,level,commodity,lvl_temporal)  mapping of charge-discharging technologies to their respective storage container tec and level-commodity
 
     map_spatial_hierarchy(lvl_spatial,node,node)    mapping of spatial resolution to nodes (last index is 'parent')
     map_temporal_hierarchy(lvl_temporal,time,time)  mapping of temporal resolution to time (last index is 'parent')
 
     map_shares_commodity_share(shares,node,
         node,type_tec,mode,commodity,level)   mapping for commodity share constraints (numerator)
     map_shares_commodity_total(shares,node,
```

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE/version_check.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE/version_check.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE-MACRO_run.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE-MACRO_run.gms`

 * *Files 10% similar despite different names*

```diff
@@ -93,15 +93,20 @@
     max_adjustment_pre maximum adjustment in previous iteration                     / 0 /
     max_adjustment_pos maximum positive adjustment in current iteration
     max_adjustment_neg maximum negative adjustment in current iteration
     max_adjustment     maximum adjustment in current iteration
     convergence_status status of convergence (1 if successful)                      / 0 /
     scaling            scaling factor to adjust step size when iteration oscillates / 1 /
     max_it             maximum number of iterations                                 / %MAX_ITERATION% /
-    ctr                iteration counter                                            /0/
+    ctr                iteration counter                                            / 0 /
+    obj_func_chng      change of objective function compared to iteration-1         / 0 /
+    obj_func_chng_pre  change of objective function of iteration-1 compared to iteration-2 / 0 /
+    obj_func_pre       objective function from iteration-1                          / 0 /
+    osc_check          tracks which oscillation check is used                       / 0 /
+    osc_check_final    tracks if any oscillation check has been triggered           / 0 /
 ;
 
 
 * declarations moved from solve files to avoid inclusion in loop
 Parameters
     demand_init(node,sector,year_all)
     demand_new(node,sector,year_all)
@@ -240,39 +245,83 @@
 max_adjustment_pos = smax((node_macro,sector,year)$( NOT macro_base_period(year) AND demand_scale(node_macro,sector,year) > 1),
     demand_scale(node_macro,sector,year) - 1 ) ;
 max_adjustment_neg = smin((node_macro,sector,year)$( NOT macro_base_period(year) AND demand_scale(node_macro,sector,year) < 1),
     demand_scale(node_macro,sector,year) - 1 ) ;
 max_adjustment = max_adjustment_pos ;
 max_adjustment$( max_adjustment_neg < - max_adjustment_pos ) = max_adjustment_neg ;
 
+* Add entries to log-file
 report_iteration(iteration, 'max adjustment pos') = max_adjustment_pos ;
 report_iteration(iteration, 'max adjustment neg') = -max_adjustment_neg ;
 report_iteration(iteration, 'absolute max adjustment max/min') = abs(max_adjustment) ;
 report_iteration(iteration, 'adjustment bound') = %MAX_ADJUSTMENT% / scaling ;
 
 * terminate iteration if convergence criterion is satisfied
 if ( abs(max_adjustment) < %CONVERGENCE_CRITERION%,
     convergence_status = 1 ;
     if ( ORD(iteration) = 1,
         put_utility 'log' /"+++ Convergence criteria satisfied after the first iteration +++ " ;
     else
         put_utility 'log' /"+++ Convergence criteria satisfied after ", ORD(iteration):0:0, " iterations +++ " ;
     ) ;
+    if ( osc_check_final = 1,
+        put_utility 'log' /"+++ Convergence achieved via oscillation check mechanism; check iteration log for further details +++ " ;
+    else
+        put_utility 'log' /"+++ Natural convergence achieved +++ " ;
+    ) ;
     break ;
 ) ;
 
-* check whether oscillation occurs during the iteration - if the sign of the adjusment switches, reduce maximum adjustment
+* Calculate change in objective function for use in oscillation check 3
+if ( ORD(iteration) > 1,
+    obj_func_chng = 1 - (OBJ.l / obj_func_pre);
+) ;
+
+* Perform oscillation checks:
+* Oscillation check 1: Does the sign of the `max_adjustment` parameter change?
 if ( ORD(iteration) > 1 AND sign(max_adjustment_pre) = -sign(max_adjustment)
         AND abs(max_adjustment_pre) > abs(max_adjustment) * 0.9,
     scaling = scaling * sqrt(2) ;
+    osc_check = 1 ;
+    osc_check_final = 1;
     put_utility 'log' /"+++ Indication of oscillation, increase the scaling parameter (", scaling:0:0, ") +++" ;
+* Oscillation check 2: Are the maximum-positive and maximum-negative adjustments equal to each other?
 elseif abs( max_adjustment_pos + max_adjustment_neg ) < 1e-4 ,
     scaling = scaling * sqrt(2) ;
-*    scaling = scaling + 1;
+    osc_check = 2 ;
+    osc_check_final = 1 ;
     put_utility 'log' /"+++ Indication of instability, increase the scaling parameter (", scaling:0:0, ") +++" ;
+* Oscillation check 3: Do the solutions jump between two objective functions?
+elseif ORD(iteration) > 2 AND abs(obj_func_chng_pre + obj_func_chng) < 1e-4 ,
+    scaling = scaling * sqrt(2) ;
+    osc_check = 3 ;
+    osc_check_final = 1;
+    put_utility 'log' /"+++ Indication of oscillating objective function, increase the scaling parameter (", scaling:0:0, ") +++" ;
+) ;
+
+* Add entry to log-file about which of the checks have been used.
+report_iteration(iteration, 'oscillation check') = osc_check ;
+* Reset check for next iteration.
+osc_check = 0;
+
+* Store current calculated change in objective function to *_pre* for use in the next iteration.
+obj_func_pre = OBJ.l
+if ( ORD(Iteration) > 1,
+    obj_func_chng_pre = obj_func_chng;
+) ;
+
+* In the case that the model solves with unscaled infeasibilities, the cplex options file `cplex.op2`
+* will be used which forces the use of `Dual Crossover` when solving with Barrier. This will avoid
+* solving further with unscaled infeasibilities.
+* When encountering unscaled infeasibilities, modelstat = 1 and solvestat = 4.
+
+if( MESSAGE_LP.solvestat = 4,
+   put_utility 'log' /'+++ Detected issues solving with unscaled infeasibilities. Enforcing Dual crossover +++ ' ;
+   MESSAGE_LP.optFile = 2;
+   report_iteration(iteration, 'unscaled infeasibilities') = 1 ;
 ) ;
 
 * store the maximum adjustment in this iteration for the oscillation-prevention query in the next iteration
 max_adjustment_pre = max_adjustment;
 
 * demand adjustment for next iteration (only implemented if convergence criterion not met)
 demand_fixed(node_macro,commodity,level,year,time) $(NOT macro_base_period(year) AND (SUM(sector $ mapping_macro_sector(sector, commodity, level), 1) > 0)) =
```

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE_master.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE_master.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/MESSAGE_run.gms` & `message_ix-3.7.0/message_ix/model/MESSAGE_run.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/includes/aux_computation_time.gms` & `message_ix-3.7.0/message_ix/model/includes/aux_computation_time.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/includes/period_parameter_assignment.gms` & `message_ix-3.7.0/message_ix/model/includes/period_parameter_assignment.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/model/version.gms` & `message_ix-3.7.0/message_ix/model/version.gms`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/models.py` & `message_ix-3.7.0/message_ix/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 import logging
 from collections import ChainMap
 from copy import copy, deepcopy
 from functools import lru_cache
 from pathlib import Path
+from warnings import warn
 
 import ixmp.model.gams
 from ixmp import config
+from ixmp.utils import maybe_check_out, maybe_commit
 
 from .macro import MACRO_ITEMS
 
 log = logging.getLogger(__name__)
 
-#: Solver options used by :meth:`message_ix.Scenario.solve`.
+#: Solver options used by :meth:`.Scenario.solve`.
 DEFAULT_CPLEX_OPTIONS = {
     "advind": 0,
-    "lpmethod": 2,
+    "lpmethod": 4,
     "threads": 4,
     "epopt": 1e-6,
 }
 
 # Abbreviations for index sets and index names; the same used in the inline
 # documentation of the GAMS code.
 _ABBREV = {
     "c": ("commodity", "commodity"),
     "e": ("emission", "emission"),
     "g": ("grade", "grade"),
     "l": ("level", "level"),
     "m": ("mode", "mode"),
+    "ms": ("mode", "storage_mode"),
     "n": ("node", "node"),
     "nd": ("node", "node_dest"),
     "nl": ("node", "node_loc"),
     "no": ("node", "node_origin"),
     "nr": ("node", "node_rel"),
     "ns": ("node", "node_share"),
     "r": ("rating", "rating"),
     "s": ("shares", "shares"),
     "t": ("technology", "technology"),
+    "ts": ("technology", "storage_tec"),
     "h": ("time", "time"),
     "hd": ("time", "time_dest"),
     "ho": ("time", "time_origin"),
     "y": ("year", "year"),
     "ya": ("year", "year_act"),
     "yr": ("year", "year_rel"),
     "yv": ("year", "year_vtg"),
@@ -70,15 +74,15 @@
         # Index names are distinct from index sets; also return these
         result["idx_names"] = names
 
     return result
 
 
 # NB order by ix_type (set, par, var, equ), then alphabetically.
-#: List of ixmp items for MESSAGE.
+#: ixmp items (sets, parameters, variables, and equations) for MESSAGE.
 MESSAGE_ITEMS = {
     # Index sets
     "commodity": dict(ix_type="set"),
     "emission": dict(ix_type="set"),
     "grade": dict(ix_type="set"),
     "land_scenario": dict(ix_type="set"),
     "land_type": dict(ix_type="set"),
@@ -130,15 +134,15 @@
     "map_spatial_hierarchy": dict(
         ix_type="set",
         idx_sets=["lvl_spatial", "node", "node"],
         idx_names=["lvl_spatial", "node", "node_parent"],
     ),
     "map_tec_addon": dict(ix_type="set", idx_sets=["technology", "type_addon"]),
     # Mapping of storage reservoir to charger/discharger
-    "map_tec_storage": item("set", "n t storage_tec l c"),
+    "map_tec_storage": item("set", "n t m ts ms l c lvl_temporal"),
     "map_temporal_hierarchy": dict(
         ix_type="set",
         idx_sets=["lvl_temporal", "time", "time"],
         idx_names=["lvl_temporal", "time", "time_parent"],
     ),
     "map_time": dict(
         ix_type="set", idx_sets=["time", "time"], idx_names=["time_parent", "time"]
@@ -241,31 +245,31 @@
     "share_mode_lo": item("par", "s ns t m ya h"),
     "share_mode_up": item("par", "s ns t m ya h"),
     "soft_activity_lo": item("par", "nl t ya h"),
     "soft_activity_up": item("par", "nl t ya h"),
     "soft_new_capacity_lo": item("par", "nl t yv"),
     "soft_new_capacity_up": item("par", "nl t yv"),
     # Initial amount of storage
-    "storage_initial": item("par", "n t l c y h"),
+    "storage_initial": item("par", "n t m l c y h"),
     # Storage losses as a percentage of installed capacity
-    "storage_self_discharge": item("par", "n t l c y h"),
+    "storage_self_discharge": item("par", "n t m l c y h"),
     "subsidy": item("par", "nl type_tec ya"),
     "tax_emission": dict(
         ix_type="par", idx_sets=["node", "type_emission", "type_tec", "type_year"]
     ),
     "tax": item("par", "nl type_tec ya"),
     "technical_lifetime": item("par", "nl t yv"),
-    # Order of sub-annual time steps
+    # Order of sub-annual time slices
     "time_order": dict(ix_type="par", idx_sets=["lvl_temporal", "time"]),
     "var_cost": item("par", "nl t yv ya m h"),
     #
-    # commented: for both variables and equations, ixmp_source requires that the
+    # commented: for certain variables and equations, ixmp_source requires that the
     # `idx_sets` and `idx_names` parameters be empty, but then internally uses the
     # correct sets and names to initialize.
-    # TODO adjust ixmp_source to accept these values, then uncomment.
+    # TODO adjust JDBCBackend to accept these values (or replace it), then uncomment.
     #
     # Variables
     #
     # # Activity
     # "ACT": item("var", "nl t yv ya m h"),
     # # Maintained capacity
     # "CAP": item("var", "nl t yv ya"),
@@ -280,14 +284,17 @@
     # # Objective (scalar)
     # "OBJ": dict(ix_type="var", idx_sets=[]),
     # # Relation (lhs)
     # "REL": item("var", "relation nr yr"),
     # # Stock
     # "STOCK": item("var", "n c l y"),
     #
+    "STORAGE": item("var", "n t m l c y h"),
+    "STORAGE_CHARGE": item("var", "n t m l c y h"),
+    #
     # # Equations
     # # Commodity balance
     # "RESOURCE_HORIZON": item("equ", "n c g"),
 }
 
 
 def _template(*parts):
@@ -317,31 +324,14 @@
             # Disable the feature to put input/output GDX files, list files, etc. in a
             # temporary directory
             "use_temp_dir": False,
         },
         ixmp.model.gams.GAMSModel.defaults,
     )
 
-    @classmethod
-    def initialize(cls, scenario):
-        """Set up *scenario* with required sets and parameters for MESSAGE.
-
-        See Also
-        --------
-        :data:`MESSAGE_ITEMS`
-        """
-        # Initialize the ixmp items
-        cls.initialize_items(scenario, MESSAGE_ITEMS)
-
-    @staticmethod
-    def enforce(scenario):
-        """Enforce data consistency in `scenario`."""
-        # No-op; implemented in MESSAGE sub-class, below
-        # TODO make this an optional method of the ixmp.model.base.Model abstract class
-
     def __init__(self, name=None, **model_options):
         # Update the default options with any user-provided options
         model_options.setdefault("model_dir", config.get("message model dir"))
         self.cplex_opts = copy(DEFAULT_CPLEX_OPTIONS)
         self.cplex_opts.update(config.get("message solve options") or dict())
         self.cplex_opts.update(model_options.pop("solve_options", {}))
 
@@ -369,35 +359,80 @@
 
         # Write CPLEX options into an options file
         optfile = Path(self.model_dir).joinpath("cplex.opt")
         lines = ("{} = {}".format(*kv) for kv in self.cplex_opts.items())
         optfile.write_text("\n".join(lines))
         log.info(f"Use CPLEX options {self.cplex_opts}")
 
-        try:
-            result = super().run(scenario)
-        finally:
-            # Remove the optfile regardless of whether the run completed without error.
-            # The file may have been removed already by another run (in a separate
-            # process) that completed before this one.
-            # py37 compat: check for existence instead of using unlink(missing_ok=True)
-            if optfile.exists():
-                optfile.unlink()
+        self.cplex_opts.update({"barcrossalg": 2})
+        optfile2 = Path(self.model_dir).joinpath("cplex.op2")
+        lines2 = ("{} = {}".format(*kv) for kv in self.cplex_opts.items())
+        optfile2.write_text("\n".join(lines2))
+
+        result = super().run(scenario)
+
+        # In previous versions, the `cplex.opt` file(s) were removed at this point
+        # in the workflow. This has been removed due to issues when running
+        # scenarios asynchronously.
 
         return result
 
 
+def _check_structure(scenario):
+    """Check dimensionality of some items related to the storage representation.
+
+    Yields a sequence of 4-tuples:
+
+    1. Item name.
+    2. Item ix_type.
+    3. Number of data points in the item; -1 if it does not exist in `scenario`.
+    4. A warning/error message, *if* the index names/sets do not match those in
+       `MESSAGE_ITEMS` and the item contains data. Otherwise, the message is an empty
+       string.
+    """
+    if scenario.has_solution():
+        return
+
+    # NB could rename this e.g. _check_structure_0 if there are multiple such methods
+    for name in ("storage_initial", "storage_self_discharge", "map_tec_storage"):
+        info = MESSAGE_ITEMS[name]
+        message = ""
+
+        try:
+            # Retrieve the index names and data length of the item
+            idx_names = tuple(scenario.idx_names(name))
+            N = len(getattr(scenario, info["ix_type"])(name))
+        except KeyError:
+            N = -1  # Item does not exist
+        else:
+            # Item exists
+            expected_names = info.get("idx_names", info["idx_sets"])
+            if expected_names != idx_names and N > 0:
+                message = (
+                    f"{info['ix_type']} {name!r} has data with dimensions {idx_names!r}"
+                    f" != {expected_names!r} and cannot be solved; try expand_dims()"
+                )
+        finally:
+            yield name, info["ix_type"], N, message
+
+
 class MESSAGE(GAMSModel):
     """Model class for MESSAGE."""
 
     name = "MESSAGE"
 
     @staticmethod
     def enforce(scenario):
         """Enforce data consistency in `scenario`."""
+        # Raise an exception if any of the storage items have incorrect dimensions, i.e.
+        # non-empty error messages
+        messages = list(filter(None, [msg for *_, msg in _check_structure(scenario)]))
+        if messages:
+            raise ValueError("\n".join(messages))
+
         # Check masks ("mapping sets") that indicate which elements of corresponding
         # parameters are active/non-zero. Note that there are other masks currently
         # handled in JDBCBackend. For the moment, this code does not backstop that
         # behaviour.
         # TODO Extend to handle all masks, e.g. for new backends.
         for par_name in ("capacity_factor",):
             # Name of the corresponding set
@@ -411,14 +446,39 @@
                 continue  # Contents are as expected; do nothing
 
             # Not consistent; empty and then re-populate the set
             with scenario.transact(f"Enforce consistency of {set_name} and {par_name}"):
                 scenario.remove_set(set_name, existing)
                 scenario.add_set(set_name, expected)
 
+    @classmethod
+    def initialize(cls, scenario):
+        """Set up *scenario* with required sets and parameters for MESSAGE.
+
+        See Also
+        --------
+        :data:`MESSAGE_ITEMS`
+        """
+        # Check for storage items that may contain incompatible data or need to be
+        # re-initialized
+        state = None
+        for name, ix_type, N, message in _check_structure(scenario):
+            if len(message):
+                warn(message)  # Existing, incompatible data → conspicuous warning
+            elif N == 0:
+                # Existing, empty item → remove, even if it has the correct dimensions.
+                state = maybe_check_out(scenario, state)
+                getattr(scenario, f"remove_{ix_type}")(name)
+
+        # Initialize the ixmp items for MESSAGE
+        cls.initialize_items(scenario, MESSAGE_ITEMS)
+
+        # Commit if anything was removed
+        maybe_commit(scenario, state, f"{cls.__name__}.initialize")
+
 
 class MACRO(GAMSModel):
     """Model class for MACRO."""
 
     name = "MACRO"
 
     #: MACRO uses the GAMS ``break;`` statement, and thus requires GAMS 24.8.1 or later.
@@ -465,7 +525,12 @@
                 continue
 
         # Let the parent constructor handle other solve_args
         super().__init__(*args, **kwargs)
 
         # Append to the prepared solve_args
         self.solve_args.extend(mm_iter_args)
+
+    @classmethod
+    def initialize(cls, scenario, with_data=False):
+        MESSAGE.initialize(scenario)
+        MACRO.initialize(scenario, with_data)
```

### Comparing `message_ix-3.6.0/message_ix/reporting/__init__.py` & `message_ix-3.7.0/message_ix/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/reporting/computations.py` & `message_ix-3.7.0/message_ix/reporting/computations.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/reporting/pyam.py` & `message_ix-3.7.0/message_ix/reporting/pyam.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Callable
+from typing import Callable, Optional
 
 import pandas as pd
 from genno.compat.pyam import util
 
 
 def collapse_message_cols(
-    df: pd.DataFrame, var: str = None, kind: str = None, var_cols=[]
+    df: pd.DataFrame, var: Optional[str] = None, kind: Optional[str] = None, var_cols=[]
 ) -> Callable:
     """:func:`.as_pyam` `collapse=...` callback for MESSAGEix quantities.
 
     Wraps :func:`.collapse` with arguments particular to MESSAGEix.
 
     Parameters
     ----------
```

### Comparing `message_ix-3.6.0/message_ix/testing/__init__.py` & `message_ix-3.7.0/message_ix/testing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 appliances
 bulb                      0.1    1     5
 cfl                  0.0  0.1   10   900
 """,
 )
 
 
-def make_austria(mp, solve=False, quiet=True):
+# FIXME reduce complexity from 18 to <=14
+def make_austria(mp, solve=False, quiet=True):  # noqa: C901
     """Return an :class:`message_ix.Scenario` for the Austrian energy system.
 
     This is the same model used in the ``austria.ipynb`` tutorial.
 
     Parameters
     ----------
     mp : ixmp.Platform
@@ -420,15 +421,17 @@
     scen.add_timeseries(HIST_DF, meta=True)
     scen.add_timeseries(INP_DF)
     scen.commit("Import Dantzig's transport problem for testing.")
 
     return scen
 
 
-def make_westeros(mp, emissions=False, solve=False, quiet=True):
+def make_westeros(
+    mp, emissions=False, solve=False, quiet=True, model_horizon=[700, 710, 720]
+):
     """Return an :class:`message_ix.Scenario` for the Westeros model.
 
     This is the same model used in the ``westeros_baseline.ipynb`` tutorial.
 
     Parameters
     ----------
     mp : ixmp.Platform
@@ -440,15 +443,14 @@
     """
     mp.add_unit("USD/kW")
     mp.add_unit("tCO2/kWa")
     scen = Scenario(mp, version="new", **SCENARIO["westeros"])
 
     # Sets
     history = [690]
-    model_horizon = [700, 710, 720]
     scen.add_horizon(year=history + model_horizon, firstmodelyear=model_horizon[0])
     year_df = scen.vintage_and_active_years()
     vintage_years, act_years = year_df["year_vtg"], year_df["year_act"]
 
     country = "Westeros"
     scen.add_spatial_sets({"country": country})
 
@@ -472,15 +474,33 @@
         time_origin="year",
         time="year",
         year_act=act_years,
         year_vtg=vintage_years,
         year=model_horizon,
     )
 
-    gdp_profile = np.array([1.0, 1.5, 1.9])
+    gdp_profile = pd.DataFrame({"years": [700, 710, 720], "values": [1.0, 1.5, 1.9]})
+    missing_years = [y for y in model_horizon if y not in set(gdp_profile.years)]
+    if missing_years:
+        gdp_profile = pd.concat(
+            [
+                gdp_profile,
+                pd.DataFrame(
+                    {"years": missing_years, "values": [np.nan] * len(missing_years)}
+                ),
+            ]
+        )
+        # Interpolate missing years
+        gdp_profile = (
+            gdp_profile.sort_values(by="years")
+            .set_index("years")
+            .interpolate(how="index", limit_direction="both")
+            .reset_index()
+        )
+    gdp_profile = np.array(gdp_profile.set_index("years")["values"])
     demand_per_year = 40 * 12 * 1000 / 8760
     scen.add_par(
         "demand",
         make_df(
             "demand",
             **common,
             commodity="light",
@@ -595,14 +615,15 @@
     time_steps,
     demand,
     time_relative=[],
     com_dict={"gas_ppl": {"input": "fuel", "output": "electr"}},
     capacity={"gas_ppl": {"inv_cost": 0.1, "technical_lifetime": 5}},
     capacity_factor={},
     var_cost={},
+    operation_factor={},
 ):
     """Return an :class:`message_ix.Scenario` with subannual time resolution.
 
     The scenario contains a simple model with two technologies, and a number of time
     slices.
 
     Parameters
@@ -628,14 +649,16 @@
         (e.g., ``com_dict = {"gas_ppl": {"input": "fuel", "output": "electr"}}``)
     capacity : dict, optional
         Data for "inv_cost" and "technical_lifetime" per technology.
     capacity_factor : dict, optional
         "capacity_factor" with technology as key and "time"/"value" pairs as value.
     var_cost : dict, optional
         "var_cost" with technology as key and "time"/"value" pairs as value.
+    operation_factor : dict, optional
+        "operation_factor" with technology as key and "value" as value.
     """
     # Get the `test_mp` fixture for the requesting test function
     mp = request.getfixturevalue("test_mp")
 
     # Build an empty scenario
     scen = Scenario(mp, request.node.name, scenario="test", version="new")
 
@@ -652,32 +675,34 @@
     scen.add_set("year", y)
     scen.add_set("type_year", y)
     scen.add_set("mode", "mode")
 
     scen.add_set("technology", list(tec_dict.keys()))
 
     # Add "time" and "duration_time" to the model
-    for (h, dur, tmp_lvl, parent) in time_steps:
+    for h, dur, tmp_lvl, parent in time_steps:
         scen.add_set("time", h)
         scen.add_set("time", parent)
         scen.add_set("lvl_temporal", tmp_lvl)
         scen.add_set("map_temporal_hierarchy", [tmp_lvl, h, parent])
         scen.add_par("duration_time", [h], dur, "-")
 
     scen.add_set("time_relative", time_relative)
 
     # Common dimensions for parameter data
     common = dict(
         node="node",
         node_loc="node",
+        node_rel="node",
         mode="mode",
         level="level",
         year=y,
         year_vtg=y,
         year_act=y,
+        year_rel=y,
     )
 
     # Define demand; unpack (key, value) pairs into individual pd.DataFrame rows
     df = make_df(
         "demand",
         **common,
         commodity="electr",
@@ -719,11 +744,22 @@
     for name, arg in [("capacity_factor", capacity_factor), ("var_cost", var_cost)]:
         for tec, data in arg.items():
             df = make_df(
                 name, **common, technology=tec, time=data.keys(), value=data.values()
             )
             scen.add_par(name, df)
 
+    # Add operation factor and an arbitrary relation (optional)
+    for name, arg in [("operation_factor", operation_factor)]:
+        for tec, data in arg.items():
+            df = make_df(name, **common, technology=tec, value=data)
+            scen.add_par(name, df)
+            # Arbitray relation to create "map_tec_relation". This is for testing
+            # average capacity factor, used for calculating "operation_factor"
+            scen.add_set("relation", "yearly_activity")
+            common.update(relation="yearly_activity", technology=tec, value=1)
+            scen.add_par("relation_activity", make_df("relation_activity", **common))
+
     scen.commit(f"Scenario with subannual time resolution for {request.node.name}")
     scen.solve()
 
     return scen
```

### Comparing `message_ix-3.6.0/message_ix/testing/nightly.py` & `message_ix-3.7.0/message_ix/testing/nightly.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/conftest.py` & `message_ix-3.7.0/message_ix/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 def ureg():
     """Session-scoped :class:`pint.UnitRegistry` with units needed by tests."""
     registry = pint.get_application_registry()
 
     for unit in "USD", "case":
         try:
             registry.define(f"{unit} = [{unit}]")
-        except pint.DefinitionSyntaxError:
+        except (pint.RedefinitionError, pint.DefinitionSyntaxError):
             # Already defined
             pass
 
     yield registry
 
 
 @pytest.fixture
```

### Comparing `message_ix-3.6.0/message_ix/tests/data/legacy.lobs` & `message_ix-3.7.0/message_ix/tests/data/legacy.lobs`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/data/legacy.script` & `message_ix-3.7.0/message_ix/tests/data/legacy.script`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/data/multiregion_macro_input.xlsx` & `message_ix-3.7.0/message_ix/tests/data/multiregion_macro_input.xlsx`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/data/report-pyam-write.csv` & `message_ix-3.7.0/message_ix/tests/data/report-pyam-write.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Model,Scenario,Region,Variable,Unit,1963
 Canning problem (MESSAGE scheme),standard,san-diego,Activity|canning_plant|production,,600.0
 Canning problem (MESSAGE scheme),standard,san-diego,Activity|transport_from_san-diego|to_chicago,,0.0
-Canning problem (MESSAGE scheme),standard,san-diego,Activity|transport_from_san-diego|to_new-york,,275.0
+Canning problem (MESSAGE scheme),standard,san-diego,Activity|transport_from_san-diego|to_new-york,,325.0
 Canning problem (MESSAGE scheme),standard,san-diego,Activity|transport_from_san-diego|to_topeka,,275.0
 Canning problem (MESSAGE scheme),standard,seattle,Activity|canning_plant|production,,350.0
 Canning problem (MESSAGE scheme),standard,seattle,Activity|transport_from_seattle|to_chicago,,300.0
-Canning problem (MESSAGE scheme),standard,seattle,Activity|transport_from_seattle|to_new-york,,50.0
+Canning problem (MESSAGE scheme),standard,seattle,Activity|transport_from_seattle|to_new-york,,0.0
 Canning problem (MESSAGE scheme),standard,seattle,Activity|transport_from_seattle|to_topeka,,0.0
```

### Comparing `message_ix-3.6.0/message_ix/tests/data/scenarios.yaml` & `message_ix-3.7.0/message_ix/tests/data/scenarios.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
   model: CD_Links_SSP2
   scenario: baseline
   solve: MESSAGE-MACRO
   solve_options:
     lpmethod: 4
   cases: # Each entry in this list is eval()'d in Python, so must be a string
   - obs: scen.var('OBJ')['lvl']
-    exp: '3870157.5'
+    exp: '3869529.75'
     test: partial(np.isclose, rtol=3e-6)  # not sure why 1e-6 doesn't work
 
 CD_Links_SSP2_v2_1000:
   model: CD_Links_SSP2_v2
   scenario: NPi2020_1000-con-prim-dir-ncr
   solve: MESSAGE-MACRO
   solve_options:
     lpmethod: 4
   cases:
   - obs: scen.var('OBJ')['lvl']
-    exp: '3358441.5'
+    exp: '3359089.0'
     test: partial(np.isclose, rtol=3e-6)  # not sure why 1e-6 doesn't work
```

### Comparing `message_ix-3.6.0/message_ix/tests/data/westeros_macro_input.xlsx` & `message_ix-3.7.0/message_ix/tests/data/westeros_macro_input.xlsx`

 * *Files 17% similar despite different names*

```diff
@@ -109,1378 +109,1366 @@
 000006c0: 374d af69 cb7a 6fc9 a523 2b90 a644 ce90  7M.i.zo..#+..D..
 000006d0: 59f8 90d9 42ea f335 a256 a1a5 24c1 b07e  Y...B..5.V..$..~
 000006e0: cae9 88ca fb22 6303 1e27 5afd 9fe8 ef6b  ....."c..'Z....k
 000006f0: d152 5246 2585 9a03 9de6 f9ec 3805 b4bc  .RRF%.......8...
 00000700: a445 7313 7fdc 9946 7ce7 30bc 320f a758  .Es....F|.0.2..X
 00000710: 6e2f c9a2 f731 b13d 63ce 57cf 3712 cede  n/...1.=c.W.7...
 00000720: b2fa 0000 00ff ff03 0050 4b03 0414 0006  .........PK.....
-00000730: 0008 0000 0021 0006 2513 c833 0400 00c9  .....!..%..3....
+00000730: 0008 0000 0021 0031 c744 201b 0400 00a9  .....!.1.D .....
 00000740: 0a00 000f 0000 0078 6c2f 776f 726b 626f  .......xl/workbo
-00000750: 6f6b 2e78 6d6c a456 516f a338 107e 3fe9  ok.xml.VQo.8.~?.
-00000760: fe03 e29d 0513 2001 355d 3524 e82a b5ab  ...... .5]5$.*..
-00000770: a8ed b62f 9122 074c e22b 60ce 366d aad5  .../.".L.+`.6m..
-00000780: fef7 1d9b 8490 e474 ca75 a3d6 18fb f3f0  .......t.u......
-00000790: cdcc 3703 575f b765 61bc 112e 28ab c626  ..7.W_.ea...(..&
-000007a0: fae2 9806 a952 96d1 6a3d 36bf 3f25 d6c8  .....R..j=6.?%..
-000007b0: 3484 c455 860b 5691 b1f9 4184 f9f5 facf  4..U..V...A.....
-000007c0: 3fae de19 7f5d 31f6 6a80 814a 8ccd 8d94  ?....]1.j..J....
-000007d0: 7564 db22 dd90 128b 2fac 2615 ece4 8c97  ud."..../.&.....
-000007e0: 58c2 2d5f dba2 e604 6762 4388 2c0b db75  X.-_....gbC.,..u
-000007f0: 9cc0 2e31 adcc d642 c42f b1c1 f29c a664  ...1...B./.....d
-00000800: cad2 a624 956c 8d70 5260 09f4 c586 d662  ...$.l.pR`.....b
-00000810: 6fad 4c2f 3157 62fe dad4 56ca ca1a 4cac  o.L/1Wb...V...L.
-00000820: 6841 e587 366a 1a65 1add ae2b c6f1 aa00  hA..6j.e...+....
-00000830: b7b7 c837 b61c fe02 f847 0e0c eefe 49b0  ...7.....G....I.
-00000840: 75f6 a892 a69c 0996 cb2f 60da 6e49 9ff9  u......../`.nI..
-00000850: 8f1c 1ba1 a310 6ccf 6370 9925 cfe6 e48d  ......l.cp.%....
-00000860: aa1c 76ac 78f0 4956 4167 2b38 1843 ce6f  ..v.x.IVAg+8.C.o
-00000870: 5b43 202d ad95 0882 f749 6b7e c7cd 35af  [C -.....Ik~..5.
-00000880: af72 5a90 e756 ba06 aeeb 6fb8 5499 2a4c  .rZ..V....o.T.*L
-00000890: a3c0 42ce 322a 4936 3687 70cb dec9 d102  ..B.2*I66.p.....
-000008a0: 6fea 4943 0bd8 75bd 7080 4cfb ba93 f39c  o.IC..u.p.L.....
-000008b0: 1b19 c971 53c8 2710 f2de 3c54 4610 84ae  ...qS.'...<TF...
-000008c0: af90 208c 9b42 125e 6149 6256 49d0 e1ce  .. ..B.^aIbVI...
-000008d0: afdf d59c b61d 6f18 28dc 7820 ff34 9413  ......o.(.x .4..
-000008e0: 282c d017 f80a 234e 23bc 1273 2c37 46c3  (,....#N#..s,7F.
-000008f0: 8bb1 1947 8bef 02dc 5f14 b8e1 7831 e76c  ...G...._...x1.l
-00000900: cd71 5942 e5c2 f46f 924a b1b8 c3cd 0b25  .qYB...o.J.....%
-00000910: d5a2 2442 e035 59d2 6d7f 2a21 2a62 9161  ..$B.5Y.m.*!*b.a
-00000920: 8917 3d31 e3f3 caf9 1f72 c6a9 8a91 0d41  ..=1.....r.....A
-00000930: 6a1d 69e7 a701 037f 78b4 97ec 5c72 03e6  j.i.....x...\r..
-00000940: b7d3 3b48 db23 7e83 2482 54b2 5d8d df42  ..;H.#~.$.T.]..B
-00000950: 96d0 6059 a53c 42cb 1f37 d341 ec8d 2653  ..`Y.<B..7.A..&S
-00000960: 6b84 dcd0 f292 11b2 6e66 716c 0d47 8349  k.......nfql.G.I
-00000970: 3099 4c93 e170 f613 9ce1 4194 32dc c8cd  0.L..p....A.2...
-00000980: 4e1f caf4 d8f4 400c 675b f778 bbdf 414e  N.....@.g[.x..AN
-00000990: d4d0 ec40 e387 b3fb 59ea 7a32 ecf7 7e2a  ...@....Y.z2..~*
-000009a0: 8755 277c a6e4 5d1c 94a4 6e8d ed0b ad32  .U'|..]...n....2
-000009b0: f6ae 3dfa d8cf 911f 8083 ef7a e785 6672  ..=........z..fr
-000009c0: 031e 0e87 9ebf 5ffb 8bd0 f506 e882 8b6a  ......_........j
-000009d0: 51e2 d583 6a70 6333 1c86 a681 5349 dfc8  Q...jpc3....SI..
-000009e0: 135e 0140 b9e3 2ace 63f3 88eb b4e5 9ac0  .^.@..*.c.......
-000009f0: cf52 c311 57bb 4756 7763 20ad af46 a52b  .R..W.GVwc ..F.+
-00000a00: a8e6 20c0 2527 3974 7ed5 ac75 064c 8347  .. .%'9t~..u.L.G
-00000a10: ea31 fc36 d3f5 d23f 9032 214f f0d0 1d3b  .1.6...?.2!O...;
-00000a20: bcab 02d4 c767 f086 a8b2 9313 83de 89c1  .....g..........
-00000a30: e989 8249 0675 ddd1 f17a 60ef 144c 44b3  ...I.u...z`..LD.
-00000a40: ea61 2182 1d15 5dc0 4754 3854 710f 0c2d  .a!...].GT8Tq..-
-00000a50: af03 07e7 bc6b dec3 8298 3aec f014 fb5a  .....k....:....Z
-00000a60: bfc1 bba8 230c 6fd1 0e3b 3ac3 aeb3 ba87  ....#.o..;:.....
-00000a70: 851c 77d8 f014 0bd0 658a 0bba 3a21 aeba  ..w.....e...:!..
-00000a80: eb21 43ce e931 4c08 eda7 1394 7340 9f25  .!C..1L.....s@.%
-00000a90: f47e f620 d97c 3eef 9fe8 6714 9da5 3465  .~. .|>...g...4e
-00000aa0: 554e d77d 7c3f 9f48 27d4 de8b 0df8 a7d0  UN.}|?.H'.......
-00000ab0: 67d5 456b 2b44 8eab 1d25 5b79 27e4 f515  g.Ek+D...%[y'...
-00000ac0: 5ca1 c551 10f5 c41f 4d9c 41e8 42a9 a3c4  \..Q....M.A.B...
-00000ad0: f250 e858 9349 e059 fe34 19f8 4334 8d67  .P.X.I.Y.4..C4.g
-00000ae0: 7ea2 ea5d 7d83 445b 6531 ffe4 ab65 64eb  ~..]}.D[e1...ed.
-00000af0: d304 cb06 daae eab8 fa3e 5263 b25b ed16  .........>Rc.[..
-00000b00: f376 6157 3047 ed31 7a98 aae0 ef4e ff17  .vaW0G.1z....N..
-00000b10: f011 3a75 412e 0427 cf17 02e3 6ff7 4ff7  ..:uA..'....o.O.
-00000b20: 1762 ef66 4fcb 9744 37ec 7ff5 d686 44f4  .b.fO..D7.....D.
-00000b30: b331 0cdc 201e 05ae e5de a081 85d0 ccb7  .1.. ...........
-00000b40: 2603 cfb7 9259 029d 388c a771 78c8 46c1  &....Y..8..qx.F.
-00000b50: e0f4 5932 9472 49fb 41a4 3f0a 21d0 1a18  ..Y2.rI.A.?.!...
-00000b60: 0138 6e75 2124 87c8 3c90 fcf1 a392 aa39  .8nu!$..<......9
-00000b70: cfb6 2929 6eb4 4a5b 466a d442 b1f7 5fa1  ..))n.J[Fj.B.._.
-00000b80: d7bf 0000 00ff ff03 0050 4b03 0414 0006  .........PK.....
-00000b90: 0008 0000 0021 0029 001d 8f55 0100 00e7  .....!.)...U....
-00000ba0: 0900 001a 0008 0178 6c2f 5f72 656c 732f  .......xl/_rels/
-00000bb0: 776f 726b 626f 6f6b 2e78 6d6c 2e72 656c  workbook.xml.rel
-00000bc0: 7320 a204 0128 a000 0100 0000 0000 0000  s ...(..........
+00000750: 6f6b 2e78 6d6c a456 5d6f a338 147d 5f69  ok.xml.V]o.8.}_i
+00000760: ff03 f23b 0513 2009 6a3a ca17 da4a ed28  ...;.. .j:...J.(
+00000770: 4abb ed4b a5c8 0193 5805 ccda a649 359a  J..K....X....I5.
+00000780: ff3e d790 1042 56ab 6c07 2506 dbc7 97e3  .>...BV.l.%.....
+00000790: 7bcf bdf8 f6db 3e4b 8d0f 2a24 e3f9 08e1  {.....>K..*$....
+000007a0: 1b1b 1934 8f78 ccf2 cd08 fdfd 1c9a 0364  ...4.x.........d
+000007b0: 4845 f298 a43c a723 f449 25fa 76f7 e71f  HE...<.#.I%.v...
+000007c0: b73b 2ede d79c bf1b 6020 9723 b455 aa08  .;......` .#.U..
+000007d0: 2c4b 465b 9a11 79c3 0b9a c34c c245 4614  ,KF[..y....L.EF.
+000007e0: 74c5 c692 85a0 2496 5b4a 5596 5a8e 6dfb  t.....$.[JU.Z.m.
+000007f0: 5646 588e 6a0b 81b8 c606 4f12 16d1 198f  VFX.j.....O.....
+00000800: ca8c e6aa 3622 684a 14d0 975b 56c8 a3b5  ....6"hJ...[V...
+00000810: 2cba c65c 46c4 7b59 9811 cf0a 30b1 6629  ,..\F.{Y....0.f)
+00000820: 539f 9551 6464 5170 bfc9 b920 eb14 b6bd  S..QddQp... ....
+00000830: c79e b117 f0f3 e18f 6d68 9ce3 9b60 eae2  ........mh...`..
+00000840: 5519 8b04 973c 5137 60da aa49 5fec 1fdb  U....<Q7`..I_...
+00000850: 16c6 672e d85f fae0 3a4b ae25 e807 d331  ..g.._..:K.%...1
+00000860: 6c58 09ff 8bac fcc6 967f 3286 eddf b686  lX........2.....
+00000870: 415a 9556 0270 de17 ad79 0d37 07dd dd26  AZ.V.p...y.7...&
+00000880: 2ca5 2fb5 740d 5214 df49 a623 9522 2325  ,./.t.R..I.#."#%
+00000890: 52cd 63a6 683c 427d e8f2 1d3d 1b10 6531  R.c.h<B}...=..e1
+000008a0: 2959 0ab3 4e6f e80c 9175 d7c8 7921 8c98  )Y..No...u..y!..
+000008b0: 26a4 4cd5 3308 f968 1e32 c3f7 878e a791  &.L.3..h.2......
+000008c0: 208c 71aa a8c8 89a2 539e 2bd0 e161 5fbf   .q.....S.+..a_.
+000008d0: abb9 caf6 74cb 41e1 c692 fe53 3241 21b1  ....t.A....S2A!.
+000008e0: 405f b057 6849 1490 b55c 10b5 354a 918e  @_.WhI...\..5J..
+000008f0: d034 785b d282 bf65 544a b2a1 2bb6 6f3f  .4x[...eTJ..+.o?
+00000900: 2ad8 b27c 8b89 226f 2da5 92cb b4f8 1f5a  *..|.."o-......Z
+00000910: 2591 7680 051e a859 d6cf 5d6f 0059 111c  %.v....Y..]o.Y..
+00000920: f5b8 50c2 80e7 fbd9 03c4 e489 7c40 8440  ..P.........|@.@
+00000930: 07f1 2181 ef21 04b8 b7ca 2311 e0d5 8f69  ..!..!....#....i
+00000940: 7f10 86e3 b16b 62c7 0e4d d777 e7e6 c0b6  .....kb..M.w....
+00000950: 7b66 184e 301e bb76 6fdc 777f c266 841f  {f.N0..vo.w..f..
+00000960: 449c 946a 7b08 be36 3d42 ae96 6b77 ea91  D..j{..6=B..kw..
+00000970: ec61 0634 a0b3 3628 597c a2f1 c33e 5ca6  .a.4..6(Y|...>\.
+00000980: be77 9ae3 dc4f bd61 5de6 5e18 ddc9 934c  .w...O.a].^....L
+00000990: 74d7 d8bf b23c e6bb 11d2 8491 f179 dedd  t....<.......y..
+000009a0: 5593 af2c 565b d0d9 d076 0152 8ffd 45d9  U..,V[...v.R..E.
+000009b0: 660b 8cb1 37d0 838a ac97 ba80 8dd0 b03f  f...7..........?
+000009c0: 4406 8914 fba0 cf64 0d00 cddb d1b4 47e8  D......d......G.
+000009d0: 8cee aca6 1bc2 05de 09c3 33ba 568b 6f55  ..........3.V.oU
+000009e0: 6d81 7775 37f2 2a43 0a01 025b 099a 4065  m.wu7.*C...[..@e
+000009f0: d7c5 b80a 0232 44a0 5f23 ee63 acf7 dc5e  .....2D._#.c...^
+00000a00: 1071 a93a 78a8 7e0d dee9 e263 f802 e471  .q.:x.~....c...q
+00000a10: 6745 afb5 a2d7 5d91 72c5 216f 1b3a 6e0b  gE....].r.!o.:n.
+00000a20: ec76 c154 96eb 16d6 6b61 ab04 6d53 8f05  .v.T....ka..mS..
+00000a30: 6469 0b0c 1a69 78fb 97bc 0bd1 c282 6a1a  di...ix.......j.
+00000a40: 6cbf 8b7d 2f3e e05b d310 86af 6483 1d5c  l..}/>.[....d..\
+00000a50: 6037 71d1 c242 8c1b 6c55 7bda 8401 ba8a  `7q..B..lU{.....
+00000a60: 48ca d61d e2ba 7a9e 2264 775f 4128 65ed  H.....z."dw_A(e.
+00000a70: 7082 724e e88b 803e ce97 8a2f 168b f68a  p.rN...>.../....
+00000a80: 7644 f145 4823 9e27 6cd3 c6b7 e389 ab80  vD.EH#.'l.......
+00000a90: 5a47 b101 ff08 eaa8 be55 da1a 62bb 2eb2  ZG.......U..b...
+00000aa0: 74af 1ea4 babb 853b 9430 06a2 9e78 8389  t......;.0...x..
+00000ab0: 0d35 d874 430c 298f 87b6 3999 f8ae e9cd  .5.tC.)...9.....
+00000ac0: c29e d7c7 b3e9 dc0b 75ca eb33 46b0 d716  ........u..3F...
+00000ad0: 932f 7e3a 0656 b59a 1255 4259 d515 b5ea  ./~:.V...UBY....
+00000ae0: 07ba 0d0f a3cd 6052 0f1c 12e6 ac42 06cb  ......`R.....B..
+00000af0: 9976 fe61 f57f 019f e00c 95d2 2bc1 e1cb  .v.a........+...
+00000b00: 95c0 e9f7 c7e7 c72b b10f f3e7 d56b 58d5  .......+.....kX.
+00000b10: ec7f ddad 0581 6847 a3ef 3bfe 74e0 3ba6  ......hG..;.t.;.
+00000b20: 33c6 3d13 e3b9 674e 7aae 6786 f330 1ce0  3.=...gNz.g..0..
+00000b30: e174 361d 9ea2 9172 587d 110c ad5c 5a1f  .t6....rX}...\Z.
+00000b40: 78aa 431f 38ba 0206 009e d6ba 904a 8067  x.C.8........J.g
+00000b50: 9634 79fa cc95 aecf f37d 44d3 71a5 d29a  .4y......}D.q...
+00000b60: 916e 2ba1 58c7 53e6 dd2f 0000 00ff ff03  .n+.X.S../......
+00000b70: 0050 4b03 0414 0006 0008 0000 0021 0029  .PK..........!.)
+00000b80: 001d 8f55 0100 00e7 0900 001a 0008 0178  ...U...........x
+00000b90: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
+00000ba0: 2e78 6d6c 2e72 656c 7320 a204 0128 a000  .xml.rels ...(..
+00000bb0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00000bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000cc0: 0000 0000 0000 0000 00bc 96cd 6ac3 300c  ............j.0.
-00000cd0: c7ef 83bd 43f0 7d75 9cb6 693b 9af4 b031  ....C.}u..i;...1
-00000ce0: e875 eb1e c038 ca07 4dec 6079 1f7d fb99  .u...8..M.`y.}..
-00000cf0: 0ed2 058a d643 f0c5 2019 4b3f fe92 2d6f  .....C.. .K?..-o
-00000d00: 77df 5d1b 7d82 c5c6 e88c 8959 cc22 d0ca  w.].}......Y."..
-00000d10: 148d ae32 f67e 7879 58b3 089d d485 6c8d  ...2.~xyX.....l.
-00000d20: 868c 9d00 d92e bfbf dbbe 422b 9d3f 8475  ..........B+.?.u
-00000d30: d363 e4a3 68cc 58ed 5cff c839 aa1a 3a89  .c..h.X.\..9..:.
-00000d40: 33d3 83f6 3ba5 b19d 74de b415 efa5 3aca  3...;...t.....:.
-00000d50: 0a78 12c7 29b7 7f63 b07c 1433 da17 19b3  .x..)..c.|.3....
-00000d60: fbc2 e73f 9c7a 9ff9 ffd8 a62c 1b05 cf46  ...?.z.....,...F
-00000d70: 7d74 a0dd 9514 fccb d823 d600 ce07 95b6  }t.......#......
-00000d80: 0297 b1c1 85fc bcb3 9e79 62c6 afc3 8879  .........yb....y
-00000d90: 601a 31a7 7042 d390 30ab c0d2 acc8 4225  `.1.pB..0.....B%
-00000da0: a10b 9590 3893 8aa3 64ab 9e6a d9e8 4b17  ....8...d..j..K.
-00000db0: 0f2e 8a22 b426 b424 e994 15c2 5a5a 28de  ...".&.$....ZZ(.
-00000dc0: 9cf5 ef16 5e64 19b9 c902 856e 170a 6652  ....^d.....n..fR
-00000dd0: 656e 78f2 5252 1911 5a1a 41e1 2c03 d32c  enx.RR..Z.A.,..,
-00000de0: 496d 26a5 4177 6afd 741d 26d3 af4d e6f7  Im&.Awj.t.&..M..
-00000df0: d33a e870 1431 85b3 084c b3a0 6036 8161  .:.p.1...L..`6.a
-00000e00: 3664 a126 95c6 f9df 155c fae4 6cf2 f33a  6d.&.....\..l..:
-00000e10: 5c1d 3efa 9ee5 3f00 0000 ffff 0300 504b  \.>...?.......PK
-00000e20: 0304 1400 0600 0800 0000 2100 5baf d84c  ..........!.[..L
-00000e30: 1e03 0000 ad06 0000 1800 0000 786c 2f77  ............xl/w
-00000e40: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00000e50: 2e78 6d6c 9c93 db8e 9b30 1086 ef2b f51d  .xml.....0...+..
-00000e60: 2cdf 0703 9b64 1314 b2aa 365d 756f aaaa  ,....d....6]uo..
-00000e70: c76b c70c c18a 0fd4 764e adfa ee1d 4343  .k......vN....CC
-00000e80: 568a 2a45 8bc0 187b fcfd 33f6 cfe2 e1a8  V.*E...{..3.....
-00000e90: 15d9 83f3 d29a 9266 494a 0918 612b 6936  .......fIJ..a+i6
-00000ea0: 25fd f6f5 6934 a3c4 076e 2aae ac81 929e  %...i4...n*.....
-00000eb0: c0d3 87e5 db37 8b83 755b df00 0482 04e3  .....7..u[......
-00000ec0: 4bda 84d0 168c 79d1 80e6 3eb1 2d18 9ca9  K.....y...>.-...
-00000ed0: add3 3ce0 a7db 30df 3ae0 55b7 482b 96a7  ..<...0.:.U.H+..
-00000ee0: e994 692e 0ded 0985 bb85 61eb 5a0a 5859  ..i.......a.Z.XY
-00000ef0: b1d3 6042 0f71 a078 c0fc 7d23 5b7f a669  ..`B.q.x..}#[..i
-00000f00: 710b 4e73 b7dd b523 6175 8b88 b554 329c  q.Ns...#au...T2.
-00000f10: 3a28 255a 14cf 1b63 1d5f 2bac fb98 8db9  :(%Z...c._+.....
-00000f20: 2047 8777 8ecf dd59 a61b bf52 d252 38eb   G.w...Y...R.R8.
-00000f30: 6d1d 1224 b33e e7eb f2e7 6cce b818 48d7  m..$.>....l...H.
-00000f40: f5df 84c9 c6cc c15e c603 bca0 f2d7 a594  .......^........
-00000f50: 4d06 567e 81dd bd12 361d 6071 bb5c b193  M.V~....6.`q.\..
-00000f60: 5549 7fa7 ffae 11be b3d8 a497 e63c f787  UI...........<..
-00000f70: 2e17 95c4 138e 5511 0775 49df 65c5 fb9c  ......U..uI.e...
-00000f80: b2e5 a2f3 cf77 0907 ffa2 4f7e 59ab bf08  .....w....O~Y...
-00000f90: aee0 6334 9c42 2ba7 68e5 68d2 b5b5 db18  ..c4.B+.h.h.....
-00000fa0: fe8c e229 723d 2810 d12e 84e3 6b0f 8fa0  ...)r=(.....k...
-00000fb0: 307c 758f 3eff d929 6117 65d8 a0f3 b27f  0|u.>..)a.e.....
-00000fc0: d67c ea6c fdc9 9135 f7f0 68d5 0f59 8526  .|.l...5..h..Y.&
-00000fd0: 8a52 5241 cd77 2a5c 06e7 4936 4ea7 f964  .RRA.w*\..I6N..d
-00000fe0: 98fa 6c0f 1f40 6e9a 800b 70b4 b350 519d  ..l..@n...p..PQ.
-00000ff0: 56e0 057a 1ab3 4c30 1853 1056 a11e b644  V..z..L0.S.V...D
-00001000: cbf8 73a2 27f9 b1a4 b899 875e 6e96 8cf3  ..s.'......^n...
-00001010: c9fd 2c1b c2fb 4064 7681 599a 4fff 13cb  ..,...@dv.Y.O...
-00001020: 3af6 5f00 0000 ffff 0000 00ff ff94 d14b  :._............K
-00001030: 0ec2 2014 05d0 ad10 e60a 8f96 4943 49aa  .. .........ICI.
-00001040: 7421 0469 1c55 5348 d5dd 0b7e 4a00 27ce  t!.i.USH...~J.'.
-00001050: 081c 78b9 17e1 ced6 7aa5 bd96 62b9 dcd0  ..x.....z...b...
-00001060: d263 c0c8 5df5 ecc2 aae3 18dd a1d5 a63b  .c..]..........;
-00001070: 3d94 75c6 cebe c774 cf38 96c2 443b 44fc  =.u....t.8..D;D.
-00001080: ba12 0e5c d85d 2515 6495 8298 8f38 d402  ...\.]%.d....8..
-00001090: 7271 ac05 cb85 faf1 4693 93b1 2649 9090  rq......F...&I..
-000010a0: 6c8b c7fe 8917 711e af2d e2d5 8217 f1be  l.....q..-......
-000010b0: 428a 4972 805d 4343 4553 ac8a 4151 850a  B.Ir.]CCES..AQ..
-000010c0: 762b 128a 5163 3d0a 5251 ef8c 247d e713  v+..Qc=.RQ..$}..
-000010d0: 0000 ffff 0000 00ff ff74 8e41 0a83 400c  .........t.A..@.
-000010e0: 45af 32e4 0055 a1b6 b538 eebb 6829 7882  E.2..U...8..h)x.
-000010f0: 9189 1a5a cd90 8914 7afa 8e82 cb66 f5ff  ...Z....z....f..
-00001100: 7ffc 2475 7003 de9d 0c34 47f3 c65e 2de4  ..$up....4G..^-.
-00001110: 8733 18a1 61dc b572 d8d2 124c c7aa 3ced  .3..a..r...L..<.
-00001120: 6e44 e751 5657 16c5 252f f739 5627 303d  nD.QVW..%/.9V'0=
-00001130: b3fe 8359 53af 775b d425 98e0 024a 4b5f  ...YS.w[.%...JK_
-00001140: b450 a51a 49d4 6782 8f65 eab6 3e18 16c2  .P..I.g..e..>...
-00001150: 599d 12cf 1602 8b8a 234d 3f5e c95b 909b  Y.......#M?^.[..
-00001160: 2f20 2dcc 3e2c af38 226a f303 0000 ffff  / -.>,.8"j......
-00001170: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00001180: 861b 55f6 5403 0000 db06 0000 1800 0000  ..U.T...........
-00001190: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-000011a0: 6565 7432 2e78 6d6c 9c93 db8e db20 1086  eet2.xml..... ..
-000011b0: ef2b f51d 10f7 31c6 9ba4 8915 67d5 6eb4  .+....1.....g.n.
-000011c0: eade 5455 b787 6b82 c731 0a18 17c8 a9d5  ..TU..k..1......
-000011d0: be7b 0767 e344 8a2a 458b 6c8c 8799 ef9f  .{.g.D.*E.l.....
-000011e0: 31e3 d9fd de68 b205 e795 6d0a ca93 9412  1....h....m.....
-000011f0: 68a4 2d55 b32a e88f ef8f 8309 253e 88a6  h.-U.*......%>..
-00001200: 14da 3650 d003 787a 3f7f ff6e b6b3 6eed  ..6P..xz?..n..n.
-00001210: 6b80 4090 d0f8 82d6 21b4 3963 5ed6 6084  k.@.....!.9c^.`.
-00001220: 4f6c 0b0d ee54 d619 11f0 d5ad 986f 1d88  Ol...T.......o..
-00001230: b20b 329a 6569 3a66 46a8 861e 09b9 bb85  ..2.ei:fF.......
-00001240: 61ab 4a49 5858 b931 d084 23c4 8116 01f3  a.JIXX.1..#.....
-00001250: f7b5 6afd 8966 e42d 3823 dc7a d30e a435  ..j..f.-8#.z...5
-00001260: 2d22 964a ab70 e8a0 9418 993f ad1a ebc4  -".J.p.....?....
-00001270: 5263 dd7b 3e14 92ec 1d5e 19de 7727 99ce  Rc.{>....^..w'..
-00001280: 7ea5 6494 74d6 db2a 2448 66c7 9caf cb9f  ~.d.t..*$Hf.....
-00001290: b229 13b2 275d d77f 1386 0f99 83ad 8a07  .)..']..........
-000012a0: 7846 656f 4b89 8f7a 5676 86dd bd11 36ee  xFeoK..zVv....6.
-000012b0: 61f1 73b9 7ca3 ca82 fe4d 5fc7 009f 3c4e  a.s.|....M_...<N
-000012c0: e920 e571 ba18 2f74 3e2b 159e 70ac 8a38  . .q../t>+..p..8
-000012d0: a80a fa91 e78b 8cb2 f9ac eb9f 9f0a 76fe  ..............v.
-000012e0: 624d 8258 3e83 0619 0035 3825 7fac 35cf  bM.X>....58%..5.
-000012f0: 5268 f812 1b50 a32d c5d6 8e4d bbb4 761d  Rh...P.-...M..v.
-00001300: c39f d031 451d df85 451d 2183 dac2 0368  ...1E...E.!....h
-00001310: 74ff 8429 fbdf 9d32 2e51 96f5 ba97 eb53  t..)...2.Q.....S
-00001320: 0e8f 5d9b 7f75 6429 3c3c 58fd 4b95 a18e  ..]..ud)<<X.K...
-00001330: a294 9450 898d 0e67 e334 e1c3 749c 8dfa  ...P...g.4..t...
-00001340: ad6f 76f7 19d4 aa0e 1880 d6ae a5f2 f2b0  .ov.............
-00001350: 002f b1c7 31cb 049d 3105 6935 eae1 4c8c  ./..1...1.i5..L.
-00001360: 8a3f 2bf6 a8d8 1714 4f6a 7794 9b24 c36c  .?+.....Ojw..$.l
-00001370: f461 c27b f7a3 e3f0 d591 a7d9 f83f beac  .a.{.........?..
-00001380: 63ff 0300 00ff ff00 0000 ffff 9491 4d0e  c.............M.
-00001390: 8320 1046 af62 d82b 0c45 3106 495a e941  . .F.b.+.E1.IZ.A
-000013a0: 08c5 7465 1b31 b6bd 7da1 3f58 6555 5613  ..te.1..}.?XeUV.
-000013b0: e60d 79df 20dc d9da 49e9 494b 315e 6ed9  ..y. ...I.IK1^n.
-000013c0: d822 4099 bbea c1f9 aa61 28bb 03d3 a639  ."@......a(....9
-000013d0: 3d94 75c6 0e53 8b48 414b 2485 09ec 3ec0  =.u..S.HAK$...>.
-000013e0: af11 df70 fe76 9644 e059 0a6c 3ec4 2125  ...p.v.D.Y.l>.!%
-000013f0: e89a e852 0276 6b44 a5c8 4260 ef1d e5e9  ...R.vkD..B`....
-00001400: 3ff2 015e cbb3 8dfc 9790 a297 a420 a4ae  ?..^......... ..
-00001410: 2a02 3c0f 2565 9cf3 52e0 3e84 ae0a a829  *.<.%e..R.>....)
-00001420: a324 1e38 e69b 0c9d 7f2b 2e09 fce0 ef96  .$.8.....+......
-00001430: 54aa 0210 9177 42bc 7cd5 1300 00ff ff00  T....wB.|.......
-00001440: 0000 ffff 748e 4b0e 8330 0c44 af12 e500  ....t.K..0.D....
-00001450: 854a a51f 0958 b16d 85c4 0902 3560 15e2  .J...X.m....5`..
-00001460: c831 adc4 e91b 52b1 ac57 9ef1 d38c 7367  .1....R..W....sg
-00001470: 06b8 1b1e d07a 3541 2f85 4e0f 17ad 1887  .....z5A/.N.....
-00001480: 71df 855c 7433 ad5a 12a1 7957 2398 27f0  q..\t3.Z..yW#.'.
-00001490: a6b2 e3f1 9a66 fb9c 6e67 ad7a 22f9 774c  .....f..ng.z".wL
-000014a0: ca7c eb6d 4016 a79c 71c0 0dae 1082 b4f2  .|.m@...q.......
-000014b0: 9d99 7e5b 8fec a50e d863 99db 98a4 1531  ..~[.....c.....1
-000014c0: 8215 2348 b6d0 8e58 d8a0 68b5 78a8 196d  ..#H...X..h.x..m
-000014d0: e8ab a037 cb24 3e66 8d01 5f29 f053 e530  ...7.$>f.._).S.0
-000014e0: 3a6f 60c1 d0b0 eb8e 1c42 84c3 4bc9 87f8  :o`......B..K...
-000014f0: e547 0029 bf00 0000 ffff 0300 504b 0304  .G.)........PK..
-00001500: 1400 0600 0800 0000 2100 d029 2692 3503  ........!..)&.5.
-00001510: 0000 e806 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
-00001520: 6b73 6865 6574 732f 7368 6565 7433 2e78  ksheets/sheet3.x
-00001530: 6d6c 9c93 db8e db20 1086 ef2b f51d 10f7  ml..... ...+....
-00001540: 31c6 9ba4 8915 6755 6dba eade 5455 8fd7  1.....gUm...TU..
-00001550: 048f 6314 302e 9053 ab7d f70e 76e3 ac14  ..c.0..S.}..v...
-00001560: 558a d6b2 3186 e1fb 67e0 f7e2 fe68 34d9  U...1...g....h4.
-00001570: 83f3 ca36 05e5 494a 0934 d296 aad9 14f4  ...6..IJ.4......
-00001580: fbb7 c7d1 8c12 1f44 530a 6d1b 28e8 093c  .......DS.m.(..<
-00001590: bd5f be7d b338 58b7 f535 4020 4868 7c41  ._.}.8X..5@ Hh|A
-000015a0: eb10 da9c 312f 6b30 c227 b685 0667 2aeb  ....1/k0.'...g*.
-000015b0: 8c08 f8e9 36cc b70e 44d9 2d32 9a65 693a  ....6...D.-2.ei:
-000015c0: 6546 a886 f684 dcdd c2b0 55a5 24ac acdc  eF........U.$...
-000015d0: 1968 420f 71a0 45c0 fc7d ad5a 7fa6 1979  .hB.q.E..}.Z...y
-000015e0: 0bce 08b7 ddb5 2369 4d8b 88b5 d22a 9c3a  ......#iM....*.:
-000015f0: 2825 46e6 4f9b c63a b1d6 58f7 918f 8524  (%F.O..:..X....$
-00001600: 4787 7786 cfdd 59a6 1bbf 5232 4a3a eb6d  G.w...Y...R2J:.m
-00001610: 1512 24b3 3ee7 ebf2 e76c ce84 1c48 d7f5  ..$.>....l...H..
-00001620: df84 e163 e660 afe2 015e 50d9 eb52 e293  ...c.`...^P..R..
-00001630: 8195 5d60 77af 844d 0758 dc2e 97ef 5459  ..]`w..M.X....TY
-00001640: d03f e9bf 6b84 6f1e 9b74 94a2 17ba de79  .?..k.o..t.....y
-00001650: ee99 2e17 a5c2 138e 5511 0755 41df f3fc  ........U..UA...
-00001660: 4346 d972 d1f9 e787 8283 7fd1 27bf ad35  CF.r........'..5
-00001670: 5fa5 d0f0 291a 4ea3 9553 b472 34e9 dada  _...).N..S.r4...
-00001680: 6d0c 7f42 f114 b91e 34c8 6817 22f0 b587  m..B....4.h."...
-00001690: 07d0 18be e21c 8dfe ab93 8a7d 1462 83d2  ...........}.b..
-000016a0: cbfe 59f5 b133 f667 47d6 c2c3 83d5 3f55  ..Y..3.gG.....?U
-000016b0: 19ea 284b 4909 95d8 e970 199c 277c 9c4e  ..(KI....p..'|.N
-000016c0: b3c9 30f5 c51e 3e82 dad4 0117 e068 67a2  ..0...>......hg.
-000016d0: bc3c adc0 4b74 35e6 9960 30a6 20ad 463d  .<..Kt5..`0. .F=
-000016e0: 6c89 51f1 f744 578a 6341 713b 0fbd dc2c  l.Q..DW.cAq;...,
-000016f0: 1967 9377 333e 84f7 81c8 ec02 799a 4dff  .g.w3>......y.M.
-00001700: 13cb 3af6 5f00 0000 ffff 0000 00ff ff94  ..:._...........
-00001710: d1dd 0ac2 2014 c0f1 5711 1f20 a7cd 8271  .... ...W.. ...q
-00001720: 26b4 d983 8809 5dad d891 556f 9ff6 25ea  &.....]...Uo..%.
-00001730: 6eba 13fd 29fc 8f80 67e7 bc36 de28 982f  n...)...g..6.(./
-00001740: 3732 f794 5382 5733 6158 7592 923b 6f8d  72..S.W3aXu..;o.
-00001750: ed4e 0fed d0ba c9f7 b4d9 0849 15d8 680f  .N.........I..h.
-00001760: 11bf ae84 030c bb8b 6a80 2d0a 98fd 88a1  ........j.-.....
-00001770: 163c 1763 2d44 2ef4 ca1b db9c 1c6b 9204  .<.c-D.......k..
-00001780: 0b65 bf3c f14f 5ec4 795e 5be4 d542 1679  .e.<.O^.y^[..B.y
-00001790: 5f11 8723 f645 597d 9def 8ab2 1592 66fc  _..#.EY}......f.
-000017a0: 4e63 e917 9f00 0000 ffff 0000 00ff ff74  Nc.............t
-000017b0: 8e4b 0e83 300c 44af 12e5 0085 4aa5 1f09  .K..0.D.....J...
-000017c0: 58b1 6d85 c409 0235 6015 e2c8 31ad c4e9  X.m....5`...1...
-000017d0: 1b52 b1ac 579e f1d3 8c73 6706 b81b 1ed0  .R..W....sg.....
-000017e0: 7a35 412f 854e 0f17 ad18 8771 df85 5c74  z5A/.N.....q..\t
-000017f0: 33ad 5a12 a179 5723 9827 f0a6 b2e3 f19a  3.Z..yW#.'......
-00001800: 66fb 9c6e 67ad 7a22 f977 4cca 7ceb 6d40  f..ng.z".wL.|.m@
-00001810: 16a7 9c71 c00d ae10 82b4 f29d 997e 5b8f  ...q.........~[.
-00001820: eca5 0ed8 6399 db98 a415 3182 1523 48b6  ....c.....1..#H.
-00001830: d08e 58d8 a068 b578 a819 6de8 aba0 37cb  ..X..h.x..m...7.
-00001840: 243e 668d 015f 29f0 53e5 303a 6f60 c1d0  $>f.._).S.0:o`..
-00001850: b0eb 8e1c 4284 c34b c987 f8e5 4700 29bf  ....B..K....G.).
-00001860: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00001870: 0000 0021 0023 9eec 802d 0300 00a3 0600  ...!.#...-......
-00001880: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00001890: 7473 2f73 6865 6574 342e 786d 6c9c 93db  ts/sheet4.xml...
-000018a0: 8e9b 3010 86ef 2bf5 1d2c df07 0321 6982  ..0...+..,...!i.
-000018b0: 4256 d546 abee 4d55 f578 ed98 2158 b131  BV.F..MU.x..!X.1
-000018c0: b59d 53ab befb 8e61 4322 4595 a245 601b  ..S....aC"E..E`.
-000018d0: 7bfc fd33 f867 f170 d48a ecc1 3a69 9a82  {..3.g.p....:i..
-000018e0: 2651 4c09 34c2 94b2 d914 f4c7 f7a7 d18c  &QL.4...........
-000018f0: 12e7 7953 7265 1a28 e809 1c7d 58be 7fb7  ..ySre.(...}X...
-00001900: 3818 bb75 3580 2748 685c 416b efdb 9c31  8..u5.'Hh\Ak...1
-00001910: 276a d0dc 45a6 8506 572a 6335 f7f8 6a37  'j..E...W*c5..j7
-00001920: ccb5 1678 d96d d28a a571 3c65 9acb 86f6  ...x.m...q<e....
-00001930: 84dc dec3 3055 2505 ac8c d869 687c 0fb1  ....0U%....ih|..
-00001940: a0b8 c7fc 5d2d 5b77 a669 710f 4e73 bbdd  ....]-[w.iq.Ns..
-00001950: b523 6174 8b88 b554 d29f 3a28 255a e4cf  .#at...T..:(%Z..
-00001960: 9bc6 58be 5658 f731 c9b8 2047 8b77 8acf  ..X.VX.1.. G.w..
-00001970: f82c d3cd df28 6929 ac71 a6f2 1192 599f  .,...(i).q....Y.
-00001980: f36d f973 3667 5c0c a4db faef c224 19b3  .m.s6g\......$..
-00001990: b097 e100 2fa8 f46d 2925 9381 955e 60e3  ..../..m)%...^`.
-000019a0: 37c2 a603 2c7c 2e9b ef64 59d0 bff1 eb35  7...,|...dY....5
-000019b0: c23e 094d 3c8a c7a1 b9ba fed1 e5a2 9478  .>.M<..........x
-000019c0: c2a1 2a62 a12a e8c7 245f a594 2d17 9d7f  ..*b.*..$_..-...
-000019d0: 7e4a 38b8 ab31 f963 8cfe 26b8 82cf c170  ~J8..1.c..&....p
-000019e0: 0aad 1ca3 9583 49d7 c66c 43f8 338a c7c8  ......I..lC.3...
-000019f0: 75a0 4004 bb10 8edd 1e1e 4161 f82a f8fc  u.@.......Aa.*..
-00001a00: 77a7 8443 9461 83ce f5f8 acf9 d4d9 fa8b  w..C.a..........
-00001a10: 256b eee0 d1a8 5fb2 f475 10a5 a484 8aef  %k...._..u......
-00001a20: 94bf 4cce a324 8ba7 e964 58fa 6a0e 9f40  ..L..$...dX.j..@
-00001a30: 6e6a 8f1b 70b6 b350 5e9e 56e0 047a 1ab3  nj..p..P^.V..z..
-00001a40: 8c30 1853 1046 a11e b644 cbf0 73a2 27f9  .0.S.F...D..s.'.
-00001a50: b1a0 7832 875e 6e16 65e9 e4c3 2c19 c2fb  ..x2.^n.e...,...
-00001a60: c0ec 3530 89d3 e97f 6259 c77e 0100 00ff  ..50....bY.~....
-00001a70: ff00 0000 ffff 94d1 dd0a c220 1880 e15b  ........... ...[
-00001a80: 91ef 02e6 cf5c c170 42cb 1b11 133a 5a31  .....\.pB....:Z1
-00001a90: 65d5 dd4f b772 a847 9d89 3ee2 fba1 7077  e..O.r.G..>...pw
-00001aa0: 6bbd d25e 4b31 3f5e 681e 8002 724f 3db9  k..^K1?^h...rO=.
-00001ab0: b0ea 39a0 37e5 daf4 b78f b2ce d8c9 0f40  ..9.7..........@
-00001ac0: 1ad6 8114 26da 4bc4 db95 70e0 c2ee 2289  ....&.K...p...".
-00001ad0: c08b 14d8 7cc5 580b 968b 6b2d 689b 1355  ....|.X...k-h..U
-00001ae0: 9343 e0d0 9de2 d93f f111 e7f1 bc88 ff89  .C.....?........
-00001af0: 6db0 8674 45f9 7edc 024a d3d3 7351 5ebf  m..tE.~..J..sQ^.
-00001b00: 714a 622f c7c7 17ac 0000 00ff ff00 0000  qJb/............
-00001b10: ffff 748e 4b0e 8330 0c44 af12 e500 854a  ..t.K..0.D.....J
-00001b20: a51f 0958 b16d 85c4 0902 3560 15e2 c831  ...X.m....5`...1
-00001b30: adc4 e91b 52b1 ac57 9ef1 d38c 7367 06b8  ....R..W....sg..
-00001b40: 1b1e d07a 3541 2f85 4e0f 17ad 1887 71df  ...z5A/.N.....q.
-00001b50: 855c 7433 ad5a 12a1 7957 2398 27f0 a6b2  .\t3.Z..yW#.'...
-00001b60: e3f1 9a66 fb9c 6e67 ad7a 22f9 774c ca7c  ...f..ng.z".wL.|
-00001b70: eb6d 4016 a79c 71c0 0dae 1082 b4f2 9d99  .m@...q.........
-00001b80: 7e5b 8fec a50e d863 99db 98a4 1531 8215  ~[.....c.....1..
-00001b90: 2348 b6d0 8e58 d8a0 68b5 78a8 196d e8ab  #H...X..h.x..m..
-00001ba0: a037 cb24 3e66 8d01 5f29 f053 e530 3a6f  .7.$>f.._).S.0:o
-00001bb0: 60c1 d0b0 eb8e 1c42 84c3 4bc9 87f8 e547  `......B..K....G
-00001bc0: 0029 bf00 0000 ffff 0300 504b 0304 1400  .)........PK....
-00001bd0: 0600 0800 0000 2100 8608 71bb 2b03 0000  ......!...q.+...
-00001be0: a206 0000 1800 0000 786c 2f77 6f72 6b73  ........xl/works
-00001bf0: 6865 6574 732f 7368 6565 7435 2e78 6d6c  heets/sheet5.xml
-00001c00: 9c93 db8e 9b30 1086 ef2b f51d 2cdf 0703  .....0...+..,...
-00001c10: 4bd2 0485 acaa 44ab ee4d 55f5 78ed 9821  K.....D..MU.x..!
-00001c20: 58b1 31b5 9d53 abbe fb8e 6143 2245 95a2  X.1..S....aC"E..
-00001c30: 4560 1b7b fcfd 33f8 67fe 78d4 8aec c13a  E`.{..3.g.x....:
-00001c40: 699a 8226 514c 0934 c294 b2d9 14f4 c7f7  i..&QL.4........
-00001c50: a7d1 9412 e779 5372 651a 28e8 091c 7d5c  .....ySre.(...}\
-00001c60: bc7f 373f 18bb 7535 8027 4868 5c41 6bef  ..7?..u5.'Hh\Ak.
-00001c70: db9c 3127 6ad0 dc45 a685 0657 2a63 35f7  ..1'j..E...W*c5.
-00001c80: f86a 37cc b516 78d9 6dd2 8aa5 713c 619a  .j7...x.m...q<a.
-00001c90: cb86 f684 dcde c330 5525 05ac 8cd8 6968  .......0U%....ih
-00001ca0: 7c0f b1a0 b8c7 fc5d 2d5b 77a6 6971 0f4e  |......]-[w.iq.N
-00001cb0: 73bb ddb5 2361 748b 88b5 54d2 9f3a 2825  s...#at...T..:(%
-00001cc0: 5ae4 cf9b c658 be56 58f7 31c9 b820 478b  Z....X.VX.1.. G.
-00001cd0: 778a cfc3 59a6 9bbf 51d2 5258 e34c e523  w...Y...Q.RX.L.#
-00001ce0: 24b3 3ee7 dbf2 676c c6b8 1848 b7f5 df85  $.>...gl...H....
-00001cf0: 4932 6661 2fc3 015e 50e9 db52 4ac6 032b  I2fa/..^P..RJ..+
-00001d00: bdc0 1ede 089b 0cb0 f0b9 6cbe 9365 41ff  ..........l..eA.
-00001d10: c6af d708 fb24 34f1 28ce 4273 75fd a38b  .....$4.(.Bsu...
-00001d20: 7929 f184 4355 c442 55d0 8f49 be4a 295b  y)..CU.BU..I.J)[
-00001d30: cc3b fffc 9470 7057 63f2 c718 fd4d 7005  .;...ppWc....Mp.
-00001d40: 9f83 e114 5a39 462b 0793 ae8d d986 f067  ....Z9F+.......g
-00001d50: 148f 91eb 4081 0876 211c bb3d 2c41 61f8  ....@..v!..=,Aa.
-00001d60: 32f8 fc77 a784 4394 6183 cef5 f8ac f9d4  2..w..C.a.......
-00001d70: d9fa 8b25 6bee 6069 d42f 59fa 3a88 5252  ...%k.`i./Y.:.RR
-00001d80: 42c5 77ca 5f26 6751 92c5 9374 3c2c 7d35  B.w._&gQ...t<,}5
-00001d90: 874f 2037 b5c7 0d38 db59 282f 4f2b 7002  .O 7...8.Y(/O+p.
-00001da0: 3d8d 5946 188c 2908 a350 0f5b a265 f839  =.YF..)..P.[.e.9
-00001db0: d193 fc58 503c 9943 2f37 8db2 74fc 619a  ...XP<.C/7..t.a.
-00001dc0: 0ce1 7d60 f61a 98c4 e9e4 3fb1 ac63 bf00  ..}`......?..c..
-00001dd0: 0000 ffff 0000 00ff ff94 d1d1 0ac2 2014  .............. .
-00001de0: 80e1 5791 f300 733a 2b18 4ea8 7c11 31a1  ..W...s:+.N.|.1.
-00001df0: ab15 3bb2 d5db a75b 39d4 abee 443f f13f  ..;....[9...D?.?
-00001e00: 28f1 ee9c d7c6 1b25 a7c7 42a6 0118 107c  (......%..B....|
-00001e10: 9a11 c3aa 1740 5e4c 18db dfde daa1 75a3  .....@^L......u.
-00001e20: 1fa0 6df8 0194 b4d1 9e23 5eaf 8403 0cbb  ..m......#^.....
-00001e30: b36a 259d 95a4 f62b 2eb5 e0b9 b8d6 8275  .j%....+.......u
-00001e40: 39d1 35d9 050d dd29 9eff 131f 711e 2f8a  9.5....)....q./.
-00001e50: f89f 5807 6bca f0ed b403 9286 67a7 22bc  ..X.k.......g.".
-00001e60: 7ee2 98c4 164e f71f f800 0000 ffff 0000  ~....N..........
-00001e70: 00ff ff74 8e4b 0e83 300c 44af 12e5 0085  ...t.K..0.D.....
-00001e80: 4aa5 1f09 58b1 6d85 c409 0235 6015 e2c8  J...X.m....5`...
-00001e90: 31ad c4e9 1b52 b1ac 579e f1d3 8c73 6706  1....R..W....sg.
-00001ea0: b81b 1ed0 7a35 412f 854e 0f17 ad18 8771  ....z5A/.N.....q
-00001eb0: df85 5c74 33ad 5a12 a179 5723 9827 f0a6  ..\t3.Z..yW#.'..
-00001ec0: b2e3 f19a 66fb 9c6e 67ad 7a22 f977 4cca  ....f..ng.z".wL.
-00001ed0: 7ceb 6d40 16a7 9c71 c00d ae10 82b4 f29d  |.m@...q........
-00001ee0: 997e 5b8f eca5 0ed8 6399 db98 a415 3182  .~[.....c.....1.
-00001ef0: 1523 48b6 d08e 58d8 a068 b578 a819 6de8  .#H...X..h.x..m.
-00001f00: aba0 37cb 243e 668d 015f 29f0 53e5 303a  ..7.$>f.._).S.0:
-00001f10: 6f60 c1d0 b0eb 8e1c 4284 c34b c987 f8e5  o`......B..K....
-00001f20: 4700 29bf 0000 00ff ff03 0050 4b03 0414  G.)........PK...
-00001f30: 0006 0008 0000 0021 0034 75cd 852f 0300  .......!.4u../..
-00001f40: 00a5 0600 0018 0000 0078 6c2f 776f 726b  .........xl/work
-00001f50: 7368 6565 7473 2f73 6865 6574 362e 786d  sheets/sheet6.xm
-00001f60: 6c9c 935d 6f9b 3014 86ef 27ed 3f58 be0f  l..]o.0...'.?X..
-00001f70: 064a b204 8554 53a3 6abd 99a6 7df5 da31  .J...TS.j...}..1
-00001f80: 8760 c5c6 cc76 be36 edbf f718 1a12 29aa  .`...v.6......).
-00001f90: 1415 816d ece3 e73d 07bf ccef 0f5a 911d  ...m...=.....Z..
-00001fa0: 5827 4d53 d024 8a29 8146 9852 36eb 82fe  X'MS.$.).F.R6...
-00001fb0: faf9 389a 52e2 3c6f 4aae 4c03 053d 82a3  ..8.R.<oJ.L..=..
-00001fc0: f78b 8f1f e67b 6337 ae06 f004 098d 2b68  .....{c7......+h
-00001fd0: ed7d 9b33 e644 0d9a bbc8 b4d0 e04a 65ac  .}.3.D.......Je.
-00001fe0: e61e 5fed 9ab9 d602 2fbb 4d5a b134 8e27  .._...../.MZ.4.'
-00001ff0: 4c73 d9d0 9e90 db5b 18a6 aaa4 80a5 115b  Ls.....[.......[
-00002000: 0d8d ef21 1614 f798 bfab 65eb 4e34 2d6e  ...!......e.N4-n
-00002010: c169 6e37 db76 248c 6e11 b192 4afa 6307  .in7.v$.n...J.c.
-00002020: a544 8bfc 69dd 18cb 570a eb3e 2419 17e4  .D..i...W..>$...
-00002030: 60f1 4ef1 b93b c974 f357 4a5a 0a6b 9ca9  `.N..;.t.WJZ.k..
-00002040: 7c84 64d6 e77c 5dfe 8ccd 1817 03e9 bafe  |.d..|].........
-00002050: 9b30 49c6 2cec 6438 c033 2a7d 5f4a c978  .0I.,.d8.3*}_J.x
-00002060: 60a5 67d8 dd3b 6193 0116 3e97 cdb7 b22c  `.g..;a...>....,
-00002070: e8bf f8f5 1a61 9f84 261e c5e3 d05c 5cff  .....a..&....\\.
-00002080: e962 5e4a 3ce1 5015 b150 15f4 7392 2f53  .b^J<.P..P..s./S
-00002090: ca16 f3ce 3fbf 25ec ddc5 98fc 3546 ff10  ....?.%.....5F..
-000020a0: 5cc1 d760 3885 568e d1ca c1a4 2b63 3621  \..`8.V.....+c6!
-000020b0: fc09 c563 e43a 5020 825d 08c7 6e07 0fa0  ...c.:P .]..n...
-000020c0: 307c 9960 c1ee 4f27 15c6 28c4 06a5 cbf1  0|.`..O'..(.....
-000020d0: 49f5 b133 f637 4b56 dcc1 8351 cfb2 f475  I..3.7KV...Q...u
-000020e0: 90a5 a484 8a6f 953f 4fce a224 8b27 e978  .....o.?O..$.'.x
-000020f0: 58fa 6ef6 5f40 ae6b 8f1b 70b6 3351 5e1e  X.n._@.k..p.3Q^.
-00002100: 97e0 04ba 1af3 8c30 1853 1046 a11e b644  .......0.S.F...D
-00002110: cbf0 7ba2 2bf9 a1a0 98ea be97 9b46 593a  ..{.+........FY:
-00002120: fe34 4d86 f03e 307b 0d4c e274 f246 2ceb  .4M..>0{.L.t.F,.
-00002130: d82f 0000 00ff ff00 0000 ffff 94d1 dd0a  ./..............
-00002140: c220 1880 e15b 91ef 02e6 cf5c c170 42cb  . ...[.....\.pB.
-00002150: 1b11 133a 5a31 65d5 dd4f b772 a847 9d89  ...:Z1e..O.r.G..
-00002160: 3ee2 fba1 7077 6bbd d25e 4b31 3f5e 681e  >...pwk..^K1?^h.
-00002170: 8002 724f 3db9 b0ea 39a0 37e5 daf4 b78f  ..rO=...9.7.....
-00002180: b2ce d8c9 0f40 1ad6 8114 26da 4bc4 db95  .....@....&.K...
-00002190: 70e0 c2ee 2289 c08b 14d8 7cc5 580b 968b  p...".....|.X...
-000021a0: 6b2d 689b 1355 9343 e0d0 9de2 d93f f111  k-h..U.C.....?..
-000021b0: e7f1 bc88 ff89 6db0 8674 45f9 7edc 024a  ......m..tE.~..J
-000021c0: d3d3 7351 5ebf 714a 622f c7c7 17ac 0000  ..sQ^.qJb/......
-000021d0: 00ff ff00 0000 ffff 748e 4b0e 8330 0c44  ........t.K..0.D
-000021e0: af12 e500 854a a51f 0958 b16d 85c4 0902  .....J...X.m....
-000021f0: 3560 15e2 c831 adc4 e91b 52b1 ac57 9ef1  5`...1....R..W..
-00002200: d38c 7367 06b8 1b1e d07a 3541 2f85 4e0f  ..sg.....z5A/.N.
-00002210: 17ad 1887 71df 855c 7433 ad5a 12a1 7957  ....q..\t3.Z..yW
-00002220: 2398 27f0 a6b2 e3f1 9a66 fb9c 6e67 ad7a  #.'......f..ng.z
-00002230: 22f9 774c ca7c eb6d 4016 a79c 71c0 0dae  ".wL.|.m@...q...
-00002240: 1082 b4f2 9d99 7e5b 8fec a50e d863 99db  ......~[.....c..
-00002250: 98a4 1531 8215 2348 b6d0 8e58 d8a0 68b5  ...1..#H...X..h.
-00002260: 78a8 196d e8ab a037 cb24 3e66 8d01 5f29  x..m...7.$>f.._)
-00002270: f053 e530 3a6f 60c1 d0b0 eb8e 1c42 84c3  .S.0:o`......B..
-00002280: 4bc9 87f8 e547 0029 bf00 0000 ffff 0300  K....G.)........
-00002290: 504b 0304 1400 0600 0800 0000 2100 f77d  PK..........!..}
-000022a0: c8d5 2e03 0000 a306 0000 1800 0000 786c  ..............xl
-000022b0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-000022c0: 7437 2e78 6d6c 9c93 5d6f 9b30 1486 ef27  t7.xml..]o.0...'
-000022d0: ed3f 58be 0f06 4ad2 0485 5455 a36a bd99  .?X...J...TU.j..
-000022e0: a67d 5e3b e610 acd8 98d9 ced7 a6fd f71d  .}^;............
-000022f0: 4343 2245 95a2 22b0 8d7d fcbc e7e0 97f9  CC"E.."..}......
-00002300: c341 2bb2 03eb a469 0a9a 4431 25d0 0853  .A+....i..D1%..S
-00002310: ca66 5dd0 1fdf 9f47 534a 9ce7 4dc9 9569  .f]....GSJ..M..i
-00002320: a0a0 4770 f461 f1f1 c37c 6fec c6d5 009e  ..Gp.a...|o.....
-00002330: 20a1 7105 adbd 6f73 c69c a841 7317 9916   .q...os...As...
-00002340: 1a5c a98c d5dc e3ab 5d33 d75a e065 b749  .\......]3.Z.e.I
-00002350: 2b96 c6f1 8469 2e1b da13 727b 0bc3 5495  +....i....r{..T.
-00002360: 14b0 3462 aba1 f13d c482 e21e f377 b56c  ..4b...=.....w.l
-00002370: dd89 a6c5 2d38 cded 66db 8e84 d12d 2256  ....-8..f....-"V
-00002380: 5249 7fec a094 6891 bfac 1b63 f94a 61dd  RI....h....c.Ja.
-00002390: 8724 e382 1c2c de29 3e77 2799 6efe 4a49  .$...,.)>w'.n.JI
-000023a0: 4b61 8d33 958f 90cc fa9c afcb 9fb1 19e3  Ka.3............
-000023b0: 6220 5dd7 7f13 26c9 9885 9d0c 0778 46a5  b ]...&......xF.
-000023c0: ef4b 2919 0fac f40c bb7b 276c 32c0 c2e7  .K)......{'l2...
-000023d0: b2f9 5696 05fd 1bbf 5e23 ec93 d0c4 a378  ..V.....^#.....x
-000023e0: 129a 8beb 1f5d cc4b 8927 1caa 2216 aa82  .....].K.'.."...
-000023f0: 3e26 f932 a56c 31ef fcf3 53c2 de5d 8cc9  >&.2.l1...S..]..
-00002400: 1f63 f437 c115 7c0e 8653 68e5 18ad 1c4c  .c.7..|..Sh....L
-00002410: ba32 6613 c25f 503c 46ae 0305 22d8 8570  .2f.._P<F..."..p
-00002420: ec76 f004 0ac3 97f7 e8f3 df9d 120e 5186  .v............Q.
-00002430: 0d3a 97e3 93e6 7367 eb2f 96ac b883 27a3  .:....sg./....'.
-00002440: 7ec9 d2d7 4194 9212 2abe 55fe 3c39 8b92  ~...A...*.U.<9..
-00002450: 2c9e a4e3 61e9 abd9 7f02 b9ae 3d6e c0d9  ,...a.......=n..
-00002460: ce42 7979 5c82 13e8 69cc 32c2 604c 4118  .Byy\...i.2.`LA.
-00002470: 857a d812 2dc3 cf89 9ee4 8782 e2c9 ec7b  .z..-..........{
-00002480: b969 94a5 e3fb 6932 84f7 81d9 6b60 12a7  .i....i2....k`..
-00002490: 9337 6259 c7fe 0f00 00ff ff00 0000 ffff  .7bY............
-000024a0: 94d1 dd0a c220 1880 e15b 91ef 02e6 cf5c  ..... ...[.....\
-000024b0: c170 42cb 1b11 133a 5a31 65d5 dd4f b772  .pB....:Z1e..O.r
-000024c0: a847 9d89 3ee2 fba1 7077 6bbd d25e 4b31  .G..>...pwk..^K1
-000024d0: 3f5e 681e 8002 724f 3db9 b0ea 39a0 37e5  ?^h...rO=...9.7.
-000024e0: daf4 b78f b2ce d8c9 0f40 1ad6 8114 26da  .........@....&.
-000024f0: 4bc4 db95 70e0 c2ee 2289 c08b 14d8 7cc5  K...p...".....|.
-00002500: 580b 968b 6b2d 689b 1355 9343 e0d0 9de2  X...k-h..U.C....
-00002510: d93f f111 e7f1 bc88 ff89 6db0 8674 45f9  .?........m..tE.
-00002520: 7edc 024a d3d3 7351 5ebf 714a 622f c7c7  ~..J..sQ^.qJb/..
-00002530: 17ac 0000 00ff ff00 0000 ffff 748e 4b0e  ............t.K.
-00002540: 8330 0c44 af12 e500 854a a51f 0958 b16d  .0.D.....J...X.m
-00002550: 85c4 0902 3560 15e2 c831 adc4 e91b 52b1  ....5`...1....R.
-00002560: ac57 9ef1 d38c 7367 06b8 1b1e d07a 3541  .W....sg.....z5A
-00002570: 2f85 4e0f 17ad 1887 71df 855c 7433 ad5a  /.N.....q..\t3.Z
-00002580: 12a1 7957 2398 27f0 a6b2 e3f1 9a66 fb9c  ..yW#.'......f..
-00002590: 6e67 ad7a 22f9 774c ca7c eb6d 4016 a79c  ng.z".wL.|.m@...
-000025a0: 71c0 0dae 1082 b4f2 9d99 7e5b 8fec a50e  q.........~[....
-000025b0: d863 99db 98a4 1531 8215 2348 b6d0 8e58  .c.....1..#H...X
-000025c0: d8a0 68b5 78a8 196d e8ab a037 cb24 3e66  ..h.x..m...7.$>f
-000025d0: 8d01 5f29 f053 e530 3a6f 60c1 d0b0 eb8e  .._).S.0:o`.....
-000025e0: 1c42 84c3 4bc9 87f8 e547 0029 bf00 0000  .B..K....G.)....
-000025f0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00002600: 2100 7576 beb0 2e03 0000 a406 0000 1800  !.uv............
-00002610: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00002620: 7368 6565 7438 2e78 6d6c 9c93 5d6f 9b30  sheet8.xml..]o.0
-00002630: 1486 ef27 ed3f 58be 0f06 4ad2 0485 5455  ...'.?X...J...TU
-00002640: a36a bd99 a67d 5e3b e610 acd8 98d9 ced7  .j...}^;........
-00002650: a6fd f71d 4343 2245 95a2 22b0 8d7d fcbc  ....CC"E.."..}..
-00002660: e7e0 97f9 c341 2bb2 03eb a469 0a9a 4431  .....A+....i..D1
-00002670: 25d0 0853 ca66 5dd0 1fdf 9f47 534a 9ce7  %..S.f]....GSJ..
-00002680: 4dc9 9569 a0a0 4770 f461 f1f1 c37c 6fec  M..i..Gp.a...|o.
-00002690: c6d5 009e 20a1 7105 adbd 6f73 c69c a841  .... .q...os...A
-000026a0: 7317 9916 1a5c a98c d5dc e3ab 5d33 d75a  s....\......]3.Z
-000026b0: e065 b749 2b96 c6f1 8469 2e1b da13 727b  .e.I+....i....r{
-000026c0: 0bc3 5495 14b0 3462 aba1 f13d c482 e21e  ..T...4b...=....
-000026d0: f377 b56c dd89 a6c5 2d38 cded 66db 8e84  .w.l....-8..f...
-000026e0: d12d 2256 5249 7fec a094 6891 bfac 1b63  .-"VRI....h....c
-000026f0: f94a 61dd 8724 e382 1c2c de29 3e77 2799  .Ja..$...,.)>w'.
-00002700: 6efe 4a49 4b61 8d33 958f 90cc fa9c afcb  n.JIKa.3........
-00002710: 9fb1 19e3 6220 5dd7 7f13 26c9 9885 9d0c  ....b ]...&.....
-00002720: 0778 46a5 ef4b 2919 0fac f40c bb7b 276c  .xF..K)......{'l
-00002730: 32c0 c2e7 b2f9 5696 05fd 1bbf 5e23 ec93  2.....V.....^#..
-00002740: d0c4 a3f8 3e34 17d7 3fba 9897 124f 3854  ....>4..?....O8T
-00002750: 452c 5405 7d4c f265 4ad9 62de f9e7 a784  E,T.}L.eJ.b.....
-00002760: bdbb 1893 3fc6 e86f 822b f81c 0ca7 d0ca  ....?..o.+......
-00002770: 315a 3998 7465 cc26 84bf a078 8c5c 070a  1Z9.te.&...x.\..
-00002780: 44b0 0be1 d8ed e009 1486 2f13 0c77 bf3b  D........./..w.;
-00002790: a930 4621 3628 5d8e 4faa cf9d b1bf 58b2  .0F!6(].O.....X.
-000027a0: e20e 9e8c fa25 4b5f 0759 4a4a a8f8 56f9  .....%K_.YJJ..V.
-000027b0: f3e4 2c4a b278 928e 87a5 af66 ff09 e4ba  ..,J.x.....f....
-000027c0: f6b8 0167 3b13 e5e5 7109 4ea0 ab31 cf08  ...g;...q.N..1..
-000027d0: 8331 0561 14ea 614b b40c bf27 ba92 1f0a  .1.a..aK...'....
-000027e0: 8a67 b3ef e5a6 5196 8eef a7c9 10de 0766  .g....Q........f
-000027f0: af81 499c 4ede 8865 1dfb 3f00 0000 ffff  ..I.N..e..?.....
-00002800: 0000 00ff ff94 d1d1 0ac2 2014 80e1 5791  .......... ...W.
-00002810: f300 733a 2b18 6742 cd17 1113 ba5a 3165  ..s:+.gB.....Z1e
-00002820: d5db a75b 39d4 abee 443f f13f 88ee 66ad  ...[9...D?.?..f.
-00002830: 57da 6b89 f3fd 49e6 0118 10f7 d093 0bab  W.k...I.........
-00002840: 5e00 7931 a14d 7f7d 2beb 8c9d fc00 6dc3  ^.y1.M.}+.....m.
-00002850: 0f20 d144 7b8e 78bd 120e 5cd8 5d64 8b74  . .D{.x...\.]d.t
-00002860: 9148 cd57 5c6a c173 31d6 8275 3951 35d9  .H.W\j.s1..u9Q5.
-00002870: 050d dd29 9eff 131f 711e 2f8a f89f 5807  ...)....q./...X.
-00002880: 6b8a aa71 3bed 80a4 e1d9 a908 af9f 3826  k..q;.........8&
-00002890: b185 d3fd 073e 0000 00ff ff00 0000 ffff  .....>..........
-000028a0: 748e 4b0e 8330 0c44 af12 e500 854a a51f  t.K..0.D.....J..
-000028b0: 0958 b16d 85c4 0902 3560 15e2 c831 adc4  .X.m....5`...1..
-000028c0: e91b 52b1 ac57 9ef1 d38c 7367 06b8 1b1e  ..R..W....sg....
-000028d0: d07a 3541 2f85 4e0f 17ad 1887 71df 855c  .z5A/.N.....q..\
-000028e0: 7433 ad5a 12a1 7957 2398 27f0 a6b2 e3f1  t3.Z..yW#.'.....
-000028f0: 9a66 fb9c 6e67 ad7a 22f9 774c ca7c eb6d  .f..ng.z".wL.|.m
-00002900: 4016 a79c 71c0 0dae 1082 b4f2 9d99 7e5b  @...q.........~[
-00002910: 8fec a50e d863 99db 98a4 1531 8215 2348  .....c.....1..#H
-00002920: b6d0 8e58 d8a0 68b5 78a8 196d e8ab a037  ...X..h.x..m...7
-00002930: cb24 3e66 8d01 5f29 f053 e530 3a6f 60c1  .$>f.._).S.0:o`.
-00002940: d0b0 eb8e 1c42 84c3 4bc9 87f8 e547 0029  .....B..K....G.)
-00002950: bf00 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00002960: 0800 0000 2100 c55f 466e 2e03 0000 a206  ....!.._Fn......
-00002970: 0000 1800 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-00002980: 6574 732f 7368 6565 7439 2e78 6d6c 9c93  ets/sheet9.xml..
-00002990: db8e db20 1086 ef2b f51d 10f7 31c6 9ba4  ... ...+....1...
-000029a0: 8915 6755 6dba eade 5455 0fbb d704 8f63  ..gUm...TU.....c
-000029b0: 1430 2e90 53ab be7b 0767 e344 8a2a 456b  .0..S..{.g.D.*Ek
-000029c0: d980 61f8 fe19 f37b 76bf 379a 6cc1 7965  ..a....{v.7.l.ye
-000029d0: 9b82 f224 a504 1a69 4bd5 ac0a faf3 c7e3  ...$...iK.......
-000029e0: 6042 890f a229 85b6 0d14 f400 9ede cfdf  `B...)..........
-000029f0: bf9b edac 5bfb 1a20 1024 34be a075 086d  ....[.. .$4..u.m
-00002a00: ce98 9735 18e1 13db 4283 2b95 7546 047c  ...5....B.+.uF.|
-00002a10: 752b e65b 07a2 ec36 19cd b234 1d33 2354  u+.[...6...4.3#T
-00002a20: 438f 84dc ddc2 b055 a524 2cac dc18 68c2  C......U.$,...h.
-00002a30: 11e2 408b 80f9 fb5a b5fe 4433 f216 9c11  ..@....Z..D3....
-00002a40: 6ebd 6907 d29a 1611 4ba5 5538 7450 4a8c  n.i.....K.U8tPJ.
-00002a50: cc9f 568d 7562 a9b1 ee3d 1f0a 49f6 0eef  ..V.ub...=..I...
-00002a60: 0c9f bb93 4c37 7fa5 6494 74d6 db2a 2448  ....L7..d.t..*$H
-00002a70: 66c7 9caf cb9f b229 13b2 275d d77f 1386  f......)..']....
-00002a80: 0f99 83ad 8a07 7846 656f 4b89 8f7a 5676  ......xFeoK..zVv
-00002a90: 86dd bd11 36ee 61f1 73b9 7ca3 ca82 fe49  ....6.a.s.|....I
-00002aa0: 5faf 01f6 3c36 e920 9dc4 e6e2 fa4b e7b3  _...<6. .....K..
-00002ab0: 52e1 09c7 aa88 83aa a01f 79be c828 9bcf  R.........y..(..
-00002ac0: 3aff 3c2b d8f9 8b31 f96d adf9 2e85 862f  :.<+...1.m...../
-00002ad0: d170 1aad 9ca2 95a3 4997 d6ae 63f8 138a  .p......I...c...
-00002ae0: a7c8 f5a0 4146 bb10 81dd 161e 4063 f827  ....AF......@c.'
-00002af0: ced1 e8bf 3aa9 3846 21d6 2b5d 8e4f aa8f  ....:.8F!.+].O..
-00002b00: 9db1 bf3a b214 1e1e ac7e 5165 a8a3 2c25  ...:.....~Qe..,%
-00002b10: 2554 62a3 c379 729a f061 3ace 46fd d237  %Tb..yr..a:.F..7
-00002b20: bbfb 0c6a 5507 dc80 b39d 89f2 f2b0 002f  ...jU........../
-00002b30: d1d5 9867 82c1 9882 b41a f5b0 2546 c5df  ...g........%F..
-00002b40: 135d 29f6 05c5 b3d9 1de5 26c9 301b 7d98  .]).......&.0.}.
-00002b50: f03e fc18 387c 0de4 6936 fe4f 2ceb d8ff  .>..8|..i6.O,...
-00002b60: 0000 00ff ff00 0000 ffff 94d0 d10a c220  ............... 
-00002b70: 1480 e157 91f3 0039 9d15 8c33 a1cd 1711  ...W...9...3....
-00002b80: 13ba 5a31 65d5 db4f 5b39 d4ab ee44 3ff1  ..Z1e..O[9...D?.
-00002b90: 3fa2 bb59 eb95 f65a e27c 7f92 b907 06c4  ?..Y...Z.|......
-00002ba0: 3df4 e4c2 aa13 405e 4c68 d35d dfca 3a63  =.....@^Lh.]..:c
-00002bb0: 27df 4373 e047 9068 a2bd 44fc b912 0e5c  '.Cs.G.h..D....\
-00002bc0: d85d 6483 7491 48cd 570c b5e0 b918 6bc1  .]d.t.H.W.....k.
-00002bd0: da9c a89a ec82 86ee 14cf ff89 8f38 8f17  .............8..
-00002be0: 45fc 4fc4 c18a a671 3b6b 81a4 d1d9 b9c8  E.O....q;k......
-00002bf0: ae1f 3825 b165 d3fd ff57 0000 00ff ff00  ..8%.e...W......
-00002c00: 0000 ffff 748e 4b0e 8330 0c44 af12 e500  ....t.K..0.D....
-00002c10: 854a a51f 0958 b16d 85c4 0902 3560 15e2  .J...X.m....5`..
-00002c20: c831 adc4 e91b 52b1 ac57 9ef1 d38c 7367  .1....R..W....sg
-00002c30: 06b8 1b1e d07a 3541 2f85 4e0f 17ad 1887  .....z5A/.N.....
-00002c40: 71df 855c 7433 ad5a 12a1 7957 2398 27f0  q..\t3.Z..yW#.'.
-00002c50: a6b2 e3f1 9a66 fb9c 6e67 ad7a 22f9 774c  .....f..ng.z".wL
-00002c60: ca7c eb6d 4016 a79c 71c0 0dae 1082 b4f2  .|.m@...q.......
-00002c70: 9d99 7e5b 8fec a50e d863 99db 98a4 1531  ..~[.....c.....1
-00002c80: 8215 2348 b6d0 8e58 d8a0 68b5 78a8 196d  ..#H...X..h.x..m
-00002c90: e8ab a037 cb24 3e66 8d01 5f29 f053 e530  ...7.$>f.._).S.0
-00002ca0: 3a6f 60c1 d0b0 eb8e 1c42 84c3 4bc9 87f8  :o`......B..K...
-00002cb0: e547 0029 bf00 0000 ffff 0300 504b 0304  .G.)........PK..
-00002cc0: 1400 0600 0800 0000 2100 85a1 db38 bc03  ........!....8..
-00002cd0: 0000 e00a 0000 1900 0000 786c 2f77 6f72  ..........xl/wor
-00002ce0: 6b73 6865 6574 732f 7368 6565 7431 302e  ksheets/sheet10.
-00002cf0: 786d 6c9c 935d 6fdb 2014 86ef 27ed 3f20  xml..]o. ...'.? 
-00002d00: ee63 6c37 9f96 9daa 6a57 adbb 98a6 addb  .cl7....jW......
-00002d10: ae09 3e8e 51c0 7840 be36 edbf ef60 374e  ..>.Q.x@.6...`7N
-00002d20: a568 5254 6403 86c3 f372 e075 7e7b d08a  .hRTd....r.u~{..
-00002d30: ecc0 3a69 9a82 2651 4c09 34c2 94b2 5917  ..:i..&QL.4...Y.
-00002d40: f4fb f3e3 684e 89f3 bc29 b932 0d14 f408  ....hN...).2....
-00002d50: 8ede 2edf bfcb f7c6 6e5c 0de0 0912 1a57  ........n\.....W
-00002d60: d0da fb36 63cc 891a 3477 9169 a1c1 99ca  ...6c...4w.i....
-00002d70: 58cd 3d7e da35 73ad 055e 768b b462 691c  X.=~.5s..^v..bi.
-00002d80: 4f99 e6b2 a13d 21b3 d730 4c55 4901 0f46  O....=!..0LUI..F
-00002d90: 6c35 34be 8758 50dc e3fe 5d2d 5b77 a269  l54..XP...]-[w.i
-00002da0: 710d 4e73 bbd9 b623 6174 8b88 9554 d21f  q.Ns...#at...T..
-00002db0: 3b28 255a 644f ebc6 58be 5298 f721 1973  ;(%ZdO..X.R..!.s
-00002dc0: 410e 169f 14df 9b93 4c37 7ea1 a4a5 b0c6  A.......L7~.....
-00002dd0: 99ca 4748 66fd 9e2f d35f b005 e362 205d  ..GHf../._...b ]
-00002de0: e67f 1526 1933 0b3b 192e f08c 4adf b6a5  ...&.3.;....J...
-00002df0: 6432 b0d2 33ec e68d b0e9 000b c765 b3ad  d2..3........e..
-00002e00: 2c0b fa27 7e29 236c 9350 c5a3 7811 aa57  ,..'~)#l.P..x..W
-00002e10: e52f 5de6 a5c4 1b0e 5911 0b55 41ef 92ec  ./].....Y..UA...
-00002e20: c38c b265 def9 e787 84bd 7bd5 27bf 8dd1  ...e......{.'...
-00002e30: df04 57f0 3918 4ea1 9563 b472 30e9 ca98  ..W.9.N..c.r0...
-00002e40: 4d08 7f42 f118 b90e 1488 6017 c2b1 d9c1  M..B......`.....
-00002e50: 3d28 0cbf 9ba1 cf7f f54a b3ec 53a7 c406  =(.......J..S...
-00002e60: a965 7eee 9f64 1f3b 677f b164 c51d dc1b  .e~..d.;g..d....
-00002e70: f553 96be 0eba 9494 50f1 adf2 e7c1 4594  .S......P.....E.
-00002e80: 8ce3 693a 19a6 be9a fd47 90eb dae3 021c  ..i:.....G......
-00002e90: ed5c 9495 c707 7002 6d8d 1b8d 3018 9315  .\....p.m...0...
-00002ea0: 46a1 1ed6 44cb f07f a22d f9a1 a078 9efb  F...D....-...x..
-00002eb0: 5e6e 1e8d d3c9 6c9e 0ce1 7d20 32bb c024  ^n....l...} 2..$
-00002ec0: 4ea7 ff89 651d fb1f 0000 00ff ff00 0000  N...e...........
-00002ed0: ffff 94d4 e16e 8230 10c0 f157 217d 8041  .....n.0...W!}.A
-00002ee0: 5bb0 ce54 920d 7c10 8224 fbe4 164b 747b  [..T..|..$...Kt{
-00002ef0: fb5d 3b0b ed9d 25eb 37c3 fdf5 f861 a836  .];...%.7....a.6
-00002f00: 1fd3 34f7 c33c b4fa fa79 2fae 47c6 5961  ..4..<...y/.G.Ya
-00002f10: be86 8b81 4f87 8615 dfbc 1ec6 c3f9 a79f  ....O...........
-00002f20: cc38 5de6 23ab 5e44 c35a 3dda f6cd c6ee  .8].#.^D.Z=.....
-00002f30: 2b30 3070 f5d6 56ba bcb5 ba1c 1fc5 3b2d  +00p..V.......;-
-00002f40: 545c 74b4 1071 d1d3 82cb 3839 d164 2d4a  T\t..q....89.d-J
-00002f50: 902d 3c91 c3b3 71cc ab11 cf17 96be db23  .-<...q........#
-00002f60: 7c17 4e65 83a6 3d4c 97c7 c6f7 0844 57af  |.Ne..=L.....DW.
-00002f70: 4504 9239 201b 6f83 7ce1 40af 1814 4e9b  E..9 .o.|.@...N.
-00002f80: 0a83 609a 06d1 d509 509d 03b2 f136 c817  ..`.....P....6..
-00002f90: 16a4 f02d 77e1 9457 4404 e3b4 88ee 4e88  ...-w..WD.....N.
-00002fa0: e035 faff 2b65 e36d 912f 9c88 e3bf 289c  .5..+e.m./....(.
-00002fb0: 0a2a 8271 5a44 7727 44bb 1c91 8db7 45be  .*.qZDw'D.....E.
-00002fc0: 7022 8145 e154 5211 8cd3 22ba 3b21 5239  p".E.TR...".;!R9
-00002fd0: 2288 9795 f844 50ee 1854 122b feae 3fb9  "....DP..T.+..?.
-00002fe0: fff0 c7c8 3110 0ef1 9d97 ebe1 fd0b 0000  ....1...........
-00002ff0: ffff 0000 00ff ff74 8e4b 0e83 300c 44af  .......t.K..0.D.
-00003000: 12e5 0085 4aa5 1f09 58b1 6d85 c409 0235  ....J...X.m....5
-00003010: 6015 e2c8 31ad c4e9 1b52 b1ac 579e f1d3  `...1....R..W...
-00003020: 8c73 6706 b81b 1ed0 7a35 412f 854e 0f17  .sg.....z5A/.N..
-00003030: ad18 8771 df85 5c74 33ad 5a12 a179 5723  ...q..\t3.Z..yW#
-00003040: 9827 f0a6 b2e3 f19a 66fb 9c6e 67ad 7a22  .'......f..ng.z"
-00003050: f977 4cca 7ceb 6d40 16a7 9c71 c00d ae10  .wL.|.m@...q....
-00003060: 82b4 f29d 997e 5b8f eca5 0ed8 6399 db98  .....~[.....c...
-00003070: a415 3182 1523 48b6 d08e 58d8 a068 b578  ..1..#H...X..h.x
-00003080: a819 6de8 aba0 37cb 243e 668d 015f 29f0  ..m...7.$>f.._).
-00003090: 53e5 303a 6f60 c1d0 b0eb 8e1c 4284 c34b  S.0:o`......B..K
-000030a0: c987 f8e5 4700 29bf 0000 00ff ff03 0050  ....G.)........P
-000030b0: 4b03 0414 0006 0008 0000 0021 0095 8c23  K..........!...#
-000030c0: 639e 0300 0018 0a00 0019 0000 0078 6c2f  c............xl/
-000030d0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-000030e0: 3131 2e78 6d6c 9c93 4d8f 9b30 1086 ef95  11.xml..M..0....
-000030f0: fa1f 2cdf 8381 4dd2 0441 56ab dd44 dd4b  ..,...M..AV..D.K
-00003100: 55f5 f3ec 9821 58b1 31b5 9daf 56fd ef1d  U....!X.1...V...
-00003110: c386 ac94 1ea2 4560 1b7b fcbc 33f8 25bf  ......E`.{..3.%.
-00003120: 3f6a 45f6 609d 344d 4193 28a6 041a 614a  ?jE.`.4MA.(...aJ
-00003130: d96c 0afa fddb 6a34 a3c4 79de 945c 9906  .l....j4..y..\..
-00003140: 0a7a 0247 ef17 efdf e507 63b7 ae06 f004  .z.G......c.....
-00003150: 098d 2b68 ed7d 9b31 e644 0d9a bbc8 b4d0  ..+h.}.1.D......
-00003160: e04a 65ac e61e 5fed 86b9 d602 2fbb 4d5a  .Je..._...../.MZ
-00003170: b134 8ea7 4c73 d9d0 9e90 d95b 18a6 aaa4  .4..Ls.....[....
-00003180: 8027 2376 1a1a df43 2c28 ee31 7f57 cbd6  .'#v...C,(.1.W..
-00003190: 9d69 5adc 82d3 dc6e 77ed 4818 dd22 622d  .iZ....nw.H.."b-
-000031a0: 95f4 a70e 4a89 16d9 f3a6 3196 af15 d67d  ....J.....1....}
-000031b0: 4cc6 5c90 a3c5 3bc5 e7ee 2cd3 cd5f 2969  L.\...;...,.._)i
-000031c0: 29ac 71a6 f211 9259 9ff3 75f9 7336 675c  ).q....Y..u.s6g\
-000031d0: 0ca4 ebfa 6fc2 2463 6661 2fc3 015e 50e9  ....o.$cfa/..^P.
-000031e0: db52 4a26 032b bdc0 eede 089b 0eb0 f0b9  .RJ&.+..........
-000031f0: 6cb6 9365 41ff c42f d708 fb24 34f1 287e  l..eA../...$4.(~
-00003200: 08cd abeb 2f5d e4a5 c413 0e55 110b 5541  ..../].....U..UA
-00003210: 1f92 6c35 a16c 9177 fef9 21e1 e05e 8dc9  ..l5.l.w..!..^..
-00003220: 6f63 f457 c115 7c0a 8653 68e5 18ad 1c4c  oc.W..|..Sh....L
-00003230: ba36 661b c29f 513c 46ae 0305 22d8 8570  .6f...Q<F..."..p
-00003240: ecf6 f008 0ac3 9758 affb d529 2dd3 6cd9  .......X...)-.l.
-00003250: 29b1 416a 915f c667 d955 e7ec cf96 acb9  ).Aj._.g.U......
-00003260: 8347 a37e cad2 d741 9792 122a be53 fe32  .G.~...A...*.S.2
-00003270: 398f 9271 3c4d 27c3 d217 73f8 0872 537b  9..q<M'...s..rS{
-00003280: dc80 b39d 8bb2 f2f4 044e a0ad 31d1 0883  .........N..1...
-00003290: b158 6114 ea61 4bb4 0cff 27da 921f 0b3a  .Xa..aK...'....:
-000032a0: c6d2 7ab9 5934 4e27 1f66 c910 de07 4e5f  ..z.Y4N'.f....N_
-000032b0: 0293 38c5 e17f 6359 c7fe 0700 00ff ff00  ..8...cY........
-000032c0: 0000 ffff 9494 5b0e 8230 1045 b742 ba00  ......[..0.E.B..
-000032d0: a115 3092 42a2 a0fb 2048 e217 1a4a 7cec  ..0.B... H...J|.
-000032e0: de96 1148 676c 237f 847b a693 734b 90ea  ...Hgl#..{..sK..
-000032f0: dab6 4355 0f75 21fb db33 e873 c659 a0ee  ..CU.u!..3.s.Y..
-00003300: 75a7 f453 96b2 e0c5 e3ba c92e efaa 554d  u..S..........UM
-00003310: db0d 398b 3622 6185 6c0c 7b30 f038 a203  ..9.6"a.l.{0.8..
-00003320: a5df 3e8a 4886 8f42 86cd 9738 5262 6713  ..>.H..B...8Rbg.
-00003330: 2525 b84d 5494 1036 71fa 71c6 d646 ce14  %%.MT..6q.q..F..
-00003340: 5988 50bb cf05 8835 0518 d82e 2046 054c  Y.P....5.... F.L
-00003350: 8429 27dd a37a 4a3a 9f20 7920 0494 bb89  .)'..zJ:. y ....
-00003360: b039 c431 0be6 1be0 a8e0 33dd 91ce 3b2c  .9.1......3...;,
-00003370: f3ed 1a73 03fb cd27 c298 ef22 6c4e e7b1  ...s...'..."lN..
-00003380: 3910 4e73 88bd e674 87c3 5c9f f2ff 476f  9.Ns...t..\...Go
-00003390: 60bf f944 8ce6 1c9b d379 6c0e 84d3 1c62  `..D.....yl....b
-000033a0: af39 dde1 304f d698 1bd8 6f3e 11a3 b9c0  .9..0O....o>....
-000033b0: e674 1e9b 03e1 3487 d86b 4e77 60f3 70f9  .t....4..kNw`.p.
-000033c0: e97d 0000 00ff ff00 0000 ffff 748e 4b0e  .}..........t.K.
-000033d0: 8330 0c44 af12 e500 854a a51f 0958 b16d  .0.D.....J...X.m
-000033e0: 85c4 0902 3560 15e2 c831 adc4 e91b 52b1  ....5`...1....R.
-000033f0: ac57 9ef1 d38c 7367 06b8 1b1e d07a 3541  .W....sg.....z5A
-00003400: 2f85 4e0f 17ad 1887 71df 855c 7433 ad5a  /.N.....q..\t3.Z
-00003410: 12a1 7957 2398 27f0 a6b2 e3f1 9a66 fb9c  ..yW#.'......f..
-00003420: 6e67 ad7a 22f9 774c ca7c eb6d 4016 a79c  ng.z".wL.|.m@...
-00003430: 71c0 0dae 1082 b4f2 9d99 7e5b 8fec a50e  q.........~[....
-00003440: d863 99db 98a4 1531 8215 2348 b6d0 8e58  .c.....1..#H...X
-00003450: d8a0 68b5 78a8 196d e8ab a037 cb24 3e66  ..h.x..m...7.$>f
-00003460: 8d01 5f29 f053 e530 3a6f 60c1 d0b0 eb8e  .._).S.0:o`.....
-00003470: 1c42 84c3 4bc9 87f8 e547 0029 bf00 0000  .B..K....G.)....
-00003480: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00003490: 2100 8ec7 9b39 7303 0000 a008 0000 1900  !....9s.........
-000034a0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-000034b0: 7368 6565 7431 322e 786d 6c9c 93db 8edb  sheet12.xml.....
-000034c0: 2010 86ef 2bf5 1d10 f731 b6d7 4913 cbce   ...+....1..I...
-000034d0: aadd 74d5 bda9 aa1e af09 1ec7 2860 5c20  ..t.........(`\ 
-000034e0: a756 7df7 0e76 e3ac 1455 8a16 d980 61f8  .V}..v...U....a.
-000034f0: 7e06 7e17 f747 adc8 1eac 93a6 2d69 12c5  ~.~..G......-i..
-00003500: 9440 2b4c 25db 4d49 bf7d 7d9c cc29 719e  .@+L%.MI.}}..)q.
-00003510: b715 57a6 8592 9ec0 d1fb e5eb 57c5 c1d8  ..W.........W...
-00003520: ad6b 003c 4142 eb4a da78 dfe5 8c39 d180  .k.<AB.J.x...9..
-00003530: e62e 321d b438 531b abb9 c74f bb61 aeb3  ..2..8S....O.a..
-00003540: c0ab 7e91 562c 8de3 19d3 5cb6 7420 e4f6  ..~.V,....\.t ..
-00003550: 1686 a96b 2960 65c4 4e43 eb07 8805 c53d  ...k)`e.NC.....=
-00003560: eedf 35b2 7367 9a16 b7e0 34b7 db5d 3711  ..5.sg....4..]7.
-00003570: 4677 8858 4b25 fda9 8752 a245 feb4 698d  Fw.XK%...R.E..i.
-00003580: e56b 8579 1f93 8c0b 72b4 f8a4 f8de 9d65  .k.y....r......e
-00003590: faf1 2b25 2d85 35ce d43e 4232 1bf6 7c9d  ..+%-.5..>B2..|.
-000035a0: fe82 2d18 1723 e93a ff9b 3049 c62c ec65  ..-..#.:..0I.,.e
-000035b0: b8c0 0b2a 7dd9 9692 e9c8 4a2f b0bb 17c2  ...*}.....J/....
-000035c0: 6623 2c1c 97cd 77b2 2ae9 eff8 5f99 609b  f#,...w.*..._.`.
-000035d0: 842a 9ec4 ef42 f5ac fca1 cba2 9278 c321  .*...B.......x.!
-000035e0: 2b62 a12e e9db 247f 9f51 b62c 7aff 7c97  +b....$..Q.,z.|.
-000035f0: 7070 cffa e497 31fa 8be0 0a3e 06c3 29b4  pp....1....>..).
-00003600: 728c 560e 265d 1bb3 0de1 4f28 1e23 d781  r.V.&]....O(.#..
-00003610: 0211 ec42 3836 7b78 0085 e12b ccd7 fdec  ...B86{x...+....
-00003620: 9556 69be ea95 d828 b52c 2efd b3ec 63ef  .Vi....(.,....c.
-00003630: ec4f 96ac b983 07a3 7ec8 ca37 4197 920a  .O......~..7A...
-00003640: 6abe 53fe 32b8 8892 2c9e a5d3 71ea b339  j.S.2...,...q..9
-00003650: 7c00 b969 3c2e c0d1 de45 7975 5a81 1368  |..i<....EyuZ..h
-00003660: 6bdc 6884 c198 ac30 0af5 b026 5a86 ff13  k.h....0...&Z...
-00003670: 6dc9 8f25 c5f3 3c0c 72f3 284b a76f e6c9  m..%..<.r.(K.o..
-00003680: 183e 0422 b30f 4ce2 74f6 9f58 d6b3 ff02  .>."..L.t..X....
-00003690: 0000 ffff 0000 00ff ff94 d3ed 0a83 2014  .............. .
-000036a0: 80e1 5b09 2f20 3d7d d016 266c d585 840b  ..[./ =}..&l....
-000036b0: f6ab 8d8c b6dd fdb4 d687 4726 d4af e8bc  ..........G&....
-000036c0: a18f 1157 f7b6 1daa 6668 04ef 1faf a02f  ...W....fh...../
-000036d0: 0890 403d 9b4e e9bb 3c25 c11b 9246 e6b7  ..@=.N..<%...F..
-000036e0: 4fd5 2ad9 7643 4158 18a5 4470 69da 8b89  O.*.vCAX..Dpi...
-000036f0: a757 f440 e9a7 a360 9c8e 8253 f92b ae6e  .W.@...`...S.+.n
-00003700: 91d9 45e9 1691 5d54 6e01 b19d d46e b215  ..E...]Tn....n..
-00003710: 54cb 565e 7484 6762 9b97 20de 5218 7ac6  T.V^t.gb.. .R.z.
-00003720: 10be dc4f 316a 9ee9 135e 8f0e d0c9 d4ee  ...O1j...^......
-00003730: f2e7 7579 0b15 1f41 99d8 8f5a 8a09 0518  ..uy...A...Z....
-00003740: b59f 4278 42df 6a9e 7a59 ee06 feb0 9223  ..BxB.j.zY.....#
-00003750: 2c13 fb59 4b31 b122 ccda 4f21 0466 5d80  ,..YK1."..O!.f].
-00003760: 9473 ec55 bafb c14a bafd 7c5f 0000 00ff  .s.U...J..|_....
-00003770: ff00 0000 ffff 748e 4b0e 8330 0c44 af12  ......t.K..0.D..
-00003780: e500 854a a51f 0958 b16d 85c4 0902 3560  ...J...X.m....5`
-00003790: 15e2 c831 adc4 e91b 52b1 ac57 9ef1 d38c  ...1....R..W....
-000037a0: 7367 06b8 1b1e d07a 3541 2f85 4e0f 17ad  sg.....z5A/.N...
-000037b0: 1887 71df 855c 7433 ad5a 12a1 7957 2398  ..q..\t3.Z..yW#.
-000037c0: 27f0 a6b2 e3f1 9a66 fb9c 6e67 ad7a 22f9  '......f..ng.z".
-000037d0: 774c ca7c eb6d 4016 a79c 71c0 0dae 1082  wL.|.m@...q.....
-000037e0: b4f2 9d99 7e5b 8fec a50e d863 99db 98a4  ....~[.....c....
-000037f0: 1531 8215 2348 b6d0 8e58 d8a0 68b5 78a8  .1..#H...X..h.x.
-00003800: 196d e8ab a037 cb24 3e66 8d01 5f29 f053  .m...7.$>f.._).S
-00003810: e530 3a6f 60c1 d0b0 eb8e 1c42 84c3 4bc9  .0:o`......B..K.
-00003820: 87f8 e547 0029 bf00 0000 ffff 0300 504b  ...G.)........PK
-00003830: 0304 1400 0600 0800 0000 2100 445e 6938  ..........!.D^i8
-00003840: 8403 0000 0708 0000 1900 0000 786c 2f77  ............xl/w
-00003850: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00003860: 332e 786d 6c9c 93c9 6edb 3010 86ef 05f2  3.xml...n.0.....
-00003870: 0e04 ef16 45c5 3662 c172 1038 0d9a 4b51  ....E.6b.r.8..KQ
-00003880: 743d d3d4 c822 cc45 25e9 ad45 dfbd 4339  t=...".E%..E..C9
-00003890: 5e00 5f8c 1012 4971 f9fe 19f2 d7f4 7167  ^._...Iq......qg
-000038a0: 34d9 800f cad9 8af2 2ca7 04ac 74b5 b2cb  4.......,...t...
-000038b0: 8afe f8fe 3278 a024 4461 6ba1 9d85 8aee  ....2x.$Dak.....
-000038c0: 21d0 c7d9 dd87 e9d6 f955 6801 2241 820d  !........Uh."A..
-000038d0: 156d 63ec 4ac6 826c c188 90b9 0e2c ce34  .mc.J..l.....,.4
-000038e0: ce1b 11f1 d32f 59e8 3c88 badf 6434 2bf2  ...../Y.<...d4+.
-000038f0: 7ccc 8c50 961e 08a5 bf85 e19a 4649 7876  |..P........FIxv
-00003900: 726d c0c6 03c4 8316 11e3 0fad eac2 9166  rm.............f
-00003910: e42d 3823 fc6a dd0d a433 1d22 164a abb8  .-8#.j...3.".J..
-00003920: efa1 9418 59be 2ead f362 a131 ef1d 1f0a  ....Y....b.1....
-00003930: 4976 1e9f 02df fba3 4c3f 7ea5 6494 f42e  Iv......L?~.d...
-00003940: b826 6648 6687 98af d39f b009 13f2 44ba  .&fHf.........D.
-00003950: ceff 260c 1f32 0f1b 952e f08c 2ade 1712  ..&..2......*...
-00003960: 1f9d 58c5 1976 ff4e d8f8 044b c7e5 cbb5  ..X..v.N...K....
-00003970: aa2b fa37 7f2b 036c 79aa f241 3e4f d545  .+.7.+.ly..A>O.E
-00003980: f947 67d3 5ae1 0da7 ac88 87a6 a24f bcfc  .Gg.Z........O..
-00003990: 38a4 6c36 edfd f353 c136 5cf4 c91f e7cc  8.l6...S.6\.....
-000039a0: 3729 347c 4e86 d368 e51c ad9c 4cba 706e  7)4|N..h....L.pn
-000039b0: 9596 bfa2 788e dc00 1a64 b20b 11d8 6c60  ....x....d....l`
-000039c0: 0e1a 97cf 39c6 187e f752 a98f 42ec a474  ....9..~.R..B..t
-000039d0: d93f aabe f4c6 fee2 c942 0498 3bfd 4bd5  .?.......B..;.K.
-000039e0: b14d b294 d4d0 88b5 8ee7 c149 c687 f9b8  .M.........I....
-000039f0: 189d a6be baed 2750 cb36 e206 1ced 4d54  ......'P.6....MT
-00003a00: d6fb 6708 125d 8d71 66b8 1843 904e a31e  ..g..].qf..C.N..
-00003a10: d6c4 a8f4 7ba2 2bc5 2e89 24d6 f64d 9167  ....{.+...$..M.g
-00003a20: c5c3 888f 123f 45dd eff9 0f00 00ff ff00  .....?E.........
-00003a30: 0000 ffff 9492 ed0a c220 1846 6f65 7801  ......... .Foex.
-00003a40: f931 6534 9c50 e985 8809 fd5a 3165 d5dd  .1e4.P.....Z1e..
-00003a50: 6719 4e85 02ff a9e7 f5e1 3922 7717 6bbd  g.N.......9"w.k.
-00003a60: d45e 0bbe 5cef dd32 010c 3a77 d3b3 0bab  .^..\..2..:w....
-00003a70: 9181 ee81 a936 e3f9 29ad 3376 f613 403b  .....6..).3v..@;
-00003a80: c280 e0e6 3d7b 08c3 e1c8 85fd 2a10 87ab  ....={......*...
-00003a90: e0d0 7cd9 3167 b864 a782 ed4b 2873 48aa  ..|.1g.d...K(sH.
-00003aa0: 5495 c321 5d84 a17c 3220 2d06 6138 19d0  T..!]..|2 -.a8..
-00003ab0: ca20 67ac 32f8 c364 ce48 a5ae c8e7 b106  . g.2..d.H......
-00003ac0: b489 15e5 fb86 f2aa 8f59 f847 166d c9a2  .........Y.G.m..
-00003ad0: 312b 7bf0 d80b 6e5f e405 0000 ffff 0000  1+{...n_........
-00003ae0: 00ff ff94 8fcb 4ec3 3010 457f c5f2 8215  ......N.0.E.....
-00003af0: 6ada 0a94 2292 4888 0ab1 a18a 5a7e c06d  j...".H.....Z~.m
-00003b00: 26c9 0827 638d 2754 ead7 e3b8 9487 4416  &..'c.'T......D.
-00003b10: 78e1 d7bd 73e6 4ee6 4c03 2f86 1bec bdb2  x...s.N.L./.....
-00003b20: 504b aee7 b374 95de dcfd 582b ad18 9b76  PK...t....X+...v
-00003b30: 4a13 72b9 5ecc e6b7 cbf4 6b85 923d 8950  J.r.^.....k..=.P
-00003b40: f797 d282 a980 273a d544 3225 2645 36e6  ......':.D2%&E6.
-00003b50: dd81 0c4e 39e3 8077 7882 00d2 ca1f 8c3d  ...N9..wx......=
-00003b60: df6a 642f 65b0 6d86 6e1f 495a 1123 f462  .jd/e.m.n.IZ.#.b
-00003b70: 04a9 cfb5 2316 3628 5a0d 1e4a c63e f45b  ....#.6(Z..J.>.[
-00003b80: 436d 062b 3eb2 da60 3f51 f0db b5c3 f8f3  Cm.+>..`?Q......
-00003b90: 0e2c 183a 5cde 0772 08d1 1c22 9dc7 798a  .,.:\..r..."..y.
-00003ba0: b98b 8caa ea39 ce57 5c99 cedd 3fc6 5dbf  .....9.W\...?.].
-00003bb0: 6207 5e6d e0a8 b6d4 99fe 7a0b cd60 0deb  b.^m......z..`..
-00003bc0: a82e 96f1 78c8 92ef e291 f389 fc07 671c  ....x.........g.
-00003bd0: 5b45 7f19 6197 50c9 ef8c c991 f8cd b700  [E..a.P.........
-00003be0: 527c 0000 00ff ff03 0050 4b03 0414 0006  R|.......PK.....
-00003bf0: 0008 0000 0021 0058 0737 e94e 0700 00c0  .....!.X.7.N....
-00003c00: 2000 0013 0000 0078 6c2f 7468 656d 652f   ......xl/theme/
-00003c10: 7468 656d 6531 2e78 6d6c ec59 cd8b 1b37  theme1.xml.Y...7
-00003c20: 14bf 17fa 3f0c 7377 fc35 e38f 25de e0cf  ....?.sw.5..%...
-00003c30: 6c93 dd24 649d 941c b5b6 ec51 5633 3292  l..$d......QV32.
-00003c40: bc1b 1302 2539 f552 28a4 a597 426f 3d94  ....%9.R(...Bo=.
-00003c50: d240 030d bdf4 8f09 24b4 e91f d127 cdd8  .@......$....'..
-00003c60: 23ad e524 9b6c 4a5a 760d 8b47 febd a7a7  #..$.lJZv..G....
-00003c70: f79e 7e7a f374 f1d2 bd98 7a47 980b c292  ..~z.t....zG....
-00003c80: 965f be50 f23d 9c8c d898 24d3 967f 6b38  ._.P.=....$...k8
-00003c90: 2834 7c4f 4894 8c11 6509 6ef9 0b2c fc4b  (4|OH...e.n..,.K
-00003ca0: db9f 7e72 116d c908 c7d8 03f9 446c a196  ..~r.m......Dl..
-00003cb0: 1f49 39db 2a16 c508 8691 b8c0 6638 81df  .I9.*.......f8..
-00003cc0: 268c c748 c223 9f16 c71c 1d83 de98 162b  &..H.#.........+
-00003cd0: a552 ad18 2392 f85e 8262 507b 7d32 2123  .R..#..^.bP{}2!#
-00003ce0: ec6f 2fd5 f629 e84e a450 0323 caf7 9552  .o/..).N.P.#...R
-00003cf0: bc8e 1d1f 9615 422c 4497 72ef 08d1 960f  ......B,D.r.....
-00003d00: 338c d9f1 10df 93be 4791 90f0 43cb 2fe9  3.......G...C./.
-00003d10: 3fbf b87d b188 b632 212a 37c8 1a72 03fd  ?..}...2!*7..r..
-00003d20: 97c9 6502 e3c3 8a9e 934f 0f56 9306 4118  ..e......O.V..A.
-00003d30: d4da 2bfd 1a40 e53a ae5f efd7 fab5 953e  ..+..@.:._.....>
-00003d40: 0d40 a311 ac34 b5c5 d659 af74 830c 6b80  .@...4...Y.t..k.
-00003d50: d2af 0edd bd7a af5a b6f0 86fe ea9a cded  .....z.Z........
-00003d60: 507d 2cbc 06a5 fa83 35fc 60d0 052f 5a78  P},.....5.`../Zx
-00003d70: 0d4a f1e1 1a3e ec34 3b3d 5bbf 06a5 f8da  .J...>.4;=[.....
-00003d80: 1abe 5e6a f782 baa5 5f83 224a 92c3 3574  ..^j...._."J..5t
-00003d90: 29ac 55bb cbd5 ae20 1346 779c f066 180c  ).U.... .Fw..f..
-00003da0: ea95 4c79 8e82 6c58 6597 9a62 c212 b929  ..Ly..lXe..b...)
-00003db0: d762 7497 f101 0014 9022 4912 4f2e 6678  .bt......"I.O.fx
-00003dc0: 8246 90bf 5d44 c901 27de 2e99 4690 7833  .F..]D..'...F.x3
-00003dd0: 9430 01c3 a54a 6950 aac2 7ff5 09f4 371d  .0...JiP......7.
-00003de0: 51b4 8591 21ad ec02 4bc4 da90 b2c7 1323  Q...!...K......#
-00003df0: 4e66 b2e5 5f01 adbe 0179 f1ec d9f3 874f  Nf.._....y.....O
-00003e00: 9f3f fced f9a3 47cf 1ffe 92cd ad55 5972  .?....G......UYr
-00003e10: 3b28 999a 72af 7efc faef efbf f0fe faf5  ;(..r.~.........
-00003e20: 8757 8fbf 49a7 3e89 1726 fee5 cf5f befc  .W..I.>..&..._..
-00003e30: fd8f d7a9 8715 e7ae 78f1 ed93 974f 9fbc  ........x....O..
-00003e40: f8ee ab3f 7f7a ecd0 dee6 e8c0 840f 498c  ...?.z........I.
-00003e50: 8577 0d1f 7b37 590c 0b74 d88f 0ff8 e924  .w..{7Y..t.....$
-00003e60: 8611 2296 048a 40b7 4375 5f46 16f0 da02  .."...@.Cu_F....
-00003e70: 5117 ae83 6d17 dee6 c032 2ee0 e5f9 5dcb  Q...m....2....].
-00003e80: d6fd 88cf 2571 cc7c 358a 2de0 1e63 b4c3  ....%q.|5.-..c..
-00003e90: b8d3 0157 d55c 8687 87f3 64ea 9e9c cf4d  ...W.\....d....M
-00003ea0: dc4d 848e 5c73 7751 6205 b83f 9f01 bd12  .M..\swQb..?....
-00003eb0: 97ca 6e84 2d33 6f50 9448 34c5 0996 9efa  ..n.-3oP.H4.....
-00003ec0: 8d1d 62ec 58dd 1d42 2cbf ee91 1167 824d  ..b.X..B,....g.M
-00003ed0: a477 8778 1d44 9c2e 1992 032b 9172 a11d  .w.x.D.....+.r..
-00003ee0: 1243 5c16 2e03 21d4 966f f66e 7b1d 465d  .C\...!..o.n{.F]
-00003ef0: abee e123 1b09 db02 5187 f143 4c2d 375e  ...#....Q..CL-7^
-00003f00: 4673 8962 97ca 218a a9e9 f05d 2423 9791  Fs.b..!....]$#..
-00003f10: fb0b 3e32 717d 2121 d253 4c99 d71f 6321  ..>2q}!!.SL...c!
-00003f20: 5c32 d739 acd7 08fa 5560 1877 d8f7 e822  \2.9....U`.w..."
-00003f30: b691 5c92 4397 ce5d c498 89ec b1c3 6e84  ..\.C..]......n.
-00003f40: e299 d366 9244 26f6 3371 0829 8abc 1b4c  ...f.D&.3q.)...L
-00003f50: bae0 7bcc de21 ea19 e280 928d e1be 4db0  ..{..!........M.
-00003f60: 15ee 3713 c12d 2057 d3a4 3c41 d42f 73ee  ..7..- W..<A./s.
-00003f70: 88e5 65cc ecfd b8a0 1384 5d2c d3e6 b1c5  ..e.......],....
-00003f80: ae6d 4e9c d9d1 994f add4 dec5 98a2 6334  .mN....O......c4
-00003f90: c6d8 bbf5 99c3 820e 9b59 3ecf 8dbe 1201  .........Y>.....
-00003fa0: abec 6057 625d 4176 aeaa e704 0bec e9ba  ..`Wb]Av........
-00003fb0: 669d 2277 89b0 5276 1f4f d906 7bf6 1627  f."w..Rv.O..{..'
-00003fc0: 8867 8192 18f1 4d9a af41 d4ad d485 53ce  .g....M..A....S.
-00003fd0: 49a5 d7e9 e8d0 045e 2350 f841 be38 9d72  I......^#P.A.8.r
-00003fe0: 5d80 0e23 b9fb 9bb4 de88 9075 76a9 67e1  ]..#.......uv.g.
-00003ff0: ced7 05b7 e2f7 367b 0cf6 e5dd d3ee 4b90  ......6{......K.
-00004000: c1a7 9601 627f 6bdf 0c11 b526 c813 6688  ....b.k....&..f.
-00004010: a0c0 70d1 2d88 58e1 cf45 d4b9 aac5 e64e  ..p.-.X..E.....N
-00004020: b989 bd69 f330 4061 64d5 3b31 49de 58fc  ...i.0@ad.;1I.X.
-00004030: 9c28 7bc2 7fa7 ec71 1730 6750 f0b8 15bf  .({....q.0gP....
-00004040: 4fa9 b389 5276 4e14 389b 70ff c1b2 a687  O...RvN.8.p.....
-00004050: e6c9 0d0c 27c9 3a67 9d57 35e7 558d ffbf  ....'.:g.W5.U...
-00004060: af6a 36ed e5f3 5ae6 bc96 39af 655c 6f5f  .j6...Z...9.e\o_
-00004070: 1fa4 96c9 cb17 a86c f22e 8fee f9c4 1b5b  .......l.......[
-00004080: 3e13 42e9 be5c 50bc 2b74 d747 c01b cd78  >.B..\P.+t.G...x
-00004090: 0083 ba1d a57b 92ab 16e0 2c82 af59 83c9  .....{....,..Y..
-000040a0: c24d 39d2 321e 67f2 7322 a3fd 08cd a035  .M9.2.g.s".....5
-000040b0: 54d6 cdce a9c8 544f 8537 6302 3a46 7a58  T.....TO.7c.:FzX
-000040c0: 3751 f109 ddba ef34 8ff7 d838 ed74 96cb  7Q.....4...8.t..
-000040d0: aaab 99ba 5020 998f 97c2 d538 74a9 648a  ....P .....8t.d.
-000040e0: aed5 f3ee dd4a bdee 874e 7597 7569 8092  .....J...Nu.ui..
-000040f0: 3d8d 11c6 64b6 1155 8711 f5e5 2044 e175  =...d..U.... D.u
-00004100: 46e8 959d 8915 4d87 150d a57e 19aa 6514  F.....M....~..e.
-00004110: 57ae 00d3 5651 8157 6e0f 5ed4 5b7e 18a4  W...VQ.Wn.^.[~..
-00004120: 1d64 68c6 4179 3e56 714a 9bc9 cbe8 aae0  .dh.Ay>VqJ......
-00004130: 9c69 a437 3993 9a19 0025 f632 03f2 4837  .i.79....%.2..H7
-00004140: 95ad 1b97 a756 97a6 da5b 44da 32c2 4837  .....V...[D.2.H7
-00004150: db08 230d 2378 11ce b2d3 6cb9 9f65 ac9b  ..#.#x....l..e..
-00004160: 7948 2df3 942b 96bb 2137 a3de f810 b156  yH-..+..!7.....V
-00004170: 2472 821b 6862 3205 4dbc e396 5fab 8670  $r..hb2.M..._..p
-00004180: 9f32 42b3 963f 818e 317c 8d67 903b 42bd  .2B..?..1|.g.;B.
-00004190: 7521 3a85 0b97 91e4 e986 7f17 6699 7121  u!:.........f.q!
-000041a0: 7b48 44a9 c335 e9a4 6c10 1389 b947 49dc  {HD..5..l....GI.
-000041b0: f2d5 f257 d940 13cd 21da b672 0508 e1a3  ...W.@..!..r....
-000041c0: 35ae 09b4 f2b1 1907 41b7 838c 2713 3c92  5.......A...'.<.
-000041d0: 66d8 8d11 e5e9 f411 183e e50a e7af 5afc  f........>....Z.
-000041e0: ddc1 4a92 cd21 dcfb d1f8 d83b a073 7e13  ..J..!.....;.s~.
-000041f0: 418a 85f5 b272 e098 08b8 3828 a7de 1c13  A....r....8(....
-00004200: b809 5b11 599e 7f27 0ea6 8c76 cdab 289d  ..[.Y..'...v..(.
-00004210: 43e9 38a2 b308 6527 8a49 e629 5c93 e8ca  C.8...e'.I.)\...
-00004220: 1cfd b4f2 81f1 94ad 191c baee c283 a93a  ...............:
-00004230: 60df fbd4 7df3 51ad 3c67 9066 7e66 5aac  `...}.Q.<g.f~fZ.
-00004240: a24e 4d37 997e b843 deb0 2a3f 442d ab52  .NM7.~.C..*?D-.R
-00004250: ead6 efd4 22e7 bae6 92eb 2051 9da7 c41b  ...."..... Q....
-00004260: 4edd b738 100c d3f2 c92c d394 c5eb 34ac  N..8.....,....4.
-00004270: 383b 1bb5 4d3b c382 c0f0 446d 83df 5667  8;..M;....Dm..Vg
-00004280: 84d3 13ef 7af2 83dc c9ac 5507 c4b2 aed4  ....z.....U.....
-00004290: 89af 2fcb cd5b 6d76 7017 c8a3 07f7 8773  ../..[mvp......s
-000042a0: 2a85 0e25 dc59 7304 455f 7a03 99d2 066c  *..%.Ys.E_z....l
-000042b0: 917b 32ab 11e1 9b37 e7a4 e5df 2f85 eda0  .{2....7..../...
-000042c0: 5b09 bb85 5223 ec17 826a 502a 34c2 76b5  [...R#...jP*4.v.
-000042d0: d00e c36a b91f 964b bd4e e501 1c2c 328a  ...j...K.N...,2.
-000042e0: cb61 7a51 3f80 2b0c bac8 aeeb f5f8 da95  .azQ?.+.........
-000042f0: 7dbc bca5 b930 6271 91e9 2bf9 a236 5c5f  }....0bq..+..6\_
-00004300: d997 2b8e 2b7b 6fa8 6ee6 7d8f 00e9 dcaf  ..+.+{o.n.}.....
-00004310: 5506 cd6a b353 2b34 abed 4121 e875 1a85  U..j.S+4..A!.u..
-00004320: 66b7 d629 f46a dd7a 6fd0 eb86 8de6 e081  f..).j.zo.......
-00004330: ef1d 6970 d0ae 7683 5abf 51a8 95bb dd42  ..ip..v.Z.Q....B
-00004340: 502b 29f3 1bcd 423d a854 da41 bddd e807  P+)...B=.T.A....
-00004350: ed07 5919 032b 4fe9 23f3 05b8 57db b5fd  ..Y..+O.#...W...
-00004360: 0f00 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00004370: 0800 0000 2100 64c1 ee86 ed02 0000 0608  ....!.d.........
-00004380: 0000 0d00 0000 786c 2f73 7479 6c65 732e  ......xl/styles.
-00004390: 786d 6cb4 555d 6fd3 3014 7d47 e23f 587e  xml.U]o.0.}G.?X~
-000043a0: cff2 b1a6 b455 9289 ae8b 3409 d0a4 0e89  .....U....4.....
-000043b0: 5727 715a 6bfe 088e 5352 10ff 9deb a44d  W'qZk...SR.....M
-000043c0: 5a6d 82b1 411f 9aeb 6bfb f8dc 7b8f afa3  Zm..A...k...{...
-000043d0: ab56 70b4 a3ba 664a c6d8 bff0 30a2 3257  .Vp...fJ....0.2W
-000043e0: 0593 9b18 7fbe 4f9d 1946 b521 b220 5c49  ......O..F.!. \I
-000043f0: 1ae3 3dad f155 f2f6 4d54 9b3d a7eb 2da5  ..=..U..MT.=..-.
-00004400: 0601 84ac 63bc 35a6 5ab8 6e9d 6fa9 20f5  ....c.5.Z.n.o. .
-00004410: 85aa a884 9952 6941 0c0c f5c6 ad2b 4d49  .....RiA.....+MI
-00004420: 51db 4d82 bb81 e74d 5d41 98c4 3dc2 42e4  Q.M....M]A..=.B.
-00004430: cf01 1144 3f34 9593 2b51 11c3 32c6 99d9  ...D?4..+Q..2...
-00004440: 7758 1889 7c71 bb91 4a93 8c03 d5d6 9f90  wX..|q..J.......
-00004450: 1cb5 fe54 07a8 d5c7 433a efa3 7304 cbb5  ...T....C:..s...
-00004460: aa55 692e 00d7 5565 c972 fa98 eedc 9dbb  .Ui...Ue.r......
-00004470: 241f 9100 f965 487e e87a c159 ecad 7e21  $....eH~.z.Y..~!
-00004480: d2c4 d574 c76c f970 1295 4a9a 1ae5 aa91  ...t.l.p..J.....
-00004490: 068a 0944 6d0a 160f 527d 93a9 9db2 ce7e  ...Dm...R}.....~
-000044a0: 5512 d5df d18e 70f0 f8d8 4da2 5c71 a591  U.....p...M.\q..
-000044b0: de64 314e 53af fb59 b724 82f6 cbae 0967  .d1NS..Y.$.....g
-000044c0: 9966 d659 12c1 f8be 7707 dde6 2dd1 3508  .f.Y....w...-.5.
-000044d0: a1c7 b31e d732 397c 6ad8 c138 1f78 0596  .....29|j..8.x..
-000044e0: 0238 9208 0a68 a896 290c d0c1 bedf 5750  .8...h..).....WP
-000044f0: 3a09 5aeb 61ba 757f 58bd d164 ef07 e1c9  :.Z.a.u.X..d....
-00004500: 06b7 3b30 8932 a50b d0f6 9891 a32b 8938  ..;0.2.......+.8
-00004510: 2d0d 10d5 6cb3 b55f a32a f8cf 9431 50ff  -...l.._.*...1P.
-00004520: 242a 18d9 2849 b80d a507 190c 0827 a79c  $*..(I.......'..
-00004530: afad febf 9467 d86d 8964 2352 616e 8b18  .....g.m.d#Ran..
-00004540: c34d b249 389a 10c8 c1ec f1fa 81c5 3f45  .M.I8.........?E
-00004550: ebb1 4f60 a790 acbf 8745 6d39 e0bf 6237  ..O`.....Em9..b7
-00004560: 2255 c5f7 5639 5638 c0f5 0c0b 84f3 8c08  "U..V9V8........
-00004570: 072a 3dd8 a746 6454 a75d 5378 0af4 5959  .*=..FdT.]Sx..YY
-00004580: 1b31 bf36 cad0 3b4d 4bd6 7682 ffa7 849f  .1.6..;MK.v.....
-00004590: 04ff bf01 1cf5 000a 3891 d999 c806 b920  ........8...... 
-000045a0: 7b39 63bc eeba b32e e0b6 1f8a 8eb2 8671  {9c............q
-000045b0: c3e4 1312 03d4 a21d 45eb d9a2 1adb 2e3b  ........E......;
-000045c0: 390f e740 150a 5a92 869b fb61 32c6 a3fd  9..@..Z....a2...
-000045d0: 9116 ac11 c1b0 ea8e ed94 e920 623c da1f  ........... b<..
-000045e0: ecdd f2a7 f60c da9a 0f35 3404 f8a2 46b3  .........54...F.
-000045f0: 18ff b859 be9b af6e d2c0 9979 cb99 33b9  ...Y...n...y..3.
-00004600: a4a1 330f 972b 279c 5c2f 57ab 74ee 05de  ..3..+'.\/W.t...
-00004610: f5cf 93a6 fd8a 96dd bd31 205e 7fb2 a839  .........1 ^...9
-00004620: 3476 7d08 f610 e27a f441 36c7 414f bfeb  4v}....z.A6.AO..
-00004630: 2a40 fb94 fb3c 987a ef43 df73 d24b cf77  *@...<.z.C.s.K.w
-00004640: 2653 3273 66d3 cbd0 4943 3f58 4d27 cb9b  &S2sf...IC?XM'..
-00004650: 300d 4fb8 872f 6ced 9eeb fbfd 2361 c987  0.O../l.....#a..
-00004660: 0bc3 04e5 4c1e 6b75 acd0 a917 8a04 c3df  ....L.ku........
-00004670: 04e1 1e2b e18e 0f78 f20b 0000 ffff 0300  ...+...x........
-00004680: 504b 0304 1400 0600 0800 0000 2100 4792  PK..........!.G.
-00004690: ec58 ce01 0000 b603 0000 1400 0000 786c  .X............xl
-000046a0: 2f73 6861 7265 6453 7472 696e 6773 2e78  /sharedStrings.x
-000046b0: 6d6c 9c53 cb6e db30 10bc 17e8 3f2c 8402  ml.S.n.0....?,..
-000046c0: 4d8b d892 9d38 ea43 5650 c449 2e85 5320  M....8.CVP.I..S 
-000046d0: 0e72 3468 7165 b111 4995 bb72 e2bf efca  .r4hqe..I..r....
-000046e0: 6e80 4242 2f3d 7238 331c ce92 d9e5 8bad  n.BB/=r83.......
-000046f0: 6187 818c 77f3 6832 4e22 4057 786d dc76  a...w.h2N"@Wxm.v
-00004700: 1e3d ac6e 469f 2220 564e abda 3b9c 477b  .=.nF." VN..;.G{
-00004710: a4e8 327f fb26 2362 10ad a379 5431 375f  ..2..&#b...yT17_
-00004720: e298 8a0a ada2 b16f d0c9 4ee9 8355 2ccb  .......o..N..U,.
-00004730: b08d a909 a834 5588 6ceb 789a 2417 b155  .....4U.l.x.$..U
-00004740: c645 50f8 d6b1 9c7b 368b a075 e657 8b57  .EP....{6..u.W.W
-00004750: 4764 3a8d f28c 4c9e 71ee bcc6 2ce6 3c8b  Gd:...L.q...,.<.
-00004760: bbf5 1123 2cd8 873e ba53 753b a03a cf03  ...#,..>.Su;.:..
-00004770: ec11 8931 78ea 1bd4 665b 711f 64f5 840e  ...1x...f[q.d...
-00004780: cae0 2de0 8b21 966a c0aa 2278 d08a 1594  ..-..!.j.."x....
-00004790: a6c6 81d1 1ed5 209d 0401 6a03 c273 a518  ...... ...j..s..
-000047a0: d843 d332 2882 9d0a 466d 6a84 dbc5 0f58  .C.2(...Fmj....X
-000047b0: 2caf 419a 837f 25fc d94a ef56 6984 b639  ,.A...%..J.Vi..9
-000047c0: 858d 38fc 4fbc 2025 6bd4 72b4 1476 0a5a  ..8.O. %k.r..v.Z
-000047d0: e6e6 f4ba c1b0 ee82 c347 48c6 b37e 0d01  .........GH..~..
-000047e0: 755b 8866 b307 5216 a154 dd08 802b e560  u[.f..R..T...+.`
-000047f0: 8392 19df 93cc 9378 1db0 3c3a c389 1825  .......x..<:...%
-00004800: 93f4 3c4d d319 9c1c bcd3 24f9 00a3 03fe  ..<M......$.....
-00004810: 0a5d 7c16 08e6 1d96 4c0f dcaf 7ff4 9319  .]|.....L.......
-00004820: 3c4b 4365 1717 8c83 abbb fbd5 7a79 b7f8  <KCe........zy..
-00004830: f67d bdbc 5ef5 139e 2509 c82c e898 e970  .}..^...%..,...p
-00004840: b74e 549a 209d c9e5 8cd7 7d89 bcb9 c1bc  .NT. .....}.....
-00004850: 1fee 17f1 d3a3 ea53 6fdf 0d90 2169 d4e7  .......So...!i..
-00004860: ac06 aac2 5b2b ff8b f783 c787 3bac 0701  ....[+......;...
-00004870: 09cb f62f 3496 7f97 ff06 0000 ffff 0300  .../4...........
-00004880: 504b 0304 1400 0600 0800 0000 2100 3b6d  PK..........!.;m
-00004890: 324b c100 0000 4201 0000 2300 0000 786c  2K....B...#...xl
-000048a0: 2f77 6f72 6b73 6865 6574 732f 5f72 656c  /worksheets/_rel
-000048b0: 732f 7368 6565 7431 2e78 6d6c 2e72 656c  s/sheet1.xml.rel
-000048c0: 7384 8fc1 8ac2 3014 45f7 03fe 4378 7b93  s.....0.E...Cx{.
-000048d0: d685 0c43 5337 22b8 55e7 0362 fada 06db  ...CS7".U..b....
-000048e0: 9790 f714 fd7b b31c 65c0 e5e5 70cf e536  .....{..e...p..6
-000048f0: 9bfb 3ca9 1b66 0e91 2cd4 ba02 85e4 6317  ..<..f..,.....c.
-00004900: 68b0 f07b da2d bf41 b138 eadc 1409 2d3c  h..{.-.A.8....-<
-00004910: 9061 d32e be9a 034e 4e4a 89c7 9058 150b  .a.....NNJ...X..
-00004920: b185 5124 fd18 c37e c4d9 b18e 09a9 903e  ..Q$...~.......>
-00004930: e6d9 4989 7930 c9f9 8b1b d0ac aa6a 6df2  ..I.y0.......jm.
-00004940: 5f07 b42f 4eb5 ef2c e47d 5783 3a3d 5259  _../N..,.}W.:=RY
-00004950: feec 8e7d 1f3c 6ea3 bfce 48f2 cf84 4939  ...}.<n...H...I9
-00004960: 9060 3ea2 4839 c845 edf2 8062 41eb 77f6  .`>.H9.E...bA.w.
-00004970: 9e6b 7d0e 04a6 6dcc cbf3 f609 0000 ffff  .k}...m.........
-00004980: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00004990: dd2c f4a4 c302 0000 d023 0000 2700 0000  .,.......#..'...
-000049a0: 786c 2f70 7269 6e74 6572 5365 7474 696e  xl/printerSettin
-000049b0: 6773 2f70 7269 6e74 6572 5365 7474 696e  gs/printerSettin
-000049c0: 6773 312e 6269 6eec 5acb 6ed3 5010 3dd7  gs1.bin.Z.n.P.=.
-000049d0: 49d5 4024 1012 128f 5529 1b04 029a 36c0  I.@$....U)....6.
-000049e0: 3a44 bc44 5245 6d50 b2a8 1419 2520 4b4d  :D.DREmP....% KM
-000049f0: 8c12 95b4 0b04 1b7e a29f c096 0fe0 23d8  .......~......#.
-00004a00: f201 2d6b 16ec c299 6b3b 0f62 5b81 a46a  ..-k....k;.b[..j
-00004a10: 2077 2c5b f678 ae3d f7cc c377 46de c10e   w,[.x.=...wF...
-00004a20: 1ec3 c52e 3717 5d14 d120 e7d5 10a7 494e  ....7.].. ....IN
-00004a30: 0d0f 5101 b081 dbc8 f0f8 0879 9e65 c951  ..Q........y.e.Q
-00004a40: 49a8 6ff8 b17a fe0b 2c85 3338 4c67 5375  I.o..z..,.38LgSu
-00004a50: 282c a3ca 6b8b c704 a572 5af6 2ed6 b1cf  (,..k....rZ.....
-00004a60: f119 7266 494a 453f ed68 15d8 2e15 aa22  ..rfIJE?.h....."
-00004a70: 22e7 f907 f7d6 9c21 f152 be50 2d4c a08c  "......!.R.P-L..
-00004a80: cc2d 9b3a 4cdf 82b7 2937 f5fd 2cc7 65af  .-.:L...)7..,.e.
-00004a90: 013f 6f02 0d25 773d 6ec0 53a8 735b 469c  .?o..%w=n.S.s[F.
-00004aa0: 7e23 af56 2442 aaf0 ac55 6edb 07d1 3879  ~#.V$B...Un...8y
-00004ab0: 6223 c2eb 9193 a01d f8cc 11e1 8d48 e1c4  b#...........H..
-00004ac0: b8b0 9839 9c92 e3c2 857c 3942 f888 8ef0  ...9.....|9B....
-00004ad0: 9b1a 45bb b567 ef86 c927 c9ec 0b4f e42b  ..E..g...'...O.+
-00004ae0: c104 4f59 3878 bd62 0ccc 07cd 8b1e 7302  ..OY8x.b......s.
-00004af0: 8751 c320 6010 5800 044c de9b a591 e54b  .Q. `.X..L.....K
-00004b00: 2fcf 33a8 9ae4 6110 5874 042c e601 5970  /.3...a.Xt.,..Yp
-00004b10: 7bab 5ce6 8473 c335 4e48 8e08 2981 e232  {.\..s.5NH..)..2
-00004b20: 89dc 4b80 a5a5 1692 6240 328f 3f42 33eb  ..K.....b@2.?B3.
-00004b30: 7807 2479 2abb 56a5 f71e 3896 f245 1f82  x.$y*.V...8..E..
-00004b40: 7c15 58aa 52ac 65d6 32d1 767b 812d 3c61  |.X.R.e.2.v{.-<a
-00004b50: 5dbb 89a8 fa25 dee6 d38e fff7 3d2a 8736  ]....%......=*.6
-00004b60: 1cd8 ec23 fc1d 293c 452f 7468 6079 b1ff  ...#..)<E/th`y..
-00004b70: 60d7 dea7 7dc1 3ba3 c3cc 2189 730e 79af  `...}.;...!.s.y.
-00004b80: 764b cf8f fb6c 4f64 7872 32c6 9f94 eff4  vK...lOdxr2.....
-00004b90: bc5a f267 17c4 4d3f f6a6 9ef5 b496 037a  .Z.g..M?.......z
-00004ba0: e186 9b81 3d2c dd0f 6147 499a 299c babc  ....=,..aGI.)...
-00004bb0: 6950 5b0b 74d2 8599 90c6 b390 920e 55d5  iP[.t.........U.
-00004bc0: 2a25 2e4b 274b 9397 39f4 5560 3a26 19b3  *%.K'K..9.U`:&..
-00004bd0: f039 f9e0 f29d 7e1e c3d8 e864 1030 089c  .9....~....d.0..
-00004be0: 2202 352e 3973 6d27 bc5b eceb 9577 f7da  ".5.9sm'.[...w..
-00004bf0: 4ea3 bdb2 d9e8 866a 5a76 9a8d 8edc 5dd9  N......jZv....].
-00004c00: 729b 766b 4c66 fba0 f9d2 8d59 be54 9cd6  r.vkLf.....Y.T..
-00004c10: eb3a f78e f104 83c0 7f88 c052 fad2 c5ab  .:.........R....
-00004c20: e1f3 9a30 f422 4131 a167 22c6 2010 8380  ...0."A1.g". ...
-00004c30: 5477 c72c 3dae b30a 7178 f196 85cf a793  Tw.,=...qx......
-00004c40: ad68 bdda 59e1 3982 d272 c12d 1454 d6c6  .h..Y.9..r.-.T..
-00004c50: 510d 027f e60b fa67 900f d387 6b07 6fd8  Q......g....k.o.
-00004c60: 3feb ea3f 71ee f39f 993b fcf7 669f fb80  ?..?q....;..f...
-00004c70: fc6e 47bf ebc1 3481 cf5f 3f76 aed8 176e  .nG...4.._?v...n
-00004c80: 88d4 2f00 0000 ffff 0300 504b 0304 1400  ../.......PK....
-00004c90: 0600 0800 0000 2100 b215 5fdf 9b00 0000  ......!..._.....
-00004ca0: ba00 0000 1000 0000 786c 2f63 616c 6343  ........xl/calcC
-00004cb0: 6861 696e 2e78 6d6c 3c8e c10a c230 1044  hain.xml<....0.D
-00004cc0: ef82 ff10 f66e b7f6 2022 4d0b 16fc 02fd  .....n.. "M.....
-00004cd0: 8090 ae4d 20d9 946c 10fd 7b83 8a97 8179  ...M ..l..{....y
-00004ce0: 0333 d38f cf18 d483 b2f8 c41a f64d 0b8a  .3...........M..
-00004cf0: d8a6 d9f3 a2e1 76bd ec8e a0a4 189e 4d48  ......v.......MH
-00004d00: 4c1a 5e24 300e db4d 6f4d b093 339e 556d  L.^$0..MoM..3.Um
-00004d10: 60d1 e04a 594f 8862 1d45 234d 5a89 6b72  `..JYO.b.E#MZ.kr
-00004d20: 4f39 9a52 6d5e 50d6 4c66 1647 5462 c0ae  O9.Rm^P.Lf.GTb..
-00004d30: 6d0f 186b 010c bd55 59c3 b903 e535 540d  m..k...UY....5T.
-00004d40: f509 e00f 4f5f fc01 f85f 1dde 0000 00ff  ....O_..._......
-00004d50: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00004d60: 0084 b45f d295 0100 00ef 0200 0011 0008  ..._............
-00004d70: 0164 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
-00004d80: 6d6c 20a2 0401 28a0 0001 0000 0000 0000  ml ...(.........
+00000cb0: 00bc 96cd 6ac3 300c c7ef 83bd 43f0 7d75  ....j.0.....C.}u
+00000cc0: 9cb6 693b 9af4 b031 e875 eb1e c038 ca07  ..i;...1.u...8..
+00000cd0: 4dec 6079 1f7d fb99 0ed2 058a d643 f0c5  M.`y.}.......C..
+00000ce0: 2019 4b3f fe92 2d6f 77df 5d1b 7d82 c5c6   .K?..-ow.].}...
+00000cf0: e88c 8959 cc22 d0ca 148d ae32 f67e 7879  ...Y.".....2.~xy
+00000d00: 58b3 089d d485 6c8d 868c 9d00 d92e bfbf  X.....l.........
+00000d10: dbbe 422b 9d3f 8475 d363 e4a3 68cc 58ed  ..B+.?.u.c..h.X.
+00000d20: 5cff c839 aa1a 3a89 33d3 83f6 3ba5 b19d  \..9..:.3...;...
+00000d30: 74de b415 efa5 3aca 0a78 12c7 29b7 7f63  t.....:..x..)..c
+00000d40: b07c 1433 da17 19b3 fbc2 e73f 9c7a 9ff9  .|.3.......?.z..
+00000d50: ffd8 a62c 1b05 cf46 7d74 a0dd 9514 fccb  ...,...F}t......
+00000d60: d823 d600 ce07 95b6 0297 b1c1 85fc bcb3  .#..............
+00000d70: 9e79 62c6 afc3 8879 601a 31a7 7042 d390  .yb....y`.1.pB..
+00000d80: 30ab c0d2 acc8 4225 a10b 9590 3893 8aa3  0.....B%....8...
+00000d90: 64ab 9e6a d9e8 4b17 0f2e 8a22 b426 b424  d..j..K....".&.$
+00000da0: e994 15c2 5a5a 28de 9cf5 ef16 5e64 19b9  ....ZZ(.....^d..
+00000db0: c902 856e 170a 6652 656e 78f2 5252 1911  ...n..fRenx.RR..
+00000dc0: 5a1a 41e1 2c03 d32c 496d 26a5 4177 6afd  Z.A.,..,Im&.Awj.
+00000dd0: 741d 26d3 af4d e6f7 d33a e870 1431 85b3  t.&..M...:.p.1..
+00000de0: 084c b3a0 6036 8161 3664 a126 95c6 f9df  .L..`6.a6d.&....
+00000df0: 155c fae4 6cf2 f33a 5c1d 3efa 9ee5 3f00  .\..l..:\.>...?.
+00000e00: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00000e10: 0000 2100 5ead c532 1203 0000 6506 0000  ..!.^..2....e...
+00000e20: 1800 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+00000e30: 732f 7368 6565 7431 2e78 6d6c 9c93 5d6f  s/sheet1.xml..]o
+00000e40: 9b30 1486 ef27 f53f 58be 0f06 9aa4 090a  .0...'.?X.......
+00000e50: a9aa a6d5 7a33 4dfb bc76 cc21 58f1 07b5  ....z3M..v.!X...
+00000e60: 9daf 4dfb ef3b c020 95a2 4951 11d8 c63e  ..M..;. ..IQ...>
+00000e70: 3cef 39f6 cbe2 fea8 15d9 83f3 d29a 9c26  <.9............&
+00000e80: 514c 0918 610b 6936 39fd feed 7934 a3c4  QL..a.i69...y4..
+00000e90: 076e 0aae ac81 9c9e c0d3 fbe5 cd87 c5c1  .n..............
+00000ea0: baad af00 0241 82f1 39ad 42a8 33c6 bca8  .....A..9.B.3...
+00000eb0: 4073 1fd9 1a0c ae94 d669 1ef0 d56d 98af  @s.......i...m..
+00000ec0: 1df0 a2fd 482b 96c6 f194 692e 0ded 0899  ....H+....i.....
+00000ed0: bb86 61cb 520a 5859 b1d3 6042 0771 a078  ..a.R.XY..`B.q.x
+00000ee0: c0fc 7d25 6bdf d3b4 b806 a7b9 dbee ea91  ..}%k...........
+00000ef0: b0ba 46c4 5a2a 194e 2d94 122d b297 8db1  ..F.Z*.N-..-....
+00000f00: 8eaf 15d6 7d4c c65c 90a3 c33b c5e7 b697  ....}L.\...;....
+00000f10: 69e7 2f94 b414 ce7a 5b86 08c9 accb f9b2  i./....z[.......
+00000f20: fc39 9b33 2e06 d265 fd57 6192 3173 b097  .9.3...e.Wa.1s..
+00000f30: cd01 9e51 e9fb 524a 2603 2b3d c36e df09  ...Q..RJ&.+=.n..
+00000f40: 9b0e b066 bb5c b693 454e 7fc7 ffae 11f6  ...f.\..EN......
+00000f50: 49d3 c4e7 a65f fb43 978b 42e2 0937 5511  I...._.C..B..7U.
+00000f60: 0765 4e1f 92ec 29a5 6cb9 68fd f343 c2c1  .eN...).l.h..C..
+00000f70: bf19 935f d6ea af82 2bf8 d418 4ea1 9563  ..._....+...N..c
+00000f80: b472 63d2 b5b5 db26 fc05 c563 e47a 5020  .rc....&...c.zP 
+00000f90: 1abb 108e dd1e 1e41 61f8 ea0e 7dfe da2a  .......Aa...}..*
+00000fa0: e110 65d8 a0f3 76dc 6b3e b7b6 feec 4801  ..e...v.k>....H.
+00000fb0: 25df a9f0 68d5 4f59 842a a7f3 2819 c7d3  %...h.OY.*..(...
+00000fc0: 7442 fba5 2ff6 f011 e4a6 0a98 13ce b686  tB../...........
+00000fd0: c98a d30a bc40 0763 4e11 06a3 a0b0 0ae9  .....@.cN.......
+00000fe0: d812 2d9b 5f11 1dc8 8f39 c5ad 3b74 e459  ..-._....9..;t.Y
+00000ff0: 344e 2777 b364 08ef 0291 d906 2671 3afd  4N'w.d......&q:.
+00001000: 4f2c 6bd9 7f01 0000 ffff 0000 00ff ff94  O,k.............
+00001010: 914d 0ec2 2010 46af 42d8 2b0c 2d9b 8692  .M.. .F.B.+.-...
+00001020: a8f4 2004 69ba 6a4d 2155 6fef 349a f2b3  .. .i.jM!Uo.4...
+00001030: 73c7 f0be 99f0 0615 26ef a3b1 d16a b52e  s.......&....j..
+00001040: 4fb2 f614 2809 0f3b 073c 7592 9217 b4d6  O...(..;.<u.....
+00001050: 75f7 b7f1 c1f9 39f6 949f 85a4 5ab9 3d7b  u.....9.....Z.={
+00001060: c130 5e05 ac37 cd15 dbb4 62ee c7ae 3983  .0^..7....b...9.
+00001070: 92dd 7226 4a66 8abe a684 430e 1363 f8f6  ..r&Jf....C..c..
+00001080: 4340 fc23 80e1 43a0 ad04 7226 2b01 81ca  C@.#..C...r&+...
+00001090: a396 00a7 86a3 f8b8 2f40 40a5 69f2 0950  ......../@@.i..P
+000010a0: 8d1f 0a98 96f0 7561 e963 3e00 0000 ffff  ......ua.c>.....
+000010b0: 0000 00ff ff74 8e41 0a83 400c 45af 32e4  .....t.A..@.E.2.
+000010c0: 0055 a1b6 b538 eebb 6829 7882 9189 1a5a  .U...8..h)x....Z
+000010d0: cd90 8914 7afa 8e82 cb66 f5ff 7ffc 2475  ....z....f....$u
+000010e0: 7003 de9d 0c34 47f3 c65e 2de4 8733 18a1  p....4G..^-..3..
+000010f0: 61dc b572 d8d2 124c c7aa 3ced 6e44 e751  a..r...L..<.nD.Q
+00001100: 5657 16c5 252f f739 5627 303d b3fe 8359  VW..%/.9V'0=...Y
+00001110: 53af 775b d425 98e0 024a 4b5f b450 a51a  S.w[.%...JK_.P..
+00001120: 49d4 6782 8f65 eab6 3e18 16c2 599d 12cf  I.g..e..>...Y...
+00001130: 1602 8b8a 234d 3f5e c95b 909b 2f20 2dcc  ....#M?^.[../ -.
+00001140: 3e2c af38 226a f303 0000 ffff 0300 504b  >,.8"j........PK
+00001150: 0304 1400 0600 0800 0000 2100 9d2b 3105  ..........!..+1.
+00001160: 4b03 0000 a306 0000 1800 0000 786c 2f77  K...........xl/w
+00001170: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
+00001180: 2e78 6d6c 9c93 5d6f 9b30 1486 ef27 ed3f  .xml..]o.0...'.?
+00001190: 58be 0fc6 9464 090a a9b6 46d5 7a33 4deb  X....d....F.z3M.
+000011a0: d65e 3be6 10ac d898 d9ce d7a6 fef7 1da0  .^;.............
+000011b0: a191 a249 512d 30c6 3e7e de73 f0cb fcf6  ...IQ-0.>~.s....
+000011c0: 6034 d981 f3ca d639 e551 4c09 d4d2 16aa  `4.....9.QL.....
+000011d0: 5ee7 f4d7 cffb d194 121f 445d 086d 6bc8  ^.........D].mk.
+000011e0: e911 3cbd 5d7c fc30 df5b b7f1 1540 2048  ..<.]|.0.[...@ H
+000011f0: a87d 4eab 109a 8c31 2f2b 30c2 47b6 811a  .}N....1/+0.G...
+00001200: 574a eb8c 08f8 ead6 cc37 0e44 d16d 329a  WJ.......7.D.m2.
+00001210: 2571 3c61 46a8 9af6 84cc 5dc3 b065 a924  %q<aF.....]..e.$
+00001220: 2cad dc1a a843 0f71 a045 c0fc 7da5 1a7f  ,....C.q.E..}...
+00001230: a219 790d ce08 b7d9 3623 694d 8388 95d2  ..y.....6#iM....
+00001240: 2a1c 3b28 2546 660f ebda 3ab1 d258 f781  *.;(%Ff...:..X..
+00001250: a742 9283 c32b c1fb e624 d3cd 5f28 1925  .B...+...$.._(.%
+00001260: 9df5 b60c 1192 599f f365 f933 3663 420e  ......Y..e.36cB.
+00001270: a4cb faaf c2f0 9439 d8a9 f600 df50 c9fb  .......9.....P..
+00001280: 52e2 e381 95bc c16e de09 9b0c b0f6 73b9  R......n......s.
+00001290: 6cab 8a9c fe8d 5fdb 089f bced e251 ccdb  l....._......Q..
+000012a0: eeac bdd0 c5bc 5078 c26d 55c4 4199 d3cf  ......Px.mU.A...
+000012b0: 3c5b 2694 2de6 9d7f 9e14 ecfd d998 04b1  <[&.-...........
+000012c0: 7a04 0d32 006a 704a fe58 6b1e a5d0 f0ad  z..2.jpJ.Xk.....
+000012d0: 35a0 c6b9 18ad dd9a 7665 eda6 ddfe 8081  5.......ve......
+000012e0: 31ea f86e 5bab 2364 503b b803 8de1 5f30  1..n[.#dP;...._0
+000012f0: 65ff bb53 c621 cab2 41f7 7c7c cae1 beb3  e..S.!..A.||....
+00001300: f977 470a 28c5 5687 3bab 9f55 11aa 9cce  .wG.(.V.;..U....
+00001310: 229e c693 644c 4f4b 3fec fe2b a875 1530  "...dLOK?..+.u.0
+00001320: 279c ed0c 9415 c725 7889 8ec6 9c22 0c46  '......%x....".F
+00001330: 4169 35d2 b127 46b5 bf26 3a52 1c72 8ae7  Ai5..'F..&:R.r..
+00001340: b2ef c9d3 284d c69f a67c 08ef 03d3 d740  ....(M...|.....@
+00001350: 1e27 93ff c4b2 8efd 0f00 00ff ff00 0000  .'..............
+00001360: ffff 9491 4d0e c220 1046 afd2 b052 13cb  ....M.. .F...R..
+00001370: 0cd2 d234 9444 e522 0469 5c55 539a aab7  ...4.D.".i\US...
+00001380: 771a 9bfe ed64 35cc 1b32 ef0b 3ade 43e8  w....d5..2..:.C.
+00001390: aceb 9cd1 ede3 95b4 1543 96c4 a76b 2255  .........C...k"U
+000013a0: a564 c91b a5f3 e5ed 6343 f4a1 e92a 06a9  .d......cC...*..
+000013b0: c898 d17e 983d d330 b522 dd7b 039a f746  ...~.=.0.".{...F
+000013c0: 733f b2cb 9289 35bb 2e19 9ed6 d02e e1cc  s?....5.........
+000013d0: 38f9 4d92 e21f 491a 9e24 e546 5290 7a6d  8.M...I..$.FR.zm
+000013e0: 7690 0214 790e a88e 4329 a452 2adb 1f10  v...y...C).R*...
+000013f0: 8052 d543 ba3c c542 4841 8df1 649b 48cb  .R.C.<.BHA..d.H.
+00001400: 2db8 8176 0571 7af9 cbc4 e74f f802 0000  -..v.qz....O....
+00001410: ffff 0000 00ff ff74 8e4b 0e83 300c 44af  .......t.K..0.D.
+00001420: 12e5 0085 4aa5 1f09 58b1 6d85 c409 0235  ....J...X.m....5
+00001430: 6015 e2c8 31ad c4e9 1b52 b1ac 579e f1d3  `...1....R..W...
+00001440: 8c73 6706 b81b 1ed0 7a35 412f 854e 0f17  .sg.....z5A/.N..
+00001450: ad18 8771 df85 5c74 33ad 5a12 a179 5723  ...q..\t3.Z..yW#
+00001460: 9827 f0a6 b2e3 f19a 66fb 9c6e 67ad 7a22  .'......f..ng.z"
+00001470: f977 4cca 7ceb 6d40 16a7 9c71 c00d ae10  .wL.|.m@...q....
+00001480: 82b4 f29d 997e 5b8f eca5 0ed8 6399 db98  .....~[.....c...
+00001490: a415 3182 1523 48b6 d08e 58d8 a068 b578  ..1..#H...X..h.x
+000014a0: a819 6de8 aba0 37cb 243e 668d 015f 29f0  ..m...7.$>f.._).
+000014b0: 53e5 303a 6f60 c1d0 b0eb 8e1c 4284 c34b  S.0:o`......B..K
+000014c0: c987 f8e5 4700 29bf 0000 00ff ff03 0050  ....G.)........P
+000014d0: 4b03 0414 0006 0008 0000 0021 003f b0ce  K..........!.?..
+000014e0: ff2d 0300 009a 0600 0018 0000 0078 6c2f  .-...........xl/
+000014f0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00001500: 332e 786d 6c9c 935d 6fdb 2014 86ef 27ed  3.xml..]o. ...'.
+00001510: 3f20 ee63 8c9b 6489 15a7 9a9a 55eb cd34  ? .c..d.....U..4
+00001520: eda3 bd26 f838 4601 e301 f9da d4ff be83  ...&.8F.........
+00001530: bdb8 95a2 4951 2d1b 301c 3fef 39f0 7a71  ....IQ-.0.?.9.zq
+00001540: 7b34 9aec c179 659b 82f2 24a5 041a 694b  {4...ye...$...iK
+00001550: d56c 0afa f3c7 fd68 4689 0fa2 2985 b60d  .l.....hF...)...
+00001560: 14f4 049e de2e dfbf 5b1c acdb fa1a 2010  ........[..... .
+00001570: 2434 bea0 7508 6dce 9897 3518 e113 db42  $4..u.m...5....B
+00001580: 832b 9575 4604 7c75 1be6 5b07 a2ec 3e32  .+.uF.|u..[...>2
+00001590: 9a65 693a 6546 a886 f684 dc5d c3b0 55a5  .ei:eF.....]..U.
+000015a0: 24ac acdc 1968 420f 71a0 45c0 fc7d ad5a  $....hB.q.E..}.Z
+000015b0: 7fa6 1979 0dce 08b7 ddb5 2369 4d8b 88b5  ...y......#iM...
+000015c0: d22a 9c3a 2825 46e6 0f9b c63a b1d6 58f7  .*.:(%F....:..X.
+000015d0: 918f 8524 4787 7786 cfcd 59a6 9bbf 5032  ...$G.w...Y...P2
+000015e0: 4a3a eb6d 1512 24b3 3ee7 cbf2 e76c ce84  J:.m..$.>....l..
+000015f0: 1c48 97f5 5f85 e163 e660 afe2 01be a0b2  .H.._..c.`......
+00001600: b7a5 c427 032b 7b81 ddbc 1136 1d60 71bb  ...'.+{....6.`q.
+00001610: 5cbe 5365 41ff a4ff ae11 f63c 36e9 2845  \.SeA......<6.(E
+00001620: 2f74 a3f3 da33 5d2e 4a85 271c ab22 0eaa  /t...3].J.'.."..
+00001630: 827e e4f9 a78c b2e5 a2f3 cfa3 8283 7f35  .~.............5
+00001640: 26bf ad35 dfa5 d0f0 251a 4ea3 9553 b472  &..5....%.N..S.r
+00001650: 34e9 dada 6d0c 7f40 f114 b91e 34c8 6817  4...m..@....4.h.
+00001660: 22b0 dbc3 1d68 0c5f 718e 46ff d549 c531  "....h._q.F..I.1
+00001670: 0ab1 41e9 f5f8 ac7a df19 fbab 2325 5462  ..A....z....#%Tb
+00001680: a7c3 9dd5 4faa 0c75 41e7 091f a7d3 6c42  ....O..uA.....lB
+00001690: cf4b dfec e133 a84d 1d30 2b9c ed2c 9397  .K...3.M.0+..,..
+000016a0: a715 7889 1ec6 ac12 0c46 4169 35d2 b125  ..x......FAi5..%
+000016b0: 46c5 9f11 3d28 8e05 c5cd 3bf4 e459 32ce  F...=(....;..Y2.
+000016c0: 261f 667c 08ef 0391 d905 f234 9bfe 2796  &.f|.......4..'.
+000016d0: 75ec bf00 0000 ffff 0000 00ff ff94 915b  u..............[
+000016e0: 0ec2 2010 45b7 4258 8014 5a34 69a6 242a  .. .E.BX..Z4i.$*
+000016f0: 2e84 2089 5fd5 14d2 dadd 3b3e 5218 fefc  .. ._.....;>R...
+00001700: 03ce 9de4 9e01 e22d 8464 5d72 06a6 fbc2  .......-.d]r....
+00001710: a681 4bce e2c3 8d11 4fbd e6ec 293b e7fb  ..K.....O...);..
+00001720: eb6a 43f4 614c 036f 764a 7303 fe9d 3d62  .jC.aL.ovJs...=b
+00001730: 189f 22de 67d3 8098 0d08 ff63 a792 49ca  ..".g......c..I.
+00001740: ce25 5394 5932 d752 7829 6166 02bb 6f02  .%S.Y2.Rx)af..o.
+00001750: ea1f 010c 6f02 5d25 5032 5d09 a88f b23a  ....o.]%P2]....:
+00001760: 54dd cb11 b9af ba13 98b7 f52d 2ff2 4fbc  T..........-/.O.
+00001770: 0000 00ff ff00 0000 ffff 748e 4b0e 8330  ..........t.K..0
+00001780: 0c44 af12 e500 854a a51f 0958 b16d 85c4  .D.....J...X.m..
+00001790: 0902 3560 15e2 c831 adc4 e91b 52b1 ac57  ..5`...1....R..W
+000017a0: 9ef1 d38c 7367 06b8 1b1e d07a 3541 2f85  ....sg.....z5A/.
+000017b0: 4e0f 17ad 1887 71df 855c 7433 ad5a 12a1  N.....q..\t3.Z..
+000017c0: 7957 2398 27f0 a6b2 e3f1 9a66 fb9c 6e67  yW#.'......f..ng
+000017d0: ad7a 22f9 774c ca7c eb6d 4016 a79c 71c0  .z".wL.|.m@...q.
+000017e0: 0dae 1082 b4f2 9d99 7e5b 8fec a50e d863  ........~[.....c
+000017f0: 99db 98a4 1531 8215 2348 b6d0 8e58 d8a0  .....1..#H...X..
+00001800: 68b5 78a8 196d e8ab a037 cb24 3e66 8d01  h.x..m...7.$>f..
+00001810: 5f29 f053 e530 3a6f 60c1 d0b0 eb8e 1c42  _).S.0:o`......B
+00001820: 84c3 4bc9 87f8 e547 0029 bf00 0000 ffff  ..K....G.)......
+00001830: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00001840: 3444 4cfb 2303 0000 6706 0000 1800 0000  4DL.#...g.......
+00001850: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00001860: 6565 7434 2e78 6d6c 9c93 5d6f 9b30 1486  eet4.xml..]o.0..
+00001870: ef27 ed3f 58be 0f06 42b2 0485 5453 a36a  .'.?X...B...TS.j
+00001880: bd99 a67d f5da 3187 60c5 c6cc 76be 36ed  ...}..1.`...v.6.
+00001890: bff7 181a 1a29 aa14 d502 dbd8 87e7 3d07  .....)........=.
+000018a0: bf2c ee8e 5a91 3d58 274d 53d0 248a 2981  .,..Z.=X'MS.$.).
+000018b0: 4698 5236 9b82 fefa f930 9a51 e23c 6f4a  F.R6.....0.Q.<oJ
+000018c0: ae4c 0305 3d81 a377 cb8f 1f16 0763 b7ae  .L..=..w.....c..
+000018d0: 06f0 0409 8d2b 68ed 7d9b 33e6 440d 9abb  .....+h.}.3.D...
+000018e0: c8b4 d0e0 4e65 ace6 1e1f ed86 b9d6 022f  ....Ne........./
+000018f0: bb97 b462 691c 4f99 e6b2 a13d 21b7 b730  ...bi.O....=!..0
+00001900: 4c55 4901 2b23 761a 1adf 432c 28ee 317f  LUI.+#v...C,(.1.
+00001910: 57cb d69d 695a dc82 d3dc 6e77 ed48 18dd  W...iZ....nw.H..
+00001920: 2262 2d95 f4a7 0e4a 8916 f9e3 a631 96af  "b-....J.....1..
+00001930: 15d6 7d4c 322e c8d1 e295 e23d 3ecb 74eb  ..}L2......=>.t.
+00001940: 574a 5a0a 6b9c a97c 8464 d6e7 7c5d fe9c  WJZ.k..|.d..|]..
+00001950: cd19 1703 e9ba fe9b 3049 c62c ec65 38c0  ........0I.,.e8.
+00001960: 5754 fabe 9492 c9c0 4a5f 61e3 77c2 a603  WT......J_a.w...
+00001970: 2c7c 2e9b ef64 59d0 7ff1 4b1b e198 842e  ,|...dY...K.....
+00001980: 1ec5 e3d0 5db4 ff74 b928 259e 70a8 8a58  ....]..t.(%.p..X
+00001990: a80a fa39 c957 2965 cb45 e79f df12 0eee  ...9.W)e.E......
+000019a0: 624e fe1a a37f 08ae e06b 309c 422b c768  bN.......k0.B+.h
+000019b0: e560 d2b5 31db 10fe 88e2 3172 1d28 10c1  .`..1.....1r.(..
+000019c0: 2e84 e3b0 877b 5018 be0a 3eff d329 e114  .....{P...>..)..
+000019d0: 65d8 a073 393f 6b3e 74b6 fe66 4909 15df  e..s9?k>t..fI...
+000019e0: 297f 6fd4 932c 7d5d d079 9464 f134 9dd0  ).o..,}].y.d.4..
+000019f0: f3d6 7773 f802 7253 7bcc 0957 3bc3 e4e5  ..ws..rS{..W;...
+00001a00: 6905 4ea0 8331 a708 8351 5018 8574 ec89  i.N..1...QP..t..
+00001a10: 96e1 5744 07f2 6341 f11c 0e3d 7916 65e9  ..WD..cA...=y.e.
+00001a20: e4d3 2c19 c2fb c0ec 2530 89d3 e91b b1ac  ..,.....%0......
+00001a30: 633f 0300 00ff ff00 0000 ffff 9490 dd0a  c?..............
+00001a40: c230 0c46 5fa5 e401 d61f 3b85 d116 d4be  .0.F_.....;.....
+00001a50: 48a9 05af a62c 65ea db9b 31e9 bade 7997  H....,e...1...y.
+00001a60: e47c 2187 18bc a794 7dc8 c199 e9f1 6293  .|!.....}.....b.
+00001a70: 0509 0c9f 6144 aa06 0dec 2d75 88c3 ede3  ....aD....-u....
+00001a80: 13c6 3466 0ba2 533d 3813 97ec 99c2 3442  ..4f..S=8.....4B
+00001a90: ea67 270c 9f9d e1f1 c72e 3553 7b76 ad99  .g'.......5S{v..
+00001aa0: 3cec a1af e1c6 38f9 1549 f58f 2485 8ba4  <.....8..I..$...
+00001ab0: 6e24 d5aa de89 be31 5c2e 58a8 57e5 a9f1  n$.....1\.X.W...
+00001ac0: ace1 b1b0 d593 6f8f fd02 0000 ffff 0000  ......o.........
+00001ad0: 00ff ff74 8e4b 0e83 300c 44af 12e5 0085  ...t.K..0.D.....
+00001ae0: 4aa5 1f09 58b1 6d85 c409 0235 6015 e2c8  J...X.m....5`...
+00001af0: 31ad c4e9 1b52 b1ac 579e f1d3 8c73 6706  1....R..W....sg.
+00001b00: b81b 1ed0 7a35 412f 854e 0f17 ad18 8771  ....z5A/.N.....q
+00001b10: df85 5c74 33ad 5a12 a179 5723 9827 f0a6  ..\t3.Z..yW#.'..
+00001b20: b2e3 f19a 66fb 9c6e 67ad 7a22 f977 4cca  ....f..ng.z".wL.
+00001b30: 7ceb 6d40 16a7 9c71 c00d ae10 82b4 f29d  |.m@...q........
+00001b40: 997e 5b8f eca5 0ed8 6399 db98 a415 3182  .~[.....c.....1.
+00001b50: 1523 48b6 d08e 58d8 a068 b578 a819 6de8  .#H...X..h.x..m.
+00001b60: aba0 37cb 243e 668d 015f 29f0 53e5 303a  ..7.$>f.._).S.0:
+00001b70: 6f60 c1d0 b0eb 8e1c 4284 c34b c987 f8e5  o`......B..K....
+00001b80: 4700 29bf 0000 00ff ff03 0050 4b03 0414  G.)........PK...
+00001b90: 0006 0008 0000 0021 0070 d984 8d22 0300  .......!.p..."..
+00001ba0: 0066 0600 0018 0000 0078 6c2f 776f 726b  .f.......xl/work
+00001bb0: 7368 6565 7473 2f73 6865 6574 352e 786d  sheets/sheet5.xm
+00001bc0: 6c9c 935d 6f9b 3014 86ef 27ed 3f58 be0f  l..]o.0...'.?X..
+00001bd0: 064a b204 8554 53a2 6abd 99a6 7df5 da31  .J...TS.j...}..1
+00001be0: 8760 c5c6 cc76 be36 edbf f718 1a1a 29aa  .`...v.6......).
+00001bf0: 14d5 02db d887 e73d 07bf ccef 8f5a 913d  .......=.....Z.=
+00001c00: 5827 4d53 d024 8a29 8146 9852 369b 82fe  X'MS.$.).F.R6...
+00001c10: faf9 309a 52e2 3c6f 4aae 4c03 053d 81a3  ..0.R.<oJ.L..=..
+00001c20: f78b 8f1f e607 63b7 ae06 f004 098d 2b68  ......c.......+h
+00001c30: ed7d 9b33 e644 0d9a bbc8 b4d0 e04e 65ac  .}.3.D.......Ne.
+00001c40: e61e 1fed 86b9 d602 2fbb 97b4 6269 1c4f  ......../...bi.O
+00001c50: 98e6 b2a1 3d21 b7b7 304c 5549 012b 2376  ....=!..0LUI.+#v
+00001c60: 1a1a df43 2c28 ee31 7f57 cbd6 9d69 5adc  ...C,(.1.W...iZ.
+00001c70: 82d3 dc6e 77ed 4818 dd22 622d 95f4 a70e  ...nw.H.."b-....
+00001c80: 4a89 16f9 e3a6 3196 af15 d67d 4c32 2ec8  J.....1....}L2..
+00001c90: d1e2 95e2 7d77 96e9 d6af 94b4 14d6 3853  ....}w........8S
+00001ca0: f908 c9ac cff9 bafc 199b 312e 06d2 75fd  ..........1...u.
+00001cb0: 3761 928c 59d8 cb70 80af a8f4 7d29 25e3  7a..Y..p....})%.
+00001cc0: 8195 bec2 eede 099b 0cb0 f0b9 6cbe 9365  ............l..e
+00001cd0: 41ff c52f 6d84 6312 ba78 1467 a1bb 68ff  A../m.c..x.g..h.
+00001ce0: e962 5e4a 3ce1 5015 b150 15f4 7392 af52  .b^J<.P..P..s..R
+00001cf0: ca16 f3ce 3fbf 251c dcc5 9cfc 3546 ff10  ....?.%.....5F..
+00001d00: 5cc1 d760 3885 568e d1ca c1a4 6b63 b621  \..`8.V.....kc.!
+00001d10: fc11 c563 e43a 5020 825d 08c7 610f 4b50  ...c.:P .]..a.KP
+00001d20: 18be 0c3e ffd3 29e1 1465 d8a0 7339 3f6b  ...>..)..e..s9?k
+00001d30: 3e74 b6fe 6649 0915 df29 bf34 ea49 96be  >t..fI...).4.I..
+00001d40: 2ee8 2c4a b278 928e e979 ebbb 397c 01b9  ..,J.x...y..9|..
+00001d50: a93d e684 ab9d 61f2 f2b4 0227 d0c1 9853  .=....a....'...S
+00001d60: 84c1 2828 8c42 3af6 44cb f02b a203 f9b1  ..((.B:.D..+....
+00001d70: a078 0e87 9e3c 8db2 74fc 699a 0ce1 7d60  .x...<..t.i...}`
+00001d80: f612 98c4 e9e4 8d58 d6b1 9f01 0000 ffff  .......X........
+00001d90: 0000 00ff ff94 9051 0ac3 200c 86af 2239  .......Q.. ..."9
+00001da0: 40ad d66d 5054 e8e6 45c4 097b ea46 23ed  @..mPT..E..{.F#.
+00001db0: 76fb a574 58eb dbde 927c 7fc8 4734 3e62  v..tX....|..G4>b
+00001dc0: 4cce 276f f5f4 5cd8 6440 00c3 971f 91aa  L.'o..\.d@......
+00001dd0: 5e01 7b0b e543 7fff b888 218e c940 dbc8  ^.{..C....!..@..
+00001de0: 1358 1dd6 ec40 611a 21f5 b36d 359f ade6  .X...@a.!..m5...
+00001df0: e1c7 ae25 9347 762b 99e8 8ed0 9570 679c  ...%.Gv+.....pg.
+00001e00: fcb2 a4fc 4792 c259 5255 9272 536f 6ac1  ....G..YRU.rSoj.
+00001e10: f580 8172 535c 2acd 129e 33db 34f9 fed7  ...rS\*...3.4...
+00001e20: 2f00 0000 ffff 0000 00ff ff74 8e4b 0e83  /..........t.K..
+00001e30: 300c 44af 12e5 0085 4aa5 1f09 58b1 6d85  0.D.....J...X.m.
+00001e40: c409 0235 6015 e2c8 31ad c4e9 1b52 b1ac  ...5`...1....R..
+00001e50: 579e f1d3 8c73 6706 b81b 1ed0 7a35 412f  W....sg.....z5A/
+00001e60: 854e 0f17 ad18 8771 df85 5c74 33ad 5a12  .N.....q..\t3.Z.
+00001e70: a179 5723 9827 f0a6 b2e3 f19a 66fb 9c6e  .yW#.'......f..n
+00001e80: 67ad 7a22 f977 4cca 7ceb 6d40 16a7 9c71  g.z".wL.|.m@...q
+00001e90: c00d ae10 82b4 f29d 997e 5b8f eca5 0ed8  .........~[.....
+00001ea0: 6399 db98 a415 3182 1523 48b6 d08e 58d8  c.....1..#H...X.
+00001eb0: a068 b578 a819 6de8 aba0 37cb 243e 668d  .h.x..m...7.$>f.
+00001ec0: 015f 29f0 53e5 303a 6f60 c1d0 b0eb 8e1c  ._).S.0:o`......
+00001ed0: 4284 c34b c987 f8e5 4700 29bf 0000 00ff  B..K....G.).....
+00001ee0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00001ef0: 009b a382 4524 0300 0069 0600 0018 0000  ....E$...i......
+00001f00: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00001f10: 6865 6574 362e 786d 6c9c 93db 8edb 2010  heet6.xml..... .
+00001f20: 86ef 2bf5 1d10 f731 d8eb a489 1567 556d  ..+....1.....gUm
+00001f30: b4ea de54 558f d704 8f63 1430 2e90 53ab  ...TU....c.0..S.
+00001f40: befb 0ece c61b 29aa 142d b201 c3f8 fb67  ......)..-.....g
+00001f50: ccef f9fd c168 b203 e795 6d4b 9a26 9c12  .....h....mK.&..
+00001f60: 68a5 ad54 bb2e e98f ef8f a329 253e 88b6  h..T.......)%>..
+00001f70: 12da b650 d223 787a bf78 ff6e beb7 6ee3  ...P.#xz.x.n..n.
+00001f80: 1b80 4090 d0fa 9236 2174 0563 5e36 6084  ..@....6!t.c^6`.
+00001f90: 4f6c 072d eed4 d619 11f0 d1ad 99ef 1c88  Ol.-............
+00001fa0: aa7f c968 9671 3e61 46a8 969e 0885 bb85  ...h.q>aF.......
+00001fb0: 61eb 5a49 585a b935 d086 13c4 8116 01f3  a.ZIXZ.5........
+00001fc0: f78d eafc 9966 e42d 3823 dc66 db8d a435  .....f.-8#.f...5
+00001fd0: 1d22 564a ab70 eca1 9418 593c ad5b ebc4  ."VJ.p....Y<.[..
+00001fe0: 4a63 dd87 3417 921c 1c5e 19de 7767 997e  Jc..4....^..wg.~
+00001ff0: fd4a c928 e9ac b775 4890 cc4e 395f 973f  .J.(...uH..N9_.?
+00002000: 6333 26e4 40ba aeff 264c 9a33 073b 150f  c3&.@...&L.3.;..
+00002010: f015 95bd 2da5 743c b0b2 57d8 dd1b 6193  ....-.t<..W...a.
+00002020: 0116 3f97 2bb6 aa2a e95f fed2 4638 a6b1  ..?.+..*._..F8..
+00002030: e323 3e8e dd45 fb47 17f3 4ae1 09c7 aa88  .#>..E.G..J.....
+00002040: 83ba a41f d362 9951 b698 f7fe f9a9 60ef  .....b.Q......`.
+00002050: 2fe6 e48f b5e6 9b14 1a3e 47c3 69b4 3247  /........>G.i.2G
+00002060: 2b47 93ae acdd c4f0 2714 e7c8 f5a0 4146  +G......'.....AF
+00002070: bb10 81c3 0e1e 4063 f832 c582 fdef 5e2a  ......@c.2....^*
+00002080: ce51 880d 4a97 f3b3 ea63 6fec 2f8e 5450  .Q..J....co./.TP
+00002090: 8bad 0e0f 56ff 5255 684a 3a4b d29c 4fb2  ....V.RUhJ:K..O.
+000020a0: 313d 6f7d b5fb 4fa0 d64d c0ac 70b5 b74c  1=o}..O..M..p..L
+000020b0: 511d 97e0 257a 18b3 4a30 1805 a5d5 48c7  Q...%z..J0....H.
+000020c0: 9e18 157f 46f4 a038 9414 13db 9fc8 d324  ....F..8.......$
+000020d0: cfc6 1fa6 e910 7e0a cc5f 0253 9e4d fe13  ......~.._.S.M..
+000020e0: cb7a f633 0000 00ff ff00 0000 ffff 9490  .z.3............
+000020f0: dd0a c230 0c46 5fa5 e401 d61f 3b85 d116  ...0.F_.....;...
+00002100: d4be 48a9 05af a62c 65ea db9b 31e9 bade  ..H....,e...1...
+00002110: 7997 e47c 2187 18bc a794 7dc8 c199 e9f1  y..|!.....}.....
+00002120: 6293 0509 0c9f 6144 aa06 0dec 2d75 88c3  b.....aD....-u..
+00002130: ede3 13c6 3466 0ba2 533d 3813 97ec 99c2  ....4f..S=8.....
+00002140: 3442 ea67 270c 9f9d e1f1 c72e 3553 7b76  4B.g'.......5S{v
+00002150: ad99 3cec a1af e1c6 38f9 1549 f58f 2485  ..<.....8..I..$.
+00002160: 8ba4 6e24 d5aa de89 be31 5c2e 58a8 57e5  ..n$.....1\.X.W.
+00002170: a9f1 ace1 b1b0 d593 6f8f fd02 0000 ffff  ........o.......
+00002180: 0000 00ff ff74 8e4b 0e83 300c 44af 12e5  .....t.K..0.D...
+00002190: 0085 4aa5 1f09 58b1 6d85 c409 0235 6015  ..J...X.m....5`.
+000021a0: e2c8 31ad c4e9 1b52 b1ac 579e f1d3 8c73  ..1....R..W....s
+000021b0: 6706 b81b 1ed0 7a35 412f 854e 0f17 ad18  g.....z5A/.N....
+000021c0: 8771 df85 5c74 33ad 5a12 a179 5723 9827  .q..\t3.Z..yW#.'
+000021d0: f0a6 b2e3 f19a 66fb 9c6e 67ad 7a22 f977  ......f..ng.z".w
+000021e0: 4cca 7ceb 6d40 16a7 9c71 c00d ae10 82b4  L.|.m@...q......
+000021f0: f29d 997e 5b8f eca5 0ed8 6399 db98 a415  ...~[.....c.....
+00002200: 3182 1523 48b6 d08e 58d8 a068 b578 a819  1..#H...X..h.x..
+00002210: 6de8 aba0 37cb 243e 668d 015f 29f0 53e5  m...7.$>f.._).S.
+00002220: 303a 6f60 c1d0 b0eb 8e1c 4284 c34b c987  0:o`......B..K..
+00002230: f8e5 4700 29bf 0000 00ff ff03 0050 4b03  ..G.)........PK.
+00002240: 0414 0006 0008 0000 0021 002e 4410 4c23  .........!..D.L#
+00002250: 0300 0067 0600 0018 0000 0078 6c2f 776f  ...g.......xl/wo
+00002260: 726b 7368 6565 7473 2f73 6865 6574 372e  rksheets/sheet7.
+00002270: 786d 6c9c 93db 8e9b 3010 86ef 2bf5 1d2c  xml.....0...+..,
+00002280: df07 1b96 b009 0a59 551b adba 3755 d5e3  .......YU...7U..
+00002290: b563 8660 c5c6 d476 4ead faee 1d60 c346  .c.`...vN....`.F
+000022a0: 8a2a 456b 816d ece1 fb67 f0cf e2e1 6834  .*Ek.m...g....h4
+000022b0: d983 f3ca 3605 8d23 4e09 34d2 96aa d914  ....6..#N.4.....
+000022c0: f4fb b7a7 c98c 121f 4453 0a6d 1b28 e809  ........DS.m.(..
+000022d0: 3c7d 58be 7fb7 3858 b7f5 3540 2048 687c  <}X...8X..5@ Hh|
+000022e0: 41eb 10da 9c31 2f6b 30c2 47b6 8506 772a  A....1/k0.G...w*
+000022f0: eb8c 08f8 e836 ccb7 0e44 d9bf 6434 4b38  .....6...D..d4K8
+00002300: cf98 11aa a103 2177 b730 6c55 2909 2b2b  ......!w.0lU).++
+00002310: 7706 9a30 401c 6811 307f 5fab d69f 6946  w..0@.h.0._...iF
+00002320: de82 33c2 6d77 ed44 5ad3 2262 adb4 0aa7  ..3.mw.DZ."b....
+00002330: 1e4a 8991 f9f3 a6b1 4eac 35d6 7d8c 5321  .J......N.5.}.S!
+00002340: c9d1 e195 e07d 7796 e9d7 af94 8c92 ce7a  .....}w........z
+00002350: 5b85 08c9 6cc8 f9ba fc39 9b33 2147 d275  [...l....9.3!G.u
+00002360: fd37 61e2 9439 d8ab ee00 5f51 c9db 528a  .7a..9...._Q..R.
+00002370: a723 2b79 85dd bd11 968d b0ee 73b9 7ca7  .#+y........s.|.
+00002380: ca82 fee1 2f6d 8263 dc75 7cc2 b3ae bb68  ..../m.c.u|....h
+00002390: 7fe9 7251 2a3c e1ae 2ae2 a02a e887 385f  ..rQ*<..*..*..8_
+000023a0: 2594 2d17 bd7f 7e28 38f8 8b39 f96d adf9  %.-...~(8..9.m..
+000023b0: 2a85 864f 9de1 345a 99a3 953b 93ae addd  *..O..4Z...;....
+000023c0: 76e1 cf28 ce91 eb41 83ec ec42 040e 7b78  v..(...A...B..{x
+000023d0: 048d e1ab 7bf4 f9af 5e09 a728 c346 9dcb  ....{...^..(.F..
+000023e0: f959 f3a9 b7f5 6747 4aa8 c44e 8747 ab7f  .Y....gGJ..N.G..
+000023f0: aa32 d405 9d47 71ca b364 4acf 5b5f ece1  .2...Gq..dJ.[_..
+00002400: 23a8 4d1d 3027 5ced 0d93 97a7 1578 890e  #.M.0'\......x..
+00002410: c69c 220c 4641 6935 d2b1 2746 75bf 223a  ..".FAi5..'Fu.":
+00002420: 501c 0b8a e770 18c8 b328 4da6 f7b3 780c  P....p...(M...x.
+00002430: 1f02 d397 c098 27d9 7f62 59cf fe07 0000  ......'..bY.....
+00002440: ffff 0000 00ff ff94 90dd 0ac2 300c 465f  ............0.F_
+00002450: a5e4 01d6 1f3b 85d1 16d4 be48 a905 afa6  .....;.....H....
+00002460: 2c65 eadb 9b31 e9ba de79 97e4 7c21 8718  ,e...1...y..|!..
+00002470: bca7 947d c8c1 99e9 f162 9305 090c 9f61  ...}.....b.....a
+00002480: 44aa 060d ec2d 7588 c3ed e313 c634 660b  D....-u......4f.
+00002490: a253 3d38 1397 ec99 c234 42ea 6727 0c9f  .S=8.....4B.g'..
+000024a0: 9de1 f1c7 2e35 537b 76ad 993c eca1 afe1  .....5S{v..<....
+000024b0: c638 f915 49f5 8f24 858b a46e 24d5 aade  .8..I..$...n$...
+000024c0: 89be 315c 2e58 a857 e5a9 f1ac e1b1 b0d5  ..1\.X.W........
+000024d0: 936f 8ffd 0200 00ff ff00 0000 ffff 748e  .o............t.
+000024e0: 4b0e 8330 0c44 af12 e500 854a a51f 0958  K..0.D.....J...X
+000024f0: b16d 85c4 0902 3560 15e2 c831 adc4 e91b  .m....5`...1....
+00002500: 52b1 ac57 9ef1 d38c 7367 06b8 1b1e d07a  R..W....sg.....z
+00002510: 3541 2f85 4e0f 17ad 1887 71df 855c 7433  5A/.N.....q..\t3
+00002520: ad5a 12a1 7957 2398 27f0 a6b2 e3f1 9a66  .Z..yW#.'......f
+00002530: fb9c 6e67 ad7a 22f9 774c ca7c eb6d 4016  ..ng.z".wL.|.m@.
+00002540: a79c 71c0 0dae 1082 b4f2 9d99 7e5b 8fec  ..q.........~[..
+00002550: a50e d863 99db 98a4 1531 8215 2348 b6d0  ...c.....1..#H..
+00002560: 8e58 d8a0 68b5 78a8 196d e8ab a037 cb24  .X..h.x..m...7.$
+00002570: 3e66 8d01 5f29 f053 e530 3a6f 60c1 d0b0  >f.._).S.0:o`...
+00002580: eb8e 1c42 84c3 4bc9 87f8 e547 0029 bf00  ...B..K....G.)..
+00002590: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+000025a0: 0000 2100 9e72 8fd1 2303 0000 6806 0000  ..!..r..#...h...
+000025b0: 1800 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+000025c0: 732f 7368 6565 7438 2e78 6d6c 9c93 db8a  s/sheet8.xml....
+000025d0: db30 1086 ef0b 7d07 a1fb 58b6 37c9 2626  .0....}...X.7.&&
+000025e0: ce52 362c dd9b 527a bc56 e471 2ca2 832b  .R6,..Rz.V.q,..+
+000025f0: 29a7 96be 7b47 f6c6 1b08 85b0 c296 64e9  )...{G........d.
+00002600: f737 33d6 efc5 c351 2bb2 07e7 a535 25cd  .73....Q+....5%.
+00002610: 9294 1230 c256 d26c 4afa fddb d368 4689  ...0.V.lJ....hF.
+00002620: 0fdc 545c 5903 253d 81a7 0fcb f7ef 1607  ..T\Y.%=........
+00002630: ebb6 be01 0804 09c6 97b4 09a1 2d18 f3a2  ............-...
+00002640: 01cd 7d62 5b30 b853 5ba7 79c0 47b7 61be  ..}b[0.S[.y.G.a.
+00002650: 75c0 abee 25ad 589e a653 a6b9 34b4 2714  u...%.X..S..4.'.
+00002660: ee16 86ad 6b29 6065 c54e 8309 3dc4 81e2  ....k)`e.N..=...
+00002670: 01f3 f78d 6cfd 99a6 c52d 38cd dd76 d78e  ....l....-8..v..
+00002680: 84d5 2d22 d652 c970 eaa0 9468 513c 6f8c  ..-".R.p...hQ<o.
+00002690: 757c adb0 ee63 36e6 821c 1d5e 39de 77e7  u|...c6....^9.w.
+000026a0: 30dd fa55 242d 85b3 ded6 2141 32eb 73be  0..U$-....!A2.s.
+000026b0: 2e7f cee6 8c8b 8174 5dff 4d98 6ccc 1cec  .......t].M.l...
+000026c0: 653c c057 54fe b694 b2c9 c0ca 5f61 776f  e<.WT......._awo
+000026d0: 844d 0758 fc5c aed8 c9aa a47f d297 36c2  .M.X.\........6.
+000026e0: 318b 5d3a 4aef 6377 d1fe d2e5 a292 78c2  1.]:J.cw......x.
+000026f0: b12a e2a0 2ee9 87ac 58e5 942d 179d 7f7e  .*......X..-...~
+00002700: 4838 f88b 39f9 6dad fe2a b882 4fd1 700a  H8..9.m..*..O.p.
+00002710: ad9c a295 a349 d7d6 6ea3 fc19 83a7 c8f5  .....I..n.......
+00002720: a040 44bb 108e c31e 1e41 a17c 95a1 dcff  .@D......A.|....
+00002730: ea42 c539 0662 43a4 cbf9 39ea 5367 eccf  .B.9.bC...9.Sg..
+00002740: 8e54 50f3 9d0a 8f56 fd94 5568 4a3a 4fb2  .TP....V..UhJ:O.
+00002750: 713a cd27 f4bc f5c5 1e3e 82dc 3401 b3c2  q:.'.....>..4...
+00002760: d5ce 3245 755a 8117 e861 cc2a 4131 0614  ..2EuZ...a.*A1..
+00002770: 5621 1d7b a265 fc19 d183 fc58 523c 8943  V!.{.e.....XR<.C
+00002780: 4f9e 25e3 7c72 3fcb 0679 2f1c bf08 b334  O.%.|r?..y/....4
+00002790: 9ffe 47cb 3af6 3f00 0000 ffff 0000 00ff  ..G.:.?.........
+000027a0: ff94 9051 0ac3 200c 86af 2239 40ad d66d  ...Q.. ..."9@..m
+000027b0: 5054 d8ea 45c4 097b ea46 23dd 76fb a674  PT..E..{.F#.v..t
+000027c0: 58eb dbde 927c 7fc8 4734 3e62 4cce 276f  X....|..G4>bL.'o
+000027d0: f5f4 7cb3 c980 0086 2f3f 2255 bd02 f611  ..|...../?"U....
+000027e0: ca87 fefe 7511 431c 9381 b691 27b0 3aac  ....u.C.....'.:.
+000027f0: d92b 8569 84d4 cfb6 d57c b69a 871f bb95  .+.i.....|......
+00002800: 4c1e d950 32d1 1da1 2be1 ce38 f965 49f9  L..P2...+..8.eI.
+00002810: 8f24 85b3 a4aa 24e5 a6de 540e c37a c040  .$....$...T..z.@
+00002820: b929 2e95 6609 cf99 6d9a 7cff eb02 0000  .)..f...m.|.....
+00002830: ffff 0000 00ff ff74 8e4b 0e83 300c 44af  .......t.K..0.D.
+00002840: 12e5 0085 4aa5 1f09 58b1 6d85 c409 0235  ....J...X.m....5
+00002850: 6015 e2c8 31ad c4e9 1b52 b1ac 579e f1d3  `...1....R..W...
+00002860: 8c73 6706 b81b 1ed0 7a35 412f 854e 0f17  .sg.....z5A/.N..
+00002870: ad18 8771 df85 5c74 33ad 5a12 a179 5723  ...q..\t3.Z..yW#
+00002880: 9827 f0a6 b2e3 f19a 66fb 9c6e 67ad 7a22  .'......f..ng.z"
+00002890: f977 4cca 7ceb 6d40 16a7 9c71 c00d ae10  .wL.|.m@...q....
+000028a0: 82b4 f29d 997e 5b8f eca5 0ed8 6399 db98  .....~[.....c...
+000028b0: a415 3182 1523 48b6 d08e 58d8 a068 b578  ..1..#H...X..h.x
+000028c0: a819 6de8 aba0 37cb 243e 668d 015f 29f0  ..m...7.$>f.._).
+000028d0: 53e5 303a 6f60 c1d0 b0eb 8e1c 4284 c34b  S.0:o`......B..K
+000028e0: c987 f8e5 4700 29bf 0000 00ff ff03 0050  ....G.)........P
+000028f0: 4b03 0414 0006 0008 0000 0021 00d5 5fc3  K..........!.._.
+00002900: 3923 0300 0066 0600 0018 0000 0078 6c2f  9#...f.......xl/
+00002910: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00002920: 392e 786d 6c9c 93db 8edb 2010 86ef 2bf5  9.xml..... ...+.
+00002930: 1d10 f731 c69b a489 1567 556d baea de54  ...1.....gUm...T
+00002940: 558f d704 8f63 1430 2e90 53ab be7b 077b  U....c.0..S..{.{
+00002950: e38d 1455 8a16 d980 61fc fd33 e6f7 e2fe  ...U....a..3....
+00002960: 6834 d983 f3ca 3605 e549 4a09 34d2 96aa  h4....6..IJ.4...
+00002970: d914 f4fb b7c7 d18c 121f 4453 0a6d 1b28  ..........DS.m.(
+00002980: e809 3cbd 5fbe 7db3 3858 b7f5 3540 2048  ..<._.}.8X..5@ H
+00002990: 687c 41eb 10da 9c31 2f6b 30c2 27b6 8506  h|A....1/k0.'...
+000029a0: 772a eb8c 08f8 e836 ccb7 0e44 d9bd 6434  w*.....6...D..d4
+000029b0: cbd2 74ca 8c50 0ded 09b9 bb85 61ab 4a49  ..t..P......a.JI
+000029c0: 5859 b933 d084 1ee2 408b 80f9 fb5a b5fe  XY.3....@....Z..
+000029d0: 4c33 f216 9c11 6ebb 6b47 d29a 1611 6ba5  L3....n.kG....k.
+000029e0: 5538 7550 4a8c cc9f 368d 7562 adb1 ee23  U8uPJ...6.ub...#
+000029f0: 1f0b 498e 0eaf 0cef bbb3 4cb7 7ea5 6494  ..I.......L.~.d.
+00002a00: 74d6 db2a 2448 667d ced7 e5cf d99c 0939  t..*$Hf}.......9
+00002a10: 90ae ebbf 09c3 c7cc c15e c503 7c41 65af  .........^..|Ae.
+00002a20: 4b89 4f06 56f6 02bb 7b25 6c3a c0e2 e772  K.O.V...{%l:...r
+00002a30: f94e 9505 fd93 3eb7 118e 3c76 e928 9dc5  .N....>...<v.(..
+00002a40: eea2 fda5 cb45 a9f0 8463 55c4 4155 d0f7  .....E...cU.AU..
+00002a50: 3c5f 6594 2d17 9d7f 7e28 38f8 8b39 f96d  <_e.-...~(8..9.m
+00002a60: adf9 2a85 864f d170 1aad 9ca2 95a3 49d7  ..*..O.p......I.
+00002a70: d66e 63f8 138a a7c8 f5a0 4146 bb10 81c3  .nc.......AF....
+00002a80: 1e1e 4063 f807 ced1 e8bf 3aa9 3847 2136  ..@c......:.8G!6
+00002a90: 285d cecf aa8f 9db1 3f3b 5242 2576 3a3c  (]......?;RB%v:<
+00002aa0: 58fd 5395 a12e e83c e1e3 749a 4de8 79eb  X.S....<..t.M.y.
+00002ab0: 8b3d 7c04 b5a9 0366 85ab 9d65 f2f2 b402  .=|....f...e....
+00002ac0: 2fd1 c398 5582 c128 28ad 463a f6c4 a8f8  /...U..((.F:....
+00002ad0: 33a2 07c5 b1a0 7812 879e 3c4b c6d9 e4dd  3.....x...<K....
+00002ae0: 8c0f e17d e0f8 3990 a7d9 f43f b1ac 63ff  ...}..9....?..c.
+00002af0: 0300 00ff ff00 0000 ffff 9490 510e c220  ............Q.. 
+00002b00: 0c86 af42 7a00 190c 3559 8064 8e8b 1024  ...Bz...5Y.d...$
+00002b10: f169 9a95 6c7a 7b3b 358c f1e6 5bdb ef6f  .i..lz{;5...[..o
+00002b20: f3a5 1a6f 3126 e793 b77a ba2f 6c32 2080  ...o1&...z./l2 .
+00002b30: e1c3 8f48 55a7 803d 85f2 a1bb be5c c410  ...HU..=.....\..
+00002b40: c764 a039 c823 581d d66c 4f61 1a21 f5b3  .d.9.#X..lOa.!..
+00002b50: 6d34 9fad e6e1 c72e 2593 7b36 944c b47b  m4......%.{6.L.{
+00002b60: e84a b831 4e7e 5952 fe23 49e1 2ca9 2a49  .J.1N~YR.#I.,.*I
+00002b70: f951 af0c 86f5 bc81 724f 9c2b c912 9e32  .Q......rO.+...2
+00002b80: fb4a f2ed ab6f 0000 00ff ff00 0000 ffff  .J...o..........
+00002b90: 748e 4b0e 8330 0c44 af12 e500 854a a51f  t.K..0.D.....J..
+00002ba0: 0958 b16d 85c4 0902 3560 15e2 c831 adc4  .X.m....5`...1..
+00002bb0: e91b 52b1 ac57 9ef1 d38c 7367 06b8 1b1e  ..R..W....sg....
+00002bc0: d07a 3541 2f85 4e0f 17ad 1887 71df 855c  .z5A/.N.....q..\
+00002bd0: 7433 ad5a 12a1 7957 2398 27f0 a6b2 e3f1  t3.Z..yW#.'.....
+00002be0: 9a66 fb9c 6e67 ad7a 22f9 774c ca7c eb6d  .f..ng.z".wL.|.m
+00002bf0: 4016 a79c 71c0 0dae 1082 b4f2 9d99 7e5b  @...q.........~[
+00002c00: 8fec a50e d863 99db 98a4 1531 8215 2348  .....c.....1..#H
+00002c10: b6d0 8e58 d8a0 68b5 78a8 196d e8ab a037  ...X..h.x..m...7
+00002c20: cb24 3e66 8d01 5f29 f053 e530 3a6f 60c1  .$>f.._).S.0:o`.
+00002c30: d0b0 eb8e 1c42 84c3 4bc9 87f8 e547 0029  .....B..K....G.)
+00002c40: bf00 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+00002c50: 0800 0000 2100 a514 31c1 ab03 0000 380a  ....!...1.....8.
+00002c60: 0000 1900 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00002c70: 6574 732f 7368 6565 7431 302e 786d 6c9c  ets/sheet10.xml.
+00002c80: 935d 6f9b 3014 86ef 27ed 3f58 be0f 069a  .]o.0...'.?X....
+00002c90: 4f04 a9aa 76d5 ba8b 69da baed da31 8760  O...v...i....1.`
+00002ca0: c5c6 cc76 be36 edbf ef18 1a52 299a 14d5  ...v.6.....R)...
+00002cb0: 02db d887 e73d c7bc e4b7 07ad c80e ac93  .....=..........
+00002cc0: a629 6812 c594 4023 4c29 9b75 41bf 3f3f  .)h...@#L).uA.??
+00002cd0: 8ee6 9438 cf9b 922b d340 418f e0e8 edf2  ...8...+.@A.....
+00002ce0: fdbb 7c6f ecc6 d500 9e20 a171 05ad bd6f  ..|o..... .q...o
+00002cf0: 33c6 9ca8 4173 1799 161a dca9 8cd5 dce3  3...As..........
+00002d00: a35d 33d7 5ae0 65f7 9256 2c8d e329 d35c  .]3.Z.e..V,..).\
+00002d10: 36b4 2764 f61a 86a9 2a29 e0c1 88ad 86c6  6.'d....*)......
+00002d20: f710 0b8a 7bcc dfd5 b275 279a 16d7 e034  ....{....u'....4
+00002d30: b79b 6d3b 1246 b788 5849 25fd b183 52a2  ..m;.F..XI%...R.
+00002d40: 45f6 b46e 8ce5 2b85 751f 9231 17e4 60f1  E..n..+.u..1..`.
+00002d50: 4af1 be39 c974 eb17 4a5a 0a6b 9ca9 7c84  J..9.t..JZ.k..|.
+00002d60: 64d6 e77c 59fe 822d 1817 03e9 b2fe ab30  d..|Y..-.......0
+00002d70: c998 59d8 c9f0 01cf a8f4 6d29 2593 8195  ..Y.......m)%...
+00002d80: 9e61 376f 844d 0758 382e 9b6d 6559 d03f  .a7o.M.X8..meY.?
+00002d90: f14b 1be1 9884 2e1e c58b d0bd 6a7f e932  .K..........j..2
+00002da0: 2f25 7ee1 5015 b150 15f4 2ec9 3ecc 285b  /%~.P..P....>.([
+00002db0: e69d 7f7e 48d8 bb57 73f2 db18 fd4d 7005  ...~H..Ws....Mp.
+00002dc0: 9f83 e114 5a39 462b 0793 ae8c d984 f027  ....Z9F+.......'
+00002dd0: 148f 91eb 4081 0876 211c 871d dc83 c2f0  ....@..v!.......
+00002de0: bb19 fafc 57af 34cb 3e75 4a6c 905a e6e7  ....W.4.>uJl.Z..
+00002df0: f949 f6b1 73f6 174b 4aa8 f856 f97b a37e  .I..s..KJ..V.{.~
+00002e00: cad2 d705 5d44 c938 9ea6 137a dafa 6af6  ....]D.8...z..j.
+00002e10: 1f41 ae6b 8f69 e16a e799 ac3c 3e80 1368  .A.k.i.j...<>..h
+00002e20: 624c 2bc2 602c 4d18 8574 ec89 96e1 6f44  bL+.`,M..t....oD
+00002e30: 13f2 4341 f1f4 f63d 791e 8dd3 c96c 9e0c  ..CA...=y....l..
+00002e40: e17d 2032 bbc0 244e a7ff 8965 1dfb 1f00  .} 2..$N...e....
+00002e50: 0000 ffff 0000 00ff ff94 d451 6e83 300c  ...........Qn.0.
+00002e60: 06e0 aba0 1c60 9004 4857 a591 36e8 4110  .....`..HW..6.A.
+00002e70: 43da 5337 3588 6db7 9f5b 57c5 38b5 d4bc  C.S75.m..[W.8...
+00002e80: b5fe 7f59 9f11 ad8f 9fd3 34f7 c33c 047f  ...Y......4..<..
+00002e90: fefa 29ce 07a5 5511 bf87 5384 4ffb 4615  ..)...U...S.O.F.
+00002ea0: bfba 1ec6 fdc7 5f3f c571 3acd 0755 bd98  ......_?.q:..U..
+00002eb0: 4605 3f5e ba6f 5086 5184 ef4b a87c b904  F.?^.oP.Q..K.|..
+00002ec0: 5f8e b7ec 9d66 6e9b 7534 33db aca7 99b6  _....fn.u43.....
+00002ed0: dbf0 48c3 352b c17e 3fc0 e41c 00e5 fb01  ..H.5+.~?.......
+00002ee0: 353b c05c cf6a 77ec b00e e7b6 61f3 9eee  5;.\.jw.....a...
+00002ef0: d23b 06a7 e19a 6de0 3607 0e65 116e 11fe  .;....m.6..e.n..
+00002f00: cae1 386f 2a0e a7bb 1238 0d05 789d 0387  ..8o*....8..x...
+00002f10: b208 afaf 70c7 811d ce75 95c8 e9b2 444e  ....p....u....DN
+00002f20: 4341 0e2f f8f3 2f3b 9445 f9e5 27b1 04a7  CA./../;.E..'...
+00002f30: f923 c7b9 49e5 7459 22a7 a120 6f73 e450  .#..I.tY".. os.P
+00002f40: 16e5 2dca 0d97 e3dc a672 ba2c 91d3 5090  ..-......r.,..P.
+00002f50: bb1c 3994 45b9 43b9 e572 9c3f 90d3 6589  ..9.E.C..r.?..e.
+00002f60: 9c86 5c5e ae7f 93ff 0000 00ff ff00 0000  ..\^............
+00002f70: ffff 748e 4b0e 8330 0c44 af12 e500 854a  ..t.K..0.D.....J
+00002f80: a51f 0958 b16d 85c4 0902 3560 15e2 c831  ...X.m....5`...1
+00002f90: adc4 e91b 52b1 ac57 9ef1 d38c 7367 06b8  ....R..W....sg..
+00002fa0: 1b1e d07a 3541 2f85 4e0f 17ad 1887 71df  ...z5A/.N.....q.
+00002fb0: 855c 7433 ad5a 12a1 7957 2398 27f0 a6b2  .\t3.Z..yW#.'...
+00002fc0: e3f1 9a66 fb9c 6e67 ad7a 22f9 774c ca7c  ...f..ng.z".wL.|
+00002fd0: eb6d 4016 a79c 71c0 0dae 1082 b4f2 9d99  .m@...q.........
+00002fe0: 7e5b 8fec a50e d863 99db 98a4 1531 8215  ~[.....c.....1..
+00002ff0: 2348 b6d0 8e58 d8a0 68b5 78a8 196d e8ab  #H...X..h.x..m..
+00003000: a037 cb24 3e66 8d01 5f29 f053 e530 3a6f  .7.$>f.._).S.0:o
+00003010: 60c1 d0b0 eb8e 1c42 84c3 4bc9 87f8 e547  `......B..K....G
+00003020: 0029 bf00 0000 ffff 0300 504b 0304 1400  .)........PK....
+00003030: 0600 0800 0000 2100 4a9a 38ce 9403 0000  ......!.J.8.....
+00003040: 8209 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
+00003050: 6865 6574 732f 7368 6565 7431 312e 786d  heets/sheet11.xm
+00003060: 6c9c 93db 8e9b 3010 86ef 2bf5 1d2c df07  l.....0...+..,..
+00003070: 034b d204 4156 abdd 44dd 9baa eaf1 da31  .K..AV..D......1
+00003080: 43b0 e203 b59d 53ab be7b 07d8 242b a517  C.....S..{..$+..
+00003090: d15a 601b fbe7 9b19 fc53 dc1f b422 3b70  .Z`......S...";p
+000030a0: 5e5a 53d2 248a 2901 236c 25cd baa4 dfbf  ^ZS.$.).#l%.....
+000030b0: 2d47 534a 7ce0 a6e2 ca1a 28e9 113c bd9f  -GSJ|.....(..<..
+000030c0: bf7f 57ec addb f806 2010 2418 5fd2 2684  ..W..... .$._.&.
+000030d0: 3667 cc8b 0634 f791 6dc1 e04e 6d9d e601  6g...4..m..Nm...
+000030e0: 1fdd 9af9 d601 affa 97b4 6269 1c4f 98e6  ..........bi.O..
+000030f0: d2d0 8190 bb5b 18b6 aea5 8027 2bb6 1a4c  .....[.....'+..L
+00003100: 1820 0e14 0f98 bf6f 64eb 4f34 2d6e c169  . .....od.O4-n.i
+00003110: ee36 db76 24ac 6e11 b192 4a86 630f a544  .6.v$.n...J.c..D
+00003120: 8bfc 796d ace3 2b85 751f 928c 0b72 7078  ..ym..+.u....rpx
+00003130: a578 df9d c2f4 eb57 91b4 14ce 7a5b 8708  .x.....W....z[..
+00003140: c96c c8f9 bafc 199b 312e cea4 ebfa 6fc2  .l......1.....o.
+00003150: 2419 73b0 93dd 015e 50e9 db52 4ac6 6756  $.s....^P..RJ.gV
+00003160: 7a81 ddbd 1136 39c3 bacf e5f2 adac 4afa  z....69.......J.
+00003170: 277e 6923 1c93 ae8b 47f1 43d7 bd6a 7fe9  '~i#....G.C..j..
+00003180: bca8 249e 7057 1571 5097 f421 c997 63ca  ..$.pW.qP..!..c.
+00003190: e645 ef9f 1f12 f6fe d59c fcb6 567f 155c  .E..........V..\
+000031a0: c1a7 ce70 0aad 1ca3 953b 93ae acdd 74f2  ...p.....;....t.
+000031b0: 670c 1e23 d783 02d1 d985 701c 76f0 080a  g..#......p.v...
+000031c0: e50b acd7 ffea 232d d27c d147 62e7 50f3  ......#-.|.Gb.P.
+000031d0: e232 3f85 5df6 cefe ec48 0535 dfaa f068  .2?.]....H.5...h
+000031e0: d54f 5985 a6a4 b328 c9e2 493a a6a7 ad2f  .OY....(..I:.../
+000031f0: 76ff 11e4 ba09 9816 aef6 9ec9 abe3 1378  v..............x
+00003200: 8126 c6b4 2214 6369 c22a a463 4fb4 ecfe  .&..".ci.*.cO...
+00003210: 4634 213f 9434 c342 06f2 34ca d2f1 8769  F4!?.4.B..4....i
+00003220: 7296 0fc2 c98b 3089 539c fe57 cb7a f63f  r.....0.S..W.z.?
+00003230: 0000 00ff ff00 0000 ffff 94d4 6d0e 8230  ............m..0
+00003240: 0c06 e0ab 901d 40d8 f88a 642c 5190 7b10  ......@...d,Q.{.
+00003250: 24f1 971a 4650 6f6f c70c 744d 58e4 1ff0  $...FPoo..tMX...
+00003260: b62b cf16 90fa d6f7 63dd 8ead 92c3 e315  .+......c.......
+00003270: 0c25 e32c d0cf f6ae e1aa c858 f0e6 49db  .%.,.......X..I.
+00003280: 15d7 4fdd ebae bf8f 258b 0e22 654a 76a6  ..O.....%.."eJv.
+00003290: f604 c5f0 48c3 fda4 2219 4e4a 86dd 2f3b  ....H...".NJ../;
+000032a0: e32c 77b3 0a67 dccd 6a9c 0937 bb38 7db1  .,w..g..j..7.8}.
+000032b0: 1b36 385c b310 5c0b 4eec c141 f182 4b08  .68\..\.N..A..K.
+000032c0: 4ecc e4ec 48d0 15ee 4909 cc0c 37fb 3b6f  N...H...I...7.;o
+000032d0: d621 a236 1bc7 6828 27db d6e0 d5b3 6575  .!.6..h('.....eu
+000032e0: 4708 fdff 1f1f 1e46 85f1 fc9e 7944 85b8  G......F....yD..
+000032f0: 870a cd70 8fd0 c65e 210e 3784 c91e 2114  ...p...^!.7...!.
+00003300: 6f9e 6162 859c 0a71 0f15 9ae1 1ea1 8dbd  o.ab...q........
+00003310: 42bc fa86 30dd 2384 e24d a1f9 5027 950b  B...0.#..M..P'..
+00003320: 2ac4 3d54 6886 7b84 36f6 0af1 ea54 18ae  *.=Th.{.6....T..
+00003330: 3f9c 2f00 0000 ffff 0000 00ff ff74 8e4b  ?./..........t.K
+00003340: 0e83 300c 44af 12e5 0085 4aa5 1f09 58b1  ..0.D.....J...X.
+00003350: 6d85 c409 0235 6015 e2c8 31ad c4e9 1b52  m....5`...1....R
+00003360: b1ac 579e f1d3 8c73 6706 b81b 1ed0 7a35  ..W....sg.....z5
+00003370: 412f 854e 0f17 ad18 8771 df85 5c74 33ad  A/.N.....q..\t3.
+00003380: 5a12 a179 5723 9827 f0a6 b2e3 f19a 66fb  Z..yW#.'......f.
+00003390: 9c6e 67ad 7a22 f977 4cca 7ceb 6d40 16a7  .ng.z".wL.|.m@..
+000033a0: 9c71 c00d ae10 82b4 f29d 997e 5b8f eca5  .q.........~[...
+000033b0: 0ed8 6399 db98 a415 3182 1523 48b6 d08e  ..c.....1..#H...
+000033c0: 58d8 a068 b578 a819 6de8 aba0 37cb 243e  X..h.x..m...7.$>
+000033d0: 668d 015f 29f0 53e5 303a 6f60 c1d0 b0eb  f.._).S.0:o`....
+000033e0: 8e1c 4284 c34b c987 f8e5 4700 29bf 0000  ..B..K....G.)...
+000033f0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00003400: 0021 0069 5d0d 9269 0300 0028 0800 0019  .!.i]..i...(....
+00003410: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00003420: 2f73 6865 6574 3132 2e78 6d6c 9c93 db8e  /sheet12.xml....
+00003430: 9b30 1086 ef2b f51d 2cdf 0703 4bd2 0441  .0...+..,...K..A
+00003440: 56ed a6ab ee4d 55f5 78ed 9821 58f1 81da  V....MU.x..!X...
+00003450: cea9 55df bd03 3464 a5a8 52b4 16d8 c61e  ..U...4d..R.....
+00003460: be7f c6fc 14f7 47ad c81e 9c97 d694 3489  ......G.......4.
+00003470: 624a c008 5b49 b329 e9b7 af8f 9339 253e  bJ..[I.).....9%>
+00003480: 7053 7165 0d94 f404 9ede 2f5f bf2a 0ed6  pSqe....../_.*..
+00003490: 6d7d 0310 0812 8c2f 6913 429b 33e6 4503  m}...../i.B.3.E.
+000034a0: 9afb c8b6 6070 a7b6 4ef3 808f 6ec3 7ceb  ....`p..N...n.|.
+000034b0: 8057 fd4b 5ab1 348e 674c 7369 e840 c8dd  .W.KZ.4.gLsi.@..
+000034c0: 2d0c 5bd7 52c0 ca8a 9d06 1306 8803 c503  -.[.R...........
+000034d0: e6ef 1bd9 fa33 4d8b 5b70 9abb edae 9d08  .....3M.[p......
+000034e0: ab5b 44ac a592 e1d4 4329 d122 7fda 18eb  .[D.....C)."....
+000034f0: f85a 61dd c724 e382 1c1d 5e29 de77 6799  .Za..$....^).wg.
+00003500: 7efd 4a49 4be1 acb7 7588 90cc 869c afcb  ~.JIK...u.......
+00003510: 5fb0 05e3 6224 5dd7 7f13 26c9 9883 bdec  _...b$]...&.....
+00003520: 3ee0 0595 be2c a564 3ab2 d20b ecee 85b0  >....,.d:.......
+00003530: d908 eb8e cbe5 3b59 95f4 77fc af4d 704c  ......;Y..w..MpL
+00003540: ba2e 9ec4 efba ee59 fb43 9745 25f1 0b77  .......Y.C.E%..w
+00003550: 5511 0775 49df 26f9 fb8c b265 d1fb e7bb  U..uI.&....e....
+00003560: 8483 7f36 27bf acd5 5f04 57f0 b133 9c42  ...6'..._.W..3.B
+00003570: 2bc7 68e5 cea4 6b6b b75d f813 8ac7 c8f5  +.h...kk.]......
+00003580: a040 7476 211c 873d 3c80 c2f0 15d6 eb7f  .@tv!..=<.......
+00003590: f64a ab34 5ff5 4a6c 945a 1697 f959 f6b1  .J.4_.Jl.Z...Y..
+000035a0: 77f6 2747 2aa8 f94e 8507 ab7e c82a 3425  w.'G*..N...~.*4%
+000035b0: 5d44 4916 cfd2 293d 6f7d b687 0f20 374d  ]DI...)=o}... 7M
+000035c0: c0b4 70b5 f74c 5e9d 56e0 059a 18d3 8a30  ..p..L^.V......0
+000035d0: 184b 1356 211d 7ba2 65f7 37a2 09f9 b1a4  .K.V!.{.e.7.....
+000035e0: 787a 8781 3c8f b274 fa66 9e8c e143 2032  xz..<..t.f...C 2
+000035f0: fbc0 244e 67ff 8965 3dfb 2f00 0000 ffff  ..$Ng..e=./.....
+00003600: 0000 00ff ff94 93d1 0a83 2014 865f 257c  .......... .._%|
+00003610: 80f2 98d1 1616 6cd5 8388 1376 d546 46db  ......l....v.FF.
+00003620: de7e 3a47 e981 88ba aaf3 1ffc bf2f 5098  .~:G........./P.
+00003630: bbd6 5327 27d9 88f1 f14a c69a 0049 cc53  ..S''....J...I.S
+00003640: 0ec6 be55 0549 dec0 a5aa 6e9f 4e1b a587  ...U.I....n.N...
+00003650: a926 3465 0569 8472 bb17 bb6c 47c6 7ecf  .&4e.i.r...lG.~.
+00003660: 0d15 d9dc 884c fdb3 6b98 9571 d686 198b  .....L..k..q....
+00003670: b32e cc20 8fc3 3e0c d72c b3ec 8b00 3b22  ... ..>..,....;"
+00003680: 6097 1701 8e04 d84f aba4 48ac f573 8ced  `......O..H..s..
+00003690: 6a6b 129e 07c8 ba0f c3f3 5216 c1e7 47e0  jk........R...G.
+000036a0: edf2 267c eee1 01c3 fb39 a427 f4d7 5df1  ..&|.....9.'..].
+000036b0: 0e7e 58b7 81cf 8fe0 dbe5 4d7c eef1 19c6  .~X.......M|....
+000036c0: f773 4881 460f 201b c7b1 6313 b663 9b6c  .sH.F. ...c..c.l
+000036d0: bd16 5f00 0000 ffff 0000 00ff ff74 8e4b  .._..........t.K
+000036e0: 0e83 300c 44af 12e5 0085 4aa5 1f09 58b1  ..0.D.....J...X.
+000036f0: 6d85 c409 0235 6015 e2c8 31ad c4e9 1b52  m....5`...1....R
+00003700: b1ac 579e f1d3 8c73 6706 b81b 1ed0 7a35  ..W....sg.....z5
+00003710: 412f 854e 0f17 ad18 8771 df85 5c74 33ad  A/.N.....q..\t3.
+00003720: 5a12 a179 5723 9827 f0a6 b2e3 f19a 66fb  Z..yW#.'......f.
+00003730: 9c6e 67ad 7a22 f977 4cca 7ceb 6d40 16a7  .ng.z".wL.|.m@..
+00003740: 9c71 c00d ae10 82b4 f29d 997e 5b8f eca5  .q.........~[...
+00003750: 0ed8 6399 db98 a415 3182 1523 48b6 d08e  ..c.....1..#H...
+00003760: 58d8 a068 b578 a819 6de8 aba0 37cb 243e  X..h.x..m...7.$>
+00003770: 668d 015f 29f0 53e5 303a 6f60 c1d0 b0eb  f.._).S.0:o`....
+00003780: 8e1c 4284 c34b c987 f8e5 4700 29bf 0000  ..B..K....G.)...
+00003790: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+000037a0: 0021 00cf 3ada 9c7f 0300 00f5 0700 0019  .!..:...........
+000037b0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+000037c0: 2f73 6865 6574 3133 2e78 6d6c 9c93 cb6e  /sheet13.xml...n
+000037d0: e320 1486 f723 cd3b 20f6 31c6 4da2 c68a  . ...#.; .1.M...
+000037e0: 538d d256 d3cd a89a eb9a e0e3 1885 8b0b  S..V............
+000037f0: e4d6 d1bc 7b0f ce24 8d94 4d54 6403 e6f2  ....{..$..MTd...
+00003800: fde7 c0ef e9dd ce68 b201 1f94 b315 e559  .......h.......Y
+00003810: 4e09 58e9 6a65 9715 fdf5 f371 704b 4988  N.X.je.....qpKI.
+00003820: c2d6 423b 0b15 dd43 a077 b3cf 9fa6 5be7  ..B;...C.w....[.
+00003830: 57a1 0588 0409 3654 b48d b12b 190b b205  W.....6T...+....
+00003840: 2342 e63a b038 d338 6f44 c44f bf64 a1f3  #B.:.8.8oD.O.d..
+00003850: 20ea 7e93 d1ac c8f3 3133 4259 7a20 94fe   .~.....13BYz ..
+00003860: 1a86 6b1a 25e1 dec9 b501 1b0f 100f 5a44  ..k.%.........ZD
+00003870: 8c3f b4aa 0b47 9a91 d7e0 8cf0 ab75 3790  .?...G.......u7.
+00003880: ce74 8858 28ad e2be 8752 6264 f9b4 b4ce  .t.X(....Rbd....
+00003890: 8b85 c6bc 777c 2824 d979 7c0a 7c6f 8e32  ....w|($.y|.|o.2
+000038a0: fdf8 8592 51d2 bbe0 9a98 2199 1d62 be4c  ....Q.....!..b.L
+000038b0: 7fc2 264c c813 e932 ffab 307c c83c 6c54  ..&L...2..0|.<lT
+000038c0: bac0 7754 f1b1 90f8 e8c4 2ade 6137 1f84  ..wT......*.a7..
+000038d0: 8d4f b074 5cbe 5cab baa2 7ff3 ff65 802d  .O.t\.\......e.-
+000038e0: 4f55 3ec8 e7a9 3a2b ffe8 6c5a 2bbc e194  OU>...:+..lZ+...
+000038f0: 15f1 d054 f40b 2f1f 8694 cda6 bd7f 7e2b  ...T../.......~+
+00003900: d886 b33e 7975 cefc 9042 c3b7 6438 8d56  ...>yu...B..d8.V
+00003910: ced1 cac9 a40b e756 69f9 138a e7c8 0da0  .......Vi.......
+00003920: 4126 bb10 81cd 06e6 a071 f99c 638c e1a5  A&.......q..c...
+00003930: 974a 7d14 6227 a5f3 fe51 f5b1 37f6 b327  .J}.b'...Q..7..'
+00003940: 3534 62ad e3dc e93f aa8e 6d45 2719 1fe6  54b....?..mE'...
+00003950: e362 448f 53df ddf6 2ba8 651b 312a 1ced  .bD.S...+.e.1*..
+00003960: 2d53 d6fb 7b08 123d 8c51 65b8 1805 a5d3  -S..{..=.Qe.....
+00003970: 48c7 9a18 957e 46f4 a0d8 a54c 126b 7b80  H....~F....L.k{.
+00003980: 739e 15b7 233e 4afc 1463 bfe7 0d00 00ff  s...#>J..c......
+00003990: ff00 0000 ffff 9492 ed0a c220 1846 6f65  ........... .Foe
+000039a0: 7801 f931 6534 9c50 e985 8809 fd5a 3165  x..1e4.P.....Z1e
+000039b0: d5dd 6719 4e85 02ff a9e7 f5e1 3922 7717  ..g.N.......9"w.
+000039c0: 6bbd d45e 0bbe 5cef dd32 010c 3a77 d3b3  k..^..\..2..:w..
+000039d0: 0bab 9181 ee81 a936 e3f9 29ad 3376 f613  .......6..).3v..
+000039e0: 403b c280 e0e6 3d7b 08c3 e1c8 85fd 2a10  @;....={......*.
+000039f0: 87ab e0d0 7cd9 3167 b864 a782 ed4b 2873  ....|.1g.d...K(s
+00003a00: 48aa 5495 c321 5d84 a17c 3220 2d06 6138  H.T..!]..|2 -.a8
+00003a10: 19d0 ca20 67ac 32f8 c364 ce48 a5ae c8e7  ... g.2..d.H....
+00003a20: b106 b489 15e5 fb86 f2aa 8f59 f847 166d  ...........Y.G.m
+00003a30: c9a2 312b 7bf0 d80b 6e5f e405 0000 ffff  ..1+{...n_......
+00003a40: 0000 00ff ff94 8fcb 4ec3 3010 457f c5f2  ........N.0.E...
+00003a50: 8215 6ada 0a94 2292 4888 0ab1 a18a 5a7e  ..j...".H.....Z~
+00003a60: c06d 26c9 0827 638d 2754 ead7 e3b8 9487  .m&..'c.'T......
+00003a70: 4416 78e1 d7bd 73e6 4ee6 4c03 2f86 1bec  D.x...s.N.L./...
+00003a80: bdb2 504b aee7 b374 95de dcfd 582b ad18  ..PK...t....X+..
+00003a90: 9b76 4a13 72b9 5ecc e6b7 cbf4 6b85 923d  .vJ.r.^.....k..=
+00003aa0: 8950 f797 d282 a980 273a d544 3225 2645  .P......':.D2%&E
+00003ab0: 36e6 dd81 0c4e 39e3 8077 7882 00d2 ca1f  6....N9..wx.....
+00003ac0: 8c3d df6a 642f 65b0 6d86 6e1f 495a 1123  .=.jd/e.m.n.IZ.#
+00003ad0: f462 04a9 cfb5 2316 3628 5a0d 1e4a c63e  .b....#.6(Z..J.>
+00003ae0: f45b 436d 062b 3eb2 da60 3f51 f0db b5c3  .[Cm.+>..`?Q....
+00003af0: f8f3 0e2c 183a 5cde 0772 08d1 1c22 9dc7  ...,.:\..r..."..
+00003b00: 798a b98b 8caa ea39 ce57 5c99 cedd 3fc6  y......9.W\...?.
+00003b10: 5dbf 6207 5e6d e0a8 b6d4 99fe 7a0b cd60  ].b.^m......z..`
+00003b20: 0deb a82e 96f1 78c8 92ef e291 f389 fc07  ......x.........
+00003b30: 671c 5b45 7f19 6197 50c9 ef8c c991 f8cd  g.[E..a.P.......
+00003b40: b700 527c 0000 00ff ff03 0050 4b03 0414  ..R|.......PK...
+00003b50: 0006 0008 0000 0021 00c1 1710 be4e 0700  .......!.....N..
+00003b60: 00c6 2000 0013 0000 0078 6c2f 7468 656d  .. ......xl/them
+00003b70: 652f 7468 656d 6531 2e78 6d6c ec59 cd8b  e/theme1.xml.Y..
+00003b80: 1b37 14bf 17fa 3f0c 7377 fc35 e38f 25de  .7....?.sw.5..%.
+00003b90: e0cf 6c93 dd24 649d 941c b5b6 ec51 5633  ..l..$d......QV3
+00003ba0: 3292 bc1b 1302 2539 f552 28a4 a597 426f  2.....%9.R(...Bo
+00003bb0: 3d94 d240 030d bdf4 8f09 24b4 e91f d127  =..@......$....'
+00003bc0: cdd8 23ad e524 9b6c 4a5a 760d 8b47 febd  ..#..$.lJZv..G..
+00003bd0: a7a7 f79e 7e7a f374 f1d2 bd98 7a47 980b  ....~z.t....zG..
+00003be0: c292 965f be50 f23d 9c8c d898 24d3 967f  ..._.P.=....$...
+00003bf0: 6b38 2834 7c4f 4894 8c11 6509 6ef9 0b2c  k8(4|OH...e.n..,
+00003c00: fc4b db9f 7e72 116d c908 c7d8 03f9 446c  .K..~r.m......Dl
+00003c10: a196 1f49 39db 2a16 c508 8691 b8c0 6638  ...I9.*.......f8
+00003c20: 81df 268c c748 c223 9f16 c71c 1d83 de98  ..&..H.#........
+00003c30: 162b a552 ad18 2392 f85e 8262 507b 7d32  .+.R..#..^.bP{}2
+00003c40: 2123 ec0d 954a 7f7b a9bc 4fe1 3191 420d  !#...J.{..O.1.B.
+00003c50: 8c28 df57 aab1 25a1 b1e3 c3b2 4288 85e8  .(.W..%.....B...
+00003c60: 52ee 1d21 daf2 619e 313b 1ee2 7bd2 f728  R..!..a.1;..{..(
+00003c70: 1212 7e68 f925 fde7 17b7 2f16 d156 2644  ..~h.%..../..V&D
+00003c80: e506 5943 6ea0 ff32 b94c 607c 58d1 73f2  ..YCn..2.L`|X.s.
+00003c90: e9c1 6ad2 2008 835a 7ba5 5f03 a85c c7f5  ..j. ..Z{._..\..
+00003ca0: ebfd 5abf b6d2 a701 6834 8295 a6b6 d83a  ..Z.....h4.....:
+00003cb0: eb95 6e90 610d 50fa d5a1 bb57 ef55 cb16  ..n.a.P....W.U..
+00003cc0: ded0 5f5d b3b9 1daa 8f85 d7a0 547f b086  .._]........T...
+00003cd0: 1f0c bae0 450b af41 293e 5cc3 879d 66a7  ....E..A)>\...f.
+00003ce0: 67eb d7a0 145f 5bc3 d74b ed5e 50b7 f46b  g...._[..K.^P..k
+00003cf0: 5044 4972 b886 2e85 b56a 77b9 da15 64c2  PDIr.....jw...d.
+00003d00: e88e 13de 0c83 41bd 9229 cf51 900d abec  ......A..).Q....
+00003d10: 5253 4c58 2237 e55a 8cee 323e 0080 0252  RSLX"7.Z..2>...R
+00003d20: 2449 e2c9 c50c 4fd0 08b2 b88b 2839 e0c4  $I....O.....(9..
+00003d30: db25 d308 126f 8612 2660 b854 290d 4a55  .%...o..&`.T).JU
+00003d40: f8af 3e81 fea6 238a b630 32a4 955d 6089  ..>...#..02..]`.
+00003d50: 581b 52f6 7862 c4c9 4cb6 fc2b a0d5 3720  X.R.xb..L..+..7 
+00003d60: 2f9e 3d7b fef0 e9f3 87bf 3d7f f4e8 f9c3  /.={......=.....
+00003d70: 5fb2 b9b5 2a4b 6e07 2553 53ee d58f 5fff  _...*Kn.%SS..._.
+00003d80: fdfd 17de 5fbf fef0 eaf1 37e9 d427 f1c2  ...._.....7..'..
+00003d90: c4bf fcf9 cb97 bfff f13a f5b0 e2dc 152f  .........:...../
+00003da0: be7d f2f2 e993 17df 7df5 e74f 8f1d dadb  .}......}..O....
+00003db0: 1c1d 98f0 2189 b1f0 aee1 63ef 268b 6181  ....!.....c.&.a.
+00003dc0: 0efb f101 3f9d c430 42c4 9240 11e8 76a8  ....?..0B..@..v.
+00003dd0: eecb c802 5e5b 20ea c275 b0ed c2db 1c58  ....^[ ..u.....X
+00003de0: c605 bc3c bf6b d9ba 1ff1 b924 8e99 af46  ...<.k.....$...F
+00003df0: b105 dc63 8c76 1877 3ae0 aa9a cbf0 f070  ...c.v.w:......p
+00003e00: 9e4c dd93 f3b9 89bb 89d0 916b ee2e 4aac  .L.........k..J.
+00003e10: 00f7 e733 a057 e252 d98d b065 e60d 8a12  ...3.W.R...e....
+00003e20: 89a6 38c1 d253 bfb1 438c 1dab bb43 88e5  ..8..S..C....C..
+00003e30: d73d 32e2 4cb0 89f4 ee10 af83 88d3 2543  .=2.L.........%C
+00003e40: 7260 2552 2eb4 4362 88cb c265 2084 daf2  r`%R..Cb...e ...
+00003e50: cdde 6daf c3a8 6bd5 3d7c 6423 615b 20ea  ..m...k.=|d#a[ .
+00003e60: 307e 88a9 e5c6 cb68 2e51 ec52 3944 3135  0~.....h.Q.R9D15
+00003e70: 1dbe 8b64 e432 727f c147 26ae 2f24 447a  ...d.2r..G&./$Dz
+00003e80: 8a29 f3fa 632c 844b e63a 87f5 1a41 bf0a  .)..c,.K.:...A..
+00003e90: 0ce3 0efb 1e5d c436 924b 72e8 d2b9 8b18  .....].6.Kr.....
+00003ea0: 3391 3d76 d88d 503c 73da 4c92 c8c4 7e26  3.=v..P<s.L...~&
+00003eb0: 0e21 4591 7783 4917 7c8f d93b 443d 431c  .!E.w.I.|..;D=C.
+00003ec0: 50b2 31dc b709 b6c2 fd66 22b8 05e4 6a9a  P.1......f"...j.
+00003ed0: 9427 88fa 65ce 1db1 bc8c 99bd 1f17 7482  .'..e.........t.
+00003ee0: b08b 65da 3cb6 d8b5 cd89 333b 3af3 a995  ..e.<.....3;:...
+00003ef0: dabb 1853 748c c618 7bb7 3e73 58d0 6133  ...St...{.>sX.a3
+00003f00: cbe7 b9d1 5722 6095 1dec 4aac 2bc8 ce55  ....W"`...J.+..U
+00003f10: f59c 6001 6592 aa6b d629 7297 082b 65f7  ..`.e..k.)r..+e.
+00003f20: f194 6db0 676f 7182 7816 2889 11df a4f9  ..m.goq.x.(.....
+00003f30: 1a44 dd4a 5d38 e59c 547a 9d8e 0e4d e035  .D.J]8..Tz...M.5
+00003f40: 02e5 1fe4 8bd3 29d7 05e8 3092 bbbf 49eb  ......)...0...I.
+00003f50: 8d08 5967 977a 16ee 7c5d 702b 7e6f b3c7  ..Yg.z..|]p+~o..
+00003f60: 605f de3d edbe 0419 7c6a 1920 f6b7 f6cd  `_.=....|j. ....
+00003f70: 1051 6b82 3c61 8608 0a0c 17dd 8288 15fe  .Qk.<a..........
+00003f80: 5c44 9dab 5a6c ee94 9bd8 9b36 0f03 1446  \D..Zl.....6...F
+00003f90: 56bd 1393 e48d c5cf 89b2 27fc 77ca 1e77  V.........'.w..w
+00003fa0: 0173 0605 8f5b f1fb 943a 9b28 65e7 4481  .s...[...:.(e.D.
+00003fb0: b309 f71f 2c6b 7a68 9edc c070 92ac 73d6  ....,kzh...p..s.
+00003fc0: 7955 735e d5f8 fffb aa66 d35e 3eaf 65ce  yUs^.....f.^>.e.
+00003fd0: 6b99 f35a c6f5 f6f5 416a 99bc 7c81 ca26  k..Z....Aj..|..&
+00003fe0: eff2 e89e 4fbc b1e5 3321 94ee cb05 c5bb  ....O...3!......
+00003ff0: 4277 7d04 bcd1 8c07 30a8 db51 ba27 b96a  Bw}.....0..Q.'.j
+00004000: 01ce 22f8 9a35 982c dc94 232d e371 263f  .."..5.,..#-.q&?
+00004010: 2732 da8f d00c 5a43 65dd c09c 8a4c f554  '2....ZCe....L.T
+00004020: 7833 26a0 63a4 8775 2b15 9fd0 adfb 4ef3  x3&.c..u+.....N.
+00004030: 788f 8dd3 4e67 b9ac ba9a a90b 0592 f978  x...Ng.........x
+00004040: 295c 8d43 974a a6e8 5a3d efde add4 eb7e  )\.C.J..Z=.....~
+00004050: e854 7759 9706 28d9 d318 614c 661b 5175  .TwY..(...aLf.Qu
+00004060: 1851 5f0e 4214 5e67 845e d999 58d1 7458  .Q_.B.^g.^..X.tX
+00004070: d150 ea97 a15a 4671 e50a 306d 1515 78e5  .P...ZFq..0m..x.
+00004080: f6e0 45bd e587 41da 4186 661c 94e7 6315  ..E...A.A.f...c.
+00004090: a7b4 99bc 8cae 0ace 9946 7a93 33a9 9901  .........Fz.3...
+000040a0: 5062 2f33 208f 7453 d9ba 7179 6a75 69aa  Pb/3 .tS..qyjui.
+000040b0: bd45 a42d 238c 74b3 8d30 d230 8217 e12c  .E.-#.t..0.0...,
+000040c0: 3bcd 96fb 59c6 ba99 87d4 324f b962 b91b  ;...Y.....2O.b..
+000040d0: 7233 ea8d 0f11 6b45 2227 b881 2626 53d0  r3....kE"'..&&S.
+000040e0: c43b 6ef9 b56a 08b7 2a23 346b f913 e818  .;n..j..*#4k....
+000040f0: c3d7 7806 b923 d45b 17a2 53b8 7619 499e  ..x..#.[..S.v.I.
+00004100: 6ef8 7761 9619 17b2 8744 943a 5c93 4eca  n.wa.....D.:\.N.
+00004110: 0631 9198 7b94 c42d 5f2d 7f95 0d34 d11c  .1..{..-_-...4..
+00004120: a26d 2b57 8010 3e5a e39a 402b 1f9b 7110  .m+W..>Z..@+..q.
+00004130: 743b c878 32c1 2369 86dd 1851 9e4e 1f81  t;.x2.#i...Q.N..
+00004140: e153 ae70 feaa c5df 1dac 24d9 1cc2 bd1f  .S.p......$.....
+00004150: 8d8f bd03 3ae7 3711 a458 582f 2b07 8e89  ....:.7..XX/+...
+00004160: 808b 8372 eacd 3181 9bb0 1591 e5f9 77e2  ...r..1.......w.
+00004170: 60ca 68d7 bc8a d239 948e 233a 8b50 76a2  `.h....9..#:.Pv.
+00004180: 9864 9ec2 3589 aecc d14f 2b1f 184f d99a  .d..5....O+..O..
+00004190: c1a1 eb2e 3c98 aa03 f6bd 4fdd 371f d5ca  ....<.....O.7...
+000041a0: 7306 69e6 67a6 c52a ead4 7493 e987 3be4  s.i.g..*..t...;.
+000041b0: 0dab f243 d4b2 2aa5 6efd 4e2d 72ae 6b2e  ...C..*.n.N-r.k.
+000041c0: b90e 12d5 794a bce1 d47d 8b03 c130 2d9f  ....yJ...}...0-.
+000041d0: cc32 4d59 bc4e c38a b3b3 51db b433 2c08  .2MY.N....Q..3,.
+000041e0: 0c4f d436 f86d 7546 383d f1ae 273f c89d  .O.6.muF8=..'?..
+000041f0: cc5a 7540 2ceb 4a9d f8fa cadc bcd5 6607  .Zu@,.J.......f.
+00004200: 7781 3c7a 707f 38a7 52e8 5042 6f97 2328  w.<zp.8.R.PBo.#(
+00004210: fad2 1bc8 9436 608b dc93 598d 08df bc39  .....6`...Y....9
+00004220: 272d ff7e 296c 07dd 4ad8 2d94 1a61 bf10  '-.~)l..J.-..a..
+00004230: 5483 52a1 11b6 ab85 7618 56cb fdb0 5cea  T.R.....v.V...\.
+00004240: 752a 0fe0 6091 515c 0ed3 ebfa 015c 61d0  u*..`.Q\.....\a.
+00004250: 4576 69af c7d7 2eee e3e5 2dcd 8511 8b8b  Evi.......-.....
+00004260: 4c5f cc17 b5e1 fae2 be5c d97c 71ef 1120  L_.......\.|q.. 
+00004270: 9dfb b5ca a059 6d76 6a85 66b5 3d28 04bd  .....Ymvj.f.=(..
+00004280: 4ea3 d0ec d63a 855e ad5b ef0d 7add b0d1  N....:.^.[..z...
+00004290: 1c3c f0bd 230d 0eda d56e 50eb 370a b572  .<..#....nP.7..r
+000042a0: b75b 086a 2565 7ea3 59a8 0795 4a3b a8b7  .[.j%e~.Y...J;..
+000042b0: 1bfd a0fd 202b 6360 e529 7d64 be00 f76a  .... +c`.)}d...j
+000042c0: bbb6 ff01 0000 ffff 0300 504b 0304 1400  ..........PK....
+000042d0: 0600 0800 0000 2100 b1db eb05 df02 0000  ......!.........
+000042e0: 5c07 0000 0d00 0000 786c 2f73 7479 6c65  \.......xl/style
+000042f0: 732e 786d 6ca4 555b 6f9b 3014 7e9f b4ff  s.xml.U[o.0.~...
+00004300: 60f9 9d72 69c8 9208 a896 a648 95b6 aa52  `..ri......H...R
+00004310: 3b69 af06 4c62 d517 664c 4636 edbf ef18  ;i..Lb..fLF6....
+00004320: 1242 d66e eb25 0ff1 f1b1 fdf9 3be7 3b3e  .B.n.%......;.;>
+00004330: 4417 ade0 684b 75cd 948c b17f e661 4465  D...hKu......aDe
+00004340: ae0a 26d7 31fe 729f 3a33 8c6a 4364 41b8  ..&.1.r.:3.jCdA.
+00004350: 9234 c63b 5ae3 8be4 fdbb a836 3b4e ef36  .4.;Z......6;N.6
+00004360: 941a 0410 b28e f1c6 986a e1ba 75be a182  .........j..u...
+00004370: d467 aaa2 1256 4aa5 0531 30d5 6bb7 ae34  .g...VJ..10.k..4
+00004380: 2545 6d0f 09ee 069e 3775 0561 12f7 080b  %Em.....7u.a....
+00004390: 913f 0744 10fd d054 4eae 4445 0ccb 1867  .?.D...TN.DE...g
+000043a0: 66d7 6161 24f2 c5f5 5a2a 4d32 0e54 5b7f  f.aa$...Z*M2.T[.
+000043b0: 4272 d4fa 531d a056 1f2e e9bc 8fee 112c  Br..S..V.......,
+000043c0: d7aa 56a5 3903 5c57 9525 cbe9 63ba 7377  ..V.9.\W.%..c.sw
+000043d0: ee92 fc88 04c8 af43 f243 d70b 4e62 6ff5  .......C.C..Nbo.
+000043e0: 2b91 26ae a65b 66e5 c349 542a 696a 94ab  +.&..[f..IT*ij..
+000043f0: 461a 1013 88da 142c 1ea4 fa2e 53bb 649d  F......,....S.d.
+00004400: fdae 24aa 7fa0 2de1 e0f1 b19b 44b9 e24a  ..$...-.....D..J
+00004410: 23bd ce62 9ca6 5ef7 b36e 4904 edb7 5d12  #..b..^..nI...].
+00004420: ce32 cdac b324 82f1 5def 0eba c31b a26b  .2...$..]......k
+00004430: 2884 1ecf 7a5c cb64 3fd4 7082 713e f00a  (...z\.d?.p.q>..
+00004440: 2c05 7024 1108 68a8 9629 4cd0 debe df55  ,.p$..h..)L....U
+00004450: 209d 845a eb61 ba7d ffd9 bdd6 64e7 07e1   ..Z.a.}....d...
+00004460: e880 db5d 9844 99d2 05d4 f631 2307 5712  ...].D.....1#.W.
+00004470: 715a 1a20 aad9 7a63 47a3 2af8 cf94 31a0  qZ. ..zcG.*...1.
+00004480: 7f12 158c ac95 24dc 86d2 830c 0684 9353  ......$........S
+00004490: ceef 6cfd 7f2d 4fb0 db12 c946 a4c2 5c17  ..l..-O....F..\.
+000044a0: 3186 9764 9370 3021 90bd d9e3 f513 8b3f  1..d.p0!.......?
+000044b0: 46eb b147 b013 48d6 cb61 515b 0ef8 27a7  F..G..H..aQ[..'.
+000044c0: 41ec 67b0 1a8e 2352 557c 77d3 888c eab4  A.g...#RU|w.....
+000044d0: 7bc8 b682 80f4 1b28 a16f 8d32 f456 d392  {......(.o.2.V..
+000044e0: b54f a1bd 94e2 1f70 7fa5 dce5 1932 3b92  .O.....p.....2;.
+000044f0: ef44 bc41 0664 8b3e c637 365e 0e6f 689f  .D.A.d.>.76^.oh.
+00004500: 4a94 358c 1b26 9f10 0e30 8bf6 580a 9ecd  J.5..&...0..X...
+00004510: 90b1 4da8 2b92 e116 a888 8296 a4e1 e67e  ..M.+..........~
+00004520: 588c f1d1 fe4c 0bd6 8860 d875 cbb6 ca74  X....L...`.u...t
+00004530: 1031 3eda 9f6c c5fa 537b 076d cda7 1a9e  .1>..l..S{.m....
+00004540: 198c a8d1 2cc6 3faf 961f e6ab ab34 7066  ....,.?......4pf
+00004550: de72 e64c ce69 e8cc c3e5 ca09 2797 cbd5  .r.L.i......'...
+00004560: 2a9d 7b81 77f9 6bd4 0adf d008 bbce 0d95  *.{.w.k.........
+00004570: e04f 1635 8776 a9f7 c1ee 43bc 3bfa 623c  .O.5.v....C.;.b<
+00004580: 9af4 f4bb b70a b4c7 dce7 c1d4 fb18 fa9e  ................
+00004590: 939e 7bbe 3399 9299 339b 9e87 4e1a fac1  ..{.3...3...N...
+000045a0: 6a3a 595e 8569 38e2 1ebe b261 7aae eff7  j:Y^.i8....az...
+000045b0: add7 920f 1786 09ca 993c 6875 5068 ec05  .........<huPh..
+000045c0: 9160 fa8f 20dc 8312 eef1 b398 fc06 0000  .`.. ...........
+000045d0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+000045e0: 2100 4792 ec58 ce01 0000 b603 0000 1400  !.G..X..........
+000045f0: 0000 786c 2f73 6861 7265 6453 7472 696e  ..xl/sharedStrin
+00004600: 6773 2e78 6d6c 9c53 cb6e db30 10bc 17e8  gs.xml.S.n.0....
+00004610: 3f2c 8402 4d8b d892 9d38 ea43 5650 c449  ?,..M....8.CVP.I
+00004620: 2e85 5320 0e72 3468 7165 b111 4995 bb72  ..S .r4hqe..I..r
+00004630: e2bf efca 6e80 4242 2f3d 7238 331c ce92  ....n.BB/=r83...
+00004640: d9e5 8bad 6187 818c 77f3 6832 4e22 4057  ....a...w.h2N"@W
+00004650: 786d dc76 1e3d ac6e 469f 2220 564e abda  xm.v.=.nF." VN..
+00004660: 3b9c 477b a4e8 327f fb26 2362 10ad a379  ;.G{..2..&#b...y
+00004670: 5431 375f e298 8a0a ada2 b16f d0c9 4ee9  T17_.......o..N.
+00004680: 8355 2ccb b08d a909 a834 5588 6ceb 789a  .U,......4U.l.x.
+00004690: 2417 b155 c645 50f8 d6b1 9c7b 368b a075  $..U.EP....{6..u
+000046a0: e657 8b57 4764 3a8d f28c 4c9e 71ee bcc6  .W.WGd:...L.q...
+000046b0: 2ce6 3c8b bbf5 1123 2cd8 873e ba53 753b  ,.<....#,..>.Su;
+000046c0: a03a cf03 ec11 8931 78ea 1bd4 665b 711f  .:.....1x...f[q.
+000046d0: 64f5 840e cae0 2de0 8b21 966a c0aa 2278  d.....-..!.j.."x
+000046e0: d08a 1594 a6c6 81d1 1ed5 209d 0401 6a03  .......... ...j.
+000046f0: c273 a518 d843 d332 2882 9d0a 466d 6a84  .s...C.2(...Fmj.
+00004700: dbc5 0f58 2caf 419a 837f 25fc d94a ef56  ...X,.A...%..J.V
+00004710: 6984 b639 858d 38fc 4fbc 2025 6bd4 72b4  i..9..8.O. %k.r.
+00004720: 1476 0a5a e6e6 f4ba c1b0 ee82 c347 48c6  .v.Z.........GH.
+00004730: b37e 0d01 755b 8866 b307 5216 a154 dd08  .~..u[.f..R..T..
+00004740: 802b e560 8392 19df 93cc 9378 1db0 3c3a  .+.`.......x..<:
+00004750: c389 1825 93f4 3c4d d319 9c1c bcd3 24f9  ...%..<M......$.
+00004760: 00a3 03fe 0a5d 7c16 08e6 1d96 4c0f dcaf  .....]|.....L...
+00004770: 7ff4 9319 3c4b 4365 1717 8c83 abbb fbd5  ....<KCe........
+00004780: 7a79 b7f8 f67d bdbc 5ef5 139e 2509 c82c  zy...}..^...%..,
+00004790: e898 e970 b74e 549a 209d c9e5 8cd7 7d89  ...p.NT. .....}.
+000047a0: bcb9 c1bc 1fee 17f1 d3a3 ea53 6fdf 0d90  ...........So...
+000047b0: 2169 d4e7 ac06 aac2 5b2b ff8b f783 c787  !i......[+......
+000047c0: 3bac 0701 09cb f62f 3496 7f97 ff06 0000  ;....../4.......
+000047d0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+000047e0: 2100 3b6d 324b c100 0000 4201 0000 2300  !.;m2K....B...#.
+000047f0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00004800: 5f72 656c 732f 7368 6565 7431 2e78 6d6c  _rels/sheet1.xml
+00004810: 2e72 656c 7384 8fc1 8ac2 3014 45f7 03fe  .rels.....0.E...
+00004820: 4378 7b93 d685 0c43 5337 22b8 55e7 0362  Cx{....CS7".U..b
+00004830: fada 06db 9790 f714 fd7b b31c 65c0 e5e5  .........{..e...
+00004840: 70cf e536 9bfb 3ca9 1b66 0e91 2cd4 ba02  p..6..<..f..,...
+00004850: 85e4 6317 68b0 f07b da2d bf41 b138 eadc  ..c.h..{.-.A.8..
+00004860: 1409 2d3c 9061 d32e be9a 034e 4e4a 89c7  ..-<.a.....NNJ..
+00004870: 9058 150b b185 5124 fd18 c37e c4d9 b18e  .X....Q$...~....
+00004880: 09a9 903e e6d9 4989 7930 c9f9 8b1b d0ac  ...>..I.y0......
+00004890: aa6a 6df2 5f07 b42f 4eb5 ef2c e47d 5783  .jm._../N..,.}W.
+000048a0: 3a3d 5259 feec 8e7d 1f3c 6ea3 bfce 48f2  :=RY...}.<n...H.
+000048b0: cf84 4939 9060 3ea2 4839 c845 edf2 8062  ..I9.`>.H9.E...b
+000048c0: 41eb 77f6 9e6b 7d0e 04a6 6dcc cbf3 f609  A.w..k}...m.....
+000048d0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+000048e0: 0000 2100 dd2c f4a4 c302 0000 d023 0000  ..!..,.......#..
+000048f0: 2700 0000 786c 2f70 7269 6e74 6572 5365  '...xl/printerSe
+00004900: 7474 696e 6773 2f70 7269 6e74 6572 5365  ttings/printerSe
+00004910: 7474 696e 6773 312e 6269 6eec 5acb 6ed3  ttings1.bin.Z.n.
+00004920: 5010 3dd7 49d5 4024 1012 128f 5529 1b04  P.=.I.@$....U)..
+00004930: 029a 36c0 3a44 bc44 5245 6d50 b2a8 1419  ..6.:D.DREmP....
+00004940: 2520 4b4d 8c12 95b4 0b04 1b7e a29f c096  % KM.......~....
+00004950: 0fe0 23d8 f201 2d6b 16ec c299 6b3b 0f62  ..#...-k....k;.b
+00004960: 5b81 a46a 2077 2c5b f678 ae3d f7cc c377  [..j w,[.x.=...w
+00004970: 46de c10e 1ec3 c52e 3717 5d14 d120 e7d5  F.......7.].. ..
+00004980: 10a7 494e 0d0f 5101 b081 dbc8 f0f8 0879  ..IN..Q........y
+00004990: 9e65 c951 49a8 6ff8 b17a fe0b 2c85 3338  .e.QI.o..z..,.38
+000049a0: 4c67 5375 282c a3ca 6b8b c704 a572 5af6  LgSu(,..k....rZ.
+000049b0: 2ed6 b1cf f119 7266 494a 453f ed68 15d8  ......rfIJE?.h..
+000049c0: 2e15 aa22 22e7 f907 f7d6 9c21 f152 be50  ...""......!.R.P
+000049d0: 2d4c a08c cc2d 9b3a 4cdf 82b7 2937 f5fd  -L...-.:L...)7..
+000049e0: 2cc7 65af 013f 6f02 0d25 773d 6ec0 53a8  ,.e..?o..%w=n.S.
+000049f0: 735b 469c 7e23 af56 2442 aaf0 ac55 6edb  s[F.~#.V$B...Un.
+00004a00: 07d1 3879 6223 c2eb 9193 a01d f8cc 11e1  ..8yb#..........
+00004a10: 8d48 e1c4 b8b0 9839 9c92 e3c2 857c 3942  .H.....9.....|9B
+00004a20: f888 8ef0 9b1a 45bb b567 ef86 c927 c9ec  ......E..g...'..
+00004a30: 0b4f e42b c104 4f59 3878 bd62 0ccc 07cd  .O.+..OY8x.b....
+00004a40: 8b1e 7302 8751 c320 6010 5800 044c de9b  ..s..Q. `.X..L..
+00004a50: a591 e54b 2fcf 33a8 9ae4 6110 5874 042c  ...K/.3...a.Xt.,
+00004a60: e601 5970 7bab 5ce6 8473 c335 4e48 8e08  ..Yp{.\..s.5NH..
+00004a70: 2981 e232 89dc 4b80 a5a5 1692 6240 328f  )..2..K.....b@2.
+00004a80: 3f42 33eb 7807 2479 2abb 56a5 f71e 3896  ?B3.x.$y*.V...8.
+00004a90: f245 1f82 7c15 58aa 52ac 65d6 32d1 767b  .E..|.X.R.e.2.v{
+00004aa0: 812d 3c61 5dbb 89a8 fa25 dee6 d38e fff7  .-<a]....%......
+00004ab0: 3d2a 8736 1cd8 ec23 fc1d 293c 452f 7468  =*.6...#..)<E/th
+00004ac0: 6079 b1ff 60d7 dea7 7dc1 3ba3 c3cc 2189  `y..`...}.;...!.
+00004ad0: 730e 79af 764b cf8f fb6c 4f64 7872 32c6  s.y.vK...lOdxr2.
+00004ae0: 9f94 eff4 bc5a f267 17c4 4d3f f6a6 9ef5  .....Z.g..M?....
+00004af0: b496 037a e186 9b81 3d2c dd0f 6147 499a  ...z....=,..aGI.
+00004b00: 299c babc 6950 5b0b 74d2 8599 90c6 b390  )...iP[.t.......
+00004b10: 920e 55d5 2a25 2e4b 274b 9397 39f4 5560  ..U.*%.K'K..9.U`
+00004b20: 3a26 19b3 f039 f9e0 f29d 7e1e c3d8 e864  :&...9....~....d
+00004b30: 1030 089c 2202 352e 3973 6d27 bc5b eceb  .0..".5.9sm'.[..
+00004b40: 9577 f7da 4ea3 bdb2 d9e8 866a 5a76 9a8d  .w..N......jZv..
+00004b50: 8edc 5dd9 729b 766b 4c66 fba0 f9d2 8d59  ..].r.vkLf.....Y
+00004b60: be54 9cd6 eb3a f78e f104 83c0 7f88 c052  .T...:.........R
+00004b70: fad2 c5ab e1f3 9a30 f422 4131 a167 22c6  .......0."A1.g".
+00004b80: 2010 8380 5477 c72c 3dae b30a 7178 f196   ...Tw.,=...qx..
+00004b90: 85cf a793 ad68 bdda 59e1 3982 d272 c12d  .....h..Y.9..r.-
+00004ba0: 1454 d6c6 510d 027f e60b fa67 900f d387  .T..Q......g....
+00004bb0: 6b07 6fd8 3feb ea3f 71ee f39f 993b fcf7  k.o.?..?q....;..
+00004bc0: 669f fb80 fc6e 47bf ebc1 3481 cf5f 3f76  f....nG...4.._?v
+00004bd0: aed8 176e 88d4 2f00 0000 ffff 0300 504b  ...n../.......PK
+00004be0: 0304 1400 0600 0800 0000 2100 b215 5fdf  ..........!..._.
+00004bf0: 9b00 0000 ba00 0000 1000 0000 786c 2f63  ............xl/c
+00004c00: 616c 6343 6861 696e 2e78 6d6c 3c8e c10a  alcChain.xml<...
+00004c10: c230 1044 ef82 ff10 f66e b7f6 2022 4d0b  .0.D.....n.. "M.
+00004c20: 16fc 02fd 8090 ae4d 20d9 946c 10fd 7b83  .......M ..l..{.
+00004c30: 8a97 8179 0333 d38f cf18 d483 b2f8 c41a  ...y.3..........
+00004c40: f64d 0b8a d8a6 d9f3 a2e1 76bd ec8e a0a4  .M........v.....
+00004c50: 189e 4d48 4c1a 5e24 300e db4d 6f4d b093  ..MHL.^$0..MoM..
+00004c60: 339e 556d 60d1 e04a 594f 8862 1d45 234d  3.Um`..JYO.b.E#M
+00004c70: 5a89 6b72 4f39 9a52 6d5e 50d6 4c66 1647  Z.krO9.Rm^P.Lf.G
+00004c80: 5462 c0ae 6d0f 186b 010c bd55 59c3 b903  Tb..m..k...UY...
+00004c90: e535 540d f509 e00f 4f5f fc01 f85f 1dde  .5T.....O_..._..
+00004ca0: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00004cb0: 0000 0021 005b 450c 5395 0100 00ef 0200  ...!.[E.S.......
+00004cc0: 0011 0008 0164 6f63 5072 6f70 732f 636f  .....docProps/co
+00004cd0: 7265 2e78 6d6c 20a2 0401 28a0 0001 0000  re.xml ...(.....
+00004ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004e80: 0000 0000 0000 0000 0000 7c52 5d6f db20  ..........|R]o. 
-00004e90: 147d 9fb4 ff60 f1ee 80ed ae1f c8a1 5297  .}...`........R.
-00004ea0: 759a b44c 939a 6a55 df28 dc26 6c36 4670  u..L..jU.(.&l6Fp
-00004eb0: 5337 ffbe 1827 6ea2 4d7b e3de 7338 9c7b  S7...'n.M{..s8.{
-00004ec0: 2ef5 f56b db64 2fe0 83e9 ec9c 1433 4632  ...k.d/......3F2
-00004ed0: b0aa d3c6 aee7 e47e 759b 5f92 2ca0 b45a  .......~u._.,..Z
-00004ee0: 369d 8539 d941 20d7 e2e3 875a 39ae 3a0f  6..9.A ....Z9.:.
-00004ef0: 3f7d e7c0 a381 9045 251b b872 73b2 4174  ?}.....E%..rs.At
-00004f00: 9cd2 a036 d0ca 308b 0c1b c1e7 ceb7 1263  ...6..0........c
-00004f10: e9d7 d449 f547 ae81 968c 9dd3 1650 6a89  ...I.G.......Pj.
-00004f20: 920e 82b9 9b14 c95e 52ab 49d2 6d7d 9304  .......^R.I.m}..
-00004f30: b4a2 d040 0b16 032d 6605 7de7 22f8 36fc  ...@...-f.}.".6.
-00004f40: f342 428e 98ad c19d 8b33 eded 1e6b 6b35  .BB......3...kk5
-00004f50: 8213 fb35 9889 d8f7 fdac af92 8de8 bfa0  ...5............
-00004f60: 0fcb ef77 69d4 dcd8 212b 0544 d45a 7134  ...wi...!+.D.Zq4
-00004f70: d880 a8e9 fb31 9ec2 f6e9 3728 1cdb 5311  .....1....7(..S.
-00004f80: 01e5 4162 e7c5 5222 6ea0 cfbe 7e5b 2cbe  ..Ab..R"n...~[,.
-00004f90: fc48 b70f d020 aa21 286f 1cc6 7d8d 1a27  .H... .!(o..}..'
-00004fa0: 8db8 9546 065c c605 3e1b d037 3bd1 c8ad  ...F.\..>..7;...
-00004fb0: 9735 fd1b 1836 e8e1 c50c 9b17 9789 3195  .5...6........1.
-00004fc0: f1a1 14d6 680a 7416 c7e7 6358 07e4 57f5  ....h.t...cX..W.
-00004fd0: 79b1 ba25 a264 c555 ce2e f2b2 5ab1 2bce  y..%.d.U....Z.+.
-00004fe0: cef8 a7e2 7130 7d72 7f88 636c b47b 67ff  ....q0}r..cl.{g.
-00004ff0: 552c cb9c 5579 55ac d839 3fbb e045 79a4  U,..UyU..9?..Ey.
-00005000: 7810 4809 37d2 aeb7 f11f 09b0 f9fd 5dca  x.H.7.........].
-00005010: 6a6a a589 4ebf a878 0300 00ff ff03 0050  jj..N..x.......P
-00005020: 4b03 0414 0006 0008 0000 0021 00f3 0d72  K..........!...r
-00005030: 65ee 0100 007c 0400 0010 0008 0164 6f63  e....|.......doc
-00005040: 5072 6f70 732f 6170 702e 786d 6c20 a204  Props/app.xml ..
-00005050: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
+00004dd0: 0000 0000 0000 0000 0000 0000 0000 7c52  ..............|R
+00004de0: d16e db20 147d 9fd4 7fb0 7877 b09d 764b  .n. .}....xw..vK
+00004df0: 9043 a52e eb34 6999 2a35 55a7 bd31 b84d  .C...4i.*5U..1.M
+00004e00: d80c 4670 5337 7f3f 8c13 3751 abbd 71ef  ..FpS7.?..7Q..q.
+00004e10: 391c ce3d 97fa fac5 34d9 33f8 a05b bb20  9..=....4.3..[. 
+00004e20: e5a4 2019 58d9 2a6d 370b f2b0 becd 6724  .. .X.*m7.....g$
+00004e30: 0b28 ac12 4d6b 6141 f610 c835 bff8 504b  .(..MkaA...5..PK
+00004e40: c764 ebe1 ceb7 0e3c 6a08 5954 b281 49b7  .d.....<j.YT..I.
+00004e50: 205b 44c7 280d 720b 4684 4964 d808 3eb5   [D.(.r.F.Id..>.
+00004e60: de08 8ca5 df50 27e4 5fb1 015a 15c5 476a  .....P'._..Z..Gj
+00004e70: 0085 1228 682f 98bb 5191 1c24 951c 25dd  ...(h/..Q..$..%.
+00004e80: ce37 4940 490a 0d18 b018 6839 29e9 2b17  .7I@I.....h9).+.
+00004e90: c19b f0ee 8584 9c30 8dc6 bd8b 331d ec9e  .......0....3...
+00004ea0: 6a2b 3980 23fb 25e8 91d8 75dd a49b 261b  j+9.#.%...u...&.
+00004eb0: d17f 497f aebe dfa7 5173 6dfb ac24 105e  ..I.....Qsm..$.^
+00004ec0: 2bc9 5063 03bc a6af c778 0abb df7f 40e2  +.Pc.....x....@.
+00004ed0: d01e 8b08 480f 025b cf57 0271 0b5d f6f5  ....H..[.W.q.]..
+00004ee0: db72 f9e5 47ba 7d84 7a51 0541 7aed 30ee  .r..G.}.zQ.Az.0.
+00004ef0: 6bd0 386b c4ad 3422 e02a 2ef0 4983 bad9  k.8k..4".*..I...
+00004f00: 73a1 8cb6 357d 0bf4 1bf4 f0ac fbcd f359  s...5}.........Y
+00004f10: 628c 657c 2885 3598 0295 c5f1 d910 d611  b.e|(.5.........
+00004f20: 799c 7e5e ae6f 09af 8a72 9e17 9ff2 6aba  y.~^.o...r....j.
+00004f30: 2ee6 acb8 6457 e5af def4 d9fd 3e8e a161  ....dW......>..a
+00004f40: 0ece feab 5855 7931 cfcb cb75 59b2 e99c  ....XUy1...uY...
+00004f50: 5dcd 4e14 8f02 29e1 46d8 cd2e fe23 0e36  ].N...).F....#.6
+00004f60: 7fb8 4f59 8dad 34d1 f917 e5ff 0000 00ff  ..OY..4.........
+00004f70: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00004f80: 00b0 d006 72e7 0100 0077 0400 0010 0008  ....r....w......
+00004f90: 0164 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
+00004fa0: 6c20 a204 0128 a000 0100 0000 0000 0000  l ...(..........
+00004fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000050a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000050b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000050c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000050d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000050e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000050f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005150: 0000 0000 009c 54c1 6edb 300c bd0f d83f  ......T.n.0....?
-00005160: 18be 3776 9aa1 1802 4545 d176 e861 c58c  ..7v....EE.v.a..
-00005170: c5ed b550 243a 1122 4b82 c418 c9be 677f  ...P$:."K.....g.
-00005180: b21f 1b1d 778e 833a 97dd 483e eaf9 897c  ....w..:..H>...|
-00005190: 32bb ddd7 2669 2044 edec 229d 4ef2 3401  2...&i D..".N.4.
-000051a0: 2b9d d276 bd48 5fca 6f57 5fd3 24a2 b04a  +..v.H_.oW_.$..J
-000051b0: 1867 6191 1e20 a6b7 fcf3 2756 04e7 21a0  .ga.. ....'V..!.
-000051c0: 8698 1085 8d8b 7483 e8e7 5916 e506 6a11  ......t...Y...j.
-000051d0: 2704 5b42 2a17 6a81 9486 75e6 aa4a 4b78  '.[B*.j...u..JKx
-000051e0: 7072 5783 c5ec 3acf 6f32 d823 5805 eaca  prW...:.o2.#X...
-000051f0: f784 69c7 386f f07f 4995 93ad bef8 5a1e  ..i.8o..I.....Z.
-00005200: 3c09 e6ac 84da 1b81 c059 760a 4b87 c294  <........Yv.K...
-00005210: ba06 9e53 b94f d89d f746 4b81 3412 feac  ...S.O...FK.4...
-00005220: 6570 d155 983c ee25 1896 0d41 4657 5982  ep.U.<.%...AFWY.
-00005230: dc05 8d87 9663 98b2 a514 06ee 4905 af84  .....c......I...
-00005240: 89c0 b253 813d 8168 275c 081d 2267 0dce  ...S.=.h'\.."g..
-00005250: 1b90 e842 12f5 2f9a f175 9aac 4484 56fb  ...B../..u..D.V.
-00005260: 226d 44d0 c222 dda1 6deb 9263 6c7c c4c0  "mD.."..m..cl|..
-00005270: efc2 0a34 c695 f9f3 1b11 02cb a8ab 438e  ...4..........C.
-00005280: e1f0 c030 d65f f874 76ec a0e8 bcb3 65e8  ...0._.tv.....e.
-00005290: e410 702e b4d4 6820 fea8 0a11 7044 f774  ..p...h ....pD.t
-000052a0: 3614 7e54 d1c9 ee04 f940 cb7f 0b50 0d45  6.~T.....@...P.E
-000052b0: f672 a58b 7811 54e4 28ab 2ec2 c6a1 a3d5  .r..x.T.(.......
-000052c0: 9cae de47 1077 ab51 4005 72c3 3802 fe6c  ...G.w.Q@.r.8..l
-000052d0: 8c3d d7d6 3771 f4c4 76ad fc28 40f5 3772  .=..7q..v..(@.7r
-000052e0: 815e 5dfc 9800 d0a3 479f 1f7f a22b 8ae2  .^].....G....+..
-000052f0: c2ac 6ca5 d71f 767d f450 ebf0 f335 7dd7  ..l...v}.P...5}.
-00005300: 761b 5f7c e91e da07 f06e c6f3 225b 6e44  v._|.....n.."[nD
-00005310: 0045 feed cdda 17d8 13f9 3098 96e4 7e23  .E........0...~#
-00005320: ec1a d4bf 9e8f 40fb 745e bb9f 099f de4c  ......@.t^.....L
-00005330: f259 4eaf 6250 63d9 e9b7 c1ff 0200 00ff  .YN.bPc.........
-00005340: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00005350: 0016 2918 194f 0100 00bc 0300 0013 0008  ..)..O..........
-00005360: 0164 6f63 5072 6f70 732f 6375 7374 6f6d  .docProps/custom
-00005370: 2e78 6d6c 20a2 0401 28a0 0001 0000 0000  .xml ...(.......
+000050a0: 0000 0000 0000 0000 009c 544d 6fdb 300c  ..........TMo.0.
+000050b0: bd0f e87f 307c 6fec 3443 3104 8a8a a11f  ....0|o.4C1.....
+000050c0: e861 c58c c5ed 8e85 22d1 8910 5912 24c6  .a......"...Y.$.
+000050d0: 48f6 eb47 c79d e3a0 ce65 3792 8fa2 1ec9  H..G.....e7.....
+000050e0: 27b1 bb7d 6d92 0642 d4ce 2ed2 e924 4f13  '..}m..B.....$O.
+000050f0: b0d2 296d d78b f4b5 7cba fe96 2611 8555  ..)m....|...&..U
+00005100: c238 0b8b f400 31bd e357 5f58 119c 8780  .8....1..W_X....
+00005110: 1a62 4225 6c5c a41b 443f cfb2 2837 508b  .bB%l\..D?..(7P.
+00005120: 3821 d812 52b9 500b 2437 ac33 5755 5ac2  8!..R.P.$7.3WUZ.
+00005130: 8393 bb1a 2c66 3779 7e9b c11e c12a 50d7  ....,f7y~....*P.
+00005140: be2f 9876 15e7 0dfe 6f51 e564 cb2f be95  ./.v....oQ.d./..
+00005150: 074f 8439 2ba1 f646 2070 969d ccd2 a130  .O.9+..F p.....0
+00005160: a5ae 81e7 14ee 1df6 dd7b a3a5 401a 097f  .........{..@...
+00005170: d132 b8e8 2a4c 1ef7 120c cb86 20a3 5696  .2..*L...... .V.
+00005180: 2077 41e3 a1ad 3174 d952 0a03 f7c4 8257   wA...1t.R.....W
+00005190: c244 60d9 29c0 9e41 b413 2e84 0e91 b306  .D`.)..A........
+000051a0: e70d 4874 2189 fa0f cdf8 264d 5622 42cb  ..Ht!.....&MV"B.
+000051b0: 7d91 3622 6861 917a 68d3 3ae7 681b 1f31  }.6"ha.zh.:.h..1
+000051c0: f0df 2e6c e306 0023 cb28 a10b 1ecd 61ee  ...l...#.(....a.
+000051d0: d0d6 5ff9 7476 cc20 eb3c b3ad d031 21e0  .._.tv. .<...1!.
+000051e0: 9c63 a9d1 40fc 5915 22e0 08e5 e96c c8f9  .c..@.Y."....l..
+000051f0: c8a2 63dc 11f2 81f6 fe1e a01a 92ec e94a  ..c............J
+00005200: 17f1 22a8 484c 565d 848d 4347 5b39 b5de  ..".HLV]..CG[9..
+00005210: 5b10 77ab 5140 0512 c238 023e 8c02 5bdf  [.w.Q@...8.>..[.
+00005220: 9ccd b7bf 64bb 567e f404 c5df 4900 7a75  ....d.V~....I.zu
+00005230: f132 01a0 478f be3c fe42 5714 c585 59d9  .2..G..<.BW...Y.
+00005240: 4aaf 3fed fa28 9f56 dce7 6bfa a1ed 36be  J.?..(.V..k...6.
+00005250: fad2 3db4 daff d0e1 7990 2d37 2280 22e9  ..=.....y.-7".".
+00005260: f63a ed03 ec99 2418 4c5b e47e 23ec 1ad4  .:....$.L[.~#...
+00005270: bf9c cf40 fb6a deba 7f84 4f6f 27f9 2ca7  ...@.j....Oo'.,.
+00005280: 0731 88b1 ecf4 63f0 bf00 0000 ffff 0300  .1....c.........
+00005290: 504b 0304 1400 0600 0800 0000 2100 1629  PK..........!..)
+000052a0: 1819 4f01 0000 bc03 0000 1300 0801 646f  ..O...........do
+000052b0: 6350 726f 7073 2f63 7573 746f 6d2e 786d  cProps/custom.xm
+000052c0: 6c20 a204 0128 a000 0100 0000 0000 0000  l ...(..........
+000052d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000052e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000052f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000053a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000053b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000053c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000053d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000053e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000053f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005470: 0000 0000 0000 0000 0000 0000 bcd3 4d6f  ..............Mo
-00005480: 8230 1807 f0fb 927d 07d2 3bb6 a0a8 18c0  .0.....}..;.....
-00005490: 2868 76d8 6189 2ff7 ae14 6906 6dd3 5637  (hv.a./...i.m.V7
-000054a0: b2ec bbaf c8d0 ebb2 196f 7dcb fff7 f449  .........o}....I
-000054b0: 1bcd 3fea ca39 51a5 99e0 31f0 0608 3894  ..?..9Q...1...8.
-000054c0: 1391 337e 88c1 6ebb 76a7 c0d1 06f3 1c57  ..3~..n.v......W
-000054d0: 82d3 1834 5483 79f2 f810 bd28 21a9 328c  ...4T.y....(!.2.
-000054e0: 6ac7 4670 1d83 d218 3983 5093 92d6 580f  j.Fp....9.P...X.
-000054f0: ec36 b73b 8550 3536 76aa 0e50 1405 2334  .6.;.P56v..P..#4
-00005500: 13e4 5853 6ea0 8fd0 1892 a336 a276 e525  ..XSn......6.v.%
-00005510: 0e74 79b3 93f9 6b64 2e48 5b9d de6f 1b69  .ty...kd.H[..o.i
-00005520: cb4d a29f f0c6 296a c3f2 187c 6641 9a65  .M....)j...|fA.e
-00005530: 010a 5c7f 15a6 ae87 bca5 1b0e c389 8ba6  ..\.............
-00005540: 08f9 4b3f 5d87 8bd5 1770 647b d807 0ec7  ..K?]....pd{....
-00005550: b5bd fa42 ca7d d728 1b79 32b3 4abe 6ba3  ...B.}.(.y2.J.k.
-00005560: 122f 18a0 2142 11bc 2e45 b017 ff69 0f7b  ./..!B...E...i.{
-00005570: dbf6 6c43 c951 31d3 7438 1b25 1d69 0737  ..lC.Q1.t8.%.i.7
-00005580: e346 3df7 641b a72a c6df 745a 627e a079  .F=.d..*..tZb~.y
-00005590: 87be 0a51 2505 ae34 3ddf f63c bd19 1ef4  ...Q%..4=..<....
-000055a0: f873 ebee e456 64d8 d03b c0e3 1ede 105c  .s...Vd..;.....\
-000055b0: d1d4 be9c 3ba0 930b 5a62 d57e 89df 99f0  ....;...Zb.~....
-000055c0: faed 926f 0000 00ff ff03 0050 4b01 022d  ...o.......PK..-
-000055d0: 0014 0006 0008 0000 0021 00d6 9dc7 d6bd  .........!......
-000055e0: 0100 0065 0c00 0013 0000 0000 0000 0000  ...e............
-000055f0: 0000 0000 0000 0000 005b 436f 6e74 656e  .........[Conten
-00005600: 745f 5479 7065 735d 2e78 6d6c 504b 0102  t_Types].xmlPK..
-00005610: 2d00 1400 0600 0800 0000 2100 135e be65  -.........!..^.e
-00005620: 0201 0000 df02 0000 0b00 0000 0000 0000  ................
-00005630: 0000 0000 0000 f603 0000 5f72 656c 732f  .........._rels/
-00005640: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
-00005650: 0000 0021 0006 2513 c833 0400 00c9 0a00  ...!..%..3......
-00005660: 000f 0000 0000 0000 0000 0000 0000 0029  ...............)
-00005670: 0700 0078 6c2f 776f 726b 626f 6f6b 2e78  ...xl/workbook.x
-00005680: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-00005690: 2100 2900 1d8f 5501 0000 e709 0000 1a00  !.)...U.........
-000056a0: 0000 0000 0000 0000 0000 0000 890b 0000  ................
-000056b0: 786c 2f5f 7265 6c73 2f77 6f72 6b62 6f6f  xl/_rels/workboo
-000056c0: 6b2e 786d 6c2e 7265 6c73 504b 0102 2d00  k.xml.relsPK..-.
-000056d0: 1400 0600 0800 0000 2100 5baf d84c 1e03  ........!.[..L..
-000056e0: 0000 ad06 0000 1800 0000 0000 0000 0000  ................
-000056f0: 0000 0000 1e0e 0000 786c 2f77 6f72 6b73  ........xl/works
-00005700: 6865 6574 732f 7368 6565 7431 2e78 6d6c  heets/sheet1.xml
-00005710: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00005720: 861b 55f6 5403 0000 db06 0000 1800 0000  ..U.T...........
-00005730: 0000 0000 0000 0000 0000 7211 0000 786c  ..........r...xl
-00005740: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00005750: 7432 2e78 6d6c 504b 0102 2d00 1400 0600  t2.xmlPK..-.....
-00005760: 0800 0000 2100 d029 2692 3503 0000 e806  ....!..)&.5.....
-00005770: 0000 1800 0000 0000 0000 0000 0000 0000  ................
-00005780: fc14 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00005790: 732f 7368 6565 7433 2e78 6d6c 504b 0102  s/sheet3.xmlPK..
-000057a0: 2d00 1400 0600 0800 0000 2100 239e ec80  -.........!.#...
-000057b0: 2d03 0000 a306 0000 1800 0000 0000 0000  -...............
-000057c0: 0000 0000 0000 6718 0000 786c 2f77 6f72  ......g...xl/wor
-000057d0: 6b73 6865 6574 732f 7368 6565 7434 2e78  ksheets/sheet4.x
-000057e0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-000057f0: 2100 8608 71bb 2b03 0000 a206 0000 1800  !...q.+.........
-00005800: 0000 0000 0000 0000 0000 0000 ca1b 0000  ................
-00005810: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00005820: 6565 7435 2e78 6d6c 504b 0102 2d00 1400  eet5.xmlPK..-...
-00005830: 0600 0800 0000 2100 3475 cd85 2f03 0000  ......!.4u../...
-00005840: a506 0000 1800 0000 0000 0000 0000 0000  ................
-00005850: 0000 2b1f 0000 786c 2f77 6f72 6b73 6865  ..+...xl/workshe
-00005860: 6574 732f 7368 6565 7436 2e78 6d6c 504b  ets/sheet6.xmlPK
-00005870: 0102 2d00 1400 0600 0800 0000 2100 f77d  ..-.........!..}
-00005880: c8d5 2e03 0000 a306 0000 1800 0000 0000  ................
-00005890: 0000 0000 0000 0000 9022 0000 786c 2f77  ........."..xl/w
-000058a0: 6f72 6b73 6865 6574 732f 7368 6565 7437  orksheets/sheet7
-000058b0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-000058c0: 0000 2100 7576 beb0 2e03 0000 a406 0000  ..!.uv..........
-000058d0: 1800 0000 0000 0000 0000 0000 0000 f425  ...............%
-000058e0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-000058f0: 7368 6565 7438 2e78 6d6c 504b 0102 2d00  sheet8.xmlPK..-.
-00005900: 1400 0600 0800 0000 2100 c55f 466e 2e03  ........!.._Fn..
-00005910: 0000 a206 0000 1800 0000 0000 0000 0000  ................
-00005920: 0000 0000 5829 0000 786c 2f77 6f72 6b73  ....X)..xl/works
-00005930: 6865 6574 732f 7368 6565 7439 2e78 6d6c  heets/sheet9.xml
-00005940: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00005950: 85a1 db38 bc03 0000 e00a 0000 1900 0000  ...8............
-00005960: 0000 0000 0000 0000 0000 bc2c 0000 786c  ...........,..xl
-00005970: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00005980: 7431 302e 786d 6c50 4b01 022d 0014 0006  t10.xmlPK..-....
-00005990: 0008 0000 0021 0095 8c23 639e 0300 0018  .....!...#c.....
-000059a0: 0a00 0019 0000 0000 0000 0000 0000 0000  ................
-000059b0: 00af 3000 0078 6c2f 776f 726b 7368 6565  ..0..xl/workshee
-000059c0: 7473 2f73 6865 6574 3131 2e78 6d6c 504b  ts/sheet11.xmlPK
-000059d0: 0102 2d00 1400 0600 0800 0000 2100 8ec7  ..-.........!...
-000059e0: 9b39 7303 0000 a008 0000 1900 0000 0000  .9s.............
-000059f0: 0000 0000 0000 0000 8434 0000 786c 2f77  .........4..xl/w
-00005a00: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00005a10: 322e 786d 6c50 4b01 022d 0014 0006 0008  2.xmlPK..-......
-00005a20: 0000 0021 0044 5e69 3884 0300 0007 0800  ...!.D^i8.......
-00005a30: 0019 0000 0000 0000 0000 0000 0000 002e  ................
-00005a40: 3800 0078 6c2f 776f 726b 7368 6565 7473  8..xl/worksheets
-00005a50: 2f73 6865 6574 3133 2e78 6d6c 504b 0102  /sheet13.xmlPK..
-00005a60: 2d00 1400 0600 0800 0000 2100 5807 37e9  -.........!.X.7.
-00005a70: 4e07 0000 c020 0000 1300 0000 0000 0000  N.... ..........
-00005a80: 0000 0000 0000 e93b 0000 786c 2f74 6865  .......;..xl/the
-00005a90: 6d65 2f74 6865 6d65 312e 786d 6c50 4b01  me/theme1.xmlPK.
-00005aa0: 022d 0014 0006 0008 0000 0021 0064 c1ee  .-.........!.d..
-00005ab0: 86ed 0200 0006 0800 000d 0000 0000 0000  ................
-00005ac0: 0000 0000 0000 0068 4300 0078 6c2f 7374  .......hC..xl/st
-00005ad0: 796c 6573 2e78 6d6c 504b 0102 2d00 1400  yles.xmlPK..-...
-00005ae0: 0600 0800 0000 2100 4792 ec58 ce01 0000  ......!.G..X....
-00005af0: b603 0000 1400 0000 0000 0000 0000 0000  ................
-00005b00: 0000 8046 0000 786c 2f73 6861 7265 6453  ...F..xl/sharedS
-00005b10: 7472 696e 6773 2e78 6d6c 504b 0102 2d00  trings.xmlPK..-.
-00005b20: 1400 0600 0800 0000 2100 3b6d 324b c100  ........!.;m2K..
-00005b30: 0000 4201 0000 2300 0000 0000 0000 0000  ..B...#.........
-00005b40: 0000 0000 8048 0000 786c 2f77 6f72 6b73  .....H..xl/works
-00005b50: 6865 6574 732f 5f72 656c 732f 7368 6565  heets/_rels/shee
-00005b60: 7431 2e78 6d6c 2e72 656c 7350 4b01 022d  t1.xml.relsPK..-
-00005b70: 0014 0006 0008 0000 0021 00dd 2cf4 a4c3  .........!..,...
-00005b80: 0200 00d0 2300 0027 0000 0000 0000 0000  ....#..'........
-00005b90: 0000 0000 0082 4900 0078 6c2f 7072 696e  ......I..xl/prin
-00005ba0: 7465 7253 6574 7469 6e67 732f 7072 696e  terSettings/prin
-00005bb0: 7465 7253 6574 7469 6e67 7331 2e62 696e  terSettings1.bin
-00005bc0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00005bd0: b215 5fdf 9b00 0000 ba00 0000 1000 0000  .._.............
-00005be0: 0000 0000 0000 0000 0000 8a4c 0000 786c  ...........L..xl
-00005bf0: 2f63 616c 6343 6861 696e 2e78 6d6c 504b  /calcChain.xmlPK
-00005c00: 0102 2d00 1400 0600 0800 0000 2100 84b4  ..-.........!...
-00005c10: 5fd2 9501 0000 ef02 0000 1100 0000 0000  _...............
-00005c20: 0000 0000 0000 0000 534d 0000 646f 6350  ........SM..docP
-00005c30: 726f 7073 2f63 6f72 652e 786d 6c50 4b01  rops/core.xmlPK.
-00005c40: 022d 0014 0006 0008 0000 0021 00f3 0d72  .-.........!...r
-00005c50: 65ee 0100 007c 0400 0010 0000 0000 0000  e....|..........
-00005c60: 0000 0000 0000 001f 5000 0064 6f63 5072  ........P..docPr
-00005c70: 6f70 732f 6170 702e 786d 6c50 4b01 022d  ops/app.xmlPK..-
-00005c80: 0014 0006 0008 0000 0021 0016 2918 194f  .........!..)..O
-00005c90: 0100 00bc 0300 0013 0000 0000 0000 0000  ................
-00005ca0: 0000 0000 0043 5300 0064 6f63 5072 6f70  .....CS..docProp
-00005cb0: 732f 6375 7374 6f6d 2e78 6d6c 504b 0506  s/custom.xmlPK..
-00005cc0: 0000 0000 1a00 1a00 f106 0000 cb55 0000  .............U..
-00005cd0: 0000                                     ..
+000053c0: 0000 0000 0000 0000 00bc d34d 6f82 3018  ...........Mo.0.
+000053d0: 07f0 fb92 7d07 d23b b6a0 a818 c028 6876  ....}..;.....(hv
+000053e0: d861 892f f7ae 1469 066d d356 37b2 ecbb  .a./...i.m.V7...
+000053f0: afc8 d0eb b219 6f7d cbff f7f4 491b cd3f  ......o}....I..?
+00005400: eaca 3951 a599 e031 f006 0838 9413 9133  ..9Q...1...8...3
+00005410: 7e88 c16e bb76 a7c0 d106 f31c 5782 d318  ~..n.v......W...
+00005420: 3454 8379 f2f8 10bd 2821 a932 8c6a c746  4T.y....(!.2.j.F
+00005430: 701d 83d2 1839 8350 9392 d658 0fec 36b7  p....9.P...X..6.
+00005440: 3b85 5035 3676 aa0e 5014 0523 3413 e458  ;.P56v..P..#4..X
+00005450: 536e a08f d018 92a3 36a2 76e5 250e 7479  Sn......6.v.%.ty
+00005460: b393 f96b 642e 485b 9dde 6f1b 69cb 4da2  ...kd.H[..o.i.M.
+00005470: 9ff0 c629 6ac3 f218 7c66 419a 6501 0a5c  ...)j...|fA.e..\
+00005480: 7f15 a6ae 87bc a51b 0ec3 898b a608 f94b  ...............K
+00005490: 3f5d 878b d517 7064 7bd8 070e c7b5 bdfa  ?]....pd{.......
+000054a0: 42ca 7dd7 281b 7932 b34a be6b a312 2f18  B.}.(.y2.J.k../.
+000054b0: a021 4211 bc2e 45b0 17ff 690f 7bdb f66c  .!B...E...i.{..l
+000054c0: 43c9 5131 d374 381b 251d 6907 37e3 463d  C.Q1.t8.%.i.7.F=
+000054d0: f764 1ba7 2ac6 df74 5a62 7ea0 7987 be0a  .d..*..tZb~.y...
+000054e0: 5125 05ae 343d dff6 3cbd 191e f4f8 73eb  Q%..4=..<.....s.
+000054f0: eee4 5664 d8d0 3bc0 e31e de10 5cd1 d4be  ..Vd..;.....\...
+00005500: 9c3b a093 0b5a 62d5 7e89 df99 f0fa ed92  .;...Zb.~.......
+00005510: 6f00 0000 ffff 0300 504b 0102 2d00 1400  o.......PK..-...
+00005520: 0600 0800 0000 2100 d69d c7d6 bd01 0000  ......!.........
+00005530: 650c 0000 1300 0000 0000 0000 0000 0000  e...............
+00005540: 0000 0000 0000 5b43 6f6e 7465 6e74 5f54  ......[Content_T
+00005550: 7970 6573 5d2e 786d 6c50 4b01 022d 0014  ypes].xmlPK..-..
+00005560: 0006 0008 0000 0021 0013 5ebe 6502 0100  .......!..^.e...
+00005570: 00df 0200 000b 0000 0000 0000 0000 0000  ................
+00005580: 0000 00f6 0300 005f 7265 6c73 2f2e 7265  ......._rels/.re
+00005590: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
+000055a0: 2100 31c7 4420 1b04 0000 a90a 0000 0f00  !.1.D ..........
+000055b0: 0000 0000 0000 0000 0000 0000 2907 0000  ............)...
+000055c0: 786c 2f77 6f72 6b62 6f6f 6b2e 786d 6c50  xl/workbook.xmlP
+000055d0: 4b01 022d 0014 0006 0008 0000 0021 0029  K..-.........!.)
+000055e0: 001d 8f55 0100 00e7 0900 001a 0000 0000  ...U............
+000055f0: 0000 0000 0000 0000 0071 0b00 0078 6c2f  .........q...xl/
+00005600: 5f72 656c 732f 776f 726b 626f 6f6b 2e78  _rels/workbook.x
+00005610: 6d6c 2e72 656c 7350 4b01 022d 0014 0006  ml.relsPK..-....
+00005620: 0008 0000 0021 005e adc5 3212 0300 0065  .....!.^..2....e
+00005630: 0600 0018 0000 0000 0000 0000 0000 0000  ................
+00005640: 0006 0e00 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+00005650: 7473 2f73 6865 6574 312e 786d 6c50 4b01  ts/sheet1.xmlPK.
+00005660: 022d 0014 0006 0008 0000 0021 009d 2b31  .-.........!..+1
+00005670: 054b 0300 00a3 0600 0018 0000 0000 0000  .K..............
+00005680: 0000 0000 0000 004e 1100 0078 6c2f 776f  .......N...xl/wo
+00005690: 726b 7368 6565 7473 2f73 6865 6574 322e  rksheets/sheet2.
+000056a0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+000056b0: 0021 003f b0ce ff2d 0300 009a 0600 0018  .!.?...-........
+000056c0: 0000 0000 0000 0000 0000 0000 00cf 1400  ................
+000056d0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+000056e0: 6865 6574 332e 786d 6c50 4b01 022d 0014  heet3.xmlPK..-..
+000056f0: 0006 0008 0000 0021 0034 444c fb23 0300  .......!.4DL.#..
+00005700: 0067 0600 0018 0000 0000 0000 0000 0000  .g..............
+00005710: 0000 0032 1800 0078 6c2f 776f 726b 7368  ...2...xl/worksh
+00005720: 6565 7473 2f73 6865 6574 342e 786d 6c50  eets/sheet4.xmlP
+00005730: 4b01 022d 0014 0006 0008 0000 0021 0070  K..-.........!.p
+00005740: d984 8d22 0300 0066 0600 0018 0000 0000  ..."...f........
+00005750: 0000 0000 0000 0000 008b 1b00 0078 6c2f  .............xl/
+00005760: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00005770: 352e 786d 6c50 4b01 022d 0014 0006 0008  5.xmlPK..-......
+00005780: 0000 0021 009b a382 4524 0300 0069 0600  ...!....E$...i..
+00005790: 0018 0000 0000 0000 0000 0000 0000 00e3  ................
+000057a0: 1e00 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+000057b0: 2f73 6865 6574 362e 786d 6c50 4b01 022d  /sheet6.xmlPK..-
+000057c0: 0014 0006 0008 0000 0021 002e 4410 4c23  .........!..D.L#
+000057d0: 0300 0067 0600 0018 0000 0000 0000 0000  ...g............
+000057e0: 0000 0000 003d 2200 0078 6c2f 776f 726b  .....="..xl/work
+000057f0: 7368 6565 7473 2f73 6865 6574 372e 786d  sheets/sheet7.xm
+00005800: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00005810: 009e 728f d123 0300 0068 0600 0018 0000  ..r..#...h......
+00005820: 0000 0000 0000 0000 0000 0096 2500 0078  ............%..x
+00005830: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+00005840: 6574 382e 786d 6c50 4b01 022d 0014 0006  et8.xmlPK..-....
+00005850: 0008 0000 0021 00d5 5fc3 3923 0300 0066  .....!.._.9#...f
+00005860: 0600 0018 0000 0000 0000 0000 0000 0000  ................
+00005870: 00ef 2800 0078 6c2f 776f 726b 7368 6565  ..(..xl/workshee
+00005880: 7473 2f73 6865 6574 392e 786d 6c50 4b01  ts/sheet9.xmlPK.
+00005890: 022d 0014 0006 0008 0000 0021 00a5 1431  .-.........!...1
+000058a0: c1ab 0300 0038 0a00 0019 0000 0000 0000  .....8..........
+000058b0: 0000 0000 0000 0048 2c00 0078 6c2f 776f  .......H,..xl/wo
+000058c0: 726b 7368 6565 7473 2f73 6865 6574 3130  rksheets/sheet10
+000058d0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+000058e0: 0000 2100 4a9a 38ce 9403 0000 8209 0000  ..!.J.8.........
+000058f0: 1900 0000 0000 0000 0000 0000 0000 2a30  ..............*0
+00005900: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00005910: 7368 6565 7431 312e 786d 6c50 4b01 022d  sheet11.xmlPK..-
+00005920: 0014 0006 0008 0000 0021 0069 5d0d 9269  .........!.i]..i
+00005930: 0300 0028 0800 0019 0000 0000 0000 0000  ...(............
+00005940: 0000 0000 00f5 3300 0078 6c2f 776f 726b  ......3..xl/work
+00005950: 7368 6565 7473 2f73 6865 6574 3132 2e78  sheets/sheet12.x
+00005960: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00005970: 2100 cf3a da9c 7f03 0000 f507 0000 1900  !..:............
+00005980: 0000 0000 0000 0000 0000 0000 9537 0000  .............7..
+00005990: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+000059a0: 6565 7431 332e 786d 6c50 4b01 022d 0014  eet13.xmlPK..-..
+000059b0: 0006 0008 0000 0021 00c1 1710 be4e 0700  .......!.....N..
+000059c0: 00c6 2000 0013 0000 0000 0000 0000 0000  .. .............
+000059d0: 0000 004b 3b00 0078 6c2f 7468 656d 652f  ...K;..xl/theme/
+000059e0: 7468 656d 6531 2e78 6d6c 504b 0102 2d00  theme1.xmlPK..-.
+000059f0: 1400 0600 0800 0000 2100 b1db eb05 df02  ........!.......
+00005a00: 0000 5c07 0000 0d00 0000 0000 0000 0000  ..\.............
+00005a10: 0000 0000 ca42 0000 786c 2f73 7479 6c65  .....B..xl/style
+00005a20: 732e 786d 6c50 4b01 022d 0014 0006 0008  s.xmlPK..-......
+00005a30: 0000 0021 0047 92ec 58ce 0100 00b6 0300  ...!.G..X.......
+00005a40: 0014 0000 0000 0000 0000 0000 0000 00d4  ................
+00005a50: 4500 0078 6c2f 7368 6172 6564 5374 7269  E..xl/sharedStri
+00005a60: 6e67 732e 786d 6c50 4b01 022d 0014 0006  ngs.xmlPK..-....
+00005a70: 0008 0000 0021 003b 6d32 4bc1 0000 0042  .....!.;m2K....B
+00005a80: 0100 0023 0000 0000 0000 0000 0000 0000  ...#............
+00005a90: 00d4 4700 0078 6c2f 776f 726b 7368 6565  ..G..xl/workshee
+00005aa0: 7473 2f5f 7265 6c73 2f73 6865 6574 312e  ts/_rels/sheet1.
+00005ab0: 786d 6c2e 7265 6c73 504b 0102 2d00 1400  xml.relsPK..-...
+00005ac0: 0600 0800 0000 2100 dd2c f4a4 c302 0000  ......!..,......
+00005ad0: d023 0000 2700 0000 0000 0000 0000 0000  .#..'...........
+00005ae0: 0000 d648 0000 786c 2f70 7269 6e74 6572  ...H..xl/printer
+00005af0: 5365 7474 696e 6773 2f70 7269 6e74 6572  Settings/printer
+00005b00: 5365 7474 696e 6773 312e 6269 6e50 4b01  Settings1.binPK.
+00005b10: 022d 0014 0006 0008 0000 0021 00b2 155f  .-.........!..._
+00005b20: df9b 0000 00ba 0000 0010 0000 0000 0000  ................
+00005b30: 0000 0000 0000 00de 4b00 0078 6c2f 6361  ........K..xl/ca
+00005b40: 6c63 4368 6169 6e2e 786d 6c50 4b01 022d  lcChain.xmlPK..-
+00005b50: 0014 0006 0008 0000 0021 005b 450c 5395  .........!.[E.S.
+00005b60: 0100 00ef 0200 0011 0000 0000 0000 0000  ................
+00005b70: 0000 0000 00a7 4c00 0064 6f63 5072 6f70  ......L..docProp
+00005b80: 732f 636f 7265 2e78 6d6c 504b 0102 2d00  s/core.xmlPK..-.
+00005b90: 1400 0600 0800 0000 2100 b0d0 0672 e701  ........!....r..
+00005ba0: 0000 7704 0000 1000 0000 0000 0000 0000  ..w.............
+00005bb0: 0000 0000 734f 0000 646f 6350 726f 7073  ....sO..docProps
+00005bc0: 2f61 7070 2e78 6d6c 504b 0102 2d00 1400  /app.xmlPK..-...
+00005bd0: 0600 0800 0000 2100 1629 1819 4f01 0000  ......!..)..O...
+00005be0: bc03 0000 1300 0000 0000 0000 0000 0000  ................
+00005bf0: 0000 9052 0000 646f 6350 726f 7073 2f63  ...R..docProps/c
+00005c00: 7573 746f 6d2e 786d 6c50 4b05 0600 0000  ustom.xmlPK.....
+00005c10: 001a 001a 00f1 0600 0018 5500 0000 00    ..........U....
```

### Comparing `message_ix-3.6.0/message_ix/tests/reporting/test_computations.py` & `message_ix-3.7.0/message_ix/tests/reporting/test_computations.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_cli.py` & `message_ix-3.7.0/message_ix/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_core.py` & `message_ix-3.7.0/message_ix/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_feature_addon.py` & `message_ix-3.7.0/message_ix/tests/test_feature_addon.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_feature_bound_activity_shares.py` & `message_ix-3.7.0/message_ix/tests/test_feature_bound_activity_shares.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,18 +42,33 @@
 
     orig_obj = scen.var("OBJ")["lvl"]
     new_obj = clone.var("OBJ")["lvl"]
     assert new_obj >= orig_obj
 
 
 def test_add_bound_activity_up_all_modes(message_test_mp):
+    # This test specifically has two solutions for which the `OBJ` function is the same
+    # therefore the lpmethod must be set to "2".
+    # lpmethod 2:
+    # "transport_from_seattle" needs to provide "to_chicago" with 300.
+    # the unconstrained example seattle delivers 50 to "to_new_york" and 300
+    # "to_chicago".
+    # additional 275 to "to_new_york" comes from san-diego.
+    # The activity bound for "transport_from_seattle" (see below) below is therefore
+    # set to 325.
+    # lpmehtod 4:
+    # the unconstrained example seattle delivers 300 "to_chicago".
+    # san-diego delivers 325 to "to_new_york"
+    # the resulting bound on activity for seattle, therefore is below what is required
+    # for "to_chicago"
     scen = Scenario(message_test_mp, **SCENARIO["dantzig"]).clone()
-    scen.solve(quiet=True)
+    scen.solve(quiet=True, solve_options=dict(lpmethod=2))
 
     # data for act bound
+    print(calculate_activity(scen))
     exp = 0.95 * calculate_activity(scen).sum()
     data = pd.DataFrame(
         {
             "node_loc": "seattle",
             "technology": "transport_from_seattle",
             "year_act": _year,
             "time": "year",
@@ -65,15 +80,15 @@
     )
 
     # test limiting all modes
     clone = scen.clone("foo", "baz", keep_solution=False)
     clone.check_out()
     clone.add_par("bound_activity_up", data)
     clone.commit("foo")
-    clone.solve(quiet=True)
+    clone.solve(quiet=True, solve_options=dict(lpmethod=2))
     obs = calculate_activity(clone).sum()
     assert np.isclose(obs, exp)
 
     orig_obj = scen.var("OBJ")["lvl"]
     new_obj = clone.var("OBJ")["lvl"]
     assert new_obj >= orig_obj
 
@@ -95,14 +110,15 @@
     Constraint Test
     ---------------
 
     Seattle canning_plant production (original: 350) is limited to 50% of all
     transport_from_san-diego (original: 550). Expected outcome: some increase
     of transport_from_san-diego with some decrease of production in seattle.
     """
+
     # data for share bound
     def calc_share(s):
         a = s.var(
             "ACT", filters={"technology": ["canning_plant"], "node_loc": ["seattle"]}
         )["lvl"][0]
         b = calculate_activity(s, tec="transport_from_san-diego").sum()
         return a / b
```

### Comparing `message_ix-3.6.0/message_ix/tests/test_feature_bound_emission.py` & `message_ix-3.7.0/message_ix/tests/test_feature_bound_emission.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_feature_capacity_factor.py` & `message_ix-3.7.0/message_ix/tests/test_feature_capacity_factor.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,37 +3,50 @@
 
 from message_ix import ModelError, Scenario
 from message_ix.testing import make_subannual
 
 
 def check_solution(scen: Scenario) -> None:
     """Perform several assertions about the solution of `scen`."""
-    # Reading "ACT" and "CAP" from the solution
+    # Reading "ACT" and "CAP" from the solution, plus "operation_factor"
     act = scen.var("ACT").set_index(["technology", "time"])
     cap = scen.var("CAP").set_index(["technology"])
+    op_fac = scen.par("operation_factor").set_index(["technology"])
 
-    # 1) ACT is zero when capacity factor is zero
+    # 1) ACT is zero when capacity factor (CF) is zero
     cf = scen.par("capacity_factor").set_index(["technology", "time"])
     cf_zero = cf.loc[cf["value"] == 0]
     for i in cf_zero.index:
         assert act.loc[i, "lvl"] == 0
 
-    # 2) CAP is correctly calculated based on ACT and capacity_factor
-    for i in act.loc[act["lvl"] > 0].index:
-        # Correct ACT based on duration of each time slice
+    # 2) CAP is correctly calculated based on "ACT", CF, and "operation_factor"
+    for i in act.index:
+        # Correct CF based on duration of each time slice
         duration = float(scen.par("duration_time", {"time": i[1]})["value"])
-        act.loc[i, "duration-corrected"] = act.loc[i, "lvl"] / duration
-        # Divide by (non-zero) capacity factor
-        act.loc[i, "cf-corrected"] = act.loc[i, "duration-corrected"] / float(
-            cf.loc[i, "value"]
-        )
+        if i[1] != "year":
+            cf.loc[i, "duration-corrected"] = cf.loc[i, "value"] * duration
+            if cf.loc[i, "value"] == 0 or duration == 0:
+                act.loc[i, "cf-corrected"] = act.loc[i, "lvl"]
+            else:
+                act.loc[i, "cf-corrected"] = act.loc[i, "lvl"] / float(
+                    cf.loc[i, "duration-corrected"]
+                )
     act = act.fillna(0).reset_index().set_index(["technology"])
-    # CAP = max("ACT" / "duration_time" / "capcity_factor")
+    # CAP = max("ACT" / "duration_time" / "capacity_factor") / "operation_factor"
     for i in cap.index:
-        assert max(act.loc[i, "cf-corrected"]) == float(cap.loc[i, "lvl"])
+        # Considering operation factor (if specified)
+        if not op_fac.empty:
+            # Weighted average CF for "year" (for calculating "operation_factor")
+            cf_year = sum(cf["duration-corrected"])
+            # Capacity is related to "operation_factor", when defined, and yearly CF
+            assert sum(act.loc[i, "lvl"]) == round(
+                float(cap.loc[i, "lvl"]) * float(op_fac.loc[i, "value"]) * cf_year, 6
+            )
+        else:
+            assert max(act.loc[i, "cf-corrected"]) == float(cap.loc[i, "lvl"])
 
 
 # Dictionary of technology input/output
 TD_0 = {
     "gas_ppl": {
         "time_origin": [],
         "time": ["summer", "winter"],
@@ -152,7 +165,26 @@
         },
         var_cost={
             "solar_pv_ppl": {"day": 0, "night": 0},
             "gas_ppl": {"day": 0.2, "night": 0.2},
         },
     )
     check_solution(scen)
+
+
+def test_capacity_factor_average(request):
+    """Weighted average of ``capacity_factor`` for "year" is calculated correctly,
+    based on time slices, when there is no capacity factor defined for "year"."""
+    # Build model and solve
+    scen = make_subannual(
+        request,
+        TD_0,
+        time_steps=[
+            ("summer", 0.5, "season", "year"),
+            ("winter", 0.5, "season", "year"),
+        ],
+        demand={"summer": 2, "winter": 1},
+        capacity_factor={"gas_ppl": {"summer": 0.8, "winter": 0.6}},
+        var_cost={"gas_ppl": {"summer": 0.2, "winter": 0.2}},
+        operation_factor={"gas_ppl": 0.8},
+    )
+    check_solution(scen)
```

### Comparing `message_ix-3.6.0/message_ix/tests/test_feature_duration_time.py` & `message_ix-3.7.0/message_ix/tests/test_feature_duration_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         # If technology is linking two different temporal levels
         if tmp_lvl_in != tmp_lvl_out:
             time_pairs = product(times_in, times_out)
         else:
             time_pairs = zip(times_in, times_out)
 
         # Configuring data for "time_origin" and "time" in "input"
-        for (h_in, h_act) in time_pairs:
+        for h_in, h_act in time_pairs:
             # "input"
             inp = com_dict[tec]["input"]
             if inp:
                 inp_spec = [yr, yr, "standard", "fairyland", inp, "final", h_act, h_in]
                 scen.add_par("input", ["fairyland", tec] + inp_spec, 1, "-")
         # "output"
         for h in times_out:
@@ -145,14 +145,15 @@
 
 
 # Tests for "duration_time" of different numbers of time slices, at different
 # temporal levels ("lvl_temporal")
 # In these tests "demand" is defined in different time slices and one power plant
 # to meet demand, which receives fuel from a supply technology.
 
+
 # Testing one temporal level ("season") and different number of time slices
 def test_season(test_mp, n_time=[4, 12, 50]):
     comment = "season"
     com_dict = {"power-plant": {"input": [], "output": "electr"}}
     tec_time = {"power-plant": ["season", "season"]}
     demand_time = {"season": 100}
```

### Comparing `message_ix-3.6.0/message_ix/tests/test_feature_price_commodity.py` & `message_ix-3.7.0/message_ix/tests/test_feature_price_commodity.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_feature_price_emission.py` & `message_ix-3.7.0/message_ix/tests/test_feature_price_emission.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_feature_storage.py` & `message_ix-3.7.0/message_ix/tests/test_feature_storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-# -*- coding: utf-8 -*-
-"""
-This is a unit test for representing storage in the MESSAGEix model, and
-testing the functionality of storage equations. The workflow is as follows:
-    - building a stylized MESSAGEix model
-    - adding seasonality and modifying parameters for timesteps accordingly
-    - adding storage implementation (dam: storage device, pump: charger,
-                                     turbine: discharger)
-    - testing storage functionality and equations
+"""Test storage representation.
 
-"""
+This is a unit test for representing storage in the MESSAGEix model, and testing the
+functionality of storage equations. The workflow is as follows:
 
+- Build a stylized MESSAGEix model.
+- Add seasonality and modify parameters for timesteps accordingly.
+- Add storage implementation (dam: storage device, pump: charger, turbine: discharger).
+- Test storage functionality and equations.
+"""
+import logging
 from itertools import product
 
+import pandas as pd
+import pytest
+from ixmp.testing import assert_logs
+
 from message_ix import Scenario
+from message_ix.models import MESSAGE
+from message_ix.testing import make_dantzig
+from message_ix.util import expand_dims
 
 
 # A function for generating a simple MESSAGEix model with two technologies
 def model_setup(scen, years):
     scen.add_set("node", "node")
     scen.add_set("commodity", "electr")
     scen.add_set("level", "level")
     scen.add_set("year", years)
     scen.add_set("type_year", years)
     scen.add_set("technology", ["wind_ppl", "gas_ppl"])
-    scen.add_set("mode", "mode")
+    scen.add_set("mode", "M1")
     output_specs = ["node", "electr", "level", "year", "year"]
     # Two technologies, one cheaper than the other
     var_cost = {"wind_ppl": 0, "gas_ppl": 2}
     for year, (tec, cost) in product(years, var_cost.items()):
         scen.add_par("demand", ["node", "electr", "level", year, "year"], 1, "GWa")
-        tec_specs = ["node", tec, year, year, "mode"]
+        tec_specs = ["node", tec, year, year, "M1"]
         scen.add_par("output", tec_specs + output_specs, 1, "GWa")
         scen.add_par("var_cost", tec_specs + ["year"], cost, "USD/GWa")
 
 
 # A function for adding sub-annual time steps to a MESSAGEix model
 def add_seasonality(scen, time_duration):
     scen.add_set("time", sorted(list(set(time_duration.keys()))))
@@ -71,15 +77,18 @@
     scen.add_set("storage_tec", "dam")
 
     # Specifying storage level
     scen.add_set("level_storage", "storage")
 
     # Adding mapping for storage and charger/discharger technologies
     for tec in ["pump", "turbine"]:
-        scen.add_set("map_tec_storage", ["node", tec, "dam", "storage", "water"])
+        scen.add_set(
+            "map_tec_storage",
+            ["node", tec, "M1", "dam", "M1", "storage", "water", "season"],
+        )
 
     # Adding time sequence
     for h in time_order.keys():
         scen.add_par("time_order", ["season", h], time_order[h], "-")
 
     # Adding input, output, and capacity factor for storage technologies
     output_spec = {
@@ -93,32 +102,31 @@
         "pump": ["node", "electr", "level"],
         "turbine": ["node", "water", "storage"],
     }
 
     var_cost = {"dam": 0, "pump": 0.2, "turbine": 0.3}
     stor_tecs = ["dam", "pump", "turbine"]
     for year, h, tec in product(set(scen.set("year")), time_order.keys(), stor_tecs):
-        tec_sp = ["node", tec, year, year, "mode"]
+        tec_sp = ["node", tec, year, year, "M1"]
         scen.add_par("output", tec_sp + output_spec[tec] + [h, h], 1, "GWa")
         scen.add_par("input", tec_sp + input_spec[tec] + [h, h], 1, "GWa")
         scen.add_par("var_cost", tec_sp + [h], var_cost[tec], "USD/GWa")
 
     # Adding storage self-discharge (as %) and initial content
     for year, h in product(set(scen.set("year")), time_order.keys()):
-        storage_spec = ["node", "dam", "storage", "water", year, h]
+        storage_spec = ["node", "dam", "M1", "storage", "water", year, h]
         scen.add_par("storage_self_discharge", storage_spec, 0.05, "%")
 
         # Adding initial content of storage (optional)
-        storage_spec = ["node", "dam", "storage", "water", year, "a"]
-        scen.add_par("storage_initial", storage_spec, 0.08, "GWa")
+        storage_spec = ["node", "dam", "M1", "storage", "water", year, "a"]
+        scen.add_par("storage_initial", storage_spec, 0.5, "%")
 
 
 # Main function for building a model with storage and testing the functionality
 def storage_setup(test_mp, time_duration, comment):
-
     # First, building a simple model and adding seasonality
     scen = Scenario(test_mp, "no_storage", "standard", version="new")
     model_setup(scen, [2020])
     add_seasonality(scen, time_duration)
     # Fixed share for parameters that don't change across timesteps
     fixed_share = {"a": 1, "b": 1, "c": 1, "d": 1}
     year_to_time(scen, "output", fixed_share)
@@ -131,15 +139,15 @@
     scen.solve(case="no_storage" + comment, quiet=True)
 
     # Second, adding upper bound on activity of the cheap technology (wind_ppl)
     scen.remove_solution()
     scen.check_out()
     for h in time_duration.keys():
         scen.add_par(
-            "bound_activity_up", ["node", "wind_ppl", 2020, "mode", h], 0.25, "GWa"
+            "bound_activity_up", ["node", "wind_ppl", 2020, "M1", h], 0.25, "GWa"
         )
     scen.commit("activity bounded")
     scen.solve(case="no_storage_bounded" + comment, quiet=True)
     cost_no_stor = scen.var("OBJ")["lvl"]
     act_no_stor = scen.var("ACT", {"technology": "gas_ppl"})["lvl"].sum()
 
     # Third, adding storage technologies but with no input to storage device
@@ -162,33 +170,36 @@
     df["commodity"] = "cooling"
     scen.add_par("output", df)
     # Changing input of dam from 1 to 1.2 to test commodity balance
     df = scen.par("input", {"technology": "dam"})
     df["value"] = 1.2
     scen.add_par("input", df)
     scen.commit("storage needs no separate input")
-    scen.solve(case="with_storage_and_input" + comment, quiet=True)
+    scen.solve(
+        case="with_storage_and_input" + comment,
+        quiet=True,
+        var_list=["STORAGE", "STORAGE_CHARGE"],
+    )
     cost_with_stor = scen.var("OBJ")["lvl"]
     act_with_stor = scen.var("ACT", {"technology": "gas_ppl"})["lvl"].sum()
 
     # Fifth. Tests for the functionality of storage
     # 1. Check that "dam" is not active if no "input" commodity is defined
     assert "dam" not in act[act["lvl"] > 0]["technology"].tolist()
 
     # 2. Testing functionality of storage
     # Check the contribution of storage to the system cost
     assert cost_with_stor < cost_no_stor
     # Activity of expensive technology should be lower with storage
     assert act_with_stor < act_no_stor
 
-    # 3. Activity of discharger <= activity of charger + initial content
+    # 3. Activity of discharger <= activity of charger
     act_pump = scen.var("ACT", {"technology": "pump"})["lvl"]
     act_turb = scen.var("ACT", {"technology": "turbine"})["lvl"]
-    initial_content = float(scen.par("storage_initial")["value"])
-    assert act_turb.sum() <= act_pump.sum() + initial_content
+    assert act_turb.sum() <= act_pump.sum()
 
     # 4. Activity of input provider to storage = act of storage * storage input
     for ts in time_duration.keys():
         act_cooler = scen.var("ACT", {"technology": "cooler", "time": ts})["lvl"]
         inp = scen.par("input", {"technology": "dam", "time": ts})["value"]
         act_stor = scen.var("ACT", {"technology": "dam", "time": ts})["lvl"]
         assert float(act_cooler) == float(inp) * float(act_stor)
@@ -201,30 +212,29 @@
 
     # 6. Max activity of discharger <= max storage act - self discharge losses
     max_turb = max(act_turb)
     loss = scen.par("storage_self_discharge")["value"][0]
     assert max_turb <= max_stor * (1 - loss)
 
     # Sixth, testing equations of storage (when added to ixmp variables)
-    if scen.has_var("STORAGE"):
-        # 1. Equality: storage content in the beginning and end is related
-        storage_first = scen.var("STORAGE", {"time": "a"})["lvl"]
-        storage_last = scen.var("STORAGE", {"time": "d"})["lvl"]
-        relation = scen.par("relation_storage", {"time_first": "d", "time_last": "a"})[
-            "value"
-        ][0]
-        assert storage_last >= storage_first * relation
+    if scen.has_var("STORAGE") and not scen.var("STORAGE").empty:
+        # 1. Equality: storage content at the end is equal to the beginning
+        # (i.e., the difference is what is pumped in the first time slice)
+        storage_first = float(scen.var("STORAGE", {"time": "a"})["lvl"])
+        storage_last = float(scen.var("STORAGE", {"time": "d"})["lvl"])
+        pump_first = float(scen.var("ACT", {"technology": "pump", "time": "a"})["lvl"])
+        assert storage_last == storage_first - pump_first
 
         # 2. Storage content should never exceed storage activity
         assert max(scen.var("STORAGE")["lvl"]) <= max_stor
 
         # 3. Commodity balance: charge - discharge - losses = 0
-        change = scen.var("STORAGE_CHARGE").set_index(["year_act", "time"])["lvl"]
+        change = scen.var("STORAGE_CHARGE").set_index(["year", "time"])["lvl"]
         loss = scen.par("storage_self_discharge").set_index(["year", "time"])["value"]
-        assert sum(change[change > 0] * (1 - loss)) == -sum(change[change < 0])
+        assert (change[change > 0] * (1 - loss)).sum() >= -(change[change < 0]).sum()
 
         # 4. Energy balance: storage change + losses = storage content
         storage = scen.var("STORAGE").set_index(["year", "time"])["lvl"]
         assert storage[(2020, "b")] * (1 - loss[(2020, "b")]) == -change[(2020, "c")]
 
 
 # Storage test for different duration times
@@ -234,7 +244,68 @@
 
     """
     time_duration = {"a": 0.25, "b": 0.25, "c": 0.25, "d": 0.25}
     storage_setup(test_mp, time_duration, "_equal_time")
 
     time_duration = {"a": 0.3, "b": 0.25, "c": 0.25, "d": 0.2}
     storage_setup(test_mp, time_duration, "_unequal_time")
+
+
+def test_structure(caplog, test_mp):
+    """:meth:`MESSAGE.initialize` and :meth:`MESSAGE.enforce` handle old structure."""
+    scen = make_dantzig(test_mp)
+
+    # Item name to use for the tests, a parameter, and its dimensions
+    name = "storage_initial"
+    dims = ["node", "technology", "level", "commodity", "year", "time"]
+    # NB here we cannot use make_df, since that refers to the current dimensionality of
+    #    storage_initial per MESSAGE_ITEMS
+    data = pd.Series(
+        ["topeka", "canning_plant", "supply", "cases", 1963, "year", 1.0, "kg"],
+        index=dims + ["value", "unit"],
+    )
+
+    def prepare(s, with_data=False):
+        """Re-initialize to the former definition, i.e. omitting mode."""
+        with scen.transact():
+            scen.remove_par(name)
+            scen.init_par(name, idx_sets=dims)
+            if with_data:
+                scen.add_par(name, data.to_frame().transpose())
+
+    # Test by calling the MESSAGE model class methods directory. This is not the typical
+    # user behaviour; we just want to avoid a more complex way of doing so.
+
+    # Calling initialize() with no data automatically expands the dimensions
+    prepare(scen)
+    assert "mode" not in scen.idx_sets(name)
+
+    with scen.transact():
+        MESSAGE.initialize(scen)
+
+    assert "mode" in scen.idx_sets(name)
+    # …and enforce() completes without raising an exception
+    MESSAGE.enforce(scen)
+
+    # Now with data in storage_initial, a warning is raised
+    prepare(scen, with_data=True)
+
+    # Two context managers for the with: block
+    c1 = pytest.warns(UserWarning, match="'storage_initial' has data with dimensions")
+    c2 = assert_logs(caplog, "Existing index sets of 'stora", at_level=logging.WARNING)
+    with c1, c2:
+        with scen.transact():
+            MESSAGE.initialize(scen)
+
+    # …the dimensions are *not* expanded automatically
+    assert "mode" not in scen.idx_sets(name)
+
+    # …and the scenario would not solve
+    with pytest.raises(ValueError, match="'storage_initial' has data with dimensions"):
+        MESSAGE.enforce(scen)
+
+    # expand_dims() results in the correct dimensionality and complete data
+    expand_dims(scen, name, mode="production")
+    assert "mode" in scen.idx_sets(name)
+
+    # …and enforce() completes without raising an exception
+    MESSAGE.enforce(scen)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `message_ix-3.6.0/message_ix/tests/test_feature_temporal_level.py` & `message_ix-3.7.0/message_ix/tests/test_feature_temporal_level.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_feature_vintage_and_active_years.py` & `message_ix-3.7.0/message_ix/tests/test_feature_vintage_and_active_years.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_integration.py` & `message_ix-3.7.0/message_ix/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_legacy_version.py` & `message_ix-3.7.0/message_ix/tests/test_legacy_version.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_macro.py` & `message_ix-3.7.0/message_ix/tests/test_macro.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 
 # Test for selecting desirable years specified in config from the Excel input
 def test_calc_valid_years(westeros_solved):
     s = westeros_solved
     data = pd.read_excel(W_DATA_PATH, sheet_name=None, engine="openpyxl")
     # Adding an arbitrary year
     arbitrary_yr = 2021
-    gdp_extra_yr = data["gdp_calibrate"].iloc[0, :].copy()
+    gdp_extra_yr = data["gdp_calibrate"].copy()
     gdp_extra_yr["year"] = arbitrary_yr
-    data["gdp_calibrate"] = data["gdp_calibrate"].append(gdp_extra_yr)
+    data["gdp_calibrate"] = pd.concat([data["gdp_calibrate"], gdp_extra_yr])
     # Check the arbitrary year is not in config
     assert arbitrary_yr not in data["config"]["year"]
     # But it is in gdp_calibrate
     assert arbitrary_yr in set(data["gdp_calibrate"]["year"])
     # And macro does calibration without error
     c = macro.Calculate(s, data)
     c.read_data()
@@ -160,15 +160,15 @@
         ("_growth", "allclose", [0.02658363, 0.04137974, 0.04137974, 0.02918601]),
         ("_rho", "equal", [-4.0]),
         ("_gdp0", "equal", [500.0]),
         ("_k0", "equal", [1500.0]),
         (
             "_total_cost",
             "allclose",
-            1e-3 * np.array([6.18242, 8.6601720, 13.4040172, 14.9067117]),
+            np.array([6.18242, 8.6601720, 13.4040172, 14.9067117]),
         ),
         ("_price", "allclose", [211, 511.0282933, 162.0395393, 161.0026274]),
         ("_demand", "allclose", [27, 55, 82, 104]),
         ("_bconst", "allclose", [9.68838201e-08]),
         ("_aconst", "allclose", [26.027323]),
     ),
 )
@@ -268,26 +268,26 @@
 
 def test_calibrate_roundtrip(westeros_solved):
     # this is a regression test with values observed on Aug 9, 2019
     with_macro = westeros_solved.add_macro(W_DATA_PATH, check_convergence=True)
     aeei = with_macro.par("aeei")["value"].values
     npt.assert_allclose(
         aeei,
-        1e-3 * np.array([20, -7.5142661, 43.6256127, 21.14346]),
+        1e-3 * np.array([20, -7.53474955303437, 43.6388021078658, 21.1470758210961]),
     )
     grow = with_macro.par("grow")["value"].values
     npt.assert_allclose(
         grow,
         1e-3
         * np.array(
             [
-                26.5836313,
-                69.1417537,
-                79.1435885,
-                24.5225555,
+                26.583631304232,
+                69.1441230700944,
+                79.1406795348988,
+                24.5225816398262,
             ]
         ),
     )
 
 
 #
 # These are a series of tests to guarantee multiregion/multisector
```

### Comparing `message_ix-3.6.0/message_ix/tests/test_models.py` & `message_ix-3.7.0/message_ix/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_nightly.py` & `message_ix-3.7.0/message_ix/tests/test_nightly.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_reporting.py` & `message_ix-3.7.0/message_ix/tests/test_reporting.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # IXMPReporter can be initialized on a MESSAGE Scenario
     rep_ix = ixmp_Reporter.from_scenario(scen)
 
     # message_ix.Reporter can also be initialized
     rep = Reporter.from_scenario(scen)
 
     # Number of quantities available in a rudimentary MESSAGEix Scenario
-    assert len(rep.graph["all"]) == 123
+    assert len(rep.graph["all"]) == 125
 
     # Quantities have short dimension names
     assert "demand:n-c-l-y-h" in rep
 
     # Aggregates are available
     assert "demand:n-l-h" in rep
 
@@ -65,19 +65,19 @@
 
     # NB the call to squeeze() drops the length-1 dimensions c-l-y-h
     obs = rep.get("demand:n-c-l-y-h").squeeze(drop=True)
     # check_attrs False because we don't get the unit addition in bare xarray
     assert_qty_equal(obs, demand, check_attrs=False)
 
     # ixmp.Reporter pre-populated with only model quantities and aggregates
-    assert len(rep_ix.graph) == 5225
+    assert len(rep_ix.graph) == 5609
 
     # message_ix.Reporter pre-populated with additional, derived quantities
     # This is the same value as in test_tutorials.py
-    assert len(rep.graph) == 12690
+    assert len(rep.graph) == 13074
 
     # Derived quantities have expected dimensions
     vom_key = rep.full_key("vom")
     assert vom_key not in rep_ix
     assert vom_key == "vom:nl-t-yv-ya-m-h"
 
     # …and expected values
```

### Comparing `message_ix-3.6.0/message_ix/tests/test_soft_constraints.py` & `message_ix-3.7.0/message_ix/tests/test_soft_constraints.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/test_util.py` & `message_ix-3.7.0/message_ix/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/tools/test_add_year.py` & `message_ix-3.7.0/message_ix/tests/tools/test_add_year.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     scen.add_set("commodity", "comm")
     scen.add_set("level", "level")
     scen.add_set("year", years)
     scen.add_set("technology", "tec")
     scen.add_set("mode", "mode")
     output_specs = ["node", "comm", "level", "year", "year"]
 
-    for (yr, value) in data.items():
+    for yr, value in data.items():
         scen.add_par("demand", ["node", "comm", "level", yr, "year"], 1, "GWa")
         scen.add_par("technical_lifetime", ["node", "tec", yr], 10, "y")
         tec_specs = ["node", "tec", yr, yr, "mode"]
         scen.add_par("output", tec_specs + output_specs, 1, "-")
         scen.add_par("var_cost", tec_specs + ["year"], value, "USD/GWa")
 
     scen.commit("initialize test model")
```

### Comparing `message_ix-3.6.0/message_ix/tests/util/test_sphinx_gams.py` & `message_ix-3.7.0/message_ix/tests/util/test_sphinx_gams.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tests/util/test_tutorial.py` & `message_ix-3.7.0/message_ix/tests/util/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tools/add_year/README.rst` & `message_ix-3.7.0/message_ix/tools/add_year/README.rst`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/tools/add_year/__init__.py` & `message_ix-3.7.0/message_ix/tools/add_year/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,18 @@
             ].mode()[0]
     else:
         df["unit"] = df["unit"].mode()[0]
     return df
 
 
 # %% III) The main function
-def add_year(
+
+
+# FIXME reduce complexity from 17 to <=14
+def add_year(  # noqa: C901
     sc_ref,
     sc_new,
     years_new,
     firstyear_new=None,
     lastyear_new=None,
     macro=False,
     baseyear_macro=None,
@@ -316,16 +319,17 @@
 
     yr_pair = []
     for yr in years_new:
         yr_pair.append([yr, yr])
         yr_pair.append(["cumulative", yr])
 
     yr_cat = (
-        yr_cat.append(
-            pd.DataFrame(yr_pair, columns=["type_year", "year"]), ignore_index=True
+        pd.concat(
+            [yr_cat, pd.DataFrame(yr_pair, columns=["type_year", "year"])],
+            ignore_index=True,
         )
         .sort_values("year")
         .reset_index(drop=True)
     )
 
     # A.6. Changing the cumulative years based on the new first model year
     if "firstmodelyear" in set(yr_cat["type_year"]):
@@ -526,15 +530,18 @@
         )
         sc_new.add_par(parname, df_y)
         sc_new.commit(parname)
         log.info(f"Parameter {parname} copied and new years added for node(s): {nodes}")
 
 
 # %% VI) Required functions
-def interpolate_1d(
+
+
+# FIXME reduce complexity from 19 to <=14
+def interpolate_1d(  # noqa: C901
     df,
     yrs_new,
     horizon,
     year_col,
     value_col="value",
     extrapolate=False,
     extrapol_neg=None,
@@ -678,17 +685,18 @@
     else:
         log.warning("The submitted dataframe is empty, so returned empty results")
         df2 = df
     return df2
 
 
 # %% VI.B) Interpolating parameters with two dimensions related to time
-# TODO this is the most complex piece of code in the message_ix, at a McCabe
-#      complexity of 38 (next nearest: 18). Simplify.
-def interpolate_2d(
+
+
+# FIXME reduce complexity from 38 to <=14
+def interpolate_2d(  # noqa: C901
     df,
     yrs_new,
     horizon,
     year_ref,
     year_col,
     tec_list,
     par_tec,
@@ -811,15 +819,14 @@
 
             df2[yr] = intpol(df2[year_pre], df2[year_pp], year_pre, year_pp, yr)
             df2[yr][np.isinf(df2[year_pre].shift(+1))] = df2[year_pre].shift(+1)
             df2[yr] = df2[yr].fillna(df2[year_pre])
 
             j = horizon_new.index(yr)
             if yr - horizon_new[j - 1] >= horizon_new[j - 1] - horizon_new[j - 2]:
-
                 df2[yr].loc[
                     (pd.isna(df2[year_pre].shift(+1)))
                     & (~pd.isna(df2[year_pp].shift(+1)))
                 ] = np.nan
             cond = (df2[yr] < 0) & (df2[year_pre].shift(+1) >= 0)
             if not df2[yr].loc[cond].empty and extrapol_neg:
                 df2.loc[cond, yr] = df2.loc[cond, year_pre] * extrapol_neg
@@ -928,20 +935,19 @@
                         mask_df(df_yr, i, df_count["c_pre"][i] + 1, np.nan)
                     else:
                         mask_df(df_yr, i, df_count["c_pre"][i], np.nan)
 
         else:
             continue
 
-        df2 = df2.append(df_yr)
+        df2 = pd.concat([df2, df_yr])
         df2 = df2.reindex(sorted(df2.columns), axis=1).sort_index()
     # -------------------------------------------------------------------------
     # Forth: final masking based on technical lifetime
     if tec_list and not df_dur.empty:
-
         df3 = (
             df2.loc[df2.index.get_level_values("technology").isin(tec_list), :]
             .copy()
             .dropna(how="all")
         )
         idx_list = list(set(df3.index.get_level_values(year_ref)))
         for y in sorted([x for x in idx_list if x in df_dur.index]):
```

### Comparing `message_ix-3.6.0/message_ix/tools/add_year/cli.py` & `message_ix-3.7.0/message_ix/tools/add_year/cli.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix/util/__init__.py` & `message_ix-3.7.0/message_ix/util/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import warnings
 from collections import ChainMap, defaultdict
 from collections.abc import Mapping
 
 import pandas as pd
 from pandas.api.types import is_scalar
 
+from message_ix.core import Scenario
 from message_ix.macro import MACRO_ITEMS
-from message_ix.models import MESSAGE_ITEMS
+from message_ix.models import MESSAGE, MESSAGE_ITEMS
 
 
 def make_df(name, **data):
     """Return a data frame for parameter `name` filled with `data`.
 
     :func:`make_df` always returns a data frame with the columns required by
     :meth:`.add_par`: the dimensions of the parameter `name`, plus 'value' and
@@ -98,14 +99,16 @@
 
     Raises
     ------
     ValueError
         if `name` is not the name of a MESSAGE or MACRO parameter; if arrays in `data`
         have uneven lengths.
     """
+    # NB could be expanded to handle "mapping sets"
+
     if isinstance(name, (Mapping, pd.Series, pd.DataFrame)):
         return _deprecated_make_df(name, **data)
 
     # Get parameter information
     try:
         info = ChainMap(MESSAGE_ITEMS, MACRO_ITEMS)[name]
     except KeyError:
@@ -185,7 +188,47 @@
     )
 
     base = copy.deepcopy(base)
     if not isinstance(base, Mapping):
         base = base.to_dict()
     base.update(**kwargs)
     return pd.DataFrame(base)
+
+
+def expand_dims(scenario: Scenario, name, **data):
+    """Expand dimensions of parameter `name` on `scenario`, filling with `data`.
+
+    This function is for use when an existing parameter `name` has dimensions that are a
+    subset of those that would be created by :func:`make_df`, i.e. those given by
+    :data:`.MESSAGE_ITEMS`.
+
+    This can occur when the underlying structure of MESSAGE and the model core is
+    enhanced by adding dimensions to existing parameters. Existing scenario data in
+    users' databases can not then be automatically updated.
+
+    :func:`expand_dims` helps users to update this data manually. It:
+
+    1. Retrieves the existing parameter data for `name`.
+    2. Passes this existing data, plus any `data` given as keyword arguments, to
+       :func:`make_df`. The result must be a data frame with no empty values; in other
+       words, `data` must include all the dimensions to be added to `name`.
+    3. Re-initializes the parameter `name` on `scenario`, with the dimensions given by
+       :data:`.MESSAGE_ITEMS`.
+    4. Adds the expanded data.
+
+    The modifications (steps 3 and 4) are wrapped using :meth:`.transact`.
+    """
+    # NB could be improved by allowing `data` to include callables; these would be
+    #    pd.DataFrame.apply(…)'d to each row in order to compute values for the new
+    #    dimension(s).
+
+    # Create the expanded data
+    new_data = make_df(name, **scenario.par(name), **data)
+    assert not new_data.isna().any(axis=None), "Expanded data are incomplete"
+
+    with scenario.transact(f"expand_dims({name}, …)"):
+        # Remove the parameter entirely, and re-initialize
+        scenario.remove_par(name)
+        MESSAGE.initialize_items(scenario, {name: MESSAGE_ITEMS[name]})
+
+        # Add the expanded data
+        scenario.add_par(name, new_data)
```

### Comparing `message_ix-3.6.0/message_ix/util/sphinx_gams.py` & `message_ix-3.7.0/message_ix/util/sphinx_gams.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Sphinx extension for extracting inline documentation from GAMS source files."""
 
 from os import PathLike
 from pathlib import Path
 
-from sphinx.util import status_iterator
+try:
+    from sphinx.util.display import status_iterator
+except ImportError:  # Sphinx < 6.1
+    # TODO remove this clause once message_ix requires Sphinx >= 6.1
+    from sphinx.util import status_iterator  # type: ignore
 
 
 def files(src_dir, target_dir, match="*.gms", ext=".rst"):
     """Return files in *src_dir* matching *match*.
 
     Two lists are returned; the second contains file names in *target_dir* with
     the replacement *ext*.
```

### Comparing `message_ix-3.6.0/message_ix/util/tutorial.py` & `message_ix-3.7.0/message_ix/util/tutorial.py`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/message_ix.egg-info/PKG-INFO` & `message_ix-3.7.0/message_ix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: message-ix
-Version: 3.6.0
-Summary: the MESSAGEix integrated assessment model
-Home-page: http://github.com/iiasa/message_ix
+Version: 3.7.0
+Summary: The MESSAGEix integrated assessment model framework
 Author: IIASA Energy, Climate, and Environment (ECE) Program
-Author-email: message_ix@iiasa.ac.at
-License: Apache
-Project-URL: Documentation, https://docs.messageix.org/
+Maintainer-email: Paul Natsuo Kishimoto <mail@paul.kishimoto.name>, Fridolin Glatter <glatter@iiasa.ac.at>
+Project-URL: homepage, https://github.com/iiasa/message_ix
+Project-URL: repository, https://github.com/iiasa/message_ix
+Project-URL: documentation, https://docs.messageix.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -19,17 +19,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: R
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
-Provides-Extra: report
 Provides-Extra: docs
 Provides-Extra: tutorial
+Provides-Extra: report
 Provides-Extra: tests
 License-File: LICENSE
 License-File: NOTICE.rst
 License-File: AUTHORS.md
 
 # The MESSAGEix framework
 
@@ -75,13 +75,13 @@
 - Documentation for the ‘latest’ or ‘stable’ release is shown by default.
 - Use the chooser to access the [‘latest’ version](https://docs.messageix.org/en/latest/), corresponding to the ``main`` branch and including the latest development code; or to access docs for a specific release, e.g. `v3.2.0`.
 - For offline use, the documentation can be built from the source code.
   See the file [`doc/README.rst`](doc/README.rst)
 
 ## License
 
-Copyright © 2018–2022 IIASA Energy, Climate, and Environment (ECE) Program
+Copyright © 2018–2023 IIASA Energy, Climate, and Environment (ECE) Program
 
 The MESSAGEix framework is licensed under the Apache License, Version 2.0 (the "License"); you may not use the files in this repository except in compliance with the License. You may obtain a copy of the License in [`LICENSE`](LICENSE) or at <http://www.apache.org/licenses/LICENSE-2.0>.
 
 In addition and per good scientific practice, you **must** cite the appropriate publications when you use MESSAGEix in scientific work.
 Again, see [‘User guidelines and notice’](https://docs.messageix.org/en/stable/notice.html) or the file [`NOTICE.rst`](NOTICE.rst).
```

### Comparing `message_ix-3.6.0/message_ix.egg-info/SOURCES.txt` & `message_ix-3.7.0/message_ix.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 AUTHORS.md
+CITATION.cff
 CONTRIBUTOR_LICENSE.rst
 Dockerfile
 INSTALL.rst
 LICENSE
 MANIFEST.in
 NOTICE.rst
 README.md
 RELEASE_NOTES.rst
 conftest.py
 pyproject.toml
-setup.cfg
-setup.py
 doc/Makefile
 doc/README.rst
 doc/api.rst
 doc/bibliography.rst
 doc/conf.py
 doc/contributing.rst
 doc/debugging.rst
@@ -43,14 +42,15 @@
 doc/_static/messageix-community-logo-white.svg
 doc/_static/messageix-community-logo.svg
 doc/_static/messageix-favicon.svg
 doc/_static/messageix-logo-white.svg
 doc/_static/messageix-logo.svg
 doc/_static/storage.png
 doc/_static/usage_figures/1-s2.0-S2210670721005333-gr19_lrg.jpg
+doc/_static/usage_figures/10.1016-j.est.2022.104587.JPG
 doc/_static/usage_figures/10.1016-j.scs.2021.103257.jpg
 doc/_static/usage_figures/10.1038-s41560-018-0172-6.webp
 doc/_static/usage_figures/10.1038-s41560-018-0179-z.webp
 doc/_static/usage_figures/10.3390-en12081483.png
 doc/_static/usage_figures/41560_2021_904.webp
 doc/contrib/cla.rst
 doc/contrib/release.rst
@@ -68,15 +68,14 @@
 message_ix/utils.py
 message_ix.egg-info/PKG-INFO
 message_ix.egg-info/SOURCES.txt
 message_ix.egg-info/dependency_links.txt
 message_ix.egg-info/entry_points.txt
 message_ix.egg-info/requires.txt
 message_ix.egg-info/top_level.txt
-message_ix.egg-info/zip-safe
 message_ix/model/MACRO_run.gms
 message_ix/model/MESSAGE-MACRO_run.gms
 message_ix/model/MESSAGE_master.gms
 message_ix/model/MESSAGE_project.gpr
 message_ix/model/MESSAGE_run.gms
 message_ix/model/conopt.opt
 message_ix/model/version.gms
@@ -105,14 +104,15 @@
 message_ix/reporting/pyam.py
 message_ix/testing/__init__.py
 message_ix/testing/nightly.py
 message_ix/tests/__init__.py
 message_ix/tests/conftest.py
 message_ix/tests/test_cli.py
 message_ix/tests/test_core.py
+message_ix/tests/test_equation_NEW_CAPACITY_CONTRAINT.py
 message_ix/tests/test_feature_addon.py
 message_ix/tests/test_feature_bound_activity_shares.py
 message_ix/tests/test_feature_bound_emission.py
 message_ix/tests/test_feature_capacity_factor.py
 message_ix/tests/test_feature_duration_time.py
 message_ix/tests/test_feature_price_commodity.py
 message_ix/tests/test_feature_price_emission.py
@@ -169,31 +169,35 @@
 tutorial/westeros/westeros_baseline_using_xlsx_import_part2.ipynb
 tutorial/westeros/westeros_emissions_bounds.ipynb
 tutorial/westeros/westeros_emissions_taxes.ipynb
 tutorial/westeros/westeros_firm_capacity.ipynb
 tutorial/westeros/westeros_flexible_generation.ipynb
 tutorial/westeros/westeros_fossil_resource.ipynb
 tutorial/westeros/westeros_historical_new_capacity.ipynb
+tutorial/westeros/westeros_multinode.ipynb
 tutorial/westeros/westeros_renewable_resource.ipynb
 tutorial/westeros/westeros_report.ipynb
 tutorial/westeros/westeros_seasonality.ipynb
 tutorial/westeros/westeros_share_constraint.ipynb
 tutorial/westeros/westeros_soft_constraints.ipynb
 tutorial/westeros/_static/addon_technologies_res.png
 tutorial/westeros/_static/baseline_res.png
+tutorial/westeros/_static/bilateral.JPG
 tutorial/westeros/_static/cf_wind.png
 tutorial/westeros/_static/doc_page.png
+tutorial/westeros/_static/external.JPG
 tutorial/westeros/_static/firm-capacity.png
 tutorial/westeros/_static/firm-capacity.pptx
 tutorial/westeros/_static/fossil_resource_res.png
 tutorial/westeros/_static/historical_new_capacity_and_total_installed_capacity.png
 tutorial/westeros/_static/historical_new_capacity_and_total_installed_capacity.pptx
 tutorial/westeros/_static/historical_new_capacity_res.png
 tutorial/westeros/_static/historical_new_capacity_use_in_scenarios.png
 tutorial/westeros/_static/historical_new_capacity_use_in_scenarios.xlsx
+tutorial/westeros/_static/hub.JPG
 tutorial/westeros/_static/load_seasons.png
 tutorial/westeros/_static/message_ixmp.png
 tutorial/westeros/_static/renewable_resource_res.png
 tutorial/westeros/_static/renewable_resource_res_exercise.png
 tutorial/westeros/_static/soft-constraint.PNG
 tutorial/westeros/_static/westeroes_tax_emission_soft_constraint_figures.xlsx
 tutorial/westeros/_static/westeros.jpg
```

### Comparing `message_ix-3.6.0/tutorial/Austrian_energy_system/R_austria.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_addon_technologies.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7414366731901454%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(0, \'# Westeros Tutorial - Introducing `"addon"` '*

 * *            "technologies\\n'), (2, 'This tutorial shows how to establish an inter-dependency "*

 * *            'between two technologies by configuring one of them as `"addon"`  to another one, '*

 * *            'i.e., parent technology. This can be used to model additional technology features '*

 * *            'such as carbon-capture-and-storage (CCS) retrofits, passout-turbines (for optional '*

 * *            "heat cogeneration)  […]*

```diff
@@ -1,891 +1,719 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Austrian energy system Tutorial Part 1: Building an Energy Model (in R)\n",
+                "# Westeros Tutorial - Introducing `\"addon\"` technologies\n",
                 "\n",
-                "For information on how to install *MESSAGEix*, please refer to [Installation page](https://docs.messageix.org/en/stable/#getting-started) and for getting *MESSAGEix* tutorials, please follow the steps mentioned in [Tutorials](https://docs.messageix.org/en/stable/tutorials.html).\n",
+                "This tutorial shows how to establish an inter-dependency between two technologies by configuring one of them as `\"addon\"`  to another one, i.e., parent technology. This can be used to model additional technology features such as carbon-capture-and-storage (CCS) retrofits, passout-turbines (for optional heat cogeneration) or cooling technologies, to existing technologies.\n",
                 "\n",
-                "Please refer to the [user guidelines](https://docs.messageix.org/en/stable/notice.html) for additional information on using *MESSAGEix*, including the recommended citation and how to name new models.\n",
+                "There are several ways to tackle this issue. Lets take the example of a coal power plant (`\"coal_ppl\"`). All of the above mentioned additional features could be implemented by introducing different *modes* of operation for `\"coal_ppl\"`. For example, heat cogeneration could be implemented as a separate operation `\"mode\"` of `\"coal_ppl\"`, where instead of just generating electricity, heat can also be produced at the cost of reducing the amount of electricity generated. Another approach would make use of the generic `\"relations\"` in MESSAGEix, therefore linking the newly added technology representing the passout-turbine with the activity of `\"coal_ppl\"`. Both of these approaches have some downsides. Using a separate `\"mode\"` will not permit explicitly modelling investment costs and lifetime associated with the asset being added to `\"coal_ppl\"`. Generic relations are very flexible, but if too many of them are added, the model becomes very hard to understand. MESSAGEix offers an explicit `\"addon\"` formulation for tackling this issue.\n",
                 "\n",
-                "**Pre-requisites**\n",
-                "- You have the *MESSAGEix* framework installed and working\n",
-                "\n",
-                "**Structure of these tutorials.** After having run this baseline tutorial, you are able to start with any of the other tutorials, but we recommend to follow the order below for going through the information step-wise:\n",
-                "\n",
-                "1. Prepare the base model version (Python: ``austria.ipynb``, R: ``R_austria.ipynb``)\n",
-                "2. Plot the results of the baseline runs (Python: ``austria_load_scenario.ipynb``, R: ``R_austria_load_scenario.ipynb``).\n",
-                "\n",
-                "Currently only available in Python:\n",
-                "3. Run a single policy scenario (``austria_single_policy.ipynb``).\n",
-                "4. Run multiple policy scenarios. This tutorial has two notebooks: an introduction with some exercises and completed code for the exercises (exercises: ``austria_multiple_policies.ipynb``, answers: ``austria_multiple_policies-answers.ipynb``).\n",
-                "\n",
-                "**Introduction**\n",
-                "\n",
-                "In this notebook, we will build a model of the Austrian energy system from scratch. The process will involve defining our model's time horizon and spatial extent, and then populating the model with data associated with model parameters. Once we have a baseline model, we will then move on to investigating policy scenarios.\n",
-                "\n",
-                "We will be populating different kinds of parameters including:\n",
-                "\n",
-                "### Economic Parameters\n",
-                "\n",
-                "- `interestrate`\n",
-                "- `demand`\n",
-                "\n",
-                "### Technology Parameters\n",
-                "\n",
-                "#### Engineering Parameters\n",
-                "\n",
-                "- `input`\n",
-                "- `output`\n",
-                "- `technical_lifetime`\n",
-                "- `capacity_factor`\n",
-                "\n",
-                "\n",
-                "#### Technoeconomic Parameters\n",
-                "\n",
-                "- `inv_cost`\n",
-                "- `fix_cost`\n",
-                "- `var_cost`\n",
-                "\n",
-                "### Dynamic Behavior Parameters\n",
-                "\n",
-                "- `bound_activity_up`\n",
-                "- `bound_activity_lo`\n",
-                "- `bound_new_capacity_up`\n",
-                "- `initial_activity_up`\n",
-                "- `growth_activity_up`\n",
+                "The additional technology options are explicitly modelled as separate technologies, classified as `\"addon\"` technologies, linked to the activity of the technology to which they serve as additional configuration options, i.e., the parent technology. Through an `\"addon_conversion\"` factor, the activity of `\"addon\"` technology can further be restricted to a minimum or maximum share of the activity of the parent technology.\n",
                 "\n",
-                "### Emissions\n",
-                "\n",
-                "- `emission_factor`\n",
-                "\n",
-                "A full list of parameters can be found on the (internal) [MESSAGEix documentation website](http://ienecat.iiasa.ac.at:8787/message_ix_doc). This website can be built in the future from the repository that you are using. \n",
-                "\n",
-                "## The Final Product\n",
-                "\n",
-                "At the completion of this exercise, we will have developed an energy model is comprised of the below Reference Energy System (RES):\n",
-                "\n",
-                "![title](austria.png)\n",
-                "\n"
+                "**Pre-requisites for running this tutorial**\n",
+                "- You have the *MESSAGEix* framework installed and working\n",
+                "- You have run Westeros baseline scenario (`westeros_baseline.ipynb`) and solved it successfully"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Setup\n",
+                "# Importing required software packages\n",
+                "import pandas as pd\n",
+                "import ixmp\n",
+                "import message_ix\n",
                 "\n",
-                "We begin by loading the ``rmessageix`` package.\n",
-                "We also load the common R package ``dplyr``, which will be used for some data manipulation."
+                "from message_ix.utils import make_df\n",
+                "\n",
+                "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Load dplyr, used for data manipulation in R\n",
-                "library(dplyr)\n",
-                "\n",
-                "# Load reticulate, used to access the Python API from R\n",
-                "library(reticulate)\n",
-                "\n",
-                "# Import ixmp and message_ix, just as in Python\n",
-                "ixmp <- import(\"ixmp\")\n",
-                "message_ix <- import(\"message_ix\")"
+                "mp = ixmp.Platform()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "These two objects named ``ixmp`` and ``message_ix`` can now be used to access all the features of the API (application programming interface) provided by the Python packages."
+                "## Making a clone of the existing scenario '*baseline*'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "# launch the IX modeling platform using the local default database\n",
-                "mp <- ixmp$Platform()"
+                "model = \"Westeros Electrified\"\n",
+                "base = message_ix.Scenario(mp, model=model, scenario=\"baseline\")\n",
+                "scen = base.clone(\n",
+                "    model, \"addon_technology\", \"illustration of addon formulation\", keep_solution=False\n",
+                ")\n",
+                "scen.check_out()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### i. Setting up parameters"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "model <- \"Austrian energy model\"\n",
-                "scen <- \"baseline\"\n",
-                "annot <- \"developing a stylized energy system model for illustration and testing\" \n",
-                "\n",
-                "scenario <- message_ix$Scenario(mp, model, scen, version='new', annotation=annot)"
+                "year_df = scen.vintage_and_active_years()\n",
+                "vintage_years, act_years = year_df[\"year_vtg\"], year_df[\"year_act\"]\n",
+                "model_horizon = scen.set(\"year\")\n",
+                "country = \"Westeros\"\n",
+                "gdp_profile = pd.Series([1.0, 1.5, 1.9], index=pd.Index([700, 710, 720], name=\"time\"))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Time and Spatial Detail\n",
-                "\n",
-                "The model includes the time periods 2010, 2020, 2030 and 2040."
+                "### ii. Define helper dictionaries used for subsequent operations"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "horizon = as.integer(seq(2010, 2040, 10))\n",
-                "firstyear = as.integer(horizon[1])"
+                "base_input = {\n",
+                "    \"node_loc\": country,\n",
+                "    \"year_vtg\": vintage_years,\n",
+                "    \"year_act\": act_years,\n",
+                "    \"mode\": \"standard\",\n",
+                "    \"node_origin\": country,\n",
+                "    \"time\": \"year\",\n",
+                "    \"time_origin\": \"year\",\n",
+                "}\n",
+                "base_output = {\n",
+                "    \"node_loc\": country,\n",
+                "    \"year_vtg\": vintage_years,\n",
+                "    \"year_act\": act_years,\n",
+                "    \"mode\": \"standard\",\n",
+                "    \"node_dest\": country,\n",
+                "    \"time\": \"year\",\n",
+                "    \"time_dest\": \"year\",\n",
+                "    \"unit\": \"-\",\n",
+                "}\n",
+                "base_capacity_factor = {\n",
+                "    \"node_loc\": country,\n",
+                "    \"year_vtg\": vintage_years,\n",
+                "    \"year_act\": act_years,\n",
+                "    \"time\": \"year\",\n",
+                "    \"unit\": \"-\",\n",
+                "}\n",
+                "base_technical_lifetime = {\n",
+                "    \"node_loc\": country,\n",
+                "    \"year_vtg\": model_horizon,\n",
+                "    \"unit\": \"y\",\n",
+                "}\n",
+                "base_inv_cost = {\n",
+                "    \"node_loc\": country,\n",
+                "    \"year_vtg\": model_horizon,\n",
+                "    \"unit\": \"USD/kW\",\n",
+                "}\n",
+                "base_fix_cost = {\n",
+                "    \"node_loc\": country,\n",
+                "    \"year_vtg\": vintage_years,\n",
+                "    \"year_act\": act_years,\n",
+                "    \"unit\": \"USD/kW\",\n",
+                "}\n",
+                "base_var_cost = {\n",
+                "    \"node_loc\": country,\n",
+                "    \"year_vtg\": vintage_years,\n",
+                "    \"year_act\": act_years,\n",
+                "    \"mode\": \"standard\",\n",
+                "    \"time\": \"year\",\n",
+                "    \"unit\": \"USD/kWa\",\n",
+                "}"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
-            "outputs": [],
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "scenario$add_set(\"year\", horizon)\n",
-                "scenario$add_set(\"cat_year\", c(\"firstmodelyear\", firstyear) )"
+                "## `\"addon\"` technology in MESSAGEix\n",
+                "This tutorial will extend the current reference-energy-system to include a demand for heat and the necessary technologies to meet this demand. Heat will be generated via a passout-turbine which will be linked to the `\"coal_ppl\"` using the `\"addon\"` formulation.\n",
+                "\n",
+                "<img src='_static/addon_technologies_res.png' width='700'>\n",
+                "\n",
+                "We will therefore carry out the following three steps:\n",
+                "1. Define a new commodity and demand for heat:\n",
+                "    - Define new `\"commodity\"` `\"heat\"`.\n",
+                "    - Parametrize `\"demand\"` for `\"heat\"`.\n",
+                "    \n",
+                "    \n",
+                "2. Add new technologies:\n",
+                "    - Add a new technology to generate heat: `\"passout-turbine\"`.\n",
+                "    - Add a new technology district heat network to transport heat to the end-use technology: `\"dh_grid\"`.\n",
+                "    - Add a new end-use technology, an in-house district heat connection which is linked to `\"demand\": \"hs_house\"`.\n",
+                "    \n",
+                "3. Link the passout-turbine to the coal_ppl using the `\"addon\"` feature."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
-            "outputs": [],
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "country = \"Austria\"\n",
-                "scenario$add_set(\"node\", country)\n",
-                "scenario$add_set(\"lvl_spatial\", \"country\")\n",
-                "scenario$add_set(\"map_spatial_hierarchy\", c(\"country\", country, \"World\"))\n",
-                "scenario$add_set(\"mode\", \"standard\")"
+                "### 1: Define a new commodity and demand\n",
+                "We therefore add a new `\"commodity\"` `\"heat\"` and a corresponding demand, which will rise at the same rate as electricity demand."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "scenario$add_set(\"commodity\", c(\"electricity\", \"light\", \"other_electricity\") )\n",
-                "scenario$add_set(\"level\", c(\"secondary\", \"final\", \"useful\") )"
+                "# Define a new commodity `\"heat\"`\n",
+                "scen.add_set(\"commodity\", [\"heat\"])\n",
+                "\n",
+                "# Add heat demand at the useful level\n",
+                "heat_demand = pd.DataFrame(\n",
+                "    {\n",
+                "        \"node\": country,\n",
+                "        \"commodity\": \"heat\",\n",
+                "        \"level\": \"useful\",\n",
+                "        \"year\": [700, 710, 720],\n",
+                "        \"time\": \"year\",\n",
+                "        \"value\": (25 * gdp_profile).round(),\n",
+                "        \"unit\": \"GWa\",\n",
+                "    }\n",
+                ")\n",
+                "scen.add_par(\"demand\", heat_demand)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Economic Parameters"
+                "### 2: Define new technologies\n",
+                "\n",
+                "i. Heat will be generated via a pass-out turbine:\n",
+                "Passout-turbine (`\"po_turbine\"`) characteristics: The passout-turbine requires one unit of electricity to generate five units of heat. The lifetime is assumed to be 30 years, 10 years longer then that of `\"coal_ppl\"`.  Investment costs are 150\\\\$/kW compared to 500\\\\$/kW for `\"coal_ppl\"`.  A coal heatplant would have higher investment costs, approximately double that of \"po_turbine\". Lastly, `\"po_turbine\"` represents an alternative production mode of `\"coal_ppl\"`, hence in order to produce heat, the electricity of `\"coal_ppl\"` is reduced. Thus, electricity is parametrized as an input to `\"po_turbine\"`; for each unit of electricity, 5 units of heat can be produced. This will later also be used for establishing a \"link\" between `\"coal_ppl\"` and `\"po_turbine\"`.\n",
+                "\n",
+                "ii. Heat will be transported via a district heating grid:\n",
+                "District heat (`\"dh_grid\"`) network characteristics: District heating networks have only very low losses as these cover only short distances (within city perimeters). We will assume the district heating network to have an efficiency of 97%.\n",
+                "\n",
+                "iii. Heat demand will be linked to an end-use technology:\n",
+                "`\"hs_house\"` will represent the end-use technology, which distributes heat within the buildings."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
-            "outputs": [],
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "scenario$add_par(\"interestrate\", horizon, value=0.05, unit='%')"
+                "Similar to previous tutorials, we work our way backwards, starting from the `\"heat\"` demand defined at the `\"useful\"` energy level and connecting this to the `\"final\"` energy level via a technology, `\"hs_house\"`, representing the in-house heat distribution system."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "beta = 0.7 \n",
-                "gdp = c(1., 1.21631, 1.4108, 1.63746)\n",
-                "demand = gdp ** beta"
+                "tec = \"hs_house\"\n",
+                "scen.add_set(\"technology\", tec)\n",
+                "\n",
+                "hs_house_out = make_df(\n",
+                "    \"output\", **base_output, technology=tec, commodity=\"heat\", level=\"useful\", value=1.0\n",
+                ")\n",
+                "scen.add_par(\"output\", hs_house_out)\n",
+                "\n",
+                "hs_house_in = make_df(\n",
+                "    \"input\",\n",
+                "    **base_input,\n",
+                "    technology=tec,\n",
+                "    commodity=\"heat\",\n",
+                "    level=\"final\",\n",
+                "    value=1.0,\n",
+                "    unit=\"-\"\n",
+                ")\n",
+                "scen.add_par(\"input\", hs_house_in)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Technologies"
+                "Next, we add the information for the district heating network."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "plants = c(    \"coal_ppl\", \n",
-                "    \"gas_ppl\", \n",
-                "    \"oil_ppl\", \n",
-                "    \"bio_ppl\", \n",
-                "    \"hydro_ppl\",\n",
-                "    \"wind_ppl\", \n",
-                "    \"solar_pv_ppl\" # actually primary -> final\n",
-                ")\n",
-                "secondary_energy_techs = c(plants,'import')\n",
+                "tec = \"dh_grid\"\n",
+                "scen.add_set(\"technology\", tec)\n",
                 "\n",
-                "final_energy_techs = c('electricity_grid')\n",
+                "dh_grid_out = make_df(\n",
+                "    \"output\", **base_output, technology=tec, commodity=\"heat\", level=\"final\", value=1.0\n",
+                ")\n",
+                "scen.add_par(\"output\", dh_grid_out)\n",
                 "\n",
-                "lights = c(\n",
-                "    \"bulb\", \n",
-                "    \"cfl\" \n",
+                "dh_grid_in = make_df(\n",
+                "    \"input\",\n",
+                "    **base_input,\n",
+                "    technology=tec,\n",
+                "    commodity=\"heat\",\n",
+                "    level=\"secondary\",\n",
+                "    value=1.03,\n",
+                "    unit=\"-\",\n",
                 ")\n",
-                "useful_energy_techs = c(lights ,'appliances')"
+                "scen.add_par(\"input\", dh_grid_in)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
-            "outputs": [],
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "technologies = c(secondary_energy_techs, final_energy_techs,  useful_energy_techs)\n",
-                "scenario$add_set(\"technology\", technologies)"
+                "Last, we add `\"po_turbine\"` as a technology."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "demand_per_year = 55209. / 8760 # from IEA statistics\n",
-                "elec_demand = data.frame(\n",
-                "    node = rep(country,4),\n",
-                "    commodity = rep('other_electricity',4),\n",
-                "    level = rep('useful',4),\n",
-                "    year = horizon,\n",
-                "    time = rep('year',4),\n",
-                "    value = demand_per_year * demand,\n",
-                "    unit = rep('GWa',4),\n",
-                "    row.names = horizon\n",
-                ")\n",
-                "scenario$add_par(\"demand\", elec_demand)\n",
-                "\n",
-                "demand_per_year = 6134. / 8760 # from IEA statistics\n",
-                "light_demand = data.frame(\n",
-                "    node = country,\n",
-                "    commodity = 'light',\n",
-                "    level = 'useful',\n",
-                "    year = horizon,\n",
-                "    time = 'year',\n",
-                "    value = demand_per_year * demand,\n",
-                "    unit = 'GWa'\n",
+                "tec = \"po_turbine\"\n",
+                "scen.add_set(\"technology\", tec)\n",
+                "\n",
+                "po_out = make_df(\n",
+                "    \"output\",\n",
+                "    **base_output,\n",
+                "    technology=tec,\n",
+                "    commodity=\"heat\",\n",
+                "    level=\"secondary\",\n",
+                "    value=1.0,\n",
+                ")\n",
+                "scen.add_par(\"output\", po_out)\n",
+                "\n",
+                "po_in = make_df(\n",
+                "    \"input\",\n",
+                "    **base_input,\n",
+                "    technology=tec,\n",
+                "    commodity=\"electricity\",\n",
+                "    level=\"secondary\",\n",
+                "    value=0.2,\n",
+                "    unit=\"-\",\n",
+                ")\n",
+                "scen.add_par(\"input\", po_in)\n",
+                "\n",
+                "po_tl = make_df(\n",
+                "    \"technical_lifetime\", **base_technical_lifetime, technology=tec, value=30\n",
                 ")\n",
-                "scenario$add_par(\"demand\", light_demand)"
+                "scen.add_par(\"technical_lifetime\", po_tl)\n",
+                "\n",
+                "po_inv = make_df(\"inv_cost\", **base_inv_cost, technology=tec, value=150)\n",
+                "scen.add_par(\"inv_cost\", po_inv)\n",
+                "\n",
+                "po_fix = make_df(\"fix_cost\", **base_fix_cost, technology=tec, value=15)\n",
+                "scen.add_par(\"fix_cost\", po_fix)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "source": [
-                "### Engineering Parameters"
+                "### 3: Link `\"po_turbine\"` with `\"coal_ppl\"`\n",
+                "`\"po_turbine\"` could already operate as all required parameters are defined, yet without a link to the activity of `\"coal_ppl\"`, `\"po_turbine\"` has the possibility of using electricity generated from either `\"coal_ppl\"` or `\"wind_ppl\"`.  But because `\"po_turbine\"` is an addon component to `\"coal_ppl\"` a distinct linkage needs to be established."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
-            "outputs": [],
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "year_pairs = as.matrix(expand.grid(horizon,horizon) %>%\n",
-                "                         rowwise() %>%\n",
-                "                         filter(Var2 >= Var1) %>%\n",
-                "                         arrange(Var1))\n",
-                "vintage_years <- year_pairs[,1]\n",
-                "act_years <- year_pairs[,1]"
+                "First, the newly added technology `\"po_turbine\"` needs to be classified as an `\"addon\"` technology"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "base_input = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_vtg = vintage_years,\n",
-                "    year_act = act_years,\n",
-                "    mode = 'standard',\n",
-                "    node_origin = country,\n",
-                "    commodity = 'electricity',\n",
-                "    time = 'year',\n",
-                "    time_origin = 'year'\n",
-                ")\n",
-                "\n",
-                "grid = data.frame(base_input,data.frame(\n",
-                "        technology = 'electricity_grid',\n",
-                "        level = 'secondary',\n",
-                "        value = 1.0,\n",
-                "        unit = '%'\n",
-                "        ))\n",
-                "scenario$add_par(\"input\", grid)\n",
-                "\n",
-                "bulb = data.frame(base_input,data.frame(\n",
-                "        technology = 'bulb',\n",
-                "        level = 'final',\n",
-                "        value = 1.0,\n",
-                "        unit = '%'\n",
-                "        ))\n",
-                "scenario$add_par(\"input\", bulb)\n",
-                "\n",
-                "cfl = data.frame(base_input,data.frame(\n",
-                "        technology = 'cfl',\n",
-                "        level = 'final',\n",
-                "        value = 0.3, \n",
-                "        unit = '%'\n",
-                "        ))\n",
-                "scenario$add_par(\"input\", cfl)\n",
-                "\n",
-                "app = data.frame(base_input,data.frame(\n",
-                "        technology = 'appliances',\n",
-                "        level = 'final',\n",
-                "        value = 1.0,\n",
-                "        unit = '%'\n",
-                "        ))\n",
-                "scenario$add_par(\"input\", app)"
+                "scen.add_set(\"addon\", \"po_turbine\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Next, we need a new `\"type_addon\"`, which we will name `\"cogeneration_heat\"`.  We will classify the `\"po_turbine\"` via the *category* `\"addon\"` as one of the addon technologies as part of this specific `\"type_addon\"`.  In some cases, for example when modelling cooling technologies, multiple technologies can be classfied within a single `\"type_addon\"`.\n",
+                "\n",
+                "Via the set `\"map_tec_addon\"` we map the electricity generation technology, `\"coal_ppl\"`, to the `\"addon\"` technology, `\"po_turbine\"`. Multiple technologies, for example further fossil powerplants, could also be added to this `\"type_addon\"` so as to be able to produce heat via `\"po_turbine\"`.\n",
+                "\n",
+                "Note: the `\"addon\"` technology as well as the parent technology must have the same `\"mode\"`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "base_output = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_vtg = vintage_years,\n",
-                "    year_act = act_years,\n",
-                "    mode = 'standard',\n",
-                "    node_dest = country,\n",
-                "    time = 'year',\n",
-                "    time_dest = 'year', \n",
-                "    unit = '%'\n",
-                ")\n",
-                "\n",
-                "imports = data.frame(base_output,data.frame( technology='import', commodity='electricity', \n",
-                "                  level='secondary', value=1.))\n",
-                "scenario$add_par('output', imports)\n",
-                "\n",
-                "grid = data.frame(base_output,data.frame( technology='electricity_grid', commodity='electricity', \n",
-                "               level='final', value=0.873))\n",
-                "scenario$add_par('output', grid)\n",
-                "\n",
-                "bulb = data.frame(base_output,data.frame( technology='bulb', commodity='light', \n",
-                "               level='useful', value=1.))\n",
-                "scenario$add_par('output', bulb)\n",
-                "\n",
-                "cfl = data.frame(base_output,data.frame( technology='cfl', commodity='light', \n",
-                "              level='useful', value=1.))\n",
-                "scenario$add_par('output', cfl)\n",
-                "\n",
-                "app = data.frame(base_output,data.frame( technology='appliances', commodity='other_electricity', \n",
-                "              level='useful', value=1.))\n",
-                "scenario$add_par('output', app)\n",
-                "\n",
-                "coal = data.frame(base_output,data.frame( technology='coal_ppl', commodity='electricity', \n",
-                "               level='secondary', value=1.))\n",
-                "scenario$add_par('output', coal)\n",
-                "\n",
-                "gas = data.frame(base_output,data.frame( technology='gas_ppl', commodity='electricity', \n",
-                "              level='secondary', value=1.))\n",
-                "scenario$add_par('output', gas)\n",
-                "\n",
-                "oil = data.frame(base_output,data.frame( technology='oil_ppl', commodity='electricity', \n",
-                "              level='secondary', value=1.))\n",
-                "scenario$add_par('output', oil)\n",
-                "\n",
-                "bio = data.frame(base_output,data.frame( technology='bio_ppl', commodity='electricity', \n",
-                "              level='secondary', value=1.))\n",
-                "scenario$add_par('output', bio)\n",
-                "\n",
-                "hydro = data.frame(base_output,data.frame( technology='hydro_ppl', commodity='electricity', \n",
-                "                level='secondary', value=1.))\n",
-                "scenario$add_par('output', hydro)\n",
-                "\n",
-                "wind = data.frame(base_output,data.frame( technology='wind_ppl', commodity='electricity', \n",
-                "               level='secondary', value=1.))\n",
-                "scenario$add_par('output', wind)\n",
-                "\n",
-                "solar_pv = data.frame(base_output,data.frame( technology='solar_pv_ppl', commodity='electricity', \n",
-                "                   level='final', value=1.))\n",
-                "scenario$add_par('output', solar_pv)"
+                "type_addon_ch = \"cogeneration_heat\"\n",
+                "addon_tech = \"po_turbine\"\n",
+                "tec = \"coal_ppl\"\n",
+                "scen.add_cat(\"addon\", type_addon_ch, addon_tech)\n",
+                "scen.add_set(\n",
+                "    \"map_tec_addon\", pd.DataFrame({\"technology\": tec, \"type_addon\": [type_addon_ch]})\n",
+                ")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The last step required in order to link the `\"coal_ppl\"` is to define the `\"addon_conversion\"` factor between the `\"coal_ppl\"` and the `\"type_addon\"`.  This is important, because the `\"coal_ppl\"` generates electricity while the `\"po_turbine\"` generates heat. Therefore, we can use the inverse of the `\"input\"` coefficient from the `\"po_turbine\"`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# NB this and the following cell can be modified to a syntax like the above\n",
-                "\n",
-                "base_technical_lifetime = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_vtg = horizon,\n",
-                "    unit = 'y'\n",
-                ")\n",
-                "\n",
-                "lifetimes = list(\n",
-                "    coal_ppl = 40,\n",
-                "    gas_ppl =  30,\n",
-                "    oil_ppl = 30,\n",
-                "    bio_ppl =  30,\n",
-                "    hydro_ppl = 60,\n",
-                "    wind_ppl = 20,\n",
-                "    solar_pv_ppl = 20,\n",
-                "    bulb = 1,\n",
-                "    cfl = 10\n",
+                "df = pd.DataFrame(\n",
+                "    {\n",
+                "        \"node\": country,\n",
+                "        \"technology\": tec,\n",
+                "        \"year_vtg\": vintage_years,\n",
+                "        \"year_act\": act_years,\n",
+                "        \"mode\": \"standard\",\n",
+                "        \"time\": \"year\",\n",
+                "        \"type_addon\": type_addon_ch,\n",
+                "        \"value\": 5,\n",
+                "        \"unit\": \"-\",\n",
+                "    }\n",
                 ")\n",
-                "base_technical_lifetime\n",
-                "\n",
-                "for (i in seq_along(lifetimes)){\n",
-                "    df = data.frame(base_technical_lifetime, technology=names(lifetimes[i]), value=lifetimes[[i]])\n",
-                "    scenario$add_par('technical_lifetime', df)\n",
-                "}"
+                "scen.add_par(\"addon_conversion\", df)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Although not necessary for this specific example, it is also possible to limit the activity of `\"po_turbine\"` to a specific share of `\"coal_ppl\"` activity. In the example below, `\"po_turbine\"` is limited to using 15% of `\"coal_ppl\"` activity.  Likewise, a constraint on the minimum amount of electricity used from `\"po_turbine\"` can be applied by using the parameter `\"addon_lo\"`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "base_capacity_factor = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_vtg = vintage_years,\n",
-                "    year_act = act_years,\n",
-                "    time = 'year',\n",
-                "    unit = '%'\n",
-                ")\n",
-                "\n",
-                "capacity_factor = list(\n",
-                "    coal_ppl = 0.85,\n",
-                "    gas_ppl =  0.75,\n",
-                "    oil_ppl = 0.75,\n",
-                "    bio_ppl = 0.75,\n",
-                "    hydro_ppl = 0.5,\n",
-                "    wind_ppl = 0.2,\n",
-                "    solar_pv_ppl = 0.15,\n",
-                "    bulb = 0.1, \n",
-                "    cfl =  0.1\n",
+                "# Index for \"addon_up\" is [\"node\", \"technology\", \"year_act\",\n",
+                "#                          \"mode\", \"time\", \"type_addon\",\n",
+                "#                          \"value\", \"unit\"]\n",
+                "df = pd.DataFrame(\n",
+                "    {\n",
+                "        \"node\": country,\n",
+                "        \"technology\": tec,\n",
+                "        \"year_act\": act_years,\n",
+                "        \"mode\": \"standard\",\n",
+                "        \"time\": \"year\",\n",
+                "        \"type_addon\": type_addon_ch,\n",
+                "        \"value\": 0.15,\n",
+                "        \"unit\": \"-\",\n",
+                "    }\n",
                 ")\n",
-                "    \n",
-                "for (i in seq_along(capacity_factor)){\n",
-                "    df = data.frame(base_capacity_factor, technology=names(capacity_factor[i]), value=capacity_factor[[i]])\n",
-                "    scenario$add_par('capacity_factor', df)\n",
-                "}"
+                "scen.add_par(\"addon_up\", df)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Technoeconomic Parameters"
+                "### Commit and solve"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "base_inv_cost = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_vtg = horizon,\n",
-                "    unit = 'USD/GWa'\n",
-                ")\n",
-                "\n",
-                "# in $ / kW\n",
-                "costs = list(\n",
-                "    coal_ppl = 1500,\n",
-                "    gas_ppl =   870,\n",
-                "    oil_ppl =  950,\n",
-                "    hydro_ppl = 3000,\n",
-                "    bio_ppl =  1600,\n",
-                "    wind_ppl = 1100,\n",
-                "    solar_pv_ppl = 4000,\n",
-                "    bulb = 5,\n",
-                "    cfl =  900\n",
-                ")\n",
-                "\n",
-                "for (i in seq_along(costs)){\n",
-                "    df = data.frame(base_inv_cost, technology=names(costs[i]), value=costs[[i]] * 1e6)\n",
-                "    scenario$add_par('inv_cost', df)\n",
-                "}"
+                "scen.commit(comment=\"define parameters for renewable implementation\")\n",
+                "scen.set_as_default()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "base_fix_cost = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_vtg = vintage_years,\n",
-                "    year_act = act_years,\n",
-                "    unit = 'USD/GWa'\n",
-                ")\n",
-                "\n",
-                "# in $ / kW\n",
-                "costs = list(\n",
-                "    coal_ppl = 40,\n",
-                "    gas_ppl =   25,\n",
-                "    oil_ppl =  25,\n",
-                "    hydro_ppl = 60,\n",
-                "    bio_ppl =  30,\n",
-                "    wind_ppl = 40,\n",
-                "    solar_pv_ppl = 25\n",
-                ")\n",
-                "\n",
-                "for (i in seq_along(costs)){\n",
-                "    df = data.frame(base_fix_cost, technology=names(costs[i]), value=costs[[i]] * 1e6)\n",
-                "    scenario$add_par('fix_cost', df)\n",
-                "}"
+                "scen.solve()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "base_var_cost = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_vtg = vintage_years,\n",
-                "    year_act = act_years,\n",
-                "    mode = 'standard',\n",
-                "    time = 'year',\n",
-                "    unit = 'USD/GWa'\n",
-                ")\n",
-                "\n",
-                "# in $ / MWh\n",
-                "costs = list(\n",
-                "    coal_ppl = 24.4,\n",
-                "    gas_ppl =   42.4,\n",
-                "    oil_ppl =   77.8,\n",
-                "    bio_ppl =  48.2,\n",
-                "    electricity_grid = 47.8\n",
-                ")\n",
-                "    \n",
-                "for (i in seq_along(costs)){\n",
-                "    df = data.frame(base_var_cost, technology=names(costs[i]), value=costs[[i]] * 8760 * 1e3)\n",
-                "    scenario$add_par('var_cost', df)\n",
-                "}"
+                "scen.var(\"OBJ\")[\"lvl\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Dynamic Behavior Parameters"
+                "# Plotting Results"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "base_growth = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_act = horizon[-1],\n",
-                "    value = 0.05,\n",
-                "    time = 'year',\n",
-                "    unit = '%'\n",
-                ")\n",
-                "\n",
-                "growth_technologies = c(\n",
-                "    \"coal_ppl\", \n",
-                "    \"gas_ppl\", \n",
-                "    \"oil_ppl\", \n",
-                "    \"bio_ppl\", \n",
-                "    \"hydro_ppl\",\n",
-                "    \"wind_ppl\", \n",
-                "    \"solar_pv_ppl\", \n",
-                "    \"cfl\",\n",
-                "    \"bulb\"\n",
-                ")\n",
-                "\n",
-                "for (tec in (growth_technologies)){\n",
-                "    df = data.frame(base_growth, technology= tec)\n",
-                "    scenario$add_par('growth_activity_up', df)\n",
-                "}"
+                "# Create a Reporter object to describe and carry out reporting\n",
+                "# calculations and operations (like plotting) based on `scenario`\n",
+                "from message_ix.reporting import Reporter\n",
+                "\n",
+                "rep_bl = Reporter.from_scenario(base)\n",
+                "rep_addon = Reporter.from_scenario(scen)\n",
+                "\n",
+                "# \"prepare_plots\" enables several to describe reporting operations, e.g.\n",
+                "# \"plot activity\", \"plot capacity\", or \"plot prices\"\n",
+                "# See message_ix/util/tutorial.py for more information\n",
+                "from message_ix.util.tutorial import prepare_plots\n",
+                "\n",
+                "prepare_plots(rep_bl)\n",
+                "prepare_plots(rep_addon)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
-            "outputs": [],
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "base_initial = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_act = horizon[-1],\n",
-                "    time = 'year',\n",
-                "    unit = '%'\n",
-                ")\n",
-                "\n",
-                "for (tec in (lights)){\n",
-                "    df = data.frame(base_initial, technology= tec, value = 0.01 *light_demand$value[light_demand$year %in% c(2020,2030,2040)])\n",
-                "    scenario$add_par('initial_activity_up', df)\n",
-                "}"
+                "## Activity\n",
+                "***"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Scenario: '*baseline*'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "base_activity = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_act = as.integer(2010),\n",
-                "    mode = 'standard',\n",
-                "    time = 'year',\n",
-                "    unit = 'GWa'\n",
-                ")\n",
-                "\n",
-                "# in GWh - from IEA Electricity Output\n",
-                "activity = list(\n",
-                "    coal_ppl = 7184,\n",
-                "    gas_ppl =  14346,\n",
-                "    oil_ppl =  1275,\n",
-                "    hydro_ppl = 38406,\n",
-                "    bio_ppl =  4554,\n",
-                "    wind_ppl = 2064,\n",
-                "    solar_pv_ppl = 89,\n",
-                "    import = 2340,\n",
-                "    cfl = 0\n",
-                ")\n",
-                "\n",
-                "for (i in seq_along(activity)){\n",
-                "    df = data.frame(base_activity, technology=names(activity[i]), value=activity[[i]]/8760)\n",
-                "    scenario$add_par('bound_activity_up', df)\n",
-                "    scenario$add_par('bound_activity_lo', df)\n",
-                "}"
+                "rep_bl.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
+                "rep_bl.get(\"plot activity\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Scenario: '*addon_technology*'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "base_capacity = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_vtg = as.integer(2010),\n",
-                "    unit = 'GWa'\n",
-                ")\n",
-                "\n",
-                "a = as.data.frame(t(as.data.frame(activity))) %>% rename(act = V1)\n",
-                "b = as.data.frame(t(as.data.frame(capacity_factor)))%>% rename(cf = V1) \n",
-                "capacity = left_join(\n",
-                "    a%>% mutate(technology = row.names(a)),\n",
-                "    b%>% mutate(technology = row.names(b))) %>% \n",
-                "  mutate(value = (act / 8760 / cf)) %>% \n",
-                "  filter(!is.na(value))\n",
-                "\n",
-                "df = data.frame(base_capacity,capacity)\n",
-                "scenario$add_par('bound_new_capacity_up', df)"
+                "rep_addon.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
+                "rep_addon.get(\"plot activity\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "base_activity = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_act = horizon[-1],\n",
-                "    mode = 'standard',\n",
-                "    time = 'year',\n",
-                "    unit = 'GWa'\n",
-                ")\n",
-                "\n",
-                "# in GWh - base value from IEA Electricity Output\n",
-                "keep_activity = list(\n",
-                "    hydro_ppl = 38406,\n",
-                "    bio_ppl =  4554,\n",
-                "    import = 2340\n",
-                ")\n",
-                "    \n",
-                "for (i in seq_along(keep_activity)){\n",
-                "    df = data.frame(base_activity, technology=names(keep_activity[i]), value=keep_activity[[i]])\n",
-                "    scenario$add_par('bound_activity_up', df)\n",
-                "}"
+                "rep_addon.set_filters(t=[\"po_turbine\"])\n",
+                "rep_addon.get(\"plot activity\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Question\n",
+                "Comparing the electricity generation of wind power plants in *baseline* and in this scenario shows that wind is generating more electricity now. Can you explain the reason? You can find the answer at the end of this tutorial."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Capacity\n",
+                "***\n",
+                "The behavior observed for the activity of the two electricity generation technologies is reflected in the capacity."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Emissions"
+                "### Scenario: '*baseline*'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "scenario$add_set(\"emission\", \"CO2\")\n",
-                "scenario$add_cat('emission', 'GHGs', 'CO2')"
+                "rep_bl.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
+                "rep_bl.get(\"plot capacity\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Scenario: '*addon_technology*'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "base_emissions = data.frame(\n",
-                "    node_loc = country,\n",
-                "    year_vtg = vintage_years,\n",
-                "    year_act = act_years,\n",
-                "    mode = 'standard',\n",
-                "    unit = 'kg/kWa' # actually is tCO2/GWa\n",
-                ")\n",
-                "\n",
-                "# units: tCO2/MWh\n",
-                "emissions = list(\n",
-                "    coal_ppl =  c('CO2', 0.854),\n",
-                "    gas_ppl =   c('CO2', 0.339),\n",
-                "    oil_ppl =   c('CO2', 0.57)\n",
-                ")\n",
-                "    \n",
-                "for (i in seq_along(emissions)){\n",
-                "    df = data.frame(base_emissions, technology=names(emissions[i]),emission = emissions[[i]][1], value = (as.numeric(emissions[[i]][2])* 8760. * 1000) )\n",
-                "    scenario$add_par('emission_factor', df)\n",
-                "}"
+                "rep_addon.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
+                "rep_addon.get(\"plot capacity\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Prices\n",
+                "***\n",
+                "The resulting impact on the electricity price is negligable, though. Yet we can see that the price of heat is significantly lower than that of light."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Commit the datastructure and solve the model"
+                "### Scenario: '*baseline*'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "comment = 'initial commit for Austria model'\n",
-                "scenario$commit(comment)\n",
-                "scenario$set_as_default()"
+                "rep_bl.set_filters(c=[\"light\"])\n",
+                "rep_bl.get(\"plot prices\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Scenario: '*addon_technology*'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "scenario$solve('MESSAGE')"
+                "rep_addon.set_filters(c=[\"light\"])\n",
+                "rep_addon.get(\"plot prices\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "scenario$var('OBJ')['lvl']"
+                "rep_addon.set_filters(c=[\"heat\"])\n",
+                "rep_addon.get(\"plot prices\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Answer to the question:\n",
+                "In the new scenario ('*addon_technology*'), the effects of the addon technology can be seen when comparing the activity to the baseline scenario ('*baseline*'). From 700 onwards, the activity of the `\"wind_ppl\"` has increased to compensate for the electricity required from the `\"coal_ppl\"` for use in the `\"po_turbine\"`. In 720, when the `\"wind_ppl\"` is phased out, more electricity is required to be produced by the `\"coal_ppl\"`. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "mp$close_db()"
+                "mp.close_db()"
             ]
         }
     ],
     "metadata": {
-        "anaconda-cloud": {},
         "kernelspec": {
-            "display_name": "R",
-            "language": "R",
-            "name": "ir"
+            "display_name": "message_ix",
+            "language": "python",
+            "name": "python3"
         },
         "language_info": {
-            "codemirror_mode": "r",
-            "file_extension": ".r",
-            "mimetype": "text/x-r-source",
-            "name": "R",
-            "pygments_lexer": "r",
-            "version": "3.4.3"
+            "codemirror_mode": {
+                "name": "ipython",
+                "version": 3
+            },
+            "file_extension": ".py",
+            "mimetype": "text/x-python",
+            "name": "python",
+            "nbconvert_exporter": "python",
+            "pygments_lexer": "ipython3",
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 1
+    "nbformat_minor": 2
 }
```

### Comparing `message_ix-3.6.0/tutorial/Austrian_energy_system/R_austria_load_scenario.ipynb` & `message_ix-3.7.0/tutorial/Austrian_energy_system/R_austria_load_scenario.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9911744505494505%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(12, 'This tutorial can be executed after the "*

 * *            '``R_austria.ipynb`` tutorial, to check the basic functions of the `rmessageix` '*

 * *            "package.')], delete: [12]}, 'attachments': OrderedDict()}, 2: {'metadata': {replace: "*

 * *            "OrderedDict([('vscode', OrderedDict([('languageId', 'r')]))])}}, 3: {'metadata': "*

 * *            "{'vscode': OrderedDict([('languageId', 'r')])}}, 4: {'metadata': {replace: "*

 * *            "OrderedDict([('vscode', OrderedDi […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Austrian energy system Tutorial Part 2: Further analysing an Energy Model (in R)\n",
                 "\n",
                 "**Pre-requisites**\n",
                 "- You have the *MESSAGEix* framework installed and working\n",
@@ -12,65 +13,79 @@
                 "\n",
                 "**Introduction**\n",
                 "\n",
                 "In this notebook, we load the previously built model of the Austrian energy system to do some further analysis. The aim of this tutorial is to illustrate the workflow for subsequent analysis after the initial model development.\n",
                 "\n",
                 "**Testing tutorial**\n",
                 "\n",
-                "This tutorial can be executed after the ``R_austria.ipynb`` tutorial, to check the basic functions of `rmessageix` package."
+                "This tutorial can be executed after the ``R_austria.ipynb`` tutorial, to check the basic functions of the `rmessageix` package."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Setup"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "vscode": {
+                    "languageId": "r"
+                }
+            },
             "outputs": [],
             "source": [
                 "# Load reticulate \n",
                 "library(reticulate)\n",
                 "\n",
                 "# Import ixmp and message_ix\n",
                 "ixmp <- import(\"ixmp\")\n",
                 "message_ix <- import(\"message_ix\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": true
+                "collapsed": true,
+                "vscode": {
+                    "languageId": "r"
+                }
             },
             "outputs": [],
             "source": [
                 "model <- \"Austrian energy model\"\n",
                 "scen <- \"baseline\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "vscode": {
+                    "languageId": "r"
+                }
+            },
             "outputs": [],
             "source": [
                 "# launch the IX modeling platform using the local default database\n",
                 "mp <- ixmp$Platform()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": true
+                "collapsed": true,
+                "vscode": {
+                    "languageId": "r"
+                }
             },
             "outputs": [],
             "source": [
                 "scenario <- message_ix$Scenario(mp, model, scen)"
             ]
         },
         {
@@ -80,15 +95,18 @@
                 "### Show input data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": true
+                "collapsed": true,
+                "vscode": {
+                    "languageId": "r"
+                }
             },
             "outputs": [],
             "source": [
                 "scenario$par('input')"
             ]
         },
         {
@@ -97,45 +115,59 @@
             "source": [
                 "### Solve the model"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "vscode": {
+                    "languageId": "r"
+                }
+            },
             "outputs": [],
             "source": [
                 "scenario$remove_solution()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": true
+                "collapsed": true,
+                "vscode": {
+                    "languageId": "r"
+                }
             },
             "outputs": [],
             "source": [
                 "scenario$solve('MESSAGE')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "vscode": {
+                    "languageId": "r"
+                }
+            },
             "outputs": [],
             "source": [
                 "scenario$var('OBJ')['lvl']"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": true
+                "collapsed": true,
+                "vscode": {
+                    "languageId": "r"
+                }
             },
             "outputs": [],
             "source": [
                 "mp$close_db()"
             ]
         }
     ],
```

### Comparing `message_ix-3.6.0/tutorial/Austrian_energy_system/austria.ipynb` & `message_ix-3.7.0/tutorial/Austrian_energy_system/austria.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9627522376978899%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'For information on how to install *MESSAGEix*, please "*

 * *            'refer to [Installation page](https://docs.messageix.org/en/stable/#getting-started), '*

 * *            'and for getting the *MESSAGEix* tutorials, please follow the steps mentioned in '*

 * *            "[Tutorials](https://docs.messageix.org/en/stable/tutorials.html).\\n'), (13, '2. Plot "*

 * *            'the results of the baseline runs (Python: ``austria_load_scenario.ipynb``, also '*

 * *            "available […]*

```diff
@@ -1,29 +1,30 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Austrian energy system Tutorial Part 1: Building an Energy Model\n",
                 "\n",
-                "For information on how to install *MESSAGEix*, please refer to [Installation page](https://docs.messageix.org/en/stable/#getting-started) and for getting *MESSAGEix* tutorials, please follow the steps mentioned in [Tutorials](https://docs.messageix.org/en/stable/tutorials.html).\n",
+                "For information on how to install *MESSAGEix*, please refer to [Installation page](https://docs.messageix.org/en/stable/#getting-started), and for getting the *MESSAGEix* tutorials, please follow the steps mentioned in [Tutorials](https://docs.messageix.org/en/stable/tutorials.html).\n",
                 "\n",
                 "Please refer to the [user guidelines](https://github.com/iiasa/message_ix/blob/master/NOTICE.rst)\n",
                 "for additional information on using *MESSAGEix*, including the recommended citation and how to name new models.\n",
                 "\n",
                 "**Pre-requisites**\n",
                 "- You have the *MESSAGEix* framework installed and working\n",
                 "\n",
                 "**Structure of these tutorials.** After having run this baseline tutorial, you are able to start with any of the other tutorials, but we recommend to follow the order below for going through the information step-wise:\n",
                 "\n",
                 "1. Prepare the base model version (Python: ``austria.ipynb``, also available in R: ``austria_reticulate.ipynb``)\n",
-                "2. Plot the results of the baseline runs (Python: ``austria_load_scenario.ipynb``, also available in R: ``austria_load_scenario_R.ipynb``).\n",
-                "3. Run a single policy scenario (``austria_single_policy.ipynb``).\n",
-                "4. Run multiple policy scenarios. This tutorial has two notebooks: an introduction with some exercises and completed code for the exercises (exercises: ``austria_multiple_policies.ipynb``, answers: ``austria_multiple_policies-answers.ipynb``).\n",
+                "2. Plot the results of the baseline runs (Python: ``austria_load_scenario.ipynb``, also available in R: ``austria_load_scenario_R.ipynb``)\n",
+                "3. Run a single policy scenario (``austria_single_policy.ipynb``)\n",
+                "4. Run multiple policy scenarios. This tutorial has two notebooks: an introduction with some exercises and completed code for the exercises (exercises: ``austria_multiple_policies.ipynb``, answers: ``austria_multiple_policies-answers.ipynb``)\n",
                 "\n",
                 "**Introduction**\n",
                 "\n",
                 "In this notebook, we will build a model of the Austrian energy system from scratch. The process will involve defining our model's time horizon and spatial extent, and then populating the model with data associated with model parameters. Once we have a baseline model, we will then move on to investigating policy scenarios.\n",
                 "\n",
                 "We will be populating different kinds of parameters including:\n",
                 "\n",
@@ -60,15 +61,15 @@
                 "\n",
                 "- `emission_factor`\n",
                 "\n",
                 "A full list of parameters can be found in the [MESSAGEix documentation](http://messageix.iiasa.ac.at/model/MESSAGE/parameter_def.html). (If you have cloned the MESSAGEix [Github repository](https://github.com/iiasa/message_ix), the documentation can also be built offline; see `doc/README.md`.) \n",
                 "\n",
                 "## The Final Product\n",
                 "\n",
-                "At the completion of this exercise, we will have developed an energy model is comprised of the below Reference Energy System (RES):\n",
+                "At the completion of this exercise, we will have developed an energy model that is comprised of the below Reference Energy System (RES):\n",
                 "\n",
                 "![title](austria.png)\n",
                 "\n"
             ]
         },
         {
             "cell_type": "markdown",
@@ -187,18 +188,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "scenario.add_par(\"interestrate\", horizon, value=0.05, unit='-')"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The fundamental premise of the model is to satisfy demand for energy (services). To first order, demands for services (e.g. electricity) track with economic productivity (GDP). Therefore, as a simple example, we define both a GDP profile and a correlation factor between GDP growth and demand, called beta. Beta will then be used to obtain a simplistic demand profile."
+                "The fundamental premise of the model is to satisfy demand for energy (services). To first order, demands for services (e.g. electricity) track with economic productivity (GDP). Therefore, as a simple example, we define both a GDP profile and a correlation parameter between GDP growth and demand, called beta. Beta will then be used to obtain a simplistic demand profile."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -361,15 +363,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "make_df?\n",
-                "# to see what the funcion \"df\" does."
+                "# to see what the funcion \"make_df\" does."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -547,15 +549,15 @@
                 "    'unit': 'USD/kWa',\n",
                 "}\n",
                 "\n",
                 "# Adding a new unit to the library\n",
                 "mp.add_unit('USD/kWa')  \n",
                 "\n",
                 "# in $ / kW / year (every year a fixed quantity is destinated to cover part of the O&M costs\n",
-                "# based on the size of the plant, e.g. lightning, labor, scheduled maintenance, etc.)\n",
+                "# based on the size of the plant, e.g. lighting, labor, scheduled maintenance, etc.)\n",
                 "\n",
                 "costs = {\n",
                 "    'coal_ppl': 40,\n",
                 "    'gas_ppl':  25,\n",
                 "    'oil_ppl':  25,\n",
                 "    'hydro_ppl': 60,\n",
                 "    'bio_ppl':  30,\n",
@@ -579,15 +581,15 @@
                 "    'year_vtg': vintage_years,\n",
                 "    'year_act': act_years,\n",
                 "    'mode': 'standard',\n",
                 "    'time': 'year',\n",
                 "    'unit': 'USD/kWa',\n",
                 "}\n",
                 "\n",
-                "# Variable O&M (costs associatied to the degradation of equipment when the plant is functioning\n",
+                "# Variable O&M (costs associated with the degradation of equipment when the plant is functioning\n",
                 "# per unit of energy produced)\n",
                 "# kWa = kW\u00b7year = 8760 kWh. Therefore this costs represents USD per 8760 kWh of energy.\n",
                 "# Do not confuse with fixed O&M units.\n",
                 "\n",
                 "\n",
                 "#var O&M in $ / MWh \n",
                 "costs = {\n",
@@ -607,25 +609,26 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Dynamic Behavior Parameters"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In this section the following parameters will be added to the different technologies:\n",
                 "- `bound_activity_up`\n",
                 "- `bound_activity_lo`\n",
                 "- `bound_new_capacity_up`\n",
                 "- `initial_activity_up`\n",
                 "- `growth_activity_up`\n",
                 "\n",
-                "As stated in the **Introduction**, a full list of parameters can be found in the *MESSAGEix* documentation. Specifically for this list, please refer to the section [Bounds on capacity and activity](https://docs.messageix.org/en/stable/model/MESSAGE/parameter_def.html#bounds-on-capacity-and-activity)"
+                "As stated in the **Introduction**, a full list of parameters can be found in the *MESSAGEix* documentation. Specifically for this list, please refer to the section [Bounds on capacity and activity](https://docs.messageix.org/en/stable/model/MESSAGE/parameter_def.html#bounds-on-capacity-and-activity)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -951,27 +954,32 @@
                 "mp.close_db()"
             ]
         }
     ],
     "metadata": {
         "anaconda-cloud": {},
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.6"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `message_ix-3.6.0/tutorial/Austrian_energy_system/austria.png` & `message_ix-3.7.0/tutorial/Austrian_energy_system/austria.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/Austrian_energy_system/austria_load_scenario.ipynb` & `message_ix-3.7.0/tutorial/Austrian_energy_system/austria_load_scenario.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9648652882205514%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(4, 'import matplotlib_inline\\n'), (12, "*

 * *            '\'matplotlib_inline.backend_inline.set_matplotlib_formats("svg")\\n\')], delete: [12, '*

 * *            '4]}}}',*

 * * "'metadata'": "{'kernelspec': {'display_name': 'message_ix'}, 'language_info': {'version': "*

 * *               "'3.10.6'}, 'vscode': OrderedDict([('interpreter', OrderedDict([('hash', "*

 * *               "'29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e')]))])}"}*

```diff
@@ -29,23 +29,23 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# load required packages \n",
                 "import pandas as pd\n",
                 "\n",
                 "from matplotlib.pyplot import style\n",
-                "from IPython.display import set_matplotlib_formats\n",
+                "import matplotlib_inline\n",
                 "\n",
                 "import ixmp as ix\n",
                 "import message_ix\n",
                 "from message_ix.reporting import Reporter\n",
                 "from message_ix.util.tutorial import prepare_plots\n",
                 "\n",
                 "%matplotlib inline\n",
-                "set_matplotlib_formats(\"svg\")\n",
+                "matplotlib_inline.backend_inline.set_matplotlib_formats(\"svg\")\n",
                 "style.use(\"ggplot\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -230,27 +230,32 @@
                 "mp.close_db()"
             ]
         }
     ],
     "metadata": {
         "anaconda-cloud": {},
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.6"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `message_ix-3.6.0/tutorial/Austrian_energy_system/austria_multiple_policies.ipynb` & `message_ix-3.7.0/tutorial/Austrian_energy_system/austria_multiple_policies.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9465119408509017%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, '- You have run Austrian energy system baseline scenario "*

 * *            "(`austria.ipynb`) and solved it successfully\\n'), (5, '- You have completed the "*

 * *            "tutorial on introducing one policy scenario (`austria_single_policy.ipynb`) \\n')], "*

 * *            "delete: [5, 4]}, 'attachments': OrderedDict()}, 2: {'source': {insert: [(5, 'import "*

 * *            "matplotlib_inline\\n'), (15, "*

 * *            '\'matplotlib_inline.backend_inline.set_matplotlib_formats("s […]*

```diff
@@ -1,19 +1,20 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Austrian energy system Tutorial Part 4: Investigating Many Policy Scenarios\n",
                 "\n",
                 "**Pre-requisites**\n",
                 "- You have the *MESSAGEix* framework installed and working\n",
-                "- You have run Austrian energy system baseline scenario (``austria.ipynb``) and solved it successfully\n",
-                "- You have completed the tutorial on introducing one policy scenario (``austria_single_policy.ipynb``) \n",
+                "- You have run Austrian energy system baseline scenario (`austria.ipynb`) and solved it successfully\n",
+                "- You have completed the tutorial on introducing one policy scenario (`austria_single_policy.ipynb`) \n",
                 "\n",
                 "**Answers**\n",
                 "- Answers to the exercises below can be found in another Jupyter Notebook in this folder called ``austria_multiple_policies-answers.ipynb``\n",
                 "\n",
                 "**Introduction**\n",
                 "\n",
                 "In this notebook, we investigate a number of different scenarios.\n",
@@ -52,25 +53,25 @@
             "outputs": [],
             "source": [
                 "# Load required packages \n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "\n",
                 "from matplotlib.pyplot import style\n",
-                "from IPython.display import set_matplotlib_formats\n",
+                "import matplotlib_inline\n",
                 "\n",
                 "import ixmp as ix\n",
                 "import message_ix\n",
                 "from message_ix.reporting import Reporter\n",
                 "from message_ix.util.tutorial import prepare_plots, solve_modified\n",
                 "from message_ix.testing import make_austria\n",
                 "\n",
                 "# Appearance of plots\n",
                 "%matplotlib inline\n",
-                "set_matplotlib_formats(\"svg\")\n",
+                "matplotlib_inline.backend_inline.set_matplotlib_formats(\"svg\")\n",
                 "style.use(\"ggplot\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -167,20 +168,21 @@
                 "# Run the same reporting on both the base and modified scenarios\n",
                 "for r in base_rep, wind_rep:\n",
                 "    r.set_filters(t=plants)\n",
                 "    r.get(\"plot new capacity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Demand-Side Learning\n",
                 "\n",
-                "This model does not use `cfl`s in the basline because they are too expensive. What happens if their cost reduces with time?"
+                "This model does not use `cfl`s in the baseline because they are too expensive. What happens if their cost reduces with time?"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": true
@@ -188,15 +190,15 @@
             "outputs": [],
             "source": [
                 "# Cost as a fraction of the baseline cost, due to learning\n",
                 "learning = np.array([1.0, 0.6, 0.3, 0.1])\n",
                 "\n",
                 "with solve_modified(base_scen, new_name=\"cheap_cfls\") as cfl_scen:\n",
                 "    # Load the investment cost data (cloned from `base_scen`) for cfl\n",
-                "    data = wind_scen.par(\"inv_cost\", filters=dict(technology=\"cfl\"))\n",
+                "    data = cfl_scen.par(\"inv_cost\", filters=dict(technology=\"cfl\"))\n",
                 "    \n",
                 "    # Reduce the values according to the learning curve\n",
                 "    data[\"value\"] = data[\"value\"] * learning\n",
                 "    \n",
                 "    # Overwrite the values in `cfl_scen` at the same indices\n",
                 "    cfl_scen.add_par(\"inv_cost\", data)\n",
                 "\n",
@@ -256,45 +258,51 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# TODO based on the examples above, plot (a) new capacity and (b) prices"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Exercise: Carbon Tax\n",
                 "\n",
                 "What effect does a carbon tax have on the system? What if it is phased in over time? What is the effect on energy prices?\n",
                 "\n",
                 "Hints:\n",
                 "\n",
-                "- what emissions parameters are available from `scenario.par_list()`?\n",
-                "- find out which fields are required using `scenario.idx_names(par_name)`\n",
-                "- carbon taxes are normally provided in units of USD/tCO2\n",
-                "- a normal proposed carbon tax is ~30 USD/tCO2"
+                "- Which emissions parameters are available from `scenario.par_list()`?\n",
+                "- Find out which fields are required using `scenario.idx_names(par_name)`\n",
+                "- Carbon taxes are normally provided in units of USD/tCO2\n",
+                "- A normal proposed carbon tax is ~30 USD/tCO2"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.6"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `message_ix-3.6.0/tutorial/Austrian_energy_system/austria_single_policy.ipynb` & `message_ix-3.7.0/tutorial/Austrian_energy_system/austria_single_policy.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.946933621933622%*

 * *Differences: {"'cells'": "{6: {'source': ['scen_df = mp.scenario_list() # to find the name of the wanted "*

 * *            'scenario, simply print scen_df\\n\', \'scen_df.loc[scen_df["scenario"] == "baseline"] '*

 * *            '# to show just the scenario we are interested in\']}, 10: {\'source\': ["inv_cost_df '*

 * *            '= scenario.par(\'inv_cost\')\\n", \'inv_cost_df.loc[inv_cost_df["technology"] == '*

 * *            '"wind_ppl"]\']}, 11: {\'source\': {insert: [(5, "        \'value\': 1100 * '*

 * *            'subsidies,\\n"), ( […]*

```diff
@@ -87,15 +87,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "mp.scenario_list().tail()"
+                "scen_df = mp.scenario_list() # to find the name of the wanted scenario, simply print scen_df\n",
+                "scen_df.loc[scen_df[\"scenario\"] == \"baseline\"] # to show just the scenario we are interested in"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -128,30 +129,31 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "scenario.par('inv_cost').tail()"
+                "inv_cost_df = scenario.par('inv_cost')\n",
+                "inv_cost_df.loc[inv_cost_df[\"technology\"] == \"wind_ppl\"]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "subsidies = np.array([0.5, 0.5, 0.75, 1])\n",
                 "inv_cost = pd.DataFrame({\n",
                 "        'node_loc': country,\n",
                 "        'year_vtg': horizon,\n",
                 "        'technology': 'wind_ppl',\n",
-                "        'value': 1100 * subsidies * 1e6,\n",
-                "        'unit': 'USD/GWa',\n",
+                "        'value': 1100 * subsidies,\n",
+                "        'unit': 'USD/kW',\n",
                 "})\n",
                 "scenario.add_par('inv_cost', inv_cost)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -257,38 +259,36 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mp.close_db()"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.4"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `message_ix-3.6.0/tutorial/README.rst` & `message_ix-3.7.0/tutorial/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,17 @@
       Add the possibility of co-generation for the coal power plant, by
       allowing it to produce heat via a passout-turbine
       (:tut:`westeros/westeros_addon_technologies.ipynb`).
 
    #. Use parameters to represent the historical characteristics of the energy
       system (:tut:`westeros/westeros_historical_new_capacity.ipynb`).
 
+   #. Modeling of a multi-node energy system and representing trade between nodes
+      (:tut:`westeros/westeros_multinode.ipynb`).
+
 #. Use other features of :mod:`message_ix` and :mod:`ixmp`:
 
    #. ⭐ After the MESSAGE model has solved, use the :mod:`.message_ix.reporting`
       module to ‘report’ results, e.g. do post-processing, plotting, and other
       calculations (:tut:`westeros/westeros_report.ipynb`).
 
    #. Build the baseline scenario using data stored in Excel files to
```

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/addon_technologies_res.png` & `message_ix-3.7.0/tutorial/westeros/_static/addon_technologies_res.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/baseline_res.png` & `message_ix-3.7.0/tutorial/westeros/_static/baseline_res.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/cf_wind.png` & `message_ix-3.7.0/tutorial/westeros/_static/cf_wind.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/doc_page.png` & `message_ix-3.7.0/tutorial/westeros/_static/doc_page.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/firm-capacity.png` & `message_ix-3.7.0/tutorial/westeros/_static/firm-capacity.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/firm-capacity.pptx` & `message_ix-3.7.0/tutorial/westeros/_static/firm-capacity.pptx`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/fossil_resource_res.png` & `message_ix-3.7.0/tutorial/westeros/_static/fossil_resource_res.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/historical_new_capacity_and_total_installed_capacity.png` & `message_ix-3.7.0/tutorial/westeros/_static/historical_new_capacity_and_total_installed_capacity.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/historical_new_capacity_and_total_installed_capacity.pptx` & `message_ix-3.7.0/tutorial/westeros/_static/historical_new_capacity_and_total_installed_capacity.pptx`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/historical_new_capacity_res.png` & `message_ix-3.7.0/tutorial/westeros/_static/historical_new_capacity_res.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/historical_new_capacity_use_in_scenarios.png` & `message_ix-3.7.0/tutorial/westeros/_static/historical_new_capacity_use_in_scenarios.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/historical_new_capacity_use_in_scenarios.xlsx` & `message_ix-3.7.0/tutorial/westeros/_static/historical_new_capacity_use_in_scenarios.xlsx`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/load_seasons.png` & `message_ix-3.7.0/tutorial/westeros/_static/load_seasons.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/message_ixmp.png` & `message_ix-3.7.0/tutorial/westeros/_static/message_ixmp.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/renewable_resource_res.png` & `message_ix-3.7.0/tutorial/westeros/_static/renewable_resource_res.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/renewable_resource_res_exercise.png` & `message_ix-3.7.0/tutorial/westeros/_static/renewable_resource_res_exercise.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/soft-constraint.PNG` & `message_ix-3.7.0/tutorial/westeros/_static/soft-constraint.PNG`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/westeroes_tax_emission_soft_constraint_figures.xlsx` & `message_ix-3.7.0/tutorial/westeros/_static/westeroes_tax_emission_soft_constraint_figures.xlsx`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/westeros.jpg` & `message_ix-3.7.0/tutorial/westeros/_static/westeros.jpg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow.pptx` & `message_ix-3.7.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow.pptx`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow_part1.jpg` & `message_ix-3.7.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow_part1.jpg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow_part2.jpg` & `message_ix-3.7.0/tutorial/westeros/_static/westeros_baseline_xlsx_workflow_part2.jpg`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/westeros_renewable_resource_potentials.png` & `message_ix-3.7.0/tutorial/westeros/_static/westeros_renewable_resource_potentials.png`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/westeros_renewable_resource_potentials.pptx` & `message_ix-3.7.0/tutorial/westeros/_static/westeros_renewable_resource_potentials.pptx`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/_static/westeros_res.pptx` & `message_ix-3.7.0/tutorial/westeros/_static/westeros_res.pptx`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_addon_technologies.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_seasonality.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95586231589968%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Westeros Tutorial - Introducing sub-annual "*

 * *            "time-steps: Modeling of variability in energy supply and demand\\n'), (1, '## "*

 * *            '"*Winter is coming!*" \\n\'), (2, \'Time-dependent variations in demand and supply '*

 * *            "are common characteristics of an electricity system, and Westeros is not an\\n'), (3, "*

 * *            "'exception. This tutorial helps to learn how to add sub-annual time steps to a "*

 * *            "MESSAGEix model and inv […]*

```diff
@@ -1,678 +1,573 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Westeros Tutorial - Introducing `\"addon\"` technologies\n",
+                "# Westeros Tutorial - Introducing sub-annual time-steps: Modeling of variability in energy supply and demand\n",
+                "## \"*Winter is coming!*\" \n",
+                "Time-dependent variations in demand and supply are common characteristics of an electricity system, and Westeros is not an\n",
+                "exception. This tutorial helps to learn how to add sub-annual time steps to a MESSAGEix model and investigate the impact of the\n",
+                "variability in supply and demand. It is structured as follows:\n",
+                "1. A short note on seasonality\n",
+                "2. Adding sub-annual time steps\n",
+                "3. Analyzing the results\n",
                 "\n",
-                "This tutorial shows how to establish an inter-dependency between two technologies by configuring one of them as `\"addon\"`  to another one, i.e., parent technology. This can be used to model additional technology features such as carbon-capture-and-storage (CCS) retrofits, passout-turbines (for optional heat cogeneration) or cooling technologies, to existing technologies.\n",
+                "**Pre-requisites**\n",
+                "- You have the *MESSAGEix* framework installed and working\n",
+                "- You have run Westeros baseline scenario (``westeros_baseline.ipynb``) and solved it successfully\n",
                 "\n",
-                "There are several ways to tackle this issue. Lets take the example of a coal power plant (`\"coal_ppl\"`). All of the above mentioned additional features could be implemented by introducing different *modes* of operation for `\"coal_ppl\"`. For example, heat cogeneration could be implemented as a separate operation `\"mode\"` of `\"coal_ppl\"`, where instead of just generating electricity, heat can also be produced at the cost of reducing the amount of electricity generated. Another approach would make use of the generic `\"relations\"` in MESSAGEix, therefore linking the newly added technology representing the passout-turbine with the activity of `\"coal_ppl\"`. Both of these approaches have some downsides. Using a separate `\"mode\"` will not permit explicitly modelling investment costs and lifetime associated with the asset being added to `\"coal_ppl\"`. Generic relations are very flexible, but if too many of them will be added, the model becomes very hard to understand. MESSAGEix offers an explicit `\"addon\"` formulation for tackling this issue.\n",
                 "\n",
-                "The additional technology options are explicitly modelled as separate technologies, classified as `\"addon\"` technologies, linked to the activity of the technology to which they serve as additional configuration options, i.e., the parent technology. Through an `\"addon_conversion\"` factor, the activity of `\"addon\"` technology can further be restricted to a minimum or maximum share of the activity of the parent technology.\n",
+                "_This tutorial was developed by Behnam Zakeri ([@behnam-zakeri](https://github.com/behnam-zakeri)) for the course Energy\n",
+                "Economics and Modeling held at the International Summer School in Energy Technology, St. Petersburg Polytechnique University in August 2018._"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## 1. Seasonal variations in demand and supply\n",
+                "The electricity demand can vary on different time scales, e.g., seasonally, monthly, daily, and hourly. In Westeros, the winter time is typically cold and long, which increases the demand for electricity and lighting. We investigate this seasonality in this tutorial, but the procedure discussed here can be adopted for studying different lengths of temporal resolution.\n",
                 "\n",
-                "**Pre-requisites for running this tutorial**\n",
-                "- You have the *MESSAGEix* framework installed and working.\n",
-                "- You have run Westeros baseline scenario (`westeros_baseline.ipynb`) and solved it successfully."
+                "<img src='_static/load_seasons.png'>"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# Importing required software packages\n",
-                "import pandas as pd\n",
-                "import ixmp\n",
-                "import message_ix\n",
+                "Seasonality can be relevant to some supply technologies as well. For example, Westeros has more windy days in winter months compared to summer. This means the capacity factor of a wind power plant is higher in winter compared to summer. The figure below, rendered from renewables.ninja*, shows the monthly capacity factor of a wind power plant somewhere near Westeros.                                                       \n",
                 "\n",
-                "from message_ix.utils import make_df\n",
+                "<img src=\"_static/cf_wind.png\" style=\"width: 600px;\"/>\n",
                 "\n",
-                "%matplotlib inline"
+                "*You can also find the capacity factor of wind and solar PV for your location at https://www.renewables.ninja/, as we found for a place near Westeros."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## 2. Implementation of seasonality\n",
+                "In this tutorial we add two sub-annual time steps, winter and summer. First, we load the baseline scenario, then we add the required sets related to seasonality, next we modify the parameters, and finally we analyze the results.\n",
+                "\n",
+                "### Loading Westeros baseline scenario "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "mp = ixmp.Platform()"
+                "# Importing required packages\n",
+                "import pandas as pd\n",
+                "import ixmp as ix\n",
+                "import message_ix\n",
+                "\n",
+                "%matplotlib inline"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Making a clone of the existing scenario '*baseline*'"
+                "# Loading modelling platform\n",
+                "mp = ix.Platform()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# Specifying model/scenario to be loaded from the database\n",
                 "model = \"Westeros Electrified\"\n",
-                "base = message_ix.Scenario(mp, model=model, scenario=\"baseline\")\n",
+                "scenario = \"baseline\"\n",
+                "base = message_ix.Scenario(mp, model, scenario)\n",
+                "\n",
+                "# Cloning a scenario for adding time steps\n",
                 "scen = base.clone(\n",
-                "    model, \"addon_technology\", \"illustration of addon formulation\", keep_solution=False\n",
+                "    model, \"westeros_seasonal\", \"introducing seasonality\", keep_solution=False\n",
                 ")\n",
                 "scen.check_out()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### i. Setting up parameters"
+                "### Modifying sets\n",
+                "First, we specify subannual time steps and add them to relevant MESSAGE sets. In the MESSAGEix framework, the set `\"time\"` is devoted for sub-annual time steps, denoted by index *h* in the mathematical formulation:\n",
+                "\n",
+                "| Set name | Math notation | Explanation |\n",
+                "|:---------|:--------------|:------------|\n",
+                "| time     | $h \\in H$     | subannual time periods |"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "year_df = scen.vintage_and_active_years()\n",
-                "vintage_years, act_years = year_df[\"year_vtg\"], year_df[\"year_act\"]\n",
-                "model_horizon = scen.set(\"year\")\n",
-                "country = \"Westeros\"\n",
-                "gdp_profile = pd.Series([1.0, 1.5, 1.9], index=pd.Index([700, 710, 720], name=\"time\"))"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### ii. Define helper dictionaries used for subsequent operations"
+                "# Adding sub-annual time steps\n",
+                "time_steps = [\"winter\", \"summer\"]\n",
+                "scen.add_set(\"time\", time_steps)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "base_input = {\n",
-                "    \"node_loc\": country,\n",
-                "    \"year_vtg\": vintage_years,\n",
-                "    \"year_act\": act_years,\n",
-                "    \"mode\": \"standard\",\n",
-                "    \"node_origin\": country,\n",
-                "    \"time\": \"year\",\n",
-                "    \"time_origin\": \"year\",\n",
-                "}\n",
-                "base_output = {\n",
-                "    \"node_loc\": country,\n",
-                "    \"year_vtg\": vintage_years,\n",
-                "    \"year_act\": act_years,\n",
-                "    \"mode\": \"standard\",\n",
-                "    \"node_dest\": country,\n",
-                "    \"time\": \"year\",\n",
-                "    \"time_dest\": \"year\",\n",
-                "    \"unit\": \"-\",\n",
-                "}\n",
-                "base_capacity_factor = {\n",
-                "    \"node_loc\": country,\n",
-                "    \"year_vtg\": vintage_years,\n",
-                "    \"year_act\": act_years,\n",
-                "    \"time\": \"year\",\n",
-                "    \"unit\": \"-\",\n",
-                "}\n",
-                "base_technical_lifetime = {\n",
-                "    \"node_loc\": country,\n",
-                "    \"year_vtg\": model_horizon,\n",
-                "    \"unit\": \"y\",\n",
-                "}\n",
-                "base_inv_cost = {\n",
-                "    \"node_loc\": country,\n",
-                "    \"year_vtg\": model_horizon,\n",
-                "    \"unit\": \"USD/kW\",\n",
-                "}\n",
-                "base_fix_cost = {\n",
-                "    \"node_loc\": country,\n",
-                "    \"year_vtg\": vintage_years,\n",
-                "    \"year_act\": act_years,\n",
-                "    \"unit\": \"USD/kW\",\n",
-                "}\n",
-                "base_var_cost = {\n",
-                "    \"node_loc\": country,\n",
-                "    \"year_vtg\": vintage_years,\n",
-                "    \"year_act\": act_years,\n",
-                "    \"mode\": \"standard\",\n",
-                "    \"time\": \"year\",\n",
-                "    \"unit\": \"USD/kWa\",\n",
-                "}"
+                "# We can see the elements of the set\n",
+                "scen.set(\"time\")"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## `\"addon\"` technology in MESSAGEix\n",
-                "This tutorial will extend the current reference-energy-system to include a demand for heat and the necessary technologies to meet this demand.  Heat will be generated via a passout-turbine which will be linked to the `\"coal_ppl\"` using the `\"addon\"` formulation.\n",
-                "\n",
-                "<img src='_static/addon_technologies_res.png' width='700'>\n",
-                "\n",
-                "We will therefore carry out the following three steps:\n",
-                "1. Define a new commodity and demand for heat:\n",
-                "    - Define new `\"commodity\"` `\"heat\"`.\n",
-                "    - Parametrize `\"demand\"` for `\"heat\"`.\n",
-                "    \n",
-                "    \n",
-                "2. Add new technologies:\n",
-                "    - add a new technology to generate heat: `\"passout-turbine\"`.\n",
-                "    - add a new technology district heat network to transport heat to the end-use technology: `\"dh_grid\"`.\n",
-                "    - add a new end-use technology, an in-house district heat connection which is linked to `\"demand\": \"hs_house\"`.\n",
-                "    \n",
-                "3. Link the passout-turbine to the coal_ppl using the `\"addon\"` feature."
+                "# Defining a new temporal level\n",
+                "time_level = \"season\"\n",
+                "scen.add_set(\"lvl_temporal\", time_level)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### 1: Define a new commodity and demand\n",
-                "We therefore add a new `\"commodity\"` `\"heat\"` and a corresponding demand, which will rise at the same rate as electricity demand."
+                "Next, the temporal hierarchy will be defined to map different levels of time with respect to `\"year\"`, which is the parent temporal level for any `\"time\"`. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Define a new commodity `\"heat\"`\n",
-                "scen.add_set(\"commodity\", [\"heat\"])\n",
-                "\n",
-                "# Add heat demand at the useful level\n",
-                "heat_demand = pd.DataFrame(\n",
-                "    {\n",
-                "        \"node\": country,\n",
-                "        \"commodity\": \"heat\",\n",
-                "        \"level\": \"useful\",\n",
-                "        \"year\": [700, 710, 720],\n",
-                "        \"time\": \"year\",\n",
-                "        \"value\": (25 * gdp_profile).round(),\n",
-                "        \"unit\": \"GWa\",\n",
-                "    }\n",
-                ")\n",
-                "scen.add_par(\"demand\", heat_demand)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### 2: Define new technologies\n",
+                "# Adding temporal hierarchy\n",
+                "for t in time_steps:\n",
+                "    scen.add_set(\"map_temporal_hierarchy\", [time_level, t, \"year\"])\n",
                 "\n",
-                "i. Heat will be generated via a pass-out turbine:\n",
-                "Passout-turbine (`\"po_turbine\"`) characteristics: The passout-turbine requires one unit of electricity to generate five units of heat. The lifetime is assumed to be 30 years, 10 years longer then that of `\"coal_ppl\"`.  Investment costs are 150\\\\$/kW compared to 500\\\\$/kW for `\"coal_ppl\"`.  A coal heatplant would have higher investment costs, approximately double that of \"po_turbine\". Lastly, `\"po_turbine\"` represents an alternative production mode of `\"coal_ppl\"`, hence in order to produce heat, the electricity of `\"coal_ppl\"` is reduced. Thus, electricity is parametrized as an input to `\"po_turbine\"`; for each unit of electricity, 5 units of heat can be produced. This will later also be used for establishing a \"link\" between `\"coal_ppl\"` and `\"po_turbine\"`.\n",
-                "\n",
-                "ii. Heat will be transported via a district heating grid:\n",
-                "District heat (`\"dh_grid\"`) network characteristics: District heating networks have only very low losses as these cover only short distances (within city perimeters). We will assume the district heating network to have an efficiency of 97%.\n",
-                "\n",
-                "iii. Heat demand will be linked to an end-use technology:\n",
-                "`\"hs_house\"` will represent the end-use technology, which distributed heat within the buildings."
+                "# We can see the content of the set\n",
+                "scen.set(\"map_temporal_hierarchy\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Similar to previous tutorials, we work our way backwards, starting from the `\"heat\"` demand defined at the `\"useful\"` energy level and connecting this to the `\"final\"` energy level via a technology, `\"hs_house\"`, representing the in-house heat distribution system."
+                "### Modifying parameters\n",
+                "In this section, we modify some parameters based on the new time steps. In principle, we need to examine all parameters that have an index of `\"time\"` to see if we need to modify them or not."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "tec = \"hs_house\"\n",
-                "scen.add_set(\"technology\", tec)\n",
-                "\n",
-                "hs_house_out = make_df(\n",
-                "    \"output\", **base_output, technology=tec, commodity=\"heat\", level=\"useful\", value=1.0\n",
-                ")\n",
-                "scen.add_par(\"output\", hs_house_out)\n",
+                "# All parameters with at least one sub-annual time index\n",
+                "parameters = [p for p in scen.par_list() if \"time\" in scen.idx_sets(p)]\n",
                 "\n",
-                "hs_house_in = make_df(\n",
-                "    \"input\",\n",
-                "    **base_input,\n",
-                "    technology=tec,\n",
-                "    commodity=\"heat\",\n",
-                "    level=\"final\",\n",
-                "    value=1.0,\n",
-                "    unit=\"-\"\n",
-                ")\n",
-                "scen.add_par(\"input\", hs_house_in)"
+                "# Those parameters with time index that are not empty in our model\n",
+                "[p for p in parameters if not scen.par(p).empty]"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Next, we add the information for the district heating network."
+                "### Parameter `duration_time`\n",
+                "We start by modifying the parameter `\"duration_time\"`, which shows the length of each subannual time step relative to the whole year:\n",
+                "\n",
+                "| Parameter | Index set| Explanation|\n",
+                "|:----------|:---------| :----------|\n",
+                "| duration_time\t| time\t|duration of sub-annual time slices (relative to 1)| \n",
+                "\n",
+                "In our example, winter and summer are each defined as half of the year. However, the duration of time steps can be\n",
+                "different in a MESSAGEix model, e.g., winter 0.4 and summer 0.6. Only the sum of the duration times must be equal to 1."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "tec = \"dh_grid\"\n",
-                "scen.add_set(\"technology\", tec)\n",
-                "\n",
-                "dh_grid_out = make_df(\n",
-                "    \"output\", **base_output, technology=tec, commodity=\"heat\", level=\"final\", value=1.0\n",
-                ")\n",
-                "scen.add_par(\"output\", dh_grid_out)\n",
-                "\n",
-                "dh_grid_in = make_df(\n",
-                "    \"input\",\n",
-                "    **base_input,\n",
-                "    technology=tec,\n",
-                "    commodity=\"heat\",\n",
-                "    level=\"secondary\",\n",
-                "    value=1.03,\n",
-                "    unit=\"-\",\n",
-                ")\n",
-                "scen.add_par(\"input\", dh_grid_in)"
+                "# Adding the duration time\n",
+                "for t in time_steps:\n",
+                "    scen.add_par(\"duration_time\", [t], 0.5, \"-\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Last, we add `\"po_turbine\"` as a technology."
+                "### A function for modifying parameters\n",
+                "At this stage, we introduce a function that helps us modify the parameters after adding new time steps. This function called `yearly_to_season` does the following:\n",
+                "- remove old values, where the `\"time\"` index was `\"year\"`\n",
+                "- populate data for new `\"time\"` indexes\n",
+                "- use the ratios defined by the user to convert yearly values to seasonal ones\n",
+                "\n",
+                "This is a common code pattern when modelling using MESSAGEix:\n",
+                "writing re-usable code that helps modify existing parameter data to reflect some desired change in the reference energy system."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "tec = \"po_turbine\"\n",
-                "scen.add_set(\"technology\", tec)\n",
-                "\n",
-                "po_out = make_df(\n",
-                "    \"output\",\n",
-                "    **base_output,\n",
-                "    technology=tec,\n",
-                "    commodity=\"heat\",\n",
-                "    level=\"secondary\",\n",
-                "    value=1.0,\n",
-                ")\n",
-                "scen.add_par(\"output\", po_out)\n",
-                "\n",
-                "po_in = make_df(\n",
-                "    \"input\",\n",
-                "    **base_input,\n",
-                "    technology=tec,\n",
-                "    commodity=\"electricity\",\n",
-                "    level=\"secondary\",\n",
-                "    value=0.2,\n",
-                "    unit=\"-\",\n",
-                ")\n",
-                "scen.add_par(\"input\", po_in)\n",
-                "\n",
-                "po_tl = make_df(\n",
-                "    \"technical_lifetime\", **base_technical_lifetime, technology=tec, value=30\n",
-                ")\n",
-                "scen.add_par(\"technical_lifetime\", po_tl)\n",
+                "# A function for adding sub-annual data to a parameter\n",
+                "def yearly_to_season(scen, parameter, data, filters=None):\n",
+                "    if filters:\n",
+                "        old = scen.par(parameter, filters)\n",
+                "    else:\n",
+                "        old = scen.par(parameter)\n",
+                "    scen.remove_par(parameter, old)\n",
                 "\n",
-                "po_inv = make_df(\"inv_cost\", **base_inv_cost, technology=tec, value=150)\n",
-                "scen.add_par(\"inv_cost\", po_inv)\n",
-                "\n",
-                "po_fix = make_df(\"fix_cost\", **base_fix_cost, technology=tec, value=15)\n",
-                "scen.add_par(\"fix_cost\", po_fix)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### 3: Link `\"po_turbine\"` with `\"coal_ppl\"`\n",
-                "`\"po_turbine\"` could already operate as all required parameters are defined, yet without a link to the activity of `\"coal_ppl\"`, `\"po_turbine\"` has the possibility of using electricity generated from either `\"coal_ppl\"` or `\"wind_ppl\"`.  But because `\"po_turbine\"` is an addon component to `\"coal_ppl\"` a distinct linkage needs to be established."
+                "    # Finding time related indexes\n",
+                "    time_idx = [x for x in scen.idx_names(parameter) if \"time\" in x]\n",
+                "    for h in data.keys():\n",
+                "        new = old.copy()\n",
+                "        for time in time_idx:\n",
+                "            new[time] = h\n",
+                "        new[\"value\"] = data[h] * old[\"value\"]\n",
+                "        scen.add_par(parameter, new)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "First, the newly added technology `\"po_turbine\"` needs to be classified as an `\"addon\"` technology"
+                "### Modifying electricity demand in sub-annual time steps\n",
+                "The seasonality in demand for electricity and lighting can be taken into account by estimating different values for each time step. For example, the share of electricity demand in winter and summer in Westeros is approximately 0.6 and 0.4 of the yearly demand. We can get the yearly demand from the baseline scenario and divide it to the two seasons according to their shares."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "scen.add_set(\"addon\", \"po_turbine\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Next, we need a new `\"type_addon\"`, which we will name `\"cogeneration_heat\"`.  We will classify the `\"po_turbine\"` via the *category* `\"addon\"` as one of the addon technologies as part of this specific `\"type_addon\"`.  In some cases, for example when modelling cooling technologies, multiple technologies can be classfied within a single `\"type_addon\"`.\n",
-                "\n",
-                "Via the set `\"map_tec_addon\"` we map the electricity generation technology, `\"coal_ppl\"`, to the `\"addon\"` technology, `\"po_turbine\"`. Multiple technologies, for example further fossil powerplants, could also be added to the this `\"type_addon\"` so as to be able to produce heat via `\"po_turbine\"`.\n",
-                "\n",
-                "Note: the `\"addon\"` technology as well as the parent technology must have the same `\"mode\"`."
+                "# Before modifying, let's look at the demand in the baseline\n",
+                "scen.par(\"demand\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "type_addon_ch = \"cogeneration_heat\"\n",
-                "addon_tech = \"po_turbine\"\n",
-                "tec = \"coal_ppl\"\n",
-                "scen.add_cat(\"addon\", type_addon_ch, addon_tech)\n",
-                "scen.add_set(\n",
-                "    \"map_tec_addon\", pd.DataFrame({\"technology\": tec, \"type_addon\": [type_addon_ch]})\n",
-                ")"
+                "# Modifying the demand for each season\n",
+                "demand_data = {\"winter\": 0.60, \"summer\": 0.40}\n",
+                "yearly_to_season(scen, \"demand\", demand_data)\n",
+                "\n",
+                "# Let's look at demand now\n",
+                "scen.par(\"demand\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The last step required in order to link the `\"coal_ppl\"` is to define the `\"addon_conversion\"` factor between the `\"coal_ppl\"` and the `\"type_addon\"`.  This is important, because the `\"coal_ppl\"` generates electricty while the `\"po_turbine\"` generates heat. Therefore, we can use the inverse of the `\"input\"` coefficient from the `\"po_turbine\"`."
+                "### Modifying `\"input\"` and `\"output\"`\n",
+                "However, not all parameters that have subannual time steps need to divide their annual values for each time step. For example, the `\"output\"` parameter shows the output efficiency, commodities and the level of a technology. Hence, as far as the efficiency of a technology remains unchanged in different seasons, the value of `\"output\"` will be the same. As such, we only need to add the sub-annual time steps but with the same value as for the yearly one."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df = pd.DataFrame(\n",
-                "    {\n",
-                "        \"node\": country,\n",
-                "        \"technology\": tec,\n",
-                "        \"year_vtg\": vintage_years,\n",
-                "        \"year_act\": act_years,\n",
-                "        \"mode\": \"standard\",\n",
-                "        \"time\": \"year\",\n",
-                "        \"type_addon\": type_addon_ch,\n",
-                "        \"value\": 5,\n",
-                "        \"unit\": \"-\",\n",
-                "    }\n",
-                ")\n",
-                "scen.add_par(\"addon_conversion\", df)"
+                "# Modifying input and output parameters for each season\n",
+                "fixed_data = {\"winter\": 1, \"summer\": 1}\n",
+                "# Output\n",
+                "yearly_to_season(scen, \"output\", fixed_data)\n",
+                "# Input\n",
+                "yearly_to_season(scen, \"input\", fixed_data)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Although not necessary for this specific example, it is also possible to limit the activity of `\"po_turbine\"` to a specific share of `\"coal_ppl\"` activity. In the example below, `\"po_turbine\"` is limited to using 15% of `\"coal_ppl\"` activity.  Likewise, a constraint on the minimum amount of electricity used from `\"po_turbine\"` can be applied by using the parameter `\"addon_lo\"`."
+                "### Modifying dynamic constraints\n",
+                "Next, we modify dynamic constraints with a `\"time\"` index, i.e. growth and decline rates of activities. In the Westeros baseline scenario, there is only `\"growth_activity_up\"`, so this parameter will be modified for seasonality but with the same values. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Index for \"addon_up\" is [\"node\", \"technology\", \"year_act\",\n",
-                "#                          \"mode\", \"time\", \"type_addon\",\n",
-                "#                          \"value\", \"unit\"]\n",
-                "df = pd.DataFrame(\n",
-                "    {\n",
-                "        \"node\": country,\n",
-                "        \"technology\": tec,\n",
-                "        \"year_act\": act_years,\n",
-                "        \"mode\": \"standard\",\n",
-                "        \"time\": \"year\",\n",
-                "        \"type_addon\": type_addon_ch,\n",
-                "        \"value\": 0.15,\n",
-                "        \"unit\": \"-\",\n",
-                "    }\n",
-                ")\n",
-                "scen.add_par(\"addon_up\", df)"
+                "# Modifying growth rates for each season\n",
+                "yearly_to_season(scen, \"growth_activity_up\", fixed_data)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Commit and solve"
+                "### Modifying capacity factor\n",
+                "We discussed the variation in the capacity factor of wind power in each month. By averaging the values for the respective months, we reach a capacity factor of 0.46 for winter and 0.25 for summer in Westeros.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "scen.commit(comment=\"define parameters for renewable implementation\")\n",
-                "scen.set_as_default()"
+                "# Modifying capacity factor\n",
+                "# Let's get the yearly capacity factor of wind in the baseline scenario\n",
+                "cf_wind = scen.par(\"capacity_factor\", {\"technology\": \"wind_ppl\"})[\"value\"].mean()\n",
+                "\n",
+                "# Converting yearly capacity factor to seasonal\n",
+                "cf_data = {\"winter\": 0.46 / cf_wind, \"summer\": 0.25 / cf_wind}\n",
+                "cf_filters = {\"technology\": \"wind_ppl\"}\n",
+                "yearly_to_season(scen, \"capacity_factor\", cf_data, cf_filters)\n",
+                "\n",
+                "# Capacity factor of other technologies remains unchanged in each season\n",
+                "cf_filters = {\"technology\": [\"coal_ppl\", \"bulb\", \"grid\"]}\n",
+                "yearly_to_season(scen, \"capacity_factor\", fixed_data, cf_filters)\n",
+                "\n",
+                "# Let's look at capacity factor in year 710\n",
+                "scen.par(\"capacity_factor\", {\"year_act\": 710, \"year_vtg\": 710})"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "scen.solve()"
+                "### Modifying historical activity\n",
+                "`\"historical_activity\"` is one of the parameters for which the data should be divided between the seasons. In the absence of recorded data in Westeros before 690, we assume historical values can be divided by half for each season:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "scen.var(\"OBJ\")[\"lvl\"]"
+                "# Modifying historical activity\n",
+                "hist_data = {\"winter\": 0.5, \"summer\": 0.5}\n",
+                "yearly_to_season(scen, \"historical_activity\", hist_data)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Plotting Results"
+                "### Economic parameters\n",
+                "Investment cost is defined per installed capacity per year and is not related to subannual time steps, so it remains unchanged. Variable cost is time-dependent so the `\"time\"` index should be updated. However, as variable cost is defined per unit of activity, the `value` can remain unchanged for different time steps."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Create a Reporter object to describe and carry out reporting\n",
-                "# calculations and operations (like plotting) based on `scenario`\n",
-                "from message_ix.reporting import Reporter\n",
-                "\n",
-                "rep_bl = Reporter.from_scenario(base)\n",
-                "rep_addon = Reporter.from_scenario(scen)\n",
-                "\n",
-                "# Add keys like \"plot activity\" to describe reporting operations.\n",
-                "# See tutorial/utils/plotting.py\n",
-                "from message_ix.util.tutorial import prepare_plots\n",
-                "\n",
-                "prepare_plots(rep_bl)\n",
-                "prepare_plots(rep_addon)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Activity\n",
-                "***"
+                "# Modifying variable cost\n",
+                "yearly_to_season(scen, \"var_cost\", fixed_data)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Scenario: '*baseline*'"
+                "### Solving the model"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rep_bl.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
-                "rep_bl.get(\"plot activity\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Scenario: '*addon_technology*'"
+                "scen.commit(comment=\"introducing seasonality\")\n",
+                "scen.set_as_default()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rep_addon.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
-                "rep_addon.get(\"plot activity\")"
+                "scen.solve()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rep_addon.set_filters(t=[\"po_turbine\"])\n",
-                "rep_addon.get(\"plot activity\")"
+                "scen.var(\"OBJ\")[\"lvl\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Question\n",
-                "Comparing the electricity generation of wind power plant in *baseline* and in this scenario, shows that wind is generating more. Can you explain the reason? You can find the answer at the end of this tutorial."
+                "## 3. Postprocessing and analyzing results\n",
+                "### Plotting results"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Capacity\n",
-                "***\n",
-                "The behavior observed for the activity of the two electricity generation technologies is reflected in the capacity."
+                "from message_ix.reporting import Reporter\n",
+                "from message_ix.util.tutorial import prepare_plots\n",
+                "\n",
+                "rep = Reporter.from_scenario(scen)\n",
+                "prepare_plots(rep)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Scenario: '*baseline*'"
+                "### Activity\n",
+                "\n",
+                "How much energy is generated in each time period from the different potential sources?"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rep_bl.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
-                "rep_bl.get(\"plot capacity\")"
+                "rep.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
+                "rep.get(\"plot activity\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Scenario: '*addon_technology*'"
+                "### Installed capacity\n",
+                "\n",
+                "Given how many new plants are built, how many are actually used?"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rep_addon.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
-                "rep_addon.get(\"plot capacity\")"
+                "rep.get(\"plot capacity\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Prices\n",
-                "***\n",
-                "The resulting impact on the electricity price though is negligable. Yet we can see that the prices of heat are significantly lower than that of light."
+                "### Electricity Price\n",
+                "\n",
+                "Electricity prices are **dual variables** of the optimization solution called **shadow prices** as well. They reflect the marginal cost of producing one more unit of electricity, hence, representing the marginal cost of the most expensive generator in the system.  "
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Scenario: '*baseline*'"
+                "rep.set_filters(t=None, c=[\"light\"])\n",
+                "rep.get(\"plot prices\")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "rep_bl.set_filters(c=[\"light\"])\n",
-                "rep_bl.get(\"plot prices\")"
+                "## Questions and discussion\n",
+                "1. Compare the objective value of this scenario with the baseline; which power system is more costly? Given the fact that electricity demand and the cost of technologies are equal between these two scenarios, how do you justify the change in the total costs?\n",
+                "\n",
+                "2. Compare the figure for \"Activity\" between this scenario and the baseline; do you observe any changes in the energy mix? The results show more wind integration in this scenario. What is the reason?\n",
+                " \n",
+                "3. If you check out the figure for \"Capacity\" in both scenarios, you'll notice that the increase in the installed capacity of wind is much higher than the growth in wind generation. Can you explain the reason?\n",
+                "\n",
+                "4. Rerun this tutorial for a scenario with 4 sub-annual time steps: winter, spring, summer and autumn (each one quarter of the whole year).\n",
+                "\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Scenario: '*addon_technology*'"
+                "### *Discussion*: \n",
+                "The greater availability of wind in wintertime coincides with the higher demand for electricity in winter compared to summer. Hence, when coal power plants are not able to cover the increased electricity demand in winter, the system needs more wind generation compared to the baseline (for example, see the results for \"Activity\" in 700):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rep_addon.set_filters(c=[\"light\"])\n",
-                "rep_addon.get(\"plot prices\")"
+                "scen.var(\"ACT\", {\"year_act\": 700})"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "rep_addon.set_filters(c=[\"heat\"])\n",
-                "rep_addon.get(\"plot prices\")"
+                "Adding seasonality to the model shows the impact of any coincidence or mismatch between wind generation and electricity demand. This seasonality can be averaged out if the yearly values are taken into account. The capacity factor of wind is different in winter and summer, while it was an average yearly value in the baseline scenario. Without any bound or tax on emissions, coal is the cheapest option. Wind will be installed only when coal cannot ramp up quickly to meet the whole demand, mainly in winter. Therefore, we observe relatively much higher installed capacity for wind compared in this scenario to the baseline, even though wind is more expensive. Thus, we see a more expensive system when considering seasonality (compare the objective values). "
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Answer to the question:\n",
-                "In the new scenario ('*add_technology*'), the effects of the addon technology can be seen when comparing the activity to the baseline scenario ('*baseline*'). From 700 onwards, the activity of the `\"wind_ppl\"` has increased to compensate for the electricity required from the `\"coal_ppl\"` for use in the `\"po_turbine\"`. In 720, when the `\"wind_ppl\"` is phased out, then more electricity is required to be produced by the `\"coal_ppl\"`. "
+                "### Final note\n",
+                "\n",
+                "Thank you for trying this tutorial!\n",
+                "\n",
+                "Check us out on Github: https://github.com/iiasa/message_ix  \n",
+                "\n",
+                "Get in touch with us online: https://groups.google.com/forum/message-ix  \n",
+                "\n",
+                "And feel free to contact us with any further questions or feedback for improving this tutorial: zakeri@iiasa.ac.at"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_baseline.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_baseline.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9567692792078953%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, '> $\\\\min \\\\quad ~c^T \\\\cdot X$  \\n'), (5, '> "*

 * *            "$~s.t. \\\\quad a \\\\cdot X \\\\leq b$\\n'), (14, '- decision **VARIABLES** ($X$) "*

 * *            "are capitalized\\n'), (15, '- input **parameters** ($a$, $b$) are lower case')], "*

 * *            "delete: [15, 14, 5, 4]}, 'attachments': OrderedDict()}, 19: {'source': {insert: [(1, "*

 * *            "'To first order, demand for services like electricity tracks with economic "*

 * *            "productivity (GDP) […]*

```diff
@@ -61,37 +61,38 @@
                 "\n",
                 "This tutorial is based on the country of Westeros from the TV show \"Game of Thrones\".\n",
                 "\n",
                 "<img src='_static/baseline_res.png' width='900'>"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "## MESSAGEix: the mathematical paradigm\n",
                 "\n",
                 "At its core, *MESSAGEix* is an optimization problem:\n",
                 "\n",
-                "> $\\min \\quad ~c^T \\cdot x$  \n",
-                "> $~s.t. \\quad A \\cdot x \\leq b$\n",
+                "> $\\min \\quad ~c^T \\cdot X$  \n",
+                "> $~s.t. \\quad a \\cdot X \\leq b$\n",
                 "\n",
                 "More explicitly, the model...\n",
                 "- optimizes an **objective function**, nominally minimizing total **system costs**\n",
                 "- under a system of **constraints** (inequalities or equality conditions)\n",
                 "\n",
                 "The mathematical implementation includes a number of features that make it particularly geared towards the modelling of *energy-water-land systems* in the context of *climate change mitigation and sustainable development*.\n",
                 "\n",
                 "Throughout this document, the mathematical formulation follows the convention that\n",
-                "- decision **VARIABLES** ($x$) are capitalized\n",
-                "- input **parameters** ($A$, $b$) are lower case"
+                "- decision **VARIABLES** ($X$) are capitalized\n",
+                "- input **parameters** ($a$, $b$) are lower case"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
@@ -304,23 +305,24 @@
                 }
             },
             "source": [
                 "## Supply and Demand (or Balancing Commodities)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "fragment"
                 }
             },
             "source": [
                 "The fundamental premise of the model is to satisfy demand for energy (services).\n",
-                "To first order, demand for services like electricity track with economic productivity (GDP).\n",
+                "To first order, demand for services like electricity tracks with economic productivity (GDP).\n",
                 "We define a GDP profile similar to first-world GDP growth from [1900-1930](https://en.wikipedia.org/wiki/List_of_regions_by_past_GDP):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -342,17 +344,17 @@
                 }
             },
             "source": [
                 "The `COMMODITY_BALANCE_GT` and `COMMODITY_BALANCE_LT` equations ensure that `\"demand\"` for each `\"commodity\"` is met at each `\"level\"` in the energy system.\n",
                 "The equation is copied below in this tutorial notebook, but every model equation is available for reference in\n",
                 "the [Mathematical formulation](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html) section of the *MESSAGEix* documentation.\n",
                 "\n",
-                "$\\sum_{\\substack{n^L,t,m \\\\ y^V \\leq y}} \\text{output}_{n^L,t,y^V,y,m,n,c,l} \\cdot \\text{ACT}_{n^L,t,y^V,y,m}$\n",
-                "$- \\sum_{\\substack{n^L,t,m, \\\\ y^V \\leq y}} \\text{input}_{n^L,t,y^V,y,m,n,c,l} \\cdot \\text{ACT}_{n^L,t,m,y}$  \n",
-                "$\\geq \\text{demand}_{n,c,l,y} \\quad \\forall \\ l \\in L$\n",
+                "$\\sum_{\\substack{n^L,t,m \\\\ y^V \\leq y}} \\mathrm{output}_{n^L,t,y^V,y,m,n,c,l} \\cdot \\mathrm{ACT}_{n^L,t,y^V,y,m}$\n",
+                "$- \\sum_{\\substack{n^L,t,m, \\\\ y^V \\leq y}} \\mathrm{input}_{n^L,t,y^V,y,m,n,c,l} \\cdot \\mathrm{ACT}_{n^L,t,m,y}$  \n",
+                "$\\geq \\mathrm{demand}_{n,c,l,y} \\quad \\forall \\ l \\in L$\n",
                 "\n",
                 "While `\"demand\"` must be met, supply can *exceed* demand allowing the model to plan for meeting demand in future periods by storing storable commodities.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -490,27 +492,28 @@
                 "base_input = make_df(\"input\", **base, node_origin=country, time_origin=\"year\")\n",
                 "\n",
                 "# Create a base data frame for different \"output\" parameter values\n",
                 "base_output = make_df(\"output\", **base, node_dest=country, time_dest=\"year\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "Working backwards along the Reference Energy System, we can add connections for the `\"bulb\"`. A light bulb\u2026\n",
                 "\n",
                 "- receives `\"input\"` in the form of the `\"electricity\"` `commodity` at the `\"final\"` energy `level`, and\n",
                 "- `\"output\"`s the `commodity` `\"light\"` at the `\"useful\"` energy `level`.\n",
                 "\n",
-                "The `value` in the input and output parameter is used to represent the effiecieny of a technology (efficiency = output/input).\n",
+                "The `value` in the input and output parameter is used to represent the efficiency of a technology (efficiency = output/input).\n",
                 "For example, input of 1.0 and output of 1.0 for a technology shows that the efficiency of that technology is 100% in converting\n",
                 "the input commodity to the output commodity."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -531,18 +534,19 @@
                 "bulb_in = base_input.assign(\n",
                 "    technology=\"bulb\", commodity=\"electricity\", level=\"final\", value=1.0\n",
                 ")\n",
                 "scenario.add_par(\"input\", bulb_in)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "If you don't know the dimensions for a specific parameter\u2014in other works, which keyword arguments you need to pass to `make_df()`, you can use `Scenario.idx_names()`:"
+                "If you don't know the dimensions for a specific parameter\u2014in other words, which keyword arguments you need to pass to `make_df()`, you can use `Scenario.idx_names()`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -588,22 +592,23 @@
                 "grid_in = base_input.assign(\n",
                 "    technology=\"grid\", commodity=\"electricity\", level=\"secondary\", value=1.0\n",
                 ")\n",
                 "scenario.add_par(\"input\", grid_in)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
-                "And finally, our power plants. The model does not include the fossil resources used as `\"input\"` for coal plants; however, costs of coal extraction are included in the parameter $variable\\_cost$."
+                "And finally, our power plants. The model does not include the fossil resources used as `\"input\"` for coal plants; however, costs of coal extraction are included in the parameter $\\mathrm{var\\_cost}$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "slideshow": {
@@ -639,27 +644,28 @@
                 }
             },
             "source": [
                 "## Operational Constraints and Parameters"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "fragment"
                 }
             },
             "source": [
                 "The model has a number of \"reality\" constraints, which relate built *capacity* (`CAP`) to available power, or the *activity* (`ACT`) of that technology.\n",
                 "\n",
-                "The **capacity constraint** limits the activity of a technology to the installed capacity multiplied by a capacity factor. Capacity factor or is the fraction of installed capacity that can be active in a certain period (here the sub-annual time step *h*).\n",
+                "The **capacity constraint** limits the activity of a technology to the installed capacity multiplied by a capacity factor. The capacity factor is the fraction of installed capacity that can be active in a certain period (here the sub-annual time step *h*).\n",
                 "\n",
-                "$$\\sum_{m} \\text{ACT}_{n,t,y^V,y,m,h}\n",
-                "    \\leq \\text{duration_time}_{h} \\cdot \\text{capacity_factor}_{n,t,y^V,y,h} \\cdot \\text{CAP}_{n,t,y^V,y}\n",
+                "$$\\sum_{m} \\mathrm{ACT}_{n,t,y^V,y,m,h}\n",
+                "    \\leq \\mathrm{duration\\_time}_{h} \\cdot \\mathrm{capacity\\_factor}_{n,t,y^V,y,h} \\cdot \\mathrm{CAP}_{n,t,y^V,y}\n",
                 "    \\quad t \\ \\in \\ T^{INV}$$\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
@@ -697,36 +703,37 @@
                 "        technology=tec,\n",
                 "        value=val,\n",
                 "    )\n",
                 "    scenario.add_par(\"capacity_factor\", df)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "The model can further be provided `\"technical_lifetime\"`s in order to properly manage deployed capacity and related costs via the **capacity maintenance** constraint:\n",
                 "\n",
-                "$\\text{CAP}_{n,t,y^V,y} \\leq \\text{remaining_capacity}_{n,t,y^V,y} \\cdot \\text{value} \\quad \\forall \\quad t \\in T^{INV}$\n",
+                "$\\mathrm{CAP}_{n,t,y^V,y} \\leq \\mathrm{remaining\\_capacity}_{n,t,y^V,y} \\cdot \\mathrm{value} \\quad \\forall \\quad t \\in T^{INV}$\n",
                 "\n",
                 "where `value` can take different forms depending on what time period is considered:\n",
                 "\n",
                 "| Value                                               | Condition                                           |\n",
                 "|:----------------------------------------------------|:----------------------------------------------------|\n",
-                "| $\\Delta_y \\text{historical_new_capacity}_{n,t,y^V}$ | $y$ is first model period                           |\n",
-                "| $\\Delta_y \\text{CAP_NEW}_{n,t,y^V}$                 | $y = y^V$                                           |\n",
-                "| $\\text{CAP}_{n,t,y^V,y-1}$                          | $0 < y - y^V < \\text{technical_lifetime}_{n,t,y^V}$ |\n",
+                "| $\\Delta_y \\mathrm{historical\\_new\\_capacity}_{n,t,y^V}$ | $y$ is first model period                           |\n",
+                "| $\\Delta_y \\mathrm{CAP\\_NEW}_{n,t,y^V}$                 | $y = y^V$                                           |\n",
+                "| $\\mathrm{CAP}_{n,t,y^V,y-1}$                          | $0 < y - y^V < \\mathrm{technical\\_lifetime}_{n,t,y^V}$ |\n",
                 "\n",
                 "\n",
-                "$\\text{CAP_NEW}_{n,t,y^V}$ is the newly installed capacity in one year, where as \n",
-                "$\\text{CAP}_{n,t,y^V,y-1}$ is the amount installed at the end of a (usually multi-year) period."
+                "$\\mathrm{CAP\\_NEW}_{n,t,y^V}$ is the newly installed capacity in one year, whereas \n",
+                "$\\mathrm{CAP}_{n,t,y^V,y-1}$ is the amount installed at the end of a (usually multi-year) period."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "slideshow": {
@@ -763,25 +770,26 @@
             "source": [
                 "## Technological Diffusion and Contraction\n",
                 "\n",
                 "We know from historical precedent that energy systems can not be transformed instantaneously. Therefore, we use a family of dynamic constraints on activity and capacity. These constraints define the upper and lower limit of the domain of activity and capacity over time based on their value in the previous time step, an initial value, and growth/decline rates."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "fragment"
                 }
             },
             "source": [
-                "$\\sum_{y^V \\leq y,m} \\text{ACT}_{n,t,y^V,y,m,h} \\leq$  \n",
-                "$\\text{initial_activity_up}_{n,t,y,h}\n",
-                "        \\cdot \\frac{ \\Big( 1 + growth\\_activity\\_up_{n,t,y,h} \\Big)^{|y|} - 1 }\n",
-                "                   { growth\\_activity\\_up_{n,t,y,h} }+ \\Big( 1 + growth\\_activity\\_up_{n,t,y,h} \\Big)^{|y|} \\cdot \\Big( \\sum_{y^V \\leq y-1,m} ACT_{n,t,y^V,y-1,m,h} + \\sum_{m} historical\\_activity_{n,t,y-1,m,h}\\Big)$  "
+                "$\\sum_{y^V \\leq y,m} \\mathrm{ACT}_{n,t,y^V,y,m,h} \\leq$  \n",
+                "$\\mathrm{initial\\_activity\\_up}_{n,t,y,h}\n",
+                "        \\cdot \\frac{ \\Big( 1 + \\mathrm{growth\\_activity\\_up}_{n,t,y,h} \\Big)^{|y|} - 1 }\n",
+                "                   { \\mathrm{growth\\_activity\\_up}_{n,t,y,h} }+ \\Big( 1 + \\mathrm{growth\\_activity\\_up}_{n,t,y,h} \\Big)^{|y|} \\cdot \\Big( \\sum_{y^V \\leq y-1,m} \\mathrm{ACT}_{n,t,y^V,y-1,m,h} + \\sum_{m} \\mathrm{historical\\_activity}_{n,t,y-1,m,h}\\Big)$  "
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
@@ -892,32 +900,33 @@
                 "        technology=tec,\n",
                 "        value=val,\n",
                 "    )\n",
                 "    scenario.add_par(\"historical_activity\", df)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "And the **new capacity** in the historic period.\n",
                 "\n",
-                "Remember $$\\sum_{m} \\text{ACT}_{n,t,y^V,y,m,h}\n",
-                "    \\leq \\text{duration_time}_{h} \\cdot \\text{capacity_factor}_{n,t,y^V,y,h} \\cdot \\text{CAP}_{n,t,y^V,y}\n",
+                "Remember $$\\sum_{m} \\mathrm{ACT}_{n,t,y^V,y,m,h}\n",
+                "    \\leq \\mathrm{duration\\_time}_{h} \\cdot \\mathrm{capacity\\_factor}_{n,t,y^V,y,h} \\cdot \\mathrm{CAP}_{n,t,y^V,y}\n",
                 "    \\quad t \\ \\in \\ T^{INV}$$\n",
                 "\n",
                 "and \n",
                 "\n",
-                "$$ \\text{CAP}_{n,t,y^V,y} = \\text{CAP_NEW}_{n,t,y^V} \\cdot \\text{duration_period}_{y} $$\n",
+                "$$ \\mathrm{CAP}_{n,t,y^V,y} = \\mathrm{CAP\\_NEW}_{n,t,y^V} \\cdot \\mathrm{duration\\_period}_{y} $$\n",
                 "\n",
                 "Since we want to get the activity during the whole historic year 690 and not of a sub-annual time slice, e.g., only spring (`duration_time` = 0.25), the `duration_time` is 1.  \n",
                 "\n",
-                "To get the new capacity in the historic period, the capacity, which needs to get build **per year** to meet the demand in the year 690, we resolve to the following:\n",
+                "To get the new capacity in the historic period, the capacity, which needs to get built **per year** to meet the demand in the year 690, we resolve to the following:\n",
                 "\n",
-                "$$\\text{CAP_NEW}_{n,t,y^V} = \\frac{\\sum_{m} \\text{ACT}_{n,t,y^V,y,m,h}}{\\text{duration_time}_{h} \\cdot \\text{duration_period}_{y}  \\cdot \\text{capacity_factor}_{n,t,y^V,y,h}} $$.\n",
+                "$$ \\mathrm{CAP\\_NEW}_{n,t,y^V} = \\frac{\\sum_{m} \\mathrm{ACT}_{n,t,y^V,y,m,h}}{\\mathrm{duration\\_time}_{h} \\cdot \\mathrm{duration\\_period}_{y}  \\cdot \\mathrm{capacity\\_factor}_{n,t,y^V,y,h}} $$ \n",
                 "\n",
                 "The `duration_period` of the first period (historic period) is set to the value that appears most frequently. Here every period has 10 years, so the `duration_period` of the first period is likewise 10 years."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -938,26 +947,27 @@
                 "        technology=tec,\n",
                 "        value=value,\n",
                 "    )\n",
                 "    scenario.add_par(\"historical_new_capacity\", df)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "## Objective Function\n",
                 "\n",
-                "The objective function drives the purpose of the optimization. Do we wish to seek maximum utility of the social planner, minimize carbon emissions, or something else? Classical IAMs seek to minimize total discounted system cost over space and time. \n",
+                "The objective function drives the purpose of the optimization. Do we wish to seek the maximum utility of the social planner, minimize carbon emissions, or something else? Classical IAMs seek to minimize total discounted system cost over space and time. \n",
                 "\n",
-                "$$\\min \\sum_{n,y \\in Y^{M}} \\text{interestrate}_{y} \\cdot \\text{COST_NODAL}_{n,y}$$\n"
+                "$$\\min \\sum_{n,y \\in Y^{M}} \\mathrm{interestrate}_{y} \\cdot \\mathrm{COST\\_NODAL}_{n,y}$$\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "fragment"
@@ -988,26 +998,27 @@
                 }
             },
             "source": [
                 "`COST_NODAL` is comprised of a variety of costs related to the use of different technologies."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "### Investment Costs\n",
                 "\n",
                 "Capital, or investment, costs are invoked whenever a new plant or unit is built\n",
                 "\n",
-                "$$\\text{inv_cost}_{n,t,y} \\cdot \\text{construction_time_factor}_{n,t,y} \\cdot \\text{CAP_NEW}_{n,t,y}$$"
+                "$$\\mathrm{inv\\_cost}_{n,t,y} \\cdot \\mathrm{construction\\_time\\_factor}_{n,t,y} \\cdot \\mathrm{CAP\\_NEW}_{n,t,y}$$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "slideshow": {
@@ -1035,40 +1046,41 @@
                 "        technology=tec,\n",
                 "        value=val,\n",
                 "    )\n",
                 "    scenario.add_par(\"inv_cost\", df)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "### Fixed O&M Costs\n",
                 "\n",
                 "Fixed cost are only relevant as long as the capacity is active. This formulation allows to include the potential cost savings from early retirement of installed capacity.\n",
                 "\n",
-                "$$\\sum_{y^V \\leq y} \\text{fix_cost}_{n,t,y^V,y} \\cdot \\text{CAP}_{n,t,y^V,y}$$"
+                "$$\\sum_{y^V \\leq y} \\mathrm{fix\\_cost}_{n,t,y^V,y} \\cdot \\mathrm{CAP}_{n,t,y^V,y}$$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "slideshow": {
                     "slide_type": "fragment"
                 }
             },
             "outputs": [],
             "source": [
                 "# in $ / kW / year (every year a fixed quantity is destinated to cover part of the O&M costs\n",
-                "# based on the size of the plant, e.g. lightning, labor, scheduled maintenance, etc.)\n",
+                "# based on the size of the plant, e.g. lighting, labor, scheduled maintenance, etc.)\n",
                 "\n",
                 "costs = {\n",
                 "    \"coal_ppl\": 30,\n",
                 "    \"wind_ppl\": 10,\n",
                 "}\n",
                 "\n",
                 "for tec, val in costs.items():\n",
@@ -1081,39 +1093,40 @@
                 "        technology=tec,\n",
                 "        value=val,\n",
                 "    )\n",
                 "    scenario.add_par(\"fix_cost\", df)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "### Variable O&M Costs\n",
                 "\n",
                 "Variable Operation and Maintence costs are associated with the costs of actively running the plant. Thus, they are not applied if a plant is on standby (i.e., constructed, but not currently in use).\n",
                 "\n",
-                "$$\\sum_{\\substack{y^V \\leq y \\\\ m,h}} \\text{var_cost}_{n,t,y^V,y,m,h} \\cdot \\text{ACT}_{n,t,y^V,y,m,h} $$"
+                "$$\\sum_{\\substack{y^V \\leq y \\\\ m,h}} \\mathrm{var\\_cost}_{n,t,y^V,y,m,h} \\cdot \\mathrm{ACT}_{n,t,y^V,y,m,h} $$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "slideshow": {
                     "slide_type": "fragment"
                 }
             },
             "outputs": [],
             "source": [
-                "# In $ / kWa (costs associated to the degradation of equipment\n",
+                "# In $ / kWa (costs associated with the degradation of equipment\n",
                 "# when the plant is functioning per unit of energy produced\n",
                 "# kW\u00b7year = 8760 kWh. Therefore the costs represents USD per 8760 kWh\n",
                 "# of energy). Do not confuse with fixed O&M units.\n",
                 "\n",
                 "costs = {\n",
                 "    \"coal_ppl\": 30,\n",
                 "    \"grid\": 50,\n",
@@ -1131,41 +1144,42 @@
                 "        technology=tec,\n",
                 "        value=val,\n",
                 "    )\n",
                 "    scenario.add_par(\"var_cost\", df)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
-                "A full model will also have costs associated with\n",
+                "A full model will not only have costs associated with technologies (investment, fixed, variable costs), but also\n",
                 "\n",
-                "- costs associated with technologies (investment, fixed, variable costs)\n",
-                "- resource extraction: $\\sum_{c,g} \\ resource\\_cost_{n,c,g,y} \\cdot EXT_{n,c,g,y} $\n",
+                "- resource extraction: $\\sum_{c,g} \\ \\mathrm{resource\\_cost}_{n,c,g,y} \\cdot \\mathrm{EXT}_{n,c,g,y} $\n",
                 "- emissions\n",
-                "- land use (emulator): $\\sum_{s} land\\_cost_{n,s,y} \\cdot LAND_{n,s,y}$"
+                "- land use (emulator): $\\sum_{s} \\mathrm{land\\_cost}_{n,s,y} \\cdot \\mathrm{LAND}_{n,s,y}$"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "## Time to Solve the Model\n",
                 "\n",
                 "First, we *commit* the model structure and input data (sets and parameters).\n",
-                "Because we created `scenario` with `version=\"new\"`, the `ixmp` storage back end automatically creates and assigns a new version number."
+                "Because we created `scenario` with `version=\"new\"`, the `ixmp` storage backend automatically creates and assigns a new version number."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "slideshow": {
@@ -1236,25 +1250,26 @@
             },
             "outputs": [],
             "source": [
                 "scenario.var(\"OBJ\")[\"lvl\"]"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "## Plotting Results\n",
                 "\n",
                 "Analyzing the results of a scenario after it is solved is called **reporting**.\n",
-                "MESSAGE*ix* includes flexible and customizable message_ix/tutorial for reporting, but here we wish to focus on the results of our example scenario.\n",
+                "MESSAGE*ix* includes a flexible and customizable message_ix/tutorial for reporting, but here we wish to focus on the results of our example scenario.\n",
                 "We use some custom code to set up some simple plots:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -1266,16 +1281,17 @@
             "source": [
                 "# Create a Reporter object to describe and carry out reporting\n",
                 "# calculations and operations (like plotting) based on `scenario`\n",
                 "from message_ix.reporting import Reporter\n",
                 "\n",
                 "rep = Reporter.from_scenario(scenario)\n",
                 "\n",
-                "# Add keys like \"plot activity\" to describe reporting operations.\n",
-                "# See tutorial/utils/plotting.py\n",
+                "# \"prepare_plots\" enables several to describe reporting operations, e.g.\n",
+                "# \"plot activity\", \"plot capacity\", or \"plot prices\"\n",
+                "# See message_ix/util/tutorial.py for more information\n",
                 "from message_ix.util.tutorial import prepare_plots\n",
                 "\n",
                 "prepare_plots(rep)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -1300,15 +1316,15 @@
             "metadata": {
                 "slideshow": {
                     "slide_type": "fragment"
                 }
             },
             "outputs": [],
             "source": [
-                "# Only show a subset of technologies in the follow plots;\n",
+                "# Only show a subset of technologies in the following plots;\n",
                 "# e.g. exclude \"bulb\" and \"grid\"\n",
                 "rep.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
                 "\n",
                 "# Trigger the calculation and plotting\n",
                 "rep.get(\"plot activity\")"
             ]
         },
@@ -1355,28 +1371,29 @@
             "outputs": [],
             "source": [
                 "# Create another plot. The same filters are still active.\n",
                 "rep.get(\"plot new capacity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "### Electricity Price\n",
                 "\n",
                 "And how much does the electricity cost? These prices are in fact **shadow prices** taken from the **dual variables** of the model solution.\n",
                 "They reflect the marginal cost of electricity generation (i.e., the additional cost of the system for supplying one more unit of\n",
                 "electricity), which is in fact the marginal cost of the most expensive operating generator.  \n",
                 "\n",
-                "Note the price drop when the more expensive technology, i.e., wind, is no longer being invested in the system."
+                "Note the price drop when the more expensive technology, i.e., wind, is no longer being invested in by the system."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "slideshow": {
@@ -1439,27 +1456,32 @@
                 "Check us out on Github at https://github.com/iiasa/message_ix and share your progress and questions in the [discussion forums](https://github.com/iiasa/message_ix/discussions)."
             ]
         }
     ],
     "metadata": {
         "anaconda-cloud": {},
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_baseline_demand.xlsx` & `message_ix-3.7.0/tutorial/westeros/westeros_baseline_technology_constraint.xlsx`

 * *Files 20% similar despite different names*

```diff
@@ -103,375 +103,375 @@
 00000660: ea93 cf9b 7fd7 96a6 e90d 3f88 394c ecd2  ..........?.9L..
 00000670: 9915 c873 6267 d9ae 7cc8 6c21 f5f9 1a55  ...sbg..|.l!...U
 00000680: 5368 3969 b062 9e72 3a22 795f 646c c0f3  Sh9i.b.r:"y_dl..
 00000690: 449b bf13 fd7c 2d4e 9cc8 5222 3412 f832  D....|-N..R"4..2
 000006a0: cf47 c725 a0f5 7f5a b434 f1cb 9d79 c437  .G.%...Z.4...y.7
 000006b0: 09c3 abc8 f0c9 828b 1fa8 de01 0000 ffff  ................
 000006c0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-000006d0: 597b 8763 c302 0000 6106 0000 0f00 0000  Y{.c....a.......
+000006d0: dbd9 233a d902 0000 8106 0000 0f00 0000  ..#:............
 000006e0: 786c 2f77 6f72 6b62 6f6f 6b2e 786d 6ca4  xl/workbook.xml.
-000006f0: 5551 6fda 3010 7e9f b4ff 60f9 9d26 0e10  UQo.0.~...`..&..
-00000700: d2a8 a16a cbd0 90b6 a9ea baf6 0509 99c4  ...j............
-00000710: 10ab 8e9d d90e 0455 fdef 3b07 02b4 bc74  .......U..;....t
-00000720: 6d04 76ec 4bbe fbee fcdd e5e2 b22e 045a  m.v.K..........Z
-00000730: 316d b892 0926 673e 464c a62a e372 99e0  1m...&g>FL.*.r..
-00000740: 3ff7 e34e 8491 b154 6654 28c9 12bc 6106  ?..N...TfT(...a.
-00000750: 5f0e bf7e b958 2bfd 3457 ea09 0180 3409  _..~.X+.4W....4.
-00000760: cead 2d63 cf33 69ce 0a6a ce54 c924 5816  ..-c.3i..j.T.$X.
-00000770: 4a17 d4c2 522f 3d53 6a46 3393 3366 0be1  J...R/=SjF3.3f..
-00000780: 05be 1f7a 05e5 126f 1162 fd1e 0cb5 58f0  ...z...o.b....X.
-00000790: 948d 545a 154c da2d 8866 825a a06f 725e  ..TZ.L.-.f.Z.or^
-000007a0: 9a16 ad48 df03 5750 fd54 959d 5415 2540  ...H..WP.T..T.%@
-000007b0: ccb9 e076 d380 6254 a4f1 6429 95a6 7301  ...v..bT..d)..s.
-000007c0: 61d7 a48f 6a0d bf10 fec4 8721 683d 81e9  a...j......!h=..
-000007d0: c455 c153 ad8c 5ad8 3380 f6b6 a44f e227  .U.S..Z.3....O.'
-000007e0: be47 c8ab 14d4 a739 781f 52cf d36c c5dd  .G.....9x.R..l..
-000007f0: 19ee 59e9 f083 acc2 3d56 7800 23fe a7d1  ..Y.....=Vx.#...
-00000800: 0848 abd1 4a0c c9fb 205a 7fcf 2dc0 c38b  .H..J... Z..-...
-00000810: 0517 ec61 2b5d 44cb f217 2ddc 4909 8c04  ...a+]D...-.I...
-00000820: 35f6 5bc6 2dcb 123c 80a5 5ab3 c346 0f23  5.[.-..<..Z..F.#
-00000830: 5d95 d715 1760 0dba 914f b037 dccb f956  ]....`...O.7...V
-00000840: a38c 2d68 25ec 3d08 b985 87ca 087a 4110  ..-h%.=......zA.
-00000850: ba27 4118 57c2 322d a965 374a 5ad0 e12e  .'A.W.2-.e7JZ...
-00000860: aecf 6aae c1be c915 281c ddb1 bf15 d70c  ..j.....(.......
-00000870: 0a0b f405 b1c2 48d3 98ce cd2d b539 aab4  ......H....-.9..
-00000880: 48f0 4d3c bd63 a59a 16cc 18ba 6433 5e4f  H.M<.c......d3^O
-00000890: 6d65 95e6 544c 5dc0 0c24 383d 5229 3d2d  me..TL]..$8=R)=-
-000008a0: 89ff d029 4d5d f01e 44bf 65b8 bd7f 9b09  ...)M]..D.e.....
-000008b0: 20aa e356 8bb7 5623 b89f 8c7e c079 fca6   ..V..V#...~.y..
-000008c0: 2b38 1dd0 40b6 2bde 09a4 3f9a 3d93 6ee8  +8..@.+...?.=.n.
-000008d0: 8fc7 61b7 731d f5a3 4eaf 7b0e 2da7 e70f  ..a.s...N.{.-...
-000008e0: 3aa4 fb8d 5c8d af82 f128 8a5e 200a 1dc6  :...\....(.^ ...
-000008f0: a9a2 95cd 7727 ee30 13dc 731a 7d6b fa49  ....w'.0..s.}k.I
-00000900: ebd6 42fc b8e2 d9c1 ffb3 bfbb 3a6e 7e33  ..B.........:n~3
-00000910: b4b6 1717 a9eb 6d0f 9cad cd41 1b6e 89ea  ......m....A.n..
-00000920: 472e 33b5 0645 f811 44b3 d92f a1a1 61b4  G.3..E..D../..a.
-00000930: 6e8c 8f3c b3b9 13d7 f960 bff7 9df1 650e  n..<.....`....e.
-00000940: 8c49 3008 fb18 d1d4 f215 bba7 73d8 7121  .I0.........s.q!
-00000950: 048e 6782 5ff1 1b6d f98d e1ea b8e1 153f  ..g._..m.......?
-00000960: ef88 60d3 5381 6833 23d9 d441 066d 5866  ..`.S.h3#..A.mXf
-00000970: d0bc 5dbf 75b9 0e80 8a8e 9d13 3dc9 1acd  ..].u.......=...
-00000980: 1f3f ceeb 99dd 946c 5640 2141 ef3f 7e0f  .?.....lV@!A.?~.
-00000990: f8ed df0b 1a11 b4fe 522a 5228 1837 390f  ........R*R(.79.
-000009a0: 5023 7d72 de3c d17e 1d86 ff00 0000 ffff  P#}r.<.~........
-000009b0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-000009c0: 4aa9 a661 fa00 0000 4703 0000 1a00 0801  J..a....G.......
-000009d0: 786c 2f5f 7265 6c73 2f77 6f72 6b62 6f6f  xl/_rels/workboo
-000009e0: 6b2e 786d 6c2e 7265 6c73 20a2 0401 28a0  k.xml.rels ...(.
-000009f0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
-00000a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006f0: 555d 6f9b 3014 7d9f b4ff 60f9 9d82 4942  U]o.0.}...`...IB
+00000700: 022a a9ba 7c68 91b6 a9ea baf6 2552 e480  .*..|h......%R..
+00000710: 13ac 0266 b649 88aa fef7 5d43 c847 f3d2  ...f.I....]C.G..
+00000720: b528 b1b1 af7d 7cae efb9 97eb 9b2a 4bd1  .(...}|......*K.
+00000730: 8649 c545 1e62 72e5 60c4 f248 c43c 5f87  .I.E.br.`..H.<_.
+00000740: f8cf c3d4 1a60 a434 cd63 9a8a 9c85 78c7  .....`.4.c....x.
+00000750: 14be 197e fd72 bd15 f279 29c4 3302 805c  ...~.r...y).3..\
+00000760: 8538 d1ba 086c 5b45 09cb a8ba 1205 cbc1  .8...l[E........
+00000770: b212 32a3 1a86 726d ab42 321a ab84 319d  ..2...rm.B2...1.
+00000780: a5b6 eb38 9e9d 519e e306 2190 efc1 10ab  ...8..Q...!.....
+00000790: 158f d858 4465 c672 dd80 4896 520d f455  ...XDe.r..H.R..U
+000007a0: c20b d5a2 65d1 7be0 322a 9fcb c28a 4456  ....e.{.2*....DV
+000007b0: 00c4 92a7 5cef 6a50 8cb2 2898 ad73 21e9  ....\.jP..(..s!.
+000007c0: 3205 b72b d243 9584 9f07 7fe2 40e3 b627  2..+.C......@..'
+000007d0: 81e9 e2a8 8c47 5228 b1d2 5700 6d37 a42f  .....GR(..W.m7./
+000007e0: fc27 8e4d c8d9 1554 9777 f03e a4ae 2dd9  .'.M...T.w.>..-.
+000007f0: 869b 181e 5849 ef83 acbc 0396 7704 23ce  ....XI......w.#.
+00000800: a7d1 0848 abd6 4a00 97f7 41b4 de81 9b8b  ...H..J...A.....
+00000810: 87d7 2b9e b2c7 46ba 8816 c52f 9a99 48a5  ..+...F..../..H.
+00000820: 18a5 54e9 49cc 358b 43dc 87a1 d8b2 e344  ..T.I.5.C......D
+00000830: 1723 5916 df4a 9e82 d5ed 0c1c 82ed e141  .#Y..J.........A
+00000840: ce77 12c5 6c45 cb54 3f80 905b 78c8 0cb7  .w..lE.T?..[x...
+00000850: ebba 9e59 09c2 b84d 3593 39d5 6c24 720d  ...Y...M5.9.l$r.
+00000860: 3adc fbf5 59cd d5d8 a344 80c2 d13d fb5b  :...Y....D...=.[
+00000870: 72c9 20b1 405f e02b b434 0ae8 52dd 519d  r. .@_.+.4..R.Q.
+00000880: a052 a621 1e05 f37b 5688 79c6 94a2 6bb6  .R.!...{V.y...k.
+00000890: e0d5 5c97 5a48 4ed3 b971 9881 04e7 272a  ..\.ZHN..q....'*
+000008a0: a597 29f1 1f3a a591 71de 06ef 1b86 cdfb  ..)..:..q.......
+000008b0: db9b 00a2 3268 b578 a725 82f7 d9f8 07c4  ....2h.x.%......
+000008c0: e337 dd40 7440 03f1 3e79 6770 fda4 b3c8  .7.@t@..>ygp....
+000008d0: 2319 90c5 cb37 7f32 980c faae e5dd 4e7d  #....7.2......N}
+000008e0: ab3b be25 964f dca9 3571 7bbd be3f f27b  .;.%.O..5q{..?.{
+000008f0: 5dcf 7905 67a4 1744 8296 3ad9 07de 4087  ].y.g..D..:...@.
+00000900: b86b a4fa d6f4 9356 ad85 3841 c9e3 238d  .k.....V..8A..#.
+00000910: 1767 ff58 a67f d3b4 b657 e3b0 2971 8f9c  .g.X.....W..)q..
+00000920: 6dd5 5122 6688 aa27 9ec7 621b e24e bf87  m.Q"f..'..b..N..
+00000930: d1ee 6cb4 ad4d 4f3c d689 5198 df07 af9b  ..l..MO<..Q.....
+00000940: b9ef 8caf 13e0 4bdc 8199 d474 796f 4a57  ......K....tyoJW
+00000950: 887d 9760 4423 cd37 ec81 2e61 81f1 c735  .}.`D#.7...a...5
+00000960: a443 7c46 76dc 909d c263 99e6 8cac 7dc2  .C|Fv....c....}.
+00000970: b6ae b3c0 baee 515e e7c6 5a8a ad4e 16f5  ......Q^..Z..N..
+00000980: 3950 e916 6501 c5dd d463 130b d724 4660  9P..e....c...$F`
+00000990: 0e94 b3b8 ce89 d3ad bc5a e85d c116 1924  .........Z.]...$
+000009a0: 1a7c 1b4e f675 3a27 fbdc 5a24 edd9 114d  .|.N.u:'..Z$...M
+000009b0: 2348 28d3 d5d1 76bb 3de2 d72b daaf c7f0  #H(...v.=..+....
+000009c0: 1f00 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+000009d0: 0800 0000 2100 4aa9 a661 fa00 0000 4703  ....!.J..a....G.
+000009e0: 0000 1a00 0801 786c 2f5f 7265 6c73 2f77  ......xl/_rels/w
+000009f0: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
+00000a00: 20a2 0401 28a0 0001 0000 0000 0000 0000   ...(...........
 00000a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000af0: 0000 bc92 cd6a c430 0c84 ef85 be83 d1bd  .....j.0........
-00000b00: 7192 fe50 ca3a 7b29 85bd b6db 0730 b112  q..P.:{).....0..
-00000b10: 874d 6c63 a93f 79fb 9a94 ee36 b0a4 97d0  .Mlc.?y....6....
-00000b20: a324 34f3 31cc 66fb 39f4 e21d 2375 de29  .$4.1.f.9...#u.)
-00000b30: 28b2 1c04 bada 9bce b50a 5ef7 4f57 f720  (.........^.OW. 
-00000b40: 88b5 33ba f70e 158c 48b0 ad2e 2f36 cfd8  ..3.....H.../6..
-00000b50: 6b4e 4f64 bb40 22a9 3852 6099 c383 9454  kNOd.@".8R`....T
-00000b60: 5b1c 3465 3ea0 4b97 c6c7 4173 1a63 2b83  [.4e>.K...As.c+.
-00000b70: ae0f ba45 59e6 f99d 8cbf 35a0 9a69 8a9d  ...EY.....5..i..
-00000b80: 5110 77e6 1ac4 7e0c c9f9 6f6d df34 5d8d  Q.w...~...om.4].
-00000b90: 8fbe 7e1b d0f1 190b c989 0b93 a08e 2db2  ..~...........-.
-00000ba0: 8269 fc5e 1659 0205 799e a15c 93e1 c3c7  .i.^.Y..y..\....
-00000bb0: 0359 443e 711c 5724 a74b b904 53fc 33cc  .YD>q.W$.K..S.3.
-00000bc0: 6232 b76b c290 d511 cd0b c754 3e3a a533  b2.k.......T>:.3
-00000bd0: 5b2f 2573 b32a 0c8f 7dea fab1 2b34 cd3f  [/%s.*..}...+4.?
-00000be0: f672 56ff ea0b 0000 ffff 0300 504b 0304  .rV.........PK..
-00000bf0: 1400 0600 0800 0000 2100 271c 6c8b 9302  ........!.'.l...
-00000c00: 0000 da07 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
-00000c10: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
-00000c20: 6d6c 9c55 d16e 9b30 147d 9fb4 7f40 7e4f  ml.U.n.0.}...@~O
-00000c30: 8c49 d236 08a8 baa6 cdfa 3069 9ab6 bd3b  .I.6......0i...;
-00000c40: c624 5601 33db 495a 4dfb f75d 4343 1cd3  .$V.3.IZM..]CC..
-00000c50: 4851 2302 c6e7 f8d8 e7fa fa92 dcbe 5465  HQ#...........Te
-00000c60: b0e3 4a0b 59a7 888c 4314 f09a c95c d4eb  ..J.Y...C....\..
-00000c70: 14fd faf9 38ba 4181 36b4 ce69 296b 9ea2  ....8.A.6..i)k..
-00000c80: 57ae d16d f6f9 53b2 97ea 596f 3837 0128  W..m..S...Yo87.(
-00000c90: d43a 451b 639a 1863 cd36 bca2 7a2c 1b5e  .:E.c..c.6..z,.^
-00000ca0: 0352 4855 5103 af6a 8d75 a338 cddb 4155  .RHUQ..j.u.8..AU
-00000cb0: 89a3 30bc c215 1535 ea14 6275 8986 2c0a  ..0....5..bu..,.
-00000cc0: c1f8 42b2 6dc5 6bd3 8928 5e52 03eb d71b  ..B.m.k..(^R....
-00000cd0: d1e8 835a c52e 91ab a87a de36 2326 ab06  ...Z.....z.6#&..
-00000ce0: 2456 a214 e6b5 1545 41c5 e2a7 752d 155d  $V.....EA...u-.]
-00000cf0: 95e0 fb85 4c29 0b5e 145c 11fc 2787 69da  ....L).^.\..'.i.
-00000d00: fec1 4c95 604a 6a59 9831 28e3 6ecd 43fb  ..L.`JjY.1(.n.C.
-00000d10: 733c c794 f54a 43ff 17c9 9029 567c 27ec  s<...JC....)V|'.
-00000d20: 061e a5a2 8f2d 89cc 7aad e828 36f9 a0d8  .....-..z..(6...
-00000d30: 552f 66c3 a5e2 adc8 53f4 377c fb8d e049  U/f.....S.7|...I
-00000d40: ec2d 1c91 09dc 0efd f6f9 0f65 492e 6087  .-.........eI.`.
-00000d50: adab 40f1 2245 7724 5e4e 11ce 9236 7f7e  ..@."Ew$^N...6.~
-00000d60: 0bbe d74e 3bb0 e9b8 92f2 d902 4f30 4d08  ...N;.......O0M.
-00000d70: 0a9a 979c d9c4 0828 3c76 fc9e 9765 8a96  .......(<v...e..
-00000d80: 640a 29fd a715 b56d 90c4 bda6 db3e e83f  d.)....m.....>.?
-00000d90: b629 fc5d 0539 2fe8 b634 3fe4 fe2b 17eb  .).].9/..4?..+..
-00000da0: 8d81 f332 0363 3633 e2fc 75c1 3583 9484  ...2.c63..u.5...
-00000db0: a9c7 d1ac 5fe8 821a 9a25 4aee 03d8 5e02  ...._....%J...^.
-00000dc0: 1337 d41e 1612 5f9f 1b99 25cc 72ef 2cb9  .7...._...%.r.,.
-00000dd0: 1d02 921a dcec b29b 04ef 6081 ec8d f165  ..........`....e
-00000de0: c898 9e32 ee87 8cab 53c6 62c8 084f 190f  ...2....S.b..O..
-00000df0: 4306 f128 8fef 50c8 a9ca f21d 4ad4 5330  C..(..P.....J.S0
-00000e00: c4a7 0f12 24de e541 0272 1f9e b917 1e17  ....$..A.r......
-00000e10: 9b79 8171 b16b 2f24 2ee6 d978 7031 3f0a  .y.q.k/$...xp1?.
-00000e20: 51bb 4924 f4fa 9727 7a93 f74d c301 b9dc  Q.I$...'z..M....
-00000e30: 3490 cf9a 7631 dfb4 8bf9 a65d ecb8 316d  4...v1.....]..1m
-00000e40: 263e b898 6f7a d299 9ef9 a6dd 31e4 8c69  &>..oz......1..i
-00000e50: 7b0e 2f3e 0e40 3e6b dac5 7cd3 2ee6 9b76  {./>.@>k..|....v
-00000e60: b1e3 1a3b d32e e69b 9e76 a6e7 be69 77cc  ...;.....v...iw.
-00000e70: c074 5764 ba7a d0d0 35ff 46d5 5ad4 3a28  .tWd.z..5.F.Z.:(
-00000e80: 79d1 160d 2808 aaab 2ae1 18da 4636 b694  y...(...*...F6..
-00000e90: 5c43 8559 4963 6475 78db c037 9443 8108  \C.YIcdux..7.C..
-00000ea0: c710 e342 4a73 78b1 85ac ff2a 67ff 0100  ...BJsx....*g...
-00000eb0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00000ec0: 0021 0052 bb24 fb4f 0200 0018 0500 0018  .!.R.$.O........
-00000ed0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00000ee0: 2f73 6865 6574 322e 786d 6c9c 945b 6f9b  /sheet2.xml..[o.
-00000ef0: 3018 86ef 27ed 3f58 be4f 0c34 2405 8554  0...'.?X.O.4$..T
-00000f00: 3934 5a2f 264d 3b5e 3be6 2358 c198 d9ce  94Z/&M;^;.#X....
-00000f10: a19a fadf f719 16d2 b5bd 882a 85c8 c62f  ...........*.../
-00000f20: cffb 9d60 7a77 5215 3980 b152 d719 0d87  ...`zwR.9..R....
-00000f30: 0125 500b 9dcb 7a9b d11f dfd7 835b 4aac  .%P...z......[J.
-00000f40: e375 ce2b 5d43 461f c1d2 bbd9 c70f d3a3  .u.+]CF.........
-00000f50: 363b 5b02 3882 84da 66b4 74ae 4919 b3a2  6;[.8...f.t.I...
-00000f60: 04c5 ed50 3750 e349 a18d e20e b766 cb6c  ...P7P.I.....f.l
-00000f70: 6380 e7ed 43aa 6251 108c 99e2 b2a6 1d21  c...C.bQ.......!
-00000f80: 35d7 3074 5148 012b 2df6 0a6a d741 0c54  5.0tQH.+-..j.A.T
-00000f90: dc61 fcb6 948d 3dd3 94b8 06a7 b8d9 ed9b  .a....=.........
-00000fa0: 81d0 aa41 c446 56d2 3db6 504a 9448 1fb6  ...A.FV.=.PJ.H..
-00000fb0: b536 7c53 61de a770 c405 3919 fc45 78dd  .6|Sa..p..9..Ex.
-00000fc0: 9c6d dafb af9c 9414 465b 5db8 2192 5917  .m......F[].!.Y.
-00000fd0: f3eb f413 9630 2e7a d2eb fcaf c284 2366  .....0.z......#f
-00000fe0: e020 7d03 2fa8 e87d 2185 71cf 8a2e b09b  . }./..}!.q.....
-00000ff0: 77c2 c63d cc97 cba4 7b99 67f4 cf22 9c27  w..=....{.g..".'
-00001000: cbdb 381c 24d1 fc66 304a e268 90ac ee27  ..8.$..f0J.h...'
-00001010: 8345 1cac e7f1 ea7e b15c 8c9f e86c 9a4b  .E.....~.\...l.K
-00001020: ecb0 cf8a 1828 323a 0fd3 4544 d96c dace  .....(2:..ED.l..
-00001030: cf4f 0947 fb6c 4d1c df7c 830a 8403 f408  .O.G.lM..|......
-00001040: 29f1 e3b9 d17a e785 0f78 2b40 a26d 059e  )....z...x+@.m..
-00001050: c885 9307 5842 5565 7415 6274 f677 6be2  ....XBUet.bt.wk.
-00001060: d768 c17a 8fe7 ebb3 dfba 1de9 2f86 e450  .h.z......../..P
-00001070: f07d e5be eae3 2790 dbd2 a171 8c89 fa49  .}....'....q...I
-00001080: 49f3 c715 5881 238a d6c3 28f6 54a1 2b44  I...X.#...(.T.+D
-00001090: e03f 51d2 bf6b 3862 fcd4 052b 7357 6634  .?Q..k8b...+sWf4
-000010a0: 4a28 d980 756b e951 9488 bd75 5afd ea0e  J(..uk.Q...uZ...
-000010b0: c336 b08e d186 b7e2 8ecf a646 1f09 0e0e  .6.........F....
-000010c0: aa6d c3fd 6b18 a6be 736f c680 e65e 3bf7  .m..k...so...^;.
-000010d0: e2f6 11b4 b158 97c3 2c1c 4dd9 0173 15ff  .....X..,.M..s..
-000010e0: 248b 3724 712f 6168 da3b a3db f5ce 28be  $.7$q/ah.;....(.
-000010f0: 784e 5e78 fe77 387e e1d6 b5a4 cbb9 e15b  xN^x.w8~.......[
-00001100: f8cc cd56 d696 5450 b425 9e50 62ba 1e04  ...V..TP.%.Pb...
-00001110: 435c 3bdd f8c2 4fb0 1f1b edb0 8ae7 5d89  C\;...O.......].
-00001120: 5f20 c022 0443 ec7a a1b5 3b6f 7cdb fb6f  _ .".C.z..;o|..o
-00001130: daec 2f00 0000 ffff 0300 504b 0304 1400  ../.......PK....
-00001140: 0600 0800 0000 2100 bda0 bfbd 4b07 0000  ......!.....K...
-00001150: 1d22 0000 1300 0000 786c 2f74 6865 6d65  ."......xl/theme
-00001160: 2f74 6865 6d65 312e 786d 6cec 5a4b 6f1b  /theme1.xml.ZKo.
-00001170: 3710 be17 e87f 20f6 9e58 b225 c732 2207  7..... ..X.%.2".
-00001180: 962c c549 fc82 ada4 c891 5a51 bbb4 b9cb  .,.I......ZQ....
-00001190: 0549 d9d1 ad48 8e05 0a14 4d8b 5e0a f4d6  .I...H....M.^...
-000011a0: 43d1 3640 02f4 92fe 1ab7 29da 14c8 5fe8  C.6@......)..._.
-000011b0: 905c 494b 8b8a adc6 455f 7680 781f df0c  .\IK....E_v.x...
-000011c0: e7cd d9a1 6fde 7a94 3074 4c84 a43c ad07  ....o.z.0tL..<..
-000011d0: e5eb a500 9134 e43d 9a46 f5e0 7ea7 7d6d  .....4.=.F..~.}m
-000011e0: 2540 52e1 b487 194f 493d 1812 19dc 5a7b  %@R....OI=....Z{
-000011f0: ffbd 9b78 55c5 2421 08e8 53b9 8aeb 41ac  ...xU.$!..S...A.
-00001200: 54b6 bab0 2043 788c e575 9e91 14de f5b9  T... Cx..u......
-00001210: 48b0 825b 112d f404 3e01 be09 5b58 2c95  H..[.-..>...[X,.
-00001220: 9617 124c d300 a538 01b6 bbfd 3e0d 09ea  ...L...8....>...
-00001230: 6896 c1da 8879 8bc1 6daa a47e 1032 71a0  h....y..m..~.2q.
-00001240: 5913 87c2 607b 4765 8d90 43d9 6402 1d63  Y...`{Ge..C.d..c
-00001250: 560f 609d 1e3f e990 472a 400c 4b05 2fea  V.`..?..G*@.K./.
-00001260: 41c9 fc04 0b6b 3717 f06a 4ec4 d40c da02  A....k7..jN.....
-00001270: 5ddb fce4 7439 41ef 68d1 ac29 a2ee 78d1  ]...t9A.h..)..x.
-00001280: 72bb 52bb b131 e66f 004c 4de3 5aad 56b3  r.R..1.o.LM.Z.V.
-00001290: 551e f333 001c 86a0 a995 a5c8 b3d2 5e29  U..3..........^)
-000012a0: 3746 3c0b 207b 39cd bb59 aa96 2a2e bec0  7F<. {9..Y..*...
-000012b0: 7f69 4ae6 5aa3 d1a8 d672 592c 5303 b297  .iJ.Z....rY,S...
-000012c0: 9529 fc4a 69b9 b2be e8e0 0dc8 e2ab 53f8  .).Ji.........S.
-000012d0: 4a63 bdd9 5c76 f006 64f1 cb53 f8f6 8dda  Jc..\v..d..S....
-000012e0: 72c5 c51b 50cc 687a 3485 d60e 6db7 73ee  r...P.hz4...m.s.
-000012f0: 6348 9fb3 4d2f 7c05 e02b a51c 3e41 4134  cH..M/|..+..>AA4
-00001300: 8ca3 4b2f d1e7 a99a 156b 093e e4a2 0d00  ..K/.....k.>....
-00001310: 0d64 58d1 14a9 6146 fa38 8428 6ee2 a42b  .dX...aF.8.(n..+
-00001320: 280e 5086 532e e141 69b1 d42e 2dc1 fffa  (.P.S..Ai...-...
-00001330: 5fc5 5c55 f4f2 7895 e002 9d7d 14ca a947  _.\U..x....}...G
-00001340: 5a12 2443 4133 550f ee02 d7a0 0079 f3f2  Z.$CA3U......y..
-00001350: db37 2f9f a337 2f9f 9d3e 7e71 faf8 87d3  .7/..7/..>~q....
-00001360: 274f 4e1f 7f6f 7939 849b 388d 8a84 afbf  'ON..oy9..8.....
-00001370: fee4 f72f 3f44 bf3d ffea f5d3 cffc 7859  .../?D.=......xY
-00001380: c4ff fcdd 473f fdf8 a91f 08f9 35d1 ffd5  ....G?......5...
-00001390: e7cf 7e79 f1ec d517 1fff facd 530f 7c5d  ..~y........S.|]
-000013a0: e06e 11de a109 9168 879c a07d 9e80 6ec6  .n.....h...}..n.
-000013b0: 30ae e4a4 2be6 a3e8 c498 3a14 3806 de1e  0...+.....:.8...
-000013c0: d62d 153b c09d 2166 3e5c 83b8 c67b 20a0  .-.;..!f>\...{ .
-000013d0: b4f8 80b7 0787 8eac 07b1 1828 ea59 f95e  ...........(.Y.^
-000013e0: 9c38 c06d ce59 830b af01 eee9 b50a 16ee  .8.m.Y..........
-000013f0: 0cd2 c8bf b818 1471 fb18 1ffb d66e e2d4  .......q.....n..
-00001400: 716d 6b90 414d 8590 9db6 7d33 268e 987b  qmk.AM....}3&..{
-00001410: 0ca7 0a47 2425 0ae9 77fc 8810 0fd9 434a  ...G$%..w.....CJ
-00001420: 1dbb 6ed3 5070 c9fb 0a3d a4a8 81a9 d724  ..n.Pp...=.....$
-00001430: 1dda 7502 6942 b449 13f0 cbd0 2720 b8da  ..u.iB.I....' ..
-00001440: b1cd f603 d4e0 cca7 f506 3976 9190 1098  ..........9v....
-00001450: 7984 ef10 e698 f136 1e28 9cf8 5876 70c2  y......6.(..Xvp.
-00001460: 8a06 dfc2 2af6 0979 3014 6111 d792 0a3c  ....*..y0.a....<
-00001470: 1d11 c651 ab47 a4f4 d1ec 0ad0 b7e0 f47b  ...Q.G.........{
-00001480: 18aa 99d7 eddb 6c98 b848 a1e8 918f e716  ......l..H......
-00001490: e6bc 88dc e047 cd18 2799 5766 9ac6 45ec  .....G..'.Wf..E.
-000014a0: 1d79 0421 8ad1 1e57 3ef8 3677 3344 df83  .y.!...W>.6w3D..
-000014b0: 1f70 3ad3 dd0f 2871 dc7d 7e21 b84f 2347  .p:...(q.}~!.O#G
-000014c0: a449 80e8 3703 e1f1 e56d c2dd 7c1c b23e  .I..7....m..|..>
-000014d0: 26be 2ab3 2e12 a7b0 ae43 0df7 4547 6310  &.*......C..EGc.
-000014e0: 39a1 bd45 08c3 27b8 4708 ba7f c723 4183  9..E..'.G....#A.
-000014f0: 678e cd27 42df 8da1 aa6c 125f 60dd c56e  g..'B....l._`..n
-00001500: acea fb94 48e8 8d74 3333 9da6 5b54 3a21  ....H..t33..[T:!
-00001510: 7b40 223e 439e ede1 99c2 33c4 6982 c52c  {@">C.....3.i..,
-00001520: ce3b e075 2774 616f f396 d25d 161e 1581  .;.u'tao...]....
-00001530: 3b14 7a3e 8817 af51 7625 f028 0477 6b16  ;.z>...Qv%.(.wk.
-00001540: d7bd 183b bb96 be97 fe78 1d0a c77f 17c9  ...;.....x......
-00001550: 31c8 cbc3 79f3 1268 c8dc 3450 d82f 6c9b  1...y..h..4P./l.
-00001560: 0e66 ce02 9380 e960 8ab6 7ce5 1648 1cf7  .f.....`..|..H..
-00001570: 4f48 f4be 6ac8 065e babe 9bb4 1337 4037  OH..j..^.....7@7
-00001580: e434 3909 4ddf d6f1 300a 0e3c d3f1 54af  .49.M...0..<..T.
-00001590: 3a1e dbb2 9ded 7866 5596 cd33 7dce 2cdc  :.....xfU..3}.,.
-000015a0: bfb0 bbd9 c083 748f c086 325d baae 9a9b  ......t...2]....
-000015b0: abe6 26f8 cf37 37b3 72f9 aaa5 b96a 69ae  ..&..77.r....ji.
-000015c0: 5a1a df47 d85f d2d2 4cba 1868 7026 131e  Z..G._..L..hp&..
-000015d0: 33ef 4966 8e7b fa94 b103 3564 644b 9a89  3.If.{....5ddK..
-000015e0: 8f84 0f9b 5e1b 1e9a 5194 9947 8ec7 7f59  ....^...Q..G...Y
-000015f0: 0c97 5a1f 58c0 c145 021b 1a24 b8fa 80aa  ..Z.X..E...$....
-00001600: f820 c619 0c87 ca66 7819 c99c 7524 51c6  . .....fx...u$Q.
-00001610: 25cc 8ccc 6333 4625 6778 9bc1 2885 9190  %...c3F%gx..(...
-00001620: 9971 56f5 f4cb da4f 62b5 cd7b f6f1 5271  .qV....Ob..{..Rq
-00001630: ca39 6663 a48a cc24 75b4 d092 6670 d1c5  .9fc...$u...fp..
-00001640: 966e bcdb 6265 2bd5 4cb3 b9aa 958d 68a6  .n..be+.L.....h.
-00001650: 6370 541b abac 4d3c b2fe 5835 7838 b626  cpT...M<..X5x8.&
-00001660: 7c31 23f8 ce06 2b2f c3b0 59cb 0e73 3468  |1#...+/..Y..s4h
-00001670: af7b daee d647 23b7 e8a5 2fd5 4532 866f  .{...G#.../.E2.o
-00001680: c2dc 475a ef69 1f95 8d93 46b1 32a5 88d6  ..GZ.i....F.2...
-00001690: c306 839e 589e e3a3 c26a 35cd f61d 56bb  ....X....j5...V.
-000016a0: 8893 8acb 5566 2c37 f2de bb78 6934 a69d  ....Uf,7...xi4..
-000016b0: 7849 e7ed 9974 6469 3139 598a 4eea 41ad  xI...tdi19Y.N.A.
-000016c0: ba58 0d50 88b3 7ad0 8701 2d5c 2619 785d  .X.P..z...-\&.x]
-000016d0: eaef 1dcc 2238 e508 95b0 617f 6e32 9b70  ...."8....a.n2.p
-000016e0: 9d78 b3e6 0fcb 32cc dcad dda7 1476 ea40  .x....2......v.@
-000016f0: 26a4 dac0 32b6 a161 5ee5 21c0 5233 4e36  &...2..a^.!.R3N6
-00001700: f22f 56c1 ac97 a580 a71a 5d4c 8aa5 1508  ./V.......]L....
-00001710: 86bf 4d0a b0a3 eb5a d2ef 9350 159d 5d78  ..M....Z...P..]x
-00001720: 62e6 e906 9097 523e 5044 1cc4 bd13 d465  b.....R>PD.....e
-00001730: 03b1 8fc1 fd3a 5441 9f1e 9530 4937 1541  .....:TA...0I7.A
-00001740: dfc0 a190 b6b6 79e5 16e7 3ce9 8a47 3106  ......y...<..G1.
-00001750: 679f 6396 c538 2fb7 3a45 4799 6ce1 a620  g.c..8/.:EG.l.. 
-00001760: 8d65 3077 565a 231e e8e6 95dd 2837 bf2a  .e0wVZ#.....(7.*
-00001770: 26e5 2f49 9562 18ff cf54 d1fb 098c b697  &./I.b...T......
-00001780: 7ada 0321 9c49 0a8c 74a6 d403 2e54 cca1  z..!.I..t....T..
-00001790: 0a65 310d db02 0e64 4ced 8068 8183 4578  .e1....dL..h..Ex
-000017a0: 0d41 0527 a3e6 b720 c7fa b7cd 39cb c3a4  .A.'... ....9...
-000017b0: 354c 28d5 3e8d 90a0 b01f a958 10b2 0765  5L(.>......X...e
-000017c0: c944 df39 ccca f9de 6559 b29c 91ed 3026  .D.9....eY....0&
-000017d0: e2ca cc8a dd25 c784 7574 0d5c d67b 7b80  .....%..ut.\.{{.
-000017e0: 6208 7553 4df2 3260 7067 e3cf bdcf 33a8  b.uSM.2`pg....3.
-000017f0: 1be9 26e7 9fda f9d8 649e b73d 98ec aa96  ..&.....d..=....
-00001800: fe82 bd48 a550 f40b 5b41 cdbb f799 9e6a  ...H.P..[A.....j
-00001810: 5c0e deb2 b1cf b9d5 da8a 35a5 f162 f5c2  \.........5..b..
-00001820: 5b6d 0607 1470 2ea9 2026 422a 4218 349a  [m...p.. &B*B.4.
-00001830: d617 bcdc e1fb 505b 119c 9adb f60a 4154  ......P[......AT
-00001840: 5fb3 8d07 d205 d296 c72e 344e f6a1 0d26  _.........4N...&
-00001850: cdca 765e 7977 7be9 6d14 9cad e69d ee78  ..v^yw{.m......x
-00001860: 5dc8 d23f d3e9 ce69 ec71 73e6 2ee7 e4e2  ]..?...i.qs.....
-00001870: dbbb cff9 8c9d 5bd8 b175 b1d3 f598 1a92  ......[..u......
-00001880: f66c 8aea f668 f421 631c 63fe 3ea3 f827  .l...h.!c.c.>..'
-00001890: 14bc 7b08 8ede 80c3 ea01 53d2 1e43 3f82  ..{.......S..C?.
-000018a0: e328 f8ca b0c7 dd90 fcd6 b986 74ed 0f00  .(..........t...
-000018b0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-000018c0: 0000 2100 296b b8a1 1c03 0000 2c08 0000  ..!.)k......,...
-000018d0: 0d00 0000 786c 2f73 7479 6c65 732e 786d  ....xl/styles.xm
-000018e0: 6cb4 556d 6bdb 3010 fe3e d87f 10fa eeca  l.Umk.0..>......
-000018f0: 76e3 2c09 b64b d3d4 50d8 c6a0 1dec ab62  v.,..K..P......b
-00001900: cb89 a85e 8cac 744e c7fe fb4e 7e49 5cda  ...^..tN...N~I\.
-00001910: 2d23 635f 12e9 747a eeb9 7bee e4f8 aa91  -#c_..tz..{.....
-00001920: 023d 3153 73ad 121c 5cf8 1831 95eb 82ab  .=1Ss...\..1....
-00001930: 4d82 bf3e 64de 0ca3 da52 5550 a115 4bf0  M..>d....RUP..K.
-00001940: 9ed5 f82a 7dff 2eae ed5e b0fb 2d63 1601  ...*}....^..-c..
-00001950: 84aa 13bc b5b6 5a10 52e7 5b26 697d a12b  ......Z.R.[&i}.+
-00001960: a6e0 a4d4 4652 0b5b b321 7565 182d 6a77  ....FR.[.!ue.-jw
-00001970: 490a 12fa fe94 48ca 15ee 1016 32ff 1b10  I.....H.....2...
-00001980: 49cd e3ae f272 2d2b 6af9 9a0b 6ef7 2d16  I....r-+j...n.-.
-00001990: 4632 5fdc 6d94 3674 2d80 6a13 4c68 8e9a  F2_.m.6t-.j.Lh..
-000019a0: 606a 42d4 9821 486b 7d15 47f2 dce8 5a97  `jB..!Hk}.G...Z.
-000019b0: f602 7089 2e4b 9eb3 d774 e764 4e68 7e44  ..p..K...t.dNh~D
-000019c0: 02e4 f390 8288 f8e1 8bdc 1b73 26d2 8418  ...........s&...
-000019d0: f6c4 9d7c 388d 4bad 6c8d 72bd 5336 c121  ...|8.K.l.r.S6.!
-000019e0: 1075 2558 3c2a fd5d 65ee 0814 eebd d2b8  .u%X<*.]e.......
-000019f0: 7e46 4f54 8025 c024 8d73 2db4 4116 a483  ~FOT.%.$.s-.A...
-00001a00: cab5 1645 25eb 3c6e a8e0 6bc3 9d5b 4925  ...E%.<n..k..[I%
-00001a10: 17fb ce1c 3a43 ab76 ef27 39d4 de19 89e3  ....:C.v.'9.....
-00001a20: d1b1 49e3 b5f3 faef b1da 9035 c4e4 428c  ..I........5..B.
-00001a30: 2ad0 19d2 185a c532 a332 3845 fdfa 615f  *....Z.2.28E..a_
-00001a40: 41aa 0aba baa3 0c47 27bd 3786 ee83 301a  A......G'.7...0.
-00001a50: 5d20 6d40 c852 9b02 a6e8 58fb c194 c682  ] m@.R....X.....
-00001a60: 9516 6a60 f866 ebfe adae e077 adad 854e  ..j`.f.....w...N
-00001a70: 4be3 82d3 8d56 54b8 b275 202f 6fc2 f4c1  K....VT..u /o...
-00001a80: a025 d86e 6150 069d e8ce ea5e 26e2 e07b  .%.naP.....^&..{
-00001a90: f493 be2d 8796 c249 57a0 39b0 3ce9 db25  ...-...IW.9.<..%
-00001aa0: f376 2e7d 5220 4dce 84b8 77c9 7c2b 0f75  .v.}R M...w.|+.u
-00001ab0: 72ed d894 48ed 6426 ed5d 9160 787f 5cf3  r...H.d&.].`x.\.
-00001ac0: 0c4b 10a5 5f76 b5e9 36ae 5663 b40e 7b04  .K.._v..6.Vc..{.
-00001ad0: 1b9e 058b 9af2 80ff 3b52 01f0 7b8b 14d8  ........;R..{...
-00001ae0: 87db 8856 95d8 bb79 7312 75bb 65db 1ec7  ...V...ys.u.e...
-00001af0: fdb5 e01b 2559 e792 c630 60dd 166d b5e1  ....%Y...0`..m..
-00001b00: cf70 d54d 660e e70c 1e2e 789e 2dcf 9d05  .p.Mf.....x.-...
-00001b10: 4469 7baf 29fb 0a40 cea3 c2be 28eb a140  Di{.)..@....(..@
-00001b20: c84d 7282 3fbb 8758 8c68 ae77 5c58 aede  .Mr.?..X.h.w\X..
-00001b30: 2829 6016 cd51 24df c5b4 ee51 6de5 3b44  ()`..Q$....Qm.;D
-00001b40: 01ad 0a56 d29d b00f 87c3 041f d79f 58c1  ...V..........X.
-00001b50: 7772 7ef0 fac2 9fb4 6d21 127c 5c7f 7473  wr~.....m!.|\.ts
-00001b60: 114c 5d0c d6d8 8f35 3433 fca3 9de1 09fe  .L]....543......
-00001b70: 71bb fc30 5fdd 66a1 37f3 9733 6f72 c922  q..0_.f.7..3or."
-00001b80: 6f1e 2d57 5e34 b959 ae56 d9dc 0ffd 9b9f  o.-W^4.Y.V......
-00001b90: a3a7 fd1f 1ef6 f64b 04dd 184c 16b5 80e7  .......K...L....
-00001ba0: dff4 c9f6 29de 1f6d 091e 6d3a faad 2a40  ....)..m..m:..*@
-00001bb0: 7bcc 7d1e 4efd eb28 f0bd ecd2 0fbc c994  {.}.N..(........
-00001bc0: cebc d9f4 32f2 b228 0857 d3c9 f236 caa2  ....2..(.W...6..
-00001bd0: 11f7 e8cc 0f80 4f82 a0fb 9438 f2d1 c272  ......O....8...r
-00001be0: c904 5783 5683 4263 2b88 04db 3f24 4106  ..W.V.Bc+...?$A.
-00001bf0: 25c8 f133 9ffe 0200 00ff ff03 0050 4b03  %..3.........PK.
-00001c00: 0414 0006 0008 0000 0021 0017 b4e6 faf4  .........!......
-00001c10: 0000 0018 0200 0014 0000 0078 6c2f 7368  ...........xl/sh
-00001c20: 6172 6564 5374 7269 6e67 732e 786d 6c64  aredStrings.xmld
-00001c30: d1c1 6ec3 200c 00d0 fba4 fd03 e2be 92e4  ..n. ...........
-00001c40: b075 13a1 8749 db0f 6cea 7142 c14d 90c0  .u...I..l.qB.M..
-00001c50: a4d8 899a bf1f 530f 93c2 d10f dbc2 b63e  ......S........>
-00001c60: dd62 102b 64f2 097b d91e 1a29 0087 e43c  .b.+d..{...)...<
-00001c70: 8ebd fcfe fa78 3a4a 416c d1d9 9010 7ab9  .....x:JAl....z.
-00001c80: 01c9 9379 7cd0 442c 4a2d 522f 27e6 f94d  ...y|.D,J-R/'..M
-00001c90: 291a 2688 960e 6906 2c2f 9794 a3e5 12e6  ).&...i.,/......
-00001ca0: 51d1 9cc1 3a9a 0038 06d5 35cd b38a d6a3  Q...:..8..5.....
-00001cb0: 1443 5a90 7bd9 bd4a b1a0 bf2e f07e 87f6  .CZ.{..J.....~..
-00001cc0: 288d 266f 349b 0d6c d68a 8d56 7ff1 dd5e  (.&o4..l...V...^
-00001cd0: 9aa6 a2b6 a6ae a221 c558 86e3 6d5f 1efc  .......!.X..m_..
-00001ce0: 3871 85b0 42d8 e342 7059 2ac5 e460 9f79  8q..B..BpY*..`.y
-00001cf0: 0662 c889 f6ce 3e56 b9ab 0d4b 8565 25d5  .b....>V...K.e%.
-00001d00: 9f3e cf76 dfcf 33c4 ca6e 3fbc cd55 c7b9  .>.v..3..n?..U..
-00001d10: dea5 2b47 43f7 5faf ca65 cd2f 0000 00ff  ..+GC._..e./....
-00001d20: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00001d30: 0004 da6b 1a4b 0100 0063 0200 0011 0008  ...k.K...c......
-00001d40: 0164 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
-00001d50: 6d6c 20a2 0401 28a0 0001 0000 0000 0000  ml ...(.........
+00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b00: 0000 0000 0000 0000 bc92 cd6a c430 0c84  ...........j.0..
+00000b10: ef85 be83 d1bd 7192 fe50 ca3a 7b29 85bd  ......q..P.:{)..
+00000b20: b6db 0730 b112 874d 6c63 a93f 79fb 9a94  ...0...Mlc.?y...
+00000b30: ee36 b0a4 97d0 a324 34f3 31cc 66fb 39f4  .6.....$4.1.f.9.
+00000b40: e21d 2375 de29 28b2 1c04 bada 9bce b50a  ..#u.)(.........
+00000b50: 5ef7 4f57 f720 88b5 33ba f70e 158c 48b0  ^.OW. ..3.....H.
+00000b60: ad2e 2f36 cfd8 6b4e 4f64 bb40 22a9 3852  ../6..kNOd.@".8R
+00000b70: 6099 c383 9454 5b1c 3465 3ea0 4b97 c6c7  `....T[.4e>.K...
+00000b80: 4173 1a63 2b83 ae0f ba45 59e6 f99d 8cbf  As.c+....EY.....
+00000b90: 35a0 9a69 8a9d 5110 77e6 1ac4 7e0c c9f9  5..i..Q.w...~...
+00000ba0: 6f6d df34 5d8d 8fbe 7e1b d0f1 190b c989  om.4]...~.......
+00000bb0: 0b93 a08e 2db2 8269 fc5e 1659 0205 799e  ....-..i.^.Y..y.
+00000bc0: a15c 93e1 c3c7 0359 443e 711c 5724 a74b  .\.....YD>q.W$.K
+00000bd0: b904 53fc 33cc 6232 b76b c290 d511 cd0b  ..S.3.b2.k......
+00000be0: c754 3e3a a533 5b2f 2573 b32a 0c8f 7dea  .T>:.3[/%s.*..}.
+00000bf0: fab1 2b34 cd3f f672 56ff ea0b 0000 ffff  ..+4.?.rV.......
+00000c00: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00000c10: f8a1 9805 ab02 0000 bb09 0000 1800 0000  ................
+00000c20: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00000c30: 6565 7431 2e78 6d6c 9c96 5d6f 9b30 1885  eet1.xml..]o.0..
+00000c40: ef27 ed3f 20df 0703 f96a 11a1 ea96 46eb  .'.? ....j....F.
+00000c50: c5a4 69da 76ef 8049 ac02 46b6 93b4 9af6  ..i.v..I..F.....
+00000c60: dff7 1a1a e298 5aa2 8d12 089c e363 3ff6  ......Z......c?.
+00000c70: 4b9c e4ee b92a bd23 1592 f17a 8542 3f40  K....*.#...z.B?@
+00000c80: 1ead 339e b37a b742 bf7f 6d26 37c8 938a  ..3..z.B..m&7...
+00000c90: d439 2979 4d57 e885 4a74 977e fe94 9cb8  .9)yMW..Jt.~....
+00000ca0: 7892 7b4a 9507 09b5 5ca1 bd52 4d8c b1cc  x.{J....\..RM...
+00000cb0: f6b4 22d2 e70d ad41 29b8 a888 824b b1c3  .."....A)....K..
+00000cc0: b211 94e4 6da3 aac4 5110 2c70 4558 8dba  ....m...Q.,pEX..
+00000cd0: 8458 8cc9 e045 c132 bae6 d9a1 a2b5 ea42  .X...E.2.......B
+00000ce0: 042d 8982 f1cb 3d6b e439 adca c6c4 5544  .-....=k.9....UD
+00000cf0: 3c1d 9a49 c6ab 0622 b6ac 64ea a50d 455e  <..I..."..d...E^
+00000d00: 95c5 8fbb 9a0b b22d 81fb 399c 91cc 7b16  .......-..9...{.
+00000d10: f08e e033 3d77 d3de 1ff4 54b1 4c70 c90b  ...3=w....T.Lp..
+00000d20: e543 32ee c63c c4bf c5b7 9864 7dd2 907f  .C2..<.....d}...
+00000d30: 544c 38c3 821e 995e c04b 54f4 b121 85f3  TL8....^.KT..!..
+00000d40: 3e2b ba84 4d3f 18b6 e8c3 f474 89f8 c0f2  >+..M?.....t....
+00000d50: 15fa 1bbc be26 700e f521 9884 4b38 9cef  .....&p..!..K8..
+00000d60: ebf3 3f94 2639 8315 d654 9ea0 c50a dd87  ..?.&9...T......
+00000d70: f166 8970 9ab4 f5f3 87d1 9334 be7b ba1c  .f.p.......4.{..
+00000d80: b79c 3f69 e111 ba09 b415 0fbc 9bb6 1c7f  ..?i............
+00000d90: 082f a705 3994 ea27 3f7d a36c b757 50fb  ./..9..'?}.l.WP.
+00000da0: 7318 a45e e538 7f59 5399 4179 418c 1fcd  s..^.8.YS.AyA...
+00000db0: fb4e d744 9134 11fc e4c1 5285 f05c 3444  .N.D.4....R..\4D
+00000dc0: 177e 182f 5c2d d324 d3de 7b6d 6e9b 40a4  .~./\-.$..{mn.@.
+00000dd0: 04b6 637a 9be0 230c 307b 757c 193a 16d7  ..cz..#.0{u|.:..
+00000de0: 8eaf 4347 185c 5bd6 43cb fcda f1f0 4648  ..CG.\[.C.....FH
+00000df0: 786d d9bc 6189 7a0b 06fa 7e0a a044 c64f  xm..a.z...~..D.O
+00000e00: 0198 7bf8 9905 6f6a 4b0b dbd4 aca1 ae4d  ..{...ojK......M
+00000e10: cd9a 8b87 a89d e6c0 b7f1 aef2 a66f 8341  .............o.A
+00000e20: b98e 0703 b313 ccd4 6c30 53bb 4c70 5b2f  ........l0S.Lp[/
+00000e30: 6b53 b3c1 a60e 30b3 4de8 009b bd07 0ccc  kS....0.M.......
+00000e40: 4e30 53b3 c14c ed32 8e0e ccd4 6cb0 9903  N0S..L.2....l...
+00000e50: cc6c e302 8367 77fc 8a81 d909 666a 3756  .l...gw.....fj7V
+00000e60: 299a 9a5d 8aa6 6683 cd1d 6057 798e 1583  )..]..f...`Wy...
+00000e70: 9f96 f160 6076 8299 9a0d 666a 7629 9a9a  ...``v....fjv)..
+00000e80: 0db6 7080 996d 5c2b b67c 0f18 989d 60a6  ..p..m\+.|....`.
+00000e90: 6683 999a 5d8a a666 832d 1d60 669b 0158  f...]..f.-.`f..X
+00000ea0: b7db 749b 4443 76f4 3b11 3b56 4baf a445  ..t.DCv.;.;VK..E
+00000eb0: bb93 4063 d16d 3581 af83 78a3 f797 2554  ..@c.m5...x...%T
+00000ec0: c196 2bc5 abf3 d51e fe24 51d8 3502 1f1e  ..+......$Q.5...
+00000ed0: e982 7375 bed0 3b5a ffb7 2bfd 0f00 00ff  ..su..;Z..+.....
+00000ee0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00000ef0: 0002 c6a1 3716 0200 00ce 0400 0018 0000  ....7...........
+00000f00: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00000f10: 6865 6574 322e 786d 6c9c 944b 6f9c 3010  heet2.xml..Ko.0.
+00000f20: c7ef 95fa 1d2c df77 0d64 1f0d 02a2 a4ab  .....,.w.d......
+00000f30: a87b a854 a58f bbd7 0c60 2dc6 d4f6 be54  .{.T.....`-....T
+00000f40: f5bb 770c 814d b339 ac82 788c f1f8 f79f  ..w..M.9..x.....
+00000f50: 190f 2477 4755 933d 182b 7593 d270 1a50  ..$wGU.=.+u..p.P
+00000f60: 028d d0b9 6cca 94fe fcf1 38f9 4489 75bc  ....l.....8.D.u.
+00000f70: c979 ad1b 48e9 092c bdcb 3e7e 480e da6c  .y..H..,..>~H..l
+00000f80: 6d05 e008 121a 9bd2 cab9 3666 cc8a 0a14  m.........6f....
+00000f90: b753 dd42 8333 8536 8a3b 1c9a 92d9 d600  .S.B.3.6.;......
+00000fa0: cfbb 45aa 6651 102c 98e2 b2a1 3d21 36d7  ..E.fQ.,....=!6.
+00000fb0: 3074 5148 012b 2d76 0a1a d743 0cd4 dc61  0tQH.+-v...C...a
+00000fc0: fcb6 92ad 1d68 4a5c 8353 dc6c 77ed 4468  .....hJ\.S.lw.Dh
+00000fd0: d522 6223 6be9 4e1d 9412 25e2 75d9 68c3  ."b#k.N...%.u.h.
+00000fe0: 3735 e67d 0c67 5c90 a3c1 33c2 eb66 90e9  75.}.g\...3..f..
+00000ff0: de5f 2829 298c b6ba 7053 24b3 3ee6 cbf4  ._())...pS$.>...
+00001000: 6fd9 2de3 6224 5de6 7f15 269c 3103 7be9  o.-.b$]...&.1.{.
+00001010: 37f0 8c8a de17 5238 1f59 d119 76f3 4ed8  7.....R8.Y..v.N.
+00001020: 6284 f972 9978 27f3 94fe 099e 8f09 3e43  b..r.x'.......>C
+00001030: 7f0b 26d8 0a41 670d 737f 6996 e412 77d8  ..&..Ag.s.i...w.
+00001040: 6745 0c14 29bd 0fe3 8788 b22c e9fa e797  gE..)......,....
+00001050: 8483 7d61 13c7 37df a106 e100 3542 4a7c  ..}a..7.....5BJ|
+00001060: 7b6e b4de 7ac7 35be 0a90 683b 074f e4c2  {n..z.5...h;.O..
+00001070: c93d 7c86 ba4e e93a 5c62 8bff ee44 bc8d  .=|..N.:\b...D..
+00001080: 126c d478 690f 7a8f 5d4b 7f33 2487 82ef  .l.xi.z.]K.3$...
+00001090: 6af7 a40f 5f40 9695 43e1 3926 ea3b 25ce  j..._@..C.9&.;%.
+000010a0: 4f2b b002 5b14 a5a7 d17c 0c7c c51d cf12  O+..[....|.|....
+000010b0: a30f 04b7 1be3 b42d f71f 4f18 fb7a bfb9  .......-..O..z..
+000010c0: 324b 84f7 bdf7 cedd 1244 5acc 669f 85b3  2K.......DZ.f...
+000010d0: 84ed 3142 f1ec f2f0 86cb 7c74 6128 3a2a  ..1B......|ta(:*
+000010e0: a3da f5ca e87c d65c bcd2 fc6f 72f9 4aad  .....|.\...or.J.
+000010f0: 2f64 9f73 cb4b f8ca 4d29 1b4b 6a28 bac2  /d.s.K..M).Kj(..
+00001100: 60e5 4d5f b960 8ab6 d3ad 2fd7 12ab b8d1  `.M_.`..../.....
+00001110: ce69 358c 2afc 6f00 1621 9862 2715 5abb  .i5.*.o..!.b'.Z.
+00001120: 61e0 376b fc13 65ff 0000 00ff ff03 0050  a.7k..e........P
+00001130: 4b03 0414 0006 0008 0000 0021 00bd a0bf  K..........!....
+00001140: bd4b 0700 001d 2200 0013 0000 0078 6c2f  .K...."......xl/
+00001150: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
+00001160: ec5a 4b6f 1b37 10be 17e8 7f20 f69e 58b2  .ZKo.7..... ..X.
+00001170: 25c7 3222 0796 2cc5 49fc 82ad a4c8 915a  %.2"..,.I......Z
+00001180: 51bb b4b9 cb05 49d9 d1ad 488e 050a 144d  Q.....I...H....M
+00001190: 8b5e 0af4 d643 d136 4002 f492 fe1a b729  .^...C.6@......)
+000011a0: da14 c85f e890 5c49 4b8b 8aad c645 5f76  ..._..\IK....E_v
+000011b0: 8078 1fdf 0ce7 cdd9 a16f de7a 9430 744c  .x.......o.z.0tL
+000011c0: 84a4 3cad 07e5 eba5 0091 34e4 3d9a 46f5  ..<.......4.=.F.
+000011d0: e07e a77d 6d25 4052 e1b4 8719 4f49 3d18  .~.}m%@R....OI=.
+000011e0: 1219 dc5a 7bff bd9b 7855 c524 2108 e853  ...Z{...xU.$!..S
+000011f0: b98a eb41 ac54 b6ba b020 4378 8ce5 759e  ...A.T... Cx..u.
+00001200: 9114 def5 b948 b082 5b11 2df4 043e 01be  .....H..[.-..>..
+00001210: 095b 582c 9596 1712 4cd3 00a5 3801 b6bb  .[X,....L...8...
+00001220: fd3e 0d09 ea68 96c1 da88 798b c16d aaa4  .>...h....y..m..
+00001230: 7e10 3271 a059 1387 c260 7b47 658d 9043  ~.2q.Y...`{Ge..C
+00001240: d964 021d 6356 0f60 9d1e 3fe9 9047 2a40  .d..cV.`..?..G*@
+00001250: 0c4b 052f ea41 c9fc 040b 6b37 17f0 6a4e  .K./.A....k7..jN
+00001260: c4d4 0cda 025d dbfc e474 3941 ef68 d1ac  .....]...t9A.h..
+00001270: 29a2 ee78 d172 bb52 bbb1 31e6 6f00 4c4d  )..x.r.R..1.o.LM
+00001280: e35a ad56 b355 1ef3 3300 1c86 a0a9 95a5  .Z.V.U..3.......
+00001290: c8b3 d25e 2937 463c 0b20 7b39 cdbb 59aa  ...^)7F<. {9..Y.
+000012a0: 962a 2ebe c07f 694a e65a a3d1 a8d6 7259  .*....iJ.Z....rY
+000012b0: 2c53 03b2 9795 29fc 4a69 b9b2 bee8 e00d  ,S....).Ji......
+000012c0: c8e2 ab53 f84a 63bd d95c 76f0 0664 f1cb  ...S.Jc..\v..d..
+000012d0: 53f8 f68d da72 c5c5 1b50 cc68 7a34 85d6  S....r...P.hz4..
+000012e0: 0e6d b773 ee63 489f b34d 2f7c 05e0 2ba5  .m.s.cH..M/|..+.
+000012f0: 1c3e 4141 348c a34b 2fd1 e7a9 9a15 6b09  .>AA4..K/.....k.
+00001300: 3ee4 a20d 000d 6458 d114 a961 46fa 3884  >.....dX...aF.8.
+00001310: 286e e2a4 2b28 0e50 8653 2ee1 4169 b1d4  (n..+(.P.S..Ai..
+00001320: 2e2d c1ff fa5f c55c 55f4 f278 95e0 029d  .-..._.\U..x....
+00001330: 7d14 caa9 475a 1224 4341 3355 0fee 02d7  }...GZ.$CA3U....
+00001340: a000 79f3 f2db 372f 9fa3 372f 9f9d 3e7e  ..y...7/..7/..>~
+00001350: 71fa f887 d327 4f4e 1f7f 6f79 3984 9b38  q....'ON..oy9..8
+00001360: 8d8a 84af bffe e4f7 2f3f 44bf 3dff eaf5  ......../?D.=...
+00001370: d3cf fc78 59c4 fffc dd47 3ffd f8a9 1f08  ...xY....G?.....
+00001380: f935 d1ff d5e7 cf7e 79f1 ecd5 171f fffa  .5.....~y.......
+00001390: cd53 0f7c 5de0 6e11 dea1 0991 6887 9ca0  .S.|].n.....h...
+000013a0: 7d9e 806e c630 aee4 a42b e6a3 e8c4 983a  }..n.0...+.....:
+000013b0: 1438 06de 1ed6 2d15 3bc0 9d21 663e 5c83  .8....-.;..!f>\.
+000013c0: b8c6 7b20 a0b4 f880 b707 878e ac07 b118  ..{ ............
+000013d0: 28ea 59f9 5e9c 38c0 6dce 5983 0baf 01ee  (.Y.^.8.m.Y.....
+000013e0: e9b5 0a16 ee0c d2c8 bfb8 1814 71fb 181f  ............q...
+000013f0: fbd6 6ee2 d471 6d6b 9041 4d85 909d b67d  ..n..qmk.AM....}
+00001400: 3326 8e98 7b0c a70a 4724 250a e977 fc88  3&..{...G$%..w..
+00001410: 100f d943 4a1d bb6e d350 70c9 fb0a 3da4  ...CJ..n.Pp...=.
+00001420: a881 a9d7 241d da75 0269 42b4 4913 f0cb  ....$..u.iB.I...
+00001430: d027 20b8 dab1 cdf6 03d4 e0cc a7f5 0639  .' ............9
+00001440: 7691 9010 9879 84ef 10e6 98f1 361e 289c  v....y......6.(.
+00001450: f858 7670 c28a 06df c22a f609 7930 1461  .Xvp.....*..y0.a
+00001460: 11d7 920a 3c1d 11c6 51ab 47a4 f4d1 ec0a  ....<...Q.G.....
+00001470: d0b7 e0f4 7b18 aa99 d7ed db6c 98b8 48a1  ....{......l..H.
+00001480: e891 8fe7 16e6 bc88 dce0 47cd 1827 9957  ..........G..'.W
+00001490: 669a c645 ec1d 7904 218a d11e 573e f836  f..E..y.!...W>.6
+000014a0: 7733 44df 831f 703a d3dd 0f28 71dc 7d7e  w3D...p:...(q.}~
+000014b0: 21b8 4f23 47a4 4980 e837 03e1 f1e5 6dc2  !.O#G.I..7....m.
+000014c0: dd7c 1cb2 3e26 be2a b32e 12a7 b0ae 430d  .|..>&.*......C.
+000014d0: f745 4763 1039 a1bd 4508 c327 b847 08ba  .EGc.9..E..'.G..
+000014e0: 7fc7 2341 8367 8ecd 2742 df8d a1aa 6c12  ..#A.g..'B....l.
+000014f0: 5f60 ddc5 6eac eafb 9448 e88d 7433 339d  _`..n....H..t33.
+00001500: a65b 543a 217b 4022 3e43 9eed e199 c233  .[T:!{@">C.....3
+00001510: c469 82c5 2cce 3be0 7527 7461 6ff3 96d2  .i..,.;.u'tao...
+00001520: 5d16 1e15 813b 147a 3e88 17af 5176 25f0  ]....;.z>...Qv%.
+00001530: 2804 776b 16d7 bd18 3bbb 96be 97fe 781d  (.wk....;.....x.
+00001540: 0ac7 7f17 c931 c8cb c379 f312 68c8 dc34  .....1...y..h..4
+00001550: 50d8 2f6c 9b0e 66ce 0293 80e9 608a b67c  P./l..f.....`..|
+00001560: e516 481c f74f 48f4 be6a c806 5eba be9b  ..H..OH..j..^...
+00001570: b413 3740 37e4 3439 094d dfd6 f130 0a0e  ..7@7.49.M...0..
+00001580: 3cd3 f154 af3a 1edb b29d ed78 6655 96cd  <..T.:.....xfU..
+00001590: 337d ce2c dcbf b0bb d9c0 8374 8fc0 8632  3}.,.......t...2
+000015a0: 5dba ae9a 9bab e626 f8cf 3737 b372 f9aa  ]......&..77.r..
+000015b0: a5b9 6a69 ae5a 1adf 47d8 5fd2 d24c ba18  ..ji.Z..G._..L..
+000015c0: 6870 2613 1e33 ef49 668e 7bfa 94b1 0335  hp&..3.If.{....5
+000015d0: 6464 4b9a 898f 840f 9b5e 1b1e 9a51 9499  ddK......^...Q..
+000015e0: 478e c77f 590c 975a 1f58 c0c1 4502 1b1a  G...Y..Z.X..E...
+000015f0: 24b8 fa80 aaf8 20c6 190c 87ca 6678 19c9  $..... .....fx..
+00001600: 9c75 2451 c625 cc8c cc63 3346 2567 789b  .u$Q.%...c3F%gx.
+00001610: c128 8591 9099 7156 f5f4 cbda 4f62 b5cd  .(....qV....Ob..
+00001620: 7bf6 f152 71ca 3966 63a4 8acc 2475 b4d0  {..Rq.9fc...$u..
+00001630: 9266 70d1 c596 6ebc db62 652b d54c b3b9  .fp...n..be+.L..
+00001640: aa95 8d68 a663 7054 1bab ac4d 3cb2 fe58  ...h.cpT...M<..X
+00001650: 3578 38b6 267c 3123 f8ce 062b 2fc3 b059  5x8.&|1#...+/..Y
+00001660: cb0e 7334 68af 7bda eed6 4723 b7e8 a52f  ..s4h.{...G#.../
+00001670: d545 3286 6fc2 dc47 5aef 691f 958d 9346  .E2.o..GZ.i....F
+00001680: b132 a588 d6c3 0683 9e58 9ee3 a3c2 6a35  .2.......X....j5
+00001690: cdf6 1d56 bb88 938a cb55 662c 37f2 debb  ...V.....Uf,7...
+000016a0: 7869 34a6 9d78 49e7 ed99 7464 6931 3959  xi4..xI...tdi19Y
+000016b0: 8a4e ea41 adba 580d 5088 b37a d087 012d  .N.A..X.P..z...-
+000016c0: 5c26 1978 5dea ef1d cc22 38e5 0895 b061  \&.x]...."8....a
+000016d0: 7f6e 329b 709d 78b3 e60f cb32 ccdc addd  .n2.p.x....2....
+000016e0: a714 76ea 4026 a4da c032 b6a1 615e e521  ..v.@&...2..a^.!
+000016f0: c052 334e 36f2 2f56 c1ac 97a5 80a7 1a5d  .R3N6./V.......]
+00001700: 4c8a a515 0886 bf4d 0ab0 a3eb 5ad2 ef93  L......M....Z...
+00001710: 5015 9d5d 7862 e6e9 0690 9752 3e50 441c  P..]xb.....R>PD.
+00001720: c4bd 13d4 6503 b18f c1fd 3a54 419f 1e95  ....e.....:TA...
+00001730: 3049 3715 41df c0a1 90b6 b679 e516 e73c  0I7.A......y...<
+00001740: e98a 4731 0667 9f63 96c5 382f b73a 4547  ..G1.g.c..8/.:EG
+00001750: 996c e1a6 208d 6530 7756 5a23 1ee8 e695  .l.. .e0wVZ#....
+00001760: dd28 37bf 2a26 e52f 4995 6218 ffcf 54d1  .(7.*&./I.b...T.
+00001770: fb09 8cb6 977a da03 219c 490a 8c74 a6d4  .....z..!.I..t..
+00001780: 032e 54cc a10a 6531 0ddb 020e 644c ed80  ..T...e1....dL..
+00001790: 6881 8345 780d 4105 27a3 e6b7 20c7 fab7  h..Ex.A.'... ...
+000017a0: cd39 cbc3 a435 4c28 d53e 8d90 a0b0 1fa9  .9...5L(.>......
+000017b0: 5810 b207 65c9 44df 39cc caf9 de65 59b2  X...e.D.9....eY.
+000017c0: 9c91 ed30 26e2 cacc 8add 25c7 8475 740d  ...0&.....%..ut.
+000017d0: 5cd6 7b7b 8062 0875 534d f232 6070 67e3  \.{{.b.uSM.2`pg.
+000017e0: cfbd cf33 a81b e926 e79f daf9 d864 9eb7  ...3...&.....d..
+000017f0: 3d98 ecaa 96fe 82bd 48a5 50f4 0b5b 41cd  =.......H.P..[A.
+00001800: bbf7 999e 6a5c 0ede b2b1 cfb9 d5da 8a35  ....j\.........5
+00001810: a5f1 62f5 c25b 6d06 0714 702e a920 2642  ..b..[m...p.. &B
+00001820: 2a42 1834 9ad6 17bc dce1 fb50 5b11 9c9a  *B.4.......P[...
+00001830: dbf6 0a41 545f b38d 07d2 05d2 96c7 2e34  ...AT_.........4
+00001840: 4ef6 a10d 26cd ca76 5e79 777b e96d 149c  N...&..v^yw{.m..
+00001850: ade6 9dee 785d c8d2 3fd3 e9ce 69ec 7173  ....x]..?...i.qs
+00001860: e62e e7e4 e2db bbcf f98c 9d5b d8b1 75b1  ...........[..u.
+00001870: d3f5 981a 92f6 6c8a eaf6 68f4 2163 1c63  ......l...h.!c.c
+00001880: fe3e a3f8 2714 bc7b 088e de80 c3ea 0153  .>..'..{.......S
+00001890: d21e 433f 82e3 28f8 cab0 c7dd 90fc d6b9  ..C?..(.........
+000018a0: 8674 ed0f 0000 00ff ff03 0050 4b03 0414  .t.........PK...
+000018b0: 0006 0008 0000 0021 0029 6bb8 a11c 0300  .......!.)k.....
+000018c0: 002c 0800 000d 0000 0078 6c2f 7374 796c  .,.......xl/styl
+000018d0: 6573 2e78 6d6c b455 6d6b db30 10fe 3ed8  es.xml.Umk.0..>.
+000018e0: 7f10 faee ca76 e32c 09b6 4bd3 d450 d8c6  .....v.,..K..P..
+000018f0: a01d ecab 62cb 89a8 5e8c ac74 4ec7 fefb  ....b...^..tN...
+00001900: 4e7e 495c da2d 2363 5f12 e974 7aee b97b  N~I\.-#c_..tz..{
+00001910: eee4 f8aa 9102 3d31 5373 ad12 1c5c f818  ......=1Ss...\..
+00001920: 3195 eb82 ab4d 82bf 3e64 de0c a3da 5255  1....M..>d....RU
+00001930: 50a1 154b f09e d5f8 2a7d ff2e aeed 5eb0  P..K....*}....^.
+00001940: fb2d 6316 0184 aa13 bcb5 b65a 1052 e75b  .-c........Z.R.[
+00001950: 2669 7da1 2ba6 e0a4 d446 520b 5bb3 2175  &i}.+....FR.[.!u
+00001960: 6518 2d6a 7749 0a12 fafe 9448 ca15 ee10  e.-jwI.....H....
+00001970: 1632 ff1b 1049 cde3 aef2 722d 2b6a f99a  .2...I....r-+j..
+00001980: 0b6e f72d 1646 325f dc6d 9436 742d 806a  .n.-.F2_.m.6t-.j
+00001990: 134c 688e 9a60 6a42 d498 2148 6b7d 1547  .Lh..`jB..!Hk}.G
+000019a0: f2dc e85a 97f6 0270 892e 4b9e b3d7 74e7  ...Z...p..K...t.
+000019b0: 644e 687e 4402 e4f3 9082 88f8 e18b dc1b  dNh~D...........
+000019c0: 7326 d284 18f6 c49d 7c38 8d4b ad6c 8d72  s&......|8.K.l.r
+000019d0: bd53 36c1 2110 7525 583c 2afd 5d65 ee08  .S6.!.u%X<*.]e..
+000019e0: 14ee bdd2 b87e 464f 5480 25c0 248d 732d  .....~FOT.%.$.s-
+000019f0: b441 16a4 83ca b516 4525 eb3c 6ea8 e06b  .A......E%.<n..k
+00001a00: c39d 5b49 2517 fbce 1c3a 43ab 76ef 2739  ..[I%....:C.v.'9
+00001a10: d4de 1989 e3d1 b149 e3b5 f3fa efb1 da90  .......I........
+00001a20: 35c4 e442 8c2a d019 d218 5ac5 32a3 3238  5..B.*....Z.2.28
+00001a30: 45fd fa61 5f41 aa0a baba a30c 4727 bd37  E..a_A......G'.7
+00001a40: 86ee 8330 1a5d 206d 40c8 529b 02a6 e858  ...0.] m@.R....X
+00001a50: fbc1 94c6 8295 166a 60f8 66eb fead aee0  .......j`.f.....
+00001a60: 77ad ad85 4e4b e382 d38d 5654 b8b2 7520  w...NK....VT..u 
+00001a70: 2f6f c2f4 c1a0 25d8 6e61 5006 9de8 ceea  /o....%.naP.....
+00001a80: 5e26 e2e0 7bf4 93be 2d87 96c2 4957 a039  ^&..{...-...IW.9
+00001a90: b03c e9db 25f3 762e 7d52 204d ce84 b877  .<..%.v.}R M...w
+00001aa0: c97c 2b0f 7572 edd8 9448 ed64 26ed 5d91  .|+.ur...H.d&.].
+00001ab0: 6078 7f5c f30c 4b10 a55f 76b5 e936 ae56  `x.\..K.._v..6.V
+00001ac0: 63b4 0e7b 041b 9e05 8b9a f280 ff3b 5201  c..{.........;R.
+00001ad0: f07b 8b14 d887 db88 5695 d8bb 7973 1275  .{......V...ys.u
+00001ae0: bb65 db1e c7fd b5e0 1b25 59e7 92c6 3060  .e.......%Y...0`
+00001af0: dd16 6db5 e1cf 70d5 4d66 0ee7 0c1e 2e78  ..m...p.Mf.....x
+00001b00: 9e2d cf9d 0544 697b af29 fb0a 40ce a3c2  .-...Di{.)..@...
+00001b10: be28 eba1 40c8 4d72 823f bb87 588c 68ae  .(..@.Mr.?..X.h.
+00001b20: 775c 58ae de28 2960 16cd 5124 dfc5 b4ee  w\X..()`..Q$....
+00001b30: 516d e53b 4401 ad0a 56d2 9db0 0f87 c304  Qm.;D...V.......
+00001b40: 1fd7 9f58 c177 727e f0fa c29f b46d 2112  ...X.wr~.....m!.
+00001b50: 7c5c 7f74 7311 4c5d 0cd6 d88f 3534 33fc  |\.ts.L]....543.
+00001b60: a39d e109 fe71 bbfc 305f dd66 a137 f397  .....q..0_.f.7..
+00001b70: 336f 72c9 226f 1e2d 575e 34b9 59ae 56d9  3or."o.-W^4.Y.V.
+00001b80: dc0f fd9b 9fa3 a7fd 1f1e f6f6 4b04 dd18  ............K...
+00001b90: 4c16 b580 e7df f4c9 f629 de1f 6d09 1e6d  L........)..m..m
+00001ba0: 3afa ad2a 407b cc7d 1e4e fdeb 28f0 bdec  :..*@{.}.N..(...
+00001bb0: d20f bcc9 94ce bcd9 f432 f2b2 2808 57d3  .........2..(.W.
+00001bc0: c9f2 36ca a211 f7e8 cc0f 804f 82a0 fb94  ..6........O....
+00001bd0: 38f2 d1c2 72c9 0457 8356 8342 632b 8804  8...r..W.V.Bc+..
+00001be0: db3f 2441 0625 c8f1 339f fe02 0000 ffff  .?$A.%..3.......
+00001bf0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00001c00: 8959 ffd7 0101 0000 2f02 0000 1400 0000  .Y....../.......
+00001c10: 786c 2f73 6861 7265 6453 7472 696e 6773  xl/sharedStrings
+00001c20: 2e78 6d6c 6c91 cf4e c330 0cc6 ef48 bc43  .xmll..N.0...H.C
+00001c30: 95fb 9676 4230 a1b6 3b20 f104 208e 5594  ...vB0..; .. .U.
+00001c40: 9a36 5262 87d8 ddd6 b7a7 d32e 28e1 e89f  .6Rb........(...
+00001c50: bfcf 7fdb d335 f8ea 0c89 1d61 a79a 7dad  .....5.....a..}.
+00001c60: 2a40 4ba3 c3a9 539f 1fef bba3 aa58 0c8e  *@K...S......X..
+00001c70: c613 42a7 5660 75ea 1f1f 5a66 a936 2f72  ..B.V`u...Zf.6/r
+00001c80: a766 91f8 aa35 db19 82e1 3d45 c02d f34d  .f...5....=E.-.M
+00001c90: 2918 d9c2 3469 8e09 ccc8 3380 04af 0f75  )...4i....3....u
+00001ca0: fdac 8371 a82a 4b0b 4aa7 9eb6 b60b ba9f  ...q.*K.J.......
+00001cb0: 05de eea0 39aa be65 d7b7 d2af 6052 aba5  ....9..e....`R..
+00001cc0: 6ff5 2dbe b397 ba2e 5053 a243 81be 8005  o.-.....PS.C....
+00001cd0: 1271 ee16 17a0 6060 6724 4fd3 9a67 2c19  .q....``g$O..g,.
+00001ce0: 3fc4 e873 7e71 38fe c791 4618 3cd9 5c7f  ?..s~q8...F.<.\.
+00001cf0: 5b6d 3056 727e 367e 29c6 d9ee 5308 77b9  [m0Vr~6~)...S.w.
+00001d00: d309 8482 5d07 5963 516f 4a74 91f9 d6de  ....].YcQoJt....
+00001d10: 9d9d acc3 1273 63fc 7b78 bd3d bcff 0500  .....sc.{x.=....
+00001d20: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00001d30: 0021 009f 7344 234a 0100 0063 0200 0011  .!..sD#J...c....
+00001d40: 0008 0164 6f63 5072 6f70 732f 636f 7265  ...docProps/core
+00001d50: 2e78 6d6c 20a2 0401 28a0 0001 0000 0000  .xml ...(.......
 00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -479,39 +479,39 @@
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e50: 0000 0000 0000 0000 0000 8c92 514b c330  ............QK.0
-00001e60: 1485 df05 ff43 c97b 9ba6 d3a1 a1ed c0c9  .....C.{........
-00001e70: 4074 4c74 a2f8 1692 bb2d d8a4 2189 6efb  @tLt.....-..!.n.
-00001e80: f7a6 ed56 3bf4 c1c7 e49c fbe5 9c4b f2c9  ...V;........K..
-00001e90: 4e55 d117 5827 6b5d 2092 a428 02cd 6b21  NU..X'k] ..(..k!
-00001ea0: f5ba 402f cb59 7c85 22e7 9916 acaa 3514  ..@/.Y|.".....5.
-00001eb0: 680f 0e4d caf3 b39c 1bca 6b0b 8fb6 3660  h..M......k...6`
-00001ec0: bd04 1705 9276 949b 026d bc37 1463 c737  .....v...m.7.c.7
-00001ed0: a098 4b82 4307 7155 5bc5 7c38 da35 368c  ..K.C.qU[.|8.56.
-00001ee0: 7fb0 35e0 2c4d c758 8167 8279 861b 606c  ..5.,M.X.g.y..`l
-00001ef0: 7a22 3a20 05ef 91e6 d356 2d40 700c 1528  z": .....V-@p..(
-00001f00: d0de 6192 10fc e3f5 6095 fb73 a055 064e  ..a.....`..s.U.N
-00001f10: 25fd de84 4e87 b843 b6e0 9dd8 bb77 4ef6  %...N..C.....wN.
-00001f20: c6ed 769b 6c47 6d8c 909f e0b7 f9c3 735b  ..v.lGm.......s[
-00001f30: 3596 bad9 1507 54e6 8253 6e81 f9da 96b3  5.....T..Sn.....
-00001f40: a7bb e9fd 225a 5432 2c3a c703 a5d9 62c5  ...."ZT2,:....b.
-00001f50: 9c9f 8785 af24 889b 7dc9 8492 3ac7 bf85  .....$..}...:...
-00001f60: 406c 0b74 5810 5188 44bb 0247 e575 34bd  @l.tX.Q.D..G.u4.
-00001f70: 5dce 5099 a519 89d3 514c ae96 8450 32a6  ].P.....QL...P2.
-00001f80: 97e9 7bf3 eec9 7c13 b1bb 5087 d7ff 4dbc  ..{...|...P...M.
-00001f90: 4869 763d 201e 0165 9bfb f45b 94df 0000  Hiv= ..e...[....
-00001fa0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00001fb0: 0021 003b d646 5197 0100 0035 0300 0010  .!.;.FQ....5....
-00001fc0: 0008 0164 6f63 5072 6f70 732f 6170 702e  ...docProps/app.
-00001fd0: 786d 6c20 a204 0128 a000 0100 0000 0000  xml ...(........
+00001e50: 0000 0000 0000 0000 0000 0000 8c92 514b  ..............QK
+00001e60: c330 1485 df05 ff43 c97b 9ba6 c339 42db  .0.....C.{...9B.
+00001e70: 8193 81e8 98e8 44f1 2d24 775b b049 4312  ......D.-$w[.IC.
+00001e80: edf6 ef4d dbad 6ee8 838f c939 f7cb 3997  ...M..n....9..9.
+00001e90: e4d3 9daa a22f b04e d6ba 4024 4951 049a  ...../.N..@$IQ..
+00001ea0: d742 ea4d 815e 56f3 7882 22e7 9916 acaa  .B.M.^V.x.".....
+00001eb0: 3514 680f 0e4d cbcb 8b9c 1bca 6b0b 8fb6  5.h..M......k...
+00001ec0: 3660 bd04 1705 9276 949b 026d bd37 1463  6`.....v...m.7.c
+00001ed0: c7b7 a098 4b82 4307 715d 5bc5 7c38 da0d  ....K.C.q][.|8..
+00001ee0: 368c 7fb0 0de0 2c4d c758 8167 8279 865b  6.....,M.X.g.y.[
+00001ef0: 606c 0622 3a20 051f 90e6 d356 1d40 700c  `l.": .....V.@p.
+00001f00: 1528 d0de 6192 10fc e3f5 6095 fb73 a053  .(..a.....`..s.S
+00001f10: 4e9c 4afa bd09 9d0e 714f d982 f7e2 e0de  N.J.....qO......
+00001f20: 3939 189b a649 9a51 1723 e427 f86d f1f0  99...I.Q.#.'.m..
+00001f30: dc55 8da5 6e77 c501 95b9 e094 5b60 beb6  .U..nw......[`..
+00001f40: e5fc e96e 76bf 8c96 950c 8bce f189 d26e  ...nv..........n
+00001f50: b162 ce2f c2c2 d712 c4cd be64 4249 9de3  .b./.......dBI..
+00001f60: df42 2076 057a 2c88 2844 a27d 81a3 f23a  .B v.z,.(D.}...:
+00001f70: 9add aee6 a8cc d28c c4e9 2826 9315 2194  ..........(&..!.
+00001f80: 8ce9 55fa debe 7b36 df46 ec2f d4e1 f57f  ..U...{6.F./....
+00001f90: 1233 4aae cf89 4740 d9e5 3eff 16e5 3700  .3J...G@..>...7.
+00001fa0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00001fb0: 0000 2100 0fd4 d937 9f01 0000 4103 0000  ..!....7....A...
+00001fc0: 1000 0801 646f 6350 726f 7073 2f61 7070  ....docProps/app
+00001fd0: 2e78 6d6c 20a2 0401 28a0 0001 0000 0000  .xml ...(.......
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -519,79 +519,80 @@
 00002060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000020d0: 0000 0000 0000 0000 0000 009c 93c1 6edb  ..............n.
-000020e0: 300c 86ef 03fa 0e86 ee8d dc6c 2886 4056  0..........l(.@V
-000020f0: 51a4 2b7a d8b0 0049 db63 a14a 742c 5496  Q.+z...I.c.Jt,T.
-00002100: 0489 3592 3dfd 681b 759d f630 6037 923f  ..5.=.h.u..0`7.?
-00002110: f1fb 2329 8bab 43eb 8a0e 52b6 c157 ec62  ..#)..C...R..W.b
-00002120: 51b2 02bc 0ec6 fa7d c5ee 77b7 e7df 5991  Q......}..w...Y.
-00002130: 5179 a35c f050 b123 6476 25cf be88 4d0a  Qy.\.P.#dv%...M.
-00002140: 1112 5ac8 0559 f85c b106 31ae 38cf ba81  ..Z..Y.\..1.8...
-00002150: 56e5 05c9 9e94 3aa4 5621 a569 cf43 5d5b  V.....:.V!.i.C][
-00002160: 0d37 41bf b6e0 912f cbf2 92c3 01c1 1b30  .7A..../.......0
-00002170: e771 3264 a3e3 aac3 ff35 3541 f77c f961  .q2d.....55A.|.a
-00002180: 778c 042c c575 8cce 6a85 34a5 fc65 750a  w..,.u..j.4..eu.
-00002190: 39d4 58fc 3868 7082 cf45 4174 5bd0 afc9  9.X.8hp..EAt[...
-000021a0: e251 9682 cf53 b1d5 cac1 9a8c 65ad 5c06  .Q...S......e.\.
-000021b0: c1df 0be2 0e54 bfb4 8db2 294b d1e1 aa03  .....T....)K....
-000021c0: 8d21 15d9 fea1 b52d 59f1 ac32 f438 15eb  .!.....-Y..2.8..
-000021d0: 54b2 ca23 61f5 6d63 32c4 2e66 4cf2 31a4  T..#a.mc2..fL.1.
-000021e0: 97dc 0060 169c 1ac6 e210 ce7b e7b1 fd26  ...`.......{...&
-000021f0: 9743 0305 a78d bdc1 0842 c229 e2ce a283  .C.......B.)....
-00002200: fcbb dea8 84ff 221e 1846 de11 c7d0 89bd  ......"..F......
-00002210: 99f3 4da4 f6f0 8434 e653 ab62 a485 7c9a  ..M....4.S.b..|.
-00002220: 6158 0bd1 7cf8 fe3a b451 f923 0953 f4d3  aX..|..:.Q.#.S..
-00002230: fa97 7c1f 77e1 4621 bcad fcb4 28b6 8d4a  ..|.w.F!....(..J
-00002240: 60e8 4ad3 49a6 82b8 238c e47a 9375 a3fc  `.J.I...#..z.u..
-00002250: 1ecc 5bcf 67a1 7f20 0fe3 5f20 2f2e 17e5  ..[.g.. .._ /...
-00002260: d792 6e3f ab09 fefe dee5 5f00 0000 ffff  ..n?......_.....
-00002270: 0300 504b 0102 2d00 1400 0600 0800 0000  ..PK..-.........
-00002280: 2100 1218 dedd 6401 0000 1805 0000 1300  !.....d.........
-00002290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022a0: 5b43 6f6e 7465 6e74 5f54 7970 6573 5d2e  [Content_Types].
-000022b0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-000022c0: 0021 00b5 5530 23f4 0000 004c 0200 000b  .!..U0#....L....
-000022d0: 0000 0000 0000 0000 0000 0000 009d 0300  ................
-000022e0: 005f 7265 6c73 2f2e 7265 6c73 504b 0102  ._rels/.relsPK..
-000022f0: 2d00 1400 0600 0800 0000 2100 597b 8763  -.........!.Y{.c
-00002300: c302 0000 6106 0000 0f00 0000 0000 0000  ....a...........
-00002310: 0000 0000 0000 c206 0000 786c 2f77 6f72  ..........xl/wor
-00002320: 6b62 6f6f 6b2e 786d 6c50 4b01 022d 0014  kbook.xmlPK..-..
-00002330: 0006 0008 0000 0021 004a a9a6 61fa 0000  .......!.J..a...
-00002340: 0047 0300 001a 0000 0000 0000 0000 0000  .G..............
-00002350: 0000 00b2 0900 0078 6c2f 5f72 656c 732f  .......xl/_rels/
-00002360: 776f 726b 626f 6f6b 2e78 6d6c 2e72 656c  workbook.xml.rel
-00002370: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
-00002380: 0027 1c6c 8b93 0200 00da 0700 0018 0000  .'.l............
-00002390: 0000 0000 0000 0000 0000 00ec 0b00 0078  ...............x
-000023a0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-000023b0: 6574 312e 786d 6c50 4b01 022d 0014 0006  et1.xmlPK..-....
-000023c0: 0008 0000 0021 0052 bb24 fb4f 0200 0018  .....!.R.$.O....
-000023d0: 0500 0018 0000 0000 0000 0000 0000 0000  ................
-000023e0: 00b5 0e00 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-000023f0: 7473 2f73 6865 6574 322e 786d 6c50 4b01  ts/sheet2.xmlPK.
-00002400: 022d 0014 0006 0008 0000 0021 00bd a0bf  .-.........!....
-00002410: bd4b 0700 001d 2200 0013 0000 0000 0000  .K....".........
-00002420: 0000 0000 0000 003a 1100 0078 6c2f 7468  .......:...xl/th
-00002430: 656d 652f 7468 656d 6531 2e78 6d6c 504b  eme/theme1.xmlPK
-00002440: 0102 2d00 1400 0600 0800 0000 2100 296b  ..-.........!.)k
-00002450: b8a1 1c03 0000 2c08 0000 0d00 0000 0000  ......,.........
-00002460: 0000 0000 0000 0000 b618 0000 786c 2f73  ............xl/s
-00002470: 7479 6c65 732e 786d 6c50 4b01 022d 0014  tyles.xmlPK..-..
-00002480: 0006 0008 0000 0021 0017 b4e6 faf4 0000  .......!........
-00002490: 0018 0200 0014 0000 0000 0000 0000 0000  ................
-000024a0: 0000 00fd 1b00 0078 6c2f 7368 6172 6564  .......xl/shared
-000024b0: 5374 7269 6e67 732e 786d 6c50 4b01 022d  Strings.xmlPK..-
-000024c0: 0014 0006 0008 0000 0021 0004 da6b 1a4b  .........!...k.K
-000024d0: 0100 0063 0200 0011 0000 0000 0000 0000  ...c............
-000024e0: 0000 0000 0023 1d00 0064 6f63 5072 6f70  .....#...docProp
-000024f0: 732f 636f 7265 2e78 6d6c 504b 0102 2d00  s/core.xmlPK..-.
-00002500: 1400 0600 0800 0000 2100 3bd6 4651 9701  ........!.;.FQ..
-00002510: 0000 3503 0000 1000 0000 0000 0000 0000  ..5.............
-00002520: 0000 0000 a51f 0000 646f 6350 726f 7073  ........docProps
-00002530: 2f61 7070 2e78 6d6c 504b 0506 0000 0000  /app.xmlPK......
-00002540: 0b00 0b00 c602 0000 7222 0000 0000       ........r"....
+000020d0: 0000 0000 0000 0000 0000 0000 9c93 c16e  ...............n
+000020e0: db30 0c86 ef03 f60e 86ee 8ddc 6c28 8640  .0..........l(.@
+000020f0: 5631 a41b 7ad8 b000 49db 63c0 c974 2cd4  V1..z...I.c..t,.
+00002100: 9604 89f1 923d fd68 1b75 9df5 3060 3792  .....=.h.u..0`7.
+00002110: 3ff1 e323 45a9 db53 db64 1dc6 64bd 2bc4  ?..#E..S.d..d.+.
+00002120: f522 1719 3ae3 4beb 0e85 78d8 7dbd fa24  ."..:.K...x.}..$
+00002130: b244 e04a 68bc c342 9c31 895b fdfe 9dda  .D.Jh..B.1.[....
+00002140: 441f 3092 c594 b185 4b85 a889 c24a ca64  D.0.....K....J.d
+00002150: 6a6c 212d 5876 ac54 3eb6 409c c683 f455  jl!-Xv.T>.@....U
+00002160: 650d de79 736c d191 5ce6 f98d c413 a12b  e..ysl..\......+
+00002170: b1bc 0a93 a118 1d57 1dfd af69 e94d cf97  .......W...i.M..
+00002180: 1e77 e7c0 c05a 7d0e a1b1 0688 a7d4 dfad  .w...Z}.........
+00002190: 893e f98a b22f 2783 8d92 7351 31dd 16cd  .>.../'...sQ1...
+000021a0: 315a 3aeb 5cc9 79aa b606 1a5c b3b1 aea0  1Z:.\.y....\....
+000021b0: 49a8 e46b 41dd 23f4 4bdb 808d 49ab 8e56  I..kA.#.K...I..V
+000021c0: 1d1a f231 4bf6 37af 6d29 b29f 90b0 c729  ...1K.7.m).....)
+000021d0: 4407 d182 23c6 eadb c664 889b 9028 ea27  D...#....d...(.'
+000021e0: 1f9f 538d 4849 496e 188b 4338 ef9d c7f6  ..S.HIIn..C8....
+000021f0: a35e 0e0d 1c5c 36f6 0623 080b 9788 3b4b  .^...\6..#....;K
+00002200: 0da6 1fd5 0622 fd8b 7860 1879 479c 43f4  ....."..x`.yG.C.
+00002210: bfa8 de83 21db f1a6 f6c7 3067 9da8 ed69  ....!.....0g...i
+00002220: 4f3c f2be 8510 7839 6fe6 1956 c464 7fb1  O<....x9o..V.d..
+00002230: ac7d 1bc0 9d59 98a2 6fd6 3da7 87b0 f377  .}...Y..o.=....w
+00002240: 40f8 b2fe cba2 dad6 10b1 e417 9b9e 672a  @.............g*
+00002250: a87b c688 4d6f b2ae c11d b07c e979 2bf4  .{..Mo.....|.y+.
+00002260: c7f2 38fe 087d 7db3 c83f e47c 07b3 9a92  ..8..}}..?.|....
+00002270: afb7 afff 0000 00ff ff03 0050 4b01 022d  ...........PK..-
+00002280: 0014 0006 0008 0000 0021 0012 18de dd64  .........!.....d
+00002290: 0100 0018 0500 0013 0000 0000 0000 0000  ................
+000022a0: 0000 0000 0000 0000 005b 436f 6e74 656e  .........[Conten
+000022b0: 745f 5479 7065 735d 2e78 6d6c 504b 0102  t_Types].xmlPK..
+000022c0: 2d00 1400 0600 0800 0000 2100 b555 3023  -.........!..U0#
+000022d0: f400 0000 4c02 0000 0b00 0000 0000 0000  ....L...........
+000022e0: 0000 0000 0000 9d03 0000 5f72 656c 732f  .........._rels/
+000022f0: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
+00002300: 0000 0021 00db d923 3ad9 0200 0081 0600  ...!...#:.......
+00002310: 000f 0000 0000 0000 0000 0000 0000 00c2  ................
+00002320: 0600 0078 6c2f 776f 726b 626f 6f6b 2e78  ...xl/workbook.x
+00002330: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00002340: 2100 4aa9 a661 fa00 0000 4703 0000 1a00  !.J..a....G.....
+00002350: 0000 0000 0000 0000 0000 0000 c809 0000  ................
+00002360: 786c 2f5f 7265 6c73 2f77 6f72 6b62 6f6f  xl/_rels/workboo
+00002370: 6b2e 786d 6c2e 7265 6c73 504b 0102 2d00  k.xml.relsPK..-.
+00002380: 1400 0600 0800 0000 2100 f8a1 9805 ab02  ........!.......
+00002390: 0000 bb09 0000 1800 0000 0000 0000 0000  ................
+000023a0: 0000 0000 020c 0000 786c 2f77 6f72 6b73  ........xl/works
+000023b0: 6865 6574 732f 7368 6565 7431 2e78 6d6c  heets/sheet1.xml
+000023c0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+000023d0: 02c6 a137 1602 0000 ce04 0000 1800 0000  ...7............
+000023e0: 0000 0000 0000 0000 0000 e30e 0000 786c  ..............xl
+000023f0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00002400: 7432 2e78 6d6c 504b 0102 2d00 1400 0600  t2.xmlPK..-.....
+00002410: 0800 0000 2100 bda0 bfbd 4b07 0000 1d22  ....!.....K...."
+00002420: 0000 1300 0000 0000 0000 0000 0000 0000  ................
+00002430: 2f11 0000 786c 2f74 6865 6d65 2f74 6865  /...xl/theme/the
+00002440: 6d65 312e 786d 6c50 4b01 022d 0014 0006  me1.xmlPK..-....
+00002450: 0008 0000 0021 0029 6bb8 a11c 0300 002c  .....!.)k......,
+00002460: 0800 000d 0000 0000 0000 0000 0000 0000  ................
+00002470: 00ab 1800 0078 6c2f 7374 796c 6573 2e78  .....xl/styles.x
+00002480: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00002490: 2100 8959 ffd7 0101 0000 2f02 0000 1400  !..Y....../.....
+000024a0: 0000 0000 0000 0000 0000 0000 f21b 0000  ................
+000024b0: 786c 2f73 6861 7265 6453 7472 696e 6773  xl/sharedStrings
+000024c0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+000024d0: 0000 2100 9f73 4423 4a01 0000 6302 0000  ..!..sD#J...c...
+000024e0: 1100 0000 0000 0000 0000 0000 0000 251d  ..............%.
+000024f0: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
+00002500: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+00002510: 0021 000f d4d9 379f 0100 0041 0300 0010  .!....7....A....
+00002520: 0000 0000 0000 0000 0000 0000 00a6 1f00  ................
+00002530: 0064 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
+00002540: 6c50 4b05 0600 0000 000b 000b 00c6 0200  lPK.............
+00002550: 007b 2200 0000 00                        .{"....
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_baseline_technology_basic.xlsx` & `message_ix-3.7.0/tutorial/westeros/westeros_baseline_technology_basic.xlsx`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_baseline_technology_economic.xlsx` & `message_ix-3.7.0/tutorial/westeros/westeros_baseline_technology_economic.xlsx`

 * *Files identical despite different names*

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_baseline_using_xlsx_import_part1.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_baseline_using_xlsx_import_part1.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946204836829837%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'This tutorial is the first of two tutorials, which "*

 * *            'explain how the Westeros Baseline scenario can be built using data imported from '*

 * *            'Excel (.xlsx) files. The figure below compares the workflows of the original Westeros '*

 * *            'baseline tutorial, where data was added using the '*

 * *            '[`add_par()`](https://docs.messageix.org/projects/ixmp/en/stable/api.html?highlight=add_set()#ixmp.Scenario.add_par) '*

 * *            'and '*

 * *    […]*

```diff
@@ -8,37 +8,39 @@
                 }
             },
             "source": [
                 "# Westeros Tutorial - Introducing the use of Excel files: Building a scenario by importing data from a single \".xlsx\" file"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "## Scope of this tutorial\n",
                 "\n",
-                "This tutorial is the first of two tutorials, which explains how the Westeros Baseline scenario can be built using data imported from Excel (.xlsx) files. The figure below compares the workflows of the original Westeros baseline tutorial, where data was added using the [`add_par()`](https://docs.messageix.org/projects/ixmp/en/stable/api.html?highlight=add_set()#ixmp.Scenario.add_par) and [`add_set()`](https://docs.messageix.org/projects/ixmp/en/stable/api.html?highlight=add_set()#ixmp.Scenario.add_set) functions. The same scenario can also be created by importing data from Excel files, using [`ixmp.Scenario.read_excel()`](https://docs.messageix.org/projects/ixmp/en/latest/api.html#ixmp.Scenario.read_excel) as shown in the figure below.\n",
+                "This tutorial is the first of two tutorials, which explain how the Westeros Baseline scenario can be built using data imported from Excel (.xlsx) files. The figure below compares the workflows of the original Westeros baseline tutorial, where data was added using the [`add_par()`](https://docs.messageix.org/projects/ixmp/en/stable/api.html?highlight=add_set()#ixmp.Scenario.add_par) and [`add_set()`](https://docs.messageix.org/projects/ixmp/en/stable/api.html?highlight=add_set()#ixmp.Scenario.add_set) functions. The same scenario can also be created by importing data from Excel files, using [`ixmp.Scenario.read_excel()`](https://docs.messageix.org/projects/ixmp/en/latest/api.html#ixmp.Scenario.read_excel) as shown in the figure below.\n",
                 "\n",
                 "**Pre-requisites**\n",
                 "- You have the *MESSAGEix* framework installed and working\n",
                 "- You have run Westeros baseline scenario (``westeros_baseline.ipynb``) and solved it successfully\n",
                 "\n",
-                "In this tutorial, we will generate a single data file, which we require to generate a new scenario, by exporting the scenario data of the `westeros_baseline.ipynb` to an Excel file.  Subsequently, we will import this data into a new scenario, therefore creating an exact replica of the original baseline scenario.\n",
+                "In this tutorial, we will generate a single data file, which we require to generate a new scenario, by exporting the scenario data of the `westeros_baseline.ipynb` to an Excel file. Subsequently, we will import this data into a new scenario, therefore creating an exact replica of the original baseline scenario.\n",
                 "\n",
                 "<img src='_static/westeros_baseline_xlsx_workflow_part1.jpg'>\n",
                 "\n",
                 "In the second tutorial, we will then import data from multiple Excel files. This will provide a more detailed look at the underlying structure of the Excel files."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
@@ -46,17 +48,17 @@
                 "    \n",
                 "**Please Note:**\n",
                 "    \n",
                 "At this point, it should be emphasized that the use of this method to build complex models is not recommended. There are multiple reasons for this.  Most importantly, experience has shown that relying on Excel files as the only source of data often results in issues of data management. While at the beginning of the model building exercise, there are only a few files, their number will increase over time.  This can result in possible confusions as to which dataset was used for which scenario. Further, the `read_excel()` function makes use of many other MESSAGEix functionalities. Hence, the modeler will rely on the use of a single function instead of the underlying functions. This can result in the development of workflows that are more complex than required.\n",
                 "\n",
                 "<u>An example:</u>\n",
                 "\n",
-                "Assume that the 'baseline' scenario is built from an Excel file. It is easy to duplicate the excel file, change/add one or two parameters in the new excel file in order to create a new scenario. But for each additional scenario, a new excel file is created, which requires manual intervention.\n",
+                "Assume that the 'baseline' scenario is built from an Excel file. It is easy to duplicate the Excel file, change/add one or two parameters in the new Excel file in order to create a new scenario. But for each additional scenario, a new Excel file is created, which requires manual intervention.\n",
                 "    \n",
-                "The method which we advise in such cases would be to `clone()` the 'baseline' scenario. Functions such as `par()` can then be used to retrieve existing parameters from a scenario.  The data can be modified and added back to the scenario using `add_par()`. Setting up clear workflows is key to also ensuring the reproducibility and transparency of your work."
+                "The method which we advise in such cases would be to `clone()` the 'baseline' scenario. Functions such as `par()` can then be used to retrieve existing parameters from a scenario. The data can be modified and added back to the scenario using `add_par()`. Setting up clear workflows is key to ensuring the reproducibility as well as the transparency of your work."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
@@ -161,22 +163,23 @@
                 }
             },
             "source": [
                 "## Step 4: Importing data from Excel"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "fragment"
                 }
             },
             "source": [
-                "Instead of using the `message_ix.Scenario.add_par()` for adding data to a MESSAGEix parameter, we import data from an Excel file. The arguments `add_units` has been set to `True`, so that any units which have not yet been specified in the modeling platform will be defined automatically."
+                "Instead of using the `message_ix.Scenario.add_par()` for adding data to a MESSAGEix parameter, we import data from an Excel file. The argument `add_units` has been set to `True`, so that any units which have not yet been specified in the modeling platform will be defined automatically."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_baseline_using_xlsx_import_part2.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_baseline_using_xlsx_import_part2.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989995226656812%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(2, \'This tutorial builds on "Westeros Tutorial Part '*

 * *            '3.2.1", which explained how data from the Westeros Baseline scenario can be exported '*

 * *            'to an Excel (.xlsx) file using the function '*

 * *            '[`ixmp.Scenario.to_excel()`](https://docs.messageix.org/projects/ixmp/en/latest/api.html#ixmp.Scenario.to_excel) '*

 * *            'and how this data can be used to build a new scenario via '*

 * *            '[`ixmp.Scenario.read_excel()`](https://docs […]*

```diff
@@ -8,54 +8,56 @@
                 }
             },
             "source": [
                 "# Westeros Tutorial - Introducing the use of Excel files: Building a scenario by importing data from multiple \".xlsx\" file"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "## Scope of this tutorial\n",
                 "\n",
-                "This tutorial builds on \"Westeros Tutorial Part 4.a\", which explained how data from the Westeros Baseline scenario can be exported to an Excel (.xlsx) file using the function [`ixmp.Scenario.to_excel()`](https://docs.messageix.org/projects/ixmp/en/latest/api.html#ixmp.Scenario.to_excel) and how this data can be used to build a new scenario [`ixmp.Scenario.read_excel()`](https://docs.messageix.org/projects/ixmp/en/latest/api.html#ixmp.Scenario.read_excel). This tutorial will look at the workflow of building a new scenario from data stored in an Excel file more carefully. \n",
+                "This tutorial builds on \"Westeros Tutorial Part 3.2.1\", which explained how data from the Westeros Baseline scenario can be exported to an Excel (.xlsx) file using the function [`ixmp.Scenario.to_excel()`](https://docs.messageix.org/projects/ixmp/en/latest/api.html#ixmp.Scenario.to_excel) and how this data can be used to build a new scenario via [`ixmp.Scenario.read_excel()`](https://docs.messageix.org/projects/ixmp/en/latest/api.html#ixmp.Scenario.read_excel). This tutorial will look at the workflow of building a new scenario from data stored in an Excel file more carefully. \n",
                 "\n",
                 "**Pre-requisites**\n",
                 "- You have the *MESSAGEix* framework installed and working\n",
                 "- You have run Westeros baseline scenario (``westeros_baseline.ipynb``) and solved it successfully\n",
                 "- You have gone through Westeros Tutorial 4a, part 1 on importing data from an Excel file  (``westeros_baseline_using_xlsx_import_part1.ipynb``)\n",
                 "\n",
                 "To do this, we are again going to build the Westeros Baseline, but this time combining elements from the original baseline tutorial with the import of data from multiple Excel files (see figure below - the red line indicates at which point of the process this tutorial will commence i.e. the source Excel files have already been generated). \n",
                 "\n",
                 "<img src='_static/westeros_baseline_xlsx_workflow_part2.jpg'>\n",
                 "\n",
                 "The first part will create a scenario and basic parameters will be added including the modeling time-horizon and the discount rate. This code is a repetition of that used in the tutorial `westeros_baseline.ipynb`, which will be referred to as the \"original\" scenario throughout the remainder of this tutorial.\n",
                 "\n",
-                "The second part will then import various parameters from Excel files, adding technologies, demand, and constraints to the model. We have chosen to distribute the import of data across various excel files. This helps to outline a possible approach on how to structure the import methods if used for loading large amounts of data into scenarios.  It further demonstrates the required data contents of the excel files."
+                "The second part will then import various parameters from Excel files, adding technologies, demand, and constraints to the model. We have chosen to distribute the import of data across various Excel files. This helps to outline a possible approach on how to structure the import methods if used for loading large amounts of data into scenarios. It further demonstrates the required data contents of the Excel files."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-block alert-success\">\n",
                 " \n",
                 "**Please Note:**\n",
                 "\n",
                 "This tutorial specifically targets users looking to build larger models using the Excel import functionalities. The advantage of using multiple files, especially for large data sets, is that this provides a more transparent structuring of the underlying workflow. Scripts related to creating the Excel source files and the respective imports will be limited to certain model aspects. \n",
                 "    \n",
                 "<u>An example:</u>\n",
                 "    \n",
                 "As shown in the figure above (right panel), a script can generate and import \"technology\" data, another the \"demand\" and a third generates \"constraints\". If alternative demand projects are to be used, for example to account for more factors influencing near term economic growth, then only a single script will need to be revised.  \n",
                 "    \n",
-                "This means that maintenance and updates can be performed more readily in the future. While acknowledging the fact that in some cases, for example when transitioning from other model platforms, importing data as demonstrated in this tutorial is possible, it is only advised to rely on these methods temporarily. Using multiple Excel files can aid in this respect. It allows the modeler to subsequently replace the use of \"read_excel()\" functionality in a more structured manner, updating the workflow for smaller more manageable scenario aspects."
+                "This means that maintenance and updates can be performed more readily in the future. While acknowledging the fact that in some cases, for example when transitioning from other model platforms, importing data as demonstrated in this tutorial is possible, it is only advised to rely on these methods temporarily. Using multiple Excel files can aid in this respect. It allows the modeler to subsequently replace the use of `read_excel()` functionality in a more structured manner, updating the workflow for smaller more manageable scenario aspects."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Step 1. Setting up the scenario"
@@ -116,24 +118,25 @@
                 "# Creating a new, empty scenario\n",
                 "scenario = message_ix.Scenario(\n",
                 "    mp, model=\"Westeros Electrified\", scenario=\"baseline_xlsx\", version=\"new\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "## Model Structure\n",
                 "\n",
-                "As in the original tuorial, basic characteristics of the model, including model years, location, and the energy system structure are defined. We also define the interest rate."
+                "As in the original tutorial, basic characteristics of the model, including model years, location, and the energy system structure are defined. We also define the interest rate."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "slideshow": {
@@ -160,18 +163,19 @@
             "source": [
                 "# Defining a spatial level and adding a node to it\n",
                 "node = \"Westeros\"\n",
                 "scenario.add_spatial_sets({\"country\": node})"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Contrary to the original tutorial for building the Westros model, we only define commodities and levels here. If additional `\"commodity\"` or `\"level\"` types are required later on, these can also be defined with uploading technologoy data using the excel files. Either method is fine.\n",
+                "Contrary to the original tutorial for building the Westeros model, we only define commodities and levels here. If additional `\"commodity\"` or `\"level\"` types are required later on, these can also be defined with uploading technologoy data using the Excel files. Either method is fine.\n",
                 "Note that we populated the set `\"technology\"` and `\"mode\"` in the original tutorial. We will address these in the second half of this tutorial."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -193,18 +197,19 @@
             "outputs": [],
             "source": [
                 "# Adding interest rate of 5% per model year\n",
                 "scenario.add_par(\"interestrate\", model_horizon, value=0.05, unit=\"-\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Note that the data has not yet been commited. This is because at a minimum, the set technology needs to be defined otherwise an error message will be raised when commiting the scenario. Hence, we will continue in this tutorial by adding data, step-by-step, in the process of which commits are automatically made."
+                "Note that the data has not yet been commited. This is because at a minimum, the set technology needs to be defined, otherwise an error message will be raised when commiting the scenario. Hence, we will continue in this tutorial by adding data, step-by-step, in the process of which commits are automatically made."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
@@ -222,38 +227,40 @@
                 }
             },
             "source": [
                 "### 2.1 Supply and Demand (or Balancing Commodities)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "fragment"
                 }
             },
             "source": [
-                "Instead of using the `message_ix.Scenario.add_par()` for adding data to a MESSAGEix parameter, we import data from a xlsx file. The arguments `add_units` has been set to `True`, so that any units which have not yet been specified in the modeling platform will be defined automatically."
+                "Instead of using the `message_ix.Scenario.add_par()` for adding data to a MESSAGEix parameter, we import data from an xlsx file. The argument `add_units` has been set to `True`, so that any units which have not yet been specified in the modeling platform will be defined automatically."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "scenario.read_excel(\"westeros_baseline_demand.xlsx\", add_units=True, commit_steps=False)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Open the above indicated xlsx (\"westeros_baseline_demand.xlsx\") file and browse its contents. You will find that it includes two sheets. A sheet `\"demand\"` which contains the based on the index structure of the parameters `\"demand\"`."
+                "Open the above indicated xlsx (\"westeros_baseline_demand.xlsx\") file and browse its contents. You will find that it includes two sheets, of which we will need only one here (the other will be explained below). Namely, the sheet \"demand\", which contains the data based on the index structure of the parameter `\"demand\"`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -265,35 +272,36 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In addition, numerical values have been added under the index-name `value` and the units have been specified under the index-name `unit`. These two index names are used for adding numerical values and units across all parameters."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 2.2 Adding technologies\n",
                 "\n",
-                "The next step is to add a basic configuration for technologies, using the data input file `westeros_baseline_technology_basic.xlsx`.\n",
+                "The next step is to add a basic configuration for technologies, using the data input file \"westeros_baseline_technology_basic.xlsx\".\n",
                 "This Excel file has the following sheets:\n",
                 "\n",
                 "- mode\n",
                 "- technology\n",
                 "- capacity_factor\n",
                 "- input\n",
                 "- output\n",
                 "- technical_lifetime\n",
                 "- ix_type_mapping\n",
                 "\n",
                 "The `ixmp` documentation ([\u201cScenario/model data\u201d](https://docs.messageix.org/projects/ixmp/en/latest/file-io.html#excel-data-format) section of the \u201cFile formats and input/output\u201d page) gives a complete description of the file format. To summarize:\n",
-                "- Most sheets have a name like \"technology\" or \"input\" that corresponds to a set or parameter in the MESSAGE formulation.\n",
-                "- The \"ix_type_mapping\" sheet is used by the export/import code to keep track of this correspondence.\n",
+                "- Most sheets have a name like \"technology\" or \"input\" that corresponds to a set or parameter in the MESSAGE formulation\n",
+                "- The \"ix_type_mapping\" sheet is used by the export/import code to keep track of this correspondence\n",
                 "\n",
-                "The importer handles sets first, and then parameters. The sheets for sets *must* include all elements used by the parameter data; otherwise the data is invalid and a Python exception will be raised. For example, if data in the sheet `\"capacity_factor\"` refers to a technology which is not listed in the sheet `\"technology\"`, the data are invalid. If the files are created by hand (instead of using the `to_excel()` method), it is important to ensure they are valid."
+                "The importer handles sets first, and then parameters. The sheets for sets *must* include all elements used by the parameter data; otherwise the data is invalid and a Python exception will be raised. For example, if data in the sheet `\"capacity_factor\"` refers to a technology which is not listed in the sheet \"technology\", the data are invalid. If the files are created by hand (instead of using the `to_excel()` method), it is important to ensure they are valid."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "slideshow": {
@@ -336,23 +344,24 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "scenario.par(\"capacity_factor\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
                 "### 2.3 Technological Diffusion and Contraction\n",
-                "As we have already undertaken an initial definition of technologies, and will now proceed to add additional parameters for already defined technologies, the input data file (\"westeros_baseline_technology_constraint.xlsx\") does not contain and sheets relating to sets."
+                "As we have already undertaken an initial definition of technologies, and will now proceed to add additional parameters for already defined technologies, the input data file (\"westeros_baseline_technology_constraint.xlsx\") does not contain any sheets relating to sets. Still, we import the parameter `\"growth_activity_up\"` from there."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -386,22 +395,23 @@
             "source": [
                 "scenario.read_excel(\n",
                 "    \"westeros_baseline_technology_historic.xlsx\", add_units=True, commit_steps=False\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "slideshow": {
                     "slide_type": "slide"
                 }
             },
             "source": [
-                "### 2.5 Investment, Fixed O&M and Varaible O&M Costs\n",
+                "### 2.5 Investment, Fixed O&M and Variable O&M Costs\n",
                 "Here, we import the cost data from a separate file."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_emissions_bounds.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_emissions_bounds.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970703125%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, "In the first part, the model chose not to base the '*

 * *            'power system on wind power as electricity from wind turbines was more expensive than '*

 * *            'electricity produced from coal. However, we now introduce emissions to investigate '*

 * *            'the impact of climate policy. Let\'s see what happens then.\\n")], delete: [2]}, '*

 * *            "'attachments': OrderedDict()}, 20: {'source': {insert: [(6, 'The share of the "*

 * *            'activity of th […]*

```diff
@@ -1,16 +1,17 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Westeros Tutorial - Introducing emissions (part1/2): Adding emission bounds\n",
                 "\n",
-                "In the first part, the model chose not base the power system on wind power as electricity from  wind turbines was more expensive than electricity produced from coal. However, now we introduce emissions to investigate the impact of climate policy. Let's see what happens then.\n",
+                "In the first part, the model chose not to base the power system on wind power as electricity from wind turbines was more expensive than electricity produced from coal. However, we now introduce emissions to investigate the impact of climate policy. Let's see what happens then.\n",
                 "\n",
                 "**Pre-requisites**\n",
                 "- You have the *MESSAGEix* framework installed and working\n",
                 "- You have run Westeros baseline scenario (``westeros_baseline.ipynb``) and solved it successfully"
             ]
         },
         {
@@ -219,24 +220,25 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "rep.get(\"plot capacity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Electricity Price\n",
                 "\n",
                 "And how much does the electricity cost? These prices are in fact **shadow prices** taken from the **dual variables** of the model solution. They reflect the marginal cost of electricity generation (i.e., the additional cost of the system for supplying one more unit of electricity), which is in fact the marginal cost of the most expensive generator.  \n",
                 "\n",
                 "Notice the drop in the price in the period of 710? \n",
                 "\n",
-                "The share of the activity of the coal power plant is in the period of 710 higher then the share in the period of 700. With lower electricity costs of the coal power plant, this leads to reduced electricity costs. To stay within the emission bounds with an increased electricity demand, in the upcoming period of 720, the capacity of the wind turbines increases drastically, while the capacity of the coal power plants remains the same. This results in the increased electricity price."
+                "The share of the activity of the coal power plant is higher in the period of 710 than in the period of 700. With lower electricity costs of the coal power plant, this leads to reduced electricity costs. To stay within the emission bounds with an increased electricity demand, in the upcoming period of 720, the capacity of the wind turbines increases drastically, while the capacity of the coal power plants remains the same. This results in the increased electricity price."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_emissions_taxes.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_emissions_taxes.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9506386408730159%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(0, 'When setting a cumulative bound, the undiscounted price "*

 * *            "of emission is the same in different model years (see the marginals of\\n')], delete: "*

 * *            "[0]}, 'attachments': OrderedDict()}, 25: {'source': {insert: [(1, '- How do these "*

 * *            "prices compare to the scenario with a cumulative emission bound (`scen_bd`)?\\n')], "*

 * *            "delete: [1]}, 'attachments': OrderedDict()}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'messa […]*

```diff
@@ -85,18 +85,19 @@
             "source": [
                 "# Price in USD/tCO2\n",
                 "emission_prices = scen_bd.var(\"PRICE_EMISSION\")\n",
                 "emission_prices"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "When setting a cumlulative bound, the undiscounted price of emission is the same in different model years (see the marginals of\n",
+                "When setting a cumulative bound, the undiscounted price of emission is the same in different model years (see the marginals of\n",
                 "equation `\"EMISSION_CONSTRAINT\"`). However, considering the year-to-year discount factor, we observe an ascending trend in\n",
                 "emission prices shown in `\"PRICE_EMISSION\"` above. This means the emission price in later years is higher as the value of money in\n",
                 "the future is lower compared to today. "
             ]
         },
         {
             "cell_type": "markdown",
@@ -282,19 +283,20 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "scen_tax.var(\"EMISS\", {\"node\": \"Westeros\"})"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Exercises\n",
-                "- How does these prices compare to the scenario with a cumulative emission bound (`scen_bd`)?\n",
+                "- How do these prices compare to the scenario with a cumulative emission bound (`scen_bd`)?\n",
                 "- Try setting the emission tax again by using emission prices obtained from the scenario with yearly bounds on emissions (`scen_bd_by_year`). What is the difference in emissions (i.e., variable `EMISS`)?"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -309,27 +311,32 @@
             "source": [
                 "mp.close_db()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_firm_capacity.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_firm_capacity.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9487637502917834%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'This tutorial demonstrates how to apply various "*

 * *            'features of the MESSAGEix formulation to provide a more realistic representation of '*

 * *            "renewable energy integration in the energy system.\\n'), (4, 'In the first part of "*

 * *            'this series of tutorials, we show how to ensure that in a model setup which does not '*

 * *            'use sub-annual timesteps, and therefore does not depict peak load, we can still '*

 * *            'account for [` […]*

```diff
@@ -1,24 +1,25 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Westeros Tutorial - Adding representation of renewables (part1/3): Introducing `\"firm capacity\"`\n",
                 "\n",
-                "This tutorial demonstrates how to apply various features of MESSAGEix formulation to provide a more realistic representation of renewable energy integration in the energy system.\n",
+                "This tutorial demonstrates how to apply various features of the MESSAGEix formulation to provide a more realistic representation of renewable energy integration in the energy system.\n",
                 "\n",
-                "In the first part of these series of tutorials, we show how to ensure that in a model setup which does not use sub-annual timesteps, and therefore does not depict peak load, we can still account for [`\"firm capacity\"`](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=FIRM_CAPACITY_PROVISION#equation-firm-capacity-provision). In power systems, firm or reliable capacity means sufficient power capacity from different electricity generation plants is available to maintain system reliability through reasonable load and contingency events.\n",
+                "In the first part of this series of tutorials, we show how to ensure that in a model setup which does not use sub-annual timesteps, and therefore does not depict peak load, we can still account for [`\"firm capacity\"`](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=FIRM_CAPACITY_PROVISION#equation-firm-capacity-provision). In power systems, firm or reliable capacity means sufficient power capacity from different electricity generation plants is available to maintain system reliability through reasonable load and contingency events.\n",
                 "\n",
-                "Further information can be found in https://doi.org/10.1016/j.esr.2013.01.001 (*Sullivan et al., 2013*)\n",
+                "Further information can be found in [Sullivan et al., 2013](https://doi.org/10.1016/j.esr.2013.01.001).\n",
                 "\n",
                 "**Pre-requisites**\n",
-                "- You have the *MESSAGEix* framework installed and working.\n",
-                "- You have run Westeros scenario which adds emission bounds (``westeros_emissions_bounds.ipynb``) and solved it successfully."
+                "- You have the *MESSAGEix* framework installed and working\n",
+                "- You have run Westeros scenario which adds emission bounds (``westeros_emissions_bounds.ipynb``) and solved it successfully"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -83,23 +84,24 @@
                 "year_df = scen.vintage_and_active_years()\n",
                 "vintage_years, act_years = year_df[\"year_vtg\"], year_df[\"year_act\"]\n",
                 "model_horizon = scen.set(\"year\")\n",
                 "country = \"Westeros\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## `\"peak_load_factor\"` - Describing the Electricity Sector\n",
-                "For systems across the U.S., load duration curves are similar from one location to another. Based on load data it was calculated that the peak load is, on average, 1.7 times the average load (a load factor of 59%). As illustrated in the figure below, when coupled with a standard reserve margin of 15\u201320% of peak load, firm capacity requirements for the U.S. should be roughly twice average load. (*Sullivan et al., 2013*)\n",
+                "For systems across the U.S., load duration curves are similar from one location to another. Based on load data it was calculated that the peak load is, on average, 1.7 times the average load (a load factor of 59%). As illustrated in the figure below, when coupled with a standard reserve margin of 15\u201320% of peak load, firm capacity requirements for the U.S. should be roughly twice average load. ([Sullivan et al., 2013](https://doi.org/10.1016/j.esr.2013.01.001))\n",
                 "\n",
                 "<img src='_static/firm-capacity.png' width='400'>\n",
                 "\n",
-                "In this example, a [`\"peak_load_factor\"`](https://docs.messageix.org/en/stable/model/MESSAGE/parameter_def.html?highlight=peak_load_factor#parameters-of-the-demand-section) of 2 is introduced for the `\"level\": \"secondary\"` and `\"commodity\": \"electricity\"`, which is the level/commodity where power plant generation is accounted."
+                "In this example, a [`\"peak_load_factor\"`](https://docs.messageix.org/en/stable/model/MESSAGE/parameter_def.html?highlight=peak_load_factor#parameters-of-the-demand-section) of 2 is introduced for the `\"level\": \"secondary\"` and `\"commodity\": \"electricity\"`, which is the level/commodity where power plant generation is accounted for."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -285,22 +287,23 @@
             "outputs": [],
             "source": [
                 "rep_scen.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
                 "rep_scen.get(\"plot activity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Capacity\n",
                 "***\n",
-                "The difference between the two scenarios can be seen when comparing the capacity. Whereas in the '*emission_bound*' scenario, coal capacity is quickly phased out, the `\"firm_capacity\"` scenario shows, that there is a substantial amount of capacity required from the `\"coal_ppl\"` in order for the `\"wind_ppl\"` to achieve such high market share levels\n",
+                "The difference between the two scenarios can be seen when comparing the capacity. Whereas in the '*emission_bound*' scenario, coal capacity is quickly phased out, the `\"firm_capacity\"` scenario shows that there is a substantial amount of capacity required from the `\"coal_ppl\"` in order for the `\"wind_ppl\"` to achieve such high market share levels.\n",
                 "\n",
-                "Please notice the different maximum values of the y-axis of both plots."
+                "Please note the different maximum values of the y-axis of both plots."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Scenario: '*emission_bound*'"
@@ -328,22 +331,23 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "rep_scen.get(\"plot capacity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Prices\n",
                 "***\n",
                 "This has a substantial impact on the electricity price, which is reflected in the prices for lighting.\n",
                 "\n",
-                "Please notice the different maximum values of the y-axis of both plots."
+                "Please note the different maximum values of the y-axis of both plots."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Scenario: '*emission_bound*'"
@@ -384,27 +388,32 @@
             "source": [
                 "mp.close_db()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_flexible_generation.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_flexible_generation.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9476508246527777%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(4, \'In the first part, we introduced [`"firm '*

 * *            'capacity"`](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=FIRM_CAPACITY_PROVISION#equation-firm-capacity-provision) '*

 * *            'constraints to ensure that conventional electricity generation plants supplied '*

 * *            'sufficient backup capacity to allow for a high share of renewable electricity '*

 * *            'generation. In this tutorial, we will address [`"flexible '*

 * *  […]*

```diff
@@ -1,28 +1,29 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Westeros Tutorial - Adding representation of renewables (part2/3): Introducing `\"flexible generation\"`\n",
                 "\n",
                 "This tutorial, which demonstrates how to apply various model features to provide a more realistic representation of renewable energy integration in the energy system, is comprised of three parts. \n",
                 "\n",
-                "In the first part, we introduced [`\"firm capacity\"`](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=FIRM_CAPACITY_PROVISION#equation-firm-capacity-provision) constraints to ensure that conventional electricity generation plants supplied sufficient backup capacity to allow for high renewable electricity generation penetration. In this tutorial, we will address [`\"flexible generation\"`](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=flexibility#equation-system-flexibility-constraint) i.e., the ability of a power plant to ramp up and down its generation in response to the system needs. The power system needs to be flexible to respond to fluctuations in both electricity load and supply.\n",
+                "In the first part, we introduced [`\"firm capacity\"`](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=FIRM_CAPACITY_PROVISION#equation-firm-capacity-provision) constraints to ensure that conventional electricity generation plants supplied sufficient backup capacity to allow for a high share of renewable electricity generation. In this tutorial, we will address [`\"flexible generation\"`](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=flexibility#equation-system-flexibility-constraint) i.e., the ability of a power plant to ramp up and down its generation in response to the system needs. The power system needs to be flexible to respond to fluctuations in both electricity load and supply.\n",
                 "\n",
-                "Further information can be found in https://doi.org/10.1016/j.esr.2013.01.001 (*Sullivan et al., 2013*).\n",
+                "Further information can be found in [Sullivan et al., 2013](https://doi.org/10.1016/j.esr.2013.01.001).\n",
                 "\n",
                 "**Pre-requisites**\n",
-                "- You have the *MESSAGEix* framework installed and working.\n",
-                "- You have run Westeros scenario which adds emission taxes (``westeros_emissions_taxes.ipynb``) and solved it successfully.\n",
+                "- You have the *MESSAGEix* framework installed and working\n",
+                "- You have run Westeros scenario which adds emission taxes (``westeros_emissions_taxes.ipynb``) and solved it successfully\n",
                 "\n",
                 "## Online documentation\n",
                 "\n",
-                "The full framework documentation is available at [https://docs.messageix.org](https://docs.messageix.org)]."
+                "The full framework documentation is available at [https://docs.messageix.org](https://docs.messageix.org)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -87,24 +88,25 @@
                 "year_df = scen.vintage_and_active_years()\n",
                 "vintage_years, act_years = year_df[\"year_vtg\"], year_df[\"year_act\"]\n",
                 "model_horizon = scen.set(\"year\")\n",
                 "country = \"Westeros\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Describing Flexibility Requirements\n",
                 "\n",
-                "Electric-sector flexibility is the ability of power system to match supply and demand at any time scale. This characteristic can be represented in a stylized way as follows: \n",
+                "Electric-sector flexibility is the ability of a power system to match supply and demand at any time scale. This characteristic can be represented in a stylized way as follows: \n",
                 "\n",
-                "Each generating technology is assigned a coefficient between \u22121 and 1 representing (if positive) the fraction of generation from that technology that is considered to be flexible or (if negative) the additional flexible generation required for each unit of generation from that technology. A negative coefficient on load reveals a parameterization of the amount of flexible energy the system requires solely to meet changes and uncertainty in load. (*Sullivan et al., 2013*)\n",
+                "Each generating technology is assigned a coefficient between \u22121 and 1 representing (if positive) the fraction of generation from that technology that is considered to be flexible or (if negative) the additional flexible generation required for each unit of generation from that technology. A negative coefficient on load reveals a parameterization of the amount of flexible energy the system requires solely to meet changes and uncertainty in load. ([Sullivan et al., 2013](https://doi.org/10.1016/j.esr.2013.01.001))\n",
                 "\n",
-                "The coefficients used in this tutorial are derived in *Sullivan et al., 2013*.\n",
+                "The coefficients used in this tutorial are derived in [Sullivan et al., 2013](https://doi.org/10.1016/j.esr.2013.01.001).\n",
                 "\n",
                 "| Technology | Flexibility parameter |\n",
                 "| :--------- | :-------------------- |\n",
                 "| Load | \u22120.1 |\n",
                 "| Wind | \u22120.08 |\n",
                 "| Solar PV | \u22120.05 |\n",
                 "| Geothermal | 0 |\n",
@@ -114,17 +116,17 @@
                 "| Gas-CC | 0.5 |\n",
                 "| Hydropower | 0.5 |\n",
                 "| H2 Electrolysis | 0.5 |\n",
                 "| Oil/gas steam | 1 |\n",
                 "| Gas-CT | 1 |\n",
                 "| Electricity storage | 1 |\n",
                 "\n",
-                "Based on the above listed coefficients, our `\"wind_ppl\"` will need fleixblity equal to 8% of its activity. Likewise, the electricity grid has a flexibility need of 10%. `\"coal_ppl\"` can provide 15% of its activity as flexibility for meeting the system needs.  \n",
+                "Based on the above listed coefficients, our `\"wind_ppl\"` will need flexibility equal to 8% of its activity. Likewise, the electricity grid has a flexibility need of 10%. `\"coal_ppl\"` can provide 15% of its activity as flexibility for meeting the system needs.  \n",
                 "\n",
-                "Recall that in the previous tutorial two `\"rating_bin\"`s were introduced for `\"wind_ppl\"`, depicting the different firm capacity requirements as market penetration increases.  We will again use the two rating bins previously defined. Here we make the assumption that the above flexibility parameter (8%) applies to the larger of two rating bins (`\"r2\"`), and assume that the smaller rating bin (`\"r1\"`) has a lower flexibility demand of 6%, correlating to the fact that the first 20% of installed capacity required contributes more to firm capacity.  "
+                "Recall that in the previous tutorial two `\"rating_bin\"`s were introduced for `\"wind_ppl\"`, depicting the different firm capacity requirements as market share increases.  We will again use the two rating bins previously defined. Here we make the assumption that the above flexibility parameter (8%) applies to the larger of the two rating bins (`\"r2\"`), and assume that the smaller rating bin (`\"r1\"`) has a lower flexibility demand of 6%, correlating to the fact that the first 20% of installed capacity required contributes more to firm capacity.  "
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Add and parametrize rating bins\n",
@@ -207,18 +209,19 @@
                 "flexibility_factor = make_df(\n",
                 "    name, **base_flexibility_factor, technology=\"coal_ppl\", rating=\"unrated\", value=0.15\n",
                 ")\n",
                 "scen.add_par(name, flexibility_factor)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Note, that `\"coal_ppl\"` has a dynamic growth constraint on activity. This constraint will render the problem infeasible due to the flexibility requirements, hence we will remove this constraint."
+                "Note that `\"coal_ppl\"` has a dynamic growth constraint on activity. This constraint will render the problem infeasible due to the flexibility requirements, hence we will remove this constraint."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -282,22 +285,23 @@
                 "prepare_plots(rep_base)\n",
                 "\n",
                 "rep_scen = Reporter.from_scenario(scen)\n",
                 "prepare_plots(rep_scen)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Activity\n",
                 "***\n",
-                "The impact of adding the flexibility constraint to electricity generation technologies on the model behavior can be observed by comparing the activity levels between the two scenarios. In the '*carbon_tax*' scenario, from which started, electricity generation from `\"wind_ppl\"` is significantly scaled up over the years. By 720, almost all the electricity is generated by the `\"wind_ppl\"`.\n",
+                "The impact of adding the flexibility constraint to electricity generation technologies on the model behavior can be observed by comparing the activity levels between the two scenarios. In the '*carbon_tax*' scenario, from which we started, electricity generation from `\"wind_ppl\"` is significantly scaled up over the years. By 720, almost all the electricity is generated by the `\"wind_ppl\"`.\n",
                 "\n",
-                "When adding the flexibility constraint, the `\"coal_ppl\"` is required to generate a larger portion of electricity in order to provide activity to meet the demanded flexibility by the \"load\" and the `\"wind_ppl\"`."
+                "When adding the flexibility constraint, the `\"coal_ppl\"` is required to generate a larger portion of electricity in order to provide activity to meet the flexibility demanded by the \"load\" and the `\"wind_ppl\"`."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Scenario: '*carbon_tax*'"
@@ -327,20 +331,21 @@
             "outputs": [],
             "source": [
                 "rep_scen.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
                 "rep_scen.get(\"plot activity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Impacts on emissions\n",
+                "### Impact on emissions\n",
                 "***\n",
-                "As a further consequnece, the `\"carbon_tax\"`, which remains unchanged, does not result in emission reductions achieved in the '*carbon_tax*' scenario as shown below. We can see, that the emissions in 720 increase almost fivefold. Hence, adding the flexibility requirements to the scenario will require the `\"carbon_tax\"` to be increased  significantly to achieve the same emission reducitons. Alterantively, a technology which contributes more of its activity to the flexibility constraint, like a gas combustion turbine, could be added to the model."
+                "As a further consequence, the `\"carbon_tax\"`, which remains unchanged, does not result in the same emission reductions as achieved in the '*carbon_tax*' scenario (shown below). We can see that the emissions in 720 increase almost fivefold. Hence, adding the flexibility requirements to the scenario will require the `\"carbon_tax\"` to be increased  significantly to achieve the same emission reductions. Alternatively, a technology which contributes more of its activity to the flexibility constraint, like a gas combustion turbine, could be added to the model."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Scenario: '*carbon_tax*'"
@@ -422,27 +427,32 @@
             "source": [
                 "mp.close_db()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_fossil_resource.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_fossil_resource.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9477407484311554%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(5, \'"Reserves" are generally defined as being those '*

 * *            'quantities for which geological and engineering information indicate with reasonable '*

 * *            'certainty that they can be recovered in the future from known reservoirs under '*

 * *            'existing economic and operating conditions. "Resources" are detected quantities that '*

 * *            'cannot be profitably recovered with current technology, but might be recoverable in '*

 * *            'the future […]*

```diff
@@ -1,19 +1,20 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Westeros Tutorial - Introducing resource: Adding fossil resources\n",
                 "\n",
                 "This tutorial shows how to add fossil fuel resources in the form of resource supply curves to a MESSAGEix scenario. This includes defining `\"resource_volume\"` and `\"resource_cost\"`. Multiple resource categories can be added for a single commodity like coal, allowing, for example, a differentiation between '*reserves*' and '*resources*', the quality, or location of the resources, i.e., above or below ground, or on- or off-shore.\n",
                 "\n",
                 "## Difference between reserves and resources\n",
-                "\"Reserves\" are generally defined as being those quantities for which geological and engineering information indicate with reasonable certainty that they can be recovered in the future from known reservoirs under existing economic and operating conditions. \"Resources\" are detected quantities that cannot be profitably recovered with current technology, but might be recoverable in the future, as well as those quantities that are geologically possible, but yet to be found. Definitions are based on Rogner et al. (2012). \n",
+                "\"Reserves\" are generally defined as being those quantities for which geological and engineering information indicate with reasonable certainty that they can be recovered in the future from known reservoirs under existing economic and operating conditions. \"Resources\" are detected quantities that cannot be profitably recovered with current technology, but might be recoverable in the future, as well as those quantities that are geologically possible, but yet to be found. Definitions are based on [Rogner et al. (2012)](https://doi.org/10.1017/CBO9780511793677.013). \n",
                 "\n",
                 "In this tutorial, we add two categories of coal resources. We assume a resource potential based on the coal requirements by the `\"coal_ppl\"` in the baseline scenario. We also show the use of multiple resource categories. \n",
                 "\n",
                 "Two further tutorials on adding fossil resources are available, which will elaborate on the modelling of fossil resources. Part (ii) will introduce the constraint `\"resource_remaining\"`, for specifying what share of these resources must be preserved over time.  In Part (iii), we will further add a coal extraction technology, linking the coal resources to the primary energy level, which can be used to model energy requirements of the extraction process.\n",
                 "\n",
                 "**Pre-requisites**\n",
                 "- You have the *MESSAGEix* framework installed and working\n",
@@ -97,19 +98,20 @@
                 "   - `\"historical_extraction\"`\n",
                 "\n",
                 "\n",
                 "3. Linking the existing `\"coal_ppl\"` technology to the relevant resource, by updating the `\"input\"` parameter."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 1. Defining level, grade, and commodity\n",
-                "We define two grades *a and b* for coal resources. Later, we define different costs for these grades."
+                "We define two grades *a* and *b* for coal resources. Later, we define different costs for these grades."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -120,19 +122,20 @@
                 "scen.add_set(\"commodity\", commodity)\n",
                 "scen.add_set(\"level\", level)\n",
                 "scen.add_set(\"level_resource\", level)\n",
                 "scen.add_set(\"grade\", [\"a\", \"b\"])"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 2. Setting up parameters\n",
-                "Based on the coal use in the *baseline* scenario, we set a sufficient potential for coal resources to be used by `\"coal_ppl\"`. In real examples, the amount of resources can be limited, which will be one of the criteria for employing different technologies. We update parameter `\"historical_extraction\"`, though it is not used in this tutorial. We show this as it can be useful when there is a history of resource extraction."
+                "Based on the coal use in the *baseline* scenario, we set a sufficient potential for coal resources to be used by `\"coal_ppl\"`. In real examples, the amount of resources can be limited, which will be one of the criteria for employing different technologies. We update the parameter `\"historical_extraction\"`, though it is not used in this tutorial. We show this as it can be useful when there is a history of resource extraction."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -146,15 +149,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Information for each \"grade\" including, potential, costs, historical extraction:\n",
+                "# Information for each \"grade\" including potential, costs, historical extraction:\n",
                 "potentials = {\"a\": [1500, 10, 280], \"b\": [3500, 52, 0]}"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -298,20 +301,21 @@
                 "\n",
                 "# Scenario with coal resource potentials added\n",
                 "rep = Reporter.from_scenario(scen)\n",
                 "prepare_plots(rep)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Activity\n",
                 "***\n",
-                "When comparing the results of the original scenario without coal resource potentials ('*baseline*') to the results of our newly modified scenario ('*fossil_resources*'), the activity of the both electricity generation technologies is the same."
+                "When comparing the results of the original scenario without coal resource potentials ('*baseline*') to the results of our newly modified scenario ('*fossil_resources*'), the activity of the electricity generating technologies is the same."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Scenario: '*baseline*'"
@@ -383,20 +387,21 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "rep.get(\"plot capacity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Prices\n",
                 "***\n",
-                "The impact of introducing coal resources and therewith associated costs, only becomes noticeable when looking at prices for `\"light\"`.  Especially in the latter two timeperiods the impact is noticable, where prices increase  from below 2cents/kWhr in the '*baseline*' scenario to ~2.5cents/kWhr."
+                "The impact of introducing coal resources and therewith associated costs only becomes noticeable when looking at prices for `\"light\"`.  Especially in the latter two timeperiods the impact is noticable, where prices increase from below 2cents/kWhr in the '*baseline*' scenario to ~2.5cents/kWhr."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Scenario: '*baseline*'"
@@ -427,20 +432,21 @@
             "outputs": [],
             "source": [
                 "rep.set_filters(**filters)\n",
                 "rep.get(\"plot prices\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Extraction\n",
                 "***\n",
-                "In the first plot below, we can see the coal supply curve. In the figure below, depicting extraction over time, we can see that the model uses up the available potential of the cheaper `\"grade\"` *a* early on. The switch to the more expensive `\"grade\"` *b* as of 710, which is the reason forthe increase in the price of `\"light\"`."
+                "In the first plot below, we can see the coal supply curve. In the figure below, depicting extraction over time, we can see that the model uses up the available potential of the cheaper `\"grade\"` *a* early on. The switch to the more expensive `\"grade\"` *b* happens as of 710, which is the reason for the increase in the price of `\"light\"`."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Scenario: '*fossil_resource*'"
@@ -488,27 +494,32 @@
             "source": [
                 "mp.close_db()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_historical_new_capacity.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_historical_new_capacity.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916732334744011%*

 * *Differences: {"'cells'": "{9: {'source': {insert: [(9, 'In order to account for these dependencies, we can use "*

 * *            'the parameters `"historical_new_capacity"`, `"historical_capacity"` and '*

 * *            '`"historical_emissions"` respectively.\\n\'), (11, \'In the case of emissions, '*

 * *            '`"historical_emissions"` can be accounted for in cumulative emission bounds.\\n\')], '*

 * *            "delete: [11, 9]}, 'attachments': OrderedDict()}, 12: {'source': {insert: [(4, '  - We "*

 * *            'will reduce the e […]*

```diff
@@ -113,29 +113,30 @@
             "outputs": [],
             "source": [
                 "country = \"Westeros\"\n",
                 "model_horizon = [700, 710, 720]"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-block alert-success\">\n",
                 "\n",
                 "### A quick look at historical parameters and their purpose\n",
                 "\"Historical parameters\" can only be set for \"historical time-periods\".\n",
                 "The \"historical time-periods\" are all the years which have been defined prior to the `firstmodelyear`.\n",
                 "These can be used for two purposes.\n",
                 "\n",
                 "1. For **calibration of the model**: The `firstmodelyear` is used to specify as of which time-period the \"optimization\" should be carried out.\n",
                 "There will be some past dependencies though, such as technology investments, their activity or emissions amongst others.\n",
-                "In order to account for these dependencies, we can use the parameters `\"historical_new_capacity\"`, \"historical_capacity\" and \"historical_emissions\" respectively.\n",
+                "In order to account for these dependencies, we can use the parameters `\"historical_new_capacity\"`, `\"historical_capacity\"` and `\"historical_emissions\"` respectively.\n",
                 "These will have implications on dynamic constraints on capacities or activity.\n",
-                "In the case of emissions, \"historical_emissions\" can be accounted for in cumulative emission bounds.\n",
+                "In the case of emissions, `\"historical_emissions\"` can be accounted for in cumulative emission bounds.\n",
                 "2. The second application is when running **complex scenario setups**.\n",
                 "If for example the aim is to assess climate mitigation efforts based on achieving the NDCs in 2030, then two scenarios can be run.\n",
                 "Scenario a) implements \"only\" the NDCs related policies up to 2030 (see dashed orange line *\\\"NDC\\\"* in the panel a. of the figure below).\n",
                 "After 2030, there is no continuation of policies assumed, hence the model will return to a \"baseline\" trajectory (see solid blue line *\\\"Baseline\\\"* in the panel a. of the figure below).\n",
                 "This scenario will then serve as a basis for further analysis - e.g. scenario b) (see red dashed line *\\\"NDC-mitigation\\\"* in panel b. in the figure below).\n",
                 "In order to avoid an \"overachievement\" of the NDCs, the time-periods until 2030 should be *fixed*.\n",
                 "The historical time-periods (see the extension of the grey block in panel b. in the figure below) are therefore shifted.\n",
@@ -169,44 +170,46 @@
                 "print(f\"the `firstmodelyear` is {scenario.firstmodelyear}\")\n",
                 "\n",
                 "# Retrieve historic time-steps\n",
                 "history = [y for y in years if y < scenario.firstmodelyear]"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Part 1.: Parametrizing `\"historical_new_capacity\"`\n",
                 "We are going to undertake a few simplications of the baseline scenario to demonstrate how to set the parameter `\"historical_new_capacity\"`.\n",
                 "\n",
                 "- Step 1.1: Scenario simplifications.\n",
-                "  - We will reduce the example to a single technology, by removing `\"wind_ppl\"`.\n",
-                "  - We will change the `\"demand\"` to remain constant.\n",
+                "  - We will reduce the example to a single technology, by removing `\"wind_ppl\"`\n",
+                "  - We will change the `\"demand\"` to remain constant\n",
                 "- Step 1.2: Scenario adjustments to account for simplifications.\n",
-                "  - We will remove the growth constraint for `\"coal_ppl\"`.\n",
-                "  - We will reparametrize \"historical_new_capacity\" so that `\"coal_ppl\"` can meet demand in the `firstmodelyear`.\n",
-                "  - We will adjust the technical lifetime of `\"coal_ppl\"`."
+                "  - We will remove the growth constraint for `\"coal_ppl\"`\n",
+                "  - We will reparametrize `\"historical_new_capacity\"` so that `\"coal_ppl\"` can meet demand in the `firstmodelyear`\n",
+                "  - We will adjust the technical lifetime of `\"coal_ppl\"`"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Step 1.1.: Scenario simplifications"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Remove `\"wind_ppl\"`\n",
-                "First, we are going to remove the technology 'wind_ppl'.\n",
-                "Later on in the tutorial we are instead going to add a more efficient gas powerplant.\n",
-                "We do this, because we want to introduce a technology, which will result in the early retirement of the current coal_ppl."
+                "First, we are going to remove the technology `\"wind_ppl\"`.\n",
+                "Later on in the tutorial we are instead going to add a more efficient gas power plant.\n",
+                "We do this because we want to introduce a technology which will result in the early retirement of the current `\"coal_ppl\"`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -219,18 +222,19 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Adjust `\"demand\"`"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Next we will modify the demand to remain constant, hence to avoid the requirement in the optimization time-period to build any new capacity"
+                "Next we will modify the demand to remain constant, hence to avoid the requirement in the optimization time-period to build any new capacity."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -245,41 +249,43 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Step 1.2: Adjust `\"coal_ppl\"`"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Remove dynamic growth constraints\n",
-                "Now, we will remove the growth constraint on the current coal_ppl."
+                "Now, we will remove the growth constraint on the current `\"coal_ppl\"`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "df = scenario.par(\"growth_activity_up\", filters={\"technology\": \"coal_ppl\"})\n",
                 "scenario.remove_par(\"growth_activity_up\", df)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Reparametrize `\"historical_new_capacity\"`\n",
-                "Now, the `\"historical_new_capacity\"` parameter of `\"coal_ppl\"` will be adjusted so that sufficient capacity is installed in 690, to meet demand in the `firstmodelyear`.\n",
+                "Now, the `\"historical_new_capacity\"` parameter of `\"coal_ppl\"` will be adjusted so that sufficient capacity is installed in 690, to meet the demand in the `firstmodelyear`.\n",
                 "\n",
-                "- Retrieve demand of `firstmodelyear`.\n",
-                "- Account for grid losses. As both the `\"capacity_factor\"` and efficicency for `\"coal_ppl\"` are one, these need not be accounted for.\n",
-                "- Account for duration of the time-period, as the parameter `\"historical_new_capacity\"` is an annual value."
+                "- Retrieve demand of `firstmodelyear`\n",
+                "- Account for grid losses. As both the `\"capacity_factor\"` and efficicency for `\"coal_ppl\"` are one, these need not be accounted for\n",
+                "- Account for duration of the time-period, as the parameter `\"historical_new_capacity\"` is an annual value"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -295,15 +301,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# We know that there are loses that occur when electricity is transmitted via the `grid`.\n",
+                "# We know that there are losses that occur when electricity is transmitted via the `grid`.\n",
                 "grid_eff = float(\n",
                 "    scenario.par(\n",
                 "        \"output\",\n",
                 "        filters={\n",
                 "            \"year_vtg\": scenario.firstmodelyear,\n",
                 "            \"year_act\": scenario.firstmodelyear,\n",
                 "            \"technology\": \"grid\",\n",
@@ -455,63 +461,65 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For the optimization time-periods, we can see from the above figure that `\"coal_ppl\"` capacity remains constant."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-block alert-success\">\n",
                 "    \n",
                 "**New capacity installations vs. Total installed capacity**\n",
                 "\n",
                 "In the figure below we have illustrated the correlation between new capacity installations (left hand side) and total installed capacity.\n",
-                "The corresponding scenario results can be retrieved executing `scenario.var(\"CAP_NEW\")` and `scenario.var(\"CAP\")` respectively.\n",
+                "The corresponding scenario results can be retrieved executing `scenario.var(\"CAP_NEW\")` and `scenario.var(\"CAP\")`, respectively.\n",
                 "\n",
                 "As can be seen in the left hand panel, new capacity is installed at two points in time.\n",
                 "The first occurs in a *historical* time-period, in the year 690.\n",
                 "The investment costs for these capacities lie outside the optimization time-frame.\n",
                 "Therefore these do not contribute to the objective function.\n",
-                "The powerplant in our example has a `\"technical_lifetime\"` of 20 years.\n",
+                "The power plant in our example has a `\"technical_lifetime\"` of 20 years.\n",
                 "The capacity installed in 690 will therefore need to be replaced in 710.\n",
                 "The investment costs for this capacity addition is therefore accounted for in 710.\n",
                 "    \n",
                 "In the righthand panel, we can see the corresponding total installed capacity.\n",
-                "The `\"duration_period\"` of the time-steps in our example are always 10 years.\n",
+                "The `\"duration_period\"` of the time-steps in our example is always 10 years.\n",
                 "In order to determine the total installed capacity, we can multiply the new installed capacity, which is an annual value, by 10. \n",
                 "    \n",
                 "<img src='_static/historical_new_capacity_and_total_installed_capacity.png' width='800'>\n",
                 "    \n",
-                "**NOTE: that if the technical lifetime is such that it covers a time-period only partially, then the total installed capacity shown in the variable \"CAP\", will only reflect the number of years covered.**"
+                "**NOTE: if the technical lifetime is such that it covers a time-period only partially, then the total installed capacity shown in the variable \"CAP\", will only reflect the number of years covered.**"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Part 2.: Exploring early retirement.\n",
+                "## Part 2.: Exploring early retirement\n",
                 "In order to demonstrate early retirement of technologies, we are going to add a new, cheaper electricity generation technology.\n",
                 "We will then look at what parameters can be used to *force* the model to use *non-economical* technology options.\n",
                 "\n",
-                "- Step 2.1: Add technology `\"gas_ppl\"`.\n",
-                "  - We will add the technology `\"gas_ppl\"` to the set `\"technology\"`.\n",
-                "  - We will add parameters `\"output\"`, `\"capacity_factor\"`, `\"technical_lifetime\"`, `\"inv_cost\"` and `\"var_cost\"` (the parameters are listed in the table below).\n",
+                "- Step 2.1: Add technology `\"gas_ppl\"`\n",
+                "  - We will add the technology `\"gas_ppl\"` to the set `\"technology\"`\n",
+                "  - We will add the parameters `\"output\"`, `\"capacity_factor\"`, `\"technical_lifetime\"`, `\"inv_cost\"` and `\"var_cost\"` (the parameters are listed in the table below)\n",
                 "\n",
                 "| Parameter  | coal_ppl | gas_ppl |\n",
                 "| :--------- | :--------- | :-------- |\n",
                 "| Efficiency \\[%\\] | 100 | 100 |\n",
                 "| Capacity factor \\[%\\] | 100 | 100 |\n",
                 "| Technical lifetime \\[years\\] | 20 | 40 |\n",
                 "| Investment costs \\[USD/kW\\] | 500 | 300 |\n",
                 "| Variable costs \\[USD/kWa\\] | 30 | 10 |\n",
                 "\n",
                 "  \n",
-                "- Step 2.2: Explore parameters that can force the use of `\"coal_ppl\"`, despite being uneconomical.\n",
+                "- Step 2.2: Explore parameters that can force the use of `\"coal_ppl\"`, despite being uneconomical\n",
                 "  - `\"bound_capacity_lo\"`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -522,18 +530,19 @@
                 "    scenario=\"baseline_historic_new_capacity_part2\",\n",
                 "    keep_solution=False,\n",
                 ")\n",
                 "scenario2.check_out()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Define generic Functions"
+                "# Define generic functions"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -602,18 +611,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "scenario2.add_set(\"technology\", [\"gas_ppl\"])"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Parmetrize `\"output\"`"
+                "#### Parametrize `\"output\"`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -750,19 +760,20 @@
             "outputs": [],
             "source": [
                 "rep2 = Reporter.from_scenario(scenario2)\n",
                 "prepare_plots(rep2)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Capacity\n",
-                "We will first plot the capacity of our first scenario and then compare these to the capacity installations for the exmple for which we added the cheaper electricity generation option, `\"gas_ppl\"`."
+                "We will first plot the capacity of our first scenario and then compare these to the capacity installations for the example for which we added the cheaper electricity generation option, `\"gas_ppl\"`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -793,45 +804,47 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "scenario2.var(\"CAP\", filters={\"technology\": [\"coal_ppl\", \"gas_ppl\"]})"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Step 2.2: Using bounds to force the model to use `\"coal_ppl\"`\n",
                 "There are multiple bounds that can be used to *force* the model to use the historical capacity of `\"coal_ppl\"` until the end of its lifetime.\n",
-                "- `\"bound_total_capacity_lo\"` (possibly in combination with `\"bound_total_capacity_up\"`).\n",
-                "- `\"bound_activity_lo\"` (possibly in combination with `\"bound_activity_up\"`).\n",
-                "- dynamic constraints on activity and/or capacity.\n",
-                "- `\"fixed_activity\"` or `\"fixed_capacity\"` can also be used."
+                "- `\"bound_total_capacity_lo\"` (possibly in combination with `\"bound_total_capacity_up\"`)\n",
+                "- `\"bound_activity_lo\"` (possibly in combination with `\"bound_activity_up\"`)\n",
+                "- dynamic constraints on activity and/or capacity\n",
+                "- `\"fixed_activity\"` or `\"fixed_capacity\"` can also be used"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "scenario2.remove_solution()\n",
                 "scenario2.check_out()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### `\"bound_total_capacity_lo\"`\n",
-                "Add lower bound on capacity for `\"coal_ppl\"` in `\"year_act\"` installed in 690.\n",
+                "Add a lower bound on capacity for `\"coal_ppl\"` in `\"year_act\"` installed in 690.\n",
                 "\n",
                 "In order to calculate the `\"bound_capacity_lo\"`, we first need to retrieve the `\"historical_new_capacity\"`. As this is an annual value, we will need to account for the `\"duration_period\"` when defining the `\"bound_capacity_lo\"`.\n",
                 "\n",
-                "**NOTE: That `\"bound_capacity_lo\"` is indexed over the activity years, so if there are multiple vintages installed in historical years, their individual `\"technical_lifetime\"` will need to be accounted for when formualting the constraint.**"
+                "**NOTE: `\"bound_capacity_lo\"` is indexed over the activity years, so if there are multiple vintages installed in historical years, their individual `\"technical_lifetime\"`s will need to be accounted for when formulating the constraint.**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -889,19 +902,20 @@
             "outputs": [],
             "source": [
                 "rep2 = Reporter.from_scenario(scenario2)\n",
                 "prepare_plots(rep2)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Capacity\n",
-                "When plotting capacity, we can see that the bound has in fact achieved the desired effect, but only partialy. While the capacity of the `\"coal_ppl\"` is maintained, we can also observe that the capacity for `\"gas_ppl\"` is also built in the `firstmodelyear`. This can be caused for example, because there are no costs associated with maintaining the capacity of `\"coal_ppl\"` i.e. as we haven't defined fixed operating and maintance costs."
+                "When plotting the capacity, we can see that the bound has in fact achieved the desired effect, but only partially. While the capacity of the `\"coal_ppl\"` is maintained, we can also observe that the capacity for `\"gas_ppl\"` is also built in the `firstmodelyear`. This can e.g. be caused by there being no costs associated with maintaining the capacity of `\"coal_ppl\"` i.e. we haven't defined fixed operating and maintance costs."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -924,42 +938,44 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "rep2.get(\"plot activity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "so, an alternative would be to use the `\"bound_activity_lo\"`."
+                "So, an alternative would be to use the `\"bound_activity_lo\"`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "scenario2.remove_solution()\n",
                 "scenario2.check_out()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### `\"bound_activity_lo\"`\n",
-                "Add lower bound on activity for 'coal_ppl' in `\"year_act\"` installed in 690.\n",
+                "Add a lower bound on activity for `\"coal_ppl\"` in `\"year_act\"` installed in 690.\n",
                 "\n",
                 "In order to calculate the `\"bound_activity_lo\"`, we first need to retrieve the `\"historical_new_capacity\"`.\n",
                 "As this is an annual value, we will need to account for the `\"duration_period\"` when defining the `\"bound_activity_lo\"`.\n",
-                "We would normally also need to account for the `\"capacity_factor\"` as well as the efficiency, but we know that there are both 1.\n",
+                "We would normally also need to account for the `\"capacity_factor\"` as well as the efficiency, but we know that they are both 1.\n",
                 "\n",
-                "**NOTE: That `\"bound_activity_lo\"` is indexed over the activity years, so if there are multiple vintages installed in historical years, their individual `\"technical_lifetime\"` will need to be accounted for when formualting the constraint.**"
+                "**NOTE: `\"bound_activity_lo\"` is indexed over the activity years, so if there are multiple vintages installed in historical years, their individual `\"technical_lifetime\"`s will need to be accounted for when formulating the constraint.**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1042,37 +1058,39 @@
             "outputs": [],
             "source": [
                 "rep2 = Reporter.from_scenario(scenario2)\n",
                 "prepare_plots(rep2)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Capacity\n",
-                "If we now replot capacity, we can see that capacity for `\"gas_ppl\"` is only added of 710."
+                "If we now replot the capacity, we can see that capacity for `\"gas_ppl\"` is only added as of 710."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "rep2.set_filters(t=[\"coal_ppl\", \"gas_ppl\"])\n",
                 "rep2.get(\"plot capacity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Activity\n",
-                "Look at the results for activity, we can see that `\"coal_ppl\"` generating electricity up until the year 700."
+                "Looking at the results for activity, we can see that `\"coal_ppl\"` is generating electricity up until the year 700."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_renewable_resource.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_renewable_resource.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9440823151527669%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'In the third part we will show you how to introduce "*

 * *            'renewable resource potentials.  Up until now, `"wind_ppl"` activity was '*

 * *            'unrestricted.  In order to reflect the fact that there are limited wind potentials '*

 * *            'within a given region and the fact that these differ in quality, we will add '*

 * *            "[`renewable_potentials`][1] and [`renewable_capacity_factors`][1] for wind.\\n'), (5, "*

 * *            "'\\n'), (6, '[1]: "*

 * *     […]*

```diff
@@ -1,22 +1,25 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Westeros Tutorial - Adding representation of renewables (part 3/3): Introducing `renewable_resource_constraints`\n",
                 "\n",
                 "This tutorial, which demonstrates how to apply various model features to provide a more realistic representation of renewable energy integration in the energy system, is comprised of three parts. Previously, we introduced constraints on [`\"firm capacity\"`](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=FIRM_CAPACITY_PROVISION#equation-firm-capacity-provision) and [`\"flexible generation\"`](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=flexibility#equation-system-flexibility-constraint).\n",
                 "\n",
-                "In the third part we will show you how to introduce renewable resource potentials.  Up until now, `\"wind_ppl\"` activity was unrestricted.  In order to reflect the fact that there are limited wind potentials within a given region and the fact that these differ in quality, we will add introduce [`renewable_potentials` and `renewable_capacity_factors`](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=renewable#constraints-representing-renewable-integration) for wind.\n",
+                "In the third part we will show you how to introduce renewable resource potentials.  Up until now, `\"wind_ppl\"` activity was unrestricted.  In order to reflect the fact that there are limited wind potentials within a given region and the fact that these differ in quality, we will add [`renewable_potentials`][1] and [`renewable_capacity_factors`][1] for wind.\n",
+                "\n",
+                "[1]: https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html?highlight=renewable#constraints-representing-renewable-integration\n",
                 "\n",
                 "<img src='_static/renewable_resource_res.png' width='900'>\n",
                 "\n",
-                "Further information can be found in https://doi.org/10.1016/j.esr.2013.01.001 (*Sullivan et al., 2013*)\n",
+                "Further information can be found in [Sullivan et al., 2013](https://doi.org/10.1016/j.esr.2013.01.001).\n",
                 "\n",
                 "**Pre-requisites**\n",
                 "- You have the *MESSAGEix* framework installed and working\n",
                 "- You have run Westeros scenario which adds emission taxes (`westeros_emissions_taxes.ipynb`) and solved it successfully"
             ]
         },
         {
@@ -38,19 +41,20 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "mp = ixmp.Platform()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Load existing and clone to new scenario\n",
-                "We load the existing scenario '*carbon_tax*' and clone it to a new scenario '*renewable_potential*' to which we will apply the `renewable_resource_constraints` constraint"
+                "We load the existing scenario '*carbon_tax*' and clone it to a new scenario '*renewable_potential*' to which we will apply the `renewable_resource_constraints` constraint."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -63,19 +67,20 @@
                 "    \"illustration of renewable_resource_constraint formulation\",\n",
                 "    keep_solution=False,\n",
                 ")\n",
                 "scen.check_out()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Retrieve parameters\n",
-                "We will retrieve those parameters necessary to perform subsequent additions of parameters"
+                "We will retrieve those parameters necessary to perform subsequent additions of parameters."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -83,14 +88,15 @@
                 "year_df = scen.vintage_and_active_years()\n",
                 "vintage_years, act_years = year_df[\"year_vtg\"], year_df[\"year_act\"]\n",
                 "model_horizon = scen.set(\"year\")\n",
                 "country = \"Westeros\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## `renewable_resource_constraints` - Describing the renewable resource potentials\n",
                 "From the previous tutorials we know that in 720 wind capacity reaches over 150 GWa. We will therefore define 4 wind potential categories which in total will provide 200 GWa, yet the quality of these potentials will vary substantially from the current assumptions, where the capacity factor for `\"wind_ppl\"` has been assumed to be 1, meaning that the installed `\"wind_ppl\"` capacity can operate 8760 hours per year i.e., 100% of the year. Depending on the region, high quality on-shore wind potentials result in capacity factors around 35%, yet the majority of the potentials will lie below this value.  Therefore, 4 resource categories will be introduced:\n",
                 "\n",
                 "| Resource Category | Potential \\[GWa\\] | Capacity Factor \\[%\\] |\n",
@@ -104,31 +110,32 @@
                 "\n",
                 "<img src='_static/westeros_renewable_resource_potentials.png' width='500'>\n",
                 "\n",
                 "The capacity factor of the `\"wind_ppl\"` will remain unchanged and will be reflected in the parametrization of the renewable resources.  \n",
                 "\n",
                 "The following steps are required:\n",
                 "1. Add level and commodity:\n",
-                "   - Specify and new level and commodity which accounts for the wind potentials and which serve as inputs to the `\"wind_ppl\"`\n",
+                "   - Specify a new level and commodity which account for the wind potentials and which serve as inputs to the `\"wind_ppl\"`\n",
                 "   - Specify which level is a `\"level_renewable\"`\n",
                 "2. Modify existing renewable technology:\n",
                 "   - Specify which technology is classified as a `\"type_tec\"` `\"renewable\"` (optional) \n",
                 "   - Modify the input of the `\"wind_ppl\"`\n",
                 "3. Add potentials and corresponding capacity factors:\n",
                 "   - Add grades\n",
                 "   - Add `\"renewable_potential\"`s\n",
-                "   - Add `\"renewable_capacity_factor\"`"
+                "   - Add `\"renewable_capacity_factor\"`s"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 1. Add level and commodity\n",
-                "The level and commodity which we add will allow us to account for potentials for wind"
+                "The level and commodity which we add will allow us to account for potentials for wind."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -142,19 +149,20 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 2. Modify existing renewable technology"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Define a new technology category `\"renewable\"`\n",
-                "We will define `\"type_tec\"` and add `\"wind_ppl\"` to this new category. This can be used for example, to simplify the reporting code, where results can be retrieved for technologies within a given sets as opposed to specifying individual technologies."
+                "We will define `\"type_tec\"` and add `\"wind_ppl\"` to this new category. This can be used e.g. to simplify the reporting code, where results can be retrieved for technologies within given sets as opposed to specifying individual technologies."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -219,19 +227,20 @@
             "outputs": [],
             "source": [
                 "grades = [\"c1\", \"c2\", \"c3\", \"c4\"]\n",
                 "scen.add_set(\"grade\", grades)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Add `\"renewable_potential\"`s\n",
-                "Note, that unlike fossil resources which are finite, renewable resources must be defined for each year."
+                "Note that unlike fossil resources which are finite, renewable resources must be defined for each year."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -253,18 +262,19 @@
                 "df = pd.DataFrame(\n",
                 "    {\"value\": sorted([100, 50, 25, 25] * len(model_horizon), reverse=True)}, idx\n",
                 ").reset_index()\n",
                 "scen.add_par(\"renewable_potential\", df)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Add `\"renewable_capacity_factor\"`"
+                "#### Add `\"renewable_capacity_factor\"`s"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -344,21 +354,22 @@
                 "prepare_plots(rep_base)\n",
                 "\n",
                 "rep_scen = Reporter.from_scenario(scen)\n",
                 "prepare_plots(rep_scen)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Activity\n",
                 "***\n",
                 "When comparing the results of the original scenario without the renewable potentials ('*carbon_tax*') with the results of our newly modified scenario ('*renewable_potential*'), for the same carbon price we can observe that the activity of the `\"wind_ppl\"` has substantially decreased.  This is because through adding potentials with corresponding plant factors, the `\"wind_ppl\"` has become increasingly economically unattractive and despite the carbon tax is not used. \n",
-                "Note, that the `\"coal_ppl\"` still has a plant factor of 1 and has no resource constraints, thus in order to further improve the model, the parameters for the `\"coal_ppl\"` would need to be adjusted."
+                "Note that the `\"coal_ppl\"` still has a plant factor of 1 and has no resource constraints, thus in order to further improve the model, the parameters for the `\"coal_ppl\"` would need to be adjusted."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Scenario: '*carbon_tax*'"
@@ -388,20 +399,21 @@
             "outputs": [],
             "source": [
                 "rep_scen.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
                 "rep_scen.get(\"plot activity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Capacity\n",
                 "***\n",
-                "The behavior observed for the activity of the two electricity generation technologies is reflected in the capacity. No further capacity is built for the `\"wind_ppl\"` and thus is phased out by 720."
+                "The behavior observed for the activity of the two electricity generating technologies is reflected in the capacity. No further capacity is built for the `\"wind_ppl\"` and thus it is phased out by 720."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Scenario: '*carbon_tax*'"
@@ -481,51 +493,57 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "mp.close_db()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-block alert-success\">\n",
                 "    \n",
                 "***Additional exercise***\n",
                 "    \n",
-                "The renewable potential categories have been defined such that `\"capacity_factor\"` decreases with increasing potentials. The model will thus first make of use the renewable potential with the highest capacity factor, and when saturated, the model proceed with the next highest capacity factor. Typically, the potentials of better quality are not necessarily located close to the demand centers. As an exercise in separate tutorial, add cost to these potentials, by adding one technology for each grade, called something like \"connection_to_grid_\\<potential grade name\\>\", with variable costs as shown in the table below.\n",
+                "The renewable potential categories have been defined such that `\"capacity_factor\"` decreases with increasing potentials. The model will thus first make of use the renewable potential with the highest capacity factor, and when saturated, the model proceeds with the next highest capacity factor. Typically, the potentials of better quality are not necessarily located close to the demand centers. As an exercise in a separate tutorial, add a cost to these potentials, by adding one technology for each grade, called something like \"connection_to_grid_\\<potential grade name\\>\", with variable costs as shown in the table below.\n",
                 "    \n",
                 "| Resource Category | Potential \\[GWa\\] | Capacity Factor \\[%\\] | Variable OM Cost in \\[USD/kWa\\] |\n",
                 "| :---------------- | :---------------- | :-------------------- | :------------------------------|\n",
                 "| c1 | 100 | 15 | 1 |\n",
                 "| c2 | 50 | 20 | 15 |\n",
                 "| c3 | 25 | 25 | 10 |\n",
                 "| c4 | 25 | 30 | 30 |\n",
                 "    \n",
-                "Remember that each of the renewable potential categories will require an individual `\"commodity\"` the `\"wind_ppl\"`.\n",
+                "Remember that each of the renewable potential categories will require an individual `\"commodity\"` as input to the `\"wind_ppl\"`.\n",
                 "    \n",
                 "<img src='_static/renewable_resource_res_exercise.png' width='900'>"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_report.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_report.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9494233310608193%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(10, '- You have the *MESSAGEix* framework installed and "*

 * *            "working\\n'), (11, '  In particular, you should have installed "*

 * *            '``message_ix[report]``, which requires ``ixmp[report]``, ``genno[compat]``, and '*

 * *            "``plotnine``\\n'), (13, '  - Understand the following MESSAGEix terms: ‘variable’, "*

 * *            "‘parameter’\\n'), (15, '  Some text in this tutorial is drawn from that page, and it "*

 * *            "provides a concise reference fo […]*

```diff
@@ -1,32 +1,34 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Westeros Tutorial - Introducing reporting\n",
                 "\n",
                 "\u2018Reporting\u2019 is the term used in the MESSAGEix ecosystem to refer to any calculations performed _after_ the MESSAGE mathematical optimization problem has been solved.\n",
                 "\n",
                 "This tutorial introduces the reporting features provided by the ``ixmp`` and ``message_ix`` packages.\n",
                 "It was developed by Paul Natsuo Kishimoto ([@khaeru](https://github.com/khaeru)) for a MESSAGEix training workshop held at IIASA in October 2019.\n",
                 "Participants in the MESSAGEix workshops of June and September 2020 contributed feedback.\n",
                 "<!-- Add a line here if you revise the tutorial! -->\n",
                 "\n",
                 "**Pre-requisites**\n",
-                "- You have the *MESSAGEix* framework installed and working.\n",
-                "  In particular, you should have installed ``message_ix[report]``, which requires ``ixmp[report]``, ``genno[compat]``, and ``plotnine``.\n",
+                "- You have the *MESSAGEix* framework installed and working\n",
+                "  In particular, you should have installed ``message_ix[report]``, which requires ``ixmp[report]``, ``genno[compat]``, and ``plotnine``\n",
                 "- Complete tutorial Part 1 (``westeros_baseline.ipynb``)\n",
-                "  - Understand the following MESSAGEix terms: \u2018variable\u2019, \u2018parameter\u2019.\n",
+                "  - Understand the following MESSAGEix terms: \u2018variable\u2019, \u2018parameter\u2019\n",
                 "- Open the [\u2018Reporting\u2019 page in the MESSAGEix documentation](https://docs.messageix.org/en/stable/reporting.html); bookmark it or keep it open in a tab.\n",
-                "  Some text in this tutorial is drawn from that page, and it provides a concise reference for concepts explained below."
+                "  Some text in this tutorial is drawn from that page, and it provides a concise reference for concepts explained below"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Introduction\n",
                 "### What does \u2018reporting\u2019 include?\n",
                 "\n",
                 "Individual modelers will make different distinctions between\u2014on one hand\u2014the internals of an optimization model and\u2014on the other\u2014reporting, \u2018post-processing\u2019, \u2018analysis\u2019, and other tasks.\n",
@@ -38,15 +40,15 @@
                 "1. The raw data from the `Scenario`, after `.solve()` has been called, **only** tells us the `\"ACT\"` variable has certain values.\n",
                 "2. To get the 9 GWa figure, we must:\n",
                 "   1. Compute the product of activity (`\"ACT\"`, which is dimensionless) and output efficiency (`\"output\"` in GWa/year), then\n",
                 "   2. Sum across the `\"technology\"` dimension, and finally\n",
                 "   3. Select the single value for the `\"year\"` 720.\n",
                 "   \n",
                 "In this example, steps A, B, and C under #2 are part of \u2018reporting\u2019.\n",
-                "Even a intuitive concept like \u201ctotal secondary energy\u201d is not a *direct* output of the model, but must be reported.\n",
+                "Even an intuitive concept like \u201ctotal secondary energy\u201d is not a *direct* output of the model, but must be reported.\n",
                 "\n",
                 "Next, we may want to create a plot of electricity output by year.\n",
                 "Some modelers consider this part of \u2018reporting\u2019; for others, \u2018reporting\u2019 is complete when the values needed for the plot are written to a file, which they can then use with their favourite plotting tool."
             ]
         },
         {
             "cell_type": "markdown",
@@ -270,14 +272,15 @@
                 "# Replace \"C\" with a reference to sum_calc (instead of an anonymous function)\n",
                 "rep.add(\"C\", (sum_calc, \"A\", \"B\"))\n",
                 "\n",
                 "# Add your code here:"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Concepts: Quantities, Keys, and data formats\n",
                 "\n",
                 "In the last section, $A$, $B$, and so on were *scalar* variables with a single value.\n",
                 "In energy systems modeling, including with MESSAGE*ix*, we usually deal with scientific **quantities** that are sparse, multi-dimensional arrays with associated units.\n",
@@ -290,16 +293,16 @@
                 "Mathematically, we can say the following:\n",
                 "\n",
                 "$$\n",
                 "\\begin{align}\n",
                 "A^{ij} & = \\left[a_{i,j} \\right] \\\\\n",
                 "i & \\in I \\\\\n",
                 "j & \\in J \\\\\n",
-                "a_{i,j} & \\in \\left\\{ \\mathbb{R}, \\text{NaN} \\right\\} \\\\\n",
-                "a_{i,j} & [=]\\, \\text{units of X}\n",
+                "a_{i,j} & \\in \\left\\{ \\mathbb{R}, \\mathrm{NaN} \\right\\} \\\\\n",
+                "a_{i,j} & [=]\\, \\mathrm{units\\ of\\ X}\n",
                 "\\end{align}\n",
                 "$$\n",
                 "\u2026where \u2018NaN\u2019 means \u201cnot a number,\u201d i.e. a missing value.\n",
                 "\n",
                 "(Note: The ``westeros_baseline.ipynb`` distinguishes fixed *parameters*, also called \u201cinput data\u201d, from the decision *variables* that the optimization algorithm changes to find the model solution, or \u201coutput data\u201d.\n",
                 "While reporting the solution is finished and this distinction is not important; so we refer to everything as a *quantity*.)"
             ]
@@ -309,32 +312,32 @@
             "metadata": {},
             "source": [
                 "### Dimensionality of quantities\n",
                 "\n",
                 "Some of the quantities in the MESSAGE mathematical formulation have many dimensions.\n",
                 "For some calculations, we may not care about some of these dimensions.\n",
                 "\n",
-                "For instance, $\\text{output}$ has ten dimensions: $\\text{output}^{n^Lty^Vymnclh^Ah}$.\n",
+                "For instance, $\\mathrm{output}$ has ten dimensions: $\\mathrm{output}^{n^Lty^Vymnclh^Ah}$.\n",
                 "But we may be interested in the total output in a given period ($y$), but not concerned about different vintages of a technology ($y^V$).\n",
                 "In this case, we don't really want the 10-dimensional quantity\u2014but its **partial sum** over all values of $y^V$.\n",
                 "\n",
                 "**Notation.**\n",
                 "Consider a quantity with three dimensions, $A^{ijk}$, and another with two, $B^{kl}$, and a scalar $C$.\n",
                 "We define partial sums over every possible combination of dimensions:\n",
                 "\n",
                 "$$\n",
                 "\\begin{align}\n",
                 "A^{ij} = \\left[ a_{i,j} \\right],\n",
                 "  & a_{i,j} = \\sum_{k}{a_{i,j,k}} \\ \\forall \\ i, j\n",
-                "  & \\text{similarly } A^{ik}, A^{jk} \\\\\n",
+                "  & \\mathrm{similarly } A^{ik}, A^{jk} \\\\\n",
                 "A^{i} = \\left[ a_i \\right],\n",
                 "  & a_i = \\sum_j\\sum_{k}{a_{i,j,k}} \\ \\forall\\  i\n",
-                "  & \\text{similarly } A^j, A^k \\\\\n",
+                "  & \\mathrm{similarly } A^j, A^k \\\\\n",
                 "& \\qquad A = \\sum_i\\sum_j\\sum_k{a_{i,j,k}}\n",
-                "  & \\text{(a scalar)}\n",
+                "  & \\mathrm{(a scalar)}\n",
                 "\\end{align}\n",
                 "$$\n",
                 "\n",
                 "Note that $A$ and $B$ share one dimension, $k$, but the other dimensions are distinct.\n",
                 "We specify that simple arithmetic operations result in a quantity whose dimensions are the union of the dimensions of the operands. In other words:\n",
                 "\n",
                 "$$\n",
@@ -550,16 +553,16 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### More automated contents\n",
                 "\n",
                 "As mentioned, because `Reporter.from_scenario()` knows that `scen` follows the MESSAGE mathematical formulation, it can automatically populate the graph with useful derived quantities.\n",
                 "\n",
-                "For example: the $\\text{ACT}$ for various technologies $t$ is a dimensionless quantity.\n",
-                "The specific commodities produced by $t$, with units, are given by the product $\\text{ACT} \\times \\text{output}$.\n",
+                "For example: the $\\mathrm{ACT}$ for various technologies $t$ is a dimensionless quantity.\n",
+                "The specific commodities produced by $t$, with units, are given by the product $\\mathrm{ACT} \\times \\mathrm{output}$.\n",
                 "This product is given the name \"out\" (the documentation contains [the names for all automatic quantities](https://docs.messageix.org/en/latest/reporting.html#message_ix.reporting.Reporter.from_scenario)):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -909,14 +912,16 @@
                 "# Restore the saved value rep1\n",
                 "rep = rep1\n",
                 "\n",
                 "rep.add(\"D\", 12)\n",
                 "rep.add(\"foo1\", (ratio, \"A\", \"C\"))\n",
                 "rep.add(\"foo2\", (product, \"D\", \"foo1\"))\n",
                 "rep.add(\"E\", (sum_calc, \"A\", \"foo2\"))\n",
+                "print(rep.describe(\"E\"))\n",
+                "\n",
                 "rep.get(\"E\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -927,33 +932,49 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "rep.add(\"D\", 12)\n",
                 "rep.add(\"E\", (lambda a, c, d: a + d * (a / c), \"A\", \"C\", \"D\"))\n",
+                "print(rep.describe(\"E\"))\n",
+                "\n",
                 "rep.get(\"E\")"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "mp.close_db()"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "message_ix",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "29605b568787f5559ca1ba05da75d155c3dcfa15a1a63b1885b057c5465ade2e"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_share_constraint.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_share_constraint.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920524691358025%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'This is a very useful feature for policy analysis. For "*

 * *            'example, in many of the nationally determined contributions (NDCs) as part of the '*

 * *            'Paris Agreement, numerous countries formulated part of their targets in terms of '*

 * *            '*shares*. The European Union, for example, has comitted to a target where renewables '*

 * *            'will make up 30% of the energy mix by 2030. How to implement such a policy in an '*

 * *            "energy mod […]*

```diff
@@ -1,22 +1,23 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Westeros Tutorial - Introducing share constraints\n",
                 "\n",
                 "In this tutorial, we show how to add *share constraints* to a MESSAGEix scenario. The share constraints are aimed at limiting the activity of a single or set of technologies to a certain share of the activity of another single or set of technologies.\n",
                 "\n",
-                "This is a very useful feature for policy analysis. For example, in many of the nationaly determined contributions (NDCs) as part of the Paris Agreement, numerous countries formulated part of their targets in terms of *shares*. The European Union, for example, has comitted to a target, where renewables will make up 30% of the energy mix by 2030. How to implement such a policy in an energy model will be the focus of this tutorial.\n",
+                "This is a very useful feature for policy analysis. For example, in many of the nationally determined contributions (NDCs) as part of the Paris Agreement, numerous countries formulated part of their targets in terms of *shares*. The European Union, for example, has comitted to a target where renewables will make up 30% of the energy mix by 2030. How to implement such a policy in an energy model will be the focus of this tutorial.\n",
                 "\n",
                 "**Pre-requisites**\n",
-                "- You have the *MESSAGEix* framework installed and working.\n",
-                "- You have run Westeros baseline scenario (``westeros_baseline.ipynb``) and solved it successfully."
+                "- You have the *MESSAGEix* framework installed and working\n",
+                "- You have run Westeros baseline scenario (``westeros_baseline.ipynb``) and solved it successfully"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Adding a minimum share constraint\n",
@@ -92,22 +93,23 @@
                 "year_df = scen.vintage_and_active_years()\n",
                 "vintage_years, act_years = year_df[\"year_vtg\"], year_df[\"year_act\"]\n",
                 "model_horizon = scen.set(\"year\")\n",
                 "country = \"Westeros\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Steps required to add share constraints\n",
                 "The following steps are required in order to introduce a share constraint:\n",
                 "1. Define a new 'share' and add this to the *set* `\"shares\"`\n",
                 "2. Define which technologies contribute towards the total\n",
-                "3. Define which technologies contribute towards fullfilling the share\n",
+                "3. Define which technologies contribute towards fulfilling the share\n",
                 "4. Define the share for relevant periods\n",
                 "\n",
                 "The implementation of shares in MESSAGEix is generic and flexible, so that any combination of commodities, levels, technologies and nodes can be put in relation to any other combination."
             ]
         },
         {
             "cell_type": "markdown",
@@ -124,21 +126,22 @@
             "outputs": [],
             "source": [
                 "shares = \"share_renewable_electricity\"\n",
                 "scen.add_set(\"shares\", shares)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 2. Defining technologies that make up the total\n",
-                "We need to define which technologies make up the group accounting for the total, to which the share applies. To do this, we need to map the share to relevant *commodity* and *level*.\n",
+                "We need to define which technologies make up the group accounting for the total, to which the share applies. To do this, we need to map the share to the relevant *commodity* and *level*.\n",
                 "\n",
-                "The aim is to increase the share of electricity generated from renewables to 50% in 720. Therefore, we need to define, which technologies contribute to total electricity generation at the secondary energy level. In our example, these are `\"wind_ppl\"` and `\"coal_ppl\"` technologies, which will be grouped as a new `type_tec`, called `\"electricity_total\"` in the scenario. For this `type_tec`, we need to define the relevant node, mode, level and commodity through the *set* `\"map_shares_commodity_total\"`."
+                "The aim is to increase the share of electricity generated from renewables to 50% in 720. Therefore, we need to define which technologies contribute to total electricity generation at the secondary energy level. In our example, these are `\"wind_ppl\"` and `\"coal_ppl\"` technologies, which will be grouped as a new `type_tec`, called `\"electricity_total\"` in the scenario. For this `type_tec`, we need to define the relevant node, mode, level and commodity through the *set* `\"map_shares_commodity_total\"`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -183,19 +186,20 @@
                 "        \"level\": \"secondary\",\n",
                 "    }\n",
                 ")\n",
                 "scen.add_set(\"map_shares_commodity_total\", df)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 3. Defining technologies of share\n",
-                "Next, we define technologies that contribute towards fullfilling the share. We also need to set corresponding commodity and level for which the share constraint applies. In our example, the technology that provides 50% electricity from renewable energy is `\"wind_ppl\"`."
+                "Next, we define technologies that contribute towards fulfilling the share. We also need to set the corresponding commodity and level for which the share constraint applies. In our example, the technology that provides 50% electricity from renewable energy is `\"wind_ppl\"`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -215,19 +219,20 @@
                 "        \"level\": \"secondary\",\n",
                 "    }\n",
                 ")\n",
                 "scen.add_set(\"map_shares_commodity_share\", df)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 4. Defining the share\n",
-                "Lastly, the actual share value needs to be added to the model. To represent a minimum share of 50% of total electricity generation from renewables, we use parameter `\"share_commodity_lo\"`. If this constraint should act as an upper bound, then parameter `\"share_commodity_up\"` can be used."
+                "Lastly, the actual share value needs to be added to the model. To represent a minimum share of 50% of total electricity generation from renewables, we use the parameter `\"share_commodity_lo\"`. If this constraint should act as an upper bound, then the parameter `\"share_commodity_up\"` can be used."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -313,23 +318,24 @@
                 "\n",
                 "# Scenario with share constraint\n",
                 "rep = Reporter.from_scenario(scen)\n",
                 "prepare_plots(rep)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Activity\n",
                 "***\n",
-                "In the new scenario ('*share_constraint*'), the activity of `\"wind_ppl\"` accounts for 50% of total electricity generation in 720. This was the share constraint, we added to the scenario.\n",
+                "In the new scenario ('*share_constraint*'), the activity of `\"wind_ppl\"` accounts for 50% of total electricity generation in 720. This was the share constraint we added to the scenario.\n",
                 "\n",
                 "### Question:\n",
-                "The results show that the activity of `\"wind_ppl\"` in 710 is higher than the '*baseline*'. Do you know why this happens?"
+                "The results show that the activity of `\"wind_ppl\"` in 710 is higher than in the '*baseline*' scenario. Do you know why this happens?"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Scenario: '*baseline*'"
@@ -360,28 +366,30 @@
             "outputs": [],
             "source": [
                 "rep.set_filters(t=plants)\n",
                 "rep.get(\"plot activity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Response to the question: \n",
-                "This is because `\"wind_ppl\"` has a diffusion constraint in this scenario, limiting the activity growth rate by 10% per year. Thus, to achieve the 50% target in 720 specified by the share constraint, additional activity is required in the previous periods to ramp up the wind generation."
+                "This is because `\"wind_ppl\"` has a diffusion constraint in this scenario, limiting the activity growth rate to 10% per year. Thus, to achieve the 50% target in 720 specified by the share constraint, additional activity is required in the previous periods to ramp up the wind generation."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Capacity\n",
                 "***\n",
-                "There is big increase in 720 regarding activity which is reflected in the capacity for the two technologies."
+                "There is a big increase in 720 regarding activity which is reflected in the capacity for the two technologies."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Scenario: '*baseline*'"
@@ -409,20 +417,21 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "rep.get(\"plot capacity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Prices\n",
                 "***\n",
-                "As expected, electricity prices in 720 have also increased vis-a-vis the '*baseline*'"
+                "As expected, electricity prices in 720 have also increased vis-a-vis the '*baseline*'."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Scenario: '*baseline*'"
```

### Comparing `message_ix-3.6.0/tutorial/westeros/westeros_soft_constraints.ipynb` & `message_ix-3.7.0/tutorial/westeros/westeros_soft_constraints.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9856001420454545%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'In this tutorial, we are going to explore how to "*

 * *            'provide additional flexibility to the dynamic growth constraints. We will explore '*

 * *            'so-called [`soft '*

 * *            'constraints`](https://docs.messageix.org/en/stable/model/MESSAGE/parameter_def.html?highlight=soft%20constraint#dynamic-constraints-on-new-capacity-and-activity). '*

 * *            'Soft constraints can be configured to provide a relaxation for both activity and '*

 * *            'ca […]*

```diff
@@ -1,22 +1,23 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Westeros Tutorial - Introducing soft constraints\n",
                 "\n",
                 "In the baseline tutorial, we added dynamic constraints on activity via the parameter `\"growth_activity_up\"` for the electricity generation technologies. As a result, when we added an emission tax, `\"wind_ppl\"` was scaled up at the maximum rate of 10% annually in the last period.\n",
                 "\n",
-                "In this tutorial, we are going to explore how to provide additional flexibility to the dynamic growth constraints. We will explore so called [`soft constraints`](https://docs.messageix.org/en/stable/model/MESSAGE/parameter_def.html?highlight=soft%20constraint#dynamic-constraints-on-new-capacity-and-activity). Soft constraints can be configured to provide a relaxation for both activity and capacity related dynamic constraints. At a certain cost, additional annual growth rate can be realized. The cost can be absolute or defined as a share of the levelized cost (see details [here](https://docs.messageix.org/en/stable/model/MESSAGE/parameter_def.html?highlight=soft%20constraint#cost-parameters-for-soft-relaxations-of-dynamic-constraints)).\n",
+                "In this tutorial, we are going to explore how to provide additional flexibility to the dynamic growth constraints. We will explore so-called [`soft constraints`](https://docs.messageix.org/en/stable/model/MESSAGE/parameter_def.html?highlight=soft%20constraint#dynamic-constraints-on-new-capacity-and-activity). Soft constraints can be configured to provide a relaxation for both activity and capacity related dynamic constraints. At a certain cost, additional annual growth rate can be realized. The cost can be absolute or defined as a share of the levelized cost (see details [here](https://docs.messageix.org/en/stable/model/MESSAGE/parameter_def.html?highlight=soft%20constraint#cost-parameters-for-soft-relaxations-of-dynamic-constraints)).\n",
                 "\n",
-                "Providing this additional flexibility to dynamic constraints can be useful for assessing mitigation pathways. While without these for example, certain emission targets may not be achievable, the additional flexibility provided reflects the fact that investments i.e. technology diffusion, can be realized faster taking into account higher costs. This can provide interesting insights as to where additional subsidies or policies can help pursue more ambitious targets.\n",
+                "Providing this additional flexibility to dynamic constraints can be useful for assessing mitigation pathways. While without these e.g. certain emission targets may not be achievable, the additional flexibility provided reflects the fact that investments i.e. technology diffusion, can be realized faster taking into account higher costs. This can provide interesting insights as to where additional subsidies or policies can help pursue more ambitious targets.\n",
                 "\n",
-                "Further information can be found in https://doi.org/10.1016/j.energy.2010.01.019 (*Kepp and Strubegger, 2010*)\n",
+                "Further information can be found in [Kepp and Strubegger, 2010](https://doi.org/10.1016/j.energy.2010.01.019). \n",
                 "\n",
                 "**Pre-requisites**\n",
                 "- You have the *MESSAGEix* framework installed and working\n",
                 "- You have run Westeros tutorial on emission taxes (`westeros_emissions_taxes.ipynb`) and solved it successfully"
             ]
         },
         {
@@ -60,40 +61,42 @@
                 "scen = base.clone(\n",
                 "    model, \"carbon_tax_soft_constraints\", \"adding_soft_constraints\", keep_solution=False\n",
                 ")\n",
                 "scen.check_out()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Retrieve parameters\n",
-                "We will retrieve those parameters necessary to perform subsequent additions of parameters"
+                "We will retrieve those parameters necessary to perform subsequent additions of parameters."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "model_horizon = base.set(\"year\")\n",
                 "country = \"Westeros\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Add soft activity up for `\"wind_ppl\"`\n",
                 "\n",
                 "Recall that when setting up the Westeros baseline scenario, we added the parameter `\"growth_activity_up\"` for `\"wind_ppl\"`, with a value of 10%. As the growth rate is an annual value and the duration of the periods in this example are 10 years, activity within a single period can increase by a maximum of 259% ((1 + .10)^10).\n",
                 "\n",
-                "We will now add a soft constraint for the year 720, allowing additional growth of up 1% per year. This means that activity can increase by a maximum of 259% + 10% (((1 + .01)^10) - 1). The costs will be defined in relative terms i.e. relative to the [levelized cost](https://docs.messageix.org/en/stable/model/MESSAGE/scaling_investment_costs.html?highlight=levelized%20cost#levelized-capital-costs). By specifying the `\"level_cost_activity_soft_up\"` as 1%, we are defining that per unit of activity from the previous period, used to determine the allowable additional activity, 1% of the `levelized_cost` are applied (see [link](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html#objective-function) for more information)."
+                "We will now add a soft constraint for the year 720, allowing additional growth of up to 1% per year. This means that activity can increase by a maximum of 259% + 10% (((1 + .01)^10) - 1). The costs will be defined in relative terms i.e. relative to the [levelized cost](https://docs.messageix.org/en/stable/model/MESSAGE/scaling_investment_costs.html?highlight=levelized%20cost#levelized-capital-costs). By specifying the `\"level_cost_activity_soft_up\"` as 1%, we are defining that per unit of activity from the previous period, used to determine the allowable additional activity, 1% of the `levelized_cost` are applied (see [link](https://docs.messageix.org/en/stable/model/MESSAGE/model_core.html#objective-function) for more information)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Define additional annual growth.\n",
@@ -184,20 +187,21 @@
                 "prepare_plots(rep_base)\n",
                 "\n",
                 "rep_scen = Reporter.from_scenario(scen)\n",
                 "prepare_plots(rep_scen)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Activity\n",
                 "***\n",
-                "When comparing the results of the scenario '*tax_carbon*', `\"coal_ppl\"` still contributed to the eletricity generation mix in 710."
+                "When comparing the results of the scenario '*carbon_tax*', `\"coal_ppl\"` still contributed to the eletricity generation mix in 710."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -220,22 +224,32 @@
             "outputs": [],
             "source": [
                 "rep_scen.set_filters(t=[\"coal_ppl\", \"wind_ppl\"])\n",
                 "rep_scen.get(\"plot activity\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In the figure below the dark-blue bars represent the maximum activity for each period. This is calculated based on the activity of the preceding period and accounting for the annual growth of 10% (`\"growth_activity_up\"`). The orange bar shows that additional activity based on the soft constraint added for `\"wind_ppl\"` in 720.\n",
-                "The lines compare the results (`var(\"ACT\")`) for `\"wind_ppl\"` of the carbon tax scenario without (gold  line) and with soft constraints (grey line). In the scenario with soft constraints, you can see that already in 710 `\"wind_ppl\"` has increased activity, so that the full use can be made of the relaxation provided by the soft constraints in 720.\n",
+                "The lines compare the results (`var(\"ACT\")`) for `\"wind_ppl\"` of the carbon tax scenario without (gold  line) and with soft constraints (grey line). In the scenario with soft constraints, you can see that already in 710 `\"wind_ppl\"` has increased activity, so that full use can be made of the relaxation provided by the soft constraints in 720.\n",
                 "\n",
                 "<img src='_static/soft-constraint.PNG' width='600'>"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "mp.close_db()"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

