# Comparing `tmp/EllipSect-3.2.2.tar.gz` & `tmp/EllipSect-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EllipSect-3.2.2.tar", last modified: Sat May 13 20:12:56 2023, max compression
+gzip compressed data, was "EllipSect-3.2.3.tar", last modified: Tue May 16 22:37:19 2023, max compression
```

## Comparing `EllipSect-3.2.2.tar` & `EllipSect-3.2.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.582309 EllipSect-3.2.2/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      206 2022-05-19 20:23:00.000000 EllipSect-3.2.2/AUTHORS.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1126 2022-08-31 20:39:25.000000 EllipSect-3.2.2/CHANGELOG.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    13841 2022-05-19 05:38:00.000000 EllipSect-3.2.2/CONTRIBUTING.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    35147 2020-07-24 13:17:31.000000 EllipSect-3.2.2/LICENSE.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     6819 2023-05-13 20:12:56.582309 EllipSect-3.2.2/PKG-INFO
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     5874 2023-03-17 05:15:08.000000 EllipSect-3.2.2/README.rst
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.558309 EllipSect-3.2.2/docs/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1154 2022-05-19 05:38:00.000000 EllipSect-3.2.2/docs/Makefile
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.558309 EllipSect-3.2.2/docs/_static/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       18 2022-05-19 05:38:00.000000 EllipSect-3.2.2/docs/_static/.gitignore
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     7461 2022-06-03 20:18:01.000000 EllipSect-3.2.2/docs/api.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       41 2022-05-19 05:38:00.000000 EllipSect-3.2.2/docs/authors.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       43 2022-05-19 05:38:00.000000 EllipSect-3.2.2/docs/changelog.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     9758 2022-05-19 05:38:00.000000 EllipSect-3.2.2/docs/conf.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       33 2022-05-19 05:38:00.000000 EllipSect-3.2.2/docs/contributing.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    17760 2022-09-07 23:14:29.000000 EllipSect-3.2.2/docs/howto.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2321 2022-05-19 05:38:00.000000 EllipSect-3.2.2/docs/index.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       67 2022-05-19 05:38:00.000000 EllipSect-3.2.2/docs/license.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       39 2022-05-19 05:38:00.000000 EllipSect-3.2.2/docs/readme.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      307 2022-05-27 21:03:59.000000 EllipSect-3.2.2/docs/requirements.txt
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.558309 EllipSect-3.2.2/example/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      341 2020-09-18 22:51:02.000000 EllipSect-3.2.2/example/README
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 EllipSect-3.2.2/example/gal.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2646 2020-08-14 03:16:26.000000 EllipSect-3.2.2/example/galfit.feedme
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 EllipSect-3.2.2/example/psf.fits
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.566309 EllipSect-3.2.2/img/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   251092 2021-05-21 15:14:44.000000 EllipSect-3.2.2/img/A2029.ring.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   149798 2021-10-21 21:59:56.000000 EllipSect-3.2.2/img/A85.comp.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   573061 2022-03-30 17:48:47.000000 EllipSect-3.2.2/img/A85.con-cub.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   670362 2022-03-30 17:49:48.000000 EllipSect-3.2.2/img/A85.cub.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    98164 2021-10-21 22:00:51.000000 EllipSect-3.2.2/img/A85.def.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   610346 2022-03-30 17:44:31.000000 EllipSect-3.2.2/img/A85.ell-cub.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   503397 2021-10-21 22:01:09.000000 EllipSect-3.2.2/img/A85.grid.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    95479 2021-10-21 22:01:39.000000 EllipSect-3.2.2/img/A85.log.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   102981 2021-10-21 22:02:04.000000 EllipSect-3.2.2/img/A85.pix.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   327227 2020-08-14 03:16:26.000000 EllipSect-3.2.2/img/A85.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    95328 2021-10-21 22:02:35.000000 EllipSect-3.2.2/img/A85.ranx1.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    89311 2021-10-21 22:03:30.000000 EllipSect-3.2.2/img/A85.ranx2.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    91257 2021-10-21 22:04:08.000000 EllipSect-3.2.2/img/A85.rany1.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      355 2022-05-19 05:38:00.000000 EllipSect-3.2.2/pyproject.toml
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1760 2023-05-13 20:12:56.582309 EllipSect-3.2.2/setup.cfg
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      706 2022-05-19 05:38:00.000000 EllipSect-3.2.2/setup.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.550309 EllipSect-3.2.2/src/
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.570309 EllipSect-3.2.2/src/EllipSect.egg-info/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     6819 2023-05-13 20:12:56.000000 EllipSect-3.2.2/src/EllipSect.egg-info/PKG-INFO
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1610 2023-05-13 20:12:56.000000 EllipSect-3.2.2/src/EllipSect.egg-info/SOURCES.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2023-05-13 20:12:56.000000 EllipSect-3.2.2/src/EllipSect.egg-info/dependency_links.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       57 2023-05-13 20:12:56.000000 EllipSect-3.2.2/src/EllipSect.egg-info/entry_points.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2022-05-23 00:05:26.000000 EllipSect-3.2.2/src/EllipSect.egg-info/not-zip-safe
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      146 2023-05-13 20:12:56.000000 EllipSect-3.2.2/src/EllipSect.egg-info/requires.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       10 2023-05-13 20:12:56.000000 EllipSect-3.2.2/src/EllipSect.egg-info/top_level.txt
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.570309 EllipSect-3.2.2/src/ellipsect/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      675 2022-05-29 17:51:45.000000 EllipSect-3.2.2/src/ellipsect/__init__.py
--rwxrwxr-x   0 canorve   (1000) canorve   (1000)     2080 2023-02-08 06:36:48.000000 EllipSect-3.2.2/src/ellipsect/ellipsectors.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.574309 EllipSect-3.2.2/src/ellipsect/inout/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:19.000000 EllipSect-3.2.2/src/ellipsect/inout/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    22988 2023-03-14 00:31:50.000000 EllipSect-3.2.2/src/ellipsect/inout/galfit.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     3380 2023-02-10 20:37:56.000000 EllipSect-3.2.2/src/ellipsect/inout/gfits.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    23250 2023-05-13 17:48:01.000000 EllipSect-3.2.2/src/ellipsect/inout/plots.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    20007 2023-04-19 15:30:49.000000 EllipSect-3.2.2/src/ellipsect/inout/prt.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    20009 2023-05-12 21:16:51.000000 EllipSect-3.2.2/src/ellipsect/inout/read.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.574309 EllipSect-3.2.2/src/ellipsect/lib/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 06:03:15.000000 EllipSect-3.2.2/src/ellipsect/lib/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     7905 2023-02-19 04:21:12.000000 EllipSect-3.2.2/src/ellipsect/lib/clas.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1506 2023-03-14 03:32:46.000000 EllipSect-3.2.2/src/ellipsect/lib/libs.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.578309 EllipSect-3.2.2/src/ellipsect/phot/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:10:40.000000 EllipSect-3.2.2/src/ellipsect/phot/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     5474 2023-02-09 23:00:09.000000 EllipSect-3.2.2/src/ellipsect/phot/ned.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    15252 2023-03-14 00:35:39.000000 EllipSect-3.2.2/src/ellipsect/phot/phot.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    12271 2023-05-11 07:29:38.000000 EllipSect-3.2.2/src/ellipsect/phot/tidal.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.578309 EllipSect-3.2.2/src/ellipsect/sectors/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:40.000000 EllipSect-3.2.2/src/ellipsect/sectors/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     3065 2023-02-09 23:00:21.000000 EllipSect-3.2.2/src/ellipsect/sectors/comp.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     6814 2023-02-09 23:00:25.000000 EllipSect-3.2.2/src/ellipsect/sectors/ellip.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2981 2023-02-09 23:00:28.000000 EllipSect-3.2.2/src/ellipsect/sectors/num.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    19192 2023-05-12 00:52:31.000000 EllipSect-3.2.2/src/ellipsect/sectors/sect.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.578309 EllipSect-3.2.2/src/ellipsect/sky/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 07:02:06.000000 EllipSect-3.2.2/src/ellipsect/sky/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    24185 2023-02-09 23:00:47.000000 EllipSect-3.2.2/src/ellipsect/sky/sky.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-13 20:12:56.582309 EllipSect-3.2.2/tests/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      277 2022-05-19 05:38:00.000000 EllipSect-3.2.2/tests/conftest.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 EllipSect-3.2.2/tests/gal.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2879 2022-05-27 20:24:55.000000 EllipSect-3.2.2/tests/galfit.01
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   192960 2023-05-13 20:11:02.000000 EllipSect-3.2.2/tests/imgblock.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 EllipSect-3.2.2/tests/psf.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    14837 2023-05-13 17:24:07.000000 EllipSect-3.2.2/tests/test_ellipsect.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2575 2022-05-19 05:38:00.000000 EllipSect-3.2.2/tox.ini
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.282305 EllipSect-3.2.3/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      206 2022-05-19 20:23:00.000000 EllipSect-3.2.3/AUTHORS.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1126 2022-08-31 20:39:25.000000 EllipSect-3.2.3/CHANGELOG.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    13841 2022-05-19 05:38:00.000000 EllipSect-3.2.3/CONTRIBUTING.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    35147 2020-07-24 13:17:31.000000 EllipSect-3.2.3/LICENSE.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     6819 2023-05-16 22:37:19.282305 EllipSect-3.2.3/PKG-INFO
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     5874 2023-03-17 05:15:08.000000 EllipSect-3.2.3/README.rst
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.266304 EllipSect-3.2.3/docs/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1154 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/Makefile
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.266304 EllipSect-3.2.3/docs/_static/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       18 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/_static/.gitignore
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     7461 2022-06-03 20:18:01.000000 EllipSect-3.2.3/docs/api.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       41 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/authors.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       43 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/changelog.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     9758 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/conf.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       33 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/contributing.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    17760 2022-09-07 23:14:29.000000 EllipSect-3.2.3/docs/howto.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2321 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/index.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       67 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/license.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       39 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/readme.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      307 2022-05-27 21:03:59.000000 EllipSect-3.2.3/docs/requirements.txt
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.266304 EllipSect-3.2.3/example/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      341 2020-09-18 22:51:02.000000 EllipSect-3.2.3/example/README
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 EllipSect-3.2.3/example/gal.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2646 2020-08-14 03:16:26.000000 EllipSect-3.2.3/example/galfit.feedme
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 EllipSect-3.2.3/example/psf.fits
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.274304 EllipSect-3.2.3/img/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   251092 2021-05-21 15:14:44.000000 EllipSect-3.2.3/img/A2029.ring.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   149798 2021-10-21 21:59:56.000000 EllipSect-3.2.3/img/A85.comp.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   573061 2022-03-30 17:48:47.000000 EllipSect-3.2.3/img/A85.con-cub.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   670362 2022-03-30 17:49:48.000000 EllipSect-3.2.3/img/A85.cub.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    98164 2021-10-21 22:00:51.000000 EllipSect-3.2.3/img/A85.def.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   610346 2022-03-30 17:44:31.000000 EllipSect-3.2.3/img/A85.ell-cub.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   503397 2021-10-21 22:01:09.000000 EllipSect-3.2.3/img/A85.grid.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    95479 2021-10-21 22:01:39.000000 EllipSect-3.2.3/img/A85.log.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   102981 2021-10-21 22:02:04.000000 EllipSect-3.2.3/img/A85.pix.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   327227 2020-08-14 03:16:26.000000 EllipSect-3.2.3/img/A85.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    95328 2021-10-21 22:02:35.000000 EllipSect-3.2.3/img/A85.ranx1.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    89311 2021-10-21 22:03:30.000000 EllipSect-3.2.3/img/A85.ranx2.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    91257 2021-10-21 22:04:08.000000 EllipSect-3.2.3/img/A85.rany1.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      355 2022-05-19 05:38:00.000000 EllipSect-3.2.3/pyproject.toml
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1760 2023-05-16 22:37:19.282305 EllipSect-3.2.3/setup.cfg
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      706 2022-05-19 05:38:00.000000 EllipSect-3.2.3/setup.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.262304 EllipSect-3.2.3/src/
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.274304 EllipSect-3.2.3/src/EllipSect.egg-info/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     6819 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/PKG-INFO
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1610 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/SOURCES.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/dependency_links.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       57 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/entry_points.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2022-05-23 00:05:26.000000 EllipSect-3.2.3/src/EllipSect.egg-info/not-zip-safe
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      146 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/requires.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       10 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/top_level.txt
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.274304 EllipSect-3.2.3/src/ellipsect/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      675 2022-05-29 17:51:45.000000 EllipSect-3.2.3/src/ellipsect/__init__.py
+-rwxrwxr-x   0 canorve   (1000) canorve   (1000)     2080 2023-02-08 06:36:48.000000 EllipSect-3.2.3/src/ellipsect/ellipsectors.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/src/ellipsect/inout/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:19.000000 EllipSect-3.2.3/src/ellipsect/inout/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    22988 2023-03-14 00:31:50.000000 EllipSect-3.2.3/src/ellipsect/inout/galfit.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     3380 2023-02-10 20:37:56.000000 EllipSect-3.2.3/src/ellipsect/inout/gfits.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    23292 2023-05-16 19:51:58.000000 EllipSect-3.2.3/src/ellipsect/inout/plots.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    20007 2023-04-19 15:30:49.000000 EllipSect-3.2.3/src/ellipsect/inout/prt.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    20009 2023-05-12 21:16:51.000000 EllipSect-3.2.3/src/ellipsect/inout/read.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/src/ellipsect/lib/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 06:03:15.000000 EllipSect-3.2.3/src/ellipsect/lib/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     7905 2023-02-19 04:21:12.000000 EllipSect-3.2.3/src/ellipsect/lib/clas.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1506 2023-03-14 03:32:46.000000 EllipSect-3.2.3/src/ellipsect/lib/libs.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/src/ellipsect/phot/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:10:40.000000 EllipSect-3.2.3/src/ellipsect/phot/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     5474 2023-02-09 23:00:09.000000 EllipSect-3.2.3/src/ellipsect/phot/ned.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    15252 2023-03-14 00:35:39.000000 EllipSect-3.2.3/src/ellipsect/phot/phot.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    12271 2023-05-11 07:29:38.000000 EllipSect-3.2.3/src/ellipsect/phot/tidal.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/src/ellipsect/sectors/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:40.000000 EllipSect-3.2.3/src/ellipsect/sectors/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     3065 2023-02-09 23:00:21.000000 EllipSect-3.2.3/src/ellipsect/sectors/comp.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     6814 2023-02-09 23:00:25.000000 EllipSect-3.2.3/src/ellipsect/sectors/ellip.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2981 2023-02-09 23:00:28.000000 EllipSect-3.2.3/src/ellipsect/sectors/num.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    19192 2023-05-12 00:52:31.000000 EllipSect-3.2.3/src/ellipsect/sectors/sect.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/src/ellipsect/sky/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 07:02:06.000000 EllipSect-3.2.3/src/ellipsect/sky/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    24185 2023-02-09 23:00:47.000000 EllipSect-3.2.3/src/ellipsect/sky/sky.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/tests/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      277 2022-05-19 05:38:00.000000 EllipSect-3.2.3/tests/conftest.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 EllipSect-3.2.3/tests/gal.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2879 2022-05-27 20:24:55.000000 EllipSect-3.2.3/tests/galfit.01
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   192960 2023-05-16 22:34:54.000000 EllipSect-3.2.3/tests/imgblock.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 EllipSect-3.2.3/tests/psf.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    14837 2023-05-13 17:24:07.000000 EllipSect-3.2.3/tests/test_ellipsect.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2575 2022-05-19 05:38:00.000000 EllipSect-3.2.3/tox.ini
```

### Comparing `EllipSect-3.2.2/CHANGELOG.rst` & `EllipSect-3.2.3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/CONTRIBUTING.rst` & `EllipSect-3.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/LICENSE.txt` & `EllipSect-3.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/PKG-INFO` & `EllipSect-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EllipSect
-Version: 3.2.2
+Version: 3.2.3
 Summary: A surface brightness analysis tool for GALFIT output.
 Home-page: https://github.com/canorve/EllipSect
 Author: Christopher Añorve
 Author-email: canorve@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://github.com/canorve/EllipSect/blob/master/README.rst
 Project-URL: Source, https://github.com/canorve/EllipSect
```

### Comparing `EllipSect-3.2.2/README.rst` & `EllipSect-3.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/docs/Makefile` & `EllipSect-3.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/docs/api.rst` & `EllipSect-3.2.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/docs/conf.py` & `EllipSect-3.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/docs/howto.rst` & `EllipSect-3.2.3/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/docs/index.rst` & `EllipSect-3.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/example/gal.fits` & `EllipSect-3.2.3/example/gal.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/example/galfit.feedme` & `EllipSect-3.2.3/example/galfit.feedme`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/example/psf.fits` & `EllipSect-3.2.3/example/psf.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A2029.ring.png` & `EllipSect-3.2.3/img/A2029.ring.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.comp.png` & `EllipSect-3.2.3/img/A85.comp.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.con-cub.png` & `EllipSect-3.2.3/img/A85.con-cub.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.cub.png` & `EllipSect-3.2.3/img/A85.cub.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.def.png` & `EllipSect-3.2.3/img/A85.def.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.ell-cub.png` & `EllipSect-3.2.3/img/A85.ell-cub.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.grid.png` & `EllipSect-3.2.3/img/A85.grid.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.log.png` & `EllipSect-3.2.3/img/A85.log.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.pix.png` & `EllipSect-3.2.3/img/A85.pix.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.png` & `EllipSect-3.2.3/img/A85.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.ranx1.png` & `EllipSect-3.2.3/img/A85.ranx1.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.ranx2.png` & `EllipSect-3.2.3/img/A85.ranx2.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/img/A85.rany1.png` & `EllipSect-3.2.3/img/A85.rany1.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/setup.cfg` & `EllipSect-3.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/setup.py` & `EllipSect-3.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/EllipSect.egg-info/PKG-INFO` & `EllipSect-3.2.3/src/EllipSect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EllipSect
-Version: 3.2.2
+Version: 3.2.3
 Summary: A surface brightness analysis tool for GALFIT output.
 Home-page: https://github.com/canorve/EllipSect
 Author: Christopher Añorve
 Author-email: canorve@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://github.com/canorve/EllipSect/blob/master/README.rst
 Project-URL: Source, https://github.com/canorve/EllipSect
```

### Comparing `EllipSect-3.2.2/src/EllipSect.egg-info/SOURCES.txt` & `EllipSect-3.2.3/src/EllipSect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/__init__.py` & `EllipSect-3.2.3/src/ellipsect/__init__.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/ellipsectors.py` & `EllipSect-3.2.3/src/ellipsect/ellipsectors.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/inout/galfit.py` & `EllipSect-3.2.3/src/ellipsect/inout/galfit.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/inout/gfits.py` & `EllipSect-3.2.3/src/ellipsect/inout/gfits.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/inout/plots.py` & `EllipSect-3.2.3/src/ellipsect/inout/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     xran = minrad * (maxrad/minrad)**np.array([-0.02, +1.02])
     yran = mincnt * (maxcnt/mincnt)**np.array([+1.05, -0.05]) #inverted axis
 
    
     # ULISES begin
     axsec = plt.subplot(gs[0])
 
-    axsec.set_ylabel("Surface Brightness (mag/'')")
+    axsec.set_ylabel(r"Surface Brightness $(mag\; arcsec^{-2})$")
     # ULISES end
 
     axsec.errorbar(xradq, ysbq,yerr=ysberrq,fmt='o-',capsize=2,color='red',markersize=0.7,label="galaxy",linewidth=2)
 
 
     if ellconf.flagalax == False:
         axsec.errorbar(xradm, ysbm,yerr=ysberrm,fmt='o-',capsize=2,color='blue',markersize=0.7,label="Model",linewidth=2)
@@ -132,15 +132,15 @@
 
     if len(xradq) != len(residual):
         axred.errorbar(xradm, residual, yerr=err,fmt='.',capsize=2,color='k')
     else:
         axred.errorbar(xradq, residual, yerr=err,fmt='.',capsize=2,color='k')
 
     axred.axhline(y=0,ls='dashed', color='k')
-    axred.set_xlabel('Radius (arcsec)')
+    axred.set_xlabel('Radius $(arcsec)$')
     axred.set_ylabel('Residual (%)')
     axred.set_ylim(-2,2)
     # ULISES end
 
 
     if ellconf.flaglogx == True:
 
@@ -369,15 +369,14 @@
 
 
 
         mask=data < 0 
         data[mask] = 1 # avoids problems in log
      
         fig, (ax1, ax2, ax3) = plt.subplots(figsize=(14, 5), nrows = 1, ncols = 3)
-        fig.subplots_adjust(left=0.04, right=0.98, bottom=0.02, top=0.98)
 
         im = ax1.imshow(newdata, origin ='lower', interpolation='nearest', norm 
                     = colors.LogNorm(vmin=modmin, vmax=modmax), cmap = cmap)
 
 
         ax1.set_title('Data')
 
@@ -418,14 +417,15 @@
 
         ax2.set_title('GALFIT Model')
 
         ax3.imshow(residual, origin='lower', vmin = resmin, vmax = resmax, cmap = cmap)
         ax3.set_title('Residual')
 
 
+        fig.subplots_adjust(left=0.04, right=0.98, bottom=0.02, top=0.98)
         plt.savefig(namepng, dpi = dpival)
     
 
         #plt.show()
 
 
 def PlotMul(ellconf, galhead, galcomps, mgegal, mgemod, mgecom):
@@ -463,19 +463,19 @@
     fig.subplots_adjust(hspace=0.01)
 
 
     if ellconf.flagpix:
         axpix = axsec[0,0].twiny()
         axpix2 = axsec[0,1].twiny()
 
-    fig.text(0.04, 0.5, "Surface Brightness (mag/'')", va='center', rotation='vertical')
+    fig.text(0.04, 0.5, r"Surface Brightness $(mag\; arcsec^{-2})$", va='center', rotation='vertical')
     fig.text(0.96, 0.5, 'error ', va='center', rotation='vertical')
 
-    axsec[-1, 0].set_xlabel("radius ('')")
-    axsec[-1, 1].set_xlabel("radius ('')")
+    axsec[-1, 0].set_xlabel("radius $(arcsec)$")
+    axsec[-1, 1].set_xlabel("radius $(arcsec)$")
 
     if ellconf.flaglogx == True:
         axsec[-1, 0].xaxis.set_major_locator(LogLocator(base=10.0, numticks=15))
         if ellconf.flagpix:
             axpix.set_xscale("log")
             axpix2.set_xscale("log")
```

### Comparing `EllipSect-3.2.2/src/ellipsect/inout/prt.py` & `EllipSect-3.2.3/src/ellipsect/inout/prt.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/inout/read.py` & `EllipSect-3.2.3/src/ellipsect/inout/read.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/lib/clas.py` & `EllipSect-3.2.3/src/ellipsect/lib/clas.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/lib/libs.py` & `EllipSect-3.2.3/src/ellipsect/lib/libs.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/phot/ned.py` & `EllipSect-3.2.3/src/ellipsect/phot/ned.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/phot/phot.py` & `EllipSect-3.2.3/src/ellipsect/phot/phot.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/phot/tidal.py` & `EllipSect-3.2.3/src/ellipsect/phot/tidal.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/sectors/comp.py` & `EllipSect-3.2.3/src/ellipsect/sectors/comp.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/sectors/ellip.py` & `EllipSect-3.2.3/src/ellipsect/sectors/ellip.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/sectors/num.py` & `EllipSect-3.2.3/src/ellipsect/sectors/num.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/sectors/sect.py` & `EllipSect-3.2.3/src/ellipsect/sectors/sect.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/src/ellipsect/sky/sky.py` & `EllipSect-3.2.3/src/ellipsect/sky/sky.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/tests/gal.fits` & `EllipSect-3.2.3/tests/gal.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/tests/galfit.01` & `EllipSect-3.2.3/tests/galfit.01`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/tests/imgblock.fits` & `EllipSect-3.2.3/tests/imgblock.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/tests/psf.fits` & `EllipSect-3.2.3/tests/psf.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/tests/test_ellipsect.py` & `EllipSect-3.2.3/tests/test_ellipsect.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.2/tox.ini` & `EllipSect-3.2.3/tox.ini`

 * *Files identical despite different names*

