# Comparing `tmp/pynamer-1.3.1.tar.gz` & `tmp/pynamer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-1.3.1.tar", last modified: Wed May 17 16:09:52 2023, max compression
+gzip compressed data, was "pynamer-1.4.0.tar", last modified: Tue May 16 15:47:16 2023, max compression
```

## Comparing `pynamer-1.3.1.tar` & `pynamer-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.338316 pynamer-1.3.1/
--rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-1.3.1/AUTHORS.md
--rw-rw-rw-   0        0        0     8219 2023-05-17 16:09:37.000000 pynamer-1.3.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0    18474 2023-05-17 16:09:52.338316 pynamer-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    16952 2023-05-16 18:56:04.000000 pynamer-1.3.1/README.md
--rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     1840 2023-05-17 16:09:52.338316 pynamer-1.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.215853 pynamer-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.253662 pynamer-1.3.1/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-13 20:08:21.000000 pynamer-1.3.1/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1895 2023-05-17 16:09:37.000000 pynamer-1.3.1/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0      754 2023-05-15 18:15:27.000000 pynamer-1.3.1/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.269311 pynamer-1.3.1/src/pynamer/project_name/
--rw-rw-rw-   0        0        0       37 2023-05-13 20:08:54.000000 pynamer-1.3.1/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0    34592 2023-05-17 11:05:22.000000 pynamer-1.3.1/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      401 2023-05-17 16:00:31.000000 pynamer-1.3.1/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-15 18:15:27.000000 pynamer-1.3.1/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0     1594 2023-05-16 19:07:11.000000 pynamer-1.3.1/src/pynamer/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.269311 pynamer-1.3.1/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    18474 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.338316 pynamer-1.3.1/tests/
--rw-rw-rw-   0        0        0     1869 2023-05-15 11:23:19.000000 pynamer-1.3.1/tests/test_args.py
--rw-rw-rw-   0        0        0     1923 2023-05-12 17:32:19.000000 pynamer-1.3.1/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1080 2023-05-12 17:31:19.000000 pynamer-1.3.1/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1018 2023-05-17 16:03:17.000000 pynamer-1.3.1/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1587 2023-05-15 18:15:27.000000 pynamer-1.3.1/tests/test_defaults.py
--rw-rw-rw-   0        0        0      538 2023-05-12 17:32:19.000000 pynamer-1.3.1/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-15 11:23:19.000000 pynamer-1.3.1/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2698 2023-05-09 14:10:02.000000 pynamer-1.3.1/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-12 17:32:19.000000 pynamer-1.3.1/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1259 2023-05-12 17:31:19.000000 pynamer-1.3.1/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0      282 2023-05-12 16:17:19.000000 pynamer-1.3.1/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     1664 2023-05-11 09:16:33.000000 pynamer-1.3.1/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1496 2023-05-11 08:50:00.000000 pynamer-1.3.1/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-12 17:31:19.000000 pynamer-1.3.1/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1117 2023-05-12 17:31:19.000000 pynamer-1.3.1/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      405 2023-05-12 17:32:19.000000 pynamer-1.3.1/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      737 2023-05-08 13:03:26.000000 pynamer-1.3.1/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      882 2023-05-12 17:32:19.000000 pynamer-1.3.1/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1617 2023-05-15 13:42:17.000000 pynamer-1.3.1/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-12 17:31:19.000000 pynamer-1.3.1/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:47:16.204834 pynamer-1.4.0/
+-rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-1.4.0/AUTHORS.md
+-rw-rw-rw-   0        0        0     7902 2023-05-16 15:47:04.000000 pynamer-1.4.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    18048 2023-05-16 15:47:16.205842 pynamer-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16533 2023-05-15 13:57:45.000000 pynamer-1.4.0/README.md
+-rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1840 2023-05-16 15:47:16.207833 pynamer-1.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 15:47:16.116302 pynamer-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 15:47:16.145303 pynamer-1.4.0/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-13 20:08:21.000000 pynamer-1.4.0/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1879 2023-05-16 15:47:04.000000 pynamer-1.4.0/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0      754 2023-05-15 18:15:27.000000 pynamer-1.4.0/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:47:16.157297 pynamer-1.4.0/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0       37 2023-05-13 20:08:54.000000 pynamer-1.4.0/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0    33544 2023-05-16 15:39:12.000000 pynamer-1.4.0/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      401 2023-05-16 15:41:36.000000 pynamer-1.4.0/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-15 18:15:27.000000 pynamer-1.4.0/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0     1589 2023-05-15 13:55:37.000000 pynamer-1.4.0/src/pynamer/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:47:16.156299 pynamer-1.4.0/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    18048 2023-05-16 15:47:16.000000 pynamer-1.4.0/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2023-05-16 15:47:16.000000 pynamer-1.4.0/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 15:47:16.000000 pynamer-1.4.0/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-16 15:47:16.000000 pynamer-1.4.0/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2023-05-16 15:47:16.000000 pynamer-1.4.0/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 15:47:16.000000 pynamer-1.4.0/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 15:47:16.202837 pynamer-1.4.0/tests/
+-rw-rw-rw-   0        0        0     1869 2023-05-15 11:23:19.000000 pynamer-1.4.0/tests/test_args.py
+-rw-rw-rw-   0        0        0     1923 2023-05-12 17:32:19.000000 pynamer-1.4.0/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1080 2023-05-12 17:31:19.000000 pynamer-1.4.0/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1018 2023-05-15 18:15:27.000000 pynamer-1.4.0/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1587 2023-05-15 18:15:27.000000 pynamer-1.4.0/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      538 2023-05-12 17:32:19.000000 pynamer-1.4.0/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-15 11:23:19.000000 pynamer-1.4.0/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2698 2023-05-09 14:10:02.000000 pynamer-1.4.0/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-12 17:32:19.000000 pynamer-1.4.0/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1259 2023-05-12 17:31:19.000000 pynamer-1.4.0/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0      282 2023-05-12 16:17:19.000000 pynamer-1.4.0/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0      199 2023-05-09 19:42:58.000000 pynamer-1.4.0/tests/test_main TBC.py
+-rw-rw-rw-   0        0        0     1664 2023-05-11 09:16:33.000000 pynamer-1.4.0/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1496 2023-05-11 08:50:00.000000 pynamer-1.4.0/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-12 17:31:19.000000 pynamer-1.4.0/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1117 2023-05-12 17:31:19.000000 pynamer-1.4.0/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      405 2023-05-12 17:32:19.000000 pynamer-1.4.0/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      737 2023-05-08 13:03:26.000000 pynamer-1.4.0/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      232 2023-05-12 11:41:53.000000 pynamer-1.4.0/tests/test_run_command TBD.py
+-rw-rw-rw-   0        0        0      882 2023-05-12 17:32:19.000000 pynamer-1.4.0/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1617 2023-05-15 13:42:17.000000 pynamer-1.4.0/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-12 17:31:19.000000 pynamer-1.4.0/tests/test_write_output_file.py
```

### Comparing `pynamer-1.3.1/CHANGELOG.md` & `pynamer-1.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
-## v1.3.1 (2023-05-17)
-### Fix
-* Restore text in setup ([`087d094`](https://github.com/Stephen-RA-King/pynamer/commit/087d094a554a9c70738fefe57e4f469e08252b48))
-
-### Documentation
-* Update readme images ([`392ec09`](https://github.com/Stephen-RA-King/pynamer/commit/392ec09379268bca7f85b40d0319a4fec8a5a1c4))
-
 ## v1.4.0 (2023-05-16)
 
 
 ## v1.3.0 (2023-05-16)
 
 
 ## v1.2.1 (2023-05-16)
```

### Comparing `pynamer-1.3.1/LICENSE` & `pynamer-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/PKG-INFO` & `pynamer-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 1.3.1
+Version: 1.4.0
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -31,14 +31,15 @@
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
+[![pre-commit][pre-commit-image]][pre-commit-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -296,30 +297,20 @@
 ersa            Found       Found       Found           Not Available
 pandia          Not Found   Not Found   Found           Not Available
 leda            Not Found   Not Found   Not Found       Available
 ```
 
 Again you can use a combination of names from the command line and input file.
 
-## Register the package name with PyPI
+## Register the name with PyPI
 
 You can optionally 'register' the name on PyPI by using the -r argument.
-If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
+If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded to
 to PyPI.
 
-The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
-You can also optionally choose to change the version and description.
-
-![](assets/usage_register_first.png)
-
-This information will be retained and you will not be prompted to enter this information again. However, you can regenerate
-this meta data by using the -m argument along with the -r argument. You can just enter on the options you dont want to change.
-
-![](assets/usage_register_meta.png)
-
 ```bash
 ~ $ pynamer agrajag -r
 ```
 
 ![](assets/usage_register.png)
 
 ## Verbose output
@@ -339,29 +330,30 @@
 As one of its tests Pynamer makes use of a list of package names scraped from its simple index site.
 
 The PyPI Simple Index is a plain text file that lists the names of all the packages available on PyPI.
 
 It is a simplified version of the PyPI index that makes it easier for users to browse and download packages.
 
 The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
-The Index is updated every few hours.
 
-Using the -g argument can be used to regenerate the local file contents.
+The PyPI Simple Index is updated every few hours
+
+Using the -r argument can be used to regenerate the local file contents.
 
 ```bash
 ~ $ pynamer -g
 ```
 
 ![](assets/usage_generate.png)
 
 See planned future improvements
 
 ## The Oddities
 
-The reason I wrote this application in the first place...
+The reason I wrote this application in the first place.
 
 ```bash
 ~ $ pynamer zaphod
 ```
 
 ![](assets/usage_zaphod.png)
 
@@ -405,14 +397,15 @@
 -   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
 
 ## Planned Future improvements
 
 -   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
+-   Filter out invalid PyPI package names at the start
 
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
```

### Comparing `pynamer-1.3.1/README.md` & `pynamer-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
+[![pre-commit][pre-commit-image]][pre-commit-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -268,30 +269,20 @@
 ersa            Found       Found       Found           Not Available
 pandia          Not Found   Not Found   Found           Not Available
 leda            Not Found   Not Found   Not Found       Available
 ```
 
 Again you can use a combination of names from the command line and input file.
 
-## Register the package name with PyPI
+## Register the name with PyPI
 
 You can optionally 'register' the name on PyPI by using the -r argument.
-If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
+If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded to
 to PyPI.
 
-The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
-You can also optionally choose to change the version and description.
-
-![](assets/usage_register_first.png)
-
-This information will be retained and you will not be prompted to enter this information again. However, you can regenerate
-this meta data by using the -m argument along with the -r argument. You can just enter on the options you dont want to change.
-
-![](assets/usage_register_meta.png)
-
 ```bash
 ~ $ pynamer agrajag -r
 ```
 
 ![](assets/usage_register.png)
 
 ## Verbose output
@@ -311,29 +302,30 @@
 As one of its tests Pynamer makes use of a list of package names scraped from its simple index site.
 
 The PyPI Simple Index is a plain text file that lists the names of all the packages available on PyPI.
 
 It is a simplified version of the PyPI index that makes it easier for users to browse and download packages.
 
 The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
-The Index is updated every few hours.
 
-Using the -g argument can be used to regenerate the local file contents.
+The PyPI Simple Index is updated every few hours
+
+Using the -r argument can be used to regenerate the local file contents.
 
 ```bash
 ~ $ pynamer -g
 ```
 
 ![](assets/usage_generate.png)
 
 See planned future improvements
 
 ## The Oddities
 
-The reason I wrote this application in the first place...
+The reason I wrote this application in the first place.
 
 ```bash
 ~ $ pynamer zaphod
 ```
 
 ![](assets/usage_zaphod.png)
 
@@ -377,14 +369,15 @@
 -   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
 
 ## Planned Future improvements
 
 -   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
+-   Filter out invalid PyPI package names at the start
 
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
```

### Comparing `pynamer-1.3.1/pyproject.toml` & `pynamer-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/setup.cfg` & `pynamer-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/src/pynamer/__init__.py` & `pynamer-1.4.0/src/pynamer/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python3
 """Top-level package for pynamer."""
 # Core Library modules
 import logging.config
 import pickle
-from importlib.resources import as_file, files, path
-from pathlib import Path
+from importlib.resources import as_file, files
 
 # Third party modules
-import yaml
+import yaml  # type: ignore
 
 __title__ = "pynamer"
-__version__ = "1.3.1"
+__version__ = "1.4.0"
 __author__ = "Stephen R A King"
 __description__ = (
-    "Utility to find an available package name in the PyPI repository and register it "
+    "Utility to find an available package name on the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
 
 
 LOGGING_CONFIG = """
```

### Comparing `pynamer-1.3.1/src/pynamer/config.py` & `pynamer-1.4.0/src/pynamer/config.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/src/pynamer/pynamer.py` & `pynamer-1.4.0/src/pynamer/pynamer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,986 +1,985 @@
-#!/usr/bin/env python3
-
-# Core Library modules
-import argparse
-import json
-import logging
-import os
-import pickle
-import re
-import shutil
-import string
-import subprocess
-import sys
-import webbrowser
-from datetime import datetime
-from pathlib import Path
-from typing import Any, Union
-
-# Third party modules
-import build
-import requests
-from bs4 import BeautifulSoup
-from colorama import Back, Fore, Style
-from jinja2 import Template
-from rich.console import Console
-from rich.table import Table
-from tqdm import tqdm
-
-# Local modules
-from . import meta, project_count, project_path, setup_text
-from .config import config
-from .utils import _check_version
-
-logger = logging.getLogger()
-project_path = Path(str(project_path))
-
-
-def _feedback(message: str, feedback_type: str) -> None:
-    """Generates a formatted messages appropriate to the message type.
-
-    Args:
-        message:        Text to be echoed.
-        feedback_type:  identifies type of message to display.
-    """
-    if feedback_type not in ["null", "nominal", "warning", "error"]:
-        return
-    if config.idlemode == 1:
-        print(message)
-    else:
-        if feedback_type == "null":
-            print(Fore.WHITE + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
-        elif feedback_type == "nominal":
-            print(Fore.GREEN + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
-        elif feedback_type == "warning":
-            print(
-                Fore.YELLOW + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL
-            )
-        elif feedback_type == "error":
-            print(
-                Fore.RED
-                + Back.BLACK
-                + Style.BRIGHT
-                + f"ERROR: {message}"
-                + Style.RESET_ALL
-            )
-
-
-def _find_pypirc_file(filename: str = ".pypirc") -> None:
-    """Function to iterate over paths in the PATH environment variable to find a file.
-
-     Designed to find a .pypirc file starting with the current working directory.
-     If identified will update the config.pypirc variable, so it can be used elsewhere.
-
-    Args:
-        filename:       filename to find.
-    """
-    system_path = os.getenv("PATH")
-    if system_path is not None:
-        path_directories = [os.getcwd()]
-        path_directories.extend(system_path.split(os.pathsep))
-        for directory in path_directories:
-            file_path = Path(directory) / filename
-            if file_path.exists():
-                logger.debug(
-                    "%s is present in the system's PATH at %s", filename, directory
-                )
-                config.pypirc = file_path
-                break
-    logger.debug("%s is not present in the system's PATH.", filename)
-
-
-def _rename_project_dir(old_name: str, new_name: str) -> None:
-    """Utility script to rename a directory.
-
-    The object being to rename a 'template' directory for the purpose of creating a
-    minimalist package for upload to PyPI.
-
-    Args:
-        old_name:       source name.
-        new_name:       dst name.
-
-    Raises:
-        FileNotFoundError
-    """
-    old_directory_path = Path(old_name)
-    new_directory_path = Path(new_name)
-    logger.debug("renaming project directory from %s to %s", old_name, new_name)
-    try:
-        old_directory_path.rename(new_directory_path)
-    except FileNotFoundError:
-        logger.error("directory %s cannot be found:", old_directory_path)
-        raise FileNotFoundError
-
-
-def _create_setup(new_project_name: str, new_meta: bool = False) -> None:
-    """Utility script to create a setup.py file.
-
-    The object being to create a setup.py file from a 'template' file for the purpose of
-    creating a minimalist package for upload to PyPI.
-
-    Args:
-        new_project_name:       name used to render the template.
-    """
-    meta_file = Path(project_path / "meta.pickle")
-    setup_file = Path(project_path / "setup.txt")
-    setup_base_file = Path(project_path / "setup_base.txt")
-    setup_file_py = Path(project_path / "setup.py")
-
-    author = meta["author"] if meta else ""
-    email = meta["email"] if meta else ""
-    description = meta["description"] if meta else config.description
-    version = meta["version"] if meta else config.package_version
-
-    _email_pattern = (
-        r"[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*@(?:"
-        r"[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?"
-    )
-
-    if "AUTHOR" in setup_text or "EMAIL" in setup_text or not meta or new_meta:
-        try:
-            while True:
-                author = (
-                    input(
-                        Fore.YELLOW
-                        + Back.BLACK
-                        + Style.BRIGHT
-                        + f"please enter your author name ({author}): "
-                        + Style.RESET_ALL
-                    )
-                    or author
-                )
-                if author != "":
-                    break
-        except KeyboardInterrupt:
-            _feedback("...bye!", "warning")
-            raise SystemExit()
-
-        try:
-            while True:
-                email = (
-                    input(
-                        Fore.YELLOW
-                        + Back.BLACK
-                        + Style.BRIGHT
-                        + f"please enter your email address ({email}): "
-                        + Style.RESET_ALL
-                    )
-                    or email
-                )
-                if re.search(_email_pattern, email):
-                    break
-                else:
-                    print(
-                        Fore.YELLOW
-                        + Back.BLACK
-                        + Style.BRIGHT
-                        + "does not appear to be a valid email address"
-                        + Style.RESET_ALL
-                    )
-        except KeyboardInterrupt:
-            _feedback("...bye!", "warning")
-            raise SystemExit()
-
-        try:
-            while True:
-                version = (
-                    input(
-                        Fore.YELLOW
-                        + Back.BLACK
-                        + Style.BRIGHT
-                        + f"version number: ({version}): "
-                        + Style.RESET_ALL
-                    )
-                    or version
-                )
-                if version != "":
-                    break
-        except KeyboardInterrupt:
-            raise SystemExit("Bye!")
-
-        try:
-            while True:
-                description = (
-                    input(
-                        Fore.YELLOW
-                        + Back.BLACK
-                        + Style.BRIGHT
-                        + f"description: ({description}): "
-                        + Style.RESET_ALL
-                    )
-                    or description
-                )
-                if description != "":
-                    break
-        except KeyboardInterrupt:
-            raise SystemExit("Bye!")
-
-        setup_file.unlink()
-
-        with open(setup_base_file, encoding="utf-8") as f:
-            setup_text_base = f.read()
-
-        template = Template(setup_text_base)
-        content = template.render(
-            PROJECT_NAME="{{ PROJECT_NAME }}",
-            PACKAGE_VERSION=version,
-            DESCRIPTION=description,
-            AUTHOR=author,
-            EMAIL=email,
-        )
-        with open(setup_file, mode="w", encoding="utf-8") as f:
-            f.write(content)
-
-    meta_save = {
-        "author": author,
-        "email": email,
-        "description": description,
-        "version": version,
-    }
-    with open(meta_file, "wb") as f:
-        pickle.dump(meta_save, f)
-
-    with open(setup_file) as f:
-        setup_text_file = f.read()
-        template = Template(setup_text_file)
-        content = template.render(
-            PROJECT_NAME=new_project_name,
-        )
-    with open(setup_file_py, mode="w", encoding="utf-8") as message:
-        logger.debug("creating new setup.py with the following: \n %s", content)
-        message.write(content)
-
-
-def _delete_director(items_to_delete: list[Path]) -> None:
-    """Utility function to delete files and directories.
-
-    Args:
-        items_to_delete:    A list of Path like objects to delete.
-    """
-    for item in items_to_delete:
-        if not item.exists():
-            logger.debug("trying to delete %s but it does not exist", item)
-            continue
-        if item.is_dir():
-            logger.debug("Deleting Directory: %s", item)
-            shutil.rmtree(item, ignore_errors=True)
-        else:
-            logger.debug("Deleting File: %s", item)
-            Path.unlink(item, missing_ok=True)
-
-
-def _run_command(
-    *arguments: str,
-    shell: bool = True,
-    working_dir: Union[Path, str, None] = None,
-    project: Union[None, str] = None,
-) -> None:  # pragma: no cover
-    """Utility designed to execute a command line utility.
-
-    Args:
-        arguments:  Comma separated strings- "utility", "arg1", "arg2", etc.
-        shell:      command executed by the shell or directly by the operating system.
-        cwd:        specifies the current working directory to use when starting
-                    the subprocess.
-                    e.g. "/home/user/mydir"
-        project:    the name of the project currently being tested
-    """
-    working_dir = os.getcwd() if working_dir is None else working_dir
-    try:
-        process = subprocess.Popen(
-            arguments,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            shell=shell,
-            text=True,
-            cwd=working_dir,
-        )
-        stdout, stderr = process.communicate()
-        if process.returncode != 0:
-            logger.error("Error running command: %s", arguments)
-            logger.error("stderr: %s", stderr)
-            if project is not None:
-                _cleanup(project)
-            return
-        logger.debug("%s", stdout)
-        return
-    except Exception as e:
-        logger.error("Exception running command: %s", arguments)
-        logger.error(e)
-        if project is not None:
-            _cleanup(project)
-        return
-
-
-def _is_valid_package_name(project_name: str) -> bool:
-    """Function does a basic check of project name validity.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Returns:
-        True:           If the name passes the basic check
-        False:          If the name fails the basic check
-
-
-    """
-    pattern = r"^[a-z][_\-a-z0-9]*$"
-    if re.match(pattern, project_name) is not None:
-        return True
-    else:
-        return False
-
-
-def _ping_project(project_name: str) -> bool:
-    """Determines if the URL to the project exists in PyPIs project area.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Returns:
-        True:           If the URLs response code is 200
-        False:          If the URLs response code is not 200
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-    """
-    url_project = "".join([config.pypi_project_url, project_name, "/"])
-    logger.debug("attempting to get url %s", url_project)
-    try:
-        project_ping = requests.get(url_project, timeout=10)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    if project_ping.status_code == 200:
-        logger.debug("%s FOUND in the project area of PyPI", project_name)
-        return True
-    logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
-    return False
-
-
-def _ping_json(project_name: str) -> str:
-    """Collects some details about the project if it exists.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-    """
-    url_json = "".join([config.pypi_json_url, project_name, "/json"])
-    logger.debug("attempting to get url %s", url_json)
-    try:
-        project_json_raw = requests.get(url_json, timeout=10)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    if project_json_raw.status_code == 200:
-        project_json = json.loads(project_json_raw.content)
-        result = "".join(
-            [
-                project_json["info"]["author"],
-                "\n",
-                project_json["info"]["author_email"],
-                "\n",
-                project_json["info"]["version"],
-                "\n",
-                project_json["info"]["summary"],
-            ]
-        )
-        return result
-    logger.debug("No response from JSON URL")
-    return ""
-
-
-def _build_dist() -> None:
-    """Builds the sdist and wheel of the minimalist project to upload to PyPI."""
-    logger.debug("Building the distribution... ")
-    builder = build.ProjectBuilder(project_path)
-    builder.build("wheel", project_path / "dist")
-    builder.build("sdist", project_path / "dist")
-
-
-def _upload_dist(project_name: str) -> None:
-    """Builds the twine command line to upload the minimalist project to PyPI.
-
-    Args:
-        project_name:   the name of the project currently under test.
-
-    Notes:
-        twine expects a filesystem path not Path object so use os.fspath()
-    """
-    logger.debug("Uploading the distribution... ")
-    dir_path = os.fspath(project_path / "dist" / "*")
-    pypirc_path = os.fspath(config.pypirc)
-    _run_command(
-        sys.executable,
-        "-m",
-        "twine",
-        "upload",
-        "--config-file",
-        pypirc_path,
-        dir_path,
-        project=project_name,
-    )
-
-
-def _cleanup(project_name: str) -> None:
-    """Builds a manifest of artifacts to delete into a list of Path objects.
-
-    Args:
-        project_name:   the name of the project currently under test.
-    """
-    if config.no_cleanup is True:
-        return
-    _rename_project_dir(
-        project_path.joinpath(project_name),
-        project_path.joinpath(config.original_project_name),
-    )
-    build_artifacts = [
-        project_path / "build",
-        project_path / "dist",
-        project_path / "".join([project_name, ".egg-info"]),
-        project_path / "setup.py",
-    ]
-    logger.debug("cleaning build artifacts %s", build_artifacts)
-    _delete_director(build_artifacts)
-
-
-def _generate_pypi_index() -> None:
-    """Generates a list of projects in PyPI's simple index - writes results to a file.
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-
-    Notes:
-        A potentially expensive operation as there are almost 500,000 projects to
-        process. Can take 2-3 seconds. Look to improve performance at a later date:
-        look at asyncio, asyncio.http etc.
-        An improvement is to automatically periodically run this in the background.
-    """
-    new_count = 0
-    pattern = re.compile(r">([\w\W]*?)<")
-    progress_bar = tqdm(total=config.project_count)
-    pypi_index = project_path / "pypi_index"
-    pypi_count = project_path / "project_count.pickle"
-    if pypi_index.exists():
-        Path.unlink(pypi_index, missing_ok=True)
-    try:
-        index_object_raw = requests.get(config.pypi_simple_index_url, timeout=10)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    with pypi_index.open(mode="a") as file:
-        for line in index_object_raw.iter_lines():
-            line = str(line)
-            project_text = re.search(pattern, line)
-            if project_text is not None:
-                new_count += 1
-                progress_bar.update(1)
-                project = "".join([project_text.group(1), " \n"])
-                file.write(project)
-    progress_bar.close()
-    with open(pypi_count, "wb") as f:
-        pickle.dump(new_count, f)
-
-
-def _pypi_search_index(project_name: str) -> bool:
-    """Open the generated index file and search for the project name.
-
-    Args:
-        project_name:   the name of the project currently under test.
-
-    Returns:
-        True:           A match was found.
-        False:          A match was not found.
-    """
-    pypi_index = project_path / "pypi_index"
-    if not pypi_index.exists():
-        _generate_pypi_index()
-    with pypi_index.open(mode="r") as file:
-        projects = file.read()
-        if project_name in projects:
-            logger.debug("%s FOUND in the PyPI simple index", project_name)
-            return True
-        logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
-        return False
-
-
-def _pypi_search(
-    search_project: str,
-) -> tuple[list[list[Union[str, Any]]], list[list[Union[str, Any]]], str]:
-    """Performs a get request to PyPI's search API for the project name.
-
-    Args:
-        search_project:   The name of the project currently under test.
-
-    Returns:
-        match:          A list of projects matching name comprising:
-                            [project_name, version, released, description]
-        others:         A list of projects not matching but PyPI thinks are relevant.
-                            [project_name, version, released, description]
-        others_total:   A str representation of total projects found (minus matches).
-    """
-    pattern = re.compile(r">([\d,+]*?)<")
-    s = requests.Session()
-    projects_raw: list = []
-    match: list[list[str]] = []
-    others: list[list[str]] = []
-    params = {"q": {search_project}, "page": 1}
-    r = s.get(config.pypi_search_url, params=params)  # type: ignore
-    soup = BeautifulSoup(r.text, "html.parser")
-    projects_raw.extend(soup.select('a[class*="package-snippet"]'))
-    for project_raw in projects_raw:
-        project_name = project_raw.select_one(
-            'span[class*="package-snippet__name"]'
-        ).text.strip()
-        version = project_raw.select_one(
-            'span[class*="package-snippet__version"]'
-        ).text.strip()
-        released_iso_8601 = project_raw.select_one(
-            'span[class*="package-snippet__created"]'
-        ).find("time")["datetime"]
-        released = datetime.strptime(released_iso_8601, "%Y-%m-%dT%H:%M:%S%z").strftime(
-            "%Y-%m-%d"
-        )
-        description = project_raw.select_one(
-            'p[class*="package-snippet__description"]'
-        ).text.strip()
-        if project_name.lower() == search_project.lower():
-            match.append([project_name, version, released, description])
-        else:
-            others.append([project_name, version, released, description])
-
-    total_div_raw = soup.select(
-        'div[class="split-layout split-layout--table split-layout--wrap-on-tablet"]'
-    )
-    total_raw = re.search(pattern, str(total_div_raw))
-    if total_raw is not None:
-        total_string = total_raw.group(1)
-        total = int(total_string.translate(str.maketrans("", "", string.punctuation)))
-        others_total = (
-            "".join([str(total), "+"])
-            if total == 10000
-            else (str(int(total) - len(match)))
-        )
-    else:
-        others_total = "0"
-    return match, others, others_total
-
-
-def _process_input_file(file: str) -> list[Union[str, Any]]:
-    """Processes the contents of the file to a list of strings.
-
-    Args:
-        file:           simple string for the file.
-
-    Raises:
-        SystemExit:     If the file is found to not exist.
-
-    Notes:
-        file contents should contain any number of space separated strings on any
-        number of lines.
-    """
-    file_path = Path(file)
-    try:
-        with file_path.open(mode="r") as f:
-            file_contents = f.read()
-            projects = file_contents.split()
-            return list(set(projects))
-    except FileNotFoundError:
-        _feedback(f"The file {file} does not exist", "warning")
-        raise SystemExit()  # pragma: no cover
-    except PermissionError:
-        _feedback(f"Permission denied to file: {file}", "warning")
-        raise SystemExit()  # pragma: no cover
-    except IsADirectoryError:
-        _feedback(f"{file} is a directory not a file", "warning")
-        raise SystemExit()  # pragma: no cover
-    except OSError:
-        _feedback(f"A general IO error has occurred opening file: {file}", "warning")
-        raise SystemExit()  # pragma: no cover
-    except Exception as e:
-        _feedback(f"An error occurred:, {str(e)}", "warning")
-        raise SystemExit()  # pragma: no cover
-
-
-def _write_output_file(file_name: str, results: dict) -> None:
-    """Write the results to a file
-
-    Args:
-        file_name:      Name of file to save as a simple string.
-        results:        Dictionary containing the test results e.g.
-                        {"pynball": [1, 1, 1]}
-    """
-    header_width = 83
-    truncation_width = 25
-    file_path = Path(file_name)
-    title = "Results from pynamer PyPI utility\n"
-    title = "".join([title, "=" * header_width, "\n\n"])
-    title = "".join(
-        [
-            title,
-            "Test 1 - Basic url lookup on PyPI\n",
-            "Test 2 - Search of PyPIs simple index\n",
-            "Test 3 - Search using an request to PyPIs search 'API'\n\n",
-        ]
-    )
-    header = f"{'Project':30}{'Test1':12}{'Test2':12}{'Test3':12}{'Conclusion'}\n"
-    header = "".join([header, "=" * header_width, "\n"])
-    projects_results: str = ""
-    for project in results:
-        project_name = (
-            project
-            if len(project) <= truncation_width
-            else project[: truncation_width - 3] + "..."
-        )
-        projects_results = "".join([projects_results, f"{project_name:30}"])
-        for test in results[project]:
-            test = "Found" if test == 1 else "Not Found"
-            projects_results = "".join([projects_results, f"{test:12}"])
-        conclusion = "Not Available" if sum(results[project]) > 0 else "Available"
-        projects_results = "".join([projects_results, f"{conclusion}"])
-        projects_results = "".join([projects_results, "\n", "-" * header_width, "\n"])
-
-    final_output_text = "".join([title, header, projects_results])
-
-    try:  # pragma: no cover
-        with file_path.open(mode="w") as f:
-            f.write(final_output_text)
-    except PermissionError:
-        _feedback(f"Permission denied to file: {file_path.open}", "warning")
-        raise SystemExit()  # pragma: no cover
-    except FileExistsError:
-        _feedback(f"File {file_path.open} already exists", "warning")
-        raise SystemExit()  # pragma: no cover
-    except IsADirectoryError:
-        _feedback(f"{file_path.open} is a directory not a file", "warning")
-        raise SystemExit()  # pragma: no cover
-    except OSError:
-        _feedback("General IO error has occurred", "warning")
-        raise SystemExit()  # pragma: no cover
-    except Exception as e:
-        _feedback(f"An error occurred:, {str(e)}", "warning")
-        raise SystemExit()  # pragma: no cover
-
-
-def _final_analysis(pattern: list[int]) -> None:
-    """Displays a rich console table displaying the conclusion of the test results
-
-    Args:
-        pattern:    A list of the test results:
-                    1 - A 'negative' result, indicating the project has been found.
-                    0 - A 'positive' result, indicating the project was not found.
-    """
-    table = Table(show_header=True)
-    table.add_column("FINAL ANALYSIS", style="bold cyan")
-    if pattern == [0, 1, 0]:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row(
-            "A Gotcha!, whereby the package is not found even with PyPI's own search"
-            " facility.\n"
-            "It can only be found by searching the simple index which is not available "
-            "through the interface"
-        )
-    elif pattern == [1, 1, 0]:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row(
-            "A Gotcha!, whereby the package is not found even with PyPI's own search"
-            " facility.\n"
-            "However if appears in the simple index and can be displayed by simply"
-            " browsing "
-            "to the projects URL"
-        )
-    elif sum(pattern) >= 1:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row("The package name was found in at least one place")
-    elif sum(pattern) == 0:
-        table.add_row("[green]AVAILABLE![/green]\n")
-        table.add_row("The package name was not found in any part of PyPI")
-
-    console = Console()
-    console.print(table)
-
-
-def _parse_args(args: list) -> tuple[argparse.Namespace, argparse.ArgumentParser]:
-    """Function to return the ArgumentParser object created from all the args.
-
-    Args:
-        args:   A list of arguments from the commandline
-                e.g. ['pynball', '-v', '-g']
-    """
-    parser = argparse.ArgumentParser(
-        prog="pynamer",
-        description="Determine if project name is available on pypi with the "
-        "option to 'register' it for future use if available",
-    )
-    parser.add_argument(
-        "projects",
-        nargs="*",
-        default="None",
-        help="Optional - one or more project names",
-    )
-    parser.add_argument(
-        "-r",
-        "--register",
-        action="store_true",
-        help="register the name on PyPi if the name is available",
-    )
-    parser.add_argument(
-        "-d",
-        "--dryrun",
-        action="store_true",
-        help=argparse.SUPPRESS,
-    )
-
-    parser.add_argument(
-        "-n",
-        "--nocleanup",
-        action="store_true",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        help="display information about similar projects",
-    )
-    parser.add_argument(
-        "-g",
-        "--generate",
-        action="store_true",
-        help="generate a new PyPI simple index",
-    )
-    parser.add_argument(
-        "-m",
-        "--meta",
-        action="store_true",
-        help="input new meta data when registering (Author and email address)",
-    )
-
-    parser.add_argument(
-        "-w",
-        "--webbrowser",
-        action="store_true",
-        help="open the project on PyPI in a webbrowser",
-    )
-
-    parser.add_argument(
-        "--version",
-        action="store_true",
-        help="display version number",
-    )
-    parser.add_argument(
-        "-f",
-        "--file",
-        default="None",
-        type=str,
-        help="file containing a list of projects to analyze",
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        default="None",
-        type=str,
-        help="file to store the test results",
-    )
-    return parser.parse_args(args), parser
-
-
-def main() -> None:  # pragma: no cover, type: ignore
-    args, parser = _parse_args(sys.argv[1:])
-    logger.debug(" args: %s", args)
-
-    if args.generate:
-        _generate_pypi_index()
-
-    if args.version:
-        version, message, result = _check_version()
-        if result:
-            _feedback(f"{version} : {message}", "nominal")
-        else:
-            _feedback(f"{version} : {message}", "warning")
-
-    if args.projects == "None" and args.file == "None" and args.register:
-        _feedback("You need to specify a project name to register it", "error")
-        raise SystemExit()
-
-    if args.projects == "None" and args.file == "None" and args.meta:
-        _feedback(
-            "You can only update the meta data during the registration process", "error"
-        )
-        raise SystemExit()
-
-    if (
-        args.projects == "None"
-        and args.file == "None"
-        and args.version is False
-        and args.generate is False
-    ):
-        parser.print_help()
-        raise SystemExit()
-
-    project_list = []
-    test_results = []
-    aggregated_result = {}
-    _find_pypirc_file()
-    if args.nocleanup is True:
-        config.no_cleanup = True
-
-    # Gather the projects into one list
-    if args.projects != "None":
-        logger.debug("adding project names from command line %s", args.projects)
-        project_list.extend(list(set(args.projects)))
-        logger.debug("project_list = %s", project_list)
-    if args.file != "None":
-        logger.debug("adding project names from file %s", args.file)
-        project_list.extend(_process_input_file(args.file))
-        logger.debug("project_list = %s", project_list)
-    project_list.sort()
-
-    # Main loop
-    for new_project in project_list:
-        if not _is_valid_package_name(new_project):
-            _feedback(f"{new_project} is not a valid package name", "error")
-            continue
-
-        test_table = Table(title=f"Test Results for {new_project}", show_lines=True)
-        test_table.add_column("No.", style="bold yellow")
-        test_table.add_column("Test", style="bold cyan")
-        test_table.add_column("Result")
-        test_table.add_column("Details", style="bold cyan")
-
-        match_table = Table(title=f"PyPI Search: Exact Match {new_project}")
-        match_table.add_column("Package", style="bold yellow")
-        match_table.add_column("Version", style="bold green")
-        match_table.add_column("Released", style="bold yellow")
-        match_table.add_column("Description", style="bold cyan")
-
-        others_table = Table(
-            title="Other Close Matches or Related Projects (from page 1)"
-        )
-        others_table.add_column("Package", style="bold yellow")
-        others_table.add_column("Version", style="bold green")
-        others_table.add_column("Released", style="bold yellow")
-        others_table.add_column("Description", style="bold cyan")
-
-        # perform the tests
-        # Test 1
-        if _ping_project(new_project):
-            test_results.append(1)
-            json_data = _ping_json(new_project)
-            test_table.add_row(
-                "1", "Basic http get to project URL", "[red]FOUND[/red]", json_data
-            )
-        else:
-            test_results.append(0)
-            test_table.add_row(
-                "1", "Basic http get to project URL", "[green]NOT FOUND[/green]", ""
-            )
-
-        # Test 2
-        if _pypi_search_index(new_project):
-            test_results.append(1)
-            test_table.add_row(
-                "2",
-                "Check PyPI simple index",
-                "[red]FOUND[/red]",
-                f"Searched {project_count} projects",
-            )
-        else:
-            test_results.append(0)
-            test_table.add_row(
-                "2",
-                "Check PyPI simple index",
-                "[green]NOT FOUND[/green]",
-                f"Searched {project_count} projects",
-            )
-
-        # Test 3
-        match, others, others_total = _pypi_search(new_project)
-        if match:
-            test_results.append(1)
-            test_table.add_row(
-                "3",
-                "Check PyPI search",
-                "[red]FOUND[/red]",
-                f"Exact match found: {len(match)}, Others found: {others_total}",
-            )
-            for items in match:
-                match_table.add_row(items[0], items[1], items[2], items[3])
-        else:
-            test_results.append(0)
-            test_table.add_row(
-                "3",
-                "Check PyPI search",
-                "[green]NOT FOUND[/green]",
-                f"Exact match found: 0, Others found: {others_total}",
-            )
-
-        # Create Verbose Table
-        if others:
-            for items in others:
-                others_table.add_row(items[0], items[1], items[2], items[3])
-
-        # Display the Tables
-        console = Console()
-        console.print(test_table)
-        if match:
-            console.print(match_table)
-        if args.verbose and others:
-            console.print(others_table)
-        _final_analysis(test_results)
-
-        # build and upload
-        if (
-            test_results == [0, 0, 0]
-            and args.register is True
-            and config.pypirc is not None
-            and len(project_list) == 1
-        ):
-            _create_setup(new_project, new_meta=args.meta)
-            _rename_project_dir(
-                project_path.joinpath(config.original_project_name),
-                project_path.joinpath(new_project),
-            )
-            _build_dist()
-            if args.dryrun is False:
-                _upload_dist(new_project)
-            else:
-                _feedback("Dryrun .... bypassing upload to PyPI..", "warning")
-            _cleanup(new_project)
-        elif config.pypirc is None:
-            _feedback(
-                ".pypirc file cannot be located ... wont attempt to 'register'",
-                "error",
-            )
-        elif sum(test_results) > 0 and args.register is True:
-            _feedback("Project already exists ... wont attempt to 'register'", "error")
-
-        aggregated_result[new_project] = test_results.copy()
-        test_results.clear()
-
-    if args.output != "None":
-        _write_output_file(args.output, aggregated_result)
-
-    if args.register and len(project_list) > 1:
-        _feedback(
-            f"You can only use 'register' for one project at a time. "
-            f"You have specified {len(project_list)} projects",
-            "warning",
-        )
-
-    if args.webbrowser:
-        if len(project_list) == 1:
-            url_project = "".join([config.pypi_project_url, project_list[0], "/"])
-            webbrowser.open(url_project)
-        else:
-            _feedback(
-                f"You must choose one project to open the webbrowser. "
-                f"You have chosen {len(project_list)} projects",
-                "warning",
-            )
-
-
-if __name__ == "__main__":
-    SystemExit(main())  # type: ignore
+#!/usr/bin/env python3
+
+# Core Library modules
+import argparse
+import json
+import logging
+import os
+import pickle
+import re
+import shutil
+import string
+import subprocess
+import sys
+import webbrowser
+from datetime import datetime
+from pathlib import Path
+from typing import Any, Union
+
+# Third party modules
+import build
+import requests
+from bs4 import BeautifulSoup
+from colorama import Back, Fore, Style
+from jinja2 import Template
+from rich.console import Console
+from rich.table import Table
+from tqdm import tqdm
+
+# Local modules
+from . import meta, project_count, project_path, setup_text
+from .config import config
+from .utils import _check_version
+
+logger = logging.getLogger()
+
+
+def _feedback(message: str, feedback_type: str) -> None:
+    """Generates a formatted messages appropriate to the message type.
+
+    Args:
+        message:        Text to be echoed.
+        feedback_type:  identifies type of message to display.
+    """
+    if feedback_type not in ["null", "nominal", "warning", "error"]:
+        return
+    if config.idlemode == 1:
+        print(message)
+    else:
+        if feedback_type == "null":
+            print(Fore.WHITE + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
+        elif feedback_type == "nominal":
+            print(Fore.GREEN + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
+        elif feedback_type == "warning":
+            print(
+                Fore.YELLOW + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL
+            )
+        elif feedback_type == "error":
+            print(
+                Fore.RED
+                + Back.BLACK
+                + Style.BRIGHT
+                + f"ERROR: {message}"
+                + Style.RESET_ALL
+            )
+
+
+def _find_pypirc_file(filename: str = ".pypirc") -> None:
+    """Function to iterate over paths in the PATH environment variable to find a file.
+
+     Designed to find a .pypirc file starting with the current working directory.
+     If identified will update the config.pypirc variable, so it can be used elsewhere.
+
+    Args:
+        filename:       filename to find.
+    """
+    system_path = os.getenv("PATH")
+    if system_path is not None:
+        path_directories = [os.getcwd()]
+        path_directories.extend(system_path.split(os.pathsep))
+        for directory in path_directories:
+            file_path = Path(directory) / filename
+            if file_path.exists():
+                logger.debug(
+                    "%s is present in the system's PATH at %s", filename, directory
+                )
+                config.pypirc = file_path
+                break
+    logger.debug("%s is not present in the system's PATH.", filename)
+
+
+def _rename_project_dir(old_name: str, new_name: str) -> None:
+    """Utility script to rename a directory.
+
+    The object being to rename a 'template' directory for the purpose of creating a
+    minimalist package for upload to PyPI.
+
+    Args:
+        old_name:       source name.
+        new_name:       dst name.
+
+    Raises:
+        FileNotFoundError
+    """
+    old_directory_path = Path(old_name)
+    new_directory_path = Path(new_name)
+    logger.debug("renaming project directory from %s to %s", old_name, new_name)
+    try:
+        old_directory_path.rename(new_directory_path)
+    except FileNotFoundError:
+        logger.error("directory %s cannot be found:", old_directory_path)
+        raise FileNotFoundError
+
+
+def _create_setup(new_project_name: str, new_meta: bool = False) -> None:
+    """Utility script to create a setup.py file.
+
+    The object being to create a setup.py file from a 'template' file for the purpose of
+    creating a minimalist package for upload to PyPI.
+
+    Args:
+        new_project_name:       name used to render the template.
+    """
+    meta_file = project_path / "meta.pickle"
+    setup_file = project_path / "setup.txt"
+    setup_base_file = project_path / "setup_base.txt"
+    setup_file_py = project_path / "setup.py"
+
+    author = meta["author"] if meta else ""
+    email = meta["email"] if meta else ""
+    description = meta["description"] if meta else config.description
+    version = meta["version"] if meta else config.package_version
+
+    _email_pattern = (
+        r"[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*@(?:"
+        r"[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?"
+    )
+
+    if "AUTHOR" in setup_text or "EMAIL" in setup_text or not meta or new_meta:
+        try:
+            while True:
+                author = (
+                    input(
+                        Fore.YELLOW
+                        + Back.BLACK
+                        + Style.BRIGHT
+                        + f"Please enter your author name ({author}): "
+                        + Style.RESET_ALL
+                    )
+                    or author
+                )
+                if author != "":
+                    break
+        except KeyboardInterrupt:
+            _feedback("...bye!", "warning")
+            raise SystemExit()
+
+        try:
+            while True:
+                email = (
+                    input(
+                        Fore.YELLOW
+                        + Back.BLACK
+                        + Style.BRIGHT
+                        + f"Please enter your email address  ({email}): "
+                        + Style.RESET_ALL
+                    )
+                    or email
+                )
+                if re.search(_email_pattern, email):
+                    break
+                else:
+                    print(
+                        Fore.YELLOW
+                        + Back.BLACK
+                        + Style.BRIGHT
+                        + "does not appear to be a valid email address"
+                        + Style.RESET_ALL
+                    )
+        except KeyboardInterrupt:
+            _feedback("...bye!", "warning")
+            raise SystemExit()
+
+        try:
+            while True:
+                version = (
+                    input(
+                        Fore.YELLOW
+                        + Back.BLACK
+                        + Style.BRIGHT
+                        + f"version number: ({version}): "
+                        + Style.RESET_ALL
+                    )
+                    or version
+                )
+                if version != "":
+                    break
+        except KeyboardInterrupt:
+            raise SystemExit("Bye!")
+
+        try:
+            while True:
+                description = (
+                    input(
+                        Fore.YELLOW
+                        + Back.BLACK
+                        + Style.BRIGHT
+                        + f"description: ({description}): "
+                        + Style.RESET_ALL
+                    )
+                    or description
+                )
+                if description != "":
+                    break
+        except KeyboardInterrupt:
+            raise SystemExit("Bye!")
+
+        setup_file.unlink()
+
+        with open(setup_base_file, encoding="utf-8") as f:
+            setup_text_base = f.read()
+
+        template = Template(setup_text_base)
+        content = template.render(
+            PROJECT_NAME="{{ PROJECT_NAME }}",
+            PACKAGE_VERSION=version,
+            DESCRIPTION=description,
+            AUTHOR=author,
+            EMAIL=email,
+        )
+        with open(setup_file, mode="w", encoding="utf-8") as f:
+            f.write(content)
+
+    meta_save = {
+        "author": author,
+        "email": email,
+        "description": description,
+        "version": version,
+    }
+    with open(meta_file, "wb") as f:
+        pickle.dump(meta_save, f)
+
+    with open(setup_file) as f:
+        setup_text_file = f.read()
+        template = Template(setup_text_file)
+        content = template.render(
+            PROJECT_NAME=new_project_name,
+        )
+    with open(setup_file_py, mode="w", encoding="utf-8") as message:
+        logger.debug("creating new setup.py with the following: \n %s", content)
+        message.write(content)
+
+
+def _delete_director(items_to_delete: list[Path]) -> None:
+    """Utility function to delete files and directories.
+
+    Args:
+        items_to_delete:    A list of Path like objects to delete.
+    """
+    for item in items_to_delete:
+        if not item.exists():
+            logger.debug("trying to delete %s but it does not exist", item)
+            continue
+        if item.is_dir():
+            logger.debug("Deleting Directory: %s", item)
+            shutil.rmtree(item, ignore_errors=True)
+        else:
+            logger.debug("Deleting File: %s", item)
+            Path.unlink(item, missing_ok=True)
+
+
+def _run_command(
+    *arguments: str,
+    shell: bool = True,
+    working_dir: Union[Path, str, None] = None,
+    project: Union[None, str] = None,
+) -> None:  # pragma: no cover
+    """Utility designed to execute a command line utility.
+
+    Args:
+        arguments:  Comma separated strings- "utility", "arg1", "arg2", etc.
+        shell:      command executed by the shell or directly by the operating system.
+        cwd:        specifies the current working directory to use when starting
+                    the subprocess.
+                    e.g. "/home/user/mydir"
+        project:    the name of the project currently being tested
+    """
+    working_dir = os.getcwd() if working_dir is None else working_dir
+    try:
+        process = subprocess.Popen(
+            arguments,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            shell=shell,
+            text=True,
+            cwd=working_dir,
+        )
+        stdout, stderr = process.communicate()
+        if process.returncode != 0:
+            logger.error("Error running command: %s", arguments)
+            logger.error("stderr: %s", stderr)
+            if project is not None:
+                _cleanup(project)
+            return
+        logger.debug("%s", stdout)
+        return
+    except Exception as e:
+        logger.error("Exception running command: %s", arguments)
+        logger.error(e)
+        if project is not None:
+            _cleanup(project)
+        return
+
+
+def _is_valid_package_name(project_name: str) -> bool:
+    """Function does a basic check of project name validity.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Returns:
+        True:           If the name passes the basic check
+        False:          If the name fails the basic check
+
+
+    """
+    pattern = r"^[a-z][_\-a-z0-9]*$"
+    if re.match(pattern, project_name) is not None:
+        return True
+    else:
+        return False
+
+
+def _ping_project(project_name: str) -> bool:
+    """Determines if the URL to the project exists in PyPIs project area.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Returns:
+        True:           If the URLs response code is 200
+        False:          If the URLs response code is not 200
+
+    Raises:
+        SystemExit:     If any requests.RequestException occurs.
+    """
+    url_project = "".join([config.pypi_project_url, project_name, "/"])
+    logger.debug("attempting to get url %s", url_project)
+    try:
+        project_ping = requests.get(url_project, timeout=10)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    if project_ping.status_code == 200:
+        logger.debug("%s FOUND in the project area of PyPI", project_name)
+        return True
+    logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
+    return False
+
+
+def _ping_json(project_name: str) -> str:
+    """Collects some details about the project if it exists.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Raises:
+        SystemExit:     If any requests.RequestException occurs.
+    """
+    url_json = "".join([config.pypi_json_url, project_name, "/json"])
+    logger.debug("attempting to get url %s", url_json)
+    try:
+        project_json_raw = requests.get(url_json, timeout=10)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    if project_json_raw.status_code == 200:
+        project_json = json.loads(project_json_raw.content)
+        result = "".join(
+            [
+                project_json["info"]["author"],
+                "\n",
+                project_json["info"]["author_email"],
+                "\n",
+                project_json["info"]["version"],
+                "\n",
+                project_json["info"]["summary"],
+            ]
+        )
+        return result
+    logger.debug("No response from JSON URL")
+    return ""
+
+
+def _build_dist() -> None:
+    """Builds the sdist and wheel of the minimalist project to upload to PyPI."""
+    logger.debug("Building the distribution... ")
+    builder = build.ProjectBuilder(project_path)
+    builder.build("wheel", project_path / "dist")
+    builder.build("sdist", project_path / "dist")
+
+
+def _upload_dist(project_name: str) -> None:
+    """Builds the twine command line to upload the minimalist project to PyPI.
+
+    Args:
+        project_name:   the name of the project currently under test.
+
+    Notes:
+        twine expects a filesystem path not Path object so use os.fspath()
+    """
+    logger.debug("Uploading the distribution... ")
+    dir_path = os.fspath(project_path / "dist" / "*")
+    pypirc_path = os.fspath(config.pypirc)
+    _run_command(
+        sys.executable,
+        "-m",
+        "twine",
+        "upload",
+        "--config-file",
+        pypirc_path,
+        dir_path,
+        project=project_name,
+    )
+
+
+def _cleanup(project_name: str) -> None:
+    """Builds a manifest of artifacts to delete into a list of Path objects.
+
+    Args:
+        project_name:   the name of the project currently under test.
+    """
+    if config.no_cleanup is True:
+        return
+    _rename_project_dir(
+        project_path.joinpath(project_name),
+        project_path.joinpath(config.original_project_name),
+    )
+    build_artifacts = [
+        project_path / "build",
+        project_path / "dist",
+        project_path / "".join([project_name, ".egg-info"]),
+        project_path / "setup.py",
+    ]
+    logger.debug("cleaning build artifacts %s", build_artifacts)
+    _delete_director(build_artifacts)
+
+
+def _generate_pypi_index() -> None:
+    """Generates a list of projects in PyPI's simple index - writes results to a file.
+
+    Raises:
+        SystemExit:     If any requests.RequestException occurs.
+
+    Notes:
+        A potentially expensive operation as there are almost 500,000 projects to
+        process. Can take 2-3 seconds. Look to improve performance at a later date:
+        look at asyncio, asyncio.http etc.
+        An improvement is to automatically periodically run this in the background.
+    """
+    new_count = 0
+    pattern = re.compile(r">([\w\W]*?)<")
+    progress_bar = tqdm(total=config.project_count)
+    pypi_index = project_path / "pypi_index"
+    pypi_count = project_path / "project_count.pickle"
+    if pypi_index.exists():
+        Path.unlink(pypi_index, missing_ok=True)
+    try:
+        index_object_raw = requests.get(config.pypi_simple_index_url, timeout=10)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    with pypi_index.open(mode="a") as file:
+        for line in index_object_raw.iter_lines():
+            line = str(line)
+            project_text = re.search(pattern, line)
+            if project_text is not None:
+                new_count += 1
+                progress_bar.update(1)
+                project = "".join([project_text.group(1), " \n"])
+                file.write(project)
+    progress_bar.close()
+    with open(pypi_count, "wb") as f:
+        pickle.dump(new_count, f)
+
+
+def _pypi_search_index(project_name: str) -> bool:
+    """Open the generated index file and search for the project name.
+
+    Args:
+        project_name:   the name of the project currently under test.
+
+    Returns:
+        True:           A match was found.
+        False:          A match was not found.
+    """
+    pypi_index = project_path / "pypi_index"
+    if not pypi_index.exists():
+        _generate_pypi_index()
+    with pypi_index.open(mode="r") as file:
+        projects = file.read()
+        if project_name in projects:
+            logger.debug("%s FOUND in the PyPI simple index", project_name)
+            return True
+        logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
+        return False
+
+
+def _pypi_search(
+    search_project: str,
+) -> tuple[list[list[Union[str, Any]]], list[list[Union[str, Any]]], str]:
+    """Performs a get request to PyPI's search API for the project name.
+
+    Args:
+        search_project:   The name of the project currently under test.
+
+    Returns:
+        match:          A list of projects matching name comprising:
+                            [project_name, version, released, description]
+        others:         A list of projects not matching but PyPI thinks are relevant.
+                            [project_name, version, released, description]
+        others_total:   A str representation of total projects found (minus matches).
+    """
+    pattern = re.compile(r">([\d,+]*?)<")
+    s = requests.Session()
+    projects_raw: list = []
+    match: list[list[str]] = []
+    others: list[list[str]] = []
+    params = {"q": {search_project}, "page": 1}
+    r = s.get(config.pypi_search_url, params=params)  # type: ignore
+    soup = BeautifulSoup(r.text, "html.parser")
+    projects_raw.extend(soup.select('a[class*="package-snippet"]'))
+    for project_raw in projects_raw:
+        project_name = project_raw.select_one(
+            'span[class*="package-snippet__name"]'
+        ).text.strip()
+        version = project_raw.select_one(
+            'span[class*="package-snippet__version"]'
+        ).text.strip()
+        released_iso_8601 = project_raw.select_one(
+            'span[class*="package-snippet__created"]'
+        ).find("time")["datetime"]
+        released = datetime.strptime(released_iso_8601, "%Y-%m-%dT%H:%M:%S%z").strftime(
+            "%Y-%m-%d"
+        )
+        description = project_raw.select_one(
+            'p[class*="package-snippet__description"]'
+        ).text.strip()
+        if project_name.lower() == search_project.lower():
+            match.append([project_name, version, released, description])
+        else:
+            others.append([project_name, version, released, description])
+
+    total_div_raw = soup.select(
+        'div[class="split-layout split-layout--table split-layout--wrap-on-tablet"]'
+    )
+    total_raw = re.search(pattern, str(total_div_raw))
+    if total_raw is not None:
+        total_string = total_raw.group(1)
+        total = int(total_string.translate(str.maketrans("", "", string.punctuation)))
+        others_total = (
+            "".join([str(total), "+"])
+            if total == 10000
+            else (str(int(total) - len(match)))
+        )
+    else:
+        others_total = "0"
+    return match, others, others_total
+
+
+def _process_input_file(file: str) -> list[Union[str, Any]]:
+    """Processes the contents of the file to a list of strings.
+
+    Args:
+        file:           simple string for the file.
+
+    Raises:
+        SystemExit:     If the file is found to not exist.
+
+    Notes:
+        file contents should contain any number of space separated strings on any
+        number of lines.
+    """
+    file_path = Path(file)
+    try:
+        with file_path.open(mode="r") as f:
+            file_contents = f.read()
+            projects = file_contents.split()
+            return list(set(projects))
+    except FileNotFoundError:
+        _feedback(f"The file {file} does not exist", "warning")
+        raise SystemExit()  # pragma: no cover
+    except PermissionError:
+        _feedback(f"Permission denied to file: {file}", "warning")
+        raise SystemExit()  # pragma: no cover
+    except IsADirectoryError:
+        _feedback(f"{file} is a directory not a file", "warning")
+        raise SystemExit()  # pragma: no cover
+    except OSError:
+        _feedback(f"A general IO error has occurred opening file: {file}", "warning")
+        raise SystemExit()  # pragma: no cover
+    except Exception as e:
+        _feedback(f"An error occurred:, {str(e)}", "warning")
+        raise SystemExit()  # pragma: no cover
+
+
+def _write_output_file(file_name: str, results: dict) -> None:
+    """Write the results to a file
+
+    Args:
+        file_name:      Name of file to save as a simple string.
+        results:        Dictionary containing the test results e.g.
+                        {"pynball": [1, 1, 1]}
+    """
+    header_width = 83
+    truncation_width = 25
+    file_path = Path(file_name)
+    title = "Results from pynamer PyPI utility\n"
+    title = "".join([title, "=" * header_width, "\n\n"])
+    title = "".join(
+        [
+            title,
+            "Test 1 - Basic url lookup on PyPI\n",
+            "Test 2 - Search of PyPIs simple index\n",
+            "Test 3 - Search using an request to PyPIs search 'API'\n\n",
+        ]
+    )
+    header = f"{'Project':30}{'Test1':12}{'Test2':12}{'Test3':12}{'Conclusion'}\n"
+    header = "".join([header, "=" * header_width, "\n"])
+    projects_results: str = ""
+    for project in results:
+        project_name = (
+            project
+            if len(project) <= truncation_width
+            else project[: truncation_width - 3] + "..."
+        )
+        projects_results = "".join([projects_results, f"{project_name:30}"])
+        for test in results[project]:
+            test = "Found" if test == 1 else "Not Found"
+            projects_results = "".join([projects_results, f"{test:12}"])
+        conclusion = "Not Available" if sum(results[project]) > 0 else "Available"
+        projects_results = "".join([projects_results, f"{conclusion}"])
+        projects_results = "".join([projects_results, "\n", "-" * header_width, "\n"])
+
+    final_output_text = "".join([title, header, projects_results])
+
+    try:  # pragma: no cover
+        with file_path.open(mode="w") as f:
+            f.write(final_output_text)
+    except PermissionError:
+        _feedback(f"Permission denied to file: {file_path.open}", "warning")
+        raise SystemExit()  # pragma: no cover
+    except FileExistsError:
+        _feedback(f"File {file_path.open} already exists", "warning")
+        raise SystemExit()  # pragma: no cover
+    except IsADirectoryError:
+        _feedback(f"{file_path.open} is a directory not a file", "warning")
+        raise SystemExit()  # pragma: no cover
+    except OSError:
+        _feedback("General IO error has occurred", "warning")
+        raise SystemExit()  # pragma: no cover
+    except Exception as e:
+        _feedback(f"An error occurred:, {str(e)}", "warning")
+        raise SystemExit()  # pragma: no cover
+
+
+def _final_analysis(pattern: list[int]) -> None:
+    """Displays a rich console table displaying the conclusion of the test results
+
+    Args:
+        pattern:    A list of the test results:
+                    1 - A 'negative' result, indicating the project has been found.
+                    0 - A 'positive' result, indicating the project was not found.
+    """
+    table = Table(show_header=True)
+    table.add_column("FINAL ANALYSIS", style="bold cyan")
+    if pattern == [0, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search"
+            " facility.\n"
+            "It can only be found by searching the simple index which is not available "
+            "through the interface"
+        )
+    elif pattern == [1, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search"
+            " facility.\n"
+            "However if appears in the simple index and can be displayed by simply"
+            " browsing "
+            "to the projects URL"
+        )
+    elif sum(pattern) >= 1:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row("The package name was found in at least one place")
+    elif sum(pattern) == 0:
+        table.add_row("[green]AVAILABLE![/green]\n")
+        table.add_row("The package name was not found in any part of PyPI")
+
+    console = Console()
+    console.print(table)
+
+
+def _parse_args(args: list) -> tuple[argparse.Namespace, argparse.ArgumentParser]:
+    """Function to return the ArgumentParser object created from all the args.
+
+    Args:
+        args:   A list of arguments from the commandline
+                e.g. ['pynball', '-v', '-g']
+    """
+    parser = argparse.ArgumentParser(
+        prog="pynamer",
+        description="Determine if project name is available on pypi with the "
+        "option to 'register' it for future use if available",
+    )
+    parser.add_argument(
+        "projects",
+        nargs="*",
+        default="None",
+        help="Optional - one or more project names",
+    )
+    parser.add_argument(
+        "-r",
+        "--register",
+        action="store_true",
+        help="register the name on PyPi if the name is available",
+    )
+    parser.add_argument(
+        "-d",
+        "--dryrun",
+        action="store_true",
+        help=argparse.SUPPRESS,
+    )
+
+    parser.add_argument(
+        "-n",
+        "--nocleanup",
+        action="store_true",
+        help=argparse.SUPPRESS,
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="display information about similar projects",
+    )
+    parser.add_argument(
+        "-g",
+        "--generate",
+        action="store_true",
+        help="generate a new PyPI simple index",
+    )
+    parser.add_argument(
+        "-m",
+        "--meta",
+        action="store_true",
+        help="input new meta data when registering (Author and email address)",
+    )
+
+    parser.add_argument(
+        "-w",
+        "--webbrowser",
+        action="store_true",
+        help="open the project on PyPI in a webbrowser",
+    )
+
+    parser.add_argument(
+        "--version",
+        action="store_true",
+        help="display version number",
+    )
+    parser.add_argument(
+        "-f",
+        "--file",
+        default="None",
+        type=str,
+        help="file containing a list of projects to analyze",
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        default="None",
+        type=str,
+        help="file to store the test results",
+    )
+    return parser.parse_args(args), parser
+
+
+def main() -> None:  # pragma: no cover, type: ignore
+    args, parser = _parse_args(sys.argv[1:])
+    logger.debug(" args: %s", args)
+
+    if args.generate:
+        _generate_pypi_index()
+
+    if args.version:
+        version, message, result = _check_version()
+        if result:
+            _feedback(f"{version} : {message}", "nominal")
+        else:
+            _feedback(f"{version} : {message}", "warning")
+
+    if args.projects == "None" and args.file == "None" and args.register:
+        _feedback("You need to specify a project name to register it", "error")
+        raise SystemExit()
+
+    if args.projects == "None" and args.file == "None" and args.meta:
+        _feedback(
+            "You can only update the meta data during the registration process", "error"
+        )
+        raise SystemExit()
+
+    if (
+        args.projects == "None"
+        and args.file == "None"
+        and args.version is False
+        and args.generate is False
+    ):
+        parser.print_help()
+        raise SystemExit()
+
+    project_list = []
+    test_results = []
+    aggregated_result = {}
+    _find_pypirc_file()
+    if args.nocleanup is True:
+        config.no_cleanup = True
+
+    # Gather the projects into one list
+    if args.projects != "None":
+        logger.debug("adding project names from command line %s", args.projects)
+        project_list.extend(list(set(args.projects)))
+        logger.debug("project_list = %s", project_list)
+    if args.file != "None":
+        logger.debug("adding project names from file %s", args.file)
+        project_list.extend(_process_input_file(args.file))
+        logger.debug("project_list = %s", project_list)
+    project_list.sort()
+
+    # Main loop
+    for new_project in project_list:
+        if not _is_valid_package_name(new_project):
+            _feedback(f"{new_project} is not a valid package name", "error")
+            continue
+
+        test_table = Table(title=f"Test Results for {new_project}", show_lines=True)
+        test_table.add_column("No.", style="bold yellow")
+        test_table.add_column("Test", style="bold cyan")
+        test_table.add_column("Result")
+        test_table.add_column("Details", style="bold cyan")
+
+        match_table = Table(title=f"PyPI Search: Exact Match {new_project}")
+        match_table.add_column("Package", style="bold yellow")
+        match_table.add_column("Version", style="bold green")
+        match_table.add_column("Released", style="bold yellow")
+        match_table.add_column("Description", style="bold cyan")
+
+        others_table = Table(
+            title="Other Close Matches or Related Projects (from page 1)"
+        )
+        others_table.add_column("Package", style="bold yellow")
+        others_table.add_column("Version", style="bold green")
+        others_table.add_column("Released", style="bold yellow")
+        others_table.add_column("Description", style="bold cyan")
+
+        # perform the tests
+        # Test 1
+        if _ping_project(new_project):
+            test_results.append(1)
+            json_data = _ping_json(new_project)
+            test_table.add_row(
+                "1", "Basic http get to project URL", "[red]FOUND[/red]", json_data
+            )
+        else:
+            test_results.append(0)
+            test_table.add_row(
+                "1", "Basic http get to project URL", "[green]NOT FOUND[/green]", ""
+            )
+
+        # Test 2
+        if _pypi_search_index(new_project):
+            test_results.append(1)
+            test_table.add_row(
+                "2",
+                "Check PyPI simple index",
+                "[red]FOUND[/red]",
+                f"Searched {project_count} projects",
+            )
+        else:
+            test_results.append(0)
+            test_table.add_row(
+                "2",
+                "Check PyPI simple index",
+                "[green]NOT FOUND[/green]",
+                f"Searched {project_count} projects",
+            )
+
+        # Test 3
+        match, others, others_total = _pypi_search(new_project)
+        if match:
+            test_results.append(1)
+            test_table.add_row(
+                "3",
+                "Check PyPI search",
+                "[red]FOUND[/red]",
+                f"Exact match found: {len(match)}, Others found: {others_total}",
+            )
+            for items in match:
+                match_table.add_row(items[0], items[1], items[2], items[3])
+        else:
+            test_results.append(0)
+            test_table.add_row(
+                "3",
+                "Check PyPI search",
+                "[green]NOT FOUND[/green]",
+                f"Exact match found: 0, Others found: {others_total}",
+            )
+
+        # Create Verbose Table
+        if others:
+            for items in others:
+                others_table.add_row(items[0], items[1], items[2], items[3])
+
+        # Display the Tables
+        console = Console()
+        console.print(test_table)
+        if match:
+            console.print(match_table)
+        if args.verbose and others:
+            console.print(others_table)
+        _final_analysis(test_results)
+
+        # build and upload
+        if (
+            test_results == [0, 0, 0]
+            and args.register is True
+            and config.pypirc is not None
+            and len(project_list) == 1
+        ):
+            _create_setup(new_project, new_meta=args.meta)
+            _rename_project_dir(
+                project_path.joinpath(config.original_project_name),
+                project_path.joinpath(new_project),
+            )
+            _build_dist()
+            if args.dryrun is False:
+                _upload_dist(new_project)
+            else:
+                _feedback("Dryrun .... bypassing upload to PyPI..", "warning")
+            _cleanup(new_project)
+        elif config.pypirc is None:
+            _feedback(
+                ".pypirc file cannot be located ... wont attempt to 'register'",
+                "error",
+            )
+        elif sum(test_results) > 0 and args.register is True:
+            _feedback("Project already exists ... wont attempt to 'register'", "error")
+
+        aggregated_result[new_project] = test_results.copy()
+        test_results.clear()
+
+    if args.output != "None":
+        _write_output_file(args.output, aggregated_result)
+
+    if args.register and len(project_list) > 1:
+        _feedback(
+            f"You can only use 'register' for one project at a time. "
+            f"You have specified {len(project_list)} projects",
+            "warning",
+        )
+
+    if args.webbrowser:
+        if len(project_list) == 1:
+            url_project = "".join([config.pypi_project_url, project_list[0], "/"])
+            webbrowser.open(url_project)
+        else:
+            _feedback(
+                f"You must choose one project to open the webbrowser. "
+                f"You have chosen {len(project_list)} projects",
+                "warning",
+            )
+
+
+if __name__ == "__main__":
+    SystemExit(main())  # type: ignore
```

### Comparing `pynamer-1.3.1/src/pynamer/utils.py` & `pynamer-1.4.0/src/pynamer/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #!/usr/bin/env python3
 
 # Core Library modules
 import json
-from typing import Union
+from pathlib import Path
 
 # Third party modules
 import requests
 from packaging import version
 
 # First party modules
 import pynamer
 
 # Local modules
+from . import __version__, project_path
 from .config import config
 
 
-def _check_integrity() -> None:
+def _check_integrity():
     pass
 
 
-def _reset() -> None:
+def _reset():
     pass
 
 
-def _check_version() -> Union[tuple[version, str, bool], None]:
+def _check_version() -> tuple[version, str, bool]:
     """Utility function to compare package version against latest version on PyPI.
 
     Returns:
         current_version:    version of the installed package.
         str:                Message concerning the result of the comparison.
         bool:               True: if the installed package is up to date.
                             False: if there is a newer version on PyPI.
@@ -45,8 +46,7 @@
             return (
                 current_version,
                 f"(There is a newer version available: {pypi_version})",
                 False,
             )
         elif pypi_version == current_version:
             return current_version, "(You have the most recent version)", True
-    return None
```

### Comparing `pynamer-1.3.1/src/pynamer.egg-info/PKG-INFO` & `pynamer-1.4.0/src/pynamer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 1.3.1
+Version: 1.4.0
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -31,14 +31,15 @@
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
+[![pre-commit][pre-commit-image]][pre-commit-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -296,30 +297,20 @@
 ersa            Found       Found       Found           Not Available
 pandia          Not Found   Not Found   Found           Not Available
 leda            Not Found   Not Found   Not Found       Available
 ```
 
 Again you can use a combination of names from the command line and input file.
 
-## Register the package name with PyPI
+## Register the name with PyPI
 
 You can optionally 'register' the name on PyPI by using the -r argument.
-If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
+If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded to
 to PyPI.
 
-The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
-You can also optionally choose to change the version and description.
-
-![](assets/usage_register_first.png)
-
-This information will be retained and you will not be prompted to enter this information again. However, you can regenerate
-this meta data by using the -m argument along with the -r argument. You can just enter on the options you dont want to change.
-
-![](assets/usage_register_meta.png)
-
 ```bash
 ~ $ pynamer agrajag -r
 ```
 
 ![](assets/usage_register.png)
 
 ## Verbose output
@@ -339,29 +330,30 @@
 As one of its tests Pynamer makes use of a list of package names scraped from its simple index site.
 
 The PyPI Simple Index is a plain text file that lists the names of all the packages available on PyPI.
 
 It is a simplified version of the PyPI index that makes it easier for users to browse and download packages.
 
 The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
-The Index is updated every few hours.
 
-Using the -g argument can be used to regenerate the local file contents.
+The PyPI Simple Index is updated every few hours
+
+Using the -r argument can be used to regenerate the local file contents.
 
 ```bash
 ~ $ pynamer -g
 ```
 
 ![](assets/usage_generate.png)
 
 See planned future improvements
 
 ## The Oddities
 
-The reason I wrote this application in the first place...
+The reason I wrote this application in the first place.
 
 ```bash
 ~ $ pynamer zaphod
 ```
 
 ![](assets/usage_zaphod.png)
 
@@ -405,14 +397,15 @@
 -   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
 
 ## Planned Future improvements
 
 -   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
+-   Filter out invalid PyPI package names at the start
 
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
```

### Comparing `pynamer-1.3.1/src/pynamer.egg-info/SOURCES.txt` & `pynamer-1.4.0/src/pynamer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,18 @@
 tests/test_defaults.py
 tests/test_delete_director.py
 tests/test_feedback.py
 tests/test_final_analysis.py
 tests/test_find_pypirc_file.py
 tests/test_generate_pypi_index.py
 tests/test_is_valid_package_name.py
+tests/test_main TBC.py
 tests/test_ping_json.py
 tests/test_ping_project.py
 tests/test_process_input_file.py
 tests/test_pypi_search.py
 tests/test_pypi_search_index.py
 tests/test_rename_project_dir.py
+tests/test_run_command TBD.py
 tests/test_upload_dist.py
 tests/test_utils_version.py
 tests/test_write_output_file.py
```

### Comparing `pynamer-1.3.1/tests/test_args.py` & `pynamer-1.4.0/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_build_dist.py` & `pynamer-1.4.0/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_cleanup.py` & `pynamer-1.4.0/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_create_setup_file.py` & `pynamer-1.4.0/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_defaults.py` & `pynamer-1.4.0/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_delete_director.py` & `pynamer-1.4.0/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_feedback.py` & `pynamer-1.4.0/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_final_analysis.py` & `pynamer-1.4.0/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_find_pypirc_file.py` & `pynamer-1.4.0/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_generate_pypi_index.py` & `pynamer-1.4.0/tests/test_generate_pypi_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_ping_json.py` & `pynamer-1.4.0/tests/test_ping_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_ping_project.py` & `pynamer-1.4.0/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_process_input_file.py` & `pynamer-1.4.0/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_pypi_search.py` & `pynamer-1.4.0/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_rename_project_dir.py` & `pynamer-1.4.0/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_upload_dist.py` & `pynamer-1.4.0/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_utils_version.py` & `pynamer-1.4.0/tests/test_utils_version.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_write_output_file.py` & `pynamer-1.4.0/tests/test_write_output_file.py`

 * *Files identical despite different names*

