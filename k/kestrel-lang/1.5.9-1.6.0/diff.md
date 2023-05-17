# Comparing `tmp/kestrel-lang-1.5.9.tar.gz` & `tmp/kestrel-lang-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel-lang-1.5.9.tar", last modified: Fri Feb 17 22:47:08 2023, max compression
+gzip compressed data, was "kestrel-lang-1.6.0.tar", last modified: Wed May 17 20:40:51 2023, max compression
```

## Comparing `kestrel-lang-1.5.9.tar` & `kestrel-lang-1.6.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.207566 kestrel-lang-1.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-17 22:47:08.207566 kestrel-lang-1.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.183565 kestrel-lang-1.5.9/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/bin/kestrel
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-17 22:47:08.207566 kestrel-lang-1.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.183565 kestrel-lang-1.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.187565 kestrel-lang-1.5.9/src/kestrel/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.187565 kestrel-lang-1.5.9/src/kestrel/absinterface/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/absinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/absinterface/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.187565 kestrel-lang-1.5.9/src/kestrel/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/analytics/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/analytics/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.191566 kestrel-lang-1.5.9/src/kestrel/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.191566 kestrel-lang-1.5.9/src/kestrel/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/datasource/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/datasource/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/datasource/retstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.191566 kestrel-lang-1.5.9/src/kestrel/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/semantics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/semantics/completor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/semantics/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/semantics/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.195566 kestrel-lang-1.5.9/src/kestrel/symboltable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/symboltable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/symboltable/symtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/symboltable/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.195566 kestrel-lang-1.5.9/src/kestrel/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/ecgpattern.lark
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/ecgpattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/kestrel.lark
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/reference.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.195566 kestrel-lang-1.5.9/src/kestrel_analytics_docker/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_docker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.199566 kestrel-lang-1.5.9/src/kestrel_analytics_python/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_python/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.199566 kestrel-lang-1.5.9/src/kestrel_datasource_stixbundle/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixbundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixbundle/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.199566 kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.199566 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-17 22:47:08.000000 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-02-17 22:47:08.000000 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 22:47:08.000000 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-17 22:47:08.000000 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-17 22:47:08.000000 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.207566 kestrel-lang-1.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_find.py
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_python_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_stixshifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_timestamped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.523588 kestrel-lang-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-17 20:40:51.523588 kestrel-lang-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.499588 kestrel-lang-1.6.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/bin/kestrel
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-17 20:40:51.523588 kestrel-lang-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.495588 kestrel-lang-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.499588 kestrel-lang-1.6.0/src/kestrel/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.503588 kestrel-lang-1.6.0/src/kestrel/absinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/absinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/absinterface/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.503588 kestrel-lang-1.6.0/src/kestrel/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/analytics/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/analytics/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.503588 kestrel-lang-1.6.0/src/kestrel/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25803 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.507588 kestrel-lang-1.6.0/src/kestrel/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/datasource/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/datasource/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/datasource/retstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.507588 kestrel-lang-1.6.0/src/kestrel/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/semantics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/semantics/completor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/semantics/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/semantics/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20339 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.507588 kestrel-lang-1.6.0/src/kestrel/symboltable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/symboltable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/symboltable/symtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/symboltable/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.511588 kestrel-lang-1.6.0/src/kestrel/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/ecgpattern.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/ecgpattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/kestrel.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.511588 kestrel-lang-1.6.0/src/kestrel_analytics_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_docker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.511588 kestrel-lang-1.6.0/src/kestrel_analytics_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_python/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.515588 kestrel-lang-1.6.0/src/kestrel_datasource_stixbundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixbundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixbundle/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.515588 kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17937 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.515588 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-17 20:40:51.000000 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-17 20:40:51.000000 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:40:51.000000 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 20:40:51.000000 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 20:40:51.000000 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.523588 kestrel-lang-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_fast_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_python_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_stixshifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.5.9/AUTHORS.rst` & `kestrel-lang-1.6.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/LICENSE.md` & `kestrel-lang-1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/PKG-INFO` & `kestrel-lang-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.5.9
+Version: 1.6.0
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
 .. image:: https://github.com/opencybersecurityalliance/kestrel-lang/raw/develop/logo/logo_w_text.svg
    :width: 432
    :alt: Kestrel Threat Hunting Language
```

### Comparing `kestrel-lang-1.5.9/README.rst` & `kestrel-lang-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/setup.cfg` & `kestrel-lang-1.6.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kestrel-lang
-version = 1.5.9
+version = 1.6.0
 description = Kestrel Threat Hunting Language
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 keywords = 
 	domain specific language
 	cyber threat hunting
 	extended detection and response
@@ -21,26 +21,27 @@
 	Documentation = https://kestrel.readthedocs.io/
 
 [options]
 packages = find:
 package_dir = 
 	=src
 scripts = bin/kestrel
-python_requires = >= 3.7
+python_requires = >= 3.8
 install_requires = 
 	pyyaml
 	lxml
 	pandas
 	requests
+	nest-asyncio>=1.5.6
 	lark>=1.1.5
 	pyarrow>=5.0.0
 	docker>=5.0.0
-	stix-shifter>=4.6.0,<5.0.0
-	stix-shifter-utils>=4.6.0,<5.0.0
-	firepit>=2.3.10
+	stix-shifter>=5.3.0
+	stix-shifter-utils>=5.3.0
+	firepit>=2.3.19
 	typeguard
 tests_require = 
 	pytest
 
 [options.packages.find]
 where = src
```

### Comparing `kestrel-lang-1.5.9/src/kestrel/absinterface/manager.py` & `kestrel-lang-1.6.0/src/kestrel/absinterface/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/analytics/interface.py` & `kestrel-lang-1.6.0/src/kestrel/analytics/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/analytics/manager.py` & `kestrel-lang-1.6.0/src/kestrel/analytics/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/codegen/commands.py` & `kestrel-lang-1.6.0/src/kestrel/codegen/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     compile_generic_relation_to_query,
 )
 from kestrel.codegen.relations import (
     generic_relations,
     compile_identical_entity_search_pattern,
     fine_grained_relational_process_filtering,
     get_entity_id_attribute,
-    stix_2_0_identical_mapping,
     build_pattern_from_ids,
 )
 
 _logger = logging.getLogger(__name__)
 
 
 ################################################################
@@ -117,15 +116,15 @@
         if transform.lower() == "timestamped":
             qry = session.store.timestamped(entity_table, run=False)
         else:
             qry = Query(entity_table)
     else:
         qry = Query(entity_table)
 
-    qry = _build_query(session.store, entity_table, qry, stmt)
+    qry = _build_query(session.store, entity_table, qry, stmt, [])
 
     try:
         session.store.assign_query(stmt["output"], qry)
         output = new_var(session.store, stmt["output"], [], stmt, session.symtable)
     except InvalidAttr as e:
         var_attr = str(e).split()[-1]
         var_name, _, attr = var_attr.rpartition(".")
@@ -262,35 +261,32 @@
         )
         output = new_var(session.store, return_var_table, [], stmt, session.symtable)
         _logger.debug(f"get from variable source \"{stmt['variablesource']}\"")
 
     elif "datasource" in stmt:
         # rs: RetStruct
         rs = session.data_source_manager.query(
-            stmt["datasource"], pattern, session.session_id
+            stmt["datasource"], pattern, session.session_id, session.store
         )
         query_id = rs.load_to_store(session.store)
         session.store.extract(local_var_table, return_type, query_id, pattern)
         _output = new_var(session.store, local_var_table, [], stmt, session.symtable)
         _logger.debug(
             f"native GET pattern executed and DB view {local_var_table} extracted."
         )
 
+        # TODO: add a ECGP method to do this directly
         pat_summary = summarize_pattern(pattern)
-        pat_types = list(pat_summary.keys())
-        if return_type in stix_2_0_identical_mapping:
-            id_attrs = set(stix_2_0_identical_mapping[return_type])
-        else:
-            id_attrs = pat_summary[return_type]  # Hack
+
         if (
-            len(pat_types) == 1
-            and pat_types[0] == return_type
-            and pat_summary[return_type] == id_attrs
+            pat_summary
+            and return_type in pat_summary  # allow extended subgraph
+            and len(pat_summary[return_type]) == 1  # only one attr for center node
+            and pat_summary[return_type].pop() == get_entity_id_attribute(_output)
         ):
-            # Prefetch won't return anything new here, so skip it
             _logger.debug("To skip prefetch for direct query")
             is_direct_query = True
         else:
             is_direct_query = False
 
         if (
             not is_direct_query
@@ -313,15 +309,18 @@
                 session.store,
                 ext_graph_pattern,
                 session.session_id,
                 session.data_source_manager,
                 session.config["stixquery"]["support_id"],
             )
 
-            if return_type == "process" and get_entity_id_attribute(_output) != "id":
+            if return_type == "process" and get_entity_id_attribute(_output) not in (
+                "id",
+                "x_unique_id",
+            ):
                 prefetch_ret_entity_table = _filter_prefetched_process(
                     return_var_table,
                     session,
                     _output,
                     prefetch_ret_entity_table,
                     return_type,
                 )
@@ -434,18 +433,17 @@
                     session.data_source_manager,
                     session.config["stixquery"]["support_id"],
                 )
 
                 # special handling for process to filter out impossible relational processes
                 # this is needed since STIX 2.0 does not have mandatory fields for
                 # process and field like `pid` is not unique
-                if (
-                    return_type == "process"
-                    and get_entity_id_attribute(_output) != "id"
-                ):
+                if return_type == "process" and get_entity_id_attribute(
+                    _output
+                ) not in ("id", "x_unique_id"):
                     prefetch_ret_entity_table = _filter_prefetched_process(
                         return_var_table,
                         session,
                         _output,
                         prefetch_ret_entity_table,
                         return_type,
                     )
@@ -615,15 +613,15 @@
         pattern_ast.extend("AND", where_clause)
         _logger.info(f"prefetch pattern after extend: {pattern_ast}")
         stix_pattern = pattern_ast.to_stix(time_range, time_adj)
         _logger.info(f"STIX pattern generated in prefetch: {stix_pattern}")
 
         if stix_pattern:
             data_source = symtable[input_var_name].data_source
-            resp = ds_manager.query(data_source, stix_pattern, session_id)
+            resp = ds_manager.query(data_source, stix_pattern, session_id, store)
             query_id = resp.load_to_store(store)
 
             # build the return_var_name view in store
             store.extract(return_var_name, return_type, query_id, stix_pattern)
 
             _logger.debug(f"prefetch successful.")
             return return_var_name
@@ -687,15 +685,15 @@
 
 
 def _get_filt_columns(filts: list):
     for filt in filts:
         yield from _get_pred_columns(filt.preds)
 
 
-def _build_query(store, entity_table, qry, stmt):
+def _build_query(store, entity_table, qry, stmt, paths=None):
     where = stmt.get("where")
     if where:
         if isinstance(where, Query):
             for j in where.joins:
                 _logger.debug("Anchoring JOIN to %s", qry.table.name)
                 j.prev_name = qry.table.name
             qry.joins.extend(where.joins)
@@ -705,15 +703,22 @@
                     _logger.debug("Disambiguating predicate for %s", qry.table.name)
                     col.table = qry.table.name
             qry.where.extend(where.where)
         else:
             where.set_table(entity_table)
             qry.append(where)
     attrs = stmt.get("attrs", "*")
-    cols = attrs.split(",")
+    if attrs == "*" and not qry.joins:
+        # If user didn't ask for any paths and the where clause didn't
+        # result in any joins, fallback to the calling function's list
+        # of paths.
+        # https://github.com/opencybersecurityalliance/kestrel-lang/issues/312
+        cols = paths
+    else:
+        cols = attrs.split(",")
     _set_projection(store, entity_table, qry, cols)
     sort_by = stmt.get("attribute")
     if sort_by:
         direction = "ASC" if stmt["ascending"] else "DESC"
         qry.append(Order([(sort_by, direction)]))
     limit = stmt.get("limit")
     if limit:
```

### Comparing `kestrel-lang-1.5.9/src/kestrel/codegen/data.py` & `kestrel-lang-1.6.0/src/kestrel/codegen/data.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/codegen/display.py` & `kestrel-lang-1.6.0/src/kestrel/codegen/display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/codegen/queries.py` & `kestrel-lang-1.6.0/src/kestrel/codegen/queries.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/codegen/relations.py` & `kestrel-lang-1.6.0/src/kestrel/codegen/relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,34 +64,37 @@
     # ("process", "created", "process"): (["child_refs"], ["parent_ref"]),
     ("process", "created", "process"): ([], ["parent_ref"]),
     # service
     ("windows-service-ext", "loaded", "file"): (["service_dll_refs"], []),
     ("windows-service-ext", "loaded", "user-account"): (["creator_user_ref"], []),
 }
 
-# FIXME: is this no longer needed?
 # the first available attribute will be used to uniquely identify the entity
 stix_2_0_identical_mapping = {
     # entity-type: id attributes candidates
     "directory": ("path",),
     "domain-name": ("value",),
     "email-addr": ("value",),
     "file": ("name",),  # optional in STIX standard
     "ipv4-addr": ("value",),
     "ipv6-addr": ("value",),
     "mac-addr": ("value",),
     "mutex": ("name",),
     # `pid` is optional in STIX standard
     # `first_observed` cannot be used since it may be wrong (derived from observation)
     # `command_line` or `name` may not be in data and cannot be used
-    "process": ("pid", "name"),
+    "process": (
+        "x_unique_id",
+        "pid",
+    ),
     "software": ("name",),
     "url": ("value",),
     "user-account": ("user_id",),  # optional in STIX standard
     "windows-registry-key": ("key",),  # optional in STIX standard
+    "x-oca-asset": ("device_id",),  # oca/stix-extension repo
 }
 
 stix_x_ibm_event_mapping = {
     # entity-type to ref in x-oca-event
     "process": "process_ref",
     "domain-name": "domain_ref",
     "file": "file_ref",
```

### Comparing `kestrel-lang-1.5.9/src/kestrel/codegen/summary.py` & `kestrel-lang-1.6.0/src/kestrel/codegen/summary.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/config.py` & `kestrel-lang-1.6.0/src/kestrel/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/config.yaml` & `kestrel-lang-1.6.0/src/kestrel/config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
   default_datasource_schema: "stixshifter"
   default_analytics_schema: "docker"
 
 # how a Kestrel session is executed
 session:
   cache_directory_prefix: "kestrel-session-" # under system temp directory
   local_database_path: "local.db"
+  log_path: "session.log"
   show_execution_summary: true
 
 # whether/how to prefetch all records/observations for entities
 prefetch:
 
   # enable/disable prefetch for command
   #
```

### Comparing `kestrel-lang-1.5.9/src/kestrel/datasource/interface.py` & `kestrel-lang-1.6.0/src/kestrel/datasource/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             [str]: A list of data source names accessible from this interface.
 
         """
         return []
 
     @staticmethod
     @abstractmethod
-    def query(uri, pattern, session_id, config):
+    def query(uri, pattern, session_id, config, store=None):
         """Sending a data query to a specific data source.
 
         If the store of the session is modified and directly gets the data
         loaded into a ``query_id``, it should return
         :attr:`kestrel.datasource.ReturnFromStore`.
 
         If the interface uses local files as intermediate/temporary storage
@@ -100,14 +100,16 @@
 
             session_id (str): id of the session, may be useful for analytics
               directly writing into the store.
 
             config (dict): a layered list/dict that contains config for the
               interface and can be edited/updated by the interface.
 
+            store (firepit.SqlStorage): The internal store used by the session
+
         Returns:
             kestrel.datasource.retstruct.AbstractReturnStruct: returned data.
             Currently there are two choices:
             :attr:`kestrel.datasource.ReturnFromFile` and
             :attr:`kestrel.datasource.ReturnFromStore`.
 
         """
```

### Comparing `kestrel-lang-1.5.9/src/kestrel/datasource/retstruct.py` & `kestrel-lang-1.6.0/src/kestrel/datasource/retstruct.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/exceptions.py` & `kestrel-lang-1.6.0/src/kestrel/exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/semantics/completor.py` & `kestrel-lang-1.6.0/src/kestrel/semantics/completor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/semantics/processor.py` & `kestrel-lang-1.6.0/src/kestrel/semantics/processor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/semantics/reference.py` & `kestrel-lang-1.6.0/src/kestrel/semantics/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/session.py` & `kestrel-lang-1.6.0/src/kestrel/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,19 @@
 from kestrel.syntax.parser import parse_kestrel
 from kestrel.semantics.processor import semantics_processing
 from kestrel.semantics.completor import do_complete
 from kestrel.codegen import commands
 from kestrel.codegen.display import DisplayBlockSummary
 from kestrel.codegen.summary import gen_variable_summary
 from kestrel.symboltable.symtable import SymbolTable
-from kestrel.utils import set_current_working_directory, resolve_path_in_kestrel_env_var
+from kestrel.utils import (
+    set_current_working_directory,
+    resolve_path_in_kestrel_env_var,
+    add_logging_handler,
+)
 from kestrel.config import load_config
 from kestrel.datasource import DataSourceManager
 from kestrel.analytics import AnalyticsManager
 from firepit import get_storage
 from firepit.exceptions import StixPatternError
 
 _logger = logging.getLogger(__name__)
@@ -217,14 +221,16 @@
                     f"create new session runtime_directory: {self.runtime_directory}."
                 )
                 tmp_dir.mkdir(parents=True, exist_ok=True)
 
         if self.debug_mode:
             self._setup_runtime_directory_master()
 
+        self._logging_setup()
+
         # local database of SQLite or PostgreSQL
         if not store_path:
             # use the default local database in config.py
             local_database_path = self.config["session"]["local_database_path"]
             if "://" in local_database_path:
                 store_path = local_database_path
             else:
@@ -305,18 +311,18 @@
             )
         return ast
 
     def get_variable_names(self):
         """Get the list of Kestrel variable names created in this session."""
         return list(self.symtable.keys())
 
-    def get_variable(self, var_name):
+    def get_variable(self, var_name, deref=True):
         """Get the data of Kestrel variable ``var_name``, which is list of homogeneous entities (STIX SCOs)."""
         # In the future, consider returning a generator here?
-        return self.symtable[var_name].get_entities()
+        return self.symtable[var_name].get_entities(deref)
 
     def create_variable(self, var_name, objects, object_type=None):
         """Create a new Kestrel variable ``var_name`` with data in ``objects``.
 
         This is the API equivalent to Kestrel command ``NEW``, while allowing more
         flexible objects types (Python objects) than the objects serialized
         into text/JSON in the command ``NEW``.
@@ -358,22 +364,34 @@
         )
 
     def close(self):
         """Explicitly close the session.
 
         This may be executed by a context manager or when the program exits.
         """
-        # this subroutine could be invoked twice by a context manager and program exit.
-        # only execute it once (when self.store not deleted).
-        if hasattr(self, "store"):
+        # Note there are two conditions that trigger this function, so it is probably executed twice
+        # Be careful to write the logic in this function to avoid deleting nonexist files/dirs
+
+        # remove logging handler
+        if self.logging_handler:
+            logging.getLogger().removeHandler(self.logging_handler)
+            self.logging_handler.close()
+            # ensure this does not executed twice
+            self.logging_handler = None
+
+        # close store/database
+        if self.store:
             # release resources
             self.store.close()
-            del self.store
+            # ensure this does not executed twice
+            self.store = None
 
-            # manage temp folder for debug
+        # manage temp folder for debug
+        # ensure this does not execute if already executed
+        if os.path.exists(self.runtime_directory):
             if not self.runtime_directory_is_owned_by_upper_layer:
                 if self.debug_mode:
                     self._leave_exit_marker()
                     self._remove_obsolete_debug_folders()
                 else:
                     shutil.rmtree(self.runtime_directory)
 
@@ -434,19 +452,17 @@
         return displays
 
     def _update_symbol_table(self, output_var_name, output_var_struct):
         self.symtable[output_var_name] = output_var_struct
         self.symtable[self.config["language"]["default_variable"]] = output_var_struct
 
     def _leave_exit_marker(self):
-        exit_marker = os.path.join(
-            self.runtime_directory, self.config["debug"]["session_exit_marker"]
-        )
-        with open(exit_marker, "w"):
-            pass
+        runtime_dir = pathlib.Path(self.runtime_directory)
+        exit_marker = runtime_dir / self.config["debug"]["session_exit_marker"]
+        exit_marker.touch()
 
     def _remove_obsolete_debug_folders(self):
         # will only clean debug cache directories under system temp directory
 
         # [(cache_dir, timestamp)]
         exited_sessions = []
 
@@ -491,7 +507,13 @@
             master_dir.unlink()
         except FileNotFoundError:
             pass
         except PermissionError:
             raise DebugCacheLinkOccupied(master_dir.resolve())
 
         master_dir.symlink_to(self.runtime_directory)
+
+    def _logging_setup(self):
+        log_file_name = self.config["session"]["log_path"]
+        log_file_path = os.path.join(self.runtime_directory, log_file_name)
+        handler = logging.FileHandler(log_file_path)
+        self.logging_handler = add_logging_handler(handler, self.debug_mode)
```

### Comparing `kestrel-lang-1.5.9/src/kestrel/symboltable/variable.py` & `kestrel-lang-1.6.0/src/kestrel/symboltable/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from firepit.query import Query
+
 from kestrel.codegen.data import dump_data_to_file
 from kestrel.codegen.summary import get_variable_entity_count
 from kestrel.syntax.utils import get_all_input_var_names
 
 
 class VarStruct:
     # variable data structure in symbol table
@@ -49,16 +51,20 @@
         self.dependent_variables = dep_vars
 
         # statement that generates the variable
         self.birth_statement = statement
 
         self.data_source = data_source
 
-    def get_entities(self):
-        return self.store.lookup(self.entity_table) if self.entity_table else []
+    def get_entities(self, deref=True):
+        if not self.entity_table:
+            return []
+        if deref:
+            return self.store.lookup(self.entity_table)
+        return self.store.run_query(Query(self.entity_table)).fetchall()
 
     def dump_to_file(self, file_path):
         dump_data_to_file(self.store, self.entity_table, file_path)
 
     def __len__(self):
         return self.length
```

### Comparing `kestrel-lang-1.5.9/src/kestrel/syntax/ecgpattern.py` & `kestrel-lang-1.6.0/src/kestrel/syntax/ecgpattern.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/syntax/kestrel.lark` & `kestrel-lang-1.6.0/src/kestrel/syntax/kestrel.lark`

 * *Files 5% similar despite different names*

```diff
@@ -246,21 +246,27 @@
 //
 // Common language constructs
 //
 
 value: literal_list
      | literal
 
-literal: SIMPLESTRING
-       | ESCAPED_STRING
-       | NUMBER
+literal: reference_or_simple_string
+       | string
+       | number
 
 literal_list: "(" literal ("," literal)* ")"
             | "[" literal ("," literal)* "]"
 
+reference_or_simple_string: ECNAME ("." ATTRIBUTE)?
+
+string: ADVANCED_STRING
+
+number: NUMBER
+
 ENTITY_ATTRIBUTE_PATH: (ENTITY_TYPE ":")? ATTRIBUTE
 
 ENTITY_TYPE: ECNAME
 
 stdpath: PATH_SIMPLE
        | PATH_ESCAPED
 
@@ -268,24 +274,27 @@
 //       x.hash.SHA-256 instead of x.hash.'SHA-256'
 ATTRIBUTE: ECNAME "[*]"? ("." ECNAME_W_QUOTE)*
 ATTRIBUTES: ATTRIBUTE (WS* "," WS* ATTRIBUTE)*
 
 ECNAME: (LETTER|"_") (LETTER|DIGIT|"_"|"-")*
 ECNAME_W_QUOTE: (LETTER|DIGIT|"_"|"-"|"'")+
 
-SIMPLESTRING: (LETTER|"_") (LETTER|DIGIT|"_"|"-"|"."|"'"|"[*]")*
-
 PATH_SIMPLE: (ECNAME "://")? (LETTER|DIGIT|"_"|"-"|"."|"/")+
 
 PATH_ESCAPED: "\"" (ECNAME "://")? _STRING_ESC_INNER "\""
             | "'"  (ECNAME "://")? _STRING_ESC_INNER "'"
 
 ESCAPED_STRING: "\"" _STRING_ESC_INNER "\""
               | "'"  _STRING_ESC_INNER "'"
 ESCAPED_STRING_WS: WS* ESCAPED_STRING WS*
 
+SIMPLE_STRING: ECNAME
+
+// nearly Python string, but no [ubf]? as prefix options
+// check Lark example of Python parser for reference
+ADVANCED_STRING: /(r?)("(?!"").*?(?<!\\)(\\\\)*?"|'(?!'').*?(?<!\\)(\\\\)*?')/
 
 %import common (LETTER, DIGIT, WS, INT, WORD, NUMBER, _STRING_ESC_INNER)
 %import common.SH_COMMENT -> COMMENT
 
 %ignore WS
 %ignore COMMENT
```

### Comparing `kestrel-lang-1.5.9/src/kestrel/syntax/parser.py` & `kestrel-lang-1.6.0/src/kestrel/syntax/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,30 +42,14 @@
         import_paths=paths,
         transformer=merge_transformers(
             _ECGPatternT(), kestrel=_KestrelT(token_prefix="kestrel__")
         ),
     ).parse(pattern_str)
 
 
-def parse_reference(value_str) -> Reference:
-    grammar = get_data(__name__, "reference.lark").decode("utf-8")
-    paths = importlib.util.find_spec("kestrel.syntax").submodule_search_locations
-    parser = Lark(grammar, parser="lalr", import_paths=paths)
-
-    try:
-        ast = parser.parse(value_str)
-    except:
-        return None
-
-    variable = ast.children[0].value
-    attribute = ast.children[1].value
-
-    return Reference(variable, attribute)
-
-
 class _ECGPatternT(Transformer):
     def start(self, args):
         return ExtCenteredGraphPattern(args[0])
 
 
 class _KestrelT(Transformer):
     def __init__(
@@ -264,28 +248,40 @@
     def literal_list(self, args):
         if len(args) == 1:
             return args[0]
         else:
             return args
 
     def literal(self, args):
-        if args[0].type == self.token_prefix + "NUMBER":
-            try:
-                v = int(args[0].value)
-            except:
-                v = float(args[0].value)
-        elif args[0].type == self.token_prefix + "ESCAPED_STRING":
-            v = unescape_quoted_string(args[0].value)
+        return args[0]
+
+    def reference_or_simple_string(self, args):
+        if len(args) > 1:
+            variable = _first(args)
+            attribute = _second(args)
+            v = Reference(variable, attribute)
         else:
-            v = args[0].value
-            ref = parse_reference(v)
-            if ref:
-                v = ref
+            v = _first(args)
         return v
 
+    def string(self, args):
+        raw = _first(args)
+        if args[0].type == self.token_prefix + "SIMPLE_STRING":
+            value = raw
+        elif args[0].type == self.token_prefix + "ADVANCED_STRING":
+            value = unescape_quoted_string(raw)
+        return value
+
+    def number(self, args):
+        v = _first(args)
+        try:
+            return int(v)
+        except:
+            return float(v)
+
     def attr_clause(self, args):
         paths = self._assert_and_extract_single("ATTRIBUTES", args)
         return {
             "attrs": paths if paths else "*",
         }
 
     def sort_clause(self, args):
```

### Comparing `kestrel-lang-1.5.9/src/kestrel/syntax/reference.py` & `kestrel-lang-1.6.0/src/kestrel/syntax/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/syntax/utils.py` & `kestrel-lang-1.6.0/src/kestrel/syntax/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel/utils.py` & `kestrel-lang-1.6.0/src/kestrel/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import pathlib
 import os
 import uuid
 import collections.abc
+import logging
 
 
 def unescape_quoted_string(s):
-    return s[1:-1].encode("utf-8").decode("unicode_escape")
+    if s.startswith("r"):
+        return s[2:-1]
+    else:
+        return s[1:-1].encode("utf-8").decode("unicode_escape")
 
 
 def lowered_str_list(xs):
     return [x.lower() for x in xs if isinstance(x, str)]
 
 
 def update_nested_dict(dict_old, dict_new):
@@ -56,14 +60,35 @@
     while not ps or pathlib.Path(ps).exists():
         ps = str(uuid.uuid4())
     p = pathlib.Path(ps)
     p.mkdir(parents=True, exist_ok=True)
     return p
 
 
+def add_logging_handler(handler, if_debug):
+    fmt = "%(asctime)s %(levelname)s %(name)s %(message)s"
+    datefmt = "%H:%M:%S"
+    formatter = logging.Formatter(fmt=fmt, datefmt=datefmt)
+
+    handler.setFormatter(formatter)
+
+    root_logger = logging.getLogger()
+    root_logger.addHandler(handler)
+    root_logger.setLevel(logging.DEBUG if if_debug else logging.INFO)
+
+    return handler
+
+
+def clear_logging_handlers():
+    root_logger = logging.getLogger()
+    for h in root_logger.handlers[:]:
+        root_logger.removeHandler(h)
+        h.close()
+
+
 def resolve_path_in_kestrel_env_var():
     for key in os.environ:
         if key.startswith("KESTREL") or key.startswith("kestrel"):
             path = os.environ[key]
             if os.path.exists(path):
                 os.environ[key] = resolve_path(path)
```

### Comparing `kestrel-lang-1.5.9/src/kestrel_analytics_docker/config.py` & `kestrel-lang-1.6.0/src/kestrel_analytics_docker/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel_analytics_docker/interface.py` & `kestrel-lang-1.6.0/src/kestrel_analytics_docker/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel_analytics_python/config.py` & `kestrel-lang-1.6.0/src/kestrel_analytics_python/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel_analytics_python/interface.py` & `kestrel-lang-1.6.0/src/kestrel_analytics_python/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/src/kestrel_datasource_stixbundle/interface.py` & `kestrel-lang-1.6.0/src/kestrel_datasource_stixbundle/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     @staticmethod
     def list_data_sources(config=None):
         """This interface does not list data sources."""
         return []
 
     @staticmethod
-    def query(uri, pattern, session_id=None, config=None):
+    def query(uri, pattern, session_id=None, config=None, store=None):
         """Query a STIX bundle locally or remotely."""
 
         _logger.debug(f"query URI received at interface_stixbundle: {uri}")
 
         scheme, _, data_paths = uri.rpartition("://")
         data_paths = data_paths.split(",")
         pattern = fixup_pattern(pattern)
```

### Comparing `kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/connector.py` & `kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import sys
 import importlib
 import subprocess
 import requests
-import pkg_resources
+from importlib.metadata import version
 from lxml import html
 
 from kestrel.exceptions import DataSourceError
 
 
 _logger = logging.getLogger(__name__)
 
@@ -17,26 +17,27 @@
 STIX_SHIFTER_HOMEPAGE = "https://github.com/opencybersecurityalliance/stix-shifter"
 
 
 def get_package_name(connector_name):
     return "stix-shifter-modules-" + connector_name.replace("_", "-")
 
 
-def verify_package_origin(connector_name):
+def verify_package_origin(connector_name, stixshifter_version):
     _logger.debug("go to PyPI to verify package genuineness from STIX-shifter project")
     package_name = get_package_name(connector_name)
 
     try:
         pypi_response = requests.get(f"https://pypi.org/project/{package_name}")
         pypi_etree = html.fromstring(pypi_response.content)
     except:
         raise DataSourceError(
             f'STIX-shifter connector for "{connector_name}" is not installed '
             f'and Kestrel guessed Python package name "{package_name}" but failed to locate it at PyPI',
-            "please manually install the correct STIX-shifter connector Python package.",
+            "please verify the connector name and manually install the connector package using "
+            f"`pip install {package_name}=={stixshifter_version}`",
         )
 
     try:
         p_homepage = pypi_etree.xpath(XPATH_PYPI_PKG_HOME)[0]
         p_source = pypi_etree.xpath(XPATH_PYPI_PKG_SOURCE)[0]
     except:
         raise DataSourceError(
@@ -57,17 +58,17 @@
     _logger.info(f'"{package_name}" verified as a STIX-shifter package.')
 
 
 def install_package(connector_name):
     package_name = get_package_name(connector_name)
     _logger.debug(f"guess the connector package name: {package_name}")
 
-    verify_package_origin(connector_name)
+    stixshifter_version = version("stix_shifter")
 
-    stixshifter_version = pkg_resources.get_distribution("stix_shifter").version
+    verify_package_origin(connector_name, stixshifter_version)
 
     package_w_ver = package_name + "==" + stixshifter_version
 
     _logger.info(f'install Python package "{package_w_ver}".')
     try:
         subprocess.check_call([sys.executable, "-m", "pip", "install", package_w_ver])
     except:
@@ -77,27 +78,28 @@
         importlib.import_module(
             "stix_shifter_modules." + connector_name + ".entry_point"
         )
     except:
         raise DataSourceError(
             f'STIX-shifter connector for "{connector_name}" is not installed '
             f'and Kestrel failed to install the possible Python package "{package_name}"',
-            "please manually install the corresponding STIX-shifter connector Python package.",
+            "please manually install the corresponding STIX-shifter connector Python package using "
+            f"`pip install {package_name}=={stixshifter_version}`",
         )
 
 
 def ensure_version_consistency(connector_name):
     """Check if the installed connector package has the same version as
     stix-shifter If the version is different, uninstall connector
     package and the install the same version as stix-shifter
 
     """
-    stixshifter_version = pkg_resources.get_distribution("stix_shifter").version
+    stixshifter_version = version("stix_shifter")
     package_name = get_package_name(connector_name)
-    package_version = pkg_resources.get_distribution(package_name).version
+    package_version = version(package_name)
     if package_version == stixshifter_version:
         return
     package_w_ver = package_name + "==" + package_version
     _logger.info(
         f"{package_name} version {package_version} is different "
         f"from stix-shifter version {stixshifter_version}."
     )
```

### Comparing `kestrel-lang-1.5.9/src/kestrel_lang.egg-info/PKG-INFO` & `kestrel-lang-1.6.0/src/kestrel_lang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.5.9
+Version: 1.6.0
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
 .. image:: https://github.com/opencybersecurityalliance/kestrel-lang/raw/develop/logo/logo_w_text.svg
    :width: 432
    :alt: Kestrel Threat Hunting Language
```

### Comparing `kestrel-lang-1.5.9/src/kestrel_lang.egg-info/SOURCES.txt` & `kestrel-lang-1.6.0/src/kestrel_lang.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 src/kestrel/symboltable/symtable.py
 src/kestrel/symboltable/variable.py
 src/kestrel/syntax/__init__.py
 src/kestrel/syntax/ecgpattern.lark
 src/kestrel/syntax/ecgpattern.py
 src/kestrel/syntax/kestrel.lark
 src/kestrel/syntax/parser.py
-src/kestrel/syntax/reference.lark
 src/kestrel/syntax/reference.py
 src/kestrel/syntax/utils.py
 src/kestrel_analytics_docker/__init__.py
 src/kestrel_analytics_docker/config.py
 src/kestrel_analytics_docker/interface.py
 src/kestrel_analytics_python/__init__.py
 src/kestrel_analytics_python/config.py
@@ -71,12 +70,13 @@
 tests/test_command_merge.py
 tests/test_command_new.py
 tests/test_command_save.py
 tests/test_completion.py
 tests/test_display.py
 tests/test_exceptions.py
 tests/test_expressions.py
+tests/test_fast_translate.py
 tests/test_parser.py
 tests/test_python_analytics.py
 tests/test_session.py
 tests/test_stixshifter.py
 tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.5.9/tests/test_command_assign.py` & `kestrel-lang-1.6.0/tests/test_command_assign.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 
 
 # The * 2 on these counts is due to our inability to dedup process objects
 # Need unique IDs on process objects
 @pytest.mark.parametrize(
     "stmt, expected",
     [
-        ("x = p", 1000 * 2),
-        ("x = p WHERE pid = 1380", 106 * 2),
-        ("x = p WHERE command_line IS NULL", 948 * 2),
-        ("x = p WHERE command_line IS NOT NULL", 52 * 2),
-        ("x = p WHERE command_line LIKE '%/node%'", 1 * 2),
-        ("x = p WHERE pid = 5960 OR name = 'taskeng.exe'", 2 * 2),
+        ("x = p", 1000),
+        ("x = p WHERE pid = 1380", 106),
+        ("x = p WHERE command_line IS NULL", 948),
+        ("x = p WHERE command_line IS NOT NULL", 52),
+        ("x = p WHERE command_line LIKE '%/node%'", 1),
+        ("x = p WHERE pid = 5960 OR name = 'taskeng.exe'", 2),
         ("x = p WHERE (pid = 5960 OR name = 'taskeng.exe') AND command_line IS NULL", 0),
     ],
 )
 def test_assign_after_get(proc_bundle_file, stmt, expected):
     with Session() as s:
         s.execute(f"""
                    p = GET process
@@ -71,17 +71,21 @@
 
 def test_assign_with_reference(proc_bundle_file):
     with Session() as s:
         s.execute(f"p = GET process FROM file://{proc_bundle_file} WHERE [process:pid > 0]")
         s.execute(REF_PROCS)
         s.execute("q = p WHERE pid = ref.pid")
         q = s.get_variable("q")
-        assert len(q) == (106 + 149) * 2
+        assert len(q) == 106 + 149
 
 
 def test_assign_with_reference_and_in(proc_bundle_file):
     with Session() as s:
         s.execute(f"p = GET process FROM file://{proc_bundle_file} WHERE [process:pid > 0]")
+        p = s.get_variable("p", False)
+        assert 'binary_ref' in p[0]
         s.execute(REF_PROCS)
         s.execute("q = p WHERE pid IN (ref.pid, 9240, 10020)")
-        q = s.get_variable("q")
-        assert len(q) == (106 + 149 + 1 + 1) * 2
+        q = s.get_variable("q", False)
+        assert len(q) == 106 + 149 + 1 + 1
+        print(q[0])
+        assert 'binary_ref' in q[0]
```

### Comparing `kestrel-lang-1.5.9/tests/test_command_disp.py` & `kestrel-lang-1.6.0/tests/test_command_disp.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_command_find.py` & `kestrel-lang-1.6.0/tests/test_command_find.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_command_get.py` & `kestrel-lang-1.6.0/tests/test_command_get.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,16 +152,16 @@
                 b = GET process
                     WHERE name = 'svchost.exe'
                 """
 
         output = s.execute(stmt)
         a = s.get_variable("a")
         b = s.get_variable("b")
-        assert len(a) == 28
-        assert len(b) == 1408
+        assert len(a) == 14 * 2  # prefetch will get the same process twice
+        assert len(b) == 704 * 2  # prefetch will get the same process twice
 
 
 def test_relative_file_path(tmp_path):
     data_file_path = "doctored-1k.json"
     ori_path = os.path.join(
         os.path.dirname(__file__), data_file_path
     )
@@ -176,16 +176,16 @@
                 b = GET process
                     FROM file://./{data_file_path}
                     WHERE name = 'svchost.exe'
                 """
         output = s.execute(stmt)
         a = s.get_variable("a")
         b = s.get_variable("b")
-        assert len(a) == 28
-        assert len(b) == 1408
+        assert len(a) == 14 * 2  # prefetch will get the same process twice
+        assert len(b) == 704 * 2  # prefetch will get the same process twice
 
 
 def test_get_wrong_type(file_stix_bundles):
     with Session() as s:
         stmt = f"""
                 var = GET foo
                       FROM file://{file_stix_bundles[0]}
```

### Comparing `kestrel-lang-1.5.9/tests/test_command_group.py` & `kestrel-lang-1.6.0/tests/test_command_group.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_command_join.py` & `kestrel-lang-1.6.0/tests/test_command_join.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_command_load.py` & `kestrel-lang-1.6.0/tests/test_command_load.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_command_merge.py` & `kestrel-lang-1.6.0/tests/test_command_merge.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_command_new.py` & `kestrel-lang-1.6.0/tests/test_command_new.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_command_save.py` & `kestrel-lang-1.6.0/tests/test_command_save.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_completion.py` & `kestrel-lang-1.6.0/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_display.py` & `kestrel-lang-1.6.0/tests/test_display.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,18 @@
         stmt = """
 newvar = NEW [ {"type": "process", "name": "cmd.exe", "pid": "123"}
              , {"type": "process", "name": "explorer.exe", "pid": "99"}
              ]
 """
         d = s.execute(stmt)
     correct_json = json.loads(
-        '{"display": "execution summary", "data": {"execution time": 1, "variables updated": [{"VARIABLE": "newvar", "TYPE": "process", "#(ENTITIES)": 2, "#(RECORDS)": 2, "process*": 0}], "footnotes": ["*Number of related records cached."]}}'
+        '{"display": "execution summary", "data": {"variables updated": [{"VARIABLE": "newvar", "TYPE": "process", "#(ENTITIES)": 2, "#(RECORDS)": 2, "process*": 0}], "footnotes": ["*Number of related records cached."]}}'
     )
     output_json = json.loads(d[0].to_json())
+    del output_json["data"]["execution time"]
     assert output_json == correct_json
 
 
 def test_display_block_summary_to_dict():
     with Session() as s:
         stmt = """
 newvar = NEW [ {"type": "process", "name": "cmd.exe", "pid": "123"}
```

### Comparing `kestrel-lang-1.5.9/tests/test_exceptions.py` & `kestrel-lang-1.6.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_expressions.py` & `kestrel-lang-1.6.0/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_parser.py` & `kestrel-lang-1.6.0/tests/test_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,24 @@
         ),
         (
             r"command_line = 'C:\\abc\\xyz.exe /c asdf'",
             r"process",
             r"[process:command_line = 'C:\\abc\\xyz.exe /c asdf']",
         ),
         (
+            r"command_line = r'C:\abc\xyz.exe /c asdf'",
+            r"process",
+            r"[process:command_line = 'C:\\abc\\xyz.exe /c asdf']",
+        ),
+        (
+            r'command_line = r"C:\wbc\nyz.exe /c asdf"',
+            r"process",
+            r"[process:command_line = 'C:\\wbc\\nyz.exe /c asdf']",
+        ),
+        (
             "name LIKE 'power%.exe'",
             "process",
             "[process:name LIKE 'power%.exe']",
         ),
         (
             r"name MATCHES 'power.+\\d{1,3}[a-zA-Z0-9]+\\.exe'",
             r"process",
@@ -114,17 +124,22 @@
         ),
         (
             r"name MATCHES 'power\\(hi\\)\\w+(real)\\.exe'",
             r"process",
             r"[process:name MATCHES 'power\\(hi\\)\\w+(real)\\.exe']",
         ),
         (
-            r"name MATCHES 'C:\\Windows\\system32\\svchost\\.exe'",
+            r"name MATCHES 'C:\\\\Windows\\\\system32\\\\svchost\\.exe'",
+            r"process",
+            r"[process:name MATCHES 'C:\\\\Windows\\\\system32\\\\svchost\\.exe']",
+        ),
+        (
+            r"name MATCHES r'C:\\Windows\\system32\\svchost\.exe'",
             r"process",
-            r"[process:name MATCHES 'C:\\Windows\\system32\\svchost\\.exe']",
+            r"[process:name MATCHES 'C:\\\\Windows\\\\system32\\\\svchost\\.exe']",
         ),
     ],
 )
 def test_ecgp(ecgp, center_entity, stix):
     # test ECGP in GET
     stmt = f"x = GET {center_entity} FROM xxx WHERE {ecgp}"
     cmd = parse_kestrel(stmt)[0]
```

### Comparing `kestrel-lang-1.5.9/tests/test_python_analytics.py` & `kestrel-lang-1.6.0/tests/test_python_analytics.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.9/tests/test_session.py` & `kestrel-lang-1.6.0/tests/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         assert (
             val["user_id"] in names
         )  # Order is not preserved, so it could be any of these
 
 
 def test_session_runtime_dir():
     # standard session
-    with Session() as session:
+    with Session(debug_mode=False) as session:
         runtime_directory = session.runtime_directory
         runtime_master_dirctory = session._get_runtime_directory_master()
 
         assert os.path.exists(session.runtime_directory)
 
         # if not executed in a clean env; it has previous debug dirs
         if runtime_master_dirctory.exists():
```

### Comparing `kestrel-lang-1.5.9/tests/test_stixshifter.py` & `kestrel-lang-1.6.0/tests/test_stixshifter.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from kestrel.session import Session
 
 from kestrel_datasource_stixshifter.connector import (
     verify_package_origin,
     check_module_availability,
 )
 
+from kestrel_datasource_stixshifter.config import get_datasource_from_profiles
+
 
 def test_verify_package_origin():
     connectors = ["stix_bundle", "qradar", "elastic_ecs", "splunk"]
     for connector_name in connectors:
-        verify_package_origin(connector_name)
+        verify_package_origin(connector_name, "test_version")
 
 
 def test_check_module_availability():
     connectors = ["stix_bundle"]
     for connector_name in connectors:
         check_module_availability(connector_name)
 
@@ -41,14 +43,18 @@
 profiles:
     host101:
         connector: elastic_ecs
         connection:
             host: elastic.securitylog.company.com
             port: 9200
             indices: host101
+            options:
+                retrieval_batch_size: 10000
+                dialects:
+                    - beats
         config:
             auth:
                 id: profileB
                 api_key: asdf
 """
 
     profile_file = tmp_path / "stixshifter.yaml"
@@ -67,21 +73,25 @@
 """
         s.execute(stmt)
 
         s.data_source_manager.list_data_sources_from_scheme("stixshifter")
 
         ss_config = s.config["datasources"]["kestrel_datasource_stixshifter"]
         ss_profiles = ss_config["profiles"]
-        ss_host101_auth = ss_profiles["host101"]["config"]["auth"]
-        assert ss_host101_auth["id"] == "profileA"
-        assert ss_host101_auth["api_key"] == "qwer"
+        connector_name, connection, configuration, retrieval_batch_size = get_datasource_from_profiles("host101", ss_profiles)
+        assert connector_name == "elastic_ecs"
+        assert configuration["auth"]["id"] == "profileA"
+        assert configuration["auth"]["api_key"] == "qwer"
+        assert retrieval_batch_size == 2000
 
         with open(profile_file, "w") as pf:
             pf.write(profileB)
 
         s.data_source_manager.list_data_sources_from_scheme("stixshifter")
 
         # need to refresh the pointers since the dict is updated
         ss_profiles = ss_config["profiles"]
-        ss_host101_auth = ss_profiles["host101"]["config"]["auth"]
-        assert ss_host101_auth["id"] == "profileB"
-        assert ss_host101_auth["api_key"] == "asdf"
+        connector_name, connection, configuration, retrieval_batch_size = get_datasource_from_profiles("host101", ss_profiles)
+        assert connector_name == "elastic_ecs"
+        assert configuration["auth"]["id"] == "profileB"
+        assert configuration["auth"]["api_key"] == "asdf"
+        assert retrieval_batch_size == 10000
```

### Comparing `kestrel-lang-1.5.9/tests/test_timestamped.py` & `kestrel-lang-1.6.0/tests/test_timestamped.py`

 * *Files identical despite different names*

