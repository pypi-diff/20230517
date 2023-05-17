# Comparing `tmp/gantry-0.6.3.tar.gz` & `tmp/gantry-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry-0.6.3.tar", last modified: Tue May 16 04:41:47 2023, max compression
+gzip compressed data, was "gantry-0.6.4.tar", last modified: Wed May 17 00:34:14 2023, max compression
```

## Comparing `gantry-0.6.3.tar` & `gantry-0.6.4.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.025299 gantry-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-16 04:41:37.000000 gantry-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 04:41:37.000000 gantry-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-16 04:41:47.025299 gantry-0.6.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/alerts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/alerts/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/alerts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28655 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry/automations/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry/automations/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/automations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/automations/curators/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/curators.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/stock_curators.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/automations/triggers/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/triggers/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/data_generator/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/dataset/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/templates/load_script_template.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93878 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/query/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/gantry/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/gantry/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/distance/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/gantry/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/metric/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-16 04:41:46.000000 gantry-0.6.3/gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-16 04:41:47.000000 gantry-0.6.3/gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:41:46.000000 gantry-0.6.3/gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 04:41:46.000000 gantry-0.6.3/gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-16 04:41:46.000000 gantry-0.6.3/gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 04:41:46.000000 gantry-0.6.3/gantry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:41:47.025299 gantry-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-16 04:41:37.000000 gantry-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/tests/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/alerts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/alerts/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/alerts/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/tests/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/test_llm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/curator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/curator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/curator/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/curator/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/curator/test_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/data_generator/test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/dataset/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/dataset/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/dataset/test_gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/dataset/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   136361 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/distance/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/metric/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.092836 gantry-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-17 00:33:59.000000 gantry-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 00:33:59.000000 gantry-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-17 00:34:14.092836 gantry-0.6.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.068836 gantry-0.6.4/gantry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.068836 gantry-0.6.4/gantry/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/alerts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/alerts/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/alerts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.068836 gantry-0.6.4/gantry/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/applications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28655 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/applications/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16390 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/applications/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/applications/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/applications/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.068836 gantry-0.6.4/gantry/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.072836 gantry-0.6.4/gantry/automations/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/automations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.072836 gantry-0.6.4/gantry/automations/curators/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/curators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/curators/curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/curators/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/curators/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/curators/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/curators/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/curators/stock_curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.072836 gantry-0.6.4/gantry/automations/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/automations/triggers/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.072836 gantry-0.6.4/gantry/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/cli/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/cli/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/cli/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/cli/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.072836 gantry-0.6.4/gantry/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/data_generator/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.076836 gantry-0.6.4/gantry/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/dataset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/dataset/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/dataset/gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/dataset/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.076836 gantry-0.6.4/gantry/dataset/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/dataset/templates/load_script_template.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.076836 gantry-0.6.4/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93878 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/logger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/logger/event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/logger/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/logger/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.080836 gantry-0.6.4/gantry/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.080836 gantry-0.6.4/gantry/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/core/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/core/queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.080836 gantry-0.6.4/gantry/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/distance/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.080836 gantry-0.6.4/gantry/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/metric/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/query/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 00:33:59.000000 gantry-0.6.4/gantry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.068836 gantry-0.6.4/gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-17 00:34:14.000000 gantry-0.6.4/gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-17 00:34:14.000000 gantry-0.6.4/gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:34:14.000000 gantry-0.6.4/gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 00:34:14.000000 gantry-0.6.4/gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-17 00:34:14.000000 gantry-0.6.4/gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 00:34:14.000000 gantry-0.6.4/gantry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 00:34:14.092836 gantry-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-17 00:33:59.000000 gantry-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.080836 gantry-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.084836 gantry-0.6.4/tests/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/alerts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/alerts/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/alerts/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.084836 gantry-0.6.4/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/applications/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/applications/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/applications/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/applications/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/applications/test_llm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.084836 gantry-0.6.4/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/cli/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/cli/test_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/cli/test_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/cli/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.088836 gantry-0.6.4/tests/curator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/curator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/curator/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/curator/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/curator/test_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.088836 gantry-0.6.4/tests/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/data_generator/test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.088836 gantry-0.6.4/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/dataset/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/dataset/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/dataset/test_gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/dataset/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.088836 gantry-0.6.4/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/logger/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136361 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/logger/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/logger/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/logger/test_event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/logger/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/logger/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/logger/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.092836 gantry-0.6.4/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.092836 gantry-0.6.4/tests/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/core/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/core/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/core/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/core/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/core/test_queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/core/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.092836 gantry-0.6.4/tests/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/distance/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:34:14.092836 gantry-0.6.4/tests/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/metric/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/query/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-17 00:33:59.000000 gantry-0.6.4/tests/test_validator.py
```

### Comparing `gantry-0.6.3/LICENSE` & `gantry-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/PKG-INFO` & `gantry-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.3
+Version: 0.6.4
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.3/gantry/__init__.py` & `gantry-0.6.4/gantry/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/alerts/client.py` & `gantry-0.6.4/gantry/alerts/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/alerts/globals.py` & `gantry-0.6.4/gantry/alerts/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/alerts/main.py` & `gantry-0.6.4/gantry/alerts/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/api_client.py` & `gantry-0.6.4/gantry/api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/applications/client.py` & `gantry-0.6.4/gantry/applications/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/applications/core.py` & `gantry-0.6.4/gantry/applications/core.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/applications/llm.py` & `gantry-0.6.4/gantry/applications/llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import atexit
 import json
 import logging
+import os
 import uuid
 from dataclasses import dataclass
 from queue import Queue
 from typing import Callable, Dict, List, Optional, Union
 
 import backoff
 import requests
 
+from gantry.const import PROD_API_URL
 from gantry.exceptions import GantryRequestException
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal  # type: ignore
 
@@ -145,15 +147,15 @@
         on_giveup=backoff_giveup_handler,
         giveup=non_retry_error,
         jitter=None,
     )
     def send_completion_event(self, event: Dict) -> None:
         response = self._api_client.request(
             "POST",
-            "/api/v1/completions",
+            "/api/v1/logging/completions",
             json=event,
             raise_for_status=True,
         )
         if response.get("response") != "ok":
             logger.error("Failed to log events. Response = %s", response)
 
     def _join(self):
@@ -274,18 +276,21 @@
             json={
                 "configuration_data": configuration_data,
                 "description": description,
             },
             raise_for_status=True,
         )
         logger.info(
-            "Version created for application '%s' with prompt template:\n'%s'",
+            "Version %s created for application '%s'",
+            res["data"]["version"],
             self._name,
-            prompt_template,
         )
+        host = os.environ.get("GANTRY_LOGS_LOCATION", PROD_API_URL)
+        link_to_versions = "{}/applications/{}/versions/".format(host, self._name)
+        logger.info("See the new version here: %s", link_to_versions)
 
         return VersionDetails(
             config=configuration_data,
             description=description,
             app_name=self._name,
             version_id=uuid.UUID(res["data"]["id"]),
             version_number=res["data"]["version"],
@@ -397,30 +402,41 @@
         Log request/response OpenAI pair into Gantry.
 
         Example usage:
 
         .. code-block:: python
 
             import gantry
+            from gantry.applications.llm_utils import fill_prompt
+            import openai
+            from openai.util import convert_to_dict
+
+            gantry.init()
+            my_llm_app = gantry.get_application("my-llm-app")
+
+            version = my_llm_app.get_version("test")
+            config = version.config
+            prompt = config['prompt']
+
+            def generate(values):
+                filled_in_prompt = fill_prompt(prompt, values)
+                request = {
+                    "model": "text-davinci-002",
+                    "prompt": filled_in_prompt,
+                }
+                results = openai.Completion.create(**request)
+
+                my_llm_app.log_completion(
+                    open_ai_api_request=request,
+                    open_ai_api_response=convert_to_dict(results),
+                    request_attributes={"prompt_values": values},
+                    version=version.version_number,
+                )
 
-            my_llm_app = gantry.get_application("my_llm_app")
-            my_llm_app.log_completion(
-                open_ai_api_request={
-                    ...
-                },
-                open_ai_api_response={
-                    ...
-                },
-                request_attributes={"additional_input": "value"},
-                response_attributes={"additional_output": "value"},
-                selected_choice_index=1,
-                session_id="some-id",
-                tags={"additionl_tag": "yes"},
-                version=10,
-            )
+                return results
 
         For more details on request/response content, see `OpenAI API Reference for Completion
         <https://platform.openai.com/docs/api-reference/completions/create>`_.
 
         Args:
             open_ai_api_request (dict): The OpenAI request.
                 For more details on content, see `OpenAI API Reference for Completion
```

### Comparing `gantry-0.6.3/gantry/applications/llm_utils.py` & `gantry-0.6.4/gantry/applications/llm_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/applications/main.py` & `gantry-0.6.4/gantry/applications/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/automations/actions/actions.py` & `gantry-0.6.4/gantry/automations/actions/actions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/automations/automations.py` & `gantry-0.6.4/gantry/automations/automations.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/automations/curators/__init__.py` & `gantry-0.6.4/gantry/automations/curators/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/automations/curators/curators.py` & `gantry-0.6.4/gantry/automations/curators/curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/automations/curators/main.py` & `gantry-0.6.4/gantry/automations/curators/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/automations/curators/models.py` & `gantry-0.6.4/gantry/automations/curators/models.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/automations/curators/selectors.py` & `gantry-0.6.4/gantry/automations/curators/selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/automations/curators/stock_curators.py` & `gantry-0.6.4/gantry/automations/curators/stock_curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/automations/main.py` & `gantry-0.6.4/gantry/automations/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/automations/triggers/triggers.py` & `gantry-0.6.4/gantry/automations/triggers/triggers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/cli/application.py` & `gantry-0.6.4/gantry/cli/application.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/cli/bucket.py` & `gantry-0.6.4/gantry/cli/bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/cli/data_connector.py` & `gantry-0.6.4/gantry/cli/data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/cli/labeling.py` & `gantry-0.6.4/gantry/cli/labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/cli/main.py` & `gantry-0.6.4/gantry/cli/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/cli/projection.py` & `gantry-0.6.4/gantry/cli/projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/cli/secret.py` & `gantry-0.6.4/gantry/cli/secret.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/data_generator/data_generator.py` & `gantry-0.6.4/gantry/data_generator/data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/dataset/client.py` & `gantry-0.6.4/gantry/dataset/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/dataset/constants.py` & `gantry-0.6.4/gantry/dataset/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/dataset/gantry_dataset.py` & `gantry-0.6.4/gantry/dataset/gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/dataset/main.py` & `gantry-0.6.4/gantry/dataset/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/dataset/templates/load_script_template.py.jinja` & `gantry-0.6.4/gantry/dataset/templates/load_script_template.py.jinja`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/exceptions.py` & `gantry-0.6.4/gantry/exceptions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/logger/client.py` & `gantry-0.6.4/gantry/logger/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/logger/constants.py` & `gantry-0.6.4/gantry/logger/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/logger/consumer.py` & `gantry-0.6.4/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/logger/event_builder.py` & `gantry-0.6.4/gantry/logger/event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/logger/main.py` & `gantry-0.6.4/gantry/logger/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/logger/stores.py` & `gantry-0.6.4/gantry/logger/stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/logger/types.py` & `gantry-0.6.4/gantry/logger/types.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/logger/utils.py` & `gantry-0.6.4/gantry/logger/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/__init__.py` & `gantry-0.6.4/gantry/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/client.py` & `gantry-0.6.4/gantry/query/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/core/dataframe.py` & `gantry-0.6.4/gantry/query/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/core/distance.py` & `gantry-0.6.4/gantry/query/core/distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/core/metric.py` & `gantry-0.6.4/gantry/query/core/metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/core/queryframe.py` & `gantry-0.6.4/gantry/query/core/queryframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,22 @@
             if end_time_ret is None:
                 raise ValueError("Invalid end_time: {}".format(end_time))
         else:
             end_time_ret = end_time
 
         return start_time_ret, end_time_ret
 
+    @staticmethod
+    def _convert_to_bool_helper(x):
+        if isinstance(x, bool):
+            return x
+        if x:
+            return strtobool(str(x))
+        return None
+
     def _prepare_pandas_dataframe(
         self,
         data: List[Dict[str, Any]],
         column: Optional[str] = None,
     ) -> pd.DataFrame:
         df = pd.DataFrame.from_records(data)
         if df.empty:
@@ -158,17 +166,15 @@
         for col in df.columns:
             dtype = self._get_dtype(col)
 
             # Bool columns from druid can be "true," "false," or None.
             # To convert to pandas boolean type we must first
             # convert to python bool where we can.
             if dtype == "bool":
-                df[col] = (
-                    df[col].map(lambda x: strtobool(x) if x else None).astype(pd.BooleanDtype())
-                )
+                df[col] = df[col].map(self._convert_to_bool_helper).astype(pd.BooleanDtype())
 
             if dtype == "str":
                 df[col] = df[col].astype(pd.StringDtype())
 
             if dtype == "category":
                 df[col] = df[col].astype(pd.CategoricalDtype())
```

### Comparing `gantry-0.6.3/gantry/query/core/utils.py` & `gantry-0.6.4/gantry/query/core/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/distance/main.py` & `gantry-0.6.4/gantry/query/distance/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/globals.py` & `gantry-0.6.4/gantry/query/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/main.py` & `gantry-0.6.4/gantry/query/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/metric/main.py` & `gantry-0.6.4/gantry/query/metric/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/query/time_window.py` & `gantry-0.6.4/gantry/query/time_window.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/serializers.py` & `gantry-0.6.4/gantry/serializers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/utils.py` & `gantry-0.6.4/gantry/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry/validators.py` & `gantry-0.6.4/gantry/validators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/gantry.egg-info/PKG-INFO` & `gantry-0.6.4/gantry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.3
+Version: 0.6.4
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.3/gantry.egg-info/SOURCES.txt` & `gantry-0.6.4/gantry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/setup.py` & `gantry-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/alerts/test_client.py` & `gantry-0.6.4/tests/alerts/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/alerts/test_main.py` & `gantry-0.6.4/tests/alerts/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/applications/test_client.py` & `gantry-0.6.4/tests/applications/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/applications/test_core.py` & `gantry-0.6.4/tests/applications/test_core.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/applications/test_llm.py` & `gantry-0.6.4/tests/applications/test_llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,14 @@
     ],
 )
 def test_create_version(
     test_llm_application: CompletionApplication, version_kwargs: dict, configuration_data: dict
 ):
     version_id = uuid.uuid4()
     description = "test description"
-
     with responses.RequestsMock() as resp:
         resp.add(
             resp.POST,
             (
                 f"{HOST}/api/v1/cms/{test_llm_application._name}/configurations/"
                 f"{test_llm_application._configuration_name}/versions"
             ),
@@ -333,36 +332,36 @@
 
 
 def test_completion_api_log_store_consumer_func(test_api_client):
     log_store = CompletionAPILogStore(test_api_client, consumer_factory=TestingBatchConsumer)
     with responses.RequestsMock() as resp:
         resp.add(
             resp.POST,
-            f"{HOST}/api/v1/completions",
+            f"{HOST}/api/v1/logging/completions",
             json={"response": "ok"},
             headers={"Content-Type": "application/json"},
             match=[matchers.json_params_matcher({"foo": "bar"})],
         )
         resp.add(
             resp.POST,
-            f"{HOST}/api/v1/completions",
+            f"{HOST}/api/v1/logging/completions",
             json={"response": "ok"},
             headers={"Content-Type": "application/json"},
             match=[matchers.json_params_matcher({"bar": "baz"})],
         )
 
         log_store.consumer_func([b'{"foo": "bar"}', b'{"bar": "baz"}'])
 
 
 def test_completion_api_log_store_send_completion_event(test_api_client):
     log_store = CompletionAPILogStore(test_api_client, consumer_factory=TestingBatchConsumer)
     event = {"foo": "bar"}
     with responses.RequestsMock() as resp:
         resp.add(
             resp.POST,
-            f"{HOST}/api/v1/completions",
+            f"{HOST}/api/v1/logging/completions",
             json={"response": "ok"},
             headers={"Content-Type": "application/json"},
             match=[matchers.json_params_matcher({"foo": "bar"})],
         )
 
         log_store.send_completion_event(event)
```

### Comparing `gantry-0.6.3/tests/applications/test_llm_utils.py` & `gantry-0.6.4/tests/applications/test_llm_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/cli/test_bucket.py` & `gantry-0.6.4/tests/cli/test_bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/cli/test_data_connector.py` & `gantry-0.6.4/tests/cli/test_data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/cli/test_labeling.py` & `gantry-0.6.4/tests/cli/test_labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/cli/test_projection.py` & `gantry-0.6.4/tests/cli/test_projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/cli/test_secrets.py` & `gantry-0.6.4/tests/cli/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/conftest.py` & `gantry-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/curator/conftest.py` & `gantry-0.6.4/tests/curator/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/curator/test_curator.py` & `gantry-0.6.4/tests/curator/test_curator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/curator/test_main.py` & `gantry-0.6.4/tests/curator/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/curator/test_selectors.py` & `gantry-0.6.4/tests/curator/test_selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/data_generator/test_data_generator.py` & `gantry-0.6.4/tests/data_generator/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/dataset/conftest.py` & `gantry-0.6.4/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/dataset/test_client.py` & `gantry-0.6.4/tests/dataset/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/dataset/test_gantry_dataset.py` & `gantry-0.6.4/tests/dataset/test_gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/dataset/test_main.py` & `gantry-0.6.4/tests/dataset/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/logger/test_client.py` & `gantry-0.6.4/tests/logger/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/logger/test_consumer.py` & `gantry-0.6.4/tests/logger/test_consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/logger/test_event_builder.py` & `gantry-0.6.4/tests/logger/test_event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/logger/test_main.py` & `gantry-0.6.4/tests/logger/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/logger/test_stores.py` & `gantry-0.6.4/tests/logger/test_stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/logger/test_utils.py` & `gantry-0.6.4/tests/logger/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/conftest.py` & `gantry-0.6.4/tests/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/core/test_dataframe.py` & `gantry-0.6.4/tests/query/core/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/core/test_distance.py` & `gantry-0.6.4/tests/query/core/test_distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/core/test_filters.py` & `gantry-0.6.4/tests/query/core/test_filters.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/core/test_metric.py` & `gantry-0.6.4/tests/query/core/test_metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/core/test_queryframe.py` & `gantry-0.6.4/tests/query/core/test_queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/core/test_series.py` & `gantry-0.6.4/tests/query/core/test_series.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/core/test_utils.py` & `gantry-0.6.4/tests/query/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/distance/test_main.py` & `gantry-0.6.4/tests/query/distance/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/metric/test_main.py` & `gantry-0.6.4/tests/query/metric/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/test_client.py` & `gantry-0.6.4/tests/query/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/query/test_main.py` & `gantry-0.6.4/tests/query/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/test_api_client.py` & `gantry-0.6.4/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/test_init.py` & `gantry-0.6.4/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/test_utils.py` & `gantry-0.6.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.3/tests/test_validator.py` & `gantry-0.6.4/tests/test_validator.py`

 * *Files identical despite different names*

