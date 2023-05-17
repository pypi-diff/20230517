# Comparing `tmp/argparse-manpage-4.2.tar.gz` & `tmp/argparse-manpage-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse-manpage-4.2.tar", last modified: Sun May 14 10:58:16 2023, max compression
+gzip compressed data, was "argparse-manpage-4.3.tar", last modified: Wed May 17 13:03:01 2023, max compression
```

## Comparing `argparse-manpage-4.2.tar` & `argparse-manpage-4.3.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.389906 argparse-manpage-4.2/
--rw-rw-r--   0 twine    (17125) twine    (17125)      136 2019-09-07 00:39:54.000000 argparse-manpage-4.2/AUTHORS
--rw-rw-r--   0 twine    (17125) twine    (17125)    11357 2019-09-07 00:39:54.000000 argparse-manpage-4.2/LICENSE
--rw-r--r--   0 twine    (17125) twine    (17125)      649 2023-05-14 10:57:58.000000 argparse-manpage-4.2/MANIFEST.in
--rw-r--r--   0 twine    (17125) twine    (17125)     4774 2023-05-14 10:57:58.000000 argparse-manpage-4.2/NEWS
--rw-r--r--   0 twine    (17125) twine    (17125)     8915 2023-05-14 10:58:16.389906 argparse-manpage-4.2/PKG-INFO
--rw-r--r--   0 twine    (17125) twine    (17125)     8472 2023-05-14 10:57:58.000000 argparse-manpage-4.2/README.md
--rwxr-xr-x   0 twine    (17125) twine    (17125)      357 2022-10-31 08:33:07.000000 argparse-manpage-4.2/argparse-manpage
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.379906 argparse-manpage-4.2/argparse_manpage/
--rw-r--r--   0 twine    (17125) twine    (17125)       54 2023-05-14 10:57:58.000000 argparse-manpage-4.2/argparse_manpage/__init__.py
--rw-r--r--   0 twine    (17125) twine    (17125)     3589 2023-05-14 10:57:58.000000 argparse-manpage-4.2/argparse_manpage/cli.py
--rw-r--r--   0 twine    (17125) twine    (17125)     1669 2023-05-14 10:57:58.000000 argparse-manpage-4.2/argparse_manpage/compat.py
--rw-r--r--   0 twine    (17125) twine    (17125)    21556 2023-05-14 10:57:58.000000 argparse-manpage-4.2/argparse_manpage/manpage.py
--rw-r--r--   0 twine    (17125) twine    (17125)     2326 2022-10-31 08:33:07.000000 argparse-manpage-4.2/argparse_manpage/tooling.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.380906 argparse-manpage-4.2/argparse_manpage.egg-info/
--rw-rw-r--   0 twine    (17125) twine    (17125)     8915 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/PKG-INFO
--rw-rw-r--   0 twine    (17125) twine    (17125)     2605 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/SOURCES.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)        1 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/dependency_links.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)       63 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/entry_points.txt
--rw-r--r--   0 twine    (17125) twine    (17125)       58 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/requires.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)       32 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/top_level.txt
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.381906 argparse-manpage-4.2/build_manpages/
--rw-r--r--   0 twine    (17125) twine    (17125)      169 2022-10-31 08:33:07.000000 argparse-manpage-4.2/build_manpages/__init__.py
--rw-r--r--   0 twine    (17125) twine    (17125)     7364 2023-04-15 19:13:21.000000 argparse-manpage-4.2/build_manpages/build_manpage.py
--rw-r--r--   0 twine    (17125) twine    (17125)     6248 2023-05-14 10:57:58.000000 argparse-manpage-4.2/build_manpages/build_manpages.py
--rw-r--r--   0 twine    (17125) twine    (17125)      980 2022-10-31 08:33:07.000000 argparse-manpage-4.2/build_manpages/compat.py
--rw-r--r--   0 twine    (17125) twine    (17125)      157 2022-10-31 08:33:07.000000 argparse-manpage-4.2/build_manpages/manpage.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.378906 argparse-manpage-4.2/examples/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.381906 argparse-manpage-4.2/examples/argument_groups/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.381906 argparse-manpage-4.2/examples/argument_groups/bin/
--rwxr-xr-x   0 twine    (17125) twine    (17125)     2250 2021-11-28 22:10:08.000000 argparse-manpage-4.2/examples/argument_groups/bin/test
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.381906 argparse-manpage-4.2/examples/argument_groups/expected/
--rw-r--r--   0 twine    (17125) twine    (17125)     2125 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/argument_groups/expected/test.1
--rw-r--r--   0 twine    (17125) twine    (17125)      115 2022-10-31 08:33:07.000000 argparse-manpage-4.2/examples/argument_groups/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)      984 2021-11-28 22:10:08.000000 argparse-manpage-4.2/examples/argument_groups/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.382906 argparse-manpage-4.2/examples/copr/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.383906 argparse-manpage-4.2/examples/copr/copr_cli/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/copr_cli/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/copr_cli/build_config.py
--rw-r--r--   0 twine    (17125) twine    (17125)    49234 2022-10-31 08:33:07.000000 argparse-manpage-4.2/examples/copr/copr_cli/main.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/copr_cli/util.py
--rw-r--r--   0 twine    (17125) twine    (17125)    26531 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/copr/expected-output.1
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.383906 argparse-manpage-4.2/examples/copr/fake-deps/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/HACK
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.384906 argparse-manpage-4.2/examples/copr/fake-deps/copr/
--rw-rw-r--   0 twine    (17125) twine    (17125)       35 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/copr/README
--rw-rw-r--   0 twine    (17125) twine    (17125)       43 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/copr/__init__.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.384906 argparse-manpage-4.2/examples/copr/fake-deps/copr/client/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/copr/client/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       29 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/copr/client/responses.py
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/copr/exceptions.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       28 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/jinja2.py
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/simplejson.py
--rw-r--r--   0 twine    (17125) twine    (17125)      113 2022-10-31 08:33:07.000000 argparse-manpage-4.2/examples/copr/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)      965 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.385906 argparse-manpage-4.2/examples/old_format/
--rw-r--r--   0 twine    (17125) twine    (17125)      917 2022-01-12 01:47:25.000000 argparse-manpage-4.2/examples/old_format/README.md
--rw-rw-r--   0 twine    (17125) twine    (17125)      519 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/old_format/example.py
--rw-r--r--   0 twine    (17125) twine    (17125)      503 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/old_format/expected-output.1
--rw-rw-r--   0 twine    (17125) twine    (17125)       59 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/old_format/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)      789 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/old_format/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.385906 argparse-manpage-4.2/examples/old_format_file_name/
--rw-r--r--   0 twine    (17125) twine    (17125)      585 2022-01-12 01:47:25.000000 argparse-manpage-4.2/examples/old_format_file_name/README.md
--rw-r--r--   0 twine    (17125) twine    (17125)      519 2022-01-12 01:47:25.000000 argparse-manpage-4.2/examples/old_format_file_name/example.py
--rw-r--r--   0 twine    (17125) twine    (17125)      503 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/old_format_file_name/expected-output.1
--rw-r--r--   0 twine    (17125) twine    (17125)       82 2022-01-12 01:47:25.000000 argparse-manpage-4.2/examples/old_format_file_name/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)      789 2022-01-12 01:47:25.000000 argparse-manpage-4.2/examples/old_format_file_name/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.386906 argparse-manpage-4.2/examples/osc/
--rw-r--r--   0 twine    (17125) twine    (17125)     2246 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/osc/expected-output.1
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.386906 argparse-manpage-4.2/examples/osc/osc/
--rw-r--r--   0 twine    (17125) twine    (17125)        0 2022-04-27 06:51:30.000000 argparse-manpage-4.2/examples/osc/osc/__init__.py
--rwxr-xr-x   0 twine    (17125) twine    (17125)     4636 2022-10-31 08:33:07.000000 argparse-manpage-4.2/examples/osc/osc/main.py
--rw-r--r--   0 twine    (17125) twine    (17125)      251 2022-10-31 08:33:07.000000 argparse-manpage-4.2/examples/osc/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)      772 2022-04-27 06:51:30.000000 argparse-manpage-4.2/examples/osc/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.387906 argparse-manpage-4.2/examples/pre-written-man-page/
--rw-r--r--   0 twine    (17125) twine    (17125)      871 2023-05-14 10:57:58.000000 argparse-manpage-4.2/examples/pre-written-man-page/psutils.1
--rw-r--r--   0 twine    (17125) twine    (17125)       60 2023-05-14 10:57:58.000000 argparse-manpage-4.2/examples/pre-written-man-page/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)      272 2023-05-14 10:57:58.000000 argparse-manpage-4.2/examples/pre-written-man-page/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.387906 argparse-manpage-4.2/examples/raw-description/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.387906 argparse-manpage-4.2/examples/raw-description/bin/
--rwxrwxr-x   0 twine    (17125) twine    (17125)     4455 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/raw-description/bin/dg
--rw-r--r--   0 twine    (17125) twine    (17125)     2035 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/raw-description/expected-output.1
--rw-rw-r--   0 twine    (17125) twine    (17125)       69 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/raw-description/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)      982 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/raw-description/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.388906 argparse-manpage-4.2/examples/resalloc/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.388906 argparse-manpage-4.2/examples/resalloc/bin/
--rwxrwxr-x   0 twine    (17125) twine    (17125)     3076 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/bin/resalloc
--rwxrwxr-x   0 twine    (17125) twine    (17125)     2070 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/bin/resalloc-maint
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.378906 argparse-manpage-4.2/examples/resalloc/expected/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.388906 argparse-manpage-4.2/examples/resalloc/expected/man/
--rw-r--r--   0 twine    (17125) twine    (17125)     1123 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/resalloc/expected/man/resalloc-maint.1
--rw-r--r--   0 twine    (17125) twine    (17125)     1351 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/resalloc/expected/man/resalloc.1
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/requirements.txt
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.388906 argparse-manpage-4.2/examples/resalloc/resalloc/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/resalloc/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       51 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/resalloc/client.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       23 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/resalloc/version.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.389906 argparse-manpage-4.2/examples/resalloc/resallocserver/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/resallocserver/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       27 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/resallocserver/maint.py
--rw-rw-r--   0 twine    (17125) twine    (17125)      146 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)     2241 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/setup.py
--rw-r--r--   0 twine    (17125) twine    (17125)      193 2023-05-14 10:57:58.000000 argparse-manpage-4.2/pyproject.toml
--rw-r--r--   0 twine    (17125) twine    (17125)      133 2023-05-14 10:58:16.390906 argparse-manpage-4.2/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)     1551 2023-05-14 10:57:58.000000 argparse-manpage-4.2/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.389906 argparse-manpage-4.2/tests/
--rw-r--r--   0 twine    (17125) twine    (17125)      849 2023-05-14 10:57:58.000000 argparse-manpage-4.2/tests/argparse_testlib.py
--rw-r--r--   0 twine    (17125) twine    (17125)       80 2023-04-15 19:13:21.000000 argparse-manpage-4.2/tests/extra.man
--rw-r--r--   0 twine    (17125) twine    (17125)     2010 2022-10-31 08:33:07.000000 argparse-manpage-4.2/tests/test_basic.py
--rw-r--r--   0 twine    (17125) twine    (17125)     7299 2023-05-14 10:57:58.000000 argparse-manpage-4.2/tests/test_examples.py
--rw-r--r--   0 twine    (17125) twine    (17125)     6098 2023-05-14 10:57:58.000000 argparse-manpage-4.2/tests/test_script.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.970826 argparse-manpage-4.3/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      136 2019-09-07 00:39:54.000000 argparse-manpage-4.3/AUTHORS
+-rw-rw-r--   0 twine    (17125) twine    (17125)    11357 2019-09-07 00:39:54.000000 argparse-manpage-4.3/LICENSE
+-rw-r--r--   0 twine    (17125) twine    (17125)      649 2023-05-14 10:57:58.000000 argparse-manpage-4.3/MANIFEST.in
+-rw-r--r--   0 twine    (17125) twine    (17125)     5007 2023-05-17 13:02:57.000000 argparse-manpage-4.3/NEWS
+-rw-r--r--   0 twine    (17125) twine    (17125)     8915 2023-05-17 13:03:01.970826 argparse-manpage-4.3/PKG-INFO
+-rw-r--r--   0 twine    (17125) twine    (17125)     8472 2023-05-14 10:57:58.000000 argparse-manpage-4.3/README.md
+-rwxr-xr-x   0 twine    (17125) twine    (17125)      357 2022-10-31 08:33:07.000000 argparse-manpage-4.3/argparse-manpage
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.964825 argparse-manpage-4.3/argparse_manpage/
+-rw-r--r--   0 twine    (17125) twine    (17125)       54 2023-05-17 13:02:57.000000 argparse-manpage-4.3/argparse_manpage/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     3589 2023-05-14 10:57:58.000000 argparse-manpage-4.3/argparse_manpage/cli.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1669 2023-05-14 10:57:58.000000 argparse-manpage-4.3/argparse_manpage/compat.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    21556 2023-05-14 10:57:58.000000 argparse-manpage-4.3/argparse_manpage/manpage.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     2326 2022-10-31 08:33:07.000000 argparse-manpage-4.3/argparse_manpage/tooling.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.965825 argparse-manpage-4.3/argparse_manpage.egg-info/
+-rw-rw-r--   0 twine    (17125) twine    (17125)     8915 2023-05-17 13:03:01.000000 argparse-manpage-4.3/argparse_manpage.egg-info/PKG-INFO
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2605 2023-05-17 13:03:01.000000 argparse-manpage-4.3/argparse_manpage.egg-info/SOURCES.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)        1 2023-05-17 13:03:01.000000 argparse-manpage-4.3/argparse_manpage.egg-info/dependency_links.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)       63 2023-05-17 13:03:01.000000 argparse-manpage-4.3/argparse_manpage.egg-info/entry_points.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)       59 2023-05-17 13:03:01.000000 argparse-manpage-4.3/argparse_manpage.egg-info/requires.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)       32 2023-05-17 13:03:01.000000 argparse-manpage-4.3/argparse_manpage.egg-info/top_level.txt
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.965825 argparse-manpage-4.3/build_manpages/
+-rw-r--r--   0 twine    (17125) twine    (17125)      169 2022-10-31 08:33:07.000000 argparse-manpage-4.3/build_manpages/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     7364 2023-04-15 19:13:21.000000 argparse-manpage-4.3/build_manpages/build_manpage.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     6363 2023-05-17 13:02:57.000000 argparse-manpage-4.3/build_manpages/build_manpages.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      980 2022-10-31 08:33:07.000000 argparse-manpage-4.3/build_manpages/compat.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      157 2022-10-31 08:33:07.000000 argparse-manpage-4.3/build_manpages/manpage.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.963825 argparse-manpage-4.3/examples/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.965825 argparse-manpage-4.3/examples/argument_groups/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.965825 argparse-manpage-4.3/examples/argument_groups/bin/
+-rwxr-xr-x   0 twine    (17125) twine    (17125)     2250 2021-11-28 22:10:08.000000 argparse-manpage-4.3/examples/argument_groups/bin/test
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.966825 argparse-manpage-4.3/examples/argument_groups/expected/
+-rw-r--r--   0 twine    (17125) twine    (17125)     2125 2023-04-15 19:13:21.000000 argparse-manpage-4.3/examples/argument_groups/expected/test.1
+-rw-r--r--   0 twine    (17125) twine    (17125)      115 2022-10-31 08:33:07.000000 argparse-manpage-4.3/examples/argument_groups/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      984 2021-11-28 22:10:08.000000 argparse-manpage-4.3/examples/argument_groups/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.966825 argparse-manpage-4.3/examples/copr/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.966825 argparse-manpage-4.3/examples/copr/copr_cli/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/copr_cli/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/copr_cli/build_config.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    49234 2022-10-31 08:33:07.000000 argparse-manpage-4.3/examples/copr/copr_cli/main.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/copr_cli/util.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    26531 2023-04-15 19:13:21.000000 argparse-manpage-4.3/examples/copr/expected-output.1
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.966825 argparse-manpage-4.3/examples/copr/fake-deps/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/fake-deps/HACK
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.967826 argparse-manpage-4.3/examples/copr/fake-deps/copr/
+-rw-rw-r--   0 twine    (17125) twine    (17125)       35 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/fake-deps/copr/README
+-rw-rw-r--   0 twine    (17125) twine    (17125)       43 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/fake-deps/copr/__init__.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.967826 argparse-manpage-4.3/examples/copr/fake-deps/copr/client/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/fake-deps/copr/client/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       29 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/fake-deps/copr/client/responses.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/fake-deps/copr/exceptions.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       28 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/fake-deps/jinja2.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/fake-deps/simplejson.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      113 2022-10-31 08:33:07.000000 argparse-manpage-4.3/examples/copr/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)      965 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/copr/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.967826 argparse-manpage-4.3/examples/old_format/
+-rw-r--r--   0 twine    (17125) twine    (17125)      917 2022-01-12 01:47:25.000000 argparse-manpage-4.3/examples/old_format/README.md
+-rw-rw-r--   0 twine    (17125) twine    (17125)      519 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/old_format/example.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      503 2023-04-15 19:13:21.000000 argparse-manpage-4.3/examples/old_format/expected-output.1
+-rw-rw-r--   0 twine    (17125) twine    (17125)       59 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/old_format/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)      789 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/old_format/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.968825 argparse-manpage-4.3/examples/old_format_file_name/
+-rw-r--r--   0 twine    (17125) twine    (17125)      585 2022-01-12 01:47:25.000000 argparse-manpage-4.3/examples/old_format_file_name/README.md
+-rw-r--r--   0 twine    (17125) twine    (17125)      519 2022-01-12 01:47:25.000000 argparse-manpage-4.3/examples/old_format_file_name/example.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      503 2023-04-15 19:13:21.000000 argparse-manpage-4.3/examples/old_format_file_name/expected-output.1
+-rw-r--r--   0 twine    (17125) twine    (17125)       82 2022-01-12 01:47:25.000000 argparse-manpage-4.3/examples/old_format_file_name/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      789 2022-01-12 01:47:25.000000 argparse-manpage-4.3/examples/old_format_file_name/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.968825 argparse-manpage-4.3/examples/osc/
+-rw-r--r--   0 twine    (17125) twine    (17125)     2246 2023-04-15 19:13:21.000000 argparse-manpage-4.3/examples/osc/expected-output.1
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.968825 argparse-manpage-4.3/examples/osc/osc/
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2022-04-27 06:51:30.000000 argparse-manpage-4.3/examples/osc/osc/__init__.py
+-rwxr-xr-x   0 twine    (17125) twine    (17125)     4636 2022-10-31 08:33:07.000000 argparse-manpage-4.3/examples/osc/osc/main.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      251 2022-10-31 08:33:07.000000 argparse-manpage-4.3/examples/osc/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      772 2022-04-27 06:51:30.000000 argparse-manpage-4.3/examples/osc/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.968825 argparse-manpage-4.3/examples/pre-written-man-page/
+-rw-r--r--   0 twine    (17125) twine    (17125)      871 2023-05-14 10:57:58.000000 argparse-manpage-4.3/examples/pre-written-man-page/psutils.1
+-rw-r--r--   0 twine    (17125) twine    (17125)       60 2023-05-14 10:57:58.000000 argparse-manpage-4.3/examples/pre-written-man-page/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      272 2023-05-14 10:57:58.000000 argparse-manpage-4.3/examples/pre-written-man-page/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.968825 argparse-manpage-4.3/examples/raw-description/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.969825 argparse-manpage-4.3/examples/raw-description/bin/
+-rwxrwxr-x   0 twine    (17125) twine    (17125)     4455 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/raw-description/bin/dg
+-rw-r--r--   0 twine    (17125) twine    (17125)     2035 2023-04-15 19:13:21.000000 argparse-manpage-4.3/examples/raw-description/expected-output.1
+-rw-rw-r--   0 twine    (17125) twine    (17125)       69 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/raw-description/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)      982 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/raw-description/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.969825 argparse-manpage-4.3/examples/resalloc/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.969825 argparse-manpage-4.3/examples/resalloc/bin/
+-rwxrwxr-x   0 twine    (17125) twine    (17125)     3076 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/resalloc/bin/resalloc
+-rwxrwxr-x   0 twine    (17125) twine    (17125)     2070 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/resalloc/bin/resalloc-maint
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.963825 argparse-manpage-4.3/examples/resalloc/expected/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.969825 argparse-manpage-4.3/examples/resalloc/expected/man/
+-rw-r--r--   0 twine    (17125) twine    (17125)     1123 2023-04-15 19:13:21.000000 argparse-manpage-4.3/examples/resalloc/expected/man/resalloc-maint.1
+-rw-r--r--   0 twine    (17125) twine    (17125)     1351 2023-04-15 19:13:21.000000 argparse-manpage-4.3/examples/resalloc/expected/man/resalloc.1
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/resalloc/requirements.txt
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.969825 argparse-manpage-4.3/examples/resalloc/resalloc/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/resalloc/resalloc/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       51 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/resalloc/resalloc/client.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       23 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/resalloc/resalloc/version.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.970826 argparse-manpage-4.3/examples/resalloc/resallocserver/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/resalloc/resallocserver/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       27 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/resalloc/resallocserver/maint.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)      146 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/resalloc/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2241 2019-09-07 00:39:54.000000 argparse-manpage-4.3/examples/resalloc/setup.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      257 2023-05-17 13:02:57.000000 argparse-manpage-4.3/pyproject.toml
+-rw-r--r--   0 twine    (17125) twine    (17125)      133 2023-05-17 13:03:01.970826 argparse-manpage-4.3/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)     1552 2023-05-17 13:02:57.000000 argparse-manpage-4.3/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-17 13:03:01.970826 argparse-manpage-4.3/tests/
+-rw-r--r--   0 twine    (17125) twine    (17125)      849 2023-05-14 10:57:58.000000 argparse-manpage-4.3/tests/argparse_testlib.py
+-rw-r--r--   0 twine    (17125) twine    (17125)       80 2023-04-15 19:13:21.000000 argparse-manpage-4.3/tests/extra.man
+-rw-r--r--   0 twine    (17125) twine    (17125)     2010 2022-10-31 08:33:07.000000 argparse-manpage-4.3/tests/test_basic.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     7299 2023-05-14 10:57:58.000000 argparse-manpage-4.3/tests/test_examples.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     6098 2023-05-14 10:57:58.000000 argparse-manpage-4.3/tests/test_script.py
```

### Comparing `argparse-manpage-4.2/LICENSE` & `argparse-manpage-4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/MANIFEST.in` & `argparse-manpage-4.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/NEWS` & `argparse-manpage-4.3/NEWS`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 WARNING: The 'build_manpage' setup.py command will be removed v5
 WARNING: We'll drop the Python 2.7 support in v5
 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+News in v4.3
+
+* The pyproject.toml parsing feature now depends on the python3-tomli library
+  instead of python-toml for "python_environment >3, <=3.10".
+
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 News in v4.2
 
 * Support for pyproject.toml specification of manpages added.
 
 * Support for pre-written man pages (the --manfile option)
 
 Bugfixes in version 4.2
```

### Comparing `argparse-manpage-4.2/PKG-INFO` & `argparse-manpage-4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-manpage
-Version: 4.2
+Version: 4.3
 Summary: Build manual page from python's ArgumentParser object.
 Home-page: https://github.com/praiskup/argparse-manpage
 Author: Gabriele Giammatteo
 Author-email: gabriele.giammatteo@eng.it
 Maintainer: Pavel Raiskup
 Maintainer-email: praiskup@redhat.com
 License: Apache 2.0
```

### Comparing `argparse-manpage-4.2/README.md` & `argparse-manpage-4.3/README.md`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/argparse_manpage/cli.py` & `argparse-manpage-4.3/argparse_manpage/cli.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/argparse_manpage/compat.py` & `argparse-manpage-4.3/argparse_manpage/compat.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/argparse_manpage/manpage.py` & `argparse-manpage-4.3/argparse_manpage/manpage.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/argparse_manpage/tooling.py` & `argparse-manpage-4.3/argparse_manpage/tooling.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/argparse_manpage.egg-info/PKG-INFO` & `argparse-manpage-4.3/argparse_manpage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-manpage
-Version: 4.2
+Version: 4.3
 Summary: Build manual page from python's ArgumentParser object.
 Home-page: https://github.com/praiskup/argparse-manpage
 Author: Gabriele Giammatteo
 Author-email: gabriele.giammatteo@eng.it
 Maintainer: Pavel Raiskup
 Maintainer-email: praiskup@redhat.com
 License: Apache 2.0
```

### Comparing `argparse-manpage-4.2/argparse_manpage.egg-info/SOURCES.txt` & `argparse-manpage-4.3/argparse_manpage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/build_manpages/build_manpage.py` & `argparse-manpage-4.3/build_manpages/build_manpage.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/build_manpages/build_manpages.py` & `argparse-manpage-4.3/build_manpages/build_manpages.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 import os
 import shutil
 
 try:
     import tomllib
     from tomllib import TOMLDecodeError
 except ImportError:
-    import toml as tomllib
-    from toml import TomlDecodeError as TOMLDecodeError
+    try:
+        import tomli as tomllib
+        from tomli import TOMLDecodeError
+    except ImportError:
+        import toml as tomllib
+        from toml import TomlDecodeError as TOMLDecodeError
 
 from argparse_manpage.compat import ConfigParser, NoSectionError
 from argparse_manpage.tooling import get_parser, write_to_filename
 from argparse_manpage.manpage import (
     Manpage,
     MANPAGE_DATA_ATTRS,
     get_manpage_data_from_distribution,
```

### Comparing `argparse-manpage-4.2/build_manpages/compat.py` & `argparse-manpage-4.3/build_manpages/compat.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/argument_groups/bin/test` & `argparse-manpage-4.3/examples/argument_groups/bin/test`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/argument_groups/expected/test.1` & `argparse-manpage-4.3/examples/argument_groups/expected/test.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/argument_groups/setup.py` & `argparse-manpage-4.3/examples/argument_groups/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/copr/copr_cli/build_config.py` & `argparse-manpage-4.3/examples/copr/copr_cli/build_config.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/copr/copr_cli/main.py` & `argparse-manpage-4.3/examples/copr/copr_cli/main.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/copr/copr_cli/util.py` & `argparse-manpage-4.3/examples/copr/copr_cli/util.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/copr/expected-output.1` & `argparse-manpage-4.3/examples/copr/expected-output.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/copr/setup.py` & `argparse-manpage-4.3/examples/copr/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/old_format/README.md` & `argparse-manpage-4.3/examples/old_format/README.md`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/old_format/example.py` & `argparse-manpage-4.3/examples/old_format/example.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/old_format/setup.py` & `argparse-manpage-4.3/examples/old_format/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/old_format_file_name/README.md` & `argparse-manpage-4.3/examples/old_format_file_name/README.md`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/old_format_file_name/example.py` & `argparse-manpage-4.3/examples/old_format_file_name/example.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/old_format_file_name/setup.py` & `argparse-manpage-4.3/examples/old_format_file_name/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/osc/expected-output.1` & `argparse-manpage-4.3/examples/osc/expected-output.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/osc/osc/main.py` & `argparse-manpage-4.3/examples/osc/osc/main.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/osc/setup.py` & `argparse-manpage-4.3/examples/osc/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/pre-written-man-page/psutils.1` & `argparse-manpage-4.3/examples/pre-written-man-page/psutils.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/raw-description/bin/dg` & `argparse-manpage-4.3/examples/raw-description/bin/dg`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/raw-description/expected-output.1` & `argparse-manpage-4.3/examples/raw-description/expected-output.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/raw-description/setup.py` & `argparse-manpage-4.3/examples/raw-description/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/resalloc/bin/resalloc` & `argparse-manpage-4.3/examples/resalloc/bin/resalloc`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/resalloc/bin/resalloc-maint` & `argparse-manpage-4.3/examples/resalloc/bin/resalloc-maint`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/resalloc/expected/man/resalloc-maint.1` & `argparse-manpage-4.3/examples/resalloc/expected/man/resalloc-maint.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/resalloc/expected/man/resalloc.1` & `argparse-manpage-4.3/examples/resalloc/expected/man/resalloc.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/examples/resalloc/setup.py` & `argparse-manpage-4.3/examples/resalloc/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/setup.py` & `argparse-manpage-4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 def get_readme():
     with open(os.path.join(ROOT_DIR, 'README.md')) as fh:
         return ''.join(fh.readlines())
 
 if sys.version_info >= (3,):
-    install_requires = ['toml;python_version<"3.11"']
+    install_requires = ['tomli;python_version<"3.11"']
 else:
     install_requires = ['toml']
 
 setup(
     name='argparse-manpage',
     version=__version__,
     url='https://github.com/praiskup/argparse-manpage',
```

### Comparing `argparse-manpage-4.2/tests/argparse_testlib.py` & `argparse-manpage-4.3/tests/argparse_testlib.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/tests/test_basic.py` & `argparse-manpage-4.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/tests/test_examples.py` & `argparse-manpage-4.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.2/tests/test_script.py` & `argparse-manpage-4.3/tests/test_script.py`

 * *Files identical despite different names*

