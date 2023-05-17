# Comparing `tmp/pyreason-1.5.1.tar.gz` & `tmp/pyreason-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.5.1.tar", last modified: Mon May 15 17:35:47 2023, max compression
+gzip compressed data, was "pyreason-1.5.2.tar", last modified: Wed May 17 09:42:38 2023, max compression
```

## Comparing `pyreason-1.5.1.tar` & `pyreason-1.5.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.578042 pyreason-1.5.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-15 17:35:36.000000 pyreason-1.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 17:35:36.000000 pyreason-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-15 17:35:47.578042 pyreason-1.5.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-15 17:35:36.000000 pyreason-1.5.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.570042 pyreason-1.5.1/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.570042 pyreason-1.5.1/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.570042 pyreason-1.5.1/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    27566 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.574042 pyreason-1.5.1/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.574042 pyreason-1.5.1/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.574042 pyreason-1.5.1/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.574042 pyreason-1.5.1/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/facts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.574042 pyreason-1.5.1/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    70360 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.574042 pyreason-1.5.1/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.574042 pyreason-1.5.1/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.574042 pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10901 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.574042 pyreason-1.5.1/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.574042 pyreason-1.5.1/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.578042 pyreason-1.5.1/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/utils/plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9056 2023-05-15 17:35:36.000000 pyreason-1.5.1/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:35:47.570042 pyreason-1.5.1/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-15 17:35:47.000000 pyreason-1.5.1/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-15 17:35:47.000000 pyreason-1.5.1/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:35:47.000000 pyreason-1.5.1/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 17:35:47.000000 pyreason-1.5.1/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 17:35:47.000000 pyreason-1.5.1/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:35:47.578042 pyreason-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-15 17:35:36.000000 pyreason-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.437632 pyreason-1.5.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-17 09:42:23.000000 pyreason-1.5.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 09:42:23.000000 pyreason-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-17 09:42:38.437632 pyreason-1.5.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-17 09:42:23.000000 pyreason-1.5.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.425632 pyreason-1.5.2/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.425632 pyreason-1.5.2/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.429632 pyreason-1.5.2/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27119 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.429632 pyreason-1.5.2/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.429632 pyreason-1.5.2/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.429632 pyreason-1.5.2/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.433632 pyreason-1.5.2/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/facts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.433632 pyreason-1.5.2/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70954 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.433632 pyreason-1.5.2/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.433632 pyreason-1.5.2/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.437632 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10901 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.437632 pyreason-1.5.2/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.437632 pyreason-1.5.2/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.437632 pyreason-1.5.2/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9056 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.425632 pyreason-1.5.2/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-17 09:42:38.000000 pyreason-1.5.2/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-17 09:42:38.000000 pyreason-1.5.2/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:42:38.000000 pyreason-1.5.2/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 09:42:38.000000 pyreason-1.5.2/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 09:42:38.000000 pyreason-1.5.2/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:42:38.437632 pyreason-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-17 09:42:23.000000 pyreason-1.5.2/setup.py
```

### Comparing `pyreason-1.5.1/LICENSE.md` & `pyreason-1.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/PKG-INFO` & `pyreason-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.5.1
+Version: 1.5.2
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.5.1/README.md` & `pyreason-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/__init__.py` & `pyreason-1.5.2/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.5.2/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.5.2/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.5.2/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/pyreason.py` & `pyreason-1.5.2/pyreason/pyreason.py`

 * *Files 2% similar despite different names*

```diff
@@ -473,24 +473,23 @@
 
     # Add to collection of rules
     if __rules is None:
         __rules = numba.typed.List.empty_list(rule.rule_type)
     __rules.append(r)
 
 
-def reason(timesteps: int=-1, convergence_threshold: int=-1, convergence_bound_threshold: float=-1, again: bool=False, node_facts: List[Type[fact_node.Fact]]=None, edge_facts: List[Type[fact_edge.Fact]]=None, include_graph_facts: bool=True):
+def reason(timesteps: int=-1, convergence_threshold: int=-1, convergence_bound_threshold: float=-1, again: bool=False, node_facts: List[Type[fact_node.Fact]]=None, edge_facts: List[Type[fact_edge.Fact]]=None):
     """Function to start the main reasoning process. Graph and rules must already be loaded.
 
-    :param timesteps: Max number of timesteps to run. -1 specifies run till convergence, defaults to -1
+    :param timesteps: Max number of timesteps to run. -1 specifies run till convergence. If reasoning again, this is the number of timesteps to reason for extra (no zero timestep), defaults to -1
     :param convergence_threshold: Maximim number of interpretations that have changed between timesteps or fixed point operations until considered convergent. Program will end at convergence. -1 => no changes, perfect convergence, defaults to -1
     :param convergence_bound_threshold: Maximum change in any interpretation (bounds) between timesteps or fixed point operations until considered convergent, defaults to -1
     :param again: Whether to reason again on an existing interpretation, defaults to False
     :param node_facts: New node facts to use during the next reasoning process. Other facts from file will be discarded, defaults to None
     :param edge_facts: New edge facts to use during the next reasoning process. Other facts from file will be discarded, defaults to None
-    :param include_graph_facts: Whether to add the graph facts to the facts supplied through `node_facts`, defaults to True
     :return: The final interpretation after reasoning.
     """
     global settings, __timestamp
 
     # Timestamp for saving files
     __timestamp = time.strftime('%Y%m%d-%H%M%S')
 
@@ -503,18 +502,18 @@
             mem_usage, interp = mp.memory_usage((_reason, [timesteps, convergence_threshold, convergence_bound_threshold]), max_usage=True, retval=True)
             print(f"\nProgram used {mem_usage-start_mem} MB of memory")
         else:
             interp = _reason(timesteps, convergence_threshold, convergence_bound_threshold)
     else:
         if settings.memory_profile:
             start_mem = mp.memory_usage(max_usage=True)
-            mem_usage, interp = mp.memory_usage((_reason_again, [timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts, include_graph_facts]), max_usage=True, retval=True)
+            mem_usage, interp = mp.memory_usage((_reason_again, [timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts]), max_usage=True, retval=True)
             print(f"\nProgram used {mem_usage-start_mem} MB of memory")
         else:
-            interp = _reason_again(timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts, include_graph_facts)
+            interp = _reason_again(timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts)
         
     return interp
 
 
 def _reason(timesteps, convergence_threshold, convergence_bound_threshold):
     # Globals
     global __graph, __rules, __node_facts, __edge_facts, __ipl, __node_labels, __edge_labels, __specific_node_labels, __specific_edge_labels, __graphml_parser
@@ -559,56 +558,48 @@
             __specific_node_labels[label_name] = nodes
 
     for label_name, edges in __specific_graph_edge_labels.items():
         if label_name in __specific_edge_labels:
             __specific_edge_labels[label_name].extend(edges)
         else:
             __specific_edge_labels[label_name] = edges
-    __node_facts.extend(__non_fluent_graph_facts_node)
-    __edge_facts.extend(__non_fluent_graph_facts_edge)   
+
+    all_node_facts = numba.typed.List(__node_facts)
+    all_edge_facts = numba.typed.List(__edge_facts)
+    all_node_facts.extend(__non_fluent_graph_facts_node)
+    all_edge_facts.extend(__non_fluent_graph_facts_edge)
 
     # Setup logical program
-    __program = Program(__graph, __node_facts, __edge_facts, __rules, __ipl, settings.reverse_digraph, settings.atom_trace, settings.save_graph_attributes_to_trace, settings.canonical, settings.inconsistency_check)
+    __program = Program(__graph, all_node_facts, all_edge_facts, __rules, __ipl, settings.reverse_digraph, settings.atom_trace, settings.save_graph_attributes_to_trace, settings.canonical, settings.inconsistency_check)
     __program.available_labels_node = __node_labels
     __program.available_labels_edge = __edge_labels
     __program.specific_node_labels = __specific_node_labels
     __program.specific_edge_labels = __specific_edge_labels
 
     # Run Program and get final interpretation
     interpretation = __program.reason(timesteps, convergence_threshold, convergence_bound_threshold, settings.verbose)
 
     return interpretation
 
 
-def _reason_again(timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts, include_graph_facts):
+def _reason_again(timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts):
     # Globals
     global __graph, __rules, __node_facts, __edge_facts, __ipl, __node_labels, __edge_labels, __specific_node_labels, __specific_edge_labels, __graphml_parser
     global settings, __timestamp, __program
 
     assert __program is not None, 'To run `reason_again` you need to have reasoned once before'
 
-    # If facts have not been inputted, use the old facts
-    __program.interp.facts_to_be_applied_node.clear()
-    __program.interp.facts_to_be_applied_edge.clear()
+    # Extend current set of nodes with the new nodes supplied
     if node_facts is not None:
-        node_facts = numba.typed.List(node_facts)
-        if include_graph_facts:
-            node_facts.extend(__non_fluent_graph_facts_node)
-    else:
-        node_facts = numba.typed.List.empty_list(fact_node.fact_type)
-
+        __node_facts.extend(numba.typed.List(node_facts))
     if edge_facts is not None:
-        edge_facts = numba.typed.List(edge_facts)
-        if include_graph_facts:
-            edge_facts.extend(__non_fluent_graph_facts_edge)
-    else:
-        edge_facts = numba.typed.List.empty_list(fact_edge.fact_type)
+        __edge_facts.extend(numba.typed.List(edge_facts))
 
     # Run Program and get final interpretation
-    interpretation = __program.reason_again(timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts, settings.verbose)
+    interpretation = __program.reason_again(timesteps, convergence_threshold, convergence_bound_threshold, __node_facts, __edge_facts, settings.verbose)
 
     return interpretation
 
 
 def save_rule_trace(interpretation, folder: str='./'):
     """Saves the trace of the program. This includes every change that has occured to the interpretation. If `atom_trace` was set to true
     this gives us full explainability of why interpretations changed
```

### Comparing `pyreason-1.5.1/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.5.2/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/args.py` & `pyreason-1.5.2/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/components/world.py` & `pyreason-1.5.2/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/diffuse.py` & `pyreason-1.5.2/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.5.2/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/facts/fact_node.py` & `pyreason-1.5.2/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.5.2/pyreason/scripts/interpretation/interpretation.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,18 @@
 		self.graph = graph
 		self.ipl = ipl
 		self.reverse_graph = reverse_graph
 		self.atom_trace = atom_trace
 		self.save_graph_attributes_to_rule_trace = save_graph_attributes_to_rule_trace
 		self.canonical = canonical
 		self.inconsistency_check = inconsistency_check
+
+		# For reasoning and reasoning again (contains previous time and previous fp operation cnt)
 		self.time = 0
+		self.prev_reasoning_data = numba.typed.List([0, 0])
 
 		# Initialize list of tuples for rules/facts to be applied, along with all the ground atoms that fired the rule. One to One correspondence between rules_to_be_applied_node and rules_to_be_applied_node_trace if atom_trace is true
 		self.rules_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.rules_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.facts_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.string)
 		self.facts_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.string)
 		self.rules_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, node_type, label.label_type, interval.interval_type, numba.types.boolean)))
@@ -72,29 +75,27 @@
 		# Setup graph neighbors
 		self.neighbors = numba.typed.Dict.empty(key_type=node_type, value_type=numba.types.ListType(node_type))
 		for n in self.graph.nodes():
 			l = numba.typed.List.empty_list(node_type)
 			[l.append(neigh) for neigh in self.graph.neighbors(n)]
 			self.neighbors[n] = l
 
-
 	@staticmethod
 	@numba.njit(cache=True)
 	def _init_interpretations_node(nodes, available_labels, specific_labels):
 		interpretations = numba.typed.Dict.empty(key_type=node_type, value_type=world.world_type)
 		# General labels
 		for n in nodes:
 			interpretations[n] = world.World(available_labels)
 		# Specific labels
 		for l, ns in specific_labels.items():
 			for n in ns:
 				interpretations[n].world[l] = interval.closed(0.0, 1.0)
 
 		return interpretations
-
 	
 	@staticmethod
 	@numba.njit(cache=True)
 	def _init_interpretations_edge(edges, available_labels, specific_labels):
 		interpretations = numba.typed.Dict.empty(key_type=edge_type, value_type=world.world_type)
 		# General labels
 		for e in edges:
@@ -115,23 +116,21 @@
 		elif convergence_bound_threshold==-1:
 			convergence_mode = 'delta_interpretation'
 			convergence_delta = convergence_threshold
 		else:
 			convergence_mode = 'delta_bound'
 			convergence_delta = convergence_bound_threshold
 		return convergence_mode, convergence_delta
-		
 
 	def start_fp(self, tmax, facts_node, facts_edge, rules, verbose, convergence_threshold, convergence_bound_threshold):
 		self.tmax = tmax
 		self._convergence_mode, self._convergence_delta = self._init_convergence(convergence_bound_threshold, convergence_threshold)
 		max_facts_time = self._init_facts(facts_node, facts_edge, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.atom_trace)
 		self._start_fp(rules, max_facts_time, verbose)
 
-
 	@staticmethod
 	@numba.njit(cache=True)
 	def _init_facts(facts_node, facts_edge, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, atom_trace):
 		max_time = 0
 		for fact in facts_node:
 			for t in range(fact.get_time_lower(), fact.get_time_upper() + 1):
 				max_time = max(max_time, t)
@@ -146,29 +145,30 @@
 				name = fact.get_name()
 				graph_attribute = True if name=='graph-attribute-fact' else False
 				facts_to_be_applied_edge.append((numba.types.int8(t), fact.get_component(), fact.get_label(), fact.get_bound(), fact.static, graph_attribute))
 				if atom_trace:
 					facts_to_be_applied_edge_trace.append(fact.get_name())
 		return max_time
 
-		
 	def _start_fp(self, rules, max_facts_time, verbose):
-		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, rules, self.nodes, self.edges, self.neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.available_labels_node, self.available_labels_edge, self.specific_node_labels, self.specific_edge_labels, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, max_facts_time, self._convergence_mode, self._convergence_delta, verbose)
-		self.time = t
+		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, self.prev_reasoning_data, rules, self.nodes, self.edges, self.neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.available_labels_node, self.available_labels_edge, self.specific_node_labels, self.specific_edge_labels, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, max_facts_time, self._convergence_mode, self._convergence_delta, verbose)
+		self.time = t - 1
+		# If we need to reason again, store the next timestep to start from
+		self.prev_reasoning_data[0] = t
+		self.prev_reasoning_data[1] = fp_cnt
 		if verbose:
 			print('Fixed Point iterations:', fp_cnt)
 
-
 	@staticmethod
 	@numba.njit(cache=True)
-	def reason(interpretations_node, interpretations_edge, tmax, rules, nodes, edges, neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, labels_node, labels_edge, specific_labels_node, specific_labels_edge, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, max_facts_time, convergence_mode, convergence_delta, verbose):
-		fp_cnt = 0
+	def reason(interpretations_node, interpretations_edge, tmax, prev_reasoning_data, rules, nodes, edges, neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, labels_node, labels_edge, specific_labels_node, specific_labels_edge, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, max_facts_time, convergence_mode, convergence_delta, verbose):
+		t = prev_reasoning_data[0]
+		fp_cnt = prev_reasoning_data[1]
 		max_rules_time = 0
 		timestep_loop = True
-		t = 0
 		while timestep_loop:
 			if t==tmax:
 				timestep_loop=False
 			if verbose:
 				with objmode():
 					print('Timestep:', t, flush=True)
 			# Reset Interpretation at beginning of timestep if non-canonical
@@ -581,27 +581,33 @@
 			# Check for convergence after each timestep (perfect convergence or convergence specified by user)
 			# Check number of changed interpretations or max bound change
 			# User specified convergence
 			if convergence_mode=='delta_interpretation':
 				if changes_cnt <= convergence_delta:
 					if verbose:
 						print(f'\nConverged at time: {t} with {int(changes_cnt)} changes from the previous interpretation')
+					# Be consistent with time returned when we don't converge
+					t += 1
 					break
 			elif convergence_mode=='delta_bound':
 				if bound_delta <= convergence_delta:
 					if verbose:
 						print(f'\nConverged at time: {t} with {float_to_str(bound_delta)} as the maximum bound change from the previous interpretation')
+					# Be consistent with time returned when we don't converge
+					t += 1
 					break
 			# Perfect convergence
 			# Make sure there are no rules to be applied, and no facts that will be applied in the future. We do this by checking the max time any rule/fact is applicable
 			# If no more rules/facts to be applied
 			elif convergence_mode=='perfect_convergence':
 				if (t>=max_facts_time and t>=max_rules_time) or (t>=max_facts_time and changes_cnt==0):
 					if verbose:
-						print(f'\nConverged at time: {t}')					
+						print(f'\nConverged at time: {t}')
+					# Be consistent with time returned when we don't converge
+					t += 1
 					break
 
 			# Increment t
 			t += 1
 
 		return fp_cnt, t
```

### Comparing `pyreason-1.5.1/pyreason/scripts/interval/interval.py` & `pyreason-1.5.2/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/program/program.py` & `pyreason-1.5.2/pyreason/scripts/program/program.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,12 +30,13 @@
 
 		self.interp = Interpretation(self._graph, self._ipl, self._reverse_graph, self._atom_trace, self._save_graph_attributes_to_rule_trace, self._canonical, self._inconsistency_check)
 		self.interp.start_fp(self._tmax, self._facts_node, self._facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold)
 
 		return self.interp
 	
 	def reason_again(self, tmax, convergence_threshold, convergence_bound_threshold, facts_node, facts_edge, verbose=True):
-		self._tmax = tmax
-		self.interp.start_fp(tmax, facts_node, facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold)
+		assert self.interp is not None, 'Call reason before calling reason again'
+		self._tmax = self.interp.time + tmax
+		self.interp.start_fp(self._tmax, facts_node, facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold)
 
 		return self.interp
```

### Comparing `pyreason-1.5.1/pyreason/scripts/rules/rule.py` & `pyreason-1.5.2/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/utils/filter.py` & `pyreason-1.5.2/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.5.2/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/utils/output.py` & `pyreason-1.5.2/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/utils/plotter.py` & `pyreason-1.5.2/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/utils/visuals.py` & `pyreason-1.5.2/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.5.2/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/pyreason.egg-info/PKG-INFO` & `pyreason-1.5.2/pyreason.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.5.1
+Version: 1.5.2
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.5.1/pyreason.egg-info/SOURCES.txt` & `pyreason-1.5.2/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.1/setup.py` & `pyreason-1.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name = 'pyreason',
-    version = '1.5.1',
+    version = '1.5.2',
     author = 'Dyuman Aditya',
     author_email = 'dyuman.aditya@gmail.com',
     description = 'An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/lab-v2/pyreason',
     license = 'BSD 3-clause',
```

