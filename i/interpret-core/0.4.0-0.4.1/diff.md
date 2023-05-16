# Comparing `tmp/interpret-core-0.4.0.tar.gz` & `tmp/interpret-core-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpret-core-0.4.0.tar", last modified: Thu May 11 12:05:49 2023, max compression
+gzip compressed data, was "interpret-core-0.4.1.tar", last modified: Tue May 16 23:05:36 2023, max compression
```

## Comparing `interpret-core-0.4.0.tar` & `interpret-core-0.4.1.tar`

### file list

```diff
@@ -1,343 +1,343 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.804068 interpret-core-0.4.0/
--rw-r--r--   0 vsts      (1001) docker     (122)      275 2023-05-11 12:00:39.000000 interpret-core-0.4.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1234 2023-05-11 12:05:49.804068 interpret-core-0.4.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.740069 interpret-core-0.4.0/interpret/
--rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.740069 interpret-core-0.4.0/interpret/api/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2543 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/api/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6294 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/api/templates.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.740069 interpret-core-0.4.0/interpret/blackbox/
--rw-r--r--   0 vsts      (1001) docker     (122)      381 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/blackbox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6145 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/blackbox/_lime.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8611 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/blackbox/_partialdependence.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10275 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/blackbox/_permutationimportance.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10783 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/blackbox/_sensitivity.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/blackbox/_shap.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.744069 interpret-core-0.4.0/interpret/data/
--rw-r--r--   0 vsts      (1001) docker     (122)      158 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15905 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/data/_response.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6307 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/develop.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.744069 interpret-core-0.4.0/interpret/ext/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/ext/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.744069 interpret-core-0.4.0/interpret/ext/blackbox/
--rw-r--r--   0 vsts      (1001) docker     (122)      366 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/ext/blackbox/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.744069 interpret-core-0.4.0/interpret/ext/data/
--rw-r--r--   0 vsts      (1001) docker     (122)      350 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/ext/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2037 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/ext/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3314 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/ext/extension.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2955 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/ext/extension_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.744069 interpret-core-0.4.0/interpret/ext/glassbox/
--rw-r--r--   0 vsts      (1001) docker     (122)      366 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/ext/glassbox/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.744069 interpret-core-0.4.0/interpret/ext/greybox/
--rw-r--r--   0 vsts      (1001) docker     (122)      362 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/ext/greybox/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.744069 interpret-core-0.4.0/interpret/ext/perf/
--rw-r--r--   0 vsts      (1001) docker     (122)      350 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/ext/perf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.744069 interpret-core-0.4.0/interpret/ext/provider/
--rw-r--r--   0 vsts      (1001) docker     (122)      340 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/ext/provider/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.744069 interpret-core-0.4.0/interpret/glassbox/
--rw-r--r--   0 vsts      (1001) docker     (122)      500 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20235 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_decisiontree.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.748069 interpret-core-0.4.0/interpret/glassbox/_ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9550 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/_bin.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6500 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/_boost.py
--rw-r--r--   0 vsts      (1001) docker     (122)   139470 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/_ebm.py
--rw-r--r--   0 vsts      (1001) docker     (122)    33662 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/_merge_ebms.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4461 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/_multiclass.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.748069 interpret-core-0.4.0/interpret/glassbox/_ebm/_research/
--rw-r--r--   0 vsts      (1001) docker     (122)      537 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/_research/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10237 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/_research/_group_importance.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4136 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/_research/_purify.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5423 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/_tensor.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17903 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_ebm/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17093 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_linear.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14262 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/glassbox/_skoperules.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.748069 interpret-core-0.4.0/interpret/greybox/
--rw-r--r--   0 vsts      (1001) docker     (122)      202 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/greybox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2765 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/greybox/_shaptree.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5420 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/greybox/_treeinterpreter.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.752069 interpret-core-0.4.0/interpret/lib/
--rw-r--r--   0 vsts      (1001) docker     (122)  4179553 2023-05-11 12:05:49.000000 interpret-core-0.4.0/interpret/lib/interpret-inline.js
--rw-r--r--   0 vsts      (1001) docker     (122)     2580 2023-05-11 12:05:49.000000 interpret-core-0.4.0/interpret/lib/interpret-inline.js.LICENSE.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.752069 interpret-core-0.4.0/interpret/perf/
--rw-r--r--   0 vsts      (1001) docker     (122)      192 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/perf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10362 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/perf/_curve.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5223 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/perf/_regression.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.756069 interpret-core-0.4.0/interpret/privacy/
--rw-r--r--   0 vsts      (1001) docker     (122)      269 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/privacy/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.756069 interpret-core-0.4.0/interpret/provider/
--rw-r--r--   0 vsts      (1001) docker     (122)      316 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      777 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/provider/_compute.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4704 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/provider/_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8375 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/provider/_visualize.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.760069 interpret-core-0.4.0/interpret/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)     2900 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_SPOTgreedy.py
--rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14758 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_clean_simple.py
--rw-r--r--   0 vsts      (1001) docker     (122)    82828 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_clean_x.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4613 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_compressed_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6217 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_explanation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2369 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_histogram.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1412 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_link.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9852 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_measure_interactions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    62132 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_native.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23690 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_preprocessor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5556 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_privacy.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1623 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_rank_interactions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2611 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_seed.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3790 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_shap_common.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3274 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_unify_data.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5003 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/utils/_unify_predict.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.760069 interpret-core-0.4.0/interpret/visual/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/visual/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7884 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/visual/_inline.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7582 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/visual/_interactive.py
--rw-r--r--   0 vsts      (1001) docker     (122)    32140 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/visual/_udash.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.760069 interpret-core-0.4.0/interpret/visual/assets/
--rw-r--r--   0 vsts      (1001) docker     (122)    15406 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/visual/assets/favicon.ico
--rw-r--r--   0 vsts      (1001) docker     (122)    15857 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/visual/assets/udash.css
--rw-r--r--   0 vsts      (1001) docker     (122)      599 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/visual/assets/udash.js
--rw-r--r--   0 vsts      (1001) docker     (122)    13340 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/visual/dashboard.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26837 2023-05-11 12:00:39.000000 interpret-core-0.4.0/interpret/visual/plot.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.760069 interpret-core-0.4.0/interpret_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1234 2023-05-11 12:05:49.000000 interpret-core-0.4.0/interpret_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    11667 2023-05-11 12:05:49.000000 interpret-core-0.4.0/interpret_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-11 12:05:49.000000 interpret-core-0.4.0/interpret_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-05-11 12:05:49.000000 interpret-core-0.4.0/interpret_core.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      717 2023-05-11 12:05:49.000000 interpret-core-0.4.0/interpret_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       10 2023-05-11 12:05:49.000000 interpret-core-0.4.0/interpret_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-05-11 12:05:49.804068 interpret-core-0.4.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     8880 2023-05-11 12:00:39.000000 interpret-core-0.4.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.764069 interpret-core-0.4.0/symbolic/
--rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-05-11 12:00:47.000000 interpret-core-0.4.0/symbolic/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)    33984 2023-05-11 12:00:47.000000 interpret-core-0.4.0/symbolic/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1565 2023-05-11 12:00:47.000000 interpret-core-0.4.0/symbolic/build.bat
--rw-r--r--   0 vsts      (1001) docker     (122)    40976 2023-05-11 12:00:47.000000 interpret-core-0.4.0/symbolic/build.sh
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.736069 interpret-core-0.4.0/symbolic/shared/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.776069 interpret-core-0.4.0/symbolic/shared/libebm/
--rw-r--r--   0 vsts      (1001) docker     (122)    25251 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/ApplyTermUpdate.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    10588 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/BinSumsBoosting.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    15618 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/BinSumsInteraction.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    30951 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/BoosterCore.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     7155 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/BoosterCore.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    19842 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/BoosterShell.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     5691 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/BoosterShell.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     8866 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/CODING_STYLE.md
--rw-r--r--   0 vsts      (1001) docker     (122)    18718 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/CalcInteractionStrength.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)   179547 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/CutQuantile.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    32876 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/CutUniform.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    20952 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/CutWinsorized.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    27679 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/DataSetBoosting.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3161 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/DataSetBoosting.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    14081 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/DataSetInteraction.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3075 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/DataSetInteraction.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/DetermineLinkFunction.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    60544 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/Discretize.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4162 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/Feature.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    19457 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/GaussianDistribution.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    42347 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/GenerateTermUpdate.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    17492 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/IMPORTANT.md
--rw-r--r--   0 vsts      (1001) docker     (122)     4536 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/InitializeGradientsAndHessians.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    10200 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/InnerBag.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2783 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/InnerBag.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    20298 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/InteractionCore.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4133 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/InteractionCore.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     9050 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/InteractionShell.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4230 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/InteractionShell.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    35081 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/PartitionOneDimensionalBoosting.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    32143 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/PartitionRandomBoosting.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    42726 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/PartitionTwoDimensionalBoosting.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    25557 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/PartitionTwoDimensionalInteraction.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     7387 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/RandomDeterministic.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    11402 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/RandomDeterministic.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4656 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/RandomNondeterministic.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4417 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/SplitPosition.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    36064 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/Tensor.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    13659 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/Tensor.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    46171 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/TensorTotalsBuild.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    18160 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/TensorTotalsSum.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     1843 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/Term.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4546 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/Term.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4849 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/Transpose.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    10239 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/TreeNode.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.776069 interpret-core-0.4.0/symbolic/shared/libebm/bridge_c/
--rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/bridge_c/bridge_c.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1371 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/bridge_c/zones.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.776069 interpret-core-0.4.0/symbolic/shared/libebm/bridge_cpp/
--rw-r--r--   0 vsts      (1001) docker     (122)    13743 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/bridge_cpp/Bin.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     8442 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/bridge_cpp/GradientPair.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     7926 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/bridge_cpp/bridge_cpp.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.780068 interpret-core-0.4.0/symbolic/shared/libebm/common_c/
--rw-r--r--   0 vsts      (1001) docker     (122)     3037 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/common_c/common_c.c
--rw-r--r--   0 vsts      (1001) docker     (122)     8476 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/common_c/common_c.h
--rw-r--r--   0 vsts      (1001) docker     (122)     6580 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/common_c/logging.c
--rw-r--r--   0 vsts      (1001) docker     (122)    10001 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/common_c/logging.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.780068 interpret-core-0.4.0/symbolic/shared/libebm/common_cpp/
--rw-r--r--   0 vsts      (1001) docker     (122)    45433 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/common_cpp/common_cpp.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.780068 interpret-core-0.4.0/symbolic/shared/libebm/compute/
--rw-r--r--   0 vsts      (1001) docker     (122)      553 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/Directory.Build.targets
--rw-r--r--   0 vsts      (1001) docker     (122)     6427 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/Objective.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    35874 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/Objective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     6723 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/Registration.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    13194 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/Registration.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    50721 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/approximate_math.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.780068 interpret-core-0.4.0/symbolic/shared/libebm/compute/avx512_ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)      257 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/avx512_ebm/avx512_32.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    13706 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)      477 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj.filters
--rw-r--r--   0 vsts      (1001) docker     (122)     4386 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/compute.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    61597 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/compute_stats.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.784069 interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)      254 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/cpu_32.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     7447 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/cpu_64.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    13427 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)      593 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj.filters
--rw-r--r--   0 vsts      (1001) docker     (122)     8950 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/sse2_32.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/sse2_64.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.784069 interpret-core-0.4.0/symbolic/shared/libebm/compute/cuda_ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)    11435 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/cuda_ebm/cuda_32.cu
--rw-r--r--   0 vsts      (1001) docker     (122)    14658 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)      505 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj.filters
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.784069 interpret-core-0.4.0/symbolic/shared/libebm/compute/metrics/
--rw-r--r--   0 vsts      (1001) docker     (122)      177 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/metrics/AucMetric.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.784069 interpret-core-0.4.0/symbolic/shared/libebm/compute/no_cuda_ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)      630 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_32.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    13332 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)      478 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj.filters
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.788069 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/
--rw-r--r--   0 vsts      (1001) docker     (122)      432 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/CrossEntropyBinaryObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3630 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassMultitaskObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4464 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/ExampleRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3033 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/GammaDevianceRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)      770 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/LogLossBinaryMultitaskObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     7535 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/LogLossBinaryObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     9437 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/LogLossMulticlassObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4596 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/PoissonDevianceRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4226 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/PseudoHuberRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3409 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/RmseLogLinkRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/RmseRegressionMultitaskObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     9116 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/RmseRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4842 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/TweedieDevianceRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3245 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/objective_registrations.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)      267 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/precompiled_header_cpp.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2301 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/registration_exceptions.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.788069 interpret-core-0.4.0/symbolic/shared/libebm/compute/special/
--rw-r--r--   0 vsts      (1001) docker     (122)      164 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/special/precompiled_header_cpp.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2366 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/zoned_bridge_c_functions.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     1068 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/zoned_bridge_c_functions.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1458 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute/zoned_bridge_cpp_functions.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2800 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/compute_accessors.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    99936 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/dataset_shared.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2242 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/dataset_shared.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    20943 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/debug_ebm.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     8264 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/ebm_internal.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    41443 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/ebm_stats.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.788069 interpret-core-0.4.0/symbolic/shared/libebm/inc/
--rw-r--r--   0 vsts      (1001) docker     (122)    20299 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/inc/libebm.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3650 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/include_ordering.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    13026 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/interpret.sln
--rw-r--r--   0 vsts      (1001) docker     (122)    77375 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/interpretable_numerics.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    24095 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/libebm.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)     5242 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/libebm.vcxproj.filters
--rw-r--r--   0 vsts      (1001) docker     (122)      975 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/libebm_exports.def
--rw-r--r--   0 vsts      (1001) docker     (122)     1233 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/libebm_exports.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/precompiled_header_cpp.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     6007 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/random.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    26424 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/sampling.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.788069 interpret-core-0.4.0/symbolic/shared/libebm/special/
--rw-r--r--   0 vsts      (1001) docker     (122)     2874 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/special/linux_wrap_functions.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      164 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/special/precompiled_header_cpp.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      790 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/special/windows_DllMain.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.792069 interpret-core-0.4.0/symbolic/shared/libebm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)    46248 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/CutQuantileTest.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    12964 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/CutUniformTest.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    24882 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/CutWinsorizedTest.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/DiscretizeTest.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     6935 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/RandomStreamTest.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    11983 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/SuggestGraphBoundsTest.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     6762 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/bit_packing_extremes.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    67788 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/boosting_unusual_inputs.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    17110 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/dataset_shared_test.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2740 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/include_c.c
--rw-r--r--   0 vsts      (1001) docker     (122)    15736 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/interaction_unusual_inputs.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     1931 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.bat
--rw-r--r--   0 vsts      (1001) docker     (122)    41550 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    14659 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    38501 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.sh
--rw-r--r--   0 vsts      (1001) docker     (122)    15718 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)     1636 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.vcxproj.filters
--rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/precompiled_header_test.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      298 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/precompiled_header_test.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    12854 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/random_test.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4839 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/tests/rehydrate_booster.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      564 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/libebm/vs_python_setup.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.796069 interpret-core-0.4.0/symbolic/shared/vis/
--rw-r--r--   0 vsts      (1001) docker     (122)      171 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/vis/.babelrc
--rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/vis/.eslintrc.json
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/vis/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (122)      238 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/vis/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1472 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/vis/package.json
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.796069 interpret-core-0.4.0/symbolic/shared/vis/src/
--rw-r--r--   0 vsts      (1001) docker     (122)     4433 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/vis/src/index.js
--rw-r--r--   0 vsts      (1001) docker     (122)     1469 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/vis/src/styles.scss
--rw-r--r--   0 vsts      (1001) docker     (122)      757 2023-05-11 12:00:39.000000 interpret-core-0.4.0/symbolic/shared/vis/webpack.config.js
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.796069 interpret-core-0.4.0/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.796069 interpret-core-0.4.0/tests/api/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1895 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/api/test_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.796069 interpret-core-0.4.0/tests/blackbox/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/blackbox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1435 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/blackbox/test_permutationimportance.py
--rw-r--r--   0 vsts      (1001) docker     (122)      477 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/blackbox/test_sensitivity.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.796069 interpret-core-0.4.0/tests/ext/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/ext/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2502 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/ext/test_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.800068 interpret-core-0.4.0/tests/glassbox/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.800068 interpret-core-0.4.0/tests/glassbox/ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/ebm/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.800068 interpret-core-0.4.0/tests/glassbox/ebm/research/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/ebm/research/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8067 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/ebm/research/test_group_importance.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8414 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/ebm/research/test_purify.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4105 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/ebm/test_bin.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28189 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/ebm/test_ebm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5551 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/ebm/test_ebm_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5393 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/ebm/test_merge_ebms.py
--rw-r--r--   0 vsts      (1001) docker     (122)      790 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/ebm/test_multiclass.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2055 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/test_decisiontree.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3499 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/glassbox/test_linear.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.800068 interpret-core-0.4.0/tests/greybox/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/greybox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1459 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/greybox/test_treeinterpreter.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.800068 interpret-core-0.4.0/tests/provider/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      470 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/provider/test_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2257 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/provider/test_providers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1505 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/test_develop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/test_example_notebooks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3215 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/test_explainers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2702 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/test_ext.py
--rw-r--r--   0 vsts      (1001) docker     (122)      691 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/test_extension_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1108 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/test_mli_interop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9489 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/test_selenium.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8241 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/tutils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.804068 interpret-core-0.4.0/tests/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1099 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/utils/test_SPOTgreedy.py
--rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/utils/test_clean_simple.py
--rw-r--r--   0 vsts      (1001) docker     (122)   113135 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/utils/test_clean_x.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3041 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/utils/test_compressed_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1453 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/utils/test_explanation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8683 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/utils/test_measure_interactions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2888 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/utils/test_native.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:49.804068 interpret-core-0.4.0/tests/visual/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/visual/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      369 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/visual/test_dashboard.py
--rw-r--r--   0 vsts      (1001) docker     (122)      898 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/visual/test_inline.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5223 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/visual/test_interactive.py
--rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-05-11 12:00:39.000000 interpret-core-0.4.0/tests/visual/test_plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.833345 interpret-core-0.4.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)      275 2023-05-16 23:00:07.000000 interpret-core-0.4.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1234 2023-05-16 23:05:36.833345 interpret-core-0.4.1/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.713344 interpret-core-0.4.1/interpret/
+-rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.713344 interpret-core-0.4.1/interpret/api/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2543 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/api/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6294 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/api/templates.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.717344 interpret-core-0.4.1/interpret/blackbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      381 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6145 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/_lime.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8611 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/_partialdependence.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10275 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/_permutationimportance.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10783 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/_sensitivity.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/_shap.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.721344 interpret-core-0.4.1/interpret/data/
+-rw-r--r--   0 vsts      (1001) docker     (122)      158 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15905 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/data/_response.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6307 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/develop.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.721344 interpret-core-0.4.1/interpret/ext/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.721344 interpret-core-0.4.1/interpret/ext/blackbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      366 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/blackbox/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.721344 interpret-core-0.4.1/interpret/ext/data/
+-rw-r--r--   0 vsts      (1001) docker     (122)      350 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2037 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3314 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/extension.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2955 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/extension_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.725344 interpret-core-0.4.1/interpret/ext/glassbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      366 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/glassbox/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.725344 interpret-core-0.4.1/interpret/ext/greybox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      362 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/greybox/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.725344 interpret-core-0.4.1/interpret/ext/perf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      350 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/perf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.725344 interpret-core-0.4.1/interpret/ext/provider/
+-rw-r--r--   0 vsts      (1001) docker     (122)      340 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/provider/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.725344 interpret-core-0.4.1/interpret/glassbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      500 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20235 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_decisiontree.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.729344 interpret-core-0.4.1/interpret/glassbox/_ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9550 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_bin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6500 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_boost.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   139474 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_ebm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    33662 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_merge_ebms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4461 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_multiclass.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.729344 interpret-core-0.4.1/interpret/glassbox/_ebm/_research/
+-rw-r--r--   0 vsts      (1001) docker     (122)      537 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_research/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10237 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_research/_group_importance.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4136 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_research/_purify.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5423 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_tensor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17903 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17093 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14262 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_skoperules.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.733344 interpret-core-0.4.1/interpret/greybox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      202 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/greybox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2765 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/greybox/_shaptree.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5420 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/greybox/_treeinterpreter.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.737344 interpret-core-0.4.1/interpret/lib/
+-rw-r--r--   0 vsts      (1001) docker     (122)  4182080 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret/lib/interpret-inline.js
+-rw-r--r--   0 vsts      (1001) docker     (122)     2580 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret/lib/interpret-inline.js.LICENSE.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.741344 interpret-core-0.4.1/interpret/perf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      192 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/perf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10362 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/perf/_curve.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5223 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/perf/_regression.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.741344 interpret-core-0.4.1/interpret/privacy/
+-rw-r--r--   0 vsts      (1001) docker     (122)      269 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/privacy/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.741344 interpret-core-0.4.1/interpret/provider/
+-rw-r--r--   0 vsts      (1001) docker     (122)      316 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      777 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/provider/_compute.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4704 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/provider/_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8375 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/provider/_visualize.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.745344 interpret-core-0.4.1/interpret/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2900 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_SPOTgreedy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14758 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_clean_simple.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    82828 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_clean_x.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4613 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_compressed_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6217 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_explanation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2369 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1412 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_link.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9852 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_measure_interactions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    61653 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_native.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23690 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_preprocessor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5556 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_privacy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1623 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_rank_interactions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2611 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_seed.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3790 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_shap_common.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3274 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_unify_data.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5003 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_unify_predict.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.745344 interpret-core-0.4.1/interpret/visual/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8094 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/_inline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7582 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/_interactive.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    32140 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/_udash.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.745344 interpret-core-0.4.1/interpret/visual/assets/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15406 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/assets/favicon.ico
+-rw-r--r--   0 vsts      (1001) docker     (122)    15857 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/assets/udash.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      599 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/assets/udash.js
+-rw-r--r--   0 vsts      (1001) docker     (122)    13340 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/dashboard.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26837 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.753344 interpret-core-0.4.1/interpret_core.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1234 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    11667 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      717 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       10 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-05-16 23:05:36.833345 interpret-core-0.4.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     8880 2023-05-16 23:00:07.000000 interpret-core-0.4.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.753344 interpret-core-0.4.1/symbolic/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-05-16 23:00:15.000000 interpret-core-0.4.1/symbolic/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)    34327 2023-05-16 23:00:15.000000 interpret-core-0.4.1/symbolic/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1565 2023-05-16 23:00:15.000000 interpret-core-0.4.1/symbolic/build.bat
+-rw-r--r--   0 vsts      (1001) docker     (122)    40976 2023-05-16 23:00:15.000000 interpret-core-0.4.1/symbolic/build.sh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.705344 interpret-core-0.4.1/symbolic/shared/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.781345 interpret-core-0.4.1/symbolic/shared/libebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)    25251 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/ApplyTermUpdate.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    10588 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BinSumsBoosting.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    15618 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BinSumsInteraction.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    30951 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BoosterCore.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7155 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BoosterCore.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    19842 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BoosterShell.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5691 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BoosterShell.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8866 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/CODING_STYLE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)    18718 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/CalcInteractionStrength.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)   179547 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/CutQuantile.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    32876 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/CutUniform.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    20952 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/CutWinsorized.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    27635 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/DataSetBoosting.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3161 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/DataSetBoosting.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    14037 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/DataSetInteraction.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3075 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/DataSetInteraction.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5223 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/DetermineLinkFunction.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    60544 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Discretize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4162 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Feature.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    19457 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/GaussianDistribution.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    42347 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/GenerateTermUpdate.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    17492 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/IMPORTANT.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     4536 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InitializeGradientsAndHessians.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    10200 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InnerBag.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2783 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InnerBag.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    20298 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InteractionCore.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4133 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InteractionCore.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9050 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InteractionShell.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4230 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InteractionShell.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    35081 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/PartitionOneDimensionalBoosting.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    32143 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/PartitionRandomBoosting.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    42726 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/PartitionTwoDimensionalBoosting.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    25557 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/PartitionTwoDimensionalInteraction.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7387 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/RandomDeterministic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    11402 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/RandomDeterministic.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4656 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/RandomNondeterministic.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4417 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/SplitPosition.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    36064 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Tensor.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13659 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Tensor.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    46171 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/TensorTotalsBuild.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    18160 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/TensorTotalsSum.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1843 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Term.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4546 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Term.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4849 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Transpose.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    10239 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/TreeNode.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.781345 interpret-core-0.4.1/symbolic/shared/libebm/bridge_c/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/bridge_c/bridge_c.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1371 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/bridge_c/zones.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.781345 interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/
+-rw-r--r--   0 vsts      (1001) docker     (122)    13743 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/Bin.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8442 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/GradientPair.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8200 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/bridge_cpp.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.785344 interpret-core-0.4.1/symbolic/shared/libebm/common_c/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3037 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/common_c/common_c.c
+-rw-r--r--   0 vsts      (1001) docker     (122)     8476 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/common_c/common_c.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6580 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/common_c/logging.c
+-rw-r--r--   0 vsts      (1001) docker     (122)    10001 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/common_c/logging.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.785344 interpret-core-0.4.1/symbolic/shared/libebm/common_cpp/
+-rw-r--r--   0 vsts      (1001) docker     (122)    45433 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/common_cpp/common_cpp.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.789345 interpret-core-0.4.1/symbolic/shared/libebm/compute/
+-rw-r--r--   0 vsts      (1001) docker     (122)      553 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/Directory.Build.targets
+-rw-r--r--   0 vsts      (1001) docker     (122)     6427 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/Objective.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    35870 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/Objective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     6723 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/Registration.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13194 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/Registration.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    50721 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/approximate_math.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.793345 interpret-core-0.4.1/symbolic/shared/libebm/compute/avx512_ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      257 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/avx512_ebm/avx512_32.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13706 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)      477 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj.filters
+-rw-r--r--   0 vsts      (1001) docker     (122)     4386 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/compute.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    61597 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/compute_stats.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.793345 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      254 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_32.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7447 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_64.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13427 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)      593 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj.filters
+-rw-r--r--   0 vsts      (1001) docker     (122)     8950 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/sse2_32.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/sse2_64.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.793345 interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11435 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/cuda_32.cu
+-rw-r--r--   0 vsts      (1001) docker     (122)    14658 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)      505 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj.filters
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.797345 interpret-core-0.4.1/symbolic/shared/libebm/compute/metrics/
+-rw-r--r--   0 vsts      (1001) docker     (122)      177 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/metrics/AucMetric.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.797345 interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      630 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_32.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13332 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)      478 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj.filters
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.801345 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/
+-rw-r--r--   0 vsts      (1001) docker     (122)      432 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/CrossEntropyBinaryObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3630 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassMultitaskObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4464 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/ExampleRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3033 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/GammaDevianceRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      770 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossBinaryMultitaskObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7535 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossBinaryObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9437 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossMulticlassObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4596 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/PoissonDevianceRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4226 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/PseudoHuberRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3409 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/RmseLogLinkRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/RmseRegressionMultitaskObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9112 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/RmseRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4842 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/TweedieDevianceRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3245 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/objective_registrations.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      267 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/precompiled_header_cpp.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2301 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/registration_exceptions.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.801345 interpret-core-0.4.1/symbolic/shared/libebm/compute/special/
+-rw-r--r--   0 vsts      (1001) docker     (122)      164 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/special/precompiled_header_cpp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2366 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_c_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1068 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_c_functions.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1458 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_cpp_functions.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2800 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute_accessors.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    99988 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/dataset_shared.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2242 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/dataset_shared.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    20943 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/debug_ebm.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8264 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/ebm_internal.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    41443 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/ebm_stats.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.801345 interpret-core-0.4.1/symbolic/shared/libebm/inc/
+-rw-r--r--   0 vsts      (1001) docker     (122)    20435 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/inc/libebm.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3650 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/include_ordering.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    13166 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/interpret.sln
+-rw-r--r--   0 vsts      (1001) docker     (122)    77375 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/interpretable_numerics.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    24095 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/libebm.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)     5242 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/libebm.vcxproj.filters
+-rw-r--r--   0 vsts      (1001) docker     (122)      994 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/libebm_exports.def
+-rw-r--r--   0 vsts      (1001) docker     (122)     1257 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/libebm_exports.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/precompiled_header_cpp.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     6007 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/random.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    26424 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/sampling.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.801345 interpret-core-0.4.1/symbolic/shared/libebm/special/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2874 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/special/linux_wrap_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      164 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/special/precompiled_header_cpp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      790 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/special/windows_DllMain.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.809345 interpret-core-0.4.1/symbolic/shared/libebm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)    46248 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/CutQuantileTest.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    12964 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/CutUniformTest.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    24882 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/CutWinsorizedTest.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/DiscretizeTest.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     6935 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/RandomStreamTest.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    11983 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/SuggestGraphBoundsTest.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     6816 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/bit_packing_extremes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    68182 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/boosting_unusual_inputs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    17110 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/dataset_shared_test.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2740 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/include_c.c
+-rw-r--r--   0 vsts      (1001) docker     (122)    15959 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/interaction_unusual_inputs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1931 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.bat
+-rw-r--r--   0 vsts      (1001) docker     (122)    41676 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    14654 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    38501 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.sh
+-rw-r--r--   0 vsts      (1001) docker     (122)    15718 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)     1636 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.vcxproj.filters
+-rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/precompiled_header_test.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      298 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/precompiled_header_test.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    12851 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/random_test.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4893 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/rehydrate_booster.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      564 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/vs_python_setup.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.813345 interpret-core-0.4.1/symbolic/shared/vis/
+-rw-r--r--   0 vsts      (1001) docker     (122)      171 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/.babelrc
+-rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/.eslintrc.json
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (122)      238 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1472 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/package.json
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.813345 interpret-core-0.4.1/symbolic/shared/vis/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4433 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/src/index.js
+-rw-r--r--   0 vsts      (1001) docker     (122)     1469 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/src/styles.scss
+-rw-r--r--   0 vsts      (1001) docker     (122)      757 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/webpack.config.js
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.817345 interpret-core-0.4.1/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.817345 interpret-core-0.4.1/tests/api/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1895 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/api/test_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.821345 interpret-core-0.4.1/tests/blackbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/blackbox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1435 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/blackbox/test_permutationimportance.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      477 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/blackbox/test_sensitivity.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.821345 interpret-core-0.4.1/tests/ext/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/ext/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2502 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/ext/test_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.821345 interpret-core-0.4.1/tests/glassbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.825345 interpret-core-0.4.1/tests/glassbox/ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.825345 interpret-core-0.4.1/tests/glassbox/ebm/research/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/research/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8067 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/research/test_group_importance.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8414 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/research/test_purify.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4105 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/test_bin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    28189 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/test_ebm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5551 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/test_ebm_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5393 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/test_merge_ebms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      790 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/test_multiclass.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2055 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/test_decisiontree.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3499 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/test_linear.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.825345 interpret-core-0.4.1/tests/greybox/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/greybox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1459 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/greybox/test_treeinterpreter.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.825345 interpret-core-0.4.1/tests/provider/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      470 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/provider/test_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2257 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/provider/test_providers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1505 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_develop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_example_notebooks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3215 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_explainers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2702 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_ext.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      691 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_extension_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1108 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_mli_interop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9489 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_selenium.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8241 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/tutils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.829345 interpret-core-0.4.1/tests/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1099 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_SPOTgreedy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_clean_simple.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   113135 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_clean_x.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3041 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_compressed_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1453 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_explanation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8683 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_measure_interactions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2888 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_native.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.833345 interpret-core-0.4.1/tests/visual/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/visual/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      369 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/visual/test_dashboard.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      898 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/visual/test_inline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5223 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/visual/test_interactive.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/visual/test_plot.py
```

### Comparing `interpret-core-0.4.0/PKG-INFO` & `interpret-core-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpret-core
-Version: 0.4.0
+Version: 0.4.1
 Summary: Fit interpretable models. Explain blackbox machine learning.
 Home-page: https://github.com/interpretml/interpret
 Author: The InterpretML Contributors
 Author-email: interpret@microsoft.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `interpret-core-0.4.0/interpret/api/base.py` & `interpret-core-0.4.1/interpret/api/base.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/api/templates.py` & `interpret-core-0.4.1/interpret/api/templates.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/blackbox/_lime.py` & `interpret-core-0.4.1/interpret/blackbox/_lime.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/blackbox/_partialdependence.py` & `interpret-core-0.4.1/interpret/blackbox/_partialdependence.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/blackbox/_permutationimportance.py` & `interpret-core-0.4.1/interpret/blackbox/_permutationimportance.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/blackbox/_sensitivity.py` & `interpret-core-0.4.1/interpret/blackbox/_sensitivity.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/blackbox/_shap.py` & `interpret-core-0.4.1/interpret/blackbox/_shap.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/data/_response.py` & `interpret-core-0.4.1/interpret/data/_response.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/develop.py` & `interpret-core-0.4.1/interpret/develop.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/ext/examples.py` & `interpret-core-0.4.1/interpret/ext/examples.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/ext/extension.py` & `interpret-core-0.4.1/interpret/ext/extension.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/ext/extension_utils.py` & `interpret-core-0.4.1/interpret/ext/extension_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_decisiontree.py` & `interpret-core-0.4.1/interpret/glassbox/_decisiontree.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_ebm/_bin.py` & `interpret-core-0.4.1/interpret/glassbox/_ebm/_bin.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_ebm/_boost.py` & `interpret-core-0.4.1/interpret/glassbox/_ebm/_boost.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_ebm/_ebm.py` & `interpret-core-0.4.1/interpret/glassbox/_ebm/_ebm.py`

 * *Files 0% similar despite different names*

```diff
@@ -2184,15 +2184,15 @@
     term_scores\\_ : List of array of float with shape ``(n_feature0_bins, ..., n_featureN_bins, n_classes)`` or ``(n_feature0_bins, ..., n_featureN_bins)``
         Per-term list of the model scores.
         The last dimension of length n_classes is dropped for binary classification.
     standard_deviations\\_ : List of array of float with shape ``(n_feature0_bins, ..., n_featureN_bins, n_classes)`` or ``(n_feature0_bins, ..., n_featureN_bins)``
         Per-term list of the standard deviations of the bagged model scores.
         The last dimension of length n_classes is dropped for binary classification.
     link\\_ : str
-        Link function used to convert the predictions or target into linear space
+        Link function used to convert the predictions or targets into linear space
         additive scores and vice versa via the inverse link. Possible values include:
         "custom_classification", "logit", "probit", "cloglog", "loglog", "cauchit"
     link_param\\_ : float
         Float value that can be used by the link function. For classification it is only used by "custom_classification".
     bag_weights\\_ : array of float with shape ``(n_outer_bags,)``
         Per-bag record of the total weight within each bag.
     breakpoint_iteration\\_ : array of int with shape ``(n_stages, n_outer_bags)``
@@ -2546,15 +2546,15 @@
     bagged_scores\\_ : List of array of float with shape ``(n_outer_bags, n_feature0_bins, ..., n_featureN_bins)``
         Per-term list of the bagged model scores.
     term_scores\\_ : List of array of float with shape ``(n_feature0_bins, ..., n_featureN_bins)``
         Per-term list of the model scores.
     standard_deviations\\_ : List of array of float with shape ``(n_feature0_bins, ..., n_featureN_bins)``
         Per-term list of the standard deviations of the bagged model scores.
     link\\_ : str
-        Link function used to convert the predictions or target into linear space
+        Link function used to convert the predictions or targets into linear space
         additive scores and vice versa via the inverse link. Possible values include:
         "custom_regression", "power", "identity", "log", "inverse", "inverse_square", "sqrt"
     link_param\\_ : float
         Float value that can be used by the link function. The primary use is for the power link.
     bag_weights\\_ : array of float with shape ``(n_outer_bags,)``
         Per-bag record of the total weight within each bag.
     breakpoint_iteration\\_ : array of int with shape ``(n_stages, n_outer_bags)``
@@ -2822,15 +2822,15 @@
     bagged_scores\\_ : List of array of float with shape ``(n_outer_bags, n_bins)``
         Per-term list of the bagged model scores.
     term_scores\\_ : List of array of float with shape ``(n_bins)``
         Per-term list of the model scores.
     standard_deviations\\_ : List of array of float with shape ``(n_bins)``
         Per-term list of the standard deviations of the bagged model scores.
     link\\_ : str
-        Link function used to convert the predictions or target into linear space
+        Link function used to convert the predictions or targets into linear space
         additive scores and vice versa via the inverse link. Possible values include:
         "custom_classification", "logit", "probit", "cloglog", "loglog", "cauchit"
     link_param\\_ : float
         Float value that can be used by the link function. For classification it is only used by "custom_classification".
     bag_weights\\_ : array of float with shape ``(n_outer_bags,)``
         Per-bag record of the total weight within each bag.
     breakpoint_iteration\\_ : array of int with shape ``(n_stages, n_outer_bags)``
@@ -3111,15 +3111,15 @@
     bagged_scores\\_ : List of array of float with shape ``(n_outer_bags, n_bins)``
         Per-term list of the bagged model scores.
     term_scores\\_ : List of array of float with shape ``(n_bins)``
         Per-term list of the model scores.
     standard_deviations\\_ : List of array of float with shape ``(n_bins)``
         Per-term list of the standard deviations of the bagged model scores.
     link\\_ : str
-        Link function used to convert the predictions or target into linear space
+        Link function used to convert the predictions or targets into linear space
         additive scores and vice versa via the inverse link. Possible values include:
         "custom_regression", "power", "identity", "log", "inverse", "inverse_square", "sqrt"
     link_param\\_ : float
         Float value that can be used by the link function. The primary use is for the power link.
     bag_weights\\_ : array of float with shape ``(n_outer_bags,)``
         Per-bag record of the total weight within each bag.
     breakpoint_iteration\\_ : array of int with shape ``(n_stages, n_outer_bags)``
```

### Comparing `interpret-core-0.4.0/interpret/glassbox/_ebm/_merge_ebms.py` & `interpret-core-0.4.1/interpret/glassbox/_ebm/_merge_ebms.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_ebm/_multiclass.py` & `interpret-core-0.4.1/interpret/glassbox/_ebm/_multiclass.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_ebm/_research/__init__.py` & `interpret-core-0.4.1/interpret/glassbox/_ebm/_research/__init__.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_ebm/_research/_group_importance.py` & `interpret-core-0.4.1/interpret/glassbox/_ebm/_research/_group_importance.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_ebm/_research/_purify.py` & `interpret-core-0.4.1/interpret/glassbox/_ebm/_research/_purify.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_ebm/_tensor.py` & `interpret-core-0.4.1/interpret/glassbox/_ebm/_tensor.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_ebm/_utils.py` & `interpret-core-0.4.1/interpret/glassbox/_ebm/_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_linear.py` & `interpret-core-0.4.1/interpret/glassbox/_linear.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/glassbox/_skoperules.py` & `interpret-core-0.4.1/interpret/glassbox/_skoperules.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/greybox/_shaptree.py` & `interpret-core-0.4.1/interpret/greybox/_shaptree.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/greybox/_treeinterpreter.py` & `interpret-core-0.4.1/interpret/greybox/_treeinterpreter.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/lib/interpret-inline.js` & `interpret-core-0.4.1/interpret/lib/interpret-inline.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1076,16 +1076,16 @@
                             const r = e.getBoundingClientRect(),
                                 {
                                     width: n,
                                     height: i,
                                     fallback: a
                                 } = function(t) {
                                     const e = Kt(t);
-                                    let r = parseFloat(e.width),
-                                        n = parseFloat(e.height);
+                                    let r = parseFloat(e.width) || 0,
+                                        n = parseFloat(e.height) || 0;
                                     const i = te(t),
                                         a = i ? t.offsetWidth : r,
                                         o = i ? t.offsetHeight : n,
                                         s = ae(r) !== a || ae(n) !== o;
                                     return s && (r = a, n = o), {
                                         width: r,
                                         height: n,
@@ -22246,31 +22246,39 @@
                                             },
                                             len: {
                                                 valType: "number",
                                                 min: 0,
                                                 dflt: 1
                                             },
                                             x: {
-                                                valType: "number",
-                                                min: -2,
-                                                max: 3
+                                                valType: "number"
+                                            },
+                                            xref: {
+                                                valType: "enumerated",
+                                                dflt: "paper",
+                                                values: ["container", "paper"],
+                                                editType: "layoutstyle"
                                             },
                                             xanchor: {
                                                 valType: "enumerated",
                                                 values: ["left", "center", "right"]
                                             },
                                             xpad: {
                                                 valType: "number",
                                                 min: 0,
                                                 dflt: 10
                                             },
                                             y: {
-                                                valType: "number",
-                                                min: -2,
-                                                max: 3
+                                                valType: "number"
+                                            },
+                                            yref: {
+                                                valType: "enumerated",
+                                                dflt: "paper",
+                                                values: ["container", "paper"],
+                                                editType: "layoutstyle"
                                             },
                                             yanchor: {
                                                 valType: "enumerated",
                                                 values: ["top", "middle", "bottom"]
                                             },
                                             ypad: {
                                                 valType: "number",
@@ -22388,34 +22396,52 @@
                                                 },
                                                 d = r.width - p.l - p.r,
                                                 v = r.height - p.t - p.b,
                                                 g = "v" === h("orientation"),
                                                 y = h("thicknessmode");
                                             h("thickness", "fraction" === y ? 30 / (g ? d : v) : 30);
                                             var m = h("lenmode");
-                                            h("len", "fraction" === m ? 1 : g ? v : d), h("x", g ? 1.02 : .5), h("xanchor", g ? "left" : "center"), h("xpad"), h("y", g ? .5 : 1.02), h("yanchor", g ? "middle" : "bottom"), h("ypad"), n.noneOrAll(f, c, ["x", "y"]), h("outlinecolor"), h("outlinewidth"), h("bordercolor"), h("borderwidth"), h("bgcolor");
-                                            var x = n.coerce(f, c, {
+                                            h("len", "fraction" === m ? 1 : g ? v : d);
+                                            var x, b, _, w = "paper" === h("yref"),
+                                                k = "paper" === h("xref"),
+                                                T = "left";
+                                            g ? (_ = "middle", T = k ? "left" : "right", x = k ? 1.02 : 1, b = .5) : (_ = w ? "bottom" : "top", T = "center", x = .5, b = w ? 1.02 : 1), n.coerce(f, c, {
+                                                x: {
+                                                    valType: "number",
+                                                    min: k ? -2 : 0,
+                                                    max: k ? 3 : 1,
+                                                    dflt: x
+                                                }
+                                            }, "x"), n.coerce(f, c, {
+                                                y: {
+                                                    valType: "number",
+                                                    min: w ? -2 : 0,
+                                                    max: w ? 3 : 1,
+                                                    dflt: b
+                                                }
+                                            }, "y"), h("xanchor", T), h("xpad"), h("yanchor", _), h("ypad"), n.noneOrAll(f, c, ["x", "y"]), h("outlinecolor"), h("outlinewidth"), h("bordercolor"), h("borderwidth"), h("bgcolor");
+                                            var M = n.coerce(f, c, {
                                                 ticklabelposition: {
                                                     valType: "enumerated",
                                                     dflt: "outside",
                                                     values: g ? ["outside", "inside", "outside top", "inside top", "outside bottom", "inside bottom"] : ["outside", "inside", "outside left", "inside left", "outside right", "inside right"]
                                                 }
                                             }, "ticklabelposition");
-                                            h("ticklabeloverflow", -1 !== x.indexOf("inside") ? "hide past domain" : "hide past div"), a(f, c, h, "linear");
-                                            var b = r.font,
-                                                _ = {
+                                            h("ticklabeloverflow", -1 !== M.indexOf("inside") ? "hide past domain" : "hide past div"), a(f, c, h, "linear");
+                                            var A = r.font,
+                                                S = {
                                                     outerTicks: !1,
-                                                    font: b
-                                                }; - 1 !== x.indexOf("inside") && (_.bgColor = "black"), l(f, c, h, "linear", _), s(f, c, h, "linear", _), o(f, c, h, "linear", _), h("title.text", r._dfltTitle.colorbar);
-                                            var w = c.showticklabels ? c.tickfont : b,
-                                                k = n.extendFlat({}, w, {
-                                                    color: b.color,
-                                                    size: n.bigFont(w.size)
+                                                    font: A
+                                                }; - 1 !== M.indexOf("inside") && (S.bgColor = "black"), l(f, c, h, "linear", S), s(f, c, h, "linear", S), o(f, c, h, "linear", S), h("title.text", r._dfltTitle.colorbar);
+                                            var E = c.showticklabels ? c.tickfont : A,
+                                                C = n.extendFlat({}, E, {
+                                                    color: A.color,
+                                                    size: n.bigFont(E.size)
                                                 });
-                                            n.coerceFont(h, "title.font", k), h("title.side", g ? "top" : "right")
+                                            n.coerceFont(h, "title.font", C), h("title.side", g ? "top" : "right")
                                         }
                                     },
                                     98981: function(t, e, r) {
                                         "use strict";
                                         var n = r(39898),
                                             i = r(84267),
                                             a = r(74875),
@@ -22508,29 +22534,31 @@
                                                             E = e.bgcolor,
                                                             C = e.xanchor,
                                                             L = e.yanchor,
                                                             P = e.xpad,
                                                             O = e.ypad,
                                                             I = e.x,
                                                             D = o ? e.y : 1 - e.y,
-                                                            z = r._fullLayout,
-                                                            R = z._size,
-                                                            F = e._fillcolor,
-                                                            B = e._line,
-                                                            N = e.title,
-                                                            j = N.side,
-                                                            U = e._zrange || n.extent(("function" == typeof F ? F : B.color).domain()),
-                                                            V = "function" == typeof B.color ? B.color : function() {
-                                                                return B.color
+                                                            z = "paper" === e.yref,
+                                                            R = "paper" === e.xref,
+                                                            F = r._fullLayout,
+                                                            B = F._size,
+                                                            N = e._fillcolor,
+                                                            j = e._line,
+                                                            U = e.title,
+                                                            V = U.side,
+                                                            H = e._zrange || n.extent(("function" == typeof N ? N : j.color).domain()),
+                                                            q = "function" == typeof j.color ? j.color : function() {
+                                                                return j.color
                                                             },
-                                                            H = "function" == typeof F ? F : function() {
-                                                                return F
+                                                            G = "function" == typeof N ? N : function() {
+                                                                return N
                                                             },
-                                                            q = e._levels,
-                                                            G = function(t, e, r) {
+                                                            Y = e._levels,
+                                                            W = function(t, e, r) {
                                                                 var n, i, a = e._levels,
                                                                     o = [],
                                                                     s = [],
                                                                     l = a.end + a.size / 100,
                                                                     u = a.size,
                                                                     c = 1.001 * r[0] - .001 * r[1],
                                                                     f = 1.001 * r[1] - .001 * r[0];
@@ -22544,35 +22572,37 @@
                                                                         return t - a.size / 2
                                                                     }))).push(s[s.length - 1] + a.size)
                                                                 } else e._fillcolor && "string" == typeof e._fillcolor && (s = [0]);
                                                                 return a.size < 0 && (o.reverse(), s.reverse()), {
                                                                     line: o,
                                                                     fill: s
                                                                 }
-                                                            }(0, e, U),
-                                                            Y = G.fill,
-                                                            W = G.line,
-                                                            Z = Math.round(y * ("fraction" === _ ? o ? R.w : R.h : 1)),
-                                                            X = Z / (o ? R.w : R.h),
-                                                            K = Math.round(l * ("fraction" === h ? o ? R.h : R.w : 1)),
-                                                            J = K / (o ? R.h : R.w),
-                                                            $ = Math.round(o ? I * R.w + P : D * R.h + O),
-                                                            Q = {
+                                                            }(0, e, H),
+                                                            Z = W.fill,
+                                                            X = W.line,
+                                                            K = Math.round(y * ("fraction" === _ ? o ? B.w : B.h : 1)),
+                                                            J = K / (o ? B.w : B.h),
+                                                            $ = Math.round(l * ("fraction" === h ? o ? B.h : B.w : 1)),
+                                                            Q = $ / (o ? B.h : B.w),
+                                                            tt = R ? B.w : r._fullLayout.width,
+                                                            et = z ? B.h : r._fullLayout.height,
+                                                            rt = Math.round(o ? I * tt + P : D * et + O),
+                                                            nt = {
                                                                 center: .5,
                                                                 right: 1
                                                             } [C] || 0,
-                                                            tt = {
+                                                            it = {
                                                                 top: 1,
                                                                 middle: .5
                                                             } [L] || 0,
-                                                            et = o ? I - Q * X : D - tt * X,
-                                                            rt = o ? D - tt * J : I - Q * J,
-                                                            nt = Math.round(o ? R.h * (1 - rt) : R.w * rt);
-                                                        e._lenFrac = J, e._thickFrac = X, e._uFrac = et, e._vFrac = rt;
-                                                        var it = e._axis = function(t, e, r) {
+                                                            at = o ? I - nt * J : D - it * J,
+                                                            ot = o ? D - it * Q : I - nt * Q,
+                                                            st = Math.round(o ? et * (1 - ot) : tt * ot);
+                                                        e._lenFrac = Q, e._thickFrac = J, e._uFrac = at, e._vFrac = ot;
+                                                        var lt = e._axis = function(t, e, r) {
                                                             var n = t._fullLayout,
                                                                 i = "v" === e.orientation,
                                                                 a = {
                                                                     type: "linear",
                                                                     range: r,
                                                                     tickmode: e.tickmode,
                                                                     nticks: e.nticks,
@@ -22620,188 +22650,203 @@
                                                                     calendar: n.calendar
                                                                 };
 
                                                             function c(t, e) {
                                                                 return u.coerce(a, s, b, t, e)
                                                             }
                                                             return m(a, s, c, l, n), x(a, s, c, l), s
-                                                        }(r, e, U);
-                                                        it.position = X + (o ? I + P / R.w : D + O / R.h);
-                                                        var at = -1 !== ["top", "bottom"].indexOf(j);
-                                                        if (o && at && (it.title.side = j, it.titlex = I + P / R.w, it.titley = rt + ("top" === N.side ? J - O / R.h : O / R.h)), o || at || (it.title.side = j, it.titley = D + O / R.h, it.titlex = rt + P / R.w), B.color && "auto" === e.tickmode) {
-                                                            it.tickmode = "linear", it.tick0 = q.start;
-                                                            var ot = q.size,
-                                                                st = u.constrain(K / 50, 4, 15) + 1,
-                                                                lt = (U[1] - U[0]) / ((e.nticks || st) * ot);
-                                                            if (lt > 1) {
-                                                                var ut = Math.pow(10, Math.floor(Math.log(lt) / Math.LN10));
-                                                                ot *= ut * u.roundUp(lt / ut, [2, 5, 10]), (Math.abs(q.start) / q.size + 1e-6) % 1 < 2e-6 && (it.tick0 = 0)
-                                                            }
-                                                            it.dtick = ot
-                                                        }
-                                                        it.domain = o ? [rt + O / R.h, rt + J - O / R.h] : [rt + P / R.w, rt + J - P / R.w], it.setScale(), t.attr("transform", c(Math.round(R.l), Math.round(R.t)));
-                                                        var ct, ft = t.select("." + M.cbtitleunshift).attr("transform", c(-Math.round(R.l), -Math.round(R.t))),
-                                                            ht = it.ticklabelposition,
-                                                            pt = it.title.font.size,
-                                                            dt = t.select("." + M.cbaxis),
-                                                            vt = 0,
-                                                            gt = 0;
+                                                        }(r, e, H);
+                                                        lt.position = J + (o ? I + P / B.w : D + O / B.h);
+                                                        var ut = -1 !== ["top", "bottom"].indexOf(V);
+                                                        if (o && ut && (lt.title.side = V, lt.titlex = I + P / B.w, lt.titley = ot + ("top" === U.side ? Q - O / B.h : O / B.h)), o || ut || (lt.title.side = V, lt.titley = D + O / B.h, lt.titlex = ot + P / B.w), j.color && "auto" === e.tickmode) {
+                                                            lt.tickmode = "linear", lt.tick0 = Y.start;
+                                                            var ct = Y.size,
+                                                                ft = u.constrain($ / 50, 4, 15) + 1,
+                                                                ht = (H[1] - H[0]) / ((e.nticks || ft) * ct);
+                                                            if (ht > 1) {
+                                                                var pt = Math.pow(10, Math.floor(Math.log(ht) / Math.LN10));
+                                                                ct *= pt * u.roundUp(ht / pt, [2, 5, 10]), (Math.abs(Y.start) / Y.size + 1e-6) % 1 < 2e-6 && (lt.tick0 = 0)
+                                                            }
+                                                            lt.dtick = ct
+                                                        }
+                                                        lt.domain = o ? [ot + O / B.h, ot + Q - O / B.h] : [ot + P / B.w, ot + Q - P / B.w], lt.setScale(), t.attr("transform", c(Math.round(B.l), Math.round(B.t)));
+                                                        var dt, vt = t.select("." + M.cbtitleunshift).attr("transform", c(-Math.round(B.l), -Math.round(B.t))),
+                                                            gt = lt.ticklabelposition,
+                                                            yt = lt.title.font.size,
+                                                            mt = t.select("." + M.cbaxis),
+                                                            xt = 0,
+                                                            bt = 0;
 
-                                                        function yt(n, i) {
+                                                        function _t(n, i) {
                                                             var a = {
-                                                                    propContainer: it,
+                                                                    propContainer: lt,
                                                                     propName: e._propPrefix + "title",
                                                                     traceIndex: e._traceIndex,
                                                                     _meta: e._meta,
-                                                                    placeholder: z._dfltTitle.colorbar,
+                                                                    placeholder: F._dfltTitle.colorbar,
                                                                     containerGroup: t.select("." + M.cbtitle)
                                                                 },
                                                                 o = "h" === n.charAt(0) ? n.substr(1) : "h" + n;
                                                             t.selectAll("." + o + ",." + o + "-math-group").remove(), v.draw(r, n, f(a, i || {}))
                                                         }
                                                         return u.syncOrAsync([a.previousPromises, function() {
                                                             var t, e;
-                                                            (o && at || !o && !at) && ("top" === j && (t = P + R.l + R.w * I, e = O + R.t + R.h * (1 - rt - J) + 3 + .75 * pt), "bottom" === j && (t = P + R.l + R.w * I, e = O + R.t + R.h * (1 - rt) - 3 - .25 * pt), "right" === j && (e = O + R.t + R.h * D + 3 + .75 * pt, t = P + R.l + R.w * rt), yt(it._id + "title", {
+                                                            (o && ut || !o && !ut) && ("top" === V && (t = P + B.l + tt * I, e = O + B.t + et * (1 - ot - Q) + 3 + .75 * yt), "bottom" === V && (t = P + B.l + tt * I, e = O + B.t + et * (1 - ot) - 3 - .25 * yt), "right" === V && (e = O + B.t + et * D + 3 + .75 * yt, t = P + B.l + tt * ot), _t(lt._id + "title", {
                                                                 attributes: {
                                                                     x: t,
                                                                     y: e,
                                                                     "text-anchor": o ? "start" : "middle"
                                                                 }
                                                             }))
                                                         }, function() {
-                                                            if (!o && !at || o && at) {
+                                                            if (!o && !ut || o && ut) {
                                                                 var a, l = t.select("." + M.cbtitle),
                                                                     f = l.select("text"),
                                                                     h = [-A / 2, A / 2],
-                                                                    d = l.select(".h" + it._id + "title-math-group").node(),
+                                                                    d = l.select(".h" + lt._id + "title-math-group").node(),
                                                                     v = 15.6;
-                                                                if (f.node() && (v = parseInt(f.node().style.fontSize, 10) * w), d ? (a = p.bBox(d), gt = a.width, (vt = a.height) > v && (h[1] -= (vt - v) / 2)) : f.node() && !f.classed(M.jsPlaceholder) && (a = p.bBox(f.node()), gt = a.width, vt = a.height), o) {
-                                                                    if (vt) {
-                                                                        if (vt += 5, "top" === j) it.domain[1] -= vt / R.h, h[1] *= -1;
+                                                                if (f.node() && (v = parseInt(f.node().style.fontSize, 10) * w), d ? (a = p.bBox(d), bt = a.width, (xt = a.height) > v && (h[1] -= (xt - v) / 2)) : f.node() && !f.classed(M.jsPlaceholder) && (a = p.bBox(f.node()), bt = a.width, xt = a.height), o) {
+                                                                    if (xt) {
+                                                                        if (xt += 5, "top" === V) lt.domain[1] -= xt / B.h, h[1] *= -1;
                                                                         else {
-                                                                            it.domain[0] += vt / R.h;
+                                                                            lt.domain[0] += xt / B.h;
                                                                             var y = g.lineCount(f);
                                                                             h[1] += (1 - y) * v
                                                                         }
-                                                                        l.attr("transform", c(h[0], h[1])), it.setScale()
+                                                                        l.attr("transform", c(h[0], h[1])), lt.setScale()
                                                                     }
-                                                                } else gt && ("right" === j && (it.domain[0] += (gt + pt / 2) / R.w), l.attr("transform", c(h[0], h[1])), it.setScale())
+                                                                } else bt && ("right" === V && (lt.domain[0] += (bt + yt / 2) / B.w), l.attr("transform", c(h[0], h[1])), lt.setScale())
                                                             }
-                                                            t.selectAll("." + M.cbfills + ",." + M.cblines).attr("transform", o ? c(0, Math.round(R.h * (1 - it.domain[1]))) : c(Math.round(R.w * it.domain[0]), 0)), dt.attr("transform", o ? c(0, Math.round(-R.t)) : c(Math.round(-R.l), 0));
-                                                            var m = t.select("." + M.cbfills).selectAll("rect." + M.cbfill).attr("style", "").data(Y);
+                                                            t.selectAll("." + M.cbfills + ",." + M.cblines).attr("transform", o ? c(0, Math.round(B.h * (1 - lt.domain[1]))) : c(Math.round(B.w * lt.domain[0]), 0)), mt.attr("transform", o ? c(0, Math.round(-B.t)) : c(Math.round(-B.l), 0));
+                                                            var m = t.select("." + M.cbfills).selectAll("rect." + M.cbfill).attr("style", "").data(Z);
                                                             m.enter().append("rect").classed(M.cbfill, !0).style("stroke", "none"), m.exit().remove();
-                                                            var x = U.map(it.c2p).map(Math.round).sort((function(t, e) {
+                                                            var x = H.map(lt.c2p).map(Math.round).sort((function(t, e) {
                                                                 return t - e
                                                             }));
                                                             m.each((function(t, a) {
-                                                                var s = [0 === a ? U[0] : (Y[a] + Y[a - 1]) / 2, a === Y.length - 1 ? U[1] : (Y[a] + Y[a + 1]) / 2].map(it.c2p).map(Math.round);
+                                                                var s = [0 === a ? H[0] : (Z[a] + Z[a - 1]) / 2, a === Z.length - 1 ? H[1] : (Z[a] + Z[a + 1]) / 2].map(lt.c2p).map(Math.round);
                                                                 o && (s[1] = u.constrain(s[1] + (s[1] > s[0]) ? 1 : -1, x[0], x[1]));
-                                                                var l = n.select(this).attr(o ? "x" : "y", $).attr(o ? "y" : "x", n.min(s)).attr(o ? "width" : "height", Math.max(Z, 2)).attr(o ? "height" : "width", Math.max(n.max(s) - n.min(s), 2));
+                                                                var l = n.select(this).attr(o ? "x" : "y", rt).attr(o ? "y" : "x", n.min(s)).attr(o ? "width" : "height", Math.max(K, 2)).attr(o ? "height" : "width", Math.max(n.max(s) - n.min(s), 2));
                                                                 if (e._fillgradient) p.gradient(l, r, e._id, o ? "vertical" : "horizontalreversed", e._fillgradient, "fill");
                                                                 else {
-                                                                    var c = H(t).replace("e-", "");
+                                                                    var c = G(t).replace("e-", "");
                                                                     l.attr("fill", i(c).toHexString())
                                                                 }
                                                             }));
-                                                            var b = t.select("." + M.cblines).selectAll("path." + M.cbline).data(B.color && B.width ? W : []);
+                                                            var b = t.select("." + M.cblines).selectAll("path." + M.cbline).data(j.color && j.width ? X : []);
                                                             b.enter().append("path").classed(M.cbline, !0), b.exit().remove(), b.each((function(t) {
-                                                                var e = $,
-                                                                    r = Math.round(it.c2p(t)) + B.width / 2 % 1;
-                                                                n.select(this).attr("d", "M" + (o ? e + "," + r : r + "," + e) + (o ? "h" : "v") + Z).call(p.lineGroupStyle, B.width, V(t), B.dash)
-                                                            })), dt.selectAll("g." + it._id + "tick,path").remove();
-                                                            var _ = $ + Z + (A || 0) / 2 - ("outside" === e.ticks ? 1 : 0),
-                                                                k = s.calcTicks(it),
-                                                                T = s.getTickSigns(it)[2];
-                                                            return s.drawTicks(r, it, {
-                                                                vals: "inside" === it.ticks ? s.clipEnds(it, k) : k,
-                                                                layer: dt,
-                                                                path: s.makeTickPath(it, _, T),
-                                                                transFn: s.makeTransTickFn(it)
-                                                            }), s.drawLabels(r, it, {
+                                                                var e = rt,
+                                                                    r = Math.round(lt.c2p(t)) + j.width / 2 % 1;
+                                                                n.select(this).attr("d", "M" + (o ? e + "," + r : r + "," + e) + (o ? "h" : "v") + K).call(p.lineGroupStyle, j.width, q(t), j.dash)
+                                                            })), mt.selectAll("g." + lt._id + "tick,path").remove();
+                                                            var _ = rt + K + (A || 0) / 2 - ("outside" === e.ticks ? 1 : 0),
+                                                                k = s.calcTicks(lt),
+                                                                T = s.getTickSigns(lt)[2];
+                                                            return s.drawTicks(r, lt, {
+                                                                vals: "inside" === lt.ticks ? s.clipEnds(lt, k) : k,
+                                                                layer: mt,
+                                                                path: s.makeTickPath(lt, _, T),
+                                                                transFn: s.makeTransTickFn(lt)
+                                                            }), s.drawLabels(r, lt, {
                                                                 vals: k,
-                                                                layer: dt,
-                                                                transFn: s.makeTransTickLabelFn(it),
-                                                                labelFns: s.makeLabelFns(it, _)
+                                                                layer: mt,
+                                                                transFn: s.makeTransTickLabelFn(lt),
+                                                                labelFns: s.makeLabelFns(lt, _)
                                                             })
                                                         }, function() {
-                                                            if (o && !at || !o && at) {
-                                                                var t, i, a = it.position || 0,
-                                                                    s = it._offset + it._length / 2;
-                                                                if ("right" === j) i = s, t = R.l + R.w * a + 10 + pt * (it.showticklabels ? 1 : .5);
-                                                                else if (t = s, "bottom" === j && (i = R.t + R.h * a + 10 + (-1 === ht.indexOf("inside") ? it.tickfont.size : 0) + ("intside" !== it.ticks && e.ticklen || 0)), "top" === j) {
-                                                                    var l = N.text.split("<br>").length;
-                                                                    i = R.t + R.h * a + 10 - Z - w * pt * l
+                                                            if (o && !ut || !o && ut) {
+                                                                var t, i, a = lt.position || 0,
+                                                                    s = lt._offset + lt._length / 2;
+                                                                if ("right" === V) i = s, t = B.l + tt * a + 10 + yt * (lt.showticklabels ? 1 : .5);
+                                                                else if (t = s, "bottom" === V && (i = B.t + et * a + 10 + (-1 === gt.indexOf("inside") ? lt.tickfont.size : 0) + ("intside" !== lt.ticks && e.ticklen || 0)), "top" === V) {
+                                                                    var l = U.text.split("<br>").length;
+                                                                    i = B.t + et * a + 10 - K - w * yt * l
                                                                 }
-                                                                yt((o ? "h" : "v") + it._id + "title", {
+                                                                _t((o ? "h" : "v") + lt._id + "title", {
                                                                     avoid: {
-                                                                        selection: n.select(r).selectAll("g." + it._id + "tick"),
-                                                                        side: j,
-                                                                        offsetTop: o ? 0 : R.t,
-                                                                        offsetLeft: o ? R.l : 0,
-                                                                        maxShift: o ? z.width : z.height
+                                                                        selection: n.select(r).selectAll("g." + lt._id + "tick"),
+                                                                        side: V,
+                                                                        offsetTop: o ? 0 : B.t,
+                                                                        offsetLeft: o ? B.l : 0,
+                                                                        maxShift: o ? F.width : F.height
                                                                     },
                                                                     attributes: {
                                                                         x: t,
                                                                         y: i,
                                                                         "text-anchor": "middle"
                                                                     },
                                                                     transform: {
                                                                         rotate: o ? -90 : 0,
                                                                         offset: 0
                                                                     }
                                                                 })
                                                             }
                                                         }, a.previousPromises, function() {
-                                                            var n, s = Z + A / 2; - 1 === ht.indexOf("inside") && (n = p.bBox(dt.node()), s += o ? n.width : n.height), ct = ft.select("text");
+                                                            var n, s = K + A / 2; - 1 === gt.indexOf("inside") && (n = p.bBox(mt.node()), s += o ? n.width : n.height), dt = vt.select("text");
                                                             var u = 0,
-                                                                f = o && "top" === j,
-                                                                v = !o && "right" === j,
+                                                                f = o && "top" === V,
+                                                                v = !o && "right" === V,
                                                                 g = 0;
-                                                            if (ct.node() && !ct.classed(M.jsPlaceholder)) {
-                                                                var m, x = ft.select(".h" + it._id + "title-math-group").node();
-                                                                x && (o && at || !o && !at) ? (u = (n = p.bBox(x)).width, m = n.height) : (u = (n = p.bBox(ft.node())).right - R.l - (o ? $ : nt), m = n.bottom - R.t - (o ? nt : $), o || "top" !== j || (s += n.height, g = n.height)), v && (ct.attr("transform", c(u / 2 + pt / 2, 0)), u *= 2), s = Math.max(s, o ? u : m)
+                                                            if (dt.node() && !dt.classed(M.jsPlaceholder)) {
+                                                                var m, x = vt.select(".h" + lt._id + "title-math-group").node();
+                                                                x && (o && ut || !o && !ut) ? (u = (n = p.bBox(x)).width, m = n.height) : (u = (n = p.bBox(vt.node())).right - B.l - (o ? rt : st), m = n.bottom - B.t - (o ? st : rt), o || "top" !== V || (s += n.height, g = n.height)), v && (dt.attr("transform", c(u / 2 + yt / 2, 0)), u *= 2), s = Math.max(s, o ? u : m)
                                                             }
                                                             var b = 2 * (o ? P : O) + s + S + A / 2,
                                                                 w = 0;
-                                                            !o && N.text && "bottom" === L && D <= 0 && (b += w = b / 2, g += w), z._hColorbarMoveTitle = w, z._hColorbarMoveCBTitle = g;
-                                                            var F = S + A;
-                                                            t.select("." + M.cbbg).attr("x", (o ? $ : nt) - F / 2 - (o ? P : 0)).attr("y", (o ? nt : $) - (o ? K : O + g - w)).attr(o ? "width" : "height", Math.max(b - w, 2)).attr(o ? "height" : "width", Math.max(K + F, 2)).call(d.fill, E).call(d.stroke, e.bordercolor).style("stroke-width", S);
-                                                            var B = v ? Math.max(u - 10, 0) : 0;
-                                                            if (t.selectAll("." + M.cboutline).attr("x", (o ? $ : nt + P) + B).attr("y", (o ? nt + O - K : $) + (f ? vt : 0)).attr(o ? "width" : "height", Math.max(Z, 2)).attr(o ? "height" : "width", Math.max(K - (o ? 2 * O + vt : 2 * P + B), 2)).call(d.stroke, e.outlinecolor).style({
-                                                                    fill: "none",
-                                                                    "stroke-width": A
-                                                                }), t.attr("transform", c(R.l - (o ? Q * b : 0), R.t - (o ? 0 : (1 - tt) * b - g))), !o && (S || i(E).getAlpha() && !i.equals(z.paper_bgcolor, E))) {
-                                                                var U = dt.selectAll("text"),
-                                                                    V = U[0].length,
-                                                                    H = t.select("." + M.cbbg).node(),
-                                                                    q = p.bBox(H),
-                                                                    G = p.getTranslate(t);
-                                                                U.each((function(t, e) {
-                                                                    var r = V - 1;
+                                                            !o && U.text && "bottom" === L && D <= 0 && (b += w = b / 2, g += w), F._hColorbarMoveTitle = w, F._hColorbarMoveCBTitle = g;
+                                                            var N = S + A,
+                                                                j = (o ? rt : st) - N / 2 - (o ? P : 0),
+                                                                H = (o ? st : rt) - (o ? $ : O + g - w);
+                                                            t.select("." + M.cbbg).attr("x", j).attr("y", H).attr(o ? "width" : "height", Math.max(b - w, 2)).attr(o ? "height" : "width", Math.max($ + N, 2)).call(d.fill, E).call(d.stroke, e.bordercolor).style("stroke-width", S);
+                                                            var q = v ? Math.max(u - 10, 0) : 0;
+                                                            t.selectAll("." + M.cboutline).attr("x", (o ? rt : st + P) + q).attr("y", (o ? st + O - $ : rt) + (f ? xt : 0)).attr(o ? "width" : "height", Math.max(K, 2)).attr(o ? "height" : "width", Math.max($ - (o ? 2 * O + xt : 2 * P + q), 2)).call(d.stroke, e.outlinecolor).style({
+                                                                fill: "none",
+                                                                "stroke-width": A
+                                                            });
+                                                            var G = o ? nt * b : 0,
+                                                                Y = o ? 0 : (1 - it) * b - g;
+                                                            if (G = R ? B.l - G : -G, Y = z ? B.t - Y : -Y, t.attr("transform", c(G, Y)), !o && (S || i(E).getAlpha() && !i.equals(F.paper_bgcolor, E))) {
+                                                                var W = mt.selectAll("text"),
+                                                                    Z = W[0].length,
+                                                                    X = t.select("." + M.cbbg).node(),
+                                                                    J = p.bBox(X),
+                                                                    Q = p.getTranslate(t);
+                                                                W.each((function(t, e) {
+                                                                    var r = Z - 1;
                                                                     if (0 === e || e === r) {
                                                                         var n, i = p.bBox(this),
                                                                             a = p.getTranslate(this);
                                                                         if (e === r) {
                                                                             var o = i.right + a.x;
-                                                                            (n = q.right + G.x + nt - S - 2 + I - o) > 0 && (n = 0)
+                                                                            (n = J.right + Q.x + st - S - 2 + I - o) > 0 && (n = 0)
                                                                         } else if (0 === e) {
                                                                             var s = i.left + a.x;
-                                                                            (n = q.left + G.x + nt + S + 2 - s) < 0 && (n = 0)
+                                                                            (n = J.left + Q.x + st + S + 2 - s) < 0 && (n = 0)
                                                                         }
-                                                                        n && (V < 3 ? this.setAttribute("transform", "translate(" + n + ",0) " + this.getAttribute("transform")) : this.setAttribute("visibility", "hidden"))
+                                                                        n && (Z < 3 ? this.setAttribute("transform", "translate(" + n + ",0) " + this.getAttribute("transform")) : this.setAttribute("visibility", "hidden"))
                                                                     }
                                                                 }))
                                                             }
-                                                            var Y = {},
-                                                                W = k[C],
-                                                                X = T[C],
-                                                                J = k[L],
-                                                                et = T[L],
-                                                                rt = b - Z;
-                                                            o ? ("pixels" === h ? (Y.y = D, Y.t = K * J, Y.b = K * et) : (Y.t = Y.b = 0, Y.yt = D + l * J, Y.yb = D - l * et), "pixels" === _ ? (Y.x = I, Y.l = b * W, Y.r = b * X) : (Y.l = rt * W, Y.r = rt * X, Y.xl = I - y * W, Y.xr = I + y * X)) : ("pixels" === h ? (Y.x = I, Y.l = K * W, Y.r = K * X) : (Y.l = Y.r = 0, Y.xl = I + l * W, Y.xr = I - l * X), "pixels" === _ ? (Y.y = 1 - D, Y.t = b * J, Y.b = b * et) : (Y.t = rt * J, Y.b = rt * et, Y.yt = D - y * J, Y.yb = D + y * et)), a.autoMargin(r, e._id, Y)
+                                                            var tt = {},
+                                                                et = k[C],
+                                                                at = T[C],
+                                                                ot = k[L],
+                                                                ct = T[L],
+                                                                ft = b - K;
+                                                            o ? ("pixels" === h ? (tt.y = D, tt.t = $ * ot, tt.b = $ * ct) : (tt.t = tt.b = 0, tt.yt = D + l * ot, tt.yb = D - l * ct), "pixels" === _ ? (tt.x = I, tt.l = b * et, tt.r = b * at) : (tt.l = ft * et, tt.r = ft * at, tt.xl = I - y * et, tt.xr = I + y * at)) : ("pixels" === h ? (tt.x = I, tt.l = $ * et, tt.r = $ * at) : (tt.l = tt.r = 0, tt.xl = I + l * et, tt.xr = I - l * at), "pixels" === _ ? (tt.y = 1 - D, tt.t = b * ot, tt.b = b * ct) : (tt.t = ft * ot, tt.b = ft * ct, tt.yt = D - y * ot, tt.yb = D + y * ct));
+                                                            var ht = e.y < .5 ? "b" : "t",
+                                                                pt = e.x < .5 ? "l" : "r";
+                                                            r._fullLayout._reservedMargin[e._id] = {};
+                                                            var bt = {
+                                                                r: F.width - j - G,
+                                                                l: j + tt.r,
+                                                                b: F.height - H - Y,
+                                                                t: H + tt.b
+                                                            };
+                                                            R && z ? a.autoMargin(r, e._id, tt) : R ? r._fullLayout._reservedMargin[e._id][ht] = bt[ht] : z || o ? r._fullLayout._reservedMargin[e._id][pt] = bt[pt] : r._fullLayout._reservedMargin[e._id][ht] = bt[ht]
                                                         }], r)
                                                     }(r, e, t);
                                                     y && y.then && (t._promises || []).push(y), t._context.edits.colorbarPosition && function(t, e, r) {
                                                         var n, i, a, s = "v" === e.orientation,
                                                             u = r._fullLayout._size;
                                                         l.init({
                                                             element: t.node(),
@@ -27203,30 +27248,38 @@
                                                 valType: "enumerated",
                                                 values: ["toggleitem", "togglegroup"],
                                                 dflt: "togglegroup",
                                                 editType: "legend"
                                             },
                                             x: {
                                                 valType: "number",
-                                                min: -2,
-                                                max: 3,
                                                 editType: "legend"
                                             },
+                                            xref: {
+                                                valType: "enumerated",
+                                                dflt: "paper",
+                                                values: ["container", "paper"],
+                                                editType: "layoutstyle"
+                                            },
                                             xanchor: {
                                                 valType: "enumerated",
                                                 values: ["auto", "left", "center", "right"],
                                                 dflt: "left",
                                                 editType: "legend"
                                             },
                                             y: {
                                                 valType: "number",
-                                                min: -2,
-                                                max: 3,
                                                 editType: "legend"
                                             },
+                                            yref: {
+                                                valType: "enumerated",
+                                                dflt: "paper",
+                                                values: ["container", "paper"],
+                                                editType: "layoutstyle"
+                                            },
                                             yanchor: {
                                                 valType: "enumerated",
                                                 values: ["auto", "top", "middle", "bottom"],
                                                 editType: "legend"
                                             },
                                             uirevision: {
                                                 valType: "any",
@@ -27303,21 +27356,40 @@
                                                     traceorder: _
                                                 }) ? "grouped+reversed" : "reversed"), void 0 !== v.legendgroup && "" !== v.legendgroup && (_ = u.isReversed({
                                                     traceorder: _
                                                 }) ? "reversed+grouped" : "grouped"));
                                                 var k = i.coerce(e, r, l, "showlegend", b && x > 1);
                                                 if (!1 === k && (r.legend = void 0), (!1 !== k || f.uirevision) && (p("uirevision", r.uirevision), !1 !== k)) {
                                                     p("borderwidth");
-                                                    var T, M, A, S = "h" === p("orientation");
-                                                    if (S ? (T = 0, n.getComponentMethod("rangeslider", "isVisible")(e.xaxis) ? (M = 1.1, A = "bottom") : (M = -.1, A = "top")) : (T = 1.02, M = 1, A = "auto"), p("traceorder", _), u.isGrouped(r.legend) && p("tracegroupgap"), p("entrywidth"), p("entrywidthmode"), p("itemsizing"), p("itemwidth"), p("itemclick"), p("itemdoubleclick"), p("groupclick"), p("x", T), p("xanchor"), p("y", M), p("yanchor", A), p("valign"), i.noneOrAll(f, h, ["x", "y"]), p("title.text")) {
+                                                    var T, M, A, S = "h" === p("orientation"),
+                                                        E = "paper" === p("yref"),
+                                                        C = "paper" === p("xref"),
+                                                        L = "left";
+                                                    if (S ? (T = 0, n.getComponentMethod("rangeslider", "isVisible")(e.xaxis) ? E ? (M = 1.1, A = "bottom") : (M = 1, A = "top") : E ? (M = -.1, A = "top") : (M = 0, A = "bottom")) : (M = 1, A = "auto", C ? T = 1.02 : (T = 1, L = "right")), i.coerce(f, h, {
+                                                            x: {
+                                                                valType: "number",
+                                                                editType: "legend",
+                                                                min: C ? -2 : 0,
+                                                                max: C ? 3 : 1,
+                                                                dflt: T
+                                                            }
+                                                        }, "x"), i.coerce(f, h, {
+                                                            y: {
+                                                                valType: "number",
+                                                                editType: "legend",
+                                                                min: E ? -2 : 0,
+                                                                max: E ? 3 : 1,
+                                                                dflt: M
+                                                            }
+                                                        }, "y"), p("traceorder", _), u.isGrouped(r.legend) && p("tracegroupgap"), p("entrywidth"), p("entrywidthmode"), p("itemsizing"), p("itemwidth"), p("itemclick"), p("itemdoubleclick"), p("groupclick"), p("xanchor", L), p("yanchor", A), p("valign"), i.noneOrAll(f, h, ["x", "y"]), p("title.text")) {
                                                         p("title.side", S ? "left" : "top");
-                                                        var E = i.extendFlat({}, d, {
+                                                        var P = i.extendFlat({}, d, {
                                                             size: i.bigFont(d.size)
                                                         });
-                                                        i.coerceFont(p, "title.font", E)
+                                                        i.coerceFont(p, "title.font", P)
                                                     }
                                                 }
                                             }
                                         }
                                         t.exports = function(t, e, r) {
                                             var n, a = ["legend"];
                                             for (n = 0; n < r.length; n++) i.pushUnique(a, r[n].legend);
@@ -27484,96 +27556,111 @@
                                                             c && "" !== a && (s = k[a]);
                                                             var h = Z ? g : M || s;
                                                             l || f || (h += v / 2), u.setRect(e, 0, -r / 2, h, r)
                                                         }))
                                                     }(t, N, j, f)
                                                 }, function() {
                                                     var e, s, c, m, x = h._size,
-                                                        b = f.borderwidth;
+                                                        b = f.borderwidth,
+                                                        _ = "paper" === f.xref,
+                                                        w = "paper" === f.yref;
                                                     if (!v) {
-                                                        var _ = function(t, e) {
-                                                            var r = t._fullLayout[e],
-                                                                n = L(r),
-                                                                i = P(r);
-                                                            return a.autoMargin(t, e, {
-                                                                x: r.x,
-                                                                y: r.y,
-                                                                l: r._width * g[n],
-                                                                r: r._width * y[n],
-                                                                b: r._effHeight * y[i],
-                                                                t: r._effHeight * g[i]
-                                                            })
-                                                        }(t, d);
-                                                        if (_) return;
-                                                        var w = x.l + x.w * f.x - g[L(f)] * f._width,
-                                                            k = x.t + x.h * (1 - f.y) - g[P(f)] * f._effHeight;
+                                                        var k, T;
+                                                        k = _ ? x.l + x.w * f.x - g[L(f)] * f._width : h.width * f.x - g[L(f)] * f._width, T = w ? x.t + x.h * (1 - f.y) - g[P(f)] * f._effHeight : h.height * (1 - f.y) - g[P(f)] * f._effHeight;
+                                                        var A = function(t, e, r, n) {
+                                                            var i = t._fullLayout,
+                                                                o = i[e],
+                                                                s = L(o),
+                                                                l = P(o),
+                                                                u = "paper" === o.xref,
+                                                                c = "paper" === o.yref;
+                                                            t._fullLayout._reservedMargin[e] = {};
+                                                            var f = o.y < .5 ? "b" : "t",
+                                                                h = o.x < .5 ? "l" : "r",
+                                                                p = {
+                                                                    r: i.width - r,
+                                                                    l: r + o._width,
+                                                                    b: i.height - n,
+                                                                    t: n + o._effHeight
+                                                                };
+                                                            if (u && c) return a.autoMargin(t, e, {
+                                                                x: o.x,
+                                                                y: o.y,
+                                                                l: o._width * g[s],
+                                                                r: o._width * y[s],
+                                                                b: o._effHeight * y[l],
+                                                                t: o._effHeight * g[l]
+                                                            });
+                                                            u ? t._fullLayout._reservedMargin[e][f] = p[f] : c || "v" === o.orientation ? t._fullLayout._reservedMargin[e][h] = p[h] : t._fullLayout._reservedMargin[e][f] = p[f]
+                                                        }(t, d, k, T);
+                                                        if (A) return;
                                                         if (h.margin.autoexpand) {
-                                                            var T = w,
-                                                                A = k;
-                                                            w = i.constrain(w, 0, h.width - f._width), k = i.constrain(k, 0, h.height - f._effHeight), w !== T && i.log("Constrain " + d + ".x to make legend fit inside graph"), k !== A && i.log("Constrain " + d + ".y to make legend fit inside graph")
+                                                            var E = k,
+                                                                C = T;
+                                                            k = _ ? i.constrain(k, 0, h.width - f._width) : E, T = w ? i.constrain(T, 0, h.height - f._effHeight) : C, k !== E && i.log("Constrain " + d + ".x to make legend fit inside graph"), T !== C && i.log("Constrain " + d + ".y to make legend fit inside graph")
                                                         }
-                                                        u.setTranslate(S, w, k)
+                                                        u.setTranslate(S, k, T)
                                                     }
                                                     if (B.on(".drag", null), S.on("wheel", null), v || f._height <= f._maxHeight || t._context.staticPlot) {
-                                                        var E = f._effHeight;
-                                                        v && (E = f._height), D.attr({
+                                                        var O = f._effHeight;
+                                                        v && (O = f._height), D.attr({
                                                             width: f._width - b,
-                                                            height: E - b,
+                                                            height: O - b,
                                                             x: b / 2,
                                                             y: b / 2
                                                         }), u.setTranslate(z, 0, 0), I.select("rect").attr({
                                                             width: f._width - 2 * b,
-                                                            height: E - 2 * b,
+                                                            height: O - 2 * b,
                                                             x: b,
                                                             y: b
                                                         }), u.setClipUrl(z, r, t), u.setRect(B, 0, 0, 0, 0), delete f._scrollY
                                                     } else {
-                                                        var C, O, R, F = Math.max(p.scrollBarMinHeight, f._effHeight * f._effHeight / f._height),
-                                                            j = f._effHeight - F - 2 * p.scrollBarMargin,
-                                                            U = f._height - f._effHeight,
-                                                            V = j / U,
-                                                            H = Math.min(f._scrollY || 0, U);
+                                                        var R, F, j, U = Math.max(p.scrollBarMinHeight, f._effHeight * f._effHeight / f._height),
+                                                            V = f._effHeight - U - 2 * p.scrollBarMargin,
+                                                            H = f._height - f._effHeight,
+                                                            q = V / H,
+                                                            G = Math.min(f._scrollY || 0, H);
                                                         D.attr({
                                                             width: f._width - 2 * b + p.scrollBarWidth + p.scrollBarMargin,
                                                             height: f._effHeight - b,
                                                             x: b / 2,
                                                             y: b / 2
                                                         }), I.select("rect").attr({
                                                             width: f._width - 2 * b + p.scrollBarWidth + p.scrollBarMargin,
                                                             height: f._effHeight - 2 * b,
                                                             x: b,
-                                                            y: b + H
-                                                        }), u.setClipUrl(z, r, t), Y(H, F, V), S.on("wheel", (function() {
-                                                            Y(H = i.constrain(f._scrollY + n.event.deltaY / j * U, 0, U), F, V), 0 !== H && H !== U && n.event.preventDefault()
+                                                            y: b + G
+                                                        }), u.setClipUrl(z, r, t), Z(G, U, q), S.on("wheel", (function() {
+                                                            Z(G = i.constrain(f._scrollY + n.event.deltaY / V * H, 0, H), U, q), 0 !== G && G !== H && n.event.preventDefault()
                                                         }));
-                                                        var q = n.behavior.drag().on("dragstart", (function() {
+                                                        var Y = n.behavior.drag().on("dragstart", (function() {
                                                             var t = n.event.sourceEvent;
-                                                            C = "touchstart" === t.type ? t.changedTouches[0].clientY : t.clientY, R = H
+                                                            R = "touchstart" === t.type ? t.changedTouches[0].clientY : t.clientY, j = G
                                                         })).on("drag", (function() {
                                                             var t = n.event.sourceEvent;
-                                                            2 === t.buttons || t.ctrlKey || (O = "touchmove" === t.type ? t.changedTouches[0].clientY : t.clientY, H = function(t, e, r) {
-                                                                var n = (r - e) / V + t;
-                                                                return i.constrain(n, 0, U)
-                                                            }(R, C, O), Y(H, F, V))
+                                                            2 === t.buttons || t.ctrlKey || (F = "touchmove" === t.type ? t.changedTouches[0].clientY : t.clientY, G = function(t, e, r) {
+                                                                var n = (r - e) / q + t;
+                                                                return i.constrain(n, 0, H)
+                                                            }(j, R, F), Z(G, U, q))
                                                         }));
-                                                        B.call(q);
-                                                        var G = n.behavior.drag().on("dragstart", (function() {
+                                                        B.call(Y);
+                                                        var W = n.behavior.drag().on("dragstart", (function() {
                                                             var t = n.event.sourceEvent;
-                                                            "touchstart" === t.type && (C = t.changedTouches[0].clientY, R = H)
+                                                            "touchstart" === t.type && (R = t.changedTouches[0].clientY, j = G)
                                                         })).on("drag", (function() {
                                                             var t = n.event.sourceEvent;
-                                                            "touchmove" === t.type && (O = t.changedTouches[0].clientY, H = function(t, e, r) {
-                                                                var n = (e - r) / V + t;
-                                                                return i.constrain(n, 0, U)
-                                                            }(R, C, O), Y(H, F, V))
+                                                            "touchmove" === t.type && (F = t.changedTouches[0].clientY, G = function(t, e, r) {
+                                                                var n = (e - r) / q + t;
+                                                                return i.constrain(n, 0, H)
+                                                            }(j, R, F), Z(G, U, q))
                                                         }));
-                                                        z.call(G)
+                                                        z.call(W)
                                                     }
 
-                                                    function Y(e, r, n) {
+                                                    function Z(e, r, n) {
                                                         f._scrollY = t._fullLayout[d]._scrollY = e, u.setTranslate(z, 0, -e), u.setRect(B, f._width, p.scrollBarMargin + e * n, p.scrollBarWidth, r), I.select("rect").attr("y", b + e)
                                                     }
                                                     t._context.edits.legendPosition && (S.classed("cursor-move", !0), l.init({
                                                         element: S.node(),
                                                         gd: t,
                                                         prepFn: function() {
                                                             var t = u.getTranslate(S);
@@ -34229,14 +34316,28 @@
                                             ONESEC: 1e3,
                                             EPOCHJD: 2440587.5,
                                             ALMOST_EQUAL: .999999,
                                             LOG_CLIP: 10,
                                             MINUS_SIGN: "−"
                                         }
                                     },
+                                    32396: function(t, e) {
+                                        "use strict";
+                                        e.CSS_DECLARATIONS = [
+                                            ["image-rendering", "optimizeSpeed"],
+                                            ["image-rendering", "-moz-crisp-edges"],
+                                            ["image-rendering", "-o-crisp-edges"],
+                                            ["image-rendering", "-webkit-optimize-contrast"],
+                                            ["image-rendering", "optimize-contrast"],
+                                            ["image-rendering", "crisp-edges"],
+                                            ["image-rendering", "pixelated"]
+                                        ], e.STYLE = e.CSS_DECLARATIONS.map((function(t) {
+                                            return t.join(": ") + "; "
+                                        })).join("")
+                                    },
                                     77922: function(t, e) {
                                         "use strict";
                                         e.xmlns = "http://www.w3.org/2000/xmlns/", e.svg = "http://www.w3.org/2000/svg", e.xlink = "http://www.w3.org/1999/xlink", e.svgAttrs = {
                                             xmlns: e.svg,
                                             "xmlns:xlink": e.xlink
                                         }
                                     },
@@ -36793,14 +36894,41 @@
                                     78614: function(t, e, r) {
                                         "use strict";
                                         var n = r(25075);
                                         t.exports = function(t) {
                                             return t ? n(t) : [0, 0, 0, 1]
                                         }
                                     },
+                                    3883: function(t, e, r) {
+                                        "use strict";
+                                        var n = r(32396),
+                                            i = r(91424),
+                                            a = r(71828),
+                                            o = null;
+                                        t.exports = function() {
+                                            if (null !== o) return o;
+                                            if (a.isIE()) o = !1;
+                                            else {
+                                                var t = Array.from(n.CSS_DECLARATIONS).reverse(),
+                                                    e = window.CSS && window.CSS.supports || window.supportsCSS;
+                                                if ("function" == typeof e) o = t.some((function(t) {
+                                                    return e.apply(null, t)
+                                                }));
+                                                else {
+                                                    var r = i.tester.append("image"),
+                                                        s = window.getComputedStyle(r.node());
+                                                    r.attr("style", n.STYLE), o = t.some((function(t) {
+                                                        var e = t[1];
+                                                        return s.imageRendering === e || s.imageRendering === e.toLowerCase()
+                                                    })), r.remove()
+                                                }
+                                            }
+                                            return o
+                                        }
+                                    },
                                     63893: function(t, e, r) {
                                         "use strict";
                                         var n = r(39898),
                                             i = r(71828),
                                             a = i.strTranslate,
                                             o = r(77922),
                                             s = r(18783).LINE_SPACING,
@@ -61456,67 +61584,55 @@
                                                 var O = e.z;
                                                 i.isArray1D(O) ? (u(e, A, S, "x", "y", ["z"]), r = e._x, x = e._y, O = e._z) : (m = e.x ? A.makeCalcdata(e, "x") : [], w = e.y ? S.makeCalcdata(e, "y") : [], r = o(e, A, "x", m).vals, x = o(e, S, "y", w).vals, e._x = r, e._y = x), g = e.x0, y = e.dx, b = e.y0, _ = e.dy, k = c(O, e, A, S)
                                             }
 
                                             function I(t) {
                                                 P = e._input.zsmooth = e.zsmooth = !1, i.warn('cannot use zsmooth: "fast": ' + t)
                                             }
-                                            if ((A.rangebreaks || S.rangebreaks) && (k = function(t, e, r) {
-                                                    for (var n = [], i = -1, a = 0; a < r.length; a++)
-                                                        if (e[a] !== d) {
-                                                            n[++i] = [];
-                                                            for (var o = 0; o < r[a].length; o++) t[o] !== d && n[i].push(r[a][o])
-                                                        } return n
-                                                }(r, x, k), C || (r = v(r), x = v(x), e._x = r, e._y = x)), C || !E && !e.connectgaps || (e._emptypoints = h(k), f(k, e._emptypoints)), "fast" === P)
-                                                if ("log" === A.type || "log" === S.type) I("log axis found");
-                                                else if (!C) {
-                                                if (r.length) {
-                                                    var D = (r[r.length - 1] - r[0]) / (r.length - 1),
-                                                        z = Math.abs(D / 100);
-                                                    for (T = 0; T < r.length - 1; T++)
-                                                        if (Math.abs(r[T + 1] - r[T] - D) > z) {
-                                                            I("x scale is not linear");
-                                                            break
-                                                        }
-                                                }
-                                                if (x.length && "fast" === P) {
-                                                    var R = (x[x.length - 1] - x[0]) / (x.length - 1),
-                                                        F = Math.abs(R / 100);
-                                                    for (T = 0; T < x.length - 1; T++)
-                                                        if (Math.abs(x[T + 1] - x[T] - R) > F) {
-                                                            I("y scale is not linear");
-                                                            break
-                                                        }
+
+                                            function D(t) {
+                                                if (t.length > 1) {
+                                                    var e = (t[t.length - 1] - t[0]) / (t.length - 1),
+                                                        r = Math.abs(e / 100);
+                                                    for (T = 0; T < t.length - 1; T++)
+                                                        if (Math.abs(t[T + 1] - t[T] - e) > r) return !1
                                                 }
-                                            }
-                                            var B = i.maxRowLength(k),
-                                                N = "scaled" === e.xtype ? "" : r,
-                                                j = p(e, N, g, y, B, A),
-                                                U = "scaled" === e.ytype ? "" : x,
-                                                V = p(e, U, b, _, k.length, S);
-                                            L || (e._extremes[A._id] = a.findExtremes(A, j), e._extremes[S._id] = a.findExtremes(S, V));
-                                            var H = {
-                                                x: j,
-                                                y: V,
+                                                return !0
+                                            }(A.rangebreaks || S.rangebreaks) && (k = function(t, e, r) {
+                                                for (var n = [], i = -1, a = 0; a < r.length; a++)
+                                                    if (e[a] !== d) {
+                                                        n[++i] = [];
+                                                        for (var o = 0; o < r[a].length; o++) t[o] !== d && n[i].push(r[a][o])
+                                                    } return n
+                                            }(r, x, k), C || (r = v(r), x = v(x), e._x = r, e._y = x)), C || !E && !e.connectgaps || (e._emptypoints = h(k), f(k, e._emptypoints)), e._islinear = !1, "log" === A.type || "log" === S.type ? "fast" === P && I("log axis found") : D(r) ? D(x) ? e._islinear = !0 : "fast" === P && I("y scale is not linear") : "fast" === P && I("x scale is not linear");
+                                            var z = i.maxRowLength(k),
+                                                R = "scaled" === e.xtype ? "" : r,
+                                                F = p(e, R, g, y, z, A),
+                                                B = "scaled" === e.ytype ? "" : x,
+                                                N = p(e, B, b, _, k.length, S);
+                                            L || (e._extremes[A._id] = a.findExtremes(A, F), e._extremes[S._id] = a.findExtremes(S, N));
+                                            var j = {
+                                                x: F,
+                                                y: N,
                                                 z: k,
                                                 text: e._text || e.text,
                                                 hovertext: e._hovertext || e.hovertext
                                             };
-                                            if (e.xperiodalignment && m && (H.orig_x = m), e.yperiodalignment && w && (H.orig_y = w), N && N.length === j.length - 1 && (H.xCenter = N), U && U.length === V.length - 1 && (H.yCenter = U), C && (H.xRanges = M.xRanges, H.yRanges = M.yRanges, H.pts = M.pts), E || l(t, e, {
+                                            if (e.xperiodalignment && m && (j.orig_x = m), e.yperiodalignment && w && (j.orig_y = w), R && R.length === F.length - 1 && (j.xCenter = R), B && B.length === N.length - 1 && (j.yCenter = B), C && (j.xRanges = M.xRanges, j.yRanges = M.yRanges, j.pts = M.pts), E || l(t, e, {
                                                     vals: k,
                                                     cLetter: "z"
                                                 }), E && e.contours && "heatmap" === e.contours.coloring) {
-                                                var q = {
+                                                var U = {
                                                     type: "contour" === e.type ? "heatmap" : "histogram2d",
                                                     xcalendar: e.xcalendar,
                                                     ycalendar: e.ycalendar
                                                 };
-                                                H.xfill = p(q, N, g, y, B, A), H.yfill = p(q, U, b, _, k.length, S)
+                                                j.xfill = p(U, R, g, y, z, A), j.yfill = p(U, B, b, _, k.length, S)
                                             }
-                                            return [H]
+                                            return [j]
                                         }
                                     },
                                     4742: function(t, e, r) {
                                         "use strict";
                                         var n = r(92770),
                                             i = r(71828),
                                             a = r(50606).BADNUM;
@@ -61829,25 +61945,27 @@
                                             u = r(63893),
                                             c = r(8225),
                                             f = r(7901),
                                             h = r(21081).extractOpts,
                                             p = r(21081).makeColorScaleFuncFromTrace,
                                             d = r(77922),
                                             v = r(18783).LINE_SPACING,
-                                            g = "heatmap-label";
+                                            g = r(3883),
+                                            y = r(32396).STYLE,
+                                            m = "heatmap-label";
 
-                                        function y(t) {
-                                            return t.selectAll("g." + g)
+                                        function x(t) {
+                                            return t.selectAll("g." + m)
                                         }
 
-                                        function m(t) {
-                                            y(t).remove()
+                                        function b(t) {
+                                            x(t).remove()
                                         }
 
-                                        function x(t, e) {
+                                        function _(t, e) {
                                             var r = e.length - 2,
                                                 n = l.constrain(l.findBin(t, e), 0, r),
                                                 i = e[n],
                                                 a = e[n + 1],
                                                 o = l.constrain(n + (t - i) / (a - i) - .5, 0, r),
                                                 s = Math.round(o),
                                                 u = Math.abs(o - s);
@@ -61858,15 +61976,15 @@
                                             } : {
                                                 bin0: s,
                                                 bin1: s,
                                                 frac: 0
                                             }
                                         }
 
-                                        function b(t, e) {
+                                        function w(t, e) {
                                             var r = e.length - 1,
                                                 n = l.constrain(l.findBin(t, e), 0, r),
                                                 i = e[n],
                                                 a = (t - i) / (e[n + 1] - i) || 0;
                                             return a <= 0 ? {
                                                 bin0: n,
                                                 bin1: n,
@@ -61878,242 +61996,244 @@
                                             } : {
                                                 bin0: n + 1,
                                                 bin1: n,
                                                 frac: 1 - a
                                             }
                                         }
 
-                                        function _(t, e, r) {
+                                        function k(t, e, r) {
                                             t[e] = r[0], t[e + 1] = r[1], t[e + 2] = r[2], t[e + 3] = Math.round(255 * r[3])
                                         }
-                                        t.exports = function(t, e, r, w) {
-                                            var k = e.xaxis,
-                                                T = e.yaxis;
-                                            l.makeTraceGroups(w, r, "hm").each((function(e) {
-                                                var r, w, M, A, S, E, C, L, P = n.select(this),
-                                                    O = e[0],
-                                                    I = O.trace,
-                                                    D = I.xgap || 0,
-                                                    z = I.ygap || 0,
-                                                    R = O.z,
-                                                    F = O.x,
-                                                    B = O.y,
-                                                    N = O.xCenter,
-                                                    j = O.yCenter,
-                                                    U = a.traceIs(I, "contour"),
-                                                    V = U ? "best" : I.zsmooth,
-                                                    H = R.length,
-                                                    q = l.maxRowLength(R),
-                                                    G = !1,
-                                                    Y = !1;
-                                                for (E = 0; void 0 === r && E < F.length - 1;) r = k.c2p(F[E]), E++;
-                                                for (E = F.length - 1; void 0 === w && E > 0;) w = k.c2p(F[E]), E--;
-                                                for (w < r && (M = w, w = r, r = M, G = !0), E = 0; void 0 === A && E < B.length - 1;) A = T.c2p(B[E]), E++;
-                                                for (E = B.length - 1; void 0 === S && E > 0;) S = T.c2p(B[E]), E--;
-                                                if (S < A && (M = A, A = S, S = M, Y = !0), U && (N = F, j = B, F = O.xfill, B = O.yfill), "fast" !== V) {
-                                                    var W = "best" === V ? 0 : .5;
-                                                    r = Math.max(-W * k._length, r), w = Math.min((1 + W) * k._length, w), A = Math.max(-W * T._length, A), S = Math.min((1 + W) * T._length, S)
-                                                }
-                                                var Z, X, K = Math.round(w - r),
-                                                    J = Math.round(S - A);
-                                                if (K <= 0 || J <= 0) return P.selectAll("image").data([]).exit().remove(), void m(P);
-                                                "fast" === V ? (Z = q, X = H) : (Z = K, X = J);
-                                                var $ = document.createElement("canvas");
-                                                $.width = Z, $.height = X;
-                                                var Q, tt, et = $.getContext("2d"),
-                                                    rt = p(I, {
+                                        t.exports = function(t, e, r, T) {
+                                            var M = e.xaxis,
+                                                A = e.yaxis;
+                                            l.makeTraceGroups(T, r, "hm").each((function(e) {
+                                                var r, T, S, E, C, L, P, O, I = n.select(this),
+                                                    D = e[0],
+                                                    z = D.trace,
+                                                    R = z.xgap || 0,
+                                                    F = z.ygap || 0,
+                                                    B = D.z,
+                                                    N = D.x,
+                                                    j = D.y,
+                                                    U = D.xCenter,
+                                                    V = D.yCenter,
+                                                    H = a.traceIs(z, "contour"),
+                                                    q = H ? "best" : z.zsmooth,
+                                                    G = B.length,
+                                                    Y = l.maxRowLength(B),
+                                                    W = !1,
+                                                    Z = !1;
+                                                for (L = 0; void 0 === r && L < N.length - 1;) r = M.c2p(N[L]), L++;
+                                                for (L = N.length - 1; void 0 === T && L > 0;) T = M.c2p(N[L]), L--;
+                                                for (T < r && (S = T, T = r, r = S, W = !0), L = 0; void 0 === E && L < j.length - 1;) E = A.c2p(j[L]), L++;
+                                                for (L = j.length - 1; void 0 === C && L > 0;) C = A.c2p(j[L]), L--;
+                                                C < E && (S = E, E = C, C = S, Z = !0), H && (U = N, V = j, N = D.xfill, j = D.yfill);
+                                                var X = "default";
+                                                if (q ? X = "best" === q ? "smooth" : "fast" : z._islinear && 0 === R && 0 === F && g() && (X = "fast"), "fast" !== X) {
+                                                    var K = "best" === q ? 0 : .5;
+                                                    r = Math.max(-K * M._length, r), T = Math.min((1 + K) * M._length, T), E = Math.max(-K * A._length, E), C = Math.min((1 + K) * A._length, C)
+                                                }
+                                                var J, $, Q = Math.round(T - r),
+                                                    tt = Math.round(C - E);
+                                                if (r >= M._length || T <= 0 || E >= A._length || C <= 0) return I.selectAll("image").data([]).exit().remove(), void b(I);
+                                                "fast" === X ? (J = Y, $ = G) : (J = Q, $ = tt);
+                                                var et = document.createElement("canvas");
+                                                et.width = J, et.height = $;
+                                                var rt, nt, it = et.getContext("2d"),
+                                                    at = p(z, {
                                                         noNumericCheck: !0,
                                                         returnArray: !0
                                                     });
-                                                "fast" === V ? (Q = G ? function(t) {
-                                                    return q - 1 - t
-                                                } : l.identity, tt = Y ? function(t) {
-                                                    return H - 1 - t
-                                                } : l.identity) : (Q = function(t) {
-                                                    return l.constrain(Math.round(k.c2p(F[t]) - r), 0, K)
-                                                }, tt = function(t) {
-                                                    return l.constrain(Math.round(T.c2p(B[t]) - A), 0, J)
+                                                "fast" === X ? (rt = W ? function(t) {
+                                                    return Y - 1 - t
+                                                } : l.identity, nt = Z ? function(t) {
+                                                    return G - 1 - t
+                                                } : l.identity) : (rt = function(t) {
+                                                    return l.constrain(Math.round(M.c2p(N[t]) - r), 0, Q)
+                                                }, nt = function(t) {
+                                                    return l.constrain(Math.round(A.c2p(j[t]) - E), 0, tt)
                                                 });
-                                                var nt, it, at, ot, st = tt(0),
-                                                    lt = [st, st],
-                                                    ut = G ? 0 : 1,
-                                                    ct = Y ? 0 : 1,
-                                                    ft = 0,
-                                                    ht = 0,
-                                                    pt = 0,
-                                                    dt = 0;
+                                                var ot, st, lt, ut, ct = nt(0),
+                                                    ft = [ct, ct],
+                                                    ht = W ? 0 : 1,
+                                                    pt = Z ? 0 : 1,
+                                                    dt = 0,
+                                                    vt = 0,
+                                                    gt = 0,
+                                                    yt = 0;
 
-                                                function vt(t, e) {
+                                                function mt(t, e) {
                                                     if (void 0 !== t) {
-                                                        var r = rt(t);
-                                                        return r[0] = Math.round(r[0]), r[1] = Math.round(r[1]), r[2] = Math.round(r[2]), ft += e, ht += r[0] * e, pt += r[1] * e, dt += r[2] * e, r
+                                                        var r = at(t);
+                                                        return r[0] = Math.round(r[0]), r[1] = Math.round(r[1]), r[2] = Math.round(r[2]), dt += e, vt += r[0] * e, gt += r[1] * e, yt += r[2] * e, r
                                                     }
                                                     return [0, 0, 0, 0]
                                                 }
 
-                                                function gt(t, e, r, n) {
+                                                function xt(t, e, r, n) {
                                                     var i = t[r.bin0];
-                                                    if (void 0 === i) return vt(void 0, 1);
+                                                    if (void 0 === i) return mt(void 0, 1);
                                                     var a, o = t[r.bin1],
                                                         s = e[r.bin0],
                                                         l = e[r.bin1],
                                                         u = o - i || 0,
                                                         c = s - i || 0;
-                                                    return a = void 0 === o ? void 0 === l ? 0 : void 0 === s ? 2 * (l - i) : 2 * (2 * l - s - i) / 3 : void 0 === l ? void 0 === s ? 0 : 2 * (2 * i - o - s) / 3 : void 0 === s ? 2 * (2 * l - o - i) / 3 : l + i - o - s, vt(i + r.frac * u + n.frac * (c + r.frac * a))
+                                                    return a = void 0 === o ? void 0 === l ? 0 : void 0 === s ? 2 * (l - i) : 2 * (2 * l - s - i) / 3 : void 0 === l ? void 0 === s ? 0 : 2 * (2 * i - o - s) / 3 : void 0 === s ? 2 * (2 * l - o - i) / 3 : l + i - o - s, mt(i + r.frac * u + n.frac * (c + r.frac * a))
                                                 }
-                                                if (V) {
-                                                    var yt, mt = 0;
+                                                if ("default" !== X) {
+                                                    var bt, _t = 0;
                                                     try {
-                                                        yt = new Uint8Array(Z * X * 4)
+                                                        bt = new Uint8Array(J * $ * 4)
                                                     } catch (t) {
-                                                        yt = new Array(Z * X * 4)
+                                                        bt = new Array(J * $ * 4)
                                                     }
-                                                    if ("best" === V) {
-                                                        var xt, bt, _t, wt = N || F,
-                                                            kt = j || B,
-                                                            Tt = new Array(wt.length),
-                                                            Mt = new Array(kt.length),
-                                                            At = new Array(K),
-                                                            St = N ? b : x,
-                                                            Et = j ? b : x;
-                                                        for (E = 0; E < wt.length; E++) Tt[E] = Math.round(k.c2p(wt[E]) - r);
-                                                        for (E = 0; E < kt.length; E++) Mt[E] = Math.round(T.c2p(kt[E]) - A);
-                                                        for (E = 0; E < K; E++) At[E] = St(E, Tt);
-                                                        for (C = 0; C < J; C++)
-                                                            for (bt = R[(xt = Et(C, Mt)).bin0], _t = R[xt.bin1], E = 0; E < K; E++, mt += 4) _(yt, mt, ot = gt(bt, _t, At[E], xt))
+                                                    if ("smooth" === X) {
+                                                        var wt, kt, Tt, Mt = U || N,
+                                                            At = V || j,
+                                                            St = new Array(Mt.length),
+                                                            Et = new Array(At.length),
+                                                            Ct = new Array(Q),
+                                                            Lt = U ? w : _,
+                                                            Pt = V ? w : _;
+                                                        for (L = 0; L < Mt.length; L++) St[L] = Math.round(M.c2p(Mt[L]) - r);
+                                                        for (L = 0; L < At.length; L++) Et[L] = Math.round(A.c2p(At[L]) - E);
+                                                        for (L = 0; L < Q; L++) Ct[L] = Lt(L, St);
+                                                        for (P = 0; P < tt; P++)
+                                                            for (kt = B[(wt = Pt(P, Et)).bin0], Tt = B[wt.bin1], L = 0; L < Q; L++, _t += 4) k(bt, _t, ut = xt(kt, Tt, Ct[L], wt))
                                                     } else
-                                                        for (C = 0; C < H; C++)
-                                                            for (at = R[C], lt = tt(C), E = 0; E < q; E++) ot = vt(at[E], 1), _(yt, mt = 4 * (lt * q + Q(E)), ot);
-                                                    var Ct = et.createImageData(Z, X);
+                                                        for (P = 0; P < G; P++)
+                                                            for (lt = B[P], ft = nt(P), L = 0; L < Y; L++) ut = mt(lt[L], 1), k(bt, _t = 4 * (ft * Y + rt(L)), ut);
+                                                    var Ot = it.createImageData(J, $);
                                                     try {
-                                                        Ct.data.set(yt)
+                                                        Ot.data.set(bt)
                                                     } catch (t) {
-                                                        var Lt = Ct.data,
-                                                            Pt = Lt.length;
-                                                        for (C = 0; C < Pt; C++) Lt[C] = yt[C]
+                                                        var It = Ot.data,
+                                                            Dt = It.length;
+                                                        for (P = 0; P < Dt; P++) It[P] = bt[P]
                                                     }
-                                                    et.putImageData(Ct, 0, 0)
+                                                    it.putImageData(Ot, 0, 0)
                                                 } else {
-                                                    var Ot = Math.floor(D / 2),
-                                                        It = Math.floor(z / 2);
-                                                    for (C = 0; C < H; C++)
-                                                        if (at = R[C], lt.reverse(), lt[ct] = tt(C + 1), lt[0] !== lt[1] && void 0 !== lt[0] && void 0 !== lt[1])
-                                                            for (nt = [it = Q(0), it], E = 0; E < q; E++) nt.reverse(), nt[ut] = Q(E + 1), nt[0] !== nt[1] && void 0 !== nt[0] && void 0 !== nt[1] && (ot = vt(at[E], (nt[1] - nt[0]) * (lt[1] - lt[0])), et.fillStyle = "rgba(" + ot.join(",") + ")", et.fillRect(nt[0] + Ot, lt[0] + It, nt[1] - nt[0] - D, lt[1] - lt[0] - z))
-                                                }
-                                                ht = Math.round(ht / ft), pt = Math.round(pt / ft), dt = Math.round(dt / ft);
-                                                var Dt = i("rgb(" + ht + "," + pt + "," + dt + ")");
-                                                t._hmpixcount = (t._hmpixcount || 0) + ft, t._hmlumcount = (t._hmlumcount || 0) + ft * Dt.getLuminance();
-                                                var zt = P.selectAll("image").data(e);
-                                                zt.enter().append("svg:image").attr({
+                                                    var zt = Math.floor(R / 2),
+                                                        Rt = Math.floor(F / 2);
+                                                    for (P = 0; P < G; P++)
+                                                        if (lt = B[P], ft.reverse(), ft[pt] = nt(P + 1), ft[0] !== ft[1] && void 0 !== ft[0] && void 0 !== ft[1])
+                                                            for (ot = [st = rt(0), st], L = 0; L < Y; L++) ot.reverse(), ot[ht] = rt(L + 1), ot[0] !== ot[1] && void 0 !== ot[0] && void 0 !== ot[1] && (ut = mt(lt[L], (ot[1] - ot[0]) * (ft[1] - ft[0])), it.fillStyle = "rgba(" + ut.join(",") + ")", it.fillRect(ot[0] + zt, ft[0] + Rt, ot[1] - ot[0] - R, ft[1] - ft[0] - F))
+                                                }
+                                                vt = Math.round(vt / dt), gt = Math.round(gt / dt), yt = Math.round(yt / dt);
+                                                var Ft = i("rgb(" + vt + "," + gt + "," + yt + ")");
+                                                t._hmpixcount = (t._hmpixcount || 0) + dt, t._hmlumcount = (t._hmlumcount || 0) + dt * Ft.getLuminance();
+                                                var Bt = I.selectAll("image").data(e);
+                                                Bt.enter().append("svg:image").attr({
                                                     xmlns: d.svg,
                                                     preserveAspectRatio: "none"
-                                                }), zt.attr({
-                                                    height: J,
-                                                    width: K,
+                                                }), Bt.attr({
+                                                    height: tt,
+                                                    width: Q,
                                                     x: r,
-                                                    y: A,
-                                                    "xlink:href": $.toDataURL("image/png")
-                                                }), m(P);
-                                                var Rt = I.texttemplate;
-                                                if (Rt) {
-                                                    var Ft = h(I),
-                                                        Bt = {
+                                                    y: E,
+                                                    "xlink:href": et.toDataURL("image/png")
+                                                }), "fast" !== X || q || Bt.attr("style", y), b(I);
+                                                var Nt = z.texttemplate;
+                                                if (Nt) {
+                                                    var jt = h(z),
+                                                        Ut = {
                                                             type: "linear",
-                                                            range: [Ft.min, Ft.max],
-                                                            _separators: k._separators,
-                                                            _numFormat: k._numFormat
+                                                            range: [jt.min, jt.max],
+                                                            _separators: M._separators,
+                                                            _numFormat: M._numFormat
                                                         },
-                                                        Nt = "histogram2dcontour" === I.type,
-                                                        jt = "contour" === I.type,
-                                                        Ut = jt ? H - 1 : H,
-                                                        Vt = jt ? 1 : 0,
-                                                        Ht = jt ? q - 1 : q,
-                                                        qt = [];
-                                                    for (E = jt ? 1 : 0; E < Ut; E++) {
-                                                        var Gt;
-                                                        if (jt) Gt = O.y[E];
-                                                        else if (Nt) {
-                                                            if (0 === E || E === H - 1) continue;
-                                                            Gt = O.y[E]
-                                                        } else if (O.yCenter) Gt = O.yCenter[E];
+                                                        Vt = "histogram2dcontour" === z.type,
+                                                        Ht = "contour" === z.type,
+                                                        qt = Ht ? G - 1 : G,
+                                                        Gt = Ht ? 1 : 0,
+                                                        Yt = Ht ? Y - 1 : Y,
+                                                        Wt = [];
+                                                    for (L = Ht ? 1 : 0; L < qt; L++) {
+                                                        var Zt;
+                                                        if (Ht) Zt = D.y[L];
+                                                        else if (Vt) {
+                                                            if (0 === L || L === G - 1) continue;
+                                                            Zt = D.y[L]
+                                                        } else if (D.yCenter) Zt = D.yCenter[L];
                                                         else {
-                                                            if (E + 1 === H && void 0 === O.y[E + 1]) continue;
-                                                            Gt = (O.y[E] + O.y[E + 1]) / 2
+                                                            if (L + 1 === G && void 0 === D.y[L + 1]) continue;
+                                                            Zt = (D.y[L] + D.y[L + 1]) / 2
                                                         }
-                                                        var Yt = Math.round(T.c2p(Gt));
-                                                        if (!(0 > Yt || Yt > T._length))
-                                                            for (C = Vt; C < Ht; C++) {
-                                                                var Wt;
-                                                                if (jt) Wt = O.x[C];
-                                                                else if (Nt) {
-                                                                    if (0 === C || C === q - 1) continue;
-                                                                    Wt = O.x[C]
-                                                                } else if (O.xCenter) Wt = O.xCenter[C];
+                                                        var Xt = Math.round(A.c2p(Zt));
+                                                        if (!(0 > Xt || Xt > A._length))
+                                                            for (P = Gt; P < Yt; P++) {
+                                                                var Kt;
+                                                                if (Ht) Kt = D.x[P];
+                                                                else if (Vt) {
+                                                                    if (0 === P || P === Y - 1) continue;
+                                                                    Kt = D.x[P]
+                                                                } else if (D.xCenter) Kt = D.xCenter[P];
                                                                 else {
-                                                                    if (C + 1 === q && void 0 === O.x[C + 1]) continue;
-                                                                    Wt = (O.x[C] + O.x[C + 1]) / 2
+                                                                    if (P + 1 === Y && void 0 === D.x[P + 1]) continue;
+                                                                    Kt = (D.x[P] + D.x[P + 1]) / 2
                                                                 }
-                                                                var Zt = Math.round(k.c2p(Wt));
-                                                                if (!(0 > Zt || Zt > k._length)) {
-                                                                    var Xt = c({
-                                                                        x: Wt,
-                                                                        y: Gt
-                                                                    }, I, t._fullLayout);
-                                                                    Xt.x = Wt, Xt.y = Gt;
-                                                                    var Kt = O.z[E][C];
-                                                                    void 0 === Kt ? (Xt.z = "", Xt.zLabel = "") : (Xt.z = Kt, Xt.zLabel = s.tickText(Bt, Kt, "hover").text);
-                                                                    var Jt = O.text && O.text[E] && O.text[E][C];
-                                                                    void 0 !== Jt && !1 !== Jt || (Jt = ""), Xt.text = Jt;
-                                                                    var $t = l.texttemplateString(Rt, Xt, t._fullLayout._d3locale, Xt, I._meta || {});
-                                                                    if ($t) {
-                                                                        var Qt = $t.split("<br>"),
-                                                                            te = Qt.length,
-                                                                            ee = 0;
-                                                                        for (L = 0; L < te; L++) ee = Math.max(ee, Qt[L].length);
-                                                                        qt.push({
-                                                                            l: te,
-                                                                            c: ee,
-                                                                            t: $t,
-                                                                            x: Zt,
-                                                                            y: Yt,
-                                                                            z: Kt
+                                                                var Jt = Math.round(M.c2p(Kt));
+                                                                if (!(0 > Jt || Jt > M._length)) {
+                                                                    var $t = c({
+                                                                        x: Kt,
+                                                                        y: Zt
+                                                                    }, z, t._fullLayout);
+                                                                    $t.x = Kt, $t.y = Zt;
+                                                                    var Qt = D.z[L][P];
+                                                                    void 0 === Qt ? ($t.z = "", $t.zLabel = "") : ($t.z = Qt, $t.zLabel = s.tickText(Ut, Qt, "hover").text);
+                                                                    var te = D.text && D.text[L] && D.text[L][P];
+                                                                    void 0 !== te && !1 !== te || (te = ""), $t.text = te;
+                                                                    var ee = l.texttemplateString(Nt, $t, t._fullLayout._d3locale, $t, z._meta || {});
+                                                                    if (ee) {
+                                                                        var re = ee.split("<br>"),
+                                                                            ne = re.length,
+                                                                            ie = 0;
+                                                                        for (O = 0; O < ne; O++) ie = Math.max(ie, re[O].length);
+                                                                        Wt.push({
+                                                                            l: ne,
+                                                                            c: ie,
+                                                                            t: ee,
+                                                                            x: Jt,
+                                                                            y: Xt,
+                                                                            z: Qt
                                                                         })
                                                                     }
                                                                 }
                                                             }
                                                     }
-                                                    var re = I.textfont,
-                                                        ne = re.family,
-                                                        ie = re.size,
-                                                        ae = t._fullLayout.font.size;
-                                                    if (!ie || "auto" === ie) {
-                                                        var oe = 1 / 0,
-                                                            se = 1 / 0,
-                                                            le = 0,
-                                                            ue = 0;
-                                                        for (L = 0; L < qt.length; L++) {
-                                                            var ce = qt[L];
-                                                            if (le = Math.max(le, ce.l), ue = Math.max(ue, ce.c), L < qt.length - 1) {
-                                                                var fe = qt[L + 1],
-                                                                    he = Math.abs(fe.x - ce.x),
-                                                                    pe = Math.abs(fe.y - ce.y);
-                                                                he && (oe = Math.min(oe, he)), pe && (se = Math.min(se, pe))
+                                                    var ae = z.textfont,
+                                                        oe = ae.family,
+                                                        se = ae.size,
+                                                        le = t._fullLayout.font.size;
+                                                    if (!se || "auto" === se) {
+                                                        var ue = 1 / 0,
+                                                            ce = 1 / 0,
+                                                            fe = 0,
+                                                            he = 0;
+                                                        for (O = 0; O < Wt.length; O++) {
+                                                            var pe = Wt[O];
+                                                            if (fe = Math.max(fe, pe.l), he = Math.max(he, pe.c), O < Wt.length - 1) {
+                                                                var de = Wt[O + 1],
+                                                                    ve = Math.abs(de.x - pe.x),
+                                                                    ge = Math.abs(de.y - pe.y);
+                                                                ve && (ue = Math.min(ue, ve)), ge && (ce = Math.min(ce, ge))
                                                             }
                                                         }
-                                                        isFinite(oe) && isFinite(se) ? (oe -= D, se -= z, oe /= ue, se /= le, oe /= v / 2, se /= v, ie = Math.min(Math.floor(oe), Math.floor(se), ae)) : ie = ae
+                                                        isFinite(ue) && isFinite(ce) ? (ue -= R, ce -= F, ue /= he, ce /= fe, ue /= v / 2, ce /= v, se = Math.min(Math.floor(ue), Math.floor(ce), le)) : se = le
                                                     }
-                                                    if (ie <= 0 || !isFinite(ie)) return;
-                                                    y(P).data(qt).enter().append("g").classed(g, 1).append("text").attr("text-anchor", "middle").each((function(e) {
+                                                    if (se <= 0 || !isFinite(se)) return;
+                                                    x(I).data(Wt).enter().append("g").classed(m, 1).append("text").attr("text-anchor", "middle").each((function(e) {
                                                         var r = n.select(this),
-                                                            i = re.color;
-                                                        i && "auto" !== i || (i = f.contrast("rgba(" + rt(e.z).join() + ")")), r.attr("data-notex", 1).call(u.positionText, function(t) {
+                                                            i = ae.color;
+                                                        i && "auto" !== i || (i = f.contrast("rgba(" + at(e.z).join() + ")")), r.attr("data-notex", 1).call(u.positionText, function(t) {
                                                             return t.x
                                                         }(e), function(t) {
-                                                            return t.y - ie * (t.l * v / 2 - 1)
-                                                        }(e)).call(o.font, ne, ie, i).text(e.t).call(u.convertToTspans, t)
+                                                            return t.y - se * (t.l * v / 2 - 1)
+                                                        }(e)).call(o.font, oe, se, i).text(e.t).call(u.convertToTspans, t)
                                                     }))
                                                 }
                                             }))
                                         }
                                     },
                                     70035: function(t, e, r) {
                                         "use strict";
@@ -63916,16 +64036,15 @@
                                                     max: [360, 100, 100, 1],
                                                     fmt: function(t) {
                                                         var e = t.slice(0, 4);
                                                         return e[1] = e[1] + "%", e[2] = e[2] + "%", e
                                                     },
                                                     suffix: ["°", "%", "%", ""]
                                                 }
-                                            },
-                                            pixelatedStyle: ["image-rendering: optimizeSpeed", "image-rendering: -moz-crisp-edges", "image-rendering: -o-crisp-edges", "image-rendering: -webkit-optimize-contrast", "image-rendering: optimize-contrast", "image-rendering: crisp-edges", "image-rendering: pixelated", ""].join("; ")
+                                            }
                                         }
                                     },
                                     13245: function(t, e, r) {
                                         "use strict";
                                         var n = r(71828),
                                             i = r(17230),
                                             a = r(51877),
@@ -64034,127 +64153,128 @@
                                     60775: function(t, e, r) {
                                         "use strict";
                                         var n = r(39898),
                                             i = r(71828),
                                             a = i.strTranslate,
                                             o = r(77922),
                                             s = r(51877),
-                                            l = i.isIOS() || i.isSafari() || i.isIE();
-                                        t.exports = function(t, e, r, u) {
-                                            var c = e.xaxis,
-                                                f = e.yaxis,
-                                                h = !(l || t._context._exportedPlot);
-                                            i.makeTraceGroups(u, r, "im").each((function(e) {
+                                            l = r(3883),
+                                            u = r(32396).STYLE;
+                                        t.exports = function(t, e, r, c) {
+                                            var f = e.xaxis,
+                                                h = e.yaxis,
+                                                p = !t._context._exportedPlot && l();
+                                            i.makeTraceGroups(c, r, "im").each((function(e) {
                                                 var r = n.select(this),
                                                     l = e[0],
-                                                    u = l.trace,
-                                                    p = ("fast" === u.zsmooth || !1 === u.zsmooth && h) && !u._hasZ && u._hasSource && "linear" === c.type && "linear" === f.type;
-                                                u._realImage = p;
-                                                var d, v, g, y, m, x, b = l.z,
-                                                    _ = l.x0,
-                                                    w = l.y0,
-                                                    k = l.w,
-                                                    T = l.h,
-                                                    M = u.dx,
-                                                    A = u.dy;
-                                                for (x = 0; void 0 === d && x < k;) d = c.c2p(_ + x * M), x++;
-                                                for (x = k; void 0 === v && x > 0;) v = c.c2p(_ + x * M), x--;
-                                                for (x = 0; void 0 === y && x < T;) y = f.c2p(w + x * A), x++;
-                                                for (x = T; void 0 === m && x > 0;) m = f.c2p(w + x * A), x--;
-                                                v < d && (g = v, v = d, d = g), m < y && (g = y, y = m, m = g), p || (d = Math.max(-.5 * c._length, d), v = Math.min(1.5 * c._length, v), y = Math.max(-.5 * f._length, y), m = Math.min(1.5 * f._length, m));
-                                                var S = Math.round(v - d),
-                                                    E = Math.round(m - y);
-                                                if (S <= 0 || E <= 0) r.selectAll("image").data([]).exit().remove();
+                                                    c = l.trace,
+                                                    d = ("fast" === c.zsmooth || !1 === c.zsmooth && p) && !c._hasZ && c._hasSource && "linear" === f.type && "linear" === h.type;
+                                                c._realImage = d;
+                                                var v, g, y, m, x, b, _ = l.z,
+                                                    w = l.x0,
+                                                    k = l.y0,
+                                                    T = l.w,
+                                                    M = l.h,
+                                                    A = c.dx,
+                                                    S = c.dy;
+                                                for (b = 0; void 0 === v && b < T;) v = f.c2p(w + b * A), b++;
+                                                for (b = T; void 0 === g && b > 0;) g = f.c2p(w + b * A), b--;
+                                                for (b = 0; void 0 === m && b < M;) m = h.c2p(k + b * S), b++;
+                                                for (b = M; void 0 === x && b > 0;) x = h.c2p(k + b * S), b--;
+                                                g < v && (y = g, g = v, v = y), x < m && (y = m, m = x, x = y), d || (v = Math.max(-.5 * f._length, v), g = Math.min(1.5 * f._length, g), m = Math.max(-.5 * h._length, m), x = Math.min(1.5 * h._length, x));
+                                                var E = Math.round(g - v),
+                                                    C = Math.round(x - m);
+                                                if (E <= 0 || C <= 0) r.selectAll("image").data([]).exit().remove();
                                                 else {
-                                                    var C = r.selectAll("image").data([e]);
-                                                    C.enter().append("svg:image").attr({
+                                                    var L = r.selectAll("image").data([e]);
+                                                    L.enter().append("svg:image").attr({
                                                         xmlns: o.svg,
                                                         preserveAspectRatio: "none"
-                                                    }), C.exit().remove();
-                                                    var L = !1 === u.zsmooth ? s.pixelatedStyle : "";
-                                                    if (p) {
-                                                        var P = i.simpleMap(c.range, c.r2l),
-                                                            O = i.simpleMap(f.range, f.r2l),
-                                                            I = P[1] < P[0],
-                                                            D = O[1] > O[0];
-                                                        if (I || D) {
-                                                            var z = d + S / 2,
-                                                                R = y + E / 2;
-                                                            L += "transform:" + a(z + "px", R + "px") + "scale(" + (I ? -1 : 1) + "," + (D ? -1 : 1) + ")" + a(-z + "px", -R + "px") + ";"
+                                                    }), L.exit().remove();
+                                                    var P = !1 === c.zsmooth ? u : "";
+                                                    if (d) {
+                                                        var O = i.simpleMap(f.range, f.r2l),
+                                                            I = i.simpleMap(h.range, h.r2l),
+                                                            D = O[1] < O[0],
+                                                            z = I[1] > I[0];
+                                                        if (D || z) {
+                                                            var R = v + E / 2,
+                                                                F = m + C / 2;
+                                                            P += "transform:" + a(R + "px", F + "px") + "scale(" + (D ? -1 : 1) + "," + (z ? -1 : 1) + ")" + a(-R + "px", -F + "px") + ";"
                                                         }
                                                     }
-                                                    C.attr("style", L);
-                                                    var F = new Promise((function(t) {
-                                                        if (u._hasZ) t();
-                                                        else if (u._hasSource)
-                                                            if (u._canvas && u._canvas.el.width === k && u._canvas.el.height === T && u._canvas.source === u.source) t();
+                                                    L.attr("style", P);
+                                                    var B = new Promise((function(t) {
+                                                        if (c._hasZ) t();
+                                                        else if (c._hasSource)
+                                                            if (c._canvas && c._canvas.el.width === T && c._canvas.el.height === M && c._canvas.source === c.source) t();
                                                             else {
                                                                 var e = document.createElement("canvas");
-                                                                e.width = k, e.height = T;
+                                                                e.width = T, e.height = M;
                                                                 var r = e.getContext("2d", {
                                                                     willReadFrequently: !0
                                                                 });
-                                                                u._image = u._image || new Image;
-                                                                var n = u._image;
+                                                                c._image = c._image || new Image;
+                                                                var n = c._image;
                                                                 n.onload = function() {
-                                                                    r.drawImage(n, 0, 0), u._canvas = {
+                                                                    r.drawImage(n, 0, 0), c._canvas = {
                                                                         el: e,
-                                                                        source: u.source
+                                                                        source: c.source
                                                                     }, t()
-                                                                }, n.setAttribute("src", u.source)
+                                                                }, n.setAttribute("src", c.source)
                                                             }
                                                     })).then((function() {
                                                         var t, e;
-                                                        if (u._hasZ) e = B((function(t, e) {
-                                                            return b[e][t]
+                                                        if (c._hasZ) e = N((function(t, e) {
+                                                            return _[e][t]
                                                         })), t = e.toDataURL("image/png");
-                                                        else if (u._hasSource)
-                                                            if (p) t = u.source;
+                                                        else if (c._hasSource)
+                                                            if (d) t = c.source;
                                                             else {
-                                                                var r = u._canvas.el.getContext("2d", {
+                                                                var r = c._canvas.el.getContext("2d", {
                                                                     willReadFrequently: !0
-                                                                }).getImageData(0, 0, k, T).data;
-                                                                e = B((function(t, e) {
-                                                                    var n = 4 * (e * k + t);
+                                                                }).getImageData(0, 0, T, M).data;
+                                                                e = N((function(t, e) {
+                                                                    var n = 4 * (e * T + t);
                                                                     return [r[n], r[n + 1], r[n + 2], r[n + 3]]
                                                                 })), t = e.toDataURL("image/png")
-                                                            } C.attr({
+                                                            } L.attr({
                                                             "xlink:href": t,
-                                                            height: E,
-                                                            width: S,
-                                                            x: d,
-                                                            y
+                                                            height: C,
+                                                            width: E,
+                                                            x: v,
+                                                            y: m
                                                         })
                                                     }));
-                                                    t._promises.push(F)
+                                                    t._promises.push(B)
                                                 }
 
-                                                function B(t) {
+                                                function N(t) {
                                                     var e = document.createElement("canvas");
-                                                    e.width = S, e.height = E;
+                                                    e.width = E, e.height = C;
                                                     var r, n = e.getContext("2d", {
                                                             willReadFrequently: !0
                                                         }),
                                                         a = function(t) {
-                                                            return i.constrain(Math.round(c.c2p(_ + t * M) - d), 0, S)
+                                                            return i.constrain(Math.round(f.c2p(w + t * A) - v), 0, E)
                                                         },
                                                         o = function(t) {
-                                                            return i.constrain(Math.round(f.c2p(w + t * A) - y), 0, E)
+                                                            return i.constrain(Math.round(h.c2p(k + t * S) - m), 0, C)
                                                         },
-                                                        h = s.colormodel[u.colormodel],
-                                                        p = h.colormodel || u.colormodel,
-                                                        v = h.fmt;
-                                                    for (x = 0; x < l.w; x++) {
-                                                        var g = a(x),
-                                                            m = a(x + 1);
-                                                        if (m !== g && !isNaN(m) && !isNaN(g))
-                                                            for (var b = 0; b < l.h; b++) {
-                                                                var k = o(b),
-                                                                    T = o(b + 1);
-                                                                T === k || isNaN(T) || isNaN(k) || !t(x, b) || (r = u._scaler(t(x, b)), n.fillStyle = r ? p + "(" + v(r).join(",") + ")" : "rgba(0,0,0,0)", n.fillRect(g, k, m - g, T - k))
+                                                        u = s.colormodel[c.colormodel],
+                                                        p = u.colormodel || c.colormodel,
+                                                        d = u.fmt;
+                                                    for (b = 0; b < l.w; b++) {
+                                                        var g = a(b),
+                                                            y = a(b + 1);
+                                                        if (y !== g && !isNaN(y) && !isNaN(g))
+                                                            for (var x = 0; x < l.h; x++) {
+                                                                var _ = o(x),
+                                                                    T = o(x + 1);
+                                                                T === _ || isNaN(T) || isNaN(_) || !t(b, x) || (r = c._scaler(t(b, x)), n.fillStyle = r ? p + "(" + d(r).join(",") + ")" : "rgba(0,0,0,0)", n.fillRect(g, _, y - g, T - _))
                                                             }
                                                     }
                                                     return e
                                                 }
                                             }))
                                         }
                                     },
@@ -82725,15 +82845,15 @@
                                                     r._indexToPoints = v, e._length = u
                                                 }
                                             }
                                         }
                                     },
                                     11506: function(t, e) {
                                         "use strict";
-                                        e.version = "2.22.0"
+                                        e.version = "2.23.0"
                                     },
                                     9330: function(t, e, r) {
                                         var n, i = r(90386);
                                         self, n = function() {
                                             return function() {
                                                 var t = {
                                                     7386: function(t, e, r) {
```

### Comparing `interpret-core-0.4.0/interpret/lib/interpret-inline.js.LICENSE.txt` & `interpret-core-0.4.1/interpret/lib/interpret-inline.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/perf/_curve.py` & `interpret-core-0.4.1/interpret/perf/_curve.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/perf/_regression.py` & `interpret-core-0.4.1/interpret/perf/_regression.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/provider/_compute.py` & `interpret-core-0.4.1/interpret/provider/_compute.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/provider/_environment.py` & `interpret-core-0.4.1/interpret/provider/_environment.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/provider/_visualize.py` & `interpret-core-0.4.1/interpret/provider/_visualize.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_SPOTgreedy.py` & `interpret-core-0.4.1/interpret/utils/_SPOTgreedy.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_clean_simple.py` & `interpret-core-0.4.1/interpret/utils/_clean_simple.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_clean_x.py` & `interpret-core-0.4.1/interpret/utils/_clean_x.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_compressed_dataset.py` & `interpret-core-0.4.1/interpret/utils/_compressed_dataset.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_explanation.py` & `interpret-core-0.4.1/interpret/utils/_explanation.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_histogram.py` & `interpret-core-0.4.1/interpret/utils/_histogram.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_link.py` & `interpret-core-0.4.1/interpret/utils/_link.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_measure_interactions.py` & `interpret-core-0.4.1/interpret/utils/_measure_interactions.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_native.py` & `interpret-core-0.4.1/interpret/utils/_native.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,14 @@
     BoostFlags_GradientSums = 0x00000004
     BoostFlags_RandomSplits = 0x00000008
 
     # InteractionFlags
     InteractionFlags_Default = 0x00000000
     InteractionFlags_Pure = 0x00000001
 
-    # OutputType
-    OutputType_Unknown = -3
-    OutputType_Ranking = -2
-    OutputType_Regression = -1
-    OutputType_GeneralClassification = 0
-    OutputType_MonoClassification = 1
-    OutputType_BinaryClassification = 2
-    OutputType_MulticlassPlus = 3
-
     # TraceLevel
     _Trace_Off = 0
     _Trace_Error = 1
     _Trace_Warning = 2
     _Trace_Info = 3
     _Trace_Verbose = 4
 
@@ -575,38 +566,36 @@
             ct.byref(link),
             ct.byref(link_param),
         )
 
         if return_code:  # pragma: no cover
             raise Native._get_native_exception(return_code, "DetermineLinkFunction")
 
-        return (
-            self._unsafe.GetLinkFunctionString(link.value).decode("ascii"),
-            link_param.value,
-        )
+        link_str = self._unsafe.GetLinkFunctionStr(link.value)
+        if not link_str:  # pragma: no cover
+            msg = "internal error in call to DetermineLinkFunction"
+            _log.error(msg)
+            raise Exception(msg)
+
+        return (link_str.decode("ascii"), link_param.value)
 
     def get_output_type(self, link):
         if link is None or link.isspace():
             msg = "link must be set to a value"
             _log.error(msg)
             raise Exception(msg)
 
-        link_int = self._unsafe.GetLinkFunctionInt(link.encode("ascii"))
-        output_type = self._unsafe.GetOutputType(link_int)
-        if Native.OutputType_GeneralClassification <= output_type:
-            return "classification"
-        elif output_type == Native.OutputType_Regression:
-            return "regression"
-        elif output_type == Native.OutputType_Ranking:
-            return "ranking"
-        else:
+        output_str = self._unsafe.GetOutputTypeStr(link.encode("ascii"))
+        if not output_str:  # pragma: no cover
             msg = f"unrecognized link function type: {link}"
             _log.error(msg)
             raise Exception(msg)
 
+        return output_str.decode("ascii")
+
     @staticmethod
     def _get_ebm_lib_path(debug=False):
         """Returns filepath of core EBM library.
 
         Returns:
             A string representing filepath.
         """
@@ -1026,31 +1015,25 @@
             # int32_t * linkOut
             ct.c_void_p,
             # double * linkParamOut
             ct.c_void_p,
         ]
         self._unsafe.DetermineLinkFunction.restype = ct.c_int32
 
-        self._unsafe.GetLinkFunctionString.argtypes = [
+        self._unsafe.GetLinkFunctionStr.argtypes = [
             # int32_t link
             ct.c_int32,
         ]
-        self._unsafe.GetLinkFunctionString.restype = ct.c_char_p
+        self._unsafe.GetLinkFunctionStr.restype = ct.c_char_p
 
-        self._unsafe.GetLinkFunctionInt.argtypes = [
+        self._unsafe.GetOutputTypeStr.argtypes = [
             # const char * link
             ct.c_char_p,
         ]
-        self._unsafe.GetLinkFunctionInt.restype = ct.c_int32
-
-        self._unsafe.GetOutputType.argtypes = [
-            # int32_t link
-            ct.c_int32,
-        ]
-        self._unsafe.GetOutputType.restype = ct.c_int64
+        self._unsafe.GetOutputTypeStr.restype = ct.c_char_p
 
         self._unsafe.CreateBooster.argtypes = [
             # void * rng
             ct.c_void_p,
             # void * dataSet
             ct.c_void_p,
             # int8_t * bag
@@ -1737,24 +1720,26 @@
             native._unsafe.FreeInteractionDetector(interaction_handle)
 
         _log.info("Deallocation interaction end")
 
     def calc_interaction_strength(
         self, feature_idxs, interaction_flags, max_cardinality, min_samples_leaf
     ):
-        """Provides strength for an feature interaction. Higher is better."""
+        """Provides a strength measurement of a feature interaction. Higher is better."""
         _log.info("Fast interaction strength start")
 
         native = Native.get_native_singleton()
 
+        feature_idxs = np.array(feature_idxs, np.int64)
+
         strength = ct.c_double(0.0)
         return_code = native._unsafe.CalcInteractionStrength(
             self._interaction_handle,
             len(feature_idxs),
-            Native._make_pointer(np.array(feature_idxs, np.int64), np.int64),
+            Native._make_pointer(feature_idxs, np.int64),
             interaction_flags,
             max_cardinality,
             min_samples_leaf,
             ct.byref(strength),
         )
         if return_code:  # pragma: no cover
             raise Native._get_native_exception(return_code, "CalcInteractionStrength")
```

### Comparing `interpret-core-0.4.0/interpret/utils/_preprocessor.py` & `interpret-core-0.4.1/interpret/utils/_preprocessor.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_privacy.py` & `interpret-core-0.4.1/interpret/utils/_privacy.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_rank_interactions.py` & `interpret-core-0.4.1/interpret/utils/_rank_interactions.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_seed.py` & `interpret-core-0.4.1/interpret/utils/_seed.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_shap_common.py` & `interpret-core-0.4.1/interpret/utils/_shap_common.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_unify_data.py` & `interpret-core-0.4.1/interpret/utils/_unify_data.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/utils/_unify_predict.py` & `interpret-core-0.4.1/interpret/utils/_unify_predict.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/visual/_inline.py` & `interpret-core-0.4.1/interpret/visual/_inline.py`

 * *Files 6% similar despite different names*

```diff
@@ -239,13 +239,19 @@
         _render_databricks(init_js + body_js)
     elif (
         "colab" in detected_envs
         or "azureml" in detected_envs
         or "azuresynapse" in detected_envs
     ):
         display(HTML(init_js + body_js))
+    elif "streamlit" in detected_envs:
+        import streamlit.components.v1 as components
+
+        components.html(
+            HTML(init_js + body_js).data, height=1000, width=1000, scrolling=True
+        )
     else:  # Fallthrough assumes we are in an IPython environment at a minimum.
         if not _current_module.jupyter_initialized:
             _current_module.jupyter_initialized = True
             display(HTML(init_js + body_js))
         else:
             display(HTML(body_js))
```

### Comparing `interpret-core-0.4.0/interpret/visual/_interactive.py` & `interpret-core-0.4.1/interpret/visual/_interactive.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/visual/_udash.py` & `interpret-core-0.4.1/interpret/visual/_udash.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/visual/assets/favicon.ico` & `interpret-core-0.4.1/interpret/visual/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/visual/assets/udash.css` & `interpret-core-0.4.1/interpret/visual/assets/udash.css`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/visual/assets/udash.js` & `interpret-core-0.4.1/interpret/visual/assets/udash.js`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/visual/dashboard.py` & `interpret-core-0.4.1/interpret/visual/dashboard.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret/visual/plot.py` & `interpret-core-0.4.1/interpret/visual/plot.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret_core.egg-info/PKG-INFO` & `interpret-core-0.4.1/interpret_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpret-core
-Version: 0.4.0
+Version: 0.4.1
 Summary: Fit interpretable models. Explain blackbox machine learning.
 Home-page: https://github.com/interpretml/interpret
 Author: The InterpretML Contributors
 Author-email: interpret@microsoft.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `interpret-core-0.4.0/interpret_core.egg-info/SOURCES.txt` & `interpret-core-0.4.1/interpret_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret_core.egg-info/entry_points.txt` & `interpret-core-0.4.1/interpret_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/interpret_core.egg-info/requires.txt` & `interpret-core-0.4.1/interpret_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/setup.py` & `interpret-core-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from distutils.command.install import install
 
 from setuptools import setup, find_packages
 from setuptools.command.sdist import sdist
 
 name = "interpret-core"
 # NOTE: Version is replaced by a regex script.
-version = "0.4.0"
+version = "0.4.1"
 long_description = """
 Core system for the interpret package.
 
 https://github.com/interpretml/interpret
 """
 
 entry_points = {
```

### Comparing `interpret-core-0.4.0/symbolic/LICENSE` & `interpret-core-0.4.1/symbolic/LICENSE`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/README.md` & `interpret-core-0.4.1/symbolic/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,2124 +1,2146 @@
-00000000: 2320 496e 7465 7270 7265 744d 4c0a 0a5b  # InterpretML..[
-00000010: 215b 4269 6e64 6572 5d28 6874 7470 733a  ![Binder](https:
-00000020: 2f2f 6d79 6269 6e64 6572 2e6f 7267 2f62  //mybinder.org/b
-00000030: 6164 6765 5f6c 6f67 6f2e 7376 6729 5d28  adge_logo.svg)](
-00000040: 6874 7470 733a 2f2f 6d79 6269 6e64 6572  https://mybinder
-00000050: 2e6f 7267 2f76 322f 6768 2f69 6e74 6572  .org/v2/gh/inter
-00000060: 7072 6574 6d6c 2f69 6e74 6572 7072 6574  pretml/interpret
-00000070: 2f64 6576 656c 6f70 3f6c 6162 7061 7468  /develop?labpath
-00000080: 3d65 7861 6d70 6c65 7325 3246 7079 7468  =examples%2Fpyth
-00000090: 6f6e 2532 4649 6e74 6572 7072 6574 6162  on%2FInterpretab
-000000a0: 6c65 5f43 6c61 7373 6966 6963 6174 696f  le_Classificatio
-000000b0: 6e5f 4d65 7468 6f64 732e 6970 796e 6229  n_Methods.ipynb)
-000000c0: 0a21 5b4c 6963 656e 7365 5d28 6874 7470  .![License](http
-000000d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000000e0: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
-000000f0: 652f 696e 7465 7270 7265 746d 6c2f 696e  e/interpretml/in
-00000100: 7465 7270 7265 742e 7376 673f 7374 796c  terpret.svg?styl
-00000110: 653d 666c 6174 2d73 7175 6172 6529 0a21  e=flat-square).!
-00000120: 5b50 7974 686f 6e20 5665 7273 696f 6e5d  [Python Version]
-00000130: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000140: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
-00000150: 6572 7369 6f6e 732f 696e 7465 7270 7265  ersions/interpre
-00000160: 742e 7376 673f 7374 796c 653d 666c 6174  t.svg?style=flat
-00000170: 2d73 7175 6172 6529 0a21 5b50 6163 6b61  -square).![Packa
-00000180: 6765 2056 6572 7369 6f6e 5d28 6874 7470  ge Version](http
-00000190: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000001a0: 696f 2f70 7970 692f 762f 696e 7465 7270  io/pypi/v/interp
-000001b0: 7265 742e 7376 673f 7374 796c 653d 666c  ret.svg?style=fl
-000001c0: 6174 2d73 7175 6172 6529 0a21 5b43 6f6e  at-square).![Con
-000001d0: 6461 5d28 6874 7470 733a 2f2f 696d 672e  da](https://img.
-000001e0: 7368 6965 6c64 732e 696f 2f63 6f6e 6461  shields.io/conda
-000001f0: 2f76 2f63 6f6e 6461 2d66 6f72 6765 2f69  /v/conda-forge/i
-00000200: 6e74 6572 7072 6574 290a 215b 4275 696c  nterpret).![Buil
-00000210: 6420 5374 6174 7573 5d28 6874 7470 733a  d Status](https:
-00000220: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000230: 2f61 7a75 7265 2d64 6576 6f70 732f 6275  /azure-devops/bu
-00000240: 696c 642f 6d73 2f69 6e74 6572 7072 6574  ild/ms/interpret
-00000250: 2f32 3933 2f64 6576 656c 6f70 2e73 7667  /293/develop.svg
-00000260: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
-00000270: 7265 290a 215b 436f 7665 7261 6765 5d28  re).![Coverage](
-00000280: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000290: 6c64 732e 696f 2f61 7a75 7265 2d64 6576  lds.io/azure-dev
-000002a0: 6f70 732f 636f 7665 7261 6765 2f6d 732f  ops/coverage/ms/
-000002b0: 696e 7465 7270 7265 742f 3239 332f 6465  interpret/293/de
-000002c0: 7665 6c6f 702e 7376 673f 7374 796c 653d  velop.svg?style=
-000002d0: 666c 6174 2d73 7175 6172 6529 0a21 5b4d  flat-square).![M
-000002e0: 6169 6e74 656e 616e 6365 5d28 6874 7470  aintenance](http
-000002f0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000300: 696f 2f6d 6169 6e74 656e 616e 6365 2f79  io/maintenance/y
-00000310: 6573 2f32 3032 333f 7374 796c 653d 666c  es/2023?style=fl
-00000320: 6174 2d73 7175 6172 6529 0a3c 6272 2f3e  at-square).<br/>
-00000330: 0a3e 2023 2323 2049 6e20 7468 6520 6265  .> ### In the be
-00000340: 6769 6e6e 696e 6720 6d61 6368 696e 6573  ginning machines
-00000350: 206c 6561 726e 6564 2069 6e20 6461 726b   learned in dark
-00000360: 6e65 7373 2c20 616e 6420 6461 7461 2073  ness, and data s
-00000370: 6369 656e 7469 7374 7320 7374 7275 6767  cientists strugg
-00000380: 6c65 6420 696e 2074 6865 2076 6f69 6420  led in the void 
-00000390: 746f 2065 7870 6c61 696e 2074 6865 6d2e  to explain them.
-000003a0: 200a 3e20 2323 2320 4c65 7420 7468 6572   .> ### Let ther
-000003b0: 6520 6265 206c 6967 6874 2e0a 0a49 6e74  e be light...Int
-000003c0: 6572 7072 6574 4d4c 2069 7320 616e 206f  erpretML is an o
-000003d0: 7065 6e2d 736f 7572 6365 2070 6163 6b61  pen-source packa
-000003e0: 6765 2074 6861 7420 696e 636f 7270 6f72  ge that incorpor
-000003f0: 6174 6573 2073 7461 7465 2d6f 662d 7468  ates state-of-th
-00000400: 652d 6172 7420 6d61 6368 696e 6520 6c65  e-art machine le
-00000410: 6172 6e69 6e67 2069 6e74 6572 7072 6574  arning interpret
-00000420: 6162 696c 6974 7920 7465 6368 6e69 7175  ability techniqu
-00000430: 6573 2075 6e64 6572 206f 6e65 2072 6f6f  es under one roo
-00000440: 662e 2057 6974 6820 7468 6973 2070 6163  f. With this pac
-00000450: 6b61 6765 2c20 796f 7520 6361 6e20 7472  kage, you can tr
-00000460: 6169 6e20 696e 7465 7270 7265 7461 626c  ain interpretabl
-00000470: 6520 676c 6173 7362 6f78 206d 6f64 656c  e glassbox model
-00000480: 7320 616e 6420 6578 706c 6169 6e20 626c  s and explain bl
-00000490: 6163 6b62 6f78 2073 7973 7465 6d73 2e20  ackbox systems. 
-000004a0: 496e 7465 7270 7265 744d 4c20 6865 6c70  InterpretML help
-000004b0: 7320 796f 7520 756e 6465 7273 7461 6e64  s you understand
-000004c0: 2079 6f75 7220 6d6f 6465 6c27 7320 676c   your model's gl
-000004d0: 6f62 616c 2062 6568 6176 696f 722c 206f  obal behavior, o
-000004e0: 7220 756e 6465 7273 7461 6e64 2074 6865  r understand the
-000004f0: 2072 6561 736f 6e73 2062 6568 696e 6420   reasons behind 
-00000500: 696e 6469 7669 6475 616c 2070 7265 6469  individual predi
-00000510: 6374 696f 6e73 2e0a 0a49 6e74 6572 7072  ctions...Interpr
-00000520: 6574 6162 696c 6974 7920 6973 2065 7373  etability is ess
-00000530: 656e 7469 616c 2066 6f72 3a0a 2d20 4d6f  ential for:.- Mo
-00000540: 6465 6c20 6465 6275 6767 696e 6720 2d20  del debugging - 
-00000550: 5768 7920 6469 6420 6d79 206d 6f64 656c  Why did my model
-00000560: 206d 616b 6520 7468 6973 206d 6973 7461   make this mista
-00000570: 6b65 3f0a 2d20 4665 6174 7572 6520 456e  ke?.- Feature En
-00000580: 6769 6e65 6572 696e 6720 2d20 486f 7720  gineering - How 
-00000590: 6361 6e20 4920 696d 7072 6f76 6520 6d79  can I improve my
-000005a0: 206d 6f64 656c 3f0a 2d20 4465 7465 6374   model?.- Detect
-000005b0: 696e 6720 6661 6972 6e65 7373 2069 7373  ing fairness iss
-000005c0: 7565 7320 2d20 446f 6573 206d 7920 6d6f  ues - Does my mo
-000005d0: 6465 6c20 6469 7363 7269 6d69 6e61 7465  del discriminate
-000005e0: 3f0a 2d20 4875 6d61 6e2d 4149 2063 6f6f  ?.- Human-AI coo
-000005f0: 7065 7261 7469 6f6e 202d 2048 6f77 2063  peration - How c
-00000600: 616e 2049 2075 6e64 6572 7374 616e 6420  an I understand 
-00000610: 616e 6420 7472 7573 7420 7468 6520 6d6f  and trust the mo
-00000620: 6465 6c27 7320 6465 6369 7369 6f6e 733f  del's decisions?
-00000630: 0a2d 2052 6567 756c 6174 6f72 7920 636f  .- Regulatory co
-00000640: 6d70 6c69 616e 6365 202d 2044 6f65 7320  mpliance - Does 
-00000650: 6d79 206d 6f64 656c 2073 6174 6973 6679  my model satisfy
-00000660: 206c 6567 616c 2072 6571 7569 7265 6d65   legal requireme
-00000670: 6e74 733f 0a2d 2048 6967 682d 7269 736b  nts?.- High-risk
-00000680: 2061 7070 6c69 6361 7469 6f6e 7320 2d20   applications - 
-00000690: 4865 616c 7468 6361 7265 2c20 6669 6e61  Healthcare, fina
-000006a0: 6e63 652c 206a 7564 6963 6961 6c2c 202e  nce, judicial, .
-000006b0: 2e2e 0a0a 215b 5d28 6874 7470 733a 2f2f  ....![](https://
-000006c0: 6769 7468 7562 2e63 6f6d 2f69 6e74 6572  github.com/inter
-000006d0: 7072 6574 6d6c 2f69 6e74 6572 7072 6574  pretml/interpret
-000006e0: 6d6c 2e67 6974 6875 622e 696f 2f62 6c6f  ml.github.io/blo
-000006f0: 622f 6d61 7374 6572 2f69 6e74 6572 7072  b/master/interpr
-00000700: 6574 2d68 6967 686c 6967 6874 2e67 6966  et-highlight.gif
-00000710: 290a 0a23 2049 6e73 7461 6c6c 6174 696f  )..# Installatio
-00000720: 6e0a 0a50 7974 686f 6e20 332e 372b 207c  n..Python 3.7+ |
-00000730: 204c 696e 7578 2c20 4d61 632c 2057 696e   Linux, Mac, Win
-00000740: 646f 7773 0a60 6060 7368 0a70 6970 2069  dows.```sh.pip i
-00000750: 6e73 7461 6c6c 2069 6e74 6572 7072 6574  nstall interpret
-00000760: 0a23 204f 520a 636f 6e64 6120 696e 7374  .# OR.conda inst
-00000770: 616c 6c20 2d63 2063 6f6e 6461 2d66 6f72  all -c conda-for
-00000780: 6765 2069 6e74 6572 7072 6574 0a60 6060  ge interpret.```
-00000790: 0a0a 2320 496e 7472 6f64 7563 696e 6720  ..# Introducing 
-000007a0: 7468 6520 4578 706c 6169 6e61 626c 6520  the Explainable 
-000007b0: 426f 6f73 7469 6e67 204d 6163 6869 6e65  Boosting Machine
-000007c0: 2028 4542 4d29 0a0a 4542 4d20 6973 2061   (EBM)..EBM is a
-000007d0: 6e20 696e 7465 7270 7265 7461 626c 6520  n interpretable 
-000007e0: 6d6f 6465 6c20 6465 7665 6c6f 7065 6420  model developed 
-000007f0: 6174 204d 6963 726f 736f 6674 2052 6573  at Microsoft Res
-00000800: 6561 7263 683c 7375 703e 5b2a 5d28 2363  earch<sup>[*](#c
-00000810: 6974 6174 696f 6e73 293c 2f73 7570 3e2e  itations)</sup>.
-00000820: 2049 7420 7573 6573 206d 6f64 6572 6e20   It uses modern 
-00000830: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
-00000840: 2074 6563 686e 6971 7565 7320 6c69 6b65   techniques like
-00000850: 2062 6167 6769 6e67 2c20 6772 6164 6965   bagging, gradie
-00000860: 6e74 2062 6f6f 7374 696e 672c 2061 6e64  nt boosting, and
-00000870: 2061 7574 6f6d 6174 6963 2069 6e74 6572   automatic inter
-00000880: 6163 7469 6f6e 2064 6574 6563 7469 6f6e  action detection
-00000890: 2074 6f20 6272 6561 7468 6520 6e65 7720   to breathe new 
-000008a0: 6c69 6665 2069 6e74 6f20 7472 6164 6974  life into tradit
-000008b0: 696f 6e61 6c20 4741 4d73 2028 4765 6e65  ional GAMs (Gene
-000008c0: 7261 6c69 7a65 6420 4164 6469 7469 7665  ralized Additive
-000008d0: 204d 6f64 656c 7329 2e20 5468 6973 206d   Models). This m
-000008e0: 616b 6573 2045 424d 7320 6173 2061 6363  akes EBMs as acc
-000008f0: 7572 6174 6520 6173 2073 7461 7465 2d6f  urate as state-o
-00000900: 662d 7468 652d 6172 7420 7465 6368 6e69  f-the-art techni
-00000910: 7175 6573 206c 696b 6520 7261 6e64 6f6d  ques like random
-00000920: 2066 6f72 6573 7473 2061 6e64 2067 7261   forests and gra
-00000930: 6469 656e 7420 626f 6f73 7465 6420 7472  dient boosted tr
-00000940: 6565 732e 2048 6f77 6576 6572 2c20 756e  ees. However, un
-00000950: 6c69 6b65 2074 6865 7365 2062 6c61 636b  like these black
-00000960: 626f 7820 6d6f 6465 6c73 2c20 4542 4d73  box models, EBMs
-00000970: 2070 726f 6475 6365 2065 7861 6374 2065   produce exact e
-00000980: 7870 6c61 6e61 7469 6f6e 7320 616e 6420  xplanations and 
-00000990: 6172 6520 6564 6974 6162 6c65 2062 7920  are editable by 
-000009a0: 646f 6d61 696e 2065 7870 6572 7473 2e0a  domain experts..
-000009b0: 0a7c 2044 6174 6173 6574 2f41 5552 4f43  .| Dataset/AUROC
-000009c0: 207c 2044 6f6d 6169 6e20 207c 204c 6f67   | Domain  | Log
-000009d0: 6973 7469 6320 5265 6772 6573 7369 6f6e  istic Regression
-000009e0: 207c 2052 616e 646f 6d20 466f 7265 7374   | Random Forest
-000009f0: 207c 2058 4742 6f6f 7374 2020 2020 2020   | XGBoost      
-00000a00: 2020 207c 2045 7870 6c61 696e 6162 6c65     | Explainable
-00000a10: 2042 6f6f 7374 696e 6720 4d61 6368 696e   Boosting Machin
-00000a20: 6520 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  e |.|-----------
-00000a30: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 7c3a  ----|---------|:
-00000a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a50: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
-00000a60: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
-00000a70: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-00000a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a90: 2d2d 2d2d 3a7c 0a7c 2041 6475 6c74 2049  ----:|.| Adult I
-00000aa0: 6e63 6f6d 6520 207c 2046 696e 616e 6365  ncome  | Finance
-00000ab0: 207c 202e 3930 37c2 b12e 3030 3320 2020   | .907...003   
-00000ac0: 2020 2020 2020 2020 7c20 2e39 3033 c2b1          | .903..
-00000ad0: 2e30 3032 2020 2020 207c 202e 3932 37c2  .002     | .927.
-00000ae0: b12e 3030 3120 2020 2020 2020 7c20 2a2a  ..001       | **
-00000af0: 5f2e 3932 38c2 b12e 3030 325f 2a2a 2020  _.928...002_**  
-00000b00: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00000b10: 4865 6172 7420 4469 7365 6173 6520 7c20  Heart Disease | 
-00000b20: 4d65 6469 6361 6c20 7c20 2e38 3935 c2b1  Medical | .895..
-00000b30: 2e30 3330 2020 2020 2020 2020 2020 207c  .030           |
-00000b40: 202e 3839 30c2 b12e 3030 3820 2020 2020   .890...008     
-00000b50: 7c20 2e38 3531 c2b1 2e30 3138 2020 2020  | .851...018    
-00000b60: 2020 207c 202a 2a5f 2e38 3938 c2b1 2e30     | **_.898...0
-00000b70: 3133 5f2a 2a20 2020 2020 2020 2020 2020  13_**           
-00000b80: 2020 207c 0a7c 2042 7265 6173 7420 4361     |.| Breast Ca
-00000b90: 6e63 6572 207c 204d 6564 6963 616c 207c  ncer | Medical |
-00000ba0: 202a 2a5f 2e39 3935 c2b1 2e30 3035 5f2a   **_.995...005_*
-00000bb0: 2a20 2020 2020 7c20 2e39 3932 c2b1 2e30  *     | .992...0
-00000bc0: 3039 2020 2020 207c 202e 3939 32c2 b12e  09     | .992...
-00000bd0: 3031 3020 2020 2020 2020 7c20 2a2a 5f2e  010       | **_.
-00000be0: 3939 35c2 b12e 3030 365f 2a2a 2020 2020  995...006_**    
-00000bf0: 2020 2020 2020 2020 2020 7c0a 7c20 5465            |.| Te
-00000c00: 6c65 636f 6d20 4368 7572 6e20 7c20 4275  lecom Churn | Bu
-00000c10: 7369 6e65 7373 7c20 2e38 3439 c2b1 2e30  siness| .849...0
-00000c20: 3035 2020 2020 2020 2020 2020 207c 202e  05           | .
-00000c30: 3832 34c2 b12e 3030 3420 2020 2020 7c20  824...004     | 
-00000c40: 2e38 3238 c2b1 2e30 3130 2020 2020 2020  .828...010      
-00000c50: 207c 202a 2a5f 2e38 3532 c2b1 2e30 3036   | **_.852...006
-00000c60: 5f2a 2a20 2020 2020 2020 2020 2020 2020  _**             
-00000c70: 207c 0a7c 2043 7265 6469 7420 4672 6175   |.| Credit Frau
-00000c80: 6420 207c 2053 6563 7572 6974 797c 202e  d  | Security| .
-00000c90: 3937 39c2 b12e 3030 3220 2020 2020 2020  979...002       
-00000ca0: 2020 2020 7c20 2e39 3530 c2b1 2e30 3037      | .950...007
-00000cb0: 2020 2020 207c 202a 2a5f 2e39 3831 c2b1       | **_.981..
-00000cc0: 2e30 3033 5f2a 2a20 7c20 2a2a 5f2e 3938  .003_** | **_.98
-00000cd0: 31c2 b12e 3030 335f 2a2a 2020 2020 2020  1...003_**      
-00000ce0: 2020 2020 2020 2020 7c0a 0a5b 2a4e 6f74          |..[*Not
-00000cf0: 6562 6f6f 6b20 666f 7220 7265 7072 6f64  ebook for reprod
-00000d00: 7563 696e 6720 7461 626c 652a 5d28 6874  ucing table*](ht
-00000d10: 7470 733a 2f2f 6e62 7669 6577 6572 2e6a  tps://nbviewer.j
-00000d20: 7570 7974 6572 2e6f 7267 2f67 6974 6875  upyter.org/githu
-00000d30: 622f 696e 7465 7270 7265 746d 6c2f 696e  b/interpretml/in
-00000d40: 7465 7270 7265 742f 626c 6f62 2f6d 6173  terpret/blob/mas
-00000d50: 7465 722f 6265 6e63 686d 6172 6b73 2f45  ter/benchmarks/E
-00000d60: 424d 2532 3043 6c61 7373 6966 6963 6174  BM%20Classificat
-00000d70: 696f 6e25 3230 436f 6d70 6172 6973 6f6e  ion%20Comparison
-00000d80: 2e69 7079 6e62 290a 0a23 2053 7570 706f  .ipynb)..# Suppo
-00000d90: 7274 6564 2054 6563 686e 6971 7565 730a  rted Techniques.
-00000da0: 0a7c 2049 6e74 6572 7072 6574 6162 696c  .| Interpretabil
-00000db0: 6974 7920 5465 6368 6e69 7175 6520 207c  ity Technique  |
-00000dc0: 2054 7970 6520 2020 2020 2020 2020 2020   Type           
-00000dd0: 2020 2020 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d      |.|---------
-00000de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000df0: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
-00000e00: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 205b 4578  ---------|.| [Ex
-00000e10: 706c 6169 6e61 626c 6520 426f 6f73 7469  plainable Boosti
-00000e20: 6e67 5d28 6874 7470 733a 2f2f 696e 7465  ng](https://inte
-00000e30: 7270 7265 742e 6d6c 2f64 6f63 732f 6562  rpret.ml/docs/eb
-00000e40: 6d2e 6874 6d6c 2920 2020 2020 2020 207c  m.html)        |
-00000e50: 2067 6c61 7373 626f 7820 6d6f 6465 6c20   glassbox model 
-00000e60: 2020 2020 7c0a 7c20 5b44 6563 6973 696f      |.| [Decisio
-00000e70: 6e20 5472 6565 5d28 6874 7470 733a 2f2f  n Tree](https://
-00000e80: 696e 7465 7270 7265 742e 6d6c 2f64 6f63  interpret.ml/doc
-00000e90: 732f 6474 2e68 746d 6c29 2020 2020 2020  s/dt.html)      
-00000ea0: 2020 2020 2020 2020 2020 7c20 676c 6173            | glas
-00000eb0: 7362 6f78 206d 6f64 656c 2020 2020 207c  sbox model     |
-00000ec0: 0a7c 205b 4465 6369 7369 6f6e 2052 756c  .| [Decision Rul
-00000ed0: 6520 4c69 7374 5d28 6874 7470 733a 2f2f  e List](https://
-00000ee0: 696e 7465 7270 7265 742e 6d6c 2f64 6f63  interpret.ml/doc
-00000ef0: 732f 6472 2e68 746d 6c29 2020 2020 2020  s/dr.html)      
-00000f00: 2020 2020 207c 2067 6c61 7373 626f 7820       | glassbox 
-00000f10: 6d6f 6465 6c20 2020 2020 7c0a 7c20 5b4c  model     |.| [L
-00000f20: 696e 6561 722f 4c6f 6769 7374 6963 2052  inear/Logistic R
-00000f30: 6567 7265 7373 696f 6e5d 2868 7474 7073  egression](https
-00000f40: 3a2f 2f69 6e74 6572 7072 6574 2e6d 6c2f  ://interpret.ml/
-00000f50: 646f 6373 2f6c 722e 6874 6d6c 2920 2020  docs/lr.html)   
-00000f60: 7c20 676c 6173 7362 6f78 206d 6f64 656c  | glassbox model
-00000f70: 2020 2020 207c 0a7c 205b 5348 4150 204b       |.| [SHAP K
-00000f80: 6572 6e65 6c20 4578 706c 6169 6e65 725d  ernel Explainer]
-00000f90: 2868 7474 7073 3a2f 2f69 6e74 6572 7072  (https://interpr
-00000fa0: 6574 2e6d 6c2f 646f 6373 2f73 6861 702e  et.ml/docs/shap.
-00000fb0: 6874 6d6c 2920 2020 2020 207c 2062 6c61  html)      | bla
-00000fc0: 636b 626f 7820 6578 706c 6169 6e65 7220  ckbox explainer 
-00000fd0: 7c0a 7c20 5b4c 494d 455d 2868 7474 7073  |.| [LIME](https
-00000fe0: 3a2f 2f69 6e74 6572 7072 6574 2e6d 6c2f  ://interpret.ml/
-00000ff0: 646f 6373 2f6c 696d 652e 6874 6d6c 2920  docs/lime.html) 
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 2020 2020 2020 7c20 626c 6163 6b62 6f78        | blackbox
-00001020: 2065 7870 6c61 696e 6572 207c 0a7c 205b   explainer |.| [
-00001030: 4d6f 7272 6973 2053 656e 7369 7469 7669  Morris Sensitivi
-00001040: 7479 2041 6e61 6c79 7369 735d 2868 7474  ty Analysis](htt
-00001050: 7073 3a2f 2f69 6e74 6572 7072 6574 2e6d  ps://interpret.m
-00001060: 6c2f 646f 6373 2f6d 7361 2e68 746d 6c29  l/docs/msa.html)
-00001070: 207c 2062 6c61 636b 626f 7820 6578 706c   | blackbox expl
-00001080: 6169 6e65 7220 7c0a 7c20 5b50 6172 7469  ainer |.| [Parti
-00001090: 616c 2044 6570 656e 6465 6e63 655d 2868  al Dependence](h
-000010a0: 7474 7073 3a2f 2f69 6e74 6572 7072 6574  ttps://interpret
-000010b0: 2e6d 6c2f 646f 6373 2f70 6470 2e68 746d  .ml/docs/pdp.htm
-000010c0: 6c29 2020 2020 2020 2020 2020 7c20 626c  l)          | bl
-000010d0: 6163 6b62 6f78 2065 7870 6c61 696e 6572  ackbox explainer
-000010e0: 207c 0a0a 2320 5472 6169 6e20 6120 676c   |..# Train a gl
-000010f0: 6173 7362 6f78 206d 6f64 656c 0a0a 4c65  assbox model..Le
-00001100: 7427 7320 6669 7420 616e 2045 7870 6c61  t's fit an Expla
-00001110: 696e 6162 6c65 2042 6f6f 7374 696e 6720  inable Boosting 
-00001120: 4d61 6368 696e 650a 0a60 6060 7079 7468  Machine..```pyth
-00001130: 6f6e 0a66 726f 6d20 696e 7465 7270 7265  on.from interpre
-00001140: 742e 676c 6173 7362 6f78 2069 6d70 6f72  t.glassbox impor
-00001150: 7420 4578 706c 6169 6e61 626c 6542 6f6f  t ExplainableBoo
-00001160: 7374 696e 6743 6c61 7373 6966 6965 720a  stingClassifier.
-00001170: 0a65 626d 203d 2045 7870 6c61 696e 6162  .ebm = Explainab
-00001180: 6c65 426f 6f73 7469 6e67 436c 6173 7369  leBoostingClassi
-00001190: 6669 6572 2829 0a65 626d 2e66 6974 2858  fier().ebm.fit(X
-000011a0: 5f74 7261 696e 2c20 795f 7472 6169 6e29  _train, y_train)
-000011b0: 0a0a 2320 6f72 2073 7562 7374 6974 7574  ..# or substitut
-000011c0: 6520 7769 7468 204c 6f67 6973 7469 6352  e with LogisticR
-000011d0: 6567 7265 7373 696f 6e2c 2044 6563 6973  egression, Decis
-000011e0: 696f 6e54 7265 6543 6c61 7373 6966 6965  ionTreeClassifie
-000011f0: 722c 2052 756c 654c 6973 7443 6c61 7373  r, RuleListClass
-00001200: 6966 6965 722c 202e 2e2e 0a23 2045 424d  ifier, ....# EBM
-00001210: 2073 7570 706f 7274 7320 7061 6e64 6173   supports pandas
-00001220: 2064 6174 6166 7261 6d65 732c 206e 756d   dataframes, num
-00001230: 7079 2061 7272 6179 732c 2061 6e64 2068  py arrays, and h
-00001240: 616e 646c 6573 2022 7374 7269 6e67 2220  andles "string" 
-00001250: 6461 7461 206e 6174 6976 656c 792e 0a60  data natively..`
-00001260: 6060 0a0a 556e 6465 7273 7461 6e64 2074  ``..Understand t
-00001270: 6865 206d 6f64 656c 0a60 6060 7079 7468  he model.```pyth
-00001280: 6f6e 0a66 726f 6d20 696e 7465 7270 7265  on.from interpre
-00001290: 7420 696d 706f 7274 2073 686f 770a 0a65  t import show..e
-000012a0: 626d 5f67 6c6f 6261 6c20 3d20 6562 6d2e  bm_global = ebm.
-000012b0: 6578 706c 6169 6e5f 676c 6f62 616c 2829  explain_global()
-000012c0: 0a73 686f 7728 6562 6d5f 676c 6f62 616c  .show(ebm_global
-000012d0: 290a 6060 600a 215b 476c 6f62 616c 2045  ).```.![Global E
-000012e0: 7870 6c61 6e61 7469 6f6e 2049 6d61 6765  xplanation Image
-000012f0: 5d28 2e2f 6578 616d 706c 6573 2f70 7974  ](./examples/pyt
-00001300: 686f 6e2f 6173 7365 7473 2f72 6561 646d  hon/assets/readm
-00001310: 655f 6562 6d5f 676c 6f62 616c 5f73 7065  e_ebm_global_spe
-00001320: 6369 6669 632e 504e 473f 7261 773d 7472  cific.PNG?raw=tr
-00001330: 7565 290a 0a3c 6272 2f3e 0a0a 556e 6465  ue)..<br/>..Unde
-00001340: 7273 7461 6e64 2069 6e64 6976 6964 7561  rstand individua
-00001350: 6c20 7072 6564 6963 7469 6f6e 730a 6060  l predictions.``
-00001360: 6070 7974 686f 6e0a 6562 6d5f 6c6f 6361  `python.ebm_loca
-00001370: 6c20 3d20 6562 6d2e 6578 706c 6169 6e5f  l = ebm.explain_
-00001380: 6c6f 6361 6c28 585f 7465 7374 2c20 795f  local(X_test, y_
-00001390: 7465 7374 290a 7368 6f77 2865 626d 5f6c  test).show(ebm_l
-000013a0: 6f63 616c 290a 6060 600a 215b 4c6f 6361  ocal).```.![Loca
-000013b0: 6c20 4578 706c 616e 6174 696f 6e20 496d  l Explanation Im
-000013c0: 6167 655d 282e 2f65 7861 6d70 6c65 732f  age](./examples/
-000013d0: 7079 7468 6f6e 2f61 7373 6574 732f 7265  python/assets/re
-000013e0: 6164 6d65 5f65 626d 5f6c 6f63 616c 5f73  adme_ebm_local_s
-000013f0: 7065 6369 6669 632e 504e 473f 7261 773d  pecific.PNG?raw=
-00001400: 7472 7565 290a 0a3c 6272 2f3e 0a0a 416e  true)..<br/>..An
-00001410: 6420 6966 2079 6f75 2068 6176 6520 6d75  d if you have mu
-00001420: 6c74 6970 6c65 206d 6f64 656c 2065 7870  ltiple model exp
-00001430: 6c61 6e61 7469 6f6e 732c 2063 6f6d 7061  lanations, compa
-00001440: 7265 2074 6865 6d0a 6060 6070 7974 686f  re them.```pytho
-00001450: 6e0a 7368 6f77 285b 6c6f 6769 7374 6963  n.show([logistic
-00001460: 5f72 6567 7265 7373 696f 6e5f 676c 6f62  _regression_glob
-00001470: 616c 2c20 6465 6369 7369 6f6e 5f74 7265  al, decision_tre
-00001480: 655f 676c 6f62 616c 5d29 0a60 6060 0a21  e_global]).```.!
-00001490: 5b44 6173 6862 6f61 7264 2049 6d61 6765  [Dashboard Image
-000014a0: 5d28 2e2f 6578 616d 706c 6573 2f70 7974  ](./examples/pyt
-000014b0: 686f 6e2f 6173 7365 7473 2f72 6561 646d  hon/assets/readm
-000014c0: 655f 6461 7368 626f 6172 642e 504e 473f  e_dashboard.PNG?
-000014d0: 7261 773d 7472 7565 290a 0a3c 6272 2f3e  raw=true)..<br/>
-000014e0: 0a0a 4966 2079 6f75 206e 6565 6420 746f  ..If you need to
-000014f0: 206b 6565 7020 796f 7572 2064 6174 6120   keep your data 
-00001500: 7072 6976 6174 652c 2075 7365 2044 6966  private, use Dif
-00001510: 6665 7265 6e74 6961 6c6c 7920 5072 6976  ferentially Priv
-00001520: 6174 6520 4542 4d73 2028 7365 6520 5b44  ate EBMs (see [D
-00001530: 502d 4542 4d73 5d28 6874 7470 733a 2f2f  P-EBMs](https://
-00001540: 7072 6f63 6565 6469 6e67 732e 6d6c 722e  proceedings.mlr.
-00001550: 7072 6573 732f 7631 3339 2f6e 6f72 6932  press/v139/nori2
-00001560: 3161 2f6e 6f72 6932 3161 2e70 6466 2929  1a/nori21a.pdf))
-00001570: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00001580: 2069 6e74 6572 7072 6574 2e70 7269 7661   interpret.priva
-00001590: 6379 2069 6d70 6f72 7420 4450 4578 706c  cy import DPExpl
-000015a0: 6169 6e61 626c 6542 6f6f 7374 696e 6743  ainableBoostingC
-000015b0: 6c61 7373 6966 6965 722c 2044 5045 7870  lassifier, DPExp
-000015c0: 6c61 696e 6162 6c65 426f 6f73 7469 6e67  lainableBoosting
-000015d0: 5265 6772 6573 736f 720a 0a64 705f 6562  Regressor..dp_eb
-000015e0: 6d20 3d20 4450 4578 706c 6169 6e61 626c  m = DPExplainabl
-000015f0: 6542 6f6f 7374 696e 6743 6c61 7373 6966  eBoostingClassif
-00001600: 6965 7228 6570 7369 6c6f 6e3d 312c 2064  ier(epsilon=1, d
-00001610: 656c 7461 3d31 652d 3529 2023 2053 7065  elta=1e-5) # Spe
-00001620: 6369 6679 2070 7269 7661 6379 2070 6172  cify privacy par
-00001630: 616d 6574 6572 730a 6470 5f65 626d 2e66  ameters.dp_ebm.f
-00001640: 6974 2858 5f74 7261 696e 2c20 795f 7472  it(X_train, y_tr
-00001650: 6169 6e29 0a0a 7368 6f77 2864 705f 6562  ain)..show(dp_eb
-00001660: 6d2e 6578 706c 6169 6e5f 676c 6f62 616c  m.explain_global
-00001670: 2829 2920 2320 4964 656e 7469 6361 6c20  ()) # Identical 
-00001680: 6675 6e63 7469 6f6e 2063 616c 6c73 2074  function calls t
-00001690: 6f20 7374 616e 6461 7264 2045 424d 730a  o standard EBMs.
-000016a0: 6060 600a 0a3c 6272 2f3e 0a3c 6272 2f3e  ```..<br/>.<br/>
-000016b0: 0a0a 466f 7220 6d6f 7265 2069 6e66 6f72  ..For more infor
-000016c0: 6d61 7469 6f6e 2c20 7365 6520 7468 6520  mation, see the 
-000016d0: 5b64 6f63 756d 656e 7461 7469 6f6e 5d28  [documentation](
-000016e0: 6874 7470 733a 2f2f 696e 7465 7270 7265  https://interpre
-000016f0: 742e 6d6c 2f64 6f63 732f 6765 7474 696e  t.ml/docs/gettin
-00001700: 672d 7374 6172 7465 642e 6874 6d6c 292e  g-started.html).
-00001710: 0a3c 6272 2f3e 0a3c 6272 2f3e 0a0a 2320  .<br/>.<br/>..# 
-00001720: 4163 6b6e 6f77 6c65 6467 656d 656e 7473  Acknowledgements
-00001730: 0a0a 496e 7465 7270 7265 744d 4c20 7761  ..InterpretML wa
-00001740: 7320 6f72 6967 696e 616c 6c79 2063 7265  s originally cre
-00001750: 6174 6564 2062 7920 2865 7175 616c 2063  ated by (equal c
-00001760: 6f6e 7472 6962 7574 696f 6e73 293a 2053  ontributions): S
-00001770: 616d 7565 6c20 4a65 6e6b 696e 732c 2048  amuel Jenkins, H
-00001780: 6172 7368 6120 4e6f 7269 2c20 5061 756c  arsha Nori, Paul
-00001790: 204b 6f63 682c 2061 6e64 2052 6963 6820   Koch, and Rich 
-000017a0: 4361 7275 616e 610a 0a45 424d 7320 6172  Caruana..EBMs ar
-000017b0: 6520 6661 7374 2064 6572 6976 6174 6976  e fast derivativ
-000017c0: 6520 6f66 2047 4132 4d2c 2069 6e76 656e  e of GA2M, inven
-000017d0: 7465 6420 6279 3a20 5969 6e20 4c6f 752c  ted by: Yin Lou,
-000017e0: 2052 6963 6820 4361 7275 616e 612c 204a   Rich Caruana, J
-000017f0: 6f68 616e 6e65 7320 4765 6872 6b65 2c20  ohannes Gehrke, 
-00001800: 616e 6420 4769 6c65 7320 486f 6f6b 6572  and Giles Hooker
-00001810: 0a0a 4d61 6e79 2070 656f 706c 6520 6861  ..Many people ha
-00001820: 7665 2073 7570 706f 7274 6564 2075 7320  ve supported us 
-00001830: 616c 6f6e 6720 7468 6520 7761 792e 2043  along the way. C
-00001840: 6865 636b 206f 7574 205b 4143 4b4e 4f57  heck out [ACKNOW
-00001850: 4c45 4447 454d 454e 5453 2e6d 645d 282e  LEDGEMENTS.md](.
-00001860: 2f41 434b 4e4f 574c 4544 4745 4d45 4e54  /ACKNOWLEDGEMENT
-00001870: 532e 6d64 2921 0a0a 5765 2061 6c73 6f20  S.md)!..We also 
-00001880: 6275 696c 6420 6f6e 2074 6f70 206f 6620  build on top of 
-00001890: 6d61 6e79 2067 7265 6174 2070 6163 6b61  many great packa
-000018a0: 6765 732e 2050 6c65 6173 6520 6368 6563  ges. Please chec
-000018b0: 6b20 7468 656d 206f 7574 210a 0a5b 706c  k them out!..[pl
-000018c0: 6f74 6c79 5d28 6874 7470 733a 2f2f 6769  otly](https://gi
-000018d0: 7468 7562 2e63 6f6d 2f70 6c6f 746c 792f  thub.com/plotly/
-000018e0: 706c 6f74 6c79 2e70 7929 207c 0a5b 6461  plotly.py) |.[da
-000018f0: 7368 5d28 6874 7470 733a 2f2f 6769 7468  sh](https://gith
-00001900: 7562 2e63 6f6d 2f70 6c6f 746c 792f 6461  ub.com/plotly/da
-00001910: 7368 2920 7c0a 5b73 6369 6b69 742d 6c65  sh) |.[scikit-le
-00001920: 6172 6e5d 2868 7474 7073 3a2f 2f67 6974  arn](https://git
-00001930: 6875 622e 636f 6d2f 7363 696b 6974 2d6c  hub.com/scikit-l
-00001940: 6561 726e 2f73 6369 6b69 742d 6c65 6172  earn/scikit-lear
-00001950: 6e29 207c 0a5b 6c69 6d65 5d28 6874 7470  n) |.[lime](http
-00001960: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00001970: 6172 636f 7463 722f 6c69 6d65 2920 7c0a  arcotcr/lime) |.
-00001980: 5b73 6861 705d 2868 7474 7073 3a2f 2f67  [shap](https://g
-00001990: 6974 6875 622e 636f 6d2f 736c 756e 6462  ithub.com/slundb
-000019a0: 6572 672f 7368 6170 2920 7c0a 5b73 616c  erg/shap) |.[sal
-000019b0: 6962 5d28 6874 7470 733a 2f2f 6769 7468  ib](https://gith
-000019c0: 7562 2e63 6f6d 2f53 414c 6962 2f53 414c  ub.com/SALib/SAL
-000019d0: 6962 2920 7c0a 5b73 6b6f 7065 2d72 756c  ib) |.[skope-rul
-000019e0: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-000019f0: 7562 2e63 6f6d 2f73 6369 6b69 742d 6c65  ub.com/scikit-le
-00001a00: 6172 6e2d 636f 6e74 7269 622f 736b 6f70  arn-contrib/skop
-00001a10: 652d 7275 6c65 7329 207c 0a5b 7472 6565  e-rules) |.[tree
-00001a20: 696e 7465 7270 7265 7465 725d 2868 7474  interpreter](htt
-00001a30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001a40: 616e 646f 7361 2f74 7265 6569 6e74 6572  andosa/treeinter
-00001a50: 7072 6574 6572 2920 7c0a 5b67 6576 656e  preter) |.[geven
-00001a60: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00001a70: 622e 636f 6d2f 6765 7665 6e74 2f67 6576  b.com/gevent/gev
-00001a80: 656e 7429 207c 0a5b 6a6f 626c 6962 5d28  ent) |.[joblib](
-00001a90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001aa0: 6f6d 2f6a 6f62 6c69 622f 6a6f 626c 6962  om/joblib/joblib
-00001ab0: 2920 7c0a 5b70 7974 6573 745d 2868 7474  ) |.[pytest](htt
-00001ac0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001ad0: 7079 7465 7374 2d64 6576 2f70 7974 6573  pytest-dev/pytes
-00001ae0: 7429 207c 0a5b 6a75 7079 7465 725d 2868  t) |.[jupyter](h
-00001af0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001b00: 6d2f 6a75 7079 7465 722f 6e6f 7465 626f  m/jupyter/notebo
-00001b10: 6f6b 290a 0a23 203c 6120 6e61 6d65 3d22  ok)..# <a name="
-00001b20: 6369 7461 7469 6f6e 7322 3e43 6974 6174  citations">Citat
-00001b30: 696f 6e73 3c2f 613e 0a0a 3c64 6574 6169  ions</a>..<detai
-00001b40: 6c73 206f 7065 6e3e 0a20 203c 7375 6d6d  ls open>.  <summ
-00001b50: 6172 793e 3c73 7472 6f6e 673e 496e 7465  ary><strong>Inte
-00001b60: 7270 7265 744d 4c3c 2f73 7472 6f6e 673e  rpretML</strong>
-00001b70: 3c2f 7375 6d6d 6172 793e 0a20 203c 6872  </summary>.  <hr
-00001b80: 2f3e 0a0a 2020 3c64 6574 6169 6c73 206f  />..  <details o
-00001b90: 7065 6e3e 0a20 2020 203c 7375 6d6d 6172  pen>.    <summar
-00001ba0: 793e 0a20 2020 2020 203c 656d 3e22 496e  y>.      <em>"In
-00001bb0: 7465 7270 7265 744d 4c3a 2041 2055 6e69  terpretML: A Uni
-00001bc0: 6669 6564 2046 7261 6d65 776f 726b 2066  fied Framework f
-00001bd0: 6f72 204d 6163 6869 6e65 204c 6561 726e  or Machine Learn
-00001be0: 696e 6720 496e 7465 7270 7265 7461 6269  ing Interpretabi
-00001bf0: 6c69 7479 2220 2848 2e20 4e6f 7269 2c20  lity" (H. Nori, 
-00001c00: 532e 204a 656e 6b69 6e73 2c20 502e 204b  S. Jenkins, P. K
-00001c10: 6f63 682c 2061 6e64 2052 2e20 4361 7275  och, and R. Caru
-00001c20: 616e 6120 3230 3139 293c 2f65 6d3e 0a20  ana 2019)</em>. 
-00001c30: 2020 203c 2f73 756d 6d61 7279 3e0a 2020     </summary>.  
-00001c40: 2020 3c62 722f 3e0a 2020 2020 3c70 7265    <br/>.    <pre
-00001c50: 3e0a 4061 7274 6963 6c65 7b6e 6f72 6932  >.@article{nori2
-00001c60: 3031 3969 6e74 6572 7072 6574 6d6c 2c0a  019interpretml,.
-00001c70: 2020 7469 746c 653d 7b49 6e74 6572 7072    title={Interpr
-00001c80: 6574 4d4c 3a20 4120 556e 6966 6965 6420  etML: A Unified 
-00001c90: 4672 616d 6577 6f72 6b20 666f 7220 4d61  Framework for Ma
-00001ca0: 6368 696e 6520 4c65 6172 6e69 6e67 2049  chine Learning I
-00001cb0: 6e74 6572 7072 6574 6162 696c 6974 797d  nterpretability}
-00001cc0: 2c0a 2020 6175 7468 6f72 3d7b 4e6f 7269  ,.  author={Nori
-00001cd0: 2c20 4861 7273 6861 2061 6e64 204a 656e  , Harsha and Jen
-00001ce0: 6b69 6e73 2c20 5361 6d75 656c 2061 6e64  kins, Samuel and
-00001cf0: 204b 6f63 682c 2050 6175 6c20 616e 6420   Koch, Paul and 
-00001d00: 4361 7275 616e 612c 2052 6963 687d 2c0a  Caruana, Rich},.
-00001d10: 2020 6a6f 7572 6e61 6c3d 7b61 7258 6976    journal={arXiv
-00001d20: 2070 7265 7072 696e 7420 6172 5869 763a   preprint arXiv:
-00001d30: 3139 3039 2e30 3932 3233 7d2c 0a20 2079  1909.09223},.  y
-00001d40: 6561 723d 7b32 3031 397d 0a7d 0a20 2020  ear={2019}.}.   
-00001d50: 203c 2f70 7265 3e0a 2020 2020 3c61 2068   </pre>.    <a h
-00001d60: 7265 663d 2268 7474 7073 3a2f 2f61 7278  ref="https://arx
-00001d70: 6976 2e6f 7267 2f70 6466 2f31 3930 392e  iv.org/pdf/1909.
-00001d80: 3039 3232 332e 7064 6622 3e50 6170 6572  09223.pdf">Paper
-00001d90: 206c 696e 6b3c 2f61 3e0a 2020 3c2f 6465   link</a>.  </de
-00001da0: 7461 696c 733e 0a0a 2020 3c68 722f 3e0a  tails>..  <hr/>.
-00001db0: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
-00001dc0: 6169 6c73 3e0a 2020 3c73 756d 6d61 7279  ails>.  <summary
-00001dd0: 3e3c 7374 726f 6e67 3e45 7870 6c61 696e  ><strong>Explain
-00001de0: 6162 6c65 2042 6f6f 7374 696e 673c 2f73  able Boosting</s
-00001df0: 7472 6f6e 673e 3c2f 7375 6d6d 6172 793e  trong></summary>
-00001e00: 0a20 203c 6872 2f3e 0a0a 2020 3c64 6574  .  <hr/>..  <det
-00001e10: 6169 6c73 3e0a 2020 2020 3c73 756d 6d61  ails>.    <summa
-00001e20: 7279 3e0a 2020 2020 2020 3c65 6d3e 2249  ry>.      <em>"I
-00001e30: 6e74 656c 6c69 6769 626c 6520 6d6f 6465  ntelligible mode
-00001e40: 6c73 2066 6f72 2068 6561 6c74 6863 6172  ls for healthcar
-00001e50: 653a 2050 7265 6469 6374 696e 6720 706e  e: Predicting pn
-00001e60: 6575 6d6f 6e69 6120 7269 736b 2061 6e64  eumonia risk and
-00001e70: 2068 6f73 7069 7461 6c20 3330 2d64 6179   hospital 30-day
-00001e80: 2072 6561 646d 6973 7369 6f6e 2220 2852   readmission" (R
-00001e90: 2e20 4361 7275 616e 612c 2059 2e20 4c6f  . Caruana, Y. Lo
-00001ea0: 752c 204a 2e20 4765 6872 6b65 2c20 502e  u, J. Gehrke, P.
-00001eb0: 204b 6f63 682c 204d 2e20 5374 7572 6d2c   Koch, M. Sturm,
-00001ec0: 2061 6e64 204e 2e20 456c 6861 6461 6420   and N. Elhadad 
-00001ed0: 3230 3135 293c 2f65 6d3e 0a20 2020 203c  2015)</em>.    <
-00001ee0: 2f73 756d 6d61 7279 3e0a 2020 2020 3c62  /summary>.    <b
-00001ef0: 722f 3e0a 2020 2020 3c70 7265 3e0a 4069  r/>.    <pre>.@i
-00001f00: 6e70 726f 6365 6564 696e 6773 7b63 6172  nproceedings{car
-00001f10: 7561 6e61 3230 3135 696e 7465 6c6c 6967  uana2015intellig
-00001f20: 6962 6c65 2c0a 2020 7469 746c 653d 7b49  ible,.  title={I
-00001f30: 6e74 656c 6c69 6769 626c 6520 6d6f 6465  ntelligible mode
-00001f40: 6c73 2066 6f72 2068 6561 6c74 6863 6172  ls for healthcar
-00001f50: 653a 2050 7265 6469 6374 696e 6720 706e  e: Predicting pn
-00001f60: 6575 6d6f 6e69 6120 7269 736b 2061 6e64  eumonia risk and
-00001f70: 2068 6f73 7069 7461 6c20 3330 2d64 6179   hospital 30-day
-00001f80: 2072 6561 646d 6973 7369 6f6e 7d2c 0a20   readmission},. 
-00001f90: 2061 7574 686f 723d 7b43 6172 7561 6e61   author={Caruana
-00001fa0: 2c20 5269 6368 2061 6e64 204c 6f75 2c20  , Rich and Lou, 
-00001fb0: 5969 6e20 616e 6420 4765 6872 6b65 2c20  Yin and Gehrke, 
-00001fc0: 4a6f 6861 6e6e 6573 2061 6e64 204b 6f63  Johannes and Koc
-00001fd0: 682c 2050 6175 6c20 616e 6420 5374 7572  h, Paul and Stur
-00001fe0: 6d2c 204d 6172 6320 616e 6420 456c 6861  m, Marc and Elha
-00001ff0: 6461 642c 204e 6f65 6d69 657d 2c0a 2020  dad, Noemie},.  
-00002000: 626f 6f6b 7469 746c 653d 7b50 726f 6365  booktitle={Proce
-00002010: 6564 696e 6773 206f 6620 7468 6520 3231  edings of the 21
-00002020: 7468 2041 434d 2053 4947 4b44 4420 496e  th ACM SIGKDD In
-00002030: 7465 726e 6174 696f 6e61 6c20 436f 6e66  ternational Conf
-00002040: 6572 656e 6365 206f 6e20 4b6e 6f77 6c65  erence on Knowle
-00002050: 6467 6520 4469 7363 6f76 6572 7920 616e  dge Discovery an
-00002060: 6420 4461 7461 204d 696e 696e 677d 2c0a  d Data Mining},.
-00002070: 2020 7061 6765 733d 7b31 3732 312d 2d31    pages={1721--1
-00002080: 3733 307d 2c0a 2020 7965 6172 3d7b 3230  730},.  year={20
-00002090: 3135 7d2c 0a20 206f 7267 616e 697a 6174  15},.  organizat
-000020a0: 696f 6e3d 7b41 434d 7d0a 7d0a 2020 2020  ion={ACM}.}.    
-000020b0: 3c2f 7072 653e 0a20 2020 203c 6120 6872  </pre>.    <a hr
-000020c0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
-000020d0: 6d69 6372 6f73 6f66 742e 636f 6d2f 656e  microsoft.com/en
-000020e0: 2d75 732f 7265 7365 6172 6368 2f77 702d  -us/research/wp-
-000020f0: 636f 6e74 656e 742f 7570 6c6f 6164 732f  content/uploads/
-00002100: 3230 3137 2f30 362f 4b44 4432 3031 3546  2017/06/KDD2015F
-00002110: 696e 616c 4472 6166 7449 6e74 656c 6c69  inalDraftIntelli
-00002120: 6769 626c 654d 6f64 656c 7334 4865 616c  gibleModels4Heal
-00002130: 7468 4361 7265 5f69 6774 3134 3365 2d63  thCare_igt143e-c
-00002140: 6172 7561 6e61 412e 7064 6622 3e50 6170  aruanaA.pdf">Pap
-00002150: 6572 206c 696e 6b3c 2f61 3e0a 2020 3c2f  er link</a>.  </
-00002160: 6465 7461 696c 733e 0a0a 2020 3c64 6574  details>..  <det
-00002170: 6169 6c73 3e0a 2020 2020 3c73 756d 6d61  ails>.    <summa
-00002180: 7279 3e0a 2020 2020 2020 3c65 6d3e 2241  ry>.      <em>"A
-00002190: 6363 7572 6174 6520 696e 7465 6c6c 6967  ccurate intellig
-000021a0: 6962 6c65 206d 6f64 656c 7320 7769 7468  ible models with
-000021b0: 2070 6169 7277 6973 6520 696e 7465 7261   pairwise intera
-000021c0: 6374 696f 6e73 2220 2859 2e20 4c6f 752c  ctions" (Y. Lou,
-000021d0: 2052 2e20 4361 7275 616e 612c 204a 2e20   R. Caruana, J. 
-000021e0: 4765 6872 6b65 2c20 616e 6420 472e 2048  Gehrke, and G. H
-000021f0: 6f6f 6b65 7220 3230 3133 293c 2f65 6d3e  ooker 2013)</em>
-00002200: 0a20 2020 203c 2f73 756d 6d61 7279 3e0a  .    </summary>.
-00002210: 2020 2020 3c62 722f 3e0a 2020 2020 3c70      <br/>.    <p
-00002220: 7265 3e0a 4069 6e70 726f 6365 6564 696e  re>.@inproceedin
-00002230: 6773 7b6c 6f75 3230 3133 6163 6375 7261  gs{lou2013accura
-00002240: 7465 2c0a 2020 7469 746c 653d 7b41 6363  te,.  title={Acc
-00002250: 7572 6174 6520 696e 7465 6c6c 6967 6962  urate intelligib
-00002260: 6c65 206d 6f64 656c 7320 7769 7468 2070  le models with p
-00002270: 6169 7277 6973 6520 696e 7465 7261 6374  airwise interact
-00002280: 696f 6e73 7d2c 0a20 2061 7574 686f 723d  ions},.  author=
-00002290: 7b4c 6f75 2c20 5969 6e20 616e 6420 4361  {Lou, Yin and Ca
-000022a0: 7275 616e 612c 2052 6963 6820 616e 6420  ruana, Rich and 
-000022b0: 4765 6872 6b65 2c20 4a6f 6861 6e6e 6573  Gehrke, Johannes
-000022c0: 2061 6e64 2048 6f6f 6b65 722c 2047 696c   and Hooker, Gil
-000022d0: 6573 7d2c 0a20 2062 6f6f 6b74 6974 6c65  es},.  booktitle
-000022e0: 3d7b 5072 6f63 6565 6469 6e67 7320 6f66  ={Proceedings of
-000022f0: 2074 6865 2031 3974 6820 4143 4d20 5349   the 19th ACM SI
-00002300: 474b 4444 2069 6e74 6572 6e61 7469 6f6e  GKDD internation
-00002310: 616c 2063 6f6e 6665 7265 6e63 6520 6f6e  al conference on
-00002320: 204b 6e6f 776c 6564 6765 2064 6973 636f   Knowledge disco
-00002330: 7665 7279 2061 6e64 2064 6174 6120 6d69  very and data mi
-00002340: 6e69 6e67 7d2c 0a20 2070 6167 6573 3d7b  ning},.  pages={
-00002350: 3632 332d 2d36 3331 7d2c 0a20 2079 6561  623--631},.  yea
-00002360: 723d 7b32 3031 337d 2c0a 2020 6f72 6761  r={2013},.  orga
-00002370: 6e69 7a61 7469 6f6e 3d7b 4143 4d7d 0a7d  nization={ACM}.}
-00002380: 0a20 2020 203c 2f70 7265 3e0a 2020 2020  .    </pre>.    
-00002390: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000023a0: 2f77 7777 2e63 732e 636f 726e 656c 6c2e  /www.cs.cornell.
-000023b0: 6564 752f 7e79 696e 6c6f 752f 7061 7065  edu/~yinlou/pape
-000023c0: 7273 2f6c 6f75 2d6b 6464 3133 2e70 6466  rs/lou-kdd13.pdf
-000023d0: 223e 5061 7065 7220 6c69 6e6b 3c2f 613e  ">Paper link</a>
-000023e0: 0a20 203c 2f64 6574 6169 6c73 3e0a 0a20  .  </details>.. 
-000023f0: 203c 6465 7461 696c 733e 0a20 2020 203c   <details>.    <
-00002400: 7375 6d6d 6172 793e 0a20 2020 2020 203c  summary>.      <
-00002410: 656d 3e22 496e 7465 6c6c 6967 6962 6c65  em>"Intelligible
-00002420: 206d 6f64 656c 7320 666f 7220 636c 6173   models for clas
-00002430: 7369 6669 6361 7469 6f6e 2061 6e64 2072  sification and r
-00002440: 6567 7265 7373 696f 6e22 2028 592e 204c  egression" (Y. L
-00002450: 6f75 2c20 522e 2043 6172 7561 6e61 2c20  ou, R. Caruana, 
-00002460: 616e 6420 4a2e 2047 6568 726b 6520 3230  and J. Gehrke 20
-00002470: 3132 293c 2f65 6d3e 0a20 2020 203c 2f73  12)</em>.    </s
-00002480: 756d 6d61 7279 3e0a 2020 2020 3c62 722f  ummary>.    <br/
-00002490: 3e0a 2020 2020 3c70 7265 3e0a 4069 6e70  >.    <pre>.@inp
-000024a0: 726f 6365 6564 696e 6773 7b6c 6f75 3230  roceedings{lou20
-000024b0: 3132 696e 7465 6c6c 6967 6962 6c65 2c0a  12intelligible,.
-000024c0: 2020 7469 746c 653d 7b49 6e74 656c 6c69    title={Intelli
-000024d0: 6769 626c 6520 6d6f 6465 6c73 2066 6f72  gible models for
-000024e0: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
-000024f0: 616e 6420 7265 6772 6573 7369 6f6e 7d2c  and regression},
-00002500: 0a20 2061 7574 686f 723d 7b4c 6f75 2c20  .  author={Lou, 
-00002510: 5969 6e20 616e 6420 4361 7275 616e 612c  Yin and Caruana,
-00002520: 2052 6963 6820 616e 6420 4765 6872 6b65   Rich and Gehrke
-00002530: 2c20 4a6f 6861 6e6e 6573 7d2c 0a20 2062  , Johannes},.  b
-00002540: 6f6f 6b74 6974 6c65 3d7b 5072 6f63 6565  ooktitle={Procee
-00002550: 6469 6e67 7320 6f66 2074 6865 2031 3874  dings of the 18t
-00002560: 6820 4143 4d20 5349 474b 4444 2069 6e74  h ACM SIGKDD int
-00002570: 6572 6e61 7469 6f6e 616c 2063 6f6e 6665  ernational confe
-00002580: 7265 6e63 6520 6f6e 204b 6e6f 776c 6564  rence on Knowled
-00002590: 6765 2064 6973 636f 7665 7279 2061 6e64  ge discovery and
-000025a0: 2064 6174 6120 6d69 6e69 6e67 7d2c 0a20   data mining},. 
-000025b0: 2070 6167 6573 3d7b 3135 302d 2d31 3538   pages={150--158
-000025c0: 7d2c 0a20 2079 6561 723d 7b32 3031 327d  },.  year={2012}
-000025d0: 2c0a 2020 6f72 6761 6e69 7a61 7469 6f6e  ,.  organization
-000025e0: 3d7b 4143 4d7d 0a7d 0a20 2020 203c 2f70  ={ACM}.}.    </p
-000025f0: 7265 3e0a 2020 2020 3c61 2068 7265 663d  re>.    <a href=
-00002600: 2268 7474 7073 3a2f 2f77 7777 2e63 732e  "https://www.cs.
-00002610: 636f 726e 656c 6c2e 6564 752f 7e79 696e  cornell.edu/~yin
-00002620: 6c6f 752f 7061 7065 7273 2f6c 6f75 2d6b  lou/papers/lou-k
-00002630: 6464 3132 2e70 6466 223e 5061 7065 7220  dd12.pdf">Paper 
-00002640: 6c69 6e6b 3c2f 613e 0a20 203c 2f64 6574  link</a>.  </det
-00002650: 6169 6c73 3e0a 0a20 203c 6465 7461 696c  ails>..  <detail
-00002660: 733e 0a20 2020 203c 7375 6d6d 6172 793e  s>.    <summary>
-00002670: 0a20 2020 2020 203c 656d 3e22 496e 7465  .      <em>"Inte
-00002680: 7270 7265 7461 6269 6c69 7479 2c20 5468  rpretability, Th
-00002690: 656e 2057 6861 743f 2045 6469 7469 6e67  en What? Editing
-000026a0: 204d 6163 6869 6e65 204c 6561 726e 696e   Machine Learnin
-000026b0: 6720 4d6f 6465 6c73 2074 6f20 5265 666c  g Models to Refl
-000026c0: 6563 7420 4875 6d61 6e20 4b6e 6f77 6c65  ect Human Knowle
-000026d0: 6467 6520 616e 6420 5661 6c75 6573 2220  dge and Values" 
-000026e0: 285a 696a 6965 204a 2e20 5761 6e67 2c20  (Zijie J. Wang, 
-000026f0: 416c 6578 204b 616c 652c 2048 6172 7368  Alex Kale, Harsh
-00002700: 6120 4e6f 7269 2c20 5065 7465 7220 5374  a Nori, Peter St
-00002710: 656c 6c61 2c20 4d61 726b 2045 2e20 4e75  ella, Mark E. Nu
-00002720: 6e6e 616c 6c79 2c20 4475 656e 2048 6f72  nnally, Duen Hor
-00002730: 6e67 2043 6861 752c 204d 6968 6165 6c61  ng Chau, Mihaela
-00002740: 2056 6f72 766f 7265 616e 752c 204a 656e   Vorvoreanu, Jen
-00002750: 6e69 6665 7220 576f 7274 6d61 6e20 5661  nifer Wortman Va
-00002760: 7567 6861 6e2c 2052 6963 6820 4361 7275  ughan, Rich Caru
-00002770: 616e 6120 3230 3232 293c 2f65 6d3e 0a20  ana 2022)</em>. 
-00002780: 2020 203c 2f73 756d 6d61 7279 3e0a 2020     </summary>.  
-00002790: 2020 3c62 722f 3e0a 2020 2020 3c70 7265    <br/>.    <pre
-000027a0: 3e0a 4061 7274 6963 6c65 7b77 616e 6732  >.@article{wang2
-000027b0: 3032 3269 6e74 6572 7072 6574 6162 696c  022interpretabil
-000027c0: 6974 792c 0a20 2074 6974 6c65 3d7b 496e  ity,.  title={In
-000027d0: 7465 7270 7265 7461 6269 6c69 7479 2c20  terpretability, 
-000027e0: 5468 656e 2057 6861 743f 2045 6469 7469  Then What? Editi
-000027f0: 6e67 204d 6163 6869 6e65 204c 6561 726e  ng Machine Learn
-00002800: 696e 6720 4d6f 6465 6c73 2074 6f20 5265  ing Models to Re
-00002810: 666c 6563 7420 4875 6d61 6e20 4b6e 6f77  flect Human Know
-00002820: 6c65 6467 6520 616e 6420 5661 6c75 6573  ledge and Values
-00002830: 7d2c 0a20 2061 7574 686f 723d 7b57 616e  },.  author={Wan
-00002840: 672c 205a 696a 6965 204a 2061 6e64 204b  g, Zijie J and K
-00002850: 616c 652c 2041 6c65 7820 616e 6420 4e6f  ale, Alex and No
-00002860: 7269 2c20 4861 7273 6861 2061 6e64 2053  ri, Harsha and S
-00002870: 7465 6c6c 612c 2050 6574 6572 2061 6e64  tella, Peter and
-00002880: 204e 756e 6e61 6c6c 792c 204d 6172 6b20   Nunnally, Mark 
-00002890: 4520 616e 6420 4368 6175 2c20 4475 656e  E and Chau, Duen
-000028a0: 2048 6f72 6e67 2061 6e64 2056 6f72 766f   Horng and Vorvo
-000028b0: 7265 616e 752c 204d 6968 6165 6c61 2061  reanu, Mihaela a
-000028c0: 6e64 2056 6175 6768 616e 2c20 4a65 6e6e  nd Vaughan, Jenn
-000028d0: 6966 6572 2057 6f72 746d 616e 2061 6e64  ifer Wortman and
-000028e0: 2043 6172 7561 6e61 2c20 5269 6368 7d2c   Caruana, Rich},
-000028f0: 0a20 206a 6f75 726e 616c 3d7b 6172 5869  .  journal={arXi
-00002900: 7620 7072 6570 7269 6e74 2061 7258 6976  v preprint arXiv
-00002910: 3a32 3230 362e 3135 3436 357d 2c0a 2020  :2206.15465},.  
-00002920: 7965 6172 3d7b 3230 3232 7d0a 7d0a 2020  year={2022}.}.  
-00002930: 2020 3c2f 7072 653e 0a20 2020 203c 6120    </pre>.    <a 
-00002940: 6872 6566 3d22 6874 7470 733a 2f2f 6172  href="https://ar
-00002950: 7869 762e 6f72 672f 7064 662f 3232 3036  xiv.org/pdf/2206
-00002960: 2e31 3534 3635 2e70 6466 223e 5061 7065  .15465.pdf">Pape
-00002970: 7220 6c69 6e6b 3c2f 613e 0a20 203c 2f64  r link</a>.  </d
-00002980: 6574 6169 6c73 3e0a 0a20 203c 6465 7461  etails>..  <deta
-00002990: 696c 733e 0a20 2020 203c 7375 6d6d 6172  ils>.    <summar
-000029a0: 793e 0a20 2020 2020 203c 656d 3e22 4178  y>.      <em>"Ax
-000029b0: 696f 6d61 7469 6320 496e 7465 7270 7265  iomatic Interpre
-000029c0: 7461 6269 6c69 7479 2066 6f72 204d 756c  tability for Mul
-000029d0: 7469 636c 6173 7320 4164 6469 7469 7665  ticlass Additive
-000029e0: 204d 6f64 656c 7322 2028 582e 205a 6861   Models" (X. Zha
-000029f0: 6e67 2c20 532e 2054 616e 2c20 502e 204b  ng, S. Tan, P. K
-00002a00: 6f63 682c 2059 2e20 4c6f 752c 2055 2e20  och, Y. Lou, U. 
-00002a10: 4368 616a 6577 736b 612c 2061 6e64 2052  Chajewska, and R
-00002a20: 2e20 4361 7275 616e 6120 3230 3139 293c  . Caruana 2019)<
-00002a30: 2f65 6d3e 0a20 2020 203c 2f73 756d 6d61  /em>.    </summa
-00002a40: 7279 3e0a 2020 2020 3c62 722f 3e0a 2020  ry>.    <br/>.  
-00002a50: 2020 3c70 7265 3e0a 4069 6e70 726f 6365    <pre>.@inproce
-00002a60: 6564 696e 6773 7b7a 6861 6e67 3230 3139  edings{zhang2019
-00002a70: 6178 696f 6d61 7469 632c 0a20 2074 6974  axiomatic,.  tit
-00002a80: 6c65 3d7b 4178 696f 6d61 7469 6320 496e  le={Axiomatic In
-00002a90: 7465 7270 7265 7461 6269 6c69 7479 2066  terpretability f
-00002aa0: 6f72 204d 756c 7469 636c 6173 7320 4164  or Multiclass Ad
-00002ab0: 6469 7469 7665 204d 6f64 656c 737d 2c0a  ditive Models},.
-00002ac0: 2020 6175 7468 6f72 3d7b 5a68 616e 672c    author={Zhang,
-00002ad0: 2058 7565 7a68 6f75 2061 6e64 2054 616e   Xuezhou and Tan
-00002ae0: 2c20 5361 7261 6820 616e 6420 4b6f 6368  , Sarah and Koch
-00002af0: 2c20 5061 756c 2061 6e64 204c 6f75 2c20  , Paul and Lou, 
-00002b00: 5969 6e20 616e 6420 4368 616a 6577 736b  Yin and Chajewsk
-00002b10: 612c 2055 7273 7a75 6c61 2061 6e64 2043  a, Urszula and C
-00002b20: 6172 7561 6e61 2c20 5269 6368 7d2c 0a20  aruana, Rich},. 
-00002b30: 2062 6f6f 6b74 6974 6c65 3d7b 5072 6f63   booktitle={Proc
-00002b40: 6565 6469 6e67 7320 6f66 2074 6865 2032  eedings of the 2
-00002b50: 3574 6820 4143 4d20 5349 474b 4444 2049  5th ACM SIGKDD I
-00002b60: 6e74 6572 6e61 7469 6f6e 616c 2043 6f6e  nternational Con
-00002b70: 6665 7265 6e63 6520 6f6e 204b 6e6f 776c  ference on Knowl
-00002b80: 6564 6765 2044 6973 636f 7665 7279 205c  edge Discovery \
-00002b90: 2620 4461 7461 204d 696e 696e 677d 2c0a  & Data Mining},.
-00002ba0: 2020 7061 6765 733d 7b32 3236 2d2d 3233    pages={226--23
-00002bb0: 347d 2c0a 2020 7965 6172 3d7b 3230 3139  4},.  year={2019
-00002bc0: 7d2c 0a20 206f 7267 616e 697a 6174 696f  },.  organizatio
-00002bd0: 6e3d 7b41 434d 7d0a 7d0a 2020 2020 3c2f  n={ACM}.}.    </
-00002be0: 7072 653e 0a20 2020 203c 6120 6872 6566  pre>.    <a href
-00002bf0: 3d22 6874 7470 733a 2f2f 6172 7869 762e  ="https://arxiv.
-00002c00: 6f72 672f 7064 662f 3138 3130 2e30 3930  org/pdf/1810.090
-00002c10: 3932 2e70 6466 223e 5061 7065 7220 6c69  92.pdf">Paper li
-00002c20: 6e6b 3c2f 613e 0a20 203c 2f64 6574 6169  nk</a>.  </detai
-00002c30: 6c73 3e0a 0a20 203c 6465 7461 696c 733e  ls>..  <details>
-00002c40: 0a20 2020 203c 7375 6d6d 6172 793e 0a20  .    <summary>. 
-00002c50: 2020 2020 203c 656d 3e22 4469 7374 696c       <em>"Distil
-00002c60: 6c2d 616e 642d 636f 6d70 6172 653a 2061  l-and-compare: a
-00002c70: 7564 6974 696e 6720 626c 6163 6b2d 626f  uditing black-bo
-00002c80: 7820 6d6f 6465 6c73 2075 7369 6e67 2074  x models using t
-00002c90: 7261 6e73 7061 7265 6e74 206d 6f64 656c  ransparent model
-00002ca0: 2064 6973 7469 6c6c 6174 696f 6e22 2028   distillation" (
-00002cb0: 532e 2054 616e 2c20 522e 2043 6172 7561  S. Tan, R. Carua
-00002cc0: 6e61 2c20 472e 2048 6f6f 6b65 722c 2061  na, G. Hooker, a
-00002cd0: 6e64 2059 2e20 4c6f 7520 3230 3138 293c  nd Y. Lou 2018)<
-00002ce0: 2f65 6d3e 0a20 2020 203c 2f73 756d 6d61  /em>.    </summa
-00002cf0: 7279 3e0a 2020 2020 3c62 722f 3e0a 2020  ry>.    <br/>.  
-00002d00: 2020 3c70 7265 3e0a 4069 6e70 726f 6365    <pre>.@inproce
-00002d10: 6564 696e 6773 7b74 616e 3230 3138 6469  edings{tan2018di
-00002d20: 7374 696c 6c2c 0a20 2074 6974 6c65 3d7b  still,.  title={
-00002d30: 4469 7374 696c 6c2d 616e 642d 636f 6d70  Distill-and-comp
-00002d40: 6172 653a 2061 7564 6974 696e 6720 626c  are: auditing bl
-00002d50: 6163 6b2d 626f 7820 6d6f 6465 6c73 2075  ack-box models u
-00002d60: 7369 6e67 2074 7261 6e73 7061 7265 6e74  sing transparent
-00002d70: 206d 6f64 656c 2064 6973 7469 6c6c 6174   model distillat
-00002d80: 696f 6e7d 2c0a 2020 6175 7468 6f72 3d7b  ion},.  author={
-00002d90: 5461 6e2c 2053 6172 6168 2061 6e64 2043  Tan, Sarah and C
-00002da0: 6172 7561 6e61 2c20 5269 6368 2061 6e64  aruana, Rich and
-00002db0: 2048 6f6f 6b65 722c 2047 696c 6573 2061   Hooker, Giles a
-00002dc0: 6e64 204c 6f75 2c20 5969 6e7d 2c0a 2020  nd Lou, Yin},.  
-00002dd0: 626f 6f6b 7469 746c 653d 7b50 726f 6365  booktitle={Proce
-00002de0: 6564 696e 6773 206f 6620 7468 6520 3230  edings of the 20
-00002df0: 3138 2041 4141 492f 4143 4d20 436f 6e66  18 AAAI/ACM Conf
-00002e00: 6572 656e 6365 206f 6e20 4149 2c20 4574  erence on AI, Et
-00002e10: 6869 6373 2c20 616e 6420 536f 6369 6574  hics, and Societ
-00002e20: 797d 2c0a 2020 7061 6765 733d 7b33 3033  y},.  pages={303
-00002e30: 2d2d 3331 307d 2c0a 2020 7965 6172 3d7b  --310},.  year={
-00002e40: 3230 3138 7d2c 0a20 206f 7267 616e 697a  2018},.  organiz
-00002e50: 6174 696f 6e3d 7b41 434d 7d0a 7d0a 2020  ation={ACM}.}.  
-00002e60: 2020 3c2f 7072 653e 0a20 2020 203c 6120    </pre>.    <a 
-00002e70: 6872 6566 3d22 6874 7470 733a 2f2f 6172  href="https://ar
-00002e80: 7869 762e 6f72 672f 7064 662f 3137 3130  xiv.org/pdf/1710
-00002e90: 2e30 3631 3639 223e 5061 7065 7220 6c69  .06169">Paper li
-00002ea0: 6e6b 3c2f 613e 0a20 203c 2f64 6574 6169  nk</a>.  </detai
-00002eb0: 6c73 3e0a 0a20 203c 6465 7461 696c 733e  ls>..  <details>
-00002ec0: 0a20 2020 203c 7375 6d6d 6172 793e 0a20  .    <summary>. 
-00002ed0: 2020 2020 203c 656d 3e22 5075 7269 6679       <em>"Purify
-00002ee0: 696e 6720 496e 7465 7261 6374 696f 6e20  ing Interaction 
-00002ef0: 4566 6665 6374 7320 7769 7468 2074 6865  Effects with the
-00002f00: 2046 756e 6374 696f 6e61 6c20 414e 4f56   Functional ANOV
-00002f10: 413a 2041 6e20 4566 6669 6369 656e 7420  A: An Efficient 
-00002f20: 416c 676f 7269 7468 6d20 666f 7220 5265  Algorithm for Re
-00002f30: 636f 7665 7269 6e67 2049 6465 6e74 6966  covering Identif
-00002f40: 6961 626c 6520 4164 6469 7469 7665 204d  iable Additive M
-00002f50: 6f64 656c 7322 2028 422e 204c 656e 6765  odels" (B. Lenge
-00002f60: 7269 6368 2c20 532e 2054 616e 2c20 432e  rich, S. Tan, C.
-00002f70: 2043 6861 6e67 2c20 472e 2048 6f6f 6b65   Chang, G. Hooke
-00002f80: 722c 2052 2e20 4361 7275 616e 6120 3230  r, R. Caruana 20
-00002f90: 3139 293c 2f65 6d3e 0a20 2020 203c 2f73  19)</em>.    </s
-00002fa0: 756d 6d61 7279 3e0a 2020 2020 3c62 722f  ummary>.    <br/
-00002fb0: 3e0a 2020 2020 3c70 7265 3e0a 4061 7274  >.    <pre>.@art
-00002fc0: 6963 6c65 7b6c 656e 6765 7269 6368 3230  icle{lengerich20
-00002fd0: 3139 7075 7269 6679 696e 672c 0a20 2074  19purifying,.  t
-00002fe0: 6974 6c65 3d7b 5075 7269 6679 696e 6720  itle={Purifying 
-00002ff0: 496e 7465 7261 6374 696f 6e20 4566 6665  Interaction Effe
-00003000: 6374 7320 7769 7468 2074 6865 2046 756e  cts with the Fun
-00003010: 6374 696f 6e61 6c20 414e 4f56 413a 2041  ctional ANOVA: A
-00003020: 6e20 4566 6669 6369 656e 7420 416c 676f  n Efficient Algo
-00003030: 7269 7468 6d20 666f 7220 5265 636f 7665  rithm for Recove
-00003040: 7269 6e67 2049 6465 6e74 6966 6961 626c  ring Identifiabl
-00003050: 6520 4164 6469 7469 7665 204d 6f64 656c  e Additive Model
-00003060: 737d 2c0a 2020 6175 7468 6f72 3d7b 4c65  s},.  author={Le
-00003070: 6e67 6572 6963 682c 2042 656e 6a61 6d69  ngerich, Benjami
-00003080: 6e20 616e 6420 5461 6e2c 2053 6172 6168  n and Tan, Sarah
-00003090: 2061 6e64 2043 6861 6e67 2c20 4368 756e   and Chang, Chun
-000030a0: 2d48 616f 2061 6e64 2048 6f6f 6b65 722c  -Hao and Hooker,
-000030b0: 2047 696c 6573 2061 6e64 2043 6172 7561   Giles and Carua
-000030c0: 6e61 2c20 5269 6368 7d2c 0a20 206a 6f75  na, Rich},.  jou
-000030d0: 726e 616c 3d7b 6172 5869 7620 7072 6570  rnal={arXiv prep
-000030e0: 7269 6e74 2061 7258 6976 3a31 3931 312e  rint arXiv:1911.
-000030f0: 3034 3937 347d 2c0a 2020 7965 6172 3d7b  04974},.  year={
-00003100: 3230 3139 7d0a 7d0a 2020 2020 3c2f 7072  2019}.}.    </pr
-00003110: 653e 0a20 2020 203c 6120 6872 6566 3d22  e>.    <a href="
-00003120: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00003130: 672f 7064 662f 3139 3131 2e30 3439 3734  g/pdf/1911.04974
-00003140: 2e70 6466 223e 5061 7065 7220 6c69 6e6b  .pdf">Paper link
-00003150: 3c2f 613e 0a20 203c 2f64 6574 6169 6c73  </a>.  </details
-00003160: 3e0a 0a20 203c 6465 7461 696c 733e 0a20  >..  <details>. 
-00003170: 2020 203c 7375 6d6d 6172 793e 0a20 2020     <summary>.   
-00003180: 2020 203c 656d 3e22 496e 7465 7270 7265     <em>"Interpre
-00003190: 7469 6e67 2049 6e74 6572 7072 6574 6162  ting Interpretab
-000031a0: 696c 6974 793a 2055 6e64 6572 7374 616e  ility: Understan
-000031b0: 6469 6e67 2044 6174 6120 5363 6965 6e74  ding Data Scient
-000031c0: 6973 7473 2720 5573 6520 6f66 2049 6e74  ists' Use of Int
-000031d0: 6572 7072 6574 6162 696c 6974 7920 546f  erpretability To
-000031e0: 6f6c 7320 666f 7220 4d61 6368 696e 6520  ols for Machine 
-000031f0: 4c65 6172 6e69 6e67 2220 2848 2e20 4b61  Learning" (H. Ka
-00003200: 7572 2c20 482e 204e 6f72 692c 2053 2e20  ur, H. Nori, S. 
-00003210: 4a65 6e6b 696e 732c 2052 2e20 4361 7275  Jenkins, R. Caru
-00003220: 616e 612c 2048 2e20 5761 6c6c 6163 682c  ana, H. Wallach,
-00003230: 204a 2e20 576f 7274 6d61 6e20 5661 7567   J. Wortman Vaug
-00003240: 6861 6e20 3230 3230 293c 2f65 6d3e 0a20  han 2020)</em>. 
-00003250: 2020 203c 2f73 756d 6d61 7279 3e0a 2020     </summary>.  
-00003260: 2020 3c62 722f 3e0a 2020 2020 3c70 7265    <br/>.    <pre
-00003270: 3e0a 4069 6e70 726f 6365 6564 696e 6773  >.@inproceedings
-00003280: 7b6b 6175 7232 3032 3069 6e74 6572 7072  {kaur2020interpr
-00003290: 6574 696e 672c 0a20 2074 6974 6c65 3d7b  eting,.  title={
-000032a0: 496e 7465 7270 7265 7469 6e67 2049 6e74  Interpreting Int
-000032b0: 6572 7072 6574 6162 696c 6974 793a 2055  erpretability: U
-000032c0: 6e64 6572 7374 616e 6469 6e67 2044 6174  nderstanding Dat
-000032d0: 6120 5363 6965 6e74 6973 7473 2720 5573  a Scientists' Us
-000032e0: 6520 6f66 2049 6e74 6572 7072 6574 6162  e of Interpretab
-000032f0: 696c 6974 7920 546f 6f6c 7320 666f 7220  ility Tools for 
-00003300: 4d61 6368 696e 6520 4c65 6172 6e69 6e67  Machine Learning
-00003310: 7d2c 0a20 2061 7574 686f 723d 7b4b 6175  },.  author={Kau
-00003320: 722c 2048 6172 6d61 6e70 7265 6574 2061  r, Harmanpreet a
-00003330: 6e64 204e 6f72 692c 2048 6172 7368 6120  nd Nori, Harsha 
-00003340: 616e 6420 4a65 6e6b 696e 732c 2053 616d  and Jenkins, Sam
-00003350: 7565 6c20 616e 6420 4361 7275 616e 612c  uel and Caruana,
-00003360: 2052 6963 6820 616e 6420 5761 6c6c 6163   Rich and Wallac
-00003370: 682c 2048 616e 6e61 2061 6e64 2057 6f72  h, Hanna and Wor
-00003380: 746d 616e 2056 6175 6768 616e 2c20 4a65  tman Vaughan, Je
-00003390: 6e6e 6966 6572 7d2c 0a20 2062 6f6f 6b74  nnifer},.  bookt
-000033a0: 6974 6c65 3d7b 5072 6f63 6565 6469 6e67  itle={Proceeding
-000033b0: 7320 6f66 2074 6865 2032 3032 3020 4348  s of the 2020 CH
-000033c0: 4920 436f 6e66 6572 656e 6365 206f 6e20  I Conference on 
-000033d0: 4875 6d61 6e20 4661 6374 6f72 7320 696e  Human Factors in
-000033e0: 2043 6f6d 7075 7469 6e67 2053 7973 7465   Computing Syste
-000033f0: 6d73 7d2c 0a20 2070 6167 6573 3d7b 312d  ms},.  pages={1-
-00003400: 2d31 347d 2c0a 2020 7965 6172 3d7b 3230  -14},.  year={20
-00003410: 3230 7d0a 7d0a 2020 2020 3c2f 7072 653e  20}.}.    </pre>
-00003420: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00003430: 7470 733a 2f2f 7777 772e 6d69 6372 6f73  tps://www.micros
-00003440: 6f66 742e 636f 6d2f 656e 2d75 732f 7265  oft.com/en-us/re
-00003450: 7365 6172 6368 2f70 7562 6c69 6361 7469  search/publicati
-00003460: 6f6e 2f69 6e74 6572 7072 6574 696e 672d  on/interpreting-
-00003470: 696e 7465 7270 7265 7461 6269 6c69 7479  interpretability
-00003480: 2d75 6e64 6572 7374 616e 6469 6e67 2d64  -understanding-d
-00003490: 6174 612d 7363 6965 6e74 6973 7473 2d75  ata-scientists-u
-000034a0: 7365 2d6f 662d 696e 7465 7270 7265 7461  se-of-interpreta
-000034b0: 6269 6c69 7479 2d74 6f6f 6c73 2d66 6f72  bility-tools-for
-000034c0: 2d6d 6163 6869 6e65 2d6c 6561 726e 696e  -machine-learnin
-000034d0: 672f 223e 5061 7065 7220 6c69 6e6b 3c2f  g/">Paper link</
-000034e0: 613e 0a20 203c 2f64 6574 6169 6c73 3e0a  a>.  </details>.
-000034f0: 0a20 203c 6465 7461 696c 733e 0a20 2020  .  <details>.   
-00003500: 203c 7375 6d6d 6172 793e 0a20 2020 2020   <summary>.     
-00003510: 203c 656d 3e22 486f 7720 496e 7465 7270   <em>"How Interp
-00003520: 7265 7461 626c 6520 616e 6420 5472 7573  retable and Trus
-00003530: 7477 6f72 7468 7920 6172 6520 4741 4d73  tworthy are GAMs
-00003540: 3f22 2028 432e 2043 6861 6e67 2c20 532e  ?" (C. Chang, S.
-00003550: 2054 616e 2c20 422e 204c 656e 6765 7269   Tan, B. Lengeri
-00003560: 6368 2c20 412e 2047 6f6c 6465 6e62 6572  ch, A. Goldenber
-00003570: 672c 2052 2e20 4361 7275 616e 6120 3230  g, R. Caruana 20
-00003580: 3230 293c 2f65 6d3e 0a20 2020 203c 2f73  20)</em>.    </s
-00003590: 756d 6d61 7279 3e0a 2020 2020 3c62 722f  ummary>.    <br/
-000035a0: 3e0a 2020 2020 3c70 7265 3e0a 4061 7274  >.    <pre>.@art
-000035b0: 6963 6c65 7b63 6861 6e67 3230 3230 696e  icle{chang2020in
-000035c0: 7465 7270 7265 7461 626c 652c 0a20 2074  terpretable,.  t
-000035d0: 6974 6c65 3d7b 486f 7720 496e 7465 7270  itle={How Interp
-000035e0: 7265 7461 626c 6520 616e 6420 5472 7573  retable and Trus
-000035f0: 7477 6f72 7468 7920 6172 6520 4741 4d73  tworthy are GAMs
-00003600: 3f7d 2c0a 2020 6175 7468 6f72 3d7b 4368  ?},.  author={Ch
-00003610: 616e 672c 2043 6875 6e2d 4861 6f20 616e  ang, Chun-Hao an
-00003620: 6420 5461 6e2c 2053 6172 6168 2061 6e64  d Tan, Sarah and
-00003630: 204c 656e 6765 7269 6368 2c20 4265 6e20   Lengerich, Ben 
-00003640: 616e 6420 476f 6c64 656e 6265 7267 2c20  and Goldenberg, 
-00003650: 416e 6e61 2061 6e64 2043 6172 7561 6e61  Anna and Caruana
-00003660: 2c20 5269 6368 7d2c 0a20 206a 6f75 726e  , Rich},.  journ
-00003670: 616c 3d7b 6172 5869 7620 7072 6570 7269  al={arXiv prepri
-00003680: 6e74 2061 7258 6976 3a32 3030 362e 3036  nt arXiv:2006.06
-00003690: 3436 367d 2c0a 2020 7965 6172 3d7b 3230  466},.  year={20
-000036a0: 3230 7d0a 7d0a 2020 2020 3c2f 7072 653e  20}.}.    </pre>
-000036b0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-000036c0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-000036d0: 7064 662f 3230 3036 2e30 3634 3636 2e70  pdf/2006.06466.p
-000036e0: 6466 223e 5061 7065 7220 6c69 6e6b 3c2f  df">Paper link</
-000036f0: 613e 0a20 203c 2f64 6574 6169 6c73 3e0a  a>.  </details>.
-00003700: 0a20 203c 6872 2f3e 0a3c 2f64 6574 6169  .  <hr/>.</detai
-00003710: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a20  ls>..<details>. 
-00003720: 203c 7375 6d6d 6172 793e 3c73 7472 6f6e   <summary><stron
-00003730: 673e 4469 6666 6572 656e 7469 616c 2050  g>Differential P
-00003740: 7269 7661 6379 3c2f 7374 726f 6e67 3e3c  rivacy</strong><
-00003750: 2f73 756d 6d61 7279 3e0a 2020 3c68 722f  /summary>.  <hr/
-00003760: 3e0a 0a20 203c 6465 7461 696c 733e 0a20  >..  <details>. 
-00003770: 2020 203c 7375 6d6d 6172 793e 0a20 2020     <summary>.   
-00003780: 2020 203c 656d 3e22 4163 6375 7261 6379     <em>"Accuracy
-00003790: 2c20 496e 7465 7270 7265 7461 6269 6c69  , Interpretabili
-000037a0: 7479 2c20 616e 6420 4469 6666 6572 656e  ty, and Differen
-000037b0: 7469 616c 2050 7269 7661 6379 2076 6961  tial Privacy via
-000037c0: 2045 7870 6c61 696e 6162 6c65 2042 6f6f   Explainable Boo
-000037d0: 7374 696e 6722 2028 482e 204e 6f72 692c  sting" (H. Nori,
-000037e0: 2052 2e20 4361 7275 616e 612c 205a 2e20   R. Caruana, Z. 
-000037f0: 4275 2c20 4a2e 2053 6865 6e2c 204a 2e20  Bu, J. Shen, J. 
-00003800: 4b75 6c6b 6172 6e69 2032 3032 3129 3c2f  Kulkarni 2021)</
-00003810: 656d 3e0a 2020 2020 3c2f 7375 6d6d 6172  em>.    </summar
-00003820: 793e 0a20 2020 203c 6272 2f3e 0a20 2020  y>.    <br/>.   
-00003830: 203c 7072 653e 0a40 696e 7072 6f63 6565   <pre>.@inprocee
-00003840: 6469 6e67 737b 706d 6c72 2d76 3133 392d  dings{pmlr-v139-
-00003850: 6e6f 7269 3231 612c 0a20 2074 6974 6c65  nori21a,.  title
-00003860: 203d 2009 207b 4163 6375 7261 6379 2c20   = . {Accuracy, 
-00003870: 496e 7465 7270 7265 7461 6269 6c69 7479  Interpretability
-00003880: 2c20 616e 6420 4469 6666 6572 656e 7469  , and Differenti
-00003890: 616c 2050 7269 7661 6379 2076 6961 2045  al Privacy via E
-000038a0: 7870 6c61 696e 6162 6c65 2042 6f6f 7374  xplainable Boost
-000038b0: 696e 677d 2c0a 2020 6175 7468 6f72 203d  ing},.  author =
-000038c0: 2020 2020 2020 207b 4e6f 7269 2c20 4861         {Nori, Ha
-000038d0: 7273 6861 2061 6e64 2043 6172 7561 6e61  rsha and Caruana
-000038e0: 2c20 5269 6368 2061 6e64 2042 752c 205a  , Rich and Bu, Z
-000038f0: 6869 7169 2061 6e64 2053 6865 6e2c 204a  hiqi and Shen, J
-00003900: 7564 7920 4861 6e77 656e 2061 6e64 204b  udy Hanwen and K
-00003910: 756c 6b61 726e 692c 204a 616e 6172 6468  ulkarni, Janardh
-00003920: 616e 7d2c 0a20 2062 6f6f 6b74 6974 6c65  an},.  booktitle
-00003930: 203d 2009 207b 5072 6f63 6565 6469 6e67   = . {Proceeding
-00003940: 7320 6f66 2074 6865 2033 3874 6820 496e  s of the 38th In
-00003950: 7465 726e 6174 696f 6e61 6c20 436f 6e66  ternational Conf
-00003960: 6572 656e 6365 206f 6e20 4d61 6368 696e  erence on Machin
-00003970: 6520 4c65 6172 6e69 6e67 7d2c 0a20 2070  e Learning},.  p
-00003980: 6167 6573 203d 2009 207b 3832 3237 2d2d  ages = . {8227--
-00003990: 3832 3337 7d2c 0a20 2079 6561 7220 3d20  8237},.  year = 
-000039a0: 0920 7b32 3032 317d 2c0a 2020 766f 6c75  . {2021},.  volu
-000039b0: 6d65 203d 2009 207b 3133 397d 2c0a 2020  me = . {139},.  
-000039c0: 7365 7269 6573 203d 2009 207b 5072 6f63  series = . {Proc
-000039d0: 6565 6469 6e67 7320 6f66 204d 6163 6869  eedings of Machi
-000039e0: 6e65 204c 6561 726e 696e 6720 5265 7365  ne Learning Rese
-000039f0: 6172 6368 7d2c 0a20 2070 7562 6c69 7368  arch},.  publish
-00003a00: 6572 203d 2020 2020 7b50 4d4c 527d 0a7d  er =    {PMLR}.}
-00003a10: 0a20 2020 203c 2f70 7265 3e0a 2020 2020  .    </pre>.    
-00003a20: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00003a30: 2f70 726f 6365 6564 696e 6773 2e6d 6c72  /proceedings.mlr
-00003a40: 2e70 7265 7373 2f76 3133 392f 6e6f 7269  .press/v139/nori
-00003a50: 3231 612f 6e6f 7269 3231 612e 7064 6622  21a/nori21a.pdf"
-00003a60: 3e50 6170 6572 206c 696e 6b3c 2f61 3e0a  >Paper link</a>.
-00003a70: 2020 3c2f 6465 7461 696c 733e 0a0a 2020    </details>..  
-00003a80: 3c68 722f 3e0a 3c2f 6465 7461 696c 733e  <hr/>.</details>
-00003a90: 0a0a 3c64 6574 6169 6c73 3e0a 2020 3c73  ..<details>.  <s
-00003aa0: 756d 6d61 7279 3e3c 7374 726f 6e67 3e4c  ummary><strong>L
-00003ab0: 494d 453c 2f73 7472 6f6e 673e 3c2f 7375  IME</strong></su
-00003ac0: 6d6d 6172 793e 0a20 203c 6872 2f3e 0a0a  mmary>.  <hr/>..
-00003ad0: 2020 3c64 6574 6169 6c73 3e0a 2020 2020    <details>.    
-00003ae0: 3c73 756d 6d61 7279 3e0a 2020 2020 2020  <summary>.      
-00003af0: 3c65 6d3e 2257 6879 2073 686f 756c 6420  <em>"Why should 
-00003b00: 6920 7472 7573 7420 796f 753f 3a20 4578  i trust you?: Ex
-00003b10: 706c 6169 6e69 6e67 2074 6865 2070 7265  plaining the pre
-00003b20: 6469 6374 696f 6e73 206f 6620 616e 7920  dictions of any 
-00003b30: 636c 6173 7369 6669 6572 2220 284d 2e20  classifier" (M. 
-00003b40: 542e 2052 6962 6569 726f 2c20 532e 2053  T. Ribeiro, S. S
-00003b50: 696e 6768 2c20 616e 6420 432e 2047 7565  ingh, and C. Gue
-00003b60: 7374 7269 6e20 3230 3136 293c 2f65 6d3e  strin 2016)</em>
-00003b70: 0a20 2020 203c 2f73 756d 6d61 7279 3e0a  .    </summary>.
-00003b80: 2020 2020 3c62 722f 3e0a 2020 2020 3c70      <br/>.    <p
-00003b90: 7265 3e0a 4069 6e70 726f 6365 6564 696e  re>.@inproceedin
-00003ba0: 6773 7b72 6962 6569 726f 3230 3136 7368  gs{ribeiro2016sh
-00003bb0: 6f75 6c64 2c0a 2020 7469 746c 653d 7b57  ould,.  title={W
-00003bc0: 6879 2073 686f 756c 6420 6920 7472 7573  hy should i trus
-00003bd0: 7420 796f 753f 3a20 4578 706c 6169 6e69  t you?: Explaini
-00003be0: 6e67 2074 6865 2070 7265 6469 6374 696f  ng the predictio
-00003bf0: 6e73 206f 6620 616e 7920 636c 6173 7369  ns of any classi
-00003c00: 6669 6572 7d2c 0a20 2061 7574 686f 723d  fier},.  author=
-00003c10: 7b52 6962 6569 726f 2c20 4d61 7263 6f20  {Ribeiro, Marco 
-00003c20: 5475 6c69 6f20 616e 6420 5369 6e67 682c  Tulio and Singh,
-00003c30: 2053 616d 6565 7220 616e 6420 4775 6573   Sameer and Gues
-00003c40: 7472 696e 2c20 4361 726c 6f73 7d2c 0a20  trin, Carlos},. 
-00003c50: 2062 6f6f 6b74 6974 6c65 3d7b 5072 6f63   booktitle={Proc
-00003c60: 6565 6469 6e67 7320 6f66 2074 6865 2032  eedings of the 2
-00003c70: 326e 6420 4143 4d20 5349 474b 4444 2069  2nd ACM SIGKDD i
-00003c80: 6e74 6572 6e61 7469 6f6e 616c 2063 6f6e  nternational con
-00003c90: 6665 7265 6e63 6520 6f6e 206b 6e6f 776c  ference on knowl
-00003ca0: 6564 6765 2064 6973 636f 7665 7279 2061  edge discovery a
-00003cb0: 6e64 2064 6174 6120 6d69 6e69 6e67 7d2c  nd data mining},
-00003cc0: 0a20 2070 6167 6573 3d7b 3131 3335 2d2d  .  pages={1135--
-00003cd0: 3131 3434 7d2c 0a20 2079 6561 723d 7b32  1144},.  year={2
-00003ce0: 3031 367d 2c0a 2020 6f72 6761 6e69 7a61  016},.  organiza
-00003cf0: 7469 6f6e 3d7b 4143 4d7d 0a7d 0a20 2020  tion={ACM}.}.   
-00003d00: 203c 2f70 7265 3e0a 2020 2020 3c61 2068   </pre>.    <a h
-00003d10: 7265 663d 2268 7474 7073 3a2f 2f61 7278  ref="https://arx
-00003d20: 6976 2e6f 7267 2f70 6466 2f31 3630 322e  iv.org/pdf/1602.
-00003d30: 3034 3933 382e 7064 6622 3e50 6170 6572  04938.pdf">Paper
-00003d40: 206c 696e 6b3c 2f61 3e0a 2020 3c2f 6465   link</a>.  </de
-00003d50: 7461 696c 733e 0a0a 2020 3c68 722f 3e0a  tails>..  <hr/>.
-00003d60: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
-00003d70: 6169 6c73 3e0a 2020 3c73 756d 6d61 7279  ails>.  <summary
-00003d80: 3e3c 7374 726f 6e67 3e53 4841 503c 2f73  ><strong>SHAP</s
-00003d90: 7472 6f6e 673e 3c2f 7375 6d6d 6172 793e  trong></summary>
-00003da0: 0a20 203c 6872 2f3e 0a0a 2020 3c64 6574  .  <hr/>..  <det
-00003db0: 6169 6c73 3e0a 2020 2020 3c73 756d 6d61  ails>.    <summa
-00003dc0: 7279 3e0a 2020 2020 2020 3c65 6d3e 2241  ry>.      <em>"A
-00003dd0: 2055 6e69 6669 6564 2041 7070 726f 6163   Unified Approac
-00003de0: 6820 746f 2049 6e74 6572 7072 6574 696e  h to Interpretin
-00003df0: 6720 4d6f 6465 6c20 5072 6564 6963 7469  g Model Predicti
-00003e00: 6f6e 7322 2028 532e 204d 2e20 4c75 6e64  ons" (S. M. Lund
-00003e10: 6265 7267 2061 6e64 2053 2e2d 492e 204c  berg and S.-I. L
-00003e20: 6565 2032 3031 3729 3c2f 656d 3e0a 2020  ee 2017)</em>.  
-00003e30: 2020 3c2f 7375 6d6d 6172 793e 0a20 2020    </summary>.   
-00003e40: 203c 6272 2f3e 0a20 2020 203c 7072 653e   <br/>.    <pre>
-00003e50: 0a40 696e 636f 6c6c 6563 7469 6f6e 7b4e  .@incollection{N
-00003e60: 4950 5332 3031 375f 3730 3632 2c0a 2074  IPS2017_7062,. t
-00003e70: 6974 6c65 203d 207b 4120 556e 6966 6965  itle = {A Unifie
-00003e80: 6420 4170 7072 6f61 6368 2074 6f20 496e  d Approach to In
-00003e90: 7465 7270 7265 7469 6e67 204d 6f64 656c  terpreting Model
-00003ea0: 2050 7265 6469 6374 696f 6e73 7d2c 0a20   Predictions},. 
-00003eb0: 6175 7468 6f72 203d 207b 4c75 6e64 6265  author = {Lundbe
-00003ec0: 7267 2c20 5363 6f74 7420 4d20 616e 6420  rg, Scott M and 
-00003ed0: 4c65 652c 2053 752d 496e 7d2c 0a20 626f  Lee, Su-In},. bo
-00003ee0: 6f6b 7469 746c 6520 3d20 7b41 6476 616e  oktitle = {Advan
-00003ef0: 6365 7320 696e 204e 6575 7261 6c20 496e  ces in Neural In
-00003f00: 666f 726d 6174 696f 6e20 5072 6f63 6573  formation Proces
-00003f10: 7369 6e67 2053 7973 7465 6d73 2033 307d  sing Systems 30}
-00003f20: 2c0a 2065 6469 746f 7220 3d20 7b49 2e20  ,. editor = {I. 
-00003f30: 4775 796f 6e20 616e 6420 552e 2056 2e20  Guyon and U. V. 
-00003f40: 4c75 7862 7572 6720 616e 6420 532e 2042  Luxburg and S. B
-00003f50: 656e 6769 6f20 616e 6420 482e 2057 616c  engio and H. Wal
-00003f60: 6c61 6368 2061 6e64 2052 2e20 4665 7267  lach and R. Ferg
-00003f70: 7573 2061 6e64 2053 2e20 5669 7368 7761  us and S. Vishwa
-00003f80: 6e61 7468 616e 2061 6e64 2052 2e20 4761  nathan and R. Ga
-00003f90: 726e 6574 747d 2c0a 2070 6167 6573 203d  rnett},. pages =
-00003fa0: 207b 3437 3635 2d2d 3437 3734 7d2c 0a20   {4765--4774},. 
-00003fb0: 7965 6172 203d 207b 3230 3137 7d2c 0a20  year = {2017},. 
-00003fc0: 7075 626c 6973 6865 7220 3d20 7b43 7572  publisher = {Cur
-00003fd0: 7261 6e20 4173 736f 6369 6174 6573 2c20  ran Associates, 
-00003fe0: 496e 632e 7d2c 0a20 7572 6c20 3d20 7b68  Inc.},. url = {h
-00003ff0: 7474 7073 3a2f 2f70 6170 6572 732e 6e69  ttps://papers.ni
-00004000: 7073 2e63 632f 7061 7065 722f 3730 3632  ps.cc/paper/7062
-00004010: 2d61 2d75 6e69 6669 6564 2d61 7070 726f  -a-unified-appro
-00004020: 6163 682d 746f 2d69 6e74 6572 7072 6574  ach-to-interpret
-00004030: 696e 672d 6d6f 6465 6c2d 7072 6564 6963  ing-model-predic
-00004040: 7469 6f6e 732e 7064 667d 0a7d 0a20 2020  tions.pdf}.}.   
-00004050: 203c 2f70 7265 3e0a 2020 2020 3c61 2068   </pre>.    <a h
-00004060: 7265 663d 2268 7474 7073 3a2f 2f70 6170  ref="https://pap
-00004070: 6572 732e 6e69 7073 2e63 632f 7061 7065  ers.nips.cc/pape
-00004080: 722f 3730 3632 2d61 2d75 6e69 6669 6564  r/7062-a-unified
-00004090: 2d61 7070 726f 6163 682d 746f 2d69 6e74  -approach-to-int
-000040a0: 6572 7072 6574 696e 672d 6d6f 6465 6c2d  erpreting-model-
-000040b0: 7072 6564 6963 7469 6f6e 732e 7064 6622  predictions.pdf"
-000040c0: 3e50 6170 6572 206c 696e 6b3c 2f61 3e0a  >Paper link</a>.
-000040d0: 2020 3c2f 6465 7461 696c 733e 0a0a 2020    </details>..  
-000040e0: 3c64 6574 6169 6c73 3e0a 2020 2020 3c73  <details>.    <s
-000040f0: 756d 6d61 7279 3e0a 2020 2020 2020 3c65  ummary>.      <e
-00004100: 6d3e 2243 6f6e 7369 7374 656e 7420 696e  m>"Consistent in
-00004110: 6469 7669 6475 616c 697a 6564 2066 6561  dividualized fea
-00004120: 7475 7265 2061 7474 7269 6275 7469 6f6e  ture attribution
-00004130: 2066 6f72 2074 7265 6520 656e 7365 6d62   for tree ensemb
-00004140: 6c65 7322 2028 4c75 6e64 6265 7267 2c20  les" (Lundberg, 
-00004150: 5363 6f74 7420 4d20 616e 6420 4572 696f  Scott M and Erio
-00004160: 6e2c 2047 6162 7269 656c 2047 2061 6e64  n, Gabriel G and
-00004170: 204c 6565 2c20 5375 2d49 6e20 3230 3138   Lee, Su-In 2018
-00004180: 293c 2f65 6d3e 0a20 2020 203c 2f73 756d  )</em>.    </sum
-00004190: 6d61 7279 3e0a 2020 2020 3c62 722f 3e0a  mary>.    <br/>.
-000041a0: 2020 2020 3c70 7265 3e0a 4061 7274 6963      <pre>.@artic
-000041b0: 6c65 7b6c 756e 6462 6572 6732 3031 3863  le{lundberg2018c
-000041c0: 6f6e 7369 7374 656e 742c 0a20 2074 6974  onsistent,.  tit
-000041d0: 6c65 3d7b 436f 6e73 6973 7465 6e74 2069  le={Consistent i
-000041e0: 6e64 6976 6964 7561 6c69 7a65 6420 6665  ndividualized fe
-000041f0: 6174 7572 6520 6174 7472 6962 7574 696f  ature attributio
-00004200: 6e20 666f 7220 7472 6565 2065 6e73 656d  n for tree ensem
-00004210: 626c 6573 7d2c 0a20 2061 7574 686f 723d  bles},.  author=
-00004220: 7b4c 756e 6462 6572 672c 2053 636f 7474  {Lundberg, Scott
-00004230: 204d 2061 6e64 2045 7269 6f6e 2c20 4761   M and Erion, Ga
-00004240: 6272 6965 6c20 4720 616e 6420 4c65 652c  briel G and Lee,
-00004250: 2053 752d 496e 7d2c 0a20 206a 6f75 726e   Su-In},.  journ
-00004260: 616c 3d7b 6172 5869 7620 7072 6570 7269  al={arXiv prepri
-00004270: 6e74 2061 7258 6976 3a31 3830 322e 3033  nt arXiv:1802.03
-00004280: 3838 387d 2c0a 2020 7965 6172 3d7b 3230  888},.  year={20
-00004290: 3138 7d0a 7d0a 2020 2020 3c2f 7072 653e  18}.}.    </pre>
-000042a0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-000042b0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-000042c0: 7064 662f 3138 3032 2e30 3338 3838 223e  pdf/1802.03888">
-000042d0: 5061 7065 7220 6c69 6e6b 3c2f 613e 0a20  Paper link</a>. 
-000042e0: 203c 2f64 6574 6169 6c73 3e0a 0a20 203c   </details>..  <
-000042f0: 6465 7461 696c 733e 0a20 2020 203c 7375  details>.    <su
-00004300: 6d6d 6172 793e 0a20 2020 2020 203c 656d  mmary>.      <em
-00004310: 3e22 4578 706c 6169 6e61 626c 6520 6d61  >"Explainable ma
-00004320: 6368 696e 652d 6c65 6172 6e69 6e67 2070  chine-learning p
-00004330: 7265 6469 6374 696f 6e73 2066 6f72 2074  redictions for t
-00004340: 6865 2070 7265 7665 6e74 696f 6e20 6f66  he prevention of
-00004350: 2068 7970 6f78 6165 6d69 6120 6475 7269   hypoxaemia duri
-00004360: 6e67 2073 7572 6765 7279 2220 2853 2e20  ng surgery" (S. 
-00004370: 4d2e 204c 756e 6462 6572 6720 6574 2061  M. Lundberg et a
-00004380: 6c2e 2032 3031 3829 3c2f 656d 3e0a 2020  l. 2018)</em>.  
-00004390: 2020 3c2f 7375 6d6d 6172 793e 0a20 2020    </summary>.   
-000043a0: 203c 6272 2f3e 0a20 2020 203c 7072 653e   <br/>.    <pre>
-000043b0: 0a40 6172 7469 636c 657b 6c75 6e64 6265  .@article{lundbe
-000043c0: 7267 3230 3138 6578 706c 6169 6e61 626c  rg2018explainabl
-000043d0: 652c 0a20 2074 6974 6c65 3d7b 4578 706c  e,.  title={Expl
-000043e0: 6169 6e61 626c 6520 6d61 6368 696e 652d  ainable machine-
-000043f0: 6c65 6172 6e69 6e67 2070 7265 6469 6374  learning predict
-00004400: 696f 6e73 2066 6f72 2074 6865 2070 7265  ions for the pre
-00004410: 7665 6e74 696f 6e20 6f66 2068 7970 6f78  vention of hypox
-00004420: 6165 6d69 6120 6475 7269 6e67 2073 7572  aemia during sur
-00004430: 6765 7279 7d2c 0a20 2061 7574 686f 723d  gery},.  author=
-00004440: 7b4c 756e 6462 6572 672c 2053 636f 7474  {Lundberg, Scott
-00004450: 204d 2061 6e64 204e 6169 722c 2042 616c   M and Nair, Bal
-00004460: 6120 616e 6420 5661 7669 6c61 6c61 2c20  a and Vavilala, 
-00004470: 4d6f 6e69 6361 2053 2061 6e64 2048 6f72  Monica S and Hor
-00004480: 6962 652c 204d 6179 756d 6920 616e 6420  ibe, Mayumi and 
-00004490: 4569 7373 6573 2c20 4d69 6368 6165 6c20  Eisses, Michael 
-000044a0: 4a20 616e 6420 4164 616d 732c 2054 7265  J and Adams, Tre
-000044b0: 766f 7220 616e 6420 4c69 7374 6f6e 2c20  vor and Liston, 
-000044c0: 4461 7669 6420 4520 616e 6420 4c6f 772c  David E and Low,
-000044d0: 2044 616e 6965 6c20 4b69 6e67 2d57 6169   Daniel King-Wai
-000044e0: 2061 6e64 204e 6577 6d61 6e2c 2053 6875   and Newman, Shu
-000044f0: 2d46 616e 6720 616e 6420 4b69 6d2c 204a  -Fang and Kim, J
-00004500: 6572 7279 2061 6e64 206f 7468 6572 737d  erry and others}
-00004510: 2c0a 2020 6a6f 7572 6e61 6c3d 7b4e 6174  ,.  journal={Nat
-00004520: 7572 6520 4269 6f6d 6564 6963 616c 2045  ure Biomedical E
-00004530: 6e67 696e 6565 7269 6e67 7d2c 0a20 2076  ngineering},.  v
-00004540: 6f6c 756d 653d 7b32 7d2c 0a20 206e 756d  olume={2},.  num
-00004550: 6265 723d 7b31 307d 2c0a 2020 7061 6765  ber={10},.  page
-00004560: 733d 7b37 3439 7d2c 0a20 2079 6561 723d  s={749},.  year=
-00004570: 7b32 3031 387d 2c0a 2020 7075 626c 6973  {2018},.  publis
-00004580: 6865 723d 7b4e 6174 7572 6520 5075 626c  her={Nature Publ
-00004590: 6973 6869 6e67 2047 726f 7570 7d0a 7d0a  ishing Group}.}.
-000045a0: 2020 2020 3c2f 7072 653e 0a20 2020 203c      </pre>.    <
-000045b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000045c0: 7777 772e 6e63 6269 2e6e 6c6d 2e6e 6968  www.ncbi.nlm.nih
-000045d0: 2e67 6f76 2f70 6d63 2f61 7274 6963 6c65  .gov/pmc/article
-000045e0: 732f 504d 4336 3436 3734 3932 2f70 6466  s/PMC6467492/pdf
-000045f0: 2f6e 6968 6d73 2d31 3530 3535 3738 2e70  /nihms-1505578.p
-00004600: 6466 223e 5061 7065 7220 6c69 6e6b 3c2f  df">Paper link</
-00004610: 613e 0a20 203c 2f64 6574 6169 6c73 3e0a  a>.  </details>.
-00004620: 0a20 203c 6872 2f3e 0a3c 2f64 6574 6169  .  <hr/>.</detai
-00004630: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a20  ls>..<details>. 
-00004640: 203c 7375 6d6d 6172 793e 3c73 7472 6f6e   <summary><stron
-00004650: 673e 5365 6e73 6974 6976 6974 7920 416e  g>Sensitivity An
-00004660: 616c 7973 6973 3c2f 7374 726f 6e67 3e3c  alysis</strong><
-00004670: 2f73 756d 6d61 7279 3e0a 2020 3c68 722f  /summary>.  <hr/
-00004680: 3e0a 0a20 203c 6465 7461 696c 733e 0a20  >..  <details>. 
-00004690: 2020 203c 7375 6d6d 6172 793e 0a20 2020     <summary>.   
-000046a0: 2020 203c 656d 3e22 5341 4c69 623a 2041     <em>"SALib: A
-000046b0: 6e20 6f70 656e 2d73 6f75 7263 6520 5079  n open-source Py
-000046c0: 7468 6f6e 206c 6962 7261 7279 2066 6f72  thon library for
-000046d0: 2053 656e 7369 7469 7669 7479 2041 6e61   Sensitivity Ana
-000046e0: 6c79 7369 7322 2028 4a2e 2044 2e20 4865  lysis" (J. D. He
-000046f0: 726d 616e 2061 6e64 2057 2e20 5573 6865  rman and W. Ushe
-00004700: 7220 3230 3137 293c 2f65 6d3e 0a20 2020  r 2017)</em>.   
-00004710: 203c 2f73 756d 6d61 7279 3e0a 2020 2020   </summary>.    
-00004720: 3c62 722f 3e0a 2020 2020 3c70 7265 3e0a  <br/>.    <pre>.
-00004730: 4061 7274 6963 6c65 7b68 6572 6d61 6e32  @article{herman2
-00004740: 3031 3773 616c 6962 2c0a 2020 7469 746c  017salib,.  titl
-00004750: 653d 7b53 414c 6962 3a20 416e 206f 7065  e={SALib: An ope
-00004760: 6e2d 736f 7572 6365 2050 7974 686f 6e20  n-source Python 
-00004770: 6c69 6272 6172 7920 666f 7220 5365 6e73  library for Sens
-00004780: 6974 6976 6974 7920 416e 616c 7973 6973  itivity Analysis
-00004790: 2e7d 2c0a 2020 6175 7468 6f72 3d7b 4865  .},.  author={He
-000047a0: 726d 616e 2c20 4a6f 6e61 7468 616e 2044  rman, Jonathan D
-000047b0: 2061 6e64 2055 7368 6572 2c20 5769 6c6c   and Usher, Will
-000047c0: 7d2c 0a20 206a 6f75 726e 616c 3d7b 4a2e  },.  journal={J.
-000047d0: 204f 7065 6e20 536f 7572 6365 2053 6f66   Open Source Sof
-000047e0: 7477 6172 657d 2c0a 2020 766f 6c75 6d65  tware},.  volume
-000047f0: 3d7b 327d 2c0a 2020 6e75 6d62 6572 3d7b  ={2},.  number={
-00004800: 397d 2c0a 2020 7061 6765 733d 7b39 377d  9},.  pages={97}
-00004810: 2c0a 2020 7965 6172 3d7b 3230 3137 7d0a  ,.  year={2017}.
-00004820: 7d0a 2020 2020 3c2f 7072 653e 0a20 2020  }.    </pre>.   
-00004830: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00004840: 2f2f 7777 772e 7265 7365 6172 6368 6761  //www.researchga
-00004850: 7465 2e6e 6574 2f70 726f 6669 6c65 2f57  te.net/profile/W
-00004860: 696c 6c5f 5573 6865 722f 7075 626c 6963  ill_Usher/public
-00004870: 6174 696f 6e2f 3331 3232 3034 3233 365f  ation/312204236_
-00004880: 5341 4c69 625f 416e 5f6f 7065 6e2d 736f  SALib_An_open-so
-00004890: 7572 6365 5f50 7974 686f 6e5f 6c69 6272  urce_Python_libr
-000048a0: 6172 795f 666f 725f 5365 6e73 6974 6976  ary_for_Sensitiv
-000048b0: 6974 795f 416e 616c 7973 6973 2f6c 696e  ity_Analysis/lin
-000048c0: 6b73 2f35 6163 3733 3264 3634 3538 3531  ks/5ac732d645851
-000048d0: 3531 6538 3061 3339 3534 372f 5341 4c69  51e80a39547/SALi
-000048e0: 622d 416e 2d6f 7065 6e2d 736f 7572 6365  b-An-open-source
-000048f0: 2d50 7974 686f 6e2d 6c69 6272 6172 792d  -Python-library-
-00004900: 666f 722d 5365 6e73 6974 6976 6974 792d  for-Sensitivity-
-00004910: 416e 616c 7973 6973 2e70 6466 3f6f 7269  Analysis.pdf?ori
-00004920: 6769 6e3d 7075 626c 6963 6174 696f 6e5f  gin=publication_
-00004930: 6465 7461 696c 223e 5061 7065 7220 6c69  detail">Paper li
-00004940: 6e6b 3c2f 613e 0a20 203c 2f64 6574 6169  nk</a>.  </detai
-00004950: 6c73 3e0a 0a20 203c 6465 7461 696c 733e  ls>..  <details>
-00004960: 0a20 2020 203c 7375 6d6d 6172 793e 0a20  .    <summary>. 
-00004970: 2020 2020 203c 656d 3e22 4661 6374 6f72       <em>"Factor
-00004980: 6961 6c20 7361 6d70 6c69 6e67 2070 6c61  ial sampling pla
-00004990: 6e73 2066 6f72 2070 7265 6c69 6d69 6e61  ns for prelimina
-000049a0: 7279 2063 6f6d 7075 7461 7469 6f6e 616c  ry computational
-000049b0: 2065 7870 6572 696d 656e 7473 2220 284d   experiments" (M
-000049c0: 2e20 442e 204d 6f72 7269 7320 3139 3931  . D. Morris 1991
-000049d0: 293c 2f65 6d3e 0a20 2020 203c 2f73 756d  )</em>.    </sum
-000049e0: 6d61 7279 3e0a 2020 2020 3c62 722f 3e0a  mary>.    <br/>.
-000049f0: 2020 2020 3c70 7265 3e0a 4061 7274 6963      <pre>.@artic
-00004a00: 6c65 7b6d 6f72 7269 7331 3939 3166 6163  le{morris1991fac
-00004a10: 746f 7269 616c 2c0a 2020 7469 746c 653d  torial,.  title=
-00004a20: 7b7d 2c0a 2020 6175 7468 6f72 3d7b 4d6f  {},.  author={Mo
-00004a30: 7272 6973 2c20 4d61 7820 447d 2c0a 2020  rris, Max D},.  
-00004a40: 6a6f 7572 6e61 6c3d 7b54 6563 686e 6f6d  journal={Technom
-00004a50: 6574 7269 6373 7d2c 0a20 2076 6f6c 756d  etrics},.  volum
-00004a60: 653d 7b33 337d 2c0a 2020 6e75 6d62 6572  e={33},.  number
-00004a70: 3d7b 327d 2c0a 2020 7061 6765 733d 7b31  ={2},.  pages={1
-00004a80: 3631 2d2d 3137 347d 2c0a 2020 7965 6172  61--174},.  year
-00004a90: 3d7b 3139 3931 7d2c 0a20 2070 7562 6c69  ={1991},.  publi
-00004aa0: 7368 6572 3d7b 5461 796c 6f72 205c 2620  sher={Taylor \& 
-00004ab0: 4672 616e 6369 7320 4772 6f75 707d 0a7d  Francis Group}.}
-00004ac0: 0a20 2020 203c 2f70 7265 3e0a 2020 2020  .    </pre>.    
-00004ad0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00004ae0: 2f61 6265 2e75 666c 2e65 6475 2f46 6163  /abe.ufl.edu/Fac
-00004af0: 756c 7479 2f6a 6a6f 6e65 732f 4142 455f  ulty/jjones/ABE_
-00004b00: 3536 3436 2f32 3031 302f 4d6f 7272 6973  5646/2010/Morris
-00004b10: 2e31 3939 3125 3230 5341 2532 3070 6170  .1991%20SA%20pap
-00004b20: 6572 2e70 6466 223e 5061 7065 7220 6c69  er.pdf">Paper li
-00004b30: 6e6b 3c2f 613e 0a20 203c 2f64 6574 6169  nk</a>.  </detai
-00004b40: 6c73 3e0a 0a20 203c 6872 2f3e 0a3c 2f64  ls>..  <hr/>.</d
-00004b50: 6574 6169 6c73 3e0a 0a3c 6465 7461 696c  etails>..<detail
-00004b60: 733e 0a20 203c 7375 6d6d 6172 793e 3c73  s>.  <summary><s
-00004b70: 7472 6f6e 673e 5061 7274 6961 6c20 4465  trong>Partial De
-00004b80: 7065 6e64 656e 6365 3c2f 7374 726f 6e67  pendence</strong
-00004b90: 3e3c 2f73 756d 6d61 7279 3e0a 2020 3c68  ></summary>.  <h
-00004ba0: 722f 3e0a 0a20 203c 6465 7461 696c 733e  r/>..  <details>
-00004bb0: 0a20 2020 203c 7375 6d6d 6172 793e 0a20  .    <summary>. 
-00004bc0: 2020 2020 203c 656d 3e22 4772 6565 6479       <em>"Greedy
-00004bd0: 2066 756e 6374 696f 6e20 6170 7072 6f78   function approx
-00004be0: 696d 6174 696f 6e3a 2061 2067 7261 6469  imation: a gradi
-00004bf0: 656e 7420 626f 6f73 7469 6e67 206d 6163  ent boosting mac
-00004c00: 6869 6e65 2220 284a 2e20 482e 2046 7269  hine" (J. H. Fri
-00004c10: 6564 6d61 6e20 3230 3031 293c 2f65 6d3e  edman 2001)</em>
-00004c20: 0a20 2020 203c 2f73 756d 6d61 7279 3e0a  .    </summary>.
-00004c30: 2020 2020 3c62 722f 3e0a 2020 2020 3c70      <br/>.    <p
-00004c40: 7265 3e0a 4061 7274 6963 6c65 7b66 7269  re>.@article{fri
-00004c50: 6564 6d61 6e32 3030 3167 7265 6564 792c  edman2001greedy,
-00004c60: 0a20 2074 6974 6c65 3d7b 4772 6565 6479  .  title={Greedy
-00004c70: 2066 756e 6374 696f 6e20 6170 7072 6f78   function approx
-00004c80: 696d 6174 696f 6e3a 2061 2067 7261 6469  imation: a gradi
-00004c90: 656e 7420 626f 6f73 7469 6e67 206d 6163  ent boosting mac
-00004ca0: 6869 6e65 7d2c 0a20 2061 7574 686f 723d  hine},.  author=
-00004cb0: 7b46 7269 6564 6d61 6e2c 204a 6572 6f6d  {Friedman, Jerom
-00004cc0: 6520 487d 2c0a 2020 6a6f 7572 6e61 6c3d  e H},.  journal=
-00004cd0: 7b41 6e6e 616c 7320 6f66 2073 7461 7469  {Annals of stati
-00004ce0: 7374 6963 737d 2c0a 2020 7061 6765 733d  stics},.  pages=
-00004cf0: 7b31 3138 392d 2d31 3233 327d 2c0a 2020  {1189--1232},.  
-00004d00: 7965 6172 3d7b 3230 3031 7d2c 0a20 2070  year={2001},.  p
-00004d10: 7562 6c69 7368 6572 3d7b 4a53 544f 527d  ublisher={JSTOR}
-00004d20: 0a7d 0a20 2020 203c 2f70 7265 3e0a 2020  .}.    </pre>.  
-00004d30: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00004d40: 3a2f 2f70 726f 6a65 6374 6575 636c 6964  ://projecteuclid
-00004d50: 2e6f 7267 2f64 6f77 6e6c 6f61 642f 7064  .org/download/pd
-00004d60: 665f 312f 6575 636c 6964 2e61 6f73 2f31  f_1/euclid.aos/1
-00004d70: 3031 3332 3033 3435 3122 3e50 6170 6572  013203451">Paper
-00004d80: 206c 696e 6b3c 2f61 3e0a 2020 3c2f 6465   link</a>.  </de
-00004d90: 7461 696c 733e 0a0a 2020 3c68 722f 3e0a  tails>..  <hr/>.
-00004da0: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
-00004db0: 6169 6c73 3e0a 2020 3c73 756d 6d61 7279  ails>.  <summary
-00004dc0: 3e3c 7374 726f 6e67 3e4f 7065 6e20 536f  ><strong>Open So
-00004dd0: 7572 6365 2053 6f66 7477 6172 653c 2f73  urce Software</s
-00004de0: 7472 6f6e 673e 3c2f 7375 6d6d 6172 793e  trong></summary>
-00004df0: 0a20 203c 6872 2f3e 0a0a 2020 3c64 6574  .  <hr/>..  <det
-00004e00: 6169 6c73 3e0a 2020 2020 3c73 756d 6d61  ails>.    <summa
-00004e10: 7279 3e0a 2020 2020 2020 3c65 6d3e 2253  ry>.      <em>"S
-00004e20: 6369 6b69 742d 6c65 6172 6e3a 204d 6163  cikit-learn: Mac
-00004e30: 6869 6e65 206c 6561 726e 696e 6720 696e  hine learning in
-00004e40: 2050 7974 686f 6e22 2028 462e 2050 6564   Python" (F. Ped
-00004e50: 7265 676f 7361 2065 7420 616c 2e20 3230  regosa et al. 20
-00004e60: 3131 293c 2f65 6d3e 0a20 2020 203c 2f73  11)</em>.    </s
-00004e70: 756d 6d61 7279 3e0a 2020 2020 3c62 722f  ummary>.    <br/
-00004e80: 3e0a 2020 2020 3c70 7265 3e0a 4061 7274  >.    <pre>.@art
-00004e90: 6963 6c65 7b70 6564 7265 676f 7361 3230  icle{pedregosa20
-00004ea0: 3131 7363 696b 6974 2c0a 2020 7469 746c  11scikit,.  titl
-00004eb0: 653d 7b53 6369 6b69 742d 6c65 6172 6e3a  e={Scikit-learn:
-00004ec0: 204d 6163 6869 6e65 206c 6561 726e 696e   Machine learnin
-00004ed0: 6720 696e 2050 7974 686f 6e7d 2c0a 2020  g in Python},.  
-00004ee0: 6175 7468 6f72 3d7b 5065 6472 6567 6f73  author={Pedregos
-00004ef0: 612c 2046 6162 6961 6e20 616e 6420 5661  a, Fabian and Va
-00004f00: 726f 7175 6175 782c 2047 617b 5c22 657d  roquaux, Ga{\"e}
-00004f10: 6c20 616e 6420 4772 616d 666f 7274 2c20  l and Gramfort, 
-00004f20: 416c 6578 616e 6472 6520 616e 6420 4d69  Alexandre and Mi
-00004f30: 6368 656c 2c20 5669 6e63 656e 7420 616e  chel, Vincent an
-00004f40: 6420 5468 6972 696f 6e2c 2042 6572 7472  d Thirion, Bertr
-00004f50: 616e 6420 616e 6420 4772 6973 656c 2c20  and and Grisel, 
-00004f60: 4f6c 6976 6965 7220 616e 6420 426c 6f6e  Olivier and Blon
-00004f70: 6465 6c2c 204d 6174 6869 6575 2061 6e64  del, Mathieu and
-00004f80: 2050 7265 7474 656e 686f 6665 722c 2050   Prettenhofer, P
-00004f90: 6574 6572 2061 6e64 2057 6569 7373 2c20  eter and Weiss, 
-00004fa0: 526f 6e20 616e 6420 4475 626f 7572 672c  Ron and Dubourg,
-00004fb0: 2056 696e 6365 6e74 2061 6e64 206f 7468   Vincent and oth
-00004fc0: 6572 737d 2c0a 2020 6a6f 7572 6e61 6c3d  ers},.  journal=
-00004fd0: 7b4a 6f75 726e 616c 206f 6620 6d61 6368  {Journal of mach
-00004fe0: 696e 6520 6c65 6172 6e69 6e67 2072 6573  ine learning res
-00004ff0: 6561 7263 687d 2c0a 2020 766f 6c75 6d65  earch},.  volume
-00005000: 3d7b 3132 7d2c 0a20 206e 756d 6265 723d  ={12},.  number=
-00005010: 7b4f 6374 7d2c 0a20 2070 6167 6573 3d7b  {Oct},.  pages={
-00005020: 3238 3235 2d2d 3238 3330 7d2c 0a20 2079  2825--2830},.  y
-00005030: 6561 723d 7b32 3031 317d 0a7d 0a20 2020  ear={2011}.}.   
-00005040: 203c 2f70 7265 3e0a 2020 2020 3c61 2068   </pre>.    <a h
-00005050: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
-00005060: 2e6a 6d6c 722e 6f72 672f 7061 7065 7273  .jmlr.org/papers
-00005070: 2f76 6f6c 756d 6531 322f 7065 6472 6567  /volume12/pedreg
-00005080: 6f73 6131 3161 2f70 6564 7265 676f 7361  osa11a/pedregosa
-00005090: 3131 612e 7064 6622 3e50 6170 6572 206c  11a.pdf">Paper l
-000050a0: 696e 6b3c 2f61 3e0a 2020 3c2f 6465 7461  ink</a>.  </deta
-000050b0: 696c 733e 0a0a 2020 3c64 6574 6169 6c73  ils>..  <details
-000050c0: 3e0a 2020 2020 3c73 756d 6d61 7279 3e0a  >.    <summary>.
-000050d0: 2020 2020 2020 3c65 6d3e 2243 6f6c 6c61        <em>"Colla
-000050e0: 626f 7261 7469 7665 2064 6174 6120 7363  borative data sc
-000050f0: 6965 6e63 6522 2028 506c 6f74 6c79 2054  ience" (Plotly T
-00005100: 6563 686e 6f6c 6f67 6965 7320 496e 632e  echnologies Inc.
-00005110: 2032 3031 3529 3c2f 656d 3e0a 2020 2020   2015)</em>.    
-00005120: 3c2f 7375 6d6d 6172 793e 0a20 2020 203c  </summary>.    <
-00005130: 6272 2f3e 0a20 2020 203c 7072 653e 0a40  br/>.    <pre>.@
-00005140: 6f6e 6c69 6e65 7b70 6c6f 746c 792c 200a  online{plotly, .
-00005150: 2020 6175 7468 6f72 203d 207b 506c 6f74    author = {Plot
-00005160: 6c79 2054 6563 686e 6f6c 6f67 6965 7320  ly Technologies 
-00005170: 496e 632e 7d2c 200a 2020 7469 746c 6520  Inc.}, .  title 
-00005180: 3d20 7b43 6f6c 6c61 626f 7261 7469 7665  = {Collaborative
-00005190: 2064 6174 6120 7363 6965 6e63 657d 2c20   data science}, 
-000051a0: 0a20 2070 7562 6c69 7368 6572 203d 207b  .  publisher = {
-000051b0: 506c 6f74 6c79 2054 6563 686e 6f6c 6f67  Plotly Technolog
-000051c0: 6965 7320 496e 632e 7d2c 200a 2020 6164  ies Inc.}, .  ad
-000051d0: 6472 6573 7320 3d20 7b4d 6f6e 7472 6561  dress = {Montrea
-000051e0: 6c2c 2051 437d 2c20 0a20 2079 6561 7220  l, QC}, .  year 
-000051f0: 3d20 7b32 3031 357d 2c20 0a20 2075 726c  = {2015}, .  url
-00005200: 203d 207b 6874 7470 733a 2f2f 706c 6f74   = {https://plot
-00005210: 2e6c 797d 0a7d 0a20 2020 203c 2f70 7265  .ly}.}.    </pre
-00005220: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-00005230: 7474 7073 3a2f 2f70 6c6f 742e 6c79 223e  ttps://plot.ly">
-00005240: 4c69 6e6b 3c2f 613e 0a20 203c 2f64 6574  Link</a>.  </det
-00005250: 6169 6c73 3e0a 2020 0a20 203c 6465 7461  ails>.  .  <deta
-00005260: 696c 733e 0a20 2020 203c 7375 6d6d 6172  ils>.    <summar
-00005270: 793e 0a20 2020 2020 203c 656d 3e22 4a6f  y>.      <em>"Jo
-00005280: 626c 6962 3a20 7275 6e6e 696e 6720 7079  blib: running py
-00005290: 7468 6f6e 2066 756e 6374 696f 6e20 6173  thon function as
-000052a0: 2070 6970 656c 696e 6520 6a6f 6273 2220   pipeline jobs" 
-000052b0: 2847 2e20 5661 726f 7175 6175 7820 616e  (G. Varoquaux an
-000052c0: 6420 4f2e 2047 7269 7365 6c20 3230 3039  d O. Grisel 2009
-000052d0: 293c 2f65 6d3e 0a20 2020 203c 2f73 756d  )</em>.    </sum
-000052e0: 6d61 7279 3e0a 2020 2020 3c62 722f 3e0a  mary>.    <br/>.
-000052f0: 2020 2020 3c70 7265 3e0a 4061 7274 6963      <pre>.@artic
-00005300: 6c65 7b76 6172 6f71 7561 7578 3230 3039  le{varoquaux2009
-00005310: 6a6f 626c 6962 2c0a 2020 7469 746c 653d  joblib,.  title=
-00005320: 7b4a 6f62 6c69 623a 2072 756e 6e69 6e67  {Joblib: running
-00005330: 2070 7974 686f 6e20 6675 6e63 7469 6f6e   python function
-00005340: 2061 7320 7069 7065 6c69 6e65 206a 6f62   as pipeline job
-00005350: 737d 2c0a 2020 6175 7468 6f72 3d7b 5661  s},.  author={Va
-00005360: 726f 7175 6175 782c 2047 617b 5c22 657d  roquaux, Ga{\"e}
-00005370: 6c20 616e 6420 4772 6973 656c 2c20 4f7d  l and Grisel, O}
-00005380: 2c0a 2020 6a6f 7572 6e61 6c3d 7b70 6163  ,.  journal={pac
-00005390: 6b61 6765 732e 2070 7974 686f 6e2e 206f  kages. python. o
-000053a0: 7267 2f6a 6f62 6c69 627d 2c0a 2020 7965  rg/joblib},.  ye
-000053b0: 6172 3d7b 3230 3039 7d0a 7d0a 2020 2020  ar={2009}.}.    
-000053c0: 3c2f 7072 653e 0a20 2020 203c 6120 6872  </pre>.    <a hr
-000053d0: 6566 3d22 6874 7470 733a 2f2f 6a6f 626c  ef="https://jobl
-000053e0: 6962 2e72 6561 6474 6865 646f 6373 2e69  ib.readthedocs.i
-000053f0: 6f2f 656e 2f6c 6174 6573 742f 223e 4c69  o/en/latest/">Li
-00005400: 6e6b 3c2f 613e 0a20 203c 2f64 6574 6169  nk</a>.  </detai
-00005410: 6c73 3e0a 2020 0a20 203c 6872 2f3e 0a3c  ls>.  .  <hr/>.<
-00005420: 2f64 6574 6169 6c73 3e0a 0a23 2056 6964  /details>..# Vid
-00005430: 656f 730a 0a2d 205b 5468 6520 5363 6965  eos..- [The Scie
-00005440: 6e63 6520 4265 6869 6e64 2049 6e74 6572  nce Behind Inter
-00005450: 7072 6574 4d4c 3a20 4578 706c 6169 6e61  pretML: Explaina
-00005460: 626c 6520 426f 6f73 7469 6e67 204d 6163  ble Boosting Mac
-00005470: 6869 6e65 5d28 6874 7470 733a 2f2f 7777  hine](https://ww
-00005480: 772e 796f 7574 7562 652e 636f 6d2f 7761  w.youtube.com/wa
-00005490: 7463 683f 763d 4d52 4569 4867 4867 6c30  tch?v=MREiHgHgl0
-000054a0: 6b29 0a2d 205b 486f 7720 746f 2045 7870  k).- [How to Exp
-000054b0: 6c61 696e 204d 6f64 656c 7320 7769 7468  lain Models with
-000054c0: 2049 6e74 6572 7072 6574 4d4c 2044 6565   InterpretML Dee
-000054d0: 7020 4469 7665 5d28 6874 7470 733a 2f2f  p Dive](https://
-000054e0: 7777 772e 796f 7574 7562 652e 636f 6d2f  www.youtube.com/
-000054f0: 7761 7463 683f 763d 5777 4265 4b4d 5130  watch?v=WwBeKMQ0
-00005500: 2d49 3829 0a2d 205b 426c 6163 6b2d 426f  -I8).- [Black-Bo
-00005510: 7820 616e 6420 476c 6173 732d 426f 7820  x and Glass-Box 
-00005520: 4578 706c 616e 6174 696f 6e20 696e 204d  Explanation in M
-00005530: 6163 6869 6e65 204c 6561 726e 696e 675d  achine Learning]
-00005540: 2868 7474 7073 3a2f 2f79 6f75 7475 2e62  (https://youtu.b
-00005550: 652f 3775 7a4e 4b59 3870 4568 5129 0a2d  e/7uzNKY8pEhQ).-
-00005560: 205b 4578 706c 6169 6e61 626c 6520 4149   [Explainable AI
-00005570: 2065 7870 6c61 696e 6564 2120 2042 792d   explained!  By-
-00005580: 6465 7369 676e 2069 6e74 6572 7072 6574  design interpret
-00005590: 6162 6c65 206d 6f64 656c 7320 7769 7468  able models with
-000055a0: 204d 6963 726f 736f 6674 7320 496e 7465   Microsofts Inte
-000055b0: 7270 7265 744d 4c5d 2868 7474 7073 3a2f  rpretML](https:/
-000055c0: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
-000055d0: 2f77 6174 6368 3f76 3d71 506e 396d 3330  /watch?v=qPn9m30
-000055e0: 6f6a 6663 290a 2d20 5b49 6e74 6572 7072  ojfc).- [Interpr
-000055f0: 6574 696e 6720 4d61 6368 696e 6520 4c65  eting Machine Le
-00005600: 6172 6e69 6e67 204d 6f64 656c 7320 7769  arning Models wi
-00005610: 7468 2049 6e74 6572 7072 6574 4d4c 5d28  th InterpretML](
-00005620: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
-00005630: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
-00005640: 4552 4e75 4666 736b 6e68 6b29 0a0a 2320  ERNuFfsknhk)..# 
-00005650: 4578 7465 726e 616c 206c 696e 6b73 0a0a  External links..
-00005660: 2d20 5b49 6e74 6572 7072 6574 6162 6c65  - [Interpretable
-00005670: 206f 7220 4163 6375 7261 7465 3f20 5768   or Accurate? Wh
-00005680: 7920 4e6f 7420 426f 7468 3f5d 2868 7474  y Not Both?](htt
-00005690: 7073 3a2f 2f74 6f77 6172 6473 6461 7461  ps://towardsdata
-000056a0: 7363 6965 6e63 652e 636f 6d2f 696e 7465  science.com/inte
-000056b0: 7270 7265 7461 626c 652d 6f72 2d61 6363  rpretable-or-acc
-000056c0: 7572 6174 652d 7768 792d 6e6f 742d 626f  urate-why-not-bo
-000056d0: 7468 2d34 6439 6337 3335 3132 3139 3229  th-4d9c73512192)
-000056e0: 0a2d 205b 5468 6520 4578 706c 6169 6e61  .- [The Explaina
-000056f0: 626c 6520 426f 6f73 7469 6e67 204d 6163  ble Boosting Mac
-00005700: 6869 6e65 2e20 4173 2061 6363 7572 6174  hine. As accurat
-00005710: 6520 6173 2067 7261 6469 656e 7420 626f  e as gradient bo
-00005720: 6f73 7469 6e67 2c20 6173 2069 6e74 6572  osting, as inter
-00005730: 7072 6574 6162 6c65 2061 7320 6c69 6e65  pretable as line
-00005740: 6172 2072 6567 7265 7373 696f 6e2e 5d28  ar regression.](
-00005750: 6874 7470 733a 2f2f 746f 7761 7264 7364  https://towardsd
-00005760: 6174 6173 6369 656e 6365 2e63 6f6d 2f74  atascience.com/t
-00005770: 6865 2d65 7870 6c61 696e 6162 6c65 2d62  he-explainable-b
-00005780: 6f6f 7374 696e 672d 6d61 6368 696e 652d  oosting-machine-
-00005790: 6632 3431 3532 3530 3965 6262 290a 2d20  f24152509ebb).- 
-000057a0: 5b50 6572 666f 726d 616e 6365 2041 6e64  [Performance And
-000057b0: 2045 7870 6c61 696e 6162 696c 6974 7920   Explainability 
-000057c0: 5769 7468 2045 424d 5d28 6874 7470 733a  With EBM](https:
-000057d0: 2f2f 626c 6f67 2e6f 616b 6269 7473 2e63  //blog.oakbits.c
-000057e0: 6f6d 2f65 626d 2d61 6c67 6f72 6974 686d  om/ebm-algorithm
-000057f0: 2e68 746d 6c29 0a2d 205b 496e 7465 7270  .html).- [Interp
-00005800: 7265 744d 4c3a 2041 6e6f 7468 6572 2057  retML: Another W
-00005810: 6179 2074 6f20 4578 706c 6169 6e20 596f  ay to Explain Yo
-00005820: 7572 204d 6f64 656c 5d28 6874 7470 733a  ur Model](https:
-00005830: 2f2f 746f 7761 7264 7364 6174 6173 6369  //towardsdatasci
-00005840: 656e 6365 2e63 6f6d 2f69 6e74 6572 7072  ence.com/interpr
-00005850: 6574 6d6c 2d61 6e6f 7468 6572 2d77 6179  etml-another-way
-00005860: 2d74 6f2d 6578 706c 6169 6e2d 796f 7572  -to-explain-your
-00005870: 2d6d 6f64 656c 2d62 3766 6166 3061 3338  -model-b7faf0a38
-00005880: 3466 3829 0a2d 205b 4120 6765 6e74 6c65  4f8).- [A gentle
-00005890: 2069 6e74 726f 6475 6374 696f 6e20 746f   introduction to
-000058a0: 2047 4132 4d73 2c20 6120 7768 6974 6520   GA2Ms, a white 
-000058b0: 626f 7820 6d6f 6465 6c5d 2868 7474 7073  box model](https
-000058c0: 3a2f 2f77 7777 2e66 6964 646c 6572 2e61  ://www.fiddler.a
-000058d0: 692f 626c 6f67 2f61 2d67 656e 746c 652d  i/blog/a-gentle-
-000058e0: 696e 7472 6f64 7563 7469 6f6e 2d74 6f2d  introduction-to-
-000058f0: 6761 326d 732d 612d 7768 6974 652d 626f  ga2ms-a-white-bo
-00005900: 782d 6d6f 6465 6c29 0a2d 205b 4d6f 6465  x-model).- [Mode
-00005910: 6c20 496e 7465 7270 7265 7461 7469 6f6e  l Interpretation
-00005920: 2077 6974 6820 4d69 6372 6f73 6f66 74e2   with Microsoft.
-00005930: 8099 7320 496e 7465 7270 7265 7420 4d4c  ..s Interpret ML
-00005940: 5d28 6874 7470 733a 2f2f 6d65 6469 756d  ](https://medium
-00005950: 2e63 6f6d 2f40 7361 6e64 2e6d 6179 7572  .com/@sand.mayur
-00005960: 2f6d 6f64 656c 2d69 6e74 6572 7072 6574  /model-interpret
-00005970: 6174 696f 6e2d 7769 7468 2d6d 6963 726f  ation-with-micro
-00005980: 736f 6674 732d 696e 7465 7270 7265 742d  softs-interpret-
-00005990: 6d6c 2d38 3561 6130 6164 3639 3761 6529  ml-85aa0ad697ae)
-000059a0: 0a2d 205b 4578 706c 6169 6e69 6e67 204d  .- [Explaining M
-000059b0: 6f64 656c 2050 6970 656c 696e 6573 2057  odel Pipelines W
-000059c0: 6974 6820 496e 7465 7270 7265 744d 4c5d  ith InterpretML]
-000059d0: 2868 7474 7073 3a2f 2f6d 6564 6975 6d2e  (https://medium.
-000059e0: 636f 6d2f 406d 6172 6975 7376 6164 6569  com/@mariusvadei
-000059f0: 6b61 2f65 7870 6c61 696e 696e 672d 6d6f  ka/explaining-mo
-00005a00: 6465 6c2d 7069 7065 6c69 6e65 732d 7769  del-pipelines-wi
-00005a10: 7468 2d69 6e74 6572 7072 6574 6d6c 2d61  th-interpretml-a
-00005a20: 3932 3134 6637 3534 3030 6229 0a2d 205b  9214f75400b).- [
-00005a30: 4578 706c 6169 6e20 596f 7572 204d 6f64  Explain Your Mod
-00005a40: 656c 2077 6974 6820 4d69 6372 6f73 6f66  el with Microsof
-00005a50: 74e2 8099 7320 496e 7465 7270 7265 744d  t...s InterpretM
-00005a60: 4c5d 2868 7474 7073 3a2f 2f6d 6564 6975  L](https://mediu
-00005a70: 6d2e 636f 6d2f 4044 6174 616d 616e 2e61  m.com/@Dataman.a
-00005a80: 692f 6578 706c 6169 6e2d 796f 7572 2d6d  i/explain-your-m
-00005a90: 6f64 656c 2d77 6974 682d 6d69 6372 6f73  odel-with-micros
-00005aa0: 6f66 7473 2d69 6e74 6572 7072 6574 6d6c  ofts-interpretml
-00005ab0: 2d35 6461 6162 3164 3639 3362 3429 0a2d  -5daab1d693b4).-
-00005ac0: 205b 4f6e 204d 6f64 656c 2045 7870 6c61   [On Model Expla
-00005ad0: 696e 6162 696c 6974 793a 2046 726f 6d20  inability: From 
-00005ae0: 4c49 4d45 2c20 5348 4150 2c20 746f 2045  LIME, SHAP, to E
-00005af0: 7870 6c61 696e 6162 6c65 2042 6f6f 7374  xplainable Boost
-00005b00: 696e 675d 2868 7474 7073 3a2f 2f65 7665  ing](https://eve
-00005b10: 7264 6172 6b2e 6769 7468 7562 2e69 6f2f  rdark.github.io/
-00005b20: 6b39 2f6e 6f74 6562 6f6f 6b73 2f6d 6c2f  k9/notebooks/ml/
-00005b30: 6d6f 6465 6c5f 6578 706c 6169 6e2f 6d6f  model_explain/mo
-00005b40: 6465 6c5f 6578 706c 6169 6e2e 6e62 2e68  del_explain.nb.h
-00005b50: 746d 6c29 0a2d 205b 4465 616c 696e 6720  tml).- [Dealing 
-00005b60: 7769 7468 2049 6d62 616c 616e 6365 6420  with Imbalanced 
-00005b70: 4461 7461 2028 4d6f 7274 6761 6765 206c  Data (Mortgage l
-00005b80: 6f61 6e73 2064 6566 6175 6c74 7329 5d28  oans defaults)](
-00005b90: 6874 7470 733a 2f2f 6d69 6b65 776c 616e  https://mikewlan
-00005ba0: 6765 2e67 6974 6875 622e 696f 2f49 6d62  ge.github.io/Imb
-00005bb0: 616c 616e 6365 6444 6174 612d 2f69 6e64  alancedData-/ind
-00005bc0: 6578 2e68 746d 6c29 0a2d 205b 5468 6520  ex.html).- [The 
-00005bd0: 7269 6768 7420 7761 7920 746f 2063 6f6d  right way to com
-00005be0: 7075 7465 2079 6f75 7220 5368 6170 6c65  pute your Shaple
-00005bf0: 7920 5661 6c75 6573 5d28 6874 7470 733a  y Values](https:
-00005c00: 2f2f 746f 7761 7264 7364 6174 6173 6369  //towardsdatasci
-00005c10: 656e 6365 2e63 6f6d 2f74 6865 2d72 6967  ence.com/the-rig
-00005c20: 6874 2d77 6179 2d74 6f2d 636f 6d70 7574  ht-way-to-comput
-00005c30: 652d 796f 7572 2d73 6861 706c 6579 2d76  e-your-shapley-v
-00005c40: 616c 7565 732d 6366 6561 3330 3530 3932  alues-cfea305092
-00005c50: 3534 290a 2d20 5b54 6865 2041 7274 206f  54).- [The Art o
-00005c60: 6620 5370 7265 7a7a 6174 7572 6120 666f  f Sprezzatura fo
-00005c70: 7220 4d61 6368 696e 6520 4c65 6172 6e69  r Machine Learni
-00005c80: 6e67 5d28 6874 7470 733a 2f2f 746f 7761  ng](https://towa
-00005c90: 7264 7364 6174 6173 6369 656e 6365 2e63  rdsdatascience.c
-00005ca0: 6f6d 2f74 6865 2d61 7274 2d6f 662d 7370  om/the-art-of-sp
-00005cb0: 7265 7a7a 6174 7572 612d 666f 722d 6d61  rezzatura-for-ma
-00005cc0: 6368 696e 652d 6c65 6172 6e69 6e67 2d65  chine-learning-e
-00005cd0: 3234 3934 6330 6462 3732 3729 0a2d 205b  2494c0db727).- [
-00005ce0: 4d69 7869 6e67 2041 7274 2069 6e74 6f20  Mixing Art into 
-00005cf0: 7468 6520 5363 6965 6e63 6520 6f66 204d  the Science of M
-00005d00: 6f64 656c 2045 7870 6c61 696e 6162 696c  odel Explainabil
-00005d10: 6974 795d 2868 7474 7073 3a2f 2f74 6f77  ity](https://tow
-00005d20: 6172 6473 6461 7461 7363 6965 6e63 652e  ardsdatascience.
-00005d30: 636f 6d2f 6d69 7869 6e67 2d61 7274 2d69  com/mixing-art-i
-00005d40: 6e74 6f2d 7468 652d 7363 6965 6e63 652d  nto-the-science-
-00005d50: 6f66 2d6d 6f64 656c 2d65 7870 6c61 696e  of-model-explain
-00005d60: 6162 696c 6974 792d 3331 3262 3832 3136  ability-312b8216
-00005d70: 6661 3935 290a 0a23 2050 6170 6572 7320  fa95)..# Papers 
-00005d80: 7468 6174 2075 7365 206f 7220 636f 6d70  that use or comp
-00005d90: 6172 6520 4542 4d73 0a0a 0a2d 205b 4d6f  are EBMs...- [Mo
-00005da0: 6465 6c20 496e 7465 7270 7265 7461 6269  del Interpretabi
-00005db0: 6c69 7479 2069 6e20 4372 6564 6974 2049  lity in Credit I
-00005dc0: 6e73 7572 616e 6365 5d28 6874 7470 3a2f  nsurance](http:/
-00005dd0: 2f68 646c 2e68 616e 646c 652e 6e65 742f  /hdl.handle.net/
-00005de0: 3130 3430 302e 352f 3237 3530 3729 0a2d  10400.5/27507).-
-00005df0: 205b 4665 6465 7261 7465 6420 426f 6f73   [Federated Boos
-00005e00: 7465 6420 4465 6369 7369 6f6e 2054 7265  ted Decision Tre
-00005e10: 6573 2077 6974 6820 4469 6666 6572 656e  es with Differen
-00005e20: 7469 616c 2050 7269 7661 6379 5d28 6874  tial Privacy](ht
-00005e30: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00005e40: 7064 662f 3232 3130 2e30 3239 3130 2e70  pdf/2210.02910.p
-00005e50: 6466 290a 2d20 5b47 414d 2845 2920 4348  df).- [GAM(E) CH
-00005e60: 414e 4745 5220 4f52 204e 4f54 3f20 414e  ANGER OR NOT? AN
-00005e70: 2045 5641 4c55 4154 494f 4e20 4f46 2049   EVALUATION OF I
-00005e80: 4e54 4552 5052 4554 4142 4c45 204d 4143  NTERPRETABLE MAC
-00005e90: 4849 4e45 204c 4541 524e 494e 4720 4d4f  HINE LEARNING MO
-00005ea0: 4445 4c53 5d28 6874 7470 733a 2f2f 6172  DELS](https://ar
-00005eb0: 7869 762e 6f72 672f 7064 662f 3232 3034  xiv.org/pdf/2204
-00005ec0: 2e30 3931 3233 2e70 6466 290a 2d20 5b47  .09123.pdf).- [G
-00005ed0: 414d 2043 6f61 6368 3a20 546f 7761 7264  AM Coach: Toward
-00005ee0: 7320 496e 7465 7261 6374 6976 6520 616e  s Interactive an
-00005ef0: 6420 5573 6572 2d63 656e 7465 7265 6420  d User-centered 
-00005f00: 416c 676f 7269 7468 6d69 6320 5265 636f  Algorithmic Reco
-00005f10: 7572 7365 5d28 6874 7470 733a 2f2f 6172  urse](https://ar
-00005f20: 7869 762e 6f72 672f 7064 662f 3233 3032  xiv.org/pdf/2302
-00005f30: 2e31 3431 3635 2e70 6466 290a 2d20 5b4d  .14165.pdf).- [M
-00005f40: 6973 7369 6e67 2056 616c 7565 7320 616e  issing Values an
-00005f50: 6420 496d 7075 7461 7469 6f6e 2069 6e20  d Imputation in 
-00005f60: 4865 616c 7468 6361 7265 2044 6174 613a  Healthcare Data:
-00005f70: 2043 616e 2049 6e74 6572 7072 6574 6162   Can Interpretab
-00005f80: 6c65 204d 6163 6869 6e65 204c 6561 726e  le Machine Learn
-00005f90: 696e 6720 4865 6c70 3f5d 2868 7474 7073  ing Help?](https
-00005fa0: 3a2f 2f61 7278 6976 2e6f 7267 2f70 6466  ://arxiv.org/pdf
-00005fb0: 2f32 3330 342e 3131 3734 3976 312e 7064  /2304.11749v1.pd
-00005fc0: 6629 0a2d 205b 5072 6163 7469 6365 2061  f).- [Practice a
-00005fd0: 6e64 2043 6861 6c6c 656e 6765 7320 696e  nd Challenges in
-00005fe0: 2042 7569 6c64 696e 6720 6120 556e 6976   Building a Univ
-00005ff0: 6572 7361 6c20 5365 6172 6368 2051 7561  ersal Search Qua
-00006000: 6c69 7479 204d 6574 7269 635d 2868 7474  lity Metric](htt
-00006010: 7073 3a2f 2f77 7777 2e72 6573 6561 7263  ps://www.researc
-00006020: 6867 6174 652e 6e65 742f 7072 6f66 696c  hgate.net/profil
-00006030: 652f 4e75 6f2d 4368 656e 2d33 382f 7075  e/Nuo-Chen-38/pu
-00006040: 626c 6963 6174 696f 6e2f 3337 3031 3236  blication/370126
-00006050: 3732 305f 5072 6163 7469 6365 5f61 6e64  720_Practice_and
-00006060: 5f43 6861 6c6c 656e 6765 735f 696e 5f42  _Challenges_in_B
-00006070: 7569 6c64 696e 675f 615f 556e 6976 6572  uilding_a_Univer
-00006080: 7361 6c5f 5365 6172 6368 5f51 7561 6c69  sal_Search_Quali
-00006090: 7479 5f4d 6574 7269 632f 6c69 6e6b 732f  ty_Metric/links/
-000060a0: 3634 3430 6130 6632 3339 6161 3437 3161  6440a0f239aa471a
-000060b0: 3532 3463 6237 3764 2f50 7261 6374 6963  524cb77d/Practic
-000060c0: 652d 616e 642d 4368 616c 6c65 6e67 6573  e-and-Challenges
-000060d0: 2d69 6e2d 4275 696c 6469 6e67 2d61 2d55  -in-Building-a-U
-000060e0: 6e69 7665 7273 616c 2d53 6561 7263 682d  niversal-Search-
-000060f0: 5175 616c 6974 792d 4d65 7472 6963 2e70  Quality-Metric.p
-00006100: 6466 3f6f 7269 6769 6e3d 7075 626c 6963  df?origin=public
-00006110: 6174 696f 6e5f 6465 7461 696c 290a 2d20  ation_detail).- 
-00006120: 5b45 7870 6c61 696e 696e 6720 5068 6973  [Explaining Phis
-00006130: 6869 6e67 2041 7474 6163 6b73 3a20 416e  hing Attacks: An
-00006140: 2058 4149 2041 7070 726f 6163 6820 746f   XAI Approach to
-00006150: 2045 6e68 616e 6365 2055 7365 7220 4177   Enhance User Aw
-00006160: 6172 656e 6573 7320 616e 6420 5472 7573  areness and Trus
-00006170: 745d 2868 7474 7073 3a2f 2f77 7777 2e72  t](https://www.r
-00006180: 6573 6561 7263 6867 6174 652e 6e65 742f  esearchgate.net/
-00006190: 7072 6f66 696c 652f 4769 7573 6570 7065  profile/Giuseppe
-000061a0: 2d44 6573 6f6c 6461 2f70 7562 6c69 6361  -Desolda/publica
-000061b0: 7469 6f6e 2f33 3730 3030 3338 3738 5f45  tion/370003878_E
-000061c0: 7870 6c61 696e 696e 675f 5068 6973 6869  xplaining_Phishi
-000061d0: 6e67 5f41 7474 6163 6b73 5f41 6e5f 5841  ng_Attacks_An_XA
-000061e0: 495f 4170 7072 6f61 6368 5f74 6f5f 456e  I_Approach_to_En
-000061f0: 6861 6e63 655f 5573 6572 5f41 7761 7265  hance_User_Aware
-00006200: 6e65 7373 5f61 6e64 5f54 7275 7374 2f6c  ness_and_Trust/l
-00006210: 696e 6b73 2f36 3433 3932 3261 3865 3838  inks/643922a8e88
-00006220: 3136 3930 6334 6264 3530 6365 642f 4578  1690c4bd50ced/Ex
-00006230: 706c 6169 6e69 6e67 2d50 6869 7368 696e  plaining-Phishin
-00006240: 672d 4174 7461 636b 732d 416e 2d58 4149  g-Attacks-An-XAI
-00006250: 2d41 7070 726f 6163 682d 746f 2d45 6e68  -Approach-to-Enh
-00006260: 616e 6365 2d55 7365 722d 4177 6172 656e  ance-User-Awaren
-00006270: 6573 732d 616e 642d 5472 7573 742e 7064  ess-and-Trust.pd
-00006280: 6629 0a2d 205b 5265 7665 616c 696e 6720  f).- [Revealing 
-00006290: 7468 6520 4761 6c61 7879 2d48 616c 6f20  the Galaxy-Halo 
-000062a0: 436f 6e6e 6563 7469 6f6e 2054 6872 6f75  Connection Throu
-000062b0: 6768 204d 6163 6869 6e65 204c 6561 726e  gh Machine Learn
-000062c0: 696e 675d 2868 7474 7073 3a2f 2f61 7278  ing](https://arx
-000062d0: 6976 2e6f 7267 2f70 6466 2f32 3230 342e  iv.org/pdf/2204.
-000062e0: 3130 3333 322e 7064 6629 0a2d 205b 4578  10332.pdf).- [Ex
-000062f0: 706c 6169 6e61 626c 6520 4172 7469 6669  plainable Artifi
-00006300: 6369 616c 2049 6e74 656c 6c69 6765 6e63  cial Intelligenc
-00006310: 6520 666f 7220 434f 5649 442d 3139 2044  e for COVID-19 D
-00006320: 6961 676e 6f73 6973 2054 6872 6f75 6768  iagnosis Through
-00006330: 2042 6c6f 6f64 2054 6573 7420 5661 7269   Blood Test Vari
-00006340: 6162 6c65 735d 2868 7474 7073 3a2f 2f6c  ables](https://l
-00006350: 696e 6b2e 7370 7269 6e67 6572 2e63 6f6d  ink.springer.com
-00006360: 2f63 6f6e 7465 6e74 2f70 6466 2f31 302e  /content/pdf/10.
-00006370: 3130 3037 2f73 3430 3331 332d 3032 312d  1007/s40313-021-
-00006380: 3030 3835 382d 792e 7064 6629 0a2d 205b  00858-y.pdf).- [
-00006390: 5573 696e 6720 4578 706c 6169 6e61 626c  Using Explainabl
-000063a0: 6520 426f 6f73 7469 6e67 204d 6163 6869  e Boosting Machi
-000063b0: 6e65 7320 2845 424d 7329 2074 6f20 4465  nes (EBMs) to De
-000063c0: 7465 6374 2043 6f6d 6d6f 6e20 466c 6177  tect Common Flaw
-000063d0: 7320 696e 2044 6174 615d 2868 7474 7073  s in Data](https
-000063e0: 3a2f 2f6c 696e 6b2e 7370 7269 6e67 6572  ://link.springer
-000063f0: 2e63 6f6d 2f63 6861 7074 6572 2f31 302e  .com/chapter/10.
-00006400: 3130 3037 2f39 3738 2d33 2d30 3330 2d39  1007/978-3-030-9
-00006410: 3337 3336 2d32 5f34 3029 0a2d 205b 4469  3736-2_40).- [Di
-00006420: 6666 6572 656e 7469 616c 6c79 2050 7269  fferentially Pri
-00006430: 7661 7465 2047 7261 6469 656e 7420 426f  vate Gradient Bo
-00006440: 6f73 7469 6e67 206f 6e20 4c69 6e65 6172  osting on Linear
-00006450: 204c 6561 726e 6572 7320 666f 7220 5461   Learners for Ta
-00006460: 6275 6c61 7220 4461 7461 2041 6e61 6c79  bular Data Analy
-00006470: 7369 735d 2868 7474 7073 3a2f 2f61 7373  sis](https://ass
-00006480: 6574 732e 616d 617a 6f6e 2e73 6369 656e  ets.amazon.scien
-00006490: 6365 2f66 612f 3361 2f61 3632 6261 3733  ce/fa/3a/a62ba73
-000064a0: 6634 6262 6461 3164 3838 3062 3637 3863  f4bbda1d880b678c
-000064b0: 3339 3139 332f 6469 6666 6572 656e 7469  39193/differenti
-000064c0: 616c 6c79 2d70 7269 7661 7465 2d67 7261  ally-private-gra
-000064d0: 6469 656e 742d 626f 6f73 7469 6e67 2d6f  dient-boosting-o
-000064e0: 6e2d 6c69 6e65 6172 2d6c 6561 726e 6572  n-linear-learner
-000064f0: 732d 666f 722d 7461 6275 6c61 722d 6461  s-for-tabular-da
-00006500: 7461 2d61 6e61 6c79 7369 732e 7064 6629  ta-analysis.pdf)
-00006510: 0a2d 205b 436f 6e63 7265 7465 2063 6f6d  .- [Concrete com
-00006520: 7072 6573 7369 7665 2073 7472 656e 6774  pressive strengt
-00006530: 6820 7072 6564 6963 7469 6f6e 2075 7369  h prediction usi
-00006540: 6e67 2061 6e20 6578 706c 6169 6e61 626c  ng an explainabl
-00006550: 6520 626f 6f73 7469 6e67 206d 6163 6869  e boosting machi
-00006560: 6e65 206d 6f64 656c 5d28 6874 7470 733a  ne model](https:
-00006570: 2f2f 7777 772e 7363 6965 6e63 6564 6972  //www.sciencedir
-00006580: 6563 742e 636f 6d2f 7363 6965 6e63 652f  ect.com/science/
-00006590: 6172 7469 636c 652f 7069 692f 5332 3231  article/pii/S221
-000065a0: 3435 3039 3532 3330 3030 3234 342f 7064  4509523000244/pd
-000065b0: 6666 743f 6d64 353d 3137 3163 3237 3562  fft?md5=171c275b
-000065c0: 3662 6361 6538 3839 3763 6566 3033 6439  6bcae8897cef03d9
-000065d0: 3331 6539 3038 6532 2670 6964 3d31 2d73  31e908e2&pid=1-s
-000065e0: 322e 302d 5332 3231 3435 3039 3532 3330  2.0-S22145095230
-000065f0: 3030 3234 342d 6d61 696e 2e70 6466 290a  00244-main.pdf).
-00006600: 2d20 5b45 7374 696d 6174 6520 4465 666f  - [Estimate Defo
-00006610: 726d 6174 696f 6e20 4361 7061 6369 7479  rmation Capacity
-00006620: 206f 6620 4e6f 6e2d 4475 6374 696c 6520   of Non-Ductile 
-00006630: 5243 2053 6865 6172 2057 616c 6c73 2055  RC Shear Walls U
-00006640: 7369 6e67 2045 7870 6c61 696e 6162 6c65  sing Explainable
-00006650: 2042 6f6f 7374 696e 6720 4d61 6368 696e   Boosting Machin
-00006660: 655d 2868 7474 7073 3a2f 2f61 7278 6976  e](https://arxiv
-00006670: 2e6f 7267 2f70 6466 2f32 3330 312e 3034  .org/pdf/2301.04
-00006680: 3635 322e 7064 6629 0a2d 205b 496e 7472  652.pdf).- [Intr
-00006690: 6f64 7563 696e 6720 7468 6520 5261 6e6b  oducing the Rank
-000066a0: 2d42 6961 7365 6420 4f76 6572 6c61 7020  -Biased Overlap 
-000066b0: 6173 2053 696d 696c 6172 6974 7920 4d65  as Similarity Me
-000066c0: 6173 7572 6520 666f 7220 4665 6174 7572  asure for Featur
-000066d0: 6520 496d 706f 7274 616e 6365 2069 6e20  e Importance in 
-000066e0: 4578 706c 6169 6e61 626c 6520 4d61 6368  Explainable Mach
-000066f0: 696e 6520 4c65 6172 6e69 6e67 3a20 4120  ine Learning: A 
-00006700: 4361 7365 2053 7475 6479 206f 6e20 5061  Case Study on Pa
-00006710: 726b 696e 736f 6ee2 8099 7320 4469 7365  rkinson...s Dise
-00006720: 6173 655d 2868 7474 7073 3a2f 2f6c 696e  ase](https://lin
-00006730: 6b2e 7370 7269 6e67 6572 2e63 6f6d 2f63  k.springer.com/c
-00006740: 6861 7074 6572 2f31 302e 3130 3037 2f39  hapter/10.1007/9
-00006750: 3738 2d33 2d30 3331 2d31 3530 3337 2d31  78-3-031-15037-1
-00006760: 5f31 3129 0a2d 205b 5461 7267 6574 696e  _11).- [Targetin
-00006770: 6720 7265 736f 7572 6365 7320 6566 6669  g resources effi
-00006780: 6369 656e 746c 7920 616e 6420 6a75 7374  ciently and just
-00006790: 6966 6961 626c 7920 6279 2063 6f6d 6269  ifiably by combi
-000067a0: 6e69 6e67 2063 6175 7361 6c20 6d61 6368  ning causal mach
-000067b0: 696e 6520 6c65 6172 6e69 6e67 2061 6e64  ine learning and
-000067c0: 2074 6865 6f72 795d 2868 7474 7073 3a2f   theory](https:/
-000067d0: 2f77 7777 2e6e 6362 692e 6e6c 6d2e 6e69  /www.ncbi.nlm.ni
-000067e0: 682e 676f 762f 706d 632f 6172 7469 636c  h.gov/pmc/articl
-000067f0: 6573 2f50 4d43 3937 3638 3138 312f 7064  es/PMC9768181/pd
-00006800: 662f 6672 6169 2d30 352d 3130 3135 3630  f/frai-05-101560
-00006810: 342e 7064 6629 0a2d 205b 4578 7472 6163  4.pdf).- [Extrac
-00006820: 7469 7665 2054 6578 7420 5375 6d6d 6172  tive Text Summar
-00006830: 697a 6174 696f 6e20 5573 696e 6720 4765  ization Using Ge
-00006840: 6e65 7261 6c69 7a65 6420 4164 6469 7469  neralized Additi
-00006850: 7665 204d 6f64 656c 7320 7769 7468 2049  ve Models with I
-00006860: 6e74 6572 6163 7469 6f6e 7320 666f 7220  nteractions for 
-00006870: 5365 6e74 656e 6365 2053 656c 6563 7469  Sentence Selecti
-00006880: 6f6e 5d28 6874 7470 733a 2f2f 6172 7869  on](https://arxi
-00006890: 762e 6f72 672f 7064 662f 3232 3132 2e31  v.org/pdf/2212.1
-000068a0: 3037 3037 2e70 6466 290a 2d20 5b44 6561  0707.pdf).- [Dea
-000068b0: 7468 2062 7920 526f 756e 6420 4e75 6d62  th by Round Numb
-000068c0: 6572 733a 2047 6c61 7373 2d42 6f78 204d  ers: Glass-Box M
-000068d0: 6163 6869 6e65 204c 6561 726e 696e 6720  achine Learning 
-000068e0: 556e 636f 7665 7273 2042 6961 7365 7320  Uncovers Biases 
-000068f0: 696e 204d 6564 6963 616c 2050 7261 6374  in Medical Pract
-00006900: 6963 655d 2868 7474 7073 3a2f 2f77 7777  ice](https://www
-00006910: 2e6d 6564 7278 6976 2e6f 7267 2f63 6f6e  .medrxiv.org/con
-00006920: 7465 6e74 2f6d 6564 7278 6976 2f65 6172  tent/medrxiv/ear
-00006930: 6c79 2f32 3032 322f 3131 2f32 382f 3230  ly/2022/11/28/20
-00006940: 3232 2e30 342e 3330 2e32 3232 3734 3532  22.04.30.2227452
-00006950: 302e 6675 6c6c 2e70 6466 290a 2d20 5b50  0.full.pdf).- [P
-00006960: 6f73 742d 486f 6320 496e 7465 7270 7265  ost-Hoc Interpre
-00006970: 7461 7469 6f6e 206f 6620 5472 616e 7366  tation of Transf
-00006980: 6f72 6d65 7220 4879 7065 7270 6172 616d  ormer Hyperparam
-00006990: 6574 6572 7320 7769 7468 2045 7870 6c61  eters with Expla
-000069a0: 696e 6162 6c65 2042 6f6f 7374 696e 6720  inable Boosting 
-000069b0: 4d61 6368 696e 6573 5d28 6874 7470 733a  Machines](https:
-000069c0: 2f2f 7777 772e 6373 2e6a 6875 2e65 6475  //www.cs.jhu.edu
-000069d0: 2f7e 787a 6861 6e31 3338 2f70 6170 6572  /~xzhan138/paper
-000069e0: 732f 424c 4143 4b32 3032 322e 7064 6629  s/BLACK2022.pdf)
-000069f0: 0a2d 205b 496e 7465 7270 7265 7461 626c  .- [Interpretabl
-00006a00: 6520 6d61 6368 696e 6520 6c65 6172 6e69  e machine learni
-00006a10: 6e67 2066 6f72 2070 7265 6469 6374 696e  ng for predictin
-00006a20: 6720 7061 7468 6f6c 6f67 6963 2063 6f6d  g pathologic com
-00006a30: 706c 6574 6520 7265 7370 6f6e 7365 2069  plete response i
-00006a40: 6e20 7061 7469 656e 7473 2074 7265 6174  n patients treat
-00006a50: 6564 2077 6974 6820 6368 656d 6f72 6164  ed with chemorad
-00006a60: 6961 7469 6f6e 2074 6865 7261 7079 2066  iation therapy f
-00006a70: 6f72 2072 6563 7461 6c20 6164 656e 6f63  or rectal adenoc
-00006a80: 6172 6369 6e6f 6d61 5d28 6874 7470 733a  arcinoma](https:
-00006a90: 2f2f 7777 772e 6e63 6269 2e6e 6c6d 2e6e  //www.ncbi.nlm.n
-00006aa0: 6968 2e67 6f76 2f70 6d63 2f61 7274 6963  ih.gov/pmc/artic
-00006ab0: 6c65 732f 504d 4339 3737 3133 3835 2f70  les/PMC9771385/p
-00006ac0: 6466 2f66 7261 692d 3035 2d31 3035 3930  df/frai-05-10590
-00006ad0: 3333 2e70 6466 290a 2d20 5b45 7870 6c6f  33.pdf).- [Explo
-00006ae0: 7269 6e67 2074 6865 2042 616c 616e 6365  ring the Balance
-00006af0: 2062 6574 7765 656e 2049 6e74 6572 7072   between Interpr
-00006b00: 6574 6162 696c 6974 7920 616e 6420 5065  etability and Pe
-00006b10: 7266 6f72 6d61 6e63 6520 7769 7468 2063  rformance with c
-00006b20: 6172 6566 756c 6c79 2064 6573 6967 6e65  arefully designe
-00006b30: 6420 436f 6e73 7472 6169 6e61 626c 6520  d Constrainable 
-00006b40: 4e65 7572 616c 2041 6464 6974 6976 6520  Neural Additive 
-00006b50: 4d6f 6465 6c73 5d28 6874 7470 733a 2f2f  Models](https://
-00006b60: 6465 6c69 7665 7279 7064 662e 7373 726e  deliverypdf.ssrn
-00006b70: 2e63 6f6d 2f64 656c 6976 6572 792e 7068  .com/delivery.ph
-00006b80: 703f 4944 3d39 3938 3130 3530 3036 3030  p?ID=99810500600
-00006b90: 3030 3639 3132 3230 3733 3039 3831 3230  0069122073098120
-00006ba0: 3130 3231 3032 3132 3130 3231 3034 3030  1021021210210400
-00006bb0: 3531 3031 3830 3535 3039 3431 3235 3032  5101805509412502
-00006bc0: 3931 3232 3031 3130 3431 3030 3330 3539  9122011041003059
-00006bd0: 3039 3331 3235 3130 3230 3732 3132 3231  0931251020721221
-00006be0: 3036 3132 3230 3737 3038 3130 3639 3031  0612207708106901
-00006bf0: 3530 3837 3132 3430 3238 3039 3730 3136  5087124028097016
-00006c00: 3030 3331 3237 3039 3530 3837 3039 3130  0031270950870910
-00006c10: 3238 3038 3730 3130 3030 3730 3335 3039  2808701000703509
-00006c20: 3830 3836 3130 3230 3836 3038 3130 3134  8086102086081014
-00006c30: 3034 3330 3133 3131 3330 3034 3038 3131  0430131130040811
-00006c40: 3137 3130 3830 3131 3032 3830 3431 3039  1710801102804109
-00006c50: 3730 3935 3036 3430 3731 3130 3031 3132  7095064071100112
-00006c60: 3036 3930 3831 3130 3030 3639 3132 3030  0690811000691200
-00006c70: 3737 3036 3731 3136 3038 3831 3030 3036  7706711608810006
-00006c80: 3930 3730 3039 3730 3933 3038 3030 3734  9070097093080074
-00006c90: 3038 3731 3135 3038 3030 3732 3036 3430  0871150800720640
-00006ca0: 3836 3131 3131 3236 2645 5854 3d70 6466  86111126&EXT=pdf
-00006cb0: 2649 4e44 4558 3d54 5255 4529 0a2d 205b  &INDEX=TRUE).- [
-00006cc0: 4573 7469 6d61 7469 6e67 2044 6973 636f  Estimating Disco
-00006cd0: 6e74 696e 756f 7573 2054 696d 652d 5661  ntinuous Time-Va
-00006ce0: 7279 696e 6720 5269 736b 2046 6163 746f  rying Risk Facto
-00006cf0: 7273 2061 6e64 2054 7265 6174 6d65 6e74  rs and Treatment
-00006d00: 2042 656e 6566 6974 7320 666f 7220 434f   Benefits for CO
-00006d10: 5649 442d 3139 2077 6974 6820 496e 7465  VID-19 with Inte
-00006d20: 7270 7265 7461 626c 6520 4d4c 5d28 6874  rpretable ML](ht
-00006d30: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00006d40: 7064 662f 3232 3131 2e30 3839 3931 2e70  pdf/2211.08991.p
-00006d50: 6466 290a 2d20 5b50 6573 7420 5072 6573  df).- [Pest Pres
-00006d60: 656e 6365 2050 7265 6469 6374 696f 6e20  ence Prediction 
-00006d70: 5573 696e 6720 496e 7465 7270 7265 7461  Using Interpreta
-00006d80: 626c 6520 4d61 6368 696e 6520 4c65 6172  ble Machine Lear
-00006d90: 6e69 6e67 5d28 6874 7470 733a 2f2f 6172  ning](https://ar
-00006da0: 7869 762e 6f72 672f 7064 662f 3232 3035  xiv.org/pdf/2205
-00006db0: 2e30 3737 3233 2e70 6466 290a 2d20 5b65  .07723.pdf).- [e
-00006dc0: 7069 746f 7065 3144 3a20 4163 6375 7261  pitope1D: Accura
-00006dd0: 7465 2054 6178 6f6e 6f6d 792d 4177 6172  te Taxonomy-Awar
-00006de0: 6520 422d 4365 6c6c 204c 696e 6561 7220  e B-Cell Linear 
-00006df0: 4570 6974 6f70 6520 5072 6564 6963 7469  Epitope Predicti
-00006e00: 6f6e 5d28 6874 7470 733a 2f2f 7777 772e  on](https://www.
-00006e10: 6269 6f72 7869 762e 6f72 672f 636f 6e74  biorxiv.org/cont
-00006e20: 656e 742f 3130 2e31 3130 312f 3230 3232  ent/10.1101/2022
-00006e30: 2e31 302e 3137 2e35 3132 3631 3376 312e  .10.17.512613v1.
-00006e40: 6675 6c6c 2e70 6466 290a 2d20 5b45 7870  full.pdf).- [Exp
-00006e50: 6c61 696e 6162 6c65 2042 6f6f 7374 696e  lainable Boostin
-00006e60: 6720 4d61 6368 696e 6573 2066 6f72 2053  g Machines for S
-00006e70: 6c6f 7065 2046 6169 6c75 7265 2053 7061  lope Failure Spa
-00006e80: 7469 616c 2050 7265 6469 6374 6976 6520  tial Predictive 
-00006e90: 4d6f 6465 6c69 6e67 5d28 6874 7470 733a  Modeling](https:
-00006ea0: 2f2f 7777 772e 6d64 7069 2e63 6f6d 2f32  //www.mdpi.com/2
-00006eb0: 3037 322d 3432 3932 2f31 332f 3234 2f34  072-4292/13/24/4
-00006ec0: 3939 312f 6874 6d29 0a2d 205b 4d69 6372  991/htm).- [Micr
-00006ed0: 6f6d 6f64 656c 7320 666f 7220 4566 6669  omodels for Effi
-00006ee0: 6369 656e 742c 2045 7870 6c61 696e 6162  cient, Explainab
-00006ef0: 6c65 2c20 616e 6420 5265 7573 6162 6c65  le, and Reusable
-00006f00: 2053 7973 7465 6d73 3a20 4120 4361 7365   Systems: A Case
-00006f10: 2053 7475 6479 206f 6e20 4d65 6e74 616c   Study on Mental
-00006f20: 2048 6561 6c74 685d 2868 7474 7073 3a2f   Health](https:/
-00006f30: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
-00006f40: 3130 392e 3133 3737 302e 7064 6629 0a2d  109.13770.pdf).-
-00006f50: 205b 4964 656e 7469 6679 696e 6720 6d61   [Identifying ma
-00006f60: 696e 2061 6e64 2069 6e74 6572 6163 7469  in and interacti
-00006f70: 6f6e 2065 6666 6563 7473 206f 6620 7269  on effects of ri
-00006f80: 736b 2066 6163 746f 7273 2074 6f20 7072  sk factors to pr
-00006f90: 6564 6963 7420 696e 7465 6e73 6976 6520  edict intensive 
-00006fa0: 6361 7265 2061 646d 6973 7369 6f6e 2069  care admission i
-00006fb0: 6e20 7061 7469 656e 7473 2068 6f73 7069  n patients hospi
-00006fc0: 7461 6c69 7a65 6420 7769 7468 2043 4f56  talized with COV
-00006fd0: 4944 2d31 395d 2868 7474 7073 3a2f 2f77  ID-19](https://w
-00006fe0: 7777 2e6d 6564 7278 6976 2e6f 7267 2f63  ww.medrxiv.org/c
-00006ff0: 6f6e 7465 6e74 2f31 302e 3131 3031 2f32  ontent/10.1101/2
-00007000: 3032 302e 3036 2e33 302e 3230 3134 3336  020.06.30.201436
-00007010: 3531 7631 2e66 756c 6c2e 7064 6629 0a2d  51v1.full.pdf).-
-00007020: 205b 436f 6d70 6172 696e 6720 7468 6520   [Comparing the 
-00007030: 696e 7465 7270 7265 7461 6269 6c69 7479  interpretability
-00007040: 206f 6620 6d61 6368 696e 6520 6c65 6172   of machine lear
-00007050: 6e69 6e67 2063 6c61 7373 6966 6965 7273  ning classifiers
-00007060: 2066 6f72 2062 7261 696e 2074 756d 6f75   for brain tumou
-00007070: 7220 7375 7276 6976 616c 2070 7265 6469  r survival predi
-00007080: 6374 696f 6e5d 2868 7474 7073 3a2f 2f64  ction](https://d
-00007090: 656c 6976 6572 7970 6466 2e73 7372 6e2e  eliverypdf.ssrn.
-000070a0: 636f 6d2f 6465 6c69 7665 7279 2e70 6870  com/delivery.php
-000070b0: 3f49 443d 3736 3031 3232 3131 3830 3637  ?ID=760122118067
-000070c0: 3130 3330 3934 3130 3830 3930 3132 3330  1030941080901230
-000070d0: 3931 3037 3930 3131 3032 3830 3332 3030  9107901102803200
-000070e0: 3930 3039 3032 3330 3835 3030 3530 3134  9009023085005014
-000070f0: 3031 3430 3032 3132 3331 3035 3038 3531  0140021231050851
-00007100: 3134 3032 3530 3232 3032 3430 3035 3034  1402502202400504
-00007110: 3730 3738 3033 3130 3139 3038 3930 3733  7078031019089073
-00007120: 3132 3030 3132 3032 3531 3137 3037 3330  1200120251170730
-00007130: 3032 3036 3430 3331 3037 3130 3732 3131  0206403107107211
-00007140: 3330 3036 3036 3630 3335 3030 3130 3638  3006066035001068
-00007150: 3132 3530 3237 3032 3130 3837 3038 3730  1250270210870870
-00007160: 3833 3038 3530 3236 3130 3030 3039 3031  8308502610000901
-00007170: 3830 3435 3130 3730 3932 3036 3330 3031  8045107092063001
-00007180: 3032 3330 3638 3037 3130 3032 3132 3430  0230680710021240
-00007190: 3730 3130 3731 3230 3132 3030 3037 3031  7010712012000701
-000071a0: 3431 3032 3039 3431 3033 3036 3930 3839  4102094103069089
-000071b0: 3131 3930 3236 3131 3031 3034 3130 3730  1190261101041070
-000071c0: 3035 3033 3130 3935 3030 3130 3932 3039  0503109500109209
-000071d0: 3026 4558 543d 7064 6626 494e 4445 583d  0&EXT=pdf&INDEX=
-000071e0: 5452 5545 290a 2d20 5b55 7369 6e67 2049  TRUE).- [Using I
-000071f0: 6e74 6572 7072 6574 6162 6c65 204d 6163  nterpretable Mac
-00007200: 6869 6e65 204c 6561 726e 696e 6720 746f  hine Learning to
-00007210: 2050 7265 6469 6374 204d 6174 6572 6e61   Predict Materna
-00007220: 6c20 616e 6420 4665 7461 6c20 4f75 7463  l and Fetal Outc
-00007230: 6f6d 6573 5d28 6874 7470 733a 2f2f 6172  omes](https://ar
-00007240: 7869 762e 6f72 672f 7064 662f 3232 3037  xiv.org/pdf/2207
-00007250: 2e30 3533 3232 2e70 6466 290a 2d20 5b43  .05322.pdf).- [C
-00007260: 616c 6962 7261 7465 3a20 496e 7465 7261  alibrate: Intera
-00007270: 6374 6976 6520 416e 616c 7973 6973 206f  ctive Analysis o
-00007280: 6620 5072 6f62 6162 696c 6973 7469 6320  f Probabilistic 
-00007290: 4d6f 6465 6c20 4f75 7470 7574 5d28 6874  Model Output](ht
-000072a0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-000072b0: 7064 662f 3232 3037 2e31 3337 3730 2e70  pdf/2207.13770.p
-000072c0: 6466 290a 2d20 5b4e 6575 7261 6c20 4164  df).- [Neural Ad
-000072d0: 6469 7469 7665 204d 6f64 656c 733a 2049  ditive Models: I
-000072e0: 6e74 6572 7072 6574 6162 6c65 204d 6163  nterpretable Mac
-000072f0: 6869 6e65 204c 6561 726e 696e 6720 7769  hine Learning wi
-00007300: 7468 204e 6575 7261 6c20 4e65 7473 5d28  th Neural Nets](
-00007310: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00007320: 672f 7064 662f 3230 3034 2e31 3339 3132  g/pdf/2004.13912
-00007330: 2e70 6466 290a 2d20 5b4e 4f44 452d 4741  .pdf).- [NODE-GA
-00007340: 4d3a 204e 6575 7261 6c20 4765 6e65 7261  M: Neural Genera
-00007350: 6c69 7a65 6420 4164 6469 7469 7665 204d  lized Additive M
-00007360: 6f64 656c 2066 6f72 2049 6e74 6572 7072  odel for Interpr
-00007370: 6574 6162 6c65 2044 6565 7020 4c65 6172  etable Deep Lear
-00007380: 6e69 6e67 5d28 6874 7470 733a 2f2f 6172  ning](https://ar
-00007390: 7869 762e 6f72 672f 7064 662f 3231 3036  xiv.org/pdf/2106
-000073a0: 2e30 3136 3133 2e70 6466 290a 2d20 5b53  .01613.pdf).- [S
-000073b0: 6361 6c61 626c 6520 496e 7465 7270 7265  calable Interpre
-000073c0: 7461 6269 6c69 7479 2076 6961 2050 6f6c  tability via Pol
-000073d0: 796e 6f6d 6961 6c73 5d28 6874 7470 733a  ynomials](https:
-000073e0: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
-000073f0: 3232 3035 2e31 3431 3038 7631 2e70 6466  2205.14108v1.pdf
-00007400: 290a 2d20 5b4e 6575 7261 6c20 4261 7369  ).- [Neural Basi
-00007410: 7320 4d6f 6465 6c73 2066 6f72 2049 6e74  s Models for Int
-00007420: 6572 7072 6574 6162 696c 6974 795d 2868  erpretability](h
-00007430: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-00007440: 2f70 6466 2f32 3230 352e 3134 3132 302e  /pdf/2205.14120.
-00007450: 7064 6629 0a2d 205b 494c 4d41 5254 3a20  pdf).- [ILMART: 
-00007460: 496e 7465 7270 7265 7461 626c 6520 5261  Interpretable Ra
-00007470: 6e6b 696e 6720 7769 7468 2043 6f6e 7374  nking with Const
-00007480: 7261 696e 6564 204c 616d 6264 614d 4152  rained LambdaMAR
-00007490: 545d 2868 7474 7073 3a2f 2f61 7278 6976  T](https://arxiv
-000074a0: 2e6f 7267 2f70 6466 2f32 3230 362e 3030  .org/pdf/2206.00
-000074b0: 3437 332e 7064 6629 0a2d 205b 496e 7465  473.pdf).- [Inte
-000074c0: 6772 6174 696e 6720 436f 2d43 6c75 7374  grating Co-Clust
-000074d0: 6572 696e 6720 616e 6420 496e 7465 7270  ering and Interp
-000074e0: 7265 7461 626c 6520 4d61 6368 696e 6520  retable Machine 
-000074f0: 4c65 6172 6e69 6e67 2066 6f72 2074 6865  Learning for the
-00007500: 2050 7265 6469 6374 696f 6e20 6f66 2049   Prediction of I
-00007510: 6e74 7261 7665 6e6f 7573 2049 6d6d 756e  ntravenous Immun
-00007520: 6f67 6c6f 6275 6c69 6e20 5265 7369 7374  oglobulin Resist
-00007530: 616e 6365 2069 6e20 4b61 7761 7361 6b69  ance in Kawasaki
-00007540: 2044 6973 6561 7365 5d28 6874 7470 733a   Disease](https:
-00007550: 2f2f 6965 6565 7870 6c6f 7265 2e69 6565  //ieeexplore.iee
-00007560: 652e 6f72 672f 7374 616d 702f 7374 616d  e.org/stamp/stam
-00007570: 702e 6a73 703f 7470 3d26 6172 6e75 6d62  p.jsp?tp=&arnumb
-00007580: 6572 3d39 3039 3738 3734 290a 2d20 5b47  er=9097874).- [G
-00007590: 414d 492d 4e65 743a 2041 6e20 4578 706c  AMI-Net: An Expl
-000075a0: 6169 6e61 626c 6520 4e65 7572 616c 204e  ainable Neural N
-000075b0: 6574 776f 726b 2062 6173 6564 206f 6e20  etwork based on 
-000075c0: 4765 6e65 7261 6c69 7a65 6420 4164 6469  Generalized Addi
-000075d0: 7469 7665 204d 6f64 656c 7320 7769 7468  tive Models with
-000075e0: 2053 7472 7563 7475 7265 6420 496e 7465   Structured Inte
-000075f0: 7261 6374 696f 6e73 5d28 6874 7470 733a  ractions](https:
-00007600: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
-00007610: 3230 3033 2e30 3731 3332 7631 2e70 6466  2003.07132v1.pdf
-00007620: 290a 2d20 5b41 2043 6f6e 6365 7074 2061  ).- [A Concept a
-00007630: 6e64 2041 7267 756d 656e 7461 7469 6f6e  nd Argumentation
-00007640: 2062 6173 6564 2049 6e74 6572 7072 6574   based Interpret
-00007650: 6162 6c65 204d 6f64 656c 2069 6e20 4869  able Model in Hi
-00007660: 6768 2052 6973 6b20 446f 6d61 696e 735d  gh Risk Domains]
-00007670: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00007680: 7267 2f70 6466 2f32 3230 382e 3038 3134  rg/pdf/2208.0814
-00007690: 392e 7064 6629 0a2d 205b 416e 616c 797a  9.pdf).- [Analyz
-000076a0: 696e 6720 7468 6520 4469 6666 6572 656e  ing the Differen
-000076b0: 6365 7320 6265 7477 6565 6e20 5072 6f66  ces between Prof
-000076c0: 6573 7369 6f6e 616c 2061 6e64 2041 6d61  essional and Ama
-000076d0: 7465 7572 2045 7370 6f72 7473 2074 6872  teur Esports thr
-000076e0: 6f75 6768 2057 696e 2050 726f 6261 6269  ough Win Probabi
-000076f0: 6c69 7479 5d28 6874 7470 733a 2f2f 646c  lity](https://dl
-00007700: 2e61 636d 2e6f 7267 2f64 6f69 2f70 6466  .acm.org/doi/pdf
-00007710: 2f31 302e 3131 3435 2f33 3438 3534 3437  /10.1145/3485447
-00007720: 2e33 3531 3232 3737 290a 2d20 5b45 7870  .3512277).- [Exp
-00007730: 6c61 696e 6162 6c65 206d 6163 6869 6e65  lainable machine
-00007740: 206c 6561 726e 696e 6720 7769 7468 2070   learning with p
-00007750: 6169 7277 6973 6520 696e 7465 7261 6374  airwise interact
-00007760: 696f 6e73 2066 6f72 2074 6865 2063 6c61  ions for the cla
-00007770: 7373 6966 6361 7469 6f6e 206f 6620 5061  ssifcation of Pa
-00007780: 726b 696e 736f 6ee2 8099 7320 6469 7365  rkinson...s dise
-00007790: 6173 6520 616e 6420 5357 4544 4420 6672  ase and SWEDD fr
-000077a0: 6f6d 2063 6c69 6e69 6361 6c20 616e 6420  om clinical and 
-000077b0: 696d 6167 696e 6720 6665 6174 7572 6573  imaging features
-000077c0: 5d28 6874 7470 733a 2f2f 7777 772e 6e63  ](https://www.nc
-000077d0: 6269 2e6e 6c6d 2e6e 6968 2e67 6f76 2f70  bi.nlm.nih.gov/p
-000077e0: 6d63 2f61 7274 6963 6c65 732f 504d 4339  mc/articles/PMC9
-000077f0: 3133 3237 3631 2f70 6466 2f31 3136 3832  132761/pdf/11682
-00007800: 5f32 3032 325f 4172 7469 636c 655f 3638  _2022_Article_68
-00007810: 382e 7064 6629 0a2d 205b 496e 7465 7270  8.pdf).- [Interp
-00007820: 7265 7461 626c 6520 5072 6564 6963 7469  retable Predicti
-00007830: 6f6e 206f 6620 476f 616c 7320 696e 2053  on of Goals in S
-00007840: 6f63 6365 725d 2868 7474 7073 3a2f 2f73  occer](https://s
-00007850: 7461 7473 626f 6d62 2e63 6f6d 2f77 702d  tatsbomb.com/wp-
-00007860: 636f 6e74 656e 742f 7570 6c6f 6164 732f  content/uploads/
-00007870: 3230 3139 2f31 302f 6465 6372 6f6f 732d  2019/10/decroos-
-00007880: 696e 7465 7270 7265 7461 6269 6c69 7479  interpretability
-00007890: 2d73 7461 7473 626f 6d62 2e70 6466 290a  -statsbomb.pdf).
-000078a0: 2d20 5b45 7874 656e 6469 6e67 2074 6865  - [Extending the
-000078b0: 2054 7365 746c 696e 204d 6163 6869 6e65   Tsetlin Machine
-000078c0: 2077 6974 6820 496e 7465 6765 722d 5765   with Integer-We
-000078d0: 6967 6874 6564 2043 6c61 7573 6573 2066  ighted Clauses f
-000078e0: 6f72 2049 6e63 7265 6173 6564 2049 6e74  or Increased Int
-000078f0: 6572 7072 6574 6162 696c 6974 795d 2868  erpretability](h
-00007900: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-00007910: 2f70 6466 2f32 3030 352e 3035 3133 312e  /pdf/2005.05131.
-00007920: 7064 6629 0a2d 205b 496e 2050 7572 7375  pdf).- [In Pursu
-00007930: 6974 206f 6620 496e 7465 7270 7265 7461  it of Interpreta
-00007940: 626c 652c 2046 6169 7220 616e 6420 4163  ble, Fair and Ac
-00007950: 6375 7261 7465 204d 6163 6869 6e65 204c  curate Machine L
-00007960: 6561 726e 696e 6720 666f 7220 4372 696d  earning for Crim
-00007970: 696e 616c 2052 6563 6964 6976 6973 6d20  inal Recidivism 
-00007980: 5072 6564 6963 7469 6f6e 5d28 6874 7470  Prediction](http
-00007990: 733a 2f2f 6172 7869 762e 6f72 672f 7064  s://arxiv.org/pd
-000079a0: 662f 3230 3035 2e30 3431 3736 2e70 6466  f/2005.04176.pdf
-000079b0: 290a 2d20 5b46 726f 6d20 5368 6170 6c65  ).- [From Shaple
-000079c0: 7920 5661 6c75 6573 2074 6f20 4765 6e65  y Values to Gene
-000079d0: 7261 6c69 7a65 6420 4164 6469 7469 7665  ralized Additive
-000079e0: 204d 6f64 656c 7320 616e 6420 6261 636b   Models and back
-000079f0: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
-00007a00: 6f72 672f 7064 662f 3232 3039 2e30 3430  org/pdf/2209.040
-00007a10: 3132 2e70 6466 290a 2d20 5b41 6e20 4578  12.pdf).- [An Ex
-00007a20: 706c 6169 6e61 626c 6520 4d61 6368 696e  plainable Machin
-00007a30: 6520 4c65 6172 6e69 6e67 2041 7070 726f  e Learning Appro
-00007a40: 6163 6820 746f 2056 6973 7561 6c2d 496e  ach to Visual-In
-00007a50: 7465 7261 6374 6976 6520 4c61 6265 6c69  teractive Labeli
-00007a60: 6e67 3a20 4120 4361 7365 2053 7475 6479  ng: A Case Study
-00007a70: 206f 6e20 4e6f 6e2d 636f 6d6d 756e 6963   on Non-communic
-00007a80: 6162 6c65 2044 6973 6561 7365 2044 6174  able Disease Dat
-00007a90: 615d 2868 7474 7073 3a2f 2f61 7278 6976  a](https://arxiv
-00007aa0: 2e6f 7267 2f70 6466 2f32 3230 392e 3132  .org/pdf/2209.12
-00007ab0: 3737 382e 7064 6629 0a2d 205b 4465 7665  778.pdf).- [Deve
-00007ac0: 6c6f 706d 656e 7420 616e 6420 5661 6c69  lopment and Vali
-00007ad0: 6461 7469 6f6e 206f 6620 616e 2049 6e74  dation of an Int
-00007ae0: 6572 7072 6574 6162 6c65 2033 2d64 6179  erpretable 3-day
-00007af0: 2049 6e74 656e 7369 7665 2043 6172 6520   Intensive Care 
-00007b00: 556e 6974 2052 6561 646d 6973 7369 6f6e  Unit Readmission
-00007b10: 2050 7265 6469 6374 696f 6e20 4d6f 6465   Prediction Mode
-00007b20: 6c20 5573 696e 6720 4578 706c 6169 6e61  l Using Explaina
-00007b30: 626c 6520 426f 6f73 7469 6e67 204d 6163  ble Boosting Mac
-00007b40: 6869 6e65 735d 2868 7474 7073 3a2f 2f77  hines](https://w
-00007b50: 7777 2e6d 6564 7278 6976 2e6f 7267 2f63  ww.medrxiv.org/c
-00007b60: 6f6e 7465 6e74 2f31 302e 3131 3031 2f32  ontent/10.1101/2
-00007b70: 3032 312e 3131 2e30 312e 3231 3236 3537  021.11.01.212657
-00007b80: 3030 7631 2e66 756c 6c2e 7064 6629 0a2d  00v1.full.pdf).-
-00007b90: 205b 4465 6174 6820 6279 2052 6f75 6e64   [Death by Round
-00007ba0: 204e 756d 6265 7273 2061 6e64 2053 6861   Numbers and Sha
-00007bb0: 7270 2054 6872 6573 686f 6c64 733a 2048  rp Thresholds: H
-00007bc0: 6f77 2074 6f20 4176 6f69 6420 4461 6e67  ow to Avoid Dang
-00007bd0: 6572 6f75 7320 4149 2045 4852 2052 6563  erous AI EHR Rec
-00007be0: 6f6d 6d65 6e64 6174 696f 6e73 5d28 6874  ommendations](ht
-00007bf0: 7470 733a 2f2f 7777 772e 6d65 6472 7869  tps://www.medrxi
-00007c00: 762e 6f72 672f 636f 6e74 656e 742f 3130  v.org/content/10
-00007c10: 2e31 3130 312f 3230 3232 2e30 342e 3330  .1101/2022.04.30
-00007c20: 2e32 3232 3734 3532 3076 312e 6675 6c6c  .22274520v1.full
-00007c30: 2e70 6466 290a 2d20 5b42 7569 6c64 696e  .pdf).- [Buildin
-00007c40: 6720 6120 7072 6564 6963 7469 7665 206d  g a predictive m
-00007c50: 6f64 656c 2074 6f20 6964 656e 7469 6679  odel to identify
-00007c60: 2063 6c69 6e69 6361 6c20 696e 6469 6361   clinical indica
-00007c70: 746f 7273 2066 6f72 2043 4f56 4944 2d31  tors for COVID-1
-00007c80: 3920 7573 696e 6720 6d61 6368 696e 6520  9 using machine 
-00007c90: 6c65 6172 6e69 6e67 206d 6574 686f 645d  learning method]
-00007ca0: 2868 7474 7073 3a2f 2f77 7777 2e6e 6362  (https://www.ncb
-00007cb0: 692e 6e6c 6d2e 6e69 682e 676f 762f 706d  i.nlm.nih.gov/pm
-00007cc0: 632f 6172 7469 636c 6573 2f50 4d43 3930  c/articles/PMC90
-00007cd0: 3337 3937 322f 7064 662f 3131 3531 375f  37972/pdf/11517_
-00007ce0: 3230 3232 5f41 7274 6963 6c65 5f32 3536  2022_Article_256
-00007cf0: 382e 7064 6629 0a2d 205b 5573 696e 6720  8.pdf).- [Using 
-00007d00: 496e 6e6f 7661 7469 7665 204d 6163 6869  Innovative Machi
-00007d10: 6e65 204c 6561 726e 696e 6720 4d65 7468  ne Learning Meth
-00007d20: 6f64 7320 746f 2053 6372 6565 6e20 616e  ods to Screen an
-00007d30: 6420 4964 656e 7469 6679 2050 7265 6469  d Identify Predi
-00007d40: 6374 6f72 7320 6f66 2043 6f6e 6765 6e69  ctors of Congeni
-00007d50: 7461 6c20 4865 6172 7420 4469 7365 6173  tal Heart Diseas
-00007d60: 6573 5d28 6874 7470 733a 2f2f 7777 772e  es](https://www.
-00007d70: 6e63 6269 2e6e 6c6d 2e6e 6968 2e67 6f76  ncbi.nlm.nih.gov
-00007d80: 2f70 6d63 2f61 7274 6963 6c65 732f 504d  /pmc/articles/PM
-00007d90: 4338 3737 3730 3232 2f70 6466 2f66 6376  C8777022/pdf/fcv
-00007da0: 6d2d 3038 2d37 3937 3030 322e 7064 6629  m-08-797002.pdf)
-00007db0: 0a2d 205b 4578 706c 6169 6e61 626c 6520  .- [Explainable 
-00007dc0: 426f 6f73 7469 6e67 204d 6163 6869 6e65  Boosting Machine
-00007dd0: 2066 6f72 2050 7265 6469 6374 696e 6720   for Predicting 
-00007de0: 416c 7a68 6569 6d65 72e2 8099 7320 4469  Alzheimer...s Di
-00007df0: 7365 6173 6520 6672 6f6d 204d 5249 2048  sease from MRI H
-00007e00: 6970 706f 6361 6d70 616c 2053 7562 6669  ippocampal Subfi
-00007e10: 656c 6473 5d28 6874 7470 733a 2f2f 6c69  elds](https://li
-00007e20: 6e6b 2e73 7072 696e 6765 722e 636f 6d2f  nk.springer.com/
-00007e30: 6368 6170 7465 722f 3130 2e31 3030 372f  chapter/10.1007/
-00007e40: 3937 382d 332d 3033 302d 3836 3939 332d  978-3-030-86993-
-00007e50: 395f 3331 290a 2d20 5b49 6d70 6163 7420  9_31).- [Impact 
-00007e60: 6f66 2041 6363 7572 6163 7920 6f6e 204d  of Accuracy on M
-00007e70: 6f64 656c 2049 6e74 6572 7072 6574 6174  odel Interpretat
-00007e80: 696f 6e73 5d28 6874 7470 733a 2f2f 6172  ions](https://ar
-00007e90: 7869 762e 6f72 672f 7064 662f 3230 3131  xiv.org/pdf/2011
-00007ea0: 2e30 3939 3033 2e70 6466 290a 0a23 2042  .09903.pdf)..# B
-00007eb0: 6f6f 6b73 2074 6861 7420 6469 7363 7573  ooks that discus
-00007ec0: 7320 4542 4d73 0a0a 2d20 5b49 6e74 6572  s EBMs..- [Inter
-00007ed0: 7072 6574 6162 6c65 204d 6163 6869 6e65  pretable Machine
-00007ee0: 204c 6561 726e 696e 6720 7769 7468 2050   Learning with P
-00007ef0: 7974 686f 6e5d 2868 7474 7073 3a2f 2f77  ython](https://w
-00007f00: 7777 2e61 6d61 7a6f 6e2e 636f 6d2f 496e  ww.amazon.com/In
-00007f10: 7465 7270 7265 7461 626c 652d 4d61 6368  terpretable-Mach
-00007f20: 696e 652d 4c65 6172 6e69 6e67 2d50 7974  ine-Learning-Pyt
-00007f30: 686f 6e2d 6861 6e64 732f 6470 2f31 3830  hon-hands/dp/180
-00007f40: 3032 3033 3930 5829 0a2d 205b 4578 706c  020390X).- [Expl
-00007f50: 6169 6e61 626c 6520 4172 7469 6669 6369  ainable Artifici
-00007f60: 616c 2049 6e74 656c 6c69 6765 6e63 653a  al Intelligence:
-00007f70: 2041 6e20 496e 7472 6f64 7563 7469 6f6e   An Introduction
-00007f80: 2074 6f20 496e 7465 7270 7265 7461 626c   to Interpretabl
-00007f90: 6520 4d61 6368 696e 6520 4c65 6172 6e69  e Machine Learni
-00007fa0: 6e67 5d28 6874 7470 733a 2f2f 7777 772e  ng](https://www.
-00007fb0: 616d 617a 6f6e 2e63 6f6d 2f45 7870 6c61  amazon.com/Expla
-00007fc0: 696e 6162 6c65 2d41 7274 6966 6963 6961  inable-Artificia
-00007fd0: 6c2d 496e 7465 6c6c 6967 656e 6365 5f2d  l-Intelligence_-
-00007fe0: 416e 2d49 6e74 726f 6475 6374 696f 6e2d  An-Introduction-
-00007ff0: 746f 2d49 6e74 6572 7072 6574 6162 6c65  to-Interpretable
-00008000: 2d58 4149 2f64 702f 3330 3330 3833 3335  -XAI/dp/30308335
-00008010: 3530 290a 2d20 5b4d 6163 6869 6e65 204c  50).- [Machine L
-00008020: 6561 726e 696e 6720 666f 7220 4869 6768  earning for High
-00008030: 2d52 6973 6b20 4170 706c 6963 6174 696f  -Risk Applicatio
-00008040: 6e73 5d28 6874 7470 733a 2f2f 7777 772e  ns](https://www.
-00008050: 6f72 6569 6c6c 792e 636f 6d2f 6c69 6272  oreilly.com/libr
-00008060: 6172 792f 7669 6577 2f6d 6163 6869 6e65  ary/view/machine
-00008070: 2d6c 6561 726e 696e 672d 666f 722f 3937  -learning-for/97
-00008080: 3831 3039 3831 3032 3432 352f 290a 2d20  81098102425/).- 
-00008090: 5b41 7070 6c69 6564 204d 6163 6869 6e65  [Applied Machine
-000080a0: 204c 6561 726e 696e 6720 4578 706c 6169   Learning Explai
-000080b0: 6e61 6269 6c69 7479 2054 6563 686e 6971  nability Techniq
-000080c0: 7565 735d 2868 7474 7073 3a2f 2f77 7777  ues](https://www
-000080d0: 2e61 6d61 7a6f 6e2e 636f 6d2f 4170 706c  .amazon.com/Appl
-000080e0: 6965 642d 4d61 6368 696e 652d 4c65 6172  ied-Machine-Lear
-000080f0: 6e69 6e67 2d45 7870 6c61 696e 6162 696c  ning-Explainabil
-00008100: 6974 792d 5465 6368 6e69 7175 6573 2f64  ity-Techniques/d
-00008110: 702f 3138 3033 3234 3631 3534 290a 2d20  p/1803246154).- 
-00008120: 5b54 6865 2065 5870 6c61 696e 6162 6c65  [The eXplainable
-00008130: 2041 2e49 2e3a 2057 6974 6820 5079 7468   A.I.: With Pyth
-00008140: 6f6e 2065 7861 6d70 6c65 735d 2868 7474  on examples](htt
-00008150: 7073 3a2f 2f77 7777 2e61 6d61 7a6f 6e2e  ps://www.amazon.
-00008160: 636f 6d2f 6558 706c 6169 6e61 626c 652d  com/eXplainable-
-00008170: 492d 5079 7468 6f6e 2d65 7861 6d70 6c65  I-Python-example
-00008180: 732d 6562 6f6f 6b2f 6470 2f42 3042 3446  s-ebook/dp/B0B4F
-00008190: 3938 4d4e 3629 0a2d 205b 4578 706c 6169  98MN6).- [Explai
-000081a0: 6e61 626c 6520 4149 2052 6563 6970 6573  nable AI Recipes
-000081b0: 5d28 6874 7470 733a 2f2f 7777 772e 616d  ](https://www.am
-000081c0: 617a 6f6e 2e63 6f6d 2f45 7870 6c61 696e  azon.com/Explain
-000081d0: 6162 6c65 2d52 6563 6970 6573 2d49 6d70  able-Recipes-Imp
-000081e0: 6c65 6d65 6e74 2d45 7870 6c61 696e 6162  lement-Explainab
-000081f0: 696c 6974 792d 496e 7465 7270 7265 7461  ility-Interpreta
-00008200: 6269 6c69 7479 2d65 626f 6f6b 2f64 702f  bility-ebook/dp/
-00008210: 4230 4253 4635 4e42 5937 290a 0a23 2045  B0BSF5NBY7)..# E
-00008220: 7874 6572 6e61 6c20 746f 6f6c 730a 0a2d  xternal tools..-
-00008230: 205b 4542 4d20 746f 204f 6e6e 7820 636f   [EBM to Onnx co
-00008240: 6e76 6572 7465 7220 6279 2053 6f66 7441  nverter by SoftA
-00008250: 7448 6f6d 655d 2868 7474 7073 3a2f 2f67  tHome](https://g
-00008260: 6974 6875 622e 636f 6d2f 696e 7465 7270  ithub.com/interp
-00008270: 7265 746d 6c2f 6562 6d32 6f6e 6e78 290a  retml/ebm2onnx).
-00008280: 2d20 5b47 414d 2043 6861 6e67 6572 5d28  - [GAM Changer](
-00008290: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000082a0: 6f6d 2f69 6e74 6572 7072 6574 6d6c 2f67  om/interpretml/g
-000082b0: 616d 2d63 6861 6e67 6572 290a 2d20 5b4d  am-changer).- [M
-000082c0: 4c20 3220 5351 4c20 2865 7870 6572 696d  L 2 SQL (experim
-000082d0: 656e 7461 6c29 5d28 6874 7470 733a 2f2f  ental)](https://
-000082e0: 6769 7468 7562 2e63 6f6d 2f6b 6173 7065  github.com/kaspe
-000082f0: 7273 6769 742f 6d6c 5f32 5f73 716c 290a  rsgit/ml_2_sql).
-00008300: 0a23 2043 6f6e 7461 6374 2075 730a 0a54  .# Contact us..T
-00008310: 6865 7265 2061 7265 206d 756c 7469 706c  here are multipl
-00008320: 6520 7761 7973 2074 6f20 6765 7420 696e  e ways to get in
-00008330: 2074 6f75 6368 3a0a 2d20 456d 6169 6c20   touch:.- Email 
-00008340: 7573 2061 7420 696e 7465 7270 7265 7440  us at interpret@
-00008350: 6d69 6372 6f73 6f66 742e 636f 6d0a 2d20  microsoft.com.- 
-00008360: 4f72 2c20 6665 656c 2066 7265 6520 746f  Or, feel free to
-00008370: 2072 6169 7365 2061 2047 6974 4875 6220   raise a GitHub 
-00008380: 6973 7375 650a 0a3c 6272 2f3e 0a3c 6272  issue..<br/>.<br
-00008390: 2f3e 0a3c 6272 2f3e 0a3c 6272 2f3e 0a3c  />.<br/>.<br/>.<
-000083a0: 6272 2f3e 0a0a 3c62 722f 3e0a 3c62 722f  br/>..<br/>.<br/
-000083b0: 3e0a 3c62 722f 3e0a 3c62 722f 3e0a 3c62  >.<br/>.<br/>.<b
-000083c0: 722f 3e0a 0a3c 6272 2f3e 0a3c 6272 2f3e  r/>..<br/>.<br/>
-000083d0: 0a3c 6272 2f3e 0a3c 6272 2f3e 0a3c 6272  .<br/>.<br/>.<br
-000083e0: 2f3e 0a0a 3c62 722f 3e0a 3c62 722f 3e0a  />..<br/>.<br/>.
-000083f0: 3c62 722f 3e0a 3c62 722f 3e0a 3c62 722f  <br/>.<br/>.<br/
-00008400: 3e0a 0a3c 6272 2f3e 0a3c 6272 2f3e 0a3c  >..<br/>.<br/>.<
-00008410: 6272 2f3e 0a3c 6272 2f3e 0a3c 6272 2f3e  br/>.<br/>.<br/>
-00008420: 0a0a 3c62 722f 3e0a 3c62 722f 3e0a 3c62  ..<br/>.<br/>.<b
-00008430: 722f 3e0a 3c62 722f 3e0a 3c62 722f 3e0a  r/>.<br/>.<br/>.
-00008440: 0a3c 6272 2f3e 0a3c 6272 2f3e 0a3c 6272  .<br/>.<br/>.<br
-00008450: 2f3e 0a3c 6272 2f3e 0a3c 6272 2f3e 0a0a  />.<br/>.<br/>..
-00008460: 3c62 722f 3e0a 3c62 722f 3e0a 3c62 722f  <br/>.<br/>.<br/
-00008470: 3e0a 3c62 722f 3e0a 3c62 722f 3e0a 0a3e  >.<br/>.<br/>..>
-00008480: 2023 2323 2049 6620 6120 7472 6565 2066   ### If a tree f
-00008490: 656c 6c20 696e 2079 6f75 7220 7261 6e64  ell in your rand
-000084a0: 6f6d 2066 6f72 6573 742c 2077 6f75 6c64  om forest, would
-000084b0: 2061 6e79 6f6e 6520 6e6f 7469 6365 3f0a   anyone notice?.
+00000000: 2320 496e 7465 7270 7265 744d 4c0a 0a3c  # InterpretML..<
+00000010: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000020: 6769 7468 7562 746f 636f 6c61 622e 636f  githubtocolab.co
+00000030: 6d2f 696e 7465 7270 7265 746d 6c2f 696e  m/interpretml/in
+00000040: 7465 7270 7265 742f 626c 6f62 2f64 6576  terpret/blob/dev
+00000050: 656c 6f70 2f65 7861 6d70 6c65 732f 7079  elop/examples/py
+00000060: 7468 6f6e 2f49 6e74 6572 7072 6574 6162  thon/Interpretab
+00000070: 6c65 5f43 6c61 7373 6966 6963 6174 696f  le_Classificatio
+00000080: 6e5f 4d65 7468 6f64 732e 6970 796e 6222  n_Methods.ipynb"
+00000090: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+000000a0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
+000000b0: 682e 676f 6f67 6c65 2e63 6f6d 2f61 7373  h.google.com/ass
+000000c0: 6574 732f 636f 6c61 622d 6261 6467 652e  ets/colab-badge.
+000000d0: 7376 6722 2061 6c74 3d22 4f70 656e 2049  svg" alt="Open I
+000000e0: 6e20 436f 6c61 6222 2f3e 3c2f 613e 0a5b  n Colab"/></a>.[
+000000f0: 215b 4269 6e64 6572 5d28 6874 7470 733a  ![Binder](https:
+00000100: 2f2f 6d79 6269 6e64 6572 2e6f 7267 2f62  //mybinder.org/b
+00000110: 6164 6765 5f6c 6f67 6f2e 7376 6729 5d28  adge_logo.svg)](
+00000120: 6874 7470 733a 2f2f 6d79 6269 6e64 6572  https://mybinder
+00000130: 2e6f 7267 2f76 322f 6768 2f69 6e74 6572  .org/v2/gh/inter
+00000140: 7072 6574 6d6c 2f69 6e74 6572 7072 6574  pretml/interpret
+00000150: 2f64 6576 656c 6f70 3f6c 6162 7061 7468  /develop?labpath
+00000160: 3d65 7861 6d70 6c65 7325 3246 7079 7468  =examples%2Fpyth
+00000170: 6f6e 2532 4649 6e74 6572 7072 6574 6162  on%2FInterpretab
+00000180: 6c65 5f43 6c61 7373 6966 6963 6174 696f  le_Classificatio
+00000190: 6e5f 4d65 7468 6f64 732e 6970 796e 6229  n_Methods.ipynb)
+000001a0: 0a21 5b4c 6963 656e 7365 5d28 6874 7470  .![License](http
+000001b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000001c0: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
+000001d0: 652f 696e 7465 7270 7265 746d 6c2f 696e  e/interpretml/in
+000001e0: 7465 7270 7265 742e 7376 673f 7374 796c  terpret.svg?styl
+000001f0: 653d 666c 6174 2d73 7175 6172 6529 0a21  e=flat-square).!
+00000200: 5b50 7974 686f 6e20 5665 7273 696f 6e5d  [Python Version]
+00000210: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000220: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+00000230: 6572 7369 6f6e 732f 696e 7465 7270 7265  ersions/interpre
+00000240: 742e 7376 673f 7374 796c 653d 666c 6174  t.svg?style=flat
+00000250: 2d73 7175 6172 6529 0a21 5b50 6163 6b61  -square).![Packa
+00000260: 6765 2056 6572 7369 6f6e 5d28 6874 7470  ge Version](http
+00000270: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000280: 696f 2f70 7970 692f 762f 696e 7465 7270  io/pypi/v/interp
+00000290: 7265 742e 7376 673f 7374 796c 653d 666c  ret.svg?style=fl
+000002a0: 6174 2d73 7175 6172 6529 0a21 5b43 6f6e  at-square).![Con
+000002b0: 6461 5d28 6874 7470 733a 2f2f 696d 672e  da](https://img.
+000002c0: 7368 6965 6c64 732e 696f 2f63 6f6e 6461  shields.io/conda
+000002d0: 2f76 2f63 6f6e 6461 2d66 6f72 6765 2f69  /v/conda-forge/i
+000002e0: 6e74 6572 7072 6574 290a 215b 4275 696c  nterpret).![Buil
+000002f0: 6420 5374 6174 7573 5d28 6874 7470 733a  d Status](https:
+00000300: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000310: 2f61 7a75 7265 2d64 6576 6f70 732f 6275  /azure-devops/bu
+00000320: 696c 642f 6d73 2f69 6e74 6572 7072 6574  ild/ms/interpret
+00000330: 2f32 3933 2f64 6576 656c 6f70 2e73 7667  /293/develop.svg
+00000340: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
+00000350: 7265 290a 215b 436f 7665 7261 6765 5d28  re).![Coverage](
+00000360: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000370: 6c64 732e 696f 2f61 7a75 7265 2d64 6576  lds.io/azure-dev
+00000380: 6f70 732f 636f 7665 7261 6765 2f6d 732f  ops/coverage/ms/
+00000390: 696e 7465 7270 7265 742f 3239 332f 6465  interpret/293/de
+000003a0: 7665 6c6f 702e 7376 673f 7374 796c 653d  velop.svg?style=
+000003b0: 666c 6174 2d73 7175 6172 6529 0a21 5b4d  flat-square).![M
+000003c0: 6169 6e74 656e 616e 6365 5d28 6874 7470  aintenance](http
+000003d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000003e0: 696f 2f6d 6169 6e74 656e 616e 6365 2f79  io/maintenance/y
+000003f0: 6573 2f32 3032 333f 7374 796c 653d 666c  es/2023?style=fl
+00000400: 6174 2d73 7175 6172 6529 0a3c 6272 2f3e  at-square).<br/>
+00000410: 0a3e 2023 2323 2049 6e20 7468 6520 6265  .> ### In the be
+00000420: 6769 6e6e 696e 6720 6d61 6368 696e 6573  ginning machines
+00000430: 206c 6561 726e 6564 2069 6e20 6461 726b   learned in dark
+00000440: 6e65 7373 2c20 616e 6420 6461 7461 2073  ness, and data s
+00000450: 6369 656e 7469 7374 7320 7374 7275 6767  cientists strugg
+00000460: 6c65 6420 696e 2074 6865 2076 6f69 6420  led in the void 
+00000470: 746f 2065 7870 6c61 696e 2074 6865 6d2e  to explain them.
+00000480: 200a 3e20 2323 2320 4c65 7420 7468 6572   .> ### Let ther
+00000490: 6520 6265 206c 6967 6874 2e0a 0a49 6e74  e be light...Int
+000004a0: 6572 7072 6574 4d4c 2069 7320 616e 206f  erpretML is an o
+000004b0: 7065 6e2d 736f 7572 6365 2070 6163 6b61  pen-source packa
+000004c0: 6765 2074 6861 7420 696e 636f 7270 6f72  ge that incorpor
+000004d0: 6174 6573 2073 7461 7465 2d6f 662d 7468  ates state-of-th
+000004e0: 652d 6172 7420 6d61 6368 696e 6520 6c65  e-art machine le
+000004f0: 6172 6e69 6e67 2069 6e74 6572 7072 6574  arning interpret
+00000500: 6162 696c 6974 7920 7465 6368 6e69 7175  ability techniqu
+00000510: 6573 2075 6e64 6572 206f 6e65 2072 6f6f  es under one roo
+00000520: 662e 2057 6974 6820 7468 6973 2070 6163  f. With this pac
+00000530: 6b61 6765 2c20 796f 7520 6361 6e20 7472  kage, you can tr
+00000540: 6169 6e20 696e 7465 7270 7265 7461 626c  ain interpretabl
+00000550: 6520 676c 6173 7362 6f78 206d 6f64 656c  e glassbox model
+00000560: 7320 616e 6420 6578 706c 6169 6e20 626c  s and explain bl
+00000570: 6163 6b62 6f78 2073 7973 7465 6d73 2e20  ackbox systems. 
+00000580: 496e 7465 7270 7265 744d 4c20 6865 6c70  InterpretML help
+00000590: 7320 796f 7520 756e 6465 7273 7461 6e64  s you understand
+000005a0: 2079 6f75 7220 6d6f 6465 6c27 7320 676c   your model's gl
+000005b0: 6f62 616c 2062 6568 6176 696f 722c 206f  obal behavior, o
+000005c0: 7220 756e 6465 7273 7461 6e64 2074 6865  r understand the
+000005d0: 2072 6561 736f 6e73 2062 6568 696e 6420   reasons behind 
+000005e0: 696e 6469 7669 6475 616c 2070 7265 6469  individual predi
+000005f0: 6374 696f 6e73 2e0a 0a49 6e74 6572 7072  ctions...Interpr
+00000600: 6574 6162 696c 6974 7920 6973 2065 7373  etability is ess
+00000610: 656e 7469 616c 2066 6f72 3a0a 2d20 4d6f  ential for:.- Mo
+00000620: 6465 6c20 6465 6275 6767 696e 6720 2d20  del debugging - 
+00000630: 5768 7920 6469 6420 6d79 206d 6f64 656c  Why did my model
+00000640: 206d 616b 6520 7468 6973 206d 6973 7461   make this mista
+00000650: 6b65 3f0a 2d20 4665 6174 7572 6520 456e  ke?.- Feature En
+00000660: 6769 6e65 6572 696e 6720 2d20 486f 7720  gineering - How 
+00000670: 6361 6e20 4920 696d 7072 6f76 6520 6d79  can I improve my
+00000680: 206d 6f64 656c 3f0a 2d20 4465 7465 6374   model?.- Detect
+00000690: 696e 6720 6661 6972 6e65 7373 2069 7373  ing fairness iss
+000006a0: 7565 7320 2d20 446f 6573 206d 7920 6d6f  ues - Does my mo
+000006b0: 6465 6c20 6469 7363 7269 6d69 6e61 7465  del discriminate
+000006c0: 3f0a 2d20 4875 6d61 6e2d 4149 2063 6f6f  ?.- Human-AI coo
+000006d0: 7065 7261 7469 6f6e 202d 2048 6f77 2063  peration - How c
+000006e0: 616e 2049 2075 6e64 6572 7374 616e 6420  an I understand 
+000006f0: 616e 6420 7472 7573 7420 7468 6520 6d6f  and trust the mo
+00000700: 6465 6c27 7320 6465 6369 7369 6f6e 733f  del's decisions?
+00000710: 0a2d 2052 6567 756c 6174 6f72 7920 636f  .- Regulatory co
+00000720: 6d70 6c69 616e 6365 202d 2044 6f65 7320  mpliance - Does 
+00000730: 6d79 206d 6f64 656c 2073 6174 6973 6679  my model satisfy
+00000740: 206c 6567 616c 2072 6571 7569 7265 6d65   legal requireme
+00000750: 6e74 733f 0a2d 2048 6967 682d 7269 736b  nts?.- High-risk
+00000760: 2061 7070 6c69 6361 7469 6f6e 7320 2d20   applications - 
+00000770: 4865 616c 7468 6361 7265 2c20 6669 6e61  Healthcare, fina
+00000780: 6e63 652c 206a 7564 6963 6961 6c2c 202e  nce, judicial, .
+00000790: 2e2e 0a0a 215b 5d28 6874 7470 733a 2f2f  ....![](https://
+000007a0: 6769 7468 7562 2e63 6f6d 2f69 6e74 6572  github.com/inter
+000007b0: 7072 6574 6d6c 2f69 6e74 6572 7072 6574  pretml/interpret
+000007c0: 6d6c 2e67 6974 6875 622e 696f 2f62 6c6f  ml.github.io/blo
+000007d0: 622f 6d61 7374 6572 2f69 6e74 6572 7072  b/master/interpr
+000007e0: 6574 2d68 6967 686c 6967 6874 2e67 6966  et-highlight.gif
+000007f0: 290a 0a23 2049 6e73 7461 6c6c 6174 696f  )..# Installatio
+00000800: 6e0a 0a50 7974 686f 6e20 332e 372b 207c  n..Python 3.7+ |
+00000810: 204c 696e 7578 2c20 4d61 632c 2057 696e   Linux, Mac, Win
+00000820: 646f 7773 0a60 6060 7368 0a70 6970 2069  dows.```sh.pip i
+00000830: 6e73 7461 6c6c 2069 6e74 6572 7072 6574  nstall interpret
+00000840: 0a23 204f 520a 636f 6e64 6120 696e 7374  .# OR.conda inst
+00000850: 616c 6c20 2d63 2063 6f6e 6461 2d66 6f72  all -c conda-for
+00000860: 6765 2069 6e74 6572 7072 6574 0a60 6060  ge interpret.```
+00000870: 0a0a 2320 496e 7472 6f64 7563 696e 6720  ..# Introducing 
+00000880: 7468 6520 4578 706c 6169 6e61 626c 6520  the Explainable 
+00000890: 426f 6f73 7469 6e67 204d 6163 6869 6e65  Boosting Machine
+000008a0: 2028 4542 4d29 0a0a 4542 4d20 6973 2061   (EBM)..EBM is a
+000008b0: 6e20 696e 7465 7270 7265 7461 626c 6520  n interpretable 
+000008c0: 6d6f 6465 6c20 6465 7665 6c6f 7065 6420  model developed 
+000008d0: 6174 204d 6963 726f 736f 6674 2052 6573  at Microsoft Res
+000008e0: 6561 7263 683c 7375 703e 5b2a 5d28 2363  earch<sup>[*](#c
+000008f0: 6974 6174 696f 6e73 293c 2f73 7570 3e2e  itations)</sup>.
+00000900: 2049 7420 7573 6573 206d 6f64 6572 6e20   It uses modern 
+00000910: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
+00000920: 2074 6563 686e 6971 7565 7320 6c69 6b65   techniques like
+00000930: 2062 6167 6769 6e67 2c20 6772 6164 6965   bagging, gradie
+00000940: 6e74 2062 6f6f 7374 696e 672c 2061 6e64  nt boosting, and
+00000950: 2061 7574 6f6d 6174 6963 2069 6e74 6572   automatic inter
+00000960: 6163 7469 6f6e 2064 6574 6563 7469 6f6e  action detection
+00000970: 2074 6f20 6272 6561 7468 6520 6e65 7720   to breathe new 
+00000980: 6c69 6665 2069 6e74 6f20 7472 6164 6974  life into tradit
+00000990: 696f 6e61 6c20 4741 4d73 2028 4765 6e65  ional GAMs (Gene
+000009a0: 7261 6c69 7a65 6420 4164 6469 7469 7665  ralized Additive
+000009b0: 204d 6f64 656c 7329 2e20 5468 6973 206d   Models). This m
+000009c0: 616b 6573 2045 424d 7320 6173 2061 6363  akes EBMs as acc
+000009d0: 7572 6174 6520 6173 2073 7461 7465 2d6f  urate as state-o
+000009e0: 662d 7468 652d 6172 7420 7465 6368 6e69  f-the-art techni
+000009f0: 7175 6573 206c 696b 6520 7261 6e64 6f6d  ques like random
+00000a00: 2066 6f72 6573 7473 2061 6e64 2067 7261   forests and gra
+00000a10: 6469 656e 7420 626f 6f73 7465 6420 7472  dient boosted tr
+00000a20: 6565 732e 2048 6f77 6576 6572 2c20 756e  ees. However, un
+00000a30: 6c69 6b65 2074 6865 7365 2062 6c61 636b  like these black
+00000a40: 626f 7820 6d6f 6465 6c73 2c20 4542 4d73  box models, EBMs
+00000a50: 2070 726f 6475 6365 2065 7861 6374 2065   produce exact e
+00000a60: 7870 6c61 6e61 7469 6f6e 7320 616e 6420  xplanations and 
+00000a70: 6172 6520 6564 6974 6162 6c65 2062 7920  are editable by 
+00000a80: 646f 6d61 696e 2065 7870 6572 7473 2e0a  domain experts..
+00000a90: 0a7c 2044 6174 6173 6574 2f41 5552 4f43  .| Dataset/AUROC
+00000aa0: 207c 2044 6f6d 6169 6e20 207c 204c 6f67   | Domain  | Log
+00000ab0: 6973 7469 6320 5265 6772 6573 7369 6f6e  istic Regression
+00000ac0: 207c 2052 616e 646f 6d20 466f 7265 7374   | Random Forest
+00000ad0: 207c 2058 4742 6f6f 7374 2020 2020 2020   | XGBoost      
+00000ae0: 2020 207c 2045 7870 6c61 696e 6162 6c65     | Explainable
+00000af0: 2042 6f6f 7374 696e 6720 4d61 6368 696e   Boosting Machin
+00000b00: 6520 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  e |.|-----------
+00000b10: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 7c3a  ----|---------|:
+00000b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b30: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+00000b40: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+00000b50: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
+00000b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b70: 2d2d 2d2d 3a7c 0a7c 2041 6475 6c74 2049  ----:|.| Adult I
+00000b80: 6e63 6f6d 6520 207c 2046 696e 616e 6365  ncome  | Finance
+00000b90: 207c 202e 3930 37c2 b12e 3030 3320 2020   | .907...003   
+00000ba0: 2020 2020 2020 2020 7c20 2e39 3033 c2b1          | .903..
+00000bb0: 2e30 3032 2020 2020 207c 202e 3932 37c2  .002     | .927.
+00000bc0: b12e 3030 3120 2020 2020 2020 7c20 2a2a  ..001       | **
+00000bd0: 5f2e 3932 38c2 b12e 3030 325f 2a2a 2020  _.928...002_**  
+00000be0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00000bf0: 4865 6172 7420 4469 7365 6173 6520 7c20  Heart Disease | 
+00000c00: 4d65 6469 6361 6c20 7c20 2e38 3935 c2b1  Medical | .895..
+00000c10: 2e30 3330 2020 2020 2020 2020 2020 207c  .030           |
+00000c20: 202e 3839 30c2 b12e 3030 3820 2020 2020   .890...008     
+00000c30: 7c20 2e38 3531 c2b1 2e30 3138 2020 2020  | .851...018    
+00000c40: 2020 207c 202a 2a5f 2e38 3938 c2b1 2e30     | **_.898...0
+00000c50: 3133 5f2a 2a20 2020 2020 2020 2020 2020  13_**           
+00000c60: 2020 207c 0a7c 2042 7265 6173 7420 4361     |.| Breast Ca
+00000c70: 6e63 6572 207c 204d 6564 6963 616c 207c  ncer | Medical |
+00000c80: 202a 2a5f 2e39 3935 c2b1 2e30 3035 5f2a   **_.995...005_*
+00000c90: 2a20 2020 2020 7c20 2e39 3932 c2b1 2e30  *     | .992...0
+00000ca0: 3039 2020 2020 207c 202e 3939 32c2 b12e  09     | .992...
+00000cb0: 3031 3020 2020 2020 2020 7c20 2a2a 5f2e  010       | **_.
+00000cc0: 3939 35c2 b12e 3030 365f 2a2a 2020 2020  995...006_**    
+00000cd0: 2020 2020 2020 2020 2020 7c0a 7c20 5465            |.| Te
+00000ce0: 6c65 636f 6d20 4368 7572 6e20 7c20 4275  lecom Churn | Bu
+00000cf0: 7369 6e65 7373 7c20 2e38 3439 c2b1 2e30  siness| .849...0
+00000d00: 3035 2020 2020 2020 2020 2020 207c 202e  05           | .
+00000d10: 3832 34c2 b12e 3030 3420 2020 2020 7c20  824...004     | 
+00000d20: 2e38 3238 c2b1 2e30 3130 2020 2020 2020  .828...010      
+00000d30: 207c 202a 2a5f 2e38 3532 c2b1 2e30 3036   | **_.852...006
+00000d40: 5f2a 2a20 2020 2020 2020 2020 2020 2020  _**             
+00000d50: 207c 0a7c 2043 7265 6469 7420 4672 6175   |.| Credit Frau
+00000d60: 6420 207c 2053 6563 7572 6974 797c 202e  d  | Security| .
+00000d70: 3937 39c2 b12e 3030 3220 2020 2020 2020  979...002       
+00000d80: 2020 2020 7c20 2e39 3530 c2b1 2e30 3037      | .950...007
+00000d90: 2020 2020 207c 202a 2a5f 2e39 3831 c2b1       | **_.981..
+00000da0: 2e30 3033 5f2a 2a20 7c20 2a2a 5f2e 3938  .003_** | **_.98
+00000db0: 31c2 b12e 3030 335f 2a2a 2020 2020 2020  1...003_**      
+00000dc0: 2020 2020 2020 2020 7c0a 0a5b 2a4e 6f74          |..[*Not
+00000dd0: 6562 6f6f 6b20 666f 7220 7265 7072 6f64  ebook for reprod
+00000de0: 7563 696e 6720 7461 626c 652a 5d28 6874  ucing table*](ht
+00000df0: 7470 733a 2f2f 6e62 7669 6577 6572 2e6a  tps://nbviewer.j
+00000e00: 7570 7974 6572 2e6f 7267 2f67 6974 6875  upyter.org/githu
+00000e10: 622f 696e 7465 7270 7265 746d 6c2f 696e  b/interpretml/in
+00000e20: 7465 7270 7265 742f 626c 6f62 2f6d 6173  terpret/blob/mas
+00000e30: 7465 722f 6265 6e63 686d 6172 6b73 2f45  ter/benchmarks/E
+00000e40: 424d 2532 3043 6c61 7373 6966 6963 6174  BM%20Classificat
+00000e50: 696f 6e25 3230 436f 6d70 6172 6973 6f6e  ion%20Comparison
+00000e60: 2e69 7079 6e62 290a 0a23 2053 7570 706f  .ipynb)..# Suppo
+00000e70: 7274 6564 2054 6563 686e 6971 7565 730a  rted Techniques.
+00000e80: 0a7c 2049 6e74 6572 7072 6574 6162 696c  .| Interpretabil
+00000e90: 6974 7920 5465 6368 6e69 7175 6520 207c  ity Technique  |
+00000ea0: 2054 7970 6520 2020 2020 2020 2020 2020   Type           
+00000eb0: 2020 2020 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d      |.|---------
+00000ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ed0: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
+00000ee0: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 205b 4578  ---------|.| [Ex
+00000ef0: 706c 6169 6e61 626c 6520 426f 6f73 7469  plainable Boosti
+00000f00: 6e67 5d28 6874 7470 733a 2f2f 696e 7465  ng](https://inte
+00000f10: 7270 7265 742e 6d6c 2f64 6f63 732f 6562  rpret.ml/docs/eb
+00000f20: 6d2e 6874 6d6c 2920 2020 2020 2020 207c  m.html)        |
+00000f30: 2067 6c61 7373 626f 7820 6d6f 6465 6c20   glassbox model 
+00000f40: 2020 2020 7c0a 7c20 5b44 6563 6973 696f      |.| [Decisio
+00000f50: 6e20 5472 6565 5d28 6874 7470 733a 2f2f  n Tree](https://
+00000f60: 696e 7465 7270 7265 742e 6d6c 2f64 6f63  interpret.ml/doc
+00000f70: 732f 6474 2e68 746d 6c29 2020 2020 2020  s/dt.html)      
+00000f80: 2020 2020 2020 2020 2020 7c20 676c 6173            | glas
+00000f90: 7362 6f78 206d 6f64 656c 2020 2020 207c  sbox model     |
+00000fa0: 0a7c 205b 4465 6369 7369 6f6e 2052 756c  .| [Decision Rul
+00000fb0: 6520 4c69 7374 5d28 6874 7470 733a 2f2f  e List](https://
+00000fc0: 696e 7465 7270 7265 742e 6d6c 2f64 6f63  interpret.ml/doc
+00000fd0: 732f 6472 2e68 746d 6c29 2020 2020 2020  s/dr.html)      
+00000fe0: 2020 2020 207c 2067 6c61 7373 626f 7820       | glassbox 
+00000ff0: 6d6f 6465 6c20 2020 2020 7c0a 7c20 5b4c  model     |.| [L
+00001000: 696e 6561 722f 4c6f 6769 7374 6963 2052  inear/Logistic R
+00001010: 6567 7265 7373 696f 6e5d 2868 7474 7073  egression](https
+00001020: 3a2f 2f69 6e74 6572 7072 6574 2e6d 6c2f  ://interpret.ml/
+00001030: 646f 6373 2f6c 722e 6874 6d6c 2920 2020  docs/lr.html)   
+00001040: 7c20 676c 6173 7362 6f78 206d 6f64 656c  | glassbox model
+00001050: 2020 2020 207c 0a7c 205b 5348 4150 204b       |.| [SHAP K
+00001060: 6572 6e65 6c20 4578 706c 6169 6e65 725d  ernel Explainer]
+00001070: 2868 7474 7073 3a2f 2f69 6e74 6572 7072  (https://interpr
+00001080: 6574 2e6d 6c2f 646f 6373 2f73 6861 702e  et.ml/docs/shap.
+00001090: 6874 6d6c 2920 2020 2020 207c 2062 6c61  html)      | bla
+000010a0: 636b 626f 7820 6578 706c 6169 6e65 7220  ckbox explainer 
+000010b0: 7c0a 7c20 5b4c 494d 455d 2868 7474 7073  |.| [LIME](https
+000010c0: 3a2f 2f69 6e74 6572 7072 6574 2e6d 6c2f  ://interpret.ml/
+000010d0: 646f 6373 2f6c 696d 652e 6874 6d6c 2920  docs/lime.html) 
+000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010f0: 2020 2020 2020 7c20 626c 6163 6b62 6f78        | blackbox
+00001100: 2065 7870 6c61 696e 6572 207c 0a7c 205b   explainer |.| [
+00001110: 4d6f 7272 6973 2053 656e 7369 7469 7669  Morris Sensitivi
+00001120: 7479 2041 6e61 6c79 7369 735d 2868 7474  ty Analysis](htt
+00001130: 7073 3a2f 2f69 6e74 6572 7072 6574 2e6d  ps://interpret.m
+00001140: 6c2f 646f 6373 2f6d 7361 2e68 746d 6c29  l/docs/msa.html)
+00001150: 207c 2062 6c61 636b 626f 7820 6578 706c   | blackbox expl
+00001160: 6169 6e65 7220 7c0a 7c20 5b50 6172 7469  ainer |.| [Parti
+00001170: 616c 2044 6570 656e 6465 6e63 655d 2868  al Dependence](h
+00001180: 7474 7073 3a2f 2f69 6e74 6572 7072 6574  ttps://interpret
+00001190: 2e6d 6c2f 646f 6373 2f70 6470 2e68 746d  .ml/docs/pdp.htm
+000011a0: 6c29 2020 2020 2020 2020 2020 7c20 626c  l)          | bl
+000011b0: 6163 6b62 6f78 2065 7870 6c61 696e 6572  ackbox explainer
+000011c0: 207c 0a0a 2320 5472 6169 6e20 6120 676c   |..# Train a gl
+000011d0: 6173 7362 6f78 206d 6f64 656c 0a0a 4c65  assbox model..Le
+000011e0: 7427 7320 6669 7420 616e 2045 7870 6c61  t's fit an Expla
+000011f0: 696e 6162 6c65 2042 6f6f 7374 696e 6720  inable Boosting 
+00001200: 4d61 6368 696e 650a 0a60 6060 7079 7468  Machine..```pyth
+00001210: 6f6e 0a66 726f 6d20 696e 7465 7270 7265  on.from interpre
+00001220: 742e 676c 6173 7362 6f78 2069 6d70 6f72  t.glassbox impor
+00001230: 7420 4578 706c 6169 6e61 626c 6542 6f6f  t ExplainableBoo
+00001240: 7374 696e 6743 6c61 7373 6966 6965 720a  stingClassifier.
+00001250: 0a65 626d 203d 2045 7870 6c61 696e 6162  .ebm = Explainab
+00001260: 6c65 426f 6f73 7469 6e67 436c 6173 7369  leBoostingClassi
+00001270: 6669 6572 2829 0a65 626d 2e66 6974 2858  fier().ebm.fit(X
+00001280: 5f74 7261 696e 2c20 795f 7472 6169 6e29  _train, y_train)
+00001290: 0a0a 2320 6f72 2073 7562 7374 6974 7574  ..# or substitut
+000012a0: 6520 7769 7468 204c 6f67 6973 7469 6352  e with LogisticR
+000012b0: 6567 7265 7373 696f 6e2c 2044 6563 6973  egression, Decis
+000012c0: 696f 6e54 7265 6543 6c61 7373 6966 6965  ionTreeClassifie
+000012d0: 722c 2052 756c 654c 6973 7443 6c61 7373  r, RuleListClass
+000012e0: 6966 6965 722c 202e 2e2e 0a23 2045 424d  ifier, ....# EBM
+000012f0: 2073 7570 706f 7274 7320 7061 6e64 6173   supports pandas
+00001300: 2064 6174 6166 7261 6d65 732c 206e 756d   dataframes, num
+00001310: 7079 2061 7272 6179 732c 2061 6e64 2068  py arrays, and h
+00001320: 616e 646c 6573 2022 7374 7269 6e67 2220  andles "string" 
+00001330: 6461 7461 206e 6174 6976 656c 792e 0a60  data natively..`
+00001340: 6060 0a0a 556e 6465 7273 7461 6e64 2074  ``..Understand t
+00001350: 6865 206d 6f64 656c 0a60 6060 7079 7468  he model.```pyth
+00001360: 6f6e 0a66 726f 6d20 696e 7465 7270 7265  on.from interpre
+00001370: 7420 696d 706f 7274 2073 686f 770a 0a65  t import show..e
+00001380: 626d 5f67 6c6f 6261 6c20 3d20 6562 6d2e  bm_global = ebm.
+00001390: 6578 706c 6169 6e5f 676c 6f62 616c 2829  explain_global()
+000013a0: 0a73 686f 7728 6562 6d5f 676c 6f62 616c  .show(ebm_global
+000013b0: 290a 6060 600a 215b 476c 6f62 616c 2045  ).```.![Global E
+000013c0: 7870 6c61 6e61 7469 6f6e 2049 6d61 6765  xplanation Image
+000013d0: 5d28 2e2f 6578 616d 706c 6573 2f70 7974  ](./examples/pyt
+000013e0: 686f 6e2f 6173 7365 7473 2f72 6561 646d  hon/assets/readm
+000013f0: 655f 6562 6d5f 676c 6f62 616c 5f73 7065  e_ebm_global_spe
+00001400: 6369 6669 632e 504e 473f 7261 773d 7472  cific.PNG?raw=tr
+00001410: 7565 290a 0a3c 6272 2f3e 0a0a 556e 6465  ue)..<br/>..Unde
+00001420: 7273 7461 6e64 2069 6e64 6976 6964 7561  rstand individua
+00001430: 6c20 7072 6564 6963 7469 6f6e 730a 6060  l predictions.``
+00001440: 6070 7974 686f 6e0a 6562 6d5f 6c6f 6361  `python.ebm_loca
+00001450: 6c20 3d20 6562 6d2e 6578 706c 6169 6e5f  l = ebm.explain_
+00001460: 6c6f 6361 6c28 585f 7465 7374 2c20 795f  local(X_test, y_
+00001470: 7465 7374 290a 7368 6f77 2865 626d 5f6c  test).show(ebm_l
+00001480: 6f63 616c 290a 6060 600a 215b 4c6f 6361  ocal).```.![Loca
+00001490: 6c20 4578 706c 616e 6174 696f 6e20 496d  l Explanation Im
+000014a0: 6167 655d 282e 2f65 7861 6d70 6c65 732f  age](./examples/
+000014b0: 7079 7468 6f6e 2f61 7373 6574 732f 7265  python/assets/re
+000014c0: 6164 6d65 5f65 626d 5f6c 6f63 616c 5f73  adme_ebm_local_s
+000014d0: 7065 6369 6669 632e 504e 473f 7261 773d  pecific.PNG?raw=
+000014e0: 7472 7565 290a 0a3c 6272 2f3e 0a0a 416e  true)..<br/>..An
+000014f0: 6420 6966 2079 6f75 2068 6176 6520 6d75  d if you have mu
+00001500: 6c74 6970 6c65 206d 6f64 656c 2065 7870  ltiple model exp
+00001510: 6c61 6e61 7469 6f6e 732c 2063 6f6d 7061  lanations, compa
+00001520: 7265 2074 6865 6d0a 6060 6070 7974 686f  re them.```pytho
+00001530: 6e0a 7368 6f77 285b 6c6f 6769 7374 6963  n.show([logistic
+00001540: 5f72 6567 7265 7373 696f 6e5f 676c 6f62  _regression_glob
+00001550: 616c 2c20 6465 6369 7369 6f6e 5f74 7265  al, decision_tre
+00001560: 655f 676c 6f62 616c 5d29 0a60 6060 0a21  e_global]).```.!
+00001570: 5b44 6173 6862 6f61 7264 2049 6d61 6765  [Dashboard Image
+00001580: 5d28 2e2f 6578 616d 706c 6573 2f70 7974  ](./examples/pyt
+00001590: 686f 6e2f 6173 7365 7473 2f72 6561 646d  hon/assets/readm
+000015a0: 655f 6461 7368 626f 6172 642e 504e 473f  e_dashboard.PNG?
+000015b0: 7261 773d 7472 7565 290a 0a3c 6272 2f3e  raw=true)..<br/>
+000015c0: 0a0a 4966 2079 6f75 206e 6565 6420 746f  ..If you need to
+000015d0: 206b 6565 7020 796f 7572 2064 6174 6120   keep your data 
+000015e0: 7072 6976 6174 652c 2075 7365 2044 6966  private, use Dif
+000015f0: 6665 7265 6e74 6961 6c6c 7920 5072 6976  ferentially Priv
+00001600: 6174 6520 4542 4d73 2028 7365 6520 5b44  ate EBMs (see [D
+00001610: 502d 4542 4d73 5d28 6874 7470 733a 2f2f  P-EBMs](https://
+00001620: 7072 6f63 6565 6469 6e67 732e 6d6c 722e  proceedings.mlr.
+00001630: 7072 6573 732f 7631 3339 2f6e 6f72 6932  press/v139/nori2
+00001640: 3161 2f6e 6f72 6932 3161 2e70 6466 2929  1a/nori21a.pdf))
+00001650: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00001660: 2069 6e74 6572 7072 6574 2e70 7269 7661   interpret.priva
+00001670: 6379 2069 6d70 6f72 7420 4450 4578 706c  cy import DPExpl
+00001680: 6169 6e61 626c 6542 6f6f 7374 696e 6743  ainableBoostingC
+00001690: 6c61 7373 6966 6965 722c 2044 5045 7870  lassifier, DPExp
+000016a0: 6c61 696e 6162 6c65 426f 6f73 7469 6e67  lainableBoosting
+000016b0: 5265 6772 6573 736f 720a 0a64 705f 6562  Regressor..dp_eb
+000016c0: 6d20 3d20 4450 4578 706c 6169 6e61 626c  m = DPExplainabl
+000016d0: 6542 6f6f 7374 696e 6743 6c61 7373 6966  eBoostingClassif
+000016e0: 6965 7228 6570 7369 6c6f 6e3d 312c 2064  ier(epsilon=1, d
+000016f0: 656c 7461 3d31 652d 3529 2023 2053 7065  elta=1e-5) # Spe
+00001700: 6369 6679 2070 7269 7661 6379 2070 6172  cify privacy par
+00001710: 616d 6574 6572 730a 6470 5f65 626d 2e66  ameters.dp_ebm.f
+00001720: 6974 2858 5f74 7261 696e 2c20 795f 7472  it(X_train, y_tr
+00001730: 6169 6e29 0a0a 7368 6f77 2864 705f 6562  ain)..show(dp_eb
+00001740: 6d2e 6578 706c 6169 6e5f 676c 6f62 616c  m.explain_global
+00001750: 2829 2920 2320 4964 656e 7469 6361 6c20  ()) # Identical 
+00001760: 6675 6e63 7469 6f6e 2063 616c 6c73 2074  function calls t
+00001770: 6f20 7374 616e 6461 7264 2045 424d 730a  o standard EBMs.
+00001780: 6060 600a 0a3c 6272 2f3e 0a3c 6272 2f3e  ```..<br/>.<br/>
+00001790: 0a0a 466f 7220 6d6f 7265 2069 6e66 6f72  ..For more infor
+000017a0: 6d61 7469 6f6e 2c20 7365 6520 7468 6520  mation, see the 
+000017b0: 5b64 6f63 756d 656e 7461 7469 6f6e 5d28  [documentation](
+000017c0: 6874 7470 733a 2f2f 696e 7465 7270 7265  https://interpre
+000017d0: 742e 6d6c 2f64 6f63 732f 6765 7474 696e  t.ml/docs/gettin
+000017e0: 672d 7374 6172 7465 642e 6874 6d6c 292e  g-started.html).
+000017f0: 0a3c 6272 2f3e 0a3c 6272 2f3e 0a0a 2320  .<br/>.<br/>..# 
+00001800: 4163 6b6e 6f77 6c65 6467 656d 656e 7473  Acknowledgements
+00001810: 0a0a 496e 7465 7270 7265 744d 4c20 7761  ..InterpretML wa
+00001820: 7320 6f72 6967 696e 616c 6c79 2063 7265  s originally cre
+00001830: 6174 6564 2062 7920 2865 7175 616c 2063  ated by (equal c
+00001840: 6f6e 7472 6962 7574 696f 6e73 293a 2053  ontributions): S
+00001850: 616d 7565 6c20 4a65 6e6b 696e 732c 2048  amuel Jenkins, H
+00001860: 6172 7368 6120 4e6f 7269 2c20 5061 756c  arsha Nori, Paul
+00001870: 204b 6f63 682c 2061 6e64 2052 6963 6820   Koch, and Rich 
+00001880: 4361 7275 616e 610a 0a45 424d 7320 6172  Caruana..EBMs ar
+00001890: 6520 6661 7374 2064 6572 6976 6174 6976  e fast derivativ
+000018a0: 6520 6f66 2047 4132 4d2c 2069 6e76 656e  e of GA2M, inven
+000018b0: 7465 6420 6279 3a20 5969 6e20 4c6f 752c  ted by: Yin Lou,
+000018c0: 2052 6963 6820 4361 7275 616e 612c 204a   Rich Caruana, J
+000018d0: 6f68 616e 6e65 7320 4765 6872 6b65 2c20  ohannes Gehrke, 
+000018e0: 616e 6420 4769 6c65 7320 486f 6f6b 6572  and Giles Hooker
+000018f0: 0a0a 4d61 6e79 2070 656f 706c 6520 6861  ..Many people ha
+00001900: 7665 2073 7570 706f 7274 6564 2075 7320  ve supported us 
+00001910: 616c 6f6e 6720 7468 6520 7761 792e 2043  along the way. C
+00001920: 6865 636b 206f 7574 205b 4143 4b4e 4f57  heck out [ACKNOW
+00001930: 4c45 4447 454d 454e 5453 2e6d 645d 282e  LEDGEMENTS.md](.
+00001940: 2f41 434b 4e4f 574c 4544 4745 4d45 4e54  /ACKNOWLEDGEMENT
+00001950: 532e 6d64 2921 0a0a 5765 2061 6c73 6f20  S.md)!..We also 
+00001960: 6275 696c 6420 6f6e 2074 6f70 206f 6620  build on top of 
+00001970: 6d61 6e79 2067 7265 6174 2070 6163 6b61  many great packa
+00001980: 6765 732e 2050 6c65 6173 6520 6368 6563  ges. Please chec
+00001990: 6b20 7468 656d 206f 7574 210a 0a5b 706c  k them out!..[pl
+000019a0: 6f74 6c79 5d28 6874 7470 733a 2f2f 6769  otly](https://gi
+000019b0: 7468 7562 2e63 6f6d 2f70 6c6f 746c 792f  thub.com/plotly/
+000019c0: 706c 6f74 6c79 2e70 7929 207c 0a5b 6461  plotly.py) |.[da
+000019d0: 7368 5d28 6874 7470 733a 2f2f 6769 7468  sh](https://gith
+000019e0: 7562 2e63 6f6d 2f70 6c6f 746c 792f 6461  ub.com/plotly/da
+000019f0: 7368 2920 7c0a 5b73 6369 6b69 742d 6c65  sh) |.[scikit-le
+00001a00: 6172 6e5d 2868 7474 7073 3a2f 2f67 6974  arn](https://git
+00001a10: 6875 622e 636f 6d2f 7363 696b 6974 2d6c  hub.com/scikit-l
+00001a20: 6561 726e 2f73 6369 6b69 742d 6c65 6172  earn/scikit-lear
+00001a30: 6e29 207c 0a5b 6c69 6d65 5d28 6874 7470  n) |.[lime](http
+00001a40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00001a50: 6172 636f 7463 722f 6c69 6d65 2920 7c0a  arcotcr/lime) |.
+00001a60: 5b73 6861 705d 2868 7474 7073 3a2f 2f67  [shap](https://g
+00001a70: 6974 6875 622e 636f 6d2f 736c 756e 6462  ithub.com/slundb
+00001a80: 6572 672f 7368 6170 2920 7c0a 5b73 616c  erg/shap) |.[sal
+00001a90: 6962 5d28 6874 7470 733a 2f2f 6769 7468  ib](https://gith
+00001aa0: 7562 2e63 6f6d 2f53 414c 6962 2f53 414c  ub.com/SALib/SAL
+00001ab0: 6962 2920 7c0a 5b73 6b6f 7065 2d72 756c  ib) |.[skope-rul
+00001ac0: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00001ad0: 7562 2e63 6f6d 2f73 6369 6b69 742d 6c65  ub.com/scikit-le
+00001ae0: 6172 6e2d 636f 6e74 7269 622f 736b 6f70  arn-contrib/skop
+00001af0: 652d 7275 6c65 7329 207c 0a5b 7472 6565  e-rules) |.[tree
+00001b00: 696e 7465 7270 7265 7465 725d 2868 7474  interpreter](htt
+00001b10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001b20: 616e 646f 7361 2f74 7265 6569 6e74 6572  andosa/treeinter
+00001b30: 7072 6574 6572 2920 7c0a 5b67 6576 656e  preter) |.[geven
+00001b40: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00001b50: 622e 636f 6d2f 6765 7665 6e74 2f67 6576  b.com/gevent/gev
+00001b60: 656e 7429 207c 0a5b 6a6f 626c 6962 5d28  ent) |.[joblib](
+00001b70: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001b80: 6f6d 2f6a 6f62 6c69 622f 6a6f 626c 6962  om/joblib/joblib
+00001b90: 2920 7c0a 5b70 7974 6573 745d 2868 7474  ) |.[pytest](htt
+00001ba0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001bb0: 7079 7465 7374 2d64 6576 2f70 7974 6573  pytest-dev/pytes
+00001bc0: 7429 207c 0a5b 6a75 7079 7465 725d 2868  t) |.[jupyter](h
+00001bd0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001be0: 6d2f 6a75 7079 7465 722f 6e6f 7465 626f  m/jupyter/notebo
+00001bf0: 6f6b 290a 0a23 203c 6120 6e61 6d65 3d22  ok)..# <a name="
+00001c00: 6369 7461 7469 6f6e 7322 3e43 6974 6174  citations">Citat
+00001c10: 696f 6e73 3c2f 613e 0a0a 3c64 6574 6169  ions</a>..<detai
+00001c20: 6c73 206f 7065 6e3e 0a20 203c 7375 6d6d  ls open>.  <summ
+00001c30: 6172 793e 3c73 7472 6f6e 673e 496e 7465  ary><strong>Inte
+00001c40: 7270 7265 744d 4c3c 2f73 7472 6f6e 673e  rpretML</strong>
+00001c50: 3c2f 7375 6d6d 6172 793e 0a20 203c 6872  </summary>.  <hr
+00001c60: 2f3e 0a0a 2020 3c64 6574 6169 6c73 206f  />..  <details o
+00001c70: 7065 6e3e 0a20 2020 203c 7375 6d6d 6172  pen>.    <summar
+00001c80: 793e 0a20 2020 2020 203c 656d 3e22 496e  y>.      <em>"In
+00001c90: 7465 7270 7265 744d 4c3a 2041 2055 6e69  terpretML: A Uni
+00001ca0: 6669 6564 2046 7261 6d65 776f 726b 2066  fied Framework f
+00001cb0: 6f72 204d 6163 6869 6e65 204c 6561 726e  or Machine Learn
+00001cc0: 696e 6720 496e 7465 7270 7265 7461 6269  ing Interpretabi
+00001cd0: 6c69 7479 2220 2848 2e20 4e6f 7269 2c20  lity" (H. Nori, 
+00001ce0: 532e 204a 656e 6b69 6e73 2c20 502e 204b  S. Jenkins, P. K
+00001cf0: 6f63 682c 2061 6e64 2052 2e20 4361 7275  och, and R. Caru
+00001d00: 616e 6120 3230 3139 293c 2f65 6d3e 0a20  ana 2019)</em>. 
+00001d10: 2020 203c 2f73 756d 6d61 7279 3e0a 2020     </summary>.  
+00001d20: 2020 3c62 722f 3e0a 2020 2020 3c70 7265    <br/>.    <pre
+00001d30: 3e0a 4061 7274 6963 6c65 7b6e 6f72 6932  >.@article{nori2
+00001d40: 3031 3969 6e74 6572 7072 6574 6d6c 2c0a  019interpretml,.
+00001d50: 2020 7469 746c 653d 7b49 6e74 6572 7072    title={Interpr
+00001d60: 6574 4d4c 3a20 4120 556e 6966 6965 6420  etML: A Unified 
+00001d70: 4672 616d 6577 6f72 6b20 666f 7220 4d61  Framework for Ma
+00001d80: 6368 696e 6520 4c65 6172 6e69 6e67 2049  chine Learning I
+00001d90: 6e74 6572 7072 6574 6162 696c 6974 797d  nterpretability}
+00001da0: 2c0a 2020 6175 7468 6f72 3d7b 4e6f 7269  ,.  author={Nori
+00001db0: 2c20 4861 7273 6861 2061 6e64 204a 656e  , Harsha and Jen
+00001dc0: 6b69 6e73 2c20 5361 6d75 656c 2061 6e64  kins, Samuel and
+00001dd0: 204b 6f63 682c 2050 6175 6c20 616e 6420   Koch, Paul and 
+00001de0: 4361 7275 616e 612c 2052 6963 687d 2c0a  Caruana, Rich},.
+00001df0: 2020 6a6f 7572 6e61 6c3d 7b61 7258 6976    journal={arXiv
+00001e00: 2070 7265 7072 696e 7420 6172 5869 763a   preprint arXiv:
+00001e10: 3139 3039 2e30 3932 3233 7d2c 0a20 2079  1909.09223},.  y
+00001e20: 6561 723d 7b32 3031 397d 0a7d 0a20 2020  ear={2019}.}.   
+00001e30: 203c 2f70 7265 3e0a 2020 2020 3c61 2068   </pre>.    <a h
+00001e40: 7265 663d 2268 7474 7073 3a2f 2f61 7278  ref="https://arx
+00001e50: 6976 2e6f 7267 2f70 6466 2f31 3930 392e  iv.org/pdf/1909.
+00001e60: 3039 3232 332e 7064 6622 3e50 6170 6572  09223.pdf">Paper
+00001e70: 206c 696e 6b3c 2f61 3e0a 2020 3c2f 6465   link</a>.  </de
+00001e80: 7461 696c 733e 0a0a 2020 3c68 722f 3e0a  tails>..  <hr/>.
+00001e90: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
+00001ea0: 6169 6c73 3e0a 2020 3c73 756d 6d61 7279  ails>.  <summary
+00001eb0: 3e3c 7374 726f 6e67 3e45 7870 6c61 696e  ><strong>Explain
+00001ec0: 6162 6c65 2042 6f6f 7374 696e 673c 2f73  able Boosting</s
+00001ed0: 7472 6f6e 673e 3c2f 7375 6d6d 6172 793e  trong></summary>
+00001ee0: 0a20 203c 6872 2f3e 0a0a 2020 3c64 6574  .  <hr/>..  <det
+00001ef0: 6169 6c73 3e0a 2020 2020 3c73 756d 6d61  ails>.    <summa
+00001f00: 7279 3e0a 2020 2020 2020 3c65 6d3e 2249  ry>.      <em>"I
+00001f10: 6e74 656c 6c69 6769 626c 6520 6d6f 6465  ntelligible mode
+00001f20: 6c73 2066 6f72 2068 6561 6c74 6863 6172  ls for healthcar
+00001f30: 653a 2050 7265 6469 6374 696e 6720 706e  e: Predicting pn
+00001f40: 6575 6d6f 6e69 6120 7269 736b 2061 6e64  eumonia risk and
+00001f50: 2068 6f73 7069 7461 6c20 3330 2d64 6179   hospital 30-day
+00001f60: 2072 6561 646d 6973 7369 6f6e 2220 2852   readmission" (R
+00001f70: 2e20 4361 7275 616e 612c 2059 2e20 4c6f  . Caruana, Y. Lo
+00001f80: 752c 204a 2e20 4765 6872 6b65 2c20 502e  u, J. Gehrke, P.
+00001f90: 204b 6f63 682c 204d 2e20 5374 7572 6d2c   Koch, M. Sturm,
+00001fa0: 2061 6e64 204e 2e20 456c 6861 6461 6420   and N. Elhadad 
+00001fb0: 3230 3135 293c 2f65 6d3e 0a20 2020 203c  2015)</em>.    <
+00001fc0: 2f73 756d 6d61 7279 3e0a 2020 2020 3c62  /summary>.    <b
+00001fd0: 722f 3e0a 2020 2020 3c70 7265 3e0a 4069  r/>.    <pre>.@i
+00001fe0: 6e70 726f 6365 6564 696e 6773 7b63 6172  nproceedings{car
+00001ff0: 7561 6e61 3230 3135 696e 7465 6c6c 6967  uana2015intellig
+00002000: 6962 6c65 2c0a 2020 7469 746c 653d 7b49  ible,.  title={I
+00002010: 6e74 656c 6c69 6769 626c 6520 6d6f 6465  ntelligible mode
+00002020: 6c73 2066 6f72 2068 6561 6c74 6863 6172  ls for healthcar
+00002030: 653a 2050 7265 6469 6374 696e 6720 706e  e: Predicting pn
+00002040: 6575 6d6f 6e69 6120 7269 736b 2061 6e64  eumonia risk and
+00002050: 2068 6f73 7069 7461 6c20 3330 2d64 6179   hospital 30-day
+00002060: 2072 6561 646d 6973 7369 6f6e 7d2c 0a20   readmission},. 
+00002070: 2061 7574 686f 723d 7b43 6172 7561 6e61   author={Caruana
+00002080: 2c20 5269 6368 2061 6e64 204c 6f75 2c20  , Rich and Lou, 
+00002090: 5969 6e20 616e 6420 4765 6872 6b65 2c20  Yin and Gehrke, 
+000020a0: 4a6f 6861 6e6e 6573 2061 6e64 204b 6f63  Johannes and Koc
+000020b0: 682c 2050 6175 6c20 616e 6420 5374 7572  h, Paul and Stur
+000020c0: 6d2c 204d 6172 6320 616e 6420 456c 6861  m, Marc and Elha
+000020d0: 6461 642c 204e 6f65 6d69 657d 2c0a 2020  dad, Noemie},.  
+000020e0: 626f 6f6b 7469 746c 653d 7b50 726f 6365  booktitle={Proce
+000020f0: 6564 696e 6773 206f 6620 7468 6520 3231  edings of the 21
+00002100: 7468 2041 434d 2053 4947 4b44 4420 496e  th ACM SIGKDD In
+00002110: 7465 726e 6174 696f 6e61 6c20 436f 6e66  ternational Conf
+00002120: 6572 656e 6365 206f 6e20 4b6e 6f77 6c65  erence on Knowle
+00002130: 6467 6520 4469 7363 6f76 6572 7920 616e  dge Discovery an
+00002140: 6420 4461 7461 204d 696e 696e 677d 2c0a  d Data Mining},.
+00002150: 2020 7061 6765 733d 7b31 3732 312d 2d31    pages={1721--1
+00002160: 3733 307d 2c0a 2020 7965 6172 3d7b 3230  730},.  year={20
+00002170: 3135 7d2c 0a20 206f 7267 616e 697a 6174  15},.  organizat
+00002180: 696f 6e3d 7b41 434d 7d0a 7d0a 2020 2020  ion={ACM}.}.    
+00002190: 3c2f 7072 653e 0a20 2020 203c 6120 6872  </pre>.    <a hr
+000021a0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
+000021b0: 6d69 6372 6f73 6f66 742e 636f 6d2f 656e  microsoft.com/en
+000021c0: 2d75 732f 7265 7365 6172 6368 2f77 702d  -us/research/wp-
+000021d0: 636f 6e74 656e 742f 7570 6c6f 6164 732f  content/uploads/
+000021e0: 3230 3137 2f30 362f 4b44 4432 3031 3546  2017/06/KDD2015F
+000021f0: 696e 616c 4472 6166 7449 6e74 656c 6c69  inalDraftIntelli
+00002200: 6769 626c 654d 6f64 656c 7334 4865 616c  gibleModels4Heal
+00002210: 7468 4361 7265 5f69 6774 3134 3365 2d63  thCare_igt143e-c
+00002220: 6172 7561 6e61 412e 7064 6622 3e50 6170  aruanaA.pdf">Pap
+00002230: 6572 206c 696e 6b3c 2f61 3e0a 2020 3c2f  er link</a>.  </
+00002240: 6465 7461 696c 733e 0a0a 2020 3c64 6574  details>..  <det
+00002250: 6169 6c73 3e0a 2020 2020 3c73 756d 6d61  ails>.    <summa
+00002260: 7279 3e0a 2020 2020 2020 3c65 6d3e 2241  ry>.      <em>"A
+00002270: 6363 7572 6174 6520 696e 7465 6c6c 6967  ccurate intellig
+00002280: 6962 6c65 206d 6f64 656c 7320 7769 7468  ible models with
+00002290: 2070 6169 7277 6973 6520 696e 7465 7261   pairwise intera
+000022a0: 6374 696f 6e73 2220 2859 2e20 4c6f 752c  ctions" (Y. Lou,
+000022b0: 2052 2e20 4361 7275 616e 612c 204a 2e20   R. Caruana, J. 
+000022c0: 4765 6872 6b65 2c20 616e 6420 472e 2048  Gehrke, and G. H
+000022d0: 6f6f 6b65 7220 3230 3133 293c 2f65 6d3e  ooker 2013)</em>
+000022e0: 0a20 2020 203c 2f73 756d 6d61 7279 3e0a  .    </summary>.
+000022f0: 2020 2020 3c62 722f 3e0a 2020 2020 3c70      <br/>.    <p
+00002300: 7265 3e0a 4069 6e70 726f 6365 6564 696e  re>.@inproceedin
+00002310: 6773 7b6c 6f75 3230 3133 6163 6375 7261  gs{lou2013accura
+00002320: 7465 2c0a 2020 7469 746c 653d 7b41 6363  te,.  title={Acc
+00002330: 7572 6174 6520 696e 7465 6c6c 6967 6962  urate intelligib
+00002340: 6c65 206d 6f64 656c 7320 7769 7468 2070  le models with p
+00002350: 6169 7277 6973 6520 696e 7465 7261 6374  airwise interact
+00002360: 696f 6e73 7d2c 0a20 2061 7574 686f 723d  ions},.  author=
+00002370: 7b4c 6f75 2c20 5969 6e20 616e 6420 4361  {Lou, Yin and Ca
+00002380: 7275 616e 612c 2052 6963 6820 616e 6420  ruana, Rich and 
+00002390: 4765 6872 6b65 2c20 4a6f 6861 6e6e 6573  Gehrke, Johannes
+000023a0: 2061 6e64 2048 6f6f 6b65 722c 2047 696c   and Hooker, Gil
+000023b0: 6573 7d2c 0a20 2062 6f6f 6b74 6974 6c65  es},.  booktitle
+000023c0: 3d7b 5072 6f63 6565 6469 6e67 7320 6f66  ={Proceedings of
+000023d0: 2074 6865 2031 3974 6820 4143 4d20 5349   the 19th ACM SI
+000023e0: 474b 4444 2069 6e74 6572 6e61 7469 6f6e  GKDD internation
+000023f0: 616c 2063 6f6e 6665 7265 6e63 6520 6f6e  al conference on
+00002400: 204b 6e6f 776c 6564 6765 2064 6973 636f   Knowledge disco
+00002410: 7665 7279 2061 6e64 2064 6174 6120 6d69  very and data mi
+00002420: 6e69 6e67 7d2c 0a20 2070 6167 6573 3d7b  ning},.  pages={
+00002430: 3632 332d 2d36 3331 7d2c 0a20 2079 6561  623--631},.  yea
+00002440: 723d 7b32 3031 337d 2c0a 2020 6f72 6761  r={2013},.  orga
+00002450: 6e69 7a61 7469 6f6e 3d7b 4143 4d7d 0a7d  nization={ACM}.}
+00002460: 0a20 2020 203c 2f70 7265 3e0a 2020 2020  .    </pre>.    
+00002470: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00002480: 2f77 7777 2e63 732e 636f 726e 656c 6c2e  /www.cs.cornell.
+00002490: 6564 752f 7e79 696e 6c6f 752f 7061 7065  edu/~yinlou/pape
+000024a0: 7273 2f6c 6f75 2d6b 6464 3133 2e70 6466  rs/lou-kdd13.pdf
+000024b0: 223e 5061 7065 7220 6c69 6e6b 3c2f 613e  ">Paper link</a>
+000024c0: 0a20 203c 2f64 6574 6169 6c73 3e0a 0a20  .  </details>.. 
+000024d0: 203c 6465 7461 696c 733e 0a20 2020 203c   <details>.    <
+000024e0: 7375 6d6d 6172 793e 0a20 2020 2020 203c  summary>.      <
+000024f0: 656d 3e22 496e 7465 6c6c 6967 6962 6c65  em>"Intelligible
+00002500: 206d 6f64 656c 7320 666f 7220 636c 6173   models for clas
+00002510: 7369 6669 6361 7469 6f6e 2061 6e64 2072  sification and r
+00002520: 6567 7265 7373 696f 6e22 2028 592e 204c  egression" (Y. L
+00002530: 6f75 2c20 522e 2043 6172 7561 6e61 2c20  ou, R. Caruana, 
+00002540: 616e 6420 4a2e 2047 6568 726b 6520 3230  and J. Gehrke 20
+00002550: 3132 293c 2f65 6d3e 0a20 2020 203c 2f73  12)</em>.    </s
+00002560: 756d 6d61 7279 3e0a 2020 2020 3c62 722f  ummary>.    <br/
+00002570: 3e0a 2020 2020 3c70 7265 3e0a 4069 6e70  >.    <pre>.@inp
+00002580: 726f 6365 6564 696e 6773 7b6c 6f75 3230  roceedings{lou20
+00002590: 3132 696e 7465 6c6c 6967 6962 6c65 2c0a  12intelligible,.
+000025a0: 2020 7469 746c 653d 7b49 6e74 656c 6c69    title={Intelli
+000025b0: 6769 626c 6520 6d6f 6465 6c73 2066 6f72  gible models for
+000025c0: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
+000025d0: 616e 6420 7265 6772 6573 7369 6f6e 7d2c  and regression},
+000025e0: 0a20 2061 7574 686f 723d 7b4c 6f75 2c20  .  author={Lou, 
+000025f0: 5969 6e20 616e 6420 4361 7275 616e 612c  Yin and Caruana,
+00002600: 2052 6963 6820 616e 6420 4765 6872 6b65   Rich and Gehrke
+00002610: 2c20 4a6f 6861 6e6e 6573 7d2c 0a20 2062  , Johannes},.  b
+00002620: 6f6f 6b74 6974 6c65 3d7b 5072 6f63 6565  ooktitle={Procee
+00002630: 6469 6e67 7320 6f66 2074 6865 2031 3874  dings of the 18t
+00002640: 6820 4143 4d20 5349 474b 4444 2069 6e74  h ACM SIGKDD int
+00002650: 6572 6e61 7469 6f6e 616c 2063 6f6e 6665  ernational confe
+00002660: 7265 6e63 6520 6f6e 204b 6e6f 776c 6564  rence on Knowled
+00002670: 6765 2064 6973 636f 7665 7279 2061 6e64  ge discovery and
+00002680: 2064 6174 6120 6d69 6e69 6e67 7d2c 0a20   data mining},. 
+00002690: 2070 6167 6573 3d7b 3135 302d 2d31 3538   pages={150--158
+000026a0: 7d2c 0a20 2079 6561 723d 7b32 3031 327d  },.  year={2012}
+000026b0: 2c0a 2020 6f72 6761 6e69 7a61 7469 6f6e  ,.  organization
+000026c0: 3d7b 4143 4d7d 0a7d 0a20 2020 203c 2f70  ={ACM}.}.    </p
+000026d0: 7265 3e0a 2020 2020 3c61 2068 7265 663d  re>.    <a href=
+000026e0: 2268 7474 7073 3a2f 2f77 7777 2e63 732e  "https://www.cs.
+000026f0: 636f 726e 656c 6c2e 6564 752f 7e79 696e  cornell.edu/~yin
+00002700: 6c6f 752f 7061 7065 7273 2f6c 6f75 2d6b  lou/papers/lou-k
+00002710: 6464 3132 2e70 6466 223e 5061 7065 7220  dd12.pdf">Paper 
+00002720: 6c69 6e6b 3c2f 613e 0a20 203c 2f64 6574  link</a>.  </det
+00002730: 6169 6c73 3e0a 0a20 203c 6465 7461 696c  ails>..  <detail
+00002740: 733e 0a20 2020 203c 7375 6d6d 6172 793e  s>.    <summary>
+00002750: 0a20 2020 2020 203c 656d 3e22 496e 7465  .      <em>"Inte
+00002760: 7270 7265 7461 6269 6c69 7479 2c20 5468  rpretability, Th
+00002770: 656e 2057 6861 743f 2045 6469 7469 6e67  en What? Editing
+00002780: 204d 6163 6869 6e65 204c 6561 726e 696e   Machine Learnin
+00002790: 6720 4d6f 6465 6c73 2074 6f20 5265 666c  g Models to Refl
+000027a0: 6563 7420 4875 6d61 6e20 4b6e 6f77 6c65  ect Human Knowle
+000027b0: 6467 6520 616e 6420 5661 6c75 6573 2220  dge and Values" 
+000027c0: 285a 696a 6965 204a 2e20 5761 6e67 2c20  (Zijie J. Wang, 
+000027d0: 416c 6578 204b 616c 652c 2048 6172 7368  Alex Kale, Harsh
+000027e0: 6120 4e6f 7269 2c20 5065 7465 7220 5374  a Nori, Peter St
+000027f0: 656c 6c61 2c20 4d61 726b 2045 2e20 4e75  ella, Mark E. Nu
+00002800: 6e6e 616c 6c79 2c20 4475 656e 2048 6f72  nnally, Duen Hor
+00002810: 6e67 2043 6861 752c 204d 6968 6165 6c61  ng Chau, Mihaela
+00002820: 2056 6f72 766f 7265 616e 752c 204a 656e   Vorvoreanu, Jen
+00002830: 6e69 6665 7220 576f 7274 6d61 6e20 5661  nifer Wortman Va
+00002840: 7567 6861 6e2c 2052 6963 6820 4361 7275  ughan, Rich Caru
+00002850: 616e 6120 3230 3232 293c 2f65 6d3e 0a20  ana 2022)</em>. 
+00002860: 2020 203c 2f73 756d 6d61 7279 3e0a 2020     </summary>.  
+00002870: 2020 3c62 722f 3e0a 2020 2020 3c70 7265    <br/>.    <pre
+00002880: 3e0a 4061 7274 6963 6c65 7b77 616e 6732  >.@article{wang2
+00002890: 3032 3269 6e74 6572 7072 6574 6162 696c  022interpretabil
+000028a0: 6974 792c 0a20 2074 6974 6c65 3d7b 496e  ity,.  title={In
+000028b0: 7465 7270 7265 7461 6269 6c69 7479 2c20  terpretability, 
+000028c0: 5468 656e 2057 6861 743f 2045 6469 7469  Then What? Editi
+000028d0: 6e67 204d 6163 6869 6e65 204c 6561 726e  ng Machine Learn
+000028e0: 696e 6720 4d6f 6465 6c73 2074 6f20 5265  ing Models to Re
+000028f0: 666c 6563 7420 4875 6d61 6e20 4b6e 6f77  flect Human Know
+00002900: 6c65 6467 6520 616e 6420 5661 6c75 6573  ledge and Values
+00002910: 7d2c 0a20 2061 7574 686f 723d 7b57 616e  },.  author={Wan
+00002920: 672c 205a 696a 6965 204a 2061 6e64 204b  g, Zijie J and K
+00002930: 616c 652c 2041 6c65 7820 616e 6420 4e6f  ale, Alex and No
+00002940: 7269 2c20 4861 7273 6861 2061 6e64 2053  ri, Harsha and S
+00002950: 7465 6c6c 612c 2050 6574 6572 2061 6e64  tella, Peter and
+00002960: 204e 756e 6e61 6c6c 792c 204d 6172 6b20   Nunnally, Mark 
+00002970: 4520 616e 6420 4368 6175 2c20 4475 656e  E and Chau, Duen
+00002980: 2048 6f72 6e67 2061 6e64 2056 6f72 766f   Horng and Vorvo
+00002990: 7265 616e 752c 204d 6968 6165 6c61 2061  reanu, Mihaela a
+000029a0: 6e64 2056 6175 6768 616e 2c20 4a65 6e6e  nd Vaughan, Jenn
+000029b0: 6966 6572 2057 6f72 746d 616e 2061 6e64  ifer Wortman and
+000029c0: 2043 6172 7561 6e61 2c20 5269 6368 7d2c   Caruana, Rich},
+000029d0: 0a20 206a 6f75 726e 616c 3d7b 6172 5869  .  journal={arXi
+000029e0: 7620 7072 6570 7269 6e74 2061 7258 6976  v preprint arXiv
+000029f0: 3a32 3230 362e 3135 3436 357d 2c0a 2020  :2206.15465},.  
+00002a00: 7965 6172 3d7b 3230 3232 7d0a 7d0a 2020  year={2022}.}.  
+00002a10: 2020 3c2f 7072 653e 0a20 2020 203c 6120    </pre>.    <a 
+00002a20: 6872 6566 3d22 6874 7470 733a 2f2f 6172  href="https://ar
+00002a30: 7869 762e 6f72 672f 7064 662f 3232 3036  xiv.org/pdf/2206
+00002a40: 2e31 3534 3635 2e70 6466 223e 5061 7065  .15465.pdf">Pape
+00002a50: 7220 6c69 6e6b 3c2f 613e 0a20 203c 2f64  r link</a>.  </d
+00002a60: 6574 6169 6c73 3e0a 0a20 203c 6465 7461  etails>..  <deta
+00002a70: 696c 733e 0a20 2020 203c 7375 6d6d 6172  ils>.    <summar
+00002a80: 793e 0a20 2020 2020 203c 656d 3e22 4178  y>.      <em>"Ax
+00002a90: 696f 6d61 7469 6320 496e 7465 7270 7265  iomatic Interpre
+00002aa0: 7461 6269 6c69 7479 2066 6f72 204d 756c  tability for Mul
+00002ab0: 7469 636c 6173 7320 4164 6469 7469 7665  ticlass Additive
+00002ac0: 204d 6f64 656c 7322 2028 582e 205a 6861   Models" (X. Zha
+00002ad0: 6e67 2c20 532e 2054 616e 2c20 502e 204b  ng, S. Tan, P. K
+00002ae0: 6f63 682c 2059 2e20 4c6f 752c 2055 2e20  och, Y. Lou, U. 
+00002af0: 4368 616a 6577 736b 612c 2061 6e64 2052  Chajewska, and R
+00002b00: 2e20 4361 7275 616e 6120 3230 3139 293c  . Caruana 2019)<
+00002b10: 2f65 6d3e 0a20 2020 203c 2f73 756d 6d61  /em>.    </summa
+00002b20: 7279 3e0a 2020 2020 3c62 722f 3e0a 2020  ry>.    <br/>.  
+00002b30: 2020 3c70 7265 3e0a 4069 6e70 726f 6365    <pre>.@inproce
+00002b40: 6564 696e 6773 7b7a 6861 6e67 3230 3139  edings{zhang2019
+00002b50: 6178 696f 6d61 7469 632c 0a20 2074 6974  axiomatic,.  tit
+00002b60: 6c65 3d7b 4178 696f 6d61 7469 6320 496e  le={Axiomatic In
+00002b70: 7465 7270 7265 7461 6269 6c69 7479 2066  terpretability f
+00002b80: 6f72 204d 756c 7469 636c 6173 7320 4164  or Multiclass Ad
+00002b90: 6469 7469 7665 204d 6f64 656c 737d 2c0a  ditive Models},.
+00002ba0: 2020 6175 7468 6f72 3d7b 5a68 616e 672c    author={Zhang,
+00002bb0: 2058 7565 7a68 6f75 2061 6e64 2054 616e   Xuezhou and Tan
+00002bc0: 2c20 5361 7261 6820 616e 6420 4b6f 6368  , Sarah and Koch
+00002bd0: 2c20 5061 756c 2061 6e64 204c 6f75 2c20  , Paul and Lou, 
+00002be0: 5969 6e20 616e 6420 4368 616a 6577 736b  Yin and Chajewsk
+00002bf0: 612c 2055 7273 7a75 6c61 2061 6e64 2043  a, Urszula and C
+00002c00: 6172 7561 6e61 2c20 5269 6368 7d2c 0a20  aruana, Rich},. 
+00002c10: 2062 6f6f 6b74 6974 6c65 3d7b 5072 6f63   booktitle={Proc
+00002c20: 6565 6469 6e67 7320 6f66 2074 6865 2032  eedings of the 2
+00002c30: 3574 6820 4143 4d20 5349 474b 4444 2049  5th ACM SIGKDD I
+00002c40: 6e74 6572 6e61 7469 6f6e 616c 2043 6f6e  nternational Con
+00002c50: 6665 7265 6e63 6520 6f6e 204b 6e6f 776c  ference on Knowl
+00002c60: 6564 6765 2044 6973 636f 7665 7279 205c  edge Discovery \
+00002c70: 2620 4461 7461 204d 696e 696e 677d 2c0a  & Data Mining},.
+00002c80: 2020 7061 6765 733d 7b32 3236 2d2d 3233    pages={226--23
+00002c90: 347d 2c0a 2020 7965 6172 3d7b 3230 3139  4},.  year={2019
+00002ca0: 7d2c 0a20 206f 7267 616e 697a 6174 696f  },.  organizatio
+00002cb0: 6e3d 7b41 434d 7d0a 7d0a 2020 2020 3c2f  n={ACM}.}.    </
+00002cc0: 7072 653e 0a20 2020 203c 6120 6872 6566  pre>.    <a href
+00002cd0: 3d22 6874 7470 733a 2f2f 6172 7869 762e  ="https://arxiv.
+00002ce0: 6f72 672f 7064 662f 3138 3130 2e30 3930  org/pdf/1810.090
+00002cf0: 3932 2e70 6466 223e 5061 7065 7220 6c69  92.pdf">Paper li
+00002d00: 6e6b 3c2f 613e 0a20 203c 2f64 6574 6169  nk</a>.  </detai
+00002d10: 6c73 3e0a 0a20 203c 6465 7461 696c 733e  ls>..  <details>
+00002d20: 0a20 2020 203c 7375 6d6d 6172 793e 0a20  .    <summary>. 
+00002d30: 2020 2020 203c 656d 3e22 4469 7374 696c       <em>"Distil
+00002d40: 6c2d 616e 642d 636f 6d70 6172 653a 2061  l-and-compare: a
+00002d50: 7564 6974 696e 6720 626c 6163 6b2d 626f  uditing black-bo
+00002d60: 7820 6d6f 6465 6c73 2075 7369 6e67 2074  x models using t
+00002d70: 7261 6e73 7061 7265 6e74 206d 6f64 656c  ransparent model
+00002d80: 2064 6973 7469 6c6c 6174 696f 6e22 2028   distillation" (
+00002d90: 532e 2054 616e 2c20 522e 2043 6172 7561  S. Tan, R. Carua
+00002da0: 6e61 2c20 472e 2048 6f6f 6b65 722c 2061  na, G. Hooker, a
+00002db0: 6e64 2059 2e20 4c6f 7520 3230 3138 293c  nd Y. Lou 2018)<
+00002dc0: 2f65 6d3e 0a20 2020 203c 2f73 756d 6d61  /em>.    </summa
+00002dd0: 7279 3e0a 2020 2020 3c62 722f 3e0a 2020  ry>.    <br/>.  
+00002de0: 2020 3c70 7265 3e0a 4069 6e70 726f 6365    <pre>.@inproce
+00002df0: 6564 696e 6773 7b74 616e 3230 3138 6469  edings{tan2018di
+00002e00: 7374 696c 6c2c 0a20 2074 6974 6c65 3d7b  still,.  title={
+00002e10: 4469 7374 696c 6c2d 616e 642d 636f 6d70  Distill-and-comp
+00002e20: 6172 653a 2061 7564 6974 696e 6720 626c  are: auditing bl
+00002e30: 6163 6b2d 626f 7820 6d6f 6465 6c73 2075  ack-box models u
+00002e40: 7369 6e67 2074 7261 6e73 7061 7265 6e74  sing transparent
+00002e50: 206d 6f64 656c 2064 6973 7469 6c6c 6174   model distillat
+00002e60: 696f 6e7d 2c0a 2020 6175 7468 6f72 3d7b  ion},.  author={
+00002e70: 5461 6e2c 2053 6172 6168 2061 6e64 2043  Tan, Sarah and C
+00002e80: 6172 7561 6e61 2c20 5269 6368 2061 6e64  aruana, Rich and
+00002e90: 2048 6f6f 6b65 722c 2047 696c 6573 2061   Hooker, Giles a
+00002ea0: 6e64 204c 6f75 2c20 5969 6e7d 2c0a 2020  nd Lou, Yin},.  
+00002eb0: 626f 6f6b 7469 746c 653d 7b50 726f 6365  booktitle={Proce
+00002ec0: 6564 696e 6773 206f 6620 7468 6520 3230  edings of the 20
+00002ed0: 3138 2041 4141 492f 4143 4d20 436f 6e66  18 AAAI/ACM Conf
+00002ee0: 6572 656e 6365 206f 6e20 4149 2c20 4574  erence on AI, Et
+00002ef0: 6869 6373 2c20 616e 6420 536f 6369 6574  hics, and Societ
+00002f00: 797d 2c0a 2020 7061 6765 733d 7b33 3033  y},.  pages={303
+00002f10: 2d2d 3331 307d 2c0a 2020 7965 6172 3d7b  --310},.  year={
+00002f20: 3230 3138 7d2c 0a20 206f 7267 616e 697a  2018},.  organiz
+00002f30: 6174 696f 6e3d 7b41 434d 7d0a 7d0a 2020  ation={ACM}.}.  
+00002f40: 2020 3c2f 7072 653e 0a20 2020 203c 6120    </pre>.    <a 
+00002f50: 6872 6566 3d22 6874 7470 733a 2f2f 6172  href="https://ar
+00002f60: 7869 762e 6f72 672f 7064 662f 3137 3130  xiv.org/pdf/1710
+00002f70: 2e30 3631 3639 223e 5061 7065 7220 6c69  .06169">Paper li
+00002f80: 6e6b 3c2f 613e 0a20 203c 2f64 6574 6169  nk</a>.  </detai
+00002f90: 6c73 3e0a 0a20 203c 6465 7461 696c 733e  ls>..  <details>
+00002fa0: 0a20 2020 203c 7375 6d6d 6172 793e 0a20  .    <summary>. 
+00002fb0: 2020 2020 203c 656d 3e22 5075 7269 6679       <em>"Purify
+00002fc0: 696e 6720 496e 7465 7261 6374 696f 6e20  ing Interaction 
+00002fd0: 4566 6665 6374 7320 7769 7468 2074 6865  Effects with the
+00002fe0: 2046 756e 6374 696f 6e61 6c20 414e 4f56   Functional ANOV
+00002ff0: 413a 2041 6e20 4566 6669 6369 656e 7420  A: An Efficient 
+00003000: 416c 676f 7269 7468 6d20 666f 7220 5265  Algorithm for Re
+00003010: 636f 7665 7269 6e67 2049 6465 6e74 6966  covering Identif
+00003020: 6961 626c 6520 4164 6469 7469 7665 204d  iable Additive M
+00003030: 6f64 656c 7322 2028 422e 204c 656e 6765  odels" (B. Lenge
+00003040: 7269 6368 2c20 532e 2054 616e 2c20 432e  rich, S. Tan, C.
+00003050: 2043 6861 6e67 2c20 472e 2048 6f6f 6b65   Chang, G. Hooke
+00003060: 722c 2052 2e20 4361 7275 616e 6120 3230  r, R. Caruana 20
+00003070: 3139 293c 2f65 6d3e 0a20 2020 203c 2f73  19)</em>.    </s
+00003080: 756d 6d61 7279 3e0a 2020 2020 3c62 722f  ummary>.    <br/
+00003090: 3e0a 2020 2020 3c70 7265 3e0a 4061 7274  >.    <pre>.@art
+000030a0: 6963 6c65 7b6c 656e 6765 7269 6368 3230  icle{lengerich20
+000030b0: 3139 7075 7269 6679 696e 672c 0a20 2074  19purifying,.  t
+000030c0: 6974 6c65 3d7b 5075 7269 6679 696e 6720  itle={Purifying 
+000030d0: 496e 7465 7261 6374 696f 6e20 4566 6665  Interaction Effe
+000030e0: 6374 7320 7769 7468 2074 6865 2046 756e  cts with the Fun
+000030f0: 6374 696f 6e61 6c20 414e 4f56 413a 2041  ctional ANOVA: A
+00003100: 6e20 4566 6669 6369 656e 7420 416c 676f  n Efficient Algo
+00003110: 7269 7468 6d20 666f 7220 5265 636f 7665  rithm for Recove
+00003120: 7269 6e67 2049 6465 6e74 6966 6961 626c  ring Identifiabl
+00003130: 6520 4164 6469 7469 7665 204d 6f64 656c  e Additive Model
+00003140: 737d 2c0a 2020 6175 7468 6f72 3d7b 4c65  s},.  author={Le
+00003150: 6e67 6572 6963 682c 2042 656e 6a61 6d69  ngerich, Benjami
+00003160: 6e20 616e 6420 5461 6e2c 2053 6172 6168  n and Tan, Sarah
+00003170: 2061 6e64 2043 6861 6e67 2c20 4368 756e   and Chang, Chun
+00003180: 2d48 616f 2061 6e64 2048 6f6f 6b65 722c  -Hao and Hooker,
+00003190: 2047 696c 6573 2061 6e64 2043 6172 7561   Giles and Carua
+000031a0: 6e61 2c20 5269 6368 7d2c 0a20 206a 6f75  na, Rich},.  jou
+000031b0: 726e 616c 3d7b 6172 5869 7620 7072 6570  rnal={arXiv prep
+000031c0: 7269 6e74 2061 7258 6976 3a31 3931 312e  rint arXiv:1911.
+000031d0: 3034 3937 347d 2c0a 2020 7965 6172 3d7b  04974},.  year={
+000031e0: 3230 3139 7d0a 7d0a 2020 2020 3c2f 7072  2019}.}.    </pr
+000031f0: 653e 0a20 2020 203c 6120 6872 6566 3d22  e>.    <a href="
+00003200: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00003210: 672f 7064 662f 3139 3131 2e30 3439 3734  g/pdf/1911.04974
+00003220: 2e70 6466 223e 5061 7065 7220 6c69 6e6b  .pdf">Paper link
+00003230: 3c2f 613e 0a20 203c 2f64 6574 6169 6c73  </a>.  </details
+00003240: 3e0a 0a20 203c 6465 7461 696c 733e 0a20  >..  <details>. 
+00003250: 2020 203c 7375 6d6d 6172 793e 0a20 2020     <summary>.   
+00003260: 2020 203c 656d 3e22 496e 7465 7270 7265     <em>"Interpre
+00003270: 7469 6e67 2049 6e74 6572 7072 6574 6162  ting Interpretab
+00003280: 696c 6974 793a 2055 6e64 6572 7374 616e  ility: Understan
+00003290: 6469 6e67 2044 6174 6120 5363 6965 6e74  ding Data Scient
+000032a0: 6973 7473 2720 5573 6520 6f66 2049 6e74  ists' Use of Int
+000032b0: 6572 7072 6574 6162 696c 6974 7920 546f  erpretability To
+000032c0: 6f6c 7320 666f 7220 4d61 6368 696e 6520  ols for Machine 
+000032d0: 4c65 6172 6e69 6e67 2220 2848 2e20 4b61  Learning" (H. Ka
+000032e0: 7572 2c20 482e 204e 6f72 692c 2053 2e20  ur, H. Nori, S. 
+000032f0: 4a65 6e6b 696e 732c 2052 2e20 4361 7275  Jenkins, R. Caru
+00003300: 616e 612c 2048 2e20 5761 6c6c 6163 682c  ana, H. Wallach,
+00003310: 204a 2e20 576f 7274 6d61 6e20 5661 7567   J. Wortman Vaug
+00003320: 6861 6e20 3230 3230 293c 2f65 6d3e 0a20  han 2020)</em>. 
+00003330: 2020 203c 2f73 756d 6d61 7279 3e0a 2020     </summary>.  
+00003340: 2020 3c62 722f 3e0a 2020 2020 3c70 7265    <br/>.    <pre
+00003350: 3e0a 4069 6e70 726f 6365 6564 696e 6773  >.@inproceedings
+00003360: 7b6b 6175 7232 3032 3069 6e74 6572 7072  {kaur2020interpr
+00003370: 6574 696e 672c 0a20 2074 6974 6c65 3d7b  eting,.  title={
+00003380: 496e 7465 7270 7265 7469 6e67 2049 6e74  Interpreting Int
+00003390: 6572 7072 6574 6162 696c 6974 793a 2055  erpretability: U
+000033a0: 6e64 6572 7374 616e 6469 6e67 2044 6174  nderstanding Dat
+000033b0: 6120 5363 6965 6e74 6973 7473 2720 5573  a Scientists' Us
+000033c0: 6520 6f66 2049 6e74 6572 7072 6574 6162  e of Interpretab
+000033d0: 696c 6974 7920 546f 6f6c 7320 666f 7220  ility Tools for 
+000033e0: 4d61 6368 696e 6520 4c65 6172 6e69 6e67  Machine Learning
+000033f0: 7d2c 0a20 2061 7574 686f 723d 7b4b 6175  },.  author={Kau
+00003400: 722c 2048 6172 6d61 6e70 7265 6574 2061  r, Harmanpreet a
+00003410: 6e64 204e 6f72 692c 2048 6172 7368 6120  nd Nori, Harsha 
+00003420: 616e 6420 4a65 6e6b 696e 732c 2053 616d  and Jenkins, Sam
+00003430: 7565 6c20 616e 6420 4361 7275 616e 612c  uel and Caruana,
+00003440: 2052 6963 6820 616e 6420 5761 6c6c 6163   Rich and Wallac
+00003450: 682c 2048 616e 6e61 2061 6e64 2057 6f72  h, Hanna and Wor
+00003460: 746d 616e 2056 6175 6768 616e 2c20 4a65  tman Vaughan, Je
+00003470: 6e6e 6966 6572 7d2c 0a20 2062 6f6f 6b74  nnifer},.  bookt
+00003480: 6974 6c65 3d7b 5072 6f63 6565 6469 6e67  itle={Proceeding
+00003490: 7320 6f66 2074 6865 2032 3032 3020 4348  s of the 2020 CH
+000034a0: 4920 436f 6e66 6572 656e 6365 206f 6e20  I Conference on 
+000034b0: 4875 6d61 6e20 4661 6374 6f72 7320 696e  Human Factors in
+000034c0: 2043 6f6d 7075 7469 6e67 2053 7973 7465   Computing Syste
+000034d0: 6d73 7d2c 0a20 2070 6167 6573 3d7b 312d  ms},.  pages={1-
+000034e0: 2d31 347d 2c0a 2020 7965 6172 3d7b 3230  -14},.  year={20
+000034f0: 3230 7d0a 7d0a 2020 2020 3c2f 7072 653e  20}.}.    </pre>
+00003500: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00003510: 7470 733a 2f2f 7777 772e 6d69 6372 6f73  tps://www.micros
+00003520: 6f66 742e 636f 6d2f 656e 2d75 732f 7265  oft.com/en-us/re
+00003530: 7365 6172 6368 2f70 7562 6c69 6361 7469  search/publicati
+00003540: 6f6e 2f69 6e74 6572 7072 6574 696e 672d  on/interpreting-
+00003550: 696e 7465 7270 7265 7461 6269 6c69 7479  interpretability
+00003560: 2d75 6e64 6572 7374 616e 6469 6e67 2d64  -understanding-d
+00003570: 6174 612d 7363 6965 6e74 6973 7473 2d75  ata-scientists-u
+00003580: 7365 2d6f 662d 696e 7465 7270 7265 7461  se-of-interpreta
+00003590: 6269 6c69 7479 2d74 6f6f 6c73 2d66 6f72  bility-tools-for
+000035a0: 2d6d 6163 6869 6e65 2d6c 6561 726e 696e  -machine-learnin
+000035b0: 672f 223e 5061 7065 7220 6c69 6e6b 3c2f  g/">Paper link</
+000035c0: 613e 0a20 203c 2f64 6574 6169 6c73 3e0a  a>.  </details>.
+000035d0: 0a20 203c 6465 7461 696c 733e 0a20 2020  .  <details>.   
+000035e0: 203c 7375 6d6d 6172 793e 0a20 2020 2020   <summary>.     
+000035f0: 203c 656d 3e22 486f 7720 496e 7465 7270   <em>"How Interp
+00003600: 7265 7461 626c 6520 616e 6420 5472 7573  retable and Trus
+00003610: 7477 6f72 7468 7920 6172 6520 4741 4d73  tworthy are GAMs
+00003620: 3f22 2028 432e 2043 6861 6e67 2c20 532e  ?" (C. Chang, S.
+00003630: 2054 616e 2c20 422e 204c 656e 6765 7269   Tan, B. Lengeri
+00003640: 6368 2c20 412e 2047 6f6c 6465 6e62 6572  ch, A. Goldenber
+00003650: 672c 2052 2e20 4361 7275 616e 6120 3230  g, R. Caruana 20
+00003660: 3230 293c 2f65 6d3e 0a20 2020 203c 2f73  20)</em>.    </s
+00003670: 756d 6d61 7279 3e0a 2020 2020 3c62 722f  ummary>.    <br/
+00003680: 3e0a 2020 2020 3c70 7265 3e0a 4061 7274  >.    <pre>.@art
+00003690: 6963 6c65 7b63 6861 6e67 3230 3230 696e  icle{chang2020in
+000036a0: 7465 7270 7265 7461 626c 652c 0a20 2074  terpretable,.  t
+000036b0: 6974 6c65 3d7b 486f 7720 496e 7465 7270  itle={How Interp
+000036c0: 7265 7461 626c 6520 616e 6420 5472 7573  retable and Trus
+000036d0: 7477 6f72 7468 7920 6172 6520 4741 4d73  tworthy are GAMs
+000036e0: 3f7d 2c0a 2020 6175 7468 6f72 3d7b 4368  ?},.  author={Ch
+000036f0: 616e 672c 2043 6875 6e2d 4861 6f20 616e  ang, Chun-Hao an
+00003700: 6420 5461 6e2c 2053 6172 6168 2061 6e64  d Tan, Sarah and
+00003710: 204c 656e 6765 7269 6368 2c20 4265 6e20   Lengerich, Ben 
+00003720: 616e 6420 476f 6c64 656e 6265 7267 2c20  and Goldenberg, 
+00003730: 416e 6e61 2061 6e64 2043 6172 7561 6e61  Anna and Caruana
+00003740: 2c20 5269 6368 7d2c 0a20 206a 6f75 726e  , Rich},.  journ
+00003750: 616c 3d7b 6172 5869 7620 7072 6570 7269  al={arXiv prepri
+00003760: 6e74 2061 7258 6976 3a32 3030 362e 3036  nt arXiv:2006.06
+00003770: 3436 367d 2c0a 2020 7965 6172 3d7b 3230  466},.  year={20
+00003780: 3230 7d0a 7d0a 2020 2020 3c2f 7072 653e  20}.}.    </pre>
+00003790: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+000037a0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+000037b0: 7064 662f 3230 3036 2e30 3634 3636 2e70  pdf/2006.06466.p
+000037c0: 6466 223e 5061 7065 7220 6c69 6e6b 3c2f  df">Paper link</
+000037d0: 613e 0a20 203c 2f64 6574 6169 6c73 3e0a  a>.  </details>.
+000037e0: 0a20 203c 6872 2f3e 0a3c 2f64 6574 6169  .  <hr/>.</detai
+000037f0: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a20  ls>..<details>. 
+00003800: 203c 7375 6d6d 6172 793e 3c73 7472 6f6e   <summary><stron
+00003810: 673e 4469 6666 6572 656e 7469 616c 2050  g>Differential P
+00003820: 7269 7661 6379 3c2f 7374 726f 6e67 3e3c  rivacy</strong><
+00003830: 2f73 756d 6d61 7279 3e0a 2020 3c68 722f  /summary>.  <hr/
+00003840: 3e0a 0a20 203c 6465 7461 696c 733e 0a20  >..  <details>. 
+00003850: 2020 203c 7375 6d6d 6172 793e 0a20 2020     <summary>.   
+00003860: 2020 203c 656d 3e22 4163 6375 7261 6379     <em>"Accuracy
+00003870: 2c20 496e 7465 7270 7265 7461 6269 6c69  , Interpretabili
+00003880: 7479 2c20 616e 6420 4469 6666 6572 656e  ty, and Differen
+00003890: 7469 616c 2050 7269 7661 6379 2076 6961  tial Privacy via
+000038a0: 2045 7870 6c61 696e 6162 6c65 2042 6f6f   Explainable Boo
+000038b0: 7374 696e 6722 2028 482e 204e 6f72 692c  sting" (H. Nori,
+000038c0: 2052 2e20 4361 7275 616e 612c 205a 2e20   R. Caruana, Z. 
+000038d0: 4275 2c20 4a2e 2053 6865 6e2c 204a 2e20  Bu, J. Shen, J. 
+000038e0: 4b75 6c6b 6172 6e69 2032 3032 3129 3c2f  Kulkarni 2021)</
+000038f0: 656d 3e0a 2020 2020 3c2f 7375 6d6d 6172  em>.    </summar
+00003900: 793e 0a20 2020 203c 6272 2f3e 0a20 2020  y>.    <br/>.   
+00003910: 203c 7072 653e 0a40 696e 7072 6f63 6565   <pre>.@inprocee
+00003920: 6469 6e67 737b 706d 6c72 2d76 3133 392d  dings{pmlr-v139-
+00003930: 6e6f 7269 3231 612c 0a20 2074 6974 6c65  nori21a,.  title
+00003940: 203d 2009 207b 4163 6375 7261 6379 2c20   = . {Accuracy, 
+00003950: 496e 7465 7270 7265 7461 6269 6c69 7479  Interpretability
+00003960: 2c20 616e 6420 4469 6666 6572 656e 7469  , and Differenti
+00003970: 616c 2050 7269 7661 6379 2076 6961 2045  al Privacy via E
+00003980: 7870 6c61 696e 6162 6c65 2042 6f6f 7374  xplainable Boost
+00003990: 696e 677d 2c0a 2020 6175 7468 6f72 203d  ing},.  author =
+000039a0: 2020 2020 2020 207b 4e6f 7269 2c20 4861         {Nori, Ha
+000039b0: 7273 6861 2061 6e64 2043 6172 7561 6e61  rsha and Caruana
+000039c0: 2c20 5269 6368 2061 6e64 2042 752c 205a  , Rich and Bu, Z
+000039d0: 6869 7169 2061 6e64 2053 6865 6e2c 204a  hiqi and Shen, J
+000039e0: 7564 7920 4861 6e77 656e 2061 6e64 204b  udy Hanwen and K
+000039f0: 756c 6b61 726e 692c 204a 616e 6172 6468  ulkarni, Janardh
+00003a00: 616e 7d2c 0a20 2062 6f6f 6b74 6974 6c65  an},.  booktitle
+00003a10: 203d 2009 207b 5072 6f63 6565 6469 6e67   = . {Proceeding
+00003a20: 7320 6f66 2074 6865 2033 3874 6820 496e  s of the 38th In
+00003a30: 7465 726e 6174 696f 6e61 6c20 436f 6e66  ternational Conf
+00003a40: 6572 656e 6365 206f 6e20 4d61 6368 696e  erence on Machin
+00003a50: 6520 4c65 6172 6e69 6e67 7d2c 0a20 2070  e Learning},.  p
+00003a60: 6167 6573 203d 2009 207b 3832 3237 2d2d  ages = . {8227--
+00003a70: 3832 3337 7d2c 0a20 2079 6561 7220 3d20  8237},.  year = 
+00003a80: 0920 7b32 3032 317d 2c0a 2020 766f 6c75  . {2021},.  volu
+00003a90: 6d65 203d 2009 207b 3133 397d 2c0a 2020  me = . {139},.  
+00003aa0: 7365 7269 6573 203d 2009 207b 5072 6f63  series = . {Proc
+00003ab0: 6565 6469 6e67 7320 6f66 204d 6163 6869  eedings of Machi
+00003ac0: 6e65 204c 6561 726e 696e 6720 5265 7365  ne Learning Rese
+00003ad0: 6172 6368 7d2c 0a20 2070 7562 6c69 7368  arch},.  publish
+00003ae0: 6572 203d 2020 2020 7b50 4d4c 527d 0a7d  er =    {PMLR}.}
+00003af0: 0a20 2020 203c 2f70 7265 3e0a 2020 2020  .    </pre>.    
+00003b00: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00003b10: 2f70 726f 6365 6564 696e 6773 2e6d 6c72  /proceedings.mlr
+00003b20: 2e70 7265 7373 2f76 3133 392f 6e6f 7269  .press/v139/nori
+00003b30: 3231 612f 6e6f 7269 3231 612e 7064 6622  21a/nori21a.pdf"
+00003b40: 3e50 6170 6572 206c 696e 6b3c 2f61 3e0a  >Paper link</a>.
+00003b50: 2020 3c2f 6465 7461 696c 733e 0a0a 2020    </details>..  
+00003b60: 3c68 722f 3e0a 3c2f 6465 7461 696c 733e  <hr/>.</details>
+00003b70: 0a0a 3c64 6574 6169 6c73 3e0a 2020 3c73  ..<details>.  <s
+00003b80: 756d 6d61 7279 3e3c 7374 726f 6e67 3e4c  ummary><strong>L
+00003b90: 494d 453c 2f73 7472 6f6e 673e 3c2f 7375  IME</strong></su
+00003ba0: 6d6d 6172 793e 0a20 203c 6872 2f3e 0a0a  mmary>.  <hr/>..
+00003bb0: 2020 3c64 6574 6169 6c73 3e0a 2020 2020    <details>.    
+00003bc0: 3c73 756d 6d61 7279 3e0a 2020 2020 2020  <summary>.      
+00003bd0: 3c65 6d3e 2257 6879 2073 686f 756c 6420  <em>"Why should 
+00003be0: 6920 7472 7573 7420 796f 753f 3a20 4578  i trust you?: Ex
+00003bf0: 706c 6169 6e69 6e67 2074 6865 2070 7265  plaining the pre
+00003c00: 6469 6374 696f 6e73 206f 6620 616e 7920  dictions of any 
+00003c10: 636c 6173 7369 6669 6572 2220 284d 2e20  classifier" (M. 
+00003c20: 542e 2052 6962 6569 726f 2c20 532e 2053  T. Ribeiro, S. S
+00003c30: 696e 6768 2c20 616e 6420 432e 2047 7565  ingh, and C. Gue
+00003c40: 7374 7269 6e20 3230 3136 293c 2f65 6d3e  strin 2016)</em>
+00003c50: 0a20 2020 203c 2f73 756d 6d61 7279 3e0a  .    </summary>.
+00003c60: 2020 2020 3c62 722f 3e0a 2020 2020 3c70      <br/>.    <p
+00003c70: 7265 3e0a 4069 6e70 726f 6365 6564 696e  re>.@inproceedin
+00003c80: 6773 7b72 6962 6569 726f 3230 3136 7368  gs{ribeiro2016sh
+00003c90: 6f75 6c64 2c0a 2020 7469 746c 653d 7b57  ould,.  title={W
+00003ca0: 6879 2073 686f 756c 6420 6920 7472 7573  hy should i trus
+00003cb0: 7420 796f 753f 3a20 4578 706c 6169 6e69  t you?: Explaini
+00003cc0: 6e67 2074 6865 2070 7265 6469 6374 696f  ng the predictio
+00003cd0: 6e73 206f 6620 616e 7920 636c 6173 7369  ns of any classi
+00003ce0: 6669 6572 7d2c 0a20 2061 7574 686f 723d  fier},.  author=
+00003cf0: 7b52 6962 6569 726f 2c20 4d61 7263 6f20  {Ribeiro, Marco 
+00003d00: 5475 6c69 6f20 616e 6420 5369 6e67 682c  Tulio and Singh,
+00003d10: 2053 616d 6565 7220 616e 6420 4775 6573   Sameer and Gues
+00003d20: 7472 696e 2c20 4361 726c 6f73 7d2c 0a20  trin, Carlos},. 
+00003d30: 2062 6f6f 6b74 6974 6c65 3d7b 5072 6f63   booktitle={Proc
+00003d40: 6565 6469 6e67 7320 6f66 2074 6865 2032  eedings of the 2
+00003d50: 326e 6420 4143 4d20 5349 474b 4444 2069  2nd ACM SIGKDD i
+00003d60: 6e74 6572 6e61 7469 6f6e 616c 2063 6f6e  nternational con
+00003d70: 6665 7265 6e63 6520 6f6e 206b 6e6f 776c  ference on knowl
+00003d80: 6564 6765 2064 6973 636f 7665 7279 2061  edge discovery a
+00003d90: 6e64 2064 6174 6120 6d69 6e69 6e67 7d2c  nd data mining},
+00003da0: 0a20 2070 6167 6573 3d7b 3131 3335 2d2d  .  pages={1135--
+00003db0: 3131 3434 7d2c 0a20 2079 6561 723d 7b32  1144},.  year={2
+00003dc0: 3031 367d 2c0a 2020 6f72 6761 6e69 7a61  016},.  organiza
+00003dd0: 7469 6f6e 3d7b 4143 4d7d 0a7d 0a20 2020  tion={ACM}.}.   
+00003de0: 203c 2f70 7265 3e0a 2020 2020 3c61 2068   </pre>.    <a h
+00003df0: 7265 663d 2268 7474 7073 3a2f 2f61 7278  ref="https://arx
+00003e00: 6976 2e6f 7267 2f70 6466 2f31 3630 322e  iv.org/pdf/1602.
+00003e10: 3034 3933 382e 7064 6622 3e50 6170 6572  04938.pdf">Paper
+00003e20: 206c 696e 6b3c 2f61 3e0a 2020 3c2f 6465   link</a>.  </de
+00003e30: 7461 696c 733e 0a0a 2020 3c68 722f 3e0a  tails>..  <hr/>.
+00003e40: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
+00003e50: 6169 6c73 3e0a 2020 3c73 756d 6d61 7279  ails>.  <summary
+00003e60: 3e3c 7374 726f 6e67 3e53 4841 503c 2f73  ><strong>SHAP</s
+00003e70: 7472 6f6e 673e 3c2f 7375 6d6d 6172 793e  trong></summary>
+00003e80: 0a20 203c 6872 2f3e 0a0a 2020 3c64 6574  .  <hr/>..  <det
+00003e90: 6169 6c73 3e0a 2020 2020 3c73 756d 6d61  ails>.    <summa
+00003ea0: 7279 3e0a 2020 2020 2020 3c65 6d3e 2241  ry>.      <em>"A
+00003eb0: 2055 6e69 6669 6564 2041 7070 726f 6163   Unified Approac
+00003ec0: 6820 746f 2049 6e74 6572 7072 6574 696e  h to Interpretin
+00003ed0: 6720 4d6f 6465 6c20 5072 6564 6963 7469  g Model Predicti
+00003ee0: 6f6e 7322 2028 532e 204d 2e20 4c75 6e64  ons" (S. M. Lund
+00003ef0: 6265 7267 2061 6e64 2053 2e2d 492e 204c  berg and S.-I. L
+00003f00: 6565 2032 3031 3729 3c2f 656d 3e0a 2020  ee 2017)</em>.  
+00003f10: 2020 3c2f 7375 6d6d 6172 793e 0a20 2020    </summary>.   
+00003f20: 203c 6272 2f3e 0a20 2020 203c 7072 653e   <br/>.    <pre>
+00003f30: 0a40 696e 636f 6c6c 6563 7469 6f6e 7b4e  .@incollection{N
+00003f40: 4950 5332 3031 375f 3730 3632 2c0a 2074  IPS2017_7062,. t
+00003f50: 6974 6c65 203d 207b 4120 556e 6966 6965  itle = {A Unifie
+00003f60: 6420 4170 7072 6f61 6368 2074 6f20 496e  d Approach to In
+00003f70: 7465 7270 7265 7469 6e67 204d 6f64 656c  terpreting Model
+00003f80: 2050 7265 6469 6374 696f 6e73 7d2c 0a20   Predictions},. 
+00003f90: 6175 7468 6f72 203d 207b 4c75 6e64 6265  author = {Lundbe
+00003fa0: 7267 2c20 5363 6f74 7420 4d20 616e 6420  rg, Scott M and 
+00003fb0: 4c65 652c 2053 752d 496e 7d2c 0a20 626f  Lee, Su-In},. bo
+00003fc0: 6f6b 7469 746c 6520 3d20 7b41 6476 616e  oktitle = {Advan
+00003fd0: 6365 7320 696e 204e 6575 7261 6c20 496e  ces in Neural In
+00003fe0: 666f 726d 6174 696f 6e20 5072 6f63 6573  formation Proces
+00003ff0: 7369 6e67 2053 7973 7465 6d73 2033 307d  sing Systems 30}
+00004000: 2c0a 2065 6469 746f 7220 3d20 7b49 2e20  ,. editor = {I. 
+00004010: 4775 796f 6e20 616e 6420 552e 2056 2e20  Guyon and U. V. 
+00004020: 4c75 7862 7572 6720 616e 6420 532e 2042  Luxburg and S. B
+00004030: 656e 6769 6f20 616e 6420 482e 2057 616c  engio and H. Wal
+00004040: 6c61 6368 2061 6e64 2052 2e20 4665 7267  lach and R. Ferg
+00004050: 7573 2061 6e64 2053 2e20 5669 7368 7761  us and S. Vishwa
+00004060: 6e61 7468 616e 2061 6e64 2052 2e20 4761  nathan and R. Ga
+00004070: 726e 6574 747d 2c0a 2070 6167 6573 203d  rnett},. pages =
+00004080: 207b 3437 3635 2d2d 3437 3734 7d2c 0a20   {4765--4774},. 
+00004090: 7965 6172 203d 207b 3230 3137 7d2c 0a20  year = {2017},. 
+000040a0: 7075 626c 6973 6865 7220 3d20 7b43 7572  publisher = {Cur
+000040b0: 7261 6e20 4173 736f 6369 6174 6573 2c20  ran Associates, 
+000040c0: 496e 632e 7d2c 0a20 7572 6c20 3d20 7b68  Inc.},. url = {h
+000040d0: 7474 7073 3a2f 2f70 6170 6572 732e 6e69  ttps://papers.ni
+000040e0: 7073 2e63 632f 7061 7065 722f 3730 3632  ps.cc/paper/7062
+000040f0: 2d61 2d75 6e69 6669 6564 2d61 7070 726f  -a-unified-appro
+00004100: 6163 682d 746f 2d69 6e74 6572 7072 6574  ach-to-interpret
+00004110: 696e 672d 6d6f 6465 6c2d 7072 6564 6963  ing-model-predic
+00004120: 7469 6f6e 732e 7064 667d 0a7d 0a20 2020  tions.pdf}.}.   
+00004130: 203c 2f70 7265 3e0a 2020 2020 3c61 2068   </pre>.    <a h
+00004140: 7265 663d 2268 7474 7073 3a2f 2f70 6170  ref="https://pap
+00004150: 6572 732e 6e69 7073 2e63 632f 7061 7065  ers.nips.cc/pape
+00004160: 722f 3730 3632 2d61 2d75 6e69 6669 6564  r/7062-a-unified
+00004170: 2d61 7070 726f 6163 682d 746f 2d69 6e74  -approach-to-int
+00004180: 6572 7072 6574 696e 672d 6d6f 6465 6c2d  erpreting-model-
+00004190: 7072 6564 6963 7469 6f6e 732e 7064 6622  predictions.pdf"
+000041a0: 3e50 6170 6572 206c 696e 6b3c 2f61 3e0a  >Paper link</a>.
+000041b0: 2020 3c2f 6465 7461 696c 733e 0a0a 2020    </details>..  
+000041c0: 3c64 6574 6169 6c73 3e0a 2020 2020 3c73  <details>.    <s
+000041d0: 756d 6d61 7279 3e0a 2020 2020 2020 3c65  ummary>.      <e
+000041e0: 6d3e 2243 6f6e 7369 7374 656e 7420 696e  m>"Consistent in
+000041f0: 6469 7669 6475 616c 697a 6564 2066 6561  dividualized fea
+00004200: 7475 7265 2061 7474 7269 6275 7469 6f6e  ture attribution
+00004210: 2066 6f72 2074 7265 6520 656e 7365 6d62   for tree ensemb
+00004220: 6c65 7322 2028 4c75 6e64 6265 7267 2c20  les" (Lundberg, 
+00004230: 5363 6f74 7420 4d20 616e 6420 4572 696f  Scott M and Erio
+00004240: 6e2c 2047 6162 7269 656c 2047 2061 6e64  n, Gabriel G and
+00004250: 204c 6565 2c20 5375 2d49 6e20 3230 3138   Lee, Su-In 2018
+00004260: 293c 2f65 6d3e 0a20 2020 203c 2f73 756d  )</em>.    </sum
+00004270: 6d61 7279 3e0a 2020 2020 3c62 722f 3e0a  mary>.    <br/>.
+00004280: 2020 2020 3c70 7265 3e0a 4061 7274 6963      <pre>.@artic
+00004290: 6c65 7b6c 756e 6462 6572 6732 3031 3863  le{lundberg2018c
+000042a0: 6f6e 7369 7374 656e 742c 0a20 2074 6974  onsistent,.  tit
+000042b0: 6c65 3d7b 436f 6e73 6973 7465 6e74 2069  le={Consistent i
+000042c0: 6e64 6976 6964 7561 6c69 7a65 6420 6665  ndividualized fe
+000042d0: 6174 7572 6520 6174 7472 6962 7574 696f  ature attributio
+000042e0: 6e20 666f 7220 7472 6565 2065 6e73 656d  n for tree ensem
+000042f0: 626c 6573 7d2c 0a20 2061 7574 686f 723d  bles},.  author=
+00004300: 7b4c 756e 6462 6572 672c 2053 636f 7474  {Lundberg, Scott
+00004310: 204d 2061 6e64 2045 7269 6f6e 2c20 4761   M and Erion, Ga
+00004320: 6272 6965 6c20 4720 616e 6420 4c65 652c  briel G and Lee,
+00004330: 2053 752d 496e 7d2c 0a20 206a 6f75 726e   Su-In},.  journ
+00004340: 616c 3d7b 6172 5869 7620 7072 6570 7269  al={arXiv prepri
+00004350: 6e74 2061 7258 6976 3a31 3830 322e 3033  nt arXiv:1802.03
+00004360: 3838 387d 2c0a 2020 7965 6172 3d7b 3230  888},.  year={20
+00004370: 3138 7d0a 7d0a 2020 2020 3c2f 7072 653e  18}.}.    </pre>
+00004380: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00004390: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+000043a0: 7064 662f 3138 3032 2e30 3338 3838 223e  pdf/1802.03888">
+000043b0: 5061 7065 7220 6c69 6e6b 3c2f 613e 0a20  Paper link</a>. 
+000043c0: 203c 2f64 6574 6169 6c73 3e0a 0a20 203c   </details>..  <
+000043d0: 6465 7461 696c 733e 0a20 2020 203c 7375  details>.    <su
+000043e0: 6d6d 6172 793e 0a20 2020 2020 203c 656d  mmary>.      <em
+000043f0: 3e22 4578 706c 6169 6e61 626c 6520 6d61  >"Explainable ma
+00004400: 6368 696e 652d 6c65 6172 6e69 6e67 2070  chine-learning p
+00004410: 7265 6469 6374 696f 6e73 2066 6f72 2074  redictions for t
+00004420: 6865 2070 7265 7665 6e74 696f 6e20 6f66  he prevention of
+00004430: 2068 7970 6f78 6165 6d69 6120 6475 7269   hypoxaemia duri
+00004440: 6e67 2073 7572 6765 7279 2220 2853 2e20  ng surgery" (S. 
+00004450: 4d2e 204c 756e 6462 6572 6720 6574 2061  M. Lundberg et a
+00004460: 6c2e 2032 3031 3829 3c2f 656d 3e0a 2020  l. 2018)</em>.  
+00004470: 2020 3c2f 7375 6d6d 6172 793e 0a20 2020    </summary>.   
+00004480: 203c 6272 2f3e 0a20 2020 203c 7072 653e   <br/>.    <pre>
+00004490: 0a40 6172 7469 636c 657b 6c75 6e64 6265  .@article{lundbe
+000044a0: 7267 3230 3138 6578 706c 6169 6e61 626c  rg2018explainabl
+000044b0: 652c 0a20 2074 6974 6c65 3d7b 4578 706c  e,.  title={Expl
+000044c0: 6169 6e61 626c 6520 6d61 6368 696e 652d  ainable machine-
+000044d0: 6c65 6172 6e69 6e67 2070 7265 6469 6374  learning predict
+000044e0: 696f 6e73 2066 6f72 2074 6865 2070 7265  ions for the pre
+000044f0: 7665 6e74 696f 6e20 6f66 2068 7970 6f78  vention of hypox
+00004500: 6165 6d69 6120 6475 7269 6e67 2073 7572  aemia during sur
+00004510: 6765 7279 7d2c 0a20 2061 7574 686f 723d  gery},.  author=
+00004520: 7b4c 756e 6462 6572 672c 2053 636f 7474  {Lundberg, Scott
+00004530: 204d 2061 6e64 204e 6169 722c 2042 616c   M and Nair, Bal
+00004540: 6120 616e 6420 5661 7669 6c61 6c61 2c20  a and Vavilala, 
+00004550: 4d6f 6e69 6361 2053 2061 6e64 2048 6f72  Monica S and Hor
+00004560: 6962 652c 204d 6179 756d 6920 616e 6420  ibe, Mayumi and 
+00004570: 4569 7373 6573 2c20 4d69 6368 6165 6c20  Eisses, Michael 
+00004580: 4a20 616e 6420 4164 616d 732c 2054 7265  J and Adams, Tre
+00004590: 766f 7220 616e 6420 4c69 7374 6f6e 2c20  vor and Liston, 
+000045a0: 4461 7669 6420 4520 616e 6420 4c6f 772c  David E and Low,
+000045b0: 2044 616e 6965 6c20 4b69 6e67 2d57 6169   Daniel King-Wai
+000045c0: 2061 6e64 204e 6577 6d61 6e2c 2053 6875   and Newman, Shu
+000045d0: 2d46 616e 6720 616e 6420 4b69 6d2c 204a  -Fang and Kim, J
+000045e0: 6572 7279 2061 6e64 206f 7468 6572 737d  erry and others}
+000045f0: 2c0a 2020 6a6f 7572 6e61 6c3d 7b4e 6174  ,.  journal={Nat
+00004600: 7572 6520 4269 6f6d 6564 6963 616c 2045  ure Biomedical E
+00004610: 6e67 696e 6565 7269 6e67 7d2c 0a20 2076  ngineering},.  v
+00004620: 6f6c 756d 653d 7b32 7d2c 0a20 206e 756d  olume={2},.  num
+00004630: 6265 723d 7b31 307d 2c0a 2020 7061 6765  ber={10},.  page
+00004640: 733d 7b37 3439 7d2c 0a20 2079 6561 723d  s={749},.  year=
+00004650: 7b32 3031 387d 2c0a 2020 7075 626c 6973  {2018},.  publis
+00004660: 6865 723d 7b4e 6174 7572 6520 5075 626c  her={Nature Publ
+00004670: 6973 6869 6e67 2047 726f 7570 7d0a 7d0a  ishing Group}.}.
+00004680: 2020 2020 3c2f 7072 653e 0a20 2020 203c      </pre>.    <
+00004690: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000046a0: 7777 772e 6e63 6269 2e6e 6c6d 2e6e 6968  www.ncbi.nlm.nih
+000046b0: 2e67 6f76 2f70 6d63 2f61 7274 6963 6c65  .gov/pmc/article
+000046c0: 732f 504d 4336 3436 3734 3932 2f70 6466  s/PMC6467492/pdf
+000046d0: 2f6e 6968 6d73 2d31 3530 3535 3738 2e70  /nihms-1505578.p
+000046e0: 6466 223e 5061 7065 7220 6c69 6e6b 3c2f  df">Paper link</
+000046f0: 613e 0a20 203c 2f64 6574 6169 6c73 3e0a  a>.  </details>.
+00004700: 0a20 203c 6872 2f3e 0a3c 2f64 6574 6169  .  <hr/>.</detai
+00004710: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a20  ls>..<details>. 
+00004720: 203c 7375 6d6d 6172 793e 3c73 7472 6f6e   <summary><stron
+00004730: 673e 5365 6e73 6974 6976 6974 7920 416e  g>Sensitivity An
+00004740: 616c 7973 6973 3c2f 7374 726f 6e67 3e3c  alysis</strong><
+00004750: 2f73 756d 6d61 7279 3e0a 2020 3c68 722f  /summary>.  <hr/
+00004760: 3e0a 0a20 203c 6465 7461 696c 733e 0a20  >..  <details>. 
+00004770: 2020 203c 7375 6d6d 6172 793e 0a20 2020     <summary>.   
+00004780: 2020 203c 656d 3e22 5341 4c69 623a 2041     <em>"SALib: A
+00004790: 6e20 6f70 656e 2d73 6f75 7263 6520 5079  n open-source Py
+000047a0: 7468 6f6e 206c 6962 7261 7279 2066 6f72  thon library for
+000047b0: 2053 656e 7369 7469 7669 7479 2041 6e61   Sensitivity Ana
+000047c0: 6c79 7369 7322 2028 4a2e 2044 2e20 4865  lysis" (J. D. He
+000047d0: 726d 616e 2061 6e64 2057 2e20 5573 6865  rman and W. Ushe
+000047e0: 7220 3230 3137 293c 2f65 6d3e 0a20 2020  r 2017)</em>.   
+000047f0: 203c 2f73 756d 6d61 7279 3e0a 2020 2020   </summary>.    
+00004800: 3c62 722f 3e0a 2020 2020 3c70 7265 3e0a  <br/>.    <pre>.
+00004810: 4061 7274 6963 6c65 7b68 6572 6d61 6e32  @article{herman2
+00004820: 3031 3773 616c 6962 2c0a 2020 7469 746c  017salib,.  titl
+00004830: 653d 7b53 414c 6962 3a20 416e 206f 7065  e={SALib: An ope
+00004840: 6e2d 736f 7572 6365 2050 7974 686f 6e20  n-source Python 
+00004850: 6c69 6272 6172 7920 666f 7220 5365 6e73  library for Sens
+00004860: 6974 6976 6974 7920 416e 616c 7973 6973  itivity Analysis
+00004870: 2e7d 2c0a 2020 6175 7468 6f72 3d7b 4865  .},.  author={He
+00004880: 726d 616e 2c20 4a6f 6e61 7468 616e 2044  rman, Jonathan D
+00004890: 2061 6e64 2055 7368 6572 2c20 5769 6c6c   and Usher, Will
+000048a0: 7d2c 0a20 206a 6f75 726e 616c 3d7b 4a2e  },.  journal={J.
+000048b0: 204f 7065 6e20 536f 7572 6365 2053 6f66   Open Source Sof
+000048c0: 7477 6172 657d 2c0a 2020 766f 6c75 6d65  tware},.  volume
+000048d0: 3d7b 327d 2c0a 2020 6e75 6d62 6572 3d7b  ={2},.  number={
+000048e0: 397d 2c0a 2020 7061 6765 733d 7b39 377d  9},.  pages={97}
+000048f0: 2c0a 2020 7965 6172 3d7b 3230 3137 7d0a  ,.  year={2017}.
+00004900: 7d0a 2020 2020 3c2f 7072 653e 0a20 2020  }.    </pre>.   
+00004910: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00004920: 2f2f 7777 772e 7265 7365 6172 6368 6761  //www.researchga
+00004930: 7465 2e6e 6574 2f70 726f 6669 6c65 2f57  te.net/profile/W
+00004940: 696c 6c5f 5573 6865 722f 7075 626c 6963  ill_Usher/public
+00004950: 6174 696f 6e2f 3331 3232 3034 3233 365f  ation/312204236_
+00004960: 5341 4c69 625f 416e 5f6f 7065 6e2d 736f  SALib_An_open-so
+00004970: 7572 6365 5f50 7974 686f 6e5f 6c69 6272  urce_Python_libr
+00004980: 6172 795f 666f 725f 5365 6e73 6974 6976  ary_for_Sensitiv
+00004990: 6974 795f 416e 616c 7973 6973 2f6c 696e  ity_Analysis/lin
+000049a0: 6b73 2f35 6163 3733 3264 3634 3538 3531  ks/5ac732d645851
+000049b0: 3531 6538 3061 3339 3534 372f 5341 4c69  51e80a39547/SALi
+000049c0: 622d 416e 2d6f 7065 6e2d 736f 7572 6365  b-An-open-source
+000049d0: 2d50 7974 686f 6e2d 6c69 6272 6172 792d  -Python-library-
+000049e0: 666f 722d 5365 6e73 6974 6976 6974 792d  for-Sensitivity-
+000049f0: 416e 616c 7973 6973 2e70 6466 3f6f 7269  Analysis.pdf?ori
+00004a00: 6769 6e3d 7075 626c 6963 6174 696f 6e5f  gin=publication_
+00004a10: 6465 7461 696c 223e 5061 7065 7220 6c69  detail">Paper li
+00004a20: 6e6b 3c2f 613e 0a20 203c 2f64 6574 6169  nk</a>.  </detai
+00004a30: 6c73 3e0a 0a20 203c 6465 7461 696c 733e  ls>..  <details>
+00004a40: 0a20 2020 203c 7375 6d6d 6172 793e 0a20  .    <summary>. 
+00004a50: 2020 2020 203c 656d 3e22 4661 6374 6f72       <em>"Factor
+00004a60: 6961 6c20 7361 6d70 6c69 6e67 2070 6c61  ial sampling pla
+00004a70: 6e73 2066 6f72 2070 7265 6c69 6d69 6e61  ns for prelimina
+00004a80: 7279 2063 6f6d 7075 7461 7469 6f6e 616c  ry computational
+00004a90: 2065 7870 6572 696d 656e 7473 2220 284d   experiments" (M
+00004aa0: 2e20 442e 204d 6f72 7269 7320 3139 3931  . D. Morris 1991
+00004ab0: 293c 2f65 6d3e 0a20 2020 203c 2f73 756d  )</em>.    </sum
+00004ac0: 6d61 7279 3e0a 2020 2020 3c62 722f 3e0a  mary>.    <br/>.
+00004ad0: 2020 2020 3c70 7265 3e0a 4061 7274 6963      <pre>.@artic
+00004ae0: 6c65 7b6d 6f72 7269 7331 3939 3166 6163  le{morris1991fac
+00004af0: 746f 7269 616c 2c0a 2020 7469 746c 653d  torial,.  title=
+00004b00: 7b7d 2c0a 2020 6175 7468 6f72 3d7b 4d6f  {},.  author={Mo
+00004b10: 7272 6973 2c20 4d61 7820 447d 2c0a 2020  rris, Max D},.  
+00004b20: 6a6f 7572 6e61 6c3d 7b54 6563 686e 6f6d  journal={Technom
+00004b30: 6574 7269 6373 7d2c 0a20 2076 6f6c 756d  etrics},.  volum
+00004b40: 653d 7b33 337d 2c0a 2020 6e75 6d62 6572  e={33},.  number
+00004b50: 3d7b 327d 2c0a 2020 7061 6765 733d 7b31  ={2},.  pages={1
+00004b60: 3631 2d2d 3137 347d 2c0a 2020 7965 6172  61--174},.  year
+00004b70: 3d7b 3139 3931 7d2c 0a20 2070 7562 6c69  ={1991},.  publi
+00004b80: 7368 6572 3d7b 5461 796c 6f72 205c 2620  sher={Taylor \& 
+00004b90: 4672 616e 6369 7320 4772 6f75 707d 0a7d  Francis Group}.}
+00004ba0: 0a20 2020 203c 2f70 7265 3e0a 2020 2020  .    </pre>.    
+00004bb0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00004bc0: 2f61 6265 2e75 666c 2e65 6475 2f46 6163  /abe.ufl.edu/Fac
+00004bd0: 756c 7479 2f6a 6a6f 6e65 732f 4142 455f  ulty/jjones/ABE_
+00004be0: 3536 3436 2f32 3031 302f 4d6f 7272 6973  5646/2010/Morris
+00004bf0: 2e31 3939 3125 3230 5341 2532 3070 6170  .1991%20SA%20pap
+00004c00: 6572 2e70 6466 223e 5061 7065 7220 6c69  er.pdf">Paper li
+00004c10: 6e6b 3c2f 613e 0a20 203c 2f64 6574 6169  nk</a>.  </detai
+00004c20: 6c73 3e0a 0a20 203c 6872 2f3e 0a3c 2f64  ls>..  <hr/>.</d
+00004c30: 6574 6169 6c73 3e0a 0a3c 6465 7461 696c  etails>..<detail
+00004c40: 733e 0a20 203c 7375 6d6d 6172 793e 3c73  s>.  <summary><s
+00004c50: 7472 6f6e 673e 5061 7274 6961 6c20 4465  trong>Partial De
+00004c60: 7065 6e64 656e 6365 3c2f 7374 726f 6e67  pendence</strong
+00004c70: 3e3c 2f73 756d 6d61 7279 3e0a 2020 3c68  ></summary>.  <h
+00004c80: 722f 3e0a 0a20 203c 6465 7461 696c 733e  r/>..  <details>
+00004c90: 0a20 2020 203c 7375 6d6d 6172 793e 0a20  .    <summary>. 
+00004ca0: 2020 2020 203c 656d 3e22 4772 6565 6479       <em>"Greedy
+00004cb0: 2066 756e 6374 696f 6e20 6170 7072 6f78   function approx
+00004cc0: 696d 6174 696f 6e3a 2061 2067 7261 6469  imation: a gradi
+00004cd0: 656e 7420 626f 6f73 7469 6e67 206d 6163  ent boosting mac
+00004ce0: 6869 6e65 2220 284a 2e20 482e 2046 7269  hine" (J. H. Fri
+00004cf0: 6564 6d61 6e20 3230 3031 293c 2f65 6d3e  edman 2001)</em>
+00004d00: 0a20 2020 203c 2f73 756d 6d61 7279 3e0a  .    </summary>.
+00004d10: 2020 2020 3c62 722f 3e0a 2020 2020 3c70      <br/>.    <p
+00004d20: 7265 3e0a 4061 7274 6963 6c65 7b66 7269  re>.@article{fri
+00004d30: 6564 6d61 6e32 3030 3167 7265 6564 792c  edman2001greedy,
+00004d40: 0a20 2074 6974 6c65 3d7b 4772 6565 6479  .  title={Greedy
+00004d50: 2066 756e 6374 696f 6e20 6170 7072 6f78   function approx
+00004d60: 696d 6174 696f 6e3a 2061 2067 7261 6469  imation: a gradi
+00004d70: 656e 7420 626f 6f73 7469 6e67 206d 6163  ent boosting mac
+00004d80: 6869 6e65 7d2c 0a20 2061 7574 686f 723d  hine},.  author=
+00004d90: 7b46 7269 6564 6d61 6e2c 204a 6572 6f6d  {Friedman, Jerom
+00004da0: 6520 487d 2c0a 2020 6a6f 7572 6e61 6c3d  e H},.  journal=
+00004db0: 7b41 6e6e 616c 7320 6f66 2073 7461 7469  {Annals of stati
+00004dc0: 7374 6963 737d 2c0a 2020 7061 6765 733d  stics},.  pages=
+00004dd0: 7b31 3138 392d 2d31 3233 327d 2c0a 2020  {1189--1232},.  
+00004de0: 7965 6172 3d7b 3230 3031 7d2c 0a20 2070  year={2001},.  p
+00004df0: 7562 6c69 7368 6572 3d7b 4a53 544f 527d  ublisher={JSTOR}
+00004e00: 0a7d 0a20 2020 203c 2f70 7265 3e0a 2020  .}.    </pre>.  
+00004e10: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00004e20: 3a2f 2f70 726f 6a65 6374 6575 636c 6964  ://projecteuclid
+00004e30: 2e6f 7267 2f64 6f77 6e6c 6f61 642f 7064  .org/download/pd
+00004e40: 665f 312f 6575 636c 6964 2e61 6f73 2f31  f_1/euclid.aos/1
+00004e50: 3031 3332 3033 3435 3122 3e50 6170 6572  013203451">Paper
+00004e60: 206c 696e 6b3c 2f61 3e0a 2020 3c2f 6465   link</a>.  </de
+00004e70: 7461 696c 733e 0a0a 2020 3c68 722f 3e0a  tails>..  <hr/>.
+00004e80: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
+00004e90: 6169 6c73 3e0a 2020 3c73 756d 6d61 7279  ails>.  <summary
+00004ea0: 3e3c 7374 726f 6e67 3e4f 7065 6e20 536f  ><strong>Open So
+00004eb0: 7572 6365 2053 6f66 7477 6172 653c 2f73  urce Software</s
+00004ec0: 7472 6f6e 673e 3c2f 7375 6d6d 6172 793e  trong></summary>
+00004ed0: 0a20 203c 6872 2f3e 0a0a 2020 3c64 6574  .  <hr/>..  <det
+00004ee0: 6169 6c73 3e0a 2020 2020 3c73 756d 6d61  ails>.    <summa
+00004ef0: 7279 3e0a 2020 2020 2020 3c65 6d3e 2253  ry>.      <em>"S
+00004f00: 6369 6b69 742d 6c65 6172 6e3a 204d 6163  cikit-learn: Mac
+00004f10: 6869 6e65 206c 6561 726e 696e 6720 696e  hine learning in
+00004f20: 2050 7974 686f 6e22 2028 462e 2050 6564   Python" (F. Ped
+00004f30: 7265 676f 7361 2065 7420 616c 2e20 3230  regosa et al. 20
+00004f40: 3131 293c 2f65 6d3e 0a20 2020 203c 2f73  11)</em>.    </s
+00004f50: 756d 6d61 7279 3e0a 2020 2020 3c62 722f  ummary>.    <br/
+00004f60: 3e0a 2020 2020 3c70 7265 3e0a 4061 7274  >.    <pre>.@art
+00004f70: 6963 6c65 7b70 6564 7265 676f 7361 3230  icle{pedregosa20
+00004f80: 3131 7363 696b 6974 2c0a 2020 7469 746c  11scikit,.  titl
+00004f90: 653d 7b53 6369 6b69 742d 6c65 6172 6e3a  e={Scikit-learn:
+00004fa0: 204d 6163 6869 6e65 206c 6561 726e 696e   Machine learnin
+00004fb0: 6720 696e 2050 7974 686f 6e7d 2c0a 2020  g in Python},.  
+00004fc0: 6175 7468 6f72 3d7b 5065 6472 6567 6f73  author={Pedregos
+00004fd0: 612c 2046 6162 6961 6e20 616e 6420 5661  a, Fabian and Va
+00004fe0: 726f 7175 6175 782c 2047 617b 5c22 657d  roquaux, Ga{\"e}
+00004ff0: 6c20 616e 6420 4772 616d 666f 7274 2c20  l and Gramfort, 
+00005000: 416c 6578 616e 6472 6520 616e 6420 4d69  Alexandre and Mi
+00005010: 6368 656c 2c20 5669 6e63 656e 7420 616e  chel, Vincent an
+00005020: 6420 5468 6972 696f 6e2c 2042 6572 7472  d Thirion, Bertr
+00005030: 616e 6420 616e 6420 4772 6973 656c 2c20  and and Grisel, 
+00005040: 4f6c 6976 6965 7220 616e 6420 426c 6f6e  Olivier and Blon
+00005050: 6465 6c2c 204d 6174 6869 6575 2061 6e64  del, Mathieu and
+00005060: 2050 7265 7474 656e 686f 6665 722c 2050   Prettenhofer, P
+00005070: 6574 6572 2061 6e64 2057 6569 7373 2c20  eter and Weiss, 
+00005080: 526f 6e20 616e 6420 4475 626f 7572 672c  Ron and Dubourg,
+00005090: 2056 696e 6365 6e74 2061 6e64 206f 7468   Vincent and oth
+000050a0: 6572 737d 2c0a 2020 6a6f 7572 6e61 6c3d  ers},.  journal=
+000050b0: 7b4a 6f75 726e 616c 206f 6620 6d61 6368  {Journal of mach
+000050c0: 696e 6520 6c65 6172 6e69 6e67 2072 6573  ine learning res
+000050d0: 6561 7263 687d 2c0a 2020 766f 6c75 6d65  earch},.  volume
+000050e0: 3d7b 3132 7d2c 0a20 206e 756d 6265 723d  ={12},.  number=
+000050f0: 7b4f 6374 7d2c 0a20 2070 6167 6573 3d7b  {Oct},.  pages={
+00005100: 3238 3235 2d2d 3238 3330 7d2c 0a20 2079  2825--2830},.  y
+00005110: 6561 723d 7b32 3031 317d 0a7d 0a20 2020  ear={2011}.}.   
+00005120: 203c 2f70 7265 3e0a 2020 2020 3c61 2068   </pre>.    <a h
+00005130: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+00005140: 2e6a 6d6c 722e 6f72 672f 7061 7065 7273  .jmlr.org/papers
+00005150: 2f76 6f6c 756d 6531 322f 7065 6472 6567  /volume12/pedreg
+00005160: 6f73 6131 3161 2f70 6564 7265 676f 7361  osa11a/pedregosa
+00005170: 3131 612e 7064 6622 3e50 6170 6572 206c  11a.pdf">Paper l
+00005180: 696e 6b3c 2f61 3e0a 2020 3c2f 6465 7461  ink</a>.  </deta
+00005190: 696c 733e 0a0a 2020 3c64 6574 6169 6c73  ils>..  <details
+000051a0: 3e0a 2020 2020 3c73 756d 6d61 7279 3e0a  >.    <summary>.
+000051b0: 2020 2020 2020 3c65 6d3e 2243 6f6c 6c61        <em>"Colla
+000051c0: 626f 7261 7469 7665 2064 6174 6120 7363  borative data sc
+000051d0: 6965 6e63 6522 2028 506c 6f74 6c79 2054  ience" (Plotly T
+000051e0: 6563 686e 6f6c 6f67 6965 7320 496e 632e  echnologies Inc.
+000051f0: 2032 3031 3529 3c2f 656d 3e0a 2020 2020   2015)</em>.    
+00005200: 3c2f 7375 6d6d 6172 793e 0a20 2020 203c  </summary>.    <
+00005210: 6272 2f3e 0a20 2020 203c 7072 653e 0a40  br/>.    <pre>.@
+00005220: 6f6e 6c69 6e65 7b70 6c6f 746c 792c 200a  online{plotly, .
+00005230: 2020 6175 7468 6f72 203d 207b 506c 6f74    author = {Plot
+00005240: 6c79 2054 6563 686e 6f6c 6f67 6965 7320  ly Technologies 
+00005250: 496e 632e 7d2c 200a 2020 7469 746c 6520  Inc.}, .  title 
+00005260: 3d20 7b43 6f6c 6c61 626f 7261 7469 7665  = {Collaborative
+00005270: 2064 6174 6120 7363 6965 6e63 657d 2c20   data science}, 
+00005280: 0a20 2070 7562 6c69 7368 6572 203d 207b  .  publisher = {
+00005290: 506c 6f74 6c79 2054 6563 686e 6f6c 6f67  Plotly Technolog
+000052a0: 6965 7320 496e 632e 7d2c 200a 2020 6164  ies Inc.}, .  ad
+000052b0: 6472 6573 7320 3d20 7b4d 6f6e 7472 6561  dress = {Montrea
+000052c0: 6c2c 2051 437d 2c20 0a20 2079 6561 7220  l, QC}, .  year 
+000052d0: 3d20 7b32 3031 357d 2c20 0a20 2075 726c  = {2015}, .  url
+000052e0: 203d 207b 6874 7470 733a 2f2f 706c 6f74   = {https://plot
+000052f0: 2e6c 797d 0a7d 0a20 2020 203c 2f70 7265  .ly}.}.    </pre
+00005300: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
+00005310: 7474 7073 3a2f 2f70 6c6f 742e 6c79 223e  ttps://plot.ly">
+00005320: 4c69 6e6b 3c2f 613e 0a20 203c 2f64 6574  Link</a>.  </det
+00005330: 6169 6c73 3e0a 2020 0a20 203c 6465 7461  ails>.  .  <deta
+00005340: 696c 733e 0a20 2020 203c 7375 6d6d 6172  ils>.    <summar
+00005350: 793e 0a20 2020 2020 203c 656d 3e22 4a6f  y>.      <em>"Jo
+00005360: 626c 6962 3a20 7275 6e6e 696e 6720 7079  blib: running py
+00005370: 7468 6f6e 2066 756e 6374 696f 6e20 6173  thon function as
+00005380: 2070 6970 656c 696e 6520 6a6f 6273 2220   pipeline jobs" 
+00005390: 2847 2e20 5661 726f 7175 6175 7820 616e  (G. Varoquaux an
+000053a0: 6420 4f2e 2047 7269 7365 6c20 3230 3039  d O. Grisel 2009
+000053b0: 293c 2f65 6d3e 0a20 2020 203c 2f73 756d  )</em>.    </sum
+000053c0: 6d61 7279 3e0a 2020 2020 3c62 722f 3e0a  mary>.    <br/>.
+000053d0: 2020 2020 3c70 7265 3e0a 4061 7274 6963      <pre>.@artic
+000053e0: 6c65 7b76 6172 6f71 7561 7578 3230 3039  le{varoquaux2009
+000053f0: 6a6f 626c 6962 2c0a 2020 7469 746c 653d  joblib,.  title=
+00005400: 7b4a 6f62 6c69 623a 2072 756e 6e69 6e67  {Joblib: running
+00005410: 2070 7974 686f 6e20 6675 6e63 7469 6f6e   python function
+00005420: 2061 7320 7069 7065 6c69 6e65 206a 6f62   as pipeline job
+00005430: 737d 2c0a 2020 6175 7468 6f72 3d7b 5661  s},.  author={Va
+00005440: 726f 7175 6175 782c 2047 617b 5c22 657d  roquaux, Ga{\"e}
+00005450: 6c20 616e 6420 4772 6973 656c 2c20 4f7d  l and Grisel, O}
+00005460: 2c0a 2020 6a6f 7572 6e61 6c3d 7b70 6163  ,.  journal={pac
+00005470: 6b61 6765 732e 2070 7974 686f 6e2e 206f  kages. python. o
+00005480: 7267 2f6a 6f62 6c69 627d 2c0a 2020 7965  rg/joblib},.  ye
+00005490: 6172 3d7b 3230 3039 7d0a 7d0a 2020 2020  ar={2009}.}.    
+000054a0: 3c2f 7072 653e 0a20 2020 203c 6120 6872  </pre>.    <a hr
+000054b0: 6566 3d22 6874 7470 733a 2f2f 6a6f 626c  ef="https://jobl
+000054c0: 6962 2e72 6561 6474 6865 646f 6373 2e69  ib.readthedocs.i
+000054d0: 6f2f 656e 2f6c 6174 6573 742f 223e 4c69  o/en/latest/">Li
+000054e0: 6e6b 3c2f 613e 0a20 203c 2f64 6574 6169  nk</a>.  </detai
+000054f0: 6c73 3e0a 2020 0a20 203c 6872 2f3e 0a3c  ls>.  .  <hr/>.<
+00005500: 2f64 6574 6169 6c73 3e0a 0a23 2056 6964  /details>..# Vid
+00005510: 656f 730a 0a2d 205b 5468 6520 5363 6965  eos..- [The Scie
+00005520: 6e63 6520 4265 6869 6e64 2049 6e74 6572  nce Behind Inter
+00005530: 7072 6574 4d4c 3a20 4578 706c 6169 6e61  pretML: Explaina
+00005540: 626c 6520 426f 6f73 7469 6e67 204d 6163  ble Boosting Mac
+00005550: 6869 6e65 5d28 6874 7470 733a 2f2f 7777  hine](https://ww
+00005560: 772e 796f 7574 7562 652e 636f 6d2f 7761  w.youtube.com/wa
+00005570: 7463 683f 763d 4d52 4569 4867 4867 6c30  tch?v=MREiHgHgl0
+00005580: 6b29 0a2d 205b 486f 7720 746f 2045 7870  k).- [How to Exp
+00005590: 6c61 696e 204d 6f64 656c 7320 7769 7468  lain Models with
+000055a0: 2049 6e74 6572 7072 6574 4d4c 2044 6565   InterpretML Dee
+000055b0: 7020 4469 7665 5d28 6874 7470 733a 2f2f  p Dive](https://
+000055c0: 7777 772e 796f 7574 7562 652e 636f 6d2f  www.youtube.com/
+000055d0: 7761 7463 683f 763d 5777 4265 4b4d 5130  watch?v=WwBeKMQ0
+000055e0: 2d49 3829 0a2d 205b 426c 6163 6b2d 426f  -I8).- [Black-Bo
+000055f0: 7820 616e 6420 476c 6173 732d 426f 7820  x and Glass-Box 
+00005600: 4578 706c 616e 6174 696f 6e20 696e 204d  Explanation in M
+00005610: 6163 6869 6e65 204c 6561 726e 696e 675d  achine Learning]
+00005620: 2868 7474 7073 3a2f 2f79 6f75 7475 2e62  (https://youtu.b
+00005630: 652f 3775 7a4e 4b59 3870 4568 5129 0a2d  e/7uzNKY8pEhQ).-
+00005640: 205b 4578 706c 6169 6e61 626c 6520 4149   [Explainable AI
+00005650: 2065 7870 6c61 696e 6564 2120 2042 792d   explained!  By-
+00005660: 6465 7369 676e 2069 6e74 6572 7072 6574  design interpret
+00005670: 6162 6c65 206d 6f64 656c 7320 7769 7468  able models with
+00005680: 204d 6963 726f 736f 6674 7320 496e 7465   Microsofts Inte
+00005690: 7270 7265 744d 4c5d 2868 7474 7073 3a2f  rpretML](https:/
+000056a0: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
+000056b0: 2f77 6174 6368 3f76 3d71 506e 396d 3330  /watch?v=qPn9m30
+000056c0: 6f6a 6663 290a 2d20 5b49 6e74 6572 7072  ojfc).- [Interpr
+000056d0: 6574 696e 6720 4d61 6368 696e 6520 4c65  eting Machine Le
+000056e0: 6172 6e69 6e67 204d 6f64 656c 7320 7769  arning Models wi
+000056f0: 7468 2049 6e74 6572 7072 6574 4d4c 5d28  th InterpretML](
+00005700: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
+00005710: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
+00005720: 4552 4e75 4666 736b 6e68 6b29 0a0a 2320  ERNuFfsknhk)..# 
+00005730: 4578 7465 726e 616c 206c 696e 6b73 0a0a  External links..
+00005740: 2d20 5b49 6e74 6572 7072 6574 6162 6c65  - [Interpretable
+00005750: 206f 7220 4163 6375 7261 7465 3f20 5768   or Accurate? Wh
+00005760: 7920 4e6f 7420 426f 7468 3f5d 2868 7474  y Not Both?](htt
+00005770: 7073 3a2f 2f74 6f77 6172 6473 6461 7461  ps://towardsdata
+00005780: 7363 6965 6e63 652e 636f 6d2f 696e 7465  science.com/inte
+00005790: 7270 7265 7461 626c 652d 6f72 2d61 6363  rpretable-or-acc
+000057a0: 7572 6174 652d 7768 792d 6e6f 742d 626f  urate-why-not-bo
+000057b0: 7468 2d34 6439 6337 3335 3132 3139 3229  th-4d9c73512192)
+000057c0: 0a2d 205b 5468 6520 4578 706c 6169 6e61  .- [The Explaina
+000057d0: 626c 6520 426f 6f73 7469 6e67 204d 6163  ble Boosting Mac
+000057e0: 6869 6e65 2e20 4173 2061 6363 7572 6174  hine. As accurat
+000057f0: 6520 6173 2067 7261 6469 656e 7420 626f  e as gradient bo
+00005800: 6f73 7469 6e67 2c20 6173 2069 6e74 6572  osting, as inter
+00005810: 7072 6574 6162 6c65 2061 7320 6c69 6e65  pretable as line
+00005820: 6172 2072 6567 7265 7373 696f 6e2e 5d28  ar regression.](
+00005830: 6874 7470 733a 2f2f 746f 7761 7264 7364  https://towardsd
+00005840: 6174 6173 6369 656e 6365 2e63 6f6d 2f74  atascience.com/t
+00005850: 6865 2d65 7870 6c61 696e 6162 6c65 2d62  he-explainable-b
+00005860: 6f6f 7374 696e 672d 6d61 6368 696e 652d  oosting-machine-
+00005870: 6632 3431 3532 3530 3965 6262 290a 2d20  f24152509ebb).- 
+00005880: 5b50 6572 666f 726d 616e 6365 2041 6e64  [Performance And
+00005890: 2045 7870 6c61 696e 6162 696c 6974 7920   Explainability 
+000058a0: 5769 7468 2045 424d 5d28 6874 7470 733a  With EBM](https:
+000058b0: 2f2f 626c 6f67 2e6f 616b 6269 7473 2e63  //blog.oakbits.c
+000058c0: 6f6d 2f65 626d 2d61 6c67 6f72 6974 686d  om/ebm-algorithm
+000058d0: 2e68 746d 6c29 0a2d 205b 496e 7465 7270  .html).- [Interp
+000058e0: 7265 744d 4c3a 2041 6e6f 7468 6572 2057  retML: Another W
+000058f0: 6179 2074 6f20 4578 706c 6169 6e20 596f  ay to Explain Yo
+00005900: 7572 204d 6f64 656c 5d28 6874 7470 733a  ur Model](https:
+00005910: 2f2f 746f 7761 7264 7364 6174 6173 6369  //towardsdatasci
+00005920: 656e 6365 2e63 6f6d 2f69 6e74 6572 7072  ence.com/interpr
+00005930: 6574 6d6c 2d61 6e6f 7468 6572 2d77 6179  etml-another-way
+00005940: 2d74 6f2d 6578 706c 6169 6e2d 796f 7572  -to-explain-your
+00005950: 2d6d 6f64 656c 2d62 3766 6166 3061 3338  -model-b7faf0a38
+00005960: 3466 3829 0a2d 205b 4120 6765 6e74 6c65  4f8).- [A gentle
+00005970: 2069 6e74 726f 6475 6374 696f 6e20 746f   introduction to
+00005980: 2047 4132 4d73 2c20 6120 7768 6974 6520   GA2Ms, a white 
+00005990: 626f 7820 6d6f 6465 6c5d 2868 7474 7073  box model](https
+000059a0: 3a2f 2f77 7777 2e66 6964 646c 6572 2e61  ://www.fiddler.a
+000059b0: 692f 626c 6f67 2f61 2d67 656e 746c 652d  i/blog/a-gentle-
+000059c0: 696e 7472 6f64 7563 7469 6f6e 2d74 6f2d  introduction-to-
+000059d0: 6761 326d 732d 612d 7768 6974 652d 626f  ga2ms-a-white-bo
+000059e0: 782d 6d6f 6465 6c29 0a2d 205b 4d6f 6465  x-model).- [Mode
+000059f0: 6c20 496e 7465 7270 7265 7461 7469 6f6e  l Interpretation
+00005a00: 2077 6974 6820 4d69 6372 6f73 6f66 74e2   with Microsoft.
+00005a10: 8099 7320 496e 7465 7270 7265 7420 4d4c  ..s Interpret ML
+00005a20: 5d28 6874 7470 733a 2f2f 6d65 6469 756d  ](https://medium
+00005a30: 2e63 6f6d 2f40 7361 6e64 2e6d 6179 7572  .com/@sand.mayur
+00005a40: 2f6d 6f64 656c 2d69 6e74 6572 7072 6574  /model-interpret
+00005a50: 6174 696f 6e2d 7769 7468 2d6d 6963 726f  ation-with-micro
+00005a60: 736f 6674 732d 696e 7465 7270 7265 742d  softs-interpret-
+00005a70: 6d6c 2d38 3561 6130 6164 3639 3761 6529  ml-85aa0ad697ae)
+00005a80: 0a2d 205b 4578 706c 6169 6e69 6e67 204d  .- [Explaining M
+00005a90: 6f64 656c 2050 6970 656c 696e 6573 2057  odel Pipelines W
+00005aa0: 6974 6820 496e 7465 7270 7265 744d 4c5d  ith InterpretML]
+00005ab0: 2868 7474 7073 3a2f 2f6d 6564 6975 6d2e  (https://medium.
+00005ac0: 636f 6d2f 406d 6172 6975 7376 6164 6569  com/@mariusvadei
+00005ad0: 6b61 2f65 7870 6c61 696e 696e 672d 6d6f  ka/explaining-mo
+00005ae0: 6465 6c2d 7069 7065 6c69 6e65 732d 7769  del-pipelines-wi
+00005af0: 7468 2d69 6e74 6572 7072 6574 6d6c 2d61  th-interpretml-a
+00005b00: 3932 3134 6637 3534 3030 6229 0a2d 205b  9214f75400b).- [
+00005b10: 4578 706c 6169 6e20 596f 7572 204d 6f64  Explain Your Mod
+00005b20: 656c 2077 6974 6820 4d69 6372 6f73 6f66  el with Microsof
+00005b30: 74e2 8099 7320 496e 7465 7270 7265 744d  t...s InterpretM
+00005b40: 4c5d 2868 7474 7073 3a2f 2f6d 6564 6975  L](https://mediu
+00005b50: 6d2e 636f 6d2f 4044 6174 616d 616e 2e61  m.com/@Dataman.a
+00005b60: 692f 6578 706c 6169 6e2d 796f 7572 2d6d  i/explain-your-m
+00005b70: 6f64 656c 2d77 6974 682d 6d69 6372 6f73  odel-with-micros
+00005b80: 6f66 7473 2d69 6e74 6572 7072 6574 6d6c  ofts-interpretml
+00005b90: 2d35 6461 6162 3164 3639 3362 3429 0a2d  -5daab1d693b4).-
+00005ba0: 205b 4f6e 204d 6f64 656c 2045 7870 6c61   [On Model Expla
+00005bb0: 696e 6162 696c 6974 793a 2046 726f 6d20  inability: From 
+00005bc0: 4c49 4d45 2c20 5348 4150 2c20 746f 2045  LIME, SHAP, to E
+00005bd0: 7870 6c61 696e 6162 6c65 2042 6f6f 7374  xplainable Boost
+00005be0: 696e 675d 2868 7474 7073 3a2f 2f65 7665  ing](https://eve
+00005bf0: 7264 6172 6b2e 6769 7468 7562 2e69 6f2f  rdark.github.io/
+00005c00: 6b39 2f6e 6f74 6562 6f6f 6b73 2f6d 6c2f  k9/notebooks/ml/
+00005c10: 6d6f 6465 6c5f 6578 706c 6169 6e2f 6d6f  model_explain/mo
+00005c20: 6465 6c5f 6578 706c 6169 6e2e 6e62 2e68  del_explain.nb.h
+00005c30: 746d 6c29 0a2d 205b 4465 616c 696e 6720  tml).- [Dealing 
+00005c40: 7769 7468 2049 6d62 616c 616e 6365 6420  with Imbalanced 
+00005c50: 4461 7461 2028 4d6f 7274 6761 6765 206c  Data (Mortgage l
+00005c60: 6f61 6e73 2064 6566 6175 6c74 7329 5d28  oans defaults)](
+00005c70: 6874 7470 733a 2f2f 6d69 6b65 776c 616e  https://mikewlan
+00005c80: 6765 2e67 6974 6875 622e 696f 2f49 6d62  ge.github.io/Imb
+00005c90: 616c 616e 6365 6444 6174 612d 2f69 6e64  alancedData-/ind
+00005ca0: 6578 2e68 746d 6c29 0a2d 205b 5468 6520  ex.html).- [The 
+00005cb0: 7269 6768 7420 7761 7920 746f 2063 6f6d  right way to com
+00005cc0: 7075 7465 2079 6f75 7220 5368 6170 6c65  pute your Shaple
+00005cd0: 7920 5661 6c75 6573 5d28 6874 7470 733a  y Values](https:
+00005ce0: 2f2f 746f 7761 7264 7364 6174 6173 6369  //towardsdatasci
+00005cf0: 656e 6365 2e63 6f6d 2f74 6865 2d72 6967  ence.com/the-rig
+00005d00: 6874 2d77 6179 2d74 6f2d 636f 6d70 7574  ht-way-to-comput
+00005d10: 652d 796f 7572 2d73 6861 706c 6579 2d76  e-your-shapley-v
+00005d20: 616c 7565 732d 6366 6561 3330 3530 3932  alues-cfea305092
+00005d30: 3534 290a 2d20 5b54 6865 2041 7274 206f  54).- [The Art o
+00005d40: 6620 5370 7265 7a7a 6174 7572 6120 666f  f Sprezzatura fo
+00005d50: 7220 4d61 6368 696e 6520 4c65 6172 6e69  r Machine Learni
+00005d60: 6e67 5d28 6874 7470 733a 2f2f 746f 7761  ng](https://towa
+00005d70: 7264 7364 6174 6173 6369 656e 6365 2e63  rdsdatascience.c
+00005d80: 6f6d 2f74 6865 2d61 7274 2d6f 662d 7370  om/the-art-of-sp
+00005d90: 7265 7a7a 6174 7572 612d 666f 722d 6d61  rezzatura-for-ma
+00005da0: 6368 696e 652d 6c65 6172 6e69 6e67 2d65  chine-learning-e
+00005db0: 3234 3934 6330 6462 3732 3729 0a2d 205b  2494c0db727).- [
+00005dc0: 4d69 7869 6e67 2041 7274 2069 6e74 6f20  Mixing Art into 
+00005dd0: 7468 6520 5363 6965 6e63 6520 6f66 204d  the Science of M
+00005de0: 6f64 656c 2045 7870 6c61 696e 6162 696c  odel Explainabil
+00005df0: 6974 795d 2868 7474 7073 3a2f 2f74 6f77  ity](https://tow
+00005e00: 6172 6473 6461 7461 7363 6965 6e63 652e  ardsdatascience.
+00005e10: 636f 6d2f 6d69 7869 6e67 2d61 7274 2d69  com/mixing-art-i
+00005e20: 6e74 6f2d 7468 652d 7363 6965 6e63 652d  nto-the-science-
+00005e30: 6f66 2d6d 6f64 656c 2d65 7870 6c61 696e  of-model-explain
+00005e40: 6162 696c 6974 792d 3331 3262 3832 3136  ability-312b8216
+00005e50: 6661 3935 290a 0a23 2050 6170 6572 7320  fa95)..# Papers 
+00005e60: 7468 6174 2075 7365 206f 7220 636f 6d70  that use or comp
+00005e70: 6172 6520 4542 4d73 0a0a 2d20 5b4d 6f64  are EBMs..- [Mod
+00005e80: 656c 2049 6e74 6572 7072 6574 6162 696c  el Interpretabil
+00005e90: 6974 7920 696e 2043 7265 6469 7420 496e  ity in Credit In
+00005ea0: 7375 7261 6e63 655d 2868 7474 703a 2f2f  surance](http://
+00005eb0: 6864 6c2e 6861 6e64 6c65 2e6e 6574 2f31  hdl.handle.net/1
+00005ec0: 3034 3030 2e35 2f32 3735 3037 290a 2d20  0400.5/27507).- 
+00005ed0: 5b46 6564 6572 6174 6564 2042 6f6f 7374  [Federated Boost
+00005ee0: 6564 2044 6563 6973 696f 6e20 5472 6565  ed Decision Tree
+00005ef0: 7320 7769 7468 2044 6966 6665 7265 6e74  s with Different
+00005f00: 6961 6c20 5072 6976 6163 795d 2868 7474  ial Privacy](htt
+00005f10: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f70  ps://arxiv.org/p
+00005f20: 6466 2f32 3231 302e 3032 3931 302e 7064  df/2210.02910.pd
+00005f30: 6629 0a2d 205b 4741 4d28 4529 2043 4841  f).- [GAM(E) CHA
+00005f40: 4e47 4552 204f 5220 4e4f 543f 2041 4e20  NGER OR NOT? AN 
+00005f50: 4556 414c 5541 5449 4f4e 204f 4620 494e  EVALUATION OF IN
+00005f60: 5445 5250 5245 5441 424c 4520 4d41 4348  TERPRETABLE MACH
+00005f70: 494e 4520 4c45 4152 4e49 4e47 204d 4f44  INE LEARNING MOD
+00005f80: 454c 535d 2868 7474 7073 3a2f 2f61 7278  ELS](https://arx
+00005f90: 6976 2e6f 7267 2f70 6466 2f32 3230 342e  iv.org/pdf/2204.
+00005fa0: 3039 3132 332e 7064 6629 0a2d 205b 4741  09123.pdf).- [GA
+00005fb0: 4d20 436f 6163 683a 2054 6f77 6172 6473  M Coach: Towards
+00005fc0: 2049 6e74 6572 6163 7469 7665 2061 6e64   Interactive and
+00005fd0: 2055 7365 722d 6365 6e74 6572 6564 2041   User-centered A
+00005fe0: 6c67 6f72 6974 686d 6963 2052 6563 6f75  lgorithmic Recou
+00005ff0: 7273 655d 2868 7474 7073 3a2f 2f61 7278  rse](https://arx
+00006000: 6976 2e6f 7267 2f70 6466 2f32 3330 322e  iv.org/pdf/2302.
+00006010: 3134 3136 352e 7064 6629 0a2d 205b 4d69  14165.pdf).- [Mi
+00006020: 7373 696e 6720 5661 6c75 6573 2061 6e64  ssing Values and
+00006030: 2049 6d70 7574 6174 696f 6e20 696e 2048   Imputation in H
+00006040: 6561 6c74 6863 6172 6520 4461 7461 3a20  ealthcare Data: 
+00006050: 4361 6e20 496e 7465 7270 7265 7461 626c  Can Interpretabl
+00006060: 6520 4d61 6368 696e 6520 4c65 6172 6e69  e Machine Learni
+00006070: 6e67 2048 656c 703f 5d28 6874 7470 733a  ng Help?](https:
+00006080: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
+00006090: 3233 3034 2e31 3137 3439 7631 2e70 6466  2304.11749v1.pdf
+000060a0: 290a 2d20 5b50 7261 6374 6963 6520 616e  ).- [Practice an
+000060b0: 6420 4368 616c 6c65 6e67 6573 2069 6e20  d Challenges in 
+000060c0: 4275 696c 6469 6e67 2061 2055 6e69 7665  Building a Unive
+000060d0: 7273 616c 2053 6561 7263 6820 5175 616c  rsal Search Qual
+000060e0: 6974 7920 4d65 7472 6963 5d28 6874 7470  ity Metric](http
+000060f0: 733a 2f2f 7777 772e 7265 7365 6172 6368  s://www.research
+00006100: 6761 7465 2e6e 6574 2f70 726f 6669 6c65  gate.net/profile
+00006110: 2f4e 756f 2d43 6865 6e2d 3338 2f70 7562  /Nuo-Chen-38/pub
+00006120: 6c69 6361 7469 6f6e 2f33 3730 3132 3637  lication/3701267
+00006130: 3230 5f50 7261 6374 6963 655f 616e 645f  20_Practice_and_
+00006140: 4368 616c 6c65 6e67 6573 5f69 6e5f 4275  Challenges_in_Bu
+00006150: 696c 6469 6e67 5f61 5f55 6e69 7665 7273  ilding_a_Univers
+00006160: 616c 5f53 6561 7263 685f 5175 616c 6974  al_Search_Qualit
+00006170: 795f 4d65 7472 6963 2f6c 696e 6b73 2f36  y_Metric/links/6
+00006180: 3434 3061 3066 3233 3961 6134 3731 6135  440a0f239aa471a5
+00006190: 3234 6362 3737 642f 5072 6163 7469 6365  24cb77d/Practice
+000061a0: 2d61 6e64 2d43 6861 6c6c 656e 6765 732d  -and-Challenges-
+000061b0: 696e 2d42 7569 6c64 696e 672d 612d 556e  in-Building-a-Un
+000061c0: 6976 6572 7361 6c2d 5365 6172 6368 2d51  iversal-Search-Q
+000061d0: 7561 6c69 7479 2d4d 6574 7269 632e 7064  uality-Metric.pd
+000061e0: 663f 6f72 6967 696e 3d70 7562 6c69 6361  f?origin=publica
+000061f0: 7469 6f6e 5f64 6574 6169 6c29 0a2d 205b  tion_detail).- [
+00006200: 4578 706c 6169 6e69 6e67 2050 6869 7368  Explaining Phish
+00006210: 696e 6720 4174 7461 636b 733a 2041 6e20  ing Attacks: An 
+00006220: 5841 4920 4170 7072 6f61 6368 2074 6f20  XAI Approach to 
+00006230: 456e 6861 6e63 6520 5573 6572 2041 7761  Enhance User Awa
+00006240: 7265 6e65 7373 2061 6e64 2054 7275 7374  reness and Trust
+00006250: 5d28 6874 7470 733a 2f2f 7777 772e 7265  ](https://www.re
+00006260: 7365 6172 6368 6761 7465 2e6e 6574 2f70  searchgate.net/p
+00006270: 726f 6669 6c65 2f47 6975 7365 7070 652d  rofile/Giuseppe-
+00006280: 4465 736f 6c64 612f 7075 626c 6963 6174  Desolda/publicat
+00006290: 696f 6e2f 3337 3030 3033 3837 385f 4578  ion/370003878_Ex
+000062a0: 706c 6169 6e69 6e67 5f50 6869 7368 696e  plaining_Phishin
+000062b0: 675f 4174 7461 636b 735f 416e 5f58 4149  g_Attacks_An_XAI
+000062c0: 5f41 7070 726f 6163 685f 746f 5f45 6e68  _Approach_to_Enh
+000062d0: 616e 6365 5f55 7365 725f 4177 6172 656e  ance_User_Awaren
+000062e0: 6573 735f 616e 645f 5472 7573 742f 6c69  ess_and_Trust/li
+000062f0: 6e6b 732f 3634 3339 3232 6138 6538 3831  nks/643922a8e881
+00006300: 3639 3063 3462 6435 3063 6564 2f45 7870  690c4bd50ced/Exp
+00006310: 6c61 696e 696e 672d 5068 6973 6869 6e67  laining-Phishing
+00006320: 2d41 7474 6163 6b73 2d41 6e2d 5841 492d  -Attacks-An-XAI-
+00006330: 4170 7072 6f61 6368 2d74 6f2d 456e 6861  Approach-to-Enha
+00006340: 6e63 652d 5573 6572 2d41 7761 7265 6e65  nce-User-Awarene
+00006350: 7373 2d61 6e64 2d54 7275 7374 2e70 6466  ss-and-Trust.pdf
+00006360: 290a 2d20 5b52 6576 6561 6c69 6e67 2074  ).- [Revealing t
+00006370: 6865 2047 616c 6178 792d 4861 6c6f 2043  he Galaxy-Halo C
+00006380: 6f6e 6e65 6374 696f 6e20 5468 726f 7567  onnection Throug
+00006390: 6820 4d61 6368 696e 6520 4c65 6172 6e69  h Machine Learni
+000063a0: 6e67 5d28 6874 7470 733a 2f2f 6172 7869  ng](https://arxi
+000063b0: 762e 6f72 672f 7064 662f 3232 3034 2e31  v.org/pdf/2204.1
+000063c0: 3033 3332 2e70 6466 290a 2d20 5b45 7870  0332.pdf).- [Exp
+000063d0: 6c61 696e 6162 6c65 2041 7274 6966 6963  lainable Artific
+000063e0: 6961 6c20 496e 7465 6c6c 6967 656e 6365  ial Intelligence
+000063f0: 2066 6f72 2043 4f56 4944 2d31 3920 4469   for COVID-19 Di
+00006400: 6167 6e6f 7369 7320 5468 726f 7567 6820  agnosis Through 
+00006410: 426c 6f6f 6420 5465 7374 2056 6172 6961  Blood Test Varia
+00006420: 626c 6573 5d28 6874 7470 733a 2f2f 6c69  bles](https://li
+00006430: 6e6b 2e73 7072 696e 6765 722e 636f 6d2f  nk.springer.com/
+00006440: 636f 6e74 656e 742f 7064 662f 3130 2e31  content/pdf/10.1
+00006450: 3030 372f 7334 3033 3133 2d30 3231 2d30  007/s40313-021-0
+00006460: 3038 3538 2d79 2e70 6466 290a 2d20 5b55  0858-y.pdf).- [U
+00006470: 7369 6e67 2045 7870 6c61 696e 6162 6c65  sing Explainable
+00006480: 2042 6f6f 7374 696e 6720 4d61 6368 696e   Boosting Machin
+00006490: 6573 2028 4542 4d73 2920 746f 2044 6574  es (EBMs) to Det
+000064a0: 6563 7420 436f 6d6d 6f6e 2046 6c61 7773  ect Common Flaws
+000064b0: 2069 6e20 4461 7461 5d28 6874 7470 733a   in Data](https:
+000064c0: 2f2f 6c69 6e6b 2e73 7072 696e 6765 722e  //link.springer.
+000064d0: 636f 6d2f 6368 6170 7465 722f 3130 2e31  com/chapter/10.1
+000064e0: 3030 372f 3937 382d 332d 3033 302d 3933  007/978-3-030-93
+000064f0: 3733 362d 325f 3430 290a 2d20 5b44 6966  736-2_40).- [Dif
+00006500: 6665 7265 6e74 6961 6c6c 7920 5072 6976  ferentially Priv
+00006510: 6174 6520 4772 6164 6965 6e74 2042 6f6f  ate Gradient Boo
+00006520: 7374 696e 6720 6f6e 204c 696e 6561 7220  sting on Linear 
+00006530: 4c65 6172 6e65 7273 2066 6f72 2054 6162  Learners for Tab
+00006540: 756c 6172 2044 6174 6120 416e 616c 7973  ular Data Analys
+00006550: 6973 5d28 6874 7470 733a 2f2f 6173 7365  is](https://asse
+00006560: 7473 2e61 6d61 7a6f 6e2e 7363 6965 6e63  ts.amazon.scienc
+00006570: 652f 6661 2f33 612f 6136 3262 6137 3366  e/fa/3a/a62ba73f
+00006580: 3462 6264 6131 6438 3830 6236 3738 6333  4bbda1d880b678c3
+00006590: 3931 3933 2f64 6966 6665 7265 6e74 6961  9193/differentia
+000065a0: 6c6c 792d 7072 6976 6174 652d 6772 6164  lly-private-grad
+000065b0: 6965 6e74 2d62 6f6f 7374 696e 672d 6f6e  ient-boosting-on
+000065c0: 2d6c 696e 6561 722d 6c65 6172 6e65 7273  -linear-learners
+000065d0: 2d66 6f72 2d74 6162 756c 6172 2d64 6174  -for-tabular-dat
+000065e0: 612d 616e 616c 7973 6973 2e70 6466 290a  a-analysis.pdf).
+000065f0: 2d20 5b43 6f6e 6372 6574 6520 636f 6d70  - [Concrete comp
+00006600: 7265 7373 6976 6520 7374 7265 6e67 7468  ressive strength
+00006610: 2070 7265 6469 6374 696f 6e20 7573 696e   prediction usin
+00006620: 6720 616e 2065 7870 6c61 696e 6162 6c65  g an explainable
+00006630: 2062 6f6f 7374 696e 6720 6d61 6368 696e   boosting machin
+00006640: 6520 6d6f 6465 6c5d 2868 7474 7073 3a2f  e model](https:/
+00006650: 2f77 7777 2e73 6369 656e 6365 6469 7265  /www.sciencedire
+00006660: 6374 2e63 6f6d 2f73 6369 656e 6365 2f61  ct.com/science/a
+00006670: 7274 6963 6c65 2f70 6969 2f53 3232 3134  rticle/pii/S2214
+00006680: 3530 3935 3233 3030 3032 3434 2f70 6466  509523000244/pdf
+00006690: 6674 3f6d 6435 3d31 3731 6332 3735 6236  ft?md5=171c275b6
+000066a0: 6263 6165 3838 3937 6365 6630 3364 3933  bcae8897cef03d93
+000066b0: 3165 3930 3865 3226 7069 643d 312d 7332  1e908e2&pid=1-s2
+000066c0: 2e30 2d53 3232 3134 3530 3935 3233 3030  .0-S221450952300
+000066d0: 3032 3434 2d6d 6169 6e2e 7064 6629 0a2d  0244-main.pdf).-
+000066e0: 205b 4573 7469 6d61 7465 2044 6566 6f72   [Estimate Defor
+000066f0: 6d61 7469 6f6e 2043 6170 6163 6974 7920  mation Capacity 
+00006700: 6f66 204e 6f6e 2d44 7563 7469 6c65 2052  of Non-Ductile R
+00006710: 4320 5368 6561 7220 5761 6c6c 7320 5573  C Shear Walls Us
+00006720: 696e 6720 4578 706c 6169 6e61 626c 6520  ing Explainable 
+00006730: 426f 6f73 7469 6e67 204d 6163 6869 6e65  Boosting Machine
+00006740: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
+00006750: 6f72 672f 7064 662f 3233 3031 2e30 3436  org/pdf/2301.046
+00006760: 3532 2e70 6466 290a 2d20 5b49 6e74 726f  52.pdf).- [Intro
+00006770: 6475 6369 6e67 2074 6865 2052 616e 6b2d  ducing the Rank-
+00006780: 4269 6173 6564 204f 7665 726c 6170 2061  Biased Overlap a
+00006790: 7320 5369 6d69 6c61 7269 7479 204d 6561  s Similarity Mea
+000067a0: 7375 7265 2066 6f72 2046 6561 7475 7265  sure for Feature
+000067b0: 2049 6d70 6f72 7461 6e63 6520 696e 2045   Importance in E
+000067c0: 7870 6c61 696e 6162 6c65 204d 6163 6869  xplainable Machi
+000067d0: 6e65 204c 6561 726e 696e 673a 2041 2043  ne Learning: A C
+000067e0: 6173 6520 5374 7564 7920 6f6e 2050 6172  ase Study on Par
+000067f0: 6b69 6e73 6f6e e280 9973 2044 6973 6561  kinson...s Disea
+00006800: 7365 5d28 6874 7470 733a 2f2f 6c69 6e6b  se](https://link
+00006810: 2e73 7072 696e 6765 722e 636f 6d2f 6368  .springer.com/ch
+00006820: 6170 7465 722f 3130 2e31 3030 372f 3937  apter/10.1007/97
+00006830: 382d 332d 3033 312d 3135 3033 372d 315f  8-3-031-15037-1_
+00006840: 3131 290a 2d20 5b54 6172 6765 7469 6e67  11).- [Targeting
+00006850: 2072 6573 6f75 7263 6573 2065 6666 6963   resources effic
+00006860: 6965 6e74 6c79 2061 6e64 206a 7573 7469  iently and justi
+00006870: 6669 6162 6c79 2062 7920 636f 6d62 696e  fiably by combin
+00006880: 696e 6720 6361 7573 616c 206d 6163 6869  ing causal machi
+00006890: 6e65 206c 6561 726e 696e 6720 616e 6420  ne learning and 
+000068a0: 7468 656f 7279 5d28 6874 7470 733a 2f2f  theory](https://
+000068b0: 7777 772e 6e63 6269 2e6e 6c6d 2e6e 6968  www.ncbi.nlm.nih
+000068c0: 2e67 6f76 2f70 6d63 2f61 7274 6963 6c65  .gov/pmc/article
+000068d0: 732f 504d 4339 3736 3831 3831 2f70 6466  s/PMC9768181/pdf
+000068e0: 2f66 7261 692d 3035 2d31 3031 3536 3034  /frai-05-1015604
+000068f0: 2e70 6466 290a 2d20 5b45 7874 7261 6374  .pdf).- [Extract
+00006900: 6976 6520 5465 7874 2053 756d 6d61 7269  ive Text Summari
+00006910: 7a61 7469 6f6e 2055 7369 6e67 2047 656e  zation Using Gen
+00006920: 6572 616c 697a 6564 2041 6464 6974 6976  eralized Additiv
+00006930: 6520 4d6f 6465 6c73 2077 6974 6820 496e  e Models with In
+00006940: 7465 7261 6374 696f 6e73 2066 6f72 2053  teractions for S
+00006950: 656e 7465 6e63 6520 5365 6c65 6374 696f  entence Selectio
+00006960: 6e5d 2868 7474 7073 3a2f 2f61 7278 6976  n](https://arxiv
+00006970: 2e6f 7267 2f70 6466 2f32 3231 322e 3130  .org/pdf/2212.10
+00006980: 3730 372e 7064 6629 0a2d 205b 4465 6174  707.pdf).- [Deat
+00006990: 6820 6279 2052 6f75 6e64 204e 756d 6265  h by Round Numbe
+000069a0: 7273 3a20 476c 6173 732d 426f 7820 4d61  rs: Glass-Box Ma
+000069b0: 6368 696e 6520 4c65 6172 6e69 6e67 2055  chine Learning U
+000069c0: 6e63 6f76 6572 7320 4269 6173 6573 2069  ncovers Biases i
+000069d0: 6e20 4d65 6469 6361 6c20 5072 6163 7469  n Medical Practi
+000069e0: 6365 5d28 6874 7470 733a 2f2f 7777 772e  ce](https://www.
+000069f0: 6d65 6472 7869 762e 6f72 672f 636f 6e74  medrxiv.org/cont
+00006a00: 656e 742f 6d65 6472 7869 762f 6561 726c  ent/medrxiv/earl
+00006a10: 792f 3230 3232 2f31 312f 3238 2f32 3032  y/2022/11/28/202
+00006a20: 322e 3034 2e33 302e 3232 3237 3435 3230  2.04.30.22274520
+00006a30: 2e66 756c 6c2e 7064 6629 0a2d 205b 506f  .full.pdf).- [Po
+00006a40: 7374 2d48 6f63 2049 6e74 6572 7072 6574  st-Hoc Interpret
+00006a50: 6174 696f 6e20 6f66 2054 7261 6e73 666f  ation of Transfo
+00006a60: 726d 6572 2048 7970 6572 7061 7261 6d65  rmer Hyperparame
+00006a70: 7465 7273 2077 6974 6820 4578 706c 6169  ters with Explai
+00006a80: 6e61 626c 6520 426f 6f73 7469 6e67 204d  nable Boosting M
+00006a90: 6163 6869 6e65 735d 2868 7474 7073 3a2f  achines](https:/
+00006aa0: 2f77 7777 2e63 732e 6a68 752e 6564 752f  /www.cs.jhu.edu/
+00006ab0: 7e78 7a68 616e 3133 382f 7061 7065 7273  ~xzhan138/papers
+00006ac0: 2f42 4c41 434b 3230 3232 2e70 6466 290a  /BLACK2022.pdf).
+00006ad0: 2d20 5b49 6e74 6572 7072 6574 6162 6c65  - [Interpretable
+00006ae0: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
+00006af0: 6720 666f 7220 7072 6564 6963 7469 6e67  g for predicting
+00006b00: 2070 6174 686f 6c6f 6769 6320 636f 6d70   pathologic comp
+00006b10: 6c65 7465 2072 6573 706f 6e73 6520 696e  lete response in
+00006b20: 2070 6174 6965 6e74 7320 7472 6561 7465   patients treate
+00006b30: 6420 7769 7468 2063 6865 6d6f 7261 6469  d with chemoradi
+00006b40: 6174 696f 6e20 7468 6572 6170 7920 666f  ation therapy fo
+00006b50: 7220 7265 6374 616c 2061 6465 6e6f 6361  r rectal adenoca
+00006b60: 7263 696e 6f6d 615d 2868 7474 7073 3a2f  rcinoma](https:/
+00006b70: 2f77 7777 2e6e 6362 692e 6e6c 6d2e 6e69  /www.ncbi.nlm.ni
+00006b80: 682e 676f 762f 706d 632f 6172 7469 636c  h.gov/pmc/articl
+00006b90: 6573 2f50 4d43 3937 3731 3338 352f 7064  es/PMC9771385/pd
+00006ba0: 662f 6672 6169 2d30 352d 3130 3539 3033  f/frai-05-105903
+00006bb0: 332e 7064 6629 0a2d 205b 4578 706c 6f72  3.pdf).- [Explor
+00006bc0: 696e 6720 7468 6520 4261 6c61 6e63 6520  ing the Balance 
+00006bd0: 6265 7477 6565 6e20 496e 7465 7270 7265  between Interpre
+00006be0: 7461 6269 6c69 7479 2061 6e64 2050 6572  tability and Per
+00006bf0: 666f 726d 616e 6365 2077 6974 6820 6361  formance with ca
+00006c00: 7265 6675 6c6c 7920 6465 7369 676e 6564  refully designed
+00006c10: 2043 6f6e 7374 7261 696e 6162 6c65 204e   Constrainable N
+00006c20: 6575 7261 6c20 4164 6469 7469 7665 204d  eural Additive M
+00006c30: 6f64 656c 735d 2868 7474 7073 3a2f 2f64  odels](https://d
+00006c40: 656c 6976 6572 7970 6466 2e73 7372 6e2e  eliverypdf.ssrn.
+00006c50: 636f 6d2f 6465 6c69 7665 7279 2e70 6870  com/delivery.php
+00006c60: 3f49 443d 3939 3831 3035 3030 3630 3030  ?ID=998105006000
+00006c70: 3036 3931 3232 3037 3330 3938 3132 3031  0691220730981201
+00006c80: 3032 3130 3231 3231 3032 3130 3430 3035  0210212102104005
+00006c90: 3130 3138 3035 3530 3934 3132 3530 3239  1018055094125029
+00006ca0: 3132 3230 3131 3034 3130 3033 3035 3930  1220110410030590
+00006cb0: 3933 3132 3531 3032 3037 3231 3232 3130  9312510207212210
+00006cc0: 3631 3232 3037 3730 3831 3036 3930 3135  6122077081069015
+00006cd0: 3038 3731 3234 3032 3830 3937 3031 3630  0871240280970160
+00006ce0: 3033 3132 3730 3935 3038 3730 3931 3032  0312709508709102
+00006cf0: 3830 3837 3031 3030 3037 3033 3530 3938  8087010007035098
+00006d00: 3038 3631 3032 3038 3630 3831 3031 3430  0861020860810140
+00006d10: 3433 3031 3331 3133 3030 3430 3831 3131  4301311300408111
+00006d20: 3731 3038 3031 3130 3238 3034 3130 3937  7108011028041097
+00006d30: 3039 3530 3634 3037 3131 3030 3131 3230  0950640711001120
+00006d40: 3639 3038 3131 3030 3036 3931 3230 3037  6908110006912007
+00006d50: 3730 3637 3131 3630 3838 3130 3030 3639  7067116088100069
+00006d60: 3037 3030 3937 3039 3330 3830 3037 3430  0700970930800740
+00006d70: 3837 3131 3530 3830 3037 3230 3634 3038  8711508007206408
+00006d80: 3631 3131 3132 3626 4558 543d 7064 6626  6111126&EXT=pdf&
+00006d90: 494e 4445 583d 5452 5545 290a 2d20 5b45  INDEX=TRUE).- [E
+00006da0: 7374 696d 6174 696e 6720 4469 7363 6f6e  stimating Discon
+00006db0: 7469 6e75 6f75 7320 5469 6d65 2d56 6172  tinuous Time-Var
+00006dc0: 7969 6e67 2052 6973 6b20 4661 6374 6f72  ying Risk Factor
+00006dd0: 7320 616e 6420 5472 6561 746d 656e 7420  s and Treatment 
+00006de0: 4265 6e65 6669 7473 2066 6f72 2043 4f56  Benefits for COV
+00006df0: 4944 2d31 3920 7769 7468 2049 6e74 6572  ID-19 with Inter
+00006e00: 7072 6574 6162 6c65 204d 4c5d 2868 7474  pretable ML](htt
+00006e10: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f70  ps://arxiv.org/p
+00006e20: 6466 2f32 3231 312e 3038 3939 312e 7064  df/2211.08991.pd
+00006e30: 6629 0a2d 205b 5065 7374 2050 7265 7365  f).- [Pest Prese
+00006e40: 6e63 6520 5072 6564 6963 7469 6f6e 2055  nce Prediction U
+00006e50: 7369 6e67 2049 6e74 6572 7072 6574 6162  sing Interpretab
+00006e60: 6c65 204d 6163 6869 6e65 204c 6561 726e  le Machine Learn
+00006e70: 696e 675d 2868 7474 7073 3a2f 2f61 7278  ing](https://arx
+00006e80: 6976 2e6f 7267 2f70 6466 2f32 3230 352e  iv.org/pdf/2205.
+00006e90: 3037 3732 332e 7064 6629 0a2d 205b 6570  07723.pdf).- [ep
+00006ea0: 6974 6f70 6531 443a 2041 6363 7572 6174  itope1D: Accurat
+00006eb0: 6520 5461 786f 6e6f 6d79 2d41 7761 7265  e Taxonomy-Aware
+00006ec0: 2042 2d43 656c 6c20 4c69 6e65 6172 2045   B-Cell Linear E
+00006ed0: 7069 746f 7065 2050 7265 6469 6374 696f  pitope Predictio
+00006ee0: 6e5d 2868 7474 7073 3a2f 2f77 7777 2e62  n](https://www.b
+00006ef0: 696f 7278 6976 2e6f 7267 2f63 6f6e 7465  iorxiv.org/conte
+00006f00: 6e74 2f31 302e 3131 3031 2f32 3032 322e  nt/10.1101/2022.
+00006f10: 3130 2e31 372e 3531 3236 3133 7631 2e66  10.17.512613v1.f
+00006f20: 756c 6c2e 7064 6629 0a2d 205b 4578 706c  ull.pdf).- [Expl
+00006f30: 6169 6e61 626c 6520 426f 6f73 7469 6e67  ainable Boosting
+00006f40: 204d 6163 6869 6e65 7320 666f 7220 536c   Machines for Sl
+00006f50: 6f70 6520 4661 696c 7572 6520 5370 6174  ope Failure Spat
+00006f60: 6961 6c20 5072 6564 6963 7469 7665 204d  ial Predictive M
+00006f70: 6f64 656c 696e 675d 2868 7474 7073 3a2f  odeling](https:/
+00006f80: 2f77 7777 2e6d 6470 692e 636f 6d2f 3230  /www.mdpi.com/20
+00006f90: 3732 2d34 3239 322f 3133 2f32 342f 3439  72-4292/13/24/49
+00006fa0: 3931 2f68 746d 290a 2d20 5b4d 6963 726f  91/htm).- [Micro
+00006fb0: 6d6f 6465 6c73 2066 6f72 2045 6666 6963  models for Effic
+00006fc0: 6965 6e74 2c20 4578 706c 6169 6e61 626c  ient, Explainabl
+00006fd0: 652c 2061 6e64 2052 6575 7361 626c 6520  e, and Reusable 
+00006fe0: 5379 7374 656d 733a 2041 2043 6173 6520  Systems: A Case 
+00006ff0: 5374 7564 7920 6f6e 204d 656e 7461 6c20  Study on Mental 
+00007000: 4865 616c 7468 5d28 6874 7470 733a 2f2f  Health](https://
+00007010: 6172 7869 762e 6f72 672f 7064 662f 3231  arxiv.org/pdf/21
+00007020: 3039 2e31 3337 3730 2e70 6466 290a 2d20  09.13770.pdf).- 
+00007030: 5b49 6465 6e74 6966 7969 6e67 206d 6169  [Identifying mai
+00007040: 6e20 616e 6420 696e 7465 7261 6374 696f  n and interactio
+00007050: 6e20 6566 6665 6374 7320 6f66 2072 6973  n effects of ris
+00007060: 6b20 6661 6374 6f72 7320 746f 2070 7265  k factors to pre
+00007070: 6469 6374 2069 6e74 656e 7369 7665 2063  dict intensive c
+00007080: 6172 6520 6164 6d69 7373 696f 6e20 696e  are admission in
+00007090: 2070 6174 6965 6e74 7320 686f 7370 6974   patients hospit
+000070a0: 616c 697a 6564 2077 6974 6820 434f 5649  alized with COVI
+000070b0: 442d 3139 5d28 6874 7470 733a 2f2f 7777  D-19](https://ww
+000070c0: 772e 6d65 6472 7869 762e 6f72 672f 636f  w.medrxiv.org/co
+000070d0: 6e74 656e 742f 3130 2e31 3130 312f 3230  ntent/10.1101/20
+000070e0: 3230 2e30 362e 3330 2e32 3031 3433 3635  20.06.30.2014365
+000070f0: 3176 312e 6675 6c6c 2e70 6466 290a 2d20  1v1.full.pdf).- 
+00007100: 5b43 6f6d 7061 7269 6e67 2074 6865 2069  [Comparing the i
+00007110: 6e74 6572 7072 6574 6162 696c 6974 7920  nterpretability 
+00007120: 6f66 206d 6163 6869 6e65 206c 6561 726e  of machine learn
+00007130: 696e 6720 636c 6173 7369 6669 6572 7320  ing classifiers 
+00007140: 666f 7220 6272 6169 6e20 7475 6d6f 7572  for brain tumour
+00007150: 2073 7572 7669 7661 6c20 7072 6564 6963   survival predic
+00007160: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
+00007170: 6c69 7665 7279 7064 662e 7373 726e 2e63  liverypdf.ssrn.c
+00007180: 6f6d 2f64 656c 6976 6572 792e 7068 703f  om/delivery.php?
+00007190: 4944 3d37 3630 3132 3231 3138 3036 3731  ID=7601221180671
+000071a0: 3033 3039 3431 3038 3039 3031 3233 3039  0309410809012309
+000071b0: 3130 3739 3031 3130 3238 3033 3230 3039  1079011028032009
+000071c0: 3030 3930 3233 3038 3530 3035 3031 3430  0090230850050140
+000071d0: 3134 3030 3231 3233 3130 3530 3835 3131  1400212310508511
+000071e0: 3430 3235 3032 3230 3234 3030 3530 3437  4025022024005047
+000071f0: 3037 3830 3331 3031 3930 3839 3037 3331  0780310190890731
+00007200: 3230 3031 3230 3235 3131 3730 3733 3030  2001202511707300
+00007210: 3230 3634 3033 3130 3731 3037 3231 3133  2064031071072113
+00007220: 3030 3630 3636 3033 3530 3031 3036 3831  0060660350010681
+00007230: 3235 3032 3730 3231 3038 3730 3837 3038  2502702108708708
+00007240: 3330 3835 3032 3631 3030 3030 3930 3138  3085026100009018
+00007250: 3034 3531 3037 3039 3230 3633 3030 3130  0451070920630010
+00007260: 3233 3036 3830 3731 3030 3231 3234 3037  2306807100212407
+00007270: 3031 3037 3132 3031 3230 3030 3730 3134  0107120120007014
+00007280: 3130 3230 3934 3130 3330 3639 3038 3931  1020941030690891
+00007290: 3139 3032 3631 3130 3130 3431 3037 3030  1902611010410700
+000072a0: 3530 3331 3039 3530 3031 3039 3230 3930  5031095001092090
+000072b0: 2645 5854 3d70 6466 2649 4e44 4558 3d54  &EXT=pdf&INDEX=T
+000072c0: 5255 4529 0a2d 205b 5573 696e 6720 496e  RUE).- [Using In
+000072d0: 7465 7270 7265 7461 626c 6520 4d61 6368  terpretable Mach
+000072e0: 696e 6520 4c65 6172 6e69 6e67 2074 6f20  ine Learning to 
+000072f0: 5072 6564 6963 7420 4d61 7465 726e 616c  Predict Maternal
+00007300: 2061 6e64 2046 6574 616c 204f 7574 636f   and Fetal Outco
+00007310: 6d65 735d 2868 7474 7073 3a2f 2f61 7278  mes](https://arx
+00007320: 6976 2e6f 7267 2f70 6466 2f32 3230 372e  iv.org/pdf/2207.
+00007330: 3035 3332 322e 7064 6629 0a2d 205b 4361  05322.pdf).- [Ca
+00007340: 6c69 6272 6174 653a 2049 6e74 6572 6163  librate: Interac
+00007350: 7469 7665 2041 6e61 6c79 7369 7320 6f66  tive Analysis of
+00007360: 2050 726f 6261 6269 6c69 7374 6963 204d   Probabilistic M
+00007370: 6f64 656c 204f 7574 7075 745d 2868 7474  odel Output](htt
+00007380: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f70  ps://arxiv.org/p
+00007390: 6466 2f32 3230 372e 3133 3737 302e 7064  df/2207.13770.pd
+000073a0: 6629 0a2d 205b 4e65 7572 616c 2041 6464  f).- [Neural Add
+000073b0: 6974 6976 6520 4d6f 6465 6c73 3a20 496e  itive Models: In
+000073c0: 7465 7270 7265 7461 626c 6520 4d61 6368  terpretable Mach
+000073d0: 696e 6520 4c65 6172 6e69 6e67 2077 6974  ine Learning wit
+000073e0: 6820 4e65 7572 616c 204e 6574 735d 2868  h Neural Nets](h
+000073f0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00007400: 2f70 6466 2f32 3030 342e 3133 3931 322e  /pdf/2004.13912.
+00007410: 7064 6629 0a2d 205b 4e4f 4445 2d47 414d  pdf).- [NODE-GAM
+00007420: 3a20 4e65 7572 616c 2047 656e 6572 616c  : Neural General
+00007430: 697a 6564 2041 6464 6974 6976 6520 4d6f  ized Additive Mo
+00007440: 6465 6c20 666f 7220 496e 7465 7270 7265  del for Interpre
+00007450: 7461 626c 6520 4465 6570 204c 6561 726e  table Deep Learn
+00007460: 696e 675d 2868 7474 7073 3a2f 2f61 7278  ing](https://arx
+00007470: 6976 2e6f 7267 2f70 6466 2f32 3130 362e  iv.org/pdf/2106.
+00007480: 3031 3631 332e 7064 6629 0a2d 205b 5363  01613.pdf).- [Sc
+00007490: 616c 6162 6c65 2049 6e74 6572 7072 6574  alable Interpret
+000074a0: 6162 696c 6974 7920 7669 6120 506f 6c79  ability via Poly
+000074b0: 6e6f 6d69 616c 735d 2868 7474 7073 3a2f  nomials](https:/
+000074c0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+000074d0: 3230 352e 3134 3130 3876 312e 7064 6629  205.14108v1.pdf)
+000074e0: 0a2d 205b 4e65 7572 616c 2042 6173 6973  .- [Neural Basis
+000074f0: 204d 6f64 656c 7320 666f 7220 496e 7465   Models for Inte
+00007500: 7270 7265 7461 6269 6c69 7479 5d28 6874  rpretability](ht
+00007510: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+00007520: 7064 662f 3232 3035 2e31 3431 3230 2e70  pdf/2205.14120.p
+00007530: 6466 290a 2d20 5b49 4c4d 4152 543a 2049  df).- [ILMART: I
+00007540: 6e74 6572 7072 6574 6162 6c65 2052 616e  nterpretable Ran
+00007550: 6b69 6e67 2077 6974 6820 436f 6e73 7472  king with Constr
+00007560: 6169 6e65 6420 4c61 6d62 6461 4d41 5254  ained LambdaMART
+00007570: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
+00007580: 6f72 672f 7064 662f 3232 3036 2e30 3034  org/pdf/2206.004
+00007590: 3733 2e70 6466 290a 2d20 5b49 6e74 6567  73.pdf).- [Integ
+000075a0: 7261 7469 6e67 2043 6f2d 436c 7573 7465  rating Co-Cluste
+000075b0: 7269 6e67 2061 6e64 2049 6e74 6572 7072  ring and Interpr
+000075c0: 6574 6162 6c65 204d 6163 6869 6e65 204c  etable Machine L
+000075d0: 6561 726e 696e 6720 666f 7220 7468 6520  earning for the 
+000075e0: 5072 6564 6963 7469 6f6e 206f 6620 496e  Prediction of In
+000075f0: 7472 6176 656e 6f75 7320 496d 6d75 6e6f  travenous Immuno
+00007600: 676c 6f62 756c 696e 2052 6573 6973 7461  globulin Resista
+00007610: 6e63 6520 696e 204b 6177 6173 616b 6920  nce in Kawasaki 
+00007620: 4469 7365 6173 655d 2868 7474 7073 3a2f  Disease](https:/
+00007630: 2f69 6565 6578 706c 6f72 652e 6965 6565  /ieeexplore.ieee
+00007640: 2e6f 7267 2f73 7461 6d70 2f73 7461 6d70  .org/stamp/stamp
+00007650: 2e6a 7370 3f74 703d 2661 726e 756d 6265  .jsp?tp=&arnumbe
+00007660: 723d 3930 3937 3837 3429 0a2d 205b 4741  r=9097874).- [GA
+00007670: 4d49 2d4e 6574 3a20 416e 2045 7870 6c61  MI-Net: An Expla
+00007680: 696e 6162 6c65 204e 6575 7261 6c20 4e65  inable Neural Ne
+00007690: 7477 6f72 6b20 6261 7365 6420 6f6e 2047  twork based on G
+000076a0: 656e 6572 616c 697a 6564 2041 6464 6974  eneralized Addit
+000076b0: 6976 6520 4d6f 6465 6c73 2077 6974 6820  ive Models with 
+000076c0: 5374 7275 6374 7572 6564 2049 6e74 6572  Structured Inter
+000076d0: 6163 7469 6f6e 735d 2868 7474 7073 3a2f  actions](https:/
+000076e0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+000076f0: 3030 332e 3037 3133 3276 312e 7064 6629  003.07132v1.pdf)
+00007700: 0a2d 205b 4120 436f 6e63 6570 7420 616e  .- [A Concept an
+00007710: 6420 4172 6775 6d65 6e74 6174 696f 6e20  d Argumentation 
+00007720: 6261 7365 6420 496e 7465 7270 7265 7461  based Interpreta
+00007730: 626c 6520 4d6f 6465 6c20 696e 2048 6967  ble Model in Hig
+00007740: 6820 5269 736b 2044 6f6d 6169 6e73 5d28  h Risk Domains](
+00007750: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00007760: 672f 7064 662f 3232 3038 2e30 3831 3439  g/pdf/2208.08149
+00007770: 2e70 6466 290a 2d20 5b41 6e61 6c79 7a69  .pdf).- [Analyzi
+00007780: 6e67 2074 6865 2044 6966 6665 7265 6e63  ng the Differenc
+00007790: 6573 2062 6574 7765 656e 2050 726f 6665  es between Profe
+000077a0: 7373 696f 6e61 6c20 616e 6420 416d 6174  ssional and Amat
+000077b0: 6575 7220 4573 706f 7274 7320 7468 726f  eur Esports thro
+000077c0: 7567 6820 5769 6e20 5072 6f62 6162 696c  ugh Win Probabil
+000077d0: 6974 795d 2868 7474 7073 3a2f 2f64 6c2e  ity](https://dl.
+000077e0: 6163 6d2e 6f72 672f 646f 692f 7064 662f  acm.org/doi/pdf/
+000077f0: 3130 2e31 3134 352f 3334 3835 3434 372e  10.1145/3485447.
+00007800: 3335 3132 3237 3729 0a2d 205b 4578 706c  3512277).- [Expl
+00007810: 6169 6e61 626c 6520 6d61 6368 696e 6520  ainable machine 
+00007820: 6c65 6172 6e69 6e67 2077 6974 6820 7061  learning with pa
+00007830: 6972 7769 7365 2069 6e74 6572 6163 7469  irwise interacti
+00007840: 6f6e 7320 666f 7220 7468 6520 636c 6173  ons for the clas
+00007850: 7369 6663 6174 696f 6e20 6f66 2050 6172  sifcation of Par
+00007860: 6b69 6e73 6f6e e280 9973 2064 6973 6561  kinson...s disea
+00007870: 7365 2061 6e64 2053 5745 4444 2066 726f  se and SWEDD fro
+00007880: 6d20 636c 696e 6963 616c 2061 6e64 2069  m clinical and i
+00007890: 6d61 6769 6e67 2066 6561 7475 7265 735d  maging features]
+000078a0: 2868 7474 7073 3a2f 2f77 7777 2e6e 6362  (https://www.ncb
+000078b0: 692e 6e6c 6d2e 6e69 682e 676f 762f 706d  i.nlm.nih.gov/pm
+000078c0: 632f 6172 7469 636c 6573 2f50 4d43 3931  c/articles/PMC91
+000078d0: 3332 3736 312f 7064 662f 3131 3638 325f  32761/pdf/11682_
+000078e0: 3230 3232 5f41 7274 6963 6c65 5f36 3838  2022_Article_688
+000078f0: 2e70 6466 290a 2d20 5b49 6e74 6572 7072  .pdf).- [Interpr
+00007900: 6574 6162 6c65 2050 7265 6469 6374 696f  etable Predictio
+00007910: 6e20 6f66 2047 6f61 6c73 2069 6e20 536f  n of Goals in So
+00007920: 6363 6572 5d28 6874 7470 733a 2f2f 7374  ccer](https://st
+00007930: 6174 7362 6f6d 622e 636f 6d2f 7770 2d63  atsbomb.com/wp-c
+00007940: 6f6e 7465 6e74 2f75 706c 6f61 6473 2f32  ontent/uploads/2
+00007950: 3031 392f 3130 2f64 6563 726f 6f73 2d69  019/10/decroos-i
+00007960: 6e74 6572 7072 6574 6162 696c 6974 792d  nterpretability-
+00007970: 7374 6174 7362 6f6d 622e 7064 6629 0a2d  statsbomb.pdf).-
+00007980: 205b 4578 7465 6e64 696e 6720 7468 6520   [Extending the 
+00007990: 5473 6574 6c69 6e20 4d61 6368 696e 6520  Tsetlin Machine 
+000079a0: 7769 7468 2049 6e74 6567 6572 2d57 6569  with Integer-Wei
+000079b0: 6768 7465 6420 436c 6175 7365 7320 666f  ghted Clauses fo
+000079c0: 7220 496e 6372 6561 7365 6420 496e 7465  r Increased Inte
+000079d0: 7270 7265 7461 6269 6c69 7479 5d28 6874  rpretability](ht
+000079e0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+000079f0: 7064 662f 3230 3035 2e30 3531 3331 2e70  pdf/2005.05131.p
+00007a00: 6466 290a 2d20 5b49 6e20 5075 7273 7569  df).- [In Pursui
+00007a10: 7420 6f66 2049 6e74 6572 7072 6574 6162  t of Interpretab
+00007a20: 6c65 2c20 4661 6972 2061 6e64 2041 6363  le, Fair and Acc
+00007a30: 7572 6174 6520 4d61 6368 696e 6520 4c65  urate Machine Le
+00007a40: 6172 6e69 6e67 2066 6f72 2043 7269 6d69  arning for Crimi
+00007a50: 6e61 6c20 5265 6369 6469 7669 736d 2050  nal Recidivism P
+00007a60: 7265 6469 6374 696f 6e5d 2868 7474 7073  rediction](https
+00007a70: 3a2f 2f61 7278 6976 2e6f 7267 2f70 6466  ://arxiv.org/pdf
+00007a80: 2f32 3030 352e 3034 3137 362e 7064 6629  /2005.04176.pdf)
+00007a90: 0a2d 205b 4672 6f6d 2053 6861 706c 6579  .- [From Shapley
+00007aa0: 2056 616c 7565 7320 746f 2047 656e 6572   Values to Gener
+00007ab0: 616c 697a 6564 2041 6464 6974 6976 6520  alized Additive 
+00007ac0: 4d6f 6465 6c73 2061 6e64 2062 6163 6b5d  Models and back]
+00007ad0: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
+00007ae0: 7267 2f70 6466 2f32 3230 392e 3034 3031  rg/pdf/2209.0401
+00007af0: 322e 7064 6629 0a2d 205b 416e 2045 7870  2.pdf).- [An Exp
+00007b00: 6c61 696e 6162 6c65 204d 6163 6869 6e65  lainable Machine
+00007b10: 204c 6561 726e 696e 6720 4170 7072 6f61   Learning Approa
+00007b20: 6368 2074 6f20 5669 7375 616c 2d49 6e74  ch to Visual-Int
+00007b30: 6572 6163 7469 7665 204c 6162 656c 696e  eractive Labelin
+00007b40: 673a 2041 2043 6173 6520 5374 7564 7920  g: A Case Study 
+00007b50: 6f6e 204e 6f6e 2d63 6f6d 6d75 6e69 6361  on Non-communica
+00007b60: 626c 6520 4469 7365 6173 6520 4461 7461  ble Disease Data
+00007b70: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
+00007b80: 6f72 672f 7064 662f 3232 3039 2e31 3237  org/pdf/2209.127
+00007b90: 3738 2e70 6466 290a 2d20 5b44 6576 656c  78.pdf).- [Devel
+00007ba0: 6f70 6d65 6e74 2061 6e64 2056 616c 6964  opment and Valid
+00007bb0: 6174 696f 6e20 6f66 2061 6e20 496e 7465  ation of an Inte
+00007bc0: 7270 7265 7461 626c 6520 332d 6461 7920  rpretable 3-day 
+00007bd0: 496e 7465 6e73 6976 6520 4361 7265 2055  Intensive Care U
+00007be0: 6e69 7420 5265 6164 6d69 7373 696f 6e20  nit Readmission 
+00007bf0: 5072 6564 6963 7469 6f6e 204d 6f64 656c  Prediction Model
+00007c00: 2055 7369 6e67 2045 7870 6c61 696e 6162   Using Explainab
+00007c10: 6c65 2042 6f6f 7374 696e 6720 4d61 6368  le Boosting Mach
+00007c20: 696e 6573 5d28 6874 7470 733a 2f2f 7777  ines](https://ww
+00007c30: 772e 6d65 6472 7869 762e 6f72 672f 636f  w.medrxiv.org/co
+00007c40: 6e74 656e 742f 3130 2e31 3130 312f 3230  ntent/10.1101/20
+00007c50: 3231 2e31 312e 3031 2e32 3132 3635 3730  21.11.01.2126570
+00007c60: 3076 312e 6675 6c6c 2e70 6466 290a 2d20  0v1.full.pdf).- 
+00007c70: 5b44 6561 7468 2062 7920 526f 756e 6420  [Death by Round 
+00007c80: 4e75 6d62 6572 7320 616e 6420 5368 6172  Numbers and Shar
+00007c90: 7020 5468 7265 7368 6f6c 6473 3a20 486f  p Thresholds: Ho
+00007ca0: 7720 746f 2041 766f 6964 2044 616e 6765  w to Avoid Dange
+00007cb0: 726f 7573 2041 4920 4548 5220 5265 636f  rous AI EHR Reco
+00007cc0: 6d6d 656e 6461 7469 6f6e 735d 2868 7474  mmendations](htt
+00007cd0: 7073 3a2f 2f77 7777 2e6d 6564 7278 6976  ps://www.medrxiv
+00007ce0: 2e6f 7267 2f63 6f6e 7465 6e74 2f31 302e  .org/content/10.
+00007cf0: 3131 3031 2f32 3032 322e 3034 2e33 302e  1101/2022.04.30.
+00007d00: 3232 3237 3435 3230 7631 2e66 756c 6c2e  22274520v1.full.
+00007d10: 7064 6629 0a2d 205b 4275 696c 6469 6e67  pdf).- [Building
+00007d20: 2061 2070 7265 6469 6374 6976 6520 6d6f   a predictive mo
+00007d30: 6465 6c20 746f 2069 6465 6e74 6966 7920  del to identify 
+00007d40: 636c 696e 6963 616c 2069 6e64 6963 6174  clinical indicat
+00007d50: 6f72 7320 666f 7220 434f 5649 442d 3139  ors for COVID-19
+00007d60: 2075 7369 6e67 206d 6163 6869 6e65 206c   using machine l
+00007d70: 6561 726e 696e 6720 6d65 7468 6f64 5d28  earning method](
+00007d80: 6874 7470 733a 2f2f 7777 772e 6e63 6269  https://www.ncbi
+00007d90: 2e6e 6c6d 2e6e 6968 2e67 6f76 2f70 6d63  .nlm.nih.gov/pmc
+00007da0: 2f61 7274 6963 6c65 732f 504d 4339 3033  /articles/PMC903
+00007db0: 3739 3732 2f70 6466 2f31 3135 3137 5f32  7972/pdf/11517_2
+00007dc0: 3032 325f 4172 7469 636c 655f 3235 3638  022_Article_2568
+00007dd0: 2e70 6466 290a 2d20 5b55 7369 6e67 2049  .pdf).- [Using I
+00007de0: 6e6e 6f76 6174 6976 6520 4d61 6368 696e  nnovative Machin
+00007df0: 6520 4c65 6172 6e69 6e67 204d 6574 686f  e Learning Metho
+00007e00: 6473 2074 6f20 5363 7265 656e 2061 6e64  ds to Screen and
+00007e10: 2049 6465 6e74 6966 7920 5072 6564 6963   Identify Predic
+00007e20: 746f 7273 206f 6620 436f 6e67 656e 6974  tors of Congenit
+00007e30: 616c 2048 6561 7274 2044 6973 6561 7365  al Heart Disease
+00007e40: 735d 2868 7474 7073 3a2f 2f77 7777 2e6e  s](https://www.n
+00007e50: 6362 692e 6e6c 6d2e 6e69 682e 676f 762f  cbi.nlm.nih.gov/
+00007e60: 706d 632f 6172 7469 636c 6573 2f50 4d43  pmc/articles/PMC
+00007e70: 3837 3737 3032 322f 7064 662f 6663 766d  8777022/pdf/fcvm
+00007e80: 2d30 382d 3739 3730 3032 2e70 6466 290a  -08-797002.pdf).
+00007e90: 2d20 5b45 7870 6c61 696e 6162 6c65 2042  - [Explainable B
+00007ea0: 6f6f 7374 696e 6720 4d61 6368 696e 6520  oosting Machine 
+00007eb0: 666f 7220 5072 6564 6963 7469 6e67 2041  for Predicting A
+00007ec0: 6c7a 6865 696d 6572 e280 9973 2044 6973  lzheimer...s Dis
+00007ed0: 6561 7365 2066 726f 6d20 4d52 4920 4869  ease from MRI Hi
+00007ee0: 7070 6f63 616d 7061 6c20 5375 6266 6965  ppocampal Subfie
+00007ef0: 6c64 735d 2868 7474 7073 3a2f 2f6c 696e  lds](https://lin
+00007f00: 6b2e 7370 7269 6e67 6572 2e63 6f6d 2f63  k.springer.com/c
+00007f10: 6861 7074 6572 2f31 302e 3130 3037 2f39  hapter/10.1007/9
+00007f20: 3738 2d33 2d30 3330 2d38 3639 3933 2d39  78-3-030-86993-9
+00007f30: 5f33 3129 0a2d 205b 496d 7061 6374 206f  _31).- [Impact o
+00007f40: 6620 4163 6375 7261 6379 206f 6e20 4d6f  f Accuracy on Mo
+00007f50: 6465 6c20 496e 7465 7270 7265 7461 7469  del Interpretati
+00007f60: 6f6e 735d 2868 7474 7073 3a2f 2f61 7278  ons](https://arx
+00007f70: 6976 2e6f 7267 2f70 6466 2f32 3031 312e  iv.org/pdf/2011.
+00007f80: 3039 3930 332e 7064 6629 0a2d 205b 4d61  09903.pdf).- [Ma
+00007f90: 6368 696e 6520 4c65 6172 6e69 6e67 2041  chine Learning A
+00007fa0: 6c67 6f72 6974 686d 7320 666f 7220 4964  lgorithms for Id
+00007fb0: 656e 7469 6679 696e 6720 4465 7065 6e64  entifying Depend
+00007fc0: 656e 6369 6573 2069 6e20 4f54 2050 726f  encies in OT Pro
+00007fd0: 746f 636f 6c73 5d28 6874 7470 733a 2f2f  tocols](https://
+00007fe0: 7777 772e 6d64 7069 2e63 6f6d 2f31 3939  www.mdpi.com/199
+00007ff0: 362d 3130 3733 2f31 362f 3130 2f34 3035  6-1073/16/10/405
+00008000: 3629 0a0a 2320 426f 6f6b 7320 7468 6174  6)..# Books that
+00008010: 2064 6973 6375 7373 2045 424d 730a 0a2d   discuss EBMs..-
+00008020: 205b 4d61 6368 696e 6520 4c65 6172 6e69   [Machine Learni
+00008030: 6e67 2066 6f72 2048 6967 682d 5269 736b  ng for High-Risk
+00008040: 2041 7070 6c69 6361 7469 6f6e 735d 2868   Applications](h
+00008050: 7474 7073 3a2f 2f77 7777 2e6f 7265 696c  ttps://www.oreil
+00008060: 6c79 2e63 6f6d 2f6c 6962 7261 7279 2f76  ly.com/library/v
+00008070: 6965 772f 6d61 6368 696e 652d 6c65 6172  iew/machine-lear
+00008080: 6e69 6e67 2d66 6f72 2f39 3738 3130 3938  ning-for/9781098
+00008090: 3130 3234 3235 2f29 0a2d 205b 496e 7465  102425/).- [Inte
+000080a0: 7270 7265 7461 626c 6520 4d61 6368 696e  rpretable Machin
+000080b0: 6520 4c65 6172 6e69 6e67 2077 6974 6820  e Learning with 
+000080c0: 5079 7468 6f6e 5d28 6874 7470 733a 2f2f  Python](https://
+000080d0: 7777 772e 616d 617a 6f6e 2e63 6f6d 2f49  www.amazon.com/I
+000080e0: 6e74 6572 7072 6574 6162 6c65 2d4d 6163  nterpretable-Mac
+000080f0: 6869 6e65 2d4c 6561 726e 696e 672d 5079  hine-Learning-Py
+00008100: 7468 6f6e 2d68 616e 6473 2f64 702f 3138  thon-hands/dp/18
+00008110: 3030 3230 3339 3058 290a 2d20 5b45 7870  0020390X).- [Exp
+00008120: 6c61 696e 6162 6c65 2041 7274 6966 6963  lainable Artific
+00008130: 6961 6c20 496e 7465 6c6c 6967 656e 6365  ial Intelligence
+00008140: 3a20 416e 2049 6e74 726f 6475 6374 696f  : An Introductio
+00008150: 6e20 746f 2049 6e74 6572 7072 6574 6162  n to Interpretab
+00008160: 6c65 204d 6163 6869 6e65 204c 6561 726e  le Machine Learn
+00008170: 696e 675d 2868 7474 7073 3a2f 2f77 7777  ing](https://www
+00008180: 2e61 6d61 7a6f 6e2e 636f 6d2f 4578 706c  .amazon.com/Expl
+00008190: 6169 6e61 626c 652d 4172 7469 6669 6369  ainable-Artifici
+000081a0: 616c 2d49 6e74 656c 6c69 6765 6e63 655f  al-Intelligence_
+000081b0: 2d41 6e2d 496e 7472 6f64 7563 7469 6f6e  -An-Introduction
+000081c0: 2d74 6f2d 496e 7465 7270 7265 7461 626c  -to-Interpretabl
+000081d0: 652d 5841 492f 6470 2f33 3033 3038 3333  e-XAI/dp/3030833
+000081e0: 3535 3029 0a2d 205b 4170 706c 6965 6420  550).- [Applied 
+000081f0: 4d61 6368 696e 6520 4c65 6172 6e69 6e67  Machine Learning
+00008200: 2045 7870 6c61 696e 6162 696c 6974 7920   Explainability 
+00008210: 5465 6368 6e69 7175 6573 5d28 6874 7470  Techniques](http
+00008220: 733a 2f2f 7777 772e 616d 617a 6f6e 2e63  s://www.amazon.c
+00008230: 6f6d 2f41 7070 6c69 6564 2d4d 6163 6869  om/Applied-Machi
+00008240: 6e65 2d4c 6561 726e 696e 672d 4578 706c  ne-Learning-Expl
+00008250: 6169 6e61 6269 6c69 7479 2d54 6563 686e  ainability-Techn
+00008260: 6971 7565 732f 6470 2f31 3830 3332 3436  iques/dp/1803246
+00008270: 3135 3429 0a2d 205b 5468 6520 6558 706c  154).- [The eXpl
+00008280: 6169 6e61 626c 6520 412e 492e 3a20 5769  ainable A.I.: Wi
+00008290: 7468 2050 7974 686f 6e20 6578 616d 706c  th Python exampl
+000082a0: 6573 5d28 6874 7470 733a 2f2f 7777 772e  es](https://www.
+000082b0: 616d 617a 6f6e 2e63 6f6d 2f65 5870 6c61  amazon.com/eXpla
+000082c0: 696e 6162 6c65 2d49 2d50 7974 686f 6e2d  inable-I-Python-
+000082d0: 6578 616d 706c 6573 2d65 626f 6f6b 2f64  examples-ebook/d
+000082e0: 702f 4230 4234 4639 384d 4e36 290a 2d20  p/B0B4F98MN6).- 
+000082f0: 5b45 7870 6c61 696e 6162 6c65 2041 4920  [Explainable AI 
+00008300: 5265 6369 7065 735d 2868 7474 7073 3a2f  Recipes](https:/
+00008310: 2f77 7777 2e61 6d61 7a6f 6e2e 636f 6d2f  /www.amazon.com/
+00008320: 4578 706c 6169 6e61 626c 652d 5265 6369  Explainable-Reci
+00008330: 7065 732d 496d 706c 656d 656e 742d 4578  pes-Implement-Ex
+00008340: 706c 6169 6e61 6269 6c69 7479 2d49 6e74  plainability-Int
+00008350: 6572 7072 6574 6162 696c 6974 792d 6562  erpretability-eb
+00008360: 6f6f 6b2f 6470 2f42 3042 5346 354e 4259  ook/dp/B0BSF5NBY
+00008370: 3729 0a0a 2320 4578 7465 726e 616c 2074  7)..# External t
+00008380: 6f6f 6c73 0a0a 2d20 5b45 424d 2074 6f20  ools..- [EBM to 
+00008390: 4f6e 6e78 2063 6f6e 7665 7274 6572 2062  Onnx converter b
+000083a0: 7920 536f 6674 4174 486f 6d65 5d28 6874  y SoftAtHome](ht
+000083b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000083c0: 2f69 6e74 6572 7072 6574 6d6c 2f65 626d  /interpretml/ebm
+000083d0: 326f 6e6e 7829 0a2d 205b 4741 4d20 4368  2onnx).- [GAM Ch
+000083e0: 616e 6765 725d 2868 7474 7073 3a2f 2f67  anger](https://g
+000083f0: 6974 6875 622e 636f 6d2f 696e 7465 7270  ithub.com/interp
+00008400: 7265 746d 6c2f 6761 6d2d 6368 616e 6765  retml/gam-change
+00008410: 7229 0a2d 205b 4d4c 2032 2053 514c 2028  r).- [ML 2 SQL (
+00008420: 6578 7065 7269 6d65 6e74 616c 295d 2868  experimental)](h
+00008430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00008440: 6d2f 6b61 7370 6572 7367 6974 2f6d 6c5f  m/kaspersgit/ml_
+00008450: 325f 7371 6c29 0a0a 2320 436f 6e74 6163  2_sql)..# Contac
+00008460: 7420 7573 0a0a 5468 6572 6520 6172 6520  t us..There are 
+00008470: 6d75 6c74 6970 6c65 2077 6179 7320 746f  multiple ways to
+00008480: 2067 6574 2069 6e20 746f 7563 683a 0a2d   get in touch:.-
+00008490: 2045 6d61 696c 2075 7320 6174 2069 6e74   Email us at int
+000084a0: 6572 7072 6574 406d 6963 726f 736f 6674  erpret@microsoft
+000084b0: 2e63 6f6d 0a2d 204f 722c 2066 6565 6c20  .com.- Or, feel 
+000084c0: 6672 6565 2074 6f20 7261 6973 6520 6120  free to raise a 
+000084d0: 4769 7448 7562 2069 7373 7565 0a0a 3c62  GitHub issue..<b
+000084e0: 722f 3e0a 3c62 722f 3e0a 3c62 722f 3e0a  r/>.<br/>.<br/>.
+000084f0: 3c62 722f 3e0a 3c62 722f 3e0a 0a3c 6272  <br/>.<br/>..<br
+00008500: 2f3e 0a3c 6272 2f3e 0a3c 6272 2f3e 0a3c  />.<br/>.<br/>.<
+00008510: 6272 2f3e 0a3c 6272 2f3e 0a0a 3c62 722f  br/>.<br/>..<br/
+00008520: 3e0a 3c62 722f 3e0a 3c62 722f 3e0a 3c62  >.<br/>.<br/>.<b
+00008530: 722f 3e0a 3c62 722f 3e0a 0a3c 6272 2f3e  r/>.<br/>..<br/>
+00008540: 0a3c 6272 2f3e 0a3c 6272 2f3e 0a3c 6272  .<br/>.<br/>.<br
+00008550: 2f3e 0a3c 6272 2f3e 0a0a 3c62 722f 3e0a  />.<br/>..<br/>.
+00008560: 3c62 722f 3e0a 3c62 722f 3e0a 3c62 722f  <br/>.<br/>.<br/
+00008570: 3e0a 3c62 722f 3e0a 0a3c 6272 2f3e 0a3c  >.<br/>..<br/>.<
+00008580: 6272 2f3e 0a3c 6272 2f3e 0a3c 6272 2f3e  br/>.<br/>.<br/>
+00008590: 0a3c 6272 2f3e 0a0a 3c62 722f 3e0a 3c62  .<br/>..<br/>.<b
+000085a0: 722f 3e0a 3c62 722f 3e0a 3c62 722f 3e0a  r/>.<br/>.<br/>.
+000085b0: 3c62 722f 3e0a 0a3c 6272 2f3e 0a3c 6272  <br/>..<br/>.<br
+000085c0: 2f3e 0a3c 6272 2f3e 0a3c 6272 2f3e 0a3c  />.<br/>.<br/>.<
+000085d0: 6272 2f3e 0a0a 3e20 2323 2320 4966 2061  br/>..> ### If a
+000085e0: 2074 7265 6520 6665 6c6c 2069 6e20 796f   tree fell in yo
+000085f0: 7572 2072 616e 646f 6d20 666f 7265 7374  ur random forest
+00008600: 2c20 776f 756c 6420 616e 796f 6e65 206e  , would anyone n
+00008610: 6f74 6963 653f 0a                        otice?.
```

### Comparing `interpret-core-0.4.0/symbolic/build.bat` & `interpret-core-0.4.1/symbolic/build.bat`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/build.sh` & `interpret-core-0.4.1/symbolic/build.sh`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/ApplyTermUpdate.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/ApplyTermUpdate.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/BinSumsBoosting.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/BinSumsBoosting.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/BinSumsInteraction.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/BinSumsInteraction.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/BoosterCore.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/BoosterCore.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/BoosterCore.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/BoosterCore.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/BoosterShell.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/BoosterShell.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/BoosterShell.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/BoosterShell.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/CODING_STYLE.md` & `interpret-core-0.4.1/symbolic/shared/libebm/CODING_STYLE.md`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/CalcInteractionStrength.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/CalcInteractionStrength.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/CutQuantile.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/CutQuantile.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/CutUniform.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/CutUniform.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/CutWinsorized.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/CutWinsorized.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/DataSetBoosting.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/DataSetBoosting.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 #include "precompiled_header_cpp.hpp"
 
 #include <stdlib.h> // free
 #include <stddef.h> // size_t, ptrdiff_t
 #include <string.h> // memcpy
 
 #include "common_cpp.hpp" // INLINE_RELEASE_UNTEMPLATED
-#include "bridge_cpp.hpp" // GetCountScores
 
 #include "Feature.hpp" // Feature
 #include "Term.hpp" // Term
 #include "dataset_shared.hpp" // SharedStorageDataType
 #include "DataSetBoosting.hpp"
 
 namespace DEFINED_ZONE_NAME {
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/DataSetBoosting.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/DataSetBoosting.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/DataSetInteraction.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/DataSetInteraction.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 #include "precompiled_header_cpp.hpp"
 
 #include <stdlib.h> // free
 #include <stddef.h> // size_t, ptrdiff_t
 
 #include "common_cpp.hpp" // INLINE_RELEASE_UNTEMPLATED
-#include "bridge_cpp.hpp" // GetCountScores
 
 #include "ebm_internal.hpp" // AddPositiveFloatsSafeBig
 
 #include "Feature.hpp"
 #include "dataset_shared.hpp" // SharedStorageDataType
 #include "DataSetInteraction.hpp"
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/DataSetInteraction.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/DataSetInteraction.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/DetermineLinkFunction.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/DetermineLinkFunction.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -48,16 +48,14 @@
    }
    if(nullptr != linkParamOut) {
       *linkParamOut = objectiveWrapper.m_linkParam;
    }
    return Error_None;
 }
 
-static const char g_sERROR[] = "ERROR";
-
 static const char g_sCustomRegression[] = "custom_regression";
 static const char g_sCustomClassification[] = "custom_classification";
 static const char g_sCustomRanking[] = "custom_ranking";
 static const char g_sPower[] = "power";
 static const char g_sLogit[] = "logit";
 static const char g_sProbit[] = "probit";
 static const char g_sCloglog[] = "cloglog";
@@ -65,15 +63,15 @@
 static const char g_sCauchit[] = "cauchit";
 static const char g_sIdentity[] = "identity";
 static const char g_sLog[] = "log";
 static const char g_sInverse[] = "inverse";
 static const char g_sInverseSquare[] = "inverse_square";
 static const char g_sSqrt[] = "sqrt";
 
-EBM_API_BODY const char * EBM_CALLING_CONVENTION GetLinkFunctionString(LinkEbm link) {
+EBM_API_BODY const char * EBM_CALLING_CONVENTION GetLinkFunctionStr(LinkEbm link) {
    switch(link) {
    case Link_custom_regression:
       return g_sCustomRegression;
    case Link_custom_classification:
       return g_sCustomClassification;
    case Link_custom_ranking:
       return g_sCustomRanking;
@@ -96,15 +94,15 @@
    case Link_inverse:
       return g_sInverse;
    case Link_inverse_square:
       return g_sInverseSquare;
    case Link_sqrt:
       return g_sSqrt;
    default:
-      return g_sERROR;
+      return nullptr;
    }
 }
 
 EBM_API_BODY LinkEbm EBM_CALLING_CONVENTION GetLinkFunctionInt(const char * link) {
    if(nullptr != link) {
       link = SkipWhitespace(link);
 
@@ -136,12 +134,30 @@
          return Link_inverse_square;
       if(IsStringEqualsForgiving(link, g_sSqrt))
          return Link_sqrt;
    }
    return Link_ERROR;
 }
 
-EBM_API_BODY OutputType EBM_CALLING_CONVENTION GetOutputType(LinkEbm link) {
-   return ConvertOutputType(link);
+EBM_API_BODY OutputType EBM_CALLING_CONVENTION GetOutputTypeInt(LinkEbm link) {
+   return GetOutputType(link);
+}
+
+static const char g_sClassification[] = "classification";
+static const char g_sRegression[] = "regression";
+static const char g_sRanking[] = "ranking";
+
+EBM_API_BODY const char * EBM_CALLING_CONVENTION GetOutputTypeStr(const char * link) {
+   const OutputType outputType = GetOutputType(GetLinkFunctionInt(link));
+   if(OutputType_GeneralClassification <= outputType) {
+      return g_sClassification;
+   }
+   if(OutputType_Regression == outputType) {
+      return g_sRegression;
+   }
+   if(OutputType_Ranking == outputType) {
+      return g_sRanking;
+   }
+   return nullptr;
 }
 
 } // DEFINED_ZONE_NAME
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/Discretize.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/Discretize.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/Feature.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/Feature.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/GaussianDistribution.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/GaussianDistribution.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/GenerateTermUpdate.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/GenerateTermUpdate.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/IMPORTANT.md` & `interpret-core-0.4.1/symbolic/shared/libebm/IMPORTANT.md`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/InitializeGradientsAndHessians.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/InitializeGradientsAndHessians.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/InnerBag.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/InnerBag.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/InnerBag.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/InnerBag.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/InteractionCore.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/InteractionCore.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/InteractionCore.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/InteractionCore.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/InteractionShell.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/InteractionShell.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/InteractionShell.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/InteractionShell.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/PartitionOneDimensionalBoosting.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/PartitionOneDimensionalBoosting.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/PartitionRandomBoosting.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/PartitionRandomBoosting.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/PartitionTwoDimensionalBoosting.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/PartitionTwoDimensionalBoosting.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/PartitionTwoDimensionalInteraction.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/PartitionTwoDimensionalInteraction.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/RandomDeterministic.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/RandomDeterministic.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/RandomDeterministic.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/RandomDeterministic.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/RandomNondeterministic.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/RandomNondeterministic.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/SplitPosition.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/SplitPosition.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/Tensor.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/Tensor.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/Tensor.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/Tensor.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/TensorTotalsBuild.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/TensorTotalsBuild.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/TensorTotalsSum.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/TensorTotalsSum.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #define TENSOR_TOTALS_SUM_HPP
 
 #include <stddef.h> // size_t, ptrdiff_t
 
 #include "logging.h" // EBM_ASSERT
 #include "zones.h"
 
-#include "bridge_cpp.hpp" // GetCountScores
+#include "bridge_cpp.hpp" // GetArrayScores
 
 #include "GradientPair.hpp"
 #include "Bin.hpp"
 
 namespace DEFINED_ZONE_NAME {
 #ifndef DEFINED_ZONE_NAME
 #error DEFINED_ZONE_NAME must be defined
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/Term.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/Term.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/Term.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/Term.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/Transpose.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/Transpose.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/TreeNode.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/TreeNode.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/bridge_c/bridge_c.h` & `interpret-core-0.4.1/symbolic/shared/libebm/bridge_c/bridge_c.h`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/bridge_c/zones.h` & `interpret-core-0.4.1/symbolic/shared/libebm/bridge_c/zones.h`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/bridge_cpp/Bin.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/Bin.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/bridge_cpp/GradientPair.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/GradientPair.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/bridge_cpp/bridge_cpp.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/bridge_cpp.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -14,44 +14,48 @@
 #include "Bin.hpp"
 
 namespace DEFINED_ZONE_NAME {
 #ifndef DEFINED_ZONE_NAME
 #error DEFINED_ZONE_NAME must be defined
 #endif // DEFINED_ZONE_NAME
 
-static constexpr ptrdiff_t k_regression = -1;
-static constexpr size_t k_oneScore = 1;
-static constexpr size_t k_dynamicScores = 0;
 inline constexpr static bool IsRegression(const ptrdiff_t cClasses) noexcept {
-   return k_regression == cClasses;
+   return ptrdiff_t { OutputType_Regression } == cClasses;
 }
 inline constexpr static bool IsClassification(const ptrdiff_t cClasses) noexcept {
-   return 0 <= cClasses;
+   return ptrdiff_t { OutputType_GeneralClassification } <= cClasses;
 }
 inline constexpr static bool IsBinaryClassification(const ptrdiff_t cClasses) noexcept {
 #ifdef EXPAND_BINARY_LOGITS
    return UNUSED(cClasses), false;
 #else // EXPAND_BINARY_LOGITS
-   return 2 == cClasses;
+   return ptrdiff_t { OutputType_BinaryClassification } == cClasses;
 #endif // EXPAND_BINARY_LOGITS
 }
 inline constexpr static bool IsMulticlass(const ptrdiff_t cClasses) noexcept {
-   return IsClassification(cClasses) && !IsBinaryClassification(cClasses);
+#ifdef EXPAND_BINARY_LOGITS
+   return ptrdiff_t { OutputType_GeneralClassification } <= cClasses;
+#else // EXPAND_BINARY_LOGITS
+   return ptrdiff_t { OutputType_BinaryClassification } < cClasses;
+#endif // EXPAND_BINARY_LOGITS
 }
 
 inline constexpr static size_t GetCountScores(const ptrdiff_t cClasses) noexcept {
    // this will work for anything except if cClasses is set to DYNAMIC_CLASSIFICATION which means we should have passed in the 
    // dynamic value since DYNAMIC_CLASSIFICATION is a constant that doesn't tell us anything about the real value
 #ifdef EXPAND_BINARY_LOGITS
-   return cClasses <= ptrdiff_t { 1 } ? size_t { 1 } : static_cast<size_t>(cClasses);
+   return cClasses < ptrdiff_t { OutputType_BinaryClassification } ? size_t { 1 } : static_cast<size_t>(cClasses);
 #else // EXPAND_BINARY_LOGITS
-   return cClasses <= ptrdiff_t { 2 } ? size_t { 1 } : static_cast<size_t>(cClasses);
+   return cClasses <= ptrdiff_t { OutputType_BinaryClassification } ? size_t { 1 } : static_cast<size_t>(cClasses);
 #endif // EXPAND_BINARY_LOGITS
 }
 
+static constexpr size_t k_oneScore = 1;
+static constexpr size_t k_dynamicScores = 0;
+
 inline constexpr static size_t GetArrayScores(const size_t cScores) noexcept {
    return k_dynamicScores == cScores ? size_t { 1 } : cScores;
 }
 
 // THIS NEEDS TO BE A MACRO AND NOT AN INLINE FUNCTION -> an inline function will cause all the parameters to get resolved before calling the function
 // We want any arguments to our macro to not get resolved if they are not needed at compile time so that we do less work if it's not needed
 // This will effectively turn the variable into a compile time constant if it can be resolved at compile time
@@ -122,15 +126,15 @@
       Link_cloglog == link ||
       Link_loglog == link ||
       Link_cauchit == link;
 }
 inline constexpr static bool IsRankingOutput(const LinkEbm link) noexcept {
    return Link_custom_ranking == link;
 }
-inline constexpr static OutputType ConvertOutputType(const LinkEbm link) noexcept {
+inline constexpr static OutputType GetOutputType(const LinkEbm link) noexcept {
    return IsRegressionOutput(link) ? OutputType_Regression :
       IsClassificationOutput(link) ? OutputType_GeneralClassification :
       IsRankingOutput(link) ? OutputType_Ranking :
       OutputType_Unknown;
 }
 
 struct BinSumsBoostingBridge {
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/common_c/common_c.c` & `interpret-core-0.4.1/symbolic/shared/libebm/common_c/common_c.c`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/common_c/common_c.h` & `interpret-core-0.4.1/symbolic/shared/libebm/common_c/common_c.h`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/common_c/logging.c` & `interpret-core-0.4.1/symbolic/shared/libebm/common_c/logging.c`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/common_c/logging.h` & `interpret-core-0.4.1/symbolic/shared/libebm/common_c/logging.h`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/common_cpp/common_cpp.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/common_cpp/common_cpp.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/Directory.Build.targets` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/Directory.Build.targets`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/Objective.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/Objective.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/Objective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/Objective.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -688,15 +688,15 @@
 
 
 #define OBJECTIVE_CONSTANTS_BOILERPLATE(__EBM_TYPE, __MAXIMIZE_METRIC, __LINK_FUNCTION) \
    public: \
       static constexpr bool k_bRmse = false; \
       static constexpr BoolEbm k_bMaximizeMetric = (__MAXIMIZE_METRIC); \
       static constexpr LinkEbm k_linkFunction = (__LINK_FUNCTION); \
-      static constexpr OutputType k_outputType = ConvertOutputType(k_linkFunction); \
+      static constexpr OutputType k_outputType = GetOutputType(k_linkFunction); \
       static ErrorEbm StaticApplyUpdate(const Objective * const pThis, ApplyUpdateBridge * const pData) { \
          return (static_cast<const __EBM_TYPE<TFloat> *>(pThis))->ParentApplyUpdate<const __EBM_TYPE<TFloat>, TFloat>(pData); \
       } \
       template<typename T = void, typename std::enable_if<TFloat::bCpu, T>::type * = nullptr> \
       static double StaticFinishMetric(const Objective * const pThis, const double metricSum) { \
          return (static_cast<const __EBM_TYPE<TFloat> *>(pThis))->FinishMetric(metricSum); \
       } \
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/Registration.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/Registration.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/Registration.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/Registration.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/approximate_math.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/approximate_math.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/compute.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/compute.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/compute_stats.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/compute_stats.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/cpu_64.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_64.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj.filters` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/cpu_ebm/sse2_32.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/sse2_32.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/cuda_ebm/cuda_32.cu` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/cuda_32.cu`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_32.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_32.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassMultitaskObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassMultitaskObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/ExampleRegressionObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/ExampleRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/GammaDevianceRegressionObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/GammaDevianceRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/LogLossBinaryMultitaskObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossBinaryMultitaskObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/LogLossBinaryObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossBinaryObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/LogLossMulticlassObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossMulticlassObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/PoissonDevianceRegressionObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/PoissonDevianceRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/PseudoHuberRegressionObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/PseudoHuberRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/RmseLogLinkRegressionObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/RmseLogLinkRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/RmseRegressionObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/RmseRegressionObjective.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 template<typename TFloat>
 struct RmseRegressionObjective final : public RegressionObjective {
 public:
    static constexpr bool k_bRmse = true;
    static constexpr BoolEbm k_bMaximizeMetric = MINIMIZE_METRIC;
    static constexpr LinkEbm k_linkFunction = Link_identity;
-   static constexpr OutputType k_outputType = ConvertOutputType(k_linkFunction);
+   static constexpr OutputType k_outputType = GetOutputType(k_linkFunction);
    static ErrorEbm StaticApplyUpdate(const Objective * const pThis, ApplyUpdateBridge * const pData) {
       return (static_cast<const RmseRegressionObjective<TFloat> *>(pThis))->ParentApplyUpdate<const RmseRegressionObjective<TFloat>, TFloat>(pData);
    }
    template<typename T = void, typename std::enable_if<TFloat::bCpu, T>::type * = nullptr>
    static double StaticFinishMetric(const Objective * const pThis, const double metricSum) {
       return (static_cast<const RmseRegressionObjective<TFloat> *>(pThis))->FinishMetric(metricSum);
    }
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/TweedieDevianceRegressionObjective.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/TweedieDevianceRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/objectives/objective_registrations.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/objective_registrations.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/registration_exceptions.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/registration_exceptions.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/zoned_bridge_c_functions.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_c_functions.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/zoned_bridge_c_functions.h` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_c_functions.h`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute/zoned_bridge_cpp_functions.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_cpp_functions.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/compute_accessors.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/compute_accessors.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/dataset_shared.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/dataset_shared.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #include <stddef.h> // size_t, ptrdiff_t
 #include <string.h> // memcpy
 
 #include "logging.h" // EBM_ASSERT
 #include "common_c.h"
 
 #include "common_cpp.hpp" // IsConvertError
-#include "bridge_cpp.hpp" // k_regression
+#include "bridge_cpp.hpp" // GetCountItemsBitPacked
 
 #include "dataset_shared.hpp"
 
 namespace DEFINED_ZONE_NAME {
 #ifndef DEFINED_ZONE_NAME
 #error DEFINED_ZONE_NAME must be defined
 #endif // DEFINED_ZONE_NAME
@@ -2186,15 +2186,15 @@
 
    const TargetDataSetShared * pTargetDataSetShared =
       reinterpret_cast<const TargetDataSetShared *>(pDataSetShared + iMem);
 
    const SharedStorageDataType id = pTargetDataSetShared->m_id;
    EBM_ASSERT(IsTarget(id));
 
-   ptrdiff_t cClasses = k_regression;
+   ptrdiff_t cClasses = ptrdiff_t { OutputType_Regression };
    const void * pRet = reinterpret_cast<const void *>(pTargetDataSetShared + 1);
    if(IsClassificationTarget(id)) {
       const ClassificationTargetDataSetShared * const pClassificationTargetDataSetShared =
          reinterpret_cast<const ClassificationTargetDataSetShared *>(pRet);
 
       const SharedStorageDataType countClasses = pClassificationTargetDataSetShared->m_cClasses;
       if(IsConvertError<ptrdiff_t>(countClasses)) {
@@ -2268,15 +2268,15 @@
 
          const TargetDataSetShared * pTargetDataSetShared =
             reinterpret_cast<const TargetDataSetShared *>(static_cast<const char *>(dataSet) + iOffsetCur);
 
          const SharedStorageDataType id = pTargetDataSetShared->m_id;
          EBM_ASSERT(IsTarget(id));
 
-         IntEbm countClasses = IntEbm { -1 };
+         IntEbm countClasses = IntEbm { OutputType_Regression };
          if(IsClassificationTarget(id)) {
             const ClassificationTargetDataSetShared * const pClassificationTargetDataSetShared =
                reinterpret_cast<const ClassificationTargetDataSetShared *>(pTargetDataSetShared + 1);
 
             const SharedStorageDataType cClasses = pClassificationTargetDataSetShared->m_cClasses;
 
             if(IsConvertError<IntEbm>(cClasses)) {
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/dataset_shared.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/dataset_shared.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/debug_ebm.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/debug_ebm.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/ebm_internal.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/ebm_internal.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/ebm_stats.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/ebm_stats.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/inc/libebm.h` & `interpret-core-0.4.1/symbolic/shared/libebm/inc/libebm.h`

 * *Files 1% similar despite different names*

```diff
@@ -199,31 +199,31 @@
 // https://www.sagepub.com/sites/default/files/upm-binaries/21121_Chapter_15.pdf
 // https://www.rdocumentation.org/packages/VGAM/versions/1.1-8/topics/Links
 #define Link_ERROR                                 (LINK_CAST(0))
 // uses link param potentially
 #define Link_custom_regression                     (LINK_CAST(1))
 #define Link_custom_classification                 (LINK_CAST(2))
 #define Link_custom_ranking                        (LINK_CAST(3))
-#define Link_power                                 (LINK_CAST(4))  // Tweedie regression
+#define Link_power                                 (LINK_CAST(4))  // Tweedie regression (although we use log)
 // classification
 #define Link_logit                                 (LINK_CAST(5))  // Logistic regression
 #define Link_probit                                (LINK_CAST(6))  // Probit regression
 #define Link_cloglog                               (LINK_CAST(7))  // Complementary log-log regression
 #define Link_loglog                                (LINK_CAST(8))  // Log-log regression
 #define Link_cauchit                               (LINK_CAST(9))  // Cauchit regression
 // regression
-#define Link_identity                              (LINK_CAST(10))  // Linear regression
-#define Link_log                                   (LINK_CAST(11))  // Poisson regression
-#define Link_inverse                               (LINK_CAST(12)) // Gamma regression
+#define Link_identity                              (LINK_CAST(10)) // Linear regression
+#define Link_log                                   (LINK_CAST(11)) // Poisson regression
+#define Link_inverse                               (LINK_CAST(12)) // Gamma regression (although we use log)
 #define Link_inverse_square                        (LINK_CAST(13)) // Inverse Gaussian regression
 #define Link_sqrt                                  (LINK_CAST(14)) // Square root regression
 
-#define OutputType_Unknown                         (OUTPUT_TYPE_CAST(-3))
-#define OutputType_Ranking                         (OUTPUT_TYPE_CAST(-2))
-#define OutputType_Regression                      (OUTPUT_TYPE_CAST(-1))
+#define OutputType_Ranking                         (OUTPUT_TYPE_CAST(-3))
+#define OutputType_Regression                      (OUTPUT_TYPE_CAST(-2))
+#define OutputType_Unknown                         (OUTPUT_TYPE_CAST(-1))
 #define OutputType_GeneralClassification           (OUTPUT_TYPE_CAST(0))  // classification with unspecified # classes
 #define OutputType_MonoClassification              (OUTPUT_TYPE_CAST(1))  // degenerate case of predicting 1 class
 #define OutputType_BinaryClassification            (OUTPUT_TYPE_CAST(2))  // 2 classes
 #define OutputType_MulticlassPlus                  (OUTPUT_TYPE_CAST(3))  // 3+ classes (the value is the # of classes)
 
 // All our logging messages are pure ASCII (127 values), and therefore also conform to UTF-8
 typedef void (EBM_CALLING_CONVENTION * LogCallbackFunction)(TraceEbm traceLevel, const char * message);
@@ -393,23 +393,26 @@
 
 EBM_API_INCLUDE ErrorEbm EBM_CALLING_CONVENTION DetermineLinkFunction(
    BoolEbm isDifferentiallyPrivate,
    const char * objective,
    LinkEbm * linkOut,
    double * linkParamOut
 );
-EBM_API_INCLUDE const char * EBM_CALLING_CONVENTION GetLinkFunctionString(
+EBM_API_INCLUDE const char * EBM_CALLING_CONVENTION GetLinkFunctionStr(
    LinkEbm link
 );
 EBM_API_INCLUDE LinkEbm EBM_CALLING_CONVENTION GetLinkFunctionInt(
    const char * link
 );
-EBM_API_INCLUDE OutputType EBM_CALLING_CONVENTION GetOutputType(
+EBM_API_INCLUDE OutputType EBM_CALLING_CONVENTION GetOutputTypeInt(
    LinkEbm link
 );
+EBM_API_INCLUDE const char * EBM_CALLING_CONVENTION GetOutputTypeStr(
+   const char * link
+);
 
 EBM_API_INCLUDE ErrorEbm EBM_CALLING_CONVENTION CreateBooster(
    void * rng,
    const void * dataSet,
    const BagEbm * bag,
    // TODO: add a baseScore parameter here so that we can initialize the mains boosting without initScores
    const double * initScores, // only samples with non-zeros in the bag are included
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/include_ordering.txt` & `interpret-core-0.4.1/symbolic/shared/libebm/include_ordering.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/interpret.sln` & `interpret-core-0.4.1/symbolic/shared/libebm/interpret.sln`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 		..\..\ACKNOWLEDGEMENTS.md = ..\..\ACKNOWLEDGEMENTS.md
 		..\..\azure-pipelines.yml = ..\..\azure-pipelines.yml
 		..\..\build.bat = ..\..\build.bat
 		..\..\build.sh = ..\..\build.sh
 		..\..\CHANGELOG.md = ..\..\CHANGELOG.md
 		..\..\CONTRIBUTING.md = ..\..\CONTRIBUTING.md
 		..\..\README.md = ..\..\README.md
+		..\..\scripts\release_process.txt = ..\..\scripts\release_process.txt
+		..\..\python\interpret\setup.py = ..\..\python\interpret\setup.py
 		vs_python_setup.txt = vs_python_setup.txt
 	EndProjectSection
 EndProject
 Project("{2150E333-8FDC-42A3-9474-1A3956D46DE8}") = "R", "R", "{3939C139-57E9-4CFD-AE75-710460EF590D}"
 	ProjectSection(SolutionItems) = preProject
 		..\..\R\build.R = ..\..\R\build.R
 		..\..\R\cran_formatted_licence.txt = ..\..\R\cran_formatted_licence.txt
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/interpretable_numerics.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/interpretable_numerics.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/libebm.vcxproj` & `interpret-core-0.4.1/symbolic/shared/libebm/libebm.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/libebm.vcxproj.filters` & `interpret-core-0.4.1/symbolic/shared/libebm/libebm.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/libebm_exports.def` & `interpret-core-0.4.1/symbolic/shared/libebm/libebm_exports.def`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,18 @@
   CheckDataSet
   ExtractDataSetHeader
   ExtractBinCounts
   ExtractTargetClasses
   SampleWithoutReplacement
   SampleWithoutReplacementStratified
   DetermineLinkFunction
-  GetLinkFunctionString
+  GetLinkFunctionStr
   GetLinkFunctionInt
-  GetOutputType
+  GetOutputTypeInt
+  GetOutputTypeStr
   CreateBooster
   CreateBoosterView
   FreeBooster
   GenerateTermUpdate
   GetTermUpdateSplits
   GetTermUpdate
   SetTermUpdate
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/libebm_exports.txt` & `interpret-core-0.4.1/symbolic/shared/libebm/libebm_exports.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,17 +29,18 @@
       CheckDataSet;
       ExtractDataSetHeader;
       ExtractBinCounts;
       ExtractTargetClasses;
       SampleWithoutReplacement;
       SampleWithoutReplacementStratified;
       DetermineLinkFunction;
-      GetLinkFunctionString;
+      GetLinkFunctionStr;
       GetLinkFunctionInt;
-      GetOutputType;
+      GetOutputTypeInt;
+      GetOutputTypeStr;
       CreateBooster;
       CreateBoosterView;
       FreeBooster;
       GenerateTermUpdate;
       GetTermUpdateSplits;
       GetTermUpdate;
       SetTermUpdate;
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/precompiled_header_cpp.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/precompiled_header_cpp.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/random.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/random.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/sampling.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/sampling.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/special/linux_wrap_functions.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/special/linux_wrap_functions.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/special/windows_DllMain.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/special/windows_DllMain.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/CutQuantileTest.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/CutQuantileTest.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/CutUniformTest.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/CutUniformTest.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/CutWinsorizedTest.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/CutWinsorizedTest.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/DiscretizeTest.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/DiscretizeTest.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/RandomStreamTest.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/RandomStreamTest.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/SuggestGraphBoundsTest.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/SuggestGraphBoundsTest.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/bit_packing_extremes.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/bit_packing_extremes.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       IntEbm exponential = static_cast<IntEbm>(std::pow(2, exponentialBins));
       // if we set the number of bins to be exponential, then we'll be just under a bit packing boundary.  4 bins means bits packs 00, 01, 10, and 11
       for(IntEbm iRange = IntEbm { -1 }; iRange <= IntEbm { 1 }; ++iRange) {
          IntEbm cBins = exponential + iRange; // check one less than the tight fit, the tight fit, and one above the tight fit
          // try everything from 0 samples to 65 samples because for bitpacks with 1 bit, we can have up to 64 packed into a single data value on a 
          // 64 bit machine
          for(size_t cSamples = 1; cSamples < 66; ++cSamples) {
-            TestApi test = TestApi(k_learningTypeRegression);
+            TestApi test = TestApi(OutputType_Regression);
             test.AddFeatures({ FeatureTest(cBins) });
             test.AddTerms({ { 0 } });
 
             std::vector<TestSample> trainingSamples;
             std::vector<TestSample> validationSamples;
             for(size_t iSample = 0; iSample < cSamples; ++iSample) {
                trainingSamples.push_back(TestSample({ cBins - 1 }, 7));
@@ -46,15 +46,15 @@
       IntEbm exponential = static_cast<IntEbm>(std::pow(2, exponentialBins));
       // if we set the number of bins to be exponential, then we'll be just under a bit packing boundary.  4 bins means bits packs 00, 01, 10, and 11
       for(IntEbm iRange = IntEbm { -1 }; iRange <= IntEbm { 1 }; ++iRange) {
          IntEbm cBins = exponential + iRange; // check one less than the tight fit, the tight fit, and one above the tight fit
          // try everything from 0 samples to 65 samples because for bitpacks with 1 bit, we can have up to 64 packed into a single data value on 
          // a 64 bit machine
          for(size_t cSamples = 1; cSamples < 66; ++cSamples) {
-            TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+            TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
             test.AddFeatures({ FeatureTest(cBins) });
             test.AddTerms({ { 0 } });
 
             std::vector<TestSample> trainingSamples;
             std::vector<TestSample> validationSamples;
             for(size_t iSample = 0; iSample < cSamples; ++iSample) {
                trainingSamples.push_back(TestSample({ cBins - 1 }, 0));
@@ -82,15 +82,15 @@
       IntEbm exponential = static_cast<IntEbm>(std::pow(2, exponentialBins));
       // if we set the number of bins to be exponential, then we'll be just under a bit packing boundary.  4 bins means bits packs 00, 01, 10, and 11
       for(IntEbm iRange = IntEbm { -1 }; iRange <= IntEbm { 1 }; ++iRange) {
          IntEbm cBins = exponential + iRange; // check one less than the tight fit, the tight fit, and one above the tight fit
          // try everything from 0 samples to 65 samples because for bitpacks with 1 bit, we can have up to 64 packed into a single data value on 
          // a 64 bit machine
          for(size_t cSamples = 1; cSamples < 66; ++cSamples) {
-            TestApi test = TestApi(k_learningTypeRegression);
+            TestApi test = TestApi(OutputType_Regression);
             test.AddFeatures({ FeatureTest(2), FeatureTest(cBins) });
 
             std::vector<TestSample> samples;
             for(size_t iSample = 0; iSample < cSamples; ++iSample) {
                samples.push_back(TestSample({ 0, cBins - 1 }, 7));
             }
             test.AddInteractionSamples(samples);
@@ -108,15 +108,15 @@
       IntEbm exponential = static_cast<IntEbm>(std::pow(2, exponentialBins));
       // if we set the number of bins to be exponential, then we'll be just under a bit packing boundary.  4 bins means bits packs 00, 01, 10, and 11
       for(IntEbm iRange = IntEbm { -1 }; iRange <= IntEbm { 1 }; ++iRange) {
          IntEbm cBins = exponential + iRange; // check one less than the tight fit, the tight fit, and one above the tight fit
          // try everything from 0 samples to 65 samples because for bitpacks with 1 bit, we can have up to 64 packed into a single data value on 
          // a 64 bit machine
          for(size_t cSamples = 1; cSamples < 66; ++cSamples) {
-            TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+            TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
             test.AddFeatures({ FeatureTest(2), FeatureTest(cBins) });
 
             std::vector<TestSample> samples;
             for(size_t iSample = 0; iSample < cSamples; ++iSample) {
                samples.push_back(TestSample({ 0, cBins - 1 }, 1));
             }
             test.AddInteractionSamples(samples);
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/boosting_unusual_inputs.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/boosting_unusual_inputs.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 #include "libebm.h"
 #include "libebm_test.hpp"
 
 static constexpr TestPriority k_filePriority = TestPriority::BoostingUnusualInputs;
 
 TEST_CASE("zero learning rate, boosting, regression") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({});
    test.AddTerms({ {} });
    test.AddTrainingSamples({ TestSample({}, 10) });
    test.AddValidationSamples({ TestSample({}, 12) });
    test.InitializeBoosting();
 
    double validationMetric = double { std::numeric_limits<double>::quiet_NaN() };
@@ -29,15 +29,15 @@
          termScore = test.GetBestTermScore(iTerm, {}, 0);
          CHECK(0 == termScore);
       }
    }
 }
 
 TEST_CASE("zero learning rate, boosting, binary") {
-   TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    test.AddFeatures({});
    test.AddTerms({ {} });
    test.AddTrainingSamples({ TestSample({}, 0) });
    test.AddValidationSamples({ TestSample({}, 0) });
    test.InitializeBoosting();
 
    double validationMetric = double { std::numeric_limits<double>::quiet_NaN() };
@@ -87,15 +87,15 @@
          termScore = test.GetBestTermScore(iTerm, {}, 2);
          CHECK(0 == termScore);
       }
    }
 }
 
 TEST_CASE("negative learning rate, boosting, regression") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({});
    test.AddTerms({ {} });
    test.AddTrainingSamples({ TestSample({}, 10) });
    test.AddValidationSamples({ TestSample({}, 12) });
    test.InitializeBoosting();
 
    double validationMetric = double { std::numeric_limits<double>::quiet_NaN() };
@@ -117,15 +117,15 @@
    }
    CHECK_APPROX(validationMetric, 43929458875.235196700295656826033);
    termScore = test.GetCurrentTermScore(0, {}, 0);
    CHECK_APPROX(termScore, -209581.55637813677);
 }
 
 TEST_CASE("negative learning rate, boosting, binary") {
-   TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    test.AddFeatures({});
    test.AddTerms({ {} });
    test.AddTrainingSamples({ TestSample({}, 0) });
    test.AddValidationSamples({ TestSample({}, 0) });
    test.InitializeBoosting();
 
    double validationMetric = double { std::numeric_limits<double>::quiet_NaN() };
@@ -196,15 +196,15 @@
    CHECK_APPROX_TOLERANCE(termScore, 1.23185585569831419, double { 1e-1 });
 }
 
 TEST_CASE("zero minSamplesLeaf, boosting, regression") {
    // TODO : call test.Boost many more times in a loop, and verify the output remains the same as previous runs
    // TODO : add classification binary and multiclass versions of this
 
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(2) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({
       TestSample({ 0 }, 10),
       TestSample({ 1 }, 10),
       });
    test.AddValidationSamples({ TestSample({ 1 }, 12) });
@@ -215,15 +215,15 @@
    double termScore;
    termScore = test.GetCurrentTermScore(0, { 0 }, 0);
    CHECK_APPROX(termScore, 0.1000000000000000);
    CHECK_APPROX(termScore, test.GetCurrentTermScore(0, { 1 }, 0));
 }
 
 TEST_CASE("weights are proportional, boosting, regression") {
-   TestApi test1 = TestApi(k_learningTypeRegression);
+   TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({ FeatureTest(2) });
    test1.AddTerms({ { 0 } });
    test1.AddTrainingSamples({
       TestSample({ 0 }, 10, FloatTickIncrementTest(0.3)),
       TestSample({ 1 }, 10, 0.3),
       });
    test1.AddValidationSamples({ 
@@ -233,15 +233,15 @@
    test1.InitializeBoosting();
    double validationMetric1 = test1.Boost(0).validationMetric;
    double termScore1;
    termScore1 = test1.GetCurrentTermScore(0, { 0 }, 0);
    CHECK_APPROX(termScore1, test1.GetCurrentTermScore(0, { 1 }, 0));
 
 
-   TestApi test2 = TestApi(k_learningTypeRegression);
+   TestApi test2 = TestApi(OutputType_Regression);
    test2.AddFeatures({ FeatureTest(2) });
    test2.AddTerms({ { 0 } });
    test2.AddTrainingSamples({
       TestSample({ 0 }, 10, FloatTickIncrementTest(2)),
       TestSample({ 1 }, 10, 2),
       });
    test2.AddValidationSamples({ 
@@ -251,15 +251,15 @@
    test2.InitializeBoosting();
    double validationMetric2 = test2.Boost(0).validationMetric;
    double termScore2;
    termScore2 = test2.GetCurrentTermScore(0, { 0 }, 0);
    CHECK_APPROX(termScore2, test2.GetCurrentTermScore(0, { 1 }, 0));
 
 
-   TestApi test3 = TestApi(k_learningTypeRegression);
+   TestApi test3 = TestApi(OutputType_Regression);
    test3.AddFeatures({ FeatureTest(2) });
    test3.AddTerms({ { 0 } });
    test3.AddTrainingSamples({
       TestSample({ 0 }, 10, 0),
       TestSample({ 1 }, 10, 0),
       });
    test3.AddValidationSamples({ 
@@ -276,15 +276,15 @@
    CHECK_APPROX(validationMetric1, validationMetric2);
    CHECK_APPROX(validationMetric1, validationMetric3);
    CHECK_APPROX(termScore1, termScore2);
    CHECK_APPROX(termScore1, termScore3);
 }
 
 TEST_CASE("weights are proportional, boosting, binary") {
-   TestApi test1 = TestApi(2);
+   TestApi test1 = TestApi(OutputType_BinaryClassification);
    test1.AddFeatures({ FeatureTest(2) });
    test1.AddTerms({ { 0 } });
    test1.AddTrainingSamples({
       TestSample({ 0 }, 0, FloatTickIncrementTest(0.3)),
       TestSample({ 1 }, 0, 0.3),
       });
    test1.AddValidationSamples({ 
@@ -294,15 +294,15 @@
    test1.InitializeBoosting();
    double validationMetric1 = test1.Boost(0).validationMetric;
    double termScore1;
    termScore1 = test1.GetCurrentTermScore(0, { 0 }, 0);
    CHECK_APPROX(termScore1, test1.GetCurrentTermScore(0, { 1 }, 0));
 
 
-   TestApi test2 = TestApi(2);
+   TestApi test2 = TestApi(OutputType_BinaryClassification);
    test2.AddFeatures({ FeatureTest(2) });
    test2.AddTerms({ { 0 } });
    test2.AddTrainingSamples({
       TestSample({ 0 }, 1, FloatTickIncrementTest(2)),
       TestSample({ 1 }, 1, 2),
       });
    test2.AddValidationSamples({ 
@@ -312,15 +312,15 @@
    test2.InitializeBoosting();
    double validationMetric2 = test2.Boost(0).validationMetric;
    double termScore2;
    termScore2 = test2.GetCurrentTermScore(0, { 0 }, 0);
    CHECK_APPROX(termScore2, test2.GetCurrentTermScore(0, { 1 }, 0));
 
 
-   TestApi test3 = TestApi(2);
+   TestApi test3 = TestApi(OutputType_BinaryClassification);
    test3.AddFeatures({ FeatureTest(2) });
    test3.AddTerms({ { 0 } });
    test3.AddTrainingSamples({
       TestSample({ 0 }, 0, 0),
       TestSample({ 1 }, 0, 0),
       });
    test3.AddValidationSamples({ 
@@ -398,15 +398,15 @@
    CHECK_APPROX(validationMetric1, validationMetric2);
    CHECK_APPROX(validationMetric1, validationMetric3);
    CHECK_APPROX(termScore1, termScore2);
    CHECK_APPROX(termScore1, termScore3);
 }
 
 TEST_CASE("weights totals equivalence, boosting, regression") {
-   TestApi test1 = TestApi(k_learningTypeRegression);
+   TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({ FeatureTest(2) });
    test1.AddTerms({ { 0 } });
    test1.AddTrainingSamples({
       TestSample({ 0 }, 10, 0.15),
       TestSample({ 0 }, 10, 0.15),
       TestSample({ 1 }, 12, 1.2),
       });
@@ -416,15 +416,15 @@
       });
    test1.InitializeBoosting();
    double validationMetric1 = test1.Boost(0).validationMetric;
    double termScore1;
    termScore1 = test1.GetCurrentTermScore(0, { 0 }, 0);
 
 
-   TestApi test2 = TestApi(k_learningTypeRegression);
+   TestApi test2 = TestApi(OutputType_Regression);
    test2.AddFeatures({ FeatureTest(2) });
    test2.AddTerms({ { 0 } });
    test2.AddTrainingSamples({
       TestSample({ 0 }, 10, 0.5),
       TestSample({ 1 }, 12, 2),
       });
    test2.AddValidationSamples({ 
@@ -438,15 +438,15 @@
    termScore2 = test2.GetCurrentTermScore(0, { 0 }, 0);
 
    CHECK_APPROX(validationMetric1, validationMetric2);
    CHECK_APPROX(termScore1, termScore2);
 }
 
 TEST_CASE("weights totals equivalence, boosting, binary") {
-   TestApi test1 = TestApi(2);
+   TestApi test1 = TestApi(OutputType_BinaryClassification);
    test1.AddFeatures({ FeatureTest(2) });
    test1.AddTerms({ { 0 } });
    test1.AddTrainingSamples({
       TestSample({ 0 }, 0, 0.15),
       TestSample({ 0 }, 0, 0.15),
       TestSample({ 1 }, 1, 1.2),
       });
@@ -456,15 +456,15 @@
       });
    test1.InitializeBoosting();
    double validationMetric1 = test1.Boost(0).validationMetric;
    double termScore1;
    termScore1 = test1.GetCurrentTermScore(0, { 0 }, 1);
 
 
-   TestApi test2 = TestApi(2);
+   TestApi test2 = TestApi(OutputType_BinaryClassification);
    test2.AddFeatures({ FeatureTest(2) });
    test2.AddTerms({ { 0 } });
    test2.AddTrainingSamples({
       TestSample({ 0 }, 0, 0.5),
       TestSample({ 1 }, 1, 2),
       });
    test2.AddValidationSamples({ 
@@ -526,15 +526,15 @@
 TEST_CASE("one leavesMax, boosting, regression") {
    // TODO : add classification binary and multiclass versions of this
 
    static const std::vector<IntEbm> k_leavesMax = {
       IntEbm { 1 }
    };
 
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(2) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({
       TestSample({ 0 }, 10),
       TestSample({ 1 }, 10),
       });
    test.AddValidationSamples({ TestSample({ 1 }, 12) });
@@ -545,15 +545,15 @@
    double termScore;
    termScore = test.GetCurrentTermScore(0, { 0 }, 0);
    CHECK_APPROX(termScore, 0.1000000000000000);
    CHECK_APPROX(termScore, test.GetCurrentTermScore(0, { 1 }, 0));
 }
 
 TEST_CASE("mono-classification") {
-   TestApi test = TestApi(1);
+   TestApi test = TestApi(OutputType_MonoClassification);
    test.AddFeatures({ FeatureTest(2) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({
       TestSample({ 0 }, 0),
       TestSample({ 1 }, 0),
    });
    test.AddValidationSamples({ 
@@ -598,15 +598,15 @@
    CHECK(Error_None == error);
 
    error = GetCurrentTermScores(test.GetBoosterHandle(), 0, nullptr);
    CHECK(Error_None == error);
 }
 
 TEST_CASE("Zero training samples, boosting, regression") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(2) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({});
    test.AddValidationSamples({ TestSample({ 1 }, 12) });
    test.InitializeBoosting();
 
    for(int iEpoch = 0; iEpoch < 1000; ++iEpoch) {
@@ -616,15 +616,15 @@
       termScore = test.GetCurrentTermScore(0, { 0 }, 0);
       CHECK(0 == termScore);
       CHECK_APPROX(termScore, test.GetCurrentTermScore(0, { 1 }, 0));
    }
 }
 
 TEST_CASE("Zero training samples, boosting, binary") {
-   TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    test.AddFeatures({ FeatureTest(2) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({});
    test.AddValidationSamples({ TestSample({ 1 }, 0) });
    test.InitializeBoosting();
 
    for(int iEpoch = 0; iEpoch < 1000; ++iEpoch) {
@@ -663,15 +663,15 @@
       termScore = test.GetCurrentTermScore(0, { 0 }, 2);
       CHECK(0 == termScore);
       CHECK_APPROX(termScore, test.GetCurrentTermScore(0, { 1 }, 2));
    }
 }
 
 TEST_CASE("Zero validation samples, boosting, regression") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(2) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({ TestSample({ 1 }, 10) });
    test.AddValidationSamples({});
    test.InitializeBoosting();
 
    for(int iEpoch = 0; iEpoch < 1000; ++iEpoch) {
@@ -692,15 +692,15 @@
       termScore = test.GetBestTermScore(0, { 0 }, 0);
       CHECK(0 == termScore);
       CHECK_APPROX(termScore, test.GetBestTermScore(0, { 1 }, 0));
    }
 }
 
 TEST_CASE("Zero validation samples, boosting, binary") {
-   TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    test.AddFeatures({ FeatureTest(2) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({ TestSample({ 1 }, 0) });
    test.AddValidationSamples({});
    test.InitializeBoosting();
 
    for(int iEpoch = 0; iEpoch < 1000; ++iEpoch) {
@@ -777,15 +777,15 @@
       CHECK(0 == termScore);
       CHECK_APPROX(termScore, test.GetBestTermScore(0, { 1 }, 2));
    }
 }
 
 TEST_CASE("features with 0 states, boosting") {
    // for there to be zero states, there can't be an training data or testing data since then those would be required to have a value for the state
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(0) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({});
    test.AddValidationSamples({});
    test.InitializeBoosting();
 
    double validationMetric = test.Boost(0).validationMetric;
@@ -801,37 +801,37 @@
    termScores[0] = 9.99;
    test.GetCurrentTermScoresRaw(0, termScores);
    CHECK(9.99 == termScores[0]); // the term is a tensor with zero values since one of the dimensions is non-existant
 }
 
 
 TEST_CASE("features with 1 state in various positions, boosting") {
-   TestApi test0 = TestApi(k_learningTypeRegression);
+   TestApi test0 = TestApi(OutputType_Regression);
    test0.AddFeatures({
       FeatureTest(1),
       FeatureTest(2),
       FeatureTest(2)
       });
    test0.AddTerms({ { 0 }, { 1 }, { 2 } });
    test0.AddTrainingSamples({ TestSample({ 0, 1, 1 }, 10) });
    test0.AddValidationSamples({ TestSample({ 0, 1, 1 }, 12) });
    test0.InitializeBoosting();
 
-   TestApi test1 = TestApi(k_learningTypeRegression);
+   TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({
       FeatureTest(2),
       FeatureTest(1),
       FeatureTest(2)
       });
    test1.AddTerms({ { 0 }, { 1 }, { 2 } });
    test1.AddTrainingSamples({ TestSample({ 1, 0, 1 }, 10) });
    test1.AddValidationSamples({ TestSample({ 1, 0, 1 }, 12) });
    test1.InitializeBoosting();
 
-   TestApi test2 = TestApi(k_learningTypeRegression);
+   TestApi test2 = TestApi(OutputType_Regression);
    test2.AddFeatures({
       FeatureTest(2),
       FeatureTest(2),
       FeatureTest(1)
       });
    test2.AddTerms({ { 0 }, { 1 }, { 2 } });
    test2.AddTrainingSamples({ TestSample({ 1, 1, 0 }, 10) });
@@ -884,27 +884,27 @@
       CHECK_APPROX(termScore201, termScore011);
       CHECK_APPROX(termScore210, termScore020);
       CHECK_APPROX(termScore211, termScore021);
    }
 }
 
 TEST_CASE("zero terms, boosting, regression") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({});
    test.AddTerms({});
    test.AddTrainingSamples({ TestSample({}, 10) });
    test.AddValidationSamples({ TestSample({}, 12) });
    test.InitializeBoosting();
 
    UNUSED(testCaseHidden); // this is a hidden parameter from TEST_CASE, but we don't test anything here.. we would just crash/assert if there was a problem
    // boosting isn't legal since we'd need to specify a term index
 }
 
 TEST_CASE("zero terms, boosting, binary") {
-   TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    test.AddFeatures({});
    test.AddTerms({});
    test.AddTrainingSamples({ TestSample({}, 1) });
    test.AddValidationSamples({ TestSample({}, 1) });
    test.InitializeBoosting();
 
    UNUSED(testCaseHidden); // this is a hidden parameter from TEST_CASE, but we don't test anything here.. we would just crash/assert if there was a problem
@@ -920,15 +920,15 @@
    test.InitializeBoosting();
 
    UNUSED(testCaseHidden); // this is a hidden parameter from TEST_CASE, but we don't test anything here.. we would just crash/assert if there was a problem
    // boosting isn't legal since we'd need to specify a term index
 }
 
 TEST_CASE("Term with zero features, boosting, regression") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({});
    test.AddTerms({ {} });
    test.AddTrainingSamples({ TestSample({}, 10) });
    test.AddValidationSamples({ TestSample({}, 12) });
    test.InitializeBoosting();
 
    double validationMetric = double { std::numeric_limits<double>::quiet_NaN() };
@@ -950,15 +950,15 @@
    }
    CHECK_APPROX(validationMetric, 4.001727036272099502004735302456);
    termScore = test.GetCurrentTermScore(0, {}, 0);
    CHECK_APPROX(termScore, 9.9995682875258822);
 }
 
 TEST_CASE("Term with zero features, boosting, binary") {
-   TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    test.AddFeatures({});
    test.AddTerms({ {} });
    test.AddTrainingSamples({ TestSample({}, 0) });
    test.AddValidationSamples({ TestSample({}, 0) });
    test.InitializeBoosting();
 
    double validationMetric = double { std::numeric_limits<double>::quiet_NaN() };
@@ -1025,29 +1025,29 @@
    termScore = test.GetCurrentTermScore(0, {}, 1) - zeroLogit1;
    CHECK_APPROX_TOLERANCE(termScore, -20.875723973004794, double { 1e-3 });
    termScore = test.GetCurrentTermScore(0, {}, 2) - zeroLogit1;
    CHECK_APPROX_TOLERANCE(termScore, -20.875723973004794, double { 1e-3 });
 }
 
 TEST_CASE("Term with one feature with one or two states is the exact same as zero terms, boosting, regression") {
-   TestApi testZeroDimensions = TestApi(k_learningTypeRegression);
+   TestApi testZeroDimensions = TestApi(OutputType_Regression);
    testZeroDimensions.AddFeatures({});
    testZeroDimensions.AddTerms({ {} });
    testZeroDimensions.AddTrainingSamples({ TestSample({}, 10) });
    testZeroDimensions.AddValidationSamples({ TestSample({}, 12) });
    testZeroDimensions.InitializeBoosting();
 
-   TestApi testOneState = TestApi(k_learningTypeRegression);
+   TestApi testOneState = TestApi(OutputType_Regression);
    testOneState.AddFeatures({ FeatureTest(1) });
    testOneState.AddTerms({ { 0 } });
    testOneState.AddTrainingSamples({ TestSample({ 0 }, 10) });
    testOneState.AddValidationSamples({ TestSample({ 0 }, 12) });
    testOneState.InitializeBoosting();
 
-   TestApi testTwoStates = TestApi(k_learningTypeRegression);
+   TestApi testTwoStates = TestApi(OutputType_Regression);
    testTwoStates.AddFeatures({ FeatureTest(2) });
    testTwoStates.AddTerms({ { 0 } });
    testTwoStates.AddTrainingSamples({ TestSample({ 1 }, 10) });
    testTwoStates.AddValidationSamples({ TestSample({ 1 }, 12) });
    testTwoStates.InitializeBoosting();
 
    for(int iEpoch = 0; iEpoch < 1000; ++iEpoch) {
@@ -1066,29 +1066,29 @@
          double termScoreTwoStates = testTwoStates.GetCurrentTermScore(iTerm, { 1 }, 0);
          CHECK_APPROX(termScoreZeroDimensions, termScoreTwoStates);
       }
    }
 }
 
 TEST_CASE("Term with one feature with one or two states is the exact same as zero terms, boosting, binary") {
-   TestApi testZeroDimensions = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi testZeroDimensions = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    testZeroDimensions.AddFeatures({});
    testZeroDimensions.AddTerms({ {} });
    testZeroDimensions.AddTrainingSamples({ TestSample({}, 0) });
    testZeroDimensions.AddValidationSamples({ TestSample({}, 0) });
    testZeroDimensions.InitializeBoosting();
 
-   TestApi testOneState = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi testOneState = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    testOneState.AddFeatures({ FeatureTest(1) });
    testOneState.AddTerms({ { 0 } });
    testOneState.AddTrainingSamples({ TestSample({ 0 }, 0) });
    testOneState.AddValidationSamples({ TestSample({ 0 }, 0) });
    testOneState.InitializeBoosting();
 
-   TestApi testTwoStates = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi testTwoStates = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    testTwoStates.AddFeatures({ FeatureTest(2) });
    testTwoStates.AddTerms({ { 0 } });
    testTwoStates.AddTrainingSamples({ TestSample({ 1 }, 0) });
    testTwoStates.AddValidationSamples({ TestSample({ 1 }, 0) });
    testTwoStates.InitializeBoosting();
 
    for(int iEpoch = 0; iEpoch < 1000; ++iEpoch) {
@@ -1166,39 +1166,39 @@
          double termScoreTwoStates2 = testTwoStates.GetCurrentTermScore(iTerm, { 1 }, 2);
          CHECK_APPROX(termScoreZeroDimensions2, termScoreTwoStates2);
       }
    }
 }
 
 TEST_CASE("3 dimensional term with one dimension reduced in different ways, boosting, regression") {
-   TestApi test0 = TestApi(k_learningTypeRegression);
+   TestApi test0 = TestApi(OutputType_Regression);
    test0.AddFeatures({ FeatureTest(1), FeatureTest(2), FeatureTest(2) });
    test0.AddTerms({ { 0, 1, 2 } });
    test0.AddTrainingSamples({
       TestSample({ 0, 0, 0 }, 9),
       TestSample({ 0, 1, 0 }, 10),
       TestSample({ 0, 0, 1 }, 11),
       TestSample({ 0, 1, 1 }, 12),
       });
    test0.AddValidationSamples({ TestSample({ 0, 1, 0 }, 12) });
    test0.InitializeBoosting();
 
-   TestApi test1 = TestApi(k_learningTypeRegression);
+   TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({ FeatureTest(2), FeatureTest(1), FeatureTest(2) });
    test1.AddTerms({ { 0, 1, 2 } });
    test1.AddTrainingSamples({
       TestSample({ 0, 0, 0 }, 9),
       TestSample({ 0, 0, 1 }, 10),
       TestSample({ 1, 0, 0 }, 11),
       TestSample({ 1, 0, 1 }, 12),
       });
    test1.AddValidationSamples({ TestSample({ 0, 0, 1 }, 12) });
    test1.InitializeBoosting();
 
-   TestApi test2 = TestApi(k_learningTypeRegression);
+   TestApi test2 = TestApi(OutputType_Regression);
    test2.AddFeatures({ FeatureTest(2), FeatureTest(2), FeatureTest(1) });
    test2.AddTerms({ { 0, 1, 2 } });
    test2.AddTrainingSamples({
       TestSample({ 0, 0, 0 }, 9),
       TestSample({ 1, 0, 0 }, 10),
       TestSample({ 0, 1, 0 }, 11),
       TestSample({ 1, 1, 0 }, 12),
@@ -1435,15 +1435,15 @@
    static constexpr IntEbm cStates = 7;
    static const std::vector<IntEbm> k_leavesMax = {
       IntEbm { 3 },
       IntEbm { 3 },
       IntEbm { 3 }
    };
 
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(cStates), FeatureTest(cStates), FeatureTest(cStates) });
    test.AddTerms({ { 0, 1, 2 } });
    std::vector<TestSample> samples;
    for(IntEbm i0 = 0; i0 < cStates; ++i0) {
       for(IntEbm i1 = 0; i1 < cStates; ++i1) {
          for(IntEbm i2 = 0; i2 < cStates; ++i2) {
             if(i0 == i1 && i0 == i2) {
@@ -1555,15 +1555,15 @@
 }
 
 TEST_CASE("Random splitting, no splits, binary, sums") {
    static const std::vector<IntEbm> k_leavesMax = {
       IntEbm { 3 }
    };
 
-   TestApi test = TestApi(2);
+   TestApi test = TestApi(OutputType_BinaryClassification);
    test.AddFeatures({ FeatureTest(1) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({
       TestSample({ 0 }, 0),
       TestSample({ 0 }, 0),
       TestSample({ 0 }, 1),
       TestSample({ 0 }, 1),
@@ -1596,15 +1596,15 @@
 
 TEST_CASE("zero gain, boosting, regression") {
    // construct a case where there should be zero gain and test that we get zero.
 
    // we start with a singular bin that has 5 cases, and split it to two bins with 2 and 3 cases respectively.
    // We can arbitrarily set the gradient totals to 4 and 7, and then calculate what the 
 
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(2) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({
       TestSample({ 0 }, 10.75, 1.5),
       TestSample({ 1 }, 10.75, 2.25),
       });
    test.AddValidationSamples({ });
@@ -1615,28 +1615,28 @@
 }
 
 TEST_CASE("pair and main gain identical, boosting, regression") {
    // if we have a scenario where boosting has gain in the split in one dimension, but the gain
    // for the split on both sides into the pair are zero, then the gain from the pair boosting
    // should be identical to the gain from the main if we were to combine the pairs into mains
 
-   TestApi test1 = TestApi(k_learningTypeRegression);
+   TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test1.AddTerms({ { 0, 1 } });
    test1.AddTrainingSamples({
       TestSample({ 0, 0 }, 10.75, 1.5),
       TestSample({ 0, 1 }, 10.75, 2.25),
       TestSample({ 1, 0 }, 11.25, 3.25),
       TestSample({ 1, 1 }, 11.25, 4.5),
       });
    test1.AddValidationSamples({});
    test1.InitializeBoosting(0);
    const double gainAvg1 = test1.Boost(0).gainAvg;
 
-   TestApi test2 = TestApi(k_learningTypeRegression);
+   TestApi test2 = TestApi(OutputType_Regression);
    test2.AddFeatures({ FeatureTest(2) });
    test2.AddTerms({ { 0 } });
    test2.AddTrainingSamples({
       TestSample({ 0 }, 10.75, 1.5 + 2.25),
       TestSample({ 1 }, 11.25, 3.25 + 4.5),
       });
    test2.AddValidationSamples({});
@@ -1644,15 +1644,15 @@
 
    double gainAvg2 = test2.Boost(0).gainAvg;
 
    CHECK_APPROX(gainAvg1, gainAvg2);
 }
 
 TEST_CASE("tweedie, boosting") {
-   TestApi test = TestApi(k_learningTypeRegression, EBM_FALSE, "tweedie_deviance:variance_power=1.3");
+   TestApi test = TestApi(OutputType_Regression, EBM_FALSE, "tweedie_deviance:variance_power=1.3");
    test.AddFeatures({ FeatureTest(1) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({ TestSample({ 0 }, 10) });
    test.AddValidationSamples({ TestSample({ 0 }, 12) });
    test.InitializeBoosting();
 
    double validationMetric = double { std::numeric_limits<double>::quiet_NaN() };
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/dataset_shared_test.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/dataset_shared_test.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/include_c.c` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/include_c.c`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/interaction_unusual_inputs.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/interaction_unusual_inputs.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 #include "libebm.h"
 #include "libebm_test.hpp"
 
 static constexpr TestPriority k_filePriority = TestPriority::InteractionUnusualInputs;
 
 TEST_CASE("Zero interaction samples, interaction, regression") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(2) });
    test.AddInteractionSamples({});
    test.InitializeInteraction();
 
    double metricReturn = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == metricReturn);
 }
 
 TEST_CASE("Zero interaction samples, interaction, binary") {
-   TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    test.AddFeatures({ FeatureTest(2) });
    test.AddInteractionSamples({});
    test.InitializeInteraction();
 
    double metricReturn = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == metricReturn);
 }
@@ -46,44 +46,44 @@
    test.InitializeInteraction();
 
    double validationMetric = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == validationMetric);
 }
 
 TEST_CASE("classification with 1 possible target, interaction") {
-   TestApi test = TestApi(1);
+   TestApi test = TestApi(OutputType_MonoClassification);
    test.AddFeatures({ FeatureTest(2) });
    test.AddInteractionSamples({ TestSample({ 1 }, 0) });
    test.InitializeInteraction();
 
    double validationMetric = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == validationMetric);
 }
 
 TEST_CASE("features with 0 states, interaction") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(0) });
    test.AddInteractionSamples({});
    test.InitializeInteraction();
 
    double validationMetric = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == validationMetric);
 }
 
 TEST_CASE("Term with zero features, interaction, regression") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({});
    test.AddInteractionSamples({ TestSample({}, 10) });
    test.InitializeInteraction();
    double metricReturn = test.TestCalcInteractionStrength({});
    CHECK(0 == metricReturn);
 }
 
 TEST_CASE("Term with zero features, interaction, binary") {
-   TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    test.AddFeatures({});
    test.AddInteractionSamples({ TestSample({}, 0) });
    test.InitializeInteraction();
    double metricReturn = test.TestCalcInteractionStrength({});
    CHECK(0 == metricReturn);
 }
 
@@ -93,24 +93,24 @@
    test.AddInteractionSamples({ TestSample({}, 0) });
    test.InitializeInteraction();
    double metricReturn = test.TestCalcInteractionStrength({});
    CHECK(0 == metricReturn);
 }
 
 TEST_CASE("Term with one feature with one state, interaction, regression") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(1) });
    test.AddInteractionSamples({ TestSample({ 0 }, 10) });
    test.InitializeInteraction();
    double metricReturn = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == metricReturn);
 }
 
 TEST_CASE("Term with one feature with one state, interaction, binary") {
-   TestApi test = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    test.AddFeatures({ FeatureTest(1) });
    test.AddInteractionSamples({ TestSample({ 0 }, 0) });
    test.InitializeInteraction();
    double metricReturn = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == metricReturn);
 }
 
@@ -120,37 +120,37 @@
    test.AddInteractionSamples({ TestSample({ 0 }, 0) });
    test.InitializeInteraction();
    double metricReturn = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == metricReturn);
 }
 
 TEST_CASE("weights are proportional, interaction, regression") {
-   TestApi test1 = TestApi(k_learningTypeRegression);
+   TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test1.AddInteractionSamples({ 
       TestSample({ 0, 0 }, 10.1, FloatTickIncrementTest(0.3)),
       TestSample({ 0, 1 }, 20.2, 0.3),
       TestSample({ 1, 0 }, 30.3, 0.3),
       TestSample({ 1, 1 }, 40.4, 0.3),
       });
    test1.InitializeInteraction();
    double metricReturn1 = test1.TestCalcInteractionStrength({ 0, 1 });
 
-   TestApi test2 = TestApi(k_learningTypeRegression);
+   TestApi test2 = TestApi(OutputType_Regression);
    test2.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test2.AddInteractionSamples({
       TestSample({ 0, 0 }, 10.1, FloatTickIncrementTest(2)),
       TestSample({ 0, 1 }, 20.2, 2),
       TestSample({ 1, 0 }, 30.3, 2),
       TestSample({ 1, 1 }, 40.4, 2),
       });
    test2.InitializeInteraction();
    double metricReturn2 = test2.TestCalcInteractionStrength({ 0, 1 });
 
-   TestApi test3 = TestApi(k_learningTypeRegression);
+   TestApi test3 = TestApi(OutputType_Regression);
    test3.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test3.AddInteractionSamples({
       TestSample({ 0, 0 }, 10.1, 0),
       TestSample({ 0, 1 }, 20.2, 0),
       TestSample({ 1, 0 }, 30.3, 0),
       TestSample({ 1, 1 }, 40.4, 0),
       });
@@ -158,37 +158,37 @@
    double metricReturn3 = test3.TestCalcInteractionStrength({ 0, 1 });
 
    CHECK_APPROX(metricReturn1, metricReturn2);
    CHECK_APPROX(metricReturn1, metricReturn3);
 }
 
 TEST_CASE("weights are proportional, interaction, binary") {
-   TestApi test1 = TestApi(2);
+   TestApi test1 = TestApi(OutputType_BinaryClassification);
    test1.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test1.AddInteractionSamples({
       TestSample({ 0, 0 }, 0, FloatTickIncrementTest(0.3)),
       TestSample({ 0, 1 }, 1, 0.3),
       TestSample({ 1, 0 }, 1, 0.3),
       TestSample({ 1, 1 }, 0, 0.3),
       });
    test1.InitializeInteraction();
    double metricReturn1 = test1.TestCalcInteractionStrength({ 0, 1 });
 
-   TestApi test2 = TestApi(2);
+   TestApi test2 = TestApi(OutputType_BinaryClassification);
    test2.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test2.AddInteractionSamples({
       TestSample({ 0, 0 }, 0, FloatTickIncrementTest(2)),
       TestSample({ 0, 1 }, 1, 2),
       TestSample({ 1, 0 }, 1, 2),
       TestSample({ 1, 1 }, 0, 2),
       });
    test2.InitializeInteraction();
    double metricReturn2 = test2.TestCalcInteractionStrength({ 0, 1 });
 
-   TestApi test3 = TestApi(2);
+   TestApi test3 = TestApi(OutputType_BinaryClassification);
    test3.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test3.AddInteractionSamples({
       TestSample({ 0, 0 }, 0, 0),
       TestSample({ 0, 1 }, 1, 0),
       TestSample({ 1, 0 }, 1, 0),
       TestSample({ 1, 1 }, 0, 0),
       });
@@ -234,27 +234,27 @@
    double metricReturn3 = test3.TestCalcInteractionStrength({ 0, 1 });
 
    CHECK_APPROX(metricReturn1, metricReturn2);
    CHECK_APPROX(metricReturn1, metricReturn3);
 }
 
 TEST_CASE("weights totals equivalence, interaction, regression") {
-   TestApi test1 = TestApi(k_learningTypeRegression);
+   TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test1.AddInteractionSamples({
       TestSample({ 0, 0 }, 10.1, 0.15),
       TestSample({ 0, 0 }, 10.1, 0.15),
       TestSample({ 0, 1 }, 20.2, 0.3),
       TestSample({ 1, 0 }, 30.3, 0.3),
       TestSample({ 1, 1 }, 40.4, 0.3),
       });
    test1.InitializeInteraction();
    double metricReturn1 = test1.TestCalcInteractionStrength({ 0, 1 });
 
-   TestApi test2 = TestApi(k_learningTypeRegression);
+   TestApi test2 = TestApi(OutputType_Regression);
    test2.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test2.AddInteractionSamples({
       TestSample({ 0, 0 }, 10.1, 2),
       TestSample({ 0, 1 }, 20.2, 2),
       TestSample({ 1, 0 }, 30.3, 1),
       TestSample({ 1, 0 }, 30.3, 1),
       TestSample({ 1, 1 }, 40.4, 2),
@@ -262,27 +262,27 @@
    test2.InitializeInteraction();
    double metricReturn2 = test2.TestCalcInteractionStrength({ 0, 1 });
 
    CHECK_APPROX(metricReturn1, metricReturn2);
 }
 
 TEST_CASE("weights totals equivalence, interaction, binary") {
-   TestApi test1 = TestApi(2);
+   TestApi test1 = TestApi(OutputType_BinaryClassification);
    test1.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test1.AddInteractionSamples({
       TestSample({ 0, 0 }, 0, 0.3),
       TestSample({ 0, 1 }, 1, 0.15),
       TestSample({ 0, 1 }, 1, 0.15),
       TestSample({ 1, 0 }, 1, 0.3),
       TestSample({ 1, 1 }, 0, 0.3),
       });
    test1.InitializeInteraction();
    double metricReturn1 = test1.TestCalcInteractionStrength({ 0, 1 });
 
-   TestApi test2 = TestApi(2);
+   TestApi test2 = TestApi(OutputType_BinaryClassification);
    test2.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test2.AddInteractionSamples({
       TestSample({ 0, 0 }, 0, 2),
       TestSample({ 0, 1 }, 1, 2),
       TestSample({ 1, 0 }, 1, 2),
       TestSample({ 1, 1 }, 0, 1),
       TestSample({ 1, 1 }, 0, 1),
@@ -332,15 +332,15 @@
 
    // or:
    // 14  10
    // 16  12
 
    // we can use any random weights for impure inputs, so stress test this!
 
-   TestApi test1 = TestApi(k_learningTypeRegression);
+   TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test1.AddInteractionSamples({
       TestSample({ 0, 0 }, (3.0 + 11.0), 24.25),
       TestSample({ 0, 1 }, (3.0 + 7.0), 21.5),
       TestSample({ 1, 0 }, (5.0 + 11.0), 8.125),
       TestSample({ 1, 1 }, (5.0 + 7.0), 11.625),
       });
@@ -361,15 +361,15 @@
    // 2.5  20
    // 1.25 5
    //
    // pure:
    // -16  2
    //  32 -8
 
-   TestApi test1 = TestApi(k_learningTypeRegression);
+   TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test1.AddInteractionSamples({
       TestSample({ 0, 0 }, -16.0, 2.5),
       TestSample({ 0, 1 }, 2.0, 20),
       TestSample({ 1, 0 }, 32.0, 1.25),
       TestSample({ 1, 1 }, -8.0, 5),
       });
@@ -384,15 +384,15 @@
    // 3 + 11   3 + 7
    // 5 + 11   5 + 7
 
    // or:
    // 14  10
    // 16  12
 
-   TestApi test2 = TestApi(k_learningTypeRegression);
+   TestApi test2 = TestApi(OutputType_Regression);
    test2.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test2.AddInteractionSamples({
       TestSample({ 0, 0 }, -16.0 + (3.0 + 11.0), 2.5),
       TestSample({ 0, 1 }, 2.0 + (3.0 + 7.0), 20),
       TestSample({ 1, 0 }, 32.0 + (5.0 + 11.0), 1.25),
       TestSample({ 1, 1 }, -8.0 + (5.0 + 7.0), 5),
       });
@@ -402,29 +402,29 @@
    CHECK_APPROX(metricReturn1, metricReturn2);
 }
 
 TEST_CASE("compare boosting gain to interaction strength, which should be identical") {
    // we use the same algorithm to calculate interaction strength (gain) and during boosting (gain again)
    // so we would expect them to generate the same response
 
-   TestApi test1 = TestApi(k_learningTypeRegression);
+   TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test1.AddInteractionSamples({
       TestSample({ 0, 0 }, 3, 232.24),
       TestSample({ 0, 1 }, 11, 12.124),
       TestSample({ 1, 0 }, 5, 85.1254),
       TestSample({ 1, 1 }, 7, 1.355),
       });
    test1.InitializeInteraction();
    const double interactionStrength = test1.TestCalcInteractionStrength({ 0, 1 }, InteractionFlags_EnableNewton);
 
    // we have a 2x2 matrix for boosting, which means there is only 1 cut point and it is known
    // so the gain should be from going from a singularity to the 4 quadrants
 
-   TestApi test2 = TestApi(k_learningTypeRegression);
+   TestApi test2 = TestApi(OutputType_Regression);
    test2.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test2.AddTerms({ { 0, 1 } });
    test2.AddTrainingSamples({
       TestSample({ 0, 0 }, 3, 232.24),
       TestSample({ 0, 1 }, 11, 12.124),
       TestSample({ 1, 0 }, 5, 85.1254),
       TestSample({ 1, 1 }, 7, 1.355),
@@ -433,15 +433,15 @@
    test2.InitializeBoosting(0);
    const double gainAvg = test2.Boost(0).gainAvg;
 
    CHECK_APPROX(interactionStrength, gainAvg);
 }
 
 TEST_CASE("tweedie, interaction") {
-   TestApi test = TestApi(k_learningTypeRegression, EBM_FALSE, "tweedie_deviance:variance_power=1.3");
+   TestApi test = TestApi(OutputType_Regression, EBM_FALSE, "tweedie_deviance:variance_power=1.3");
    test.AddFeatures({ FeatureTest(2), FeatureTest(2) });
    test.AddInteractionSamples({ 
       TestSample({ 0, 0 }, 10),
       TestSample({ 0, 1 }, 11),
       TestSample({ 1, 0 }, 13),
       TestSample({ 1, 1 }, 12)
    });
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.bat` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.bat`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
          exit(1);
       }
       return aScores[0];
    }
    if(static_cast<size_t>(m_cClasses) <= iClassOrZero) {
       exit(1);
    }
-   if(2 == m_cClasses) {
+   if(OutputType_BinaryClassification == m_cClasses) {
       // binary classification
 #ifdef EXPAND_BINARY_LOGITS
       if(m_iZeroClassificationLogit < 0) {
          return aScores[iClassOrZero];
       } else {
          if(static_cast<size_t>(m_iZeroClassificationLogit) == iClassOrZero) {
             return double { 0 };
@@ -215,15 +215,15 @@
       } else {
          return aScores[iClassOrZero] - aScores[m_iZeroClassificationLogit];
       }
    }
 }
 
 TestApi::TestApi(
-   const ptrdiff_t cClasses, 
+   const OutputType cClasses,
    const BoolEbm bDifferentiallyPrivate, 
    const char * const sObjective,
    const ptrdiff_t iZeroClassificationLogit
 ) :
    m_stage(Stage::Beginning),
    m_cClasses(cClasses),
    m_iZeroClassificationLogit(iZeroClassificationLogit),
@@ -235,15 +235,15 @@
    m_bNullValidationInitScores(true),
    m_boosterHandle(nullptr),
    m_bNullInteractionWeights(true),
    m_bNullInteractionInitScores(true),
    m_interactionHandle(nullptr) 
 {
    if(IsClassification(cClasses)) {
-      if(cClasses <= iZeroClassificationLogit) {
+      if(static_cast<ptrdiff_t>(cClasses) <= iZeroClassificationLogit) {
          exit(1);
       }
    } else {
       if(ptrdiff_t { -1 } != iZeroClassificationLogit) {
          exit(1);
       }
    }
@@ -343,15 +343,15 @@
                for(const double oneLogit : oneSample.m_initScores) {
                   if(std::isnan(oneLogit)) {
                      exit(1);
                   }
                   if(std::isinf(oneLogit)) {
                      exit(1);
                   }
-                  if(2 == m_cClasses) {
+                  if(OutputType_BinaryClassification == m_cClasses) {
                      // binary classification
 #ifdef EXPAND_BINARY_LOGITS
                      if(m_iZeroClassificationLogit < 0) {
                         m_trainingInitScores.push_back(oneLogit);
                      } else {
                         m_trainingInitScores.push_back(
                            oneLogit - oneSample.m_initScores[m_iZeroClassificationLogit]);
@@ -468,15 +468,15 @@
                for(const double oneLogit : oneSample.m_initScores) {
                   if(std::isnan(oneLogit)) {
                      exit(1);
                   }
                   if(std::isinf(oneLogit)) {
                      exit(1);
                   }
-                  if(2 == m_cClasses) {
+                  if(OutputType_BinaryClassification == m_cClasses) {
                      // binary classification
 #ifdef EXPAND_BINARY_LOGITS
                      if(m_iZeroClassificationLogit < 0) {
                         m_validationInitScores.push_back(oneLogit);
                      } else {
                         m_validationInitScores.push_back(
                            oneLogit - oneSample.m_initScores[m_iZeroClassificationLogit]);
@@ -880,27 +880,26 @@
                exit(1);
             }
             if(static_cast<IntEbm>(m_cClasses) <= targetInt) {
                exit(1);
             }
             m_interactionClassificationTargets.push_back(targetInt);
             if(!bNullInitScores) {
-               if(static_cast<size_t>(m_cClasses) !=
-                  oneSample.m_initScores.size()) {
+               if(static_cast<size_t>(m_cClasses) != oneSample.m_initScores.size()) {
                   exit(1);
                }
                ptrdiff_t iLogit = 0;
                for(const double oneLogit : oneSample.m_initScores) {
                   if(std::isnan(oneLogit)) {
                      exit(1);
                   }
                   if(std::isinf(oneLogit)) {
                      exit(1);
                   }
-                  if(2 == m_cClasses) {
+                  if(OutputType_BinaryClassification == m_cClasses) {
                      // binary classification
 #ifdef EXPAND_BINARY_LOGITS
                      if(m_iZeroClassificationLogit < 0) {
                         m_interactionInitScores.push_back(oneLogit);
                      } else {
                         m_interactionInitScores.push_back(
                            oneLogit - oneSample.m_initScores[m_iZeroClassificationLogit]);
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.hpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -132,24 +132,23 @@
       if(!bApproxEqualHidden) { \
          FAILED(valHidden, &testCaseHidden, std::string(" FAILED on \"" #val "(") + std::to_string(valHidden) + ") approx " #expected "\""); \
       } \
    } while( (void)0, 0)
 
 // EBM/interpret specific stuff below here!!
 
-static constexpr ptrdiff_t k_learningTypeRegression = ptrdiff_t { -1 };
-inline constexpr static bool IsClassification(const ptrdiff_t cClasses) {
-   return 0 <= cClasses;
+inline constexpr static bool IsClassification(const OutputType cClasses) {
+   return OutputType_GeneralClassification <= cClasses;
 }
 
-inline constexpr static size_t GetCountScores(const ptrdiff_t cClasses) {
+inline constexpr static size_t GetCountScores(const OutputType cClasses) {
 #ifdef EXPAND_BINARY_LOGITS
-   return ptrdiff_t { 1 } < cClasses ? static_cast<size_t>(cClasses) : (ptrdiff_t { 0 } == cClasses || ptrdiff_t { 1 } == cClasses ? size_t { 0 } : size_t { 1 });
+   return OutputType_BinaryClassification <= cClasses ? static_cast<size_t>(cClasses) : (ptrdiff_t { 0 } == cClasses || ptrdiff_t { 1 } == cClasses ? size_t { 0 } : size_t { 1 });
 #else // EXPAND_BINARY_LOGITS
-   return ptrdiff_t { 2 } < cClasses ? static_cast<size_t>(cClasses) : (ptrdiff_t { 0 } == cClasses || ptrdiff_t { 1 } == cClasses ? size_t { 0 } : size_t { 1 });
+   return OutputType_BinaryClassification < cClasses ? static_cast<size_t>(cClasses) : (ptrdiff_t { 0 } == cClasses || ptrdiff_t { 1 } == cClasses ? size_t { 0 } : size_t { 1 });
 #endif // EXPAND_BINARY_LOGITS
 }
 
 static constexpr SeedEbm k_seed = SeedEbm { -42 };
 
 class FeatureTest final {
 public:
@@ -288,15 +287,15 @@
       InteractionAdded, 
       InitializedInteraction
    };
 
    std::vector<unsigned char> m_rng;
 
    Stage m_stage;
-   const ptrdiff_t m_cClasses;
+   const OutputType m_cClasses;
    const ptrdiff_t m_iZeroClassificationLogit;
 
    BoolEbm m_bDifferentiallyPrivate;
    const char * m_sObjective;
 
    std::vector<BoolEbm> m_featureNominals;
    std::vector<IntEbm> m_featureBinCounts;
@@ -347,15 +346,15 @@
       const std::vector<size_t> perDimensionIndexArrayForBinnedFeatures,
       const size_t iClassOrZero)
       const;
 
 public:
 
    TestApi(
-      const ptrdiff_t cClasses, 
+      const OutputType cClasses,
       const BoolEbm m_bDifferentiallyPrivate = EBM_FALSE,
       const char * const m_sObjective = nullptr,
       const ptrdiff_t iZeroClassificationLogit = k_iZeroClassificationLogitDefault
    );
    ~TestApi();
 
    inline size_t GetCountTerms() const {
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.sh` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.sh`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.vcxproj` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/libebm_test.vcxproj.filters` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/random_test.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/random_test.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
          CHECK(cValidationSamplesVerified == cValidationSamples);
          CHECK(cTrainingSamplesVerified + cValidationSamplesVerified == cRandomSamples);
       }
    }
 }
 
 TEST_CASE("test random number generator equivalency") {
-   TestApi test = TestApi(k_learningTypeRegression);
+   TestApi test = TestApi(OutputType_Regression);
    test.AddFeatures({ FeatureTest(2) });
    test.AddTerms({ { 0 } });
 
    std::vector<TestSample> samples;
    for(int i = 0; i < 1000; ++i) {
       samples.push_back(TestSample({ 0 == (i * 7) % 3 }, i % 2));
    }
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/tests/rehydrate_booster.cpp` & `interpret-core-0.4.1/symbolic/shared/libebm/tests/rehydrate_booster.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 #include "libebm.h"
 #include "libebm_test.hpp"
 
 static constexpr TestPriority k_filePriority = TestPriority::Rehydration;
 
 TEST_CASE("Test Rehydration, boosting, regression") {
-   TestApi testContinuous = TestApi(k_learningTypeRegression);
+   TestApi testContinuous = TestApi(OutputType_Regression);
    testContinuous.AddFeatures({});
    testContinuous.AddTerms({ {} });
    testContinuous.AddTrainingSamples({ TestSample({}, 10) });
    testContinuous.AddValidationSamples({ TestSample({}, 12) });
    testContinuous.InitializeBoosting();
 
    double termScore0 = 0;
 
    double validationMetricContinuous;
    double termScoreContinuous;
    double validationMetricRestart;
    for(int iEpoch = 0; iEpoch < 1000; ++iEpoch) {
-      TestApi testRestart = TestApi(k_learningTypeRegression);
+      TestApi testRestart = TestApi(OutputType_Regression);
       testRestart.AddFeatures({});
       testRestart.AddTerms({ {} });
       testRestart.AddTrainingSamples({ TestSample({}, 10, 1, { termScore0 }) });
       testRestart.AddValidationSamples({ TestSample({}, 12, 1, { termScore0 }) });
       testRestart.InitializeBoosting();
 
       validationMetricRestart = testRestart.Boost(0).validationMetric;
@@ -37,29 +37,29 @@
       termScoreContinuous = testContinuous.GetCurrentTermScore(0, {}, 0);
       termScore0 += testRestart.GetCurrentTermScore(0, {}, 0);
       CHECK_APPROX(termScoreContinuous, termScore0);
    }
 }
 
 TEST_CASE("Test Rehydration, boosting, binary") {
-   TestApi testContinuous = TestApi(2, EBM_FALSE, nullptr, 0);
+   TestApi testContinuous = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    testContinuous.AddFeatures({});
    testContinuous.AddTerms({ {} });
    testContinuous.AddTrainingSamples({ TestSample({}, 0) });
    testContinuous.AddValidationSamples({ TestSample({}, 0) });
    testContinuous.InitializeBoosting();
 
    double termScore0 = 0;
    double termScore1 = 0;
 
    double validationMetricContinuous;
    double termScoreContinuous;
    double validationMetricRestart;
    for(int iEpoch = 0; iEpoch < 1000; ++iEpoch) {
-      TestApi testRestart = TestApi(2, EBM_FALSE, nullptr, 0);
+      TestApi testRestart = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
       testRestart.AddFeatures({});
       testRestart.AddTerms({ {} });
       testRestart.AddTrainingSamples({ TestSample({}, 0, 1, { termScore0, termScore1 }) });
       testRestart.AddValidationSamples({ TestSample({}, 0, 1, { termScore0, termScore1 }) });
       testRestart.InitializeBoosting();
 
       validationMetricRestart = testRestart.Boost(0).validationMetric;
```

### Comparing `interpret-core-0.4.0/symbolic/shared/libebm/vs_python_setup.txt` & `interpret-core-0.4.1/symbolic/shared/libebm/vs_python_setup.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/vis/package.json` & `interpret-core-0.4.1/symbolic/shared/vis/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.4.1'"}*

```diff
@@ -43,9 +43,9 @@
     },
     "scripts": {
         "build-dev": "webpack --mode development",
         "build-prod": "webpack --mode production",
         "clean": "rm dist/interpret-inline.js",
         "start": "webpack-dev-server --hot --mode development"
     },
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `interpret-core-0.4.0/symbolic/shared/vis/src/index.js` & `interpret-core-0.4.1/symbolic/shared/vis/src/index.js`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/vis/src/styles.scss` & `interpret-core-0.4.1/symbolic/shared/vis/src/styles.scss`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/symbolic/shared/vis/webpack.config.js` & `interpret-core-0.4.1/symbolic/shared/vis/webpack.config.js`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/api/test_base.py` & `interpret-core-0.4.1/tests/api/test_base.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/blackbox/test_permutationimportance.py` & `interpret-core-0.4.1/tests/blackbox/test_permutationimportance.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/ext/test_examples.py` & `interpret-core-0.4.1/tests/ext/test_examples.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/glassbox/ebm/research/test_group_importance.py` & `interpret-core-0.4.1/tests/glassbox/ebm/research/test_group_importance.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/glassbox/ebm/research/test_purify.py` & `interpret-core-0.4.1/tests/glassbox/ebm/research/test_purify.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/glassbox/ebm/test_bin.py` & `interpret-core-0.4.1/tests/glassbox/ebm/test_bin.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/glassbox/ebm/test_ebm.py` & `interpret-core-0.4.1/tests/glassbox/ebm/test_ebm.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/glassbox/ebm/test_ebm_utils.py` & `interpret-core-0.4.1/tests/glassbox/ebm/test_ebm_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/glassbox/ebm/test_merge_ebms.py` & `interpret-core-0.4.1/tests/glassbox/ebm/test_merge_ebms.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/glassbox/ebm/test_multiclass.py` & `interpret-core-0.4.1/tests/glassbox/ebm/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/glassbox/test_decisiontree.py` & `interpret-core-0.4.1/tests/glassbox/test_decisiontree.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/glassbox/test_linear.py` & `interpret-core-0.4.1/tests/glassbox/test_linear.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/greybox/test_treeinterpreter.py` & `interpret-core-0.4.1/tests/greybox/test_treeinterpreter.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/provider/test_providers.py` & `interpret-core-0.4.1/tests/provider/test_providers.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/test_develop.py` & `interpret-core-0.4.1/tests/test_develop.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/test_example_notebooks.py` & `interpret-core-0.4.1/tests/test_example_notebooks.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/test_explainers.py` & `interpret-core-0.4.1/tests/test_explainers.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/test_ext.py` & `interpret-core-0.4.1/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/test_extension_utils.py` & `interpret-core-0.4.1/tests/test_extension_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/test_mli_interop.py` & `interpret-core-0.4.1/tests/test_mli_interop.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/test_selenium.py` & `interpret-core-0.4.1/tests/test_selenium.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/tutils.py` & `interpret-core-0.4.1/tests/tutils.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/utils/test_SPOTgreedy.py` & `interpret-core-0.4.1/tests/utils/test_SPOTgreedy.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/utils/test_clean_simple.py` & `interpret-core-0.4.1/tests/utils/test_clean_simple.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/utils/test_clean_x.py` & `interpret-core-0.4.1/tests/utils/test_clean_x.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/utils/test_compressed_dataset.py` & `interpret-core-0.4.1/tests/utils/test_compressed_dataset.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/utils/test_explanation.py` & `interpret-core-0.4.1/tests/utils/test_explanation.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/utils/test_measure_interactions.py` & `interpret-core-0.4.1/tests/utils/test_measure_interactions.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/utils/test_native.py` & `interpret-core-0.4.1/tests/utils/test_native.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/visual/test_inline.py` & `interpret-core-0.4.1/tests/visual/test_inline.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.0/tests/visual/test_interactive.py` & `interpret-core-0.4.1/tests/visual/test_interactive.py`

 * *Files identical despite different names*

