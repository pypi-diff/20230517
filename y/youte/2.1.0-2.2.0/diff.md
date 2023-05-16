# Comparing `tmp/youte-2.1.0.tar.gz` & `tmp/youte-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youte-2.1.0.tar", last modified: Fri Apr 14 06:04:13 2023, max compression
+gzip compressed data, was "youte-2.2.0.tar", last modified: Tue May 16 23:01:01 2023, max compression
```

## Comparing `youte-2.1.0.tar` & `youte-2.2.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.119552 youte-2.1.0/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1858 2023-02-16 01:17:30.000000 youte-2.1.0/.gitignore
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      198 2023-03-20 05:21:27.000000 youte-2.1.0/.readthedocs.yaml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    18508 2023-04-14 05:35:56.000000 youte-2.1.0/CHANGELOG.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1081 2022-06-06 05:38:09.000000 youte-2.1.0/LICENCE
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    16080 2023-04-14 06:04:13.119552 youte-2.1.0/PKG-INFO
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    15542 2023-04-14 05:35:56.000000 youte-2.1.0/README.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.111552 youte-2.1.0/docs/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    14689 2023-04-14 05:35:56.000000 youte-2.1.0/docs/documentation.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.115552 youte-2.1.0/docs/images/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    23688 2023-02-16 01:17:30.000000 youte-2.1.0/docs/images/youte-logo-black-transparent.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     7979 2023-02-16 01:17:30.000000 youte-2.1.0/docs/images/youte-logo-white-transparent-1x.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    24570 2023-02-16 01:17:30.000000 youte-2.1.0/docs/images/youte-logo-white-transparent.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    82963 2023-03-14 23:29:14.000000 youte-2.1.0/docs/images/youte_save_progress.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)   762396 2023-03-17 03:28:46.000000 youte-2.1.0/docs/images/youte_search_results.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)   183270 2023-03-17 03:37:54.000000 youte-2.1.0/docs/images/youte_search_results_pretty.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3297 2023-02-16 01:17:30.000000 youte-2.1.0/docs/index.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)       56 2023-03-17 06:57:11.000000 youte-2.1.0/docs/reference.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.115552 youte-2.1.0/docs/stylesheets/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      163 2023-02-16 01:17:30.000000 youte-2.1.0/docs/stylesheets/extra.css
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    14669 2023-03-17 05:20:49.000000 youte-2.1.0/docs/tutorial.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1243 2023-03-16 23:52:53.000000 youte-2.1.0/mkdocs.yml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      430 2023-03-16 07:04:20.000000 youte-2.1.0/noxfile.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      231 2023-04-14 05:35:56.000000 youte-2.1.0/pyproject.toml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      572 2023-03-20 05:22:46.000000 youte-2.1.0/requirements-mkdocs.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1027 2023-04-14 06:04:13.119552 youte-2.1.0/setup.cfg
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1255 2023-04-14 05:35:56.000000 youte-2.1.0/setup.py
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.111552 youte-2.1.0/src/
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.115552 youte-2.1.0/src/youte/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        0 2022-06-06 05:58:14.000000 youte-2.1.0/src/youte/__init__.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1253 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/_logging.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      994 2023-03-16 07:04:20.000000 youte-2.1.0/src/youte/_typing.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    35928 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/cli.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    26225 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/collector.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1073 2023-03-16 07:04:20.000000 youte-2.1.0/src/youte/common.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1269 2023-03-16 07:04:20.000000 youte-2.1.0/src/youte/config.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    12937 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/database.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      499 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/exceptions.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    14406 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/parser.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3080 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/resources.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3747 2023-03-16 07:04:20.000000 youte-2.1.0/src/youte/utilities.py
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.115552 youte-2.1.0/src/youte.egg-info/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    16080 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/PKG-INFO
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1034 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/SOURCES.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        1 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/dependency_links.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)       42 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/entry_points.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      147 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/requires.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        6 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/top_level.txt
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.119552 youte-2.1.0/tests/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     2820 2023-04-14 05:35:56.000000 youte-2.1.0/tests/test_archive.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     8231 2023-04-14 05:35:56.000000 youte-2.1.0/tests/test_cli.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3210 2023-03-16 07:04:20.000000 youte-2.1.0/tests/test_collector.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     2555 2023-04-14 05:35:56.000000 youte-2.1.0/tests/test_parser.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:01:01.044942 youte-2.2.0/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1858 2023-02-16 01:17:30.000000 youte-2.2.0/.gitignore
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      198 2023-03-20 05:21:27.000000 youte-2.2.0/.readthedocs.yaml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    23186 2023-05-16 23:00:47.000000 youte-2.2.0/CHANGELOG.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1081 2022-06-06 05:38:09.000000 youte-2.2.0/LICENCE
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    16795 2023-05-16 23:01:01.044942 youte-2.2.0/PKG-INFO
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    16257 2023-05-16 23:00:47.000000 youte-2.2.0/README.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:01:01.028942 youte-2.2.0/docs/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    36412 2023-05-16 23:00:47.000000 youte-2.2.0/docs/documentation.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:01:01.040942 youte-2.2.0/docs/images/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    23688 2023-02-16 01:17:30.000000 youte-2.2.0/docs/images/youte-logo-black-transparent.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     7979 2023-02-16 01:17:30.000000 youte-2.2.0/docs/images/youte-logo-white-transparent-1x.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    24570 2023-02-16 01:17:30.000000 youte-2.2.0/docs/images/youte-logo-white-transparent.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    82963 2023-03-14 23:29:14.000000 youte-2.2.0/docs/images/youte_save_progress.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)   762396 2023-03-17 03:28:46.000000 youte-2.2.0/docs/images/youte_search_results.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)   183270 2023-03-17 03:37:54.000000 youte-2.2.0/docs/images/youte_search_results_pretty.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    67111 2023-05-15 01:12:17.000000 youte-2.2.0/docs/images/youte_thumbnail.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     4122 2023-05-16 23:00:47.000000 youte-2.2.0/docs/index.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)       56 2023-03-17 06:57:11.000000 youte-2.2.0/docs/reference.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:01:01.040942 youte-2.2.0/docs/stylesheets/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      163 2023-02-16 01:17:30.000000 youte-2.2.0/docs/stylesheets/extra.css
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    14669 2023-03-17 05:20:49.000000 youte-2.2.0/docs/tutorial.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1243 2023-05-15 01:12:12.000000 youte-2.2.0/mkdocs.yml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      430 2023-03-16 07:04:20.000000 youte-2.2.0/noxfile.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      231 2023-04-14 05:35:56.000000 youte-2.2.0/pyproject.toml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      572 2023-03-20 05:22:46.000000 youte-2.2.0/requirements-mkdocs.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1027 2023-05-16 23:01:01.044942 youte-2.2.0/setup.cfg
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1255 2023-05-16 23:00:47.000000 youte-2.2.0/setup.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:01:01.028942 youte-2.2.0/src/
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:01:01.040942 youte-2.2.0/src/youte/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        0 2023-04-27 05:21:18.000000 youte-2.2.0/src/youte/__init__.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1253 2023-04-14 05:35:56.000000 youte-2.2.0/src/youte/_logging.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      967 2023-05-16 23:00:47.000000 youte-2.2.0/src/youte/_typing.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    36959 2023-05-16 23:00:47.000000 youte-2.2.0/src/youte/cli.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    28835 2023-05-16 23:00:47.000000 youte-2.2.0/src/youte/collector.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1566 2023-05-16 23:00:47.000000 youte-2.2.0/src/youte/common.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1269 2023-03-16 07:04:20.000000 youte-2.2.0/src/youte/config.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    12937 2023-04-14 05:35:56.000000 youte-2.2.0/src/youte/database.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      359 2023-05-16 23:00:47.000000 youte-2.2.0/src/youte/exceptions.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    14908 2023-05-16 23:00:47.000000 youte-2.2.0/src/youte/parser.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3185 2023-05-16 23:00:47.000000 youte-2.2.0/src/youte/resources.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3747 2023-03-16 07:04:20.000000 youte-2.2.0/src/youte/utilities.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      189 2023-05-15 04:53:11.000000 youte-2.2.0/src/youte/version.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:01:01.044942 youte-2.2.0/src/youte.egg-info/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    16795 2023-05-16 23:01:01.000000 youte-2.2.0/src/youte.egg-info/PKG-INFO
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1087 2023-05-16 23:01:01.000000 youte-2.2.0/src/youte.egg-info/SOURCES.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        1 2023-05-16 23:01:01.000000 youte-2.2.0/src/youte.egg-info/dependency_links.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)       42 2023-05-16 23:01:01.000000 youte-2.2.0/src/youte.egg-info/entry_points.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      147 2023-05-16 23:01:01.000000 youte-2.2.0/src/youte.egg-info/requires.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        6 2023-05-16 23:01:01.000000 youte-2.2.0/src/youte.egg-info/top_level.txt
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:01:01.044942 youte-2.2.0/tests/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     2820 2023-04-14 05:35:56.000000 youte-2.2.0/tests/test_archive.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     8449 2023-05-16 23:00:47.000000 youte-2.2.0/tests/test_cli.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3166 2023-05-16 23:00:47.000000 youte-2.2.0/tests/test_collector.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     2555 2023-04-14 05:35:56.000000 youte-2.2.0/tests/test_parser.py
```

### Comparing `youte-2.1.0/.gitignore` & `youte-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/CHANGELOG.md` & `youte-2.2.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,92 @@
 # Changelog
 
 <!-- insertion marker -->
-## Unreleased
+## [v2.2.0](https://github.com/QUT-Digital-Observatory/youte/releases/tag/v2.2.0) - 2023-05-16
 
-<small>[Compare with latest](https://github.com/QUT-Digital-Observatory/youte/compare/v2.1.0...HEAD)</small>
+<small>[Compare with v2.1.0](https://github.com/QUT-Digital-Observatory/youte/compare/v2.1.0...v2.2.0)</small>
+
+### Features
+
+- include metadata in parsers ([d5d79fe](https://github.com/QUT-Digital-Observatory/youte/commit/d5d79fe44c275facd9cfb0897272c38cde9ba7d8) by Boyd Nguyen).
+- add _youte metadata to returned output ([d87b97f](https://github.com/QUT-Digital-Observatory/youte/commit/d87b97fd2bc9f6092ed3bc4c55dc8d229ae4283c) by Boyd Nguyen).
+
+### Bug Fixes
+
+- fix None outdb when file doesn't exist ([802ab8f](https://github.com/QUT-Digital-Observatory/youte/commit/802ab8f2e97af9f161175bd2f6f9e41d74288aa8) by Boyd Nguyen).
+- fix KeyError in parse_video + parse_videos ([6fbbb70](https://github.com/QUT-Digital-Observatory/youte/commit/6fbbb70f320e58c4aa85c2700cecaf0bd36f91da) by Boyd Nguyen).
+
+## [v2.1.0](https://github.com/QUT-Digital-Observatory/youte/releases/tag/v2.1.0) - 2023-04-14
+
+<small>[Compare with v2.0.2](https://github.com/QUT-Digital-Observatory/youte/compare/v2.0.2...v2.1.0)</small>
+
+### Features
+
+- new 'full-archive' command ([dbaef5c](https://github.com/QUT-Digital-Observatory/youte/commit/dbaef5cf5ab9acf2b5c4eafa0b948f7f34c779ae) by Boyd Nguyen).
+
+### Bug Fixes
+
+- improve logging ([66a7b68](https://github.com/QUT-Digital-Observatory/youte/commit/66a7b68a4e77c34a05e0f4208fe62a00b9bd3182) by Boyd Nguyen).
+- use dict.get() to allow for nullable fields when parsing JSON ([3a2e8c9](https://github.com/QUT-Digital-Observatory/youte/commit/3a2e8c9db35639b31c1911da8b3d4b6905725802) by Boyd Nguyen).
+- avoid inputting error messages to output file ([4a186dc](https://github.com/QUT-Digital-Observatory/youte/commit/4a186dc2b91f2d859439e773dd1a2ec62c1e4af6) by Boyd Nguyen).
+- refine resource schema + make optional fields optional ([821bca9](https://github.com/QUT-Digital-Observatory/youte/commit/821bca98e1c237bffe90cb3f3356cefc74ab8987) by Boyd Nguyen).
+- fix KeyError in parse_video + parse_videos ([05ade72](https://github.com/QUT-Digital-Observatory/youte/commit/05ade72ddd7ce644b573069434db275fac105f98) by Boyd Nguyen).
+
+## [v2.0.2](https://github.com/QUT-Digital-Observatory/youte/releases/tag/v2.0.2) - 2023-03-31
+
+<small>[Compare with 2.0.1](https://github.com/QUT-Digital-Observatory/youte/compare/2.0.1...v2.0.2)</small>
+
+### Bug Fixes
+
+- fix KeyError in parse_video + parse_videos ([8e9d4fe](https://github.com/QUT-Digital-Observatory/youte/commit/8e9d4fe2385431e8fbb28bc94c1c27578cde4b2b) by Boyd Nguyen).
+
+## [2.0.1](https://github.com/QUT-Digital-Observatory/youte/releases/tag/2.0.1) - 2023-03-20
+
+<small>[Compare with 2.0.0](https://github.com/QUT-Digital-Observatory/youte/compare/2.0.0...2.0.1)</small>
+
+## [2.0.0](https://github.com/QUT-Digital-Observatory/youte/releases/tag/2.0.0) - 2023-03-16
+
+<small>[Compare with 1.3.0](https://github.com/QUT-Digital-Observatory/youte/compare/1.3.0...2.0.0)</small>
+
+## [1.3.0](https://github.com/QUT-Digital-Observatory/youte/releases/tag/1.3.0) - 2023-02-24
+
+<small>[Compare with 1.2.0](https://github.com/QUT-Digital-Observatory/youte/compare/1.2.0...1.3.0)</small>
+
+## [1.2.0](https://github.com/QUT-Digital-Observatory/youte/releases/tag/1.2.0) - 2023-02-07
+
+<small>[Compare with 1.1.0](https://github.com/QUT-Digital-Observatory/youte/compare/1.1.0...1.2.0)</small>
+
+## [1.1.0](https://github.com/QUT-Digital-Observatory/youte/releases/tag/1.1.0) - 2022-12-06
+
+<small>[Compare with 1.0.1](https://github.com/QUT-Digital-Observatory/youte/compare/1.0.1...1.1.0)</small>
+
+## [1.0.1](https://github.com/QUT-Digital-Observatory/youte/releases/tag/1.0.1) - 2022-12-01
+
+<small>[Compare with 1.0.0](https://github.com/QUT-Digital-Observatory/youte/compare/1.0.0...1.0.1)</small>
+
+## [1.0.0](https://github.com/QUT-Digital-Observatory/youte/releases/tag/1.0.0) - 2022-11-23
+
+<small>[Compare with 0.1.1](https://github.com/QUT-Digital-Observatory/youte/compare/0.1.1...1.0.0)</small>
+
+## [0.1.1](https://github.com/QUT-Digital-Observatory/youte/releases/tag/0.1.1) - 2022-10-10
+
+<small>[Compare with 0.1.0](https://github.com/QUT-Digital-Observatory/youte/compare/0.1.0...0.1.1)</small>
+
+## [0.1.0](https://github.com/QUT-Digital-Observatory/youte/releases/tag/0.1.0) - 2022-09-21
+
+<small>[Compare with 0.0.2](https://github.com/QUT-Digital-Observatory/youte/compare/0.0.2...0.1.0)</small>
+
+## [0.0.2](https://github.com/QUT-Digital-Observatory/youte/releases/tag/0.0.2) - 2022-09-07
+
+<small>[Compare with 0.0.1b](https://github.com/QUT-Digital-Observatory/youte/compare/0.0.1b...0.0.2)</small>
+
+## [0.0.1b](https://github.com/QUT-Digital-Observatory/youte/releases/tag/0.0.1b) - 2022-09-02
+
+<small>[Compare with first commit](https://github.com/QUT-Digital-Observatory/youte/compare/4562a2b20cdd68e305a4b51ebba3b02ba132665b...0.0.1b)</small>
 
-<!-- insertion marker -->
 ## [v2.1.0](https://github.com/QUT-Digital-Observatory/youte/releases/tag/v2.1.0) - 2023-04-14
 
 <small>[Compare with 2.0.1](https://github.com/QUT-Digital-Observatory/youte/compare/2.0.1...v2.1.0)</small>
 
 ### Added
 
 - add black to isort ([8d1f42c](https://github.com/QUT-Digital-Observatory/youte/commit/8d1f42c447bf6d5a5fa79b270b9507900658f078) by Boyd Nguyen).
```

### Comparing `youte-2.1.0/LICENCE` & `youte-2.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/PKG-INFO` & `youte-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: youte
-Version: 2.1.0
+Version: 2.2.0
 Summary: Command-line tool to collect video metadata and comments from Youtube API
 Home-page: https://github.com/QUT-Digital-Observatory/youte
 Author: Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/youte/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# youte 2.0
+# youte: A command-line tool to retrieve and tidy YouTube metadata and comments from YouTube Data API
 
-A command line utility to get YouTube video metadata and comments from YouTube Data API.
+[![PyPI Latest Release](https://img.shields.io/pypi/v/youte)](https://pypi.org/project/youte/)
+[![DOI](https://img.shields.io/badge/DOI-https%3A%2F%2Fdoi.org%2F10.25912%2FRDF__1684202566368-blue)](https://doi.org/10.25912/RDF_1684202566368)
+[![Downloads](https://static.pepy.tech/personalized-badge/youte?period=month&units=international_system&left_color=black&right_color=orange&left_text=Monthly%20PyPI%20downloads)](https://pepy.tech/project/youte)
+[![Licence](https://img.shields.io/github/license/QUT-Digital-Observatory/youte)](LICENCE)
+![Supported Versions](https://img.shields.io/pypi/pyversions/youte)
+![Development Status](https://img.shields.io/pypi/status/youte)
+
+![](docs/images/youte_thumbnail.png)
 
 ## Changes from youte 1.3.0
 
 Several major changes are made in youte 2.0. To better correspond with YouTube API endpoints and avoid confusion, some commands have been changed.
 
 - `youte hydrate` is now broken down to `youte videos` and `youte channels`.
 - `youte get-comments` is now `youte comments` and `youte replies`.
```

### Comparing `youte-2.1.0/README.md` & `youte-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
-# youte 2.0
+# youte: A command-line tool to retrieve and tidy YouTube metadata and comments from YouTube Data API
 
-A command line utility to get YouTube video metadata and comments from YouTube Data API.
+[![PyPI Latest Release](https://img.shields.io/pypi/v/youte)](https://pypi.org/project/youte/)
+[![DOI](https://img.shields.io/badge/DOI-https%3A%2F%2Fdoi.org%2F10.25912%2FRDF__1684202566368-blue)](https://doi.org/10.25912/RDF_1684202566368)
+[![Downloads](https://static.pepy.tech/personalized-badge/youte?period=month&units=international_system&left_color=black&right_color=orange&left_text=Monthly%20PyPI%20downloads)](https://pepy.tech/project/youte)
+[![Licence](https://img.shields.io/github/license/QUT-Digital-Observatory/youte)](LICENCE)
+![Supported Versions](https://img.shields.io/pypi/pyversions/youte)
+![Development Status](https://img.shields.io/pypi/status/youte)
+
+![](docs/images/youte_thumbnail.png)
 
 ## Changes from youte 1.3.0
 
 Several major changes are made in youte 2.0. To better correspond with YouTube API endpoints and avoid confusion, some commands have been changed.
 
 - `youte hydrate` is now broken down to `youte videos` and `youte channels`.
 - `youte get-comments` is now `youte comments` and `youte replies`.
```

### Comparing `youte-2.1.0/docs/documentation.md` & `youte-2.2.0/src/youte.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,102 +1,126 @@
----
-title: "youte documentation"
----
+Metadata-Version: 2.1
+Name: youte
+Version: 2.2.0
+Summary: Command-line tool to collect video metadata and comments from Youtube API
+Home-page: https://github.com/QUT-Digital-Observatory/youte
+Author: Digital Observatory
+Author-email: digitalobservatory@qut.edu.au
+Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/youte/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# youte: A command-line tool to retrieve and tidy YouTube metadata and comments from YouTube Data API
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/youte)](https://pypi.org/project/youte/)
+[![DOI](https://img.shields.io/badge/DOI-https%3A%2F%2Fdoi.org%2F10.25912%2FRDF__1684202566368-blue)](https://doi.org/10.25912/RDF_1684202566368)
+[![Downloads](https://static.pepy.tech/personalized-badge/youte?period=month&units=international_system&left_color=black&right_color=orange&left_text=Monthly%20PyPI%20downloads)](https://pepy.tech/project/youte)
+[![Licence](https://img.shields.io/github/license/QUT-Digital-Observatory/youte)](LICENCE)
+![Supported Versions](https://img.shields.io/pypi/pyversions/youte)
+![Development Status](https://img.shields.io/pypi/status/youte)
+
+![](docs/images/youte_thumbnail.png)
 
 ## Changes from youte 1.3.0
 
-Several major changes are made in youte 2.x. To better correspond with YouTube API endpoints and avoid confusion:
+Several major changes are made in youte 2.0. To better correspond with YouTube API endpoints and avoid confusion, some commands have been changed.
 
-- `youte hydrate` is now broken down to `youte videos` and `youte channels`, 
+- `youte hydrate` is now broken down to `youte videos` and `youte channels`.
 - `youte get-comments` is now `youte comments` and `youte replies`.
-- `youte most-popular` is now `youte chart`
-- `youte get-related` is now `youte related-to`
+- `youte most-popular` is now `youte chart`.
+- `youte get-related` is now `youte related-to`.
 
 Furthermore:
 
 - Resuming search is no longer available. Instead, you can set a limit on the number of search pages returned to avoid exhausting your API quota.
 - All youte commands that retrieve data from YouTube API now won't print results to the shell, but store them in a specified json or jsonl file. This is to avoid clogging up the shell.
+- You can now tidy data into a CSV or a flat JSON array.
+
+Big thanks to @Lingomat (Mat Bettinson) for code review and suggestions.
 
 ## Installation
 
-```shell
+```bash
 python -m pip install youte
-```
+```  
 
-## YouTube API key
+## YouTube API key  
 
 To get data from YouTube API, you will need a YouTube API key. Follow YouTube [instructions](https://developers.google.com/youtube/v3/getting-started) to obtain a YouTube API key if you do not already have one.
 
-## config
-
-### Store your API key
+## Configure API key (recommended)
 
-While API key can be passed straight to youte commands, you can save your API key in a youte config file for reuse. To do so, run:
+You can save your API key in the youte config file for reuse. To do so, run:
 
-```shell
+```bash  
 youte config add-key
-```
+```  
 
-In the interactive prompt, enter your API key and give it a name. The name is used to identify the key, and can be anything you choose.
+The interactive prompt will ask you to input your API key and name it. The name is used to identify the key, and can be anything you choose.
 
-You can also choose to set the key as default. When running queries, if no API key or name is specified, `youte` will automatically use the default key.
+The prompt will also ask if you want to set the given key as default.
 
-### See the list of all keys
+When running queries, if no API key or name is specified, `youte` will automatically use the default key.
 
-To see the list of all keys and their names stored in the config, run:
+### Manually set a key as default  
 
-```shell
-youte config list-keys
+If you want to manually set an existing key as a default, run:  
+
+```bash  
+youte config set-default <name-of-existing-key>
 ```
 
-The default key, if there is one, will have an asterisk next to it.
+Note that what is passed to this command is the _name_ of the API key, not the API key itself. It follows that the API key has to be first added to the config file using `youte config add-key`. If you use a name that has not been added to the config file, an error will be raised.
 
-### Manually set a key as default
+#### See the list of all keys  
 
-If you want to manually set an existing key as a default, run:
+To see the list of all keys, run:  
 
-```shell
-youte config set-default <name-of-existing-key>
-```
+```bash  
+youte config list-keys
+```  
 
-Note that what is passed to this command is the _name_ of the API key, not the API key itself. It follows that the API key has to be first added to the config file using `youte config add-key`. If you use a name that has not been added to the config file, an error will be raised.
+The default key, if there is one, will have an asterisk next to it.
 
-### Remove a key
+#### Remove a key
 
 To remove a stored key, run:
 
-```shell
+```bash
 youte config remove <name-of-key>
 ```
 
-### About the config file
+#### About the config file  
 
-youte's config file is stored in a central place whose exact location depends on the running operating system:
+youte's config file is stored in a central place whose exact location depends on the running operating system:  
 
-- Linux/Unix: ~/.config/youte/
+- Linux/Unix: ~/.config/youte/   
 - Mac OS X: ~/Library/Application Support/youte/
-- Windows: C:\Users\\\<user>\\AppData\\Roaming\\youte
+- Windows: C:\Users\\\<user>\\AppData\Roaming\youte
 
 ## search
 
 Searching can be as simple as:
 
 ```bash
 youte search <search-terms> --key <API-key> --outfile <name-of-file.json>
 # OR
 youte search <search-terms> --key <API-key> -o <name-of-file.json>
 ```
 
 If you have a default key set up using `youte config`, then there is no need to specify an API key using `--key`.
 
-This will return the maximum number of results pages (around 12-13) matching the search terms and store them in a JSON file. Unlike version 1.3, youte 2.0 does not print results to the terminal to avoid clogging it up. Instead, `--outfile` is now a required option. <search-terms> and `--outfile` must be specified. 
+This will return the maximum number of results pages (around 12-13) matching the search terms and store them in a JSON file. Unlike version 1.3, youte 2.0 does not print results to the terminal. Instead, `--outfile` is now a required option. <search-terms> and `--outfile` must be specified. 
 
 In the search terms, you can also use the Boolean NOT (-) and OR (|) operators to exclude videos or to find videos that match one of several search terms. If the terms contain spaces, the entire search term value has to be wrapped in quotes.
 
-Prettify JSON results by using the flag `--pretty`:
+Use the flag `--pretty` to pretty format the JSON output.
 
 ```bash
 youte search <search-terms> --key <API-key> --outfile <name-of-file> --pretty
 ```
 
 ### Limit pages returned
 
@@ -106,15 +130,15 @@
 youte search <search-terms> --max-pages 5
 # OR
 youte search <search-terms> -m 5
 ```
 
 ### Tidy data
 
-Raw JSONs from YouTube API contain query metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy raw JSON into will be CSV.
+Raw JSONs from YouTube API contain request metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy raw JSON into will be CSV.
 
 ```bash
 youte search <search-terms> --tidy-to <file.csv>
 ```
 
 Specify `--format json` if you want to tidy raw data into an array of flat JSON objects.
 
@@ -176,17 +200,17 @@
 youte search <search-terms> --limit 5 --type playlist,video
 ```
 
 #### Restrict by language and region
 
 The `--lang` returns results most relevant to a language. Not all results will be in the specified language: results in other languages will still be returned if they are highly relevant to the search query term. To specify the language, use [ISO 639-1 two letter code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes), except that you should use the values `zh-Hans` for simplified Chinese and `zh-Hant` for traditional Chinese.
 
-The `--region` returns results viewable in a region. It does *not* filter videos uploaded in that region only. To specify the region, use [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+The `--region` returns results viewable in a region. To specify the region, use [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2). Note that this option does *not* filter videos uploaded in that region, but rather videos that can be _viewed_ in that region.
 
-The `--location` and `--radius` options define a circular geographic area to filter videos that specify, in their metadata, a location within this area. This is *not* a robust and reliable way to geolocate YouTube videos, hence should be used with care.
+The `--location` and `--radius` options define a circular geographic area to filter videos that specify, in their metadata, a location within this area. This is *not* a robust and reliable way to geolocate YouTube videos, and hence should be used with care.
 
 -  `--location` takes in 2 values - the latitude/longitude coordinates that represent the centre of the area
 -  `--radius` specifies the maximum distance that the location associated with a video can be from that point for the video to still be included in the search results. It must be a number followed by a unit. Valid units are `m`, `km`, `ft`, and `mi`. For example, `1500m`, `5km`, `10000ft`, and `0.75mi`.
 
 Both `--location` and `--radius` have to be specified if they are to be used, otherwise an API error will be thrown.
 
 ### Sort results
@@ -234,55 +258,45 @@
 
 `youte comments` retrieves top-level comments (comment threads) on one or multiple videos or channels. It takes in a list of ids and a flag indicating which type these ids are (i.e. videos or channels).
 
 To retrieve comments on videos, specify the video ids and pass the `--by-video-id` or `-v` flag.
 
 ```shell
 youte comments <id>... --by-video-id --outfile <file.json>
-# OR
+#OR
 youte comments <id>... -v --outfile <file.json>
 ```
 
 To retrieve comments on channels, specify channel ids and pass the `--by-channel-id` or `-c` flag.
 
-```shell
+```bash
 youte comments <id>... --by-channel-id --outfile <file.json>
-# OR
+OR
 youte comments <id>... -c --outfile <file.json>
 ```
 
 If neither of the flags are specified, `youte comments` will assume the ids are thread ids and retrieve the full metadata for those threads.
 
-You can search within the threads and filter threads matching the search terms, by using the `--query` or `-q` option.
+You can search within the threads and filter threads that match the search terms, by using the `--query` or `-q` option.
 
-```shell
+```bash
 youte comments <ids>... -v --outfile <file.json> -q "search term"
 ```
 
 ## replies
 
 While `youte comments` only retrieve top-level comment threads, if those threads have replies, they can be retrieved using `youte replies`. `youte replies` takes a list of thread ids and return the replies to those threads.
 
 ```shell
 youte replies <ids>... --outfile <file.json>
 ```
 
-## chart
-
-`youte chart` retrieves the most popular videos in a region, specified by [ISO 3166-1 alpha-2 country codes](https://www.iso.org/obp/ui/#search). If no argument or option is given, it retrieves the most popular videos in the United States.
-
-For example:
-
-```shell
-youte chart <region-code> -o <file.json>
-```
-
 ## related-to
 
-`youte related-to` retrieves a list of videos related to a video.
+`related-to` retrieves videos related to a video.
 
 ```shell
 youte related-to <video-ids>... -o <file.json>
 ```
 
 If multiple video IDs are inputted, youte will iterate through each video ID separately, retrieving all related videos to each video, one by one.
 
@@ -294,14 +308,24 @@
                                   [default: none]
   --region TEXT                   Specify region the videos can be viewed in
                                   (ISO 3166-1 alpha-2 country code)
   --lang TEXT                     Return results most relevant to a language
                                   (ISO 639-1 two-letter code)
 ```
 
+## chart
+
+`youte chart` retrieves the most popular videos in a region, specified by [ISO 3166-1 alpha-2 country codes](https://www.iso.org/obp/ui/#search). If no argument or option is given, it retrieves the most popular videos in the United States.
+
+For example:
+
+```shell
+youte chart <region-code> -o <file.json>
+```
+
 ## full-archive
 
 A new feature added in `youte` 2.1.0 is the ability to run a full archive workflow in one command. `youte full-archive` runs `youte search`, then retrieving video and channel metadata for the search results, as well as getting comments and replies for those videos as well. All data are then tidied and stored in multiple tables in an SQLite database. 
 
 ```shell
 youte full-archive <query> [options] -o <name-of-database-file>
 ```
@@ -326,10 +350,20 @@
 ```
 
 ```{.shell .no-copy}
 Options:
   -o, --output FILENAME  Output text file to store IDs in
 ```
 
-## Debugging
+## YouTube API Quota system and youte handling of quota 
+
+Most often, there is a limit to how many requests you can make to YouTube API per day. YouTube Data API uses a quota system, whereby each request costs a number of units depending on the endpoint the request is made to.
+
+For example:  
+
+- search endpoint costs 100 units per request  
+- video, channel, commentThread, and comment endpoints each costs 1 unit per request  
+
+Free accounts get an API quota cap of 10,000 units per project per day, which resets at midnight Pacific Time.
+
+At present, you can only check your quota usage on the [Quotas](https://console.developers.google.com/iam-admin/quotas) page in the API Console. It is not possible to monitor quota usage via metadata returned in the API response. `youte` does not monitor quota usage.
 
-The `--verbosity` option, available for most `youte` commands, allows you to turn on debugging messages of the program. Simply specify `--verbosity DEBUG` to turn this mode on.
```

### Comparing `youte-2.1.0/docs/images/youte-logo-black-transparent.png` & `youte-2.2.0/docs/images/youte-logo-black-transparent.png`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/docs/images/youte-logo-white-transparent-1x.png` & `youte-2.2.0/docs/images/youte-logo-white-transparent-1x.png`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/docs/images/youte-logo-white-transparent.png` & `youte-2.2.0/docs/images/youte-logo-white-transparent.png`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/docs/images/youte_save_progress.png` & `youte-2.2.0/docs/images/youte_save_progress.png`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/docs/images/youte_search_results.png` & `youte-2.2.0/docs/images/youte_search_results.png`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/docs/images/youte_search_results_pretty.png` & `youte-2.2.0/docs/images/youte_search_results_pretty.png`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/docs/index.md` & `youte-2.2.0/docs/index.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 ---
 title: "youte"
 ---
 
+[![PyPI Latest Release](https://img.shields.io/pypi/v/youte)](https://pypi.org/project/youte/)
+[![DOI](https://img.shields.io/badge/DOI-https%3A%2F%2Fdoi.org%2F10.25912%2FRDF__1684202566368-blue)](https://doi.org/10.25912/RDF_1684202566368)
+[![Downloads](https://static.pepy.tech/personalized-badge/youte?period=month&units=international_system&left_color=black&right_color=orange&left_text=Monthly%20PyPI%20downloads)](https://pepy.tech/project/youte)
+[![Licence](https://img.shields.io/github/license/QUT-Digital-Observatory/youte)](LICENCE)
+![Supported Versions](https://img.shields.io/pypi/pyversions/youte)
+![Development Status](https://img.shields.io/pypi/status/youte)
+
 `youte` is a command-line tool that collects and tidies YouTube video metadata and comments from YouTube Data API v.3. At the moment, the tool supports collecting public data that does not require OAuth 2.0.
 
 `youte` can collect the following data:
 
 - search results
 - video metadata
 - channel metadata
 - comment threads and comments
 
 It does so while handling pagination and YouTube API's rate limits. `youte` also provides the functionality to tidy raw JSON data into tabular format, either in a CSV file or an SQLite database.
 
+![](images/youte_thumbnail.png)
+
 ## Installing `youte`
 
 If you have Python 3.8 and above installed, you can install `youte` with `pip`.
 
 ```shell
 python -m pip install youte
 ```
@@ -36,22 +45,22 @@
 
 Refer to [YouTube Data API's documentation](https://developers.google.com/youtube/v3/determine_quota_cost) for more details on the costs of each endpoint.
 
 Free accounts get an API quota cap of 10,000 units per project per day, which resets at midnight Pacific Time. You can complete an [Audit and Quota Extension form](https://developers.google.com/youtube/v3/guides/quota_and_compliance_audits) to request additional quota on top of your default allocation.
 
 At present, you can only check your quota usage on the Quotas page in the API Console. It is not possible to monitor quota usage via metadata returned in the API response.
 
-`youte` does not monitor quota usage. However, it handles errors when quota is exceeded by sleeping until quota reset time.
+`youte` does not monitor quota usage, so it's important to check your daily API quota before running potentially expensive commands such as `youte search` or `youte full-archive`.
 
 ## Data governance considerations
 
 Activities involving data collected from YouTube Data API (e.g. collecting, analysing, storing, sharing, and archiving) should be in accordance with [YouTube API Terms of Service](https://developers.google.com/youtube/terms/api-services-terms-of-service) and [Developer Policies](https://developers.google.com/youtube/terms/developer-policies).
 
 At the same time, it is best-practice data governance to consider data implications that might arise from using YouTube data. Refer to [this guide](https://www.digitalobservatory.net.au/data-governance-guide/) for a high-level list of data governance considerations.
 
 ## Other tools
 
 Google provides client libraries to interact with their APIs, including YouTube Data API: [https://developers.google.com/youtube/v3/libraries](https://developers.google.com/youtube/v3/libraries). The libraries are available in a number of programming languages such as Java, Python, and JavaScript.
 
 ## Feedback is welcome!
 
-`youte` is still in its infancy, and we are working to improve and expand its capabilities. Let us know your feedback or suggestions by creating GitHub issues or emailing us at [digitalobservatory@qut.edu.au](mailto:digitalobservatory@qut.edu.au).
+`youte` is still in its infancy, and we are working to improve and expand its capabilities. Let us know your feedback or suggestions by creating [GitHub issues](https://github.com/QUT-Digital-Observatory/youte/issues) or emailing us at [digitalobservatory@qut.edu.au](mailto:digitalobservatory@qut.edu.au).
```

### Comparing `youte-2.1.0/docs/tutorial.md` & `youte-2.2.0/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/mkdocs.yml` & `youte-2.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/requirements-mkdocs.txt` & `youte-2.2.0/requirements-mkdocs.txt`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/setup.cfg` & `youte-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/setup.py` & `youte-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 if __name__ == "__main__":
     setup(
         name="youte",
```

### Comparing `youte-2.1.0/src/youte/_logging.py` & `youte-2.2.0/src/youte/_logging.py`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/src/youte/_typing.py` & `youte-2.2.0/src/youte/_typing.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,31 +17,31 @@
     id: dict
     nextPageToken: str
     prevPageToken: str
     regionCode: str
     pageInfo: dict
     items: List[dict]
     related_to_video_id: NotRequired[str]
-    collection_time: datetime.datetime
+    _youte: NotRequired[dict]
 
 
 class StandardResult(TypedDict):
     kind: str
     etag: str
     nextPageToken: str
     pageInfo: dict
     items: List[dict]
-    collection_time: datetime.datetime
+    _youte: NotRequired[dict]
 
 
 class VideoChannelResult(TypedDict):
     kind: str
     etag: str
     id: dict
     nextPageToken: str
     prevPageToken: str
     pageInfo: dict
     items: List[dict]
-    collection_time: datetime.datetime
+    _youte: NotRequired[dict]
 
 
 APIResponse = Union[SearchResult, StandardResult, VideoChannelResult]
```

### Comparing `youte-2.1.0/src/youte/cli.py` & `youte-2.2.0/src/youte/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from __future__ import annotations
 
 import logging
 import sys
 from json.decoder import JSONDecodeError
 from pathlib import Path
 from typing import IO, Callable, Literal
+from warnings import simplefilter
 
 import click
 import click_log
 
 import youte.database as database
 import youte.parser as parser
 from youte._logging import MultiFormatter
@@ -27,17 +28,26 @@
 logging.getLogger("sqlalchemy.engine").setLevel(logging.WARNING)
 
 console_handler = logging.StreamHandler()
 console_handler.setFormatter(MultiFormatter())
 
 logger.addHandler(console_handler)
 
-API_KEY_OPTIONS = [
+simplefilter("always", DeprecationWarning)
+
+
+DEFAULT_OPTIONS = [
     click.option("--name", help="Specify an API key name added to youte config"),
     click.option("--key", help="Specify a YouTube API key"),
+    click.option(
+        "--metadata/--no-metadata",
+        default=True,
+        show_default=True,
+        help="Include/don't include metadata about when and how data was collected.",
+    ),
 ]
 
 OUTPUT_OPTIONS = [
     click.option(
         "-o",
         "--outfile",
         type=click.Path(),
@@ -63,17 +73,17 @@
         default="csv",
         help="Format data is parsed into. Can be 'json', 'jsonl', or 'csv'",
         show_default=True,
     ),
 ]
 
 
-def api_key_options(func) -> Callable:
+def default_options(func) -> Callable:
     """Decorator to include api key options for querying commands"""
-    for option in reversed(API_KEY_OPTIONS):
+    for option in reversed(DEFAULT_OPTIONS):
         func = option(func)
     return func
 
 
 def output_options(func) -> Callable:
     """Decorator to include output options"""
     for option in reversed(OUTPUT_OPTIONS):
@@ -105,25 +115,28 @@
                 f"Contains '{v}'. Accepted values are {accept_types}"
             )
     return value
 
 
 def _check_file_overwrite(ctx, param, value: str) -> Path:
     value = Path(value)
+
     if value.exists():
         try:
             if click.confirm(
                 f"'{value}' already exists. Keep writing to this file?", abort=True
             ):
                 return value
         except click.Abort:
             click.secho(
                 "Rerun this command and choose a different filename.", fg="green"
             )
             raise click.Abort
+    else:
+        return value
 
 
 # CLI argument set up:
 @click.group()
 @click.version_option()
 def youte():
     """
@@ -133,15 +146,15 @@
     pass
 
 
 @youte.command()
 @click.argument("query")
 @output_options
 @tidy_options
-@api_key_options
+@default_options
 @click.option(
     "--from", "from_", help="Start date (YYYY-MM-DD)", callback=_validate_date
 )
 @click.option("--to", help="End date (YYYY-MM-DD)", callback=_validate_date)
 @click.option(
     "--type",
     "type_",
@@ -273,14 +286,15 @@
     safe_search: Literal["none", "moderate", "strict"],
     location: tuple[float],
     radius: str,
     tidy_to: Path,
     format_: Literal["json", "csv"],
     max_pages: int,
     max_results: int,
+    metadata: bool,
 ) -> None:
     """Do a YouTube search
 
     Retrieve pages of results matching query and other search criteria.
 
     QUERY: The term to search for. You can also use the Boolean NOT (-) and OR (|)
     operators to exclude videos or to find videos matching one of several search terms.
@@ -310,14 +324,15 @@
             location=location,
             location_radius=radius,
             video_dimension=video_dimension,
             max_pages_retrieved=max_pages,
             max_result=max_results,
             video_license=video_license,
             channel_type=channel_type,
+            include_meta=metadata,
         )
     ]
 
     export_file(
         results, fp=outfile, file_format=output_format, pretty=pretty, ensure_ascii=True
     )
 
@@ -328,15 +343,15 @@
             parser.parse_searches(results).to_json(tidy_to)
 
 
 @youte.command()
 @click.argument("items", nargs=-1, required=False)
 @output_options
 @tidy_options
-@api_key_options
+@default_options
 @click.option("-f", "--file-path", help="Use IDs from file", default=None)
 @click.option(
     "--order",
     type=click.Choice(["time", "relevance"]),
     default="time",
     show_default=True,
     help="Specify how comment threads are sorted",
@@ -383,14 +398,15 @@
     key: str,
     file_path: Path,
     by_video_id: bool,
     by_channel_id: bool,
     tidy_to: Path,
     format_: Literal["json", "csv"],
     max_results: int,
+    metadata: bool,
 ) -> None:
     """Get YouTube comment threads (top-level comments)
 
     Retrieve comments in three ways:
     1) Get comment threads on a video or a list of videos, using video ids
     2) Get comment threads associated with a channel or a list of channels,
     including comments about the channels' videos, using channel ids
@@ -427,14 +443,15 @@
             video_ids=vid_ids,
             related_channel_ids=channel_ids,
             comment_ids=comment_ids,
             order=order,
             search_terms=query,
             text_format=text_format,
             max_results=max_results,
+            include_meta=metadata,
         )
     ]
 
     export_file(
         results, outfile, file_format=output_format, pretty=pretty, ensure_ascii=True
     )
 
@@ -445,15 +462,15 @@
             parser.parse_comments(results).to_json(tidy_to, pretty=pretty)
 
 
 @youte.command()
 @click.argument("items", nargs=-1, required=False)
 @output_options
 @tidy_options
-@api_key_options
+@default_options
 @click.option("-f", "--file-path", help="Use IDs from file", default=None)
 @click.option(
     "--text-format",
     type=click.Choice(["html", "plainText"]),
     default="html",
     show_default=True,
     help="Specify the text format of the returned data",
@@ -474,14 +491,15 @@
     text_format: Literal["html", "plainText"],
     name: str,
     key: str,
     file_path: Path,
     tidy_to: Path,
     format_: Literal["json", "csv"],
     max_results: int,
+    metadata: bool,
 ) -> None:
     """Get replies to comment threads
 
     ITEMS: ID(s) of comment thread
 
     You can use ids stored in a text file by using --file-path <FILENAME>. The file
     has to contain a line-separated list of ids, with no header.
@@ -490,15 +508,18 @@
     yob = Youte(api_key=api_key)
 
     ids = _read_ids(items, file_path)
 
     results = [
         result
         for result in yob.get_thread_replies(
-            thread_ids=ids, text_format=text_format, max_results=max_results
+            thread_ids=ids,
+            text_format=text_format,
+            max_results=max_results,
+            include_meta=metadata,
         )
     ]
 
     export_file(
         results, outfile, file_format=output_format, pretty=pretty, ensure_ascii=True
     )
 
@@ -509,15 +530,15 @@
             parser.parse_comments(results).to_json(tidy_to, pretty=pretty)
 
 
 @youte.command()
 @click.argument("items", nargs=-1, required=False)
 @output_options
 @tidy_options
-@api_key_options
+@default_options
 @click.option("-f", "--file-path", help="Get IDs from file", default=None)
 @click.option(
     "--max-results",
     type=click.IntRange(0, 50),
     help="Maximum number of results returned per page",
     default=50,
     show_default=True,
@@ -530,14 +551,15 @@
     pretty: bool,
     file_path: Path,
     name: str,
     key: str,
     tidy_to: Path,
     format_: Literal["json", "csv"],
     max_results: int,
+    metadata: bool,
 ) -> None:
     """Retrieve video metadata
 
     Get all metadata for one or multiple videos given their ids.
 
     ITEMS: ID(s) of videos
 
@@ -546,15 +568,18 @@
     """
     api_key = key if key else _get_api_key(name=name)
     yob = Youte(api_key=api_key)
 
     ids = _read_ids(string=items, file=file_path)
 
     results = [
-        result for result in yob.get_video_metadata(ids, max_results=max_results)
+        result
+        for result in yob.get_video_metadata(
+            ids, max_results=max_results, include_meta=metadata
+        )
     ]
 
     export_file(
         results, outfile, file_format=output_format, pretty=pretty, ensure_ascii=True
     )
 
     if tidy_to:
@@ -564,15 +589,15 @@
             parser.parse_videos(results).to_json(tidy_to, pretty=pretty)
 
 
 @youte.command()
 @click.argument("items", nargs=-1, required=False)
 @output_options
 @tidy_options
-@api_key_options
+@default_options
 @click.option("-f", "--file-path", help="Get IDs from file", default=None)
 @click.option(
     "--max-results",
     type=click.IntRange(0, 50),
     help="Maximum number of results returned per page",
     default=50,
     show_default=True,
@@ -585,14 +610,15 @@
     pretty: bool,
     file_path: Path,
     name: str,
     key: str,
     tidy_to: Path,
     format_: Literal["json", "csv"],
     max_results: int,
+    metadata: bool,
 ) -> None:
     """Retrieve channel metadata
 
     Get all metadata for one or multiple channels given their ids.
 
     ITEMS: ID(s) of channels
 
@@ -601,33 +627,36 @@
     """
     api_key = key if key else _get_api_key(name=name)
     yob = Youte(api_key=api_key)
 
     ids = _read_ids(string=items, file=file_path)
 
     results = [
-        result for result in yob.get_channel_metadata(ids=ids, max_results=max_results)
+        result
+        for result in yob.get_channel_metadata(
+            ids=ids, max_results=max_results, include_meta=metadata
+        )
     ]
 
     export_file(
         results, outfile, file_format=output_format, pretty=pretty, ensure_ascii=True
     )
 
     if tidy_to:
         if format_ == "csv":
             parser.parse_channels(results).to_csv(tidy_to)
         elif format_ == "json":
             parser.parse_channels(results).to_json(tidy_to, pretty=pretty)
 
 
-@youte.command()
+@youte.command(deprecated=True)
 @click.argument("items", nargs=-1, required=False)
 @output_options
 @tidy_options
-@api_key_options
+@default_options
 @click.option(
     "-f", "--file-path", type=click.Path(), help="Get IDs from file", default=None
 )
 @click.option(
     "--safe-search",
     type=click.Choice(["none", "moderate", "strict"], case_sensitive=False),
     help="Include or exclude restricted content",
@@ -668,14 +697,15 @@
     file_path: str,
     name: str,
     key: str,
     max_results: int,
     max_pages: int,
     tidy_to: Path,
     format_: Literal["json", "csv"],
+    metadata: bool,
 ):
     """Get videos related to a video
 
     Retrieve a list of videos related to a video using video id. If multiple ids are
     specified, this will iterate over them and retrieve related videos for each of the
     videos separately.
 
@@ -691,14 +721,15 @@
         for result in yob.get_related_videos(
             video_ids=ids,
             region=region,
             relevance_language=lang,
             safe_search=safe_search,
             max_results=max_results,
             max_pages_retrieved=max_pages,
+            include_meta=metadata,
         )
     ]
 
     export_file(
         results, outfile, file_format=output_format, pretty=pretty, ensure_ascii=True
     )
 
@@ -709,15 +740,15 @@
             parser.parse_searches(results).to_json(tidy_to)
 
 
 @youte.command()
 @click.argument("region_code", default="us")
 @output_options
 @tidy_options
-@api_key_options
+@default_options
 @click.option(
     "--video-category",
     help="Video category ID for which the most popular videos should be retrieved",
 )
 @click.option(
     "--max-results",
     type=click.IntRange(0, 50),
@@ -733,14 +764,15 @@
     pretty: bool,
     video_category: str,
     name: str,
     key: str,
     tidy_to: Path,
     format_: Literal["json", "jsonl", "csv"],
     max_results: int,
+    metadata: bool,
 ):
     """Return the most popular videos for a region and video category
 
     By default, if nothing is else is provided, the command retrieves the most
     popular videos in the US.
 
     REGION_CODE: ISO 3166-1 alpha-2 country codes to retrieve videos, default "us"
@@ -751,14 +783,15 @@
 
     results = [
         result
         for result in yob.get_most_popular(
             region_code=region_code,
             video_category_id=video_category,
             max_results=max_results,
+            include_meta=metadata,
         )
     ]
 
     export_file(
         results, outfile, file_format=output_format, pretty=pretty, ensure_ascii=True
     )
 
@@ -806,16 +839,17 @@
 )
 @click.option(
     "--out-db",
     "-o",
     help="Name of SQLite database to store output (must have .db ending)",
     type=click.Path(),
     callback=_check_file_overwrite,
+    required=True,
 )
-@api_key_options
+@default_options
 @click.option(
     "--from", "from_", help="Start date (YYYY-MM-DD)", callback=_validate_date
 )
 @click.option("--to", help="End date (YYYY-MM-DD)", callback=_validate_date)
 @click.option(
     "--type",
     "type_",
@@ -944,14 +978,15 @@
     video_embeddable: Literal["any", "true"],
     video_license: Literal["any", "creativeCommon", "youtube"],
     safe_search: Literal["none", "moderate", "strict"],
     location: tuple[float],
     radius: str,
     max_pages: int,
     max_results: int,
+    metadata: bool,
 ) -> None:
     """Run full archive workflow
 
     Extract all related metadata of videos found from a search. This command combines
     `youte search`, `youte videos`, `youte channels`, `youte comments` and
     `youte replies` in one clean workflow. Data are cleaned and stored in an SQlite
     database.
@@ -962,15 +997,14 @@
     A useful option is `--select`, where you specify which resource types to
     archive. It can be one or a comma-separated list containing 'video', 'channel',
     'thread', and 'reply'. Comment thread replies are retrieved using thread IDs,
     thus collecting comment threads is a must before getting replies. Because of that,
     if you want to archive the replies, both 'thread' and 'reply' will have to be
     specified.
     """
-
     _check_compatibility(select)
 
     api_key = key if key else _get_api_key(name=name)
     yob = Youte(api_key=api_key)
 
     results = [
         result
@@ -991,49 +1025,58 @@
             location=location,
             location_radius=radius,
             video_dimension=video_dimension,
             max_pages_retrieved=max_pages,
             max_result=max_results,
             video_license=video_license,
             channel_type=channel_type,
+            include_meta=metadata,
         )
     ]
 
     searches = parser.parse_searches(results)
 
     engine = database.set_up_database(out_db)
     database.populate_searches(engine, [searches])
 
     video_ids = [s.id for s in searches.items]
     channel_ids = [s.channel_id for s in searches.items]
 
     if "video" in select:
         click.echo("Retrieving video metadata")
         click.echo(f"{len(video_ids)} videos being retrieved")
-        results = [result for result in yob.get_video_metadata(video_ids)]
+        results = [
+            result
+            for result in yob.get_video_metadata(video_ids, include_meta=metadata)
+        ]
         _videos = parser.parse_videos(results)
         database.populate_videos(engine, [_videos])
 
     if "channel" in select:
         click.echo("Retrieving channel metadata")
         click.echo(f"{len(channel_ids)} channels being retrieved")
-        results = [result for result in yob.get_channel_metadata(channel_ids)]
+        results = [
+            result
+            for result in yob.get_channel_metadata(channel_ids, include_meta=metadata)
+        ]
         _channels = parser.parse_channels(results)
         database.populate_channels(engine, [_channels])
 
     if "thread" in select:
         click.echo("Retrieving comment threads")
-        results = [r for r in yob.get_comment_threads(video_ids)]
+        results = [r for r in yob.get_comment_threads(video_ids, include_meta=metadata)]
         _comments = parser.parse_comments(results)
 
         database.populate_comments(engine, [_comments])
 
         if "reply" in select:
             thread_ids = [c.id for c in _comments.items if c.total_reply_count > 0]
-            results = [r for r in yob.get_thread_replies(thread_ids)]
+            results = [
+                r for r in yob.get_thread_replies(thread_ids, include_meta=metadata)
+            ]
             _replies = parser.parse_comments(results)
             database.populate_comments(engine, [_replies])
 
     click.secho(f"ARCHIVING COMPLETED! Data is stored in {out_db}", fg="green")
 
 
 @youte.group()
```

### Comparing `youte-2.1.0/src/youte/collector.py` & `youte-2.2.0/src/youte/collector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import logging
 import random
+import warnings
 from datetime import datetime, timedelta
 from typing import Iterator, Literal, Optional
 
 import requests
 from dateutil import tz
 
 from youte._typing import APIResponse, SearchOrder
-from youte.exceptions import APIError, CommentsDisabled, InvalidRequest
+from youte.exceptions import APIError, CommentsDisabled, InvalidRequest, MaxQuotaReached
 from youte.utilities import create_utc_datetime_string
+from youte.version import user_agent, version
 
 logger = logging.getLogger(__name__)
 
 
 class Youte:
     def __init__(self, api_key: str):
         """Requires an API key to instantiate."""
@@ -38,14 +40,16 @@
         video_embeddable: Literal["any", "true"] = "any",
         video_license: Literal["any", "creativeCommon", "youtube"] = "any",
         video_dimension: Literal["2d", "3d", "any"] = "any",
         location: Optional[tuple] = None,
         location_radius: Optional[str] = None,
         max_result: int = 50,
         max_pages_retrieved: Optional[int] = None,
+        include_meta: bool = True,
+        **kwargs,
     ) -> Iterator[APIResponse]:
         """Do a YouTube search.
 
         Args:
             query (str): The term to search for.
                 You can also use the Boolean NOT (-) and OR (|)
                 operators to exclude videos or to find videos matching one of several
@@ -98,14 +102,16 @@
                 measurement unit. Valid measurement units are m, km, ft, and mi. Values
                 larger than 1000 km are not supported.
             max_result (int): Maximum number of items that should be returned in one
                 page of the result.
                 Accepted values are between 0 and 50, inclusive.
             max_pages_retrieved (int, optional): Limit the number of result pages
                 returned. Equals the maximum number of calls made to the API.
+            include_meta (bool): Include `_youte` metadata in output.
+            **kwargs: Any metadata to be included in `_youte` metadata field.
 
         Yields:
             Dict mappings containing API response.
         """
 
         url: str = r"https://www.googleapis.com/youtube/v3/search"
         params: dict = {
@@ -129,36 +135,44 @@
             "videoLicense": video_license,
             "videoType": video_type,
             "relevanceLanguage": language,
             "regionCode": region,
         }
         logger.debug(f"Search query: {params}")
         yield from _paginate_results(
-            url=url, max_pages_retrieved=max_pages_retrieved, **params
+            url=url,
+            max_pages_retrieved=max_pages_retrieved,
+            include_meta=include_meta,
+            meta=kwargs,
+            **params,
         )
 
     def get_video_metadata(
         self,
         ids: list[str],
         part: Optional[list[str]] = None,
         max_results: int = 50,
+        include_meta: bool = True,
+        **kwargs,
     ) -> Iterator[APIResponse]:
         """Retrieve full metadata for videos using their IDs.
 
         Args:
             ids (list[str]): A list of one or multiple video IDs.
                 If a single ID is specified, it should
                 be wrapped in a list as well, e.g. ["video_id"].
             part (list[str], optional): A list of video resource properties that
                 the API response will include. If not, these are the parts used:
                 ["snippet", "statistics", "topicDetails",
                 "status", "contentDetails", "recordingDetails", "id"].
             max_results (int):
                 Maximum number of results returned in one page of response.
                 Accepted value is between 0 and 50.
+            include_meta (bool): Include `_youte` metadata in output.
+            **kwargs: Any metadata to be included in `_youte` metadata field.
 
         Yields:
             Dict mappings containing API response.
 
         Raises:
             TypeError: If the value passed to ids is not a list, a TypeError will be raised.
         """
@@ -196,21 +210,25 @@
                 ids_string = ",".join(batch)
                 for elm in batch:
                     ids.remove(elm)
             params["id"] = ids_string
             logger.info(f"Retrieving video metadata: {total_batches} batches left")
             logger.debug(f"Retrieving metadata for videos: {params['id']}")
             total_batches -= 1
-            yield from _paginate_results(url=url, **params)
+            yield from _paginate_results(
+                url=url, include_meta=include_meta, meta=kwargs, **params
+            )
 
     def get_channel_metadata(
         self,
         ids: list[str],
         part: Optional[list[str]] = None,
         max_results: int = 50,
+        include_meta: bool = True,
+        **kwargs,
     ) -> Iterator[APIResponse]:
         """Retrieve full metadata for channels using their IDs.
         Currently, do not work with usernames. Channel IDs can be obtained in API
         responses to other methods such as search() or get_video_metadata().
 
         Args:
             ids (list[str]): A list of one or multiple channel IDs. If a single ID is
@@ -219,14 +237,16 @@
                 API response will include.
                 If nothing is passed, the parts used are [ "snippet", "statistics",
                 "topicDetails", "status", "contentDetails", "brandingSettings",
                 "contentOwnerDetails"]
             max_results (int):
                 Maximum number of results returned in one page of response.
                 Accepted value is between 0 and 50.
+            include_meta (bool): Include `_youte` metadata in output.
+            **kwargs: Any metadata to be included in `_youte` metadata field.
 
         Yields:
             Dict mappings containing API response.
 
         Raises:
             TypeError: If the value passed to ids is not a list,
                 a TypeError will be raised.
@@ -264,25 +284,29 @@
                 for elm in batch:
                     ids.remove(elm)
 
             params["id"] = ids_string
             logger.info(f"Retrieving channel metadata: {total_batches} pages remaining")
             logger.debug(f"Retrieving metadata for channels: {params['id']}")
             total_batches -= 1
-            yield from _paginate_results(url=url, **params)
+            yield from _paginate_results(
+                url=url, include_meta=include_meta, meta=kwargs, **params
+            )
 
     def get_comment_threads(
         self,
         video_ids: Optional[list[str]] = None,
         related_channel_ids: Optional[list[str]] = None,
         comment_ids: Optional[list[str]] = None,
         order: Literal["time", "relevance"] = "time",
         search_terms: Optional[str] = None,
         text_format: Literal["html", "plainText"] = "html",
         max_results: int = 100,
+        include_meta: bool = True,
+        **kwargs,
     ) -> Iterator[APIResponse]:
         """Retrieve comment threads (top-level comments) by their IDs, by video IDs, or
         by channel IDs.
         If video_ids are specified, retrieve all comment threads for
         those videos. If related_channel_ids are specified, retrieve all comments
         associated with those channels, including comments about the channels' videos.
         If comment_ids are specified, retrieve metadata of those comments.
@@ -313,14 +337,16 @@
             text_format ("html", "plainText"):
                 Specify the format of returned data.
             max_results (int):
                 Maximum number of results returned in one page of response.
                 Accepted value is between 0 and 100. Only applicable when retrieving
                 comment threads using video or channel IDs. When comment IDs are provided,
                 this argument is not used.
+            include_meta (bool): Include `_youte` metadata in output.
+            **kwargs: Any metadata to be included in `_youte` metadata field.
 
         Yields:
             Dict mappings containing API response.
 
         Raises:
             ValueError: If more than one of these parameters - video_ids,
                 related_channel_ids, comment_ids - are specified, a ValueError
@@ -350,30 +376,34 @@
             for video_id in video_ids:
                 params["videoId"] = video_id
                 logger.info(
                     f"{i}/{len(video_ids)}: Retrieving comments for video {video_id}"
                 )
                 logger.debug(f"Query {url}: {params}")
                 i += 1
-                yield from _paginate_results(url=url, **params)
+                yield from _paginate_results(
+                    url=url, include_meta=include_meta, meta=kwargs, **params
+                )
 
         if related_channel_ids:
             params["order"] = order
             params["maxResults"] = max_results
             if search_terms:
                 params["searchTerms"] = search_terms
             for channel_id in related_channel_ids:
                 params["allThreadsRelatedToChannelId"] = channel_id
                 logger.info(
                     f"{i}/{len(related_channel_ids)}: "
                     f"Retrieving comments for channel {channel_id}"
                 )
                 logger.debug(f"Query {url}: {params}")
                 i += 1
-                yield from _paginate_results(url=url, **params)
+                yield from _paginate_results(
+                    url=url, include_meta=include_meta, meta=kwargs, **params
+                )
 
         if comment_ids:
             comment_ids = list(set(comment_ids))
             total_batches = int(len(comment_ids) / 50)  # logging purpose only
 
             while comment_ids:
                 if len(comment_ids) <= 50:
@@ -385,35 +415,41 @@
                     for elm in batch:
                         comment_ids.remove(elm)
 
                 params["id"] = ids_string
                 logger.info(f"Retrieving comments: {total_batches} pages remaining")
                 logger.debug(f"Retrieving comments: {params['id']}")
                 total_batches -= 1
-                yield from _paginate_results(url=url, **params)
+                yield from _paginate_results(
+                    url=url, include_meta=include_meta, meta=kwargs, **params
+                )
 
     def get_thread_replies(
         self,
         thread_ids: list[str],
         text_format: Literal["html", "plainText"] = "html",
         max_results: int = 100,
+        include_meta: bool = True,
+        **kwargs,
     ) -> Iterator[APIResponse]:
         """Retrieve replies to comment threads. Currently, the API only supports getting
         replies to top-level comments. Replies to replies are not supported as of this
         version.
 
         Args:
             thread_ids (list[str]):
                 list of comment thread IDs. If a single ID, wrap in list, too, e.g.
                 ["thread_id"].
             text_format ("html", "plainText"):
                 Specify the format of returned data.
             max_results (int):
                 Maximum number of results returned in one page of response.
                 Accepted value is between 0 and 100.
+            include_meta (bool): Include `_youte` metadata in output.
+            **kwargs: Any metadata to be included in `_youte` metadata field.
 
         Yields:
             Dict mappings containing API response.
 
         Raises:
             TypeError: If thread_ids is not a list, a TypeError will be raised.
         """
@@ -433,22 +469,26 @@
         for thread_id in thread_ids:
             params["parentId"] = thread_id
             logger.info(
                 f"{i}/{len(thread_ids)}: Retrieving replies for thread {thread_id}"
             )
             logger.debug(f"Query {url}: {params}")
             i += 1
-            yield from _paginate_results(url=url, **params)
+            yield from _paginate_results(
+                url=url, include_meta=include_meta, meta=kwargs, **params
+            )
 
     def get_most_popular(
         self,
         region_code: str = "us",
         video_category_id: Optional[str] = None,
         max_results: int = 100,
         part: list[str] = None,
+        include_meta: bool = True,
+        **kwargs,
     ) -> Iterator[APIResponse]:
         """Retrieve the most popular videos for a region and video category.
 
         Args:
             region_code (str):
                 ISO 3166-1 alpha-2 country code for specifying a region.
             video_category_id (str, optional):
@@ -456,14 +496,17 @@
                 be retrieved.
             max_results (int):
                 Maximum number of results to be retrieved per page.
             part (list[str], optional):
                 A list of video resource properties that the API response will include.
                 If noting is passed, the parts used are [ "snippet", "statistics",
                 "topicDetails", "status", "contentDetails", "recordingDetails", "id"]
+            include_meta (bool): Include `_youte` metadata in output.
+            **kwargs: Any metadata to be included in `_youte` metadata field.
+
 
         Yields:
             Dict mappings containing API response.
         """
         url: str = r"https://www.googleapis.com/youtube/v3/videos"
         if part is None:
             part = [
@@ -481,24 +524,26 @@
             "key": self.api_key,
             "chart": "mostPopular",
             "regionCode": region_code,
             "videoCategoryId": video_category_id,
         }
         logger.debug(f"Query {url}: {params}")
 
-        yield from _paginate_results(url=url, **params)
+        yield from _paginate_results(url=url, meta=kwargs, **params)
 
     def get_related_videos(
         self,
         video_ids: list[str],
         region: Optional[str] = None,
         relevance_language: Optional[str] = None,
         safe_search: Literal["none", "moderate", "strict"] = "none",
         max_results: int = 50,
         max_pages_retrieved: Optional[int] = None,
+        include_meta: bool = True,
+        **kwargs,
     ) -> Iterator[APIResponse]:
         """Retrieve videos related to a specified video.
         Can iterate over a list of video IDs and retrieve related videos for each of the
         specified ID.
 
         Args:
             video_ids (list[str]):
@@ -519,18 +564,25 @@
                 Maximum number of items that should be returned in one page of the result.
                 Accepted values are between 0 and 50, inclusive.
             max_pages_retrieved (int, optional):
                 Limit the number of result pages returned PER video ID.
                 Equals the maximum number of calls made to the API PER video ID.
                 So, if this parameter is set to 2 and a list of 3 IDs is specified
                 for video_ids, that makes 6 calls to the API in total.
+            include_meta (bool): Include `_youte` metadata in output.
+            **kwargs: Any metadata to be included in `_youte` metadata field.
 
         Yields:
             Dict mappings containing API response.
         """
+
+        warnings.warn(
+            "Retrieving related videos is deprecated by YouTube on August 7, 2023",
+            DeprecationWarning,
+        )
         url: str = r"https://www.googleapis.com/youtube/v3/search"
         params: dict = {
             "part": "snippet",
             "maxResults": max_results,
             "regionCode": region,
             "relevanceLanguage": relevance_language,
             "safeSearch": safe_search,
@@ -541,51 +593,69 @@
         i: int = 1  # logging purpose only
 
         for video_id in video_ids:
             params["relatedToVideoId"] = video_id
             logger.info(f"{i}/{len(video_ids)} Getting videos related to {video_id}")
             logger.debug(f"Query {url}: {params}")
             for result in _paginate_results(
-                url=url, max_pages_retrieved=max_pages_retrieved, **params
+                url=url,
+                max_pages_retrieved=max_pages_retrieved,
+                include_meta=include_meta,
+                meta=kwargs,
+                **params,
             ):
                 result["related_to_video_id"] = video_id
                 yield result
 
 
 def _paginate_results(
-    url: str, max_pages_retrieved: Optional[int] = None, **kwargs
+    url: str,
+    max_pages_retrieved: Optional[int] = None,
+    include_meta: bool = True,
+    meta: dict = None,
+    **kwargs,
 ) -> Iterator[APIResponse]:
     page: int = 0
     logger.info(f"Getting page {page + 1}")
 
     try:
         r = _request(url=url, params=kwargs)
         page += 1
-        response = _add_meta(r.json(), collection_time=datetime.now())
+        r = _request(url=url, params=kwargs)
+        response = _add_meta(r.json()) if include_meta else r.json()
         yield response
 
         while "nextPageToken" in r.json():
             if max_pages_retrieved and page >= max_pages_retrieved:
                 logger.info("Max pages reached")
                 break
             else:
                 logger.info(f"Getting page {page + 1}")
                 next_page_token = r.json()["nextPageToken"]
                 kwargs["pageToken"] = next_page_token
                 r = _request(url=url, params=kwargs)
                 page += 1
-                response = _add_meta(r.json(), collection_time=datetime.now())
+                response = _add_meta(r.json()) if include_meta else r.json()
                 yield response
     except CommentsDisabled:
         logger.warning("Comments are disabled.")
 
 
 def _add_meta(response: APIResponse, **kwargs) -> APIResponse:
-    for key in kwargs:
-        response[key] = kwargs[key]
+    default_meta = {
+        "version": version,
+        "collected_at": datetime.now(tz=tz.UTC),
+        "user_agent": user_agent,
+    }
+
+    response["_youte"] = default_meta
+
+    if kwargs:
+        for key in kwargs:
+            response["_youte"][key] = kwargs[key]
 
     return response
 
 
 def _request(url: str, params: dict[str, str | int]) -> requests.Response:
     response = requests.get(url, params=params)
     logger.debug(f"Getting {response.url}: {response.status_code}")
@@ -597,15 +667,15 @@
             raise InvalidRequest("Check url and endpoint.")
 
         for error in errors["error"]["errors"]:
             if error["reason"] == "commentsDisabled":
                 raise CommentsDisabled(error["reason"])
             elif "quotaExceeded" in error["reason"]:
                 until_reset = _get_reset_remaining(datetime.now(tz=tz.UTC))
-                raise APIError(
+                raise MaxQuotaReached(
                     f"{error['reason']}\n{until_reset} seconds til quota reset time"
                 )
             else:
                 logger.error(f"Error {response.status_code}: {response.url}")
                 raise APIError(error["message"])
 
     return response
```

### Comparing `youte-2.1.0/src/youte/config.py` & `youte-2.2.0/src/youte/config.py`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/src/youte/database.py` & `youte-2.2.0/src/youte/database.py`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/src/youte/parser.py` & `youte-2.2.0/src/youte/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import html
 import logging
 from datetime import datetime
-from typing import Iterable, Iterator, Optional
+from typing import Callable, Iterable, Iterator, Optional
 
 from pydantic import ValidationError
 
 from youte._typing import SearchResult, StandardResult, VideoChannelResult
 from youte.resources import (
     Channel,
     Channels,
@@ -172,14 +172,18 @@
 def _parse_search(input_: SearchResult) -> Iterator[Search]:
     if "searchListResponse" not in input_["kind"]:
         raise ValueError(
             f"Object passed to input is {input_['kind']} not a searchListResponse"
         )
 
     items: list[dict] = input_["items"]
+    if "_youte" in input_:
+        meta: dict = input_["_youte"]
+    else:
+        meta: dict = {}
 
     for item in items:
         snippet = item["snippet"]
 
         for elem in item["id"]:
             if "id" in elem or "Id" in elem:
                 id_: str = item["id"][elem]
@@ -193,25 +197,30 @@
             title=html.unescape(snippet["title"]),
             thumbnail_url=snippet["thumbnails"]["high"]["url"],
             thumbnail_height=snippet["thumbnails"]["high"]["height"],
             thumbnail_width=snippet["thumbnails"]["high"]["width"],
             channel_title=snippet.get("channelTitle"),
             live_broadcast_content=snippet["liveBroadcastContent"],
             channel_id=snippet["channelId"],
+            meta=meta,
         )
         yield search
 
 
 def _parse_video(input_: VideoChannelResult) -> Iterator[Video]:
     if "videoListResponse" not in input_["kind"]:
         raise ValueError(
             f"Object passed to input is {input_['kind']} not a videoListResponse"
         )
 
     items: list[dict] = input_["items"]
+    if "_youte" in input_:
+        meta: dict = input_["_youte"]
+    else:
+        meta: dict = {}
 
     for item in items:
         snippet = item["snippet"]
         content_details = item["contentDetails"]
         status = item["status"]
         statistics = item["statistics"]
         topic_details = item.get("topicDetails")
@@ -268,23 +277,28 @@
             else None,
             live_streaming_end_scheduled=_parse_rfc3339(live_stream["scheduledEndTime"])
             if "scheduledEndTime" in live_stream
             else None,
             live_streaming_concurrent_viewers=int(live_stream["concurrentViewers"])
             if "concurrentViewers" in live_stream
             else None,
+            meta=meta,
         )
         yield search
 
 
 def _parse_channel(input_: VideoChannelResult) -> Iterator[Channel]:
     if "channelListResponse" not in input_["kind"]:
         raise ValueError("Object passed to input is not a channelListResponse")
 
     items: list[dict] = input_["items"]
+    if "_youte" in input_:
+        meta: dict = input_["_youte"]
+    else:
+        meta: dict = {}
 
     for item in items:
         snippet = item["snippet"]
         status = item["status"]
         statistics = item["statistics"]
         topic_details = item.get("topicDetails")
         branding = item["brandingSettings"]
@@ -313,27 +327,32 @@
                 if topic_details
                 else None,
                 privacy_status=status["privacyStatus"],
                 is_linked=status["isLinked"],
                 made_for_kids=status.get("madeForKids"),
                 branding_keywords=_list(branding["channel"].get("keywords")),
                 moderated_comments=branding["channel"].get("moderatedComments"),
+                meta=meta,
             )
         except ValidationError:
             print(branding["channel"].get("keywords"))
             raise ValidationError
 
         yield channel
 
 
 def _parse_comment(input_: StandardResult) -> Iterable[Comment]:
     if "comment" not in input_["kind"]:
         raise ValueError("Object passed to input is not a comment")
 
     items: list[dict] = input_["items"]
+    if "_youte" in input_:
+        meta: dict = input_["_youte"]
+    else:
+        meta: dict = {}
 
     for item in items:
         can_reply: Optional[bool] = None
         total_reply_count: Optional[int] = None
         is_public: Optional[bool] = None
         if "topLevelComment" in item["snippet"]:
             snippet = item["snippet"]["topLevelComment"]["snippet"]
@@ -360,14 +379,15 @@
             viewer_rating=snippet["viewerRating"],
             like_count=snippet["likeCount"],
             published_at=_parse_rfc3339(snippet["publishedAt"]),
             updated_at=_parse_rfc3339(snippet["updatedAt"]),
             can_reply=can_reply,
             is_public=is_public,
             total_reply_count=total_reply_count,
+            meta=meta,
         )
         yield comment
 
 
 def _parse_rfc3339(string: str) -> datetime:
     """Parser function for RFC3339 datetime string returned from YouTube.
     fromisoformat() does not work with this format, except in Python 3.11
```

### Comparing `youte-2.1.0/src/youte/resources.py` & `youte-2.2.0/src/youte/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import Any, List, Literal, Optional
 
 from pydantic.dataclasses import dataclass
 
 from youte.common import Resources
 
 
 @dataclass
@@ -17,14 +17,15 @@
     description: str
     channel_id: str
     thumbnail_url: str
     thumbnail_width: int
     thumbnail_height: int
     channel_title: str
     live_broadcast_content: str
+    meta: dict[str, Any]
 
 
 @dataclass
 class Searches(Resources):
     items: List[Search]
 
 
@@ -63,14 +64,15 @@
     comment_count: Optional[int]
     topic_categories: Optional[List[str]]
     live_streaming_start_actual: Optional[datetime]
     live_streaming_end_actual: Optional[datetime]
     live_streaming_start_scheduled: Optional[datetime]
     live_streaming_end_scheduled: Optional[datetime]
     live_streaming_concurrent_viewers: Optional[int]
+    meta: dict[str, Any]
 
 
 @dataclass
 class Videos(Resources):
     items: List[Video]
 
 
@@ -95,14 +97,15 @@
     video_count: int
     topic_categories: Optional[List[str]]
     privacy_status: Literal["private", "public", "unlisted"]
     is_linked: bool
     made_for_kids: Optional[bool]
     branding_keywords: Optional[List[str]]
     moderated_comments: Optional[bool]
+    meta: dict[str, Any]
 
 
 @dataclass
 class Channels(Resources):
     items: List[Channel]
 
 
@@ -121,12 +124,13 @@
     text_display: str
     text_original: str
     can_rate: bool
     viewer_rating: Literal["like", "none"]
     like_count: int
     published_at: datetime
     updated_at: datetime
+    meta: dict[str, Any]
 
 
 @dataclass
 class Comments(Resources):
     items: List[Comment]
```

### Comparing `youte-2.1.0/src/youte/utilities.py` & `youte-2.2.0/src/youte/utilities.py`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/src/youte.egg-info/SOURCES.txt` & `youte-2.2.0/src/youte.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 docs/tutorial.md
 docs/images/youte-logo-black-transparent.png
 docs/images/youte-logo-white-transparent-1x.png
 docs/images/youte-logo-white-transparent.png
 docs/images/youte_save_progress.png
 docs/images/youte_search_results.png
 docs/images/youte_search_results_pretty.png
+docs/images/youte_thumbnail.png
 docs/stylesheets/extra.css
 src/youte/__init__.py
 src/youte/_logging.py
 src/youte/_typing.py
 src/youte/cli.py
 src/youte/collector.py
 src/youte/common.py
 src/youte/config.py
 src/youte/database.py
 src/youte/exceptions.py
 src/youte/parser.py
 src/youte/resources.py
 src/youte/utilities.py
+src/youte/version.py
 src/youte.egg-info/PKG-INFO
 src/youte.egg-info/SOURCES.txt
 src/youte.egg-info/dependency_links.txt
 src/youte.egg-info/entry_points.txt
 src/youte.egg-info/requires.txt
 src/youte.egg-info/top_level.txt
 tests/test_archive.py
```

### Comparing `youte-2.1.0/tests/test_archive.py` & `youte-2.2.0/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `youte-2.1.0/tests/test_cli.py` & `youte-2.2.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,25 +166,27 @@
     with runner.isolated_filesystem(temp_dir=tmp_path) as td:
         runner.invoke(youte, search_params["standard"])  # type: ignore
 
         with open(outfile_json, "r") as file:
             r: list[dict] = json.loads(file.read())
             assert len(r) > 1
             assert len(r[0]["items"]) > 10
+            assert r[0]["_youte"]
 
 
 @pytest.mark.parametrize("command", ["filter-by-language", "filter-by-location"])
 def test_cli_search_filter(runner, tmp_path, search_params, command, outfile_json):
     with runner.isolated_filesystem(temp_dir=tmp_path) as td:
         runner.invoke(youte, search_params["standard"])  # type: ignore
 
         with open(outfile_json, "r") as file:
             r: list[dict] = json.loads(file.read())
             assert len(r) > 1
             assert len(r[0]["items"]) > 10
+            assert r[0]["_youte"]
 
 
 def test_cli_search_tidy_csv(runner, tmp_path, search_params, outfile_csv):
     with runner.isolated_filesystem(temp_dir=tmp_path) as td:
         runner.invoke(youte, search_params["tidy-to-csv"])  # type: ignore
         assert os.path.exists(outfile_csv)
 
@@ -214,14 +216,15 @@
 def test_cli_videos(runner, tmp_path, videos_args, extra_args, outfile_json):
     results = runner.invoke(youte, videos_args + extra_args)  # type: ignore
     assert results.exit_code == 0
 
     with open(outfile_json, "r") as file:
         r: list[dict] = json.loads(file.read())
         assert len(r[0]["items"]) >= 1
+        assert r[0]["_youte"]
 
     os.remove(outfile_json)
 
 
 # TEST channels COMMAND
 
 
@@ -239,14 +242,15 @@
         ],
     )
     assert results.exit_code == 0
 
     with open(outfile_json, "r") as file:
         r: list[dict] = json.loads(file.read())
         assert len(r[0]["items"]) >= 10
+        assert r[0]["_youte"]
 
     os.remove(outfile_json)
 
 
 # TEST comments COMMAND
 
 
@@ -267,14 +271,15 @@
 def test_cli_comments(runner, comment_args, extra_args, outfile_json):
     results = runner.invoke(youte, comment_args + extra_args)
     assert results.exit_code == 0
 
     with open(outfile_json, "r") as file:
         r: list[dict] = json.loads(file.read())
         assert len(r[0]["items"]) >= 10
+        assert r[0]["_youte"]
 
     os.remove(outfile_json)
 
 
 # TEST dehydrate COMMAND
 
 
@@ -305,14 +310,15 @@
 def test_cli_related(runner, related_params, command, outfile_json):
     results = runner.invoke(youte, related_params[command])  # type: ignore
     assert results.exit_code == 0
 
     with open(outfile_json, "r") as file:
         r: list[dict] = json.loads(file.read())
         assert len(r[0]["items"]) >= 10
+        assert r[0]["_youte"]
 
     os.remove(outfile_json)
 
 
 # TEST chart COMMAND
 
 
@@ -323,9 +329,10 @@
         ["chart", country, "--outfile", outfile_json, "--key", API_KEY],
     )
     assert results.exit_code == 0
 
     with open(outfile_json, "r") as file:
         r: list[dict] = json.loads(file.read())
         assert len(r[0]["items"]) >= 10
+        assert r[0]["_youte"]
 
     os.remove(outfile_json)
```

### Comparing `youte-2.1.0/tests/test_collector.py` & `youte-2.2.0/tests/test_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         cmt
         for cmt in yob.get_thread_replies(
             thread_ids=thread_ids, text_format="plainText"
         )
     ]
     assert len(comments)
     assert len(comments[0]["items"]) > 2
-    assert "collection_time" in comments[0]
 
 
 def test_most_popular(yob: Youte):
     videos = [vid for vid in yob.get_most_popular()]
     assert len(videos)
     assert len(videos[0]["items"]) > 10
```

### Comparing `youte-2.1.0/tests/test_parser.py` & `youte-2.2.0/tests/test_parser.py`

 * *Files identical despite different names*

