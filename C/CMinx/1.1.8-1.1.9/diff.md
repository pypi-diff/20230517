# Comparing `tmp/CMinx-1.1.8.tar.gz` & `tmp/CMinx-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMinx-1.1.8.tar", last modified: Mon Apr 10 15:51:01 2023, max compression
+gzip compressed data, was "CMinx-1.1.9.tar", last modified: Wed May 17 20:00:31 2023, max compression
```

## Comparing `CMinx-1.1.8.tar` & `CMinx-1.1.9.tar`

### file list

```diff
@@ -1,157 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.351490 CMinx-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 15:50:52.000000 CMinx-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-10 15:50:52.000000 CMinx-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-04-10 15:51:01.351490 CMinx-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-10 15:50:52.000000 CMinx-1.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.335490 CMinx-1.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.335490 CMinx-1.1.8/docs/source/.templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/docs/source/.templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/.templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/docs/source/developer/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/ci.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/repo_structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/docs/source/developer/uml_diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/uml_diagrams/aggregation.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    86638 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/uml_diagrams/aggregation.png
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/uml_diagrams/parsing.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    84711 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/uml_diagrams/parsing.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/docs/source/documenting/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/cmaketest.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/ctest_add_test.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/macro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/types_of_comments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/variable.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/full_example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-10 15:50:52.000000 CMinx-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:51:01.351490 CMinx-1.1.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-04-10 15:50:52.000000 CMinx-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/src/CMinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/src/cminx/
--rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24540 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/documentation_types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4160 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/documenter.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/src/cminx/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMake.g4
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMake.interp
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMake.tokens
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeLexer.interp
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeListener.py
--rw-r--r--   0 runner    (1001) docker     (123)    20386 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeVisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20831 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/rstwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/cmake/gen_rst.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/cmake_input/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/cmake_input/example.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1780 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/aggregator_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/examples/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/configs/exclude_filters_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/configs/exclude_input_file_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/configs/no_auto_exclude_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/configs/no_include_undocumented_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/example.cmake
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/example_2.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/examples/more_cmake_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/more_cmake_files/empty.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1518 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/rst_validator_example.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/rstwriter_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.335490 CMinx-1.1.8/tests/examples/sphinx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/examples/sphinx/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/example_no_undocumented.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/example_no_undocumented_diff_header.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/example_prefix.rst
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/index_exclusion_filters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/index_no_auto_exclude.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.347490 CMinx-1.1.8/tests/test_samples/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/add_test_and_func_after.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/advanced_function.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/advanced_macro.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/advanced_module.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/basic_function.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/basic_macro.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/basic_module.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.347490 CMinx-1.1.8/tests/test_samples/corr_rst/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/add_test_and_func_after.rst
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/advanced_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/advanced_macro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/advanced_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/basic_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/basic_macro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/basic_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/ct_test.rst
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/ctest_add_test.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.347490 CMinx-1.1.8/tests/test_samples/corr_rst/index/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/index/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/index/index_prefix.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/option.rst
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/undocumented_commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/undocumented_option_no_default.rst
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/variable.rst
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/ct_test.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/ctest_add_test.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/option.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/quickstart.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/undocumented_commands.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/undocumented_option_no_default.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/variable.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.351490 CMinx-1.1.8/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13343 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/rst_validator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19868 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4782 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_documenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_error_listener.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6615 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4914 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_rstwriter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.366110 CMinx-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 20:00:22.000000 CMinx-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-17 20:00:22.000000 CMinx-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-05-17 20:00:31.366110 CMinx-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-17 20:00:22.000000 CMinx-1.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.350110 CMinx-1.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.354110 CMinx-1.1.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.350110 CMinx-1.1.9/docs/source/.templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.354110 CMinx-1.1.9/docs/source/.templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/.templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.354110 CMinx-1.1.9/docs/source/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/ci.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/repo_structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.354110 CMinx-1.1.9/docs/source/developer/uml_diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/uml_diagrams/aggregation.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    86638 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/uml_diagrams/aggregation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/uml_diagrams/parsing.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    84711 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/developer/uml_diagrams/parsing.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.354110 CMinx-1.1.9/docs/source/documenting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/documenting/cmaketest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/documenting/ctest_add_test.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/documenting/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/documenting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/documenting/macro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/documenting/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/documenting/types_of_comments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/documenting/variable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/full_example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-17 20:00:22.000000 CMinx-1.1.9/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-17 20:00:22.000000 CMinx-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:00:31.366110 CMinx-1.1.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-05-17 20:00:22.000000 CMinx-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.354110 CMinx-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.358110 CMinx-1.1.9/src/CMinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-05-17 20:00:31.000000 CMinx-1.1.9/src/CMinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-17 20:00:31.000000 CMinx-1.1.9/src/CMinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:00:31.000000 CMinx-1.1.9/src/CMinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-17 20:00:31.000000 CMinx-1.1.9/src/CMinx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-17 20:00:31.000000 CMinx-1.1.9/src/CMinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 20:00:31.000000 CMinx-1.1.9/src/CMinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.358110 CMinx-1.1.9/src/cminx/
+-rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27352 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/config_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/documentation_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5650 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/documenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.358110 CMinx-1.1.9/src/cminx/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/parser/CMake.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/parser/CMake.interp
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/parser/CMake.tokens
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/parser/CMakeLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/parser/CMakeLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/parser/CMakeLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/parser/CMakeListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/parser/CMakeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/parser/CMakeVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/parser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21960 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/cminx/rstwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-17 20:00:22.000000 CMinx-1.1.9/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.358110 CMinx-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.358110 CMinx-1.1.9/tests/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/cmake/gen_rst.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.358110 CMinx-1.1.9/tests/cmake_input/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/cmake_input/example.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.362110 CMinx-1.1.9/tests/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1780 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/aggregator_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.362110 CMinx-1.1.9/tests/examples/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/configs/exclude_filters_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/configs/exclude_input_file_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/configs/no_auto_exclude_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/configs/no_include_undocumented_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/example.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/example_2.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.362110 CMinx-1.1.9/tests/examples/more_cmake_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/more_cmake_files/empty.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1518 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/rst_validator_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/rstwriter_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.350110 CMinx-1.1.9/tests/examples/sphinx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.362110 CMinx-1.1.9/tests/examples/sphinx/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/sphinx/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/sphinx/source/example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/sphinx/source/example_no_undocumented.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/sphinx/source/example_no_undocumented_diff_header.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/sphinx/source/example_prefix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/sphinx/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/sphinx/source/index_exclusion_filters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/examples/sphinx/source/index_no_auto_exclude.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.362110 CMinx-1.1.9/tests/test_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/add_test_and_func_after.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/advanced_function.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/advanced_macro.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/advanced_module.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/basic_function.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/basic_macro.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/basic_module.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/commented_out_function.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.366110 CMinx-1.1.9/tests/test_samples/corr_rst/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/add_test_and_func_after.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/advanced_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/advanced_macro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/advanced_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/basic_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/basic_macro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/basic_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/commented_out_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/ct_test.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/ctest_add_test.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.366110 CMinx-1.1.9/tests/test_samples/corr_rst/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/index/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/index/index_prefix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/option.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/undocumented_commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/undocumented_option_no_default.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/corr_rst/variable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/ct_test.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/ctest_add_test.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/option.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/quickstart.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/undocumented_commands.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/undocumented_option_no_default.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/test_samples/variable.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:00:31.366110 CMinx-1.1.9/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/unit_tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13343 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/unit_tests/rst_validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24863 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/unit_tests/test_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/unit_tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4782 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/unit_tests/test_documenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/unit_tests/test_error_listener.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6615 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/unit_tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/unit_tests/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/unit_tests/test_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4914 2023-05-17 20:00:22.000000 CMinx-1.1.9/tests/unit_tests/test_rstwriter.py
```

### Comparing `CMinx-1.1.8/LICENSE` & `CMinx-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/PKG-INFO` & `CMinx-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CMinx
-Version: 1.1.8
+Version: 1.1.9
 Summary: Documentation Generator for the CMake Language
 Author: CMakePP
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -238,14 +238,15 @@
 
 .. image:: https://codecov.io/gh/CMakePP/CMinx/branch/master/graph/badge.svg?token=wbiPq8Gnrs
    :target: https://codecov.io/gh/CMakePP/CMinx
 
 .. image:: https://joss.theoj.org/papers/10.21105/joss.04680/status.svg
    :target: https://doi.org/10.21105/joss.04680
 
+
 Full documentation can be found `here <https://cmakepp.github.io/CMinx/>`__.
 
 *****************
 Statement of Need
 *****************
 
 CMake build systems can be extended by writing CMake modules. CMake modules
```

### Comparing `CMinx-1.1.8/README.rst` & `CMinx-1.1.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 .. image:: https://codecov.io/gh/CMakePP/CMinx/branch/master/graph/badge.svg?token=wbiPq8Gnrs
    :target: https://codecov.io/gh/CMakePP/CMinx
 
 .. image:: https://joss.theoj.org/papers/10.21105/joss.04680/status.svg
    :target: https://doi.org/10.21105/joss.04680
 
+
 Full documentation can be found `here <https://cmakepp.github.io/CMinx/>`__.
 
 *****************
 Statement of Need
 *****************
 
 CMake build systems can be extended by writing CMake modules. CMake modules
```

### Comparing `CMinx-1.1.8/docs/Makefile` & `CMinx-1.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/README.rst` & `CMinx-1.1.9/docs/README.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/about.rst` & `CMinx-1.1.9/docs/source/about.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/conf.py` & `CMinx-1.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/config.rst` & `CMinx-1.1.9/docs/source/config.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/developer/api.rst` & `CMinx-1.1.9/docs/source/developer/api.rst`

 * *Files 14% similar despite different names*

```diff
@@ -21,18 +21,20 @@
 
 Python Modules
 ^^^^^^^^^^^^^^
 
 .. autosummary::
    :toctree: .autosummary
 
-
-   cminx.rstwriter
-   cminx.documenter
    cminx.aggregator
+   cminx.config
+   cminx.documenter
+   cminx.documentation_types
+   cminx.exceptions
+   cminx.rstwriter
    cminx.parser.CMakeLexer
    cminx.parser.CMakeParser
    cminx.parser.CMakeListener
    cminx.parser.CMakeVisitor
 
 Functions
 ^^^^^^^^^
```

### Comparing `CMinx-1.1.8/docs/source/developer/ci.rst` & `CMinx-1.1.9/docs/source/developer/ci.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/developer/dependencies.rst` & `CMinx-1.1.9/docs/source/developer/dependencies.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/developer/documentation.rst` & `CMinx-1.1.9/docs/source/developer/documentation.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/developer/index.rst` & `CMinx-1.1.9/docs/source/developer/index.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/developer/overview.rst` & `CMinx-1.1.9/docs/source/developer/overview.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/developer/repo_structure.rst` & `CMinx-1.1.9/docs/source/developer/repo_structure.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/developer/uml_diagrams/aggregation.drawio` & `CMinx-1.1.9/docs/source/developer/uml_diagrams/aggregation.drawio`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/developer/uml_diagrams/aggregation.png` & `CMinx-1.1.9/docs/source/developer/uml_diagrams/aggregation.png`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/developer/uml_diagrams/parsing.drawio` & `CMinx-1.1.9/docs/source/developer/uml_diagrams/parsing.drawio`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/developer/uml_diagrams/parsing.png` & `CMinx-1.1.9/docs/source/developer/uml_diagrams/parsing.png`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/documenting/cmaketest.rst` & `CMinx-1.1.9/docs/source/documenting/cmaketest.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/documenting/ctest_add_test.rst` & `CMinx-1.1.9/docs/source/documenting/ctest_add_test.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/documenting/function.rst` & `CMinx-1.1.9/docs/source/documenting/function.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/documenting/index.rst` & `CMinx-1.1.9/docs/source/documenting/index.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/documenting/macro.rst` & `CMinx-1.1.9/docs/source/documenting/macro.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/documenting/module.rst` & `CMinx-1.1.9/docs/source/documenting/module.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/documenting/types_of_comments.rst` & `CMinx-1.1.9/docs/source/documenting/types_of_comments.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/documenting/variable.rst` & `CMinx-1.1.9/docs/source/documenting/variable.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/full_example.rst` & `CMinx-1.1.9/docs/source/full_example.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/index.rst` & `CMinx-1.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/installation.rst` & `CMinx-1.1.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/quickstart.rst` & `CMinx-1.1.9/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/docs/source/usage.rst` & `CMinx-1.1.9/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/pyproject.toml` & `CMinx-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/setup.py` & `CMinx-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/src/CMinx.egg-info/PKG-INFO` & `CMinx-1.1.9/src/CMinx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CMinx
-Version: 1.1.8
+Version: 1.1.9
 Summary: Documentation Generator for the CMake Language
 Author: CMakePP
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -238,14 +238,15 @@
 
 .. image:: https://codecov.io/gh/CMakePP/CMinx/branch/master/graph/badge.svg?token=wbiPq8Gnrs
    :target: https://codecov.io/gh/CMakePP/CMinx
 
 .. image:: https://joss.theoj.org/papers/10.21105/joss.04680/status.svg
    :target: https://doi.org/10.21105/joss.04680
 
+
 Full documentation can be found `here <https://cmakepp.github.io/CMinx/>`__.
 
 *****************
 Statement of Need
 *****************
 
 CMake build systems can be extended by writing CMake modules. CMake modules
```

### Comparing `CMinx-1.1.8/src/CMinx.egg-info/SOURCES.txt` & `CMinx-1.1.9/src/CMinx.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 tests/test_samples/add_test_and_func_after.cmake
 tests/test_samples/advanced_function.cmake
 tests/test_samples/advanced_macro.cmake
 tests/test_samples/advanced_module.cmake
 tests/test_samples/basic_function.cmake
 tests/test_samples/basic_macro.cmake
 tests/test_samples/basic_module.cmake
+tests/test_samples/commented_out_function.cmake
 tests/test_samples/ct_test.cmake
 tests/test_samples/ctest_add_test.cmake
 tests/test_samples/option.cmake
 tests/test_samples/quickstart.cmake
 tests/test_samples/test_samples.py
 tests/test_samples/undocumented_commands.cmake
 tests/test_samples/undocumented_option_no_default.cmake
@@ -105,14 +106,15 @@
 tests/test_samples/corr_rst/add_test_and_func_after.rst
 tests/test_samples/corr_rst/advanced_function.rst
 tests/test_samples/corr_rst/advanced_macro.rst
 tests/test_samples/corr_rst/advanced_module.rst
 tests/test_samples/corr_rst/basic_function.rst
 tests/test_samples/corr_rst/basic_macro.rst
 tests/test_samples/corr_rst/basic_module.rst
+tests/test_samples/corr_rst/commented_out_function.rst
 tests/test_samples/corr_rst/ct_test.rst
 tests/test_samples/corr_rst/ctest_add_test.rst
 tests/test_samples/corr_rst/index.rst
 tests/test_samples/corr_rst/option.rst
 tests/test_samples/corr_rst/quickstart.rst
 tests/test_samples/corr_rst/undocumented_commands.rst
 tests/test_samples/corr_rst/undocumented_option_no_default.rst
```

### Comparing `CMinx-1.1.8/src/cminx/__init__.py` & `CMinx-1.1.9/src/cminx/__init__.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/src/cminx/aggregator.py` & `CMinx-1.1.9/src/cminx/aggregator.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,87 +8,120 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""
+This module interfaces with the generated CMake parser.
+The primary entrypoint is :class:`~DocumentationAggregator`,
+which subclasses :class:`cminx.parser.CMakeListener`. This
+class listens to all relevent parser rules, generates
+:class:`cminx.documentation_types.DocumentationType`
+objects that represent the parsed CMake, and
+aggregates them in a single list.
+
+:Author: Branden Butler
+:License: Apache 2.0
+"""
+
 import logging
-from typing import List
+import re
+from dataclasses import dataclass
+from typing import List, Union
+
+from antlr4 import ParserRuleContext
 
 from .documentation_types import AttributeDocumentation, FunctionDocumentation, MacroDocumentation, \
     VariableDocumentation, GenericCommandDocumentation, ClassDocumentation, TestDocumentation, SectionDocumentation, \
     MethodDocumentation, VarType, CTestDocumentation, ModuleDocumentation, AbstractCommandDefinitionDocumentation, \
-    OptionDocumentation
+    OptionDocumentation, DanglingDoccomment, DocumentationType
+
 from .exceptions import CMakeSyntaxException
 from .parser.CMakeListener import CMakeListener
 # Annoyingly, the Antl4 Python libraries use camelcase since it was originally Java, so we have convention
 # inconsistencies here
 from .parser.CMakeParser import CMakeParser
 from cminx import Settings
 
-"""
-This module interfaces with the generated CMake parser.
-It also subclasses CMakeListener to aggregate and further
-process documented commands on-the-fly.
-
-Processed documentation is stored in two different types of named tuples
-depending on the type being documented. VariableDocumentation also stores
-what type the variable is, either String or List for most purposes but also
-supports Unset in case someone wants to document why something is unset.
 
-:Author: Branden Butler
-:License: Apache 2.0
-"""
+@dataclass
+class DefinitionCommand:
+    """
+    A container for documentation of definition commands, used to update
+    the parameter list when a :code:`cmake_parse_arguments()` command
+    is encountered.
+
+    A definition command is a command that defines another command,
+    so the function() and macro() commands are definition commands.
+    Instances of this dataclass are placed on the top of a stack
+    when definition commands are encountered.
+    """
+    documentation: Union[AbstractCommandDefinitionDocumentation, None]
+    """
+    The documentation for the definition command. If None,
+    this DefinitionCommand will be ignored when popped.
+    """
 
+    should_document: bool = True
+    """
+    Whether the contained documentation object should be updated
+    if a :code:`cmake_parse_arguments()` command is found.
+    When false, this object is ignored.
+    """
 
-class DefinitionCommand:
-    def __init__(self, documentation: AbstractCommandDefinitionDocumentation, should_document = True):
-        self.documentation = documentation
-        self.should_document = should_document
 
 class DocumentationAggregator(CMakeListener):
     """
     Processes all docstrings and their associated commands, aggregating
-    them in a list.
+    them in a list. Uses the given :class:`~cminx.config.Settings` object
+    to determine aggregation settings, and will document commands without
+    doccomments if the associated settings are set.
+
+    The method used to generate the documentation object for
+    a given command is chosen by searching for a method with the name
+    :code:`"process_<command name>"` with two arguments: :code:`ctx` that is
+    of type :class:`cminx.parser.CMakeParser.Command_invocationContext`,
+    and :code:`docstring` that is of type string.
     """
 
-    def __init__(self, settings: Settings = Settings()):
-        self.settings = settings
+    def __init__(self, settings: Settings = Settings()) -> None:
+        self.settings: Settings = settings
         """Application settings used to determine what commands to document"""
 
-        self.documented = []
+        self.documented: List[DocumentationType] = []
         """All current documented commands"""
 
-        self.documented_classes_stack = []
+        self.documented_classes_stack: List[Union[ClassDocumentation, None]] = []
         """A stack containing the documented classes and inner classes as they are processed"""
 
-        self.documented_awaiting_function_def = None
+        self.documented_awaiting_function_def: Union[DocumentationType, None] = None
         """
         A variable containing a documented command such as cpp_member() that is awaiting its function/macro
         definition
         """
 
-        self.definition_command_stack = []
+        self.definition_command_stack: List[DefinitionCommand] = []
         """
         A stack containing the current definition command that we are inside.
         A definition command is any command that defines a construct with both a
         beginning command and an ending command, with all commands within being considered
         part of the definition. Examples of definition commands include
         function(), macro(), and cpp_class().
         """
 
-        self.consumed = []
+        self.consumed: List[ParserRuleContext] = []
         """
         A list containing all of the contexts that have already been processed
         """
 
-        self.logger = logging.getLogger(__name__)
+        self.logger: logging.Logger = logging.getLogger(__name__)
 
-    def process_function(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_function(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Extracts function name and declared parameters.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
 
         :param docstring: Cleaned docstring.
         """
@@ -100,24 +133,26 @@
             pretty_text += f"\n{ctx.getText()}"
 
             raise CMakeSyntaxException(
                 f"function() called with incorrect parameters: {ctx.single_argument()}\n\n{pretty_text}",
                 ctx.start.line
             )
 
-        params = [p.getText() for p in def_params[1:]]
+        params = [
+            re.sub(self.settings.input.function_parameter_name_strip_regex, "", p.getText()) for p in def_params[1:]
+        ]
         function_name = def_params[0].getText()
         has_kwargs = self.settings.input.kwargs_doc_trigger_string in docstring
 
         # Extracts function name and adds the completed function documentation to the 'documented' list
         doc = FunctionDocumentation(function_name, docstring, params, has_kwargs)
         self.documented.append(doc)
         self.definition_command_stack.append(DefinitionCommand(doc))
 
-    def process_macro(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_macro(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Extracts macro name and declared parameters.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
 
         :param docstring: Cleaned docstring.
         """
@@ -129,37 +164,42 @@
             pretty_text += f"\n{ctx.getText()}"
 
             raise CMakeSyntaxException(
                 f"macro() called with incorrect parameters: {ctx.single_argument()}\n\n{pretty_text}",
                 ctx.start.line
             )
 
-        params = [p.getText() for p in def_params[1:]]
+        params = [
+            re.sub(self.settings.input.macro_parameter_name_strip_regex, "", p.getText()) for p in def_params[1:]
+        ]
         macro_name = def_params[0].getText()
         has_kwargs = self.settings.input.kwargs_doc_trigger_string in docstring
 
         # Extracts macro name and adds the completed macro documentation to the 'documented' list
         doc = MacroDocumentation(macro_name, docstring, params, has_kwargs)
         self.documented.append(doc)
         self.definition_command_stack.append(DefinitionCommand(doc))
 
-    def process_cmake_parse_arguments(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_cmake_parse_arguments(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Determines whether a documented function or macro uses *args or *kwargs.
+        Accesses the last element in the :code:`definition_command_stack` to
+        update the documentation's :code:`has_kwargs` field.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
 
         :param docstring: Cleaned docstring.
         """
         if len(self.definition_command_stack) > 0:
             last_element = self.definition_command_stack[-1]
-            if last_element.should_document and isinstance(last_element.documentation, AbstractCommandDefinitionDocumentation):
+            if last_element.should_document and isinstance(last_element.documentation,
+                                                           AbstractCommandDefinitionDocumentation):
                 last_element.documentation.has_kwargs = True
 
-    def process_ct_add_test(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_ct_add_test(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Extracts test name and declared parameters.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
 
         :param docstring: Cleaned docstring.
         """
@@ -191,15 +231,15 @@
             if param.upper() == "EXPECTFAIL":
                 expect_fail = True
 
         test_doc = TestDocumentation(name, docstring, expect_fail)
         self.documented.append(test_doc)
         self.documented_awaiting_function_def = test_doc
 
-    def process_ct_add_section(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_ct_add_section(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Extracts section name and declared parameters.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
 
         :param docstring: Cleaned docstring.
         """
@@ -230,15 +270,15 @@
             if param.upper() == "EXPECTFAIL":
                 expect_fail = True
 
         section_doc = SectionDocumentation(name, docstring, expect_fail)
         self.documented.append(section_doc)
         self.documented_awaiting_function_def = section_doc
 
-    def process_set(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_set(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Extracts variable name and values from the documented set command.
         Also determines the type of set command/variable: String, List, or Unset.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
 
         :param docstring: Cleaned docstring.
@@ -273,15 +313,15 @@
                 value = value[:-1]
             self.documented.append(VariableDocumentation(
                 varname, docstring, VarType.STRING, value))
         else:  # Unset
             self.documented.append(VariableDocumentation(
                 varname, docstring, VarType.UNSET, None))
 
-    def process_cpp_class(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_cpp_class(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Extracts the name and the declared superclasses from the documented
         cpp_class command.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
 
         :param docstring: Cleaned docstring.
@@ -308,15 +348,15 @@
             self.documented_classes_stack[-1].inner_classes.append(clazz)
 
         # Continue processing within the class's context
         # until we reach cpp_end_class()
         self.documented_classes_stack.append(clazz)
 
     def process_cpp_member(self, ctx: CMakeParser.Command_invocationContext, docstring: str,
-                           is_constructor: bool = False):
+                           is_constructor: bool = False) -> None:
         """
         Extracts the method name and declared parameter types from the documented cpp_member
         command.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
 
         :param docstring: Cleaned docstring.
@@ -355,21 +395,21 @@
             name, docstring, parent_class, param_types, [], is_constructor)
         if is_constructor:
             clazz.constructors.append(method_doc)
         else:
             clazz.members.append(method_doc)
         self.documented_awaiting_function_def = method_doc
 
-    def process_cpp_constructor(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_cpp_constructor(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Alias for calling process_cpp_member() with is_constructor=True.
         """
         self.process_cpp_member(ctx, docstring, is_constructor=True)
 
-    def process_cpp_attr(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_cpp_attr(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Extracts the name and any default values from the documented cpp_attr
         command.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
 
         :param docstring: Cleaned docstring.
@@ -398,15 +438,15 @@
             return
         parent_class = params[0]
         name = params[1]
         default_values = params[2] if len(params) > 2 else None
         clazz.attributes.append(AttributeDocumentation(
             name, docstring, parent_class, default_values))
 
-    def process_add_test(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_add_test(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Extracts information from a CTest add_test() command.
         Note: this is not the processor for the CMakeTest ct_add_test() command,
         but the processor for the vanilla CMake add_test() command.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
 
@@ -434,15 +474,15 @@
 
                     self.logger.error(f"add_test() called with incorrect parameters: {params}\n\n{pretty_text}")
                     return
 
         test_doc = CTestDocumentation(name, docstring, [p for p in params if p != name and p != "NAME"])
         self.documented.append(test_doc)
 
-    def process_option(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_option(self, ctx: CMakeParser.Command_invocationContext, docstring: str) -> None:
         """
         Extracts information from an :code:`option()` command and creates
         an OptionDocumentation from it. It extracts the option name,
         the help text, and the default value if any.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
         :param docstring: Cleaned docstring.
@@ -460,15 +500,16 @@
             docstring,
             "bool",
             params[2] if len(params) == 3 else None,
             params[1]
         )
         self.documented.append(option_doc)
 
-    def process_generic_command(self, command_name: str, ctx: CMakeParser.Command_invocationContext, docstring: str):
+    def process_generic_command(self, command_name: str, ctx: CMakeParser.Command_invocationContext,
+                                docstring: str) -> None:
         """
         Extracts command invocation and arguments for a documented command that does not
         have a dedicated processor function.
 
         :param command_name: The documented command's name, such as add_library.
 
         :param ctx: Documented command context. Constructed by the Antlr4 parser.
@@ -505,24 +546,25 @@
         cleaned_lines[-1] = cleaned_lines[-1].rstrip("#]")
         cleaned_doc = "\n".join(cleaned_lines)
         if cleaned_doc.startswith("\n"):
             cleaned_doc = cleaned_doc[1:]
 
         return cleaned_doc
 
-    def enterDocumented_command(self, ctx: CMakeParser.Documented_commandContext):
+    def enterDocumented_command(self, ctx: CMakeParser.Documented_commandContext) -> None:
         """
         Main entrypoint into the documentation processor and aggregator. Called by ParseTreeWalker whenever
         encountering a documented command. Cleans the docstring and dispatches ctx to other functions for additional
         processing (process_{command}(), i.e. process_function())
 
         :param ctx: Documented command context, constructed by the Antlr4 parser.
 
         :raise NotImplementedError: If no processor can be found for the command that was documented.
         """
+        self.consumed.append(ctx.bracket_doccomment())
         text = ctx.bracket_doccomment().getText()
         lines = text.split("\n")
 
         cleaned_doc = DocumentationAggregator.clean_doc_lines(lines)
 
         try:
             command = ctx.command_invocation().Identifier().getText().lower()
@@ -531,18 +573,19 @@
             if f"process_{command}" in dir(self):
                 getattr(self, f"process_{command}")(ctx.command_invocation(), cleaned_doc)
             else:
                 self.process_generic_command(command, ctx.command_invocation(), cleaned_doc)
         except Exception as e:
             line_num = ctx.command_invocation().start.line
             self.logger.error(
-                f"Caught exception while processing documented command beginning at line number {line_num}")
+                f"Caught exception while processing documented command beginning at line number {line_num}"
+            )
             raise e
 
-    def enterCommand_invocation(self, ctx: CMakeParser.Command_invocationContext):
+    def enterCommand_invocation(self, ctx: CMakeParser.Command_invocationContext) -> None:
         """
         Visitor for all other commands, used for locating position-dependent
         elements of documented commands, such as cpp_end_class() that pops the class stack,
         or a function or method definition for cpp_member().
         """
 
         command = ctx.Identifier().getText().lower()
@@ -557,14 +600,19 @@
                 self.process_cmake_parse_arguments(ctx, "")
             elif ((command == "function"
                    or command == "macro")
                   and self.documented_awaiting_function_def is not None):
                 # We've found the function/macro def that the previous documented command needed
                 params = [param.getText()
                           for param in ctx.single_argument()]
+                if isinstance(self.documented_awaiting_function_def, MethodDocumentation):
+                    params = [
+                        re.sub(self.settings.input.member_parameter_name_strip_regex, "", p.getText()) for p in
+                        ctx.single_argument()
+                    ]
 
                 self.documented_awaiting_function_def.is_macro = command == "macro"
 
                 # Ignore function name and self param
                 if len(params) > 2:
                     param_names = params[2:]
                     self.documented_awaiting_function_def.params.extend(param_names)
@@ -583,13 +631,22 @@
                     self.definition_command_stack.append(DefinitionCommand(None, False))
 
         except Exception as e:
             line_num = ctx.start.line
             self.logger.error(f"Caught exception while processing command beginning at line number {line_num}")
             raise e
 
-    def enterDocumented_module(self, ctx: CMakeParser.Documented_moduleContext):
+    def enterDocumented_module(self, ctx: CMakeParser.Documented_moduleContext) -> None:
         text = ctx.Module_docstring().getText()
         cleaned_lines = DocumentationAggregator.clean_doc_lines(text.split("\n")).split("\n")
         module_name = cleaned_lines[0].replace("@module", "").strip()
         doc = "\n".join(cleaned_lines[1:])
         self.documented.append(ModuleDocumentation(module_name, doc))
+
+    def enterBracket_doccomment(self, ctx: CMakeParser.Bracket_doccommentContext) -> None:
+        if ctx not in self.consumed:
+            # text = ctx.Docstring().getText()
+            # cleaned_lines = DocumentationAggregator.clean_doc_lines(text.split("\n")).split("\n")
+            # self.documented.append(DanglingDoccomment("", "\n".join(cleaned_lines)))
+            self.logger.warning(
+                f"Detected dangling doccomment, ignoring. RST may change depending on CMinx version."
+            )
```

### Comparing `CMinx-1.1.8/src/cminx/config.py` & `CMinx-1.1.9/src/cminx/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""
+Contains config objects, their defaults,
+the config template for confuse, and a function
+to convert a dictionary to a :class:`~Settings` object.
+
+The settings object mirrors the template and
+the :code:`config_default.yaml` file. Visit that file
+for information on what each setting does.
+"""
+
 import confuse
 import os
 from typing import List
 from dataclasses import dataclass, field
 
 
 def config_template(output_dir_relative_to_config: bool = False) -> dict:
@@ -36,14 +46,17 @@
             "include_undocumented_ct_add_test": bool,
             "include_undocumented_add_test": bool,
             "include_undocumented_ct_add_section": bool,
             "include_undocumented_option": bool,
             "auto_exclude_directories_without_cmake": bool,
             "kwargs_doc_trigger_string": confuse.Optional(confuse.String(), default=":keyword"),
             "exclude_filters": confuse.Optional(list, default=()),
+            "function_parameter_name_strip_regex": confuse.Optional(confuse.String(), default=""),
+            "macro_parameter_name_strip_regex": confuse.Optional(confuse.String(), default=""),
+            "member_parameter_name_strip_regex": confuse.Optional(confuse.String(), default=""),
             "recursive": bool,
             "follow_symlinks": bool
         },
         "output": {
             "directory": confuse.Optional(
                 confuse.Filename(cwd=os.getcwd()) if not output_dir_relative_to_config
                 else confuse.Filename(in_source_dir=True)),
@@ -72,14 +85,17 @@
     include_undocumented_ct_add_test: bool = True
     include_undocumented_ct_add_section: bool = True
     include_undocumented_add_test: bool = True
     include_undocumented_option: bool = True
     auto_exclude_directories_without_cmake: bool = True
     kwargs_doc_trigger_string: str = ":param **kwargs:"
     exclude_filters: List[str] = ()
+    function_parameter_name_strip_regex: str = ""
+    macro_parameter_name_strip_regex: str = ""
+    member_parameter_name_strip_regex: str = ""
     recursive: bool = False
     follow_symlinks: bool = False
 
 
 @dataclass
 class OutputSettings:
     directory: str = None
```

### Comparing `CMinx-1.1.8/src/cminx/config_default.yaml` & `CMinx-1.1.9/src/cminx/config_default.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,38 @@
   # or macro() definition. When this string is encountered
   # the defined command parameter list will be modified to include
   # "**kwargs" as the last parameter. This will also occur
   # if a call to "cmake_parse_arguments()" exists within the
   # body of the function or macro.
   kwargs_doc_trigger_string: ":keyword"
 
+  # Strips out any string matching this regex
+  # for parameter names. This is useful for when
+  # parameter names have a prefix/postfix to prevent
+  # name collisions. This affects function definitions.
+  #
+  # An example regex that strips the prefix "_abc_"
+  # from parameter names where "abc" is any combination of letters
+  # is below:
+  # function_parameter_name_strip_regex: "^_[a-zA-Z]*_"
+  function_parameter_name_strip_regex: ""
+
+  # Strips out any string matching this regex
+  # for parameter names. This is useful for when
+  # parameter names have a prefix/postfix to prevent
+  # name collisions. This affects macro definitions
+  macro_parameter_name_strip_regex: ""
+
+  # Strips out any string matching this regex
+  # for parameter names. This is useful for when
+  # parameter names have a prefix/postfix to prevent
+  # name collisions. This affects CMakePP
+  # class member definitions.
+  member_parameter_name_strip_regex: ""
+
   # Whether directories should be documented recursively
   recursive: false
 
   # Whether CMinx should follow symlinks that resolve to directories
   # when using recursive mode.
   # This can cause infinite recursion if the symlink resolves
   # to a parent directory of itself
```

### Comparing `CMinx-1.1.8/src/cminx/documentation_types.py` & `CMinx-1.1.9/src/cminx/documentation_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,37 @@
 an abstract :code:`process()` method to convert the dataclass
 representation into an RST representation using :class:`RSTWriter`.
 
 :Author: Branden Butler
 :License: Apache 2.0
 
 """
-
+import textwrap
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Union, List
 
-from . import Settings
 from .rstwriter import RSTWriter, Directive, interpreted_text
 
 
 class VarType(Enum):
     """The types of variables accepted by the CMake :code:`set()` command"""
     
     STRING = 1
+    """A String variable, ex: :code:`set(str_var "Hello")`"""
+
     LIST = 2
+    """A List variable, ex: :code:`set(list_var item1 item2 item3)`"""
+
     UNSET = 3
+    """
+    Unsetting a variable, i.e. not an actual variable but a declaration
+    that a variable no longer exists. Ex: :code:`set(MyVar)`
+    """
 
 
 @dataclass
 class DocumentationType(ABC):
     """
     This is the base class for all documentation types. It defines a single
     abstract process() method that is used to write the documentation RST
@@ -52,21 +59,21 @@
     """The name of the documentation type. For functions this is the function
     name, for variables this is the variable name, etc."""
 
     doc: str
     """The full doc comment, cleaned of # characters."""
 
     @abstractmethod
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         """
         Processes the data stored in this documentation type,
         converting it to RST form by using the given RST writer.
 
         :param writer: RSTWriter instance that the documentation
-        will be added to.
+                       will be added to.
         """
         pass
 
 
 @dataclass
 class AbstractCommandDefinitionDocumentation(DocumentationType, ABC):
     """
@@ -85,15 +92,15 @@
 class FunctionDocumentation(AbstractCommandDefinitionDocumentation):
     """
     This class serves as the representation of a documented
     CMake function definition. It converts the function definition
     directly to a Sphinx :code:`function` directive.
     """
 
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         param_list = self.params
         if self.has_kwargs:
             param_list.append("**kwargs")
         d = writer.directive(
             "function", f"{self.name}({' '.join(param_list)})")
         d.text(self.doc)
 
@@ -103,15 +110,15 @@
     """
     This class serves as the representation of a documented
     CMake macro definition. It converts the macro definition
     directly to a Sphinx :code:`function` directive and adds a
     :code:`note` directive specifying that it is a macro.
     """
 
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         param_list = self.params
         if self.has_kwargs:
             param_list.append("**kwargs")
         d = writer.directive(
             "function", f"{self.name}({' '.join(param_list)})")
         d.directive(
             "note",
@@ -121,28 +128,28 @@
 
 @dataclass
 class VariableDocumentation(DocumentationType):
     """
     This class serves as the representation of a documented
     CMake variable definition (:code:`set()` command). It can only
     recognize the CMake primitives :code:`str` and :code:`list`, as
-    well as the :code:`UNSET` subcommand.
+    well as the implied :code:`unset()` when no value is given.
 
     This class translates the definition into a Sphinx
     :code:`data` directive, with a :code:`Default value` field
     and a :code:`type` field.
     """
 
     type: Union[VarType, str]
     """The type that the variable is."""
 
     value: Union[str, None]
     """A default value that the variable has"""
 
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         d = writer.directive("data", f"{self.name}")
         d.text(self.doc)
         d.field("Default value", self.value)
         if self.type == VarType.STRING:
             var_type = "str"
         elif self.type == VarType.LIST:
             var_type = "list"
@@ -162,23 +169,23 @@
     also uses the :code:`data` directive, but includes a note
     specifying the variable is an option.
     """
 
     help_text: str
     """The help text that the option has."""
 
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         d = writer.directive("data", f"{self.name}")
         note = d.directive("note")
-        note.text(
+        note.text(textwrap.dedent(
             f"""
             This variable is a user-editable option,
             meaning it appears within the cache and can be
             edited on the command line by the :code:`-D` flag.
-            """)
+            """))
         d.text(self.doc)
         d.field("Help text", self.help_text)
         d.field("Default value", self.value if self.value is not None else "OFF")
         d.field("type", self.type)
 
 
 @dataclass
@@ -192,15 +199,15 @@
     a warning that it is a command invocation and not
     a definition.
     """
 
     params: List[str]
     """Any parameters passed to the command, unfiltered since this documentation type has no knowledge of the command"""
 
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         d = writer.directive(
             "function", f"{self.name}({' '.join(self.params)})")
         d.directive(
             "warning",
             "This is a generic command invocation. It is not a function or macro definition.")
         d.text(self.doc)
 
@@ -212,15 +219,15 @@
     for a vanilla CTest test. These tests are created
     with the "add_test()" command from regular
     CMake, and documenting such a call will
     create this type of documentation.
     """
     params: List[str] = field(default_factory=lambda: [])
 
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         d = writer.directive(
             "function",
             f"{self.name}({' '.join(self.params)})")
         d.directive(
             "warning",
             'This is a CTest test definition, do not call this manually. '
             'Use the "ctest" program to execute this test.')
@@ -243,15 +250,15 @@
 
     params: List[str] = field(default_factory=lambda: [])
     """Any parameters defined by the linked function."""
 
     is_macro: bool = False
     """Whether the linked command is a macro or a function. If true, a warning stating so is generated."""
 
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         d = writer.directive(
             "function",
             f"{self.name}({'EXPECTFAIL' if self.expect_fail else ''})")
         d.directive(
             "warning",
             "This is a CMakeTest test definition, do not call this manually.")
         d.text(self.doc)
@@ -263,15 +270,15 @@
     This class provides support for documenting
     CMakeTest test sections. It translates the
     section exactly as :class:`TestDocumentation`
     except that the warning says that it is a test
     section.
     """
 
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         d = writer.directive(
             "function",
             f"{self.name}({'EXPECTFAIL' if self.expect_fail else ''})")
         d.directive(
             "warning",
             "This is a CMakeTest section definition, do not call this manually.")
         d.text(self.doc)
@@ -301,15 +308,15 @@
 
     is_constructor: bool
     """Whether this method is a constructor."""
 
     is_macro: bool = False
     """Whether the linked command is a macro or a function. If true, a note saying so is generated."""
 
-    def process(self, writer: Directive):
+    def process(self, writer: Directive) -> None:
         params_pretty = ', '.join(
             self.params) + ("[, ...]" if "args" in self.param_types else "")
         d = writer.directive(
             "py:method", f"{self.name}({params_pretty})")
         if self.is_macro:
             d.directive(
                 "note",
@@ -340,15 +347,15 @@
     """
     parent_class: str
     """The class that defines this attribute."""
 
     default_value: str
     """The default value of this attribute, if it has one."""
 
-    def process(self, writer: Directive):
+    def process(self, writer: Directive) -> None:
         d = writer.directive("py:attribute", f"{self.name}")
         if self.default_value is not None:
             d.option("value", self.default_value)
 
         d.text(self.doc)
 
 
@@ -380,15 +387,15 @@
 
     members: List[MethodDocumentation]
     """A list of method documentation objects describing the class's methods."""
 
     attributes: List[AttributeDocumentation]
     """A list of attribute documentation objects describing the class's attributes."""
 
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         d = writer.directive("py:class", f"{self.name}")
         if len(self.superclasses) > 0:
             bases = "Bases: " + \
                     ", ".join(
                         f":class:`{superclass}`" for superclass in self.superclasses)
             d.text(bases + '\n')
         d.text(self.doc)
@@ -415,11 +422,22 @@
 
 @dataclass
 class ModuleDocumentation(DocumentationType):
     """
     Represents documentation for an entire CMake module
     """
 
-    def process(self, writer: RSTWriter):
+    def process(self, writer: RSTWriter) -> None:
         module = writer.directive("module", self.name)
         if self.doc is not None and len(self.doc) != 0:
             module.text(self.doc)
+
+
+@dataclass
+class DanglingDoccomment(DocumentationType):
+    """
+    Represents a doccomment that is not attached to any other entity.
+    This documentation type's name is left unused, and the doc contains
+    the cleaned text of the dangling doccomment.
+    """
+    def process(self, writer: RSTWriter) -> None:
+        writer.text(self.doc)
```

### Comparing `CMinx-1.1.8/src/cminx/documenter.py` & `CMinx-1.1.9/src/cminx/documenter.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-This file contains the Documenter class, which combines functionality
-from parser.aggregator and rstwriter to generate RST documentation
-for CMake files.
+This file contains the Documenter class, which is the top-level
+entrypoint into the CMinx documentation system. It handles parsing,
+aggregating, and RST writing.
 
 :Author: Branden Butler
 :License: Apache 2.0
 
 """
 from typing import List
 
@@ -32,80 +32,102 @@
 from .parser.CMakeLexer import CMakeLexer
 from .parser.CMakeParser import CMakeParser
 from .rstwriter import RSTWriter, Directive
 
 
 class Documenter(object):
     """
-    Generates RST documentation from aggregated documentation, combining parser.aggregator and rstwriter.
+    Generates RST documentation from aggregated documentation, combining
+    :class:`~cminx.aggregator.DocumentationAggregator` and :class:`~cminx.rstwriter.RSTWriter`.
+    The entrypoint for this class is the :meth:`process` method.
     """
 
     def __init__(
             self,
             file: str,
             title: str = None,
             module_name: str = None,
-            settings: Settings = Settings()):
+            settings: Settings = Settings()) -> None:
         """
         :param file: CMake file to read documentation from.
         :param title: RST header title to use in the generated document.
+        :param module_name: The name of the CMake module, used in the module directive if
+                            no other name is given in a module doccomment.
         :param settings: Dictionary containing application settings for documentation
         """
 
-        self.settings = settings
+        self.settings: Settings = settings
+        """Settings used for aggregation and RST generation, passed down to all downstream components."""
 
         title = file if title is None else title
 
         if module_name is None:
             module_name = title
 
-        self.module_name = module_name
+        self.module_name: str = module_name
+        """The name of the CMake module, used as a default when no name given via a module doccomment."""
 
-        self.writer = RSTWriter(title, settings=settings)
+        self.writer: RSTWriter = RSTWriter(title, settings=settings)
+        """The writer that is passed to the aggregated documentation objects."""
 
         self.module: Directive
+        """The :code:`.. module::` directive that defines the module's name."""
 
         # We need a string stream of some kind, FileStream is easiest
-        self.input_stream = FileStream(file)
+        self.input_stream: InputStream = FileStream(file)
+        """The string stream used to read the CMake file."""
 
         # Convert those strings into tokens and build a stream from those
-        self.lexer = CMakeLexer(self.input_stream)
-        self.stream = CommonTokenStream(self.lexer)
+        self.lexer: CMakeLexer = CMakeLexer(self.input_stream)
+        """The lexer used to generate the token stream."""
+
+        self.stream: TokenStream = CommonTokenStream(self.lexer)
+        """The stream of tokens from the lexer, should be passed to the parser."""
 
         # We now have a stream of CommonToken instead of strings, parsers
         # require this type of stream
-        self.parser = CMakeParser(self.stream)
+        self.parser: CMakeParser = CMakeParser(self.stream)
+        """
+        The parser used to parse the token stream and call our listener.
+        By default, an instance of :class:`~cminx.parser.ParserErrorListener` is
+        added.
+        """
+
         self.parser.addErrorListener(ParserErrorListener())
 
         # Hard part is done, we now have a fully usable parse tree, now we just
         # need to walk it
-        self.aggregator = DocumentationAggregator(settings)
-        self.walker = ParseTreeWalker()
+        self.aggregator: DocumentationAggregator = DocumentationAggregator(settings)
+        """The aggregator used to listen for parser rules and generate documentation objects."""
+
+        self.walker: ParseTreeWalker = ParseTreeWalker()
+        """Walks the parser tree at a given parser rule, used to kick off aggregation."""
 
     def process(self) -> RSTWriter:
         """
-        Process Documenter.aggregator.documented and build RST document from it.
+        Process :attr:`cminx.aggregator.DocumentationAggregator.documented` and build RST document from it.
 
-        :return: Completed RSTWriter document, also located in Documenter.writer
+        :return: Completed RSTWriter document, also located in :attr:`Documenter.writer`
         """
 
         # Parse and lex the file, then walk the tree and aggregate the
         # documented commands
         self.walker.walk(self.aggregator, self.parser.cmake_file())
 
         # All the documented commands are now stored in aggregator.documented,
         # each element is a namedtuple representing the type of documentation it is.
         # So far we can document functions, macros, and variables (only strings
         # and lists built using set)
         self.process_docs(self.aggregator.documented)
         return self.writer
 
-    def process_docs(self, docs: List[DocumentationType]):
+    def process_docs(self, docs: List[DocumentationType]) -> None:
         """
-        Loops over document and calls Documentation.process() with self.writer
+        Loops over document and calls :meth:`cminx.documentation_types.DocumentationType.process` with
+        :attr:`~Documenter.writer`.
 
         :param docs: List of documentation objects.
         """
 
         module_docs = [x for x in docs if isinstance(x, ModuleDocumentation)]
 
         if len(module_docs) == 0:
```

### Comparing `CMinx-1.1.8/src/cminx/parser/CMake.g4` & `CMinx-1.1.9/src/cminx/parser/CMake.g4`

 * *Files 22% similar despite different names*

```diff
@@ -15,39 +15,47 @@
 
 /*
 Changes:
 	Renamed from file to cmake_file to avoid conflict with Python
 	Added documented_command to list of expected parser rules
 	Added bracket_doccomment to parser rules
 	Added Docstring to lexer rules
+	Added bracket_doccomment to top-level parse rule, enabling dangling doccomments
+*/
+
+/*Begin CMinx*/
+
+/*
+    WARNING: This grammar is ambiguous because of the bracket_doccomment alternative.
+    Ambiguity is resolved via order of alternatives, ensure order is consistent
+    with the desired precedence.
 */
 cmake_file
-	: documented_module? (documented_command | command_invocation)* EOF
+	: documented_module? (documented_command | command_invocation | bracket_doccomment)* EOF
 	;
 
-/*Begin CMinx*/
 
 documented_command
 	: bracket_doccomment command_invocation
 	;
 
 documented_module
     : Module_docstring
     ;
 
 bracket_doccomment
     : Docstring
     ;
 
 Module_docstring
-    : Doccomment_start Space? '@module' (Space Unquoted_argument)? .*? '#]]'
+    : Doccomment_start Space? '@module' (Space Unquoted_argument)? .*? Blockcomment_end
     ;
 
 Docstring
-        : Doccomment_start .*? '#]]'
+        : Doccomment_start Space? .*? Blockcomment_end
 	;
 
 
 Doccomment_start
     : '#[[['
     ;
```

### Comparing `CMinx-1.1.8/src/cminx/parser/CMake.interp` & `CMinx-1.1.9/src/cminx/parser/CMake.interp`

 * *Files 3% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 bracket_doccomment
 command_invocation
 single_argument
 compound_argument
 
 
 atn:
-[3, 24715, 42794, 33075, 47597, 16764, 15335, 30598, 22884, 3, 17, 59, 4, 2, 9, 2, 4, 3, 9, 3, 4, 4, 9, 4, 4, 5, 9, 5, 4, 6, 9, 6, 4, 7, 9, 7, 4, 8, 9, 8, 3, 2, 5, 2, 18, 10, 2, 3, 2, 3, 2, 7, 2, 22, 10, 2, 12, 2, 14, 2, 25, 11, 2, 3, 2, 3, 2, 3, 3, 3, 3, 3, 3, 3, 4, 3, 4, 3, 5, 3, 5, 3, 6, 3, 6, 3, 6, 3, 6, 7, 6, 40, 10, 6, 12, 6, 14, 6, 43, 11, 6, 3, 6, 3, 6, 3, 7, 3, 7, 3, 8, 3, 8, 3, 8, 7, 8, 52, 10, 8, 12, 8, 14, 8, 55, 11, 8, 3, 8, 3, 8, 3, 8, 2, 2, 9, 2, 4, 6, 8, 10, 12, 14, 2, 3, 4, 2, 9, 10, 12, 13, 2, 58, 2, 17, 3, 2, 2, 2, 4, 28, 3, 2, 2, 2, 6, 31, 3, 2, 2, 2, 8, 33, 3, 2, 2, 2, 10, 35, 3, 2, 2, 2, 12, 46, 3, 2, 2, 2, 14, 48, 3, 2, 2, 2, 16, 18, 5, 6, 4, 2, 17, 16, 3, 2, 2, 2, 17, 18, 3, 2, 2, 2, 18, 23, 3, 2, 2, 2, 19, 22, 5, 4, 3, 2, 20, 22, 5, 10, 6, 2, 21, 19, 3, 2, 2, 2, 21, 20, 3, 2, 2, 2, 22, 25, 3, 2, 2, 2, 23, 21, 3, 2, 2, 2, 23, 24, 3, 2, 2, 2, 24, 26, 3, 2, 2, 2, 25, 23, 3, 2, 2, 2, 26, 27, 7, 2, 2, 3, 27, 3, 3, 2, 2, 2, 28, 29, 5, 8, 5, 2, 29, 30, 5, 10, 6, 2, 30, 5, 3, 2, 2, 2, 31, 32, 7, 5, 2, 2, 32, 7, 3, 2, 2, 2, 33, 34, 7, 6, 2, 2, 34, 9, 3, 2, 2, 2, 35, 36, 7, 9, 2, 2, 36, 41, 7, 3, 2, 2, 37, 40, 5, 12, 7, 2, 38, 40, 5, 14, 8, 2, 39, 37, 3, 2, 2, 2, 39, 38, 3, 2, 2, 2, 40, 43, 3, 2, 2, 2, 41, 39, 3, 2, 2, 2, 41, 42, 3, 2, 2, 2, 42, 44, 3, 2, 2, 2, 43, 41, 3, 2, 2, 2, 44, 45, 7, 4, 2, 2, 45, 11, 3, 2, 2, 2, 46, 47, 9, 2, 2, 2, 47, 13, 3, 2, 2, 2, 48, 53, 7, 3, 2, 2, 49, 52, 5, 12, 7, 2, 50, 52, 5, 14, 8, 2, 51, 49, 3, 2, 2, 2, 51, 50, 3, 2, 2, 2, 52, 55, 3, 2, 2, 2, 53, 51, 3, 2, 2, 2, 53, 54, 3, 2, 2, 2, 54, 56, 3, 2, 2, 2, 55, 53, 3, 2, 2, 2, 56, 57, 7, 4, 2, 2, 57, 15, 3, 2, 2, 2, 9, 17, 21, 23, 39, 41, 51, 53]
+[3, 24715, 42794, 33075, 47597, 16764, 15335, 30598, 22884, 3, 17, 60, 4, 2, 9, 2, 4, 3, 9, 3, 4, 4, 9, 4, 4, 5, 9, 5, 4, 6, 9, 6, 4, 7, 9, 7, 4, 8, 9, 8, 3, 2, 5, 2, 18, 10, 2, 3, 2, 3, 2, 3, 2, 7, 2, 23, 10, 2, 12, 2, 14, 2, 26, 11, 2, 3, 2, 3, 2, 3, 3, 3, 3, 3, 3, 3, 4, 3, 4, 3, 5, 3, 5, 3, 6, 3, 6, 3, 6, 3, 6, 7, 6, 41, 10, 6, 12, 6, 14, 6, 44, 11, 6, 3, 6, 3, 6, 3, 7, 3, 7, 3, 8, 3, 8, 3, 8, 7, 8, 53, 10, 8, 12, 8, 14, 8, 56, 11, 8, 3, 8, 3, 8, 3, 8, 2, 2, 9, 2, 4, 6, 8, 10, 12, 14, 2, 3, 4, 2, 9, 10, 12, 13, 2, 60, 2, 17, 3, 2, 2, 2, 4, 29, 3, 2, 2, 2, 6, 32, 3, 2, 2, 2, 8, 34, 3, 2, 2, 2, 10, 36, 3, 2, 2, 2, 12, 47, 3, 2, 2, 2, 14, 49, 3, 2, 2, 2, 16, 18, 5, 6, 4, 2, 17, 16, 3, 2, 2, 2, 17, 18, 3, 2, 2, 2, 18, 24, 3, 2, 2, 2, 19, 23, 5, 4, 3, 2, 20, 23, 5, 10, 6, 2, 21, 23, 5, 8, 5, 2, 22, 19, 3, 2, 2, 2, 22, 20, 3, 2, 2, 2, 22, 21, 3, 2, 2, 2, 23, 26, 3, 2, 2, 2, 24, 22, 3, 2, 2, 2, 24, 25, 3, 2, 2, 2, 25, 27, 3, 2, 2, 2, 26, 24, 3, 2, 2, 2, 27, 28, 7, 2, 2, 3, 28, 3, 3, 2, 2, 2, 29, 30, 5, 8, 5, 2, 30, 31, 5, 10, 6, 2, 31, 5, 3, 2, 2, 2, 32, 33, 7, 5, 2, 2, 33, 7, 3, 2, 2, 2, 34, 35, 7, 6, 2, 2, 35, 9, 3, 2, 2, 2, 36, 37, 7, 9, 2, 2, 37, 42, 7, 3, 2, 2, 38, 41, 5, 12, 7, 2, 39, 41, 5, 14, 8, 2, 40, 38, 3, 2, 2, 2, 40, 39, 3, 2, 2, 2, 41, 44, 3, 2, 2, 2, 42, 40, 3, 2, 2, 2, 42, 43, 3, 2, 2, 2, 43, 45, 3, 2, 2, 2, 44, 42, 3, 2, 2, 2, 45, 46, 7, 4, 2, 2, 46, 11, 3, 2, 2, 2, 47, 48, 9, 2, 2, 2, 48, 13, 3, 2, 2, 2, 49, 54, 7, 3, 2, 2, 50, 53, 5, 12, 7, 2, 51, 53, 5, 14, 8, 2, 52, 50, 3, 2, 2, 2, 52, 51, 3, 2, 2, 2, 53, 56, 3, 2, 2, 2, 54, 52, 3, 2, 2, 2, 54, 55, 3, 2, 2, 2, 55, 57, 3, 2, 2, 2, 56, 54, 3, 2, 2, 2, 57, 58, 7, 4, 2, 2, 58, 15, 3, 2, 2, 2, 9, 17, 22, 24, 40, 42, 52, 54]
```

### Comparing `CMinx-1.1.8/src/cminx/parser/CMakeLexer.interp` & `CMinx-1.1.9/src/cminx/parser/CMakeLexer.interp`

 * *Files 4% similar despite different names*

```diff
@@ -60,8 +60,8 @@
 DEFAULT_TOKEN_CHANNEL
 HIDDEN
 
 mode names:
 DEFAULT_MODE
 
 atn:
-[3, 24715, 42794, 33075, 47597, 16764, 15335, 30598, 22884, 2, 17, 230, 8, 1, 4, 2, 9, 2, 4, 3, 9, 3, 4, 4, 9, 4, 4, 5, 9, 5, 4, 6, 9, 6, 4, 7, 9, 7, 4, 8, 9, 8, 4, 9, 9, 9, 4, 10, 9, 10, 4, 11, 9, 11, 4, 12, 9, 12, 4, 13, 9, 13, 4, 14, 9, 14, 4, 15, 9, 15, 4, 16, 9, 16, 4, 17, 9, 17, 4, 18, 9, 18, 4, 19, 9, 19, 4, 20, 9, 20, 4, 21, 9, 21, 3, 2, 3, 2, 3, 3, 3, 3, 3, 4, 3, 4, 5, 4, 50, 10, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 5, 4, 63, 10, 4, 3, 4, 7, 4, 66, 10, 4, 12, 4, 14, 4, 69, 11, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 5, 3, 5, 7, 5, 77, 10, 5, 12, 5, 14, 5, 80, 11, 5, 3, 5, 3, 5, 3, 5, 3, 5, 3, 6, 3, 6, 3, 6, 3, 6, 3, 6, 3, 7, 3, 7, 3, 7, 3, 7, 3, 8, 3, 8, 7, 8, 97, 10, 8, 12, 8, 14, 8, 100, 11, 8, 3, 9, 3, 9, 6, 9, 104, 10, 9, 13, 9, 14, 9, 105, 3, 10, 3, 10, 3, 10, 5, 10, 111, 10, 10, 3, 11, 3, 11, 3, 11, 3, 12, 3, 12, 3, 12, 3, 12, 3, 12, 3, 12, 5, 12, 122, 10, 12, 3, 13, 3, 13, 3, 13, 3, 14, 3, 14, 3, 14, 3, 14, 7, 14, 131, 10, 14, 12, 14, 14, 14, 134, 11, 14, 3, 14, 3, 14, 3, 15, 3, 15, 3, 15, 5, 15, 141, 10, 15, 3, 15, 5, 15, 144, 10, 15, 3, 16, 3, 16, 3, 16, 3, 16, 3, 17, 3, 17, 3, 17, 3, 17, 3, 17, 3, 17, 7, 17, 156, 10, 17, 12, 17, 14, 17, 159, 11, 17, 3, 17, 5, 17, 162, 10, 17, 3, 18, 3, 18, 3, 18, 3, 18, 3, 18, 3, 18, 3, 18, 3, 18, 3, 19, 3, 19, 3, 19, 3, 19, 7, 19, 176, 10, 19, 12, 19, 14, 19, 179, 11, 19, 3, 19, 3, 19, 7, 19, 183, 10, 19, 12, 19, 14, 19, 186, 11, 19, 3, 19, 3, 19, 7, 19, 190, 10, 19, 12, 19, 14, 19, 193, 11, 19, 3, 19, 3, 19, 7, 19, 197, 10, 19, 12, 19, 14, 19, 200, 11, 19, 5, 19, 202, 10, 19, 3, 19, 3, 19, 5, 19, 206, 10, 19, 3, 19, 5, 19, 209, 10, 19, 3, 19, 3, 19, 3, 20, 3, 20, 5, 20, 215, 10, 20, 3, 20, 6, 20, 218, 10, 20, 13, 20, 14, 20, 219, 3, 20, 3, 20, 3, 21, 6, 21, 225, 10, 21, 13, 21, 14, 21, 226, 3, 21, 3, 21, 5, 67, 78, 157, 2, 22, 3, 3, 5, 4, 7, 5, 9, 6, 11, 7, 13, 8, 15, 9, 17, 10, 19, 11, 21, 2, 23, 2, 25, 2, 27, 12, 29, 2, 31, 13, 33, 2, 35, 14, 37, 15, 39, 16, 41, 17, 3, 2, 12, 5, 2, 67, 92, 97, 97, 99, 124, 6, 2, 50, 59, 67, 92, 97, 97, 99, 124, 8, 2, 11, 12, 15, 15, 34, 34, 36, 37, 42, 43, 94, 94, 6, 2, 50, 59, 61, 61, 67, 92, 99, 124, 4, 2, 36, 36, 94, 94, 6, 2, 12, 12, 15, 15, 63, 63, 93, 93, 4, 2, 12, 12, 15, 15, 5, 2, 12, 12, 15, 15, 93, 93, 3, 3, 12, 12, 4, 2, 11, 11, 34, 34, 2, 255, 2, 3, 3, 2, 2, 2, 2, 5, 3, 2, 2, 2, 2, 7, 3, 2, 2, 2, 2, 9, 3, 2, 2, 2, 2, 11, 3, 2, 2, 2, 2, 13, 3, 2, 2, 2, 2, 15, 3, 2, 2, 2, 2, 17, 3, 2, 2, 2, 2, 19, 3, 2, 2, 2, 2, 27, 3, 2, 2, 2, 2, 31, 3, 2, 2, 2, 2, 35, 3, 2, 2, 2, 2, 37, 3, 2, 2, 2, 2, 39, 3, 2, 2, 2, 2, 41, 3, 2, 2, 2, 3, 43, 3, 2, 2, 2, 5, 45, 3, 2, 2, 2, 7, 47, 3, 2, 2, 2, 9, 74, 3, 2, 2, 2, 11, 85, 3, 2, 2, 2, 13, 90, 3, 2, 2, 2, 15, 94, 3, 2, 2, 2, 17, 103, 3, 2, 2, 2, 19, 110, 3, 2, 2, 2, 21, 112, 3, 2, 2, 2, 23, 121, 3, 2, 2, 2, 25, 123, 3, 2, 2, 2, 27, 126, 3, 2, 2, 2, 29, 137, 3, 2, 2, 2, 31, 145, 3, 2, 2, 2, 33, 161, 3, 2, 2, 2, 35, 163, 3, 2, 2, 2, 37, 171, 3, 2, 2, 2, 39, 217, 3, 2, 2, 2, 41, 224, 3, 2, 2, 2, 43, 44, 7, 42, 2, 2, 44, 4, 3, 2, 2, 2, 45, 46, 7, 43, 2, 2, 46, 6, 3, 2, 2, 2, 47, 49, 5, 11, 6, 2, 48, 50, 5, 41, 21, 2, 49, 48, 3, 2, 2, 2, 49, 50, 3, 2, 2, 2, 50, 51, 3, 2, 2, 2, 51, 52, 7, 66, 2, 2, 52, 53, 7, 111, 2, 2, 53, 54, 7, 113, 2, 2, 54, 55, 7, 102, 2, 2, 55, 56, 7, 119, 2, 2, 56, 57, 7, 110, 2, 2, 57, 58, 7, 103, 2, 2, 58, 62, 3, 2, 2, 2, 59, 60, 5, 41, 21, 2, 60, 61, 5, 17, 9, 2, 61, 63, 3, 2, 2, 2, 62, 59, 3, 2, 2, 2, 62, 63, 3, 2, 2, 2, 63, 67, 3, 2, 2, 2, 64, 66, 11, 2, 2, 2, 65, 64, 3, 2, 2, 2, 66, 69, 3, 2, 2, 2, 67, 68, 3, 2, 2, 2, 67, 65, 3, 2, 2, 2, 68, 70, 3, 2, 2, 2, 69, 67, 3, 2, 2, 2, 70, 71, 7, 37, 2, 2, 71, 72, 7, 95, 2, 2, 72, 73, 7, 95, 2, 2, 73, 8, 3, 2, 2, 2, 74, 78, 5, 11, 6, 2, 75, 77, 11, 2, 2, 2, 76, 75, 3, 2, 2, 2, 77, 80, 3, 2, 2, 2, 78, 79, 3, 2, 2, 2, 78, 76, 3, 2, 2, 2, 79, 81, 3, 2, 2, 2, 80, 78, 3, 2, 2, 2, 81, 82, 7, 37, 2, 2, 82, 83, 7, 95, 2, 2, 83, 84, 7, 95, 2, 2, 84, 10, 3, 2, 2, 2, 85, 86, 7, 37, 2, 2, 86, 87, 7, 93, 2, 2, 87, 88, 7, 93, 2, 2, 88, 89, 7, 93, 2, 2, 89, 12, 3, 2, 2, 2, 90, 91, 7, 37, 2, 2, 91, 92, 7, 95, 2, 2, 92, 93, 7, 95, 2, 2, 93, 14, 3, 2, 2, 2, 94, 98, 9, 2, 2, 2, 95, 97, 9, 3, 2, 2, 96, 95, 3, 2, 2, 2, 97, 100, 3, 2, 2, 2, 98, 96, 3, 2, 2, 2, 98, 99, 3, 2, 2, 2, 99, 16, 3, 2, 2, 2, 100, 98, 3, 2, 2, 2, 101, 104, 10, 4, 2, 2, 102, 104, 5, 19, 10, 2, 103, 101, 3, 2, 2, 2, 103, 102, 3, 2, 2, 2, 104, 105, 3, 2, 2, 2, 105, 103, 3, 2, 2, 2, 105, 106, 3, 2, 2, 2, 106, 18, 3, 2, 2, 2, 107, 111, 5, 21, 11, 2, 108, 111, 5, 23, 12, 2, 109, 111, 5, 25, 13, 2, 110, 107, 3, 2, 2, 2, 110, 108, 3, 2, 2, 2, 110, 109, 3, 2, 2, 2, 111, 20, 3, 2, 2, 2, 112, 113, 7, 94, 2, 2, 113, 114, 10, 5, 2, 2, 114, 22, 3, 2, 2, 2, 115, 116, 7, 94, 2, 2, 116, 122, 7, 118, 2, 2, 117, 118, 7, 94, 2, 2, 118, 122, 7, 116, 2, 2, 119, 120, 7, 94, 2, 2, 120, 122, 7, 112, 2, 2, 121, 115, 3, 2, 2, 2, 121, 117, 3, 2, 2, 2, 121, 119, 3, 2, 2, 2, 122, 24, 3, 2, 2, 2, 123, 124, 7, 94, 2, 2, 124, 125, 7, 61, 2, 2, 125, 26, 3, 2, 2, 2, 126, 132, 7, 36, 2, 2, 127, 131, 10, 6, 2, 2, 128, 131, 5, 19, 10, 2, 129, 131, 5, 29, 15, 2, 130, 127, 3, 2, 2, 2, 130, 128, 3, 2, 2, 2, 130, 129, 3, 2, 2, 2, 131, 134, 3, 2, 2, 2, 132, 130, 3, 2, 2, 2, 132, 133, 3, 2, 2, 2, 133, 135, 3, 2, 2, 2, 134, 132, 3, 2, 2, 2, 135, 136, 7, 36, 2, 2, 136, 28, 3, 2, 2, 2, 137, 143, 7, 94, 2, 2, 138, 140, 7, 15, 2, 2, 139, 141, 7, 12, 2, 2, 140, 139, 3, 2, 2, 2, 140, 141, 3, 2, 2, 2, 141, 144, 3, 2, 2, 2, 142, 144, 7, 12, 2, 2, 143, 138, 3, 2, 2, 2, 143, 142, 3, 2, 2, 2, 144, 30, 3, 2, 2, 2, 145, 146, 7, 93, 2, 2, 146, 147, 5, 33, 17, 2, 147, 148, 7, 95, 2, 2, 148, 32, 3, 2, 2, 2, 149, 150, 7, 63, 2, 2, 150, 151, 5, 33, 17, 2, 151, 152, 7, 63, 2, 2, 152, 162, 3, 2, 2, 2, 153, 157, 7, 93, 2, 2, 154, 156, 11, 2, 2, 2, 155, 154, 3, 2, 2, 2, 156, 159, 3, 2, 2, 2, 157, 158, 3, 2, 2, 2, 157, 155, 3, 2, 2, 2, 158, 160, 3, 2, 2, 2, 159, 157, 3, 2, 2, 2, 160, 162, 7, 95, 2, 2, 161, 149, 3, 2, 2, 2, 161, 153, 3, 2, 2, 2, 162, 34, 3, 2, 2, 2, 163, 164, 7, 37, 2, 2, 164, 165, 7, 93, 2, 2, 165, 166, 3, 2, 2, 2, 166, 167, 5, 33, 17, 2, 167, 168, 7, 95, 2, 2, 168, 169, 3, 2, 2, 2, 169, 170, 8, 18, 2, 2, 170, 36, 3, 2, 2, 2, 171, 201, 7, 37, 2, 2, 172, 202, 3, 2, 2, 2, 173, 177, 7, 93, 2, 2, 174, 176, 7, 63, 2, 2, 175, 174, 3, 2, 2, 2, 176, 179, 3, 2, 2, 2, 177, 175, 3, 2, 2, 2, 177, 178, 3, 2, 2, 2, 178, 202, 3, 2, 2, 2, 179, 177, 3, 2, 2, 2, 180, 184, 7, 93, 2, 2, 181, 183, 7, 63, 2, 2, 182, 181, 3, 2, 2, 2, 183, 186, 3, 2, 2, 2, 184, 182, 3, 2, 2, 2, 184, 185, 3, 2, 2, 2, 185, 187, 3, 2, 2, 2, 186, 184, 3, 2, 2, 2, 187, 191, 10, 7, 2, 2, 188, 190, 10, 8, 2, 2, 189, 188, 3, 2, 2, 2, 190, 193, 3, 2, 2, 2, 191, 189, 3, 2, 2, 2, 191, 192, 3, 2, 2, 2, 192, 202, 3, 2, 2, 2, 193, 191, 3, 2, 2, 2, 194, 198, 10, 9, 2, 2, 195, 197, 10, 8, 2, 2, 196, 195, 3, 2, 2, 2, 197, 200, 3, 2, 2, 2, 198, 196, 3, 2, 2, 2, 198, 199, 3, 2, 2, 2, 199, 202, 3, 2, 2, 2, 200, 198, 3, 2, 2, 2, 201, 172, 3, 2, 2, 2, 201, 173, 3, 2, 2, 2, 201, 180, 3, 2, 2, 2, 201, 194, 3, 2, 2, 2, 202, 208, 3, 2, 2, 2, 203, 205, 7, 15, 2, 2, 204, 206, 7, 12, 2, 2, 205, 204, 3, 2, 2, 2, 205, 206, 3, 2, 2, 2, 206, 209, 3, 2, 2, 2, 207, 209, 9, 10, 2, 2, 208, 203, 3, 2, 2, 2, 208, 207, 3, 2, 2, 2, 209, 210, 3, 2, 2, 2, 210, 211, 8, 19, 2, 2, 211, 38, 3, 2, 2, 2, 212, 214, 7, 15, 2, 2, 213, 215, 7, 12, 2, 2, 214, 213, 3, 2, 2, 2, 214, 215, 3, 2, 2, 2, 215, 218, 3, 2, 2, 2, 216, 218, 7, 12, 2, 2, 217, 212, 3, 2, 2, 2, 217, 216, 3, 2, 2, 2, 218, 219, 3, 2, 2, 2, 219, 217, 3, 2, 2, 2, 219, 220, 3, 2, 2, 2, 220, 221, 3, 2, 2, 2, 221, 222, 8, 20, 2, 2, 222, 40, 3, 2, 2, 2, 223, 225, 9, 11, 2, 2, 224, 223, 3, 2, 2, 2, 225, 226, 3, 2, 2, 2, 226, 224, 3, 2, 2, 2, 226, 227, 3, 2, 2, 2, 227, 228, 3, 2, 2, 2, 228, 229, 8, 21, 2, 2, 229, 42, 3, 2, 2, 2, 29, 2, 49, 62, 67, 78, 98, 103, 105, 110, 121, 130, 132, 140, 143, 157, 161, 177, 184, 191, 198, 201, 205, 208, 214, 217, 219, 226, 3, 8, 2, 2]
+[3, 24715, 42794, 33075, 47597, 16764, 15335, 30598, 22884, 2, 17, 229, 8, 1, 4, 2, 9, 2, 4, 3, 9, 3, 4, 4, 9, 4, 4, 5, 9, 5, 4, 6, 9, 6, 4, 7, 9, 7, 4, 8, 9, 8, 4, 9, 9, 9, 4, 10, 9, 10, 4, 11, 9, 11, 4, 12, 9, 12, 4, 13, 9, 13, 4, 14, 9, 14, 4, 15, 9, 15, 4, 16, 9, 16, 4, 17, 9, 17, 4, 18, 9, 18, 4, 19, 9, 19, 4, 20, 9, 20, 4, 21, 9, 21, 3, 2, 3, 2, 3, 3, 3, 3, 3, 4, 3, 4, 5, 4, 50, 10, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 5, 4, 63, 10, 4, 3, 4, 7, 4, 66, 10, 4, 12, 4, 14, 4, 69, 11, 4, 3, 4, 3, 4, 3, 5, 3, 5, 5, 5, 75, 10, 5, 3, 5, 7, 5, 78, 10, 5, 12, 5, 14, 5, 81, 11, 5, 3, 5, 3, 5, 3, 6, 3, 6, 3, 6, 3, 6, 3, 6, 3, 7, 3, 7, 3, 7, 3, 7, 3, 8, 3, 8, 7, 8, 96, 10, 8, 12, 8, 14, 8, 99, 11, 8, 3, 9, 3, 9, 6, 9, 103, 10, 9, 13, 9, 14, 9, 104, 3, 10, 3, 10, 3, 10, 5, 10, 110, 10, 10, 3, 11, 3, 11, 3, 11, 3, 12, 3, 12, 3, 12, 3, 12, 3, 12, 3, 12, 5, 12, 121, 10, 12, 3, 13, 3, 13, 3, 13, 3, 14, 3, 14, 3, 14, 3, 14, 7, 14, 130, 10, 14, 12, 14, 14, 14, 133, 11, 14, 3, 14, 3, 14, 3, 15, 3, 15, 3, 15, 5, 15, 140, 10, 15, 3, 15, 5, 15, 143, 10, 15, 3, 16, 3, 16, 3, 16, 3, 16, 3, 17, 3, 17, 3, 17, 3, 17, 3, 17, 3, 17, 7, 17, 155, 10, 17, 12, 17, 14, 17, 158, 11, 17, 3, 17, 5, 17, 161, 10, 17, 3, 18, 3, 18, 3, 18, 3, 18, 3, 18, 3, 18, 3, 18, 3, 18, 3, 19, 3, 19, 3, 19, 3, 19, 7, 19, 175, 10, 19, 12, 19, 14, 19, 178, 11, 19, 3, 19, 3, 19, 7, 19, 182, 10, 19, 12, 19, 14, 19, 185, 11, 19, 3, 19, 3, 19, 7, 19, 189, 10, 19, 12, 19, 14, 19, 192, 11, 19, 3, 19, 3, 19, 7, 19, 196, 10, 19, 12, 19, 14, 19, 199, 11, 19, 5, 19, 201, 10, 19, 3, 19, 3, 19, 5, 19, 205, 10, 19, 3, 19, 5, 19, 208, 10, 19, 3, 19, 3, 19, 3, 20, 3, 20, 5, 20, 214, 10, 20, 3, 20, 6, 20, 217, 10, 20, 13, 20, 14, 20, 218, 3, 20, 3, 20, 3, 21, 6, 21, 224, 10, 21, 13, 21, 14, 21, 225, 3, 21, 3, 21, 5, 67, 79, 156, 2, 22, 3, 3, 5, 4, 7, 5, 9, 6, 11, 7, 13, 8, 15, 9, 17, 10, 19, 11, 21, 2, 23, 2, 25, 2, 27, 12, 29, 2, 31, 13, 33, 2, 35, 14, 37, 15, 39, 16, 41, 17, 3, 2, 12, 5, 2, 67, 92, 97, 97, 99, 124, 6, 2, 50, 59, 67, 92, 97, 97, 99, 124, 8, 2, 11, 12, 15, 15, 34, 34, 36, 37, 42, 43, 94, 94, 6, 2, 50, 59, 61, 61, 67, 92, 99, 124, 4, 2, 36, 36, 94, 94, 6, 2, 12, 12, 15, 15, 63, 63, 93, 93, 4, 2, 12, 12, 15, 15, 5, 2, 12, 12, 15, 15, 93, 93, 3, 3, 12, 12, 4, 2, 11, 11, 34, 34, 2, 255, 2, 3, 3, 2, 2, 2, 2, 5, 3, 2, 2, 2, 2, 7, 3, 2, 2, 2, 2, 9, 3, 2, 2, 2, 2, 11, 3, 2, 2, 2, 2, 13, 3, 2, 2, 2, 2, 15, 3, 2, 2, 2, 2, 17, 3, 2, 2, 2, 2, 19, 3, 2, 2, 2, 2, 27, 3, 2, 2, 2, 2, 31, 3, 2, 2, 2, 2, 35, 3, 2, 2, 2, 2, 37, 3, 2, 2, 2, 2, 39, 3, 2, 2, 2, 2, 41, 3, 2, 2, 2, 3, 43, 3, 2, 2, 2, 5, 45, 3, 2, 2, 2, 7, 47, 3, 2, 2, 2, 9, 72, 3, 2, 2, 2, 11, 84, 3, 2, 2, 2, 13, 89, 3, 2, 2, 2, 15, 93, 3, 2, 2, 2, 17, 102, 3, 2, 2, 2, 19, 109, 3, 2, 2, 2, 21, 111, 3, 2, 2, 2, 23, 120, 3, 2, 2, 2, 25, 122, 3, 2, 2, 2, 27, 125, 3, 2, 2, 2, 29, 136, 3, 2, 2, 2, 31, 144, 3, 2, 2, 2, 33, 160, 3, 2, 2, 2, 35, 162, 3, 2, 2, 2, 37, 170, 3, 2, 2, 2, 39, 216, 3, 2, 2, 2, 41, 223, 3, 2, 2, 2, 43, 44, 7, 42, 2, 2, 44, 4, 3, 2, 2, 2, 45, 46, 7, 43, 2, 2, 46, 6, 3, 2, 2, 2, 47, 49, 5, 11, 6, 2, 48, 50, 5, 41, 21, 2, 49, 48, 3, 2, 2, 2, 49, 50, 3, 2, 2, 2, 50, 51, 3, 2, 2, 2, 51, 52, 7, 66, 2, 2, 52, 53, 7, 111, 2, 2, 53, 54, 7, 113, 2, 2, 54, 55, 7, 102, 2, 2, 55, 56, 7, 119, 2, 2, 56, 57, 7, 110, 2, 2, 57, 58, 7, 103, 2, 2, 58, 62, 3, 2, 2, 2, 59, 60, 5, 41, 21, 2, 60, 61, 5, 17, 9, 2, 61, 63, 3, 2, 2, 2, 62, 59, 3, 2, 2, 2, 62, 63, 3, 2, 2, 2, 63, 67, 3, 2, 2, 2, 64, 66, 11, 2, 2, 2, 65, 64, 3, 2, 2, 2, 66, 69, 3, 2, 2, 2, 67, 68, 3, 2, 2, 2, 67, 65, 3, 2, 2, 2, 68, 70, 3, 2, 2, 2, 69, 67, 3, 2, 2, 2, 70, 71, 5, 13, 7, 2, 71, 8, 3, 2, 2, 2, 72, 74, 5, 11, 6, 2, 73, 75, 5, 41, 21, 2, 74, 73, 3, 2, 2, 2, 74, 75, 3, 2, 2, 2, 75, 79, 3, 2, 2, 2, 76, 78, 11, 2, 2, 2, 77, 76, 3, 2, 2, 2, 78, 81, 3, 2, 2, 2, 79, 80, 3, 2, 2, 2, 79, 77, 3, 2, 2, 2, 80, 82, 3, 2, 2, 2, 81, 79, 3, 2, 2, 2, 82, 83, 5, 13, 7, 2, 83, 10, 3, 2, 2, 2, 84, 85, 7, 37, 2, 2, 85, 86, 7, 93, 2, 2, 86, 87, 7, 93, 2, 2, 87, 88, 7, 93, 2, 2, 88, 12, 3, 2, 2, 2, 89, 90, 7, 37, 2, 2, 90, 91, 7, 95, 2, 2, 91, 92, 7, 95, 2, 2, 92, 14, 3, 2, 2, 2, 93, 97, 9, 2, 2, 2, 94, 96, 9, 3, 2, 2, 95, 94, 3, 2, 2, 2, 96, 99, 3, 2, 2, 2, 97, 95, 3, 2, 2, 2, 97, 98, 3, 2, 2, 2, 98, 16, 3, 2, 2, 2, 99, 97, 3, 2, 2, 2, 100, 103, 10, 4, 2, 2, 101, 103, 5, 19, 10, 2, 102, 100, 3, 2, 2, 2, 102, 101, 3, 2, 2, 2, 103, 104, 3, 2, 2, 2, 104, 102, 3, 2, 2, 2, 104, 105, 3, 2, 2, 2, 105, 18, 3, 2, 2, 2, 106, 110, 5, 21, 11, 2, 107, 110, 5, 23, 12, 2, 108, 110, 5, 25, 13, 2, 109, 106, 3, 2, 2, 2, 109, 107, 3, 2, 2, 2, 109, 108, 3, 2, 2, 2, 110, 20, 3, 2, 2, 2, 111, 112, 7, 94, 2, 2, 112, 113, 10, 5, 2, 2, 113, 22, 3, 2, 2, 2, 114, 115, 7, 94, 2, 2, 115, 121, 7, 118, 2, 2, 116, 117, 7, 94, 2, 2, 117, 121, 7, 116, 2, 2, 118, 119, 7, 94, 2, 2, 119, 121, 7, 112, 2, 2, 120, 114, 3, 2, 2, 2, 120, 116, 3, 2, 2, 2, 120, 118, 3, 2, 2, 2, 121, 24, 3, 2, 2, 2, 122, 123, 7, 94, 2, 2, 123, 124, 7, 61, 2, 2, 124, 26, 3, 2, 2, 2, 125, 131, 7, 36, 2, 2, 126, 130, 10, 6, 2, 2, 127, 130, 5, 19, 10, 2, 128, 130, 5, 29, 15, 2, 129, 126, 3, 2, 2, 2, 129, 127, 3, 2, 2, 2, 129, 128, 3, 2, 2, 2, 130, 133, 3, 2, 2, 2, 131, 129, 3, 2, 2, 2, 131, 132, 3, 2, 2, 2, 132, 134, 3, 2, 2, 2, 133, 131, 3, 2, 2, 2, 134, 135, 7, 36, 2, 2, 135, 28, 3, 2, 2, 2, 136, 142, 7, 94, 2, 2, 137, 139, 7, 15, 2, 2, 138, 140, 7, 12, 2, 2, 139, 138, 3, 2, 2, 2, 139, 140, 3, 2, 2, 2, 140, 143, 3, 2, 2, 2, 141, 143, 7, 12, 2, 2, 142, 137, 3, 2, 2, 2, 142, 141, 3, 2, 2, 2, 143, 30, 3, 2, 2, 2, 144, 145, 7, 93, 2, 2, 145, 146, 5, 33, 17, 2, 146, 147, 7, 95, 2, 2, 147, 32, 3, 2, 2, 2, 148, 149, 7, 63, 2, 2, 149, 150, 5, 33, 17, 2, 150, 151, 7, 63, 2, 2, 151, 161, 3, 2, 2, 2, 152, 156, 7, 93, 2, 2, 153, 155, 11, 2, 2, 2, 154, 153, 3, 2, 2, 2, 155, 158, 3, 2, 2, 2, 156, 157, 3, 2, 2, 2, 156, 154, 3, 2, 2, 2, 157, 159, 3, 2, 2, 2, 158, 156, 3, 2, 2, 2, 159, 161, 7, 95, 2, 2, 160, 148, 3, 2, 2, 2, 160, 152, 3, 2, 2, 2, 161, 34, 3, 2, 2, 2, 162, 163, 7, 37, 2, 2, 163, 164, 7, 93, 2, 2, 164, 165, 3, 2, 2, 2, 165, 166, 5, 33, 17, 2, 166, 167, 7, 95, 2, 2, 167, 168, 3, 2, 2, 2, 168, 169, 8, 18, 2, 2, 169, 36, 3, 2, 2, 2, 170, 200, 7, 37, 2, 2, 171, 201, 3, 2, 2, 2, 172, 176, 7, 93, 2, 2, 173, 175, 7, 63, 2, 2, 174, 173, 3, 2, 2, 2, 175, 178, 3, 2, 2, 2, 176, 174, 3, 2, 2, 2, 176, 177, 3, 2, 2, 2, 177, 201, 3, 2, 2, 2, 178, 176, 3, 2, 2, 2, 179, 183, 7, 93, 2, 2, 180, 182, 7, 63, 2, 2, 181, 180, 3, 2, 2, 2, 182, 185, 3, 2, 2, 2, 183, 181, 3, 2, 2, 2, 183, 184, 3, 2, 2, 2, 184, 186, 3, 2, 2, 2, 185, 183, 3, 2, 2, 2, 186, 190, 10, 7, 2, 2, 187, 189, 10, 8, 2, 2, 188, 187, 3, 2, 2, 2, 189, 192, 3, 2, 2, 2, 190, 188, 3, 2, 2, 2, 190, 191, 3, 2, 2, 2, 191, 201, 3, 2, 2, 2, 192, 190, 3, 2, 2, 2, 193, 197, 10, 9, 2, 2, 194, 196, 10, 8, 2, 2, 195, 194, 3, 2, 2, 2, 196, 199, 3, 2, 2, 2, 197, 195, 3, 2, 2, 2, 197, 198, 3, 2, 2, 2, 198, 201, 3, 2, 2, 2, 199, 197, 3, 2, 2, 2, 200, 171, 3, 2, 2, 2, 200, 172, 3, 2, 2, 2, 200, 179, 3, 2, 2, 2, 200, 193, 3, 2, 2, 2, 201, 207, 3, 2, 2, 2, 202, 204, 7, 15, 2, 2, 203, 205, 7, 12, 2, 2, 204, 203, 3, 2, 2, 2, 204, 205, 3, 2, 2, 2, 205, 208, 3, 2, 2, 2, 206, 208, 9, 10, 2, 2, 207, 202, 3, 2, 2, 2, 207, 206, 3, 2, 2, 2, 208, 209, 3, 2, 2, 2, 209, 210, 8, 19, 2, 2, 210, 38, 3, 2, 2, 2, 211, 213, 7, 15, 2, 2, 212, 214, 7, 12, 2, 2, 213, 212, 3, 2, 2, 2, 213, 214, 3, 2, 2, 2, 214, 217, 3, 2, 2, 2, 215, 217, 7, 12, 2, 2, 216, 211, 3, 2, 2, 2, 216, 215, 3, 2, 2, 2, 217, 218, 3, 2, 2, 2, 218, 216, 3, 2, 2, 2, 218, 219, 3, 2, 2, 2, 219, 220, 3, 2, 2, 2, 220, 221, 8, 20, 2, 2, 221, 40, 3, 2, 2, 2, 222, 224, 9, 11, 2, 2, 223, 222, 3, 2, 2, 2, 224, 225, 3, 2, 2, 2, 225, 223, 3, 2, 2, 2, 225, 226, 3, 2, 2, 2, 226, 227, 3, 2, 2, 2, 227, 228, 8, 21, 2, 2, 228, 42, 3, 2, 2, 2, 30, 2, 49, 62, 67, 74, 79, 97, 102, 104, 109, 120, 129, 131, 139, 142, 156, 160, 176, 183, 190, 197, 200, 204, 207, 213, 216, 218, 225, 3, 8, 2, 2]
```

### Comparing `CMinx-1.1.8/src/cminx/parser/CMakeLexer.py` & `CMinx-1.1.9/src/cminx/parser/CMakeLexer.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,115 +4,115 @@
 from typing.io import TextIO
 import sys
 
 
 def serializedATN():
     with StringIO() as buf:
         buf.write("\3\u608b\ua72a\u8133\ub9ed\u417c\u3be7\u7786\u5964\2\21")
-        buf.write("\u00e6\b\1\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7")
+        buf.write("\u00e5\b\1\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7")
         buf.write("\t\7\4\b\t\b\4\t\t\t\4\n\t\n\4\13\t\13\4\f\t\f\4\r\t\r")
         buf.write("\4\16\t\16\4\17\t\17\4\20\t\20\4\21\t\21\4\22\t\22\4\23")
         buf.write("\t\23\4\24\t\24\4\25\t\25\3\2\3\2\3\3\3\3\3\4\3\4\5\4")
         buf.write("\62\n\4\3\4\3\4\3\4\3\4\3\4\3\4\3\4\3\4\3\4\3\4\3\4\5")
-        buf.write("\4?\n\4\3\4\7\4B\n\4\f\4\16\4E\13\4\3\4\3\4\3\4\3\4\3")
-        buf.write("\5\3\5\7\5M\n\5\f\5\16\5P\13\5\3\5\3\5\3\5\3\5\3\6\3\6")
-        buf.write("\3\6\3\6\3\6\3\7\3\7\3\7\3\7\3\b\3\b\7\ba\n\b\f\b\16\b")
-        buf.write("d\13\b\3\t\3\t\6\th\n\t\r\t\16\ti\3\n\3\n\3\n\5\no\n\n")
-        buf.write("\3\13\3\13\3\13\3\f\3\f\3\f\3\f\3\f\3\f\5\fz\n\f\3\r\3")
-        buf.write("\r\3\r\3\16\3\16\3\16\3\16\7\16\u0083\n\16\f\16\16\16")
-        buf.write("\u0086\13\16\3\16\3\16\3\17\3\17\3\17\5\17\u008d\n\17")
-        buf.write("\3\17\5\17\u0090\n\17\3\20\3\20\3\20\3\20\3\21\3\21\3")
-        buf.write("\21\3\21\3\21\3\21\7\21\u009c\n\21\f\21\16\21\u009f\13")
-        buf.write("\21\3\21\5\21\u00a2\n\21\3\22\3\22\3\22\3\22\3\22\3\22")
-        buf.write("\3\22\3\22\3\23\3\23\3\23\3\23\7\23\u00b0\n\23\f\23\16")
-        buf.write("\23\u00b3\13\23\3\23\3\23\7\23\u00b7\n\23\f\23\16\23\u00ba")
-        buf.write("\13\23\3\23\3\23\7\23\u00be\n\23\f\23\16\23\u00c1\13\23")
-        buf.write("\3\23\3\23\7\23\u00c5\n\23\f\23\16\23\u00c8\13\23\5\23")
-        buf.write("\u00ca\n\23\3\23\3\23\5\23\u00ce\n\23\3\23\5\23\u00d1")
-        buf.write("\n\23\3\23\3\23\3\24\3\24\5\24\u00d7\n\24\3\24\6\24\u00da")
-        buf.write("\n\24\r\24\16\24\u00db\3\24\3\24\3\25\6\25\u00e1\n\25")
-        buf.write("\r\25\16\25\u00e2\3\25\3\25\5CN\u009d\2\26\3\3\5\4\7\5")
+        buf.write("\4?\n\4\3\4\7\4B\n\4\f\4\16\4E\13\4\3\4\3\4\3\5\3\5\5")
+        buf.write("\5K\n\5\3\5\7\5N\n\5\f\5\16\5Q\13\5\3\5\3\5\3\6\3\6\3")
+        buf.write("\6\3\6\3\6\3\7\3\7\3\7\3\7\3\b\3\b\7\b`\n\b\f\b\16\bc")
+        buf.write("\13\b\3\t\3\t\6\tg\n\t\r\t\16\th\3\n\3\n\3\n\5\nn\n\n")
+        buf.write("\3\13\3\13\3\13\3\f\3\f\3\f\3\f\3\f\3\f\5\fy\n\f\3\r\3")
+        buf.write("\r\3\r\3\16\3\16\3\16\3\16\7\16\u0082\n\16\f\16\16\16")
+        buf.write("\u0085\13\16\3\16\3\16\3\17\3\17\3\17\5\17\u008c\n\17")
+        buf.write("\3\17\5\17\u008f\n\17\3\20\3\20\3\20\3\20\3\21\3\21\3")
+        buf.write("\21\3\21\3\21\3\21\7\21\u009b\n\21\f\21\16\21\u009e\13")
+        buf.write("\21\3\21\5\21\u00a1\n\21\3\22\3\22\3\22\3\22\3\22\3\22")
+        buf.write("\3\22\3\22\3\23\3\23\3\23\3\23\7\23\u00af\n\23\f\23\16")
+        buf.write("\23\u00b2\13\23\3\23\3\23\7\23\u00b6\n\23\f\23\16\23\u00b9")
+        buf.write("\13\23\3\23\3\23\7\23\u00bd\n\23\f\23\16\23\u00c0\13\23")
+        buf.write("\3\23\3\23\7\23\u00c4\n\23\f\23\16\23\u00c7\13\23\5\23")
+        buf.write("\u00c9\n\23\3\23\3\23\5\23\u00cd\n\23\3\23\5\23\u00d0")
+        buf.write("\n\23\3\23\3\23\3\24\3\24\5\24\u00d6\n\24\3\24\6\24\u00d9")
+        buf.write("\n\24\r\24\16\24\u00da\3\24\3\24\3\25\6\25\u00e0\n\25")
+        buf.write("\r\25\16\25\u00e1\3\25\3\25\5CO\u009c\2\26\3\3\5\4\7\5")
         buf.write("\t\6\13\7\r\b\17\t\21\n\23\13\25\2\27\2\31\2\33\f\35\2")
         buf.write("\37\r!\2#\16%\17\'\20)\21\3\2\f\5\2C\\aac|\6\2\62;C\\")
         buf.write("aac|\b\2\13\f\17\17\"\"$%*+^^\6\2\62;==C\\c|\4\2$$^^\6")
         buf.write("\2\f\f\17\17??]]\4\2\f\f\17\17\5\2\f\f\17\17]]\3\3\f\f")
         buf.write("\4\2\13\13\"\"\2\u00ff\2\3\3\2\2\2\2\5\3\2\2\2\2\7\3\2")
         buf.write("\2\2\2\t\3\2\2\2\2\13\3\2\2\2\2\r\3\2\2\2\2\17\3\2\2\2")
         buf.write("\2\21\3\2\2\2\2\23\3\2\2\2\2\33\3\2\2\2\2\37\3\2\2\2\2")
         buf.write("#\3\2\2\2\2%\3\2\2\2\2\'\3\2\2\2\2)\3\2\2\2\3+\3\2\2\2")
-        buf.write("\5-\3\2\2\2\7/\3\2\2\2\tJ\3\2\2\2\13U\3\2\2\2\rZ\3\2\2")
-        buf.write("\2\17^\3\2\2\2\21g\3\2\2\2\23n\3\2\2\2\25p\3\2\2\2\27")
-        buf.write("y\3\2\2\2\31{\3\2\2\2\33~\3\2\2\2\35\u0089\3\2\2\2\37")
-        buf.write("\u0091\3\2\2\2!\u00a1\3\2\2\2#\u00a3\3\2\2\2%\u00ab\3")
-        buf.write("\2\2\2\'\u00d9\3\2\2\2)\u00e0\3\2\2\2+,\7*\2\2,\4\3\2")
+        buf.write("\5-\3\2\2\2\7/\3\2\2\2\tH\3\2\2\2\13T\3\2\2\2\rY\3\2\2")
+        buf.write("\2\17]\3\2\2\2\21f\3\2\2\2\23m\3\2\2\2\25o\3\2\2\2\27")
+        buf.write("x\3\2\2\2\31z\3\2\2\2\33}\3\2\2\2\35\u0088\3\2\2\2\37")
+        buf.write("\u0090\3\2\2\2!\u00a0\3\2\2\2#\u00a2\3\2\2\2%\u00aa\3")
+        buf.write("\2\2\2\'\u00d8\3\2\2\2)\u00df\3\2\2\2+,\7*\2\2,\4\3\2")
         buf.write("\2\2-.\7+\2\2.\6\3\2\2\2/\61\5\13\6\2\60\62\5)\25\2\61")
         buf.write("\60\3\2\2\2\61\62\3\2\2\2\62\63\3\2\2\2\63\64\7B\2\2\64")
         buf.write("\65\7o\2\2\65\66\7q\2\2\66\67\7f\2\2\678\7w\2\289\7n\2")
         buf.write("\29:\7g\2\2:>\3\2\2\2;<\5)\25\2<=\5\21\t\2=?\3\2\2\2>")
         buf.write(";\3\2\2\2>?\3\2\2\2?C\3\2\2\2@B\13\2\2\2A@\3\2\2\2BE\3")
-        buf.write("\2\2\2CD\3\2\2\2CA\3\2\2\2DF\3\2\2\2EC\3\2\2\2FG\7%\2")
-        buf.write("\2GH\7_\2\2HI\7_\2\2I\b\3\2\2\2JN\5\13\6\2KM\13\2\2\2")
-        buf.write("LK\3\2\2\2MP\3\2\2\2NO\3\2\2\2NL\3\2\2\2OQ\3\2\2\2PN\3")
-        buf.write("\2\2\2QR\7%\2\2RS\7_\2\2ST\7_\2\2T\n\3\2\2\2UV\7%\2\2")
-        buf.write("VW\7]\2\2WX\7]\2\2XY\7]\2\2Y\f\3\2\2\2Z[\7%\2\2[\\\7_")
-        buf.write("\2\2\\]\7_\2\2]\16\3\2\2\2^b\t\2\2\2_a\t\3\2\2`_\3\2\2")
-        buf.write("\2ad\3\2\2\2b`\3\2\2\2bc\3\2\2\2c\20\3\2\2\2db\3\2\2\2")
-        buf.write("eh\n\4\2\2fh\5\23\n\2ge\3\2\2\2gf\3\2\2\2hi\3\2\2\2ig")
-        buf.write("\3\2\2\2ij\3\2\2\2j\22\3\2\2\2ko\5\25\13\2lo\5\27\f\2")
-        buf.write("mo\5\31\r\2nk\3\2\2\2nl\3\2\2\2nm\3\2\2\2o\24\3\2\2\2")
-        buf.write("pq\7^\2\2qr\n\5\2\2r\26\3\2\2\2st\7^\2\2tz\7v\2\2uv\7")
-        buf.write("^\2\2vz\7t\2\2wx\7^\2\2xz\7p\2\2ys\3\2\2\2yu\3\2\2\2y")
-        buf.write("w\3\2\2\2z\30\3\2\2\2{|\7^\2\2|}\7=\2\2}\32\3\2\2\2~\u0084")
-        buf.write("\7$\2\2\177\u0083\n\6\2\2\u0080\u0083\5\23\n\2\u0081\u0083")
-        buf.write("\5\35\17\2\u0082\177\3\2\2\2\u0082\u0080\3\2\2\2\u0082")
-        buf.write("\u0081\3\2\2\2\u0083\u0086\3\2\2\2\u0084\u0082\3\2\2\2")
-        buf.write("\u0084\u0085\3\2\2\2\u0085\u0087\3\2\2\2\u0086\u0084\3")
-        buf.write("\2\2\2\u0087\u0088\7$\2\2\u0088\34\3\2\2\2\u0089\u008f")
-        buf.write("\7^\2\2\u008a\u008c\7\17\2\2\u008b\u008d\7\f\2\2\u008c")
-        buf.write("\u008b\3\2\2\2\u008c\u008d\3\2\2\2\u008d\u0090\3\2\2\2")
-        buf.write("\u008e\u0090\7\f\2\2\u008f\u008a\3\2\2\2\u008f\u008e\3")
-        buf.write("\2\2\2\u0090\36\3\2\2\2\u0091\u0092\7]\2\2\u0092\u0093")
-        buf.write("\5!\21\2\u0093\u0094\7_\2\2\u0094 \3\2\2\2\u0095\u0096")
-        buf.write("\7?\2\2\u0096\u0097\5!\21\2\u0097\u0098\7?\2\2\u0098\u00a2")
-        buf.write("\3\2\2\2\u0099\u009d\7]\2\2\u009a\u009c\13\2\2\2\u009b")
-        buf.write("\u009a\3\2\2\2\u009c\u009f\3\2\2\2\u009d\u009e\3\2\2\2")
-        buf.write("\u009d\u009b\3\2\2\2\u009e\u00a0\3\2\2\2\u009f\u009d\3")
-        buf.write("\2\2\2\u00a0\u00a2\7_\2\2\u00a1\u0095\3\2\2\2\u00a1\u0099")
-        buf.write("\3\2\2\2\u00a2\"\3\2\2\2\u00a3\u00a4\7%\2\2\u00a4\u00a5")
-        buf.write("\7]\2\2\u00a5\u00a6\3\2\2\2\u00a6\u00a7\5!\21\2\u00a7")
-        buf.write("\u00a8\7_\2\2\u00a8\u00a9\3\2\2\2\u00a9\u00aa\b\22\2\2")
-        buf.write("\u00aa$\3\2\2\2\u00ab\u00c9\7%\2\2\u00ac\u00ca\3\2\2\2")
-        buf.write("\u00ad\u00b1\7]\2\2\u00ae\u00b0\7?\2\2\u00af\u00ae\3\2")
-        buf.write("\2\2\u00b0\u00b3\3\2\2\2\u00b1\u00af\3\2\2\2\u00b1\u00b2")
-        buf.write("\3\2\2\2\u00b2\u00ca\3\2\2\2\u00b3\u00b1\3\2\2\2\u00b4")
-        buf.write("\u00b8\7]\2\2\u00b5\u00b7\7?\2\2\u00b6\u00b5\3\2\2\2\u00b7")
-        buf.write("\u00ba\3\2\2\2\u00b8\u00b6\3\2\2\2\u00b8\u00b9\3\2\2\2")
-        buf.write("\u00b9\u00bb\3\2\2\2\u00ba\u00b8\3\2\2\2\u00bb\u00bf\n")
-        buf.write("\7\2\2\u00bc\u00be\n\b\2\2\u00bd\u00bc\3\2\2\2\u00be\u00c1")
-        buf.write("\3\2\2\2\u00bf\u00bd\3\2\2\2\u00bf\u00c0\3\2\2\2\u00c0")
-        buf.write("\u00ca\3\2\2\2\u00c1\u00bf\3\2\2\2\u00c2\u00c6\n\t\2\2")
-        buf.write("\u00c3\u00c5\n\b\2\2\u00c4\u00c3\3\2\2\2\u00c5\u00c8\3")
-        buf.write("\2\2\2\u00c6\u00c4\3\2\2\2\u00c6\u00c7\3\2\2\2\u00c7\u00ca")
-        buf.write("\3\2\2\2\u00c8\u00c6\3\2\2\2\u00c9\u00ac\3\2\2\2\u00c9")
-        buf.write("\u00ad\3\2\2\2\u00c9\u00b4\3\2\2\2\u00c9\u00c2\3\2\2\2")
-        buf.write("\u00ca\u00d0\3\2\2\2\u00cb\u00cd\7\17\2\2\u00cc\u00ce")
-        buf.write("\7\f\2\2\u00cd\u00cc\3\2\2\2\u00cd\u00ce\3\2\2\2\u00ce")
-        buf.write("\u00d1\3\2\2\2\u00cf\u00d1\t\n\2\2\u00d0\u00cb\3\2\2\2")
-        buf.write("\u00d0\u00cf\3\2\2\2\u00d1\u00d2\3\2\2\2\u00d2\u00d3\b")
-        buf.write("\23\2\2\u00d3&\3\2\2\2\u00d4\u00d6\7\17\2\2\u00d5\u00d7")
-        buf.write("\7\f\2\2\u00d6\u00d5\3\2\2\2\u00d6\u00d7\3\2\2\2\u00d7")
-        buf.write("\u00da\3\2\2\2\u00d8\u00da\7\f\2\2\u00d9\u00d4\3\2\2\2")
-        buf.write("\u00d9\u00d8\3\2\2\2\u00da\u00db\3\2\2\2\u00db\u00d9\3")
-        buf.write("\2\2\2\u00db\u00dc\3\2\2\2\u00dc\u00dd\3\2\2\2\u00dd\u00de")
-        buf.write("\b\24\2\2\u00de(\3\2\2\2\u00df\u00e1\t\13\2\2\u00e0\u00df")
-        buf.write("\3\2\2\2\u00e1\u00e2\3\2\2\2\u00e2\u00e0\3\2\2\2\u00e2")
-        buf.write("\u00e3\3\2\2\2\u00e3\u00e4\3\2\2\2\u00e4\u00e5\b\25\2")
-        buf.write("\2\u00e5*\3\2\2\2\35\2\61>CNbginy\u0082\u0084\u008c\u008f")
-        buf.write("\u009d\u00a1\u00b1\u00b8\u00bf\u00c6\u00c9\u00cd\u00d0")
-        buf.write("\u00d6\u00d9\u00db\u00e2\3\b\2\2")
+        buf.write("\2\2\2CD\3\2\2\2CA\3\2\2\2DF\3\2\2\2EC\3\2\2\2FG\5\r\7")
+        buf.write("\2G\b\3\2\2\2HJ\5\13\6\2IK\5)\25\2JI\3\2\2\2JK\3\2\2\2")
+        buf.write("KO\3\2\2\2LN\13\2\2\2ML\3\2\2\2NQ\3\2\2\2OP\3\2\2\2OM")
+        buf.write("\3\2\2\2PR\3\2\2\2QO\3\2\2\2RS\5\r\7\2S\n\3\2\2\2TU\7")
+        buf.write("%\2\2UV\7]\2\2VW\7]\2\2WX\7]\2\2X\f\3\2\2\2YZ\7%\2\2Z")
+        buf.write("[\7_\2\2[\\\7_\2\2\\\16\3\2\2\2]a\t\2\2\2^`\t\3\2\2_^")
+        buf.write("\3\2\2\2`c\3\2\2\2a_\3\2\2\2ab\3\2\2\2b\20\3\2\2\2ca\3")
+        buf.write("\2\2\2dg\n\4\2\2eg\5\23\n\2fd\3\2\2\2fe\3\2\2\2gh\3\2")
+        buf.write("\2\2hf\3\2\2\2hi\3\2\2\2i\22\3\2\2\2jn\5\25\13\2kn\5\27")
+        buf.write("\f\2ln\5\31\r\2mj\3\2\2\2mk\3\2\2\2ml\3\2\2\2n\24\3\2")
+        buf.write("\2\2op\7^\2\2pq\n\5\2\2q\26\3\2\2\2rs\7^\2\2sy\7v\2\2")
+        buf.write("tu\7^\2\2uy\7t\2\2vw\7^\2\2wy\7p\2\2xr\3\2\2\2xt\3\2\2")
+        buf.write("\2xv\3\2\2\2y\30\3\2\2\2z{\7^\2\2{|\7=\2\2|\32\3\2\2\2")
+        buf.write("}\u0083\7$\2\2~\u0082\n\6\2\2\177\u0082\5\23\n\2\u0080")
+        buf.write("\u0082\5\35\17\2\u0081~\3\2\2\2\u0081\177\3\2\2\2\u0081")
+        buf.write("\u0080\3\2\2\2\u0082\u0085\3\2\2\2\u0083\u0081\3\2\2\2")
+        buf.write("\u0083\u0084\3\2\2\2\u0084\u0086\3\2\2\2\u0085\u0083\3")
+        buf.write("\2\2\2\u0086\u0087\7$\2\2\u0087\34\3\2\2\2\u0088\u008e")
+        buf.write("\7^\2\2\u0089\u008b\7\17\2\2\u008a\u008c\7\f\2\2\u008b")
+        buf.write("\u008a\3\2\2\2\u008b\u008c\3\2\2\2\u008c\u008f\3\2\2\2")
+        buf.write("\u008d\u008f\7\f\2\2\u008e\u0089\3\2\2\2\u008e\u008d\3")
+        buf.write("\2\2\2\u008f\36\3\2\2\2\u0090\u0091\7]\2\2\u0091\u0092")
+        buf.write("\5!\21\2\u0092\u0093\7_\2\2\u0093 \3\2\2\2\u0094\u0095")
+        buf.write("\7?\2\2\u0095\u0096\5!\21\2\u0096\u0097\7?\2\2\u0097\u00a1")
+        buf.write("\3\2\2\2\u0098\u009c\7]\2\2\u0099\u009b\13\2\2\2\u009a")
+        buf.write("\u0099\3\2\2\2\u009b\u009e\3\2\2\2\u009c\u009d\3\2\2\2")
+        buf.write("\u009c\u009a\3\2\2\2\u009d\u009f\3\2\2\2\u009e\u009c\3")
+        buf.write("\2\2\2\u009f\u00a1\7_\2\2\u00a0\u0094\3\2\2\2\u00a0\u0098")
+        buf.write("\3\2\2\2\u00a1\"\3\2\2\2\u00a2\u00a3\7%\2\2\u00a3\u00a4")
+        buf.write("\7]\2\2\u00a4\u00a5\3\2\2\2\u00a5\u00a6\5!\21\2\u00a6")
+        buf.write("\u00a7\7_\2\2\u00a7\u00a8\3\2\2\2\u00a8\u00a9\b\22\2\2")
+        buf.write("\u00a9$\3\2\2\2\u00aa\u00c8\7%\2\2\u00ab\u00c9\3\2\2\2")
+        buf.write("\u00ac\u00b0\7]\2\2\u00ad\u00af\7?\2\2\u00ae\u00ad\3\2")
+        buf.write("\2\2\u00af\u00b2\3\2\2\2\u00b0\u00ae\3\2\2\2\u00b0\u00b1")
+        buf.write("\3\2\2\2\u00b1\u00c9\3\2\2\2\u00b2\u00b0\3\2\2\2\u00b3")
+        buf.write("\u00b7\7]\2\2\u00b4\u00b6\7?\2\2\u00b5\u00b4\3\2\2\2\u00b6")
+        buf.write("\u00b9\3\2\2\2\u00b7\u00b5\3\2\2\2\u00b7\u00b8\3\2\2\2")
+        buf.write("\u00b8\u00ba\3\2\2\2\u00b9\u00b7\3\2\2\2\u00ba\u00be\n")
+        buf.write("\7\2\2\u00bb\u00bd\n\b\2\2\u00bc\u00bb\3\2\2\2\u00bd\u00c0")
+        buf.write("\3\2\2\2\u00be\u00bc\3\2\2\2\u00be\u00bf\3\2\2\2\u00bf")
+        buf.write("\u00c9\3\2\2\2\u00c0\u00be\3\2\2\2\u00c1\u00c5\n\t\2\2")
+        buf.write("\u00c2\u00c4\n\b\2\2\u00c3\u00c2\3\2\2\2\u00c4\u00c7\3")
+        buf.write("\2\2\2\u00c5\u00c3\3\2\2\2\u00c5\u00c6\3\2\2\2\u00c6\u00c9")
+        buf.write("\3\2\2\2\u00c7\u00c5\3\2\2\2\u00c8\u00ab\3\2\2\2\u00c8")
+        buf.write("\u00ac\3\2\2\2\u00c8\u00b3\3\2\2\2\u00c8\u00c1\3\2\2\2")
+        buf.write("\u00c9\u00cf\3\2\2\2\u00ca\u00cc\7\17\2\2\u00cb\u00cd")
+        buf.write("\7\f\2\2\u00cc\u00cb\3\2\2\2\u00cc\u00cd\3\2\2\2\u00cd")
+        buf.write("\u00d0\3\2\2\2\u00ce\u00d0\t\n\2\2\u00cf\u00ca\3\2\2\2")
+        buf.write("\u00cf\u00ce\3\2\2\2\u00d0\u00d1\3\2\2\2\u00d1\u00d2\b")
+        buf.write("\23\2\2\u00d2&\3\2\2\2\u00d3\u00d5\7\17\2\2\u00d4\u00d6")
+        buf.write("\7\f\2\2\u00d5\u00d4\3\2\2\2\u00d5\u00d6\3\2\2\2\u00d6")
+        buf.write("\u00d9\3\2\2\2\u00d7\u00d9\7\f\2\2\u00d8\u00d3\3\2\2\2")
+        buf.write("\u00d8\u00d7\3\2\2\2\u00d9\u00da\3\2\2\2\u00da\u00d8\3")
+        buf.write("\2\2\2\u00da\u00db\3\2\2\2\u00db\u00dc\3\2\2\2\u00dc\u00dd")
+        buf.write("\b\24\2\2\u00dd(\3\2\2\2\u00de\u00e0\t\13\2\2\u00df\u00de")
+        buf.write("\3\2\2\2\u00e0\u00e1\3\2\2\2\u00e1\u00df\3\2\2\2\u00e1")
+        buf.write("\u00e2\3\2\2\2\u00e2\u00e3\3\2\2\2\u00e3\u00e4\b\25\2")
+        buf.write("\2\u00e4*\3\2\2\2\36\2\61>CJOafhmx\u0081\u0083\u008b\u008e")
+        buf.write("\u009c\u00a0\u00b0\u00b7\u00be\u00c5\u00c8\u00cc\u00cf")
+        buf.write("\u00d5\u00d8\u00da\u00e1\3\b\2\2")
         return buf.getvalue()
 
 
 class CMakeLexer(Lexer):
 
     atn = ATNDeserializer().deserialize(serializedATN())
```

### Comparing `CMinx-1.1.8/src/cminx/parser/CMakeListener.py` & `CMinx-1.1.9/src/cminx/parser/CMakeListener.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/src/cminx/parser/CMakeParser.py` & `CMinx-1.1.9/src/cminx/parser/CMakeParser.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 from io import StringIO
 from typing.io import TextIO
 import sys
 
 def serializedATN():
     with StringIO() as buf:
         buf.write("\3\u608b\ua72a\u8133\ub9ed\u417c\u3be7\u7786\u5964\3\21")
-        buf.write(";\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7\t\7\4\b")
-        buf.write("\t\b\3\2\5\2\22\n\2\3\2\3\2\7\2\26\n\2\f\2\16\2\31\13")
-        buf.write("\2\3\2\3\2\3\3\3\3\3\3\3\4\3\4\3\5\3\5\3\6\3\6\3\6\3\6")
-        buf.write("\7\6(\n\6\f\6\16\6+\13\6\3\6\3\6\3\7\3\7\3\b\3\b\3\b\7")
-        buf.write("\b\64\n\b\f\b\16\b\67\13\b\3\b\3\b\3\b\2\2\t\2\4\6\b\n")
-        buf.write("\f\16\2\3\4\2\t\n\f\r\2:\2\21\3\2\2\2\4\34\3\2\2\2\6\37")
-        buf.write("\3\2\2\2\b!\3\2\2\2\n#\3\2\2\2\f.\3\2\2\2\16\60\3\2\2")
-        buf.write("\2\20\22\5\6\4\2\21\20\3\2\2\2\21\22\3\2\2\2\22\27\3\2")
-        buf.write("\2\2\23\26\5\4\3\2\24\26\5\n\6\2\25\23\3\2\2\2\25\24\3")
-        buf.write("\2\2\2\26\31\3\2\2\2\27\25\3\2\2\2\27\30\3\2\2\2\30\32")
-        buf.write("\3\2\2\2\31\27\3\2\2\2\32\33\7\2\2\3\33\3\3\2\2\2\34\35")
-        buf.write("\5\b\5\2\35\36\5\n\6\2\36\5\3\2\2\2\37 \7\5\2\2 \7\3\2")
-        buf.write("\2\2!\"\7\6\2\2\"\t\3\2\2\2#$\7\t\2\2$)\7\3\2\2%(\5\f")
-        buf.write("\7\2&(\5\16\b\2\'%\3\2\2\2\'&\3\2\2\2(+\3\2\2\2)\'\3\2")
-        buf.write("\2\2)*\3\2\2\2*,\3\2\2\2+)\3\2\2\2,-\7\4\2\2-\13\3\2\2")
-        buf.write("\2./\t\2\2\2/\r\3\2\2\2\60\65\7\3\2\2\61\64\5\f\7\2\62")
-        buf.write("\64\5\16\b\2\63\61\3\2\2\2\63\62\3\2\2\2\64\67\3\2\2\2")
-        buf.write("\65\63\3\2\2\2\65\66\3\2\2\2\668\3\2\2\2\67\65\3\2\2\2")
-        buf.write("89\7\4\2\29\17\3\2\2\2\t\21\25\27\')\63\65")
+        buf.write("<\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7\t\7\4\b")
+        buf.write("\t\b\3\2\5\2\22\n\2\3\2\3\2\3\2\7\2\27\n\2\f\2\16\2\32")
+        buf.write("\13\2\3\2\3\2\3\3\3\3\3\3\3\4\3\4\3\5\3\5\3\6\3\6\3\6")
+        buf.write("\3\6\7\6)\n\6\f\6\16\6,\13\6\3\6\3\6\3\7\3\7\3\b\3\b\3")
+        buf.write("\b\7\b\65\n\b\f\b\16\b8\13\b\3\b\3\b\3\b\2\2\t\2\4\6\b")
+        buf.write("\n\f\16\2\3\4\2\t\n\f\r\2<\2\21\3\2\2\2\4\35\3\2\2\2\6")
+        buf.write(" \3\2\2\2\b\"\3\2\2\2\n$\3\2\2\2\f/\3\2\2\2\16\61\3\2")
+        buf.write("\2\2\20\22\5\6\4\2\21\20\3\2\2\2\21\22\3\2\2\2\22\30\3")
+        buf.write("\2\2\2\23\27\5\4\3\2\24\27\5\n\6\2\25\27\5\b\5\2\26\23")
+        buf.write("\3\2\2\2\26\24\3\2\2\2\26\25\3\2\2\2\27\32\3\2\2\2\30")
+        buf.write("\26\3\2\2\2\30\31\3\2\2\2\31\33\3\2\2\2\32\30\3\2\2\2")
+        buf.write("\33\34\7\2\2\3\34\3\3\2\2\2\35\36\5\b\5\2\36\37\5\n\6")
+        buf.write("\2\37\5\3\2\2\2 !\7\5\2\2!\7\3\2\2\2\"#\7\6\2\2#\t\3\2")
+        buf.write("\2\2$%\7\t\2\2%*\7\3\2\2&)\5\f\7\2\')\5\16\b\2(&\3\2\2")
+        buf.write("\2(\'\3\2\2\2),\3\2\2\2*(\3\2\2\2*+\3\2\2\2+-\3\2\2\2")
+        buf.write(",*\3\2\2\2-.\7\4\2\2.\13\3\2\2\2/\60\t\2\2\2\60\r\3\2")
+        buf.write("\2\2\61\66\7\3\2\2\62\65\5\f\7\2\63\65\5\16\b\2\64\62")
+        buf.write("\3\2\2\2\64\63\3\2\2\2\658\3\2\2\2\66\64\3\2\2\2\66\67")
+        buf.write("\3\2\2\2\679\3\2\2\28\66\3\2\2\29:\7\4\2\2:\17\3\2\2\2")
+        buf.write("\t\21\26\30(*\64\66")
         return buf.getvalue()
 
 
 class CMakeParser ( Parser ):
 
     grammarFileName = "CMake.g4"
 
@@ -109,31 +110,32 @@
         def command_invocation(self, i:int=None):
             if i is None:
                 return self.getTypedRuleContexts(CMakeParser.Command_invocationContext)
             else:
                 return self.getTypedRuleContext(CMakeParser.Command_invocationContext,i)
 
 
+        def bracket_doccomment(self, i:int=None):
+            if i is None:
+                return self.getTypedRuleContexts(CMakeParser.Bracket_doccommentContext)
+            else:
+                return self.getTypedRuleContext(CMakeParser.Bracket_doccommentContext,i)
+
+
         def getRuleIndex(self):
             return CMakeParser.RULE_cmake_file
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterCmake_file" ):
                 listener.enterCmake_file(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitCmake_file" ):
                 listener.exitCmake_file(self)
 
-        def accept(self, visitor:ParseTreeVisitor):
-            if hasattr( visitor, "visitCmake_file" ):
-                return visitor.visitCmake_file(self)
-            else:
-                return visitor.visitChildren(self)
-
 
 
 
     def cmake_file(self):
 
         localctx = CMakeParser.Cmake_fileContext(self, self._ctx, self.state)
         self.enterRule(localctx, 0, self.RULE_cmake_file)
@@ -144,37 +146,42 @@
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==CMakeParser.Module_docstring:
                 self.state = 14
                 self.documented_module()
 
 
-            self.state = 21
+            self.state = 22
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==CMakeParser.Docstring or _la==CMakeParser.Identifier:
-                self.state = 19
+                self.state = 20
                 self._errHandler.sync(self)
-                token = self._input.LA(1)
-                if token in [CMakeParser.Docstring]:
+                la_ = self._interp.adaptivePredict(self._input,1,self._ctx)
+                if la_ == 1:
                     self.state = 17
                     self.documented_command()
                     pass
-                elif token in [CMakeParser.Identifier]:
+
+                elif la_ == 2:
                     self.state = 18
                     self.command_invocation()
                     pass
-                else:
-                    raise NoViableAltException(self)
 
-                self.state = 23
+                elif la_ == 3:
+                    self.state = 19
+                    self.bracket_doccomment()
+                    pass
+
+
+                self.state = 24
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
-            self.state = 24
+            self.state = 25
             self.match(CMakeParser.EOF)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -201,32 +208,26 @@
             if hasattr( listener, "enterDocumented_command" ):
                 listener.enterDocumented_command(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitDocumented_command" ):
                 listener.exitDocumented_command(self)
 
-        def accept(self, visitor:ParseTreeVisitor):
-            if hasattr( visitor, "visitDocumented_command" ):
-                return visitor.visitDocumented_command(self)
-            else:
-                return visitor.visitChildren(self)
-
 
 
 
     def documented_command(self):
 
         localctx = CMakeParser.Documented_commandContext(self, self._ctx, self.state)
         self.enterRule(localctx, 2, self.RULE_documented_command)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 26
-            self.bracket_doccomment()
             self.state = 27
+            self.bracket_doccomment()
+            self.state = 28
             self.command_invocation()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -248,30 +249,24 @@
             if hasattr( listener, "enterDocumented_module" ):
                 listener.enterDocumented_module(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitDocumented_module" ):
                 listener.exitDocumented_module(self)
 
-        def accept(self, visitor:ParseTreeVisitor):
-            if hasattr( visitor, "visitDocumented_module" ):
-                return visitor.visitDocumented_module(self)
-            else:
-                return visitor.visitChildren(self)
-
 
 
 
     def documented_module(self):
 
         localctx = CMakeParser.Documented_moduleContext(self, self._ctx, self.state)
         self.enterRule(localctx, 4, self.RULE_documented_module)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 29
+            self.state = 30
             self.match(CMakeParser.Module_docstring)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -293,30 +288,24 @@
             if hasattr( listener, "enterBracket_doccomment" ):
                 listener.enterBracket_doccomment(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitBracket_doccomment" ):
                 listener.exitBracket_doccomment(self)
 
-        def accept(self, visitor:ParseTreeVisitor):
-            if hasattr( visitor, "visitBracket_doccomment" ):
-                return visitor.visitBracket_doccomment(self)
-            else:
-                return visitor.visitChildren(self)
-
 
 
 
     def bracket_doccomment(self):
 
         localctx = CMakeParser.Bracket_doccommentContext(self, self._ctx, self.state)
         self.enterRule(localctx, 6, self.RULE_bracket_doccomment)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 31
+            self.state = 32
             self.match(CMakeParser.Docstring)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -352,57 +341,51 @@
             if hasattr( listener, "enterCommand_invocation" ):
                 listener.enterCommand_invocation(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitCommand_invocation" ):
                 listener.exitCommand_invocation(self)
 
-        def accept(self, visitor:ParseTreeVisitor):
-            if hasattr( visitor, "visitCommand_invocation" ):
-                return visitor.visitCommand_invocation(self)
-            else:
-                return visitor.visitChildren(self)
-
 
 
 
     def command_invocation(self):
 
         localctx = CMakeParser.Command_invocationContext(self, self._ctx, self.state)
         self.enterRule(localctx, 8, self.RULE_command_invocation)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 33
-            self.match(CMakeParser.Identifier)
             self.state = 34
+            self.match(CMakeParser.Identifier)
+            self.state = 35
             self.match(CMakeParser.T__0)
-            self.state = 39
+            self.state = 40
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << CMakeParser.T__0) | (1 << CMakeParser.Identifier) | (1 << CMakeParser.Unquoted_argument) | (1 << CMakeParser.Quoted_argument) | (1 << CMakeParser.Bracket_argument))) != 0):
-                self.state = 37
+                self.state = 38
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
                 if token in [CMakeParser.Identifier, CMakeParser.Unquoted_argument, CMakeParser.Quoted_argument, CMakeParser.Bracket_argument]:
-                    self.state = 35
+                    self.state = 36
                     self.single_argument()
                     pass
                 elif token in [CMakeParser.T__0]:
-                    self.state = 36
+                    self.state = 37
                     self.compound_argument()
                     pass
                 else:
                     raise NoViableAltException(self)
 
-                self.state = 41
+                self.state = 42
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
-            self.state = 42
+            self.state = 43
             self.match(CMakeParser.T__1)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -433,31 +416,25 @@
             if hasattr( listener, "enterSingle_argument" ):
                 listener.enterSingle_argument(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitSingle_argument" ):
                 listener.exitSingle_argument(self)
 
-        def accept(self, visitor:ParseTreeVisitor):
-            if hasattr( visitor, "visitSingle_argument" ):
-                return visitor.visitSingle_argument(self)
-            else:
-                return visitor.visitChildren(self)
-
 
 
 
     def single_argument(self):
 
         localctx = CMakeParser.Single_argumentContext(self, self._ctx, self.state)
         self.enterRule(localctx, 10, self.RULE_single_argument)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 44
+            self.state = 45
             _la = self._input.LA(1)
             if not((((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << CMakeParser.Identifier) | (1 << CMakeParser.Unquoted_argument) | (1 << CMakeParser.Quoted_argument) | (1 << CMakeParser.Bracket_argument))) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
@@ -495,55 +472,49 @@
             if hasattr( listener, "enterCompound_argument" ):
                 listener.enterCompound_argument(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitCompound_argument" ):
                 listener.exitCompound_argument(self)
 
-        def accept(self, visitor:ParseTreeVisitor):
-            if hasattr( visitor, "visitCompound_argument" ):
-                return visitor.visitCompound_argument(self)
-            else:
-                return visitor.visitChildren(self)
-
 
 
 
     def compound_argument(self):
 
         localctx = CMakeParser.Compound_argumentContext(self, self._ctx, self.state)
         self.enterRule(localctx, 12, self.RULE_compound_argument)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 46
+            self.state = 47
             self.match(CMakeParser.T__0)
-            self.state = 51
+            self.state = 52
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << CMakeParser.T__0) | (1 << CMakeParser.Identifier) | (1 << CMakeParser.Unquoted_argument) | (1 << CMakeParser.Quoted_argument) | (1 << CMakeParser.Bracket_argument))) != 0):
-                self.state = 49
+                self.state = 50
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
                 if token in [CMakeParser.Identifier, CMakeParser.Unquoted_argument, CMakeParser.Quoted_argument, CMakeParser.Bracket_argument]:
-                    self.state = 47
+                    self.state = 48
                     self.single_argument()
                     pass
                 elif token in [CMakeParser.T__0]:
-                    self.state = 48
+                    self.state = 49
                     self.compound_argument()
                     pass
                 else:
                     raise NoViableAltException(self)
 
-                self.state = 53
+                self.state = 54
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
-            self.state = 54
+            self.state = 55
             self.match(CMakeParser.T__1)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
```

### Comparing `CMinx-1.1.8/src/cminx/parser/CMakeVisitor.py` & `CMinx-1.1.9/src/cminx/parser/CMakeVisitor.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/src/cminx/parser/__init__.py` & `CMinx-1.1.9/src/cminx/parser/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import logging
+
+from antlr4 import Parser, DFA
+from antlr4.atn.ATNConfigSet import ATNConfigSet
 from antlr4.error.ErrorListener import ErrorListener
 
 
 class CMakeSyntaxError(SyntaxError):
     pass
 
 
@@ -9,74 +13,102 @@
     """
     Listens for parser errors and raises exceptions when they occur.
     """
 
     def __init__(self):
         super(ParserErrorListener, self).__init__()
 
+        self.logger = logging.getLogger(__name__)
+
     def syntaxError(self, recognizer, offendingSymbol, line, column, msg, e):
         """
         As per the Antlr4 Javadoc:
-            Upon syntax error, notify any interested parties. This is not how to recover from errors or compute error messages.
-            ErrorStrategy specifies how to recover from syntax errors and how to compute error messages.
-            This listener's job is simply to emit a computed message, though it has enough information to create its own message in many cases.
-            The RecognitionException (e) is non-null for all syntax errors except when we discover mismatched token errors that we can recover from in-line,
-            without returning from the surrounding rule (via the single token insertion and deletion mechanism).
+
+            Upon syntax error, notify any interested parties. This is not how to recover from errors or compute error
+            messages. ErrorStrategy specifies how to recover from syntax errors and how to compute error messages.
+            This listener's job is simply to emit a computed message, though it has enough information to create its
+            own message in many cases. The RecognitionException (e) is non-null for all syntax errors except when we
+            discover mismatched token errors that we can recover from in-line, without returning from the surrounding
+            rule (via the single token insertion and deletion mechanism).
+
         :raises RecognitionException: When the mismatched token cannot be recovered from
         :raises CMakeSyntaxError: When it is possible to recover from this error via single token insertion/deletion.
         """
         if e is not None:
             raise e
         else:
             s = CMakeSyntaxError()
             s.lineno = f"{line}:{column}"
             s.msg = msg
             raise s
 
-    def reportAmbiguity(self, recognizer, dfa, startIndex, stopIndex, exact, ambigAlts, configs):
+    def reportAmbiguity(self, recognizer: Parser, dfa: DFA, startIndex: int,
+                        stopIndex: int, exact: bool, ambigAlts: set, configs: ATNConfigSet):
         """
         As per the Antlr4 Javadoc:
-            This method is called by the parser when a full-context prediction results in an ambiguity.
-            Each full-context prediction which does not result in a syntax error will call either ErrorListener.reportContextSensitivity() or ErrorListener.reportAmbiguity().
 
-            When ambigAlts is not None, it contains the set of potentially viable alternatives identified by the prediction algorithm. When ambigAlts is None, use ATNConfigSet.getAlts() to obtain the represented alternatives from the configs argument.
+            This method is called by the parser when a full-context prediction results in an ambiguity. Each
+            full-context prediction which does not result in a syntax error will call either
+            ErrorListener.reportContextSensitivity() or ErrorListener.reportAmbiguity().
+
+            When ambigAlts is not None, it contains the set of potentially viable alternatives identified by the
+            prediction algorithm. When ambigAlts is None, use ATNConfigSet.getAlts() to obtain the represented
+            alternatives from the configs argument.
+
+            When exact is True, all of the potentially viable alternatives are truly viable, i.e. this is reporting
+            an exact ambiguity. When exact is False, at least two of the potentially viable alternatives are viable
+            for the current input, but the prediction algorithm terminated as soon as it determined that at least the
+            minimum potentially viable alternative is truly viable.
 
-            When exact is True, all of the potentially viable alternatives are truly viable, i.e. this is reporting an exact ambiguity. When exact is False, at least two of the potentially viable alternatives are viable for the current input, but the prediction algorithm terminated as soon as it determined that at least the minimum potentially viable alternative is truly viable.
-
-            When the PredictionMode.LL_EXACT_AMBIG_DETECTION prediction mode is used, the parser is required to identify exact ambiguities so exact will always be true.
+            When the PredictionMode.LL_EXACT_AMBIG_DETECTION prediction mode is used, the parser is required to
+            identify exact ambiguities so exact will always be true.
 
             This method is not used by lexers.
 
-        :raises RuntimeError: Unconditionally, we should not encounter ambiguities
+        This method only logs ambiguities, it does not halt parsing as our grammar
+        is ambiguous. The chosen alternative is implied to be the first one in the grammar.
         """
+        self.logger.debug(f"Found parse ambiguity at starting index {startIndex}, stop index {stopIndex}")
 
-        raise RuntimeError("Parse ambiguity")
-
-    def reportAttemptingFullContext(self, recognizer, dfa, startIndex, stopIndex, conflictingAlts, configs):
+    def reportAttemptingFullContext(self, recognizer: Parser, dfa: DFA, startIndex: int,
+                                    stopIndex: int, conflictingAlts: set, configs: ATNConfigSet):
         """
         As per the Antlr4 Javadoc:
-            This method is called when an SLL conflict occurs and the parser is about to use the full context information to make an LL decision.
-            If one or more configurations in configs contains a semantic predicate, the predicates are evaluated before this method is called. The subset of alternatives which are still viable after predicates are evaluated is reported in conflictingAlts.
+
+            This method is called when an SLL conflict occurs and the parser is about to use the full context
+            information to make an LL decision. If one or more configurations in configs contains a semantic
+            predicate, the predicates are evaluated before this method is called. The subset of alternatives which
+            are still viable after predicates are evaluated is reported in conflictingAlts.
 
             This method is not used by lexers.
 
-        Currently this is a no-op, it is unknown whether we should allow or disallow full context LL decisions.
+        Currently, this is a no-op, it is unknown whether we should allow or disallow full context LL decisions.
         """
         pass
 
-    def reportContextSensitivity(self, recognizer, dfa, startIndex, stopIndex, prediction, configs):
+    def reportContextSensitivity(self, recognizer: Parser, dfa: DFA, startIndex: int,
+                                 stopIndex: int, prediction: int, configs: ATNConfigSet):
         """
         As per the Antlr4 Javadoc:
-            This method is called by the parser when a full-context prediction has a unique result.
-            Each full-context prediction which does not result in a syntax error will call either ErrorListener.reportContextSensitivity() or ErrorListener.reportAmbiguity().
-
-            For prediction implementations that only evaluate full-context predictions when an SLL conflict is found (including the default ParserATNSimulator implementation), this method reports cases where SLL conflicts were resolved to unique full-context predictions, i.e. the decision was context-sensitive.
-            This report does not necessarily indicate a problem, and it may appear even in completely unambiguous grammars.
-            configs may have more than one represented alternative if the full-context prediction algorithm does not evaluate predicates before beginning the full-context prediction. In all cases, the final prediction is passed as the prediction argument.
 
-            Note that the definition of "context sensitivity" in this method differs from the concept in DecisionInfo.contextSensitivities. This method reports all instances where an SLL conflict occurred but LL parsing produced a unique result, whether or not that unique result matches the minimum alternative in the SLL conflicting set.
+            This method is called by the parser when a full-context prediction has a unique result. Each full-context
+            prediction which does not result in a syntax error will call either
+            ErrorListener.reportContextSensitivity() or ErrorListener.reportAmbiguity().
+
+            For prediction implementations that only evaluate full-context predictions when an SLL conflict is found
+            (including the default ParserATNSimulator implementation), this method reports cases where SLL conflicts
+            were resolved to unique full-context predictions, i.e. the decision was context-sensitive. This report
+            does not necessarily indicate a problem, and it may appear even in completely unambiguous grammars.
+            configs may have more than one represented alternative if the full-context prediction algorithm does not
+            evaluate predicates before beginning the full-context prediction. In all cases, the final prediction is
+            passed as the prediction argument.
+
+            Note that the definition of "context sensitivity" in this method differs from the concept in
+            DecisionInfo.contextSensitivities. This method reports all instances where an SLL conflict occurred but
+            LL parsing produced a unique result, whether or not that unique result matches the minimum alternative in
+            the SLL conflicting set.
 
             This method is not used by lexers.
 
         This method is currently a no-op, as it being called does not indicate an error necessarily.
         """
         pass
```

### Comparing `CMinx-1.1.8/src/cminx/rstwriter.py` & `CMinx-1.1.9/src/cminx/rstwriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,27 @@
 from enum import Enum
 from typing import Any, Union, IO, List, Tuple
 
 from cminx import Settings
 
 
 class ListType(Enum):
+    """
+    Represents the different types of RST
+    lists.
+    """
+
     ENUMERATED = 0
+    """
+    An enumerated RST list.
+    """
     BULLETED = 1
+    """
+    A bulleted RST list. 
+    """
 
 
 def interpreted_text(role: str, text: str) -> str:
     """
     This function generates an interpreted text RST element
     from the specified text and using the specified role.
     Interpreted text may appear almost anywhere regular text can
@@ -51,149 +62,151 @@
 
 
 class Paragraph(object):
     """
     Represents an RST paragraph
     """
 
-    def __init__(self, text: str, indent: str = ""):
-        self.text = text
-        self.prefix = indent
-        self.text_string = ""
+    def __init__(self, text: str, indent: str = "") -> None:
+        self.text: str = text
+        self.prefix: str = indent
+        self.text_string: str = ""
         self.build_text_string()
 
-    def build_text_string(self):
+    def build_text_string(self) -> None:
         """
         Populates Paragraph.text_string with the
         RST string corresponding to this paragraph
         """
         self.text_string = "\n".join(
             [self.prefix + text for text in self.text.split("\n")])
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.text_string
 
 
 class Field(object):
     """
     Represents an RST field, such as Author
     """
 
-    def __init__(self, field_name: str, field_text: str, indent: str = ""):
-        self.field_name = field_name
-        self.field_text = field_text
-        self.field_string = ""
-        self.indent = indent
+    def __init__(self, field_name: str, field_text: str, indent: str = "") -> None:
+        self.field_name: str = field_name
+        self.field_text: str = field_text
+        self.field_string: str = ""
+        self.indent: str = indent
         self.build_field_string()
 
-    def build_field_string(self):
+    def build_field_string(self) -> None:
         """
         Populates Field.field_string with the
         RST string corresponding to this field
         """
 
         self.field_string = f"\n{self.indent}:{self.field_name}: {self.field_text}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.field_string
 
 
 class DocTest(object):
     """
     Represents an RST DocTest
     """
 
-    def __init__(self, test_line: str, expected_output: str, indent=""):
-        self.test_line = test_line
-        self.expected_output = expected_output
-        self.doctest_string = ""
-        self.indent = indent
+    def __init__(self, test_line: str, expected_output: str, indent: str = "") -> None:
+        self.test_line: str = test_line
+        self.expected_output: str = expected_output
+        self.doctest_string: str = ""
+        self.indent: str = indent
         self.build_doctest_string()
 
-    def build_doctest_string(self):
+    def build_doctest_string(self) -> None:
         """
         Populates DocTest.doctest_string with the
         RST string corresponding to this DocTest
         """
         self.doctest_string = f"\n{self.indent}>>> {self.test_line}\n{self.expected_output}\n"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.doctest_string
 
 
 class RSTList(object):
     """
     Represents one of the two types of RST lists:
     Enumerated or Bulleted
     """
 
-    def __init__(self, items: Tuple[str], list_type: ListType, indent: str = ""):
-        self.items = items
-        self.list_type = list_type
-        self.list_string = ""
-        self.indent = indent
+    def __init__(self, items: Tuple[str], list_type: ListType, indent: str = "") -> None:
+        self.items: Tuple[str] = items
+        self.list_type: ListType = list_type
+        self.list_string: str = ""
+        self.indent: str = indent
         self.build_list_string()
 
-    def build_list_string(self):
+    def build_list_string(self) -> None:
         """
         Populates RSTList.list_string with the
-        RST string corresponding to this list
+        RST string corresponding to this list.
+
+        :raises ValueError: When :py:attr:`~.RSTList.list_type` is unknown.
         """
 
         self.list_string = "\n"
         if self.list_type == ListType.ENUMERATED:
             for i in range(0, len(self.items)):
                 self.list_string += f"{self.indent}{i + 1}. {self.items[i]}\n"
         elif self.list_type == ListType.BULLETED:
             for item in self.items:
                 self.list_string += f"{self.indent}* {item}\n"
         else:
             raise ValueError("Unknown list type")
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.list_string
 
 
 class Heading(object):
     """
     Represents a section heading
     """
 
-    def __init__(self, title: str, header_char: str):
+    def __init__(self, title: str, header_char: str) -> None:
         self.title = title
         self.header_char = header_char
         self.heading_string = ""
         self.build_heading_string()
 
-    def build_heading_string(self):
+    def build_heading_string(self) -> None:
         """
         Populates Heading.heading_string with the
         RST string corresponding to this heading
         """
         heading = ""
         for _ in self.title:
             heading += self.header_char
         self.heading_string = f"\n{heading}\n{self.title}\n{heading}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.heading_string
 
 
 class SimpleTable(object):
     """
     Represents an RST simple table.
     """
 
     def __init__(self, tab: List[List[str]], headings: List[str]):
-        self.table = tab
-        self.column_headings = headings
-        self.table_string = ""
+        self.table: List[List[str]] = tab
+        self.column_headings: List[str] = headings
+        self.table_string: str = ""
         self.build_table_string()
 
-    def build_table_string(self):
+    def build_table_string(self) -> None:
         """
         Populates SimpleTable.table_string with the
         RST string equivalent of this table
         """
         # Easiest way to do this is loop over all cells and find the longest element, use that to compute the row
         # separator width, and then loop over cells again to add them in with proper separation. Fastest way is to
         # compute the separator width, then use list comprehension to build the table string. Probably going to be
@@ -208,15 +221,15 @@
         num_columns = len(self.table[0])
 
         if len(self.column_headings) != 0 and len(
                 self.column_headings) != num_columns:
             raise ValueError(
                 "Different number of headings than number of columns in table")
 
-        # Find the longest cell to use as the row separator width Yes I know doing it this way is inefficient,
+        # Find the longest cell to use as the row separator width. Yes I know doing it this way is inefficient,
         # but readability is more important unless we're dealing with thousands
         # of cells.
         for row in self.table:
             # Check column number against number of cells in row; should be
             # equal
             if len(row) != num_columns:
                 raise ValueError("Number of columns in table is inconsistent")
@@ -232,35 +245,33 @@
             row_separator_width = length if length > row_separator_width else row_separator_width
 
         # We know the width, now to construct the separator itself
         for i in range(row_separator_width):
             row_separator += "="
 
         table_str = ""
-        # Index zero is heading overline, index 1 is headings, index 2 is
-        # underline
-        heading_lines = ["", "", ""]
+        heading_lines = {"overline": "", "headings": "", "underline": ""}
         # Build heading overlines/underlines and add correct spacing
         for heading in self.column_headings:
             heading_len = len(heading)
             for i in range(0, row_separator_width):
-                heading_lines[0] += '='
+                heading_lines["overline"] += '='
 
                 # If current line position is not greater than the length of the heading, add the character at position
                 # Else, add spaces until end of row separator
                 if i < heading_len:
-                    heading_lines[1] += heading[i]
+                    heading_lines["headings"] += heading[i]
                 else:
-                    heading_lines[1] += " "
-            heading_lines[0] += "  "  # Recommended 2 spaces between columns
-            heading_lines[1] += "  "
+                    heading_lines["headings"] += " "
+            heading_lines["overline"] += "  "  # Recommended 2 spaces between columns
+            heading_lines["headings"] += "  "
 
         # Overline and underline should be the same
-        heading_lines[2] = heading_lines[0]
-        table_str += "\n".join(heading_lines) + "\n"
+        heading_lines["underline"] = heading_lines["overline"]
+        table_str += "\n".join(heading_lines.values()) + "\n"
 
         # Add cells to table string
         for row in self.table:
             row_str = ""
             for cell in row:
                 row_str += str(cell)
                 for i in range(0, row_separator_width - len(str(cell))):
@@ -268,65 +279,71 @@
                 row_str += "  "
             table_str += row_str + "\n"
         for _ in self.table[0]:
             table_str += row_separator + "  "
         table_str += "\n"
         self.table_string = table_str
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.table_string
 
 
 class DirectiveHeading(object):
     """
     Represents the unique heading for a Directive (.. :<name>:)
     """
 
-    def __init__(self, title: str, indent: str, args: str):
-        self.title = title
-        self.indent = indent
-        self.args = args
-        self.heading_string = ""
+    def __init__(self, title: str, indent: str, args: str) -> None:
+        self.title: str = title
+        self.indent: str = indent
+        self.args: str = args
+        self.heading_string: str = ""
         self.build_heading_string()
 
-    def build_heading_string(self):
+    def build_heading_string(self) -> None:
+        """Builds the directive heading string and stores in :py:attr:`~heading_str`"""
         self.heading_string = f"\n{self.indent}.. {self.title}:: {self.args}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.heading_string
 
 
 class Option(object):
     """
     Represents a directive option, such as maxdepth
     """
 
-    def __init__(self, name: str, value: str, indent: str):
-        self.name = name
-        self.value = value
-        self.indent = indent
-        self.option_string = ""
+    def __init__(self, name: str, value: str, indent: str) -> None:
+        self.name: str = name
+        self.value: str = value
+        self.indent: str = indent
+        self.option_string: str = ""
         self.build_option_string()
 
-    def build_option_string(self):
+    def build_option_string(self) -> None:
+        """Builds the option string and stores in :py:attr:`~option_string`"""
         self.option_string = f"{self.indent}:{self.name}: {self.value}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.option_string
 
 
-def get_indents(num) -> str:
+def get_indents(num: int) -> str:
     """
     Get the string containing the necessary indent.
+    The number of spaces in the returned string equals three times
+    the input number, because directives require three spaces
+    so the text lines up with the first letter of the directive name.
 
-    :return: A string containing the correct number of whitespace characters, derived from the indent level.
+    :return: A string containing the correct number of space characters, derived from the indent level.
     """
     indents = ""
     for i in range(0, num):
-        # Directives require the first non-whitespace character of every line to line up with the first letter of
+        # Directives require the first non-whitespace character
+        # of every line to line up with the first letter of
         # the directive name
         indents += '   '
     return indents
 
 
 class RSTWriter(object):
     """
@@ -335,83 +352,83 @@
     for generating reStructuredText documents. The document is
     held in an intermediate object-oriented representation until
     the text representation is requested either through
     :py:meth:`~cminx.rstwriter.RSTWriter.to_text`
     or by calling :py:func:`str` on this object.
     """
 
-    heading_level_chars = ['#', '*', '=', '-', '_', '~', '!', '&', '@', '^']
+    heading_level_chars: List[str] = ['#', '*', '=', '-', '_', '~', '!', '&', '@', '^']
     """Characters to use as heading overline/underline, indexed by section_level"""
 
     def __init__(
             self,
             title: str,
             section_level: int = 0,
-            settings=Settings(), indent: int = 0):
+            settings: Settings = Settings(), indent: int = 0) -> None:
         self.__title: str = title
         self.section_level: int = section_level
-        self.settings = settings
+        self.settings: Settings = settings
         if settings.rst.headers is not None:
             self.heading_level_chars = settings.rst.headers
 
-        self.indent = indent
+        self.indent: int = indent
         self.header_char: str = self.heading_level_chars[section_level]
         # Heading must be first in the document tree
         self.document: List[Any] = [self.build_heading()]
 
-    def clear(self):
+    def clear(self) -> None:
         """
         Clear all document tree elements (besides required heading)
         """
         del self.document[1:]
 
     @property
     def title(self) -> str:
         return self.__title
 
     @title.setter
-    def title(self, new_title: str):
+    def title(self, new_title: str) -> None:
         """
         Rebuild heading and replace the old one in the document tree whenever title is changed
 
         :param new_title: The new section title to be used.
         """
         self.__title = new_title
         self.document[0] = self.build_heading()
 
-    def bulleted_list(self, *items: str):
+    def bulleted_list(self, *items: str) -> None:
         """
         Add a bulleted list to the document tree.
 
         :param items: varargs containing the desired list items.
         """
 
         self.document.append(RSTList(items, ListType.BULLETED, indent=get_indents(self.indent)))
 
-    def enumerated_list(self, *items: str):
+    def enumerated_list(self, *items: str) -> None:
         """
         Add an enumerated list to the document tree; e.g.
             1. Item 1
             2. Item 2
 
         :param items: varargs containing the desired list items.
         """
         self.document.append(RSTList(items, ListType.ENUMERATED, indent=get_indents(self.indent)))
 
-    def field(self, field_name: str, field_text: str):
+    def field(self, field_name: str, field_text: str) -> None:
         """
         Add a field, such as Author or Version, to the document tree.
 
         :param field_name: Name of the field being added, such as Author.
 
         :param field_text: Value of the field, such as the author's name.
         """
         self.document.append(Field(field_name, field_text, get_indents(self.indent)))
 
-    def doctest(self, test_line: str, expected_output: str):
+    def doctest(self, test_line: str, expected_output: str) -> None:
         """
         Adds a doctest segment to the document tree.
         A doctest segment appears as an interactive python session.
         The doctest Python module can then be used to scan for these segments
         and execute the test_line to ensure the output is the same.
 
         :param test_line: Python code segment being used as the line to be tested.
@@ -429,15 +446,15 @@
         sect = RSTWriter(
             title,
             section_level=self.section_level + 1,
             settings=self.settings)
         self.document.append(sect)
         return sect
 
-    def text(self, txt: str):
+    def text(self, txt: str) -> None:
         """
         Add a paragraph to document tree.
 
         :param txt: The content of the new paragraph.
         """
         self.document.append(Paragraph(txt, indent=get_indents(self.indent)))
 
@@ -487,23 +504,23 @@
         :return: The completed RST document in string form.
         """
         document_string = ""
         for element in self.document:
             document_string += f"{element}\n"
         return document_string
 
-    def __str__(self):
+    def __str__(self) -> str:
         """
         Equivalent to :func: `~cminx.RSTWriter.to_text`
 
         :return: The completed RST document in string form.
         """
         return self.to_text()
 
-    def write_to_file(self, file: Union[str, IO]):
+    def write_to_file(self, file: Union[str, IO]) -> None:
         """
         Write text representation of this document to file. File may be a string (path will be opened in write mode)
         or a file-like object.
 
         :param file: File to write to. May be a string representing a real filepath on the local filesystem (will be
         overwritten), or a file-like object.
 
@@ -536,25 +553,25 @@
 class Directive(RSTWriter):
     """
     Use :func:`cminx.RSTWriter.directive` to construct.
     Represents an RST directive, such as toctree or an admonition.
     Does not verify that the directive or its arguments are valid.
     """
 
-    def __init__(self, name: str, indent: int = 0, *arguments: str, settings: Settings = Settings()):
+    def __init__(self, name: str, indent: int = 0, *arguments: str, settings: Settings = Settings()) -> None:
         """
         :param name: Name of the directive being constructed, eg. toctree or admonition.
 
         :param indent: Indent level of this directive. 0 is root, 1 is under another directive, etc.
 
         :param arguments: Varargs to be used as the directive arguments, eg. a topic's title.
         """
 
-        self.arguments = arguments
-        self.options = []
+        self.arguments: Tuple[str] = arguments
+        self.options: List[Option] = []
         super().__init__(name, settings=settings, indent=indent + 1)
 
     def build_heading(self) -> DirectiveHeading:
         """
         Build directive heading format (ex. '.. toctree::') and return.
 
         :return: Correctly formatted directive heading string.
@@ -567,15 +584,15 @@
         """
         Format argument list into the correct argument string for use with directives.
 
         :return: A string representing the directive arguments.
         """
         return ','.join(map(str, self.arguments))
 
-    def option(self, name: str, value: str = ""):
+    def option(self, name: str, value: str = "") -> None:
         """
         Add an option, such as toctree's maxdepth. Does not verify if valid option
         """
         self.options.append(
             Option(
                 name,
                 value,
```

### Comparing `CMinx-1.1.8/src/main.py` & `CMinx-1.1.9/src/main.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/CMakeLists.txt` & `CMinx-1.1.9/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/README.rst` & `CMinx-1.1.9/tests/README.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/cmake/gen_rst.cmake` & `CMinx-1.1.9/tests/cmake/gen_rst.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/cmake_input/example.cmake` & `CMinx-1.1.9/tests/cmake_input/example.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/context.py` & `CMinx-1.1.9/tests/context.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/__init__.py` & `CMinx-1.1.9/tests/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/aggregator_example.py` & `CMinx-1.1.9/tests/examples/aggregator_example.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/configs/exclude_filters_config.yaml` & `CMinx-1.1.9/tests/examples/configs/exclude_filters_config.yaml`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/configs/exclude_input_file_config.yaml` & `CMinx-1.1.9/tests/examples/configs/exclude_input_file_config.yaml`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/configs/no_auto_exclude_config.yaml` & `CMinx-1.1.9/tests/examples/configs/no_auto_exclude_config.yaml`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/configs/no_include_undocumented_config.yaml` & `CMinx-1.1.9/tests/examples/configs/no_include_undocumented_config.yaml`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/example.cmake` & `CMinx-1.1.9/tests/examples/example.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/rst_validator_example.py` & `CMinx-1.1.9/tests/examples/rst_validator_example.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/rstwriter_example.py` & `CMinx-1.1.9/tests/examples/rstwriter_example.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/sphinx/source/conf.py` & `CMinx-1.1.9/tests/examples/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/examples/sphinx/source/example.rst` & `CMinx-1.1.9/tests/examples/sphinx/source/example.rst`

 * *Files 0% similar despite different names*

```diff
@@ -342,18 +342,18 @@
 
 .. data:: TEST_OPTION
 
 
    .. note:: 
 
       
-                  This variable is a user-editable option,
-                  meaning it appears within the cache and can be
-                  edited on the command line by the :code:`-D` flag.
-                  
+      This variable is a user-editable option,
+      meaning it appears within the cache and can be
+      edited on the command line by the :code:`-D` flag.
+      
 
    This is a documented option
    
 
    :Help text: "This is a test option"
 
    :Default value: OFF
```

### Comparing `CMinx-1.1.8/tests/examples/sphinx/source/example_no_undocumented.rst` & `CMinx-1.1.9/tests/examples/sphinx/source/example_no_undocumented.rst`

 * *Files 0% similar despite different names*

```diff
@@ -142,18 +142,18 @@
 
 .. data:: TEST_OPTION
 
 
    .. note:: 
 
       
-                  This variable is a user-editable option,
-                  meaning it appears within the cache and can be
-                  edited on the command line by the :code:`-D` flag.
-                  
+      This variable is a user-editable option,
+      meaning it appears within the cache and can be
+      edited on the command line by the :code:`-D` flag.
+      
 
    This is a documented option
    
 
    :Help text: "This is a test option"
 
    :Default value: OFF
```

### Comparing `CMinx-1.1.8/tests/examples/sphinx/source/example_no_undocumented_diff_header.rst` & `CMinx-1.1.9/tests/examples/sphinx/source/example_no_undocumented_diff_header.rst`

 * *Files 0% similar despite different names*

```diff
@@ -142,18 +142,18 @@
 
 .. data:: TEST_OPTION
 
 
    .. note:: 
 
       
-                  This variable is a user-editable option,
-                  meaning it appears within the cache and can be
-                  edited on the command line by the :code:`-D` flag.
-                  
+      This variable is a user-editable option,
+      meaning it appears within the cache and can be
+      edited on the command line by the :code:`-D` flag.
+      
 
    This is a documented option
    
 
    :Help text: "This is a test option"
 
    :Default value: OFF
```

### Comparing `CMinx-1.1.8/tests/examples/sphinx/source/example_prefix.rst` & `CMinx-1.1.9/tests/examples/sphinx/source/example_prefix.rst`

 * *Files 0% similar despite different names*

```diff
@@ -342,18 +342,18 @@
 
 .. data:: TEST_OPTION
 
 
    .. note:: 
 
       
-                  This variable is a user-editable option,
-                  meaning it appears within the cache and can be
-                  edited on the command line by the :code:`-D` flag.
-                  
+      This variable is a user-editable option,
+      meaning it appears within the cache and can be
+      edited on the command line by the :code:`-D` flag.
+      
 
    This is a documented option
    
 
    :Help text: "This is a test option"
 
    :Default value: OFF
```

### Comparing `CMinx-1.1.8/tests/helpers.py` & `CMinx-1.1.9/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/test_all.py` & `CMinx-1.1.9/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/test_samples/__init__.py` & `CMinx-1.1.9/tests/test_samples/__init__.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/test_samples/advanced_function.cmake` & `CMinx-1.1.9/tests/test_samples/advanced_function.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/test_samples/advanced_macro.cmake` & `CMinx-1.1.9/tests/test_samples/advanced_macro.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/test_samples/corr_rst/advanced_function.rst` & `CMinx-1.1.9/tests/test_samples/corr_rst/advanced_function.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/test_samples/corr_rst/advanced_macro.rst` & `CMinx-1.1.9/tests/test_samples/corr_rst/advanced_macro.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/test_samples/corr_rst/undocumented_commands.rst` & `CMinx-1.1.9/tests/test_samples/corr_rst/undocumented_commands.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/test_samples/corr_rst/undocumented_option_no_default.rst` & `CMinx-1.1.9/tests/test_samples/corr_rst/undocumented_option_no_default.rst`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 .. data:: "UNDOCUMENTED_OPTION_NO_DEFAULT"
 
 
    .. note:: 
 
       
-                  This variable is a user-editable option,
-                  meaning it appears within the cache and can be
-                  edited on the command line by the :code:`-D` flag.
-                  
+      This variable is a user-editable option,
+      meaning it appears within the cache and can be
+      edited on the command line by the :code:`-D` flag.
+      
 
    
 
    :Help text: "This is an undocumented option and it doesn't have a default value"
 
    :Default value: OFF
```

### Comparing `CMinx-1.1.8/tests/test_samples/corr_rst/variable.rst` & `CMinx-1.1.9/tests/test_samples/corr_rst/variable.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/test_samples/test_samples.py` & `CMinx-1.1.9/tests/test_samples/test_samples.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/test_samples/undocumented_commands.cmake` & `CMinx-1.1.9/tests/test_samples/undocumented_commands.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/unit_tests/__init__.py` & `CMinx-1.1.9/tests/unit_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/unit_tests/rst_validator.py` & `CMinx-1.1.9/tests/unit_tests/rst_validator.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/unit_tests/test_aggregator.py` & `CMinx-1.1.9/tests/unit_tests/test_aggregator.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,50 +9,53 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import textwrap
 import unittest
 
 import pytest
 
 import context
 from antlr4 import *
 
+from cminx import Settings
+from cminx.config import InputSettings
 from cminx.exceptions import CMakeSyntaxException
 from cminx.parser import ParserErrorListener
 from cminx.parser.CMakeLexer import CMakeLexer
 from cminx.parser.CMakeParser import CMakeParser
 from cminx.aggregator import DocumentationAggregator
 from cminx.documentation_types import FunctionDocumentation, MacroDocumentation, VariableDocumentation, \
-    GenericCommandDocumentation, ClassDocumentation, VarType, DocumentationType
+    GenericCommandDocumentation, ClassDocumentation, VarType, DocumentationType, MethodDocumentation
 
 
 class TestAggregator(unittest.TestCase):
 
     def setUp(self):
         self.filename = context.example_cmake
         # We need a string stream of some kind, FileStream is easiest
         self.input_stream = FileStream(self.filename)
         self.reset()
 
-    def reset(self):
+    def reset(self, settings=Settings()):
         # Convert those strings into tokens and build a stream from those
         self.lexer = CMakeLexer(self.input_stream)
         self.stream = CommonTokenStream(self.lexer)
 
         # We now have a stream of CommonToken instead of strings, parsers require this type of stream
         self.parser = CMakeParser(self.stream)
         self.parser.addErrorListener(ParserErrorListener())
         self.tree = self.parser.cmake_file()
 
         # Hard part is done, we now have a fully useable parse tree, now we just need to walk it
-        self.aggregator = DocumentationAggregator()
+        self.aggregator = DocumentationAggregator(settings)
         self.walker = ParseTreeWalker()
         self.walker.walk(self.aggregator, self.tree)
 
     def test_aggregated_docs(self):
 
         # All of the documented commands are now stored in aggregator.documented,
         # each element is a namedtuple repesenting the type of documentation it is.
@@ -105,60 +108,60 @@
                              "Incorrect params extracted")
 
     def test_doccomment_stringvar_leading_space(self):
         docstring = "This is a string variable"
         var_name = "TEST_VAR"
         val = "This is a value"
 
-        self.input_stream = InputStream(f'''
-#[[[
- {docstring}
-#]]
-set({var_name} "{val}")
+        self.input_stream = InputStream(textwrap.dedent(f'''
+                                #[[[
+                                 {docstring}
+                                #]]
+                                set({var_name} "{val}")
 
-        ''')
+                            '''))
         self.reset()
         self.assertEqual(len(self.aggregator.documented), 1, "Different number of documented commands than expected")
         self.assertEqual(type(self.aggregator.documented[0]), VariableDocumentation, "Unexpected documentation type")
         self.assertEqual(self.aggregator.documented[0].doc.strip(), docstring, "Incorrect docstring extracted")
         self.assertEqual(self.aggregator.documented[0].name.strip(), var_name, "Incorrect function_name extracted")
         self.assertEqual(self.aggregator.documented[0].type, VarType.STRING)
         self.assertEqual(self.aggregator.documented[0].value.strip(), val.strip(), "Incorrect value extracted")
 
     def test_doccomment_listvar_leading_space(self):
         docstring = "This is a list variable"
         var_name = "listvar"
         params = ["param1", "param2"]
 
-        self.input_stream = InputStream(f'''
-#[[[
- {docstring}
-#]]
-set({var_name} {params[0]} {params[1]})
-        ''')
+        self.input_stream = InputStream(textwrap.dedent(f'''
+                                #[[[
+                                {docstring}
+                                #]]
+                                set({var_name} {params[0]} {params[1]})
+                            '''))
         self.reset()
         self.assertEqual(len(self.aggregator.documented), 1, "Different number of documented commands than expected")
         self.assertEqual(type(self.aggregator.documented[0]), VariableDocumentation, "Unexpected documentation type")
         self.assertEqual(self.aggregator.documented[0].doc.strip(), docstring, "Incorrect docstring extracted")
         self.assertEqual(self.aggregator.documented[0].name.strip(), var_name, "Incorrect var_name extracted")
         self.assertEqual(self.aggregator.documented[0].type, VarType.LIST)
 
         self.assertEqual(self.aggregator.documented[0].value, " ".join(params),
                          "Incorrect list elements extracted")
 
     def test_unset(self):
         docstring = "Unsetting a variable"
         var_name = "myvar"
 
-        self.input_stream = InputStream(f'''
-#[[[
- {docstring}
-#]]
-set({var_name})
-        ''')
+        self.input_stream = InputStream(textwrap.dedent(f'''
+                                #[[[
+                                {docstring}
+                                #]]
+                                set({var_name})
+                            '''))
         self.reset()
         self.assertEqual(len(self.aggregator.documented), 1, "Different number of documented commands than expected")
         self.assertEqual(type(self.aggregator.documented[0]), VariableDocumentation, "Unexpected documentation type")
         self.assertEqual(self.aggregator.documented[0].doc.strip(), docstring, "Incorrect docstring extracted")
         self.assertEqual(self.aggregator.documented[0].name.strip(), var_name, "Incorrect var_name extracted")
         self.assertEqual(self.aggregator.documented[0].type, VarType.UNSET)
 
@@ -172,35 +175,51 @@
                                                       inner_classes=("Inner1", "Inner2")):
         class_docstring = "This is a class"
         inner_class_docstring = "#[[[\n# This is an inner class\n#]]"
         method_docstring = "#[[[\n# This is a method\n#]]"
         attribute_docstring = "#[[[\n# This is an attribute\n#]]"
         class_name = "MyClass"
         inner_class_definitions = '\n'.join(
-            [f'{inner_class_docstring}\ncpp_class({inner_class_name})\ncpp_end_class()' for inner_class_name in
-             inner_classes])
-        method_definitions = '\n'.join([
-            f'{method_docstring}\ncpp_member({method_name} {class_name})\nfunction(' + '${' + method_name + '})\nendfunction()'
-            for method_name in methods])
+            [
+                textwrap.dedent(f"""\
+                    {inner_class_docstring}
+                    cpp_class({inner_class_name})
+                    cpp_end_class()
+                """)
+                for inner_class_name in inner_classes
+            ]
+        )
+        # Curly brackets in f strings are escaped with two brackets. So we end up with "${<value of method_name>}"
+        method_definitions = '\n'.join(
+            [
+                textwrap.dedent(f"""\
+                    {method_docstring}
+                    cpp_member({method_name} {class_name})
+                    function(${{{method_name}}})
+                    endfunction()
+                """)
+                for method_name in methods
+            ]
+        )
         attribute_definitions = '\n'.join(
             [f'{attribute_docstring}\ncpp_attr({class_name} {attr_name})' for attr_name in attributes])
-        self.input_stream = InputStream(f'''
-#[[[
-# {class_docstring}
-#]]
-cpp_class({class_name} {' '.join(superclasses)})
+        self.input_stream = InputStream(textwrap.dedent(f'''
+                                #[[[
+                                # {class_docstring}
+                                #]]
+                                cpp_class({class_name} {' '.join(superclasses)})
 
-    {attribute_definitions}
+                                    {attribute_definitions}
 
-    {method_definitions}
+                                    {method_definitions}
 
-    {inner_class_definitions}
+                                    {inner_class_definitions}
 
-cpp_end_class()
-        ''')
+                                cpp_end_class()
+                            '''))
         self.reset()
         self.assertEqual(len(self.aggregator.documented), 1 + len(inner_classes),
                          "Different number of documented commands than expected")
         self.assertEqual(type(self.aggregator.documented[0]), ClassDocumentation, "Unexpected documentation type")
         self.assertEqual(self.aggregator.documented[0].doc.strip(), class_docstring, "Incorrect docstring extracted")
         self.assertEqual(self.aggregator.documented[0].name.strip(), class_name, "Incorrect class name extracted")
         self.assertEqual(len(self.aggregator.documented[0].superclasses), len(superclasses),
@@ -210,15 +229,15 @@
                              "Superclass name not preserved")
 
         self.assertEqual(len(self.aggregator.documented[0].inner_classes), len(inner_classes),
                          "Inner classes incorrectly found")
         self.assertEqual(len(self.aggregator.documented[0].members), len(methods), "Members incorrectly found")
         self.assertEqual(len(self.aggregator.documented[0].attributes), len(attributes), "Attributes incorrectly found")
 
-    def test_cpp_class_multi_superclass_no_inner(self, superclasses=["SuperClassA", "SuperClassB", "SuperClassC"]):
+    def test_cpp_class_multi_superclass_no_inner(self, superclasses=("SuperClassA", "SuperClassB", "SuperClassC")):
         self.test_cpp_class_multi_superclass_multi_members(superclasses=superclasses, attributes=[], methods=[])
 
     def test_cpp_class_one_superclasses_no_inner(self):
         self.test_cpp_class_multi_superclass_no_inner(["SuperClass"])
 
     def test_unknown_documented_command(self):
         docstring = 'This is documentation for an unknown command'
@@ -387,10 +406,96 @@
                          f"cpp_member() call outside class was still added to documented list: {self.aggregator.documented}")
 
     def test_invalid_syntax(self):
         self.input_stream = InputStream("#[[[\n#invalid syntax\n#]]\nfunction()\nend_function()")
         with pytest.raises(CMakeSyntaxException):
             self.reset()
 
+    def test_function_param_regex(self):
+        func_name = "test_func"
+        stripped_param_names = ["param1", "param2_with_underscores"]
+        param_names = [f"_tf_{name}" for name in stripped_param_names]
+
+        docstring = "This is a function that has its param name regex-stripped"
+
+        regex = "^_[a-zA-Z]*_"
+
+        self.input_stream = InputStream(textwrap.dedent(f"""
+                    #[[[
+                    # {docstring}
+                    #]]
+                    function({func_name} {' '.join(param_names)})
+                    endfunction()
+                """))
+
+        input_settings = InputSettings(function_parameter_name_strip_regex=regex)
+        self.reset(settings=Settings(input=input_settings))
+        self.assertIsInstance(self.aggregator.documented[0], FunctionDocumentation)
+        self.assertEqual(func_name, self.aggregator.documented[0].name)
+        for i in range(0, len(stripped_param_names)):
+            self.assertEqual(
+                stripped_param_names[i], self.aggregator.documented[0].params[i],
+                "Parameter name was not stripped correctly"
+            )
+
+    def test_macro_param_regex(self):
+        func_name = "test_macro"
+        stripped_param_names = ["param1", "param2_with_underscores"]
+        param_names = [f"_tm_{name}" for name in stripped_param_names]
+
+        docstring = "This is a macro that has its param name regex-stripped"
+
+        regex = "^_[a-zA-Z]*_"
+
+        self.input_stream = InputStream(textwrap.dedent(f"""
+            #[[[
+            # {docstring}
+            #]]
+            macro({func_name} {' '.join(param_names)})
+            endmacro()
+        """))
+
+        input_settings = InputSettings(macro_parameter_name_strip_regex=regex)
+        self.reset(settings=Settings(input=input_settings))
+        self.assertIsInstance(self.aggregator.documented[0], MacroDocumentation)
+        self.assertEqual(func_name, self.aggregator.documented[0].name)
+        for i in range(0, len(stripped_param_names)):
+            self.assertEqual(
+                stripped_param_names[i], self.aggregator.documented[0].params[i],
+                "Parameter name was not stripped correctly"
+            )
+
+    def test_method_param_regex(self):
+        func_name = "test_method"
+        stripped_param_names = ["param1", "param2_with_underscores"]
+        param_names = [f"_tm_{name}" for name in stripped_param_names]
+        param_types = ["desc", "str"]
+
+        docstring = "This is a method that has its param name regex-stripped"
+
+        regex = "^_[a-zA-Z]*_"
+
+        self.input_stream = InputStream(textwrap.dedent(f"""
+                    cpp_class(TestClass)
+                        #[[[
+                        # {docstring}
+                        #]]
+                        cpp_member({func_name} TestClass {' '.join(param_types)})
+                        function("${{{func_name}}}" self {' '.join(param_names)})
+                        endfunction()
+                    cpp_end_class()
+                """))
+
+        input_settings = InputSettings(member_parameter_name_strip_regex=regex)
+        self.reset(settings=Settings(input=input_settings))
+        self.assertIsInstance(self.aggregator.documented[0], ClassDocumentation)
+        self.assertIsInstance(self.aggregator.documented[0].members[0], MethodDocumentation)
+        self.assertEqual(func_name, self.aggregator.documented[0].members[0].name)
+        for i in range(0, len(stripped_param_names)):
+            self.assertEqual(
+                stripped_param_names[i], self.aggregator.documented[0].members[0].params[i],
+                "Parameter name was not stripped correctly"
+            )
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `CMinx-1.1.8/tests/unit_tests/test_config.py` & `CMinx-1.1.9/tests/unit_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/unit_tests/test_documenter.py` & `CMinx-1.1.9/tests/unit_tests/test_documenter.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/unit_tests/test_error_listener.py` & `CMinx-1.1.9/tests/unit_tests/test_error_listener.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     def setUp(self):
         self.listener = ParserErrorListener()
 
     def test_syntax_error(self):
         self.assertRaises(CMakeSyntaxError, self.listener.syntaxError, None, None, 1, 1, "Test message", None)
 
     def test_ambiguity(self):
-        # This method will only be called if the grammar is bad, call manually to ensure that if it is ever called we get an error
-        self.assertRaises(RuntimeError, self.listener.reportAmbiguity, None, None, None, None, None, None, None)
+        # Our grammar is now ambiguous, so ensure reporting an ambiguity does not raise an exception
+        self.listener.reportAmbiguity(None, None, None, None, None, None, None)
 
     def test_full_context(self):
         # No-op, we include it for documentation purposes
         # Will be called if an SLL conflict occurs but before a full-context LL resolution is made
         # Not an error, only a notification of a differing method than normal resolution
         self.assertEqual(None, self.listener.reportAttemptingFullContext(None, None, None, None, None, None))
```

### Comparing `CMinx-1.1.8/tests/unit_tests/test_init.py` & `CMinx-1.1.9/tests/unit_tests/test_init.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/unit_tests/test_lexer.py` & `CMinx-1.1.9/tests/unit_tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/unit_tests/test_parser.py` & `CMinx-1.1.9/tests/unit_tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.8/tests/unit_tests/test_rstwriter.py` & `CMinx-1.1.9/tests/unit_tests/test_rstwriter.py`

 * *Files identical despite different names*

