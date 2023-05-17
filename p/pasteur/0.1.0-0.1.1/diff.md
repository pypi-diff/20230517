# Comparing `tmp/pasteur-0.1.0.tar.gz` & `tmp/pasteur-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasteur-0.1.0.tar", last modified: Fri Mar  3 15:07:45 2023, max compression
+gzip compressed data, was "pasteur-0.1.1.tar", last modified: Wed May 17 13:01:26 2023, max compression
```

## Comparing `pasteur-0.1.0.tar` & `pasteur-0.1.1.tar`

### file list

```diff
@@ -1,128 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.022734 pasteur-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-03 15:07:30.000000 pasteur-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-03 15:07:45.022734 pasteur-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-03 15:07:30.000000 pasteur-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-03 15:07:30.000000 pasteur-0.1.0/README_PYPI.md
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-03 15:07:30.000000 pasteur-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-03 15:07:45.022734 pasteur-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-03 15:07:30.000000 pasteur-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:44.994733 pasteur-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.002734 pasteur-0.1.0/src/pasteur/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/encode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.006734 pasteur-0.1.0/src/pasteur/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.006734 pasteur-0.1.0/src/pasteur/extras/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.006734 pasteur-0.1.0/src/pasteur/extras/datasets/adult/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/datasets/adult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.010734 pasteur-0.1.0/src/pasteur/extras/datasets/mimic/
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/datasets/mimic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/datasets/sdgym.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.010734 pasteur-0.1.0/src/pasteur/extras/datasets/texas/
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/datasets/texas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.010734 pasteur-0.1.0/src/pasteur/extras/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/metrics/distr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.010734 pasteur-0.1.0/src/pasteur/extras/metrics/models/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/metrics/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/metrics/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/metrics/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/metrics/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.010734 pasteur-0.1.0/src/pasteur/extras/synth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/synth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14269 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/synth/extern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.014734 pasteur-0.1.0/src/pasteur/extras/synth/pgm/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/synth/pgm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/synth/pgm/aim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/synth/pgm/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/synth/pgm/mst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.014734 pasteur-0.1.0/src/pasteur/extras/synth/privbayes/
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/synth/privbayes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/synth/privbayes/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21013 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.014734 pasteur-0.1.0/src/pasteur/extras/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.014734 pasteur-0.1.0/src/pasteur/extras/views/adult/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/views/adult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.014734 pasteur-0.1.0/src/pasteur/extras/views/mimic/
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/views/mimic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.014734 pasteur-0.1.0/src/pasteur/extras/views/texas/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/extras/views/texas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/hierarchy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.014734 pasteur-0.1.0/src/pasteur/kedro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.014734 pasteur-0.1.0/src/pasteur/kedro/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/hooks/pasteur.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/ipython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.018734 pasteur-0.1.0/src/pasteur/kedro/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/mlflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/mlflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/mlflow/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/mlflow/parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.018734 pasteur-0.1.0/src/pasteur/kedro/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/pipelines/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/pipelines/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/pipelines/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/pipelines/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/pipelines/synth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/pipelines/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/pipelines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/pipelines/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.018734 pasteur-0.1.0/src/pasteur/kedro/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/runner/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/runner/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/runner/sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/starters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/kedro/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.018734 pasteur-0.1.0/src/pasteur/marginal/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/marginal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/marginal/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.018734 pasteur-0.1.0/src/pasteur/marginal/native/
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/marginal/native/impl.c
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/marginal/native/wrapper.c
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/marginal/native_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/marginal/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18040 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/marginal/oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/synth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16708 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:44.998734 pasteur-0.1.0/src/pasteur/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:44.998734 pasteur-0.1.0/src/pasteur/templates/project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.018734 pasteur-0.1.0/src/pasteur/templates/project/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/templates/project/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.022734 pasteur-0.1.0/src/pasteur/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/utils/leaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/utils/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/utils/perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15007 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/utils/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.022734 pasteur-0.1.0/src/pasteur/utils/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/utils/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-03-03 15:07:30.000000 pasteur-0.1.0/src/pasteur/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:07:45.006734 pasteur-0.1.0/src/pasteur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-03 15:07:44.000000 pasteur-0.1.0/src/pasteur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-03 15:07:44.000000 pasteur-0.1.0/src/pasteur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 15:07:44.000000 pasteur-0.1.0/src/pasteur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-03 15:07:44.000000 pasteur-0.1.0/src/pasteur.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-03 15:07:44.000000 pasteur-0.1.0/src/pasteur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-03 15:07:44.000000 pasteur-0.1.0/src/pasteur.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.031859 pasteur-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 13:01:09.000000 pasteur-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 13:01:09.000000 pasteur-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-17 13:01:26.031859 pasteur-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-17 13:01:09.000000 pasteur-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-17 13:01:09.000000 pasteur-0.1.1/README_PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-17 13:01:09.000000 pasteur-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 13:01:26.031859 pasteur-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-17 13:01:09.000000 pasteur-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.011859 pasteur-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.015859 pasteur-0.1.1/src/pasteur/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/encode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.015859 pasteur-0.1.1/src/pasteur/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/datasets/adult/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/datasets/adult/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/datasets/adult/catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/datasets/mimic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/datasets/mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/datasets/mimic/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/datasets/sdgym.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/datasets/texas/
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/datasets/texas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46616 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/datasets/texas/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/metrics/distr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/metrics/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/metrics/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/metrics/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/metrics/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/metrics/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/synth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/synth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14269 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/synth/extern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/synth/pgm/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/synth/pgm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/synth/pgm/aim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/synth/pgm/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/synth/pgm/mst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/synth/privbayes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/synth/privbayes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/synth/privbayes/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21057 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/views/adult/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/adult/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/adult/parameters.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.019859 pasteur-0.1.1/src/pasteur/extras/views/mimic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/mimic/parameters_billion.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/mimic/parameters_mm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/mimic/parameters_tab.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.023859 pasteur-0.1.1/src/pasteur/extras/views/texas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/texas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/texas/parameters_base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/texas/parameters_billion.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/extras/views/texas/parameters_charges.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14597 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/hierarchy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.023859 pasteur-0.1.1/src/pasteur/kedro/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.023859 pasteur-0.1.1/src/pasteur/kedro/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/hooks/pasteur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/ipython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.023859 pasteur-0.1.1/src/pasteur/kedro/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/mlflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/mlflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/mlflow/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/mlflow/parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.023859 pasteur-0.1.1/src/pasteur/kedro/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/pipelines/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/pipelines/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/pipelines/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/pipelines/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/pipelines/synth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/pipelines/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/pipelines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/pipelines/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.023859 pasteur-0.1.1/src/pasteur/kedro/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/runner/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/runner/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/runner/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/starters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/kedro/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/marginal/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/marginal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/marginal/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/marginal/native/
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/marginal/native/impl.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/marginal/native/wrapper.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/marginal/native_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/marginal/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18040 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/marginal/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/synth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.011859 pasteur-0.1.1/src/pasteur/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/prompts.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/conf/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/conf/base/globals.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/conf/base/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/conf/base/mlflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.011859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/logs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/raw/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.027859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.031859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.031859 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.031859 pasteur-0.1.1/src/pasteur/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/utils/leaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/utils/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/utils/perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/utils/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.031859 pasteur-0.1.1/src/pasteur/utils/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/utils/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-17 13:01:09.000000 pasteur-0.1.1/src/pasteur/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:26.015859 pasteur-0.1.1/src/pasteur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-17 13:01:25.000000 pasteur-0.1.1/src/pasteur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-17 13:01:26.000000 pasteur-0.1.1/src/pasteur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:01:25.000000 pasteur-0.1.1/src/pasteur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-17 13:01:25.000000 pasteur-0.1.1/src/pasteur.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-17 13:01:25.000000 pasteur-0.1.1/src/pasteur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 13:01:25.000000 pasteur-0.1.1/src/pasteur.egg-info/top_level.txt
```

### Comparing `pasteur-0.1.0/LICENSE` & `pasteur-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/PKG-INFO` & `pasteur-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasteur
-Version: 0.1.0
+Version: 0.1.1
 Summary: A system for reproducible and scalable data synthesis.
 Author-email: Kapenekakis Antheas <antheas@cs.aau.dk>
 Project-URL: Homepage, https://pasteur.dev
 Project-URL: Bug Tracker, https://github.com/pasteur-dev/pasteur/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,13 +13,13 @@
 Provides-Extra: opt
 Provides-Extra: test
 Provides-Extra: cls
 Provides-Extra: docs
 License-File: LICENSE
 
 
-![Pasteur Logo with text. Tagline reads: 'Sanitize Your Data'](https://raw.githubusercontent.com/pasteur-dev/pasteur-web/master/assets/img/logo_text_light.svg)
+![Pasteur Logo with text. Tagline reads: 'Sanitize Your Data'](https://raw.githubusercontent.com/pasteur-dev/pasteur/master/res/logo/text_light.svg)
 
 Pasteur is a system for data synthesis in a prototype state.
 Head to https://pasteur.dev or https://github.com/pasteur-dev/pasteur for
 more information.
-Documentation and project template coming soon!
+Documentation coming soon!
```

### Comparing `pasteur-0.1.0/pyproject.toml` & `pasteur-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pasteur"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Kapenekakis Antheas", email="antheas@cs.aau.dk" },
 ]
 description = "A system for reproducible and scalable data synthesis."
 readme = "README_PYPI.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -32,32 +32,34 @@
   "jupyter~=1.0",
   "jupyterlab~=3.0",
   "kedro-viz",
   "black~=22.0",
   "flake8>=3.7.9, <4.0",
   "isort~=5.0",
   "parquet-tools",
+  "pip-tools",
 ]
 test = [
   "pytest-cov~=3.0",
   "pytest-mock>=1.7.1, <2.0",
   "pytest~=6.2",
 ]
 cls = [
   "xgboost"
 ]
 docs = [
-  "docutils<0.18.0",
-  "sphinx~=3.4.3",
-  "sphinx_rtd_theme==0.5.1",
-  "nbsphinx==0.8.1",
-  "recommonmark==0.7.1",
-  "sphinx-autodoc-typehints==1.11.1",
-  "sphinx_copybutton==0.3.1",
+  "docutils",
+  "sphinx",
+  "sphinx-book-theme",
+  "nbsphinx",
+  "recommonmark",
+  "sphinx-autodoc-typehints",
+  "sphinx_copybutton",
   "Jinja2",
+  "sphinx-autobuild",
 ]
 
 [project.urls]
 "Homepage" = "https://pasteur.dev"
 "Bug Tracker" = "https://github.com/pasteur-dev/pasteur/issues"
 
 [project.entry-points."console_scripts"]
```

### Comparing `pasteur-0.1.0/setup.py` & `pasteur-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/__init__.py` & `pasteur-0.1.1/src/pasteur/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,7 +8,14 @@
 
 try:
     from importlib import metadata
 except ImportError:
     import importlib_metadata as metadata
 
 version = metadata.version("pasteur")
+__version__ = version
+
+def load_ipython_extension(ipython):
+    """ Allows loading ipython functionality with `load_ext pasteur` """
+    from pasteur.kedro.ipython import load_ipython_extension as ld
+
+    ld(ipython)
```

### Comparing `pasteur-0.1.0/src/pasteur/dataset.py` & `pasteur-0.1.1/src/pasteur/dataset.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+""" This module holds the definitions for the Dataset module, the initial entrypoint
+for data in Pasteur. """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable
 
 from .module import Module
-from .utils import LazyChunk, LazyFrame, to_chunked
+from .utils import LazyChunk, LazyFrame, to_chunked, RawSource
 
 if TYPE_CHECKING:
     import pandas as pd
 
 
 class Dataset(Module):
     """A class for a Dataset named `name` that creates a set of tables based on the
@@ -38,76 +41,93 @@
     implemented as a callable which receives 2 strings, one for the raw location
     of the dataset (based on `folder_name`), and one for a reserved intermediary
     directory for this dataset (`#{bootstrap}`).
 
     @Warning: having a table named raw is not allowed."""
 
     deps: dict[str, list[str]] = {}
-    key_deps: list[str] = []
+    """ Defines the Tables of the dataset and their dependencies, ex.:
+    
+    ```python
+    {"table1": ["raw1", "raw2"], "table2": ["raw3", "raw4"]}
+    ```
+    """
 
+    key_deps: list[str] = []
+    """ Provides the table dependencies (Table, not raw) that are used to create 
+    the keys of the dataset. """
+    
     folder_name: str | None = None
+    """ Specifies the name of the folder in the raw directory that will be used
+    for the dataset's raw sources. If the folder does not exist, the dataset
+    is disabled (used for packaging)."""
     catalog: dict[str, Any] | str | None = None
+    """ A kedro catalog that represents the dataset's sources. Can be provided
+    as a dictionary to be used as is, or as a filepath, in which case
+    the path will be loaded and processed, by replacing the paths with appropriate
+    ones based on the raw directory and folder name."""
+    raw_sources: dict[str, RawSource] | RawSource | None = None
+    """ A raw source that can be used to download the dataset.
+    
+    Optionally, multiple sources can be supplied and downloaded with `pasteur download <name>`."""
+
     bootstrap: Callable[[str, str], None] | None = None
+    """ An optional function that is used for one-time tasks (such as extraction).
+    Can be run with `pasteur bootstrap <dataset_name>`. 
+    
+    Is provided with 2 paths: the raw directory of the dataset and another 
+    directory dedicated to the dataset named bootstrap.
+    If the dataset has any archives, extract them from the raw directory to 
+    bootstrap and then use the bootstrap directory as a base in the catalog."""
 
     def __init__(self, **_) -> None:
         pass
 
     @property
     def raw_tables(self):
+        """Returns the raw dependency names of the dataset."""
         from functools import reduce
 
         return list(dict.fromkeys(reduce(lambda a, b: a + b, self.deps.values(), [])))
 
     @property
     def tables(self):
+        """Returns the table names of the dataset."""
         return list(self.deps.keys())
 
     def ingest(self, name, **tables: Any) -> LazyFrame:
         """Creates the table <name> using the tables provided based on the dependencies.
 
-        The dependencies may be any and should be defined in the catalog.
+        The dependencies may be anything and should be defined in the catalog.
         The raw tables of a dataset are the only kedro datasets explicitly
         defined by the user.
 
         Can return a dataframe, callable which produces a dataframe, or dict of callables, dataframes.
         If it's a dict, the table will be partitioned using the dict keys.
 
         @warning: all partitioned tables should have the same partitions.
-        Some tables may not be partitioned."""
+        Some tables may not be partitioned.
+        
+        Tip: use a `match` statement to fork based on table name to per-table functions."""
         raise NotImplemented()
 
     def keys(self, **tables: LazyFrame) -> pd.DataFrame:
-        """Returns a set of keys which split the current dataset (or partition).
+        """Returns a set of keys which split the current dataset.
 
         Keys do not need to be unique per partition, since splitting will also
         be partition based.
+        Gets a set of table partitions based on `key_deps`.
 
-        Gets a set of table partitions based on `key_deps`. All tables are the
-        same partition. If a table is not partitioned, it's the whole DataFrame.
-
-        Shouldn't return a callable."""
+        Use the `to_chunked` operator to handle partitions."""
         raise NotImplemented()
 
     def __str__(self) -> str:
         return self.name
 
 
-class TypedDataset(Dataset):
-    """Extend from to create an intermediary step in ingestion, where the table
-    is loaded from `<dataset>.raw@<table>` to a parquet one `<dataset>.typed.<table>.
-
-    Useful for multiple reads to raw tables. You can also override the `type()` function to make
-    minor changes to the dataset. By default it's the identity.
-
-    Since parquet files don't support chunked loading it's unused."""
-
-    def type(self, table: Any):
-        return table
-
-
 class TabularDataset(Dataset):
     """Boilerplate for a tabular dataset. Assumes the dataset contains one table
     named `table`, the index of which is the keys.
 
     By default, assumes one raw table `raw@table`, exists. If the data is concatenated
     from multiple sources, `deps` can be modified to reflect this."""
 
@@ -129,9 +149,22 @@
     @to_chunked
     def keys(self, **tables: LazyChunk) -> pd.DataFrame:
         """Returns a DataFrame containing only the index column of table "table"."""
         assert len(tables) == 1 and "table" in tables
 
         return tables["table"]()
 
+class TypedDataset(Dataset):
+    """Extend from to create an intermediary step in ingestion, where the table
+    is loaded from `<dataset>.raw@<table>` to a parquet one `<dataset>.typed.<table>.
+
+    Useful for multiple reads to raw tables. You can also override the `type()` function to make
+    minor changes to the dataset. By default it's the identity.
+
+    Since parquet files don't support chunked loading it's unused."""
+
+    def type(self, table: Any):
+        return table
+
+
 
-__all__ = ["Dataset", "TabularDataset"]
+__all__ = ["RawSource", "Dataset", "TabularDataset"]
```

### Comparing `pasteur-0.1.0/src/pasteur/extras/__init__.py` & `pasteur-0.1.1/src/pasteur/extras/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+""" This package contains reference implementations for Pasteur modules, which
+may be extracted to a separate package in the future."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from ..dataset import Dataset
     from ..module import Module
```

### Comparing `pasteur-0.1.0/src/pasteur/extras/datasets/adult/__init__.py` & `pasteur-0.1.1/src/pasteur/extras/datasets/adult/__init__.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/datasets/mimic/__init__.py` & `pasteur-0.1.1/src/pasteur/extras/datasets/mimic/__init__.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/datasets/sdgym.py` & `pasteur-0.1.1/src/pasteur/extras/datasets/sdgym.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/datasets/texas/__init__.py` & `pasteur-0.1.1/src/pasteur/extras/datasets/texas/__init__.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/encoders.py` & `pasteur-0.1.1/src/pasteur/extras/encoders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from copy import copy
+from typing import cast
 
 import numpy as np
 import pandas as pd
 
-from ..attribute import Attribute, IdxValue, NumValue, OrdValue, get_dtype
+from ..attribute import (
+    Attribute,
+    CatValue,
+    NumValue,
+    _create_strat_value_ord,
+    get_dtype,
+)
 from ..encode import Encoder
 
 
 class DiscretizationColumnTransformer:
     """Converts a numerical column into an ordinal one using histograms."""
 
-    def fit(self, attr: NumValue, data: pd.Series) -> IdxValue:
+    def fit(self, attr: NumValue, data: pd.Series) -> CatValue:
         self.in_attr = attr
         assert data.name
-        self.col = data.name
+        self.col = cast(str, data.name)
 
         rng = (
             (attr.min, attr.max)
             if attr.min is not None and attr.max is not None
             else None
         )
         assert attr.bins is not None
         # FIXME: is not out of core
         self.edges = np.histogram_bin_edges(data[~pd.isna(data)], attr.bins, rng)
         self.vals = ((self.edges[:-1] + self.edges[1:]) / 2).astype(np.float32)
 
         if attr.common <= 1:
-            self.attr = OrdValue(self.vals, na=attr.common == 1)
+            self.attr = _create_strat_value_ord(self.vals, na=attr.common == 1)
         else:
             assert (
                 False
             ), "Discretizing multi-column attributes which contain multiple common values and numerical attributes is not supported for now"
             # The problem is that when there's one common value, ie NA, there's a floating point presentation for it
             # but for more there's not...
             # self.attr = LevelColumn(Level("ord", self.vals), attr.common)
@@ -113,25 +120,25 @@
         cols = {}
 
         common = attr.common
 
         skip_common = False
         if len(attr.vals) == 1:
             v = next(iter(attr.vals.values()))
-            if isinstance(v, IdxValue) and v.is_ordinal:
+            if isinstance(v, CatValue) and v.is_ordinal:
                 skip_common = True
 
         if not skip_common:
             for i in range(common):
                 cols[f"{attr.name}_cmn_{i}"] = NumValue()
 
         for name, col in attr.vals.items():
             if isinstance(col, NumValue):
                 cols[name] = col
-            elif isinstance(col, IdxValue):
+            elif isinstance(col, CatValue):
                 if col.is_ordinal():
                     cols[name] = NumValue()
                 else:
                     assert col.common == common
                     for i in range(col.get_domain(0) - col.common):
                         cols[f"{name}_{i}"] = NumValue()
 
@@ -146,35 +153,35 @@
         cols = []
         only_has_na = a.common == 1 and a.na
 
         # Handle common values
         skip_common = False
         if len(a.vals) == 1:
             v = next(iter(a.vals.values()))
-            if isinstance(v, IdxValue) and v.is_ordinal:
+            if isinstance(v, CatValue) and v.is_ordinal:
                 skip_common = True
 
         for i in range(a.common) if not skip_common else []:
             cmn_col = pd.Series(False, index=data.index, name=f"{a.name}_cmn_{i}", dtype=np.float32)
 
             for name, col in a.vals.items():
-                if isinstance(col, IdxValue):
+                if isinstance(col, CatValue):
                     cmn_col += data[name] == i
                 elif isinstance(col, NumValue) and only_has_na:
                     # Numerical values are expected to be NA for all common values
                     # so they are only used to set the common values when:
                     # `common == 1 and a.na`, meaning the only common value is NA.``
                     cmn_col += pd.isna(data[name])
             cols.append(cmn_col.clip(0, 1, inplace=False))
 
         # Add other columns
         for name, col in a.vals.items():
             if isinstance(col, NumValue):
                 cols.append(data[name])
-            elif isinstance(col, IdxValue):
+            elif isinstance(col, CatValue):
                 # TODO add proper encodings other than one hot
 
                 # Handle ordinal values
                 if col.is_ordinal():
                     cols.append(data[name])
                 else:
                     # One hot encode everything else
```

### Comparing `pasteur-0.1.0/src/pasteur/extras/metrics/distr.py` & `pasteur-0.1.1/src/pasteur/extras/metrics/distr.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 from scipy.special import rel_entr
 from scipy.stats import chisquare
 
-from ...attribute import Attributes, IdxValue, get_dtype
+from ...attribute import Attributes, CatValue, get_dtype
 from ...metric import Summaries, TableData, TableMetric
 from ...utils.progress import process_in_parallel
 
 if TYPE_CHECKING:
     from ...metadata import Metadata
 
 KL_ZERO_FILL = 1e-24
@@ -66,15 +66,15 @@
     ):
         self.table = table
         table_attrs = attrs["idx"][table]
 
         self.domain = {}
         for attr in table_attrs.values():
             for name, val in attr.vals.items():
-                assert isinstance(val, IdxValue)
+                assert isinstance(val, CatValue)
                 self.domain[name] = val.domain
 
     def process_chunk(
         self,
         table: pd.DataFrame,
     ):
         domain = np.array(list(self.domain.values()))
@@ -183,15 +183,15 @@
     ):
         self.table = table
         table_attrs = attrs["idx"][table]
 
         self.domain = {}
         for attr in table_attrs.values():
             for name, val in attr.vals.items():
-                assert isinstance(val, IdxValue)
+                assert isinstance(val, CatValue)
                 self.domain[name] = val.domain
 
     def process_chunk(
         self,
         table: pd.DataFrame,
     ):
         a = table()[list(self.domain)].to_numpy(dtype="uint16")
```

### Comparing `pasteur-0.1.0/src/pasteur/extras/metrics/models/base.py` & `pasteur-0.1.1/src/pasteur/extras/metrics/models/base.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/metrics/models/models.py` & `pasteur-0.1.1/src/pasteur/extras/metrics/models/models.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/metrics/visual.py` & `pasteur-0.1.1/src/pasteur/extras/metrics/visual.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/synth/extern.py` & `pasteur-0.1.1/src/pasteur/extras/synth/extern.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/synth/pgm/aim.py` & `pasteur-0.1.1/src/pasteur/extras/synth/pgm/aim.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/synth/pgm/common.py` & `pasteur-0.1.1/src/pasteur/extras/synth/pgm/common.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/synth/pgm/mst.py` & `pasteur-0.1.1/src/pasteur/extras/synth/pgm/mst.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/synth/privbayes/__init__.py` & `pasteur-0.1.1/src/pasteur/extras/synth/privbayes/__init__.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/synth/privbayes/implementation.py` & `pasteur-0.1.1/src/pasteur/extras/synth/privbayes/implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from itertools import combinations
 from typing import NamedTuple, Sequence, cast
 
 import numpy as np
 import pandas as pd
 
-from ....attribute import Attributes, IdxValue, get_dtype
+from ....attribute import Attributes, CatValue, get_dtype
 from ....marginal import (
     ZERO_FILL,
     AttrSelector,
     AttrSelectors,
     MarginalOracle,
     MarginalRequest,
 )
@@ -226,30 +226,30 @@
     group_names = []  # attr (group) -> str name
     heights = []  # col -> max height
     common = []  # col -> common val number
     domain = []  # col, height -> domain
     for i, (an, a) in enumerate(attrs.items()):
         group_names.append(an)
         for c_n, c in a.vals.items():
-            c = cast(IdxValue, c)
+            c = cast(CatValue, c)
             col_names.append(c_n)
             groups.append(i)
             heights.append(c.height)
             common.append(a.common)
             domain.append([c.get_domain(h) for h in range(c.height)])
 
     # If skip_zero_counts is on, calculate domain based on non-zero values
     domain_orig = domain
     if skip_zero_counts:
         domain = []
         counts = oracle.get_counts(f"Calculating counts for nonzero domain")
 
         for i, (an, a) in enumerate(attrs.items()):
             for c_n, c in a.vals.items():
-                c = cast(IdxValue, c)
+                c = cast(CatValue, c)
 
                 doms = []
                 for i in range(c.height):
                     mapping = c.get_mapping(i)
                     d = c.get_domain(i)
                     count = np.zeros((d,))
 
@@ -656,15 +656,15 @@
             _tmp_nd = np.zeros((n,), dtype=dtype)
             for attr_name, attr in p.items():
                 common = attr.common
                 l_mul = 1
                 p_partial = partial and attr_name == x_attr
                 for i, (col_name, h) in enumerate(attr.cols.items()):
                     col = attrs[attr_name].vals[col_name]
-                    col = cast(IdxValue, col)
+                    col = cast(CatValue, col)
                     mapping = np.array(col.get_mapping(h), dtype=dtype)
                     domain = col.get_domain(h)
 
                     col_lvl = mapping[out[col_name]]
                     if common != 0 and (i != 0 or p_partial):
                         col_lvl = np.where(col_lvl > common, col_lvl - common, 0)
                     np.multiply(col_lvl, mul * l_mul, out=_tmp_nd, dtype=dtype)
```

### Comparing `pasteur-0.1.0/src/pasteur/extras/transformers.py` & `pasteur-0.1.1/src/pasteur/extras/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_categorical_dtype
 
 from ..attribute import (
     Attribute,
     CatAttribute,
-    Level,
-    LevelValue,
+    Grouping,
+    CatValue,
     NumAttribute,
     NumValue,
     OrdAttribute,
-    OrdValue,
+    _create_strat_value_ord as OrdValue,
     get_dtype,
 )
 from ..transform import RefTransformer, Transformer
 from ..utils import list_unique
 
 
 class NumericalTransformer(Transformer):
@@ -439,49 +439,49 @@
 
         hours = []
         for hour in range(24):
             if span == "hour":
                 hours.append(f"{hour:02d}:00")
             elif span == "halfhour":
                 hours.append(
-                    Level(
+                    Grouping(
                         "ord",
                         [f"{hour:02d}:00", f"{hour:02d}:30"],
                     )
                 )
             else:
                 mins = []
                 for min in range(60):
                     if span == "minute":
                         mins.append(f"{hour:02d}:{min:02d}")
                     if span == "halfminute":
                         mins.append(
-                            Level(
+                            Grouping(
                                 "ord",
                                 [
                                     f"{hour:02d}:{min:02d}:00",
                                     f"{hour:02d}:{min:02d}:30",
                                 ],
                             )
                         )
                     if span == "second":
                         secs = []
                         for sec in range(60):
                             secs.append(f"{hour:02d}:{min:02d}:{sec:02d}")
-                        mins.append(Level("ord", secs))
+                        mins.append(Grouping("ord", secs))
 
-                hours.append(Level("ord", mins))
-        lvl = Level("ord", hours)
+                hours.append(Grouping("ord", mins))
+        lvl = Grouping("ord", hours)
         if self.nullable:
-            lvl = Level("cat", [None, lvl])
+            lvl = Grouping("cat", [None, lvl])
 
         self.domain = lvl.size
 
         self.attr = Attribute(
-            cast(str, data.name), {f"{data.name}_time": LevelValue(lvl)}, self.nullable
+            cast(str, data.name), {f"{data.name}_time": CatValue(lvl)}, self.nullable
         )
         return self.attr
 
     def transform(self, date: pd.Series) -> pd.DataFrame:
         out = pd.DataFrame(index=date.index)
         span = self.span
```

### Comparing `pasteur-0.1.0/src/pasteur/extras/utils.py` & `pasteur-0.1.1/src/pasteur/extras/utils.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/views/mimic/__init__.py` & `pasteur-0.1.1/src/pasteur/extras/views/mimic/__init__.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/extras/views/texas/__init__.py` & `pasteur-0.1.1/src/pasteur/extras/views/texas/__init__.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/hierarchy.py` & `pasteur-0.1.1/src/pasteur/hierarchy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+""" Highly experimental and unpublished class for rebalancing Stratified Values
+with Differential Privacy.
+
+@TODO: Documentation."""
+
 import logging
 from itertools import combinations
 from math import ceil, log
 from typing import TypeVar
 
 import numpy as np
-import pandas as pd
 
-from .attribute import Attributes, IdxValue, Level, LevelValue, get_dtype
+from .attribute import Attributes, CatValue, Grouping, StratifiedValue, get_dtype
 
 logger = logging.getLogger(__name__)
 
 ZERO_FILL = 1e-24
 
 
 class OrdNode(list):
@@ -18,30 +22,30 @@
 
 
 class CatNode(list):
     pass
 
 
 def create_tree(
-    node: Level, common: int = 0, ofs: int = 0, n: int | None = None
+    node: Grouping, common: int = 0, ofs: int = 0, n: int | None = None
 ) -> list:
     """Receives the top node of the tree of a hierarchical attribute and
     converts it into the same tree structure, where the leaves have been
     replaced by bucket groups, with each bucket group containing the node it replaced.
 
     For buckets lower than common, they are replaced by `None` to prevent merging
     them."""
     if n is None:
         n = node.get_domain(0)
     out = CatNode() if node.type == "cat" else OrdNode()
 
     for child in node:
         if ofs < common:
             out.append(None)
-        elif isinstance(child, Level):
+        elif isinstance(child, Grouping):
             out.append(create_tree(child, common, ofs, n))
         else:
             out.append(set([ofs]))
 
         ofs += 1
 
     return out
@@ -216,15 +220,15 @@
             ofs += 1
         else:
             ofs = create_node_to_group_map(child, grouping, ofs)
 
     return ofs
 
 
-def make_grouping(counts: np.ndarray, head: Level, common: int = 0) -> np.ndarray:
+def make_grouping(counts: np.ndarray, head: Grouping, common: int = 0) -> np.ndarray:
     """Converts the hierarchical attribute level tree provided into a node-to-group
     mapping, where `group[i][j] = z`, where `i` is the height of the mapping
     `j` is node `j` and `z` is the group the node is associated at that height.
 
     `counts` provides the class densities. It doesn't need to be normalized and
     some of its values may be *negative*.
 
@@ -301,19 +305,19 @@
             new_domains.append(int(dom))
 
         new_domains.append(max_domain)
 
     return new_domains
 
 
-class RebalancedValue(IdxValue):
+class RebalancedValue(CatValue):
     def __init__(
         self,
         counts: np.ndarray,
-        col: LevelValue,
+        col: StratifiedValue,
         reshape_domain: bool = True,
         u: float = 1.3,
         fixed: list[int] = [2, 4, 5, 8, 12],
         c: float | None = None,
         **_,
     ) -> None:
         self.common = col.common
@@ -402,15 +406,15 @@
             upsampled[mask] = np.random.choice(group_idx, p=p, size=(group_size,))
 
         return upsampled
 
 
 def rebalance_value(
     counts: np.ndarray,
-    col: LevelValue,
+    col: StratifiedValue,
     num_cols: int = 1,
     ep: float | None = None,
     gaussian: bool = False,
     unbounded_dp: bool = False,
     **kwargs,
 ):
     assert not gaussian, "Gaussian dp not supported yet"
@@ -418,15 +422,15 @@
     counts = counts.astype(np.float32)
 
     if ep is not None:
         noise_scale = (1 if unbounded_dp else 2) * num_cols / ep
         noise = np.random.laplace(scale=noise_scale, size=counts.shape)
         counts = counts + noise
 
-    assert isinstance(col, LevelValue)
+    assert isinstance(col, StratifiedValue)
     return RebalancedValue(counts, col, **kwargs)
 
 
 def rebalance_attributes(
     counts: dict[str, np.ndarray],
     attrs: Attributes,
     ep: float | None = None,
@@ -445,15 +449,15 @@
 
     num_cols = len(counts)
 
     new_attrs = {}
     for name, attr in attrs.items():
         cols = {}
         for col_name, col in attr.vals.items():
-            assert isinstance(col, LevelValue)
+            assert isinstance(col, StratifiedValue)
             cols[col_name] = rebalance_value(
                 counts[col_name],
                 col,
                 num_cols,
                 ep,
                 **kwargs,
             )
```

### Comparing `pasteur-0.1.0/src/pasteur/kedro/cli.py` & `pasteur-0.1.1/src/pasteur/kedro/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+""" In this module, all Pasteur related cli commands are defined.
+
+You can access them through `pasteur <command>` or `kedro <command>`. """
+
 import logging
 from typing import Any, Iterable
 
 import click
 from kedro.framework.session import KedroSession
 
 from ..utils.parser import eval_params, merge_params, str_params_to_dict
-from .runner import SimpleRunner
 from ..utils.progress import init_pool
+from .runner import SimpleRunner
 
 logger = logging.getLogger(__name__)
 
 
 @click.command()
 @click.argument("pipeline", type=str, default=None)
 @click.argument(
@@ -270,33 +274,51 @@
 ):
     """Downloads all Pasteur datasets from their creators, provided the user
     agrees to their access requirements, and has credentials, if required.
 
     Uses `wget` and `boto3` to download files.
 
     Only downloads missing files, can be ran to verify dataset is downloaded correctly."""
-    from ..extras.download import get_description, main
+    from ..dataset import Dataset
+    from ..extras.download import datasets as EXTRA_DATASETS
+    from ..module import get_module_dict
+    from ..utils.download import get_description, main
 
     # Setup logging and params with kedro
     with KedroSession.create() as session:
         ctx = session.load_context()
 
-        logger.info(get_description())
+        dataset_modules = get_module_dict(Dataset, getattr(ctx, "pasteur").modules)
+        all_datasets = dict(EXTRA_DATASETS)
+        for name, ds in dataset_modules.items():
+            if isinstance(ds.raw_sources, dict):
+                all_datasets.update(ds.raw_sources)
+            elif ds.raw_sources is not None:
+                all_datasets[name] = ds.raw_sources
+
+        logger.info(get_description(all_datasets))
         if not datasets:
             return
 
+        sel_datasets = {}
+        for ds in datasets:
+            if ds not in all_datasets:
+                logger.error(f"Raw sources for {ds} not found.")
+                return
+            sel_datasets[ds] = all_datasets[ds]
+
         download_dir = download_dir or ctx.params.get("raw_location", None)
         assert download_dir, f"Download dir is empty"
 
         if not accept:
             logger.error(
                 "You have to accept to the license of the data stores you're about to download from (--accept/-a)."
             )
         else:
-            main(download_dir, datasets, user)
+            main(download_dir, sel_datasets, user)
 
 
 @click.command()
 @click.argument(
     "datasets",
     nargs=-1,
     type=str,
```

### Comparing `pasteur-0.1.0/src/pasteur/kedro/dataset.py` & `pasteur-0.1.1/src/pasteur/kedro/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+""" This module provides kedro datasets that have been customized to suit Pasteur's needs.
+
+The most notable additions are that the datasets lazy load data through `PartitionedDataset`
+and can partition save data through custom `Node` return types. """
+
 import logging
 import os
 import re
 from io import BytesIO
 from typing import Callable
 
 import pandas as pd
```

### Comparing `pasteur-0.1.0/src/pasteur/kedro/hooks/pasteur.py` & `pasteur-0.1.1/src/pasteur/kedro/hooks/pasteur.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/ipython.py` & `pasteur-0.1.1/src/pasteur/kedro/ipython.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+""" This module extends Kedro's ipython functionality. """
 from pathlib import Path
 
 from IPython import get_ipython
 from kedro.framework.context import KedroContext
 from kedro.framework.session.session import KedroSession
 from kedro.framework.startup import bootstrap_project
 from kedro.io.data_catalog import DataCatalog
```

### Comparing `pasteur-0.1.0/src/pasteur/kedro/mlflow/base.py` & `pasteur-0.1.1/src/pasteur/kedro/mlflow/base.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/mlflow/config.py` & `pasteur-0.1.1/src/pasteur/kedro/mlflow/config.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/mlflow/hook.py` & `pasteur-0.1.1/src/pasteur/kedro/mlflow/hook.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/mlflow/parent.py` & `pasteur-0.1.1/src/pasteur/kedro/mlflow/parent.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/pipelines/dataset.py` & `pasteur-0.1.1/src/pasteur/kedro/pipelines/dataset.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/pipelines/main.py` & `pasteur-0.1.1/src/pasteur/kedro/pipelines/main.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/pipelines/meta.py` & `pasteur-0.1.1/src/pasteur/kedro/pipelines/meta.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/pipelines/metrics.py` & `pasteur-0.1.1/src/pasteur/kedro/pipelines/metrics.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/pipelines/synth.py` & `pasteur-0.1.1/src/pasteur/kedro/pipelines/synth.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     fr: SynthFactory,
 ):
     alg = fr.name
     type = fr.type
     tables = view.tables
 
     tags: list[str] = list(TAGS_SYNTH)
-    if fr.gpu:
-        tags.append(TAG_GPU)
+    # if fr.gpu:
+    #     tags.append(TAG_GPU)
 
     pipe = pipeline(
         [
             node(
                 func=gen_closure(synth_fit, fr),
                 inputs={
                     "metadata": f"{view}.metadata",
```

### Comparing `pasteur-0.1.0/src/pasteur/kedro/pipelines/transform.py` & `pasteur-0.1.1/src/pasteur/kedro/pipelines/transform.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/pipelines/utils.py` & `pasteur-0.1.1/src/pasteur/kedro/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/pipelines/views.py` & `pasteur-0.1.1/src/pasteur/kedro/pipelines/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 
 def create_view_pipeline(view: View):
     return PipelineMeta(
         pipeline(
             [
                 node(
-                    func=view.ingest,
-                    name=f"ingest_{t}",
+                    func=view.query,
+                    name=f"query_{t}",
                     args=[t],
                     inputs={dep: f"{view.dataset}.{dep}" for dep in view.deps[t]},
                     namespace=f"{view}.view",
                     outputs=f"{view}.view.{t}",
                     tags=TAGS_VIEW,
                 )
                 for t in view.tables
```

### Comparing `pasteur-0.1.0/src/pasteur/kedro/runner/common.py` & `pasteur-0.1.1/src/pasteur/kedro/runner/common.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/runner/parallel.py` & `pasteur-0.1.1/src/pasteur/kedro/runner/parallel.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/runner/sequential.py` & `pasteur-0.1.1/src/pasteur/kedro/runner/sequential.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/kedro/utils.py` & `pasteur-0.1.1/src/pasteur/kedro/utils.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/marginal/memory.py` & `pasteur-0.1.1/src/pasteur/marginal/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from multiprocessing.shared_memory import SharedMemory
 from typing import Any, NamedTuple, cast
 
 import numpy as np
 
-from ..attribute import Attributes, get_dtype, IdxValue
+from ..attribute import Attributes, get_dtype, CatValue
 from ..utils import LazyFrame
 
 class ArrayInfo(NamedTuple):
     shape: tuple[int]
     dtype: Any
     ofs: int
 
@@ -32,15 +32,15 @@
     info = {}
     for attr in attrs.values():
         # Skip allocation for attrs that don't have common
         if common and attr.common == 0:
             continue
 
         for name, col in attr.vals.items():
-            col = cast(IdxValue, col)
+            col = cast(CatValue, col)
             info[name] = []
             for height in range(col.height):
                 shape = (n, )
                 dtype = np.dtype(get_dtype(col.get_domain(height)))
 
                 info[name].append(ArrayInfo(shape, dtype, ofs))
                 ofs += dtype.itemsize * n
```

### Comparing `pasteur-0.1.0/src/pasteur/marginal/native/impl.c` & `pasteur-0.1.1/src/pasteur/marginal/native/impl.c`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/marginal/native/wrapper.c` & `pasteur-0.1.1/src/pasteur/marginal/native/wrapper.c`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/marginal/native_py.py` & `pasteur-0.1.1/src/pasteur/marginal/native_py.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/marginal/numpy.py` & `pasteur-0.1.1/src/pasteur/marginal/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import NamedTuple, cast
 
 import numpy as np
 import pandas as pd
 
-from ..attribute import Attributes, get_dtype, IdxValue
+from ..attribute import Attributes, get_dtype, CatValue
 
 ZERO_FILL = 1e-24
 
 
 class AttrSelector(NamedTuple):
     name: str
     common: int
@@ -59,15 +59,15 @@
 
     domains = {}
     for attr in attrs.values():
         for name, col in attr.vals.items():
             if name not in table:
                 continue
 
-            col = cast(IdxValue, col)
+            col = cast(CatValue, col)
             col_hier = []
             col_noncommon = []
             col_dom = []
 
             for height in range(col.height):
                 domain = col.get_domain(height)
                 col_dom.append(domain)
@@ -94,15 +94,15 @@
     return out_cols or cols, out_noncommon or cols_noncommon, domains
 
 
 def get_domains(attrs: Attributes) -> dict[str, list[int]]:
     domains = {}
     for attr in attrs.values():
         for name, col in attr.vals.items():
-            col = cast(IdxValue, col)
+            col = cast(CatValue, col)
             col_dom = []
 
             for height in range(col.height):
                 domain = col.get_domain(height)
                 col_dom.append(domain)
 
             domains[name] = col_dom
```

### Comparing `pasteur-0.1.0/src/pasteur/marginal/oracle.py` & `pasteur-0.1.1/src/pasteur/marginal/oracle.py`

 * *Files identical despite different names*

### Comparing `pasteur-0.1.0/src/pasteur/metadata.py` & `pasteur-0.1.1/src/pasteur/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+""" This module contains a base class `Metadata` which is used to wrap, type, 
+and check all View parameters provided to kedro.
+
+@TODO: refactor this file. """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, NamedTuple, overload
 
 if TYPE_CHECKING:
     import pandas as pd
-    from .utils import LazyFrame
 
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -169,15 +173,15 @@
     def __repr__(self) -> str:
         return self.__dict__.__repr__()
     
     def __str__(self) -> str:
         return self.__dict__.__str__()
 
 
-class DatasetMeta:
+class ViewMeta:
     TABLE_CLS = TableMeta
 
     def __init__(
         self,
         meta: dict,
     ):
         self._tables = {
@@ -222,9 +226,9 @@
     def __repr__(self) -> str:
         return self.__dict__.__repr__()
     
     def __str__(self) -> str:
         return self.__dict__.__str__()
 
 
-class Metadata(DatasetMeta):
+class Metadata(ViewMeta):
     pass
```

### Comparing `pasteur-0.1.0/src/pasteur/metric.py` & `pasteur-0.1.1/src/pasteur/metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+""" This module provides the definitions for Metric Modules.
+Metric modules can fit to a column, a table, or a whole View.
+In each case, modules are instanciated as required (for columns one is instantiated
+per column type, for tables one per table and View metrics are instantiated once)."""
+
 import logging
-from collections import defaultdict
-from typing import Generic, TypeVar, cast, TypedDict, NamedTuple, Any
+from typing import Generic, TypeVar, TypedDict, Any
 
 import pandas as pd
 
 from .attribute import Attributes
 from .metadata import ColumnMeta, Metadata
 from .module import ModuleClass, ModuleFactory
 from .table import TransformHolder
 from .utils import LazyChunk, LazyFrame
-from .utils.progress import process, process_in_parallel
+from .utils.progress import process_in_parallel
 
 logger = logging.getLogger(__name__)
 
 # Column metric -> receives one column, can't be encoded.
 # RefColumn metric -> one col + ref, can't be encoded
 
 # Table metric -> receives one table and its parents
@@ -40,17 +44,17 @@
     def __init__(
         self, cls: type["TableMetric"], *args, name: str | None = None, **kwargs
     ) -> None:
         super().__init__(cls, *args, name=name, **kwargs)
         self.encodings = cls.encodings
 
 
-class DatasetMetricFactory(ModuleFactory["DatasetMetric"]):
+class ViewMetricFactory(ModuleFactory["ViewMetric"]):
     def __init__(
-        self, cls: type["DatasetMetric"], *args, name: str | None = None, **kwargs
+        self, cls: type["ViewMetric"], *args, name: str | None = None, **kwargs
     ) -> None:
         super().__init__(cls, *args, name=name, **kwargs)
         self.encodings = cls.encodings
 
 
 A = TypeVar("A")
 
@@ -224,16 +228,16 @@
                     f"Type {col.type} of {table}.{name} does not support visualisation (Single-Column metrics)."
                 )
 
         # FIXME: does not fit on all data
         ids = data["ids"]
         tables = data["tables"].copy()
         tables["ids"] = ids
-        part = next(iter(LazyFrame.zip_values(**tables))) # FIXME: incorrect type
-        self._fit_chunk(table, meta, part, part["ids"]) #type: ignore
+        part = next(iter(LazyFrame.zip_values(**tables)))  # FIXME: incorrect type
+        self._fit_chunk(table, meta, part, part["ids"])  # type: ignore
 
     def _process_chunk(
         self,
         **tables: LazyChunk,
     ) -> dict[str, list]:
         cached = {self.table: tables[self.table]()}
         cached_ids = tables["ids"]() if "ids" in tables else None
@@ -272,20 +276,20 @@
 
         wrk_sum = {}
         ref_sum = {}
         for name, metrics in self.metrics.items():
             wrk_sum[name] = []
             ref_sum[name] = []
             for i, metric in enumerate(metrics):
-                wrk_sum[name].append(metric.combine(
-                    [chunk[name][i] for chunk in summaries_wrk]
-                ))
-                ref_sum[name].append(metric.combine(
-                    [chunk[name][i] for chunk in summaries_ref]
-                ))
+                wrk_sum[name].append(
+                    metric.combine([chunk[name][i] for chunk in summaries_wrk])
+                )
+                ref_sum[name].append(
+                    metric.combine([chunk[name][i] for chunk in summaries_ref])
+                )
 
         return Summaries(wrk_sum, ref_sum)
 
     def process(
         self, wrk: ColumnData, ref: ColumnData, syn: ColumnData, pre: Summaries
     ) -> Summaries:
         chunks_syn = list(LazyFrame.zip_values(**syn["tables"], ids=syn["ids"]))
@@ -295,17 +299,17 @@
             desc=f"Processing metric {self.unique_name()}",
         )
 
         syn_sum = {}
         for name, metrics in self.metrics.items():
             syn_sum[name] = []
             for i, metric in enumerate(metrics):
-                syn_sum[name].append(metric.combine(
-                    [chunk[name][i] for chunk in summaries]
-                ))
+                syn_sum[name].append(
+                    metric.combine([chunk[name][i] for chunk in summaries])
+                )
 
         return pre.replace(syn=syn_sum)
 
     def visualise(self, data: dict[str, Summaries]):
         for name, metrics in self.metrics.items():
             for i, metric in enumerate(metrics):
                 metric.visualise(
@@ -353,27 +357,27 @@
     ):
         raise NotImplementedError()
 
     def unique_name(self) -> str:
         return f"{self.type}_{self.name}_{self.table}"
 
 
-class DatasetData(TypedDict):
+class ViewData(TypedDict):
     tables: dict[str, dict[str, LazyFrame]]
     ids: dict[str, LazyFrame]
 
 
-class DatasetMetric(Metric[DatasetData, _INGEST, _SUMMARY], Generic[_INGEST, _SUMMARY]):
-    _factory = DatasetMetricFactory
+class ViewMetric(Metric[ViewData, _INGEST, _SUMMARY], Generic[_INGEST, _SUMMARY]):
+    _factory = ViewMetricFactory
     type = "dst"
     table: str
     encodings: list[str] = ["raw"]
 
     def fit(
-        self, meta: Metadata, attrs: dict[str, dict[str, Attributes]], data: DatasetData
+        self, meta: Metadata, attrs: dict[str, dict[str, Attributes]], data: ViewData
     ):
         raise NotImplementedError()
 
 
 def fit_column_holder(
     modules: dict[str, list[ColumnMetricFactory]],
     name: str,
@@ -403,18 +407,18 @@
 
     module = fs.build()
     module.fit(table=name, meta=meta, attrs=attrs, data=data)
     return module
 
 
 def fit_dataset_metric(
-    fs: DatasetMetricFactory,
+    fs: ViewMetricFactory,
     meta: Metadata,
     trns: dict[str, TransformHolder],
-    data: DatasetData,
+    data: ViewData,
 ):
     enc = fs.encodings
     attrs = {
         e: {
             n: h.get_attributes() if e == "bst" else h[e].get_attributes()
             for n, h in trns.items()
         }
@@ -428,7 +432,24 @@
 
 def log_metric(metric: Metric[Any, Any, _SUMMARY], summary: _SUMMARY):
     from .utils.mlflow import mlflow_log_artifacts
 
     mlflow_log_artifacts(
         "metrics", metric.unique_name(), metric=metric, summary=summary
     )
+
+
+DatasetMetric = ViewMetric
+DatasetMetricFactory = ViewMetricFactory
+
+__all__ = [
+    "ColumnMetricFactory",
+    "RefColumnMetricFactory",
+    "TableMetricFactory",
+    "ViewMetricFactory",
+    "Metric",
+    "Summaries",
+    "ColumnMetric",
+    "RefColumnMetric",
+    "TableMetric",
+    "ViewMetric",
+]
```

### Comparing `pasteur-0.1.0/src/pasteur/module.py` & `pasteur-0.1.1/src/pasteur/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,37 @@
+""" Contains the module definitions in Pasteur, the base classes all
+Pasteur modules extend from. 
+
+In Pasteur, all functionality is achieved through the use of modules.
+You should not interact with this module directly, but rather through its children."""
+
 from collections import defaultdict
 from typing import Generic, TypeVar
 
 
 class Module:
     """A Pasteur module extends a base Module class (such as Datset) and defines a name.
 
     Each base class, name combination registered in the system is considered unique*.
     Example: there should only be one registered Dataset named "adult".
 
     *the exception to this is metrics, where the name corresponds to a column type
     and there can be multiple visualizations for a certain column type.
     """
 
-    name: str
+    name: str = ""
 
 
 class ModuleClass:
     """Modules which need to be instantiated multiple times extend from ModuleClass and define
-    a Factory to act as their module"""
+    a Factory to act as their module.
+
+    For the module types provided by pasteur, you can call the classmethod `get_factory()`.
+    `get_factory()` also acts as a closure, allowing you to provide parameters to
+    the module's init function."""
 
     name: str
     _factory: type["ModuleFactory"]
 
     def __init__(self, *args, _from_factory: bool = False, **kwargs) -> None:
         assert (
             _from_factory
@@ -39,15 +49,15 @@
 A = TypeVar("A", bound=ModuleClass)
 
 
 class ModuleFactory(Module, Generic[A]):
     """Some modules (such as transformers) require multiple instances in the system. In this case,
     it's not possible to provide a module instance for them.
 
-    `ModuleFactory` is used to provide a wrapper instance to that module class."""
+    For those types, their instance is based on `ModuleFactory`."""
 
     def __init__(self, cls: type[A], *args, name: str | None = None, **kwargs) -> None:
         self._cls = cls
         self.name = name or cls.name
         self.args = args
         self.kwargs = kwargs
 
@@ -78,7 +88,16 @@
     """Same as `get_module_dict`, except for that it returns a list.
     Multiple modules can use the same name."""
     out = defaultdict(list)
     for module in modules:
         if isinstance(module, parent):
             out[module.name].append(module)
     return out
+
+
+__all__ = [
+    "Module",
+    "ModuleClass",
+    "ModuleFactory",
+    "get_module_dict",
+    "get_module_dict_multiple",
+]
```

### Comparing `pasteur-0.1.0/src/pasteur/synth.py` & `pasteur-0.1.1/src/pasteur/synth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+""" Contains the base definition for Synth(esizer modules).
+
+In addition, a test Synthesizer (IdentSynth) is provided, which returns
+the data it was provided as is. """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from .module import ModuleClass, ModuleFactory
 from .table import TransformHolder
 from .utils import LazyFrame
@@ -56,30 +61,19 @@
     return wrapped
 
 
 class SynthFactory(ModuleFactory["Synth"]):
     def __init__(self, cls: type[Synth], *args, name: str | None = None, **_) -> None:
         super().__init__(cls, *args, name=name, **_)
         self.type = cls.type
-        self.tabular = cls.tabular
-        self.multimodal = cls.multimodal
-        self.timeseries = cls.timeseries
-        self.gpu = cls.gpu
-        self.parallel = cls.parallel
 
 
 class Synth(ModuleClass):
     type = "idx"
-    tabular = True
-    multimodal = False
-    timeseries = False
     partitions = 1
-    gpu = False
-    parallel = False
-
     _factory = SynthFactory
 
     def preprocess(
         self,
         attrs: dict[str, Attributes],
         ids: dict[str, LazyFrame],
         tables: dict[str, LazyFrame],
@@ -139,16 +133,16 @@
 
     meta = metadata
     args = {**meta.algs.get(factory.name, {}), **meta.alg_override}
 
     attrs = {n: t[factory.type].get_attributes() for n, t in trns.items()}
     model = factory.build(**args, seed=meta.seed)
 
-    if factory.gpu:
-        tracker.use_gpu()
+    # if factory.gpu:
+    #     tracker.use_gpu()
 
     tracker.start("preprocess")
     model.preprocess(attrs, ids, tables)
     tracker.stop("preprocess")
 
     tracker.start("bake")
     model.bake(ids, tables)
@@ -178,18 +172,14 @@
 
 
 class IdentSynth(Synth):
     """Returns the data it was provided."""
 
     name = "ident_idx"
     type = "idx"
-
-    tabular = True
-    multimodal = True
-    timeseries = True
     partitions = 1
 
     def preprocess(
         self,
         attrs: dict[str, Attributes],
         ids: dict[str, LazyFrame],
         tables: dict[str, LazyFrame],
@@ -204,8 +194,8 @@
         self._tables = {name: table.sample() for name, table in tables.items()}
         self.partitions = len(tables[next(iter(tables))])
 
     def sample(self, n: int | None = None, i: int = 0):
         return self._ids, self._tables
 
 
-__all__ = ["Synth", "synth_fit", "synth_sample"]
+__all__ = ["Synth", "SynthFactory", "IdentSynth", "make_deterministic"]
```

### Comparing `pasteur-0.1.0/src/pasteur/table.py` & `pasteur-0.1.1/src/pasteur/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,37 @@
+""" Contains the logic for handling multiple tables, and holding transformers and
+encoders.
+
+The functionality is achieved through a class named `ReferenceManager`, which
+is used to generate the ID tables, and the `TransformHolder`, which holds
+everything required to encode and transform a table.
+
+The `TransformHolder` holds a `TableTransformer` which hosts the Table's transformers
+and multiple `TableEncoder`s, which can be accesed with array syntax (ex. `['idx']`),
+one for each supported encoding.
+
+Once the TransformHolder is fit, it can be loaded and used to transform, encode,
+reverse, and decode table partitions."""
+
 import logging
 
 import pandas as pd
 
 from .attribute import Attribute, Attributes
 from .encode import Encoder, EncoderFactory
 from .metadata import Metadata
 from .module import Module, get_module_dict
 from .transform import RefTransformer, Transformer, TransformerFactory
-from .utils import LazyChunk, LazyFrame
+from .utils import LazyChunk
 
 logger = logging.getLogger(__file__)
 
 
 class ReferenceManager:
-    """Manages the foreign relationships of a table"""
+    """Manages the foreign relationships of a table/"""
 
     def __init__(
         self,
         meta: Metadata,
         name: str,
     ) -> None:
         self.name = name
```

### Comparing `pasteur-0.1.0/src/pasteur/transform.py` & `pasteur-0.1.1/src/pasteur/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,17 @@
+""" Contains the definition for Transformer and ReferenceTransformer modules. """
+
 import logging
 import pandas as pd
 
 from .module import ModuleClass, ModuleFactory
 from .attribute import Attribute
 
 logger = logging.getLogger(__name__)
 
-"""Package with base transformers. 
-
-Contains transformers that convert raw data into 2 types (with name suffix):
-    - numerical (num): floating point values (float32), including NaN
-    - discrete (idx): integer values (uintX) with metadata that make them:
-        - categorical: integer values from 0-N with columns with no relations
-        - ordinal: integer values from 0-N where `k` val is closer to `k + 1` than other vals.
-        - hierarchical: contains a hierarchy of ordinal and categorical values.
-"""
-
 
 class TransformerFactory(ModuleFactory):
     ...
 
 
 class Transformer(ModuleClass):
     _factory = TransformerFactory
```

### Comparing `pasteur-0.1.0/src/pasteur/utils/__init__.py` & `pasteur-0.1.1/src/pasteur/utils/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+""" Pasteur's data utilities. The main funcitonality provided by this module
+is `LazyPartition` and `LazyDataset`, with their specializations for `pandas`:
+`LazyFrame`, `LazyChunk`.
+
+These data types allow for loading dataset partitions on command, and when the
+data is no longer useful, evacuating it from RAM using the `del` keyword."""
 from __future__ import annotations
 
 from functools import partial, update_wrapper
 from itertools import chain
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    NamedTuple,
     TypeVar,
     Generic,
     overload,
     Mapping,
     ParamSpec,
 )
 import logging
@@ -19,14 +26,32 @@
 
 A = TypeVar("A")
 B = TypeVar("B")
 P = ParamSpec("P")
 
 logger = logging.getLogger(__name__)
 
+class RawSource(NamedTuple):
+    """ Represents a raw data source that can be downloaded.
+
+    `files` is a list or a single URI that points to an S3 directory, index listing,
+    or file.
+
+    Files will be saved to `<raw_directory>/<save_name>` or the raw source name/dataset
+    name if not provided..
+    HTTP basic auth is supported and can be enabled by setting `credentials` to True.
+    `description` is shown by the command `pasteur download` and should contain
+    licensing information.
+    
+    @warning: Experimental API, subject to change."""
+    
+    files: str | list[str]
+    save_name: str | None = None
+    credentials: bool = False
+    desc: str | None = None
 
 class LazyPartition(Generic[A]):
     def __init__(
         self,
         fun: Callable[..., A],
         shape_fun: Callable[..., tuple[int, ...]] | None,
         /,
```

### Comparing `pasteur-0.1.0/src/pasteur/utils/leaks.py` & `pasteur-0.1.1/src/pasteur/utils/leaks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Simple wrapper that helps with finding memory leaks.
+""" Simple wrapper module that helps with finding memory leaks.
 
 >>> from pasteur.utils.leaks import clear, check, graph
 >>> clear()
 >>> a = suspicious_fun()
 >>> del a # remove result of function
 >>> check() # prints new objects, should be empty or contain misc. python objects
 
@@ -33,40 +33,45 @@
 BlockManager               4        +1 < suspicious
 ExtensionBlock             2        +1 < suspicious
 IntegerArray               2        +1 < suspicious
 ```"""
 
 import logging
 
-try:
-    import objgraph
-except:
-    print("Module 'objgraph' is required to use this module.")
-    raise
+def _get_obj():
+    try:
+        import objgraph # type: ignore
+        return objgraph
+    except:
+        print("Module 'objgraph' is required to use this module.")
+        raise
 
 logger = logging.getLogger(__name__)
 
 
 def clear():
+    objgraph = _get_obj()
     objgraph.growth()
 
 
 def check(info: str):
+    objgraph = _get_obj()
     result = objgraph.growth(1000)
     if not result:
         return
 
     width = max(len(name) for name, _, _ in result)
     for name, count, delta in result:
         info += "\n%-*s%9d %+9d" % (width, name, count, delta)
 
     logger.warning(info)
 
 
 def graph(name: str):
+    objgraph = _get_obj()
     import random
     from io import StringIO
     from urllib.parse import quote
 
     with StringIO() as output:
         objgraph.show_chain(
             objgraph.find_backref_chain(
```

### Comparing `pasteur-0.1.0/src/pasteur/utils/logging.py` & `pasteur-0.1.1/src/pasteur/utils/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+""" Logging logic that stores loges in mlflow runs. """
+
 from io import StringIO
 from logging import Handler, getLevelName
 from os import path
 from time import time
 from weakref import WeakSet
 
 import mlflow
@@ -46,15 +48,15 @@
         Handler.__init__(self)
         self._handlers.add(self)
 
         self._mlflow = None
         self.name = name
         self.logdir = logdir
 
-        self.interval = interval
+        self.interval = int(interval)
         self.last_sent = time()
 
         self.stream = StringIO()
 
     def flush(self):
         self.acquire()
         try:
@@ -94,7 +96,9 @@
             self.steam = StringIO()
         finally:
             self.release()
 
     def __repr__(self):
         level = getLevelName(self.level)
         return "<Mlflow handler %s(%s)>" % (self.name, level)
+
+__all__ = ["MlflowHandler"]
```

### Comparing `pasteur-0.1.0/src/pasteur/utils/mlflow.py` & `pasteur-0.1.1/src/pasteur/utils/mlflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+""" Mlflow utility functions.
+
+@TODO: refactor and clean the functions provided by this module."""
+
 from io import BytesIO
 
 import pandas as pd
 from matplotlib.figure import Figure
 from pandas.io.formats.style import Styler
 
 from .styles import use_style
```

### Comparing `pasteur-0.1.0/src/pasteur/utils/parser.py` & `pasteur-0.1.1/src/pasteur/utils/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-from typing import TypeVar, Any
+""" Parsing related utility functions. """
+
+from typing import Any, TypeVar
+
+from ..module import Module
 
 
 def _try_convert_to_numeric(value: str):
     """Taken from kedro.framework.cli.utils"""
     try:
-        value = float(value)
+        value = float(value) # type: ignore
     except ValueError:
         return value
-    return int(value) if value.is_integer() else value
+    return int(value) if value.is_integer() else value # type: ignore
 
 
-def _try_convert_primitive(value: any):
+def _try_convert_primitive(value: Any):
     """Converts string value to integer/float/bool/None."""
     if value == "True":
         return True
     if value == "False":
         return False
     if value == "None":
         return None
@@ -22,28 +26,28 @@
 
 
 def _try_convert_eval(value: str, locals: dict[str, object]):
     return eval(value, {}, locals)
 
 
 def _update_value_nested_dict(
-    nested_dict: dict[str, any], value: any, walking_path: list[str]
+    nested_dict: dict[str, Any], value: Any, walking_path: list[str]
 ) -> dict:
     """Taken from kedro.framework.cli.utils"""
     key = walking_path.pop(0)
     if not walking_path:
         nested_dict[key] = value
         return nested_dict
     nested_dict[key] = _update_value_nested_dict(
         nested_dict.get(key, {}), value, walking_path
     )
     return nested_dict
 
 
-def str_params_to_dict(params: list[str], locals: dict[str, any] = {}):
+def str_params_to_dict(params: list[str], locals: dict[str, Any] = {}):
     """Converts a list of format ["a.b.c=5", "c=b"] to {a: {b: {c:5}}, c: 'b'}.
 
     Note the number conversion."""
 
     param_dict = {}
     for item in params:
         item = item.split("=", 1)
@@ -55,15 +59,15 @@
         value = item[1].strip()
         param_dict = _update_value_nested_dict(
             param_dict, _try_convert_eval(value, locals), key.split(".")
         )
     return param_dict
 
 
-def eval_params(params: list[str], locals: dict[str, any] = {}):
+def eval_params(params: list[str], locals: dict[str, Any] = {}):
     return {
         name: _try_convert_eval(value, locals)
         for name, value in map(lambda x: x.split("=", 1), params)
     }
 
 
 def merge_params(params: dict[str, Any]):
@@ -71,42 +75,42 @@
 
     for key, val in params.items():
         param_dict = _update_value_nested_dict(param_dict, val, key.split("."))
 
     return param_dict
 
 
-def flat_params_to_dict(params: dict[str, any]):
+def flat_params_to_dict(params: dict[str, Any]):
     """Converts a list of format {a.b.c: 5, c: b} to {a: {b: {c:5}}, c: 'b'}.
 
     Note the number conversion."""
 
     param_dict = {}
     for key, value in params.items():
         if not key:
             raise
         param_dict = _update_value_nested_dict(
             param_dict, _try_convert_to_numeric(value), key.split(".")
         )
     return param_dict
 
 
-def dict_to_flat_params(params: dict[str, any]) -> dict[str, str]:
+def dict_to_flat_params(params: dict[str, Any]) -> dict[str, str]:
     out = {}
     for param, val in params.items():
         if not isinstance(val, dict):
             out[param] = val
         else:
             exp = dict_to_flat_params(val)
             for nest_param, nest_val in exp.items():
                 out[f"{param}.{nest_param}"] = nest_val
     return out
 
 
-CLS = TypeVar("CLS")
+CLS = TypeVar("CLS", bound=Module)
 
 
 def _find_subclasses(cls: type[CLS]) -> dict[str, type[CLS]]:
     """Returns all the subclasses of a given class."""
 
     sub_cls = {}
 
@@ -149,11 +153,11 @@
 
 def get_params_for_pipe(name: str, params: dict):
     """Returns the parameters for the provided pipeline by merging
     the nodes `default`, `<view>` and the top level one in one dictionary.
 
     This allows the user to set default values for all views in the `default`
     namespace, view specific overriding params in the `<view>` namespace and
-    override any of them using the `--params` argument without having to use
+    override Any of them using the `--params` argument without having to use
     the parameter namespace"""
     view = name.split(".")[0]
     return merge_dicts(params.get("default", {}), params.get(view, {}), params)
```

### Comparing `pasteur-0.1.0/src/pasteur/utils/perf.py` & `pasteur-0.1.1/src/pasteur/utils/perf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+""" This module provides a class named PerformanceTracker, which logs runtime
+stats to mlflow."""
+
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
 class PerformanceTracker:
```

### Comparing `pasteur-0.1.0/src/pasteur/utils/progress.py` & `pasteur-0.1.1/src/pasteur/utils/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-"""Wraps the tqdm module so the same modules are used across the project.
+""" This utility module provides constants and functions for multiprocessing
+and progress monitoring in Pasteur.
 
-Deals with vs code jupyter not supporting multiple progress bars."""
+In most cases, the functions and constants are simple wrappers around existing libraries.
+The common use of the primitives in the codebase allows for using different
+implementations in the future."""
 
 import functools
 import io
 import logging
 import sys
 import time
 from contextlib import contextmanager
@@ -254,14 +257,15 @@
         init_pool()
 
     assert _pool is not None
     return _pool
 
 
 def get_manager():
+    """ Returns the manager of the current process pool. """
     return _get_pool()[1]
 
 
 _node_name: Any | None = None
 
 
 def set_node_name(name: str):
@@ -530,10 +534,17 @@
             c.file = rich_fn
 
 
 __all__ = [
     "MULTIPROCESS_ENABLE",
     "piter",
     "prange",
+    "process",
+    "process_async",
     "process_in_parallel",
     "logging_redirect_pbar",
+    "init_pool",
+    "close_pool",
+    "get_manager",
+    "set_node_name",
+    "get_node_name"
 ]
```

### Comparing `pasteur-0.1.0/src/pasteur/view.py` & `pasteur-0.1.1/src/pasteur/view.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+""" This module holds the definitions for the View module, which appropriately
+preprocesses Datasets in Pasteur. """
+
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, overload
+from typing import TYPE_CHECKING, Any
 
 from .module import Module
 from .utils import LazyFrame, LazyChunk, to_chunked
 from .utils.progress import process_in_parallel
 
 if TYPE_CHECKING:
     import pandas as pd
@@ -136,36 +139,49 @@
     a particular order. `trn_deps` defines that order. It needs to be static,
     so it can't be placed in `parameters.yml`
 
     `parameters_fn`, if provided, will be used to load a parameters file with
     defaults for the view (such as metadata). Useful for packaging.
     Use `utils.get_relative_fn()` from datasets."""
 
-    dataset: str
+    dataset: str = ""
+    """The name of the View's Dataset. If the Dataset is not loaded, the View
+    is disabled."""
+
     deps: dict[str, list[str]] = {}
+    """ Defines the Tables of the View and their Dataset dependencies, ex.:
+    
+    ```python
+    {"table1": ["master_table1", "master_table2"], "table2": ["master_table3"]}
+    ```
+    """
     trn_deps: dict[str, list[str]] = {}
     parameters: dict[str, Any] | str | None = None
-    tabular: bool = False
 
     def __init__(self, **_) -> None:
         pass
 
     @property
     def dataset_tables(self):
+        """Returns the dataset tables required by the View."""
         from functools import reduce
 
         return list(dict.fromkeys(reduce(lambda a, b: a + b, self.deps.values(), [])))
 
     @property
     def tables(self):
+        """Returns the table names of the view."""
         return list(self.deps.keys())
-
-    def ingest(self, name, **tables: LazyFrame):
-        """Creates the table <name> using the tables provided based on the dependencies."""
-        raise NotImplementedError()
+    
+    def query(self, name, **tables: LazyFrame):
+        """ Equivalent to ingest in Dataset. """
+        if hasattr(self, "ingest"):
+            # Original name for function was ingest.
+            return getattr(self, "ingest")(name, **tables)
+        raise NotImplemented()
 
     def split_keys(
         self,
         keys: LazyFrame,
         req_splits: list[str] | None,
         splits: dict[str, Any],
         random_state: int,
@@ -183,17 +199,19 @@
         return filter_by_keys(keys, tables[name])
 
     def __str__(self) -> str:
         return self.name
 
 
 class TabularView(View):
+    """Boilerplate for views that are based on tabular datasets.
+    Has one table, named `table`, which is a copy of the table `table` of its
+    Dataset."""
     deps = {"table": ["table"]}
-    tabular: bool = True
 
     @to_chunked
     def ingest(self, name, **tables: LazyChunk):
         assert name == "table"
         return tables["table"]()
 
 
-__all__ = ["View", "TabularView", "filter_by_keys"]
+__all__ = ["View", "TabularView", "split_keys", "filter_by_keys"]
```

### Comparing `pasteur-0.1.0/src/pasteur.egg-info/PKG-INFO` & `pasteur-0.1.1/src/pasteur.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasteur
-Version: 0.1.0
+Version: 0.1.1
 Summary: A system for reproducible and scalable data synthesis.
 Author-email: Kapenekakis Antheas <antheas@cs.aau.dk>
 Project-URL: Homepage, https://pasteur.dev
 Project-URL: Bug Tracker, https://github.com/pasteur-dev/pasteur/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,13 +13,13 @@
 Provides-Extra: opt
 Provides-Extra: test
 Provides-Extra: cls
 Provides-Extra: docs
 License-File: LICENSE
 
 
-![Pasteur Logo with text. Tagline reads: 'Sanitize Your Data'](https://raw.githubusercontent.com/pasteur-dev/pasteur-web/master/assets/img/logo_text_light.svg)
+![Pasteur Logo with text. Tagline reads: 'Sanitize Your Data'](https://raw.githubusercontent.com/pasteur-dev/pasteur/master/res/logo/text_light.svg)
 
 Pasteur is a system for data synthesis in a prototype state.
 Head to https://pasteur.dev or https://github.com/pasteur-dev/pasteur for
 more information.
-Documentation and project template coming soon!
+Documentation coming soon!
```

