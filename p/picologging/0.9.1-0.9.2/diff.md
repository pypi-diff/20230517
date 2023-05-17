# Comparing `tmp/picologging-0.9.1.tar.gz` & `tmp/picologging-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picologging-0.9.1.tar", last modified: Wed Nov  9 23:18:09 2022, max compression
+gzip compressed data, was "picologging-0.9.2.tar", last modified: Wed May 17 04:09:42 2023, max compression
```

## Comparing `picologging-0.9.1.tar` & `picologging-0.9.2.tar`

### file list

```diff
@@ -1,107 +1,96 @@
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:09.064345 picologging-0.9.1/
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.043396 picologging-0.9.1/.devcontainer/
--rw-rw-rw-   0        0        0     1308 2022-06-14 02:17:26.000000 picologging-0.9.1/.devcontainer/Dockerfile
--rw-rw-rw-   0        0        0     2212 2022-06-14 02:17:26.000000 picologging-0.9.1/.devcontainer/devcontainer.json
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.060585 picologging-0.9.1/.github/
--rw-rw-rw-   0        0        0      501 2022-07-08 02:47:40.000000 picologging-0.9.1/.github/dependabot.yml
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.122850 picologging-0.9.1/.github/workflows/
--rw-rw-rw-   0        0        0     1731 2022-10-06 02:25:43.000000 picologging-0.9.1/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0     5447 2022-11-02 22:27:19.000000 picologging-0.9.1/.github/workflows/quality.yml
--rw-rw-rw-   0        0        0     1284 2022-11-02 22:27:19.000000 picologging-0.9.1/.github/workflows/test.yml
--rw-rw-rw-   0        0        0      640 2022-11-09 22:31:24.000000 picologging-0.9.1/.github/workflows/wheel.yml
--rw-rw-rw-   0        0        0      200 2022-11-02 22:27:19.000000 picologging-0.9.1/.gitignore
--rw-rw-rw-   0        0        0     7953 2022-11-09 22:31:24.000000 picologging-0.9.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1852 2022-11-02 22:27:19.000000 picologging-0.9.1/CMakeLists.txt
--rw-rw-rw-   0        0        0      444 2022-06-10 09:48:55.000000 picologging-0.9.1/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1141 2022-06-10 09:48:55.000000 picologging-0.9.1/LICENSE
--rw-rw-rw-   0        0        0     8899 2022-11-09 23:18:09.050066 picologging-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     7646 2022-11-02 22:27:19.000000 picologging-0.9.1/README.md
--rw-rw-rw-   0        0        0     2757 2022-06-10 09:48:55.000000 picologging-0.9.1/SECURITY.md
--rw-rw-rw-   0        0        0      461 2022-06-21 09:08:06.000000 picologging-0.9.1/SUPPORT.md
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:07.867380 picologging-0.9.1/_skbuild/
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:07.868800 picologging-0.9.1/_skbuild/win-amd64-3.9/
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:07.869815 picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:07.870970 picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.218453 picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/
--rw-rw-rw-   0        0        0    16757 2022-11-02 22:32:45.000000 picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/__init__.py
--rw-rw-rw-   0        0        0    10398 2022-11-02 22:32:45.000000 picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/__init__.pyi
--rw-rw-rw-   0        0        0    12956 2022-11-02 22:32:45.000000 picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/config.py
--rw-rw-rw-   0        0        0     1412 2022-11-02 22:32:45.000000 picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/config.pyi
--rw-rw-rw-   0        0        0    38064 2022-11-02 22:32:45.000000 picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/handlers.py
--rw-rw-rw-   0        0        0     4635 2022-11-02 22:32:45.000000 picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/handlers.pyi
--rw-rw-rw-   0        0        0        1 2022-11-02 22:32:45.000000 picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/py.typed
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.240482 picologging-0.9.1/benchmarks/
--rw-rw-rw-   0        0        0     5237 2022-11-02 22:27:19.000000 picologging-0.9.1/benchmarks/bench_handlers.py
--rw-rw-rw-   0        0        0     4432 2022-11-02 22:27:19.000000 picologging-0.9.1/benchmarks/bench_logger.py
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.282817 picologging-0.9.1/docs/
--rw-rw-rw-   0        0        0      638 2022-10-06 02:25:43.000000 picologging-0.9.1/docs/Makefile
--rwxrwxrwx   0        0        0      769 2022-10-06 02:25:43.000000 picologging-0.9.1/docs/make.bat
--rw-rw-rw-   0        0        0        4 2022-10-06 02:25:43.000000 picologging-0.9.1/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.352032 picologging-0.9.1/docs/source/
--rw-rw-rw-   0        0        0     1858 2022-10-06 02:25:43.000000 picologging-0.9.1/docs/source/conf.py
--rw-rw-rw-   0        0        0     1222 2022-10-06 02:25:43.000000 picologging-0.9.1/docs/source/examples.rst
--rw-rw-rw-   0        0        0     1833 2022-10-06 02:25:43.000000 picologging-0.9.1/docs/source/handlers.rst
--rw-rw-rw-   0        0        0     3004 2022-10-06 02:25:43.000000 picologging-0.9.1/docs/source/index.rst
--rw-rw-rw-   0        0        0     1008 2022-11-02 22:27:19.000000 picologging-0.9.1/docs/source/limitations.rst
--rw-rw-rw-   0        0        0      109 2022-10-06 02:25:43.000000 picologging-0.9.1/docs/source/logging.rst
--rw-rw-rw-   0        0        0      541 2022-11-09 22:31:24.000000 picologging-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-09 23:18:09.064345 picologging-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1662 2022-11-09 22:31:24.000000 picologging-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:07.878511 picologging-0.9.1/src/
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.618851 picologging-0.9.1/src/picologging/
--rw-rw-rw-   0        0        0    16757 2022-11-09 22:31:24.000000 picologging-0.9.1/src/picologging/__init__.py
--rw-rw-rw-   0        0        0    10416 2022-11-09 22:31:24.000000 picologging-0.9.1/src/picologging/__init__.pyi
--rw-rw-rw-   0        0        0     5754 2022-10-06 02:25:43.000000 picologging-0.9.1/src/picologging/_picologging.cxx
--rw-rw-rw-   0        0        0     1836 2022-06-21 09:08:06.000000 picologging-0.9.1/src/picologging/compat.hxx
--rw-rw-rw-   0        0        0    12956 2022-10-06 02:25:43.000000 picologging-0.9.1/src/picologging/config.py
--rw-rw-rw-   0        0        0     1412 2022-11-02 22:27:19.000000 picologging-0.9.1/src/picologging/config.pyi
--rw-rw-rw-   0        0        0     4977 2022-11-02 22:27:19.000000 picologging-0.9.1/src/picologging/filterer.cxx
--rw-rw-rw-   0        0        0      516 2022-10-06 02:25:43.000000 picologging-0.9.1/src/picologging/filterer.hxx
--rw-rw-rw-   0        0        0    18197 2022-10-06 02:25:43.000000 picologging-0.9.1/src/picologging/formatstyle.cxx
--rw-rw-rw-   0        0        0     1617 2022-07-08 02:47:40.000000 picologging-0.9.1/src/picologging/formatstyle.hxx
--rw-rw-rw-   0        0        0    13625 2022-11-02 22:27:19.000000 picologging-0.9.1/src/picologging/formatter.cxx
--rw-rw-rw-   0        0        0      846 2022-06-21 09:08:06.000000 picologging-0.9.1/src/picologging/formatter.hxx
--rw-rw-rw-   0        0        0     8664 2022-11-02 22:27:19.000000 picologging-0.9.1/src/picologging/handler.cxx
--rw-rw-rw-   0        0        0     1018 2022-07-08 02:47:40.000000 picologging-0.9.1/src/picologging/handler.hxx
--rw-rw-rw-   0        0        0    38064 2022-11-02 22:27:19.000000 picologging-0.9.1/src/picologging/handlers.py
--rw-rw-rw-   0        0        0     4635 2022-11-02 22:27:19.000000 picologging-0.9.1/src/picologging/handlers.pyi
--rw-rw-rw-   0        0        0    22615 2022-11-02 22:27:19.000000 picologging-0.9.1/src/picologging/logger.cxx
--rw-rw-rw-   0        0        0     2280 2022-11-02 22:27:19.000000 picologging-0.9.1/src/picologging/logger.hxx
--rw-rw-rw-   0        0        0    14982 2022-11-02 22:27:19.000000 picologging-0.9.1/src/picologging/logrecord.cxx
--rw-rw-rw-   0        0        0     1544 2022-10-06 02:25:43.000000 picologging-0.9.1/src/picologging/logrecord.hxx
--rw-rw-rw-   0        0        0      427 2022-10-06 02:25:43.000000 picologging-0.9.1/src/picologging/picologging.hxx
--rw-rw-rw-   0        0        0        1 2022-11-02 22:27:20.000000 picologging-0.9.1/src/picologging/py.typed
--rw-rw-rw-   0        0        0     6792 2022-11-02 22:27:20.000000 picologging-0.9.1/src/picologging/streamhandler.cxx
--rw-rw-rw-   0        0        0      544 2022-06-21 09:08:06.000000 picologging-0.9.1/src/picologging/streamhandler.hxx
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.670267 picologging-0.9.1/src/picologging.egg-info/
--rw-rw-rw-   0        0        0     8899 2022-11-09 23:18:07.000000 picologging-0.9.1/src/picologging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2547 2022-11-09 23:18:07.000000 picologging-0.9.1/src/picologging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-09 23:18:07.000000 picologging-0.9.1/src/picologging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2022-11-09 23:18:07.000000 picologging-0.9.1/src/picologging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-11-09 23:18:07.000000 picologging-0.9.1/src/picologging.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:07.885527 picologging-0.9.1/tests/
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.703090 picologging-0.9.1/tests/fuzzing/
--rw-rw-rw-   0        0        0     1844 2022-07-08 02:47:40.000000 picologging-0.9.1/tests/fuzzing/README.md
--rw-rw-rw-   0        0        0      435 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/fuzzing/fuzz_atheris.py
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.762993 picologging-0.9.1/tests/memray/
--rw-rw-rw-   0        0        0      563 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/memray/README.md
--rw-rw-rw-   0        0        0      520 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/memray/memray_format_exception.py
--rw-rw-rw-   0        0        0      703 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/memray/memray_logger.py
--rw-rw-rw-   0        0        0      908 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/memray/memray_logrecord.py
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:08.777260 picologging-0.9.1/tests/profile/
--rw-rw-rw-   0        0        0      538 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/profile/profile.py
-drwxrwxrwx   0        0        0        0 2022-11-09 23:18:09.044568 picologging-0.9.1/tests/unit/
--rw-rw-rw-   0        0        0     1174 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_bufferinghandler.py
--rw-rw-rw-   0        0        0     8800 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_config.py
--rw-rw-rw-   0        0        0     9334 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_filehandler.py
--rw-rw-rw-   0        0        0     7397 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_formatter.py
--rw-rw-rw-   0        0        0     3343 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_handler.py
--rw-rw-rw-   0        0        0    21492 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_logger.py
--rw-rw-rw-   0        0        0     4534 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_logrecord.py
--rw-rw-rw-   0        0        0     2629 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_percentstyle.py
--rw-rw-rw-   0        0        0     3702 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_picologging.py
--rw-rw-rw-   0        0        0     1826 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_queuehandler.py
--rw-rw-rw-   0        0        0     7669 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_sockethandler.py
--rw-rw-rw-   0        0        0     3492 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_streamhandler.py
--rw-rw-rw-   0        0        0     2943 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_strformatstyle.py
--rw-rw-rw-   0        0        0      482 2022-11-02 22:27:20.000000 picologging-0.9.1/tests/unit/test_threading.py
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.393905 picologging-0.9.2/
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.065846 picologging-0.9.2/.devcontainer/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1308 2022-09-01 01:16:52.000000 picologging-0.9.2/.devcontainer/Dockerfile
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     2295 2023-05-17 00:52:02.000000 picologging-0.9.2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.068050 picologging-0.9.2/.github/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      598 2023-05-17 02:51:27.000000 picologging-0.9.2/.github/dependabot.yml
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.135816 picologging-0.9.2/.github/workflows/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1731 2023-05-17 03:24:52.000000 picologging-0.9.2/.github/workflows/pages.yml
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     5447 2023-05-17 03:24:52.000000 picologging-0.9.2/.github/workflows/quality.yml
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1284 2023-05-17 03:24:52.000000 picologging-0.9.2/.github/workflows/test.yml
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      689 2023-05-17 03:24:52.000000 picologging-0.9.2/.github/workflows/wheel.yml
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      200 2022-10-28 22:01:12.000000 picologging-0.9.2/.gitignore
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     8714 2023-05-17 02:56:07.000000 picologging-0.9.2/CHANGELOG.md
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1852 2022-11-17 03:33:58.000000 picologging-0.9.2/CMakeLists.txt
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      444 2022-06-10 10:16:10.000000 picologging-0.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1141 2022-06-10 10:16:10.000000 picologging-0.9.2/LICENSE
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     8699 2023-05-17 04:09:42.390525 picologging-0.9.2/PKG-INFO
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     7661 2023-05-17 01:59:00.000000 picologging-0.9.2/README.md
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     2757 2022-06-10 10:16:10.000000 picologging-0.9.2/SECURITY.md
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      466 2023-05-17 00:52:02.000000 picologging-0.9.2/SUPPORT.md
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.142059 picologging-0.9.2/benchmarks/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     5237 2022-10-28 22:01:12.000000 picologging-0.9.2/benchmarks/bench_handlers.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     4432 2022-10-28 22:01:12.000000 picologging-0.9.2/benchmarks/bench_logger.py
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.162872 picologging-0.9.2/docs/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      638 2022-08-08 02:48:01.000000 picologging-0.9.2/docs/Makefile
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      769 2022-08-08 02:48:01.000000 picologging-0.9.2/docs/make.bat
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)        4 2022-08-08 02:48:01.000000 picologging-0.9.2/docs/requirements.txt
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.190691 picologging-0.9.2/docs/source/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1858 2022-08-08 02:48:10.000000 picologging-0.9.2/docs/source/conf.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1222 2022-08-08 02:48:01.000000 picologging-0.9.2/docs/source/examples.rst
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1833 2022-08-08 02:48:01.000000 picologging-0.9.2/docs/source/handlers.rst
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     3004 2022-08-08 02:48:01.000000 picologging-0.9.2/docs/source/index.rst
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1008 2022-11-08 01:30:25.000000 picologging-0.9.2/docs/source/limitations.rst
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      109 2022-08-08 02:48:01.000000 picologging-0.9.2/docs/source/logging.rst
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      719 2023-05-17 03:25:02.000000 picologging-0.9.2/pyproject.toml
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)       38 2023-05-17 04:09:42.394117 picologging-0.9.2/setup.cfg
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1662 2023-05-17 02:56:18.000000 picologging-0.9.2/setup.py
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:41.949864 picologging-0.9.2/src/
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.279047 picologging-0.9.2/src/picologging/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)    16757 2022-11-08 01:59:34.000000 picologging-0.9.2/src/picologging/__init__.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)    10468 2023-05-17 01:06:26.000000 picologging-0.9.2/src/picologging/__init__.pyi
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     5752 2023-05-17 01:59:00.000000 picologging-0.9.2/src/picologging/_picologging.cxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1836 2022-06-20 03:28:05.000000 picologging-0.9.2/src/picologging/compat.hxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)    12956 2022-10-28 22:00:59.000000 picologging-0.9.2/src/picologging/config.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1412 2022-10-28 22:00:59.000000 picologging-0.9.2/src/picologging/config.pyi
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     4977 2022-10-28 22:01:12.000000 picologging-0.9.2/src/picologging/filterer.cxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      516 2022-08-09 09:12:50.000000 picologging-0.9.2/src/picologging/filterer.hxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)    18323 2023-05-17 01:06:26.000000 picologging-0.9.2/src/picologging/formatstyle.cxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1647 2023-05-17 01:06:26.000000 picologging-0.9.2/src/picologging/formatstyle.hxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)    13647 2023-05-17 00:52:02.000000 picologging-0.9.2/src/picologging/formatter.cxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      846 2022-06-21 03:26:36.000000 picologging-0.9.2/src/picologging/formatter.hxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     8664 2022-10-28 22:01:12.000000 picologging-0.9.2/src/picologging/handler.cxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1018 2022-06-23 22:21:38.000000 picologging-0.9.2/src/picologging/handler.hxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)    38064 2022-10-28 22:01:12.000000 picologging-0.9.2/src/picologging/handlers.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     4635 2022-10-28 22:01:12.000000 picologging-0.9.2/src/picologging/handlers.pyi
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)    23376 2023-05-17 01:59:00.000000 picologging-0.9.2/src/picologging/logger.cxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     2342 2023-05-17 01:06:26.000000 picologging-0.9.2/src/picologging/logger.hxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)    14982 2022-10-28 22:01:12.000000 picologging-0.9.2/src/picologging/logrecord.cxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1544 2022-10-28 22:00:59.000000 picologging-0.9.2/src/picologging/logrecord.hxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      472 2023-05-17 01:59:00.000000 picologging-0.9.2/src/picologging/picologging.hxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)        1 2022-10-28 22:00:59.000000 picologging-0.9.2/src/picologging/py.typed
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     6797 2023-05-17 01:06:26.000000 picologging-0.9.2/src/picologging/streamhandler.cxx
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      544 2022-06-20 06:38:23.000000 picologging-0.9.2/src/picologging/streamhandler.hxx
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.290526 picologging-0.9.2/src/picologging.egg-info/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     8699 2023-05-17 04:09:41.000000 picologging-0.9.2/src/picologging.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     2125 2023-05-17 04:09:41.000000 picologging-0.9.2/src/picologging.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)        1 2023-05-17 04:09:41.000000 picologging-0.9.2/src/picologging.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)       64 2023-05-17 04:09:41.000000 picologging-0.9.2/src/picologging.egg-info/requires.txt
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)       12 2023-05-17 04:09:41.000000 picologging-0.9.2/src/picologging.egg-info/top_level.txt
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:41.956494 picologging-0.9.2/tests/
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.308514 picologging-0.9.2/tests/fuzzing/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1844 2022-06-27 23:30:16.000000 picologging-0.9.2/tests/fuzzing/README.md
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      435 2022-10-28 22:01:12.000000 picologging-0.9.2/tests/fuzzing/fuzz_atheris.py
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.320443 picologging-0.9.2/tests/memray/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      563 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/memray/README.md
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      520 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/memray/memray_format_exception.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      703 2023-05-17 00:51:56.000000 picologging-0.9.2/tests/memray/memray_logger.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      908 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/memray/memray_logrecord.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      518 2023-05-17 01:06:26.000000 picologging-0.9.2/tests/memray/memray_style.py
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.323805 picologging-0.9.2/tests/profile/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      538 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/profile/profile.py
+drwxr-xr-x   0 anthonyshaw   (501) staff       (20)        0 2023-05-17 04:09:42.386064 picologging-0.9.2/tests/unit/
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1174 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/unit/test_bufferinghandler.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     8800 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/unit/test_config.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     9334 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/unit/test_filehandler.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     7397 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/unit/test_formatter.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     3343 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/unit/test_handler.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)    22499 2023-05-17 01:59:00.000000 picologging-0.9.2/tests/unit/test_logger.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     4534 2023-05-17 00:51:56.000000 picologging-0.9.2/tests/unit/test_logrecord.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     2629 2023-05-17 00:54:21.000000 picologging-0.9.2/tests/unit/test_percentstyle.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     3702 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/unit/test_picologging.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     1826 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/unit/test_queuehandler.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     7669 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/unit/test_sockethandler.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     3492 2023-05-17 00:51:56.000000 picologging-0.9.2/tests/unit/test_streamhandler.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)     2943 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/unit/test_strformatstyle.py
+-rw-r--r--   0 anthonyshaw   (501) staff       (20)      482 2022-10-28 22:01:13.000000 picologging-0.9.2/tests/unit/test_threading.py
```

### Comparing `picologging-0.9.1/.devcontainer/Dockerfile` & `picologging-0.9.2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/.devcontainer/devcontainer.json` & `picologging-0.9.2/.devcontainer/devcontainer.json`

 * *Files 8% similar despite different names*

```diff
@@ -12,42 +12,43 @@
 			"VARIANT": "3.10",
 			// Options
 			"NODE_VERSION": "none"
 		}
 	},
 
 	// Set *default* container specific settings.json values on container create.
-	"settings": { 
-		"python.defaultInterpreterPath": "/usr/local/bin/python",
-		"python.linting.enabled": true,
-		"python.linting.pylintEnabled": true,
-		"python.formatting.autopep8Path": "/usr/local/py-utils/bin/autopep8",
-		"python.formatting.blackPath": "/usr/local/py-utils/bin/black",
-		"python.formatting.yapfPath": "/usr/local/py-utils/bin/yapf",
-		"python.linting.banditPath": "/usr/local/py-utils/bin/bandit",
-		"python.linting.flake8Path": "/usr/local/py-utils/bin/flake8",
-		"python.linting.mypyPath": "/usr/local/py-utils/bin/mypy",
-		"python.linting.pycodestylePath": "/usr/local/py-utils/bin/pycodestyle",
-		"python.linting.pydocstylePath": "/usr/local/py-utils/bin/pydocstyle",
-		"python.linting.pylintPath": "/usr/local/py-utils/bin/pylint",
-		"python.testing.pytestArgs": [
-			"tests"
-		],
-		"python.testing.cwd": "${workspaceFolder}",
-		"python.testing.unittestEnabled": false,
-		"python.testing.pytestEnabled": true
+	"customizations": {
+		"vscode": {
+			"settings": { 
+				"python.defaultInterpreterPath": "/usr/local/bin/python",
+				"python.linting.enabled": true,
+				"python.linting.pylintEnabled": true,
+				"python.formatting.autopep8Path": "/usr/local/py-utils/bin/autopep8",
+				"python.formatting.blackPath": "/usr/local/py-utils/bin/black",
+				"python.formatting.yapfPath": "/usr/local/py-utils/bin/yapf",
+				"python.linting.banditPath": "/usr/local/py-utils/bin/bandit",
+				"python.linting.flake8Path": "/usr/local/py-utils/bin/flake8",
+				"python.linting.mypyPath": "/usr/local/py-utils/bin/mypy",
+				"python.linting.pycodestylePath": "/usr/local/py-utils/bin/pycodestyle",
+				"python.linting.pydocstylePath": "/usr/local/py-utils/bin/pydocstyle",
+				"python.linting.pylintPath": "/usr/local/py-utils/bin/pylint",
+				"python.testing.pytestArgs": ["tests"],
+				"python.testing.cwd": "${workspaceFolder}",
+				"python.testing.unittestEnabled": false,
+				"python.testing.pytestEnabled": true
+			},
+			// Add the IDs of extensions you want installed when the container is created.
+			"extensions": [
+				"ms-python.python",
+				"ms-python.vscode-pylance",
+				"ms-vscode.cpptools"
+			]
+		}
 	},
-
-	// Add the IDs of extensions you want installed when the container is created.
-	"extensions": [
-		"ms-python.python",
-		"ms-python.vscode-pylance",
-		"ms-vscode.cpptools"
-	],
-
+	
 	// Use 'forwardPorts' to make a list of ports inside the container available locally.
 	// "forwardPorts": [],
 
 	// Use 'postCreateCommand' to run commands after the container is created.
 	"postCreateCommand": "python -m pip install -U pip setuptools wheel scikit-build pytest && python setup.py build_ext --inplace --build Debug",
 
 	// Comment out to connect as root instead. More info: https://aka.ms/vscode-remote/containers/non-root.
```

### Comparing `picologging-0.9.1/.github/workflows/pages.yml` & `picologging-0.9.2/.github/workflows/pages.yml`

 * *Files 2% similar despite different names*

```diff
@@ -23,29 +23,29 @@
   # Build job
   build:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
       - name: Setup python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.10"
           architecture: x64
       - name: Get latest CMake and ninja
         # Using 'latest' branch, the most recent CMake and ninja are installed.
         uses: lukka/get-cmake@latest
       - uses: actions/checkout@v3
       - name: Install requirements and package
         run: |
           python -m pip install -U pip
           python -m pip install scikit-build
           python -m pip install -v .
       - name: Setup Pages
-        uses: actions/configure-pages@v1
+        uses: actions/configure-pages@v3
       - name: Build HTML with sphinx
         run: |
           python -m pip install -r requirements.txt
           make html
         working-directory: docs/
       - name: Upload artifact
         uses: actions/upload-pages-artifact@v1
@@ -58,8 +58,8 @@
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     runs-on: ubuntu-latest
     needs: build
     steps:
       - name: Deploy to GitHub Pages
         id: deployment
-        uses: actions/deploy-pages@v1
+        uses: actions/deploy-pages@v2
```

### Comparing `picologging-0.9.1/.github/workflows/quality.yml` & `picologging-0.9.2/.github/workflows/quality.yml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # Initializes the CodeQL tools for scanning.
     - name: Initialize CodeQL
       uses: github/codeql-action/init@v2
       with:
         languages: ${{ matrix.language }}
 
     - name: Setup python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.10"
         architecture: x64
     - name: Get latest CMake and ninja
       # Using 'latest' branch, the most recent CMake and ninja are installed.
       uses: lukka/get-cmake@latest
     - name: Install and build package
@@ -119,15 +119,15 @@
   coverage:
     name: Coverage
     runs-on: ubuntu-latest
     steps:
     - name: Checkout repository
       uses: actions/checkout@v3
     - name: Setup python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.10"
         architecture: x64
     - name: Get latest CMake and ninja
       # Using 'latest' branch, the most recent CMake and ninja are installed.
       uses: lukka/get-cmake@latest
     - name: Install dependencies
@@ -148,15 +148,15 @@
   format:
     name: Check Formatting
     runs-on: ubuntu-latest
     steps:
     - name: Checkout repository
       uses: actions/checkout@v3
     - name: Setup python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.10"
         architecture: x64
     - name: Install dependencies
       run: python -m pip install -U pip black pyupgrade isort
     - name: Check Python Formatting
       run: black --check .
```

### Comparing `picologging-0.9.1/.github/workflows/test.yml` & `picologging-0.9.2/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     strategy:
       fail-fast: false
       matrix:
         os: ["macos-11", "ubuntu-20.04", "windows-latest"]
         python_version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     steps:
     - name: Setup python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python_version }}
         architecture: x64
     - name: Get latest CMake and ninja
       # Using 'latest' branch, the most recent CMake and ninja are installed.
       uses: lukka/get-cmake@latest
     - uses: actions/checkout@v3
```

### Comparing `picologging-0.9.1/.github/workflows/wheel.yml` & `picologging-0.9.2/.github/workflows/wheel.yml`

 * *Files 23% similar despite different names*

```diff
@@ -13,16 +13,20 @@
     strategy:
       fail-fast: false
       matrix:
         os: ["macos-11", ubuntu-20.04, "windows-latest"]
 
     steps:
       - uses: actions/checkout@v3
+      - name: Set up QEMU
+        if: runner.os == 'Linux'
+        uses: docker/setup-qemu-action@v2
+        with:
+          platforms: all
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.11.2
+        uses: pypa/cibuildwheel@v2.12.3
         env:
           CIBW_PRERELEASE_PYTHONS: True
-          CIBW_ARCHS_MACOS: x86_64 universal2
-          CIBW_ARCHS_WINDOWS: AMD64 x86 ARM64
-      - uses: actions/upload-artifact@v2
+
+      - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
```

### Comparing `picologging-0.9.1/CHANGELOG.md` & `picologging-0.9.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## 0.9.2
+
+* Upgrade pre-commit hooks versions by @sadikkuzu in https://github.com/microsoft/picologging/pull/133
+* Compile x86 for linux and windows. Compile aarch64 for linux by @tonybaloney in https://github.com/microsoft/picologging/pull/135
+* moves devcontainer vscode settings by @kjaymiller in https://github.com/microsoft/picologging/pull/143
+* Fix Formatter __repr__ by @aminalaee in https://github.com/microsoft/picologging/pull/141
+* Fix leaks in __dict__ and asctime fields by @tonybaloney in https://github.com/microsoft/picologging/pull/145
+* Add Logger isEnabledFor by @aminalaee in https://github.com/microsoft/picologging/pull/139
+* Support Logger.setLevel from string input by @tonybaloney in https://github.com/microsoft/picologging/pull/146
+
 ## 0.9.1
 
 * Add Windows Arm64 wheels by @aminalaee in https://github.com/microsoft/picologging/pull/130
 * Remove #22 as limitation since it's been fixed by @tonybaloney in https://github.com/microsoft/picologging/pull/128
 * Remove QueueListener test by @aminalaee in https://github.com/microsoft/picologging/pull/101
 
 ## 0.9.0
```

### Comparing `picologging-0.9.1/CMakeLists.txt` & `picologging-0.9.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/LICENSE` & `picologging-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/PKG-INFO` & `picologging-0.9.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,195 +1,192 @@
-Metadata-Version: 2.1
-Name: picologging
-Version: 0.9.1
-Summary: A fast and lightweight logging library for Python
-Home-page: https://github.com/microsoft/picologging
-Author: Microsoft
-License: MIT License
-Project-URL: Source, https://github.com/microsoft/picologging
-Project-URL: Documentation, https://microsoft.github.io/picologging/
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: System :: Logging
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# picologging
-
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/picologging)](https://pypi.org/project/picologging/)
-[![PyPI](https://img.shields.io/pypi/v/picologging)](https://pypi.org/project/picologging/)
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/picologging/badges/version.svg)](https://anaconda.org/conda-forge/picologging)
-[![codecov](https://codecov.io/gh/microsoft/picologging/branch/main/graph/badge.svg?token=KHs6FpQlVW)](https://codecov.io/gh/microsoft/picologging)
-
-> **Warning**
-> This project is in *beta*.
-> There are some incomplete features (see [Limitations](https://microsoft.github.io/picologging/limitations.html)).
-
-Picologging is a high-performance logging library for Python. picologging is 4-10x faster than the `logging` module in the standard library.
-
-Picologging is designed to be used as a *drop-in* replacement for applications which already use logging, and supports the same API as the `logging` module.
-
-Check out the [Documentation](https://microsoft.github.io/picologging/) for more.
-
-## Installation
-
-Picologging can be installed from PyPi using pip:
-
-```console
-pip install picologging
-```
-
-Or from conda forge using conda:
-
-```console
-conda install -c conda-forge picologging
-```
-
-## Usage
-
-Import `picologging as logging` to use picologging instead of the standard library logging module.
-
-This patches all the loggers registered to use picologging loggers and formatters.
-
-```python
-import picologging as logging
-logging.basicConfig()
-
-logger = logging.getLogger()
-
-logger.info("A log message!")
-
-logger.warning("A log message with %s", "arguments")
-```
-
-## Benchmarks
-
-Run `richbench benchmarks/ --markdown` with the richbench CLI to see the benchmarks, here is a sample on macOS 11:
-
-|                             Benchmark | Min     | Max     | Mean    | Min (+)         | Max (+)         | Mean (+)        |
-|---------------------------------------|---------|---------|---------|-----------------|-----------------|-----------------|
-|                         FileHandler() | 0.138   | 0.151   | 0.143   | 0.055 (2.5x)    | 0.063 (2.4x)    | 0.058 (2.5x)    |
-|                  WatchedFileHandler() | 0.189   | 0.197   | 0.193   | 0.097 (1.9x)    | 0.101 (1.9x)    | 0.099 (1.9x)    |
-|                 RotatingFileHandler() | 0.287   | 0.304   | 0.296   | 0.174 (1.6x)    | 0.178 (1.7x)    | 0.176 (1.7x)    |
-|                        QueueHandler() | 1.109   | 1.195   | 1.130   | 0.142 (7.8x)    | 0.151 (7.9x)    | 0.147 (7.7x)    |
-|      QueueListener() + QueueHandler() | 0.157   | 0.167   | 0.162   | 0.034 (4.6x)    | 0.039 (4.3x)    | 0.037 (4.3x)    |
-|                       MemoryHandler() | 0.126   | 0.144   | 0.133   | 0.051 (2.5x)    | 0.059 (2.5x)    | 0.054 (2.5x)    |
-|                           LogRecord() | 0.225   | 0.248   | 0.233   | 0.026 (8.7x)    | 0.029 (8.5x)    | 0.028 (8.4x)    |
-|                  Formatter().format() | 0.076   | 0.086   | 0.081   | 0.004 (18.7x)   | 0.005 (18.9x)   | 0.004 (19.1x)   |
-|        Formatter().format() with date | 0.298   | 0.311   | 0.304   | 0.081 (3.7x)    | 0.087 (3.6x)    | 0.084 (3.6x)    |
-|           Logger(level=DEBUG).debug() | 0.726   | 0.743   | 0.734   | 0.059 (12.3x)   | 0.061 (12.3x)   | 0.060 (12.3x)   |
-| Logger(level=DEBUG).debug() with args | 0.761   | 0.809   | 0.777   | 0.081 (9.4x)    | 0.087 (9.3x)    | 0.084 (9.2x)    |
-|            Logger(level=INFO).debug() | 0.016   | 0.018   | 0.017   | 0.004 (4.3x)    | 0.005 (3.8x)    | 0.004 (4.1x)    |
-|  Logger(level=INFO).debug() with args | 0.018   | 0.019   | 0.018   | 0.005 (3.8x)    | 0.005 (3.8x)    | 0.005 (3.7x)    |
-
-## Limitations
-
-See [Limitations](https://microsoft.github.io/picologging/limitations.html)
-
-## Contributing
-
-This project welcomes contributions and suggestions.  Most contributions require you to agree to a
-Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
-the rights to use your contribution. For details, visit [cla.opensource.microsoft.com](https://cla.opensource.microsoft.com).
-
-When you submit a pull request, a CLA bot will automatically determine whether you need to provide
-a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
-provided by the bot. You will only need to do this once across all repos using our CLA.
-
-This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
-For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
-contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
-
-## Local development
-
-This project comes bundled with a dev container which sets up an appropriate environment. If you install the Dev Containers extension for VS Code, then opening this project in VS Code should prompt it to open it in the dev container.
-
-Once opened in the dev container, run:
-
-```
-pip install -e ".[dev]"
-pre-commit install
-python setup.py build_ext --inplace --build-type Debug
-```
-
-Run the build command whenever you make changes to the files.
-
-It's also helpful to create a `.vscode/launch.json` file like this one:
-
-```
-{
-    "version": "0.2.0",
-    "configurations": [
-    {
-        "name": "(gdb) Launch pytest",
-        "type": "cppdbg",
-        "request": "launch",
-        "program": "/usr/local/bin/python",
-        "args": ["-m", "pytest", "tests"],
-        "stopAtEntry": false,
-        "cwd": "${workspaceFolder}",
-        "environment": [],
-        "externalConsole": false,
-        "MIMode": "gdb",
-        "setupCommands": [
-            {
-                "description": "Enable pretty-printing for gdb",
-                "text": "-enable-pretty-printing",
-                "ignoreFailures": true
-            },
-            {
-                "description":  "Set Disassembly Flavor to Intel",
-                "text": "-gdb-set disassembly-flavor intel",
-                "ignoreFailures": true
-            },
-        ]
-    }
-}
-```
-
-Now you can press the "Run and debug" button to run `pytest` from the `gdb` debugger
-and use breakpoint debugging in the C code.
-
-If you would like to be able to dive into the CPython code while debugging, then:
-
-1. Do a git checkout of the tagged branch for the devcontainer's Python version
-into the devcontainer's `/workspaces/` directory. You may need to `sudo`.
-2. Follow the instructions in the CPython README to compile the code.
-3. Add the following key to the the configuration in `launch.json`:
-    ```
-    "sourceFileMap": { "/usr/src/python": "/workspaces/cpython" },
-    ```
-4. Add the following command to the `setupCommands` in `launch.json`:
-    
-    ```
-    {
-        "description": "Find CPython source code",
-        "text": "-gdb-set auto-load safe-path /workspaces/cpython"
-    },
-    ```
-
-## Trademarks
-
-Some components of this Python package are from CPython 3.11 logging library for compatibility reasons.
-
-CPython 3.11 is licensed under the PSF license.
-The logging module is Copyright (C) 2001-2019 Vinay Sajip. All Rights Reserved.
-
-This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
-trademarks or logos is subject to and must follow 
-[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
-Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
-Any use of third-party trademarks or logos are subject to those third-party's policies.
-
-
+Metadata-Version: 2.1
+Name: picologging
+Version: 0.9.2
+Summary: A fast and lightweight logging library for Python
+Home-page: https://github.com/microsoft/picologging
+Author: Microsoft
+License: MIT License
+Project-URL: Source, https://github.com/microsoft/picologging
+Project-URL: Documentation, https://microsoft.github.io/picologging/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: System :: Logging
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# picologging
+
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/picologging)](https://pypi.org/project/picologging/)
+[![PyPI](https://img.shields.io/pypi/v/picologging)](https://pypi.org/project/picologging/)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/picologging/badges/version.svg)](https://anaconda.org/conda-forge/picologging)
+[![codecov](https://codecov.io/gh/microsoft/picologging/branch/main/graph/badge.svg?token=KHs6FpQlVW)](https://codecov.io/gh/microsoft/picologging)
+
+> **Warning**
+> This project is in *beta*.
+> There are some incomplete features (see [Limitations](https://microsoft.github.io/picologging/limitations.html)).
+
+Picologging is a high-performance logging library for Python. picologging is 4-10x faster than the `logging` module in the standard library.
+
+Picologging is designed to be used as a *drop-in* replacement for applications which already use logging, and supports the same API as the `logging` module.
+
+Check out the [Documentation](https://microsoft.github.io/picologging/) for more.
+
+## Installation
+
+Picologging can be installed from PyPi using pip:
+
+```console
+pip install picologging
+```
+
+Or from conda forge using conda:
+
+```console
+conda install -c conda-forge picologging
+```
+
+## Usage
+
+Import `picologging as logging` to use picologging instead of the standard library logging module.
+
+This patches all the loggers registered to use picologging loggers and formatters.
+
+```python
+import picologging as logging
+logging.basicConfig()
+
+logger = logging.getLogger()
+
+logger.info("A log message!")
+
+logger.warning("A log message with %s", "arguments")
+```
+
+## Benchmarks
+
+Run `richbench benchmarks/ --markdown` with the richbench CLI to see the benchmarks, here is a sample on macOS 11:
+
+|                             Benchmark | Min     | Max     | Mean    | Min (+)         | Max (+)         | Mean (+)        |
+|---------------------------------------|---------|---------|---------|-----------------|-----------------|-----------------|
+|                         FileHandler() | 0.138   | 0.151   | 0.143   | 0.055 (2.5x)    | 0.063 (2.4x)    | 0.058 (2.5x)    |
+|                  WatchedFileHandler() | 0.189   | 0.197   | 0.193   | 0.097 (1.9x)    | 0.101 (1.9x)    | 0.099 (1.9x)    |
+|                 RotatingFileHandler() | 0.287   | 0.304   | 0.296   | 0.174 (1.6x)    | 0.178 (1.7x)    | 0.176 (1.7x)    |
+|                        QueueHandler() | 1.109   | 1.195   | 1.130   | 0.142 (7.8x)    | 0.151 (7.9x)    | 0.147 (7.7x)    |
+|      QueueListener() + QueueHandler() | 0.157   | 0.167   | 0.162   | 0.034 (4.6x)    | 0.039 (4.3x)    | 0.037 (4.3x)    |
+|                       MemoryHandler() | 0.126   | 0.144   | 0.133   | 0.051 (2.5x)    | 0.059 (2.5x)    | 0.054 (2.5x)    |
+|                           LogRecord() | 0.225   | 0.248   | 0.233   | 0.026 (8.7x)    | 0.029 (8.5x)    | 0.028 (8.4x)    |
+|                  Formatter().format() | 0.076   | 0.086   | 0.081   | 0.004 (18.7x)   | 0.005 (18.9x)   | 0.004 (19.1x)   |
+|        Formatter().format() with date | 0.298   | 0.311   | 0.304   | 0.081 (3.7x)    | 0.087 (3.6x)    | 0.084 (3.6x)    |
+|           Logger(level=DEBUG).debug() | 0.726   | 0.743   | 0.734   | 0.059 (12.3x)   | 0.061 (12.3x)   | 0.060 (12.3x)   |
+| Logger(level=DEBUG).debug() with args | 0.761   | 0.809   | 0.777   | 0.081 (9.4x)    | 0.087 (9.3x)    | 0.084 (9.2x)    |
+|            Logger(level=INFO).debug() | 0.016   | 0.018   | 0.017   | 0.004 (4.3x)    | 0.005 (3.8x)    | 0.004 (4.1x)    |
+|  Logger(level=INFO).debug() with args | 0.018   | 0.019   | 0.018   | 0.005 (3.8x)    | 0.005 (3.8x)    | 0.005 (3.7x)    |
+
+## Limitations
+
+See [Limitations](https://microsoft.github.io/picologging/limitations.html)
+
+## Contributing
+
+This project welcomes contributions and suggestions.  Most contributions require you to agree to a
+Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
+the rights to use your contribution. For details, visit [cla.opensource.microsoft.com](https://cla.opensource.microsoft.com).
+
+When you submit a pull request, a CLA bot will automatically determine whether you need to provide
+a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
+provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
+For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
+contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
+
+## Local development
+
+This project comes bundled with a dev container which sets up an appropriate environment. If you install the Dev Containers extension for VS Code, then opening this project in VS Code should prompt it to open it in the dev container.
+
+Once opened in the dev container, run:
+
+```console
+pip install -e ".[dev]"
+pre-commit install
+python setup.py build_ext --inplace --build-type Debug
+```
+
+Run the build command whenever you make changes to the files.
+
+It's also helpful to create a `.vscode/launch.json` file like this one:
+
+```json
+{
+    "version": "0.2.0",
+    "configurations": [
+    {
+        "name": "(gdb) Launch pytest",
+        "type": "cppdbg",
+        "request": "launch",
+        "program": "/usr/local/bin/python",
+        "args": ["-m", "pytest", "tests"],
+        "stopAtEntry": false,
+        "cwd": "${workspaceFolder}",
+        "environment": [],
+        "externalConsole": false,
+        "MIMode": "gdb",
+        "setupCommands": [
+            {
+                "description": "Enable pretty-printing for gdb",
+                "text": "-enable-pretty-printing",
+                "ignoreFailures": true
+            },
+            {
+                "description":  "Set Disassembly Flavor to Intel",
+                "text": "-gdb-set disassembly-flavor intel",
+                "ignoreFailures": true
+            },
+        ]
+    }
+}
+```
+
+Now you can press the "Run and debug" button to run `pytest` from the `gdb` debugger
+and use breakpoint debugging in the C code.
+
+If you would like to be able to dive into the CPython code while debugging, then:
+
+1. Do a git checkout of the tagged branch for the devcontainer's Python version
+into the devcontainer's `/workspaces/` directory. You may need to `sudo`.
+2. Follow the instructions in the CPython README to compile the code.
+3. Add the following key to the the configuration in `launch.json`:
+
+    ```json
+    "sourceFileMap": { "/usr/src/python": "/workspaces/cpython" },
+    ```
+
+4. Add the following command to the `setupCommands` in `launch.json`:
+
+    ```json
+    {
+        "description": "Find CPython source code",
+        "text": "-gdb-set auto-load safe-path /workspaces/cpython"
+    },
+    ```
+
+## Trademarks
+
+Some components of this Python package are from CPython 3.11 logging library for compatibility reasons.
+
+CPython 3.11 is licensed under the PSF license.
+The logging module is Copyright (C) 2001-2019 Vinay Sajip. All Rights Reserved.
+
+This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft trademarks or logos is subject to and must follow [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
+Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
+Any use of third-party trademarks or logos are subject to those third-party's policies.
```

### Comparing `picologging-0.9.1/README.md` & `picologging-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,25 @@
 
 ## Local development
 
 This project comes bundled with a dev container which sets up an appropriate environment. If you install the Dev Containers extension for VS Code, then opening this project in VS Code should prompt it to open it in the dev container.
 
 Once opened in the dev container, run:
 
-```
+```console
 pip install -e ".[dev]"
 pre-commit install
 python setup.py build_ext --inplace --build-type Debug
 ```
 
 Run the build command whenever you make changes to the files.
 
 It's also helpful to create a `.vscode/launch.json` file like this one:
 
-```
+```json
 {
     "version": "0.2.0",
     "configurations": [
     {
         "name": "(gdb) Launch pytest",
         "type": "cppdbg",
         "request": "launch",
@@ -136,31 +136,31 @@
 
 If you would like to be able to dive into the CPython code while debugging, then:
 
 1. Do a git checkout of the tagged branch for the devcontainer's Python version
 into the devcontainer's `/workspaces/` directory. You may need to `sudo`.
 2. Follow the instructions in the CPython README to compile the code.
 3. Add the following key to the the configuration in `launch.json`:
-    ```
+
+    ```json
     "sourceFileMap": { "/usr/src/python": "/workspaces/cpython" },
     ```
+
 4. Add the following command to the `setupCommands` in `launch.json`:
-    
-    ```
+
+    ```json
     {
         "description": "Find CPython source code",
         "text": "-gdb-set auto-load safe-path /workspaces/cpython"
     },
     ```
 
 ## Trademarks
 
 Some components of this Python package are from CPython 3.11 logging library for compatibility reasons.
 
 CPython 3.11 is licensed under the PSF license.
 The logging module is Copyright (C) 2001-2019 Vinay Sajip. All Rights Reserved.
 
-This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
-trademarks or logos is subject to and must follow 
-[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
+This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft trademarks or logos is subject to and must follow [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
 Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
 Any use of third-party trademarks or logos are subject to those third-party's policies.
```

### Comparing `picologging-0.9.1/SECURITY.md` & `picologging-0.9.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/__init__.py` & `picologging-0.9.2/src/picologging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Formatter,
     Logger,
     LogRecord,
     StreamHandler,
     getLevelName,
 )
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 CRITICAL = 50
 FATAL = CRITICAL
 ERROR = 40
 WARNING = 30
 WARN = WARNING
 INFO = 20
```

### Comparing `picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/__init__.pyi` & `picologging-0.9.2/src/picologging/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from string import Template
 from types import TracebackType
 from typing import Any, Generic, Optional, Pattern, TextIO, TypeVar, Union, overload
 
 from _typeshed import StrPath, SupportsWrite
 from typing_extensions import Literal, TypeAlias
 
+__version__: str
+
 CRITICAL: int
 FATAL: int
 ERROR: int
 WARNING: int
 WARN: int
 INFO: int
 DEBUG: int
@@ -138,14 +140,15 @@
     parent: Logger
     handlers: list[Handler]
     disabled: bool
     manager: Optional[Manager]
     def __init__(self, name: str, level: _Level = ...) -> None: ...
     def setLevel(self, level: _Level) -> None: ...
     def getEffectiveLevel(self) -> int: ...
+    def isEnabledFor(self, level: int) -> bool: ...
     def debug(
         self,
         msg: object,
         *args: object,
         exc_info: _ExcInfoType = ...,
         stack_info: bool = ...,
         stacklevel: int = ...,
```

### Comparing `picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/config.py` & `picologging-0.9.2/src/picologging/config.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/config.pyi` & `picologging-0.9.2/src/picologging/config.pyi`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/handlers.py` & `picologging-0.9.2/src/picologging/handlers.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/_skbuild/win-amd64-3.9/cmake-install/src/picologging/handlers.pyi` & `picologging-0.9.2/src/picologging/handlers.pyi`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/benchmarks/bench_handlers.py` & `picologging-0.9.2/benchmarks/bench_handlers.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/benchmarks/bench_logger.py` & `picologging-0.9.2/benchmarks/bench_logger.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/docs/Makefile` & `picologging-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/docs/make.bat` & `picologging-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/docs/source/conf.py` & `picologging-0.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/docs/source/examples.rst` & `picologging-0.9.2/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/docs/source/handlers.rst` & `picologging-0.9.2/docs/source/handlers.rst`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/docs/source/index.rst` & `picologging-0.9.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/docs/source/limitations.rst` & `picologging-0.9.2/docs/source/limitations.rst`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/setup.py` & `picologging-0.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup(
     name="picologging",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "picologging": ["py.typed", "__init__.pyi", "config.pyi", "handlers.pyi"]
     },
-    version="0.9.1",
+    version="0.9.2",
     author="Microsoft",
     description="A fast and lightweight logging library for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/microsoft/picologging",
     license="MIT License",
     classifiers=[
```

### Comparing `picologging-0.9.1/src/picologging/_picologging.cxx` & `picologging-0.9.2/src/picologging/_picologging.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   if (it == LEVELS_TO_NAMES.end()){
     return "";
   }
 
   return it->second;
 }
 
-short _getLevelByName(std::string levelName) {
+short getLevelByName(std::string levelName) {
   std::unordered_map<std::string, short>::const_iterator it;
   it = NAMES_TO_LEVELS.find(levelName);
 
   if (it == NAMES_TO_LEVELS.end()){
     return -1;
   }
 
@@ -61,15 +61,15 @@
       return PyUnicode_FromString(levelName.c_str());
     }
     PyErr_Format(PyExc_ValueError, "Invalid level value: %d", levelValue);
     return nullptr;
   }
 
   if (PyUnicode_Check(level)) {
-    short levelValue = _getLevelByName(PyUnicode_AsUTF8(level));
+    short levelValue = getLevelByName(PyUnicode_AsUTF8(level));
     if (levelValue >= 0) {
       return PyLong_FromLong(levelValue);
     }
     PyErr_Format(PyExc_ValueError, "Invalid level value: %U", level);
     return nullptr;
   }
```

### Comparing `picologging-0.9.1/src/picologging/compat.hxx` & `picologging-0.9.2/src/picologging/compat.hxx`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/src/picologging/filterer.cxx` & `picologging-0.9.2/src/picologging/filterer.cxx`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/src/picologging/filterer.hxx` & `picologging-0.9.2/src/picologging/filterer.hxx`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/src/picologging/formatstyle.cxx` & `picologging-0.9.2/src/picologging/formatstyle.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -139,33 +139,37 @@
         self->fragments[idx].fragment = PyUnicode_FromString(format_string.substr(cursor, format_string.size() - cursor).c_str());
         idx ++;
     }
     self->defaults = defaults;
     Py_INCREF(defaults);
 
     self->_const_format = PyUnicode_FromString("format");
+    self->_const__dict__ = PyUnicode_FromString("__dict__");
 
     return 0;
 }
 
 PyObject* FormatStyle_usesTime(FormatStyle *self){
     if (self->usesDefaultFmt)
         Py_RETURN_FALSE;
     int ret = 0;
+    PyObject* asctime = nullptr;
     switch (self->style){
         case '%':
-            ret = PyUnicode_Find(self->fmt, PyUnicode_FromString("%(asctime)"), 0, PyUnicode_GET_LENGTH(self->fmt), 1);
+            asctime = PyUnicode_FromString("%(asctime)");
             break;
         case '{':
-            ret = PyUnicode_Find(self->fmt, PyUnicode_FromString("{asctime}"), 0, PyUnicode_GET_LENGTH(self->fmt), 1);
+            asctime = PyUnicode_FromString("{asctime}");
             break;
         default:
             PyErr_SetString(PyExc_ValueError, "Invalid style value");
             return nullptr;
     }
+    ret = PyUnicode_Find(self->fmt, asctime, 0, PyUnicode_GET_LENGTH(self->fmt), 1);
+    Py_XDECREF(asctime);
     if (ret >= 0){
         Py_RETURN_TRUE;
     } else if (ret == -1){
         Py_RETURN_FALSE;
     } else { // -2
         // Encountered error .
         return nullptr;
@@ -298,15 +302,15 @@
                         PyErr_SetString(PyExc_ValueError, "Unknown field");
                         _PyUnicodeWriter_Dealloc(&writer);
                         return nullptr;
                 }
             }
             return _PyUnicodeWriter_Finish(&writer);
         } else {
-            PyObject* recordDict = PyObject_GetAttrString(record, "__dict__");
+            PyObject* recordDict = PyObject_GetAttr(record, self->_const__dict__);
             if (recordDict == nullptr)
                 return nullptr;
             PyObject* result = nullptr;
             switch (self->style){
                 case '%':
                     result = PyUnicode_Format(self->fmt, recordDict);
                     break;
@@ -315,15 +319,15 @@
                     break;
             }
             Py_DECREF(recordDict);
             return result;
         }
     }
 
-    PyObject* dict = PyObject_GetAttrString(record, "__dict__");
+    PyObject* dict = PyObject_GetAttr(record, self->_const__dict__);
     if (PyDict_Merge(dict, self->defaults, 1) < 0){
         Py_DECREF(dict);
         return nullptr;
     }
     PyObject* result = nullptr;
     switch (self->style){
         case '%':
@@ -399,14 +403,15 @@
     return (PyObject*)self;
 }
 
 PyObject* FormatStyle_dealloc(FormatStyle *self){
     Py_XDECREF(self->fmt);
     Py_XDECREF(self->defaults);
     Py_XDECREF(self->_const_format);
+    Py_XDECREF(self->_const__dict__);
     for (int i = 0 ; i < self->ob_base.ob_size; i++){
         Py_XDECREF(self->fragments[i].fragment);
     }
     Py_TYPE(self)->tp_free((PyObject*)self);
     return NULL;
 }
```

### Comparing `picologging-0.9.1/src/picologging/formatstyle.hxx` & `picologging-0.9.2/src/picologging/formatstyle.hxx`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 typedef struct {
     PyObject_VAR_HEAD
     PyObject *fmt;
     PyObject *defaults;
     bool usesDefaultFmt;
     int style;
     PyObject* _const_format;
+    PyObject* _const__dict__;
     FormatFragment fragments[1];
 } FormatStyle;
 
 int FormatStyle_init(FormatStyle *self, PyObject *args, PyObject *kwds);
 PyObject* FormatStyle_usesTime(FormatStyle *self);
 PyObject* FormatStyle_validate(FormatStyle *self);
 PyObject* FormatStyle_format(FormatStyle *self, PyObject *record);
```

### Comparing `picologging-0.9.1/src/picologging/formatter.cxx` & `picologging-0.9.2/src/picologging/formatter.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -261,16 +261,16 @@
         s = s2;
     }
     return s;
 }
 
 PyObject* Formatter_repr(Formatter *self)
 {
-    return PyUnicode_FromFormat("<Formatter: fmt='%U'>",
-            self->fmt);
+    return PyUnicode_FromFormat("<%s: fmt='%U'>",
+            _PyType_Name(Py_TYPE(self)), self->fmt);
 }
 
 PyObject* Formatter_dealloc(Formatter *self) {
     Py_XDECREF(self->fmt);
     Py_XDECREF(self->dateFmt);
     Py_XDECREF(self->style);
     Py_XDECREF(self->_const_line_break);
```

### Comparing `picologging-0.9.1/src/picologging/formatter.hxx` & `picologging-0.9.2/src/picologging/formatter.hxx`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/src/picologging/handler.cxx` & `picologging-0.9.2/src/picologging/handler.cxx`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/src/picologging/handler.hxx` & `picologging-0.9.2/src/picologging/handler.hxx`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/src/picologging/logger.cxx` & `picologging-0.9.2/src/picologging/logger.cxx`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,14 @@
             ((Logger*)child_logger)->effective_level = level;
             setEnabledBasedOnEffectiveLevel((Logger*)child_logger);
             setEffectiveLevelOfChildren((Logger*)child_logger, level);
         }
     }
 }
 
-
-
 PyObject* Logger_new(PyTypeObject* type, PyObject* args, PyObject* kwds)
 {
     Logger* self = (Logger*)FiltererType.tp_new(type, args, kwds);
     if (self != NULL)
     {
         self->name = Py_None;
         Py_INCREF(self->name);
@@ -138,19 +136,28 @@
 
 PyObject* Logger_repr(Logger *self) {
     std::string level = _getLevelName(self->effective_level);
     return PyUnicode_FromFormat("<Logger '%U' (%s)>", self->name, level.c_str());
 }
 
 PyObject* Logger_setLevel(Logger *self, PyObject *level) {
-    if (!PyLong_Check(level)) {
+    if (PyLong_Check(level)) {
+        self->level = (unsigned short)PyLong_AsUnsignedLongMask(level);
+    }
+    else if (PyUnicode_Check(level)){
+        short levelValue = getLevelByName(PyUnicode_AsUTF8(level));
+        if (levelValue < 0) {
+            PyErr_Format(PyExc_ValueError, "Invalid level value: %U", level);
+            return nullptr;
+        }
+        self->level = levelValue;
+    } else {
         PyErr_SetString(PyExc_TypeError, "level must be an integer");
         return NULL;
     }
-    self->level = (unsigned short)PyLong_AsUnsignedLongMask(level);
     self->effective_level = self->level;
     setEnabledBasedOnEffectiveLevel(self);
     setEffectiveLevelOfChildren(self, self->level);
     Py_RETURN_NONE;
 }
 
 PyObject* Logger_getEffectiveLevel(Logger *self){
@@ -517,19 +524,31 @@
 
     // Rescan parent levels.
     self->effective_level = findEffectiveLevelFromParents(self);
     setEnabledBasedOnEffectiveLevel(self);
     return 0;
 }
 
+PyObject* Logger_isEnabledFor(Logger *self, PyObject *level) {
+    if (!PyLong_Check(level)) {
+        PyErr_SetString(PyExc_TypeError, "level must be an integer");
+        return NULL;
+    }
+    if (self->disabled || (unsigned short)PyLong_AsUnsignedLongMask(level) < self->effective_level) {
+        return Py_False;
+    }
+    return Py_True;
+}
+
 static PyMethodDef Logger_methods[] = {
     {"setLevel", (PyCFunction)Logger_setLevel, METH_O, "Set the level of the logger."},
     {"getEffectiveLevel", (PyCFunction)Logger_getEffectiveLevel, METH_NOARGS, "Get the effective level of the logger."},
     {"addHandler", (PyCFunction)Logger_addHandler, METH_O, "Add a handler to the logger."},
     {"removeHandler", (PyCFunction)Logger_removeHandler, METH_O, "Remove a handler from the logger."},
+    {"isEnabledFor", (PyCFunction)Logger_isEnabledFor, METH_O, "Check if logger enabled for this level."},
     // Logging methods
     {"debug", (PyCFunction)Logger_debug, METH_VARARGS | METH_KEYWORDS, "Log a message at level DEBUG."},
     {"info", (PyCFunction)Logger_info, METH_VARARGS | METH_KEYWORDS, "Log a message at level INFO."},
     {"warning", (PyCFunction)Logger_warning, METH_VARARGS | METH_KEYWORDS, "Log a message at level WARNING."},
     {"error", (PyCFunction)Logger_error, METH_VARARGS | METH_KEYWORDS, "Log a message at level ERROR."},
     {"critical", (PyCFunction)Logger_critical, METH_VARARGS | METH_KEYWORDS, "Log a message at level CRITICAL."},
     {"exception", (PyCFunction)Logger_exception, METH_VARARGS | METH_KEYWORDS, "Log a message at level ERROR."},
```

### Comparing `picologging-0.9.1/src/picologging/logger.hxx` & `picologging-0.9.2/src/picologging/logger.hxx`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 } Logger ;
 
 int Logger_init(Logger *self, PyObject *args, PyObject *kwds);
 PyObject* Logger_setLevel(Logger *self, PyObject *args);
 PyObject* Logger_getEffectiveLevel(Logger *self);
 PyObject* Logger_dealloc(Logger *self);
 PyObject* Logger_addHandler(Logger *self, PyObject *handler);
+PyObject* Logger_isEnabledFor(Logger *self, PyObject *level);
 
 PyObject* Logger_logAndHandle(Logger *self, PyObject *args, PyObject *kwds, unsigned short level);
 PyObject* Logger_debug(Logger *self, PyObject *args, PyObject *kwds);
 PyObject* Logger_info(Logger *self, PyObject *args, PyObject *kwds);
 PyObject* Logger_warning(Logger *self, PyObject *args, PyObject *kwds);
 PyObject* Logger_fatal(Logger *self, PyObject *args, PyObject *kwds);
 PyObject* Logger_error(Logger *self, PyObject *args, PyObject *kwds);
```

### Comparing `picologging-0.9.1/src/picologging/logrecord.cxx` & `picologging-0.9.2/src/picologging/logrecord.cxx`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/src/picologging/logrecord.hxx` & `picologging-0.9.2/src/picologging/logrecord.hxx`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/src/picologging/streamhandler.cxx` & `picologging-0.9.2/src/picologging/streamhandler.cxx`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         return -1;
     }
     if (stream == NULL || stream == Py_None){
         stream = PySys_GetObject("stderr");
     }
     self->stream = stream;
     Py_INCREF(self->stream);
-    self->stream_has_flush = (PyObject_HasAttrString(self->stream, "flush") == 1);
+    self->stream_has_flush = (PyObject_HasAttr(self->stream, self->_const_flush) == 1);
     return 0;
 }
 
 PyObject* StreamHandler_dealloc(StreamHandler *self) {
     Py_XDECREF(self->stream);
     Py_XDECREF(self->terminator);
     Py_XDECREF(self->_const_write);
```

### Comparing `picologging-0.9.1/src/picologging/streamhandler.hxx` & `picologging-0.9.2/src/picologging/streamhandler.hxx`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/src/picologging.egg-info/PKG-INFO` & `picologging-0.9.2/src/picologging.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,195 +1,192 @@
-Metadata-Version: 2.1
-Name: picologging
-Version: 0.9.1
-Summary: A fast and lightweight logging library for Python
-Home-page: https://github.com/microsoft/picologging
-Author: Microsoft
-License: MIT License
-Project-URL: Source, https://github.com/microsoft/picologging
-Project-URL: Documentation, https://microsoft.github.io/picologging/
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: System :: Logging
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# picologging
-
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/picologging)](https://pypi.org/project/picologging/)
-[![PyPI](https://img.shields.io/pypi/v/picologging)](https://pypi.org/project/picologging/)
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/picologging/badges/version.svg)](https://anaconda.org/conda-forge/picologging)
-[![codecov](https://codecov.io/gh/microsoft/picologging/branch/main/graph/badge.svg?token=KHs6FpQlVW)](https://codecov.io/gh/microsoft/picologging)
-
-> **Warning**
-> This project is in *beta*.
-> There are some incomplete features (see [Limitations](https://microsoft.github.io/picologging/limitations.html)).
-
-Picologging is a high-performance logging library for Python. picologging is 4-10x faster than the `logging` module in the standard library.
-
-Picologging is designed to be used as a *drop-in* replacement for applications which already use logging, and supports the same API as the `logging` module.
-
-Check out the [Documentation](https://microsoft.github.io/picologging/) for more.
-
-## Installation
-
-Picologging can be installed from PyPi using pip:
-
-```console
-pip install picologging
-```
-
-Or from conda forge using conda:
-
-```console
-conda install -c conda-forge picologging
-```
-
-## Usage
-
-Import `picologging as logging` to use picologging instead of the standard library logging module.
-
-This patches all the loggers registered to use picologging loggers and formatters.
-
-```python
-import picologging as logging
-logging.basicConfig()
-
-logger = logging.getLogger()
-
-logger.info("A log message!")
-
-logger.warning("A log message with %s", "arguments")
-```
-
-## Benchmarks
-
-Run `richbench benchmarks/ --markdown` with the richbench CLI to see the benchmarks, here is a sample on macOS 11:
-
-|                             Benchmark | Min     | Max     | Mean    | Min (+)         | Max (+)         | Mean (+)        |
-|---------------------------------------|---------|---------|---------|-----------------|-----------------|-----------------|
-|                         FileHandler() | 0.138   | 0.151   | 0.143   | 0.055 (2.5x)    | 0.063 (2.4x)    | 0.058 (2.5x)    |
-|                  WatchedFileHandler() | 0.189   | 0.197   | 0.193   | 0.097 (1.9x)    | 0.101 (1.9x)    | 0.099 (1.9x)    |
-|                 RotatingFileHandler() | 0.287   | 0.304   | 0.296   | 0.174 (1.6x)    | 0.178 (1.7x)    | 0.176 (1.7x)    |
-|                        QueueHandler() | 1.109   | 1.195   | 1.130   | 0.142 (7.8x)    | 0.151 (7.9x)    | 0.147 (7.7x)    |
-|      QueueListener() + QueueHandler() | 0.157   | 0.167   | 0.162   | 0.034 (4.6x)    | 0.039 (4.3x)    | 0.037 (4.3x)    |
-|                       MemoryHandler() | 0.126   | 0.144   | 0.133   | 0.051 (2.5x)    | 0.059 (2.5x)    | 0.054 (2.5x)    |
-|                           LogRecord() | 0.225   | 0.248   | 0.233   | 0.026 (8.7x)    | 0.029 (8.5x)    | 0.028 (8.4x)    |
-|                  Formatter().format() | 0.076   | 0.086   | 0.081   | 0.004 (18.7x)   | 0.005 (18.9x)   | 0.004 (19.1x)   |
-|        Formatter().format() with date | 0.298   | 0.311   | 0.304   | 0.081 (3.7x)    | 0.087 (3.6x)    | 0.084 (3.6x)    |
-|           Logger(level=DEBUG).debug() | 0.726   | 0.743   | 0.734   | 0.059 (12.3x)   | 0.061 (12.3x)   | 0.060 (12.3x)   |
-| Logger(level=DEBUG).debug() with args | 0.761   | 0.809   | 0.777   | 0.081 (9.4x)    | 0.087 (9.3x)    | 0.084 (9.2x)    |
-|            Logger(level=INFO).debug() | 0.016   | 0.018   | 0.017   | 0.004 (4.3x)    | 0.005 (3.8x)    | 0.004 (4.1x)    |
-|  Logger(level=INFO).debug() with args | 0.018   | 0.019   | 0.018   | 0.005 (3.8x)    | 0.005 (3.8x)    | 0.005 (3.7x)    |
-
-## Limitations
-
-See [Limitations](https://microsoft.github.io/picologging/limitations.html)
-
-## Contributing
-
-This project welcomes contributions and suggestions.  Most contributions require you to agree to a
-Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
-the rights to use your contribution. For details, visit [cla.opensource.microsoft.com](https://cla.opensource.microsoft.com).
-
-When you submit a pull request, a CLA bot will automatically determine whether you need to provide
-a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
-provided by the bot. You will only need to do this once across all repos using our CLA.
-
-This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
-For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
-contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
-
-## Local development
-
-This project comes bundled with a dev container which sets up an appropriate environment. If you install the Dev Containers extension for VS Code, then opening this project in VS Code should prompt it to open it in the dev container.
-
-Once opened in the dev container, run:
-
-```
-pip install -e ".[dev]"
-pre-commit install
-python setup.py build_ext --inplace --build-type Debug
-```
-
-Run the build command whenever you make changes to the files.
-
-It's also helpful to create a `.vscode/launch.json` file like this one:
-
-```
-{
-    "version": "0.2.0",
-    "configurations": [
-    {
-        "name": "(gdb) Launch pytest",
-        "type": "cppdbg",
-        "request": "launch",
-        "program": "/usr/local/bin/python",
-        "args": ["-m", "pytest", "tests"],
-        "stopAtEntry": false,
-        "cwd": "${workspaceFolder}",
-        "environment": [],
-        "externalConsole": false,
-        "MIMode": "gdb",
-        "setupCommands": [
-            {
-                "description": "Enable pretty-printing for gdb",
-                "text": "-enable-pretty-printing",
-                "ignoreFailures": true
-            },
-            {
-                "description":  "Set Disassembly Flavor to Intel",
-                "text": "-gdb-set disassembly-flavor intel",
-                "ignoreFailures": true
-            },
-        ]
-    }
-}
-```
-
-Now you can press the "Run and debug" button to run `pytest` from the `gdb` debugger
-and use breakpoint debugging in the C code.
-
-If you would like to be able to dive into the CPython code while debugging, then:
-
-1. Do a git checkout of the tagged branch for the devcontainer's Python version
-into the devcontainer's `/workspaces/` directory. You may need to `sudo`.
-2. Follow the instructions in the CPython README to compile the code.
-3. Add the following key to the the configuration in `launch.json`:
-    ```
-    "sourceFileMap": { "/usr/src/python": "/workspaces/cpython" },
-    ```
-4. Add the following command to the `setupCommands` in `launch.json`:
-    
-    ```
-    {
-        "description": "Find CPython source code",
-        "text": "-gdb-set auto-load safe-path /workspaces/cpython"
-    },
-    ```
-
-## Trademarks
-
-Some components of this Python package are from CPython 3.11 logging library for compatibility reasons.
-
-CPython 3.11 is licensed under the PSF license.
-The logging module is Copyright (C) 2001-2019 Vinay Sajip. All Rights Reserved.
-
-This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
-trademarks or logos is subject to and must follow 
-[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
-Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
-Any use of third-party trademarks or logos are subject to those third-party's policies.
-
-
+Metadata-Version: 2.1
+Name: picologging
+Version: 0.9.2
+Summary: A fast and lightweight logging library for Python
+Home-page: https://github.com/microsoft/picologging
+Author: Microsoft
+License: MIT License
+Project-URL: Source, https://github.com/microsoft/picologging
+Project-URL: Documentation, https://microsoft.github.io/picologging/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: System :: Logging
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# picologging
+
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/picologging)](https://pypi.org/project/picologging/)
+[![PyPI](https://img.shields.io/pypi/v/picologging)](https://pypi.org/project/picologging/)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/picologging/badges/version.svg)](https://anaconda.org/conda-forge/picologging)
+[![codecov](https://codecov.io/gh/microsoft/picologging/branch/main/graph/badge.svg?token=KHs6FpQlVW)](https://codecov.io/gh/microsoft/picologging)
+
+> **Warning**
+> This project is in *beta*.
+> There are some incomplete features (see [Limitations](https://microsoft.github.io/picologging/limitations.html)).
+
+Picologging is a high-performance logging library for Python. picologging is 4-10x faster than the `logging` module in the standard library.
+
+Picologging is designed to be used as a *drop-in* replacement for applications which already use logging, and supports the same API as the `logging` module.
+
+Check out the [Documentation](https://microsoft.github.io/picologging/) for more.
+
+## Installation
+
+Picologging can be installed from PyPi using pip:
+
+```console
+pip install picologging
+```
+
+Or from conda forge using conda:
+
+```console
+conda install -c conda-forge picologging
+```
+
+## Usage
+
+Import `picologging as logging` to use picologging instead of the standard library logging module.
+
+This patches all the loggers registered to use picologging loggers and formatters.
+
+```python
+import picologging as logging
+logging.basicConfig()
+
+logger = logging.getLogger()
+
+logger.info("A log message!")
+
+logger.warning("A log message with %s", "arguments")
+```
+
+## Benchmarks
+
+Run `richbench benchmarks/ --markdown` with the richbench CLI to see the benchmarks, here is a sample on macOS 11:
+
+|                             Benchmark | Min     | Max     | Mean    | Min (+)         | Max (+)         | Mean (+)        |
+|---------------------------------------|---------|---------|---------|-----------------|-----------------|-----------------|
+|                         FileHandler() | 0.138   | 0.151   | 0.143   | 0.055 (2.5x)    | 0.063 (2.4x)    | 0.058 (2.5x)    |
+|                  WatchedFileHandler() | 0.189   | 0.197   | 0.193   | 0.097 (1.9x)    | 0.101 (1.9x)    | 0.099 (1.9x)    |
+|                 RotatingFileHandler() | 0.287   | 0.304   | 0.296   | 0.174 (1.6x)    | 0.178 (1.7x)    | 0.176 (1.7x)    |
+|                        QueueHandler() | 1.109   | 1.195   | 1.130   | 0.142 (7.8x)    | 0.151 (7.9x)    | 0.147 (7.7x)    |
+|      QueueListener() + QueueHandler() | 0.157   | 0.167   | 0.162   | 0.034 (4.6x)    | 0.039 (4.3x)    | 0.037 (4.3x)    |
+|                       MemoryHandler() | 0.126   | 0.144   | 0.133   | 0.051 (2.5x)    | 0.059 (2.5x)    | 0.054 (2.5x)    |
+|                           LogRecord() | 0.225   | 0.248   | 0.233   | 0.026 (8.7x)    | 0.029 (8.5x)    | 0.028 (8.4x)    |
+|                  Formatter().format() | 0.076   | 0.086   | 0.081   | 0.004 (18.7x)   | 0.005 (18.9x)   | 0.004 (19.1x)   |
+|        Formatter().format() with date | 0.298   | 0.311   | 0.304   | 0.081 (3.7x)    | 0.087 (3.6x)    | 0.084 (3.6x)    |
+|           Logger(level=DEBUG).debug() | 0.726   | 0.743   | 0.734   | 0.059 (12.3x)   | 0.061 (12.3x)   | 0.060 (12.3x)   |
+| Logger(level=DEBUG).debug() with args | 0.761   | 0.809   | 0.777   | 0.081 (9.4x)    | 0.087 (9.3x)    | 0.084 (9.2x)    |
+|            Logger(level=INFO).debug() | 0.016   | 0.018   | 0.017   | 0.004 (4.3x)    | 0.005 (3.8x)    | 0.004 (4.1x)    |
+|  Logger(level=INFO).debug() with args | 0.018   | 0.019   | 0.018   | 0.005 (3.8x)    | 0.005 (3.8x)    | 0.005 (3.7x)    |
+
+## Limitations
+
+See [Limitations](https://microsoft.github.io/picologging/limitations.html)
+
+## Contributing
+
+This project welcomes contributions and suggestions.  Most contributions require you to agree to a
+Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
+the rights to use your contribution. For details, visit [cla.opensource.microsoft.com](https://cla.opensource.microsoft.com).
+
+When you submit a pull request, a CLA bot will automatically determine whether you need to provide
+a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
+provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
+For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
+contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
+
+## Local development
+
+This project comes bundled with a dev container which sets up an appropriate environment. If you install the Dev Containers extension for VS Code, then opening this project in VS Code should prompt it to open it in the dev container.
+
+Once opened in the dev container, run:
+
+```console
+pip install -e ".[dev]"
+pre-commit install
+python setup.py build_ext --inplace --build-type Debug
+```
+
+Run the build command whenever you make changes to the files.
+
+It's also helpful to create a `.vscode/launch.json` file like this one:
+
+```json
+{
+    "version": "0.2.0",
+    "configurations": [
+    {
+        "name": "(gdb) Launch pytest",
+        "type": "cppdbg",
+        "request": "launch",
+        "program": "/usr/local/bin/python",
+        "args": ["-m", "pytest", "tests"],
+        "stopAtEntry": false,
+        "cwd": "${workspaceFolder}",
+        "environment": [],
+        "externalConsole": false,
+        "MIMode": "gdb",
+        "setupCommands": [
+            {
+                "description": "Enable pretty-printing for gdb",
+                "text": "-enable-pretty-printing",
+                "ignoreFailures": true
+            },
+            {
+                "description":  "Set Disassembly Flavor to Intel",
+                "text": "-gdb-set disassembly-flavor intel",
+                "ignoreFailures": true
+            },
+        ]
+    }
+}
+```
+
+Now you can press the "Run and debug" button to run `pytest` from the `gdb` debugger
+and use breakpoint debugging in the C code.
+
+If you would like to be able to dive into the CPython code while debugging, then:
+
+1. Do a git checkout of the tagged branch for the devcontainer's Python version
+into the devcontainer's `/workspaces/` directory. You may need to `sudo`.
+2. Follow the instructions in the CPython README to compile the code.
+3. Add the following key to the the configuration in `launch.json`:
+
+    ```json
+    "sourceFileMap": { "/usr/src/python": "/workspaces/cpython" },
+    ```
+
+4. Add the following command to the `setupCommands` in `launch.json`:
+
+    ```json
+    {
+        "description": "Find CPython source code",
+        "text": "-gdb-set auto-load safe-path /workspaces/cpython"
+    },
+    ```
+
+## Trademarks
+
+Some components of this Python package are from CPython 3.11 logging library for compatibility reasons.
+
+CPython 3.11 is licensed under the PSF license.
+The logging module is Copyright (C) 2001-2019 Vinay Sajip. All Rights Reserved.
+
+This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft trademarks or logos is subject to and must follow [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
+Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
+Any use of third-party trademarks or logos are subject to those third-party's policies.
```

### Comparing `picologging-0.9.1/src/picologging.egg-info/SOURCES.txt` & `picologging-0.9.2/src/picologging.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,21 +11,14 @@
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .github/dependabot.yml
 .github/workflows/pages.yml
 .github/workflows/quality.yml
 .github/workflows/test.yml
 .github/workflows/wheel.yml
-_skbuild/win-amd64-3.9/cmake-install/src/picologging/__init__.py
-_skbuild/win-amd64-3.9/cmake-install/src/picologging/__init__.pyi
-_skbuild/win-amd64-3.9/cmake-install/src/picologging/config.py
-_skbuild/win-amd64-3.9/cmake-install/src/picologging/config.pyi
-_skbuild/win-amd64-3.9/cmake-install/src/picologging/handlers.py
-_skbuild/win-amd64-3.9/cmake-install/src/picologging/handlers.pyi
-_skbuild/win-amd64-3.9/cmake-install/src/picologging/py.typed
 benchmarks/bench_handlers.py
 benchmarks/bench_logger.py
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/conf.py
 docs/source/examples.rst
@@ -64,14 +57,15 @@
 src/picologging.egg-info/top_level.txt
 tests/fuzzing/README.md
 tests/fuzzing/fuzz_atheris.py
 tests/memray/README.md
 tests/memray/memray_format_exception.py
 tests/memray/memray_logger.py
 tests/memray/memray_logrecord.py
+tests/memray/memray_style.py
 tests/profile/profile.py
 tests/unit/test_bufferinghandler.py
 tests/unit/test_config.py
 tests/unit/test_filehandler.py
 tests/unit/test_formatter.py
 tests/unit/test_handler.py
 tests/unit/test_logger.py
```

### Comparing `picologging-0.9.1/tests/fuzzing/README.md` & `picologging-0.9.2/tests/fuzzing/README.md`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/memray/README.md` & `picologging-0.9.2/tests/memray/README.md`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/memray/memray_format_exception.py` & `picologging-0.9.2/tests/memray/memray_format_exception.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/memray/memray_logger.py` & `picologging-0.9.2/tests/memray/memray_logger.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/memray/memray_logrecord.py` & `picologging-0.9.2/tests/memray/memray_logrecord.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/profile/profile.py` & `picologging-0.9.2/tests/profile/profile.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_bufferinghandler.py` & `picologging-0.9.2/tests/unit/test_bufferinghandler.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_config.py` & `picologging-0.9.2/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_filehandler.py` & `picologging-0.9.2/tests/unit/test_filehandler.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_formatter.py` & `picologging-0.9.2/tests/unit/test_formatter.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_handler.py` & `picologging-0.9.2/tests/unit/test_handler.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_logger.py` & `picologging-0.9.2/tests/unit/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,30 @@
 
 def test_set_level():
     logger = picologging.Logger("test")
     logger.setLevel(logging.DEBUG)
     assert logger.level == logging.DEBUG
 
 
+def test_set_level_from_string():
+    logger = picologging.Logger("test")
+    logger.setLevel("DEBUG")
+    assert logger.level == logging.DEBUG
+    logger.setLevel("INFO")
+    assert logger.level == logging.INFO
+    logger.setLevel("WARNING")
+    assert logger.level == logging.WARNING
+    logger.setLevel("ERROR")
+    assert logger.level == logging.ERROR
+    logger.setLevel("CRITICAL")
+    assert logger.level == logging.CRITICAL
+    logger.setLevel("NOTSET")
+    assert logger.level == logging.NOTSET
+
+
 def test_disabled_logger():
     logger = picologging.Logger("test", logging.DEBUG)
     logger.disabled = True
     stream = io.StringIO()
     logger.handlers.append(picologging.StreamHandler(stream))
     assert logger.debug("Hello World") is None
     result = stream.getvalue()
@@ -289,15 +305,21 @@
     logger = picologging.Logger("test", level=100)
     assert repr(logger) == f"<Logger 'test' ()>"
 
 
 def test_set_level_bad_type():
     logger = picologging.Logger("goo", picologging.DEBUG)
     with pytest.raises(TypeError):
-        logger.setLevel("potato")
+        logger.setLevel(3.14)
+
+
+def test_set_level_invalid_name():
+    logger = picologging.Logger("goo", picologging.DEBUG)
+    with pytest.raises(ValueError):
+        logger.setLevel("POTATO")
 
 
 def test_add_remove_handlers():
     logger = picologging.Logger("goo", picologging.DEBUG)
     assert logger.handlers == []
     test_handler = picologging.Handler()
     logger.addHandler(test_handler)
@@ -671,7 +693,19 @@
     bottom1_logger.debug("BLD")
 
     assert stream.getvalue() == "TLW\nTLI\nBL1W\nBL1I\nBL2W\nBL2I\n"
 
     # Now breathe life into the placeholder
     middle_logger = picologging.getLogger("A.B")
     assert middle_logger.getEffectiveLevel() == picologging.INFO
+
+
+def test_is_enabled_for():
+    logger = picologging.Logger("test")
+    logger.setLevel(logging.INFO)
+
+    assert logger.isEnabledFor(logging.INFO) is True
+    assert logger.isEnabledFor(logging.WARNING) is True
+    assert logger.isEnabledFor(logging.DEBUG) is False
+
+    with pytest.raises(TypeError):
+        logger.isEnabledFor("INFO")
```

### Comparing `picologging-0.9.1/tests/unit/test_logrecord.py` & `picologging-0.9.2/tests/unit/test_logrecord.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_percentstyle.py` & `picologging-0.9.2/tests/unit/test_percentstyle.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_picologging.py` & `picologging-0.9.2/tests/unit/test_picologging.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_queuehandler.py` & `picologging-0.9.2/tests/unit/test_queuehandler.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_sockethandler.py` & `picologging-0.9.2/tests/unit/test_sockethandler.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_streamhandler.py` & `picologging-0.9.2/tests/unit/test_streamhandler.py`

 * *Files identical despite different names*

### Comparing `picologging-0.9.1/tests/unit/test_strformatstyle.py` & `picologging-0.9.2/tests/unit/test_strformatstyle.py`

 * *Files identical despite different names*

